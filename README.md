# Addons and configuration for 3D printers


#### Anycubic i3 mega S Klipper fast printing (first layer on 200 mm/s speed): https://youtu.be/GtIsCP1_Cyg 

### [Klipper configuration file for Anycubic i3 mega S](https://github.com/widapro/3d-printers/blob/master/anycubic-i3-mega-s/klipper/printer.cfg)
This config file contains settings of all printer pins (steppers, sensors) for Anycubic i3 mega S in the factory configuration



Klipper firmware should be compiled for the **atmega2560**

 Config file includes
  - Configuration for **original** or **2208(2209)**, rotated by cabel, drivers
  - Mesh bed leveling: **BLtouch** (3DTouch sensor from Triangelab)
  - **Manual meshed bed leveling** (commented out)
  - **'virtual_sdcard'** for fast printing without gaps
  - Beeper through **M300** gcode
  - Pause/Resume through **M600** for filament change

 Home position is determined by 3DTouch. **Z limit switches are not used**.

 The latest version of the config reference is also available online at: [https://www.klipper3d.org/Config_Reference.html](https://www.klipper3d.org/Config_Reference.html)
<br />
<br />
<br />
**!!! Do not forget to check your configuration for: !!!**
* step_distance
* nozzle_diameter
* pressure_advance
* serial
* [bltouch]
* [virtual_sdcard]
<br />
<b>!!!</b> Also important to follow all config check from this manual before start printing: https://www.klipper3d.org/Config_checks.html
<br />
<hr />
Useful documentation for slicer/printer (not special for Klipper) calibration: https://teachingtechyt.github.io/calibration.html#intro
