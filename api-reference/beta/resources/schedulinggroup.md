---
title: schedulingGroup 资源类型
description: 计划中成员的逻辑分组（通常按角色）。
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
ms.openlocfilehash: 644a9492e47979241ccab3f0e69eb90407eb2647
ms.sourcegitcommit: 081cacecb4960aabc9e1011d12f06fe9ecf7d188
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/16/2019
ms.locfileid: "30657866"
---
# <a name="schedulinggroup-resource-type"></a>schedulingGroup 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[计划](schedule.md)中成员的逻辑分组（通常按角色）。 

## <a name="methods"></a>方法

| 方法       | 返回类型  |说明|
|:---------------|:--------|:----------|
|[创建 schedulingGroup](../api/schedule-post-schedulinggroups.md) | [schedulingGroup](schedulinggroup.md) | 新建 `schedulingGroup`。|
|[列出 schedulingGroups](../api/schedule-list-schedulinggroups.md) | [schedulingGroup](schedulinggroup.md) 集合 | 获取计划中 `schedulingGroups` 的列表。|
|[获取 schedulingGroup](../api/schedulinggroup-get.md) | [schedulingGroup](schedulinggroup.md) | 按 ID 获取 `schedulingGroup`。|
|[更换 schedulingGroup](../api/schedulinggroup-put.md) | [schedulingGroup](schedulinggroup.md) | 更换 `schedulingGroup`。|
|[删除 schedulingGroup](../api/schedulinggroup-delete.md) | 无 | 将 `schedulingGroup` 标记为非活动状态。|

## <a name="properties"></a>属性
|名称          |类型           |说明                                                                                 |
|--------------|---------------|--------------------------------------------------------------------------------------------|
| id            | `string`      |`schedulingGroup` 的 ID。|
| displayName   | `string`      | `schedulingGroup` 的显示名称。 必需。 |
| isActive          |`bool`      | 指示在新建实体或更新现有实体时是否可以使用 `schedulingGroup`。 必需。 |
| userIds       | `collection(string)`    |  `schedulingGroup` 成员的用户 ID 列表。 必需。 |
| createdDateTime       |`DateTimeOffset`        |首次创建 `schedulingGroup` 的时间戳。 时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时间。 例如，2014 年 1 月 1 日午夜 (UTC) 如下所示：“2014-01-01T00:00:00Z”。 |
| lastModifiedDateTime      |`DateTimeOffset`        |上次更新 `schedulingGroup` 的时间戳。 时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时间。 例如，2014 年 1 月 1 日午夜 (UTC) 如下所示：“2014-01-01T00:00:00Z”。 |
| lastModifiedBy        |`microsoft.graph.identitySet`        |上次更新 `schedulingGroup` 的标识。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.schedulingGroup"
}-->

```json
{
  "id": "TAG_f914d037-00a3-4ba4-b712-ef178cbea263",
  "createdDateTime": "2019-03-12T22:10:38.242Z",
  "lastModifiedDateTime": "2019-03-12T22:10:38.242Z",
  "displayName": "Cashiers",
  "isActive": true,
  "userIds": [
    "c5d0c76b-80c4-481c-be50-923cd8d680a1",
    "2a4296b3-a28a-44ba-bc66-0274b9b95851"
  ],
  "lastModifiedBy": {
    "application": null,
    "device": null,
    "conversation": null,
    "user": {
      "id": "366c0b19-49b1-41b5-a03f-9f3887bd0ed8",
      "displayName": "John Doe"
    }
  }
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
  "suppressions": [
    "Error: /api-reference/beta/resources/schedulinggroup.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
