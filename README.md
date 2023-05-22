# techdojo-monitoring-sample
## 概要
### イベント
本repositoryは、以下イベントの際に使用するデモ環境起動用ファイルになります。
https://ibm-developer.connpass.com/event/278896/

### デモ内容
Prometheus（Grafana）でPostgreSQLを監視する

### ファイル構成
* docker-compose.yml：デモするコンテナ環境
* postgres.env：postgres-expoterのデータベース接続設定ファイル）
* prometheus/prometheus.yml：prometheus本体の設定ファイル
* prometheus/rules.yml：アラート条件設定ファイル
* alertmanager/config.yml：アラート通知先設定ファイル

## 動作確認環境
* Windows11
* Docker for Business

## 起動方法
➀任意のフォルダにすべてダウンロード

➁同じフォルダ内に以下4つのフォルダを作成する
```
$ mkdir data
$ mkdir proc
$ mkdir rootfs
$ mkdir sys
```

➂以下コマンドを実行
```
$ docker-compose up -d
```

## 動作確認
以下URLにアクセスしてadmin/adminでログイン
```
http://locaohost:3003
```
