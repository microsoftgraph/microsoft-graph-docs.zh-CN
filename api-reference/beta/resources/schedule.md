---
title: 计划资源类型
description: 团队中的 schedulingGroups、倒班、timeOffReasons 和 timesOff 的集合。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType_
ms.openlocfilehash: 6bc92b18bd0529066ef9ade2df9c6ccee9628add
ms.sourcegitcommit: 2ddc63c889fc2f4666aa55bca7ce0221ab899abf
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/07/2019
ms.locfileid: "39895376"
---
# <a name="schedule-resource-type"></a>计划资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

一个[团队](../resources/team.md)中的[schedulingGroup](schedulinggroup.md)对象、 [shift](shift.md)对象、 [timeOffReason](timeoffreason.md)对象和[timeOff](timeoff.md)对象的集合。 

## <a name="methods"></a>方法

| 方法       | 返回类型  |说明|
|:---------------|:--------|:----------|
|[创建或替换计划](../api/team-put-schedule.md) | [日程安排](schedule.md) | 创建或替换计划。|
|[获取日程安排](../api/schedule-get.md) | [日程安排](schedule.md) | 获取日程安排。|
|[共享](../api/schedule-share.md) | None | 与 schedule 成员共享计划时间范围。|

## <a name="properties"></a>属性
|名称                   |类型           |说明                                                                                                                                      |
|-----------------------|---------------|-------------------------------------------------------------------------------------------------------------------------------------------------|
| id                    |string  |计划的 ID。|
| enabled               |Boolean    | 指示是否为团队启用了计划。 必需。|
| timeZone              |string  | 指示使用 tz 数据库格式的日程安排团队的时区。 必需。|
| provisionStatus       |operationStatus    | 调度设置的状态。 可能的值为`notStarted`、 `running`、 `completed`、 `failed`。 |
| provisionStatusCode   |string  | 有关计划设置失败原因的其他信息。 |
| timeClockEnabled                  |Boolean  | 指示是否为计划启用了时间时钟。             |
| openShiftsEnabled                 |Boolean  | 指示是否为计划启用打开的班次。             | 
| swapShiftsRequestsEnabled                 |Boolean| 指示是否为计划启用交换倒班请求。             |
| offerShiftRequestsEnabled                 |Boolean  | 指示是否为计划启用了提供倒班请求。             | 
| timeOffRequestsEnabled                    |Boolean | 指示是否为计划启用时间关请求。             | 



## <a name="relationships"></a>关系
|名称                   |类型           |说明                                                                                                                                      |
|-----------------------|---------------|-------------------------------------------------------------------------------------------------------------------------------------------------|
| 发生   | [shift](shift.md)集合  | 日程中的班次。 |
| timesOff   |[timeOff](timeoff.md)集合  | 计划中的超时实例。 |
| timeOffReasons   |[timeOffReason](timeoffreason.md)集合  | 时间安排中的时间的一组原因。 |
| schedulingGroups   |[schedulingGroup](schedulinggroup.md) 集合  | 按日程安排的用户的逻辑分组（通常按角色）。 |
| openshifts   |[openShift](openshift.md)集合 | 计划组中的一组打开的班次。 |
| workforceintegrations   |[workforceIntegration](workforceintegration.md)集合  | 在同步更改通知（针对受支持的实体）中，每个团队的劳动力集成实例（针对受支持的实体的出站数据流）。 |
| swapshiftchangerequests   |[swapShiftsChangeRequest](swapshiftschangerequest.md)集合  | 计划中倒班的交换请求。 |
| openshiftchangerequests   |[openShiftChangeRequest](openshiftchangerequest.md)集合  | 计划中打开的班次请求。 |
| timeoffrequest   |[timeOffRequest](timeoffrequest.md)集合  | 计划中的休息时间请求。 |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.schedule"
}-->

```json
{
  "id": "833fc4df-c88b-4398-992f-d8afcfe41df2",
  "enabled": true,
  "timeZone": "America/Chicago",
  "provisionStatus": "Completed",
  "provisionStatusCode": null
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "schedule resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
