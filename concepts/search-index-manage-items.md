---
title: 创建、更新和删除应用程序在 Microsoft 搜索服务索引中添加的项目
description: 了解如何使用 Microsoft Graph 管理应用程序添加到 Microsoft 搜索服务的项目
localization_priority: Priority
author: snlraju-msft
ms.prod: ''
doc_type: conceptualPageType
ms.openlocfilehash: 522566fb59771dc9a4efab305a271dc89a4843af
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939521"
---
# <a name="create-update-and-delete-items-added-by-your-application-in-the-microsoft-search-service-index"></a><span data-ttu-id="9ba50-103">创建、更新和删除应用程序在 Microsoft 搜索服务索引中添加的项目</span><span class="sxs-lookup"><span data-stu-id="9ba50-103">Create, update, and delete items added by your application in the Microsoft Search service index</span></span>

<span data-ttu-id="9ba50-104">应用程序添加到 Microsoft 搜索服务的项目由 Microsoft Graph 中的 [externalItem](/graph/api/resources/externalitem?view=graph-rest-beta) 和 [externalFile](/graph/api/resources/externalfile?view=graph-rest-beta) 资源表示。</span><span class="sxs-lookup"><span data-stu-id="9ba50-104">Items added by your application to the Microsoft Search service are represented by the [externalItem](/graph/api/resources/externalitem?view=graph-rest-beta) and [externalFile](/graph/api/resources/externalfile?view=graph-rest-beta) resources in Microsoft Graph.</span></span>

<span data-ttu-id="9ba50-105">“externalItem”\*\*\*\* 资源表示自定义类型。</span><span class="sxs-lookup"><span data-stu-id="9ba50-105">The **externalItem** resource represents a custom type.</span></span> <span data-ttu-id="9ba50-106">当添加到索引的项使用“externalFile”\*\*\*\* 资源未表示的自定义架构时，应使用此方法。</span><span class="sxs-lookup"><span data-stu-id="9ba50-106">It should be used when the items you add to the index use a custom schema not represented by the **externalFile** resource.</span></span> <span data-ttu-id="9ba50-107">例如，支持人员票证或产品清单。</span><span class="sxs-lookup"><span data-stu-id="9ba50-107">For example, helpdesk tickets or product listings.</span></span>

<span data-ttu-id="9ba50-108">“externalFile”\*\*\*\* 资源表示外部系统中的文件。</span><span class="sxs-lookup"><span data-stu-id="9ba50-108">The **externalFile** resource represents a file in an external system.</span></span>

> [!NOTE]
> <span data-ttu-id="9ba50-109">无法扩展“externalFile”\*\*\*\* 的架构。</span><span class="sxs-lookup"><span data-stu-id="9ba50-109">The schema for **externalFile** cannot be extended.</span></span>

## <a name="add-an-item-or-file"></a><span data-ttu-id="9ba50-110">创建项目或文件</span><span class="sxs-lookup"><span data-stu-id="9ba50-110">Add an item or file</span></span>

<span data-ttu-id="9ba50-111">可通过[创建 externalItem](/graph/api/externalconnection-put-items?view=graph-rest-beta)，将项目或文件添加到索引。</span><span class="sxs-lookup"><span data-stu-id="9ba50-111">You can add an item or file to the index by [creating an externalItem](/graph/api/externalconnection-put-items?view=graph-rest-beta).</span></span> <span data-ttu-id="9ba50-112">创建项目时，可在 URL 中分配唯一的标识符。</span><span class="sxs-lookup"><span data-stu-id="9ba50-112">When you create an item, you assign a unique identifier in the URL.</span></span>

<span data-ttu-id="9ba50-113">例如，你的应用程序可能会使用票证编号来索引支持人员票证。</span><span class="sxs-lookup"><span data-stu-id="9ba50-113">For example, your application may index helpdesk tickets using the ticket number.</span></span> <span data-ttu-id="9ba50-114">如果票证具有 `SR00145` 票证编号，请求可能如下所示。</span><span class="sxs-lookup"><span data-stu-id="9ba50-114">If a ticket has the ticket number `SR00145`, the request may look like the following.</span></span>

```http
PUT /external/connections/contosohelpdesk/items/SR00145
Content-Type: application/json

{
  "title": "WiFi outage in Conference Room A",
  "status": "New",
  "assignee": "meganb@contoso.com"
}
```

## <a name="update-an-item-or-file"></a><span data-ttu-id="9ba50-115">更新项目或文件</span><span class="sxs-lookup"><span data-stu-id="9ba50-115">Update an item or file</span></span>

<span data-ttu-id="9ba50-116">在外部服务中更新项目或文件（重新分配支持人员票证或更新产品说明）时，可以使用创建项目时分配给项目的唯一标识符，通过[更新 externalItem](/graph/api/externalitem-update?view=graph-rest-beta) 更新其在索引中的条目。</span><span class="sxs-lookup"><span data-stu-id="9ba50-116">When an item or file is updated in the external service (helpdesk ticket is reassigned, or a product description is updated), you can update its entry in the index by [updating the externalItem](/graph/api/externalitem-update?view=graph-rest-beta), using the unique identifier assigned to the item when you created it.</span></span>

```http
PATCH /external/connections/contosohelpdesk/items/SR00145
Content-Type: application/json

{
  "assignee": "alexw@contoso.com"
}
```

## <a name="delete-an-item-or-file"></a><span data-ttu-id="9ba50-117">删除项目或文件</span><span class="sxs-lookup"><span data-stu-id="9ba50-117">Delete a previous version of an item or file in SharePoint</span></span>

<span data-ttu-id="9ba50-118">可以使用创建项目时分配给项目的唯一标识符，通过[删除 externalItem](/graph/api/externalitem-delete?view=graph-rest-beta) 删除索引中的项目或文件。</span><span class="sxs-lookup"><span data-stu-id="9ba50-118">You can remove items or files from the index by [deleting the externalItem](/graph/api/externalitem-delete?view=graph-rest-beta), using the unique identifier assigned to the item when you created it.</span></span>

```http
DELETE /external/connections/contosohelpdesk/items/SR00145
```

## <a name="next-steps"></a><span data-ttu-id="9ba50-119">后续步骤</span><span class="sxs-lookup"><span data-stu-id="9ba50-119">Next steps</span></span>

- [<span data-ttu-id="9ba50-120">为什么使用 Microsoft 搜索 API？</span><span class="sxs-lookup"><span data-stu-id="9ba50-120">Why use the Microsoft Graph Security API?</span></span>](search-concept-overview.md#why-use-the-microsoft-search-api)
- [<span data-ttu-id="9ba50-121">使用 Microsoft 搜索 API 为数据编制索引</span><span class="sxs-lookup"><span data-stu-id="9ba50-121">Use the Microsoft Search API to index data</span></span>](/graph/api/resources/indexing-api-overview?view=graph-rest-beta)
- [<span data-ttu-id="9ba50-122">搜索自定义类型 (externalItem)</span><span class="sxs-lookup"><span data-stu-id="9ba50-122">Search custom types (externalItem)</span></span>](search-concept-custom-types.md)
- [<span data-ttu-id="9ba50-123">搜索文件（包括 externalFile）</span><span class="sxs-lookup"><span data-stu-id="9ba50-123">Search files (including externalFile)</span></span>](search-concept-files.md)
- <span data-ttu-id="9ba50-124">从 GitHub 下载[示例搜索连接器](https://github.com/microsoftgraph/msgraph-search-connector-sample)</span><span class="sxs-lookup"><span data-stu-id="9ba50-124">Download the [sample search connector](https://github.com/microsoftgraph/msgraph-search-connector-sample) from GitHub</span></span>
