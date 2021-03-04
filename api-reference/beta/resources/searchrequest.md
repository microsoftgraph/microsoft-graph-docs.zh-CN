---
ms.author: yiwenwang
title: searchRequest 资源类型
description: 要发送到查询终结点的搜索请求。 它包含响应中预期的实体类型、基础源、分页参数、字段请求和实际搜索查询。
localization_priority: Normal
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 7deba4c4c59947505b0ed6eff61a0d9cae5d59ef
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50440121"
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

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|:------------|
|聚合|[aggregationOption](aggregationOption.md) 集合|指定与 (一起返回) 精简程序。 可选。|
|aggregationFilters|字符串集合|包含一个或多个筛选器，用于获取聚合并筛选为字段特定值的搜索结果。 可选。<br>基于按同一字段聚合的先前搜索生成此筛选器。 从之前搜索的响应中，确定将结果筛选为字段特定值的 [searchBucket，](searchBucket.md) 在其 **aggregationFilterToken 属性中使用该** 字符串，并构建一个聚合筛选器字符串，格式为 **"{field}： \\ "{aggregationFilterToken} \\ ""**。 <br>如果需要为同一字段提供多个值，请使用 **其 aggregationFilterToken** 属性中的字符串，并生成一个聚合筛选器字符串，格式为 **"{field}：或 \\ ("{aggregationFilterToken1} \\ "， \\ "{aggregationFilterToken2} \\ ") "。** <br>例如，按文件类型搜索和聚合驱动器项在响应中返回文件类型的 **searchBucket。** `docx` 在后续搜索查询中，可以方便地使用此 **searchBucket** 返回的 **aggregationFilterToken，** 筛选器向下匹配以驱动 `docx` 文件类型的项。 [示例 1](/graph/search-concept-aggregation#example-1-request-aggregations-by-string-fields) [和示例 2](/graph/search-concept-aggregation#example-2-apply-an-aggregation-filter-based-on-a-previous-request) 显示实际请求和响应。|
|contentSources|字符串集合|包含要定向的连接。 <br>遵循以下格式：在连接器管理中定义 `/external/connections/connectionid` `connectionid` ConnectionId 的位置。 <br> 注意：contentSource 仅适用于 entityType= `externalItem` 。 可选。|
|enableTopResults|布尔|这将触发邮件的混合排序：前 3 条消息最相关。 此属性仅适用于 entityType= `message` 。 可选。|
|entityTypes|entityType 集合| 响应中预期的一种或多种资源类型。 可取值为：`list`、`site`、`listItem`、`message`、`event`、`drive`、`driveItem`、`externalItem`。 请参阅 [同一](search-api-overview.md#known-limitations) 搜索请求中支持的两个或多个实体类型的这些组合的已知限制。 必需。|
|fields|字符串集合 |包含为 **entityTypes** 中指定的每个资源对象返回的字段，从而允许自定义默认情况下返回的字段，包括其他字段（如 SharePoint 和 OneDrive 中的自定义托管属性）或 Microsoft Graph 连接器引入的内容中的 **externalItem** 中的自定义字段。 <br>fields 属性可以使用应用于 [属性的](https://docs.microsoft.com/microsoftsearch/configure-connector#step-5-assign-property-labels) 语义标签。 例如，如果属性标记为标题，可以使用以下语法进行检索：label_title。<br>可选。|
|发件人|Int32|指定搜索结果的偏移量。 偏移量 0 返回第一个结果。 可选。|
|查询|[searchQuery](searchquery.md)|包含查询词。 必需。|
|size|Int32|要检索的页面的大小。 可选。|
|sortProperties|[sortProperty](sortProperty.md) 集合|包含排序结果的字段和方向的有序集合。 集合中最多只能有 5 个排序属性。 可选。|
|stored_fields (已弃) |字符串集合 |现在，这被 **fields 属性** 所取代。 |


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
- 搜索 [邮件](/graph/search-concept-messages)
- 搜索 [日历事件](/graph/search-concept-events)
- 搜索 SharePoint 和 OneDrive ([文件、列表和网站) ](/graph/search-concept-files)
- 搜索 [使用连接器导入的自定义) ](/graph/search-concept-custom-types) 数据
- [对](/graph/search-concept-sort) 搜索结果进行排序
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


