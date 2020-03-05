---
title: logonUser 资源类型
description: 包含有关此主机上登录的用户的状态信息
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: b9a7bb439863a39ce165235b31642e542b1bb331
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42522895"
---
# <a name="logonuser-resource-type"></a>logonUser 资源类型

命名空间： microsoft. graph

包含有关此主机上登录的用户的状态信息

## <a name="properties"></a>属性

| 属性   | 类型 |说明|
|:---------------|:--------|:----------|
|accountDomain|String|用于登录的用户帐户的域。|
|帐户|String|用于登录的用户帐户的帐户名。|
|accountType|String|每个 Windows 定义的用户帐户类型。 可取值为：`unknown`、`standard`、`power`、`administrator`。|
|firstSeenDateTime|DateTimeOffset|发生此用户帐户的最早登录（由提供程序确定的时间段）的日期时间。 时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。|
|lastSeenDateTime|DateTimeOffset|发生此用户帐户的最新登录的日期时间。 时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。|
|logonId|String|用户登录 ID。|
|了 logontypes|String 集合|从第一次查看之时开始，登录用户看到的登录类型的集合。 可取值为：`unknown`、`interactive`、`remoteInteractive`、`network`、`batch`、`service`。|

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
