---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: 获取 SharePoint 网站
localization_priority: Normal
ms.openlocfilehash: 72a99b1768486da792a401cea4b8dfde5a25a153
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27872854"
---
# <a name="get-a-site-resource"></a><span data-ttu-id="a57f5-102">获取网站资源</span><span class="sxs-lookup"><span data-stu-id="a57f5-102">Get a site resource</span></span>

> <span data-ttu-id="a57f5-103">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="a57f5-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a57f5-104">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="a57f5-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a57f5-p102">检索[网站][]资源的属性和关系。**网站**资源表示 SharePoint 中的团队网站。</span><span class="sxs-lookup"><span data-stu-id="a57f5-p102">Retrieve properties and relationships for a [site][] resource. A **site** resource represents a team site in SharePoint.</span></span>

[网站]: ../resources/site.md
[site]: ../resources/site.md

<span data-ttu-id="a57f5-108">**网站**可按唯一标识符处理，此唯一标识符是下列值的复合 ID：</span><span class="sxs-lookup"><span data-stu-id="a57f5-108">A **site** is addressed be a unique identifier which is a composite ID of the following values:</span></span>

* <span data-ttu-id="a57f5-109">网站集主机名称 (contoso.sharepoint.com)</span><span class="sxs-lookup"><span data-stu-id="a57f5-109">Site collection hostname (contoso.sharepoint.com)</span></span>
* <span data-ttu-id="a57f5-110">网站集的唯一 ID (GUID)</span><span class="sxs-lookup"><span data-stu-id="a57f5-110">Site collection unique ID (GUID)</span></span>
* <span data-ttu-id="a57f5-111">网站的唯一 ID (GUID)</span><span class="sxs-lookup"><span data-stu-id="a57f5-111">Site unique ID (GUID)</span></span>

<span data-ttu-id="a57f5-112">还有一个保留的网站标识符，即 `root`。它经常用于引用给定目标的根网站，如下所示：</span><span class="sxs-lookup"><span data-stu-id="a57f5-112">There is also a reserved site identifier, `root`, which always references the root site for a given target, as follows:</span></span>

* <span data-ttu-id="a57f5-113">`/sites/root`：租户根网站。</span><span class="sxs-lookup"><span data-stu-id="a57f5-113">`/sites/root`: The tenant root site.</span></span>
* <span data-ttu-id="a57f5-114">`/groups/{group-id}/sites/root`：该组的团队网站。</span><span class="sxs-lookup"><span data-stu-id="a57f5-114">`/groups/{group-id}/sites/root`: The group's team site.</span></span>

## <a name="permissions"></a><span data-ttu-id="a57f5-115">权限</span><span class="sxs-lookup"><span data-stu-id="a57f5-115">Permissions</span></span>

<span data-ttu-id="a57f5-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a57f5-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a57f5-118">权限类型</span><span class="sxs-lookup"><span data-stu-id="a57f5-118">Permission type</span></span>      | <span data-ttu-id="a57f5-119">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a57f5-119">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a57f5-120">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a57f5-120">Delegated (work or school account)</span></span> | <span data-ttu-id="a57f5-121">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a57f5-121">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="a57f5-122">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a57f5-122">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a57f5-123">不支持。</span><span class="sxs-lookup"><span data-stu-id="a57f5-123">Not supported.</span></span>    |
|<span data-ttu-id="a57f5-124">应用程序</span><span class="sxs-lookup"><span data-stu-id="a57f5-124">Application</span></span> | <span data-ttu-id="a57f5-125">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a57f5-125">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="get-the-tenants-root-site"></a><span data-ttu-id="a57f5-126">获取租户的根网站</span><span class="sxs-lookup"><span data-stu-id="a57f5-126">Get the tenant's root site</span></span>

<span data-ttu-id="a57f5-127">若要访问租户内的根 SharePoint 网站：</span><span class="sxs-lookup"><span data-stu-id="a57f5-127">To access the root SharePoint site within a tenant:</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /sites/root
GET /sites/contoso.sharepoint.com
```

## <a name="access-a-site-by-server-relative-url"></a><span data-ttu-id="a57f5-128">通过相对于服务器的 URL 访问网站</span><span class="sxs-lookup"><span data-stu-id="a57f5-128">Access a site by server-relative URL</span></span>

<span data-ttu-id="a57f5-129">如果你的服务器具有**网站**资源的相对于服务器的 URL，你可以构建请求，如下所示：</span><span class="sxs-lookup"><span data-stu-id="a57f5-129">If you have the server-relative URL for a **site** resource, you can construct a request as follows:</span></span>

```http
GET /sites/{hostname}:/{server-relative-path}
```

## <a name="access-a-group-team-site"></a><span data-ttu-id="a57f5-130">访问组团队网站</span><span class="sxs-lookup"><span data-stu-id="a57f5-130">Access a group team site</span></span>

<span data-ttu-id="a57f5-131">若要访问组的团队网站：</span><span class="sxs-lookup"><span data-stu-id="a57f5-131">To access the team site for a group:</span></span>

```http
GET /groups/{group-id}/sites/root
```

## <a name="example"></a><span data-ttu-id="a57f5-132">示例</span><span class="sxs-lookup"><span data-stu-id="a57f5-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="a57f5-133">请求</span><span class="sxs-lookup"><span data-stu-id="a57f5-133">Request</span></span>

<!-- { "blockType": "request", "name": "get-site" } -->

```http
GET /sites/{site-id}
```

### <a name="response"></a><span data-ttu-id="a57f5-134">响应</span><span class="sxs-lookup"><span data-stu-id="a57f5-134">Response</span></span>

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

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Sites/Get by ID"
} -->
