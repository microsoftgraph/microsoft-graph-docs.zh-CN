---
title: 趋势资源类型
description: 连接用户与用户趋势文档（与用户相关）文档的丰富关系。 OneDrive 文件和 SharePoint 团队网站上存储的文件可能是用户趋势文件。
author: simonhult
ms.localizationpriority: medium
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: 5cf846ca79088e250b4e37fa97495896fd88fe44
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59109134"
---
# <a name="trending-resource-type"></a>趋势资源类型

命名空间：microsoft.graph

连接用户与用户趋势文档（与用户相关）文档的丰富关系。 OneDrive 文件和 SharePoint 团队网站上存储的文件可能是用户趋势文件。

## <a name="methods"></a>方法

| 方法       | 返回类型  |说明|
|:---------------|:--------|:----------|
|[列出趋势](../api/insights-list-trending.md) |[trending](insights-trending.md) 集合| 获取趋势文件的列表。|

## <a name="properties"></a>属性

| 属性      | 类型                              | 说明  |
| ------------- |---------------                    | -------------|
| id                    | String                    | 关系的唯一标识符。 只读。        |
| weight                | 双精度                    | 指示文档当前趋势的值。 数字越大，文档当前围绕用户的趋势就 (越相关) 。 返回的文档按此值排序。  |
| resourceVisualization | [resourceVisualization](insights-resourcevisualization.md)    | 可用于在体验中可视化文档的属性。 |
| resourceReference     | [resourceReference](insights-resourcereference.md)        | 引用趋势文档的属性，如文档的 URL 和类型。 |
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

