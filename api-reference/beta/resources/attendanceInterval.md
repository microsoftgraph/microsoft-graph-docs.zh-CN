---
title: attendanceInterval 资源类型
description: 包含与 attendanceRecord 中的出席间隔关联的信息。
author: jsandoval-msft
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: d1746adc802534f72aa9d139c6a16d8da62dd9fd
ms.sourcegitcommit: d033e7de12bccf92efcbe40c7b671e419a3e5b94
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/17/2021
ms.locfileid: "51882656"
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
