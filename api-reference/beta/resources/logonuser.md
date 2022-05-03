---
title: logonUser 资源类型
description: 包含有关此主机上已登录用户的有状态信息
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: security
author: preetikr
ms.openlocfilehash: d665906abbbea3f49d352de5600c647f62d8bff6
ms.sourcegitcommit: 267e3baf545c8dc71ba2ab69497e3ec369379f43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/03/2022
ms.locfileid: "65176781"
---
# <a name="logonuser-resource-type"></a>logonUser 资源类型

命名空间：microsoft.graph

包含有关此主机上已登录用户的有状态信息

## <a name="properties"></a>属性

| 属性   | 类型 |Description|
|:---------------|:--------|:----------|
|accountDomain|String|用于登录的用户帐户的域。|
|accountName|String|用于登录的用户帐户的帐户名称。|
|accountType|String|用户帐户类型，根据Windows定义。 可能的值是：`unknown`、`standard`、`power`、`administrator`。|
|firstSeenDateTime|DateTimeOffset|此用户帐户最早登录的 DateTime 发生 (提供程序确定的) 期。 时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。|
|lastSeenDateTime|DateTimeOffset|发生此用户帐户最新登录的 DateTime。 时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。|
|logonId|String|用户登录 ID。|
|logonTypes|String collection|从第一次到最后一次看到时，为登录用户观察到的登录类型的集合。 可取值为：`unknown`、`interactive`、`remoteInteractive`、`network`、`batch`、`service`。|

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


