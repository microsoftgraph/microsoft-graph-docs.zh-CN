---
title: shiftActivity 资源类型
description: 表示班次中的活动。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: de42cb7722e7d24ba105880790fa2071c4714091
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/11/2021
ms.locfileid: "50721122"
---
# <a name="shiftactivity-resource-type"></a>shiftActivity 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示班次 [中的活动](shift.md)。

## <a name="properties"></a>属性
| 属性                         | 类型                    | 说明                                                                                                                                                                        |
|------------------------------|-------------------------|---------------------------------------------------------------------------------------------|
| isPaid               | `bool`                  | 指示是否应该 `microsoft.graph.user` 在活动期间为活动支付该费用 `shift` 。 必需。    |
| startDateTime               | `DateTimeOffset`                  | 的开始日期和时间 `shiftActivity` 。 时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。 必需。 |
| endDateTime               | `DateTimeOffset`                  | 的结束日期和时间 `shiftActivity` 。 时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。 必需。    |
| code               | `string`                  | 客户定义的 `shiftActivity` 代码。 必需。    |
| displayName               | `string`                  | `shiftActivity`的名称。 此为必需属性。    |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.shiftActivity"
}-->
```json
{
  "isPaid": true,
  "startDateTime": "2019-03-11T15:00:00Z",
  "endDateTime": "2019-03-11T15:15:00Z",
  "code": "",
  "displayName": "Lunch"
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "shiftActivity resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


