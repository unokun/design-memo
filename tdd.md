# 概要
ソフトウエア関連の設計メモ

# ボブ・マーティンのTDD3原則
* 失敗するユニットテストを成功させるためのプロダクトコード以外は書いては行けない。
* 失敗させるのに十分なだけのユニットテスト以外は書いてはいけない。
* 失敗するユニットテスト１つを成功させるのに十分なだけのプロダクトコード以外を書いてはいけない

# SOLID
## 概要

* S 単一責務の原則(Single Responsible Principle)
* O オープン・クローズドの原則(Open Closed Principle)
* L リスコフの置換原則(Liskov Substitution Principle)
* I インタフェース分離の原則(Interface Segregation Principle)
* D 依存関係逆転の原則(Dependency Inversion Principle)

## ゴール
* 内部的に凝集度が高い、他のモジュールとの関係が疎結合になる。
* 各モジュールの目的が明確に分けられることによって、コードの変更が局所的になる。
* テストしやすい設計になる。

## 単一責務の原則(Single Responsible Principle)
モジュールは単一の責務を持つ。
モジュールと関数に適切な名前を付けることで責務を明確にする。

## オープン・クローズドの原則(Open Closed Principle)
モジュールは、「拡張に関してオープンな状態にし、変更に関してはクローズドな状態」にする。
例）USBデバイスの規格に関してはオープンにし、個々のデバイスに関してはクローズドにする。

## リスコフの置換原則(Liskov Substitution Principle)
同じインタフェースを持つモジュールは、呼び出し側が特別な知識を持つことなく、置換可能でなければならない。

## インタフェース分離の原則(Interface Segregation Principle)
クライアントモジュールは、多機能なインタフェースに依存してはいけない。

## 依存関係逆転の原則(Dependency Inversion Principle)
上位モジュールは下位モジュールに依存してはいけない。

## 文献
* 「アジャイルソフトウエア開発の奥義」[Mars02]

# コードのにおいと改善方法
## 重複したコード
## まずい名前
関数の名前は内部動作ではなく意図した結果がわかる名前にする。
例) BinarySearchではなく、Findにする。
## まずいパスタ
スパゲティコードを、レイヤー内の凝縮性とレイヤー間の疎結合を持つコードにリファクタリングする。
大きな関数から小さな関数を抽出し、関連したデータをひとまとめにすることから始める。
## 長すぎる関数
## 抽象化の乱れ(Abstraction Distraction)
## 当惑させるブーリアン(Bewilidering Boolean)
## 恥ずかしいSwitch Case(Switch Case Disgrace)
## 重複したSwitch Case
## 非常なネスト(Nefarious Nesting)
## 機能の横恋慕(Feature Envy)
## 長すぎるパラメータリスト
## 行き当たりばったりの初期化(Willy-nilly Initialization)
## 野放しのグローバル変数(Global Free-for-All)
## コメント
## コメントアウトされたコード
変更点はソース管理にまかせ削除する。
## 条件コンパイル
