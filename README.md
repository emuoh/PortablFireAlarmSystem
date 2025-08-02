
# VRChatギミックパッケージ - 携帯型火災報知器

[English README Here](https://github.com/emuoh/PortablFireAlarmSystem/blob/main/EN_README.md)

VRChatで使えるギミック「携帯型火災報知器」のVPMパッケージです。

このギミックは、アバターの首にかけて携帯できる火災報知器です。ボタンなどの各種ギミック・エフェクトを搭載しています。

---

## 🔧 概要

- 首にかけて携帯できる火災報知器です。
- 何かが炎上している・しかかっている時にすかさず押すことで回りに周知し、延焼を防ぐことが可能かも知れません。
- 本体警報ボタンを押すと作動して音と吹き出し文字が出せます(Quest版は吹き出し文字のみ)。
- 停止ボタンのカバーを開けて警報停止ボタンを押すと停止します。
- 作動中はボタン内部のLEDも点滅します。
- デスクトップの方でも使用できるようメニューから各種オンオフ、サイズ調整を含めた全ての操作が可能です。
- PhysBone使用で手に持ったり、他の人にも押してもらえたり、あなたの首にやさしくフィットできます(形状の特性上、フィットしきれない場合もあります)。
- 軽量設計ですので、アバターへの負荷も小さくしております。
- PC 版と Quest(Pico or スマホ、以下 Quest) 版が入っております。
- PC版は音が出せますが、誤解が起きないよう公序良俗に反しない範囲で適切にご使用ください(使用に関しての一切の責任は負えませんのでご了承ください)。

---
## 📐 使用リソース (PC/Quest 共通)

| Item | Value |
|------|-------|
| Polygon Count | 2284 |
| Skinned Meshes | 1 |
| Materials | 2 |
| Textures | 2 |
| Bones | 8 |
| Physbone Tansform | 8 |
| Physbone Collision Check Count | 7 |
| Physbone Components | 1 |
| Physbone Colliders | 1 |
| Contact Receivers | 2 |
| Audio Sources | 2 (PC only) |

---

## 📦 同梱内容

| ファイル名 | 説明 |
|------------|------|
| `PortableFireAlarmSystem.zip` | 一式を含む圧縮ファイルです。 |
| `PortableFireAlarmSystem.unitypackage` | 本体のUnityパッケージです。 |
| `README.md` | この説明書です。 |
| `PortableFireAlarmSystem.prefab` | PC向けPrefab（音声あり）です。 |
| `PortableFireAlarmSystem_Quest.prefab` | Quest向けPrefab（音声なし）です。 |
| `anim` | アニメーションファイルが入ったフォルダです。 |
| `Controller` | アニメータが入ったフォルダです。 |
| `fbx` | 本体のfbxファイルが入ったフォルダです。 |
| `mat_tex` | マテリアルとテクスチャファイルが入ったフォルダです。 |
| `Sound` | 警報音のファイルが入ったフォルダです。 |
| `Voice` | 音声のファイルが入ったフォルダです。 |

---

## 🛠 対応環境

- Unity：2022.3.22f1
- Shader：Standard Lite / Multiply（SDK標準）
- 必須アセット：
  - [Modular Avatar v1.13.0 以上](https://modular-avatar.nadena.dev/ja/docs/intro)
  - [AtlasTexture v.0.10.10 以上](https://ttt.rs64.net/)
  - [Avatar Optimizer v1.8.12 以上](https://vpm.anatawa12.com/avatar-optimizer/ja/)
リンクは各アセットの最新のVPNリポジトリによる導入サイトになります。
可能な限り最新のバージョンを使用してください。
バージョンが低い環境の場合は、正常に動作しないことがあります。

---

## 🧩 インストール方法  

### ・VPMリポジトリからインストールする場合

 1. [このリンク](https://github.com/emuoh/vpm-repos/blob/main/README.md)のインストール方法からパッケージをインストールしてください。
 2.  /packages/com.emuoh.portablefirealarmsystem/Runtime にある
PortableFirealarmSystem.prefab (QUEST版は PortableFirealarmSystem_QUEST.prefab)  を
Hierarchyのアバター直下にドラッグアンドドロップしてください。
![enter image description here](https://github.com/emuoh/PortablFireAlarmSystem/blob/main/Install_Picture/VPM_Package_Install.png)

### ・ダウンロードした.zipファイルからインストールする場合

1. 解凍した.zipファイルの中のPortableFirealarmSystem.unitypackageファイルを
`.unitypackage` を `Assets` フォルダへドラッグ＆ドロップしてください。
![enter image description here](https://github.com/emuoh/PortablFireAlarmSystem/blob/main/Install_Picture/UnityPackage_Install_1.png)
Import確認画面が出ますので、Importを選択してください。
![enter image description here](https://github.com/emuoh/PortablFireAlarmSystem/blob/main/Install_Picture/UnityPackage_Install_2.png)

2. `PortableFirealarmSystem.prefab` `(QUEST版は PortableFirealarmSystem_QUEST.prefab)` をアバターの直下にドラッグアンドドロップしてください。
![enter image description here](https://github.com/emuoh/PortablFireAlarmSystem/blob/main/Install_Picture/UnityPackage_Install_3.png)
---

## 🧩位置の調整方法
Modular Avatarを使用していますので首のボーンに自動的に配置されますが、ズレがある場合は以下の方法で位置調整を行ってください。

1. `MA_BoneProxy_Neck` を選択後、矢印をドラッグしてベルトの位置を調整してください。
![enter image description here](https://github.com/emuoh/PortablFireAlarmSystem/blob/main/Install_Picture/Modify_Position.png)

2. `PB_COL_FAS_Belt` はベルトが身体を貫通しないようにするコライダーです。この位置を1.と同様に操作して、身体に沿わせるように調整してください。
![enter image description here](https://github.com/emuoh/PortablFireAlarmSystem/blob/main/Install_Picture/Modify_Colider_Position.png)

## 🧪 Quest向け注意点

- 吹き出し文字の表示に不具合のある場合は、以下の手順で透過なしのマテリアルに変更してください(透過が外れますので吹き出し文字の美観は損なわれます)。
 ![enter image description here](https://github.com/emuoh/PortablFireAlarmSystem/blob/main/Install_Picture/QUEST_Change_Shader.png)
- 導入するアバターが既にPhysBoneリソースを多く使用している場合はアップロードできない場合がありますので、不要なボーン等を削除してください。

---

## 🎮 操作方法

### ラジアルメニュー操作（PC/VR）

![enter image description here](https://github.com/emuoh/PortablFireAlarmSystem/blob/main/Install_Picture/RadialMenu.png)
![enter image description here](https://github.com/emuoh/PortablFireAlarmSystem/blob/main/Install_Picture/RadialMenu_2.png)

| ボタン名 | 機能 |
|----------|------|
| On | 報知器本体を表示します。 |
| Button On | 非常ボタンのON/OFFを切り替えます。 |
| Alarm Stop | 停止ボタンで警報を停止します。 |
| Cover Open | 停止ボタンカバーの開閉を行います。 |
| Onomatopeia On | 吹き出し文字のON/OFFを切り替えます。 |
| Sound On | 警報音のON/OFFを切り替えます（PCのみ）。 |
| Voice On | 音声のON/OFFを切り替えます（PCのみ。デフォルトはOFFです）。 |
| Body Size | 本体のサイズを調整します。 |
| Belt Spread | 首との開きを調整します。 |
| Belt Width | ベルトの幅を調整します。 |

### 手動操作（VR）

1. 人差し指で非常ボタンを押すと、警報がONになります。
2. カバーに触れると、開きます。
3. 停止ボタンを押すと、警報がOFFになります。
4. 再度カバーを触ると、閉じます。

---

## 🎁 おまけ音声

-  `Sound/Voice` フォルダに複数の警報音・音声バリエーションが含まれています。
- `FAS_Sound` や `FAS_Voice` の `AudioClip` を差し替えて使用してください。
![enter image description here](https://github.com/emuoh/PortablFireAlarmSystem/blob/main/Install_Picture/Change_Sound_Voice.png)
---
## 🔁 アップデート

- VPMパッケージからインストールした場合は、最新版が配布されると自動で通知されます。
- VCCからはアップデートしたいのプロジェクトの「Manage Project」から最新の「LatestVersion」を選択することで更新可能です。

- ALCOMからはアップデートしたいプロジェクトの「管理」から「最新のバージョン」を選択することで更新可能です。

- .zipファイルからインストールした場合は、最新版の自動通知はされません。ダウンロードしたサイト(Booth等)から最新版をダウンロードして再インストールしてください(詳細な手順はサイト上の説明もしくは.zipファイル内をご参照ください)。

---

## 👤 作者・連絡先

- 制作：emuoh(えむお～)([https://emuoh3.booth.pm/](https://emuoh3.booth.pm/))
- GitHub: [emuoh/PortablFireAlarmSystem: PortablFireAlarmSystem For VRChat Gimmick](https://github.com/emuoh/PortablFireAlarmSystem)
- X: emuoh3@x.com

---

## 📜 ライセンス

このギミックは [VN3ライセンス](https://www.vn3.org/index) に準拠しています。  
詳しくは  [LICENSE.md](https://github.com/emuoh/vpm-repos/blob/main/LICENSE.md) を参照してください。

## 🧷 クレジット

- テスト時使用アバター: [マヌカ](https://booth.pm/ja/items/5058077) (https://booth.pm/ja/items/5058077)
  

## 🔈 使用素材

- 警報音： [オトロジック](https://otologic.jp) 様
- 音声合成： VOICEVOX（四国めたん、ずんだもん、青山龍星）様を使用しています。

---

