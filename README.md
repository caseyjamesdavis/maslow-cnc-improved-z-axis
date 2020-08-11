## Improving the Z-axis of a [Maslow CNC Machine](https://www.maslowcnc.com/)

![](maslow_z_axis_improved.png)

 *A 500[mm] long actuator was intially used because at the time there were not any 250[mm] models available.*

#### Upgrade Pros
* Router moves repeatably and accurately in the z-direction
* Router no longer shifts in the x and y-directions when moving in the z-direction
* Router now moves about 2.5x faster in the z-direction

#### Upgrade Cons
* Alignment of router and actuator logitudinal axes
* Complicates dust collection
* High cost relative to kit (~$150)
* Can't adjust carriage wheel preload eccentrics without actuator disassembly
* Can't adjust lead screw nut backlash without actuator disassembly

<br/>
<br/>

## Background
I purchased my Maslow kit from [MAKER MADE](https://makermade.com/).  The kit is well made, well documented and is easy to setup.  The only complaint I had with the system was the sloppy z-axis.  

![](maslow_z_axis_stock.png)

*Original z-axis that uses the manual height adjustment mechanism of the router holder for moving the router and bit in and out of the wood. This is a well known issue and has been fixed in recent M2 versions of the kit.*

<br/>
<br/>

## Purchased Components
I decided to use the OPENBUILDS [250mm C-Beam Linear Actuator](https://openbuildspartstore.com/c-beam-linear-actuator-bundle/) as the basis for the new Z-axis.  There is no need to purchase the stepper motor as it will not work with the Maslow.

![](openbuilds_c_frame_actuator.png)

*250[mm] C-Beam Linear Actuator CAD data*

<br/>
<br/>


## DIY Components
Below are the three main components that need to be 3D printed.  
 
### Router Clamp
![](maslow_z_axis_router_clamp.png)
*Connects the Rigid R2901 router to the carriage of the linear actuator*


### Motor Mount
![](maslow_z_axis_motor_mount.png)
*Connects the existing Z-axis motor to the linear actuator* 

### Brace
![](maslow_z_axis_brace.png)
*Keeps the z-axis perpendicular to the board*

The CAD data supplied can be opened with [FreeCAD V0.19](https://www.freecadweb.org/) and the fantastic [Assembly 4 Workbench](https://github.com/Zolko-123/FreeCAD_Assembly4).

<br/>
<br/>

## Miscellaneous Hardware:
* 16 plastic [M3 T-nuts](https://www.thingiverse.com/thing:1064782)(The M3 T-nut STL is included in this repo for completeness)
* 16 M3 nuts to press into T-nuts
* 16 M3 x TBD bolts for motor mount and brace
* 4 TBD x TBD bolts to secure router clamp to carriage
* 2 TBD x TBD bolts to close router clamp
* 2 TBD x TBD bolts to secure end of actuator to sled

<br/>
<br/>

## Notes:
* The shaft coupler supplied with the actuator kit will work with the Z-axis motor
* Effective pitch of the new lead screw is 8[mm] (2mm pitch x 4 starts)
* I use [WebControl](https://github.com/WebControlCNC/WebControl) and calibrate via the ['holey calibration'](https://webcontrolcnc.github.io/WebControl/Actions/Calibration-Setup/holeyCalibration.html) method

<br/>
<br/>

## To do:
* Add dust collection panels
* Trim actuator to more reasonable length (TBD)
