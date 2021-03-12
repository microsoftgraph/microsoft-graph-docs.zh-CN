---
title: schedulingGroup 资源类型
description: 计划中成员的逻辑分组（通常按角色）。
author: akumar39
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: resourcePageType_
ms.openlocfilehash: 018359ab0dd6702a2fda40bf5f0b29c639211f4a
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/11/2021
ms.locfileid: "50719302"
---
# <a name="schedulinggroup-resource-type"></a>schedulingGroup 资源类型

命名空间：microsoft.graph

[计划](schedule.md)中成员的逻辑分组（通常按角色）。 

## <a name="methods"></a>方法

| 方法       | 返回类型  |Description|
|:---------------|:--------|:----------|
|[List](../api/schedule-list-schedulinggroups.md) | [schedulingGroup](schedulinggroup.md) 集合 | 获取计划中的 **schedulingGroups** 列表。|
|[Create](../api/schedule-post-schedulinggroups.md) | [schedulingGroup](schedulinggroup.md) | 新建 **schedulingGroup**。|
|[Get](../api/schedulinggroup-get.md) | [schedulingGroup](schedulinggroup.md) | 按 ID 获取 **schedulingGroup**。|
|[删除](../api/schedulinggroup-delete.md) | 无 | 将 **schedulingGroup** 标记为非活动。|
|[Replace](../api/schedulinggroup-put.md) | [schedulingGroup](schedulinggroup.md) | 替换 **schedulingGroup**。|

## <a name="properties"></a>属性
|名称          |类型           |说明                                                                                 |
|--------------|---------------|--------------------------------------------------------------------------------------------|
| id            | `string`      |**schedulingGroup** 的 ID。|
| displayName   | `string`      | **schedulingGroup** 的显示名称。 必填。 |
| isActive          |`bool`      | 指示在新建实体或更新现有实体时是否可以使用 `schedulingGroup`。 必需。 |
| userIds       | `collection(string)`    |  属于 **schedulingGroup** 成员的用户 ID 的列表。 必填。 |
| createdDateTime       |`DateTimeOffset`        |此 **schedulingGroup** 的首次创建时间戳。 时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。 |
| lastModifiedDateTime      |`DateTimeOffset`        |此 **schedulingGroup** 的最后更新时间戳。 时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。 |
| lastModifiedBy        | [identitySet](identityset.md) |最后更新此 **schedulingGroup** 的标识。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.schedulingGroup",
  "baseType": "microsoft.graph.changeTrackedEntity"
}-->

```json
{
  "id": "string (identifier)",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "displayName": "String",
  "isActive": true,
  "userIds": ["String (identifier)"],
  "lastModifiedBy":{"@odata.type":"microsoft.graph.identitySet"}
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "schedulingGroup resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->

