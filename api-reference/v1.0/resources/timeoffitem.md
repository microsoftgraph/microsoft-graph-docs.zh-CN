---
title: timeOffItem 资源类型
description: 表示 timeOff 的版本。
author: akumar39
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType_
ms.openlocfilehash: a710c1c2de9a2ff127b19a083a3c90d5bfface5a
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/11/2021
ms.locfileid: "50720840"
---
# <a name="timeoffitem-resource-type"></a>timeOffItem 资源类型

命名空间：microsoft.graph

表示 [timeOff 的版本](timeoff.md)。

## <a name="properties"></a>属性
| 属性                         | 类型                    | 说明                                                                                                                                                                        |
|------------------------------|-------------------------|---------------------------------------------------------------------------------------------|
| timeOffReasonId               | string                  | 的 `timeOffReason` `timeOffItem` ID。 必需。     |
| startDateTime               | DateTimeOffset                  | 的开始日期和时间 `timeOffItem` 。 必需。 时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。 |
| endDateTime               | DateTimeOffset                  | 的结束日期和时间 `timeOffItem` 。 必需。 时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。 |
| theme | scheduleEntityTheme   | 支持的颜色：白色;blue;绿色;紫色;粉色;黄色;灰色;darkBlue;darkGreen;darkPurple;darkPink;darkYellow。 |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.timeOffItem"
}-->
```json
{
  "timeOffReasonId": "String",
  "startDateTime": "String (timestamp)",
  "endDateTime": "String (timestamp)",
  "theme": "pink"
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "timeOffItem resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->

