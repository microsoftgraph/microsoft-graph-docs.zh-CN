---
title: 趋势资源类型
description: 将用户连接到在用户周围进行趋势分析的文档 (与用户相关) 的丰富关系。 OneDrive 文件和存储在 SharePoint 团队网站上的文件可围绕用户进行趋势。
author: simonhult
localization_priority: Normal
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: 7963a3c518fd4fc946da4f6714a3aa52aa4b87eb
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36006218"
---
# <a name="trending-resource-type"></a>趋势资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

将用户连接到在用户周围进行趋势分析的文档 (与用户相关) 的丰富关系。 OneDrive 文件和存储在 SharePoint 团队网站上的文件可围绕用户进行趋势。

## <a name="methods"></a>方法

| 方法       | 返回类型  |说明|
|:---------------|:--------|:----------|
|[列出趋势](../api/insights-list-trending.md) |[insights_trending](insights-trending.md)集合| 获取趋势文件的列表。|

## <a name="properties"></a>属性

| 属性      | 类型                              | 说明  |
| ------------- |---------------                    | -------------|
| id                    | String                    | 关系的唯一标识符。 只读。        |
| weight                | 双精度                    | 值, 该值指示文档当前正在进行趋势计算的程度。 数字越大, 文档当前在用户周围的趋势分析越多 (相关性越好)。 返回的文档按此值进行排序。  |
| resourceVisualization | [resourceVisualization](insights-resourcevisualization.md)    | 可用于在体验中可视化文档的属性。 |
| resourceReference     | [resourceReference](insights-resourcereference.md)        | 参考趋势文档的属性, 例如文档的 url 和类型。 |
| lastModifiedDateTime  | DateTimeOffset            | |
## <a name="relationships"></a>关系

| 属性      | 类型          | 说明  |
| ------------- |---------------| -------------|
| 资源      | 属性        | 用于导航到趋势文档。 |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "keyProperty":"id",
  "optionalProperties": [
    "resource"
  ],
  "@odata.type": "microsoft.graph.trending"
}-->

```json
{
  "id": "string",
  "weight": "double",
  "resourceVisualization": {"@odata.type": "microsoft.graph.resourceVisualization"},
  "resourceReference": {"@odata.type": "microsoft.graph.resourceReference"},
  "lastModifiedDateTime": "String (timestamp)"
}
```
