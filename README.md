[![](http://webapp.projectfdl.com/img/FDL%20Logo%20Tiny.png)](https://www.projectfdl.com)

  
# FDL-3-Blaster

Welcome to the FDL-3 blaster repository


## This project is licensed under the terms of the Creative Commons Non-Commercial Attribution Share Alike 4.0 license
Print it, tweak it, share it and if you do and give us props. Please don't sell it without Project FDL permission.


# Operating your FDL-3

  

## Settings (Applicable to full auto tail, firmware version 1.05)

  

**Speed**
Value: 0 - 100 : Default: 50
Speed or power setting used to adjust the velocity the blaster fires darts.

**ROF (Rate of Fire)**
Value: 0 - 100 : Default: 100
Rate of fire setting to adjust time between each dart fired when in burst or full auto.

**Burst**
Value: 1, 2, 3, F : Default: 1
Number of darts fired per single trigger pull. F (full auto) will continue firing darts until you release the trigger.

**MinSpin (Minimum Spinup)**
Value: 120 - 500 : Default: 220
Time in milliseconds for motors to spinup between trigger pull and firing dart when speed set to 0.

**MaxSpin (Maximum Spinup)**
Value: 150 - 500 : Default: 200
Time in milliseconds for motors to spinup between trigger pull and firing dart when speed set to 100.
Note: MinSpin and MaxSpin together create a range of spinup time. When speed is set to 50, spinup time is half way between MinSpin and MaxSpin. Eg. MinSpin = 200, MaxSpin = 300, Speed = 50. Actual spinup time = 250. Speed = 75. Actual spinup time = 275.

**Fire Mode**
Value: SAFE, ABIDE, AUTO, CACHE : Default: ABIDE
Setting for how the blaster reacts to a trigger pull prior to firing a dart.
- Safe: safety mode. Blaster will beep and not fire dart.
- Abide: Trigger abide. Blaster will only fire a dart if trigger is held down for the full spinup duration. If trigger is released prior to the completion of spinupt time, the blaster will not fire.
- Auto: Blaster will fire dart automatically. If trigger is released prior to the completion of spinup time, the blaster will continue it's fire cycle and proceed to fire all darts set by the burst setting.
- Cache: Cached mode. The blaster will "cache" the number of trigger pulls during the spinup duration. If you are able to pull the trigger three times during spinup, the blaster will fire three darts. Twice, two darts. Once, one dart.

**Spindown**
Value: 7 - 18 : Default: 14
Rate at which the blasters motors wind down or "spindown" to a stop. Lower is faster. Higher is slower. The value is technically equal to the time in milliseconds to lower the speed of the blaster by a single increment.

**Idle (Idle Time)**
Value: 0 - 10 : Default: 0
After the end of a fire cycle the motors will spin at a slow idle speed for this number of seconds. This allows the motors to spinup faster than if they were to start from a dead stop. Setting this to 0 will disable the feature. Note: if the trigger is held down at the end of a fire cycle, the motors will run at this idle speed until trigger is released.

**Load**
Load user preset 1, 2, 3 or back out of menu.

**Save**
Save current blaster settings to one of three user preset slots which can be recalled later by the load menu or user buttons on the side of the blaster. Note: only settings prior before the Load menu item are stored in presets. Speed, ROF, Burst, MinSpin, MaxSpin, FireMode, Spindown and Idle.

**MinSpd (Minimum Speed)**
Value: 0 - 100 : Default: 0
Determines the minimum speed value that may be set by the speed setting. Eg. if set to 25, the speed gauge will not go lower than 25.

**MaxSpd (Maximum Speed)**
Value: 0 - 100 : Default: 100
Determines the maximum speed value that may be set by the speed setting. Eg. if set to 80, the speed gauge will not go higher than 80. Recalled presets with higher speed values will default to this setting. The last value this setting was set to prior to powering off the blaster can be locked by flipping the red speed lock switch located on next to the screen on the board in the rear of the blaster. The rear cap piece must be removed to access this switch. This value cannot be altered while the blaster speed lock is enabled.

**BtnMode (Button Mode)**
Value: PRESET, SPEED, ROF, BURST : Default: BURST
Determines what the three user quick buttons on the side of the blaster do. These buttons must be briefly held down for action to take place.
- Preset: Loads user preset. Front button loads preset 1. Rear button closed to user loads preset 3.
- Speed: Sets blaster speed. From front to rear button. 50, 75, 100
- ROF: Set blaster rate of fire. From front to rear button. 50, 75, 100
- Burst: Sets blaster burst count. From front to rear button. 1, 2, F

**BrkAgr (Braking Aggression)**
Value: 3 - 20 : Default: 16
Determines how aggressively the pusher brakes prior to reaching a stop at the rear of its cycle. Setting lower may produce a more responsive cycle but may leave the pusher extended at the end of the cycle. Setting higher may resolve issues with a pusher that does not stop properly at the rear of its cycle. This setting should rarely need to change.

**ULock (User Lock)**
Enable complete blaster lockout by setting a user defined sequence of quick button presses. Blaster will not function once lock is set and may be unlocked by reentering the defined sequence. Note: do not forget your code. While it is possible to reset your blaster, the method of doing so is not described in this document.

**Bright (Brightness)**
Value: 0 - 100 : Default: 100
Sets the brightness of the oled display. This is a very subtle change in a high light environment but more obvious in darker surroundings.

**Sound**
Value: OFF, ON : Default: ON
Enables or disables audible beeping while navigating menus, loading presets etc.

**BatOff (Battery Offset)**
Value: -5 - 5 : Default: 0
Offsets the read battery voltage in increments of 0.1 volts. This is only for use with legacy or self built blasters if a full 3s battery does not read 12.6 volts.

**Info**
Displays current firmware version.

