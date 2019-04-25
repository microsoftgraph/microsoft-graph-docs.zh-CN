---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: 按关键字查找 SharePoint 网站
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 156093c9d3b87f0a4e44f6928b36a8aa92a4ef4d
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32537249"
---
# <a name="search-for-sites"></a><span data-ttu-id="94c2b-102">搜索网站</span><span class="sxs-lookup"><span data-stu-id="94c2b-102">Search for sites</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="94c2b-103">在 SharePoint 租户中搜索与所提供的关键字匹配的[网站][]。</span><span class="sxs-lookup"><span data-stu-id="94c2b-103">Search across a SharePoint tenant for [sites][] that match keywords provided.</span></span>

[网站]: ../resources/site.md
[sites]: ../resources/site.md

## <a name="permissions"></a><span data-ttu-id="94c2b-105">权限</span><span class="sxs-lookup"><span data-stu-id="94c2b-105">Permissions</span></span>

<span data-ttu-id="94c2b-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="94c2b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="94c2b-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="94c2b-108">Permission type</span></span>                        | <span data-ttu-id="94c2b-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="94c2b-109">Permissions (from least to most privileged)</span></span>
|:--------------------------------------|:-------------------------------------
|<span data-ttu-id="94c2b-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="94c2b-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="94c2b-111">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="94c2b-111">Sites.Read.All, Sites.ReadWrite.All</span></span>
|<span data-ttu-id="94c2b-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="94c2b-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="94c2b-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="94c2b-113">Not supported.</span></span>
|<span data-ttu-id="94c2b-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="94c2b-114">Application</span></span>                            | <span data-ttu-id="94c2b-115">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="94c2b-115">Sites.Read.All, Sites.ReadWrite.All</span></span>

## <a name="http-request"></a><span data-ttu-id="94c2b-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="94c2b-116">HTTP request</span></span>

<!-- { "blockType": "request", "name": "search-sites", "scopes": "service.sharepoint sites.readwrite.all" } -->

```http
GET https://graph.microsoft.com/beta/sites?search={query}
```

## <a name="response"></a><span data-ttu-id="94c2b-117">响应</span><span class="sxs-lookup"><span data-stu-id="94c2b-117">Response</span></span>

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
><span data-ttu-id="94c2b-118">**注意:** 用于排序的唯一属性是**createdDateTime**。</span><span class="sxs-lookup"><span data-stu-id="94c2b-118">**Note:** The only property that works for sorting is **createdDateTime**.</span></span> <span data-ttu-id="94c2b-119">搜索筛选器是在检索搜索结果时使用多个属性的无文本搜索。</span><span class="sxs-lookup"><span data-stu-id="94c2b-119">The search filter is a free text search that uses multiple properties when retrieving the search results.</span></span>

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Sites/Search",
  "suppressions": [
    "Error: /api-reference/beta/api/site-search.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
