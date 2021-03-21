---
title: 创建、更新和删除应用程序在 Microsoft Graph 连接中添加的项目
description: 了解如何使用 Microsoft Graph 管理应用程序添加到 Microsoft 搜索服务的项目
localization_priority: Priority
author: rsamai
ms.prod: search
doc_type: conceptualPageType
ms.openlocfilehash: c2cae0ca25d55fd95a7b26c0175f7e5313d6e532
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50962397"
---
# <a name="create-update-and-delete-items-added-by-your-application-in-the-microsoft-graph-connection"></a>创建、更新和删除应用程序在 Microsoft Graph 连接中添加的项目

应用程序添加到 Microsoft 搜索服务的项用 Microsoft Graph 中的 [externalItem](/graph/api/resources/externalitem?view=graph-rest-beta&preserve-view=true) 资源表示。

创建连接后，可以添加内容。 数据源中的每个项目都必须用唯一的项目 id 表示为 Microsoft Graph 中的 [externalItem](/graph/api/resources/externalitem?view=graph-rest-beta&preserve-view=true)。此 id 用于在 Microsoft Graph 中创建、更新或删除项目。 你可以将数据源中的主键用作 itemId，或者从一个或多个字段派生。 [externalItem](/graph/api/resources/externalitem?view=graph-rest-beta&preserve-view=true) 有三个关键组成部分：访问控制列表、属性和内容。

## <a name="access-control-list"></a>访问控制列表

访问控制列表用于指定是否授予或拒绝给定角色访问 Microsoft 体验中的查看项目的权限。 它是一组访问控制项，每个项表示一个 Azure Active Directory 用户或组。 有第三个访问控制条目类型 `Everyone` ，表示租户中的所有用户。

![访问控制列表示例](./images/search-index-manage-items-acl.png)

AccessType 值 `deny` 优先于 `grant`。 例如，在上面显示的项目中，如果授予 `Everyone` 访问权限，并且拒绝了特定用户的访问权限，则此用户的有效权限将被 `deny`。

如果数据源具有非 Azure Active Directory 组（例如支持人员系统中的团队），并且用于设置项目的权限，则可以使用组同步 API 复制 `allow` 或 `deny` 权限，在 Microsoft Graph 中创建外部组。 避免将外部组的成员身份直接展开为各项的访问控制列表，因为每个组成员身份更新可能会导致项更新的风暴。

外部组可以由另一个外部组、Azure Active Directory 用户和 Azure Active Directory 组组成。 如果你有非 Azure Active Directory 用户，则必须在访问控制列表中将其转换为 Azure Active Directory 用户。

## <a name="properties"></a>属性

属性组件用于添加在 Microsoft Graph 体验中有用的项元数据。 在向该连接添加项目并将数据类型转换为[支持的数据类型](/graph/api/resources/property?view=graph-rest-beta&preserve-view=true)前，必须[注册该架构](./search-index-manage-schema.md)。

![属性组件示例](./images/search-index-manage-items-1.png)

## <a name="content"></a>内容

内容组件用于添加需要进行全文检索的大量项目。 示例包括票证说明、文件正文中的已分析文本或者 wiki 网页正文。

内容是影响 Microsoft 体验[相关性](./search-index-manage-schema.md#relevance)的关键字段之一。 我们支持类型 `text` 和 `HTML`的内容。 如果数据源有二进制文件，则可以先将它们分析为文本，然后再将其添加到 Microsoft Graph。

![内容组件示例](./images/search-index-manage-items-2.png)

无法直接将内容添加到搜索结果模板中，但你可以使用生成的结果段，该片段是内容中的相关节的动态生成的预览。

![搜索结果模板的屏幕截图](./images/search-index-manage-items-3.svg)

数据源中的内容发生更改时，必须将其与连接项同步。 可更新整个项目或更新它的一个或多个组件。 将内容添加到 Microsoft Graph 后，你可以在设置[纵向和结果类型](/MicrosoftSearch/customize-search-page)或使用 [Microsoft Graph 搜索 API](/graph/api/resources/search-api-overview?view=graph-rest-beta&preserve-view=true) 后，通过 Microsoft 搜索体验搜索该内容。

## <a name="add-an-item"></a>添加项

可通过[创建 externalItem](/graph/api/externalconnection-put-items?view=graph-rest-beta&preserve-view=true)，将项添加到索引。 创建项目时，可在 URL 中分配唯一的标识符。

例如，你的应用程序可能会使用票证编号来索引支持人员票证。 如果票证具有 `SR00145` 票证编号，请求可能如下所示。

```http
PUT /external/connections/contosohelpdesk/items/SR00145
Content-Type: application/json

{
  "title": "WiFi outage in Conference Room A",
  "status": "New",
  "assignee": "meganb@contoso.com"
}
```

> ![注意] 管理员必须先[自定义相应连接的搜索结果页](/MicrosoftSearch/configure-connector#next-steps-customize-the-search-results-page)，然后索引项才能在 Microsoft 搜索 UI 中找到。

## <a name="update-an-item"></a>更新项

当项在外部服务中更新（重新分配支持人员票证或更新产品说明）时，可以使用创建项时分配给项的唯一标识符，通过[更新 externalItem](/graph/api/externalitem-update?view=graph-rest-beta&preserve-view=true) 更新项在索引中的条目。

```http
PATCH /external/connections/contosohelpdesk/items/SR00145
Content-Type: application/json

{
  "assignee": "alexw@contoso.com"
}
```

## <a name="delete-an-item"></a>删除项

可以使用创建项时分配给项的唯一标识符，通过[删除 externalItem](/graph/api/externalitem-delete?view=graph-rest-beta&preserve-view=true) 从索引中删除项。

```http
DELETE /external/connections/contosohelpdesk/items/SR00145
```

## <a name="next-steps"></a>后续步骤

- [使用 Microsoft 搜索 API 的查询](search-concept-overview.md#why-use-the-microsoft-search-api)
- [查看索引 API 参考](/graph/api/resources/indexing-api-overview?view=graph-rest-beta&preserve-view=true)
- [自定义 Microsoft 搜索结果页](/MicrosoftSearch/customize-search-page)
- [搜索自定义类型 (externalItem)](search-concept-custom-types.md)
- 从 GitHub 下载[示例搜索连接器](https://github.com/microsoftgraph/msgraph-search-connector-sample)