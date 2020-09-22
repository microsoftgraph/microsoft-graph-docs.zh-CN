---
title: 使用 Microsoft 搜索 API 查询数据
description: 使用搜索 API，应用程序可以在已认证用户的上下文中搜索 Microsoft 365 数据
localization_priority: Priority
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: e77c0170487b0762538d98376921565857c9b3c8
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47985783"
---
# <a name="use-the-microsoft-search-api-to-query-data"></a>使用 Microsoft 搜索 API 查询数据

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

可使用 Microsoft 搜索 API 来查询应用程序中的 Microsoft 365 数据。

搜索请求在登录用户的上下文中运行，并使用[包含委派权限的访问令牌](/graph/auth-v2-user)进行标识。

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="common-use-cases"></a>常见用例

Microsoft 搜索 API 提供了[查询](../api/search-query.md)方法，可在 Microsoft 搜索中跨数据搜索。 本部分列出了常见用例，具体取决于在**查询**请求正文中设置的属性。

代表用户运行搜索请求。 设定搜索结果范围，以强制执行应用到项目的任何访问控制。  例如，在文件的上下文中，将在搜索请求过程中评估对文件的权限。 用户在搜索中可访问的项目数不得多于其可通过枚举 API 调用的项目数。

| 用例 | 要在查询请求正文中定义的属性 |
|:------------------|:---------|
|[根据实体类型限定搜索范围](#scope-search-based-on-entity-types)| **entityTypes** |
|[页面结果](#page-search-results) | **起始数量**和**大小** |
|[获取最相关的电子邮件](#get-the-most-relevant-emails) | **enableTopResults** |
|[获取选定属性](#get-selected-properties) | **stored_fields** |
|[在查询条款中使用 KQL](#keyword-query-language-kql-support) | **查询** |
|[搜索外部文件](/graph/search-concept-files)| **entityTypes** |
|[在特定 contentSource 中搜索（索引 API）](/graph/search-concept-custom-types)| **contentSources** |

### <a name="scope-search-based-on-entity-types"></a>根据实体类型限定搜索范围

使用**查询**请求有效负载中的 **entityTypes** 属性定义搜索请求的范围。
下面是支持的实体类型：

- [event](event.md)
- [message](message.md)
- [driveItem](driveitem.md)
- [externalFile](externalfile.md)
- [externalItem](externalitem.md)

### <a name="page-search-results"></a>页面搜索结果

通过在**查询**请求正文中指定以下两个属性来控制搜索结果的分页：

- **起始数量** - 一个整数，它表示从 0 开始的起始数，在页面上列出搜索结果。 默认值为 0。

- **大小** - 一个整数，它表示要为页面返回的结果数。 默认值为 25。

如果你正在搜索 **event** 或 **message** 实体，则注意以下限制：

- **起始数量**在第一个页面请求中必须从零开始，否则请求将导致出现 HTTP 400 `Bad request`。
- 每页的最大结果数（**大小**）为 200。
- 分页可返回的最大总项数为 1000。
- 超出限制将返回最佳响应。 请求不会导致 HTTP 400。

最佳实践：

- 指定初始请求中的较小的首页。 例如，将**起始数量**指定为 0，将**大小**指定为 25。
- 通过更新**起始数量**和**大小**属性来对后续页面进行分页。 可以在每个后续请求中增加页面大小。 下表显示了一个示例。

    | 页面 | 起始数量 | 大小 |
    |:-----|:-----|:-----|
    | 1    | 0 | 25 |
    | 2    | 25 | 50 |
    | 3    | 75 | 75 |
    | 4    | 150 | 100 |

### <a name="get-the-most-relevant-emails"></a>获取最相关的电子邮件

搜索 **message** 实体时，将 **enableTopResults** 指定为 `true` 返回邮件的混合列表：响应中的前 3 封邮件按相关性排序，剩余邮件按日期排序。

### <a name="get-selected-properties"></a>获取选定属性

搜索 **externalItem** 实体时，使用 **stored_fields** 属性指定要在响应中返回的字段。

**stored_fields** 中指定的字段应为可检索的托管属性，且它们已通过 Microsoft 搜索租户管理针对连接进行了配置。

### <a name="keyword-query-language-kql-support"></a>关键字查询语言 (KQL) 支持

在实际搜索查询字符串（**查询**请求正文的**查询**属性）中的 KQL 语法中，指定自由文本关键字、运算符（例如 `AND`、`OR`）和属性限制。 语法和命令取决于在同一**查询**请求主体中指向的实体类型（在 **entityTypes** 属性中）。

可搜索的属性各不相同，具体取决于实体类型。 有关详细信息，请参阅：

- [电子邮件属性](/microsoft-365/compliance/keyword-queries-and-search-conditions#searchable-email-properties)
- [站点属性](/microsoft-365/compliance/keyword-queries-and-search-conditions#searchable-site-properties)

## <a name="error-handling"></a>错误处理

搜索 API 将返回由 [OData 错误对象定义](http://docs.oasis-open.org/odata/odata-json-format/v4.01/cs01/odata-json-format-v4.01-cs01.html#sec_ErrorResponse)所定义的错误响应，其中每个是包含代码和消息的 JSON 对象。

<!---TODO Describe the know errors : bad requests.--->

## <a name="known-limitations"></a>已知限制

搜索 API 存在以下限制：

- 定义**查询**方法，以允许一次传递一个或多个 **searchRequest** 实例的集合。 但是，该服务当前仅支持一次传递一个 [searchRequest](./searchrequest.md)。

- [searchRequest](./searchrequest.md) 资源支持一次传递多个类型的实体。 但是，当前唯一支持的组合是 **driveItem** 和 **externalFile**。 其他组合无效。

- 仅当将 **entityType** 指定为 `externalItem` 时，定义要使用的连接的 **contentSource** 属性才适用。
<!--todo nmoreauteam Fix the link to ContentSource  pls provide the content source url--->

- 搜索 API 不支持自定义排序，并且始终通过以下方式对结果进行排序：

  - 按日期对 **message** 或 **event** 类型结果进行排序。

  - 按相关性对 **driveItem**、**externalFile** 或 **externalItem** 类型结果进行排序。

## <a name="whats-new"></a>最近更新
了解此 API 集的[最新功能和更新](/graph/whats-new-overview)。


