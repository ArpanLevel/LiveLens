# UVC Source (Capture Card)

## Overview

The **UVC (USB Video Class) Source** allows users to connect external USB devices like **HDMI Capture Cards**, USB Webcams, or DSLR cameras to their LiveLens scene. 

This is a powerful feature for mobile gamers who want to stream from a console (like Nintendo Switch, PlayStation, or Xbox) using their phone as the streaming hub.

> **Note**: This feature is currently in **Beta**. Performance and compatibility depend on the Android device's USB support and the capture card's hardware.

---

## Adding a UVC Source

To add a capture card:

1. Connect your capture card to your phone using a USB OTG adapter or a USB-C cable.
2. Tap the **+ (plus)** icon in LiveLens and select **UVC (Beta)**.
3. A **USB Capture Cards** scanner dialog will appear.
4. Tap your device in the list.
5. Grant the system permission to access the USB device when prompted.

---

## Opening UVC Settings

To open the Capture Card Editor:

1. Select the **UVC Source** on the canvas.
2. Tap the **Settings** icon.

The Editor features a live preview of the capture card feed on the left and configuration options on the right.

---

## Capture Card Editor Features

### Resolution & Performance
Capture cards often support multiple resolutions and formats (like MJPEG or YUYV).
- **Device Resolution**: Select the desired resolution from the dropdown (e.g., 1920x1080, 1280x720).
- **Auto Mode**: Use "Default (Auto)" to let LiveLens choose the best compatible resolution.
- **Apply Change**: Note that resolution changes apply after the source is restarted.

### Audio Configuration
LiveLens provides full control over the capture card's audio:
- **Feed Audio to Stream**: Toggle this on to include the game/camera audio in your stream or recording.
- **Hear it (Monitor)**: Toggle this on if you want to listen to the capture card's audio through your phone's speakers or headphones while streaming.
- **Volume Slider**: Adjust the audio level from 0% to 200%.

### Visual Adjustments
- **Cropping**: Use the blue handles in the preview area to crop out black bars or unwanted edges from your capture feed.
- **Opacity**: Adjust the transparency of the UVC source.
- **Reset All**: A quick button to reset scale, crop, and opacity to default values.

### Troubleshooting (Report Issue)
If you encounter glitches or the device fails to load, tap the **Report Issue** button in the header. This will upload a diagnostic log to help the developer improve compatibility for your specific hardware.

---

## Canvas Controls

The UVC Source supports standard interactive controls:
- **Move & Resize**: Drag and pinch on the canvas.
- **Rotate**: Use the rotation handle (bottom-right).
- **Rotation Degree**: View the exact angle in the top-center indicator.
- **Reset Rotation**: Tap the top-right handle to return the feed to 0°.
- **Double Tap**: Quickly scale the capture feed to fill the canvas.

---

## UVC Source Settings Summary

| Setting | Description |
|---|---|
| Available Devices | Switch between connected USB video devices |
| Resolution | Set the capture quality and format (MJPEG/YUYV) |
| Feed Audio | Include capture card sound in the stream |
| Monitor Audio | Listen to the capture card sound locally |
| Volume | Boost or lower the audio signal |
| Cropping | Frame the capture area manually |

---

## Related Documentation

- [Sources](./README.md)
- [Audio Settings](../audio/README.md)
- [Troubleshooting UVC](../troubleshooting/uvc-beta.md)
