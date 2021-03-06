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


#資料安全與隱私
{: #data_security}


{{site.data.keyword.IBM}} 使用下列方法來協助確定您的資料安全與隱私：
{:shortdesc}

## 加密通訊協定
{: #cryptographic notoc}


*  連線到 Kafka 原生及 REST 介面時必須使用 TLS 1.2。
*  連線僅限於下列強式密碼組合：

      * ECDHE-RSA-AES128-GCM-SHA256 
      * ECDHE-RSA-AES256-GCM-SHA384 
      * DHE-RSA-AES128-GCM-SHA256 
      * kEDH+AESGCM 
      * ECDHE-RSA-AES128-SHA256 
      * ECDHE-RSA-AES256-SHA384 
      * DHE-RSA-AES128-SHA256 
      * DHE-RSA-AES256-SHA256



*  若要存取 {{site.data.keyword.messagehub}} 儀表板，您必須使用支援 TLS 1.2 的瀏覽器。
   
## 訊息有效負載的加密
{: #encryption_payloads notoc}

由於傳輸層安全 (TLS)，訊息資料在 {{site.data.keyword.messagehub}} 和用戶端之間傳輸時會經過加密。{{site.data.keyword.messagehub}} 會在已加密的磁碟上儲存靜止的訊息資料和訊息日誌。



