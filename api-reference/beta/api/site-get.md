---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: 获取 SharePoint 网站
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: e0242952a0cecef9ab23cad2cdcd3175dd08fe24
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2019
ms.locfileid: "33638702"
---
# <a name="get-a-site-resource"></a><span data-ttu-id="575d9-102">获取网站资源</span><span class="sxs-lookup"><span data-stu-id="575d9-102">Get a site resource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="575d9-p101">检索[网站][]资源的属性和关系。**网站**资源表示 SharePoint 中的团队网站。</span><span class="sxs-lookup"><span data-stu-id="575d9-p101">Retrieve properties and relationships for a [site][] resource. A **site** resource represents a team site in SharePoint.</span></span>

[网站]: ../resources/site.md
[site]: ../resources/site.md

<span data-ttu-id="575d9-106">**网站**可按唯一标识符处理，此唯一标识符是下列值的复合 ID：</span><span class="sxs-lookup"><span data-stu-id="575d9-106">A **site** is addressed be a unique identifier which is a composite ID of the following values:</span></span>

* <span data-ttu-id="575d9-107">网站集主机名称 (contoso.sharepoint.com)</span><span class="sxs-lookup"><span data-stu-id="575d9-107">Site collection hostname (contoso.sharepoint.com)</span></span>
* <span data-ttu-id="575d9-108">网站集的唯一 ID (GUID)</span><span class="sxs-lookup"><span data-stu-id="575d9-108">Site collection unique ID (GUID)</span></span>
* <span data-ttu-id="575d9-109">网站的唯一 ID (GUID)</span><span class="sxs-lookup"><span data-stu-id="575d9-109">Site unique ID (GUID)</span></span>

<span data-ttu-id="575d9-110">还有一个保留的网站标识符，即 `root`。它经常用于引用给定目标的根网站，如下所示：</span><span class="sxs-lookup"><span data-stu-id="575d9-110">There is also a reserved site identifier, `root`, which always references the root site for a given target, as follows:</span></span>

* <span data-ttu-id="575d9-111">`/sites/root`：租户根网站。</span><span class="sxs-lookup"><span data-stu-id="575d9-111">`/sites/root`: The tenant root site.</span></span>
* <span data-ttu-id="575d9-112">`/groups/{group-id}/sites/root`：该组的团队网站。</span><span class="sxs-lookup"><span data-stu-id="575d9-112">`/groups/{group-id}/sites/root`: The group's team site.</span></span>

## <a name="permissions"></a><span data-ttu-id="575d9-113">权限</span><span class="sxs-lookup"><span data-stu-id="575d9-113">Permissions</span></span>

<span data-ttu-id="575d9-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="575d9-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="575d9-116">权限类型</span><span class="sxs-lookup"><span data-stu-id="575d9-116">Permission type</span></span>      | <span data-ttu-id="575d9-117">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="575d9-117">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="575d9-118">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="575d9-118">Delegated (work or school account)</span></span> | <span data-ttu-id="575d9-119">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="575d9-119">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="575d9-120">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="575d9-120">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="575d9-121">不支持。</span><span class="sxs-lookup"><span data-stu-id="575d9-121">Not supported.</span></span>    |
|<span data-ttu-id="575d9-122">应用程序</span><span class="sxs-lookup"><span data-stu-id="575d9-122">Application</span></span> | <span data-ttu-id="575d9-123">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="575d9-123">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="get-the-tenants-root-site"></a><span data-ttu-id="575d9-124">获取租户的根网站</span><span class="sxs-lookup"><span data-stu-id="575d9-124">Get the tenant's root site</span></span>

<span data-ttu-id="575d9-125">若要访问租户内的根 SharePoint 网站：</span><span class="sxs-lookup"><span data-stu-id="575d9-125">To access the root SharePoint site within a tenant:</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /sites/root
GET /sites/contoso.sharepoint.com
```

## <a name="access-a-site-by-server-relative-url"></a><span data-ttu-id="575d9-126">通过相对于服务器的 URL 访问网站</span><span class="sxs-lookup"><span data-stu-id="575d9-126">Access a site by server-relative URL</span></span>

<span data-ttu-id="575d9-127">如果你的服务器具有**网站**资源的相对于服务器的 URL，你可以构建请求，如下所示：</span><span class="sxs-lookup"><span data-stu-id="575d9-127">If you have the server-relative URL for a **site** resource, you can construct a request as follows:</span></span>

```http
GET /sites/{hostname}:/{server-relative-path}
```

## <a name="access-a-group-team-site"></a><span data-ttu-id="575d9-128">访问组团队网站</span><span class="sxs-lookup"><span data-stu-id="575d9-128">Access a group team site</span></span>

<span data-ttu-id="575d9-129">若要访问组的团队网站：</span><span class="sxs-lookup"><span data-stu-id="575d9-129">To access the team site for a group:</span></span>

```http
GET /groups/{group-id}/sites/root
```

## <a name="example"></a><span data-ttu-id="575d9-130">示例</span><span class="sxs-lookup"><span data-stu-id="575d9-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="575d9-131">请求</span><span class="sxs-lookup"><span data-stu-id="575d9-131">Request</span></span>

<!-- { "blockType": "request", "name": "get-site" } -->

```http
GET /sites/{site-id}
```

### <a name="response"></a><span data-ttu-id="575d9-132">响应</span><span class="sxs-lookup"><span data-stu-id="575d9-132">Response</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="575d9-133">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="575d9-133">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="575d9-134">语言</span><span class="sxs-lookup"><span data-stu-id="575d9-134">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get-site-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="575d9-135">Javascript</span><span class="sxs-lookup"><span data-stu-id="575d9-135">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get-site-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Sites/Get by ID",
  "suppressions": [
    "Error: /api-reference/beta/api/site-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/site-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
