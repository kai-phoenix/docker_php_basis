#概要
php8.2,apache,mysql8.2の構成で検証用としてphpをdocker上で動かすプログラムです。
私の検証用と今後のphpを簡単に手を動かしたい方向けに作成しました。
backend内に何らかのphpファイルを置くと動作するように作成しています。
サンプルファイルとしてindex.php,sample.phpを置いています。
dbの検証用にadminerを接続しています。
id,passはdocker-compose.ymlファイル内db部分を参照して下さい。

#使い方
1.このプログラム上でdockerコンテナを起動する
docker compose up -d
2.動かしたいphpファイルを置く
3.動作を確認したら以下コマンドでdockerコンテナを終了する
docker compose down