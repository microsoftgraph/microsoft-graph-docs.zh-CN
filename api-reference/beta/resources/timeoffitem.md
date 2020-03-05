---
title: timeOffItem 资源类型
description: 表示 timeOff 的版本。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType_
ms.openlocfilehash: 019bb366ad9d960fd2eff6365ef987f186a0d6c3
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519727"
---
# <a name="timeoffitem-resource-type"></a>timeOffItem 资源类型

命名空间： microsoft. graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示[timeOff](timeoff.md)的版本。

## <a name="properties"></a>属性
| 属性                         | 类型                    | 说明                                                                                                                                                                        |
|------------------------------|-------------------------|---------------------------------------------------------------------------------------------|
| timeOffReasonId               | string                  | `timeOffReason`此`timeOffItem`的的 ID。 必填。     |
| startDateTime               | DateTimeOffset                  | 的开始日期和时间`timeOffItem`。 必填。 时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时间。 例如，2014 年 1 月 1 日午夜 (UTC) 如下所示：“2014-01-01T00:00:00Z”。 |
| endDateTime               | DateTimeOffset                  | 的结束日期和时间`timeOffItem`。 必填。 时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时间。 例如，2014 年 1 月 1 日午夜 (UTC) 如下所示：“2014-01-01T00:00:00Z”。 |
| theme | scheduleEntityTheme   | 支持的颜色：白色;变为表示紫粉色黄色底纹darkBlue;darkGreen;darkPurple;darkPink;darkYellow. |

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
