---
title: 趋势资源类型
description: 将用户连接到围绕用户 (的趋势的文档的丰富关系与用户) 相关。 OneDrive 文件和存储在 SharePoint 团队网站上的文件可围绕用户进行趋势。
author: simonhult
localization_priority: Normal
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: 7a9c9cf9323aa24bd50c1f817a1293088e1a4373
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48054768"
---
# <a name="trending-resource-type"></a>趋势资源类型

命名空间：microsoft.graph

将用户连接到围绕用户 (的趋势的文档的丰富关系与用户) 相关。 OneDrive 文件和存储在 SharePoint 团队网站上的文件可围绕用户进行趋势。

## <a name="methods"></a>方法

| 方法       | 返回类型  |说明|
|:---------------|:--------|:----------|
|[列出趋势](../api/insights-list-trending.md) |[trending](insights-trending.md) 集合| 获取趋势文件的列表。|

## <a name="properties"></a>属性

| 属性      | 类型                              | 说明  |
| ------------- |---------------                    | -------------|
| id                    | String                    | 关系的唯一标识符。 只读。        |
| weight                | 双精度                    | 值，该值指示文档当前正在进行趋势计算的程度。 数字越大，文档当前在用户周围的趋势 (越相关) 。 返回的文档按此值进行排序。  |
| resourceVisualization | [resourceVisualization](insights-resourcevisualization.md)    | 可用于在体验中可视化文档的属性。 |
| resourceReference     | [resourceReference](insights-resourcereference.md)        | 参考趋势文档的属性，例如文档的 url 和类型。 |
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

