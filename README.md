# FY2022 Project PLATEAU UC22-035「XR技術を用いた体感型アーバンプランニングツール」の成果物


## 1. 概要
TangibleTownPlanningはボード上のボックスを操作することによって、構築されたシーン（3D空間）に事物を配置し景観の変化を確認できるツールです。主に以下の機能を提供しています。
* シーン構築・表示
  * ボード上のボックスの位置情報をリアルタイムに取得、送信
  * ボックスの位置情報を受信し、シーン（3D空間）を構築
  * シーンの人視点での景観を表示

## 2．「XR技術を用いた体感型アーバンプランニングツール」について
### ユースケースの概要
行政機関やデベロッパーによる新規開発・再開発、にぎわいの創出、景観の保全などを目的とした、アーバンプランニングのプロセスにおいて、これまでも開発側のデベロッパーや行政は市民参画の促進を試みてきましたが、実際には現状やプランの認知の難しさやコミュニケーションツールの不足といった課題がありました。
今回の実証実験では、3D都市モデルおよびXRを用いた直感的かつ体感的なアーバンプランニングにおけるコミュニケーションツールを開発することで、市民参加を促進しました。

### 開発システムの概要
ユーザー自らがインタラクティブな操作でその場で3Dモデルを変更することで、景観の変化をその場で確認できます。ユーザーインターフェースには「タンジブルインタフェース」を用い、目の前の模型の配置を変えたり、入れ換えたりすることで、3D空間内のモデルも対応して変化します。


## 3．利用手順
## 対応Unityバージョンのインストール
#### ArUcoServer及びVR_Client は、Unityバージョン 2020.3 を想定しています。 
#### そのバージョンがインストールされていない場合は、次の手順でインストールしてください。 
* Unity Hub を[こちら](https://unity3d.com/jp/get-unity/download)からインストールします。 
* Unity Hub とは、Unityのお好きなバージョンをインストールして起動することのできるソフトウェアです。 
* Unity Hubを起動し、左のサイドバーからインストール → 右上のボタンからエディターをインストール をクリックします。 
![unityhub.png](https://github.com/rin-tani/test/blob/main/unityhub.png)

### 有償アセットについて
#### ArUcoServer 及び VR_Client は、下記の有償アセットを使用しています。したがって、ArUcoServer 及び VR_Client の使用に際し、下記のアセットを購入し、インポートする必要があります。
* OpenCV for Unity(ArUcoServer)
* UniStorm(VR_Client)

## 導入
#### ArUcoServer 及び VR_Client の導入は、下記の手順で行います。
* GitHubの配布ページから zipファイルをダウンロードします。
* ダウンロードしたzipファイルを展開します。
* Unity Hub 画面右上の開くを押し、展開したフォルダを選択します。
![unityhubp.png](https://github.com/rin-tani/test/blob/main/unityhubp.png)

* ArUcoServer 及び VR_Client それぞれのウインドウが開いたら完了です。

## ArUcoServerの起動
### シミュレーターの起動
* ウインドウ上部の Play を押します。
* Game 画面上で Debug を押します。

### 通信開始
* Game 画面上で Start Host を押します。

## VR_Clientの起動
### 通信開始
* ウインドウ上部の Play を押します。
* Game 画面上で Start Client を押します。

## 機能解説
### 事物の配置
* ArUcoServerウインドウの Game 画面上で、右側に配置された数字の書かれたボックスをドラッグし、中央のボード上に配置します。
![asSim.png](https://github.com/rin-tani/test/blob/main/asSim.png)

* VR_ClientウインドウGame画面上で、ArUcoServerで配置したボックスに対応した事物が配置されていることを確認します。
![vrcl.png](https://github.com/rin-tani/test/blob/main/vrcl.png)
# 

### フライスルー
* VR_ClientウインドウGame画面上で、下記の操作で移動することができます。
#### マウス右ドラッグ：方向転換
#### W / A / S / D / E / Q キー：前 / 左 / 後ろ / 右 / 上 / 下 に移動
# 

### 天候・時間帯の変更
* VR_ClientウインドウGame画面左下のボタン群で、時間帯や天候を変更できます。
#### Daytime / Evening / Night：昼 / 夕方 / 夜
# 

### 配置の保存・読み出し
* VR_ClientウインドウGame画面右上のボタン群で、事物の配置状態の保存、読み出しができます。
#### 各スロット Save/Load：配置状態の保存/配置状態の読み出し
#

## ライセンス <!-- 定型文のため変更しない -->
* ソースコードおよび関連ドキュメントの著作権は国土交通省に帰属します。
* 本ドキュメントは[Project PLATEAUのサイトポリシー](https://www.mlit.go.jp/plateau/sitepolicy/)（CCBY4.0および政府標準利用規約2.0）に従い提供されています。

## 注意事項 <!-- 定型文のため変更しない -->

* 本レポジトリは参考資料として提供しているものです。動作保証は行っておりません。
* 予告なく変更・削除する可能性があります。
* 本レポジトリの利用により生じた損失及び損害等について、国土交通省はいかなる責任も負わないものとします。

## 参考資料　 <!-- 各リンクは納品時に更新 -->
* XR技術を用いた体感型アーバンプランニングツール技術検証レポート（近日公開予定）: https://www.mlit.go.jp/plateau/libraries/technical-reports/
*  PLATEAU Webサイト Use caseページ「XR技術を用いた体感型アーバンプランニングツール」: https://www.mlit.go.jp/plateau/use-case/
### （利用しているライブラリなどへのリンク）
* OpenCV for Unity：https://assetstore.unity.com/packages/tools/integration/opencv-for-unity-21088?locale=ja-JP
* UniStorm：https://assetstore.unity.com/packages/tools/particles-effects/unistorm-2714
