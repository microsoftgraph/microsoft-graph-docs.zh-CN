---
title: 趋势资源类型
description: 将用户连接到的文档的用户 （与用户相关) 周围趋势丰富的关系。 OneDrive 文件和文件存储在 SharePoint 工作组网站可以趋势周围用户。
author: simonhult
localization_priority: Normal
ms.prod: insights
ms.openlocfilehash: 587b52107f3a7f9892603afb8273ce55b6faa549
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/26/2019
ms.locfileid: "29577408"
---
# <a name="trending-resource-type"></a>趋势资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

将用户连接到的文档的用户 （与用户相关) 周围趋势丰富的关系。 OneDrive 文件和文件存储在 SharePoint 工作组网站可以趋势周围用户。

## <a name="methods"></a>方法

| 方法       | 返回类型  |说明|
|:---------------|:--------|:----------|
|[列表趋势分析](../api/insights-list-trending.md) |[insights_trending](insights-trending.md)集合| 获取趋势文件的列表。|

## <a name="properties"></a>属性

| 属性      | 类型                              | 说明  |
| ------------- |---------------                    | -------------|
| id                    | String                    | 关系的唯一标识符。 只读。        |
| weight                | 双精度                    | 值，该值指示当前趋势多少文档。 较大的号码，更多文档当前趋势周围用户 （更多相关)。 按此值，返回的文档进行排序。  |
| resourceVisualization | [resourceVisualization](insights-resourcevisualization.md)集合 | 您可以使用可视化中您的体验的文档的属性。 |
| resourceReference     | [resourceReference](insights-resourcereference.md)集合 | 趋势文档，如 url 和的文档类型的引用属性。 |

## <a name="relationships"></a>关系

| 属性      | 类型          | 说明  |
| ------------- |---------------| -------------|
| 资源      | 实体集合 | 用于导航到趋势文档。 |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.trending"
}-->
```json
{
  "id": "string",
  "weight": "double",
  "resourceVisualization": [{"@odata.type": "microsoft.graph.resourceVisualization"}],
  "resourceReference": [{"@odata.type": "microsoft.graph.resourceReference"}],
  
  "resource": [ { "@odata.type": "microsoft.graph.entity" } ]
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/insights-trending.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
