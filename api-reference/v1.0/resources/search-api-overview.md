---
title: 使用 Microsoft 搜索 API 查询数据
description: 使用搜索 API，应用程序可以在已认证用户的上下文中搜索 Microsoft 365 数据
ms.localizationpriority: high
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: e7d2ce6d2eb973eb68b4cbe14754c374eec9bd3c
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59035610"
---
# <a name="use-the-microsoft-search-api-to-query-data"></a>使用 Microsoft 搜索 API 查询数据

可使用 Microsoft 搜索 API 来查询应用程序中的 Microsoft 365 数据。

搜索请求在登录用户的上下文中运行，并使用[包含委派权限的访问令牌](/graph/auth-v2-user)进行标识。

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

搜索实体类型，如 **message**、**event**、**drive**、**driveItem**、**list**、**listItem**、**site**、**externalItem**，可以在 **fields** 属性中包含特定的实体属性，以便在搜索结果中返回。 这类似于使用 [OData 系统查询选项，REST 请求中的 $select](/graph/query-parameters#select-parameter)。 搜索 API 技术上不支持这些查询选项，因为会在文章正文中表达该行为。

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

## <a name="error-handling"></a>错误处理

搜索 API 将返回由 [OData 错误对象定义](http://docs.oasis-open.org/odata/odata-json-format/v4.01/cs01/odata-json-format-v4.01-cs01.html#sec_ErrorResponse)所定义的错误响应，其中每个是包含代码和消息的 JSON 对象。

<!---TODOSEARCHAPI Describe the know errors: bad requests.--->

## <a name="known-limitations"></a>已知限制

搜索 API 存在以下限制：

- 定义 **查询** 方法，以允许一次传递一个或多个 **searchRequest** 实例的集合。 但是，该服务当前仅支持一次传递一个 [searchRequest](./searchrequest.md)。

- [searchRequest](./searchrequest.md) 资源支持一次传递多个类型的实体。 但是，目前仅支持 SharePoint 和 OneDrive entityTypes 的组合为：**driveItem**、**drive**、**site**、**list**、**listItem**。
当前不支持任何涉及 **message**、**event**、Sharepoint 和 OneDrive 类型或 **externalItem** 的组合。  

- 仅当将 **entityType** 指定为 `externalItem` 时，定义要使用的连接的 **contentSource** 属性才适用。

- 搜索 API 不支持 **message**、**event** 或 **externalItem** 的自定义排序。

- 搜索 API 不支持 **message**、**event**、**site** 或 **drive** 的聚合。

- SharePoint 搜索中的自定义设置（如自定义搜索架构或结果源）可能会干扰 Microsoft 搜索 API 的操作。

## <a name="see-also"></a>另请参阅

- 了解有关几个关键用例的详细信息：
  - [搜索 Outlook 邮件](/graph/search-concept-messages)
  - [搜索日历事件](/graph/search-concept-events)
  - [SharePoint 和 OneDrive 中的搜索内容](/graph/search-concept-files)

- 在 [Graph 浏览器](https://developer.microsoft.com/graph/graph-explorer)中探索搜索 API。
- 了解此 API 集的[最新功能和更新](/graph/whats-new-overview)。
