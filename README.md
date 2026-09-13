# 観測者不在 Webサイト

[absentobserver.com](https://absentobserver.com/) のソースです。GitHubの `main` ブランチをNetlifyへ接続しています。

## ファイル

- `public/index.html`：公開ページ。CSSとロゴ画像を含みます。
- `netlify.toml`：公開フォルダ `public` を指定します。ビルドコマンドは不要です。

## ローカル確認

Pythonが使える環境で、このフォルダから次を実行します。

```text
python -m http.server 8080 --bind 127.0.0.1 --directory public
```

ブラウザで http://127.0.0.1:8080 を開きます。終了はCtrl+Cです。

メール登録部分はBenchmark Emailの外部サービスです。表示確認だけなら登録を送信する必要はありません。

## 更新と公開

1. `public/index.html` を編集し、PC上で表示を確認します。
2. 変更をコミットし、GitHubの `main` へ反映します。
3. Netlifyが自動デプロイします。管理画面でPublishedを確認し、公開ページの表示を確認します。

公開元：https://github.com/lwmasakibiz-hub/absentobserver-site

デプロイ履歴：https://app.netlify.com/projects/absentobserver/deploys

## 移行記録

2026-09-13、元ZIPと公開HTMLを比較し、Netlifyの追加スクリプト以外は一致することを確認しました。既存のNetlifyプロジェクトへGitHubを接続し、同じドメインでの公開を確認しました。
