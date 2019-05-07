---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: 搜索网站
description: 在 SharePoint 租户中搜索与所提供的关键字匹配的网站。
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 5dedb77a362507b5d59a8372f64bd72d6504c980
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2019
ms.locfileid: "33603073"
---
# <a name="search-for-sites"></a><span data-ttu-id="fce7f-103">搜索网站</span><span class="sxs-lookup"><span data-stu-id="fce7f-103">Search for sites</span></span>

<span data-ttu-id="fce7f-104">在 SharePoint 租户中搜索与所提供的关键字匹配的[网站][]。</span><span class="sxs-lookup"><span data-stu-id="fce7f-104">Search across a SharePoint tenant for [sites][] that match keywords provided.</span></span>

[网站]: ../resources/site.md
[sites]: ../resources/site.md

## <a name="permissions"></a><span data-ttu-id="fce7f-106">权限</span><span class="sxs-lookup"><span data-stu-id="fce7f-106">Permissions</span></span>

<span data-ttu-id="fce7f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="fce7f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fce7f-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="fce7f-109">Permission type</span></span>                        | <span data-ttu-id="fce7f-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="fce7f-110">Permissions (from least to most privileged)</span></span>
|:--------------------------------------|:-------------------------------------
|<span data-ttu-id="fce7f-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="fce7f-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="fce7f-112">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fce7f-112">Sites.Read.All, Sites.ReadWrite.All</span></span>
|<span data-ttu-id="fce7f-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="fce7f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fce7f-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="fce7f-114">Not supported.</span></span>
|<span data-ttu-id="fce7f-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="fce7f-115">Application</span></span>                            | <span data-ttu-id="fce7f-116">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fce7f-116">Sites.Read.All, Sites.ReadWrite.All</span></span>

## <a name="http-request"></a><span data-ttu-id="fce7f-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="fce7f-117">HTTP request</span></span>

<!-- { "blockType": "request", "name": "search-sites", "scopes": "sites.readwrite.all", "tags": "service.sharepoint" } -->

```http
GET /sites?search={query}
```

## <a name="response"></a><span data-ttu-id="fce7f-118">响应</span><span class="sxs-lookup"><span data-stu-id="fce7f-118">Response</span></span>

<!-- { "blockType": "response", "@type": "Collection(microsoft.graph.site)", "truncated": true } -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "contoso.sharepoint.com,da60e844-ba1d-49bc-b4d4-d5e36bae9019,712a596e-90a1-49e3-9b48-bfa80bee8740",
      "name": "Team A Site",
      "description": "",
      "createdDateTime": "2016-10-18T03:05:59Z",
      "lastModifiedDateTime": "2016-10-18T10:40:59Z",
      "webUrl": "https://contoso.sharepoint.com/sites/siteA"
    },
    {
      "id": "contoso.sharepoint.com,da60e844-ba1d-49bc-b4d4-d5e36bae9019,0271110f-634f-4300-a841-3a8a2e851851",
      "name": "Team B Site",
      "description": "",
      "createdDateTime": "2016-10-18T03:05:59Z",
      "lastModifiedDateTime": "2016-10-18T10:40:59Z",
      "webUrl": "https://contoso.sharepoint.com/sites/siteB"
    }
  ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="fce7f-119">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="fce7f-119">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="fce7f-120">语言</span><span class="sxs-lookup"><span data-stu-id="fce7f-120">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/search-sites-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="fce7f-121">Javascript</span><span class="sxs-lookup"><span data-stu-id="fce7f-121">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/search-sites-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]
><span data-ttu-id="fce7f-122">**注意:** 用于排序的唯一属性是**createdDateTime**。</span><span class="sxs-lookup"><span data-stu-id="fce7f-122">**Note:** The only property that works for sorting is **createdDateTime**.</span></span> <span data-ttu-id="fce7f-123">搜索筛选器是在检索搜索结果时使用多个属性的无文本搜索。</span><span class="sxs-lookup"><span data-stu-id="fce7f-123">The search filter is a free text search that uses multiple properties when retrieving the search results.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Sites/Search",
  "suppressions": [
    "Error: /api-reference/v1.0/api/site-search.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/site-search.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
} -->
