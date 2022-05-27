---
title: searchRequest 资源类型
description: 要发送到查询终结点的搜索请求。 它包含响应中预期的实体类型、基础源、分页参数、字段请求和实际搜索查询。
ms.localizationpriority: medium
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 0f981aedcea282e2956859412d4d9c7ad8730323
ms.sourcegitcommit: 54ba08a80db85b9e84813387e8c4416eca44fa8e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/26/2022
ms.locfileid: "65694403"
---
# <a name="searchrequest-resource-type"></a>searchRequest 资源类型

命名空间：microsoft.graph

JSON Blob 中格式化的搜索请求。 

JSON blob 包含响应中预期的资源类型、基础源、分页参数、排序选项、请求的聚合和字段以及实际搜索查询。 请参阅各种资源上的搜索请求 [示例](#see-also) 。

> [!NOTE]
> 请注意搜索实体类型的特定组合以及对搜索结果进行排序或聚合的 [已知限制](search-api-overview.md#known-limitations) 。


## <a name="properties"></a>属性

| 属性     | 类型        | 描述| 
|:-------------|:------------|:------------|
|aggregationFilters|String collection|包含一个或多个筛选器，用于获取聚合的搜索结果，并将其筛选为字段的特定值。 可选。<br>基于按同一字段聚合的先前搜索生成此筛选器。 从之前搜索的响应中，确定将结果筛选为字段特定值的 [searchBucket](searchBucket.md) ，在其 **聚合FilterToken** 属性中使用字符串，并生成格式 **为“{field}：\\”{aggregationFilterToken}\\“** 的聚合筛选器字符串。 <br>如果需要为同一字段提供多个值，请使用其 **聚合FilterToken** 属性中的字符串，并生成格式为 **“{field}：或 (\\”{aggregationFilterToken1}\\“、”\\{aggregationFilterToken2}\\“) ”** 的聚合筛选器字符串。 <br>例如，按文件类型搜索和聚合驱动器项会返回响应中文件类型的 `docx` **searchBucket**。 可以方便地在后续搜索查询中使用为此 **searchBucket** 返回的 **聚合FilterToken**，并根据筛选器向下匹配来驱动文件类型的项目`docx`。 [示例 1](/graph/search-concept-aggregation#example-1-request-aggregations-by-string-fields) 和 [示例 2](/graph/search-concept-aggregation#example-2-apply-an-aggregation-filter-based-on-a-previous-request) 显示实际请求和响应。|
|聚合|[aggregationOption](aggregationOption.md) 集合|指定要与搜索结果一起返回的聚合 (也称为精简程序) 。 可选。|
|contentSources|String collection|包含要成为目标的连接。|
|enableTopResults|Boolean|这会触发消息的混合排序：前 3 条消息最相关。 此属性仅适用于 entityType=`message`。 可选。|
|entityTypes|entityType 集合| 响应中预期的一种或多种资源类型。 可取值为：`list`、`site`、`listItem`、`message`、`event`、`drive`、`driveItem`、`externalItem`。 请参阅同一搜索请求中支持的两个或更多实体类型的这些组合的 [已知限制](search-api-overview.md#known-limitations) 。 必需项。|
|fields|String collection |包含要为 **entityTypes** 中指定的每个资源对象返回的字段，允许自定义默认返回的字段;否则，包括其他字段（例如来自 SharePoint 和 OneDrive 的自定义托管属性）或 Microsoft Graph 连接器引入的内容的 **externalItem** 中的自定义字段。 字 **段** 属性可以使用应用于属性 [的语义标签](/microsoftsearch/configure-connector#step-6-assign-property-labels) 。 例如，如果属性标记为标题，则可以使用以下语法检索该属性： `label_title` 可选。|
|发件人|Int32|指定搜索结果的偏移量。 偏移量 0 返回第一个结果。 可选。|
|查询|[searchQuery](searchquery.md)|包含查询词。 必需项。|
|queryAlterationOptions|[searchAlterationOptions](searchalterationoptions.md)|JSON Blob 中格式化的查询更改选项，其中包含两个与拼写更正相关的可选标志。 可选。 |
|resultTemplateOptions|[resultTemplateOption](resulttemplateoption.md) 集合|提供搜索结果模板选项以从连接器呈现搜索结果。|
|size|Int32|要检索的页面的大小。最大值为 1000。 可选。|
|sortProperties|[sortProperty](sortProperty.md) 集合|包含对结果进行排序的字段和方向的有序集合。 集合中最多可以有 5 个排序属性。 可选。|

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
- 搜索SharePoint和OneDrive ([文件、列表和网站](/graph/search-concept-files)中的内容) 
- 对搜索结果[进行排序](/graph/search-concept-sort)
- 使用 [聚合](/graph/search-concept-aggregations) 优化搜索结果
- 使用 [显示布局](/graph/search-concept-display-layout.md)
- 在搜索结果中启用[拼写更正](/graph/search-concept-speller)


<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "searchRequest resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


