## Software screen
This is the basic window of this software and consists of the following elements.

<p align="center">
<img alt="SmartScreen" src="./images/names/main.png" style="width:70%">
</p>

#### (A) Title bar
The name of the current project file, the minimize / maximize button, and the end button of the software are arranged.

#### (B) Menu bar
Select a menu and execute various functions.

#### (C) Processing machine control area
The connection status with the processing machine and the error contents are displayed. Also, control of the processing machine is mainly done from here.

#### (D) Toolbar
The graphic area control tool is displayed.

#### (E) Property palette
The location information of the item selected in the graphic area is displayed.

#### (F) Graphic area
You can lay out the processing data.

#### (G) Item list
Processing data is added and a list of processing data is displayed.

#### (H) Parameter setting window
Click an item displayed in the item list to display and set the processing parameters of the item.


## Menu bar
### File
- New Project: Create a new project.
- Open Project: Open a saved project.
- Save Project: Save the currently open project.
- Save Project As: Save the currently open project as an alias.

### Edit
- Undo: Restore the project editing state to the previous state.
- Redo: Advance the project editing state to the next state.
- Copy: Copy the selected graphic object to the paste buffer.
- Paste: Paste the copied graphic object.
- Delete: Delete the selected item.

### Selection
- Select All: Select all graphic objects.

### Machine
- Stop operation: Stop the operation of the processing machine.
- Go to Origin: Send an origin return instruction to the processing machine.
- Create Grid Item: Create the grid displayed on the graphic area as a processing item.

### UserDictionary
- UserDictionary Manager: Open the User dictionary manager. You can edit, import / export, etc. the user dictionary.

### Setting
- User Setting: Various settings can be made.
- EtcherLaser: (EtcherLaser only) If there is a discrepancy between the camera position and the processing result, you can correct the position using the offset function. You can also upgrade the firmware version.

### Help
- About SmartDIYs Creator: You can check the version information of the software.
- Open Software Manual: Open this manual in a browser.


## Processing machine control area

<p align="center">
<img alt="SmartScreen" src="./images/names/machine_control.png" style="width:100%">
</p>

In this area, you can get information about the processing machine and give operation instructions to the processing machine. The connection status with the processing machine is displayed as "connected" or "not connected". Also, if there is an error, the content of the error is also displayed.

- Estimated processing time: Show the approximate machining time of the current project in hours: minutes 'seconds".
- Return to Origin : The processing machine checks the origin position of the laser head and eliminates the error of the head position.
- Position: Switch to position check mode. In this mode, the icon of the laser head is displayed in the graphic area, and you can confirm the actual processing position of the object. Click this icon again to cancel the position check mode.
- Check Area: The laser head of the processing machine indicates the processing range.
- Stop: Stop the operation of the processing machine.
- START: When the button is pressed, a confirmation dialog is displayed and processing starts.


## toolbar

<p align="center">
<img alt="SmartScreen" src="./images/names/toolbar.png" style="width:80%">
</p>

- (1) Selection tool: You can select a graphic object in the graphic area by clicking on it.
- (2) Pan tool: You can change the display range by dragging the graphic area.
- (3) Zoom tool: You can enlarge the display range by clicking on the graphic area. You can also reduce the display range by clicking while holding the Alt key. You can change the magnification freely with drag operation.
- (4) Preview: Create processing instruction data and displays a visualization of the generated processing instruction data.
- (5) Copy: Copy the selected graphic object to the paste buffer.
- (6) Paste: Paste the copied graphic object.
- (7) Delete: Delete the selected item.
- (8) Undo: Restore the project editing state to the previous state.
- (9) Redo: Advance the project editing state to the next state.
- (10) Capture: The range of the processing area is captured with the camera of the machine and displayed on the canvas. Be careful not to cover the camera markers with any materials.<br/>
※ A small amount of discrepancy may occur in the display position due to lens distortion.

## Property palette
### When graphic object is selected

<p align="center">
<img alt="SmartScreen" src="./images/names/object_property.png" style="width:80%">
</p>

Under normal conditions, you can display and edit the coordinate information of graphic objects in the graphic area.

- X: Show X coordinate of graphic object. Coordinates can be specified by changing this number.
- Y: Show Y coordinate of graphic object. Coordinates can be specified by changing this number.
- W: Show the width of the graphic object. Width can be specified by changing this number.
- H: Show the height of the graphic object.Height can be specified by changing this number.
- Constrain Width And Height Proportions: In this mode, when width / height is specified in the above operation, height / width is automatically set to fix aspect ratio. You can cancel / set the mode by clicking this button.
- Rotate: Show the rotation of a graphic object. Rotation can be specified by changing this number.


### In position check mode

<p align="center">
<img alt="SmartScreen" src="./images/names/laserhead_property.png" style="width:80%">
</p>

In position check mode, you can display and specify the coordinates of the laser head.

- X: Show X coordinate of laser head. You can move to the coordinate position by changing this number.
- Y: Show Y coordinate of laser head. You can move to the coordinate position by changing this number.
- Set UserOrigin: You can set the current coordinates as the user origin.

## Graphic area
This is an area to lay out the processing data.
- Canvas: Indicates the processing range of the processing machine. The processing range can be set by user setting.
- Scaling tools: You can manipulate the display area of the graphic area.

## Item list
Add Item: Click to display a menu and you can add items to the project.
- Select File: Add a local file.
- From Catalog: Adds figures etc. provided in this software.
- Text Item: Create and add text objects.
- Scan: (EtcherLaser only) Create items from scanned with the camera of machine.<br/>
※ The button is disabled when the top cover is closed.

Added Items can be checked from the list. Processing is performed in the order of this list.

### Right click menu
Right-click on an item to display the menu.
- Enable: Switch the setting item "Enable" of the machining parameter.
- Delete this item: Delete the this item and object.
- Select this objects: Select the object associated with the item. Select a group if it is grouped.

### Display mode switching
You can switch the display mode by clicking the icon at the bottom of the item list.
<p align="center">
<img alt="SmartScreen" src="./images/names/itemlist_mode.png" style="width:50%">
</p>

## Parameter setting window
Click an item displayed in the item list to display and set the processing parameters of the item.

- Manual: You can set Enables / disables of item processing and parameters manually.You can also register the set parameters in the user dictionary.
- UserDictionary: You can select the registered parameter.
- Preset: Processing parameters estimated by our company (The processing result depends on the characteristics of the material actually processed and the adjustment accuracy of the machine)
