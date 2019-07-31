---
title: shift 资源类型
description: 班次是计划中计划工时的单位。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType_
ms.openlocfilehash: f76cd25a36ba070d9fa8281f31a1520a0d7b4435
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36008339"
---
# <a name="shift-resource-type"></a>shift 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

计划中计划工时的单位。 [](schedule.md) 

## <a name="methods"></a>方法

| 方法       | 返回类型  |说明|
|:---------------|:--------|:----------|
|[创建班次](../api/schedule-post-shifts.md) | [ctrl](shift.md) | 新建 `shift`。|
|[列出班次](../api/schedule-list-shifts.md) | [shift](shift.md)集合 | 获取此计划中`shifts`的列表。|
|[获取 shift](../api/shift-get.md) | [ctrl](shift.md) | 按 ID 获取 `shift`。|
|[替换班次](../api/shift-put.md) | [ctrl](shift.md) | 更换 `shift`。|
|[删除班次](../api/shift-delete.md) | 无 | `shift`从计划中删除。|

## <a name="properties"></a>属性
|名称          |类型           |说明                                                                                                                                      |
|--------------|---------------|-------------------------------------------------------------------------------------------------------------------------------------------------|
| id            |`string`      |`shift` 的 ID。|
| userId            |`string`      |分配给的`shift`用户的 ID。 必需。 |
| schedulingGroupId         |`string`      |属于的计划组`shift`的 ID。 必需。 |
| sharedShift   |[shiftItem](shiftitem.md)  |员工和经理可查看`shift`的共享版本。 必需。 |
| draftShift        |[shiftItem](shiftitem.md)        |经理可查看的草稿`shift`版本。 必需。 |
| createdDateTime       |`DateTimeOffset`        |首次在其上`shift`创建此项的时间戳。 时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时间。 例如，2014 年 1 月 1 日午夜 (UTC) 如下所示：“2014-01-01T00:00:00Z”。 |
| lastModifiedDateTime      |`DateTimeOffset`        |上次更新此`shift`时间的时间戳。 时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时间。 例如，2014 年 1 月 1 日午夜 (UTC) 如下所示：“2014-01-01T00:00:00Z”。 |
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
