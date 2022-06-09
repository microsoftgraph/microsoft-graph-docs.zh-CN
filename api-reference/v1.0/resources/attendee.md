---
title: 与会者资源类型
description: 会议与会者。 这可以是人或在 Exchange 服务器上为租户设置的资源（例如会议室或设备）。
ms.localizationpriority: medium
author: harini84
ms.prod: calendar
doc_type: resourcePageType
ms.openlocfilehash: 15c6dbc48e07b6193ca99c7dde9239b6bcf4ec50
ms.sourcegitcommit: 4b852b92535fba8af9b2bbd6f55dc16aced9ef7e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/09/2022
ms.locfileid: "65971187"
---
# <a name="attendee-resource-type"></a>与会者资源类型

命名空间：microsoft.graph

会议与会者。 这可以是人或在 Exchange 服务器上为租户设置的资源（例如会议室或设备）。

由 [attendeeBase](attendeebase.md) 派生。

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|emailAddress|[emailAddress](emailaddress.md)|添加与会者姓名和 SMTP 地址。|
|proposedNewTime|[timeSlot](timeslot.md)|与会者为开始和结束会议请求建议的备用日期/时间。 如果与会者未提出其他时间，则此属性不包括在 GET 事件的响应中。|
|状态|[ResponseStatus](responsestatus.md)|事件与会者的响应（无、接受、拒绝等）和发送响应的日期时间。|
|type|字符串|与会者类型：`required`、`optional`、`resource`。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.attendeeBase",
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
<!-- {
  "type": "#page.annotation",
  "description": "attendee resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

