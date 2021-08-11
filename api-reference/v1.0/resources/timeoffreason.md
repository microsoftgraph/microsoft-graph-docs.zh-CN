---
title: timeOffReason 资源类型
description: 表示在计划中请假的有效原因。
author: akumar39
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType_
ms.openlocfilehash: fc16be17d4aecb377d25eff7770f3e8b3881f5f1ce936310a78eae1d0d5476a7
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54159804"
---
# <a name="timeoffreason-resource-type"></a>timeOffReason 资源类型

命名空间：microsoft.graph

表示计划 中的 [timeOff](timeoff.md) 实例的有效 [原因](schedule.md)。

## <a name="methods"></a>方法

| 方法       | 返回类型  |Description|
|:---------------|:--------|:----------|
|[List](../api/schedule-list-timeoffreasons.md) | [timeOffReason](timeoffreason.md) 集合 | 获取计划中的 **timeOffReason** 列表。|
|[Create](../api/schedule-post-timeoffreasons.md) | [timeOffReason](timeoffreason.md) | 创建新的 **timeOffReason**。|
|[Get](../api/timeoffreason-get.md) | [timeOffReason](timeoffreason.md) | 按 ID **获取 timeOffReason。**|
|[Replace](../api/timeoffreason-put.md) | [timeOffReason](timeoffreason.md) | 替换 **timeOffReason**。|
|[删除](../api/timeoffreason-delete.md) | 无 | 将 **timeOffReason** 标记为非活动状态。|

## <a name="properties"></a>属性
|名称          |类型           |说明                                                                                 |
|--------------|---------------|--------------------------------------------------------------------------------------------|
| id            |`string`      |`timeOffReason` 的 ID。|
| displayName               | `string`                  | **timeOffReason 的名称**。 必填。 |
| iconType | `timeOffReasonIconType`   | 支持的图标类型：无;car;calendar;running;plane;firstAid;一个notWorking;clock;将duty;globe;cup;phone;weather;umbrella;bankgyBank;dog;一个trafficCone;pin;。 必填。 |
| isActive          |`Boolean`      | 指示在创建新实体或更新现有实体时是否可以使用 **timeOffReason。** 必填。 |
| createdDateTime       |`DateTimeOffset`        |首次创建 **此 timeOffReason** 的时间戳。 时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。 |
| lastModifiedDateTime      |`DateTimeOffset`         |上次更新 **TimeOffReason** 的时间戳。 时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。 |
| lastModifiedBy        | [identitySet](identityset.md)        |上次更新的标识 **这次是OffReason**。|

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

