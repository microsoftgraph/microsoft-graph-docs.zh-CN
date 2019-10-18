---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: 获取 SharePoint 网站
localization_priority: Priority
ms.prod: sharepoint
description: 检索网站资源的属性和关系。
doc_type: apiPageType
ms.openlocfilehash: 102295c12ca5278b40c9540049282db360f7701b
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/04/2019
ms.locfileid: "36727717"
---
# <a name="get-a-site-resource"></a><span data-ttu-id="de4ae-103">获取网站资源</span><span class="sxs-lookup"><span data-stu-id="de4ae-103">Get a site resource</span></span>

<span data-ttu-id="de4ae-p101">检索[网站][]资源的属性和关系。**网站**资源表示 SharePoint 中的团队网站。</span><span class="sxs-lookup"><span data-stu-id="de4ae-p101">Retrieve properties and relationships for a [site][] resource. A **site** resource represents a team site in SharePoint.</span></span>

[网站]: ../resources/site.md
[site]: ../resources/site.md

<span data-ttu-id="de4ae-107">**site** 可按唯一标识符进行寻址，此唯一标识符是下列值的复合 ID：</span><span class="sxs-lookup"><span data-stu-id="de4ae-107">A **site** is addressed by a unique identifier which is a composite ID of the following values:</span></span>

* <span data-ttu-id="de4ae-108">网站集主机名称 (contoso.sharepoint.com)</span><span class="sxs-lookup"><span data-stu-id="de4ae-108">Site collection hostname (contoso.sharepoint.com)</span></span>
* <span data-ttu-id="de4ae-109">网站集的唯一 ID (GUID)</span><span class="sxs-lookup"><span data-stu-id="de4ae-109">Site collection unique ID (GUID)</span></span>
* <span data-ttu-id="de4ae-110">网站的唯一 ID (GUID)</span><span class="sxs-lookup"><span data-stu-id="de4ae-110">Site unique ID (GUID)</span></span>

<span data-ttu-id="de4ae-111">还有一个保留的网站标识符，即 `root`。它经常用于引用给定目标的根网站，如下所示：</span><span class="sxs-lookup"><span data-stu-id="de4ae-111">There is also a reserved site identifier, `root`, which always references the root site for a given target, as follows:</span></span>

* <span data-ttu-id="de4ae-112">`/sites/root`：租户根网站。</span><span class="sxs-lookup"><span data-stu-id="de4ae-112">`/sites/root`: The tenant root site.</span></span>
* <span data-ttu-id="de4ae-113">`/groups/{group-id}/sites/root`：该组的团队网站。</span><span class="sxs-lookup"><span data-stu-id="de4ae-113">`/groups/{group-id}/sites/root`: The group's team site.</span></span>

## <a name="permissions"></a><span data-ttu-id="de4ae-114">权限</span><span class="sxs-lookup"><span data-stu-id="de4ae-114">Permissions</span></span>

<span data-ttu-id="de4ae-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="de4ae-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="de4ae-117">权限类型</span><span class="sxs-lookup"><span data-stu-id="de4ae-117">Permission type</span></span>      | <span data-ttu-id="de4ae-118">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="de4ae-118">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="de4ae-119">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="de4ae-119">Delegated (work or school account)</span></span> | <span data-ttu-id="de4ae-120">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="de4ae-120">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="de4ae-121">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="de4ae-121">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="de4ae-122">不支持。</span><span class="sxs-lookup"><span data-stu-id="de4ae-122">Not supported.</span></span>    |
|<span data-ttu-id="de4ae-123">应用程序</span><span class="sxs-lookup"><span data-stu-id="de4ae-123">Application</span></span> | <span data-ttu-id="de4ae-124">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="de4ae-124">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="get-the-tenants-root-site"></a><span data-ttu-id="de4ae-125">获取租户的根网站</span><span class="sxs-lookup"><span data-stu-id="de4ae-125">Get the tenant's root site</span></span>

<span data-ttu-id="de4ae-126">若要访问租户内的根 SharePoint 网站：</span><span class="sxs-lookup"><span data-stu-id="de4ae-126">To access the root SharePoint site within a tenant:</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /sites/root
GET /sites/contoso.sharepoint.com
```

## <a name="access-a-site-by-server-relative-url"></a><span data-ttu-id="de4ae-127">通过相对于服务器的 URL 访问网站</span><span class="sxs-lookup"><span data-stu-id="de4ae-127">Access a site by server-relative URL</span></span>

<span data-ttu-id="de4ae-128">如果你的服务器具有**网站**资源的相对于服务器的 URL，你可以构建请求，如下所示：</span><span class="sxs-lookup"><span data-stu-id="de4ae-128">If you have the server-relative URL for a **site** resource, you can construct a request as follows:</span></span>

```http
GET /sites/{hostname}:/{server-relative-path}
```

## <a name="access-a-group-team-site"></a><span data-ttu-id="de4ae-129">访问组团队网站</span><span class="sxs-lookup"><span data-stu-id="de4ae-129">Access a group team site</span></span>

<span data-ttu-id="de4ae-130">若要访问组的团队网站：</span><span class="sxs-lookup"><span data-stu-id="de4ae-130">To access the team site for a group:</span></span>

```http
GET /groups/{group-id}/sites/root
```

## <a name="example"></a><span data-ttu-id="de4ae-131">示例</span><span class="sxs-lookup"><span data-stu-id="de4ae-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="de4ae-132">请求</span><span class="sxs-lookup"><span data-stu-id="de4ae-132">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="de4ae-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="de4ae-133">--Http</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-site", "scopes": "sites.read.all" } -->

```msgraph-interactive
GET /sites/{site-id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="de4ae-134">C#</span><span class="sxs-lookup"><span data-stu-id="de4ae-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-site-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="de4ae-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="de4ae-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-site-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="de4ae-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="de4ae-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-site-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="de4ae-137">Java</span><span class="sxs-lookup"><span data-stu-id="de4ae-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-site-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="de4ae-138">响应</span><span class="sxs-lookup"><span data-stu-id="de4ae-138">Response</span></span>

<!-- { "blockType": "response", "@type": "microsoft.graph.site", "truncated": true } -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "contoso.sharepoint.com,2C712604-1370-44E7-A1F5-426573FDA80A,2D2244C3-251A-49EA-93A8-39E1C3A060FE",
  "displayName": "OneDrive Team Site",
  "name": "1drvteam",
  "createdDateTime": "2017-05-09T20:56:00Z",
  "lastModifiedDateTime": "2017-05-09T20:56:01Z",
  "webUrl": "https://contoso.sharepoint.com/teams/1drvteam"
}
```

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Sites/Get by ID",
  "suppressions": [
  ]
} -->
