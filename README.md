# GTA Keyboard Mapper — Android prototype

This project maps physical keyboard keys to screen touch locations using Android AccessibilityService gesture dispatch.

## How to use

1. Open the project in Android Studio.
2. Build/install the app on the Android phone.
3. Connect a USB OTG or Bluetooth keyboard.
4. Open GTA Vice City and note where its touch controls are.
5. In GTA Keyboard Mapper, edit each mapping's normalized X/Y coordinates:
   - X=0 is the left edge, X=1 is the right edge.
   - Y=0 is the top edge, Y=1 is the bottom edge.
6. Enable the app under Android Accessibility settings.
7. Allow overlay permission if you want to add a calibration overlay in a future version.
8. Return to GTA and test.

## Default mapping

W/A/S/D, Space, Shift, F, R, E and Enter are included as starter mappings.

## Important Android limitation

Android does not expose arbitrary touch injection to ordinary apps. This prototype uses AccessibilityService `dispatchGesture`, so Android's Accessibility permission is required. Some games or Android builds may restrict/ignore simulated touches.

## Next upgrade

A proper calibration overlay can be added so you can drag a marker directly over each GTA touch button and press a physical keyboard key to assign it, instead of entering coordinates manually.
