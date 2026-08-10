# READ ALOUD LAB

大学受験のやさしめレベルをベースにした、英語音読用の静的Webサイトです。

## 収録内容
- 10本の英文（大人にも学びがあるテーマ）
- リーディング問題
- 内容解説
- 重要文法
- 構文解説
- 日本語訳
- 単語リスト
- ブラウザ標準の英語音声による読み上げ
- 音声速度・英語音声の選択

## ファイル
- `index.html` — Lesson一覧
- `lesson.html` — Lesson詳細
- `data.json` — 教材データ
- `style.css` — デザイン

## GitHub Pagesへの公開
1. GitHubで新しいRepositoryを作る（例: `read-aloud-lab`）
2. このフォルダのファイルをRepositoryへアップロード
3. Repository → Settings → Pages
4. Build and deployment の Source を GitHub Actions にする、または利用可能ならブランチ公開を選ぶ
5. 公開されたURLを開く

このサイトはビルド不要のHTML/CSS/JavaScriptだけで動きます。

## 音声について
現在は `SpeechSynthesis API` を使っています。端末・ブラウザに入っている英語音声を利用するため、英語音声の品質や声の種類は環境によって変わります。

より「教材として完成度の高いネイティブ音声」にする場合は、各LessonのMP3を `audio/01.mp3` のように配置し、`lesson.html` の音声部分を `<audio controls>` に置き換える構成がおすすめです。
