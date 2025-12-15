# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

ml5.js サンプル集 - 30個の機械学習デモ（初心者〜上級者向け）。すべてのサンプルは**単一HTMLファイルで完結**し、ビルドツール不要でブラウザで直接動作する。

## Development Commands

```bash
# ローカルサーバー起動（カメラ/マイク使用サンプルに必要）
npx serve .

# または
python -m http.server 8000
```

## Architecture

### File Structure
- `XX_name.html` - 番号付きサンプルファイル（01-30）
- `index.html` - GitHub Pages用ランディングページ
- 外部依存: `https://unpkg.com/ml5@1/dist/ml5.min.js` をCDNから読み込み

### Sample Categories
- **01-10**: 初心者向け - 各ml5.jsモデルの基本的な使い方
- **11-20**: 中級者向け - 複数機能の組み合わせ、ゲーム、Neural Network訓練
- **21-30**: 上級者向け - カスタムモデル訓練、マルチトラッキング、複合システム

### ml5.js Models Used
- `ml5.imageClassifier('MobileNet')` - 画像分類
- `ml5.bodyPose('MoveNet')` - 体のポーズ検出（17キーポイント）
- `ml5.handPose()` - 手の検出（21キーポイント）
- `ml5.faceMesh()` - 顔のランドマーク検出（478ポイント）
- `ml5.soundClassifier('SpeechCommands18w')` - 音声分類
- `ml5.neuralNetwork()` - カスタムニューラルネットワーク

### Common Patterns
各HTMLファイルは以下の構造:
1. ml5.js CDN読み込み
2. `<style>` タグ内にCSS
3. HTML要素（canvas, video, UI）
4. `<script>` タグ内に全ロジック
5. `async/await` でモデル初期化・推論
6. ウェブカメラは左右反転（`ctx.scale(-1, 1)`）で描画

## GitHub Pages
https://kkawailab.github.io/ml5js-samples/ で公開
