---
author: JeremyKelley
description: 检索网站资源的属性和关系。
ms.date: 09/10/2017
title: 获取 SharePoint 网站
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: 86bcd7073838b7af2b0decc7ed796650b9c5ad0f
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/15/2019
ms.locfileid: "36410010"
---
# <a name="get-a-site-resource"></a><span data-ttu-id="a7689-103">获取网站资源</span><span class="sxs-lookup"><span data-stu-id="a7689-103">Get a site resource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a7689-p101">检索[网站][]资源的属性和关系。**网站**资源表示 SharePoint 中的团队网站。</span><span class="sxs-lookup"><span data-stu-id="a7689-p101">Retrieve properties and relationships for a [site][] resource. A **site** resource represents a team site in SharePoint.</span></span>

[网站]: ../resources/site.md
[site]: ../resources/site.md

## <a name="permissions"></a><span data-ttu-id="a7689-107">权限</span><span class="sxs-lookup"><span data-stu-id="a7689-107">Permissions</span></span>

<span data-ttu-id="a7689-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a7689-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a7689-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="a7689-110">Permission type</span></span>      | <span data-ttu-id="a7689-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a7689-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a7689-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a7689-112">Delegated (work or school account)</span></span> | <span data-ttu-id="a7689-113">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a7689-113">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="a7689-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a7689-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a7689-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="a7689-115">Not supported.</span></span>    |
|<span data-ttu-id="a7689-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="a7689-116">Application</span></span> | <span data-ttu-id="a7689-117">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a7689-117">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="get-the-tenants-root-site"></a><span data-ttu-id="a7689-118">获取租户的根网站</span><span class="sxs-lookup"><span data-stu-id="a7689-118">Get the tenant's root site</span></span>

<span data-ttu-id="a7689-119">若要访问租户内的根 SharePoint 网站：</span><span class="sxs-lookup"><span data-stu-id="a7689-119">To access the root SharePoint site within a tenant:</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /sites/root
GET /sites/contoso.sharepoint.com
```

## <a name="access-a-site-by-server-relative-url"></a><span data-ttu-id="a7689-120">通过相对于服务器的 URL 访问网站</span><span class="sxs-lookup"><span data-stu-id="a7689-120">Access a site by server-relative URL</span></span>

<span data-ttu-id="a7689-121">如果你的服务器具有**网站**资源的相对于服务器的 URL，你可以构建请求，如下所示：</span><span class="sxs-lookup"><span data-stu-id="a7689-121">If you have the server-relative URL for a **site** resource, you can construct a request as follows:</span></span>

```http
GET /sites/{hostname}:/{server-relative-path}
```

## <a name="access-a-group-team-site"></a><span data-ttu-id="a7689-122">访问组团队网站</span><span class="sxs-lookup"><span data-stu-id="a7689-122">Access a group team site</span></span>

<span data-ttu-id="a7689-123">若要访问组的团队网站：</span><span class="sxs-lookup"><span data-stu-id="a7689-123">To access the team site for a group:</span></span>

```http
GET /groups/{group-id}/sites/root
```

## <a name="example"></a><span data-ttu-id="a7689-124">示例</span><span class="sxs-lookup"><span data-stu-id="a7689-124">Example</span></span>

### <a name="request"></a><span data-ttu-id="a7689-125">请求</span><span class="sxs-lookup"><span data-stu-id="a7689-125">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="a7689-126">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="a7689-126">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-site" } -->

```http
GET /sites/{site-id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="a7689-127">C#</span><span class="sxs-lookup"><span data-stu-id="a7689-127">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-site-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="a7689-128">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a7689-128">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-site-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="a7689-129">目标-C</span><span class="sxs-lookup"><span data-stu-id="a7689-129">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-site-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="a7689-130">响应</span><span class="sxs-lookup"><span data-stu-id="a7689-130">Response</span></span>

<!-- { "blockType": "response", "@type": "microsoft.graph.site", "truncated": true } -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "contoso.sharepoint.com,2C712604-1370-44E7-A1F5-426573FDA80A,2D2244C3-251A-49EA-93A8-39E1C3A060FE",
  "owner": {
    "user": {
      "displayName": "Daron Spektor",
      "id": "5280E7FE-DC7A-4486-9490-E790D81DFEB3"
    }
  },
  "displayName": "OneDrive Team Site",
  "name": "1drvteam",
  "createdDateTime": "2017-05-09T20:56:00Z",
  "lastModifiedDateTime": "2017-05-09T20:56:01Z",
  "webUrl": "https://contoso.sharepoint.com/teams/1drvteam"
}
```

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Sites/Get by ID",
  "suppressions": [
  ]
}
-->
