---
title: timeOff 资源类型
description: 计划中的非工作单位。
author: aaku
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 21fc3395426ea6de8c564b6de92f7fa1fd32edf3
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2022
ms.locfileid: "63336898"
---
# <a name="timeoff-resource-type"></a>timeOff 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

计划中的非工作单位。

## <a name="methods"></a>Methods

| 方法       | 返回类型  |说明|
|:---------------|:--------|:----------|
|[创建](../api/schedule-post-timesoff.md) | [timeOff](timeoff.md) | 创建新的 **timeOff** 对象。|
|[列表](../api/schedule-list-timesoff.md) | [timeOff](timeoff.md) 集合 | 获取此 **计划中的 timeOff** 对象列表。|
|[获取](../api/timeoff-get.md) | [timeOff](timeoff.md) | 按 ID **获取 timeOff** 对象。|
|[Replace](../api/timeoff-put.md) | [timeOff](timeoff.md) | 替换 **timeOff** 对象。|
|[删除](../api/timeoff-delete.md) | 无 | 从 **计划中删除 timeOff** 对象。|

## <a name="properties"></a>属性
|名称          |类型           |说明                                                                                                                                      |
|--------------|---------------|-------------------------------------------------------------------------------------------------------------------------------------------------|
| id            |`string`      |**timeOff** 的 ID。|
| userId            |`string`      |分配给 **timeOff** 的用户的 ID。 必需项。|
| sharedTimeOff     | [timeOffItem](timeoffitem.md)  |员工和经理都可查看的 **此 timeOff** 的共享版本。 必需项。|
| draftTimeOff      | [timeOffItem](timeoffitem.md)        |经理可查看的 **此时间Off** 的草稿版本。 必需。|
| createdDateTime       |`DateTimeOffset`        |首次创建 **TimeOff** 的时间戳。 时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。 |
| lastModifiedDateTime      |`DateTimeOffset`        |上次更新 **TimeOff** 的时间戳。 时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。 |
| lastModifiedBy        | [identitySet](identityset.md)        |上次更新的标识 **Off**。 |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.timeOff",
   "baseType":"microsoft.graph.changeTrackedEntity"
}-->

```json
{
  "userId": "string (identifier)",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "lastModifiedBy": {"@odata.type":"microsoft.graph.identitySet"},
  "sharedTimeOff": {"@odata.type":"microsoft.graph.timeOffItem"},
  "draftTimeOff": {"@odata.type":"microsoft.graph.timeOffItem"}
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "timeOff resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


