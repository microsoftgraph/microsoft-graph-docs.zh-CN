---
title: timeOff 资源类型
description: 计划中的非工作单位。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 848365a812053b7788db37395bee8662d69cda37
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33342013"
---
# <a name="timeoff-resource-type"></a>timeOff 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

计划中的非工作单位。

## <a name="methods"></a>方法

| 方法       | 返回类型  |说明|
|:---------------|:--------|:----------|
|[创建 timeOff](../api/schedule-post-timesoff.md) | [timeOff](timeOff.md) | 创建一个新的 `timeOff` 对象。|
|[列出 timeOffs](../api/schedule-list-timesoff.md) | [timeOff](timeOff.md)集合 | 获取此计划中`timeOff`的对象列表。|
|[获取 timeOff](../api/timeoff-get.md) | [timeOff](timeOff.md) | 按 ID 获取 `timeOff`。|
|[替换 timeOff](../api/timeoff-put.md) | [timeOff](timeOff.md) | 更换 `timeOff`。|
|[删除 timeOff](../api/timeoff-delete.md) | 无 | `timeOff`从计划中删除。|

## <a name="properties"></a>属性
|名称          |类型           |说明                                                                                                                                      |
|--------------|---------------|-------------------------------------------------------------------------------------------------------------------------------------------------|
| id            |`string`      |`timeOff` 的 ID。|
| userId            |`string`      |分配给的`timeOff`用户的 ID。 必需。|
| sharedTimeOff     | [timeOffItem](timeoffitem.md)  |员工和经理可查看`timeOff`的共享版本。 必需。|
| draftTimeOff      | [timeOffItem](timeoffitem.md)        |经理可查看的草稿`timeOff`版本。 必需。|
| createdDateTime       |`DateTimeOffset`        |首次创建时的时间`timeOff`戳。 时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时间。 例如，2014 年 1 月 1 日午夜 (UTC) 如下所示：“2014-01-01T00:00:00Z”。 |
| lastModifiedDateTime      |`DateTimeOffset`        |上次更新此`timeOff`时间戳的时间戳。 时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时间。 例如，2014 年 1 月 1 日午夜 (UTC) 如下所示：“2014-01-01T00:00:00Z”。 |
| lastModifiedBy        | [identitySet](identityset.md)        |上次更新 `timeOff` 的标识。 |

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
