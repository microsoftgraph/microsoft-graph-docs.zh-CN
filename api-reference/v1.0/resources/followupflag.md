---
title: followupFlag 资源类型
description: '允许用户在项中设置标记，供用户稍后跟进。 '
ms.localizationpriority: medium
author: abheek-das
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 17d9b1d2e12a33d5df53acf434489377089d89ea
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59078852"
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

