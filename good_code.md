# 習慣
## コードを読む機会を増やす

### コード検索サービス
* [Google Code Search](http://www.google.com/codesearch)
* [Koders](http://www.koders.com)

## コードを書く機会を増やす
環境（フレームワーク）を０からセットアップする練習をする。

##　道具を磨く
* エディタ
* 自動化
* バージョン管理

## 知る
知識を習得するには、原点とHowTo本の2冊買いがおすすめ

## 聞く
* コードレビューを受ける
* ブログを書く
* コミュニティや勉強会に参加する
* 成果を発表する

# 名前付け
## 良い名前の条件
* 説明的で意味・意図を表している
* 一貫性がある
 * 対称性を保つ

    例）begin/end, read/write, on/off
 * 単語の組み合わせを一貫させる

 　　例) scoreAvg, scoreAverage, avgScoreを混在させない。

* 英単語を確認する

　　Google Code Searchで検索する。

* イディオムに従っている
* コーディング標準に従っている

## 変数名
本は説明的な名前を付ける
* グルーバル変数、クラス変数、フィールド変数は意味を正しく表現する
* ローカル変数はスコープの長さで使い分ける
* メソッドの引き数名はわかりやすく簡潔に

## メソッド名
「動詞」、「動詞＋目的語」

### javaで良く使用されるメソッド名
|メソッドの役割|メソッド名|
|:---|:---|
|値の取得に関するメソッド|getXXX|
|値のセットに関するメソッド|setXXX|
|生成に関するメソッド|create, build, make, generate|
|初期化に関するメソッド|initialize, setupXXX|
|破棄に関するメソッド|destroy, dispose|
|状態の確認に関するメソッド|contains, exists|

## クラス名
設計的な観点

## パッケージ/ネームスペース
### フレームワーク／ライブラリ開発
* Scope
* Loader
* Engine
* Provider
* Conversion
* Behavior
* Descriptor
* Cache
* Resolver
* Processor

### GUI／フレームワーク開発
* Listener
* Handler
* RUnner
* Command
* Observer
* Node
* Adaptor
* Proxy
* Holder
* Context
* Monitor
* State
* builder
* Factory
* Visitor
* Decorator
* Strategy

### 業務Webアプリケーション開発
* Action
* Controller
* Dto
* Logic
* Service
* Util
* Entity
* Helper
* Support
* Dao
* Manager
* Bean
* Form
* Exception
* Validator
* Test
* Impl

## プロジェクト名

# スコープ
## ローカル変数のスコープ
* 変数は使用する直前で宣言する
* メソッドに抽出する
* イテレータの一時変数のスコープをループ内に閉じ込める
* 代入されない変数はfinalを付ける

# コードの分割
# コードの集約
# コードのパフォーマンス
## パフォーマンスチューニングの手順
### まずは計測する
* ログ出力による計測
* プロファイラによる計測
* 原因特定
* チューニングする
* チューニング結果を計測する

# ユニットテスト
# 抽象化
# メタプログラミング
# フレームワークを作ろう

# その他
