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

# 使用 MQ Light Node.js 客户机 
{: #mql_node}


要使用 API，请添加对用于 Node.js 的最新可用 {{site.data.keyword.mql}} 客户机 API 的引用，如下所示：

将以下引用添加到 <code>package.json</code> 文件的 dependency 部分：

<pre class="pre"><code>"mqlight" : "1.0.x"</code></pre>
{: codeblock}

将以下 require 语句添加到源文件：

<pre class="pre"><code>var mqlight = require(‘mqlight’);</code></pre>
{: codeblock}

<!-- Comment from Andrew
Instructions for getting started, with links for more info
Simple send source and receive source in-line

-->


