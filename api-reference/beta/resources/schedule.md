---
title: 计划资源类型
description: 团队中的 schedulingGroups、倒班、timeOffReasons 和 timesOff 的集合。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 48b3b5c118a39442469bc6155068664fcebe0ec2
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33343519"
---
# <a name="schedule-resource-type"></a>计划资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

一个[团队](../resources/team.md)中的[schedulingGroup](schedulinggroup.md)对象、 [shift](shift.md)对象、 [timeOffReason](timeoffreason.md)对象和[timeOff](timeoff.md)对象的集合。 

## <a name="methods"></a>方法

| 方法       | 返回类型  |说明|
|:---------------|:--------|:----------|
|[创建或替换计划](../api/team-put-schedule.md) | [设定](schedule.md) | 创建或替换`schedule`。|
|[获取日程安排](../api/schedule-get.md) | [设定](schedule.md) | 获取`schedule`。|
|[share](../api/schedule-share.md) | 无 | 与 schedule `schedule`成员共享时间范围。|

## <a name="properties"></a>属性
|名称                   |类型           |说明                                                                                                                                      |
|-----------------------|---------------|-------------------------------------------------------------------------------------------------------------------------------------------------|
| id                    |`string`  |`schedule` 的 ID。|
| enabled               |`bool`    | 指示是否为团队启用了计划。 必需。|
| timeZone              |`string`  | 指示使用 tz 数据库格式的日程安排团队的时区。 必需。|
| provisionStatus       |`operationStatus`    | 调度设置的状态。 可能的值为`notStarted`、 `running`、 `completed`、 `failed`。 |
| provisionStatusCode   |`string`  | 有关计划设置失败原因的其他信息。 |


## <a name="relationships"></a>关系
|名称                   |类型           |说明                                                                                                                                      |
|-----------------------|---------------|-------------------------------------------------------------------------------------------------------------------------------------------------|
| 发生   |`collection(shift)`  | 日程中的班次。 |
| timesOff   |`collection(timeOff)`  | 计划中的超时实例。 |
| timeOffReasons   |`collection(timeOffReason)`  | 时间安排中的时间的一组原因。 |
| schedulingGroups   |`collection(schedulingGroup)`  | 按日程安排的用户的逻辑分组 (通常按角色)。 |


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
