---
title: usedInsight 资源类型
description: 表示特定用户使用的文档的洞察力。 该见解将返回用户查看或修改的最相关的文档。
author: simonhult
localization_priority: Normal
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: aa5d5adc9b7716f26c1b05edb00122da57d625ab
ms.sourcegitcommit: a21fa7fad3a75f94e924b36d6ab94a3699983bdf
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/14/2020
ms.locfileid: "44227015"
---
# <a name="usedinsight-resource-type"></a>usedInsight 资源类型

命名空间：microsoft.graph

表示特定用户使用的文档的洞察力。 该见解将返回用户查看或修改的最相关的文档。 其中包括以下文档：

- OneDrive for Business
- SharePoint

## <a name="methods"></a>方法

| 方法       | 返回类型  |说明|
|:---------------|:--------|:----------|
|[使用的列表](../api/insights-list-used.md) |[usedInsight](insights-used.md) 集合| 获取已用文件的列表。|

## <a name="properties"></a>属性

| 属性              | 类型                      | 说明  |
| -------------         |---------------            | -------------|
| id                    | String                    | 关系的唯一标识符。 只读。        |
| lastUsed              | [usageDetails](insights-usagedetails.md)              | 有关用户上次查看或修改项目的时间的信息。 只读。      |
| resourceVisualization | [resourceVisualization](insights-resourcevisualization.md)                | 可用于在体验中可视化文档的属性。 只读      |
| resourceReference     | [resourceReference](insights-resourcereference.md)                      | 所用文档的引用属性，例如文档的 url 和类型。 只读     |

## <a name="relationships"></a>关系

| 属性      | 类型          | 说明  |
| ------------- |---------------| -------------|
| 资源      | [实体](entity.md)集合    | 用于导航到所使用的项目。 对于文件附件，类型为*fileAttachment*。 对于链接的附件，类型为*driveItem*。 |

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "keyProperty":"id",
  "optionalProperties": [
    "resource"
  ],
  "@odata.type": "microsoft.graph.usedInsight"
}-->

```json
{
  "id": "string",
  "lastUsed": "usageDetails",
  "resourceVisualization": { "@odata.type": "microsoft.graph.resourceVisualization" },
  "resourceReference": { "@odata.type": "microsoft.graph.resourceReference" }
}
```
