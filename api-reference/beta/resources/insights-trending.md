---
title: 趋势资源类型
description: 将用户连接到的文档的用户 （与用户相关) 周围趋势丰富的关系。 OneDrive 文件和文件存储在 SharePoint 工作组网站可以趋势周围用户。
author: simonhult
ms.openlocfilehash: ae3c3a876dba6c22a629cce5db8e5b4baa5fb5bf
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27347997"
---
# <a name="trending-resource-type"></a>趋势资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

将用户连接到的文档的用户 （与用户相关) 周围趋势丰富的关系。 OneDrive 文件和文件存储在 SharePoint 工作组网站可以趋势周围用户。

## <a name="methods"></a>方法

| 方法       | 返回类型  |说明|
|:---------------|:--------|:----------|
|[列表趋势分析](../api/insights-list-trending.md) |[insights_trending](insights-trending.md)集合| 获取趋势文件的列表。|

## <a name="properties"></a>属性

| 属性      | 类型                              | 说明  |
| ------------- |---------------                    | -------------|
| id                    | 字符串                    | 关系的唯一标识符。 只读。        |
| weight                | 双精度数                    | 值，该值指示当前趋势多少文档。 较大的号码，更多文档当前趋势周围用户 （更多相关)。 按此值，返回的文档进行排序。  |
| resourceVisualization | [resourceVisualization](insights-resourcevisualization.md)    | 您可以使用可视化中您的体验的文档的属性。 |
| resourceReference     | [resourceReference](insights-resourcereference.md)        | 趋势文档，如 url 和的文档类型的引用属性。 |

## <a name="relationships"></a>Relationships

| 属性      | 类型          | 说明  |
| ------------- |---------------| -------------|
| 资源      | Entity        | 用于导航到趋势文档。 |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

```json
{
  "id": "string",
  "weight": "double",
  "resourceVisualization": [{"@odata.type": "microsoft.graph.resourceVisualization"}],
  "resourceReference": [{"@odata.type": "microsoft.graph.resourceReference"}],
  
  "resource": [ { "@odata.type": "microsoft.graph.entity" } ]
}
```