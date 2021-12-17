---
title: meetingAttendanceReport 资源类型
description: 包含与会议出席报告关联的信息。
author: mkhribech
ms.localizationpriority: medium
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: a46ab1bcdb0c8a901b5257184e96b72c79801ce7
ms.sourcegitcommit: 1a607ea5bee096944e0fea14167d372f1ff652f6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/16/2021
ms.locfileid: "61547663"
---
# <a name="meetingattendancereport-resource-type"></a>meetingAttendanceReport 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

包含与会议出席报告关联的信息。

与会者报告是联机会议项目。 有关详细信息，请参阅 [联机会议项目与权限](/graph/cloud-communications-online-meeting-artifacts)。

## <a name="methods"></a>方法

|方法|返回类型|说明|
|:---|:---|:---|
|[列出 meetingAttendanceReports](../api/meetingattendancereport-list.md)|[meetingAttendanceReport](../resources/meetingattendancereport.md) 集合|获取  [meetingAttendanceReport](../resources/meetingattendancereport.md) 对象及其属性的列表。|
|[获取 meetingAttendanceReport](../api/meetingattendancereport-get.md)|[meetingAttendanceReport](../resources/meetingattendancereport.md)|读取 [meetingAttendanceReport](../resources/meetingattendancereport.md) 对象的属性和关系。|

## <a name="properties"></a>属性

| 属性              | 类型                                               | 说明                     |
|:----------------------|:---------------------------------------------------|:--------------------------------|
| id                    | String   | 与会者报告的唯一标识符。 只读。 |
| meetingEndDateTime    | DateTimeOffset | 会议结束的 UTC 时间。 只读。   |
| meetingStartDateTime  | DateTimeOffset | 会议开始的 UTC 时间。 只读。   |
| totalParticipantCount | Int32 | 参与者总数。 只读。  |

## <a name="relationships"></a>关系

| 关系 | 类型 | 说明 |
| ------------ | ---- | ----------- |
| attendanceRecords | [attendanceRecord](attendanceRecord.md) 集合 | 考勤报告的与会者记录列表。 只读。 |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.meetingAttendanceReport"
}-->

```json
{
  "@odata.type": "#microsoft.graph.meetingAttendanceReport",
  "id": "String(identifier)",
  "meetingEndDateTime": "String (timestamp)",
  "meetingStartDateTime": "String (timestamp)",
  "totalParticipantCount": "Int32",

  "attendanceRecords": [{"@odata.type": "#microsoft.graph.attendanceRecord"}]
}
```
