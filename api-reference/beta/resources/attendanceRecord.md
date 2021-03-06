---
title: attendanceRecord 资源类型
description: 包含与与会者报告中的与会者记录关联的信息。
author: mkhribech
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 20beeca97c790b8743c9038e7fddf0b5c6f69534
ms.sourcegitcommit: 7abb0672a38a6d9b11a2e0d2cc221222cb8358bb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/11/2021
ms.locfileid: "52896499"
---
# <a name="attendancerecord-resource-type"></a>attendanceRecord 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

包含与与会者报告中的与会者记录关联的信息。

## <a name="properties"></a>属性

| 属性            | 类型    | 说明|
|:--------------------|:--------|:-----------|
| identity | [标识](identity.md) | 标识符，例如显示名称。 |
| emailAddress | String | 电子邮件地址。 |
| totalAttendanceInSeconds | Int32 | 总出席持续时间（以秒表示）。 |
| attendanceIntervals | [attendanceInterval](attendanceInterval.md) 集合 | 加入和离开之间的时间段列表。 |
| role | String | 与会者的角色。 可能的值为 `None` `Attendee` 、、 `Presenter` 和 `Organizer` 。  |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.attendanceRecord"
}-->

```json

{
    "emailAddress": "String",
    "totalAttendanceInSeconds": "Int32",
    "role": "String(None|Attendee|Presenter|Organizer)",
    "identity": {"@odata.type": "#microsoft.graph.identity"},
    "attendanceIntervals": [{"@odata.type": "#microsoft.graph.attendanceInterval"}]
}

```
