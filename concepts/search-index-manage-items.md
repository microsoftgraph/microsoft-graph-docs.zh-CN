---
title: 创建、更新和删除应用程序在 Microsoft 搜索服务索引中添加的项目
description: 了解如何使用 Microsoft Graph 管理应用程序添加到 Microsoft 搜索服务的项目
localization_priority: Priority
author: snlraju-msft
ms.prod: ''
doc_type: conceptualPageType
ms.openlocfilehash: c5017943f966792e0246d3764a1c3e373718c63c
ms.sourcegitcommit: ef8eac3cf973a1971f8f1d41d75a085fad3690f0
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/19/2019
ms.locfileid: "38704334"
---
# <a name="create-update-and-delete-items-added-by-your-application-in-the-microsoft-search-service-index"></a>创建、更新和删除应用程序在 Microsoft 搜索服务索引中添加的项目

应用程序添加到 Microsoft 搜索服务的项目由 Microsoft Graph 中的 [externalItem](/graph/api/resources/externalitem?view=graph-rest-beta) 和 [externalFile](/graph/api/resources/externalfile?view=graph-rest-beta) 资源表示。

[!INCLUDE [search-api-preview-signup](../includes/search-api-preview-signup.md)]

“externalItem”**** 资源表示自定义类型。 当添加到索引的项使用“externalFile”**** 资源未表示的自定义架构时，应使用此方法。 例如，支持人员票证或产品清单。

“externalFile”**** 资源表示外部系统中的文件。

> [!NOTE]
> 无法扩展“externalFile”**** 的架构。

## <a name="add-an-item-or-file"></a>创建项目或文件

可通过[创建 externalItem](/graph/api/externalconnection-put-items?view=graph-rest-beta)，将项目或文件添加到索引。 创建项目时，可在 URL 中分配唯一的标识符。

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

## <a name="update-an-item-or-file"></a>更新项目或文件

在外部服务中更新项目或文件（重新分配支持人员票证或更新产品说明）时，可以使用创建项目时分配给项目的唯一标识符，通过[更新 externalItem](/graph/api/externalitem-update?view=graph-rest-beta) 更新其在索引中的条目。

```http
PATCH /external/connections/contosohelpdesk/items/SR00145
Content-Type: application/json

{
  "assignee": "alexw@contoso.com"
}
```

## <a name="delete-an-item-or-file"></a>删除项目或文件

可以使用创建项目时分配给项目的唯一标识符，通过[删除 externalItem](/graph/api/externalitem-delete?view=graph-rest-beta) 删除索引中的项目或文件。

```http
DELETE /external/connections/contosohelpdesk/items/SR00145
```

## <a name="next-steps"></a>后续步骤

- [为什么使用 Microsoft 搜索 API？](search-concept-overview.md#why-use-the-microsoft-search-api)
- [使用 Microsoft 搜索 API 为数据编制索引](/graph/api/resources/indexing-api-overview?view=graph-rest-beta)
- [搜索自定义类型 (externalItem)](search-concept-custom-types.md)
- [搜索文件（包括 externalFile）](search-concept-files.md)
- 从 GitHub 下载[示例搜索连接器](https://github.com/microsoftgraph/msgraph-search-connector-sample)
