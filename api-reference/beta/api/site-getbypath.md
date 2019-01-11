---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: 按路径获取 SharePoint 网站
localization_priority: Normal
ms.openlocfilehash: 09d9aef99f552079e8e5e4f7d0d260964a182786
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27821530"
---
# <a name="get-a-site-resource-by-path"></a><span data-ttu-id="42152-102">按路径获取 site 资源</span><span class="sxs-lookup"><span data-stu-id="42152-102">Get a site resource by path</span></span>

> <span data-ttu-id="42152-103">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="42152-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="42152-104">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="42152-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="42152-p102">检索[网站][]资源的属性和关系。**网站**资源表示 SharePoint 中的团队网站。</span><span class="sxs-lookup"><span data-stu-id="42152-p102">Retrieve properties and relationships for a [site][] resource. A **site** resource represents a team site in SharePoint.</span></span>

[site]: ../resources/site.md

<span data-ttu-id="42152-108">除了可以[按 ID 检索网站](site-get.md)外，还可以按相对服务器 URL 路径检索网站。</span><span class="sxs-lookup"><span data-stu-id="42152-108">In addition to retrieving a [site by ID](site-get.md) you can retrieve a site based on server-relative URL path.</span></span>

* <span data-ttu-id="42152-109">网站集主机名 (contoso.sharepoint.com)</span><span class="sxs-lookup"><span data-stu-id="42152-109">Site collection hostname (contoso.sharepoint.com)</span></span>
* <span data-ttu-id="42152-110">相对服务器主机名的网站路径。</span><span class="sxs-lookup"><span data-stu-id="42152-110">Site path, relative to server hostname.</span></span>

<span data-ttu-id="42152-111">还有一个保留的网站标识符，即 `root`。它经常用于引用给定目标的根网站，如下所示：</span><span class="sxs-lookup"><span data-stu-id="42152-111">There is also a reserved site identifier, `root`, which always references the root site for a given target, as follows:</span></span>

* <span data-ttu-id="42152-112">`/sites/root`：租户根网站。</span><span class="sxs-lookup"><span data-stu-id="42152-112">`/sites/root`: The tenant root site.</span></span>
* <span data-ttu-id="42152-113">`/groups/{group-id}/sites/root`：该组的团队网站。</span><span class="sxs-lookup"><span data-stu-id="42152-113">`/groups/{group-id}/sites/root`: The group's team site.</span></span>

## <a name="permissions"></a><span data-ttu-id="42152-114">权限</span><span class="sxs-lookup"><span data-stu-id="42152-114">Permissions</span></span>

<span data-ttu-id="42152-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="42152-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="42152-117">权限类型</span><span class="sxs-lookup"><span data-stu-id="42152-117">Permission type</span></span>      | <span data-ttu-id="42152-118">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="42152-118">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="42152-119">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="42152-119">Delegated (work or school account)</span></span> | <span data-ttu-id="42152-120">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="42152-120">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="42152-121">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="42152-121">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="42152-122">不支持。</span><span class="sxs-lookup"><span data-stu-id="42152-122">Not supported.</span></span>    |
|<span data-ttu-id="42152-123">应用程序</span><span class="sxs-lookup"><span data-stu-id="42152-123">Application</span></span> | <span data-ttu-id="42152-124">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="42152-124">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="42152-125">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="42152-125">HTTP Request</span></span>

<span data-ttu-id="42152-126">若要通过相对路径访问根 SharePoint 网站，请运行以下命令：</span><span class="sxs-lookup"><span data-stu-id="42152-126">To access the root SharePoint site with a relative path:</span></span>

<!-- { "blockType": "request", "name": "get-site-by-hostname-and-path", "scopes": "service.sharepoint sites.read.all" } -->

```http
GET /sites/{hostname}:/{relative-path}
```

## <a name="response"></a><span data-ttu-id="42152-127">响应</span><span class="sxs-lookup"><span data-stu-id="42152-127">Response</span></span>

<span data-ttu-id="42152-128">此方法返回唯一标识符引用的网站的 [网站][] 资源。</span><span class="sxs-lookup"><span data-stu-id="42152-128">This method returns a [site][] resource for the site referenced by the unique identifier.</span></span>

<!-- { "blockType": "response", "truncated": true, "@odata.type": "microsoft.graph.site" } -->

```http
HTTP/1.1 200 OK

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
  "tocPath": "Sites/Get by path"
} -->
