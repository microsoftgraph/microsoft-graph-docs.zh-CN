---
title: 与会者资源类型
description: 会议与会者。 这可以是人或在 Exchange 服务器上为租户设置的资源（例如会议室或设备）。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: outlook
author: harini84
ms.openlocfilehash: ec43db868c2934d569bf62e8e808d755b9d2cffc
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48040166"
---
# <a name="attendee-resource-type"></a>与会者资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

会议与会者。 这可以是人或在 Exchange 服务器上为租户设置的资源（例如会议室或设备）。

由 [attendeeBase](attendeebase.md) 派生。

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|emailAddress|[emailAddress](emailaddress.md)|添加与会者姓名和 SMTP 地址。|
|proposedNewTime|[timeSlot](timeslot.md)|与会者为开始和结束会议请求建议的备用日期/时间。 如果与会者尚未建议其他时间，则 GET 事件响应中不包含此属性。|
|状态|[ResponseStatus](responsestatus.md)|事件与会者的响应（无、接受、拒绝等）和发送响应的日期时间。|
|type|String|与会者类型：`required`、`optional`、`resource`。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "proposedNewTime"
  ],
  "@odata.type": "microsoft.graph.attendee"
}-->

```json
{
  "emailAddress": {"@odata.type": "microsoft.graph.emailAddress"},
  "proposedNewTime": {"@odata.type": "microsoft.graph.timeSlot"},
  "status": {"@odata.type": "microsoft.graph.responseStatus"},
  "type": "String"
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "attendee resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


