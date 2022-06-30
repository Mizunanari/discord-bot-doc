# botの作成

[Discord Developer Portal](https://discord.com/developers/applications)にて、botの登録を行います。

## 必要なもの

- discordアカウント

##　手順

1. [Discord Developer Portal](https://discord.com/developers/applications)にアクセス

右上のNew Applicationを選択します。

![image](https://discordpy.readthedocs.io/ja/latest/_images/discord_create_app_button.png)

2. botの名前を入力します。

![image](https://discordpy.readthedocs.io/ja/latest/_images/discord_create_app_form.png)

3. アイコンを設定します。

素材配布サイトです。必須設定項目ではありませんが、今回は必ず設定してください。

[Google Fonts](https://fonts.google.com/icons)

[Unsplash](https://unsplash.com/)

[ICOOON MONO](https://icooon-mono.com/)

アイコンの設定が終わったら、`Save Changes`を選択してください。

![image](/image/discordpy-doc-10.png)

1. Botを追加する

左のメニューからBotを選択。

Add Botを選択

![image](/image/discordpy-doc-2.png)

yes, do it!

![image](/image/discordpy-doc-3.png)

5. トークンを発行する

Reset Tokenを選択します。２回目以降は、現在のトークンが無効になります。

![image](image/discordpy-doc-4.png)

yes, do it!

![image](image/discordpy-doc-5.png)

トークンをコピーしてメモ帳などに控えます。コピーできるのはここだけなので、かならずコピーしておきましょう。

![image](image/discordpy-doc-6.png)

6. Intentsの設定

Intentsの設定を有効にします。設定を変更したら、`Save Changes`を押します。

![image](image/discordpy-doc-7.png)

7. botの権限設定

`OAuth2` > `URL Generatorから`　`bot`と`Send Messages`にチェックを入れ、生成されたURLにアクセスします。

![image](image/discordpy-doc-1.png)


botをインストールするサーバーの選択画面が表示されます。

![image](image/discordpy-doc-8.png)

権限を確認し、認証します。

![image](image/discordpy-doc-9.png)

サーバーにbotが入ったことを確認してください。

[home](index.md)    [next](/create-repo.md)
