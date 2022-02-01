---
title: 使用 Microsoft 搜索 API 查询数据
description: 使用搜索 API，应用程序可以在已认证用户的上下文中搜索 Microsoft 365 数据
ms.localizationpriority: high
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 6a30360dddeb06d9f8ac4d1ff5b485229087c3ce
ms.sourcegitcommit: a60e5e81cfa04b666a1df1111a1d91f6c11989e9
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/31/2022
ms.locfileid: "62282034"
---
# <a name="use-the-microsoft-search-api-to-query-data"></a>使用 Microsoft 搜索 API 查询数据

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

可使用 Microsoft 搜索 API 来查询应用程序中的 Microsoft 365 数据。

搜索请求在登录用户的上下文中运行，并使用[包含委派权限的访问令牌](/graph/auth-v2-user)进行标识。

[!INCLUDE [search-api-deprecation](../../includes/search-api-deprecation.md)]

## <a name="common-use-cases"></a>常见用例

Microsoft Search API 提供了[查询](../api/search-query.md)方法，可在 Microsoft Search 中搜索数据，在其请求正文中传递 [searchRequest](searchRequest.md) ，定义搜索的具体内容。

本部分列出了 **查询** 方法的常见用例，具体取决于在 **查询** [searchRequest](searchRequest.md)正文中设置的属性和参数。

代表用户运行搜索请求。 设定搜索结果范围，以强制执行应用到项目的任何访问控制。  例如，在文件的上下文中，将在搜索请求过程中评估对文件的权限。 在搜索中，用户无法访问更多的项目，但可以从具有相同权限和访问控制的相应 GET 操作中获得这些项目。

| 用例 | 要在查询请求正文中定义的属性 |
|:------------------|:---------|
|[根据实体类型限定搜索范围](#scope-search-based-on-entity-types)| **entityTypes** |
|[页面结果](#page-search-results) | **起始数量** 和 **大小** |
|[获取最相关的电子邮件](#get-the-most-relevant-emails) | **enableTopResults** |
|[获取选定属性](#get-selected-properties) | **fields** |
|[在查询条款中使用 KQL](#keyword-query-language-kql-support) | **查询** |
|[排序搜索结果](#sort-search-results)| **sort** |
|[使用聚合优化结果](#refine-results-using-aggregations)| **聚合** |
|[使用连接器搜索导入的自定义类型](/graph/search-concept-custom-types)| **contentSources** |
|[请求拼写更正](#request-spelling-correction)| **queryAlterationOptions** |
|[搜索显示布局](#search-display-layout)（预览版）| **resultTemplateOptions**

## <a name="scope-search-based-on-entity-types"></a>根据实体类型限定搜索范围

使用 **查询** 请求有效负载中的 **entityTypes** 属性定义搜索请求的范围。
下表介绍了可用于查询的类型以及访问数据所支持的权限。

| EntityType | 访问项目所需的权限范围| Source| 评论|
|:------------------|:---------|:---------|:---------|
|[message](message.md)|Mail.Read、Mail.ReadWrite| Exchange Online| 电子邮件。|
|[event](event.md) |Calendars.Read、Calendars.ReadWrite| Exchange Online|日历事件。 |
|[drive](drive.md)|Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All| SharePoint | 文档库。|
|[driveItem](driveitem.md)|Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All| SharePoint 和 OneDrive | 文件、文件夹、页面和新闻。 |
|[列表](list.md)|Sites.Read.All、Sites.ReadWrite.All| SharePoint 和 OneDrive | 列表。 请注意，文档库也作为列表返回。 |
|[listItem](listitem.md)|Sites.Read.All、Sites.ReadWrite.All| SharePoint 和 OneDrive | 列表项。 请注意，文件和文件夹也作为列表项返回；**driveItem** 是 **driveItem** 的超类。 |
|[网站](site.md)|Sites.Read.All、Sites.ReadWrite.All| SharePoint | SharePoint 中的网站。|
|[externalItem](externalconnectors-externalitem.md)|ExternalItem.Read.All| Microsoft Graph 连接器| 所有内容通过 Microsoft Graph 连接器 API 摄取。|
|[人员](person.md)|People.Read|Exchange Online|组织中的个人联系人、联系人或可寻址对象。|

## <a name="page-search-results"></a>页面搜索结果

通过在 **查询** 请求正文中指定以下两个属性来控制搜索结果的分页：

- **起始数量** - 一个整数，它表示从 0 开始的起始数，在页面上列出搜索结果。 默认值为 0。

- **大小** - 一个整数，它表示要为页面返回的结果数。 默认值为 25。

如果你正在搜索 **event** 或 **message** 实体，则注意以下限制：

- **起始数量** 在第一个页面请求中必须从零开始，否则请求将导致出现 HTTP 400 `Bad request`。
- 每页的 **message** 和 **event** 最大结果数（**大小**）为 25。

SharePoint 或 OneDrive 项没有上限。 合理的页面大小是 200。 较大的页面大小通常会导致更高的延迟。

最佳实践：

- 指定初始请求中的较小的首页。 例如，将 **起始数量** 指定为 0，将 **大小** 指定为 25。
- 通过更新 **起始数量** 和 **大小** 属性来对后续页面进行分页。 可以在每个后续请求中增加页面大小。 下表显示了一个示例。

    | 页面 | 起始数量 | 大小 |
    |:-----|:-----|:-----|
    | 1    | 0 | 25 |
    | 2    | 25 | 50 |
    | 3    | 75 | 75 |
    | 4    | 150 | 100 |

## <a name="get-the-most-relevant-emails"></a>获取最相关的电子邮件

搜索 **message** 实体时，将 **enableTopResults** 指定为 `true` 返回邮件的混合列表：响应中的前 3 封邮件按相关性排序，剩余邮件按日期/时间排序。

## <a name="get-selected-properties"></a>获取选定属性

搜索实体类型，如 **消息**、**事件**、**驱动**、**driveItem**、**列表**、**listItem**、**网站**、**externalItem** 或 **人员**，可以在 **字段** 属性中包含特定的实体属性，以便在搜索结果中返回。 这类似于使用 [OData 系统查询选项，REST 请求中的 $select](/graph/query-parameters#select-parameter)。 搜索 API 技术上不支持这些查询选项，因为会在文章正文中表达该行为。

对于所有这些实体类型，指定 **fields** 属性可减少响应中返回的属性数，从而通过网络优化负载。

**listItem** 和 **externalItem** 实体是唯一受支持的实体，可用于获取架构中配置的扩展可检索字段。 无法使用搜索 API 从所有其他实体检索扩展属性。 例如，如果在搜索架构中创建了 **externalItem** 的可检索字段，或者在 **listItem** 上有可检索自定义列，则可以从搜索中检索这些属性。 若要检索文件的扩展属性，请在请求中指定 **listItem** 类型。

如果请求中指定的 **字段** 在架构中不存在，或者未标记为可检索，则在响应中将不会返回这些字段。 请求中的无效字段将忽略静默。

如果你在请求中未指定任何 **字段**，则将获得所有类型的默认属性集。 对于扩展属性，在请求中未传递任何 **字段** 时，**listItem** 和 **externalItem** 的行为不同：

- **listItem** 不会返回任何自定义字段。
- **externalItem** 将返回该特定连接的 Microsoft Graph 连接器架构中标记有 **retrievable** 属性的所有字段。

## <a name="keyword-query-language-kql-support"></a>关键字查询语言 (KQL) 支持

在实际搜索查询字符串（**查询** 请求正文的 **查询** 属性）中的 KQL 语法中，指定自由文本关键字、运算符（例如 `AND`、`OR`）和属性限制。 语法和命令取决于在同一 **查询** 请求主体中指向的实体类型（在 **entityTypes** 属性中）。

可搜索的属性各不相同，具体取决于实体类型。有关详细信息，请参阅：

- [电子邮件属性](/microsoft-365/compliance/keyword-queries-and-search-conditions#searchable-email-properties)
- [站点属性](/microsoft-365/compliance/keyword-queries-and-search-conditions#searchable-site-properties)

## <a name="sort-search-results"></a>排序搜索结果

响应中的搜索结果按以下默认排序顺序排列：

- **message** 和 **event** 按日期进行排序。
- 所有 SharePoint、OneDrive 人员和连接器类型都按相关性排序。

[query](../api/search-query.md) 方法可通过在 `requests` 参数中指定 **sortProperties** 来自定义搜索顺序，后者是 [searchRequest](./searchrequest.md) 对象的集合。 这可用于指定一个或多个可排序的属性列表和排序顺序。

请注意，目前仅支持以下 SharePoint 和 OneDrive 类型的排序结果：[driveItem](driveitem.md)、[listItem](listitem.md)、[list](list.md)、[site](site.md)。

应用排序子句的属性需要在 SharePoint [搜索架构](/sharepoint/manage-search-schema)中可排序。 如果请求中指定的属性不可排序或不存在，则响应将返回错误， `HTTP 400 Bad Request`。 请注意，不能指定按使用 [sortProperty](sortproperty.md) 的相关性对文档进行排序。

指定 [sortProperty](sortproperty.md) 对象的 **名称** 时，可使用 Microsoft Graph 类型的属性名称（例如 [driveItem](driveitem.md)），或搜索索引中托管属性的名称。

有关演示如何对结果进行排序的示例，请参阅[对搜索结果进行排序](/graph/search-concept-sort)。

## <a name="refine-results-using-aggregations"></a>使用聚合优化结果

聚合（SharePoint 中也称为精简程序）是增强搜索体验的一种常见的方式。 除结果外，还提供有关匹配的搜索结果集的一些级别的聚合信息。 例如，你可以提供与查询匹配的文档最多作者和表示的文件类型等信息。

在 [searchRequest](./searchrequest.md)中，指定除了搜索结果以外应返回的聚合。 每个聚合的说明在 [aggregationOption](./aggregationoption.md) 中定义，其指定要在其中计算聚合的属性，以及在响应中需要返回的 [searchBucket](searchBucket.md) 数目。

应用排序子句的属性需要在 SharePoint [搜索架构](/sharepoint/manage-search-schema)中可排序。 如果指定的属性不可精简或不存在，则响应将返回 `HTTP 400 Bad Request`。

返回包含 [searchBucket](searchBucket.md) 对象的集合的响应后，可将搜索请求精确到 [searchBucket](searchBucket.md)中包含的匹配元素。 为实现此操作，可将 **aggregationFilters** 属性中的 **aggregationsFilterToken** 值返回到后续 [searchRequest](./searchrequest.md)中。

聚合目前仅支持在以下 SharePoint 和 OneDrive 类型上的任何可细化属性：[driveItem](driveitem.md)、[listItem](listitem.md)、[列表](list.md)、[网站](site.md)以及在Microsoft Graph 连接器上的 [externalItem](externalconnectors-externalitem.md)。

请参阅[优化搜索结果](/graph/search-concept-aggregation) ，显示使用聚合增强和缩小搜索结果的示例。

## <a name="request-spelling-correction"></a>请求拼写更正

拼写更正是处理用户查询中的拼写错误和匹配内容中正确单词之间差异的常用方法。 在原始用户查询中检测到拼写错误时，可以获得原始用户查询或更正的备用查询的搜索结果。 还可以在 [searchresponse](searchresponse.md) 的 **queryAlterationResponse** 属性中获取拼写错误的拼写更正信息。

在 [searchRequest](./searchrequest.md) 中，指定应应用于查询以进行拼写更正的 **queryAlterationOptions**。 有关 **queryAlterationOptions** 属性的详细信息，请参阅 [searchAlterationOptions](./searchalterationoptions.md)。

有关如何使用拼写更正的示例，请参见[请求拼写更正](/graph/search-concept-speller)。

## <a name="search-display-layout"></a>搜索显示布局

借助搜索 API，可以使用 IT 管理员为每个连接器配置的显示布局或结果模板，呈现来自[连接器](/microsoftsearch/connectors-overview)的搜索结果。 结果模板为[自适应卡片](https://adaptivecards.io/)，是布局和数据的语义上有意义的组合。

若要在 [searchresponse](searchresponse.md) 中获取结果模板，必须将在 [searchRequest](./searchrequest.md)中，将 [resultTemplateOptions](./resulttemplateoption.md) 中定义的 **enableResultTemplate** 属性设置为 **true**。 响应包括每个 [搜索命中](./searchhit.md)的 **resultTemplateId**，它映射到包含在响应中的 **resultTemplates** 中包含的显示布局之一。

相关示例，请参阅[使用搜索显示布局](/graph/search-concept-display-layout)。

## <a name="error-handling"></a>错误处理

搜索 API 将返回由 [OData 错误对象定义](http://docs.oasis-open.org/odata/odata-json-format/v4.01/cs01/odata-json-format-v4.01-cs01.html#sec_ErrorResponse)所定义的错误响应，其中每个是包含代码和消息的 JSON 对象。

<!---TODOSEARCHAPI Describe the know errors: bad requests.--->

## <a name="known-limitations"></a>已知限制

搜索 API 存在以下限制：

- 定义 **查询** 方法，以允许一次传递一个或多个 **searchRequest** 实例的集合。 但是，该服务当前仅支持一次传递一个 [searchRequest](./searchrequest.md)。

- [searchRequest](./searchrequest.md) 资源支持一次传递多个类型的实体。 但是，目前仅支持 SharePoint 和 OneDrive entityTypes 的组合为：**driveItem**、**drive**、**site**、**list**、**listItem**。
当前不支持任何涉及 **消息**、**事件**、**p人员**、Sharepoint 和 OneDrive 类型或 **externalItem** 的组合。

- 仅当将 **entityType** 指定为 `externalItem` 时，定义要使用的连接的 **contentSource** 属性才适用。

- 搜索 API 不支持 **消息**、**事件**、**人员**、或 **externalItem** 的自定义排序。

- 搜索 API 不支持 **消息**、**事件**、**网站**、**人员** 或 **驱动** 的聚合。

- SharePoint 搜索中的自定义设置（如自定义搜索架构或结果源）可能会干扰 Microsoft 搜索 API 的操作。

## <a name="schema-change-deprecation-warning"></a>架构更改否决警告

**在测试版中**，已重命名或删除搜索请求和响应中使用的属性。 在大多数情况下，原始属性将被否决并被当前属性替换，如下表所列。

开始更新任何现有应用，以使用当前属性和类型名称，以及在响应中获取当前属性名称。
为使向后兼容，原始属性和类型可访问且可以正常工作，直到 **2020 年 12 月 31 日**，之后它们将被删除。

| 资源                           | 更改类型   | 原始属性 | 当前属性|
|:-----------------------------------|:--------------|:------------------|:----------------|
| [searchRequest](./searchrequest.md)| 重命名属性 | **stored_fields** | **fields**      |
| [searchQuery](./searchquery.md)    | 重命名属性 | **query_string** | **queryString** |
| [searchQueryString](./searchquerystring.md) | 弃用资源 | 不适用 | 不适用 |
| [searchHit](./searchhit.md)        | 重命名属性 | **_id** | **hitId** |
| [searchHit](./searchhit.md)        | 重命名属性 | **_score** | **rank** |
| [searchHit](./searchhit.md)        | 删除属性 | **_sortField** | 不适用 |
| [searchHit](./searchhit.md)        | 重命名属性 | **_source** | **resource** |
| [searchHit](./searchhit.md)        | 重命名属性 | **_summary**  | **summary**  |
| [entityTypes](./enums.md)          | 重命名枚举值 | **unknownfuturevalue**  | **unknownFutureValue**  |

## <a name="see-also"></a>另请参阅

- 了解有关几个关键用例的详细信息：
  - [搜索 Outlook 邮件](/graph/search-concept-messages)
  - [搜索日历事件](/graph/search-concept-events)
  - [搜索人员](/graph/search-concept-person)
  - [SharePoint 和 OneDrive 中的搜索内容](/graph/search-concept-files)
  - [使用连接器搜索导入的自定义类型](/graph/search-concept-custom-types)
  - [排序搜索结果](/graph/search-concept-sort)
  - [改进搜索结果](/graph/search-concept-aggregation)
  - [请求拼写更正](/graph/search-concept-speller)
  - [用户搜索显示布局](/graph/search-concept-display-layout)

- 在 [Graph 浏览器](https://developer.microsoft.com/graph/graph-explorer) 中浏览搜索 API。

## <a name="whats-new"></a>最近更新

了解此 API 集的[最新功能和更新](/graph/whats-new-overview)。
