---
title: Shift 资源类型
description: 表示计划中的计划工作单位。
author: akumar39
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: abec7f019750dbfe30335e1c8d6df3ecbb95c2d8e99a2c3720381307560ef22a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54169282"
---
# <a name="shift-resource-type"></a>Shift 资源类型

命名空间：microsoft.graph

表示计划中的计划工作 [单位](schedule.md)。 

## <a name="methods"></a>方法

| 方法       | 返回类型  |说明|
|:---------------|:--------|:----------|
|[列出班次](../api/schedule-list-shifts.md) | [shift](shift.md) 集合 | 获取此 **计划** 中的班次列表。|
|[创建班次](../api/schedule-post-shifts.md) | [shift](shift.md) | 创建新的 **班次。**|
|[获取班次](../api/shift-get.md) | [shift](shift.md) | 按 **ID 获取** 班次。|
|[替换班次](../api/shift-put.md) | [shift](shift.md) | 替换 **班次**。|
|[删除班次](../api/shift-delete.md) | 无 | 从 **计划中删除** 班次。|

## <a name="properties"></a>属性
|名称          |类型           |说明                                                                                                                                      |
|--------------|---------------|-------------------------------------------------------------------------------------------------------------------------------------------------|
| id            |`string`      |班次的 **ID。**|
| userId            |`string`      |分配给班次 的用户的 **ID。** 必填。 |
| schedulingGroupId         |`string`      |班次属于的计划 **组的** ID。 必填。 |
| sharedShift   |[shiftItem](shiftitem.md)  |员工 **和经理都** 可查看此班次的共享版本。 必填。 |
| draftShift        |[shiftItem](shiftitem.md)        |经理 **可查看的此** 班次的草稿版本。 必填。 |
| createdDateTime       |`DateTimeOffset`        |首次创建此 **班次的时间戳** 。 时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。 |
| lastModifiedDateTime      |`DateTimeOffset`        |上次更新此 **班次的时间戳** 。 时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。 |
| lastModifiedBy        | [identitySet](identityset.md)        |上次更新此班次的 **标识**。|

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

