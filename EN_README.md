
# VRChat Gimmick Package - Portable Fire Alarm

This is a VPM package for the "Portable Fire Alarm" gimmick used in VRChat.  
The gimmick is a neck-worn fire alarm equipped with various effects and buttons.  
If you purchased or downloaded this via Booth, you can install and update it using this repository via VPM.

---

## 🔧 Overview

- A portable fire alarm that can be worn around the neck.
- Press the alarm button in emergencies to alert others. Helps prevent spreading fires.
- On activation, it produces sound and a speech bubble (Quest version shows bubble only).
- Open the cover and press the stop button to deactivate.
- The LED inside the button blinks while active.
- Menu-based control is fully supported (toggle, resizing, etc.), even for desktop users.
- With PhysBone, the alarm can be handheld, pressed by others, or fit around your neck (fit may vary by avatar).
- Lightweight design minimizes avatar load.
- Includes both PC and Quest (Pico/smartphone) versions.
- PC version supports audio playback. Use responsibly and avoid misuse. The author holds no responsibility for consequences.

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

## 📦 Included Files

| File Name | Description |
|----------|-------------|
| `PortableFireAlartSystem.zip` | Compressed package |
| `PortableFireAlartSystem.unitypackage` | Main Unity package |
| `PortableFireAlartSystem.prefab` | Prefab for PC (with sound) |
| `PortableFireAlartSystem_Quest.prefab` | Prefab for Quest (no sound) |
| `readme.txt` | This manual |

---

## 🛠 Supported Environment

- Unity: 2022.3.22f1
- Shader: Standard Lite / Multiply (SDK default)
- Required Assets:
  - Modular Avatar v1.13.0+
  - AtlasTexture v1.8.12+

---

## 🧩 Installation Instructions

### From VPM Repository

1. Follow the installation instructions [here](https://github.com/emuoh/vpm-repos/blob/main/README.md)
2. Drag and drop `PortableFirealarmSystem.prefab` (or `PortableFirealarmSystem_QUEST.prefab` for Quest) into the avatar hierarchy.

### From .zip File

1. Extract the `.unitypackage` file and drag it into your Unity `Assets` folder.
2. Drag and drop the appropriate prefab into the avatar hierarchy.

---

## 🧩 Position Adjustment

1. Adjust the position and scale of `MA_BoneProxy_Neck` to fit the neck.
2. Adjust the position of `PB_COL_FAS_Belt` to follow the body.

---

## 🧪 Notes for Quest Users

- If the Multiply Shader doesn’t show transparency, switch to an opaque material.
- Be aware that excessive PhysBone usage may prevent upload.

---

## 🎮 How to Operate

### Menu Controls (PC/VR)

| Button Name | Function |
|-------------|----------|
| On | Shows the fire alarm |
| Button On | Toggles the emergency button |
| Alarm Stop | Stops the alarm |
| Cover Open | Opens/closes the stop button cover |
| Onomatopeia On | Toggles speech bubble |
| Sound On | Toggles alarm sound (PC only) |
| Voice On | Toggles voice audio (default OFF) |
| Body Size | Adjusts alarm size |
| Belt Spread | Adjusts neck distance |
| Belt Width | Adjusts belt width |

### Manual Operation (VR)

1. Press the emergency button with your finger to activate the alarm.
2. Touch the cover to open.
3. Press the stop button to stop the alarm.
4. Touch the cover again to close.

---

## 🎁 Bonus Voice Clips

- Multiple voice variations are included in the `Sound/Voice` folder.
- You can replace the `AudioClip` in `FAS_Sound` or `FAS_Voice` to use them.

---

## 🔁 Updates

- If installed via VPM, update with one click from VCC’s "Updates" tab.
- Also detected automatically via ALCOM.
- If installed manually from .zip, redownload and reinstall from the original site (Booth, etc.).

---

## 👤 Author / Contact

- Author: emuoh ([https://emuoh3.booth.pm/](https://emuoh3.booth.pm/))
- GitHub: [emuoh/PortablFireAlarmSystem](https://github.com/emuoh/PortablFireAlarmSystem)
- X (Twitter): emuoh3@x.com

---

## 📜 License

This gimmick follows the [VN3 License](https://www.vn3.org/index).  
See [LICENSE.md](https://github.com/emuoh/vpm-repos/blob/main/LICENSE.md) for details.

---

## 🧷 Credits

- Unity 2022.3
- VRCSDK3

---

## 🔈 Audio Credits

- Sound effects: [Otologic](https://otologic.jp)
- Voice synthesis: VOICEVOX (Shikoku Metan, Zundamon, Ryusei Aoyama)
