# 🖐️ The Hand - 3D Hand Model & Animations

Blenderで作成した手の3Dモデルにボーン（リギング）を組み込み、自然なアニメーションを設定したプロジェクトです。  
スマートフォンやPCのブラウザ上で360度インタラクティブに操作できる3D Webビューワーも搭載しています。

![Preview](preview.png)

---

## 🌐 3D Webビューワー（スマホ・PC対応）

ブラウザ上で3Dモデルをグリグリ動かしたり、ボタンを押してアニメーションを切り替えて楽しめます！

👉 **[Webビューワーを動かす (GitHub Pages)](https://kam2525-hub.github.io/the-hand-3d/)**

### 🎮 操作方法
* **スワイプ / ドラッグ**: 視点を360度回転
* **ピンチイン / ピンチアウト (ホイール)**: ズームイン / ズームアウト
* **アニメーションボタン**:
  * ✊ **グー**: 力強く握り込む
  * ✌️ **ピース**: 人差し指と中指を立ててVサイン
  * 👍 **いいね**: 親指を立てるサムズアップ
  * 👋 **バイバイ**: しなやかに手を振る
  * ✋ **パー**: 開いた状態（静止）
  * ▶️ **メドレー連続再生**: すべてのアニメーションをスムーズに連続再生

---

## 📁 収録ファイル

| ファイル名 | 説明 |
| :--- | :--- |
| [`index.html`](index.html) | Three.jsで構築されたスマホ対応の3Dインタラクティブビューワー（GLBモデル内蔵・オフライン動作可能） |
| [`The_Hand_Animated.glb`](The_Hand_Animated.glb) | ボーン・ウェイト・全アニメーションがベイクされたglTF/GLBバイナリモデル（AR対応） |
| [`The_Hand_Animated.blend`](The_Hand_Animated.blend) | Blender 4.5 作業用ファイル（Armatureリグ、サブディビジョン、アニメーションActionデータ完備） |
| [`The_Hand_Animation.mp4`](The_Hand_Animation.mp4) | スマートフォン縦型画面（1080×1920, 30fps）でスタジオレンダリングしたデモ動画 |

---

## 🛠️ 技術スタック
* **3D Modeling & Rigging**: Blender 4.5 LTS (Python API `bpy` によるプロシージャルリギング・自動ウェイト・キーフレーム制御)
* **Render Engine**: Blender EEVEE Next (3-Point Studio Lighting, Subsurface Scattering Skin Shader)
* **Web 3D Viewer**: Three.js, OrbitControls, GLTFLoader
