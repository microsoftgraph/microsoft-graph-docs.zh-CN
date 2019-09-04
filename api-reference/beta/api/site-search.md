---
author: JeremyKelley
description: 在 SharePoint 租户中搜索与所提供的关键字匹配的网站。
ms.date: 09/10/2017
title: 按关键字查找 SharePoint 网站
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: dbc66bc734d4ef0a47e30ce1e967918e964489a0
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/04/2019
ms.locfileid: "36724531"
---
# <a name="search-for-sites"></a><span data-ttu-id="2018a-103">搜索网站</span><span class="sxs-lookup"><span data-stu-id="2018a-103">Search for sites</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2018a-104">在 SharePoint 租户中搜索与所提供的关键字匹配的[网站][]。</span><span class="sxs-lookup"><span data-stu-id="2018a-104">Search across a SharePoint tenant for [sites][] that match keywords provided.</span></span>

[网站]: ../resources/site.md
[sites]: ../resources/site.md

## <a name="permissions"></a><span data-ttu-id="2018a-106">权限</span><span class="sxs-lookup"><span data-stu-id="2018a-106">Permissions</span></span>

<span data-ttu-id="2018a-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2018a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2018a-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="2018a-109">Permission type</span></span>                        | <span data-ttu-id="2018a-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="2018a-110">Permissions (from least to most privileged)</span></span>
|:--------------------------------------|:-------------------------------------
|<span data-ttu-id="2018a-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2018a-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="2018a-112">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2018a-112">Sites.Read.All, Sites.ReadWrite.All</span></span>
|<span data-ttu-id="2018a-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2018a-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2018a-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="2018a-114">Not supported.</span></span>
|<span data-ttu-id="2018a-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="2018a-115">Application</span></span>                            | <span data-ttu-id="2018a-116">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2018a-116">Sites.Read.All, Sites.ReadWrite.All</span></span>

## <a name="http-request"></a><span data-ttu-id="2018a-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2018a-117">HTTP request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="2018a-118">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="2018a-118">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "search-sites", "scopes": "service.sharepoint sites.readwrite.all" } -->

```msgraph-interactive
GET https://graph.microsoft.com/beta/sites?search={query}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="2018a-119">C#</span><span class="sxs-lookup"><span data-stu-id="2018a-119">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/search-sites-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="2018a-120">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2018a-120">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/search-sites-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="2018a-121">目标-C</span><span class="sxs-lookup"><span data-stu-id="2018a-121">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/search-sites-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


## <a name="response"></a><span data-ttu-id="2018a-122">响应</span><span class="sxs-lookup"><span data-stu-id="2018a-122">Response</span></span>

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
><span data-ttu-id="2018a-123">**注意:** 用于排序的唯一属性是**createdDateTime**。</span><span class="sxs-lookup"><span data-stu-id="2018a-123">**Note:** The only property that works for sorting is **createdDateTime**.</span></span> <span data-ttu-id="2018a-124">搜索筛选器是在检索搜索结果时使用多个属性的无文本搜索。</span><span class="sxs-lookup"><span data-stu-id="2018a-124">The search filter is a free text search that uses multiple properties when retrieving the search results.</span></span>

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Sites/Search",
  "suppressions": [
  ]
}
-->
