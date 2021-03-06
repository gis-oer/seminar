# QGIS入門講習会
　QGISは、無償で利用できるオープンソースのGISとして、研究を含む幅広い分野での活用されています。この講習会では、QGISを用いて、GISの基本やソフトウェアの操作法を実習形式で解説します。今年度は異なるテーマで、2～3回のQGIS入門講習会を予定しています。※講習の前半は各回共通です。

## 第1回地形環境の分析に使えるQGIS入門
　以下は、講習で利用するリポジトリです。この講習会の前半では、QGISを用いて、GISの基本やソフトウェアの操作法を実習形式で解説します。後半では、標高データを利用して、QGISで地形情報を可視化する手法について解説します。

* [GISの実習用オープン教材](http://gis-oer.csis.u-tokyo.ac.jp/)
  * [GIS入門](https://gis-oer.github.io/gitbook/book/GISオープン教材/01_GISの基本概念/GISの基本概念.html)に進む

  * [地形環境の分析に使えるQGIS入門](https://gis-oer.github.io/gitbook/book/GISオープン教材/課題/課題ページ/1day実習コース/1day実習コース.html)に進む

* [印刷用PDF](https://github.com/gis-oer/seminar/raw/master/book.pdf)

※GitBookの仕様上、PDF内の改ページやページ番号に不具合が生じます。本PDFを印刷して使用する場合、割り付け印刷(2in1)を推奨します。

* データ(会場で配布)

* [アンケート](https://customform.jp/form/input/17227/)を記入する

* [自主学習について](https://gis-oer.github.io/gitbook/book/GISオープン教材/)

------

## 以下、講習時のメモ

* [QGIS2.8のインストール](https://github.com/gis-oer/gis-oer/blob/master/install/q2.8install.md)

* [GIS入門の教材](https://github.com/gis-oer/gis-oer/blob/master/GISオープン教材/01_GISの基本概念/GISの基本概念.md)のGitHub版
* [地形環境の分析に使えるQGIS入門](https://github.com/gis-oer/gis-oer/blob/master/GISオープン教材/課題/課題ページ/1day実習コース/1day実習コース.md)のGitHub版

* プラグインがインストールできないとき(windows版)は、実習用データの一部を`user(各自の環境に置き換えてください)/.qgis2/python/plugins`に入れてください。

### 実習時の質問：解決

* コンポーザー：スケールバーの単位を変える(m → km)  
プリントコンポーザーで地図化する範囲によって、スケールバーの単位がmかkmが自動で選択される。mの表記をkmにしたい場合、スケールバーを挿入後、アイテムプロパティ（スケールバーを選択した状態）＞単位の項目から、「ラベルをkm」とし、「バー単位の地図単位を1000」とする。

* ラスタ＞地形解析のメニューを表示する  
プラグインの管理とインストールで、`ラスター空間解析プラグイン`にチェックを入れる。


### 実習時の質問：未解決

* ラスタデータの配色について(Natural breakなどの分類ができるか)

### エラーのメモ

* 新規データの出力の際にデフォルトの書き出し先を選択するとエラーが出る

* VoGIS Profile Toolが起動しない（プラグインが壊れていると表記される）  

解決策：qProfプラグインを使用（地形断面が表示できる別のプラグイン）

プラグインの管理とインストールからqProfをインストールする。プラグイン> qProf > qProfを起動する。
![profile](./img/15pic_22-1.png)

![profile](./img/15pic_22-2.png)

1. `Digitize line`をクリックする。
2. 地図上でクリックして断面線を作成する。断面線の作成は、線の最後で右クリックすると完了する。
3. `Define topographic sources`をクリックする。
4. `Define source DEMs`をクリックする。
5. ソースラスターをチェックし、OKをクリックする。
6. DEM(s) and line sourcesのウィンドウのＯＫをクリックする。
7. ‘Calculate profile statistics’ をクリックする。
8. ‘Calculate profile statistics’をクリックする
9. OKをクリックすると地形断面図が表示される。

![profile](./img/15pic_22-3.png)
