---
title: logonUser 资源类型
description: 包含有关此主机上已登录用户的有状态信息
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: preetikr
ms.openlocfilehash: 20a5f4ab827a09fd6254f3cbe8a590eb20fd76223eb8f24445fbe3b52a5f3ea5
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54193480"
---
# <a name="logonuser-resource-type"></a>logonUser 资源类型

命名空间：microsoft.graph

包含有关此主机上已登录用户的有状态信息

## <a name="properties"></a>属性

| 属性   | 类型 |说明|
|:---------------|:--------|:----------|
|accountDomain|String|用于登录的用户帐户的域。|
|accountName|字符串|用于登录的用户帐户名。|
|accountType|字符串|用户帐户类型，根据Windows类型。 可取值为：`unknown`、`standard`、`power`、`administrator`。|
|firstSeenDateTime|DateTimeOffset|此用户帐户的最早登录发生的日期时间 (提供程序确定的时间段) 。 时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。|
|lastSeenDateTime|DateTimeOffset|此用户帐户最近一次登录的日期/时间。 时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。|
|logonId|String|用户登录 ID。|
|logonTypes|String collection|从首次看到到最后一次看到时为已登录用户观察到的登录类型的集合。 可取值为：`unknown`、`interactive`、`remoteInteractive`、`network`、`batch`、`service`。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.logonUser"
}-->

```json
{
  "accountDomain": "String",
  "accountName": "String",
  "accountType": "String",
  "firstSeenDateTime": "String (timestamp)",
  "lastSeenDateTime": "String (timestamp)",
  "logonId": "String",
  "logonTypes": ["String"]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "logonUser resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


