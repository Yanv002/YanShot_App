# YanShot_App
A screen capture and annotation tool for Windows, built for managed corporate estates.

Capture a region, a window or a whole screen; annotate it with arrows, shapes, text, numbered steps, highlighting, blur and pixelation; then copy or save it. Record a region as an animated GIF when a still picture will not do. Everything happens on the local machine. No image is uploaded, no telemetry is collected, and the application makes no network connections of its own.

Requirements
To run
Operating system	Windows 10 version 1809 or later, or Windows 11
Architecture	x64
Privileges	Standard user. No administrative rights are needed at any point
.NET runtime	None, if deployed self-contained (the default). Otherwise the .NET 10 Desktop Runtime

Command line
Argument	Effect
--tray	Start silently in the notification area. Used by the sign-in registration
--capture <mode>	Capture immediately. Modes: Region, FullScreen, AllScreens, ActiveWindow
--settings	Open the settings window on startup
--open <path>	Open an existing image in the editor
<path>	A bare path does the same, so YanShot works as an "Open with" target

Keyboard shortcuts
Global (configurable)
Shortcut	Action
Print Screen	Capture region
Ctrl+Shift+Print Screen	Capture full screen
Ctrl+Alt+Print Screen	Capture active window
(unassigned)	Record region as GIF - assign one in Settings
While recording
Control	Action
Stop	Finish the recording and open the preview
Cancel	Discard the recording
Record hotkey	Pressing it again stops the recording
Capture overlay
Key	Action
Drag	Select an area
Click a window	Capture that window
Ctrl+A	Select the whole screen under the pointer
Enter	Confirm
Esc / right-click	Cancel
Editor
Key	Action		Key	Action
V	Select		Ctrl+Z	Undo
A	Arrow		Ctrl+Y	Redo
L	Line		Ctrl+C	Copy
R	Rectangle		Ctrl+S	Save
E	Ellipse		Ctrl+Shift+S	Save As
P	Pen		Ctrl+O	Open image
H	Highlighter		Ctrl+A	Select all
T	Text		Delete	Delete selection
N	Numbered step		Ctrl++ / Ctrl+-	Zoom
B	Blur		Ctrl+0	Actual size
X	Pixelate		Ctrl+wheel	Zoom at pointer
C	Crop		Esc	Cancel / deselect
Ctrl+N	New Capture - discard and start over (timer button next to it: No delay / 3 / 5 / 10 s)
Hold Shift while drawing to constrain a rectangle to a square, an ellipse to a circle, or a line to 15-degree increments. Arrow keys nudge the selection; hold Ctrl for single-pixel steps.

