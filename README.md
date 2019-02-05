# 2018年度　地球惑星環境科学科リモートセンシング・ GISおよび実習 前半（GIS）

## 日程　2018/2/6, 7, 8

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
    - 6.ネットワーク分析(最短経路検索) ※余裕がある方のみ

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
- [入力フォーム](https://docs.google.com/forms/d/1FkX5JHxRS_v032PYuoj0BdMVSnPqI3DCNq_33hIK7Ss/viewform?edit_requested=true)
