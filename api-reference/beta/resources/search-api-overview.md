---
title: 使用 Microsoft 搜索 API 查询数据
description: 使用搜索 API，应用程序可以在已认证用户的上下文中搜索 Microsoft 365 数据
localization_priority: Priority
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 36e953866de02e81910d1b75397e90cf7fdd0f29
ms.sourcegitcommit: 7ceec757fd82ef3fd80aa3089ef46d3807aa3aa2
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/09/2020
ms.locfileid: "48405321"
---
# <a name="use-the-microsoft-search-api-to-query-data"></a>使用 Microsoft 搜索 API 查询数据

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

可使用 Microsoft 搜索 API 来查询应用程序中的 Microsoft 365 数据。

搜索请求在登录用户的上下文中运行，并使用[包含委派权限的访问令牌](/graph/auth-v2-user)进行标识。

[!INCLUDE [search-api-deprecation](../../includes/search-api-deprecation.md)]

## <a name="common-use-cases"></a>常见用例

Microsoft Search API 提供了[查询](../api/search-query.md)方法，可在 Microsoft Search 中搜索数据，在其请求正文中传递 [searchRequest](searchRequest.md) ，定义搜索的具体内容。

本部分列出了**查询**方法的常见用例，具体取决于在**查询** [searchRequest](searchRequest.md)正文中设置的属性和参数。

Search requests run on behalf of the user. Search results are scoped to enforce any access control applied to the items.  For example, in the context of files, permissions on the files are evaluated as part of the search request. Users cannot access more items in a search than they can otherwise obtain from a corresponding GET operation with the same permissions and access control.

| 用例 | 要在查询请求正文中定义的属性 |
|:------------------|:---------|
|[根据实体类型限定搜索范围](#scope-search-based-on-entity-types)| **entityTypes** |
|[页面结果](#page-search-results) | **起始数量**和**大小** |
|[获取最相关的电子邮件](#get-the-most-relevant-emails) | **enableTopResults** |
|[获取选定属性](#get-selected-properties) | **fields** |
|[在查询条款中使用 KQL](#keyword-query-language-kql-support) | **查询** |
|[排序搜索结果](#sort-search-results)| **sort** |
|[使用聚合优化结果](#refine-results-using-aggregations)| **聚合** |
|[跨图形连接器搜索](/graph/search-concept-custom-types)| **contentSources** |

## <a name="scope-search-based-on-entity-types"></a>根据实体类型限定搜索范围

Define the scope of the search request using the **entityTypes** property in the **query** request payload. The following table describes the types available to query and the supported permissions to access the data.

| EntityType | 访问项目所需的权限范围| Source| 评论|
|:------------------|:---------|:---------|:---------|
|[message](message.md)|Mail.Read、Mail.ReadWrite| Exchange Online| 电子邮件。|
|[event](event.md) |Calendars.Read、Calendars.ReadWrite| Exchange Online|日历事件。 |
|[drive](drive.md)|Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All| SharePoint | 文档库。|
|[driveItem](driveitem.md)|Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All| SharePoint 和 OneDrive | 文件、文件夹、页面和新闻。 |
|[列表](list.md)|Sites.Read.All、Sites.ReadWrite.All| SharePoint 和 OneDrive | Lists. Note that document libraries are also returned as lists. |
|[listItem](listitem.md)|Sites.Read.All、Sites.ReadWrite.All| SharePoint 和 OneDrive | List items. Note that files and folders are also returned as list items; **listItem** is the super class of **driveItem**. |
|[site](site.md)|Sites.Read.All、Sites.ReadWrite.All| SharePoint | SharePoint 中的网站。|
|[externalItem](externalitem.md)|ExternalItem.Read.All| Microsoft Graph 连接器| 所有内容通过 Microsoft Graph 连接器 API 摄取。|

## <a name="page-search-results"></a>页面搜索结果

通过在**查询**请求正文中指定以下两个属性来控制搜索结果的分页：

- **from** - An integer that indicates the 0-based starting point to list search results on the page. The default value is 0.

- **size** - An integer that indicates the number of results to be returned for a page. The default value is 25.

如果你正在搜索 **event** 或 **message** 实体，则注意以下限制：

- **起始数量**在第一个页面请求中必须从零开始，否则请求将导致出现 HTTP 400 `Bad request`。
- 每页的 **message** 和 **event**最大结果数（**大小**）为 25。 

There is no upper limit for SharePoint or OneDrive items. A reasonable page size is 200. A larger page size generally incurs higher latency.

最佳实践：

- Specify a smaller first page in the initial request. For example, specify **from** as 0, **size** as 25.
- Paginate subsequent pages by updating the **from** and **size** properties. You can increase the page size in each subsequent request. The following table shows an example.

    | 页面 | 起始数量 | 大小 |
    |:-----|:-----|:-----|
    | 1    | 0 | 25 |
    | 2    | 25 | 50 |
    | 3    | 75 | 75 |
    | 4    | 150 | 100 |

## <a name="get-the-most-relevant-emails"></a>获取最相关的电子邮件

搜索 **message** 实体时，将 **enableTopResults** 指定为 `true` 返回邮件的混合列表：响应中的前 3 封邮件按相关性排序，剩余邮件按日期/时间排序。

## <a name="get-selected-properties"></a>获取选定属性

When searching an entity type, such as **message**, **event**, **drive**, **driveItem**, **list**, **listItem**, **site**, **externalItem**, you can include in the **fields** property specific entity properties to return in the search results. This is similar to using the [OData system query option, $select](/graph/query-parameters#select-parameter) in REST requests. The search API does not technically support these query options because the behavior is expressed in the POST body.

对于所有这些实体类型，指定 **fields** 属性可减少响应中返回的属性数，从而通过网络优化负载。

The **listItem** and **externalItem** entities are the only supported entities that allow getting extended fields configured in the schema. You cannot retrieve extended properties from all the other entities. For example, if you created a field for **externalItem** in the search schema, or if you have a custom column on a **listItem**, you can retrieve these properties from search. To retrieve an extended property on a file, specify the **listItem** type in the request.

If the **fields** specified in the request are not present in the schema, they will not be returned in the response. Invalid fields in the request are silently ignored.

If you do not specify any **fields** in the request,  you will get the default set of properties for all types. For extended properties, **listItem** and **externalItem** behave differently when no **fields** are passed in the request:

- **listItem** 不会返回任何自定义字段。
- **externalItem** 将返回该特定连接的 Microsoft Graph 连接器架构中标记有 **retrievable** 属性的所有字段。

## <a name="keyword-query-language-kql-support"></a>关键字查询语言 (KQL) 支持

Specify free text keywords, operators (such as `AND`, `OR`), and property restrictions in KQL syntax in the actual search query string (**query** property of the **query** request body). The syntax and command depend on the entity types (in the **entityTypes** property) you target in the same **query** request body.

Depending on the entity type, the searchable properties vary. For details, see:

- [电子邮件属性](/microsoft-365/compliance/keyword-queries-and-search-conditions#searchable-email-properties)
- [站点属性](/microsoft-365/compliance/keyword-queries-and-search-conditions#searchable-site-properties)

## <a name="sort-search-results"></a>排序搜索结果

响应中的搜索结果按以下默认排序顺序排列：

- **message** 和 **event** 按日期进行排序。
- 所有 SharePoint、OneDrive 和连接器类型按相关性排序。

The [query](../api/search-query.md) method lets you customize the search order by specifying the **sortProperties** on the `requests` parameter, which is a collection of [searchRequest](./searchrequest.md) objects. This allows you to specify a list of one or more sortable properties and the sort order.

请注意，目前仅支持以下 SharePoint 和 OneDrive 类型的排序结果：[driveItem](driveitem.md)、[listItem](listitem.md)、[list](list.md)、[site](site.md)。

The properties on which the sort clause are applied need to be sortable in the SharePoint [search schema](/sharepoint/manage-search-schema). If the property specified in the request is not sortable or does not exist, the response will return an error, `HTTP 400 Bad Request`. Note that you cannot specify to sort documents by relevance using [sortProperty](sortproperty.md).

指定 [sortProperty](sortproperty.md) 对象的**名称**时，可使用 Microsoft Graph 类型的属性名称（例如 [driveItem](driveitem.md)），或搜索索引中托管属性的名称。

有关演示如何对结果进行排序的示例，请参阅[对搜索结果进行排序](/graph/search-concept-sort)。

## <a name="refine-results-using-aggregations"></a>使用聚合优化结果

Aggregations (also known as refiners in SharePoint) are a very popular way to enhance a search experience. In addition to the results, they provide some level of aggregate information on the matching set of search results. For example, you can provide information on the most represented authors of the documents matching the query, or the most represented file types, etc.

In the [searchRequest](./searchrequest.md), specify the aggregations that should be returned in addition to the search results. The description of each aggregation is defined in the [aggregationOption](./aggregationoption.md), which specifies the property on which the aggregation should be computed, and the number of [searchBucket](searchBucket.md) to be returned in the response.

The properties on which the aggregation is requested need to be refinable in the SharePoint [search schema](/sharepoint/manage-search-schema). If the property specified is not refinable or does not exist, the response returns `HTTP 400 Bad Request`.

Once the response is returned containing the collection of [searchBucket](searchBucket.md) objects, it is possible to refine the search request to only the matching elements contained in one [searchBucket](searchBucket.md). This is achieved by passing back the  **aggregationsFilterToken** value in the **aggregationFilters** property of the subsequent [searchRequest](./searchrequest.md).

Aggregations are currently only supported on the following SharePoint and OneDrive types: [driveItem](driveitem.md), [listItem](listitem.md), [list](list.md), [site](site.md). Soon they will be supported for refinable properties in [externalItem](externalItem.md) of Microsoft Graph connectors.

请参阅[优化搜索结果](/graph/search-concept-aggregation) ，显示使用聚合增强和缩小搜索结果的示例。

## <a name="error-handling"></a>错误处理

搜索 API 将返回由 [OData 错误对象定义](http://docs.oasis-open.org/odata/odata-json-format/v4.01/cs01/odata-json-format-v4.01-cs01.html#sec_ErrorResponse)所定义的错误响应，其中每个是包含代码和消息的 JSON 对象。

<!---TODOSEARCHAPI Describe the know errors: bad requests.--->

## <a name="known-limitations"></a>已知限制

搜索 API 存在以下限制：

- The **query** method is defined to allow passing a collection of one or more **searchRequest** instances at once. However, the service currently supports only a single [searchRequest](./searchrequest.md) at a time.

- The [searchRequest](./searchrequest.md) resource supports passing multiple types of entities at a time. However, currently the only supported combination is for SharePoint and OneDrive entityTypes: **driveItem**, **drive**, **site**, **list**, **listItem**. Any combinations involving **message**, **event**, SharePoint and OneDrive types , or **externalItem** are currently not supported.  

- 仅当将 **entityType** 指定为 `externalItem` 时，定义要使用的连接的 **contentSource** 属性才适用。

- 搜索 API 不支持 **message**、**event** 或 **externalItem** 的自定义排序。

- 搜索 API 不支持 **message**、**event**、**site** 或 **drive** 的聚合。

## <a name="schema-change-deprecation-warning"></a>架构更改否决警告

Properties used in a search request and response have been renamed or removed. In most cases, the original properties are being deprecated and replaced by the current properties, as listed in the table below.

Start updating any existing apps to use current property and type names, and to get current property names in the response. For backward compatibility, the original properties and types are accessible and functional until **December 31, 2020**, after which they will be removed.

| Resource                           | 更改类型   | 原始属性 | 当前属性|
|:-----------------------------------|:--------------|:------------------|:----------------|
| [searchRequest](./searchrequest.md)| 重命名属性 | **stored_fields** | **fields**      |
| [searchQuery](./searchquery.md)    | 重命名属性 | **query_string** | **queryString** |
| [searchQueryString](./searchquerystring.md) | 弃用资源 | 不适用 | 不适用 |
| [searchHit](./searchhit.md)        | 重命名属性 | **_id** | **hitId** |
| [searchHit](./searchhit.md)        | 重命名属性 | **_score** | **rank** |
| [searchHit](./searchhit.md)        | 删除属性 | **_sortField** | 不适用 |
| [searchHit](./searchhit.md)        | 重命名属性 | **_source** | **resource** |
| [searchHit](./searchhit.md)        | 重命名属性 | **_summary**  | **summary**  |

## <a name="search-samples"></a>搜索示例

- 了解有关几个关键用例的详细信息：
  - [搜索 Outlook 邮件](/graph/search-concept-messages)
  - [搜索日历事件](/graph/search-concept-events)
  - [SharePoint 和 OneDrive 中的搜索内容](/graph/search-concept-files)
  - [搜索外部内容](/graph/search-concept-custom-types)
  - [排序搜索结果](/graph/search-concept-sort)
  - [改进搜索结果](/graph/search-concept-aggregation)

- 在 [Graph 浏览器](https://developer.microsoft.com/graph/graph-explorer)中探索搜索 API。


## <a name="whats-new"></a>最近更新

了解此 API 集的[最新功能和更新](/graph/whats-new-overview)。