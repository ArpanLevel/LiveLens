# Web Source

## Overview

The **Web Source** allows users to add web-based content directly to their LiveLens scene. This is perfect for adding stream alerts (Streamlabs, Streamelements), live chats, widgets, or even full websites to your broadcast.

LiveLens features a highly optimized web engine designed to handle real-time updates and interactive overlays without draining your device's battery.

---

## Adding a Web Source

To add web content:

1. Tap the **+ (plus)** icon and select **Web Source**.
2. By default, it will be added to the canvas.
3. Tap the source and open **Settings** to configure the URL or local file.

---

## Web Source Editor Features

The Web Source Editor is divided into a **Preview Section** (left) and a **Settings Panel** (right).

### 1. Source Types
- **URL (Online)**: Enter any standard web address.
- **Local HTML**: Load offline HTML files from your phone's storage. Ideal for custom widgets that don't need internet.
- **Presets**: Quick access to common streaming sites like YouTube, Twitch, Streamlabs, and StreamElements.

### 2. Browser Mode (Interactive)
By default, web sources are "static" (non-interactive) to prevent accidental clicks on the canvas.
- **Toggle Browser Mode**: Turn this on to interact with the website. You can log in to accounts, click buttons, or scroll within the editor.
- **Full Screen Mode**: While in Browser Mode, you can tap the **Fullscreen icon** in the preview area to interact with the website on a larger scale.
- **Browser Toolbar**: When active, a toolbar appears with **Home**, **Back**, **Forward**, and **Reload/Stop** controls.

### 3. Crop Mode
If you only want to show a specific part of a page (e.g., just the chat box):
1. Toggle **Enable Cropping** in the settings panel.
2. Blue handles will appear in the preview area. Drag them to frame your content.
3. **Note**: Cropping is disabled when you are interacting with the page in Browser Mode.

### 4. Rendering Quality
Adjust the rendering load based on your device's performance:
- **Performance (0.5x)**: Renders at half resolution (Best for older devices).
- **Balanced (0.75x)**: A mix of quality and speed.
- **Native (1.0x)**: Full-quality rendering.

---

## Smart Features for Streamers

### Auto-Scroll (Chat Support)
LiveLens includes an intelligent script that detects scrollable chat containers (like YouTube or Twitch chat). It automatically keeps the chat scrolled to the bottom so your stream always sees the latest messages.

### OBS Compatibility
The web source simulates an OBS (Open Broadcaster Software) environment, triggering standard visibility events (`obsSourceVisibleChanged`) so that animations and alerts start correctly when you switch scenes.

### Performance Optimization
- **Idle Pacing**: When the web page isn't changing, LiveLens reduces the capture rate to save battery.
- **Warm-up Mode**: When a page first loads, the engine runs in high-performance mode to ensure animations finish loading before slowing down for power saving.

---

## Canvas Controls

- **Move & Resize**: Position the widget anywhere on your layout.
- **Rotate**: Full rotation support with a degree indicator.
- **Reset Rotation**: Tap the top-right handle to instantly reset to 0°.
- **Double Tap**: Scale the web source to fill the canvas.

---

## Web Source Settings Summary

| Setting | Description |
|---|---|
| Browser Mode | Enables touch interaction with the website |
| Full Screen | Open a larger interactive preview |
| Crop Mode | Frame a specific section of the page |
| Local HTML | Load `.html` files from your device |
| Quality Scale | Choose between Performance and Native quality |
| Presets | Quick links for popular streaming tools |

---

## Related Documentation

- [Sources](./README.md)
- [Stream Alerts Setup](../overlays/alerts.md)
- [Troubleshooting Web](../troubleshooting/web-loading.md)
