---
title: searchRequest 资源类型
description: 要发送到查询终结点的搜索请求。 它包含响应中预期的实体类型、基础源、分页参数、字段请求和实际搜索查询。
localization_priority: Normal
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 747bacce74028d785d54ce0b8fb27303fccbbc1a
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/30/2021
ms.locfileid: "53210316"
---
# <a name="searchrequest-resource-type"></a>searchRequest 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [search-api-deprecation](../../includes/search-api-deprecation.md)]

JSON blob 中格式化的搜索请求。 

JSON blob 包含响应中预期的资源类型、基础源、分页参数、排序选项、请求的聚合和字段以及实际搜索查询。 请参阅 [各种](#see-also) 资源上的搜索请求示例。

> [!NOTE]
> 请注意搜索 [实体](search-api-overview.md#known-limitations) 类型的特定组合以及排序或聚合搜索结果的已知限制。

## <a name="properties"></a>属性

| 属性     | 类型        | 说明             
|:-------------|:------------|:------------
|聚合|[aggregationOption](aggregationOption.md) 集合|指定聚合 (也称为) 搜索结果一起返回的精简条件。 可选。|
|aggregationFilters|String collection|包含一个或多个筛选器，用于获取聚合的搜索结果并按字段的特定值进行筛选。 可选。<br>基于之前按同一字段聚合的搜索生成此筛选器。 从之前搜索的响应中，确定将结果筛选为字段的特定值的 [searchBucket，](searchBucket.md) 在其 **aggregationFilterToken** 属性中使用该字符串，并生成格式为 **"{field}： \\ "{aggregationFilterToken} \\ ""** 的聚合筛选器字符串。 <br>如果需要为同一字段提供多个值，请使用 **其 aggregationFilterToken** 属性中的字符串，并生成格式为 **"{field}：或 (\\ "{aggregationFilterToken1} \\ \\ ，"{aggregationFilterToken2} \\ ") "** 的聚合筛选器字符串。 <br>例如，按文件类型搜索和聚合驱动器项在响应中返回文件类型的 **searchBucket。** `docx` 您可以在后续搜索查询中方便地使用此 **searchBucket** 返回的 **aggregationFilterToken，** 筛选器向下筛选文件类型的驱动器 `docx` 项。 [示例 1](/graph/search-concept-aggregation#example-1-request-aggregations-by-string-fields) [和示例 2](/graph/search-concept-aggregation#example-2-apply-an-aggregation-filter-based-on-a-previous-request) 显示实际请求和响应。|
|contentSources|String collection|包含要定向的连接。 <br>遵循以下格式： `/external/connections/connectionid` 其中 `connectionid` 是连接器管理中定义的 ConnectionId。 <br> 注意：contentSource 仅在 entityType= 时适用 `externalItem` 。 可选。|
|enableTopResults|Boolean|这将触发邮件的混合排序：前 3 个邮件最相关。 此属性仅适用于 entityType= `message` 。 可选。|
|entityTypes|entityType 集合| 响应中预期的一种或多种资源类型。 可取值为：`list`、`site`、`listItem`、`message`、`event`、`drive`、`driveItem`、`externalItem`。 有关 [同一](search-api-overview.md#known-limitations) 搜索请求中支持的两个或多个实体类型的组合，请参阅已知限制。 必填。|
|fields|String collection |包含为 **entityTypes** 中指定的每个资源对象返回的字段，从而允许自定义默认情况下返回的字段，包括其他字段（如 SharePoint 和 OneDrive 中的自定义托管属性）或 microsoft Graph 连接器引入的内容中的 **externalItem** 中的自定义字段。 <br>fields 属性可以使用应用于 [属性的](https://docs.microsoft.com/microsoftsearch/configure-connector#step-5-assign-property-labels) 语义标签。 例如，如果属性标记为 title，可以使用以下语法检索它：label_title。<br>可选。|
|起始数量|Int32|指定搜索结果的偏移量。 偏移量 0 返回第一个结果。 可选。|
|查询|[searchQuery](searchquery.md)|包含查询词。 必填。|
|size|Int32|要检索的页面的大小。 可选。|
|sortProperties|[sortProperty](sortProperty.md) 集合|包含排序的字段集合和排序结果的方向。 集合中最多只能有 5 个排序属性。 可选。|
|stored_fields (弃用) |String collection |现在，这将由 **fields 属性** 替换。 |
|resultTemplateOptions|[resultTemplateOption](resultTemplateOption.md) 集合|提供用于呈现连接器搜索结果的搜索结果模板选项。|


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
  "enableTopResults": true,
  "resultTemplateOptions": [{"@odata.type": "microsoft.graph.resultTemplateOption"}]  
}
```

## <a name="see-also"></a>另请参阅
- 搜索 [邮件](/graph/search-concept-messages)
- 搜索 [日历事件](/graph/search-concept-events)
- 搜索网站[SharePoint OneDrive (、列表和网站) ](/graph/search-concept-files)
- 搜索 [使用连接器数据导入的自定义](/graph/search-concept-custom-types) 类型
- [对](/graph/search-concept-sort) 搜索结果进行排序
- 使用 [聚合](/graph/search-concept-aggregations) 优化搜索结果
- 使用 [显示布局](/graph/search-concept-display-layout.md)


<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "searchRequest resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


