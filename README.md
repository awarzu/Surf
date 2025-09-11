# SURF

A Python Tkinter application that emulates the functionality of CustomCurve Pro for creating and testing custom mouse sensitivity curves.

## Features

✅ **Input DPI and Sensitivity Settings**
- Fields for mouse DPI and in-game sensitivity input
- Real-time parameter adjustment

✅ **Create Custom Sensitivity Curves**
- Interactive graphical interface for plotting sensitivity curves
- Separate curves for horizontal and vertical axes
- Add points: Double-click on the graph
- Remove points: Right-click on existing points
- Move points: Drag with left mouse button
- Zoom: Mouse wheel
- Pan: Middle mouse button + drag

✅ **Adjust Curve Bias**
- Independent sliders for horizontal and vertical curve bias
- Range: 0.1x to 3.0x multiplier

✅ **Save and Load Profiles**
- Save/load curve configurations as JSON profiles
- Profile management panel with list view
- Create, rename, delete, and switch between profiles
- Import/export profiles via file dialog
- Import external CustomCurve files (.ccurve) and apply them instantly

✅ **Apply and Test Settings**
- Built-in test area for real-time curve testing
- Mouse tracking within test canvas shows sensitivity effects
- No system-wide changes - testing is completely sandboxed
- Visual feedback showing current gain values

✅ **Modern Dark UI**
- Windows 10/11 compatible dark theme
- Professional appearance similar to CustomCurve Pro
- Responsive layout with proper scaling
