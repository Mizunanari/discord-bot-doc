# Visual Studio Code のインストールと設定

下記のURLからダウンロードもできますが、できればパッケージマネージャーを使用する方法をお勧めします。

vscordと拡張機能がいくつか必要になります。全てインストールしてください。

[Visual Studio Code - Code Editing. Redefined](https://code.visualstudio.com/)

[Japanese Language Pack for Visual Studio Code - Visual Studio Marketplace](https://marketplace.visualstudio.com/items?itemName=MS-CEINTL.vscode-language-pack-ja)

[GitHub Codespaces - Visual Studio Marketplace](https://marketplace.visualstudio.com/items?itemName=GitHub.codespaces)

## パッケージマネージャーを使用してインストール（中級者向け）

パッケージマネージャを利用してインストールするとコマンドによって環境が構築できるため、管理が楽になります。windowsとmacの方法を紹介します。

### windows

※ 未検証(windowsの方、試してokだったら教えてください。)

公式パッケージマネージャー[winget](https://docs.microsoft.com/ja-jp/windows/package-manager/)を使用します。wingetは最新のwindowsであれば、インストール済みです。
ターミナルを使用しますので、[Windows Terminal](https://apps.microsoft.com/store/detail/windows-terminal/9N0DX20HK701?hl=ja-jp&gl=JP)をインストールしてください。こちらはバンドルされていませんが、公式から出ているターミナルソフトで、コマンドプロンプトより便利です。

__vscordのインストール__

ターミナルにコマンドを入力します。

```powershell
winget install -q vscode
```

__拡張機能のインストール__

ターミナルにコマンドを入力します。

```powershell
code --install-extension MS-CEINTL.vscode-language-pack-ja
code --install-extension GitHub.codespaces
```

### mac

[Homebrew](https://brew.sh/index_ja)がインストールされていることが条件。

__vscordのインストール__

```zsh
brew install --cask visual-studio-code
```

__ターミナルで`code`コマンドが使用できることを確認する__

ターミナル上で`code --version`を打ちこんで動作する場合はこの項目を飛ばしてください。

```zsh
% code --version
1.68.1
30d9c6cd9483b2cc586687151bcbcd635f373630
arm64
```

使用できない場合は、[codeのインストール](https://code.visualstudio.com/docs/setup/mac#_launching-from-the-command-line)を行います。  
vscordで`cmd + shift + P`でコマンドパレットを開き、`>shell command`と入力します。候補の`install 'code' command in PATH`を選択します。

![image](https://code.visualstudio.com/assets/docs/setup/mac/shell-command.png)

ターミナルで`code --version`と打ち込み、バージョンなどが表示されたら完了です。

__拡張機能のインストール__

```zsh
code --install-extension MS-CEINTL.vscode-language-pack-ja
code --install-extension GitHub.codespaces
```

[home](/index.md)   [next](/create-discord-bot.md)