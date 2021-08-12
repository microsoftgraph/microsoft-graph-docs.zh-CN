---
title: followupFlag 资源类型
description: '允许用户在项中设置标记，供用户稍后跟进。 '
localization_priority: Normal
author: abheek-das
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: e45fd04fa084fbc26c8eb43316de2f25b70cc0b7e2d5aa721bfc26ab1cfd0063
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54180850"
---
# <a name="followupflag-resource-type"></a>followupFlag 资源类型

命名空间：microsoft.graph


允许用户在项中设置标记，供用户稍后跟进。

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|completedDateTime|[dateTimeTimeZone](datetimetimezone.md)|完成跟进的日期和时间。|
|dueDateTime|**dateTimeTimeZone**|跟进的完成日期和时间。 **注意**：若要设置截止日期，还必须指定 `startDateTime` ;否则，将获取 `400 Bad Request` 响应。|
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

