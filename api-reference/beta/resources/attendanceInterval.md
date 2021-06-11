---
title: attendanceInterval 资源类型
description: 包含与 attendanceRecord 中的出席间隔关联的信息。
author: mkhribech
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 13b4e20a5233b865dd5417eed4d159bce07c8717
ms.sourcegitcommit: 7abb0672a38a6d9b11a2e0d2cc221222cb8358bb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/11/2021
ms.locfileid: "52896513"
---
# <a name="attendanceinterval-resource-type"></a>attendanceInterval 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

包含与 attendanceRecord 中的出席间隔关联的信息。

## <a name="properties"></a>属性

| 属性            | 类型    | 说明|
|:--------------------|:--------|:-----------|
| joinDateTime | 日期时间 | 加入 UTC 时间与会者的时间。 |
| leaveDateTime | 日期时间 | 时间与会者以 UTC 时间离开。 |
| durationInSeconds | Int32 | 会议间隔的持续时间（以秒为单位）;即 **joinDateTime** 和 **leaveDateTime 之间的差** 值。 |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.attendanceInterval"
}-->

```json

{
    "joinDateTime": "String (timestamp)",
    "leaveDateTime": "String (timestamp)",
    "durationInSeconds": "Int32"
}
    
```
