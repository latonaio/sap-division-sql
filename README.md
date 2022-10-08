# data-platform-currency-sql  
data-platform-currency-sql は、主にエッジアプリケーションにおいて、SAPと連携された製品部門データを保存するSQLテーブルを作成するためのレポジトリです。  
data-platform-currency-sql は、そのままクラウド環境におけるアプリケーションにも、適用可能です。  

## 前提条件  
data-platform-currency-sql は、SQL の SAP とのデータ連携にあたり、オンプレミス版である（＝クラウド版ではない）SAPS4HANA API の利用を前提としています。クラウド版APIを利用する場合は、ご注意ください。  
https://api.sap.com/api/API_DIVISION_SRV/overview  
本レポジトリ の sql設定ファイルの内容は、上記URL の API 仕様を前提としています。  

## sqlの設定ファイル
data-platform-currency-sql には、sqlの設定ファイルとして以下のsqlファイルが含まれています。  

* data-platform-currency-sql-division-data.sql （SAP 製品部門 - 製品部門データ）
* data-platform-currency-sql-division-text-data.sql （SAP 製品部門 - 製品部門テキストデータ）

## MySQLのセットアップ / Kubernetesの設定 / SQLテーブルの作成方法
MySQLのセットアップ / Kubernetesの設定 / 具体的なSQLテーブルの作成方法、については、[mysql-kube](https://github.com/latonaio/mysql-kube)を参照ください。