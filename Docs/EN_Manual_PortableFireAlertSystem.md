
# 🔥 Portable Fire Alert System - User Manual

This is a neck-worn portable fire alarm gimmick.  
It can be integrated into a VRChat avatar and supports both PC and Quest platforms, including PhysBone compatibility.

---

## 📦 Included Files

| File Name | Description |
|-----------|-------------|
| `PortableFireAlartSystem.zip` | Complete compressed archive |
| `PortableFireAlartSystem.unitypackage` | Unity package containing the system |
| `PortableFireAlartSystem.prefab` | Prefab for PC (with audio) |
| `PortableFireAlartSystem_Quest.prefab` | Prefab for Quest (no audio) |
| `readme.txt` | This manual |

---

## 🛠 Supported Environment

- Unity: 2022.3.22f1
- Shader: Standard Lite / Multiply (SDK default)
- Required assets:
  - Modular Avatar v1.13.0 or higher
  - AtlasTexture v1.8.12 or higher

---

## 📐 Resource Usage (PC/Quest)

| Item | Value |
|------|-------|
| Polygon Count | 2284 |
| Skinned Meshes | 1 |
| Materials | 2 |
| Textures | 2 |
| Bones | 8 |
| PhysBones | 1 |
| PhysBone Colliders | 1 |
| Contact Receivers | 2 |
| Audio Sources | 2 (PC only) |

---

## 🧩 Installation

1. Drag and drop the `.unitypackage` into your `Assets` folder.
2. Place the `Prefab` directly under your avatar (use `_Quest` version for Quest).
3. Adjust the position and size of `MA_BoneProxy_Neck` to fit around the neck.
4. Adjust the position of `PB_COL_FAS_Belt` to fit the body.

---

## 🧪 Notes for Quest

- If Multiply Shader does not render transparency, switch to a non-transparent material.
- Upload may fail if too many PhysBones are in use. Please be cautious.

---

## 🎮 Operation Guide

### Menu Operations (PC/VR)

| Button Name | Function |
|-------------|----------|
| On | Shows the alarm system |
| Button On | Toggles the emergency button ON/OFF |
| Alarm Stop | Stops the alarm using the stop button |
| Cover Open | Opens/closes the stop button cover |
| Onomatopeia On | Toggles the speech bubble ON/OFF |
| Sound On | Toggles alarm sound ON/OFF (PC only) |
| Voice On | Toggles voice ON/OFF (default OFF) |
| Body Size | Adjusts the device size |
| Belt Spread | Adjusts distance from neck |
| Belt Width | Adjusts belt width |

### Manual Operations (VR)

1. Press the emergency button with your index finger to activate the alarm.
2. Touch the cover to open it.
3. Press the stop button to deactivate the alarm.
4. Touch the cover again to close it.

---

## 🎁 Bonus Voice Clips

- Several voice variations are included in the `Sound/Voice` folder.
- You can replace the `AudioClip` in `FAS_Sound` or `FAS_Voice` to use them.

---

## 🔈 Materials Used

- Sound effects: [Otologic](https://otologic.jp)
- Voice synthesis: VOICEVOX (Shikoku Metan, Zundamon, Ryusei Aoyama)

---

## 📜 License

This gimmick follows the [VN3 License](https://vn3.dev).  
Please refer to `LICENSE.md` for more information.
