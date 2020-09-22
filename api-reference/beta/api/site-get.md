---
author: JeremyKelley
description: 检索网站资源的属性和关系。
ms.date: 09/10/2017
title: 获取 SharePoint 网站
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: 8eeb912a8655b0020733a5b94dea9cb6ede22c5c
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48014033"
---
# <a name="get-a-site-resource"></a><span data-ttu-id="eea2b-103">获取网站资源</span><span class="sxs-lookup"><span data-stu-id="eea2b-103">Get a site resource</span></span>

<span data-ttu-id="eea2b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="eea2b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="eea2b-p101">检索[网站][]资源的属性和关系。**网站**资源表示 SharePoint 中的团队网站。</span><span class="sxs-lookup"><span data-stu-id="eea2b-p101">Retrieve properties and relationships for a [site][] resource. A **site** resource represents a team site in SharePoint.</span></span>

[site]: ../resources/site.md

## <a name="permissions"></a><span data-ttu-id="eea2b-108">权限</span><span class="sxs-lookup"><span data-stu-id="eea2b-108">Permissions</span></span>

<span data-ttu-id="eea2b-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="eea2b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="eea2b-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="eea2b-111">Permission type</span></span>      | <span data-ttu-id="eea2b-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="eea2b-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="eea2b-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="eea2b-113">Delegated (work or school account)</span></span> | <span data-ttu-id="eea2b-114">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eea2b-114">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="eea2b-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="eea2b-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="eea2b-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="eea2b-116">Not supported.</span></span>    |
|<span data-ttu-id="eea2b-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="eea2b-117">Application</span></span> | <span data-ttu-id="eea2b-118">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eea2b-118">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="get-the-tenants-root-site"></a><span data-ttu-id="eea2b-119">获取租户的根网站</span><span class="sxs-lookup"><span data-stu-id="eea2b-119">Get the tenant's root site</span></span>

<span data-ttu-id="eea2b-120">若要访问租户内的根 SharePoint 网站：</span><span class="sxs-lookup"><span data-stu-id="eea2b-120">To access the root SharePoint site within a tenant:</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /sites/root
GET /sites/contoso.sharepoint.com
```

## <a name="access-a-site-by-server-relative-url"></a><span data-ttu-id="eea2b-121">通过相对于服务器的 URL 访问网站</span><span class="sxs-lookup"><span data-stu-id="eea2b-121">Access a site by server-relative URL</span></span>

<span data-ttu-id="eea2b-122">如果你的服务器具有**网站**资源的相对于服务器的 URL，你可以构建请求，如下所示：</span><span class="sxs-lookup"><span data-stu-id="eea2b-122">If you have the server-relative URL for a **site** resource, you can construct a request as follows:</span></span>

```http
GET /sites/{hostname}:/{server-relative-path}
```

## <a name="access-a-group-team-site"></a><span data-ttu-id="eea2b-123">访问组团队网站</span><span class="sxs-lookup"><span data-stu-id="eea2b-123">Access a group team site</span></span>

<span data-ttu-id="eea2b-124">若要访问组的团队网站：</span><span class="sxs-lookup"><span data-stu-id="eea2b-124">To access the team site for a group:</span></span>

```http
GET /groups/{group-id}/sites/root
```

## <a name="example"></a><span data-ttu-id="eea2b-125">示例</span><span class="sxs-lookup"><span data-stu-id="eea2b-125">Example</span></span>

### <a name="request"></a><span data-ttu-id="eea2b-126">请求</span><span class="sxs-lookup"><span data-stu-id="eea2b-126">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="eea2b-127">HTTP</span><span class="sxs-lookup"><span data-stu-id="eea2b-127">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-site" } -->

```msgraph-interactive
GET /sites/{site-id}
```
# <a name="c"></a>[<span data-ttu-id="eea2b-128">C#</span><span class="sxs-lookup"><span data-stu-id="eea2b-128">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-site-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="eea2b-129">JavaScript</span><span class="sxs-lookup"><span data-stu-id="eea2b-129">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-site-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="eea2b-130">Objective-C</span><span class="sxs-lookup"><span data-stu-id="eea2b-130">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-site-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="eea2b-131">响应</span><span class="sxs-lookup"><span data-stu-id="eea2b-131">Response</span></span>

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


