# WebLife Japan Inc. 
<a href="https://www.web-life.co.jp/"><img src="./images/wl-logo.jpg" width="160" height="119" border="0" alt=""></a>
### EC-CUBEによる環境構築  

## EC-CUBEの概要  

>日本企業の株式会社ロックオンが提供している、ECサイト構築パッケージの名称です。日本発で、シェアは国内NO.1のオープンソースのソフトウェア
引用元：https://www.kagoya.jp/howto/netshop/ec-cube/

## 気になったことメモ  
ECサイトを作るための構築パッケージであるという事Symfonyで作られている。  
カスタマイズする事で独自のサイトを構築できる  
テンプレートエンジンがtwigを使用している。  
フロントも含めカスタマイズ可能なので業務といたしてはお客様の要望を聞きながら機能拡張などを行なう物だと思います。  
PostgerSQL MySQL SQLiteから選択可能である。  
mailサーバーを構築することも可能である。  

## install手順(仮)  
composerをインストーラでインストールした。  
サイトよりEC-CUBEをダウンロード  
ビルトインウェブサーバを立ち上げる。  
デフォルトで用意されているデモサイトが表示される。  

## ERROR
- ECCUBEセットアップ完了後に bin/console server:run が実行できなくなる（There are no commands defined in the "server"）

突然ビルトインサーバーを立ち上げる事ができなくなった。  
APP_ENV変数をproductionからdevelopmentへ変更する事で立ち上げる事ができた。  
理由や原因がわからなかったのでその辺りを調べなければいけないと思う。

