---
title: 计划资源类型
description: 团队中的 schedulingGroups、倒班、timeOffReasons 和 timesOff 的集合。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: de3662fcf3c5a8e50493e365f6a10a8641a451df
ms.sourcegitcommit: 081cacecb4960aabc9e1011d12f06fe9ecf7d188
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/16/2019
ms.locfileid: "30657509"
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
| id                    |`string`  |的 ID `schedule`。|
| enabled               |`bool`    | 指示是否为团队启用了计划。 必需。|
| timeZone              |`string`  | 指示使用 tz 数据库格式的日程安排团队的时区。 必需。|
| provisionStatus       |`enum`    | 调度设置的状态。 |
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
  "suppressions": [
    "Error: /api-reference/beta/resources/schedule.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
