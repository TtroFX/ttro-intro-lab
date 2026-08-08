# Ttro Intro Engine - GitHub Pages

GitHub repository root にこのファイル一式をそのまま置いてください。フォルダ分けは不要です。

## PDF
- `book.pdf` - 日英統合 154ページ
  - PDF 1〜77ページ: 日本語
  - PDF 78〜154ページ: English
  - JP p.n と EN p.n は 77ページ差で対応
- `book.pdf` は約20MBで、25MB未満です。

WebのPDF画面では、絶対ページ番号 1〜154 から言語を自動判定します。
例: PDF p.25 = JP p.25 / PDF p.102 = EN p.25。JP/ENボタンを押すと同じ論理ページの対応位置へ移動します。

## GitHub Pages
Settings -> Pages -> Deploy from a branch -> `main` / `(root)` を選択してください。

## 構成
すべてリポジトリ直下です。

`index.html`, `styles.css`, `app.js`, `content.js`, `labs.js`, `sw.js`, `manifest.webmanifest`, `icon.svg`, `.nojekyll`, `README.md`, `book.pdf`

PDFはService Workerのキャッシュ対象外にしているため、初回アクセス時にサイト本体のPWAキャッシュを不必要に重くしません。


## Recent update
- Added a top-level Lab tab.
- Replaced the old spline lab with an N-degree Bézier / de Casteljau lab.
- Labs now start in Auto Play mode with an ON/OFF switch.
