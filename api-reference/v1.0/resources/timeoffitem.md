---
title: timeOffItem 资源类型
description: 表示 timeOff 的版本。
author: akumar39
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType_
ms.openlocfilehash: 349b37cfdc414323d35ee4648009fd8ab4d59bbf
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59019102"
---
# <a name="timeoffitem-resource-type"></a>timeOffItem 资源类型

命名空间：microsoft.graph

表示 [timeOff 的版本](timeoff.md)。

## <a name="properties"></a>属性
| 属性                         | 类型                    | 说明                                                                                                                                                                        |
|------------------------------|-------------------------|---------------------------------------------------------------------------------------------|
| timeOffReasonId               | 字符串                  | 的 `timeOffReason` `timeOffItem` ID。 必填。     |
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

