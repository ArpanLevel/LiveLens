# VTuber Source (Live2D)

## Overview

The **VTuber Source** brings your Live2D models to life directly on your Android device. It uses an industry-standard rendering engine to support high-quality `.moc3` models with real-time physics, interactivity, and audio-based lip-syncing.

LiveLens is designed to give mobile VTubers a professional production environment without needing a PC.

---

## 🛠️ Step 1: Configuring Your Model (Required)

Before you can add a VTuber source to your scene, you must select a model folder in the app settings.

1. Go to **Settings → VTuber**.
2. Tap **Select & Configure VTuber Model**.
3. **Disclaimer**: Read and agree to the Live2D disclaimer if prompted.
4. **Selection Guide**: Tap "How to select?" for a visual guide.
5. **Folder Selection**: A file picker will open. Navigate to the **folder** that contains your `.model3.json` file.
6. **Crucial**: Do **NOT** select individual files. Simply enter the model's folder and tap **"USE THIS FOLDER"** at the bottom.
7. Grant the app permission to access the folder.

### Compatibility Note
- **Supported**: Cubism models up to version **5.1**.
- **Higher Versions**: For models exported from Cubism 5.3+, please ensure they were exported in **SDK 4.0/4.2 compatibility mode** in the Live2D Editor.

---

## 🎭 Step 2: Adding the VTuber Source

### Method A: Regular Addition
1. Open your streaming scene.
2. Tap the **+ (plus)** icon and select **VTuber**.
3. If you have already selected a model in settings, your avatar will appear on the canvas.

### Method B: Shortcut (If No Model Selected)
If you try to add a VTuber source without setting up a model first:
1. A popup titled **"VTuber Model Required"** will appear.
2. Tap **"Go to Settings"** in the popup.
3. This will take you directly to the VTuber configuration tab, where you can follow the folder selection steps.

> **Update Note**: If you update to a new model in Settings while a VTuber source is already active, you should remove and re-add the source to ensure the new rig loads correctly.

---

## 🔍 VTuber Inspector (Settings)

To fine-tune your avatar, select it on the canvas and tap the **Settings** icon to open the **VTuber Inspector**.

### 1. Basic Controls
- **Opacity**: Adjust transparency.
- **Physics Strength**: Controls how much hair and clothing react to movement.
- **Look At Touch**: When enabled, the avatar’s eyes and head will follow your finger as you touch or drag items on the canvas.

### 2. Voice & Lip Sync (Mic-driven)
LiveLens uses your microphone to animate the avatar’s mouth.
- **Threshold**: Set the minimum volume needed to trigger mouth movement (helps ignore background noise).
- **Voice Sensitivity**: Adjust how wide the mouth opens relative to your speaking volume.
- **Talking Bounce**: Adds a subtle vertical "hop" or bounce while speaking to make the avatar feel more alive.
- **Physics Boost**: Increases hair/cloth physics intensity when you speak loudly.

### 3. Motion & Physics
- **Breathing Strength**: Adjust the intensity of the automatic breathing cycle.
- **Idle Motion**: Controls the strength of natural "swaying" or subtle movements while the avatar is idle.

---

## ⚙️ Advanced Mode (Direct Parameters)

For professional riggers, **Advanced Mode** allows direct editing of the model's internal Live2D parameters.
- **Search**: Quickly find specific parameters (e.g., `ParamEyeBallX`).
- **Warning**: Incorrect values can cause unnatural movements or "break" the avatar's visual state.
- **Reset**: Tap the red **Reset** button to return all manual parameters to their default rigging values.

---

## 🎭 Expressions & Overlays
- **Toggle Expressions**: If your model has built-in expressions (Happy, Blush, etc.), you can toggle them in the Inspector.
- **Floating Overlay**: In **Settings → VTuber**, you can enable **"Show Expressions"** to have quick-toggle buttons on your screen during the stream.

---

## Canvas Controls

- **Move & Resize**: Place your avatar anywhere on the screen.
- **Rotate**: Full 360-degree rotation support with degree feedback.
- **Reset Rotation**: Tap the top-right handle to instantly reset to 0°.
- **Double Tap**: Scale the avatar to fill the canvas.

---

## Related Documentation

- [Sources](./README.md)
- [Audio Configuration](../audio/README.md)
- [Live2D Export Guide](../vtuber/export.md)
