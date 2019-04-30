# 概要
設計メモ

## Microservice

### 特性

* サービスによるコンポーネント化
* 業務に対応づけたサービス
* サービスはプロジェクトではなく独立した製品に相当
* インテリジェンスはプロットフォーム側ではなくサービス側に集約
* 分散型統治
* 分散型データ管理
* インフラの自動化
* 障害発生前提の設計
* 更新前提の設計

### 設計

* 業務要件
* ドメインモデル
* サービス・コンポーネントモデル

### マイクロサービスの見つけ方

* ケーパビリティ(Capability)に注目した方法
* ドメイン駆動開発の考え方を利用する方法

#### ケーパビリティ(Capability)に注目した方法

ケーパビリティとは、必要となる知識、スキル、資源、そして設備や施設を備えた組織が特定のアクティビティを推敲することで期待される価値を提供する能力です。ケーパビリティはアクションの集まりであるアクティビティ、つまり主にビジネスに関わる機能にリンクした言葉・概念であり、データモデルを意識しない。

#### ドメイン駆動開発の考え方を利用する方法

ドメイン駆動開発の境界づけられたコンテキストはコンポーネントを設計する際の参考になります。

#### 書籍

* [マイクロサービス入門 アーキテクチャと実装 \| 長瀬 嘉秀, 田中 明, 松本 哲也 \|本 \| 通販 \| Amazon](https://www.amazon.co.jp/%E3%83%9E%E3%82%A4%E3%82%AF%E3%83%AD%E3%82%B5%E3%83%BC%E3%83%93%E3%82%B9%E5%85%A5%E9%96%80-%E3%82%A2%E3%83%BC%E3%82%AD%E3%83%86%E3%82%AF%E3%83%81%E3%83%A3%E3%81%A8%E5%AE%9F%E8%A3%85-%E9%95%B7%E7%80%AC-%E5%98%89%E7%A7%80/dp/4865941193)
* [マイクロサービスアーキテクチャ \| Sam Newman, 佐藤 直生, 木下 哲也 \|本 \| 通販 \| Amazon](https://www.amazon.co.jp/%E3%83%9E%E3%82%A4%E3%82%AF%E3%83%AD%E3%82%B5%E3%83%BC%E3%83%93%E3%82%B9%E3%82%A2%E3%83%BC%E3%82%AD%E3%83%86%E3%82%AF%E3%83%81%E3%83%A3-Sam-Newman/dp/4873117607/ref=pd_lpo_sbs_14_t_0?_encoding=UTF8&psc=1&refRID=69SFP55AZFBN31P34ZG2)
* [プロダクションレディマイクロサービス ―運用に強い本番対応システムの実装と標準化 \| Susan J\. Fowler, 佐藤 直生, 長尾 高弘 \|本 \| 通販 \| Amazon](https://www.amazon.co.jp/%E3%83%97%E3%83%AD%E3%83%80%E3%82%AF%E3%82%B7%E3%83%A7%E3%83%B3%E3%83%AC%E3%83%87%E3%82%A3%E3%83%9E%E3%82%A4%E3%82%AF%E3%83%AD%E3%82%B5%E3%83%BC%E3%83%93%E3%82%B9-%E2%80%95%E9%81%8B%E7%94%A8%E3%81%AB%E5%BC%B7%E3%81%84%E6%9C%AC%E7%95%AA%E5%AF%BE%E5%BF%9C%E3%82%B7%E3%82%B9%E3%83%86%E3%83%A0%E3%81%AE%E5%AE%9F%E8%A3%85%E3%81%A8%E6%A8%99%E6%BA%96%E5%8C%96-Susan-J-Fowler/dp/4873118158/ref=pd_sbs_14_2/355-1019699-9113304?_encoding=UTF8&pd_rd_i=4873118158&pd_rd_r=99ed7a66-6ad0-11e9-b0e6-0756405ed8cd&pd_rd_w=95ZuW&pd_rd_wg=f4446&pf_rd_p=ad2ea29d-ea11-483c-9db2-6b5875bb9b73&pf_rd_r=T2JFVS2YDV4VTQFBV8GH&psc=1&refRID=T2JFVS2YDV4VTQFBV8GH)

## アジャイル/クリーンアーキテクチャ
* [アジャイルソフトウェア開発の奥義 第2版 オブジェクト指向開発の神髄と匠の技 \| ロバート・C・マーチン, Robert C\. Martin, 瀬谷 啓介 \|本 \| 通販 \| Amazon](https://www.amazon.co.jp/%E3%82%A2%E3%82%B8%E3%83%A3%E3%82%A4%E3%83%AB%E3%82%BD%E3%83%95%E3%83%88%E3%82%A6%E3%82%A7%E3%82%A2%E9%96%8B%E7%99%BA%E3%81%AE%E5%A5%A5%E7%BE%A9-%E7%AC%AC2%E7%89%88-%E3%82%AA%E3%83%96%E3%82%B8%E3%82%A7%E3%82%AF%E3%83%88%E6%8C%87%E5%90%91%E9%96%8B%E7%99%BA%E3%81%AE%E7%A5%9E%E9%AB%84%E3%81%A8%E5%8C%A0%E3%81%AE%E6%8A%80-%E3%83%AD%E3%83%90%E3%83%BC%E3%83%88%E3%83%BBC%E3%83%BB%E3%83%9E%E3%83%BC%E3%83%81%E3%83%B3/dp/4797347783/ref=pd_sim_14_3/355-1019699-9113304?_encoding=UTF8&pd_rd_i=4797347783&pd_rd_r=1f541812-6acf-11e9-8780-2d40c69616dc&pd_rd_w=VOPRO&pd_rd_wg=gGSsH&pf_rd_p=b88353e4-7ed3-4da1-bc65-341dfa3a88ce&pf_rd_r=07YVHB83AVF5YT9QJR17&psc=1&refRID=07YVHB83AVF5YT9QJR17)
* [Clean Architecture 達人に学ぶソフトウェアの構造と設計 \| Robert C\.Martin, 角 征典, 高木 正弘 \|本 \| 通販 \| Amazon](https://www.amazon.co.jp/Clean-Architecture-%E9%81%94%E4%BA%BA%E3%81%AB%E5%AD%A6%E3%81%B6%E3%82%BD%E3%83%95%E3%83%88%E3%82%A6%E3%82%A7%E3%82%A2%E3%81%AE%E6%A7%8B%E9%80%A0%E3%81%A8%E8%A8%AD%E8%A8%88-Robert-C-Martin/dp/4048930656/ref=pd_sim_14_2/355-1019699-9113304?_encoding=UTF8&pd_rd_i=4048930656&pd_rd_r=eb5d7b30-6ace-11e9-8780-2d40c69616dc&pd_rd_w=oZH5n&pd_rd_wg=KpaYw&pf_rd_p=b88353e4-7ed3-4da1-bc65-341dfa3a88ce&pf_rd_r=VHYFAZ0KZ8H2TEZQ9PWT&psc=1&refRID=VHYFAZ0KZ8H2TEZQ9PWT)

## ドメイン駆動開発
* [エリック・エヴァンスのドメイン駆動設計 \(IT Architects’Archive ソフトウェア開発の実践\) \| エリック・エヴァンス, 今関 剛, 和智 右桂, 牧野 祐子 \|本 \| 通販 \| Amazon](https://www.amazon.co.jp/%E3%82%A8%E3%83%AA%E3%83%83%E3%82%AF%E3%83%BB%E3%82%A8%E3%83%B4%E3%82%A1%E3%83%B3%E3%82%B9%E3%81%AE%E3%83%89%E3%83%A1%E3%82%A4%E3%83%B3%E9%A7%86%E5%8B%95%E8%A8%AD%E8%A8%88-Architects%E2%80%99Archive-%E3%82%BD%E3%83%95%E3%83%88%E3%82%A6%E3%82%A7%E3%82%A2%E9%96%8B%E7%99%BA%E3%81%AE%E5%AE%9F%E8%B7%B5-%E3%82%A8%E3%83%AA%E3%83%83%E3%82%AF%E3%83%BB%E3%82%A8%E3%83%B4%E3%82%A1%E3%83%B3%E3%82%B9/dp/4798121967/ref=pd_bxgy_14_2/355-1019699-9113304?_encoding=UTF8&pd_rd_i=4798121967&pd_rd_r=c82a1966-6ace-11e9-ba66-b11c1b973bef&pd_rd_w=77HLZ&pd_rd_wg=odCB6&pf_rd_p=2d39d87c-5ff4-47a9-a2d0-79fb936a2d97&pf_rd_r=MSHG1ZK4J7GNCMHCTFCD&psc=1&refRID=MSHG1ZK4J7GNCMHCTFCD)
* [実践ドメイン駆動設計 \(Object Oriented SELECTION\) \| ヴァーン・ヴァーノン, 高木 正弘 \|本 \| 通販 \| Amazon](https://www.amazon.co.jp/%E5%AE%9F%E8%B7%B5%E3%83%89%E3%83%A1%E3%82%A4%E3%83%B3%E9%A7%86%E5%8B%95%E8%A8%AD%E8%A8%88-Object-Oriented-SELECTION-%E3%83%B4%E3%82%A1%E3%83%BC%E3%83%B3%E3%83%BB%E3%83%B4%E3%82%A1%E3%83%BC%E3%83%8E%E3%83%B3/dp/479813161X/ref=pd_bxgy_14_img_2/355-1019699-9113304?_encoding=UTF8&pd_rd_i=479813161X&pd_rd_r=eb5d7b30-6ace-11e9-8780-2d40c69616dc&pd_rd_w=AzFEJ&pd_rd_wg=KpaYw&pf_rd_p=2d39d87c-5ff4-47a9-a2d0-79fb936a2d97&pf_rd_r=VHYFAZ0KZ8H2TEZQ9PWT&psc=1&refRID=VHYFAZ0KZ8H2TEZQ9PWT)

