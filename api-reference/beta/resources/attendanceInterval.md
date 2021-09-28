---
title: attendanceInterval 资源类型
description: 包含与 attendanceRecord 中的出席间隔关联的信息。
author: mkhribech
ms.localizationpriority: medium
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 55b218cfcecb4f2f7d3d597881b612e36fe42860
ms.sourcegitcommit: 84d9a50dfa9526a207696c69d92381c8763d986a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/28/2021
ms.locfileid: "59979248"
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

> [!TIP]
> 当缺少数据时 **，joinDateTime** 或 **leaveDateTime** 的值将设置为 `null` **，durationInSeconds** 的值将在获取会议与会者报告操作的响应正文中设置为 。 `0` [](/graph/api/onlinemeeting-get?view=graph-rest-beta&preserve-view=true)

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
