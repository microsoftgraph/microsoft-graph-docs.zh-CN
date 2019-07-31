---
title: timeOffReason 资源类型
description: 在计划中花费时间的有效原因。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType_
ms.openlocfilehash: 62943670a0c87d34fd849e988ef5bf827aa6d72a
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35964279"
---
# <a name="timeoffreason-resource-type"></a>timeOffReason 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[计划](schedule.md)中[timeOff](timeoff.md)实例的有效原因。

## <a name="methods"></a>方法

| 方法       | 返回类型  |说明|
|:---------------|:--------|:----------|
|[创建 timeOffReason](../api/schedule-post-timeoffreasons.md) | [timeOffReason](timeoffreason.md) | 新建 `timeOffReason`。|
|[列出 timeOffReason](../api/schedule-list-timeoffreasons.md) | [timeOffReason](timeoffreason.md)集合 | 获取计划中 `timeOffReasons` 的列表。|
|[获取 timeOffReason](../api/timeoffreason-get.md) | [timeOffReason](timeoffreason.md) | 按 ID 获取 `timeOffReason`。|
|[替换 timeOffReason](../api/timeoffreason-put.md) | [timeOffReason](timeoffreason.md) | 更换 `timeOffReason`。|
|[删除 timeOffReason](../api/timeoffreason-delete.md) | 无 | 将 `timeOffReason` 标记为非活动状态。|

## <a name="properties"></a>属性
|名称          |类型           |说明                                                                                 |
|--------------|---------------|--------------------------------------------------------------------------------------------|
| id            |`string`      |`timeOffReason` 的 ID。|
| displayName               | `string`                  | 的名称`timeOffReason`。 必需。 |
| iconType | `timeOffReasonIconType`   | 支持的图标类型: 无;car式运行planefirstAid;dr.notWorking;构造juryDuty;投放cup of电话气候防护piggyBank;监控桩trafficCone;针sunny. 必需。 |
| isActive          |`Boolean`      | 指示在新建实体或更新现有实体时是否可以使用 `timeOffReason`。 必需。 |
| createdDateTime       |`DateTimeOffset`        |首次在其上创建`timeOffReason`此项的时间戳。 时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时间。 例如，2014 年 1 月 1 日午夜 (UTC) 如下所示：“2014-01-01T00:00:00Z”。 |
| lastModifiedDateTime      |`DateTimeOffset`         |对其最后更新的`timeOffReason`时间戳。 时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时间。 例如，2014 年 1 月 1 日午夜 (UTC) 如下所示：“2014-01-01T00:00:00Z”。 |
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
