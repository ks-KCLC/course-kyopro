# KCLC 競プロ講座

## はじめに

### サイトをご覧になる場合

こちらで公開しています: <https://ks-kclc.github.io/course-kyopro/>

### ローカルでサイトをご覧になる場合・編集する場合

Pythonが整備された環境で、以下のコマンドを実行してください。

```sh
pip install -r requirements.txt
```

`mkdocs serve` を実行しながら、<http://127.0.0.1:8000/course-kyopro/> にアクセスしてください。

## 構成

### `main` ブランチ

`.md` をgit管理するブランチです。コンテンツを編集するときはここを編集します。

- `/.github/workflows/main.yml`  
  GitHub Actions の設定ファイルです。  
  `.md` が更新されると自動的にbuildされます。
- `/docs`  
  ここに `.md` ファイルが配置されます。
  - `assets`  
    各ページ共通のファイルを配置できます。
- `/.gitignore`  
  git管理したくないファイルを指定します。
- `/mkdocs.yml`  
  ページのスタイルなどの設定をします。

### `gh-pages` ブランチ

GitHub Actions によって出力されたファイルのブランチです。自動化されているのでノータッチです。  
<https://ks-kclc.github.io/course-kyopro/> はここがソースです。GitHub Pages によりbuildされています。

## 謝辞

[kclc-kaisei/kclc-kaisei.github.io](https://github.com/kclc-kaisei/kclc-kaisei.github.io/) をもとにして作成しています。
