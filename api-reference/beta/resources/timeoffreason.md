---
title: timeOffReason 资源类型
description: 在计划中花费时间的有效原因。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 72597fa1678110a40b9dd1a0ea6e6235625144ab
ms.sourcegitcommit: 081cacecb4960aabc9e1011d12f06fe9ecf7d188
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/16/2019
ms.locfileid: "30657530"
---
# <a name="timeoffreason-resource-type"></a>timeOffReason 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[计划](schedule.md)中[timeOff](timeoff.md)实例的有效原因。

## <a name="methods"></a>方法

| 方法       | 返回类型  |说明|
|:---------------|:--------|:----------|
|[创建 timeOffReason](../api/schedule-post-timeoffreasons.md) | [timeOffReason](timeoffreason.md) | 创建新`timeOffReason`的。|
|[列出 timeOffReason](../api/schedule-list-timeoffreasons.md) | [timeOffReason](timeoffreason.md)集合 | 获取日程安排中`timeOffReasons`的列表。|
|[获取 timeOffReason](../api/timeoffreason-get.md) | [timeOffReason](timeoffreason.md) | `timeOffReason`按 ID 获取。|
|[替换 timeOffReason](../api/timeoffreason-put.md) | [timeOffReason](timeoffreason.md) | 替换`timeOffReason`。|
|[删除 timeOffReason](../api/timeoffreason-delete.md) | 无 | 标记`timeOffReason`为非活动。|

## <a name="properties"></a>属性
|名称          |类型           |说明                                                                                 |
|--------------|---------------|--------------------------------------------------------------------------------------------|
| id            |`string`      |的 ID `timeOffReason`。|
| displayName               | `string`                  | 的名称`timeOffReason`。 必需。 |
| iconType | `enum`   | 支持的图标类型: 无;car式运行planefirstAid;dr。notWorking;构造juryDuty;投放cup of电话气候防护piggyBank;监控桩trafficCone;针sunny。 必需。 |
| isActive          |`bool`      | 指示在创建`timeOffReason`新实体或更新现有实体时是否可以使用此文件。 必需。 |
| createdDateTime       |`DateTimeOffset`        |首次在其上创建`timeOffReason`此项的时间戳。 时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时间。 例如, 2014 年1月1日午夜 UTC 将如下所示: "2014-01-01T00:00: 00Z"。 |
| lastModifiedDateTime      |`DateTimeOffset`         |对其最后更新的`timeOffReason`时间戳。 时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时间。 例如, 2014 年1月1日午夜 UTC 将如下所示: "2014-01-01T00:00: 00Z"。 |
| lastModifiedBy        |`microsoft.graph.identitySet`        |最后更新此`timeOffReason`的标识。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.timeOffReason"
}-->

```json
{
  "id": "TOR_891045ca-b5d2-406b-aa06-a3c8921245d7",
  "createdDateTime": "2019-03-12T22:10:38.242Z",
  "lastModifiedDateTime": "2019-03-12T22:10:38.242Z",
  "displayName": "Vacation",
  "iconType": "plane",
  "isActive": true,
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
  "description": "timeOffReason resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/timeoffreason.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
