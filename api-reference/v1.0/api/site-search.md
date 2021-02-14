---
author: JeremyKelley
ms.date: 09/10/2017
title: 搜索网站
description: 在 SharePoint 租户中搜索与所提供的关键字匹配的 网站。
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: 52c3fe2489b994c826506e8e4425ed508873ecbd
ms.sourcegitcommit: 5b0aab5422e0619ce8806664c479479d223129ec
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/14/2021
ms.locfileid: "50238482"
---
# <a name="search-for-sites"></a><span data-ttu-id="f8701-103">搜索网站</span><span class="sxs-lookup"><span data-stu-id="f8701-103">Search for sites</span></span>

<span data-ttu-id="f8701-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f8701-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="f8701-105">在 SharePoint 租户中搜索 [与][] 提供的关键字匹配的网站。</span><span class="sxs-lookup"><span data-stu-id="f8701-105">Search across a SharePoint tenant for [sites][] that match keywords provided.</span></span>

[网站]: ../resources/site.md
[sites]: ../resources/site.md

## <a name="permissions"></a><span data-ttu-id="f8701-107">权限</span><span class="sxs-lookup"><span data-stu-id="f8701-107">Permissions</span></span>

<span data-ttu-id="f8701-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f8701-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f8701-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="f8701-110">Permission type</span></span>                        | <span data-ttu-id="f8701-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f8701-111">Permissions (from least to most privileged)</span></span>
|:--------------------------------------|:-------------------------------------
|<span data-ttu-id="f8701-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f8701-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="f8701-113">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f8701-113">Sites.Read.All, Sites.ReadWrite.All</span></span>
|<span data-ttu-id="f8701-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f8701-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f8701-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="f8701-115">Not supported.</span></span>
|<span data-ttu-id="f8701-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="f8701-116">Application</span></span>                            | <span data-ttu-id="f8701-117">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f8701-117">Sites.Read.All, Sites.ReadWrite.All</span></span>

## <a name="http-request"></a><span data-ttu-id="f8701-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f8701-118">HTTP request</span></span>


# <a name="http"></a>[<span data-ttu-id="f8701-119">HTTP</span><span class="sxs-lookup"><span data-stu-id="f8701-119">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "search-sites", "scopes": "sites.readwrite.all", "tags": "service.sharepoint" } -->

```msgraph-interactive
GET /sites?search={query}
```
# <a name="c"></a>[<span data-ttu-id="f8701-120">C#</span><span class="sxs-lookup"><span data-stu-id="f8701-120">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/search-sites-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f8701-121">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f8701-121">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/search-sites-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f8701-122">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f8701-122">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/search-sites-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f8701-123">Java</span><span class="sxs-lookup"><span data-stu-id="f8701-123">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/search-sites-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


## <a name="response"></a><span data-ttu-id="f8701-124">响应</span><span class="sxs-lookup"><span data-stu-id="f8701-124">Response</span></span>

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
><span data-ttu-id="f8701-125">**注意：** 唯一用于排序的属性是 **createdDateTime**。</span><span class="sxs-lookup"><span data-stu-id="f8701-125">**Note:** The only property that works for sorting is **createdDateTime**.</span></span> <span data-ttu-id="f8701-126">搜索筛选器是一种自由文本搜索，在检索搜索结果时使用多个属性。</span><span class="sxs-lookup"><span data-stu-id="f8701-126">The search filter is a free text search that uses multiple properties when retrieving the search results.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Sites/Search",
  "suppressions": [
  ]
} -->

