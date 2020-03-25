---
title: 创建、更新和删除应用程序在 Microsoft 搜索服务索引中添加的项目
description: 了解如何使用 Microsoft Graph 管理应用程序添加到 Microsoft 搜索服务的项目
localization_priority: Priority
author: snlraju-msft
ms.prod: ''
doc_type: conceptualPageType
ms.openlocfilehash: 5b969bd058b8c1e2790b0039a4369623287f641d
ms.sourcegitcommit: 7baf4847486885edf08ead533c76503cd31a98a4
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/21/2020
ms.locfileid: "42892784"
---
# <a name="create-update-and-delete-items-added-by-your-application-in-the-microsoft-search-service-index"></a>创建、更新和删除应用程序在 Microsoft 搜索服务索引中添加的项目

应用程序添加到 Microsoft 搜索服务的项用 Microsoft Graph 中的 [externalItem](/graph/api/resources/externalitem?view=graph-rest-beta) 资源表示。

[!INCLUDE [search-api-preview-signup](../includes/search-api-preview-signup.md)]

## <a name="add-an-item"></a>添加项

可通过[创建 externalItem](/graph/api/externalconnection-put-items?view=graph-rest-beta)，将项添加到索引。 创建项目时，可在 URL 中分配唯一的标识符。

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

当项在外部服务中更新（重新分配支持人员票证或更新产品说明）时，可以使用创建项时分配给项的唯一标识符，通过[更新 externalItem](/graph/api/externalitem-update?view=graph-rest-beta) 更新项在索引中的条目。

```http
PATCH /external/connections/contosohelpdesk/items/SR00145
Content-Type: application/json

{
  "assignee": "alexw@contoso.com"
}
```

## <a name="delete-an-item"></a>删除项

可以使用创建项时分配给项的唯一标识符，通过[删除 externalItem](/graph/api/externalitem-delete?view=graph-rest-beta) 从索引中删除项。

```http
DELETE /external/connections/contosohelpdesk/items/SR00145
```

## <a name="next-steps"></a>后续步骤

- [为什么使用 Microsoft 搜索 API？](search-concept-overview.md#why-use-the-microsoft-search-api)
- [查看索引 API 参考](/graph/api/resources/indexing-api-overview?view=graph-rest-beta)
- [自定义 Microsoft 搜索结果页](/MicrosoftSearch/configure-connector#next-steps-customize-the-search-results-page)
- [搜索自定义类型 (externalItem)](search-concept-custom-types.md)
- 从 GitHub 下载[示例搜索连接器](https://github.com/microsoftgraph/msgraph-search-connector-sample)
