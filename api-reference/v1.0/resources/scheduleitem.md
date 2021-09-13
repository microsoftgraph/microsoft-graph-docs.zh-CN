---
title: scheduleItem 资源类型
description: 描述用户与用户默认日历上的实际事件相对应的可用性的项目。 此项还适用于会议室 (设备) 资源。
ms.localizationpriority: medium
author: harini84
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 86dc2c44f93635bd38363984d7dda8debe21147f
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59035967"
---
# <a name="scheduleitem-resource-type"></a>scheduleItem 资源类型

命名空间：microsoft.graph

描述用户与用户默认日历上的实际事件相对应的可用性的项目。 此项还适用于会议室 (设备) 资源。

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|end |[dateTimeTimeZone](datetimetimezone.md) |相应事件结束的日期、时间和时区。 |
|isPrivate |Boolean |相应事件的敏感度。 如此 如果事件标记为 `private` ， 假 否则。 可选。|
|位置 |String | 举行或参加相应事件的位置。 可选。|
|start |[dateTimeTimeZone](datetimetimezone.md) |相应事件开始的日期、时间和时区。 |
|status |freeBusyStatus | 用户或资源在相应事件期间的可用性状态。 可能的值包括 `free`、`tentative`、`busy`、`oof`、`workingElsewhere`、`unknown`。 |
|subject |String | 相应事件的主题行。 可选。|


## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "isPrivate",
    "location",
    "subject"
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
<!--
{
  "type": "#page.annotation",
  "description": "scheduleItem resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}
-->

