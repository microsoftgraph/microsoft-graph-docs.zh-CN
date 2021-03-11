---
title: logonUser 资源类型
description: 包含有关此主机上已登录用户的有状态信息
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: preetikr
ms.openlocfilehash: 9986aaa7cb5fbf5f8687c43de019b234a4a971d8
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/11/2021
ms.locfileid: "50720492"
---
# <a name="logonuser-resource-type"></a>logonUser 资源类型

命名空间：microsoft.graph

包含有关此主机上已登录用户的有状态信息

## <a name="properties"></a>属性

| 属性   | 类型 |说明|
|:---------------|:--------|:----------|
|accountDomain|String|用于登录的用户帐户的域。|
|accountName|String|用于登录的用户帐户的帐户名称。|
|accountType|String|用户帐户类型（按 Windows 定义）。 可取值为：`unknown`、`standard`、`power`、`administrator`。|
|firstSeenDateTime|DateTimeOffset|此用户帐户最早登录的日期/时间 (提供程序确定的) 。 时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。|
|lastSeenDateTime|DateTimeOffset|发生此用户帐户最新登录的日期/时间。 时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。|
|logonId|String|用户登录 ID。|
|logonTypes|字符串集合|从首次看到到最后一次看到时为登录用户观察到的登录类型的集合。 可取值为：`unknown`、`interactive`、`remoteInteractive`、`network`、`batch`、`service`。|

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


