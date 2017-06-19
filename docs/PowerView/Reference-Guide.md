# PowerView® reference guide

## Installing a hub

{!hub_installation.md!}

## Resetting a repeater

%6 Locate the following button on your repeater: %6 ![Repeater](/imgs/repeater_button.png)
%1 1. %6 Press the `repeater button` for approx **6 seconds** until the green light starts to light up. Your repeater is now reset.

## Add a repeater using the Remote.
Installation of a repeater is necessary when your shade isn't responding to a command from your remote control. 
<div class="alert alert-danger">
IMPORTANT: Put the repeater at a strategic location. Preferably halfway between the unresponsive shade and the remote control location. Look [here](#repeater_location)] for more info.
</div>
%6 This instruction will make use of the following buttons on the Remote: %6 ![Adding a remote](/imgs/remote_stop_only.svg)
%6 Find the following button/light on the repeater. %6 ![Repeater](/imgs/repeater.svg)

%1 5.1 %5 **Assemble the repeater kit and plug it in an outlet** <br/>_(The `repeater light` illuminates green  )_ %6 ![repeater outlet](/imgs/repeater-outlet.png)
%1 5.2 %6 **Press &icon-pv-stop; ```stop``` for 6 seconds.** <br/>_(Keep pressing until the remote lights start blinking.)_
%1 5.3 %6 **Hold the remote within 20cm. from the repeater.**
%1 5.4 %6 **Press &icon-pv-stop; ```stop``` .** <br/>_(The `repeater light` will turn off. The repeater is now part of your personal PowerView® Network.)_


## Add a repeater using the App.

%1 1. %11 Make sure your repeater is [reset](#resetting_a_repeater)
%1 2. %11 Open the app. Select blinds and `discover shades`.
%1 3. %11 The repeater light should start blinking and finally end with the led switched off.

## Repeater location.
The range of any indoor wireless device is always difficult to determine. Factors like used building materials and presence of other wireless devices can have a big (negative) impact on wireless range.
To improve the range of the PowerView® network repeaters can be used.

> A repeater picks up any incoming wireless **PowerView®** signal and transmits it again at full power increasing the range of the signal being sent.

In practice finding the ideal location of a repeater is a bit of trial and error. But the below rules of thumb can be a good help:

![repeater setup](/imgs/repeater-setup.png)

- Preferably don't use more than 6 repeaters.
- Ideally locate your repeater halfway between your hub/remote and the blind.
- The repeater should be in range of both hub/remote and blind. If required place a second repeater. Look [here](#check_whether_a_repeater_is_part_of_the_powerviewtm_network) to check whether a repeater is part of the PowerView® network and picking up a signal. 
- There should be just enough overlap (see yellow parts in the image) in range between hub/remote and repeater:
    - Too much overlap will make the signals of hub, remote and repeater interfere and range extension is not optimal.
    - Too little or no overlap means the signal is not being received by the repeater.

> In the image above the red blind is receiving a hub signal being repeated by the first repeater. The green blind is receiving a hub signal being repeated by the second repeater, which was being repeated by the first repeater.

## Check whether a repeater is part of the PowerView® network.
%6 Locate the following button on your repeater: %6 ![Repeater](/imgs/repeater_button.png)
%1 1. %6 Make sure you have a working remote. 
%1 2. %6 Control a blind by selecting a group and sending an open or close command. <br/> _See also [here](#moving_a_blind)_
%1 3. %6 The repeater button/light should start blinking.

## Pairing and Duplicating a remote
Out of the box each remote creates its own PowerView® network. In most cases however your remotes need to be on the same "network". [Pairing remotes](#pairing_a_remote) will be necessary. Consider the following scenario:

> Out of the box you have _two_ remotes. As soon as you [add](#adding_a_blind_to_a_group) your shade to `remote 1` they belong to the same PowerView® network and you can now control your blind with `remote 1`. As soon as you [add](#adding_a_blind_to_a_group) your blind to `remote 2` your shade moves to the network of `remote 2`. You can control the shade with `remote 2`, but not anymore with `remote 1`. [Pairing remotes](#pairing_a_remote) first would have solved this issue. Both remotes are part of the same PowerView® network. Both `remote 1` and `remote 2` would have functioned.

[Duplicating a remote](#duplicating_a_remote) not only pairs the remotes to the same network, it also copies all group information from your source / old remote to the new remote. A duplicate remote will function exactly in the same way as your source remote.

## Pairing a remote
Take two remotes. Name them `original`, `target` and follow the instructions below.
%7 Locate the following buttons on your remote: %5 ![Remote stop](/imgs/pv_white_remote_stop.svg)
### Procedure
%1 1. %6 `target` **Remove** the back cover. <br/>_(keep the batteries in place)_ %5 ![remove cover](/imgs/3-remotes-remove-cover.png)
%1 2. %6 `target:` **Press** the reset button for **six seconds**. <br/>_(The group buttons will flash on the press of the Reset button, then again at 6 seconds)_ %5 ![reset](/imgs/3-remotes-reset-with-pen.png)
%1 3. %6 `target:` **Close** the back cover.
%1 4. %6 `original:` **Press** the &icon-pv-stop;```stop``` button for **6 seconds**. <br/>_(Keep pressing until the remote lights start blinking)_
%1 5. %6 `target:` **Press and hold** the &icon-pv-stop;```stop``` button.
%1 6. %6 `original:` **Press and release** the &icon-pv-stop;```stop``` button.<br/>_(As confirmation `target` will flash the group buttons)_
%1 7. %6 `target:` **Release** the &icon-pv-stop;```stop``` button.
%1 8. %6 If `original` is still flashing **Press and hold** the &icon-pv-stop;```stop``` button for **6 seconds**. <br/>_(Keep pressing until the flashing stops)_

## Duplicating a remote
Take two remotes. Name them `original`, `target` and follow the instructions below.
%7 Locate the following buttons on both remotes: %5 ![Remote stop-all](/imgs/pv_white_remote_stop_all.svg)
### Procedure
%1 1. %6 `target:` **Remove** the back cover. <br/>_(keep batteries in place)_ %5 ![remove cover](/imgs/3-remotes-remove-cover.png)
%1 2. %6 `target:` **Press** the reset button for **6 seconds**. <br/>_(The group buttons will flash on the press of the Reset button, then again at 6 seconds)_ %5 ![reset](/imgs/3-remotes-reset-with-pen.png)
%1 3. %6 `target:` **Close** the back cover.
%1 4. %6 `original:` **Press and hold** the &icon-pv-stop;`stop` for 6 seconds. <br/>_(Keep pressing until the remote lights start blinking)_
%1 5. %6 `target:` **Press and hold** the `all` button.
%1 6. %6 `original:` **Press and release** the &icon-pv-stop;`stop` button. <br/>_(The Group numbers on the target remote will flash 2x)_
%1 7. %6 `target:` **Release** the `all` button.
%1 8. %6 If the `original` is still flashing **Press and hold** the &icon-pv-stop;`stop` button for **6 seconds**. <br/>_(Keep pressing until the flashing stops)_

## Pairing a remote to an existing Hub network
You have created a PowerView® network with shades and a hub and now want to add a remote. Another scenario could be you want to add a newly purchased remote to the network.

%7 **Locate** the `P` button on the back of the hub: %5 ![Locate P button](/imgs/pv_hub_back_p.svg)
%7 **Locate** the the &icon-pv-stop;```stop``` button on the remote you want to pair. %5 ![Remote stop](/imgs/pv_white_remote_stop.svg)
### Procedure
%1 1. %6 `Remote 2:` **Remove** the back cover. <br/>_(keep the batteries in place)_ %5 ![remove cover](/imgs/3-remotes-remove-cover.png)
%1 2. %6 `Remote 2:` **Press** the reset button for **6 seconds**. <br/>_(The group buttons will flash on the press of the Reset button, then again at 6 seconds)_ %5 ![reset](/imgs/3-remotes-reset-with-pen.png)
%1 3. %6 `Remote 2:` **Close** the back cover.
%1 4. %6 **Press and hold** the `P` button.
%1 5. %6 **Press and hold** the &icon-pv-stop;`stop` button.
%1 7. %9 **Release** both `P` and `stop` buttons. <br/>_(The group buttons will flash as confirmation.)_
%1 8. %9 If remote is still flashing **Press and hold** the &icon-pv-stop;`stop` for **6 seconds**. <br/>_(Keep pressing until the flashing stops)_

## Adding a shade to a group
A remote can control 6 individual groups of shades. To control a shade with the remote it needs to be added to one of those groups.
%7 **Locate** these buttons on your remote: %5 ![Remote group1-open-stop](/imgs/pv_white_remote_add_channel_1.svg)
Locate the `manual control button` on your shade. Different shade types have different types of buttons. Below some examples. Consult the shade documentation for the exact location of the `manual control button`.
%4 ![Duette button](/imgs/duette.png) <br/> <p style="text-align: center;">_Duette® shade_</p> %4 ![Pirouette button](/imgs/pirouette.png) <br/> <p style="text-align: center;">_Pirouette® shade_</p> %4 ![Rollerblind button](/imgs/m25t_rollerblind_detail.png) <br/> <p style="text-align: center;">_Rollerblind_</p>
Follow the instructions below for each PowerView® window shading. Depending on your preferences choose a group on one of your remotes. In this case, group &icon-pv-one;```group 1``` is used.
%1 1. %6 **Press and hold** the &icon-pv-stop;`stop` button for **6 seconds**. <br/>_(Keep pressing until the remote lights start blinking)_
%1 2. %6 **Press** the &icon-pv-one;`group 1` button. <br/>_(This will activate group 1 on the remote)_
%1 3. %6 **Press and hold** the `manual control button`.                                         
%1 4. %6 **Press** the &icon-pv-open;`open` button. <br/>_(You will see the blind jog 1x)_
%1 5. %6 **Release** the `manual control button`.
%1 6. %6 If your remote is still flashing **Press and hold** the &icon-pv-stop;`stop` button for **6 seconds**. <br/>_(Keep pressing until the flashing stops)_

## Remove a shade from a group
This will remove a shade from a group on your remote control. It will not remove the shade from the PowerView® network.
%7 **Locate** these buttons on your remote: %5 ![Removing a remote](/imgs/pv_white_remote_remove_channel_1.svg)
Locate the `manual control button` on your shade. Different shade types have different types of buttons. Below some examples. Consult the shade documentation for the exact location of the `manual control button`.
%4 ![Duette button](/imgs/duette.png) <br/> <p style="text-align: center;">_Duette® shade_</p> %4 ![Pirouette button](/imgs/pirouette.png) <br/> <p style="text-align: center;">_Pirouette® shade_</p> %4 ![Rollerblind button](/imgs/m25t_rollerblind_detail.png) <br/> <p style="text-align: center;">_Rollerblind_</p>
Follow the instructions below for each PowerView® window shading. Depending on your preferences choose a group on one of your remotes. In this case, group &icon-pv-one;```group 1``` is used.
%1 1. %6 **Press and hold** the &icon-pv-stop;`stop` button for **6 seconds**. <br/>_(Keep pressing until the remote lights start blinking)_
%1 2. %6 **Press** the &icon-pv-one;`group 1` button. <br/>_(This will activate group 1 on the remote)_
%1 3. %6 **Press and hold** the `manual control button`.                                         
%1 4. %6 **Press** the &icon-pv-close;`close` button. <br/>_(You will see the blind jog 1x)_
%1 5. %6 **Release** the `manual control button`.
%1 6. %6 If your remote is still flashing **Press and hold** the &icon-pv-stop;`stop` button for **6 seconds**. <br/>_(Keep pressing until the flashing stops)_

## Moving a blind
%7 **Locate** these buttons on your remote: %5 ![Moving a blind](/imgs/pv_white_remote_moving_blind.svg)

**&icon-pv-open;```Open```** blinds assigned to **&icon-pv-one;```group 1```**.
%1 1. %6 **Press** the &icon-pv-one;`group 1` button. <br/>_(Group 1 will light up)_
%1 2. %6 **Press** the &icon-pv-open;`open` button. <br/>_(All shades assigned to group 1 will open)_
%1 3. %6 **Press** the &icon-pv-stop;`stop` button. <br/>_(All shades assigned to group 1 will stop)_

**Pressing** the `all` instead of &icon-pv-one;`group 1` button will move all blinds from all 6 groups on the remote.

## Moving a blind to a favorite position

%7 **Locate** these buttons on your remote: %5 ![Favorite](/imgs/pv_white_remote_moving_favorite.svg)

**Move** blinds assigned to &icon-pv-one;```group 1``` to their &icon-pv-heart;```favorite``` position.
%1 1. %6 **Press** the &icon-pv-one;`group 1` button. <br/>_(Group 1 will light up)_
%1 2. %6 **Press** the &icon-pv-heart;`favorite` button. <br/>_(All shades assigned to group 1 will move to their favorite position)_

**Pressing** the `all` instead of &icon-pv-one;`group 1` button will move all blinds from all 6 groups on the remote to their &icon-pv-heart;```favorite``` position.

## Set a favorite position

%7 Locate the following buttons on your remote: %5 ![Setting a favorite](/imgs/remote_favorite_stop.svg)
%7 Locate the ```shade button``` on your shade. <br/> _(Different shade types have different shade buttons. Consult the shade documentation for the exact location of the `shade button`)_ %5 ![programming buttons](/imgs/programming-buttons.png)

%1 1. %9 **Move your shade to the desired favorite position** <br>_(Use your open, close and stop buttons to move the blind)_
%1 2. %9 **Press &icon-pv-stop; `stop` for 6 seconds.** <br>_(Keep pressing until the remote lights start blinking)_
%1 3. %9 **Press and hold the** `blind button`.
%1 4. %9 **Press the** &icon-pv-heart; `favorite` **button** <br>_(You will see the blind move up and down briefly)_
%1 5. %9 **Release the `blind button`.**
%1 6. %9 If your remote is still flashing **Press `stop` for 6 seconds.** <br>_(Keep pressing until the flashing stops)_

## Performing a programming reset
A programming reset will remove the shade from the PowerView® network and group assignments will be erased.

%1 1. %9 **Press the `blind button` for approximately 12 seconds.** <br/>_(The blind will jog after 6 seconds and finally after 12 seconds)_
%1 2. %9 **Release the `blind button`.**

Your shade is now "disconnected" from the PowerView® network. If you are using the PowerView® APP you should manually delete the blind there too. To reconnect your blind to the PowerView network see [adding a blind to a group](#adding_a_blind_to_a_group) .

## Performing an end limit calibration
An end limit calibration will recalibrate the end limits stored in the shade. The shade automatically searches its new end limits by moving up and down.
>Note: This procedure is not applicable on EOS® 500 Rollerblind and Twist™ shades.

%1 1. %9 **Press** the `manual control button` for approximately **6 seconds**. <br/>_(The blind will jog after 6 seconds)_
%1 2. %9 **Release** the `manual control button`. <br/>_(Depending on the product the shade will start moving up and down several times defining new open and close positions)_

## Put Remote in sleep mode
Sleep mode will disable the motion sensor inside the remote. This will prevent the remote lights to turn on when motion is detected (like being picked up). Doing this will increase battery lifetime.
%7 **Press** the `group 6` button for approximately **6 seconds**. <br/>_(The group buttons will flash as confirmation)_
