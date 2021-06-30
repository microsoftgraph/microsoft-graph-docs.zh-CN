---
title: Microsoft Graph 中的 Microsoft 搜索 API 概述
description: 使用 Microsoft 搜索 API 来编制内容索引，并将跨 Office 的搜索和编入索引的内容添加到你的应用。
localization_priority: Priority
ms.prod: search
author: snlraju-msft
scenarios: getting-started
ms.openlocfilehash: 732d6487bc73cf9cdf0f70168d00d4b0e13ce45e
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/30/2021
ms.locfileid: "53208832"
---
# <a name="overview-of-the-microsoft-search-api-in-microsoft-graph"></a><span data-ttu-id="7d416-103">Microsoft Graph 中的 Microsoft 搜索 API 概述</span><span class="sxs-lookup"><span data-stu-id="7d416-103">Overview of the Microsoft Search API in Microsoft Graph</span></span>

<span data-ttu-id="7d416-104">Microsoft 搜索是一种企业搜索引擎，它为组织提高了生产力并提供相关搜索结果。</span><span class="sxs-lookup"><span data-stu-id="7d416-104">Microsoft Search is an enterprise search engine that delivers productivity gains and relevant search results for your organization.</span></span> <span data-ttu-id="7d416-105">它控制组织的总体知识和生产力，并显示相关内容，使最终用户了解最新状态。</span><span class="sxs-lookup"><span data-stu-id="7d416-105">It harnesses the collective knowledge and productivity of an organization, and surfaces relevant content to keep end users up to date.</span></span> <span data-ttu-id="7d416-106">Microsoft 搜索可以在多种体验中获得，包括 Office、SharePoint、Delve、Windows 和必应。</span><span class="sxs-lookup"><span data-stu-id="7d416-106">Microsoft Search is available in various experiences including Office, SharePoint, Delve, Windows, and Bing.</span></span> <span data-ttu-id="7d416-107">可使用 Microsoft Graph 中的 Microsoft 搜索 API 将 Microsoft 搜索范围扩展到你的应用。</span><span class="sxs-lookup"><span data-stu-id="7d416-107">You can use the Microsoft Search API in Microsoft Graph to extend Microsoft Search to your apps.</span></span>


<!-- markdownlint-disable MD026 -->
## <a name="why-use-the-microsoft-search-api"></a><span data-ttu-id="7d416-108">为什么使用 Microsoft 搜索 API？</span><span class="sxs-lookup"><span data-stu-id="7d416-108">Why use the Microsoft Search API?</span></span>

### <a name="one-unified-search-endpoint-for-microsoft-cloud-data"></a><span data-ttu-id="7d416-109">Microsoft 云数据的一个统一搜索终结点</span><span class="sxs-lookup"><span data-stu-id="7d416-109">One unified search endpoint for Microsoft cloud data</span></span>

<span data-ttu-id="7d416-110">Microsoft 搜索 API 提供一个统一的搜索终结点，让你使用该终结点[查询](/graph/api/search-query) Microsoft 云中的数据（Outlook 邮箱中的邮件和事件）以及 OneDrive 和 SharePoint 中的文件（Microsoft 搜索已编制索引的数据）。</span><span class="sxs-lookup"><span data-stu-id="7d416-110">The Microsoft Search API provides one unified search endpoint that you can use to [query](/graph/api/search-query) data in the Microsoft cloud - messages and events in Outlook mailboxes, and files on OneDrive and SharePoint - that Microsoft Search already indexes.</span></span>

### <a name="include-custom-external-data-in-search-experience-preview"></a><span data-ttu-id="7d416-111">在搜索体验中加入自定义外部数据（预览版）</span><span class="sxs-lookup"><span data-stu-id="7d416-111">Include custom external data in search experience (preview)</span></span>

<span data-ttu-id="7d416-112">使用 [Microsoft Graph 连接器](/microsoftsearch/connectors-overview)将 Microsoft 云之外的数据包含在你的搜索体验中。</span><span class="sxs-lookup"><span data-stu-id="7d416-112">Use [Microsoft Graph connectors](/microsoftsearch/connectors-overview) to include data outside of the Microsoft cloud in your search experience.</span></span> <span data-ttu-id="7d416-113">例如，连接到组织的人力资源数据库或产品目录。</span><span class="sxs-lookup"><span data-stu-id="7d416-113">For instance, connect to an organization's human resources database or product catalog.</span></span> <span data-ttu-id="7d416-114">然后使用 Microsoft 搜索 API 无缝[查询](/graph/api/search-query)外部数据源。</span><span class="sxs-lookup"><span data-stu-id="7d416-114">Then use the Microsoft Search API to seamlessly [query](/graph/api/search-query) the external data source.</span></span> 

<span data-ttu-id="7d416-115">浏览 [Microsoft Graph 连接器库](/microsoftsearch/connectors-gallery)以查找随时可用的连接器。</span><span class="sxs-lookup"><span data-stu-id="7d416-115">Browse the [Microsoft Graph connectors gallery](/microsoftsearch/connectors-gallery) to find ready-to-use connectors.</span></span> <span data-ttu-id="7d416-116">或者，你可以[生成自己的连接器](/graph/api/resources/indexing-api-overview?view=graph-rest-beta&preserve-view=true#common-use-cases)，为外部自定义项目创建索引并查询特定外部数据源。</span><span class="sxs-lookup"><span data-stu-id="7d416-116">Alternatively, you can [build your own connectors](/graph/api/resources/indexing-api-overview?view=graph-rest-beta&preserve-view=true#common-use-cases) to index external custom items and query specific external data sources.</span></span>

### <a name="consistent-up-to-date-search-experience"></a><span data-ttu-id="7d416-117">一致的最新搜索体验</span><span class="sxs-lookup"><span data-stu-id="7d416-117">Consistent, up-to-date search experience</span></span>

<span data-ttu-id="7d416-118">使用 Microsoft 搜索 API 时，客户将获得 Microsoft Graph 所支持的更个性化的相关结果。</span><span class="sxs-lookup"><span data-stu-id="7d416-118">When you use the Microsoft Search API, your customers benefit from more personalized, relevant search results powered by Microsoft Graph.</span></span> <span data-ttu-id="7d416-119">你的应用中的搜索体验将返回与 Office 应用程序中的搜索一致的结果。</span><span class="sxs-lookup"><span data-stu-id="7d416-119">The search experience in your apps will return results that are consistent with search in Office applications.</span></span>

## <a name="what-data-can-i-add-or-access-by-using-the-microsoft-search-api"></a><span data-ttu-id="7d416-120">使用 Microsoft 搜索 API 可以添加或访问哪些数据？</span><span class="sxs-lookup"><span data-stu-id="7d416-120">What data can I add or access by using the Microsoft Search API?</span></span>

<span data-ttu-id="7d416-121">Microsoft 搜索 API 支持在 Microsoft 云中搜索以下内容：</span><span class="sxs-lookup"><span data-stu-id="7d416-121">The Microsoft Search API supports searching the following content in the Microsoft cloud:</span></span>

- <span data-ttu-id="7d416-122">Outlook 电子邮件[邮件](/graph/api/resources/message)和日历[事件](/graph/api/resources/event)对象</span><span class="sxs-lookup"><span data-stu-id="7d416-122">Outlook email [messages](/graph/api/resources/message) and calendar [events](/graph/api/resources/event) objects</span></span>
- <span data-ttu-id="7d416-123">SharePoint 和 OneDrive 文件和文件夹（[driveItem](/graph/api/resources/driveitem)）， [列表](/graph/api/resources/list)， [listItems](/graph/api/resources/listitem)， [网站](/graph/api/resources/site)和[驱动器](/graph/api/resources/drive)</span><span class="sxs-lookup"><span data-stu-id="7d416-123">SharePoint and OneDrive files and folders ([driveItem](/graph/api/resources/driveitem)), [lists](/graph/api/resources/list), [listItems](/graph/api/resources/listitem), [sites](/graph/api/resources/site) and [drives](/graph/api/resources/drive)</span></span>
- <span data-ttu-id="7d416-124">通过图形连接器平台摄取的内容： [externalItems](/graph/api/resources/externalitem?view=graph-rest-beta&preserve-view=true)（预览版）</span><span class="sxs-lookup"><span data-stu-id="7d416-124">Content ingested throught the Graph Connectors platform : [externalItems](/graph/api/resources/externalitem?view=graph-rest-beta&preserve-view=true) (preview)</span></span>

## <a name="api-reference"></a><span data-ttu-id="7d416-125">API 参考</span><span class="sxs-lookup"><span data-stu-id="7d416-125">API reference</span></span>

<span data-ttu-id="7d416-126">在查找此服务的 API 参考？</span><span class="sxs-lookup"><span data-stu-id="7d416-126">Looking for the API reference for this service?</span></span>

- <span data-ttu-id="7d416-127">[使用 Microsoft 搜索 API 查询数据](/graph/api/resources/search-api-overview?view=graph-rest-1.0)（v1.0版本）</span><span class="sxs-lookup"><span data-stu-id="7d416-127">[Use the Microsoft Search API to query data](/graph/api/resources/search-api-overview?view=graph-rest-1.0) (v1.0)</span></span>
- <span data-ttu-id="7d416-128">[使用 Microsoft 搜索 API 查询数据](/graph/api/resources/search-api-overview?view=graph-rest-beta)（预览版）</span><span class="sxs-lookup"><span data-stu-id="7d416-128">[Use the Microsoft Search API to query data](/graph/api/resources/search-api-overview?view=graph-rest-beta) (preview)</span></span>
- <span data-ttu-id="7d416-129">[使用 Microsoft 搜索 API 索引数据](/graph/api/resources/indexing-api-overview)（预览版）</span><span class="sxs-lookup"><span data-stu-id="7d416-129">[Use the Microsoft Search API to index data](/graph/api/resources/indexing-api-overview) (preview)</span></span>

## <a name="next-steps"></a><span data-ttu-id="7d416-130">后续步骤</span><span class="sxs-lookup"><span data-stu-id="7d416-130">Next steps</span></span>

- <span data-ttu-id="7d416-131">了解有关 [Microsoft 搜索](/microsoftsearch/)的详细信息。</span><span class="sxs-lookup"><span data-stu-id="7d416-131">Learn more about [Microsoft Search](/microsoftsearch/).</span></span>
- <span data-ttu-id="7d416-132">了解有关几个关键用例的详细信息：</span><span class="sxs-lookup"><span data-stu-id="7d416-132">Learn more about a few key use cases:</span></span>
  - [<span data-ttu-id="7d416-133">管理连接以对外部内容编制索引</span><span class="sxs-lookup"><span data-stu-id="7d416-133">Manage connections to index external content</span></span>](connecting-external-content-manage-connections.md)
  - [<span data-ttu-id="7d416-134">对外部内容编制索引</span><span class="sxs-lookup"><span data-stu-id="7d416-134">Index external content</span></span>](connecting-external-content-manage-items.md)
  - [<span data-ttu-id="7d416-135">搜索 Outlook 邮件</span><span class="sxs-lookup"><span data-stu-id="7d416-135">Search Outlook messages</span></span>](search-concept-messages.md)
  - [<span data-ttu-id="7d416-136">搜索日历事件</span><span class="sxs-lookup"><span data-stu-id="7d416-136">Search calendar events</span></span>](search-concept-events.md)
  - [<span data-ttu-id="7d416-137">SharePoint 和 OneDrive 中的搜索内容</span><span class="sxs-lookup"><span data-stu-id="7d416-137">Search content in Sharepoint and OneDrive</span></span>](search-concept-files.md)
  - <span data-ttu-id="7d416-138">[搜索外部内容](search-concept-custom-types.md)（预览版）</span><span class="sxs-lookup"><span data-stu-id="7d416-138">[Search external content](search-concept-custom-types.md) (preview)</span></span>
  - <span data-ttu-id="7d416-139">[排序搜索结果](search-concept-sort.md)（预览版）</span><span class="sxs-lookup"><span data-stu-id="7d416-139">[Sort search results](search-concept-sort.md) (preview)</span></span>
  - <span data-ttu-id="7d416-140">[改进搜索结果](search-concept-aggregation.md)（预览版）</span><span class="sxs-lookup"><span data-stu-id="7d416-140">[Refine search results](search-concept-aggregation.md) (preview)</span></span>
  - <span data-ttu-id="7d416-141">[请求拼写更正](search-concept-speller.md) （预览版）</span><span class="sxs-lookup"><span data-stu-id="7d416-141">[Request spelling correction](search-concept-speller.md) (preview)</span></span>
  - <span data-ttu-id="7d416-142">[搜索显示布局](search-concept-display-layout.md) （预览版）</span><span class="sxs-lookup"><span data-stu-id="7d416-142">[Search display layout](search-concept-display-layout.md) (preview)</span></span>
  
- <span data-ttu-id="7d416-143">在 [Graph 浏览器](https://developer.microsoft.com/graph/graph-explorer)中探索搜索 API。</span><span class="sxs-lookup"><span data-stu-id="7d416-143">Explore the search APIs in  [Graph Explorer](https://developer.microsoft.com/graph/graph-explorer).</span></span>
- <span data-ttu-id="7d416-144">从 GitHub 下载[示例搜索连接器](https://github.com/microsoftgraph/msgraph-search-connector-sample)。</span><span class="sxs-lookup"><span data-stu-id="7d416-144">Download the [sample search connector](https://github.com/microsoftgraph/msgraph-search-connector-sample) from GitHub.</span></span>

## <a name="see-also"></a><span data-ttu-id="7d416-145">另请参阅</span><span class="sxs-lookup"><span data-stu-id="7d416-145">See also</span></span>

- <span data-ttu-id="7d416-146">在 [Microsoft Q&A](/answers/products/m365#microsoft-graph) 上或 GitHub 上与社区互动</span><span class="sxs-lookup"><span data-stu-id="7d416-146">Engage with the community on [Microsoft Q&A](/answers/products/m365#microsoft-graph)  or on GitHub</span></span>
