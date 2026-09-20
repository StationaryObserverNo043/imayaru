# イマヤル（タスク完了アプリ）

やることを決めてタイマーをスタート → 画面が真っ暗になり、終わるまで止められない・タッチもできないPWA。

## 公開手順（GitHub Pages）
1. このフォルダの中身をそのままGitHubリポジトリ（例: `imayaru`）にpush
2. Settings → Pages → Branch: `main` / `/ (root)` を選んで保存
3. `https://ユーザー名.github.io/imayaru/` で公開される

## 公開後に書き換える場所（index.html）
- `og:url` / `og:image` / `twitter:image` の `https://YOUR-NAME.github.io/imayaru/` → 実際のURL

## 画像の使いどころ
| ファイル | 用途 |
|---|---|
| assets/img/title.webp | タイトル画面（縦長） |
| assets/img/ogp.png (1200×630) | X・LINE・Facebook等の共有カード |
| assets/img/ghost.webp | 励まし・完了画面（正方形） |
| assets/img/story-1.webp | ものがたり冒頭の画像（ふとんの中でスマホを見る手） |
| assets/img/story.webp | ものがたり中盤の画像（スマホにオバケが現れる） |
| icons/icon-192/512.png | PWAアイコン（丸・透過） |
| icons/maskable-*.png | Android用マスカブルアイコン |
| icons/apple-touch-icon.png | iOSホーム画面アイコン |
| icons/icon-1024.png | SNSプロフィール等の丸アイコン |
| favicon.ico, icons/favicon-*.png | ブラウザのタブ |

## 更新するとき
`sw.js` の `CACHE = 'imayaru-v24'` の番号を上げると、利用者側のキャッシュが入れ替わります。
