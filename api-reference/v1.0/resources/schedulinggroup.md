---
title: schedulingGroup 资源类型
description: 计划中成员的逻辑分组（通常按角色）。
author: akumar39
ms.localizationpriority: high
ms.prod: microsoft-teams
doc_type: resourcePageType_
ms.openlocfilehash: 998bd2ed3cf05db84dd17c4ef6c166474721105d
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59035960"
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
| displayName   | `string`      | **schedulingGroup** 的显示名称。必需。 |
| isActive          |`bool`      | 指示在新建实体或更新现有实体时是否可以使用 `schedulingGroup`。必需。 |
| userIds       | `collection(string)`    |  属于 **schedulingGroup** 成员的用户 ID 的列表。必需。 |
| createdDateTime       |`DateTimeOffset`        |首次创建此 **schedulingGroup** 的时间戳。时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 类似于如下形式：`2014-01-01T00:00:00Z` |
| lastModifiedDateTime      |`DateTimeOffset`        |首次更新此 **schedulingGroup** 的时间戳。时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 类似于如下形式：`2014-01-01T00:00:00Z` |
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

