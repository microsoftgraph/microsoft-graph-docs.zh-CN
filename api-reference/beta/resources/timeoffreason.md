---
title: timeOffReason 资源类型
description: 在日程安排中请假的有效原因。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: b449f2cb4dcfcd73208d58f8e1e969b9a701e54b
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/11/2021
ms.locfileid: "50720184"
---
# <a name="timeoffreason-resource-type"></a>timeOffReason 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

计划中的 [timeOff](timeoff.md) 实例的有效 [原因](schedule.md)。

## <a name="methods"></a>方法

| 方法       | 返回类型  |说明|
|:---------------|:--------|:----------|
|[创建](../api/schedule-post-timeoffreasons.md) | [timeOffReason](timeoffreason.md) | 创建新的 **timeOffReason**。|
|[List](../api/schedule-list-timeoffreasons.md) | [timeOffReason](timeoffreason.md) 集合 | 获取计划中的 **timeOffReason** 列表。|
|[获取](../api/timeoffreason-get.md) | [timeOffReason](timeoffreason.md) | 按 **ID 获取 timeOffReason。**|
|[Replace](../api/timeoffreason-put.md) | [timeOffReason](timeoffreason.md) | 替换 **timeOffReason**。|
|[删除](../api/timeoffreason-delete.md) | 无 | 将 **timeOffReason** 标记为非活动状态。|

## <a name="properties"></a>属性
|名称          |类型           |说明                                                                                 |
|--------------|---------------|--------------------------------------------------------------------------------------------|
| id            |`string`      |`timeOffReason` 的 ID。|
| displayName               | `string`                  | `timeOffReason`的名称。 必需。 |
| iconType | `timeOffReasonIconType`   | 支持的图标类型：无;car;日历;正在运行;plane;firstAid;或notWorking;clock;juryDuty;全球;cup;phone;weather;umbrella;bankgyBank;dog;中;trafficCone;pin;。 必需。 |
| isActive          |`Boolean`      | 指示在新建实体或更新现有实体时是否可以使用 `timeOffReason`。 必需。 |
| createdDateTime       |`DateTimeOffset`        |首次创建此时间戳 `timeOffReason` 的时间戳。 时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。 |
| lastModifiedDateTime      |`DateTimeOffset`         |上次更新时间戳 `timeOffReason` 。 时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。 |
| lastModifiedBy        | [identitySet](identityset.md)        |上次更新 `timeOffReason` 的标识。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.timeOffReason",
  "baseType":"microsoft.graph.changeTrackedEntity"
}-->

```json
{
  "id": "String",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "displayName": "String",
  "iconType": "String",
  "isActive": true,
  "lastModifiedBy": { "@odata.type":"microsoft.graph.identitySet"}
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "timeOffReason resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


