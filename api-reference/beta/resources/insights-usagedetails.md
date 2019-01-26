---
title: usageDetails 资源类型
description: 包含使用项目的属性的复杂类型。 上次访问该资源的信息 （查看） 和修改用户 （编辑）。
author: simonhult
localization_priority: Normal
ms.prod: insights
ms.openlocfilehash: 04e064d5ebf8599466218722d89f46ececc5e58c
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/26/2019
ms.locfileid: "29577485"
---
# <a name="usagedetails-resource-type"></a>usageDetails 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

包含[用于](insights-used.md)项目的属性的复杂类型。 上次访问该资源的信息 （查看） 和修改用户 （编辑）。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.usageDetails"
}-->
```json
{
  "lastAccessedDateTime": "DateTimeOffset",
  "lastModifiedDateTime": "DateTimeOffset"
}
```

## <a name="properties"></a>属性

| 属性              | 类型          | 说明  |
| -------------         |---------------| -------------|
| lastAccessedDateTime                  | DateTimeOffset        | 日期和时间用户上次访问资源。 时间戳表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。 例如，2014 年 1 月 1 日午夜 UTC 如下所示：`2014-01-01T00:00:00Z`。 只读。                      |
| lastModifiedDateTime              | DateTimeOffset        | 日期和时间用户上次修改资源。 时间戳表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。 例如，2014 年 1 月 1 日午夜 UTC 如下所示：`2014-01-01T00:00:00Z`。 只读。       |
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/insights-usagedetails.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
