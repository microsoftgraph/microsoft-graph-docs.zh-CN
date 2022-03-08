---
title: Shift 资源类型
description: 班次是计划中计划工作的一个单元。
author: aaku
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 52b170fef5a283cfaa31199d78bd943212539434
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2022
ms.locfileid: "63334441"
---
# <a name="shift-resource-type"></a>Shift 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

计划中的计划工作 [单位](schedule.md)。 

## <a name="methods"></a>Methods

| 方法       | 返回类型  |说明|
|:---------------|:--------|:----------|
|[创建班次](../api/schedule-post-shifts.md) | [shift](shift.md) | 新建 `shift`。|
|[列出班次](../api/schedule-list-shifts.md) | [shift](shift.md) 集合 | 获取此 `shifts` 计划中的 列表。|
|[获取班次](../api/shift-get.md) | [shift](shift.md) | 按 ID 获取 `shift`。|
|[替换班次](../api/shift-put.md) | [shift](shift.md) | 更换 `shift`。|
|[删除班次](../api/shift-delete.md) | 无 | `shift`从计划中删除 。|

## <a name="properties"></a>属性
|名称          |类型           |说明                                                                                                                                      |
|--------------|---------------|-------------------------------------------------------------------------------------------------------------------------------------------------|
| id            |`string`      |`shift` 的 ID。|
| userId            |`string`      |分配给 的用户 `shift`的 ID。 必需项。 |
| schedulingGroupId         |`string`      |属于的计划组的 `shift` ID。 必需项。 |
| sharedShift   |[shiftItem](shiftitem.md)  |员工和经理 `shift` 都可查看的共享版本。 必需项。 |
| draftShift        |[shiftItem](shiftitem.md)        |经理可查看 `shift` 的此草稿版本。 必需。 |
| createdDateTime       |`DateTimeOffset`        |首次创建此时间戳 `shift` 的时间戳。 时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。 |
| lastModifiedDateTime      |`DateTimeOffset`        |上次更新时间戳 `shift` 。 时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。 |
| lastModifiedBy        | [identitySet](identityset.md)        |上次更新 `shift` 的标识。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.shift"
}-->

```json
{
  "id": "SHFT_577b75d2-a927-48c0-a5d1-dc984894e7b8",
  "createdDateTime": "2019-03-14T04:32:51.451Z",
  "lastModifiedDateTime": "2019-03-14T05:32:51.451Z",
  "userId": "c5d0c76b-80c4-481c-be50-923cd8d680a1",
  "schedulingGroupId": "TAG_228940ed-ff84-4e25-b129-1b395cf78be0",
  "lastModifiedBy": {"@odata.type":"microsoft.graph.identitySet"},
  "sharedShift": {"@odata.type":"microsoft.graph.shiftItem"},
  "draftShift": {"@odata.type":"microsoft.graph.shiftItem"}
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "shift resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


