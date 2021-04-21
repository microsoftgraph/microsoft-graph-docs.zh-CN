---
title: 使用 Microsoft Graph 中的 OneNote API 的最佳做法
description: 本文提供了有关使用 Microsoft Graph 中的 OneNote API 的建议。 这些建议基于 Microsoft 问答和 Twitter 上常见问题&解答。
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
ms.openlocfilehash: d5fdffe531e8b04bc0f64caad8ea81cd9a3bda27
ms.sourcegitcommit: 32c83957ee69f21a10cd5f759adb884ce4b41c52
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/21/2021
ms.locfileid: "51920206"
---
# <a name="best-practices-for-working-with-the-onenote-api-in-microsoft-graph"></a><span data-ttu-id="6b71a-104">使用 Microsoft Graph 中的 OneNote API 的最佳做法</span><span class="sxs-lookup"><span data-stu-id="6b71a-104">Best practices for working with the OneNote API in Microsoft Graph</span></span>

<span data-ttu-id="6b71a-105">本文提供了有关使用 Microsoft Graph 中的 OneNote API 的建议。</span><span class="sxs-lookup"><span data-stu-id="6b71a-105">This article provides recommendations for working with the OneNote APIs in Microsoft Graph.</span></span> <span data-ttu-id="6b71a-106">这些建议基于 Microsoft 问答和 Twitter 上常见问题&[解答](/answers/topics/microsoft-graph-notes.html)  。</span><span class="sxs-lookup"><span data-stu-id="6b71a-106">These recommendations are based on answers to common questions on [Microsoft Q&A](/answers/topics/microsoft-graph-notes.html)  and Twitter.</span></span>

## <a name="use-select-to-select-the-minimum-set-of-properties-you-need"></a><span data-ttu-id="6b71a-107">使用 $select 选择所需的最小属性集</span><span class="sxs-lookup"><span data-stu-id="6b71a-107">Use $select to select the minimum set of properties you need</span></span>

<span data-ttu-id="6b71a-108">查询资源（例如，笔记本中的分区）时，会发出类似于以下内容的请求。</span><span class="sxs-lookup"><span data-stu-id="6b71a-108">When you query for a resource (for example, sections inside a notebook), you make a request similar to the following.</span></span>

```http
GET ~/notebooks/{id}/sections
```

<span data-ttu-id="6b71a-109">这将检索分区的所有属性。</span><span class="sxs-lookup"><span data-stu-id="6b71a-109">This retrieves all the properties of the sections.</span></span> <span data-ttu-id="6b71a-110">然而，你可能并不需要所有属性。</span><span class="sxs-lookup"><span data-stu-id="6b71a-110">However, you might not need all properties.</span></span> <span data-ttu-id="6b71a-111">可以使用 `$select` 查询参数只返回所需属性，如下面的示例中所示。</span><span class="sxs-lookup"><span data-stu-id="6b71a-111">You can use the `$select` query parameter to return just the properties that you want, as shown in the following example.</span></span>

```http
GET ~/notebooks/{id}/sections?$select=id,displayName
```

<span data-ttu-id="6b71a-112">同样的方法适用于其他 OneNote API。</span><span class="sxs-lookup"><span data-stu-id="6b71a-112">The same approach applies to other OneNote APIs.</span></span>

## <a name="use-expand-instead-of-making-multiple-api-calls"></a><span data-ttu-id="6b71a-113">使用 $expand 而不是进行多个 API 调用</span><span class="sxs-lookup"><span data-stu-id="6b71a-113">Use $expand instead of making multiple API calls</span></span>

<span data-ttu-id="6b71a-114">假定你要在分层视图中检索用户的所有笔记本、分区和分区组。</span><span class="sxs-lookup"><span data-stu-id="6b71a-114">Suppose you want to retrieve all of the user’s notebooks, sections, and section groups in a hierarchical view.</span></span> <span data-ttu-id="6b71a-115">可以通过执行以下操作来实现：</span><span class="sxs-lookup"><span data-stu-id="6b71a-115">You might accomplish that by doing the following:</span></span>

* <span data-ttu-id="6b71a-116">调用 `GET ~/notebooks` 以获取笔记本的列表。</span><span class="sxs-lookup"><span data-stu-id="6b71a-116">Call `GET ~/notebooks` to get the list of notebooks.</span></span>

* <span data-ttu-id="6b71a-117">对于每个检索的笔记本，调用 `GET ~/notebooks/{notebookId}/sections` 以检索分区的列表。</span><span class="sxs-lookup"><span data-stu-id="6b71a-117">For every retrieved notebook, call `GET ~/notebooks/{notebookId}/sections` to retrieve the list of sections.</span></span>

* <span data-ttu-id="6b71a-118">对于每个检索的笔记本，调用 `GET ~/notebooks/{notebookId}/sectionGroups` 以检索分区组的列表。</span><span class="sxs-lookup"><span data-stu-id="6b71a-118">For every retrieved notebook, call `GET ~/notebooks/{notebookId}/sectionGroups` to retrieve the list of section groups.</span></span>

* <span data-ttu-id="6b71a-119">（可选）以递归方式遍历分区组。</span><span class="sxs-lookup"><span data-stu-id="6b71a-119">Optionally recursively iterate through section groups.</span></span>

<span data-ttu-id="6b71a-120">虽然此方法有效（同时有一些到服务的额外顺序往返），但更好的方法是使用 `$expand` 查询参数。</span><span class="sxs-lookup"><span data-stu-id="6b71a-120">While this will work (with a few extra sequential roundtrips to the service), a better approach is to use the `$expand` query parameter.</span></span> 

```http
GET ~/notebooks?$expand=sections,sectionGroups($expand=sections)
```

<span data-ttu-id="6b71a-121">这将在一个网络往返中产生同样的结果，而且性能更佳。</span><span class="sxs-lookup"><span data-stu-id="6b71a-121">This will yield the same results in one network roundtrip, with better performance.</span></span>

## <a name="when-getting-all-pages-for-a-user-do-so-for-each-section-separately"></a><span data-ttu-id="6b71a-122">获取用户的所有页面时，分别对每个分区执行此操作</span><span class="sxs-lookup"><span data-stu-id="6b71a-122">When getting all pages for a user, do so for each section separately</span></span>

<span data-ttu-id="6b71a-123">当 Microsoft Graph 公开一个终结点来检索所有页面时，这并不是获取用户可以访问的所有页面的最佳方式。</span><span class="sxs-lookup"><span data-stu-id="6b71a-123">While Microsoft Graph exposes an endpoint to retrieve all pages, this isn't the best way to get all the pages the user has access to.</span></span> <span data-ttu-id="6b71a-124">如果用户拥有的分区过多，可能会导致超时或性能降低。</span><span class="sxs-lookup"><span data-stu-id="6b71a-124">When the user has too many sections, this can lead to timeouts or bad performance.</span></span> <span data-ttu-id="6b71a-125">最好遍历每个分区，从而分别获取每个分区的页面。</span><span class="sxs-lookup"><span data-stu-id="6b71a-125">It is better to iterate each section, getting pages for each one separately.</span></span>

<span data-ttu-id="6b71a-126">例如，不使用此调用（此 API 已分页，因此无法一次获取所有页面）：</span><span class="sxs-lookup"><span data-stu-id="6b71a-126">For example, instead of using this call (this API is paged, so you won't be able to fetch the pages all at once):</span></span>

```http
GET ~/pages
```

<span data-ttu-id="6b71a-127">最好多次使用以下调用（特别是在你不需要所有分区的情况下）：</span><span class="sxs-lookup"><span data-stu-id="6b71a-127">It is better to use the following call several times (especially if you don't need all sections):</span></span>

```http
GET ~/sections/{id}/pages
```

<span data-ttu-id="6b71a-128">获取页面元数据时，请覆盖默认的 `lastModifiedDateTime` 排序。</span><span class="sxs-lookup"><span data-stu-id="6b71a-128">When getting page metadata, override the default `lastModifiedDateTime` ordering.</span></span> <span data-ttu-id="6b71a-129">当不必按 `lastModifiedDateTime` 对页面进行排序时，获取页面的速度更快。</span><span class="sxs-lookup"><span data-stu-id="6b71a-129">It is faster to get pages when you don't have to sort them by `lastModifiedDateTime`.</span></span> <span data-ttu-id="6b71a-130">为此，可以按任何其他属性进行排序；例如：</span><span class="sxs-lookup"><span data-stu-id="6b71a-130">To do this, you can sort by any other property; for example:</span></span>

```http
GET ~/sections/{id}/pages?$select=id,title,createdDateTime&$orderby=createdDateTime
```