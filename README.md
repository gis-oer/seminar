# 2018年度　地球惑星環境科学科リモートセンシング・ GISおよび実習 前半（GIS）

## 日程　2019/2/6, 7, 8
## 課題提出期限は、2/14 [提出フォーム](https://docs.google.com/forms/d/1WI09sjiBq1hB1S8reIzhPdXn1kcvu-9mAl7U6DftkKU/viewform?edit_requested=true)

※2/9から朝方から11:00頃に、提出フォームが利用できれないエラーが起きていたようです。提出フォームを新規に作成しましたので、上記の提出先をご利用ください。不明な点は、メールにてご連絡ください。

- 2/6(水)：2～5限  
  10:00-12:00	講義  
  13:00-17:00	実習：GIS入門
    - 1.QGIS入門
    - 2.既存データの取得と変換

- 2/7(木)：2～5限：ベクタデータ分析入門  
  10:00-12:00	講義  
  13:00-17:00	実習
    - 1.空間座標系の変換
    - 2.基本的な空間解析（ディゾルブやクリップ等）
    - 3.領域分析（バッファ）
    - 4.点データの分析（メッシュ集計、カーネル密度推定）
    - 5.空間データの作成・編集・統合・変換（ベクタのみ）
    - 6.ネットワーク分析(最短経路検索) ※余裕がある方余裕(17:00までに1~5が終わっている方)のみ

- 2/8(金)：3～5限  
  13:00-17:00	実習 ：ラスタデータ分析入門
    - 1.空間データの作成・編集・統合・変換（ラスタのみ）
    - 2.地形情報の可視化(ラスタデータの分析）
    - 3.GRASS GIS: 流域解析(ラスタデータの分析)
    - 4.空間補間（TIN- IDW）

  - 以下は、余裕がある人のみ
    - ジオリファレンス
    - ジオコーディング


## 実習の注意事項

- 実習は、冒頭で概要と課題の簡単な説明をした後に、受講者が教材を参考に学習を進める形式で行います。実習ごとに、オンライン教材（[GIS実習オープン教材](https://gis-oer.github.io/gitbook/book/)）を用いて学習した後、指定された課題を行います。

- 課題は、実習と対応した地図の作成と設問への回答です。1回の実習で3～5枚程度の地図の作成と提出が必要です。課題として作成した地図画像は、ファイルにまとめて`右クリック＞圧縮し、zipファイルにしたものを提出してください`。

- 実習終了後、アンケートに回答してください。このアンケートの結果は、個人が特定できないように加工した後に、学習効果の評価や教材の改良等に利用します。課題の提出もアンケートフォームから行います。アンケートは、Googleフォームを利用するので、Googleアカウント（東大のメールアカウントに紐付けられたもの）を準備してください。

- 各回、教材と対応した実習用データを配布します。初回の実習以外は、`空間座標の変換作業`が必要な場合があります。

- 各実習の詳細は、使用するデータとともに、各実習日に公開します。

- 実習を行う際には、各回の注意事項を確認したうえで、進めてください。

## 実習用データ
実習用データは、当日USBで配布します。このデータは、初回の実習以外、座標変換をして利用する必要があります。

### Macの場合（初回の実習のみ、以下の点に注意が必要です）
ベクタ：shpやgeotiffへのデータ変換は、対応するソフトウェアが標準で用意されていない（ QGIS　2.x以降は、xmlをQGISで直接ドラッグアンドドロップで表示可能）。

ラスタ：http://space.geocities.jp/bischofia_vb/qgis-plugins/fgddemImporter/ に従ってプラグインをインストール。やや複雑なため、windowsでエコリスソフトウェアの使用を推奨。上記手順の`ユーザフォルダ/.qgis2/python/plugins`は隠しフォルダのため、隠しフォルダを表示する設定にする。

## 実習の問い合わせ
山内：　h.yamauchi[at]csis.u-tokyo.ac.jp ※[at]は@に置き換えてください。


## 各実習の内容

### 2/6 教材と課題
この実習は、QGISを用いたGISの入門、既存のGISデータの取得法を学習するものです。下記の教材を用いて学習をすすめ、課題を行ってください。

#### 実習項目と教材
1. QGIS入門 [教材：QGISビギナーズマニュアル](https://gis-oer.github.io/gitbook/book/materials/QGIS/QGIS.html)
2. 既存データの取得 [教材：既存の地図データと属性データ](https://gis-oer.github.io/gitbook/book/materials/07/07.html)

#### 実習の注意事項
- QGISはインストールされているものを利用してください。
- ファイル名、出力先などに日本語が含まれているとエラーが起きます。
- デフォルトの設定（ディレクトリ）でデータを出力するとエラーが起きます。
- shapeファイルは、.shp,.shx,.dbf等の複数のファイルから構成されます。そのため、移動する際にはすべてを移動してください。.shpのみを移動したために、データが表示できないというミスが多いです。
- この実習のみ、空間座標系の関係上、各教材や課題の終了後にQGISを一度閉じ（作業ファイルは任意の場所に保存）、再起動してから次の実習、課題を行ってください。
- 空間座標系についての解説は次回行います。
- 地図のレイアウト時にスケールの設定がうまくできない場合は、アンケートフォームの各課題の記述欄に「どのようにスケールが表示されているか」と「考えられる要因」について記載してください。
- 既存データの取得は、基盤地図情報（基本項目、数値標高モデル）、国土数値情報、e-statのダウンロードを中心に行ってください。ダウンロードしたデータは、QGISで表示し、データの確認を行ってください。

#### 課題
リンク先の課題を行ってください。

1. [QGIS入門の課題1](https://gis-oer.github.io/gitbook/book/materials/tasks/t_qgis_entry.html)
2. [既存の地図データと属性データの課題1](https://gis-oer.github.io/gitbook/book/materials/tasks/t_07.html)

#### 課題提出とアンケート
- [入力フォーム](https://docs.google.com/forms/d/1WI09sjiBq1hB1S8reIzhPdXn1kcvu-9mAl7U6DftkKU/viewform?edit_requested=true)

### 2/7 ベクタデータ分析入門の教材と課題
**（必読）**この実習では、ダウンロードしたデータを用いて、初歩的な空間解析を行います。GISで空間データを解析する場合、データの位置情報を示す空間座標を統一する必要があるという点に注意して実習を進めてください。この実習をはじめる前に、QGISの`設定>オプション>CRS`から`オンザフライ再投影を有効にしない`にチェックを入れ、再起動しておくと空間座標系の違いが分かりやすいです。

#### 実習項目と教材
1. 空間座標系の変換 [教材：空間データ]　※空間データの座標変換のみ
2. 基本的な空間解析 [教材：基本的な空間解析]
3. 領域分析 [教材：領域分析]　※バッファのみ
4. 点データの分析 [教材：点データの分析]※視覚的分析のみ
5. ベクトルデータの作成[教材：空間データの統合・修正]　※点線面の編集、作成のみ
6. 余裕(17:00までに1~5が終わっていれば)があれば、ネットワーク分析 [教材：ネットワーク分析]　※最短経路検索のみ

## 実習の注意事項

- この実習の課題データはすべて、緯度経度から平面直角への座標変換が必要です。実習を始める前に、[動画：座標変換の正誤事例](https://youtu.be/jAHJNI5CiKw)を参照し、間違った座標変換を行わないように注意してください。
- ベクトルデータの作成の課題は次回提出してください。この実習で作成したデータを次回使用するので、データの作成のみ行ってください。

# 要注意
- 座標変換したデータが表示されない場合：　レイヤウィンドウで右クリック＞レイヤの領域にズーム
- コンポーザーのスケールがメートルにならない場合：　右下のEPSGをクリックし、`オンザフライ再投影`にチェックを入れ平面直角の座標系を指定する
- 地理院タイルが読み込めない場合：右下のEPSGをクリックし、`オンザフライ再投影`にチェックを入れ平面直角の座標系を指定する
- 国土数値情報のデータ（インポートしたときに座標系の指定を求められるもの）は、緯度経度で提供されているため、JGD2000としてインポートする（その後、変換作業が必要）
- [課題2で使うe-statのデータ:平群町、生駒市を取得](https://www.e-stat.go.jp/gis/statmap-search?page=1&type=2&aggregateUnitForBoundary=A&toukeiCode=00200521&toukeiYear=2015&serveyId=A002005212015&prefCode=29&coordsys=1&format=shape)
- [平面直角座標系の対応表](http://www.gsi.go.jp/sokuchikijun/jpc.html)
- ポリゴン内のポイントの数の段階づけの色分けができない場合：　メッシュレイヤの属性テーブルを開く　＞　フィールド計算機＞　新しいフィールドを作る＞フィールド名（任意）を入力し、出力フィールドタイプをintegerにする。＞フィールドと値からポイントを集計した列名を選択し、OKをクリックする。最後に編集モード（鉛筆マーク）をクリックし編集を保存する。　※文字型から数値型への変換処理

#### 課題
リンク先の課題を行ってください。

1. [空間データの課題1]
2. [基本的な空間解析の課題2]
3. [領域分析の課題1]
4. [点データの分析の課題1]
5. [空間データの統合・修正の課題2] ※点（標高点）線（橋）、面（植生）のデータのみ作成してください(この課題で作成したデータを明日使用するため、本日の提出は不要)。
6. 余裕があれば、[ネットワーク分析の課題1]

#### 課題提出とアンケート
- [入力フォーム](https://docs.google.com/forms/d/1WI09sjiBq1hB1S8reIzhPdXn1kcvu-9mAl7U6DftkKU/viewform?edit_requested=true)

### 2/8 ラスタデータ分析入門教材と課題
この実習では、ラスタデータを用いて、地形情報の可視化や分析を行います。空間データの座標系に注意しながら、実習を進めてください。

#### 実習項目と教材
1. [教材：空間データの統合・修正]　※前半部のラスタデータの部分のみ（ラスタの結合、座標変換、等高線作成、配色）のみ
2. [教材：ラスタデータの分析]　※数値標高モデルの視覚的分析のみ（段彩図、傾斜区分図、斜面方位図、陰影図、鳥瞰図の作成）のみ、断面の作成は不要
3. [教材：ラスタデータの分析]　※流域解析のみ 
4. [教材：空間補間]※TIN・IDWのみ
5. 【任意　ジオリファレンス、ジオコーディング [教材：空間データ]】

## 注意事項
- 昨日作成したデータがない方、作成に失敗した方は、[こちら](https://github.com/gis-oer/seminar/raw/master/ishinomaki_shp.zip)から完成したものをダウンロードしてください。
- 2の課題は、完成例と同じように複数の図をまとめて（PowerPoint等で）、1枚の図にしたものを提出してください。
- 実習データ（day3）について、フォルダ1（実習１のデータ）、フォルダ2(実習2、３のデータ)、フォルダ3（実習4のデータ）となっている点に注意してください。

## 要注意
- ラスタデータの分析：ラスター空間解析プラグインがない場合：プラグインの管理とインストール＞地形解析を検索しチェック
- 空間補間：データ補間がない場合：プラグインの管理とインストール＞変換プラグインを検索しチェック
- 課題2について：完成例と同じものを作成する。手順4（4.陰影図をレイヤ順序の最下層とし、各ラスタデータの透過性を30％ほどにし、地形情報を視覚化する。）は無視。

#### 課題と提出先
リンク先の課題を行ってください。

1. [空間データの統合・修正の課題2] ※　課題２の背景画像を作成し、昨日作成したシェープファイルと重ねたものを提出
2. [ラスタデータの分析の課題1]
3. [ラスタデータの分析の課題4]
4. [空間補間の課題2]
5. [任意：空間データの課題2]
6. [任意：空間データの課題3]

#### 課題提出とアンケート
- [入力フォーム](https://docs.google.com/forms/d/1WI09sjiBq1hB1S8reIzhPdXn1kcvu-9mAl7U6DftkKU/viewform?edit_requested=true)

[GIS実習オープン教材]:https://gis-oer.github.io/gitbook/book/
[QGIS]:https://www.qgis.org/ja/site/
[よくある質問とエラー]:https://gis-oer.github.io/gitbook/book/materials/questions/questions.html
[教材：QGISビギナーズマニュアル]:https://gis-oer.github.io/gitbook/book/materials/QGIS/QGIS.html
[教材：既存の地図データと属性データ]:https://gis-oer.github.io/gitbook/book/materials/07/07.html
[教材：空間データの統合・修正]:https://gis-oer.github.io/gitbook/book/materials/10/10.html
[QGIS入門の課題1]:https://gis-oer.github.io/gitbook/book/materials/tasks/t_qgis_entry.html
[既存の地図データと属性データの課題1]:https://gis-oer.github.io/gitbook/book/materials/tasks/t_07.html
[空間データの統合・修正の課題2]:https://gis-oer.github.io/gitbook/book/materials/tasks/t_10.html
[教材：空間データ]:https://gis-oer.github.io/gitbook/book/materials/08/08.html
[教材：基本的な空間解析]:https://gis-oer.github.io/gitbook/book/materials/11/11.html
[教材：ネットワーク分析]:https://gis-oer.github.io/gitbook/book/materials/12/12.html
[教材：領域分析]:https://gis-oer.github.io/gitbook/book/materials/13/13.html
[空間データの課題1]:https://gis-oer.github.io/gitbook/book/materials/tasks/t_08.html
[基本的な空間解析の課題2]:https://gis-oer.github.io/gitbook/book/materials/tasks/t_11.html
[ネットワーク分析の課題1]:https://gis-oer.github.io/gitbook/book/materials/tasks/t_12.html
[領域分析の課題1]:https://gis-oer.github.io/gitbook/book/materials/tasks/t_13.html
[教材：点データの分析]:https://gis-oer.github.io/gitbook/book/materials/14/14.html
[教材：ラスタデータの分析]:https://gis-oer.github.io/gitbook/book/materials/15/15.html
[教材：空間補間]:https://gis-oer.github.io/gitbook/book/materials/18/18.html
[点データの分析の課題1]:https://gis-oer.github.io/gitbook/book/materials/tasks/t_14.html
[ラスタデータの分析の課題1]:https://gis-oer.github.io/gitbook/book/materials/tasks/t_15.html
[任意：ラスタデータの分析の課題2]:https://gis-oer.github.io/gitbook/book/materials/tasks/t_15.html
[空間補間の課題2]:https://gis-oer.github.io/gitbook/book/materials/tasks/t_18.html
[任意：ラスタデータの分析の課題3]:https://gis-oer.github.io/gitbook/book/materials/tasks/t_15.html
[ラスタデータの分析の課題4]:https://gis-oer.github.io/gitbook/book/materials/tasks/t_15.html
[任意：空間データの課題2]:https://gis-oer.github.io/gitbook/book/materials/tasks/t_08.html
[任意：空間データの課題3]:https://gis-oer.github.io/gitbook/book/materials/tasks/t_08.html
