---
title: shift 资源类型
description: 表示计划中计划工时的单位。
author: akumar39
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: e38b8a000829ead91bdee28779a0f6988dd936ef
ms.sourcegitcommit: 02c16375520853d3fa2a82ff012639550f981fc8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/07/2020
ms.locfileid: "44154302"
---
# <a name="shift-resource-type"></a>shift 资源类型

命名空间：microsoft.graph

表示计划中计划工时的[单位。](schedule.md) 

## <a name="methods"></a>方法

| 方法       | 返回类型  |说明|
|:---------------|:--------|:----------|
|[列出班次](../api/schedule-list-shifts.md) | [shift](shift.md)集合 | 获取此计划中**班次**的列表。|
|[创建班次](../api/schedule-post-shifts.md) | [ctrl](shift.md) | 创建新**班次**。|
|[获取 shift](../api/shift-get.md) | [ctrl](shift.md) | 按 ID 获取**shift** 。|
|[替换班次](../api/shift-put.md) | [ctrl](shift.md) | 替换**班次**。|
|[删除班次](../api/shift-delete.md) | None | 从计划中删除**班次轮换**。|

## <a name="properties"></a>属性
|名称          |类型           |说明                                                                                                                                      |
|--------------|---------------|-------------------------------------------------------------------------------------------------------------------------------------------------|
| id            |`string`      |**班次**的 ID。|
| userId            |`string`      |分配给**班次**的用户的 ID。 必需。 |
| schedulingGroupId         |`string`      |**班次**所属的计划组的 ID。 必需。 |
| sharedShift   |[shiftItem](shiftitem.md)  |员工和经理都可查看的此**班次**的共享版本。 必需。 |
| draftShift        |[shiftItem](shiftitem.md)        |由经理查看的此**班次**的草稿版本。 必需。 |
| createdDateTime       |`DateTimeOffset`        |此**班次**首次创建时的时间戳。 时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时间。 例如，2014 年 1 月 1 日午夜 (UTC) 如下所示：“2014-01-01T00:00:00Z”。 |
| lastModifiedDateTime      |`DateTimeOffset`        |此**班次**的上次更新时间戳。 时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时间。 例如，2014 年 1 月 1 日午夜 (UTC) 如下所示：“2014-01-01T00:00:00Z”。 |
| lastModifiedBy        | [identitySet](identityset.md)        |上次更新此**班次**的标识。|

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
