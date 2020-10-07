---
title: searchRequest 资源类型
description: 要发送到查询终结点的搜索请求。 它包含响应中的预期实体类型、基础源、分页参数、字段请求和实际搜索查询。
localization_priority: Normal
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 04bdca98f4676454a72e503e8bfe747bbda306cc
ms.sourcegitcommit: c20276369a8834a259f24038e7ee5c33de02660b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/07/2020
ms.locfileid: "48372691"
---
# <a name="searchrequest-resource-type"></a>searchRequest 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [search-api-deprecation](../../includes/search-api-deprecation.md)]

JSON blob 中格式化的搜索请求。 

JSON blob 包含响应中预期的资源类型、基础源、分页参数、排序选项、请求的聚合和字段以及实际搜索查询。 请参阅各种资源上的搜索请求的 [示例](#see-also) 。

> [!NOTE]
> 了解有关搜索实体类型的特定组合以及对搜索结果进行排序或聚合的 [已知限制](search-api-overview.md#known-limitations) 。


## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|:------------|
|聚合|[aggregationOption](aggregationOption.md) 集合|指定 (也称为精简条件) 与搜索结果一起返回的聚合。 可选。|
|aggregationFilters|字符串集合|包含一个或多个筛选器，以获取聚合并筛选为字段的特定值的搜索结果。 可选。<br>基于按相同字段聚合的先前搜索生成此筛选器。 从以前的搜索的响应中，确定将结果筛选为字段的特定值的 [searchBucket](searchBucket.md) ，使用其 **aggregationFilterToken** 属性中的字符串，并以 **"{field}： \\ {aggregationFilterToken} \\ "** 格式生成聚合筛选器字符串。 <br>例如，按文件类型搜索和聚合 drive 项目为响应中**searchBucket**的文件类型返回 searchBucket `docx` 。 您可以在随后的搜索查询中方便地使用为此**searchBucket**返回的**aggregationFilterToken** ，并筛选出与驱动文件类型的项目相匹配的项目 `docx` 。 [示例 1](/graph/search-concept-aggregation#example-1-request-aggregations-by-string-fields) 和 [示例 2](/graph/search-concept-aggregation#example-2-apply-an-aggregation-filter-based-on-a-previous-request) 显示实际的请求和响应。|
|contentSources|字符串集合|包含要设定的连接。 <br>遵循以下格式： `/external/connections/connectionid` 其中 `connectionid` 是连接器管理中定义的 ConnectionId。 <br> 注意：仅当 entityType = 时，contentSource 才适用 `externalItem` 。 可选。|
|enableTopResults|布尔值|这将触发邮件的混合排序：前3个邮件最相关。 此属性仅适用于 entityType = `message` 。 可选。|
|entityTypes|entityType 集合| 响应中预期的一种或多种类型的资源。 可取值为：`list`、`site`、`listItem`、`message`、`event`、`drive`、`driveItem`、`externalItem`。 请参阅相同搜索请求中支持的两个或更多实体类型的组合的 [已知限制](search-api-overview.md#known-limitations) 。 必需。|
|fields|字符串集合 |包含要为 **entityTypes**中指定的每个资源对象返回的字段，允许自定义默认情况下返回的字段（包括其他字段，如来自 SharePoint 和 OneDrive 的自定义托管属性）或 **externalItem** 中从内容引入 x 连接器的自定义字段。 可选。|
|起始数量|Int32|指定搜索结果的偏移量。 偏移量0返回的第一个结果。 可选。|
|查询|[searchQuery](searchquery.md)|包含查询词。 必需。|
|大小|Int32|要检索的页面的大小。 可选。|
|sortProperties|[sortProperty](sortProperty.md) 集合|包含用于对结果进行排序的字段和方向的已排序集合。 集合中最多可以有5个排序属性。 可选。|
|stored_fields (已弃用) |字符串集合 |现在，此属性将替换为 **fields** 属性。 |


## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.searchRequest",
  "baseType": null
}-->

```json
{
  "entityTypes": ["String"],
  "contentSources": ["String"],
  "query": {"@odata.type": "microsoft.graph.searchQuery"},
  "from": 1024,
  "size": 1024,
  "fields": ["String"],
  "sortProperties": [{"@odata.type": "microsoft.graph.sortProperty"}],
  "aggregations": [{"@odata.type": "microsoft.graph.aggregationOption"}],
  "aggregationFilters": ["String"],
  "enableTopResults": true  
}
```

## <a name="see-also"></a>另请参阅
- 搜索 [邮件消息](/graph/search-concept-messages)
- 搜索 [日历事件](/graph/search-concept-events)
- 在 SharePoint 和 OneDrive 中搜索内容 ([文件、列表和网站](/graph/search-concept-files)) 
- 搜索 [自定义类型 (Graph 连接器) ](/graph/search-concept-custom-types) 数据
- [对搜索结果进行排序](/graph/search-concept-sort)
- 使用 [聚合](/graph/search-concept-aggregations) 优化搜索结果


<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "searchRequest resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


