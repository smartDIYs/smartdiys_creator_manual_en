This section describes the settings in the User Settings dialog.

<p align="center">
<img alt="UserOrigin" src="./images/usersetting/about.png" style="width:70%">
</p>

## Processing machine

<!-- <p align="center">
<img alt="SmartScreen" src="./images/usersetting/settings_1.png" style="width:70%">
</p> -->

### Configuration
Set the model name and laser type of your machine. This setting affects the machining range, driver power and preset parameters.

### Processing range
Set the processing range of your processing machine. There is usually no need to change the settings, as these are automatically set when you select the model name above. Set it when using an extension frame etc.

### Driver power
Adjust the current value flowing to the motor. It is not necessary to change usually because it is set automatically when you select the model name above. If step-out occurs frequently, adjusting this value may improve the situation.

---------------
## Unit, display

<!-- <p align="center">
<img alt="SmartScreen" src="./images/usersetting/settings_2.png" style="width:70%">
</p> -->

### Unit
You can set the grid spacing, the rectangle display unit of objects, etc. to mm or inch.

### Display
You can show or hide the grid.<br/>
You can also set the grid spacing and number of divisions.
Basic grids appear gray on the campus, and split grids appear as red dotted lines.
If the division number is 1, only the basic grid is displayed.

### Preview
Specify the line width at preview. By setting the actual laser width, you can get close to the impression of the final product.

---------------
## Processing

<!-- <p align="center">
<img alt="SmartScreen" src="./images/usersetting/settings_3.png" style="width:70%">
</p> -->

Seek speed: The movement speed when the laser head does not output the laser. Basically, it is the moving speed from the point where the laser output ends to the next laser output start point.

### Seek speed
Default mode: Set the seek speed to the specified value.  
Quality mode: Set the seek speed to the processing speed.  
※ During raster processing and hatching processing (during vector painting processing), operations are always performed according to the Quality mode.

### Seek speed (during maintenance)
You can set the moving speed of the laser head for position check and range check.

### Iterative processing (vector stroke)
If this setting is enabled, the processing order during cutting will be affected.  
Example: When there are multiple pieces for a single vector item (i.e., a "◯" and a "△" as part of one item), and "Times" is set as 2 or more, the machine will process like items together.  
[Enable]: ◯ > ◯ > △ > △  |  [Disable]: ◯ > △ > ◯ > △

---------------
## Correction

<!-- <p align="center">
<img alt="SmartScreen" src="./images/usersetting/settings_4.png" style="width:70%">
</p> -->

```
※ These functions are auxiliary.
Please use it after making sufficient hardware adjustments.
```

### Size correction
When converting a figure to G-Code, it will be scaled by the specified ratio in each direction. If the object is near the boundary of the machining range, it may touch the limit switch during machining.

### X axis tilt correction
Apply shear to the object when converted to GCode to correct the machine's X-axis tilt. If the object is near the boundary of the machining range, it may touch the limit switch during machining.


<!-- ---------------
## パラメータ

<p align="center">
<img alt="SmartScreen" src="./images/usersetting/settings_5.png" style="width:70%">
</p>

### パラメータ初期値
新しいアイテムをインポートする際に設定されるレーザパラメータのデフォルト値を設定します。すでに生成されているパラメータには影響しません。 -->

---------------
## Other

<!-- <p align="center">
<img alt="SmartScreen" src="./images/usersetting/settings_6.png" style="width:70%">
</p> -->

### Intervals
You can set the automatic intervals. If the continuous processing duration is exceeded, machining will be paused for the specified duration.
This duration is not added to the estimate time and remaining time.

```
Processing: [10 - 60] minutes / Interval: [3 - 10] minutes can be set.
```

### Notice
Set enable / disable of automatic notification of software update. If there is a newer version, a dialog will appear when the software is launched.
