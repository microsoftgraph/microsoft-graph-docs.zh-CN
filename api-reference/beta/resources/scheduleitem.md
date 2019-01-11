---
title: scheduleItem 资源类型
description: " > **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。"
localization_priority: Normal
ms.openlocfilehash: e5d14826a27153af27648484554ec864d62ed6c7
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27890431"
---
# <a name="scheduleitem-resource-type"></a>scheduleItem 资源类型

 > **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。
 
介绍了在用户的默认日历上与实际事件对应的用户的可用性的项。 此项适用于资源以及。

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|end |[dateTimeTimeZone](datetimetimezone.md) |日期、 时间和结束对应的事件的时区。 |
|isPrivate |布尔 |区分大小写的对应的事件。 如果事件标记为`private`，则返回 false 否则为。 |
|location |字符串 | 相应的事件是保留或从参加的位置。 可选。|
|start |[dateTimeTimeZone](datetimetimezone.md) |日期、 时间和相应事件开始的时区。 |
|status |字符串 | 可用性的用户或资源的相应事件执行过程的状态。 可能的值为： `free`， `tentative`， `busy`， `oof`， `workingElsewhere`， `unknown`。 |
|subject |字符串 | 相应的事件的主题行。 可选。|


## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.scheduleItem"
}-->

```json
{
  "end": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "isPrivate": true,
  "location": "String",
  "start": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "status": "String",
  "subject": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "scheduleItem resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
