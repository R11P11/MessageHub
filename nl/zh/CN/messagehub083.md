---

copyright:
  years: 2015, 2017
lastupdated: "2016-22-11"

---

{:new_window: target="_blank"}
{:shortdesc: .shortdesc}
{:screen: .screen}
{:codeblock: .codeblock}
{:pre: .pre}

# 最大限制
{: #max_limits}

对于 {{site.data.keyword.mql}} API，将强制实施以下限制：
{:shortdesc}

* 可以存储的最大数据量与支付套餐的单个 Kafka 分区一致（通常为 1 GB）。如果超出此数据限制，将在发送新消息时，除去分区中的最旧消息。
* 消息存储的最长时间与支付套餐的单个 Kafka 分区一致（通常为 24 小时）。无法检索早于此时间段的消息。
* 消息的最大大小（不包括头）为 1 MB。
* 一次可连接的最大客户机数为 25 个。
* 一次可以处于活动状态的最大目标数为 25 个。活动目标的定义如下：
  - 当前连接或没有连接客户机且 TimeToLive > 0 的目标。
  - 连接了客户机且 TimeToLive = 0（缺省值）的目标。 
  <p>客户机之间共享的目标计为一个目标。</p>
