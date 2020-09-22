---
title: attendeeBase 资源类型
description: 与会者类型。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: harini84
ms.openlocfilehash: 947b137d3619cca6cc9a6faa8c3f3e761d15fb37
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48040159"
---
# <a name="attendeebase-resource-type"></a>attendeeBase 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

与会者类型。

由 [recipient](recipient.md) 派生。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.attendeeBase"
}-->

```json
{
  "type": "String",
  "emailAddress": {"@odata.type": "microsoft.graph.emailAddress"}
}

```
## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|type|String| 与会者类型。可取值为：`required`、`optional`、`resource`。目前，如果与会者是人员，[findMeetingTimes](../api/user-findmeetingtimes.md) 始终认为人员是 `Required` 类型。|
|emailAddress|[emailAddress](emailaddress.md)|添加与会者姓名和 SMTP 地址。|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "attendeeBase resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


