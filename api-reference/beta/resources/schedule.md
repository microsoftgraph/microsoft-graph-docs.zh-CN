---
title: 计划资源类型
description: 团队中的 schedulingGroups、shift、timeOffReasons 和 timesOff 集合。
author: aaku
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 0aff494a1a5fdc4c710272e279089ff35fbd51fa
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2022
ms.locfileid: "63335190"
---
# <a name="schedule-resource-type"></a>计划资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

团队中的 [schedulingGroup](schedulinggroup.md) 对象、 [shift](shift.md) 对象、 [timeOffReason](timeoffreason.md) 对象和 [timeOff](timeoff.md) [对象的集合](../resources/team.md)。 

## <a name="methods"></a>方法

| 方法       | 返回类型  |说明|
|:---------------|:--------|:----------|
|[创建或替换日程安排](../api/team-put-schedule.md) | [日程安排](schedule.md) | 创建或替换计划。|
|[获取日程安排](../api/schedule-get.md) | [日程安排](schedule.md) | 获取计划。|
|[共享](../api/schedule-share.md) | 无 | 与计划成员共享计划时间范围。|

## <a name="properties"></a>属性
|名称                   |类型           |说明                                                                                                                                      |
|-----------------------|---------------|-------------------------------------------------------------------------------------------------------------------------------------------------|
| id                    |string  |计划的 ID。|
| enabled               |Boolean    | 指示是否为团队启用日程安排。 必需项。|
| timeZone              |string  | 使用 tz 数据库格式指示计划团队的时区。 必需项。|
| provisionStatus       |operationStatus    | 计划预配的状态。 可能的值为 、、`notStarted``running``completed`、`failed`。 |
| provisionStatusCode   |string  | 有关计划设置失败原因的其他信息。 |
| timeClockEnabled                  |Boolean  | 指示是否对计划启用时间时钟。             |
| openShiftsEnabled                 |Boolean  | 指示是否针对计划启用打开的班次。             | 
| swapShiftsRequestsEnabled                 |Boolean| 指示是否针对计划启用交换班次请求。             |
| offerShiftRequestsEnabled                 |Boolean  | 指示是否针对计划启用产品/服务班次请求。             | 
| timeOffRequestsEnabled                    |Boolean | 指示是否对计划启用请假请求。             | 



## <a name="relationships"></a>关系
|名称                   |类型           |说明                                                                                                                                      |
|-----------------------|---------------|-------------------------------------------------------------------------------------------------------------------------------------------------|
| shifts   | [shift](shift.md) 集合  | 计划中的班次。 |
| timesOff   |[timeOff](timeoff.md) 集合  | 计划中的时间关闭实例。 |
| timeOffReasons   |[timeOffReason](timeoffreason.md) 集合  | 计划中请假的一组原因。 |
| schedulingGroups   |[schedulingGroup](schedulinggroup.md) 集合  | 计划中的用户逻辑分组通常 (角色) 。 |
| openshifts   |[openShift](openshift.md) 集合 | 计划中计划组中打开的班次集。 |
| workforceintegrations   |[workforceIntegration](workforceintegration.md) 集合  | 每个团队的员工集成实例，其出站数据流针对支持的实体 (同步更改) 。 |
| swapshiftchangerequests   |[swapShiftsChangeRequest](swapshiftschangerequest.md) 集合  | 计划中班次的交换请求。 |
| openshiftchangerequests   |[openShiftChangeRequest](openshiftchangerequest.md) 集合  | 计划中的打开的班次请求。 |
| timeoffrequest   |[timeOffRequest](timeoffrequest.md) 集合  | 计划中的请假请求。 |

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


