---

copyright:
  years: 2015, 2017
lastupdated: "2016-11-22"

---

{:new_window: target="_blank"}
{:shortdesc: .shortdesc}
{:screen: .screen}
{:codeblock: .codeblock}
{:pre: .pre}

# {{site.data.keyword.messagehub}}에서 {{site.data.keyword.mql}} API 사용 설정
{: #mql_enable}


**모든 메시지가 "MQLight" 토픽을 통해서 이동하므로 "MQLight"로 이름 지정된 Kafka 토픽을 우선 명시적으로 작성해야 API를 사용할 수 있습니다. 이 토픽에는 단일 파티션이 있어야 합니다. 이 토픽을 작성하면 사용자의 서비스 인스턴스에 대해 MQ Light API를 사용할 수 있습니다.**  {{site.data.keyword.messagehub}}에서 토픽 작성 방법에 대한 자세한 정보는 [토픽 관리](/docs/services/MessageHub/messagehub070.html)를 참조하십시오.

"MQLight" 토픽은 그 메시지 데이터를 저장하고 다른 Kafka 클라이언트와 상호작용하기 위해 MQ Light API에서 사용됩니다. 이 토픽이
작성되면 서비스 결제 플랜에 개요가 나와 있는 표준 비율대로 비용이 발생한다는 점에 주의하십시오. 

MQ Light API를 사용 안함으로 설정하려면 "MQLight" 토픽을 삭제하십시오. 토픽을 삭제하면 모든 데이터가 영구 삭제됨에 유의하십시오. 
