
# 🔥 Portable Fire Alert System - 使用説明書

首にかけて携帯できる、軽量な火災報知器ギミックです。  
VRChatアバターに組み込むことができ、PCとQuestの両方に対応しており、PhysBoneにも対応しています。

---

## 📦 同梱内容

| ファイル名 | 説明 |
|------------|------|
| `PortableFireAlartSystem.zip` | 一式圧縮ファイルです。 |
| `PortableFireAlartSystem.unitypackage` | 本体のUnityパッケージです。 |
| `PortableFireAlartSystem.prefab` | PC向けPrefab（音声あり）です。 |
| `PortableFireAlartSystem_Quest.prefab` | Quest向けPrefab（音声なし）です。 |
| `readme.txt` | この説明書です。 |

---

## 💡 概要

- 音と吹き出し文字で警報を出します（PC）。吹き出し文字のみ（Quest）にも対応しています。
- ボタンとカバーによる停止動作があります。
- LED点滅、軽量構造で、PhysBoneによる自然な装着感があります。
- メニュー操作と手動操作の2方式に対応しており、デスクトップ・VRの両方で利用可能です。

---

## 🛠 対応環境

- Unity：2022.3.22f1 を使用しています。
- Shader：Standard Lite / Multiply（SDK標準）です。
- 必須アセット：
  - Modular Avatar v1.13.0 以上が必要です。
  - AtlasTexture v1.8.12 以上が必要です。

---

## 📐 スペック（PC/Quest）

| 項目 | 値 |
|------|----|
| Polygon Count | 2284 |
| Skinned Meshes | 1 |
| Materials | 2 |
| Textures | 2 |
| Bones | 8 |
| PhysBones | 1 |
| Physbone Colliders | 1 |
| Contact | 2 |
| Audio Source | 2（※PCのみ） |

---

## 🧩 導入方法

1. `.unitypackage` を `Assets` フォルダへドラッグ＆ドロップしてください。
2. `Prefab` をアバターの直下に配置してください（Questは `_Quest` を使用します）。
3. `MA_BoneProxy_Neck` の位置とサイズを首に合うよう調整してください。
4. `PB_COL_FAS_Belt` の位置も身体に沿わせるように調整してください。

---

## 🧪 Quest向け注意点

- Multiply Shader が透明にならない場合は、透過なしマテリアルに変更してください。
- PhysBoneが多すぎるとアップロードできない場合がありますので、ご注意ください。

---

## 🎮 操作方法

### メニュー操作（PC/VR）

| ボタン名 | 機能 |
|----------|------|
| On | 警報器を表示します。 |
| Button On | 非常ボタンのON/OFFを切り替えます。 |
| Alarm Stop | 停止ボタンで警報を停止します。 |
| Cover Open | 停止ボタンカバーの開閉を行います。 |
| Onomatopeia On | 吹き出し文字のON/OFFを切り替えます。 |
| Sound On | 警報音のON/OFFを切り替えます（PCのみ）。 |
| Voice On | 音声のON/OFFを切り替えます（デフォルトはOFFです）。 |
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

- フォルダ内 `Sound/Voice` に複数の音声バリエーションが含まれています。
- `FAS_Sound` や `FAS_Voice` の `AudioClip` を差し替えて使用することができます。

---

## 🔈 使用素材

- 効果音： [オトロジック](https://otologic.jp) 様
- 音声合成： VOICEVOX（四国めたん、ずんだもん、青山龍星）様を使用しています。

---

## 📜 ライセンス

このギミックは [VN3ライセンス](https://vn3.dev) に準拠しています。  
詳しくは `LICENSE.md` をご確認ください。
