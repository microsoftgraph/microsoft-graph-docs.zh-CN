---
title: timeOff 资源类型
description: 计划中的非工作单位。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: c15d65c6d0a5a9749654698a51996cb21c254a9d
ms.sourcegitcommit: f58ff560fa02ac95e296375c143b0922fb6a425c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/19/2019
ms.locfileid: "30676987"
---
# <a name="timeoff-resource-type"></a>timeOff 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

计划中的非工作单位。

## <a name="methods"></a>方法

| 方法       | 返回类型  |说明|
|:---------------|:--------|:----------|
|[创建 timeOff](../api/schedule-post-timesoff.md) | [timeOff](timeOff.md) | 创建一个新的 `timeOff` 对象。|
|[列出 timeOffs](../api/schedule-list-timesoff.md) | [timeOff](timeOff.md)集合 | 获取此计划中`timeOff`的对象列表。|
|[获取 timeOff](../api/timeoff-get.md) | [timeOff](timeOff.md) | `timeOff`按 ID 获取。|
|[替换 timeOff](../api/timeoff-put.md) | [timeOff](timeOff.md) | 替换`timeOff`。|
|[删除 timeOff](../api/timeoff-delete.md) | None | `timeOff`从计划中删除。|

## <a name="properties"></a>属性
|名称          |类型           |说明                                                                                                                                      |
|--------------|---------------|-------------------------------------------------------------------------------------------------------------------------------------------------|
| id            |`string`      |的 ID `timeOff`。|
| userId            |`string`      |分配给的`timeOff`用户的 ID。 必需。|
| sharedTimeOff     |[timeOffItem](timeoffitem.md)  |员工和经理可查看`timeOff`的共享版本。 必需。|
| draftTimeOff      |[timeOffItem](timeoffitem.md)        |经理可查看的草稿`timeOff`版本。 必需。|
| createdDateTime       |`DateTimeOffset`        |首次创建时的时间`timeOff`戳。 时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时间。 例如, 2014 年1月1日午夜 UTC 将如下所示: "2014-01-01T00:00: 00Z"。 |
| lastModifiedDateTime      |`DateTimeOffset`        |上次更新此`timeOff`时间戳的时间戳。 时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时间。 例如, 2014 年1月1日午夜 UTC 将如下所示: "2014-01-01T00:00: 00Z"。 |
| lastModifiedBy        |`microsoft.graph.identitySet`        |最后更新此`timeOff`的标识。 |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.timeOff"
}-->

```json
{
  "userId": "c5d0c76b-80c4-481c-be50-923cd8d680a1",
  "createdDateTime": "2019-03-14T05:35:57.755Z",
  "lastModifiedDateTime": "2019-03-14T05:36:08.381Z",
  "lastModifiedBy": {
    "application": null,
    "device": null,
    "conversation": null,
    "user": {
      "id": "366c0b19-49b1-41b5-a03f-9f3887bd0ed8",
      "displayName": "John Doe"
    }
  },
  "sharedTimeOff": {
    "timeOffReasonId": "TOR_891045ca-b5d2-406b-aa06-a3c8921245d7",
    "startDateTime": "2019-03-11T07:00:00Z",
    "endDateTime": "2019-03-12T07:00:00Z",
    "theme": "white"
  },
  "draftTimeOff": {
    "timeOffReasonId": "TOR_891045ca-b5d2-406b-aa06-a3c8921245d7",
    "startDateTime": "2019-03-11T07:00:00Z",
    "endDateTime": "2019-03-12T07:00:00Z",
    "theme": "pink"
  }
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
  "suppressions": [
    "Error: /api-reference/beta/resources/timeoff.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
