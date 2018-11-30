---
title: attendeeBase 资源类型
description: 与会者类型。
ms.openlocfilehash: 2d7d3889cd65886eba4cf9356862417928ed3296
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27041474"
---
# <a name="attendeebase-resource-type"></a>attendeeBase 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

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
|type|字符串| 与会者类型。可取值为：`required`、`optional`、`resource`。目前，如果与会者是人员，[findMeetingTimes](../api/user-findmeetingtimes.md) 始终认为人员是 `Required` 类型。|
|emailAddress|[emailAddress](emailaddress.md)|添加与会者姓名和 SMTP 地址。|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "attendeeBase resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->