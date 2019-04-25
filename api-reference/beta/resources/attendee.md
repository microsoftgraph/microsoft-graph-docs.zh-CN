---
title: 与会者资源类型
description: 会议与会者。 这可以是人或在 Exchange 服务器上为租户设置的资源（例如会议室或设备）。
localization_priority: Normal
ms.openlocfilehash: d50b6756c7d0077ec95f10988d06fa2ff81631fc
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32544069"
---
# <a name="attendee-resource-type"></a>与会者资源类型

会议与会者。 这可以是人或在 Exchange 服务器上为租户设置的资源（例如会议室或设备）。

由 [attendeeBase](attendeebase.md) 派生。

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|状态|[ResponseStatus](responsestatus.md)|事件与会者的响应（无、接受、拒绝等）和发送响应的日期时间。|
|类型|String|与会者类型：`required`、`optional`、`resource`。|
|emailAddress|[emailAddress](emailaddress.md)|添加与会者姓名和 SMTP 地址。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.attendeeBase",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.attendee"
}-->

```json
{
  "status": {"@odata.type": "microsoft.graph.responseStatus"},
  "type": "String",
  "emailAddress": {"@odata.type": "microsoft.graph.emailAddress"}
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "attendee resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
