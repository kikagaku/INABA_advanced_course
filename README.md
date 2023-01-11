# Sphinx Templates

## テンプレートの使い方
1. New Repository 作成時に Repository template で sphinx_template を選択
2. clone
3. src フォルダに必要な資料を ipynb で作成し、追加
4. make html で ipynb -> html に変換
5. git hub に push
※ git hub 側に Webhook の設定がなされているかを確認

講義資料書き方ガイドライン
講義資料の書き方については以下を参照してください。
https://www.notion.so/9485605db012432582555f3688899801

## 種類

- markdown
- jupyter
- jupyter + markdown

## インストールガイド

Pythonをインストールしていることが前提となります。
Pythonのインストール方法を下記で説明しています。

- [WindowsでPythonを使って『機械学習』を学ぶための環境構築](https://qiita.com/yoshizaki_kkgk/items/1057ed4dcc36ed9be7f5)
- [MacでPythonを使って『機械学習』を学ぶための環境構築](https://qiita.com/yoshizaki_kkgk/items/4663148a2b3ca078ddbc)

### Windowsの方（Anacondaでインストールを前提）

```bash
python -m pip install sphinx
python -m pip install nbsphinx
python -m pip install sphinx_rtd_theme
```

### Macの方（Home Brewでインストールを前提）

```bash
pip3 instal sphinx
pip3 install nbsphinx
pip3 install sphinx_rtd_theme
```

## ビルド手順

HTMLファイルをビルドする手順は以下の通りです。

### Windowsの方

```bash
./make.bat html
```

### Macの方

```bash
make html
```