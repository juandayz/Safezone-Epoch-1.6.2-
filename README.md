# Safezone-Epoch-1.6.2-

 The very old safezone script by infistar... i was using it in 1.0.5.1  and made some changes to use in 1.6.

Instructions:
    1. Paste this "scripts" folder into mpmissioms\instance_11.chernarus\
    2. Open your init.sqf
    3. At the very bottom of the file add this line:  [] execVM "scripts\16_safezone.sqf";
    4-WARNING!!! if ure using some kind of mod that allow vehicles with GodMode out of safezones..  then you will need change 
    16_safezone.sqf  the path for veh_handleDam.sqf by the path that youre using your custom veh_handleDam.sqf

this line:  fnc_veh_handleDam = compile preprocessFileLineNumbers '\z\addons\dayz_code\compile\veh_handleDam.sqf'; 

for example:

```ruby
fnc_veh_handleDam = compile preprocessFileLineNumbers '\z\addons\dayz_code\compile\veh_handleDam.sqf'; 
```
by
```ruby
fnc_veh_handleDam = compile preprocessFileLineNumbers 'dayz_code\compile\veh_handleDam.sqf';
```
or whatever path that youre using.


