# PowerView® API

To connect a PowerView® system to a home automation system a PowerView® Hub is required.

There are two API's available:

1. HTTP REST API. (data transferred in JSON format)
2. API using a serial connection.

Currently the API is limited to commands for *getting* a list of scenes and commands to *activate* scenes.
These scenes need to be created in the PowerView® app first.
When receiving a list of scenes from the hub the scene names are base64 encoded. they needed to be programmatically converted to unicode utf-8 readable text. See [here](#base64_encoding) for code examples.

## PowerView® http API.
Make sure your hub gets a reserved/fixed ip address from the dhcp server.

### Get a list of all available scenes.
#### request.
```
method: GET
api/scenes/
```
####response example
```javascript
{
  "sceneIds":[7214,64073,15890,42747],
  "sceneData":[
    {
      "id":7214,
      "name":"QWxsIGRvd24=", //base64 encoded.
      "roomId":64902,
      "order":0,
      "colorId":2,
      "iconId":0
    },
    {
      "id":64073,
      "name":"UGxpc3NlIDE=", //base64 encoded.
      "roomId":64902,
      "order":1,
      "colorId":5,
      "iconId":0
    },
    {
      "id":15890,
      "name":"QWxsIHVw", //base64 encoded.
      "roomId":64902,
      "order":2,
      "colorId":0,
      "iconId":0
    },
    {
      "id":42747,
      "name":"UGxpc3NlIDI=", //base64 encoded.
      "roomId":64902,
      "order":3,
      "colorId":7,
      "iconId":0
    }
  ]
}
```

### Activate a scene
#### request.
```
method: GET
/api/scenes?sceneid=<sceneid>  //replace <sceneid> with actual scene id.
```
#### response example
```javascript
{
  "scene":{"shadeIds":[35523]}
}
```
---
## PowerView® Serial API
You will need a separate Serial connection cable for a serial connection to the Hub (sold separately).

![serial cable](/imgs/serial_connection.png)

Pin | Signal | Direction     | Description
--- | ------ | ---------     | ------
2   | RDX    | to computer   | Receive data
3   | TDX    | from computer  | Transmit data
5   | GND    | .             | Ground

- COM port settings: speed: 9600, stop bit: 1, Parity: None.
- Each request to the Hub begins with a `?` followed by a two-character ASCII command.  Each successful response from the Hub begins with a `!` followed by the same two ASCII characters.
- All messages are terminated with a carriage return `x0D`. In this document a carriage return is designated as `<cr>`
- Scene and Room identifiers are transmitted as an ASCII string representing an integer value ranging from zero (0) to 65535.
- Names of Scenes and Rooms are always located as the last parameter of a response and may include spaces.

---
### Request scene count
To retrieve the list of Scenes that have been configured and stored in the PowerView® Hub, a request is first sent to the Hub requesting the total number of Scenes stored
#### serial command
```javascript
?SC <cr>
```
#### Hub response
```javascript
!SC <count> //the number of scenes programmed in the hub.
```

### Request a Scene Object.
Specific information about each individual Scene may be retrieved by sending a series of requests to the Hub.  Each request includes an index within a range from one (1) to the total scene count.
#### serial command.
```javascript
?SO <index> <cr>
```
#### Hub response
```javascript
!SO <index> <scene ID> <room ID> <name>
```

### Request list of scene objects
Specific information about all Scenes may be retrieved by sending a single request to the Hub.
#### serial command
```javascript
?SL <cr>
```
#### Hub response
```javascript
!SL
<scene1 ID> <roomX ID> <name1>
<scene2 ID> <roomY ID> <name2>
<scene3 ID> <roomZ ID> <name3>
...
```

### Execute one or more scenes
A list from one (1) to 28 Scenes may be executed using a single command.
#### serial command

```javascript
?SE <scene ID 1> <scene ID 2> ...<scene ID 28> <cr>
```

#### Hub response
```javascript
!SE
```

---
## Base64 encoding

### Python

```python
import base64

def decode_base64(str):
    """
    Converts base64 to unicode text

    """
    return base64.b64decode(str).decode('utf-8')

```
### javascript

```javascript
function decode_base64(str){
  // Converts incoming base64 to unicode text.
  return new Buffer(str, 'base64').toString('binary');
}
```
