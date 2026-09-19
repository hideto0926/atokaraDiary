# あとから旅日記 — Website

あとから旅日記（Atokara Travel Diary）の公開ページ。日英切り替え（EN/JA）、ビルド不要の静的ページ。

- `index.html` — 紹介ページ（特長・プライバシーの要点・よくある質問・お問い合わせ）。App Store の「サポートURL」にもこのページを使う
- `privacy.html` — プライバシーポリシー（App Store の「プライバシーポリシーURL」）
- `assets/icon.png` — アプリアイコン、`assets/shots/` — スクリーンショット
- `.nojekyll` — GitHub Pages でそのまま配信する

## 公開（GitHub Pages）
1. このフォルダの中身を `atokaraDiary` リポジトリ（https://github.com/hideto0926/atokaraDiary ）のルートに push する
2. リポジトリ → Settings → Pages → Source: *Deploy from a branch*、branch = default、folder = `/ (root)`
3. 1分ほど待って https://hideto0926.github.io/atokaraDiary/ を開く
4. アプリ一覧ページ（`homepageRoot` = hpTop）にカードを追加する（`badge soon`、アイコンは `assets/icon.png`）

## 公開前にやること
- **スクリーンショットは仮**。シミュレータの試験用の写真（単色の絵）で撮ったもの。実機の写真で撮り直して `assets/shots/` を差し替える
- App Store の URL が決まったら、`index.html` の App Store ボタンの `href="#"` と「近日公開」表記を差し替える
- プライバシーポリシーの内容はアプリの実装（2026-09-19 時点）に合わせてある。外部への送信を増やしたら更新する
  - 送っているのは、旅行の代表地点の座標だけ（Apple の地図サービスへ、市区町村名とタイムゾーンを調べるため）
