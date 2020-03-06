---
title: 与会者资源类型
description: 会议与会者。 这可以是人或在 Exchange 服务器上为租户设置的资源（例如会议室或设备）。
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 1cadb1ca6d2ab1168c3c7f9ff2b182b57112bfb0
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42532091"
---
# <a name="attendee-resource-type"></a>与会者资源类型

命名空间：microsoft.graph

会议与会者。 这可以是人或在 Exchange 服务器上为租户设置的资源（例如会议室或设备）。

由 [attendeeBase](attendeebase.md) 派生。

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|状态|[ResponseStatus](responsestatus.md)|事件与会者的响应（无、接受、拒绝等）和发送响应的日期时间。|
|type|字符串|与会者类型：`required`、`optional`、`resource`。|
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
