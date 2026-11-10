# 商用無料 Webフォント辞典 (Commercial Free Font Dictionary)

商用利用が無償で許可されたオープンソースフォント（SIL Open Font License 1.1 / Apache 2.0）のみを厳選収録した、リアルタイム比較・タイポグラフィ検証Webツール。

任意のテキストを打ち込むと、収録書体で瞬時にプレビューされ、太字・文字色・背景色・下線・文字サイズ・行間の調整や、複数フォントの並列比較が可能です。

---

## 特徴

- **商用利用100%フリー厳選**: Webサイト制作・商用出版・商用アプリ・ロゴ等で安心して無償利用できるフォントのみを25書体収録。
- **キャンパスノート調UIUX**: 限りなく白に近いニュアンスグレー（`#f8f9fa`）背景、ダークグレー（`#2b2d42`）の基準文字色、淡い水平罫線（32pxピッチ）による紙面ライクな設計。
- **リアルタイム装飾検証**: テキスト入力、文字サイズ（14〜64px）、行間（1.0〜2.6）、字間、太字、斜体、下線、打消線、文字色、背景色を即座に変更可能。
- **複数フォント選択比較**: 各カードの「比較」チェックを入れると、ピックアップした候補フォントだけを並べて比較（ピン留め比較）。
- **コピペで使える実務コード**: 各フォントカードの「CSS」ボタンから、HTML `<link>` タグおよびMac/Windowsのフォールバック付き `font-family` CSSをワンクリックでコピー。

---

## 収録フォント（全25書体）

### ゴシック体（可読性・本文向け）
- Noto Sans JP
- Zen Kaku Gothic New
- M PLUS 1p
- IBM Plex Sans JP
- BIZ UDPGothic

### 明朝体（格式・高級感・見出し向け）
- Noto Serif JP
- Shippori Mincho（しっぽり明朝）
- Zen Old Mincho
- Kaisei Tokumin（解星 特民）
- BIZ UDPMincho

### 丸ゴシック（親しみ・やわらかさ）
- Zen Maru Gothic
- M PLUS Rounded 1c
- Kosugi Maru
- Kiwi Maru

### デザイン・手書き・個性派
- Dela Gothic One（超極太）
- RocknRoll One（躍動感ポップ）
- Reggae One（シャープ・ストリート）
- Yuji Boku（本格毛筆・墨痕）
- DotGothic16（16pxピクセルレトロゲーム）
- Potta One（ふっくら手書き風）

### 欧文・コード（英数字併用・テック向け）
- Inter（現代UIの最高水準）
- Montserrat（幾何学・都市的）
- Playfair Display（優雅なクラシックセリフ）
- Cinzel（古代ローマ碑文調）
- JetBrains Mono（プログラミング等幅）

---

## Cloudflare Pages へのデプロイ方法

### 方法1: GitHub連携（推奨・自動更新）
1. [Cloudflare ダッシュボード](https://dash.cloudflare.com/) にログイン。
2. 左メニュー「**Workers & Pages**」→「**Create application**」→「**Pages**」タブを開く。
3. 「**Connect to Git**」を選択し、リポジトリ `netch-git/commercial-font-dictionary` を選択。
4. 設定（ビルドコマンドなし、ビルド出力ディレクトリは空欄または `/`）のまま「**Save and Deploy**」をクリック。
5. 以降、リポジトリに push すると自動で全世界へCDN配信されます。

### 方法2: Direct Upload（ドラッグ＆ドロップ）
1. 本リポジトリの `index.html` と `_headers` が入ったフォルダをZIP圧縮。
2. Cloudflare ダッシュボード → **Workers & Pages** → **Create application** → **Pages** → **Upload assets** を選択。
3. プロジェクト名を入力し、ZIPファイルをアップロードして完了。

---

## ライセンス
各フォントの著作権は各ファウンダリ・制作者に帰属します（SIL Open Font License 1.1 または Apache 2.0）。
Webアプリケーション自体のコードは MIT License です。
