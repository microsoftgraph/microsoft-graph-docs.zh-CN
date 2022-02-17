---
title: searchRequest 资源类型
description: 要发送到查询终结点的搜索请求。 它包含响应中预期的实体类型、基础源、分页参数、字段请求和实际搜索查询。
ms.localizationpriority: medium
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: d7801fc7ba8d1bcdfcb9fa6da5508fb5d973d3d9
ms.sourcegitcommit: b19b19bf192688f4c513492e8391e4d8dc104633
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/17/2022
ms.locfileid: "62878860"
---
# <a name="searchrequest-resource-type"></a>searchRequest 资源类型

命名空间：microsoft.graph

JSON blob 中格式化的搜索请求。 

JSON blob 包含响应中预期的资源类型、基础源、分页参数、排序选项、请求的聚合和字段以及实际搜索查询。 请参阅 [各种](#see-also) 资源上的搜索请求示例。

> [!NOTE]
> 请注意搜索 [实体](search-api-overview.md#known-limitations) 类型的特定组合以及排序或聚合搜索结果的已知限制。


## <a name="properties"></a>属性

| 属性     | 类型        | 说明| 
|:-------------|:------------|:------------|
|aggregationFilters|String 集合|包含一个或多个筛选器，用于获取聚合的搜索结果并按字段的特定值进行筛选。 可选。<br>基于之前按同一字段聚合的搜索生成此筛选器。 从之前搜索的响应中，确定将结果筛选为字段的特定值的 [searchBucket](searchBucket.md) ，在其 **aggregationFilterToken** 属性中使用该字符串，并生成格式为 **"{field}：\\"{aggregationFilterToken}\\"** 的聚合筛选器字符串。 <br>如果需要为同一字段提供多个值，请使用 **其 aggregationFilterToken** 属性中的字符串，并生成格式为" **{field}：或 (\\"{aggregationFilterToken1}\\"，\\"{aggregationFilterToken2}\\") "** 的聚合筛选器字符串。 <br>例如，按文件类型搜索和聚合驱动器项在响应中返回文件类型的 **searchBucket**`docx`。 可以在后续搜索查询中方便地使用此 **searchBucket** `docx` 返回的 **aggregationFilterToken**，筛选器向下筛选文件类型的驱动器项。 [示例 1](/graph/search-concept-aggregation#example-1-request-aggregations-by-string-fields) [和示例 2](/graph/search-concept-aggregation#example-2-apply-an-aggregation-filter-based-on-a-previous-request) 显示实际请求和响应。|
|聚合|[aggregationOption](aggregationOption.md) 集合|指定聚合 (也称为) 搜索结果一起返回的精简条件。 可选。|
|contentSources|String 集合|包含要定向的连接。|
|enableTopResults|Boolean|这将触发邮件的混合排序：前 3 个邮件最相关。 此属性仅适用于 entityType=`message`。 可选。|
|entityTypes|entityType 集合| 响应中预期的一种或多种资源类型。 可取值为：`list`、`site`、`listItem`、`message`、`event`、`drive`、`driveItem`、`externalItem`。 有关 [同一](search-api-overview.md#known-limitations) 搜索请求中支持的两个或多个实体类型的组合，请参阅已知限制。 必需项。|
|fields|String 集合 |包含为 **entityTypes** 中指定的每个资源对象返回的字段，允许自定义默认情况下返回的字段;否则，包括其他字段（如 SharePoint 和 OneDrive 中的自定义托管属性）或 microsoft Graph 连接器引入的内容中的 **externalItem** 中的自定义字段。 **fields** 属性可以使用 [应用于属性的](/microsoftsearch/configure-connector#step-6-assign-property-labels)语义标签。 例如，如果属性被标记为 title，可以使用以下语法检索它： `label_title`。 可选。|
|起始数量|Int32|指定搜索结果的偏移量。 偏移量 0 返回第一个结果。 可选。|
|查询|[searchQuery](searchquery.md)|包含查询词。 必需项。|
|queryAlterationOptions|[searchAlterationOptions](searchalterationoptions.md)|JSON blob 中格式化的查询更改选项，其中包含与拼写更正相关的两个可选标志。 可选。 |
|resultTemplateOptions|[resultTemplateOption](resulttemplateoption.md) 集合|提供用于呈现来自连接器的搜索结果的搜索结果模板选项。|
|大小|Int32|要检索的页面的大小。 可选。|
|sortProperties|[sortProperty](sortProperty.md) 集合|包含排序的字段集合和用于对结果进行排序的方向。 集合中最多只能有 5 个排序属性。 可选。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

```json
{
  "aggregationFilters": ["String"],
  "aggregations": {"@odata.type": "microsoft.graph.aggregationOption"},
  "enableTopResults": "Boolean",
  "entityTypes": ["String"],
  "contentSources": ["String"],
  "fields": ["String"],
  "from": "Int32",
  "query": {"@odata.type": "microsoft.graph.searchQuery"},
  "queryAlterationOptions": {"@odata.type": "microsoft.graph.searchAlterationOptions"},
  "resultTemplateOptions": [{"@odata.type": "microsoft.graph.resultTemplateOption"}],
  "size": "Int32"
}
```

## <a name="see-also"></a>另请参阅
- 搜索 [邮件](/graph/search-concept-messages)
- 搜索 [日历事件](/graph/search-concept-events)
- 搜索网站SharePoint和OneDrive ([、列表和网站) ](/graph/search-concept-files)
- [对](/graph/search-concept-sort) 搜索结果进行排序
- 使用 [聚合](/graph/search-concept-aggregations) 优化搜索结果
- 使用 [显示布局](/graph/search-concept-display-layout.md)
- 在 [搜索结果中启用](/graph/search-concept-speller) 拼写更正


<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "searchRequest resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


