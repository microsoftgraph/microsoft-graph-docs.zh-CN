---
author: JeremyKelley
ms.date: 09/10/2017
title: 按路径获取 SharePoint 网站
localization_priority: Normal
ms.prod: sharepoint
description: 检索网站资源的属性和关系。
doc_type: apiPageType
ms.openlocfilehash: 2b4323788a12a1107777a8176fb04b4357ee44f3
ms.sourcegitcommit: b0194231721c68053a0be6d8eb46687574eb8d71
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/18/2021
ms.locfileid: "50292586"
---
# <a name="get-a-site-resource-by-path"></a><span data-ttu-id="3a507-103">按路径获取网站资源</span><span class="sxs-lookup"><span data-stu-id="3a507-103">Get a site resource by path</span></span>

<span data-ttu-id="3a507-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3a507-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="3a507-p101">检索 [网站][]资源的属性和关系。**网站** 资源表示 SharePoint 中的团队网站。</span><span class="sxs-lookup"><span data-stu-id="3a507-p101">Retrieve properties and relationships for a [site][] resource. A **site** resource represents a team site in SharePoint.</span></span>

[网站]: ../resources/site.md
[site]: ../resources/site.md

<span data-ttu-id="3a507-108">除了可以[按 ID 检索网站](site-get.md)外，还可以按相对服务器 URL 路径检索网站。</span><span class="sxs-lookup"><span data-stu-id="3a507-108">In addition to retrieving a [site by ID](site-get.md) you can retrieve a site based on server-relative URL path.</span></span>

* <span data-ttu-id="3a507-109">网站集主机名 (contoso.sharepoint.com)</span><span class="sxs-lookup"><span data-stu-id="3a507-109">Site collection hostname (contoso.sharepoint.com)</span></span>
* <span data-ttu-id="3a507-110">相对服务器主机名的网站路径。</span><span class="sxs-lookup"><span data-stu-id="3a507-110">Site path, relative to server hostname.</span></span>

<span data-ttu-id="3a507-111">还有一个保留的网站标识符，即 `root`。它经常用于引用给定目标的根网站，如下所示：</span><span class="sxs-lookup"><span data-stu-id="3a507-111">There is also a reserved site identifier, `root`, which always references the root site for a given target, as follows:</span></span>

* <span data-ttu-id="3a507-112">`/sites/root`：租户根网站。</span><span class="sxs-lookup"><span data-stu-id="3a507-112">`/sites/root`: The tenant root site.</span></span>
* <span data-ttu-id="3a507-113">`/groups/{group-id}/sites/root`：该组的团队网站。</span><span class="sxs-lookup"><span data-stu-id="3a507-113">`/groups/{group-id}/sites/root`: The group's team site.</span></span>

## <a name="permissions"></a><span data-ttu-id="3a507-114">权限</span><span class="sxs-lookup"><span data-stu-id="3a507-114">Permissions</span></span>

<span data-ttu-id="3a507-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="3a507-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3a507-117">权限类型</span><span class="sxs-lookup"><span data-stu-id="3a507-117">Permission type</span></span>      | <span data-ttu-id="3a507-118">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="3a507-118">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3a507-119">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3a507-119">Delegated (work or school account)</span></span> | <span data-ttu-id="3a507-120">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3a507-120">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="3a507-121">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3a507-121">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3a507-122">不支持。</span><span class="sxs-lookup"><span data-stu-id="3a507-122">Not supported.</span></span>    |
|<span data-ttu-id="3a507-123">应用程序</span><span class="sxs-lookup"><span data-stu-id="3a507-123">Application</span></span> | <span data-ttu-id="3a507-124">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3a507-124">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="3a507-125">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3a507-125">HTTP Request</span></span>

<span data-ttu-id="3a507-126">若要通过相对路径访问根 SharePoint 网站，请运行以下命令：</span><span class="sxs-lookup"><span data-stu-id="3a507-126">To access the root SharePoint site with a relative path:</span></span>

<!-- { "blockType": "request", "name": "get-site-by-hostname-and-path", "scopes": "sites.read.all", "tags": "service.sharepoint" } -->

```http
GET /sites/{hostname}:/{relative-path}
```

## <a name="response"></a><span data-ttu-id="3a507-127">响应</span><span class="sxs-lookup"><span data-stu-id="3a507-127">Response</span></span>

<span data-ttu-id="3a507-128">此方法返回唯一标识符引用的网站的 [site][] 资源。</span><span class="sxs-lookup"><span data-stu-id="3a507-128">This method returns a [site][] resource for the site referenced by the unique identifier.</span></span>

<!-- { "blockType": "response", "truncated": true, "@odata.type": "microsoft.graph.site" } -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

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
  "suppressions": [
  ],
  "tocPath": "Sites/Get by path"
} -->

