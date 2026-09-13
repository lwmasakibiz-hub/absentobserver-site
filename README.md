# 観測者不在 Webサイト

absentobserver.com の開発用コピーです。

## ファイル

- `public/index.html`：公開するページ。CSSとロゴ画像を含みます。
- `netlify.toml`：Netlifyの公開フォルダを `public` に指定します。

## ローカル確認

Python導入後、このフォルダで `python -m http.server 8080 --bind 127.0.0.1 --directory public` を実行し、ブラウザで `http://127.0.0.1:8080` を開きます。

メール登録部分はBenchmark Emailの外部サービスです。表示確認時にテスト登録は送信しません。

## GitHub・Netlify連携

1. GitHubの保存先リポジトリと、コミットに使う名前・メールアドレスを確認します。
2. このフォルダをGitHubへアップロードします。
3. 現在のNetlifyサイトに、そのリポジトリの `main` ブランチを接続します。
4. ビルドコマンドは空欄、公開フォルダは `public` とします。
5. プレビューを確認してから本番の自動公開を検証します。

DNSやドメインの移転は不要です。現在のNetlifyサイトとの接続は未実施です。

## 元データの確認

2026-09-13、Downloadsの `absentobserver_site(1).zip` 内のHTMLと公開サイトを比較しました。差分は公開ページ末尾のNetlify HUDスクリプトのみでした。元ZIPと公開サイトは変更していません。
