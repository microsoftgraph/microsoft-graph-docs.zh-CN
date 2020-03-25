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
# <a name="create-update-and-delete-items-added-by-your-application-in-the-microsoft-search-service-index"></a><span data-ttu-id="90a68-103">创建、更新和删除应用程序在 Microsoft 搜索服务索引中添加的项目</span><span class="sxs-lookup"><span data-stu-id="90a68-103">Create, update, and delete items added by your application in the Microsoft Search service index</span></span>

<span data-ttu-id="90a68-104">应用程序添加到 Microsoft 搜索服务的项用 Microsoft Graph 中的 [externalItem](/graph/api/resources/externalitem?view=graph-rest-beta) 资源表示。</span><span class="sxs-lookup"><span data-stu-id="90a68-104">Items added by your application to the Microsoft Search service are represented by the [externalItem](/graph/api/resources/externalitem?view=graph-rest-beta) resource in Microsoft Graph.</span></span>

[!INCLUDE [search-api-preview-signup](../includes/search-api-preview-signup.md)]

## <a name="add-an-item"></a><span data-ttu-id="90a68-105">添加项</span><span class="sxs-lookup"><span data-stu-id="90a68-105">Add an item</span></span>

<span data-ttu-id="90a68-106">可通过[创建 externalItem](/graph/api/externalconnection-put-items?view=graph-rest-beta)，将项添加到索引。</span><span class="sxs-lookup"><span data-stu-id="90a68-106">You can add an item to the index by [creating an externalItem](/graph/api/externalconnection-put-items?view=graph-rest-beta).</span></span> <span data-ttu-id="90a68-107">创建项目时，可在 URL 中分配唯一的标识符。</span><span class="sxs-lookup"><span data-stu-id="90a68-107">When you create an item, you assign a unique identifier in the URL.</span></span>

<span data-ttu-id="90a68-108">例如，你的应用程序可能会使用票证编号来索引支持人员票证。</span><span class="sxs-lookup"><span data-stu-id="90a68-108">For example, your application may index helpdesk tickets using the ticket number.</span></span> <span data-ttu-id="90a68-109">如果票证具有 `SR00145` 票证编号，请求可能如下所示。</span><span class="sxs-lookup"><span data-stu-id="90a68-109">If a ticket has the ticket number `SR00145`, the request may look like the following.</span></span>

```http
PUT /external/connections/contosohelpdesk/items/SR00145
Content-Type: application/json

{
  "title": "WiFi outage in Conference Room A",
  "status": "New",
  "assignee": "meganb@contoso.com"
}
```

> <span data-ttu-id="90a68-110">![注意] 管理员必须先[自定义相应连接的搜索结果页](/MicrosoftSearch/configure-connector#next-steps-customize-the-search-results-page)，然后索引项才能在 Microsoft 搜索 UI 中找到。</span><span class="sxs-lookup"><span data-stu-id="90a68-110">![NOTE] Before indexed items can be found in the Microsoft Search UI, an administrator must [customize the search results page](/MicrosoftSearch/configure-connector#next-steps-customize-the-search-results-page) for the corresponding connection.</span></span>

## <a name="update-an-item"></a><span data-ttu-id="90a68-111">更新项</span><span class="sxs-lookup"><span data-stu-id="90a68-111">Update an item</span></span>

<span data-ttu-id="90a68-112">当项在外部服务中更新（重新分配支持人员票证或更新产品说明）时，可以使用创建项时分配给项的唯一标识符，通过[更新 externalItem](/graph/api/externalitem-update?view=graph-rest-beta) 更新项在索引中的条目。</span><span class="sxs-lookup"><span data-stu-id="90a68-112">When an item is updated in the external service (helpdesk ticket is reassigned, or a product description is updated), you can update its entry in the index by [updating the externalItem](/graph/api/externalitem-update?view=graph-rest-beta), using the unique identifier assigned to the item when you created it.</span></span>

```http
PATCH /external/connections/contosohelpdesk/items/SR00145
Content-Type: application/json

{
  "assignee": "alexw@contoso.com"
}
```

## <a name="delete-an-item"></a><span data-ttu-id="90a68-113">删除项</span><span class="sxs-lookup"><span data-stu-id="90a68-113">Delete an item</span></span>

<span data-ttu-id="90a68-114">可以使用创建项时分配给项的唯一标识符，通过[删除 externalItem](/graph/api/externalitem-delete?view=graph-rest-beta) 从索引中删除项。</span><span class="sxs-lookup"><span data-stu-id="90a68-114">You can remove items from the index by [deleting the externalItem](/graph/api/externalitem-delete?view=graph-rest-beta), using the unique identifier assigned to the item when you created it.</span></span>

```http
DELETE /external/connections/contosohelpdesk/items/SR00145
```

## <a name="next-steps"></a><span data-ttu-id="90a68-115">后续步骤</span><span class="sxs-lookup"><span data-stu-id="90a68-115">Next steps</span></span>

- [<span data-ttu-id="90a68-116">为什么使用 Microsoft 搜索 API？</span><span class="sxs-lookup"><span data-stu-id="90a68-116">Why use the Microsoft Search API?</span></span>](search-concept-overview.md#why-use-the-microsoft-search-api)
- [<span data-ttu-id="90a68-117">查看索引 API 参考</span><span class="sxs-lookup"><span data-stu-id="90a68-117">Review the Indexing API reference</span></span>](/graph/api/resources/indexing-api-overview?view=graph-rest-beta)
- [<span data-ttu-id="90a68-118">自定义 Microsoft 搜索结果页</span><span class="sxs-lookup"><span data-stu-id="90a68-118">Customize Microsoft Search results page</span></span>](/MicrosoftSearch/configure-connector#next-steps-customize-the-search-results-page)
- [<span data-ttu-id="90a68-119">搜索自定义类型 (externalItem)</span><span class="sxs-lookup"><span data-stu-id="90a68-119">Search custom types (externalItem)</span></span>](search-concept-custom-types.md)
- <span data-ttu-id="90a68-120">从 GitHub 下载[示例搜索连接器](https://github.com/microsoftgraph/msgraph-search-connector-sample)</span><span class="sxs-lookup"><span data-stu-id="90a68-120">Download the [sample search connector](https://github.com/microsoftgraph/msgraph-search-connector-sample) from GitHub</span></span>
