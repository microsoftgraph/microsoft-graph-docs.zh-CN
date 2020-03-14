---
title: Microsoft Graph 中的 Microsoft 搜索 API 概述（预览版）
description: 使用 Microsoft 搜索 API 来编制内容索引，并将跨 Office 的搜索和编入索引的内容添加到你的应用。
localization_priority: Priority
ms.prod: search
author: snlraju-msft
scenarios: getting-started
ms.openlocfilehash: 48d54de1e9c758a21af1e179e83876b19c146840
ms.sourcegitcommit: 8a84ee922acd2946a3ffae9f8f7f7b485567bc05
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2020
ms.locfileid: "42618770"
---
# <a name="overview-of-the-microsoft-search-api-in-microsoft-graph-preview"></a><span data-ttu-id="0034d-103">Microsoft Graph 中的 Microsoft 搜索 API 概述（预览版）</span><span class="sxs-lookup"><span data-stu-id="0034d-103">Overview of the Microsoft Search API in Microsoft Graph (preview)</span></span>

<span data-ttu-id="0034d-104">Microsoft 搜索是一种企业搜索引擎，它为组织提高了生产力并提供相关搜索结果。</span><span class="sxs-lookup"><span data-stu-id="0034d-104">Microsoft Search is an enterprise search engine that delivers productivity gains and relevant search results for your organization.</span></span> <span data-ttu-id="0034d-105">它控制组织的总体知识和生产力，并显示相关内容，使最终用户了解最新状态。</span><span class="sxs-lookup"><span data-stu-id="0034d-105">It harnesses the collective knowledge and productivity of an organization, and surfaces relevant content to keep end users up to date.</span></span> <span data-ttu-id="0034d-106">Microsoft 搜索可以在多种体验中获得，包括 Office、SharePoint、Delve、Windows 和必应。</span><span class="sxs-lookup"><span data-stu-id="0034d-106">Microsoft Search is available in various experiences including Office, SharePoint, Delve, Windows, and Bing.</span></span> <span data-ttu-id="0034d-107">可使用 Microsoft Graph 中的 Microsoft 搜索 API 将 Microsoft 搜索范围扩展到你的应用。</span><span class="sxs-lookup"><span data-stu-id="0034d-107">You can use the Microsoft Search API in Microsoft Graph to extend Microsoft Search to your apps.</span></span>

[!INCLUDE [search-api-preview-signup](../includes/search-api-preview-signup.md)]

<!-- markdownlint-disable MD026 -->
## <a name="why-use-the-microsoft-search-api"></a><span data-ttu-id="0034d-108">为什么使用 Microsoft 搜索 API？</span><span class="sxs-lookup"><span data-stu-id="0034d-108">Why use the Microsoft Search API?</span></span>

### <a name="one-unified-search-endpoint-for-microsoft-cloud-data"></a><span data-ttu-id="0034d-109">Microsoft 云数据的一个统一搜索终结点</span><span class="sxs-lookup"><span data-stu-id="0034d-109">One unified search endpoint for Microsoft cloud data</span></span>

<span data-ttu-id="0034d-110">Microsoft 搜索 API 提供一个统一的搜索终结点，让你使用该终结点[查询](/graph/api/search-query?view=graph-rest-beta) Microsoft 云中的数据（Outlook 邮箱中的邮件和事件）以及 OneDrive 和 SharePoint 中的文件（Microsoft 搜索已编制索引的数据）。</span><span class="sxs-lookup"><span data-stu-id="0034d-110">The Microsoft Search API provides one unified search endpoint that you can use to [query](/graph/api/search-query?view=graph-rest-beta) data in the Microsoft cloud - messages and events in Outlook mailboxes, and files on OneDrive and SharePoint - that Microsoft Search already indexes.</span></span>

### <a name="include-custom-external-data-in-search-experience"></a><span data-ttu-id="0034d-111">在搜索体验中包括自定义外部数据</span><span class="sxs-lookup"><span data-stu-id="0034d-111">Include custom external data in search experience</span></span>

<span data-ttu-id="0034d-112">希望在其搜索体验中包括 Microsoft 云之外的数据的客户可以使用[连接器](/microsoftsearch/connectors-overview)连接到特定数据源（如组织的人力资源数据库或产品目录），并使用 Microsoft 索引 API 无缝[查询](/graph/api/search-query?view=graph-rest-beta)外部数据源。</span><span class="sxs-lookup"><span data-stu-id="0034d-112">Customers who want to include data outside of the Microsoft cloud in their search experience can use [connectors](/microsoftsearch/connectors-overview) to connect to a specific data source such as an organization's human resources database or product catalog, and use the Microsoft Search API to seamlessly [query](/graph/api/search-query?view=graph-rest-beta) the external data source.</span></span> <span data-ttu-id="0034d-113">[Microsoft Graph 连接器库](/microsoftsearch/connectors-gallery)列出了大量随时可用的连接器。</span><span class="sxs-lookup"><span data-stu-id="0034d-113">The [Microsoft Graph connectors gallery](/microsoftsearch/connectors-gallery) lists a number of ready-to-use connectors.</span></span> <span data-ttu-id="0034d-114">或者，客户可以[构建连接器](/graph/api/resources/indexing-api-overview?view=graph-rest-beta#common-use-cases)、索引外部自定义项目和文件以及查询特定外部数据源。</span><span class="sxs-lookup"><span data-stu-id="0034d-114">Alternatively, customers can [build connectors](/graph/api/resources/indexing-api-overview?view=graph-rest-beta#common-use-cases), index external custom items and files, and query specific external data sources as well.</span></span>

### <a name="consistent-up-to-date-search-experience"></a><span data-ttu-id="0034d-115">一致的最新搜索体验</span><span class="sxs-lookup"><span data-stu-id="0034d-115">Consistent, up-to-date search experience</span></span>

<span data-ttu-id="0034d-116">使用 Microsoft 搜索 API 时，客户将获得 Microsoft Graph 所支持的更个性化的相关结果。</span><span class="sxs-lookup"><span data-stu-id="0034d-116">When you use the Microsoft Search API, your customers benefit from more personalized, relevant search results powered by Microsoft Graph.</span></span> <span data-ttu-id="0034d-117">你的应用中的搜索体验将返回与 Office 应用程序中的搜索一致的结果。</span><span class="sxs-lookup"><span data-stu-id="0034d-117">The search experience in your apps will return results that are consistent with search in Office applications.</span></span>

## <a name="what-data-can-i-add-or-access-by-using-the-microsoft-search-api"></a><span data-ttu-id="0034d-118">使用 Microsoft 搜索 API 可以添加或访问哪些数据？</span><span class="sxs-lookup"><span data-stu-id="0034d-118">What data can I add or access by using the Microsoft Search API?</span></span>

<span data-ttu-id="0034d-119">Microsoft 搜索 API 支持在 Microsoft 云中搜索以下内容：</span><span class="sxs-lookup"><span data-stu-id="0034d-119">The Microsoft Search API supports searching the following content in the Microsoft cloud:</span></span>

- <span data-ttu-id="0034d-120">Outlook [message](/graph/api/resources/message?view=graph-rest-beta) 和 [event](/graph/api/resources/event?view=graph-rest-beta) 对象</span><span class="sxs-lookup"><span data-stu-id="0034d-120">Outlook [message](/graph/api/resources/message?view=graph-rest-beta) and [event](/graph/api/resources/event?view=graph-rest-beta) objects</span></span>
- <span data-ttu-id="0034d-121">SharePoint 和 OneDrive [driveItem](/graph/api/resources/driveitem?view=graph-rest-beta) 文件对象</span><span class="sxs-lookup"><span data-stu-id="0034d-121">SharePoint and OneDrive [driveItem](/graph/api/resources/driveitem?view=graph-rest-beta) file objects</span></span>

<span data-ttu-id="0034d-122">此外，还可通过以下对象对外部内容编制索引和搜索：</span><span class="sxs-lookup"><span data-stu-id="0034d-122">In addition, you can index and search external content via the following:</span></span>

- <span data-ttu-id="0034d-123">自定义类型的 [externalItem](/graph/api/resources/externalitem?view=graph-rest-beta) 对象</span><span class="sxs-lookup"><span data-stu-id="0034d-123">[externalItem](/graph/api/resources/externalitem?view=graph-rest-beta) objects, which are of custom types</span></span>
- <span data-ttu-id="0034d-124">熟知类型的 [externalFile](/graph/api/resources/externalfile?view=graph-rest-beta) 对象</span><span class="sxs-lookup"><span data-stu-id="0034d-124">[externalFile](/graph/api/resources/externalfile?view=graph-rest-beta) objects, which are of well-known types</span></span>

## <a name="api-reference"></a><span data-ttu-id="0034d-125">API 参考</span><span class="sxs-lookup"><span data-stu-id="0034d-125">API reference</span></span>

<span data-ttu-id="0034d-126">在查找此服务的 API 参考？</span><span class="sxs-lookup"><span data-stu-id="0034d-126">Looking for the API reference for this service?</span></span>

- [<span data-ttu-id="0034d-127">使用 Microsoft 搜索 API 查询数据</span><span class="sxs-lookup"><span data-stu-id="0034d-127">Use the Microsoft Search API to query data</span></span>](/graph/api/resources/search-api-overview?view=graph-rest-beta)
- [<span data-ttu-id="0034d-128">使用 Microsoft 搜索 API 为数据编制索引</span><span class="sxs-lookup"><span data-stu-id="0034d-128">Use the Microsoft Search API to index data</span></span>](/graph/api/resources/indexing-api-overview?view=graph-rest-beta)

## <a name="next-steps"></a><span data-ttu-id="0034d-129">后续步骤</span><span class="sxs-lookup"><span data-stu-id="0034d-129">Next steps</span></span>

- <span data-ttu-id="0034d-130">了解有关 [Microsoft 搜索](/microsoftsearch/)的详细信息。</span><span class="sxs-lookup"><span data-stu-id="0034d-130">Learn more about [Microsoft Search](/microsoftsearch/).</span></span>
- <span data-ttu-id="0034d-131">了解有关几个关键用例的详细信息：</span><span class="sxs-lookup"><span data-stu-id="0034d-131">Learn more about a few key use cases:</span></span>
  - [<span data-ttu-id="0034d-132">搜索 Outlook 邮件</span><span class="sxs-lookup"><span data-stu-id="0034d-132">Search Outlook messages</span></span>](search-concept-messages.md)
  - [<span data-ttu-id="0034d-133">搜索日历事件</span><span class="sxs-lookup"><span data-stu-id="0034d-133">Search calendar events</span></span>](search-concept-events.md)
  - [<span data-ttu-id="0034d-134">管理连接以对外部内容编制索引</span><span class="sxs-lookup"><span data-stu-id="0034d-134">Manage connections to index external content</span></span>](search-index-manage-connections.md)
  - [<span data-ttu-id="0034d-135">对外部内容编制索引</span><span class="sxs-lookup"><span data-stu-id="0034d-135">Index external content</span></span>](search-index-manage-items.md)
  - [<span data-ttu-id="0034d-136">搜索自定义类型 (externalItem)</span><span class="sxs-lookup"><span data-stu-id="0034d-136">Search custom types (externalItem)</span></span>](search-concept-custom-types.md)
  - [<span data-ttu-id="0034d-137">搜索文件（包括 externalFile）</span><span class="sxs-lookup"><span data-stu-id="0034d-137">Search files (including externalFile)</span></span>](search-concept-files.md)
- <span data-ttu-id="0034d-138">在 [Graph 浏览器](https://developer.microsoft.com/graph/graph-explorer)中探索搜索 API。</span><span class="sxs-lookup"><span data-stu-id="0034d-138">Explore the search APIs in the [Graph Explorer](https://developer.microsoft.com/graph/graph-explorer).</span></span>
- <span data-ttu-id="0034d-139">从 GitHub 下载[示例搜索连接器](https://github.com/microsoftgraph/msgraph-search-connector-sample)。</span><span class="sxs-lookup"><span data-stu-id="0034d-139">Download the [sample search connector](https://github.com/microsoftgraph/msgraph-search-connector-sample) from GitHub.</span></span>

## <a name="see-also"></a><span data-ttu-id="0034d-140">另请参阅</span><span class="sxs-lookup"><span data-stu-id="0034d-140">See also</span></span>

- <span data-ttu-id="0034d-141">在 [Stack Overflow](https://stackoverflow.com/questions/tagged/microsoft-graph-search) 上与社区互动。</span><span class="sxs-lookup"><span data-stu-id="0034d-141">Engage with the community on [Stack Overflow](https://stackoverflow.com/questions/tagged/microsoft-graph-search).</span></span>
