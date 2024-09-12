# インクルーシブなペルソナ拡張

## 視覚障害 (全盲)

### ウェブ利用時の障壁

* 目が見えない。視覚的な情報が理解できない。
* スクリーンリーダーによる音声読み上げ (または点字出力) がないと利用できない。
* 自由にポインティング (マウスでのクリックや指でのタップ) をすることができない。

### 解決方法

* 画像やアイコンに対して、代替テキストを提供する。
* 映像コンテンツに対して、代替コンテンツ (音声解説など) を提供する。
* 文字情報は画像ではなくテキストで作る。
* 見出し構造やランドマークを適切にマークアップする。
* キーボード操作だけですべての機能を利用できるようにする。
* リンクやボタンのラベルを具体的に記述する。
* フォームの入力要素にはラベル (label 要素) を付ける。
* テーブル (表) はシンプルな構造にし、見出しセルを th 要素にする。
* インタラクションに伴う動的な状況の変化がスクリーンリーダーでも伝わるようにする (WAI-ARIA)。
* ページの読み込みと同時に音声コンテンツを自動再生させない

## 視覚障害 (ロービジョン)

### ウェブ利用時の障壁

* 目が見えにくい。
    - 明瞭に見えない (ぼやける、重なる)。
    - まぶしい。
    - ちらつく。
    - 視野を広く見ることができない。
    - 視野の中心が欠ける。
    - 焦点が定まらない (震える)。
* 見えにくさによっては、スクリーンリーダーによる音声読み上げに頼ることもある。

### 解決方法

* ズーム (画面表示の拡大) を妨げない。
* 文字情報は画像ではなくテキストで作る。
* 文字色と背景色のコントラストを十分に保つ。
* キーボード操作によるフォーカス位置を視認できるようにする。
* ユーザーエージェントの機能で色を反転表示しても、情報が伝わるようにする。
* ユーザーが独自のスタイルシートを使うことを妨げない。
* 情報のチャンク (塊やつながり) に配慮してレイアウトする。
* ユーザーインターフェースの慣例 (おなじみのパターン) に従う。
* 偶発的なトリガー (マウスオーバーやキーボードフォーカス) でコンテンツを変更しない。
* 音声読み上げ順と視覚的なレイアウトを合致させる。

## 色覚特性 / グレースケール印刷

### ウェブ利用時の障壁

* 色が識別しにくい。
    - P型 (赤の視感度がないか低い)
    - D型 (緑の視感度がないか低い)
    - T型 (青の視感度がないか低い)
    - A型 (色の識別ができず明暗でしか判別できない)
* ウェブページをグレースケールで印刷する場合、情報識別を色に依存しているコンテンツだと判別できない。
* モノクロの電子書籍リーダーで (電子書籍からのリンクなどで) ウェブページを開く場合、情報識別を色に依存しているコンテンツだと判別できない。

### 解決方法

* 色だけで情報を識別させない。
    - リンク (特に文中のリンク) には下線を付ける。
    - 文字の大きさや太さなど、色以外の要素を用いてテキストのビジュアルヒエラルキー (視覚的な優􏰀度) を表現する。
    - 図 (グラフなど) においては、色以外の形状も、視覚的な判別の手がかりとして付ける。
* グレースケール表示でもコンテンツを理解/利用できるようにする。

## 聴覚障害 / 公共の場

### ウェブ利用時の障壁

* 音が聞こえない、または聞こえにくい。
* 公共の場 (交通機関、図書館、など) にいて、音を出せない (Bluetooth イヤホンのバッテリー切れ、イヤホン忘れ、といった状況も含む)。

### 解決方法

* 音声コンテンツに対して、トランスクリプト (書き起こし文) を併せて提供する。
* 音声付き動画コンテンツに対して、キャプション (字幕) を併せて提供する。

## 運動障害

### ウェブ利用時の障壁

* 自由にポインティング (マウスでのクリックや指でのタップ) ができない。以下の手段に頼る必要がある。
    - PC キーボード
    - マウススティック
    - 各種スイッチ (ボタン)
    - 音声認識ソフト
    - 視線入力装置
    - ...etc.
* デバイスの向きを自由に変えることが難しい。

### 解決方法

* キーボード操作だけですべての機能を利用できるようにする。
* キーボード操作によるフォーカス位置を視認できるようにする。
* リンクやボタンなどは、精緻なポインティング操作ができなくてもクリック / タップ / 実行できるよう、十分な大きさにする。
* 音声入力の支援として、リンクやボタンのラベルを具体的に記述する。テキストで記述し、適切にマークアップする。
* デバイスの向きが「ポートレート (縦)」「ランドスケープ (横)」どちらでも問題なく利用できるようにする。

## 認知 / 学習障害

### ウェブ利用時の障壁

* 情報を認知したり記憶することが難しい。
* 外的な刺激によって集中が妨げられる。
* 文字を読むのが難しい。(ディスレクシアなど)

### 解決方法

* ユーザーインターフェースの慣例 (おなじみのパターン) に従う。
* コンテンツはなるべく平易な言葉で表現する。
* 見出しを提示してコンテンツの概要をつかみやすくする。
* 読まなくても理解できるよう、視覚表現 (画像、図、アイコン、シンボルなど) を適宜用いる。
* コンテンツに時間制限がある場合、ユーザーが任意で解除または調整できるようにする。
* コンテンツ内の動きや点滅は、5秒以内にとどめるか、ユーザーが任意で停止できるようにする。
* コンテンツ表現において、1秒に3回以上の閃􏰁は用いない。
* ページの読み込みと同時に動画および音声コンテンツを自動再生させない。
* 視認性のよいフォントを用いる。
* 文字サイズや行間を十分な大きさにして、可読性を高くする。
* 複数のコンタクト手段を提供する。(例 : 電話+テキストチャット)

## 加齢

### ウェブ利用時の障壁

* 精緻なポインティング (マウスでのクリックや指でのタップ) が難しい。
* 小さな文字や薄い文字が見にくい。(老眼)
* 耳が遠い。
* 情報を認知したり記憶することが難しい。

### 解決方法

* リンクやボタンなどは、精緻なポインティング操作でなくてもクリック / タップ / 実行できるよう、十分な大きさにする。
* 文字色と背景色のコントラストを十分に保つ。
* 文字情報は画像ではなくテキストで作る。
* 文字サイズや行間を十分な大きさにして、可読性を高くする。
* ユーザーインターフェースの慣例 (おなじみのパターン) に従う。
* 見出しを提示してコンテンツの概要をつかみやすくする。

## モバイル

### ウェブ利用時の障壁

* 画面が小さく、情報を得るための視野が狭い。
* 文字が小さくなりがちで、読みにくい。
* 屋外で使用する場合、自然􏰁のまぶしさでコンテンツが見にくい。
* 指でタップするので、マウスに比べて精緻なポインティングが難しい。
* ハードウェアのキーボードに比べて文字のタイピングが面倒。
* マウスを前提としたインタラクション (マウスオーバーなど) を利用できない。

### 解決方法

* ユーザー体験の観点からコンテンツの優􏰀順位を明確にし、伝えたいことを上位に提示する。
* 文字サイズや行間を十分な大きさにして、可読性を高くする。
* ズーム (画面表示の拡大) を妨げない。
* 文字色と背景色のコントラストを十分に保つ。
* リンクやボタンなどは、精緻なポインティング操作でなくてもタップできるよう、十分な大きさにする。
* 文字入力 (タイピング) の発生をなるべく少なくする。
* マウスオーバー (hover) 依存のインタラクションを実装しない。