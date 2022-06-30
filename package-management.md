# Pythonパッケージの管理

テンプレートプロジェクトでは、pythonパッケージの管理に`pip`ではなく、[Poetry](https://python-poetry.org/)を使用しています。これを簡単に説明するとpipを拡張したものです。

pipとはコマンドが少しずつ違うので、注意してください。

4つほどコマンドの例を挙げます。ここにないコマンドは下記のurlが参考になります。

[コマンド - Poetry documentation (ver. 1.1.6 日本語訳)](https://cocoatomo.github.io/poetry-ja/cli/)

## パッケージのインストール

pipの場合は`install`ですが、poetryだと`add`を使用します。

```bash
# pipの場合
pip install requests

# poetryの場合
poetry add requests
```

なお、poetryでは開発に使用するパッケージを別管理することができます。

```bash
# 開発のみで使用するパッケージの場合
poetry add -D black
```

## パッケージのアンインストール

`uninstall`ではなく`remove`になります。

```bash
# pipの場合
pip uninstall requests

# poetryの場合
poetry remove requests
```

poetryでは、開発パッケージが別管理されています。`remove`でも`-D`が使用できます。

```bash
# 開発のみで使用するパッケージの場合
poetry remove -D black
```

## パッケージの一覧表示

`list`ではなく、`show`になります。

```bash
# pipの場合
pip list

# poetryの場合
poetry show
```

## パッケージの一括書き出しと一括インストール

poetryでは、管理が簡単になります。

### pipの場合

```bash
# パッケージの書き出し
pip freeze > requirements.txt

# 一括インストール
pip install -f requirements.txt
```

### poetryの場合

```bash
# パッケージの書き出し
# なし

# 一括インストール
poetry install
```

以上です。

[home](/index.md)