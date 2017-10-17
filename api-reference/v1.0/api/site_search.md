---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: "按关键字查找 SharePoint 网站"
ms.openlocfilehash: 53c9d735ad791bd42fb8b0e1c9b9f412ef469dd8
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/28/2017
---
# <a name="search-for-sites"></a><span data-ttu-id="1afe4-102">搜索网站</span><span class="sxs-lookup"><span data-stu-id="1afe4-102">Search for sites</span></span>

<span data-ttu-id="1afe4-103">在 SharePoint 租户中搜索与所提供的关键字匹配的 [sites][]。</span><span class="sxs-lookup"><span data-stu-id="1afe4-103">Search across a SharePoint tenant for [sites][] that match provided keywords.</span></span>

[sites]: ../resources/site.md

## <a name="permissions"></a><span data-ttu-id="1afe4-105">权限</span><span class="sxs-lookup"><span data-stu-id="1afe4-105">Permissions</span></span>

<span data-ttu-id="1afe4-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="1afe4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="1afe4-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="1afe4-108">Permission type</span></span>                        | <span data-ttu-id="1afe4-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="1afe4-109">Permissions (from least to most privileged)</span></span>
|:--------------------------------------|:-------------------------------------
|<span data-ttu-id="1afe4-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1afe4-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="1afe4-111">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1afe4-111">Sites.Read.All, Sites.ReadWrite.All</span></span>
|<span data-ttu-id="1afe4-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1afe4-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1afe4-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="1afe4-113">Not supported.</span></span>
|<span data-ttu-id="1afe4-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="1afe4-114">Application</span></span>                            | <span data-ttu-id="1afe4-115">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1afe4-115">Sites.Read.All, Sites.ReadWrite.All</span></span>

## <a name="http-request"></a><span data-ttu-id="1afe4-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1afe4-116">HTTP request</span></span>

<!-- { "blockType": "request", "name": "search-sites", "scopes": "service.sharepoint sites.readwrite.all" } -->

```http
GET /sites?search={query}
```

## <a name="response"></a><span data-ttu-id="1afe4-117">响应</span><span class="sxs-lookup"><span data-stu-id="1afe4-117">Response</span></span>

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

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Sites/Search"
} -->
