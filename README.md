# 商用無料 Webフォント辞典 (Commercial Free Font Dictionary)

商用利用が無償で許可されたオープンソースフォント（SIL Open Font License 1.1 / Apache 2.0）に特化した、リアルタイム比較・タイポグラフィ検証Webツール。

**Google Fonts公式収録の日本語フォント全68書体を完全網羅**し、さらに**世界中でWeb制作に愛用される欧文定番54書体**を加えた、計**122書体**の商用フリーWebフォントカタログです。

---

## 主な特徴

- **商用利用100%フリー厳選**: Webサイト制作・商用出版・商用アプリ・動画サムネイル・ロゴ等で無償利用できるフォントのみを122書体収録。
- **Google Fonts 和文フォント完全網羅（全68書体）**: 王道ゴシックから文学的明朝、丸ゴシック、80年代丸文字、レトロゲームドット、筆文字、3Dブロックまで網羅。
- **世界基準の欧文フォント増強（全54書体）**: Inter, Roboto, Playfair Display, Cinzel, JetBrains Mono, Pacifico など、ジャンル別人気書体を厳選。
- **キャンパスノート調UIUX**: 限りなく白に近いニュアンスグレー（`#f8f9fa`）背景、ダークグレー（`#2b2d42`）文字、32px間隔の淡い水平罫線（`linear-gradient`）による紙面ライクな設計。
- **超高速オンデマンド遅延ロード**: Intersection Observer により、画面内にスクロール表示されたフォントのみを動的に取得。122書体を搭載しながら初期表示は一瞬で完了。
- **リアルタイムタイポグラフィ制御**:
  - テキスト自由入力 ＋ 例文プリセット（和文見出し・エッセイ長文・英数・コード・セールPOP）
  - フォントサイズ（12〜64px）、行間（1.0〜2.6）、字間（-0.02em〜0.15em）
  - 太字（B）、斜体（I）、下線（U）、打消線（S）
  - 文字色・背景色のリアルタイムピッカー
- **複数フォント並列比較（ピン留め）**: 各カード右上の「比較」チェックを入れ、「選択フォントだけ比較」を押すと、ピックアップした候補同士をじっくり見比べられます。
- **インクリメンタル検索 & フィルタ**: フォント名（日本語名・英語名）やおすすめ用途で瞬時に絞り込み。
- **実務用コード即時コピー**: 各フォントカードの「CSS」ボタンから、HTML `<link>` タグおよびMac/Windowsのフォールバック付き `font-family` CSSをワンクリックでコピー可能。

---

## 収録フォント内訳（全122書体）

### 日本語フォント（Google Fonts 全68書体）
- **ゴシック体**: Noto Sans JP, Zen Kaku Gothic New, Zen Kaku Gothic Antique, M PLUS 1, M PLUS 1p, M PLUS 2, M PLUS U, IBM Plex Sans JP, BIZ UDGothic, BIZ UDPGothic, LINE Seed JP, Kosugi, Sawarabi Gothic, Murecho など
- **明朝体**: Noto Serif JP, Shippori Mincho, Shippori Mincho B1, Zen Old Mincho, Kaisei Tokumin, Kaisei HarunoUmi, Kaisei Opti, Kaisei Decol, Hina Mincho, BIZ UDMincho, BIZ UDPMincho, Sawarabi Mincho など
- **丸ゴシック**: Zen Maru Gothic, M PLUS Rounded 1c, Kosugi Maru, Kiwi Maru, Tsukimi Rounded, Hachi Maru Pop, Mochiy Pop One, Mochiy Pop P One など
- **デザイン・手書き・個性派**: Klee One, Dela Gothic One, RocknRoll One, Reggae One, Train One, Rampart One, Rock 3D, DotGothic16, Yuji Boku, Yuji Mai, Yuji Syuku, Yuji Hentaigana, Potta One, Cherry Bomb One, Chokokutai, Darumadrop One, Yusei Magic, Yomogi, Shizuru, New Tegomin, Slackside One, Stick, Monomaniac One, Palette Mosaic, WDXL Lubrifont JP N など

### 欧文フォント（厳選 54書体）
- **サンセリフ**: Inter, Roboto, Open Sans, Lato, Montserrat, Poppins, Raleway, Nunito, Work Sans, Plus Jakarta Sans, DM Sans, Outfit, Figtree, Manrope, Space Grotesk, Syne, Ubuntu, Cabin
- **セリフ**: Playfair Display, Merriweather, Lora, Cormorant Garamond, EB Garamond, Cinzel, Cinzel Decorative, Bodoni Moda, Libre Baskerville, Spectral, Fraunces, Prata, DM Serif Display, Newsreader
- **等幅・コード**: JetBrains Mono, Fira Code, Source Code Pro, Space Mono, Roboto Mono, Inconsolata, IBM Plex Mono, Ubuntu Mono
- **ディスプレイ**: Oswald, Bebas Neue, Anton, Archivo Black, Righteous, Abril Fatface, Alfa Slab One
- **スクリプト・筆記体**: Great Vibes, Dancing Script, Pacifico, Caveat, Sacramento, Shadows Into Light, Parisienne

---

## Cloudflare Pages へのデプロイ方法

### 方法1: GitHub連携（推奨・自動更新）
1. [Cloudflare ダッシュボード](https://dash.cloudflare.com/) に入る。
2. 左メニュー「**Workers & Pages**」→「**Create application**」→「**Pages**」タブを開く。
3. 「**Connect to Git**」を選択し、リポジトリ `netch-git/commercial-font-dictionary` を選択。
4. 設定は初期値（ビルドコマンドなし、ビルド出力ディレクトリは空欄）のまま「**Save and Deploy**」をクリック。
5. 以後、GitHubにプッシュするだけで自動的に全世界へCDN配信されます。

### 方法2: Direct Upload（ドラッグ＆ドロップ）
1. 本リポジトリのZIPファイル（`commercial_font_dictionary.zip`）を使用。
2. Cloudflare ダッシュボード → **Workers & Pages** → **Create application** → **Pages** → **Upload assets** を選択。
3. ZIPファイルをドラッグ＆ドロップするだけで即座に公開完了。

---

## ライセンス
各フォントの著作権は各ファウンダリ・制作者に帰属します（SIL Open Font License 1.1 または Apache 2.0）。
Webアプリケーション自体のコードは MIT License です。
