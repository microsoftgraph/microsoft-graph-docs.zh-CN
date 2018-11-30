---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: 按关键字查找 SharePoint 网站
ms.openlocfilehash: c3c5ba005521e3405018e9b9403976297046f242
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27049500"
---
# <a name="search-for-sites"></a><span data-ttu-id="cc4eb-102">搜索网站</span><span class="sxs-lookup"><span data-stu-id="cc4eb-102">Search for sites</span></span>

> <span data-ttu-id="cc4eb-103">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="cc4eb-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="cc4eb-104">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="cc4eb-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="cc4eb-105">在 SharePoint 租户中搜索与所提供的关键字匹配的 [网站][]。</span><span class="sxs-lookup"><span data-stu-id="cc4eb-105">Search across a SharePoint tenant for [sites][] that match provided keywords.</span></span>

[sites]: ../resources/site.md

## <a name="permissions"></a><span data-ttu-id="cc4eb-107">权限</span><span class="sxs-lookup"><span data-stu-id="cc4eb-107">Permissions</span></span>

<span data-ttu-id="cc4eb-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="cc4eb-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cc4eb-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="cc4eb-110">Permission type</span></span>                        | <span data-ttu-id="cc4eb-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="cc4eb-111">Permissions (from least to most privileged)</span></span>
|:--------------------------------------|:-------------------------------------
|<span data-ttu-id="cc4eb-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="cc4eb-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="cc4eb-113">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cc4eb-113">Sites.Read.All, Sites.ReadWrite.All</span></span>
|<span data-ttu-id="cc4eb-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="cc4eb-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cc4eb-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="cc4eb-115">Not supported.</span></span>
|<span data-ttu-id="cc4eb-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="cc4eb-116">Application</span></span>                            | <span data-ttu-id="cc4eb-117">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cc4eb-117">Sites.Read.All, Sites.ReadWrite.All</span></span>

## <a name="http-request"></a><span data-ttu-id="cc4eb-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="cc4eb-118">HTTP request</span></span>

<!-- { "blockType": "request", "name": "search-sites", "scopes": "service.sharepoint sites.readwrite.all" } -->

```http
GET https://graph.microsoft.com/beta/sites?search={query}
```

## <a name="response"></a><span data-ttu-id="cc4eb-119">响应</span><span class="sxs-lookup"><span data-stu-id="cc4eb-119">Response</span></span>

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
