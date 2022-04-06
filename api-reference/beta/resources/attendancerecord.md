---
title: attendanceRecord 资源类型
description: 包含与 meetingAttendanceReport 中的与会者记录关联的信息。
author: mkhribech
ms.localizationpriority: medium
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 957daa2412997f6db32de8f57ae196edd89e4b4e
ms.sourcegitcommit: 0e7927f34b7e55d323acbf281e11560cb40a89ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2022
ms.locfileid: "63672082"
---
# <a name="attendancerecord-resource-type"></a>attendanceRecord 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

包含与 [meetingAttendanceReport](meetingattendancereport.md) 中的与会者记录关联的信息。

## <a name="methods"></a>方法

|方法|返回类型|说明|
|:---|:---|:---|
|[列出 attendanceRecords](../api/attendancerecord-list.md)|[attendanceRecord](../resources/attendancerecord.md) 集合|获取 [attendanceRecord 对象](../resources/attendancerecord.md) 及其属性的列表。|

## <a name="properties"></a>属性

| 属性            | 类型    | 说明|
|:--------------------|:--------|:-----------|
| attendanceIntervals | [attendanceInterval](attendanceinterval.md) 集合 | 加入和离开会议之间的时间段列表。 |
| emailAddress | String | 与此 at此操作记录关联的用户的电子邮件地址。 |
| identity | [identity](identity.md) | 与此 atance 记录关联的用户的标识。 |
| role | String | 与会者的角色。 可能的值为： `None`、 `Attendee`、 `Presenter`和 `Organizer`。  |
| registrantId | String | [meetingRegistrant 的唯一标识符](meetingregistrantbase.md)。 参与者已注册会议时显示。 |
| totalAttendanceInSeconds | Int32 | 总出席持续时间（以秒表示）。 |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.attendanceRecord",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->

```json
{
  "@odata.type": "#microsoft.graph.attendanceRecord",
  "emailAddress": "String",
  "totalAttendanceInSeconds": "Int32",
  "role": "String(None|Attendee|Presenter|Organizer)",
  "registrantId": "String",
  "identity": {
    "@odata.type": "#microsoft.graph.identity"
  },
  "attendanceIntervals": [
    {
      "@odata.type": "#microsoft.graph.attendanceInterval"
    }
  ]
}
```
