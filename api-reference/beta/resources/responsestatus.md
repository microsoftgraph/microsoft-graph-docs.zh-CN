---
title: responseStatus 资源类型
description: 会议请求的响应状态。
localization_priority: Normal
ms.openlocfilehash: 270c432235b929af2cb55ff63e10397fea5f92fb
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32562984"
---
# <a name="responsestatus-resource-type"></a>responseStatus 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

会议请求的响应状态。

## <a name="properties"></a>属性

| 属性 | 类型           | 说明 |
|:---------|:---------------|:------------|
| 响应 | String         | 响应类型。 可取值为：`None`、`Organizer`、`TentativelyAccepted`、`Accepted`、`Declined`、`NotResponded`。
| 时间     | DateTimeOffset | 响应返回的日期和时间。它使用 ISO 8601 格式，并始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.responseStatus"
}-->

```json
{
  "response": "String",
  "time": "String (timestamp)"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "responseStatus resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/responsestatus.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
