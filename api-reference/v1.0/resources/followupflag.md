---
title: followupFlag 资源类型
description: '允许在项目中设置标志，以便用户以后跟进。 '
localization_priority: Normal
author: svpsiva
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: ab7894c7cec99387577994a96e459765ddf2793e
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48018240"
---
# <a name="followupflag-resource-type"></a>followupFlag 资源类型

命名空间：microsoft.graph


允许在项目中设置标志，以便用户以后跟进。

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|completedDateTime|[dateTimeTimeZone](datetimetimezone.md)|完成跟进的日期和时间。|
|dueDateTime|**dateTimeTimeZone**|后续工作的结束日期和时间。 **注意**：若要设置截止日期，您还必须指定 `startDateTime` ; 否则，你将收到 `400 Bad Request` 响应。|
|flagStatus|followupFlagStatus|项目的跟进状态。 可取值为：`notFlagged`、`complete` 和 `flagged`。|
|startDateTime|**dateTimeTimeZone**|要开始的跟进的日期和时间。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.followupFlag"
}-->

```json
{
  "completedDateTime": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "dueDateTime": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "flagStatus": "String",
  "startDateTime": {"@odata.type": "microsoft.graph.dateTimeTimeZone"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "followupFlag resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

