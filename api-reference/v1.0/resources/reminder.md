---
title: 提醒资源类型
description: 用户日历中的事件提醒。
localization_priority: Normal
author: harini84
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 1cb61064b05668193947043998749e6306d3d606
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48002952"
---
# <a name="reminder-resource-type"></a>提醒资源类型

命名空间：microsoft.graph

用户[日历](calendar.md)中的[事件](event.md)提醒。

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|changeKey|String|标识提醒的版本。每次提醒更改时，**changeKey** 也将更改。这样，Exchange 可以将更改应用于该对象的正确版本。|
|eventEndTime|[DateTimeTimeZone](datetimetimezone.md)|事件结束的日期、时间和时区。|
|eventId|String|事件的唯一 ID。只读。|
|eventLocation|[位置](location.md)|事件的位置。|
|eventStartTime|[DateTimeTimeZone](datetimetimezone.md)|事件开始的日期、时间和时区。|
|eventSubject|String|事件的主题行文本。|
|eventWebLink|String|要在 Web 上的 Outlook 中打开事件的 URL。<br/><br/>如果你通过 Web 上的 Outlook 登录邮箱，该事件将在浏览器中打开。如果你尚未使用浏览器登录，系统将提示你登录。<br/><br/>可以从 iFrame 中访问此 URL。|
|reminderFireTime|[DateTimeTimeZone](datetimetimezone.md)|设置提醒发生的日期、时间和时区。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.reminder"
}-->

```json
{
  "changeKey": "string",
  "eventEndTime": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "eventId": "string",
  "eventLocation": {"@odata.type": "microsoft.graph.location"},
  "eventStartTime": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "eventSubject": "string",
  "eventWebLink": "string",
  "reminderFireTime": {"@odata.type": "microsoft.graph.dateTimeTimeZone"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "reminder resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

