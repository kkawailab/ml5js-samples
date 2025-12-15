# ml5.js サンプル集

ml5.jsを使った機械学習サンプル集です。初心者向けの簡単なものから上級者向けの複雑なものまで、30個のサンプルを収録しています。

すべてのサンプルは**HTMLファイル1枚で完結**しており、ブラウザで直接開いて動作します。

## 必要なもの

- モダンなウェブブラウザ（Chrome, Firefox, Edge, Safari）
- ウェブカメラ（多くのサンプルで使用）
- マイク（音声関連サンプルで使用）

## サンプル一覧

### 初心者向け（01-10）

| # | サンプル | 説明 |
|:-:|---------|------|
| 01 | [Image Classifier 基本](01_image_classifier_basic.html) | MobileNetを使った画像分類の最小サンプル |
| 02 | [Image Classifier + Webcam](02_image_classifier_webcam.html) | ウェブカメラ映像をリアルタイムで分類 |
| 03 | [BodyPose 基本](03_bodypose_basic.html) | 体のキーポイント17点を検出・表示 |
| 04 | [BodyPose スケルトン](04_bodypose_skeleton.html) | 骨格を線で繋いで表示 |
| 05 | [HandPose 基本](05_handpose_basic.html) | 手のキーポイント21点を検出 |
| 06 | [FaceMesh 基本](06_facemesh_basic.html) | 顔の478個のランドマークを検出 |
| 07 | [Sound Classifier 基本](07_sound_classifier_basic.html) | マイクの音声を分類 |
| 08 | [BodyPose スクワットカウンター](08_bodypose_counter.html) | スクワットの回数を自動カウント |
| 09 | [Image Classifier アップロード](09_image_classifier_upload.html) | 画像をアップロードして分類（上位5件表示） |
| 10 | [FaceMesh 絵文字オーバーレイ](10_facemesh_emoji.html) | 顔に絵文字を重ねて表示 |

### 中級者向け（11-20）

| # | サンプル | 説明 |
|:-:|---------|------|
| 11 | [BodyPose フルーツキャッチゲーム](11_bodypose_game.html) | 手を動かしてフルーツをキャッチするゲーム |
| 12 | [HandPose お絵かき](12_handpose_drawing.html) | 人差し指で空中に絵を描く |
| 13 | [FaceMesh フェイスフィルター](13_facemesh_filter.html) | サングラス・猫耳などのフィルター |
| 14 | [Neural Network 色分類](14_neural_network_classification.html) | RGBから色名を予測するNNを訓練 |
| 15 | [Neural Network 価格予測](15_neural_network_regression.html) | 面積・築年数から住宅価格を予測 |
| 16 | [BodyPose 体で音楽](16_bodypose_sound.html) | 手の位置で音程と音量を操作 |
| 17 | [HandPose ジェスチャー認識](17_handpose_gesture.html) | グー・チョキ・パー等のジェスチャーを認識 |
| 18 | [マルチモデル同時使用](18_multi_model.html) | BodyPose・HandPose・FaceMeshを同時実行 |
| 19 | [音声ビジュアライザー](19_sound_visualizer.html) | 音声分類＋円形ビジュアライザー |
| 20 | [Image Classifier カスタムUI](20_image_classifier_custom_ui.html) | リッチなUIの画像分類器 |

### 上級者向け（21-30）

| # | サンプル | 説明 |
|:-:|---------|------|
| 21 | [Neural Network ポーズ分類器](21_neural_network_pose_classifier.html) | 独自のポーズを訓練して認識 |
| 22 | [BodyPose フィットネストラッカー](22_bodypose_fitness_tracker.html) | 複数エクササイズの回数・カロリー計測 |
| 23 | [HandPose バーチャルキーボード](23_handpose_virtual_keyboard.html) | 空中でタイピング |
| 24 | [FaceMesh 頭の向き推定](24_facemesh_head_pose.html) | Yaw/Pitch/Rollを計算・3D表示 |
| 25 | [マルチパーソントラッキング](25_multi_person_tracking.html) | 複数人を同時に追跡・個別分析 |
| 26 | [Neural Network 時系列予測](26_neural_network_timeseries.html) | 過去データから未来の値を予測 |
| 27 | [ポーズマッチングゲーム](27_pose_matching_game.html) | お題のポーズを真似してスコアを競う |
| 28 | [HandPose 指文字認識](28_handpose_sign_language.html) | 手の形からアルファベットを認識 |
| 29 | [AI お絵かきアシスタント](29_ai_drawing_assistant.html) | 描いている途中でAIが何か予測 |
| 30 | [総合AIインタラクティブ体験](30_interactive_ai_experience.html) | 全モデル＋エフェクトの統合デモ |

## 使用技術

- [ml5.js](https://ml5js.org/) - 機械学習ライブラリ
- [TensorFlow.js](https://www.tensorflow.org/js) - ml5.jsのバックエンド

## 使い方

1. このリポジトリをクローン
   ```bash
   git clone https://github.com/kkawailab/ml5js-samples.git
   ```

2. HTMLファイルをブラウザで開く
   - ローカルサーバーを使用する場合：
     ```bash
     cd ml5js-samples
     npx serve .
     ```
   - または直接ファイルをブラウザにドラッグ＆ドロップ

3. カメラ・マイクへのアクセスを許可

## ライセンス

MIT License

## 更新履歴

| 日付 | バージョン | 内容 |
|:----:|:----------:|------|
| 2024-12-15 | v1.0.0 | 初回リリース - 30個のサンプルを公開 |
| 2024-12-15 | v1.0.1 | README.mdを追加 |
| 2024-12-15 | v1.0.2 | GitHub Pages用のindex.htmlを追加 |
| 2024-12-15 | v1.0.3 | リポジトリのAbout情報を更新 |
