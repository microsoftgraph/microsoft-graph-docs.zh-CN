---
title: Microsoft Graph 中的 Microsoft 搜索 API 概述（预览版）
description: 使用 Microsoft 搜索 API 来编制内容索引，并将跨 Office 的搜索和编入索引的内容添加到你的应用。
localization_priority: Priority
ms.prod: search
author: snlraju-msft
scenarios: getting-started
ms.openlocfilehash: f64f8903276e83295547169aac867b1f2b3652fc
ms.sourcegitcommit: b70ee16cdf24daaec923acc477b86dbf76f2422b
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/22/2020
ms.locfileid: "48192561"
---
# <a name="overview-of-the-microsoft-search-api-in-microsoft-graph-preview"></a><span data-ttu-id="c5b4e-103">Microsoft Graph 中的 Microsoft 搜索 API 概述（预览版）</span><span class="sxs-lookup"><span data-stu-id="c5b4e-103">Overview of the Microsoft Search API in Microsoft Graph (preview)</span></span>

<span data-ttu-id="c5b4e-104">Microsoft 搜索是一种企业搜索引擎，它为组织提高了生产力并提供相关搜索结果。</span><span class="sxs-lookup"><span data-stu-id="c5b4e-104">Microsoft Search is an enterprise search engine that delivers productivity gains and relevant search results for your organization.</span></span> <span data-ttu-id="c5b4e-105">它控制组织的总体知识和生产力，并显示相关内容，使最终用户了解最新状态。</span><span class="sxs-lookup"><span data-stu-id="c5b4e-105">It harnesses the collective knowledge and productivity of an organization, and surfaces relevant content to keep end users up to date.</span></span> <span data-ttu-id="c5b4e-106">Microsoft 搜索可以在多种体验中获得，包括 Office、SharePoint、Delve、Windows 和必应。</span><span class="sxs-lookup"><span data-stu-id="c5b4e-106">Microsoft Search is available in various experiences including Office, SharePoint, Delve, Windows, and Bing.</span></span> <span data-ttu-id="c5b4e-107">可使用 Microsoft Graph 中的 Microsoft 搜索 API 将 Microsoft 搜索范围扩展到你的应用。</span><span class="sxs-lookup"><span data-stu-id="c5b4e-107">You can use the Microsoft Search API in Microsoft Graph to extend Microsoft Search to your apps.</span></span>

[!INCLUDE [search-api-preview-signup](../includes/search-api-preview-signup.md)]

<!-- markdownlint-disable MD026 -->
## <a name="why-use-the-microsoft-search-api"></a><span data-ttu-id="c5b4e-108">为什么使用 Microsoft 搜索 API？</span><span class="sxs-lookup"><span data-stu-id="c5b4e-108">Why use the Microsoft Search API?</span></span>

### <a name="one-unified-search-endpoint-for-microsoft-cloud-data"></a><span data-ttu-id="c5b4e-109">Microsoft 云数据的一个统一搜索终结点</span><span class="sxs-lookup"><span data-stu-id="c5b4e-109">One unified search endpoint for Microsoft cloud data</span></span>

<span data-ttu-id="c5b4e-110">Microsoft 搜索 API 提供一个统一的搜索终结点，让你使用该终结点[查询](/graph/api/search-query?view=graph-rest-beta&preserve-view=true) Microsoft 云中的数据（Outlook 邮箱中的邮件和事件）以及 OneDrive 和 SharePoint 中的文件（Microsoft 搜索已编制索引的数据）。</span><span class="sxs-lookup"><span data-stu-id="c5b4e-110">The Microsoft Search API provides one unified search endpoint that you can use to [query](/graph/api/search-query?view=graph-rest-beta&preserve-view=true) data in the Microsoft cloud - messages and events in Outlook mailboxes, and files on OneDrive and SharePoint - that Microsoft Search already indexes.</span></span>

### <a name="include-custom-external-data-in-search-experience"></a><span data-ttu-id="c5b4e-111">在搜索体验中包括自定义外部数据</span><span class="sxs-lookup"><span data-stu-id="c5b4e-111">Include custom external data in search experience</span></span>

<span data-ttu-id="c5b4e-112">希望在其搜索体验中包括 Microsoft 云之外的数据的客户可以使用[连接器](/microsoftsearch/connectors-overview)连接到特定数据源（如组织的人力资源数据库或产品目录），并使用 Microsoft 索引 API 无缝[查询](/graph/api/search-query?view=graph-rest-beta&preserve-view=true)外部数据源。</span><span class="sxs-lookup"><span data-stu-id="c5b4e-112">Customers who want to include data outside of the Microsoft cloud in their search experience can use [connectors](/microsoftsearch/connectors-overview) to connect to a specific data source such as an organization's human resources database or product catalog, and use the Microsoft Search API to seamlessly [query](/graph/api/search-query?view=graph-rest-beta&preserve-view=true) the external data source.</span></span> <span data-ttu-id="c5b4e-113">[Microsoft Graph 连接器库](/microsoftsearch/connectors-gallery)列出了大量随时可用的连接器。</span><span class="sxs-lookup"><span data-stu-id="c5b4e-113">The [Microsoft Graph connectors gallery](/microsoftsearch/connectors-gallery) lists a number of ready-to-use connectors.</span></span> <span data-ttu-id="c5b4e-114">或者，客户可以[生成连接器](/graph/api/resources/indexing-api-overview?view=graph-rest-beta&preserve-view=true#common-use-cases)、为外部自定义项编制索引，并能查询特定外部数据源。</span><span class="sxs-lookup"><span data-stu-id="c5b4e-114">Alternatively, customers can [build connectors](/graph/api/resources/indexing-api-overview?view=graph-rest-beta&preserve-view=true#common-use-cases), index external custom items, and query specific external data sources as well.</span></span>

### <a name="consistent-up-to-date-search-experience"></a><span data-ttu-id="c5b4e-115">一致的最新搜索体验</span><span class="sxs-lookup"><span data-stu-id="c5b4e-115">Consistent, up-to-date search experience</span></span>

<span data-ttu-id="c5b4e-116">使用 Microsoft 搜索 API 时，客户将获得 Microsoft Graph 所支持的更个性化的相关结果。</span><span class="sxs-lookup"><span data-stu-id="c5b4e-116">When you use the Microsoft Search API, your customers benefit from more personalized, relevant search results powered by Microsoft Graph.</span></span> <span data-ttu-id="c5b4e-117">你的应用中的搜索体验将返回与 Office 应用程序中的搜索一致的结果。</span><span class="sxs-lookup"><span data-stu-id="c5b4e-117">The search experience in your apps will return results that are consistent with search in Office applications.</span></span>

## <a name="what-data-can-i-add-or-access-by-using-the-microsoft-search-api"></a><span data-ttu-id="c5b4e-118">使用 Microsoft 搜索 API 可以添加或访问哪些数据？</span><span class="sxs-lookup"><span data-stu-id="c5b4e-118">What data can I add or access by using the Microsoft Search API?</span></span>

<span data-ttu-id="c5b4e-119">Microsoft 搜索 API 支持在 Microsoft 云中搜索以下内容：</span><span class="sxs-lookup"><span data-stu-id="c5b4e-119">The Microsoft Search API supports searching the following content in the Microsoft cloud:</span></span>

- <span data-ttu-id="c5b4e-120">Outlook 电子邮件[邮件](/graph/api/resources/message?view=graph-rest-beta&preserve-view=true)和日历[事件](/graph/api/resources/event?view=graph-rest-beta&preserve-view=true)对象</span><span class="sxs-lookup"><span data-stu-id="c5b4e-120">Outlook email [messages](/graph/api/resources/message?view=graph-rest-beta&preserve-view=true) and calendar [events](/graph/api/resources/event?view=graph-rest-beta&preserve-view=true) objects</span></span>
- <span data-ttu-id="c5b4e-121">SharePoint 和 OneDrive 文件和文件夹（[driveItem](/graph/api/resources/driveitem?view=graph-rest-beta&preserve-view=true)）， [列表](/graph/api/resources/list?view=graph-rest-beta&preserve-view=true)， [listItems](/graph/api/resources/listitem?view=graph-rest-beta&preserve-view=true)， [网站](/graph/api/resources/site?view=graph-rest-beta&preserve-view=true)和[驱动器](/graph/api/resources/drive?view=graph-rest-beta&preserve-view=true)</span><span class="sxs-lookup"><span data-stu-id="c5b4e-121">SharePoint and OneDrive files and folders ([driveItem](/graph/api/resources/driveitem?view=graph-rest-beta&preserve-view=true)), [lists](/graph/api/resources/list?view=graph-rest-beta&preserve-view=true), [listItems](/graph/api/resources/listitem?view=graph-rest-beta&preserve-view=true), [sites](/graph/api/resources/site?view=graph-rest-beta&preserve-view=true) and [drives](/graph/api/resources/drive?view=graph-rest-beta&preserve-view=true)</span></span>
- <span data-ttu-id="c5b4e-122">通过图形连接器平台摄取的内容： [externalItems](/graph/api/resources/externalitem?view=graph-rest-beta&preserve-view=true)</span><span class="sxs-lookup"><span data-stu-id="c5b4e-122">Content ingested throught the Graph Connectors platform : [externalItems](/graph/api/resources/externalitem?view=graph-rest-beta&preserve-view=true)</span></span>

## <a name="api-reference"></a><span data-ttu-id="c5b4e-123">API 参考</span><span class="sxs-lookup"><span data-stu-id="c5b4e-123">API reference</span></span>

<span data-ttu-id="c5b4e-124">在查找此服务的 API 参考？</span><span class="sxs-lookup"><span data-stu-id="c5b4e-124">Looking for the API reference for this service?</span></span>

- [<span data-ttu-id="c5b4e-125">使用 Microsoft 搜索 API 查询数据</span><span class="sxs-lookup"><span data-stu-id="c5b4e-125">Use the Microsoft Search API to query data</span></span>](/graph/api/resources/search-api-overview?view=graph-rest-beta&preserve-view=true)
- [<span data-ttu-id="c5b4e-126">使用 Microsoft 搜索 API 为数据编制索引</span><span class="sxs-lookup"><span data-stu-id="c5b4e-126">Use the Microsoft Search API to index data</span></span>](/graph/api/resources/indexing-api-overview?view=graph-rest-beta&preserve-view=true)

## <a name="next-steps"></a><span data-ttu-id="c5b4e-127">后续步骤</span><span class="sxs-lookup"><span data-stu-id="c5b4e-127">Next steps</span></span>

- <span data-ttu-id="c5b4e-128">了解有关 [Microsoft 搜索](/microsoftsearch/)的详细信息。</span><span class="sxs-lookup"><span data-stu-id="c5b4e-128">Learn more about [Microsoft Search](/microsoftsearch/).</span></span>
- <span data-ttu-id="c5b4e-129">了解有关几个关键用例的详细信息：</span><span class="sxs-lookup"><span data-stu-id="c5b4e-129">Learn more about a few key use cases:</span></span>
- 
  - [<span data-ttu-id="c5b4e-130">管理连接以对外部内容编制索引</span><span class="sxs-lookup"><span data-stu-id="c5b4e-130">Manage connections to index external content</span></span>](search-index-manage-connections.md)
  - [<span data-ttu-id="c5b4e-131">对外部内容编制索引</span><span class="sxs-lookup"><span data-stu-id="c5b4e-131">Index external content</span></span>](search-index-manage-items.md)
  - [<span data-ttu-id="c5b4e-132">搜索 Outlook 邮件</span><span class="sxs-lookup"><span data-stu-id="c5b4e-132">Search Outlook messages</span></span>](search-concept-messages.md)
  - [<span data-ttu-id="c5b4e-133">搜索日历事件</span><span class="sxs-lookup"><span data-stu-id="c5b4e-133">Search calendar events</span></span>](search-concept-events.md)
  - [<span data-ttu-id="c5b4e-134">SharePoint 和 OneDrive 中的搜索内容</span><span class="sxs-lookup"><span data-stu-id="c5b4e-134">Search content in Sharepoint and OneDrive</span></span>](search-concept-files.md)
  - [<span data-ttu-id="c5b4e-135">排序搜索结果</span><span class="sxs-lookup"><span data-stu-id="c5b4e-135">Sort search results</span></span>](search-concept-sort.md)
  - [<span data-ttu-id="c5b4e-136">改进搜索结果</span><span class="sxs-lookup"><span data-stu-id="c5b4e-136">Refine search results</span></span>](search-concept-aggregation.md)
  
- <span data-ttu-id="c5b4e-137">在 [Graph 浏览器](https://developer.microsoft.com/graph/graph-explorer)中探索搜索 API。</span><span class="sxs-lookup"><span data-stu-id="c5b4e-137">Explore the search APIs in  [Graph Explorer](https://developer.microsoft.com/graph/graph-explorer).</span></span>
- <span data-ttu-id="c5b4e-138">从 GitHub 下载[示例搜索连接器](https://github.com/microsoftgraph/msgraph-search-connector-sample)。</span><span class="sxs-lookup"><span data-stu-id="c5b4e-138">Download the [sample search connector](https://github.com/microsoftgraph/msgraph-search-connector-sample) from GitHub.</span></span>

## <a name="see-also"></a><span data-ttu-id="c5b4e-139">另请参阅</span><span class="sxs-lookup"><span data-stu-id="c5b4e-139">See also</span></span>

- <span data-ttu-id="c5b4e-140">在 [Stack Overflow](https://stackoverflow.com/questions/tagged/microsoft-graph-search) 或 GitHub 上与社区互动。</span><span class="sxs-lookup"><span data-stu-id="c5b4e-140">Engage with the community on [Stack Overflow](https://stackoverflow.com/questions/tagged/microsoft-graph-search) or on GitHub</span></span>
