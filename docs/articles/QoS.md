---
title: QoS
date: 2020-04-02T03:30:00
---

# QoS

* Quality of Service
* サービスがどれくらいユーザーを満足させられるかの尺度
* モデル
  * Integrated Services
    * アプリケーションの通信フローごとに帯域を予約する方式
  * Differentiated Services
    * トラフィックを分類、マーキング(優先度付け)、キューイング(トラフィックのキューへの振り分け)
　スケジューリング（キューの優先度に応じたパケットの送出）して、ネットワーク機器ごとに実施
  * ベストエフォート
    * DiffServ や IntServ のアーキテクチャによるQoSが実装されていなかった場合、パケットの内容や
　サイズに関係なく、先着順にパケットを送出していくベストエフォート型 (= FIFO) が提供される

> https://ja.wikipedia.org/wiki/Quality_of_Service

> https://www.infraexpert.com/study/telephony6.html