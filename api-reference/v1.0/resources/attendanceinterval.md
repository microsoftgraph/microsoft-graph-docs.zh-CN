---
title: attendanceInterval 资源类型
description: 包含与 attendanceRecord 中的出席间隔关联的信息。
author: mkhribech
ms.localizationpriority: medium
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 643dcfa2e7c032fba93af164271150c41b6693b2
ms.sourcegitcommit: 1a607ea5bee096944e0fea14167d372f1ff652f6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/16/2021
ms.locfileid: "61547518"
---
# <a name="attendanceinterval-resource-type"></a>attendanceInterval 资源类型

命名空间：microsoft.graph

包含与 [attendanceRecord](attendancerecord.md)中的出席间隔相关联的信息。

## <a name="properties"></a>属性

| 属性            | 类型    | 说明|
|:--------------------|:--------|:-----------|
| durationInSeconds | Int32 | 会议间隔的持续时间（以秒为单位）;即 **joinDateTime** 和 **leaveDateTime 之间的差** 值。 |
| joinDateTime | 日期时间 | 参与者以 UTC 加入的时间。 |
| leaveDateTime | 日期时间 | 与会者以 UTC 离开的时间。 |

> [!TIP]
> 当缺少数据时 **，joinDateTime** 或 **leaveDateTime** 的值将设置为 `null` **，durationInSeconds** 的值将在 `0` Get [meetingAttendanceReport](/graph/api/meetingattendancereport-get?view=graph-rest-v1.0&preserve-view=true) 方法的响应正文中设置为 。

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
