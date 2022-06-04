# Introduction

## Next.jsとは
* Reactをベースに開発されたフロントエンドフレームワーク
* ReactはSPA(Single Page Application)として1ページに対して巨大なJSを生成して動かしているのに対して、Next.jsはSSR(サーバーサイドレンダリング)やSSG(Static Site Generation)が簡単に作れる
* SSRやSSGやFile Base Routingなど多くの機能をゼロコンフィグ(webpack等の設定が要らない)で提供してくれる
* 開発プロセスとアプリケーションの両方を高速化してくれる

=> WebApplicationを少ない設定で簡単につくれてしまうフレーワークってことかな？

## どうやって動かすのか
* 開発環境と本番環境で工程が異なる
* **compiled**
  * JSX、TypeScript、JavaScriptの最新バージョンをブラウザが理解するJSファイルにコンパイルする
* **bundled**
  * 内部モジュールや外部のサードパーティーパッケージとの依存関係を解決し、ファイルをブラウザ用に最適化されたバンドルにマージすることで、ユーザーがウェブページを訪れた際のファイル要求の回数を減らす
* **minified**
  * ファイルサイズを小さくすることでロードを短縮（本番環境用）
* **code split**
  * 各ページのエンドポイント毎に読み込むJSを分割することでレンダリングを高速化させる
* **Pre-rendering**
  * アプリを静的なHTMLにプリレンダリングしておくことで、ページ遷移が速い&JavascriptがOFFでもHTMLを表示することができる
