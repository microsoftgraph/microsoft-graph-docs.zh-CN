---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: "按路径获取 SharePoint 网站"
ms.openlocfilehash: 789d4b3f24818a8bc5a06d0c6c14c0002f58f142
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/28/2017
---
# <a name="get-a-site-resource-by-path"></a><span data-ttu-id="13464-102">按路径获取 site 资源</span><span class="sxs-lookup"><span data-stu-id="13464-102">Get a site resource by path</span></span>

<span data-ttu-id="13464-p101">检索[网站][]资源的属性和关系。**网站**资源表示 SharePoint 中的团队网站。</span><span class="sxs-lookup"><span data-stu-id="13464-p101">Retrieve properties and relationships for a [site][] resource. A **site** resource represents a team site in SharePoint.</span></span>

[网站]: ../resources/site.md

<span data-ttu-id="13464-106">除了可以[按 ID 检索网站](site_get.md)外，还可以按相对服务器 URL 路径检索网站。</span><span class="sxs-lookup"><span data-stu-id="13464-106">In addition to retrieving a [site by ID](site_get.md) you can retrieve a site based on server-relative URL path.</span></span>

* <span data-ttu-id="13464-107">网站集主机名 (contoso.sharepoint.com)</span><span class="sxs-lookup"><span data-stu-id="13464-107">Site collection hostname (contoso.sharepoint.com)</span></span>
* <span data-ttu-id="13464-108">相对服务器主机名的网站路径。</span><span class="sxs-lookup"><span data-stu-id="13464-108">Site path, relative to server hostname.</span></span>

<span data-ttu-id="13464-109">还有一个保留的网站标识符，即 `root`。它经常用于引用给定目标的根网站，如下所示：</span><span class="sxs-lookup"><span data-stu-id="13464-109">There is also a reserved site identifier, `root`, which always references the root site for a given target, as follows:</span></span>

* <span data-ttu-id="13464-110">`/sites/root`：租户根网站。</span><span class="sxs-lookup"><span data-stu-id="13464-110">`/sites/root`: The tenant root site.</span></span>
* <span data-ttu-id="13464-111">`/groups/{group-id}/sites/root`：该组的团队网站。</span><span class="sxs-lookup"><span data-stu-id="13464-111">`/groups/{group-id}/sites/root`: The group's team site.</span></span>

## <a name="permissions"></a><span data-ttu-id="13464-112">权限</span><span class="sxs-lookup"><span data-stu-id="13464-112">Permissions</span></span>

<span data-ttu-id="13464-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="13464-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="13464-115">权限类型</span><span class="sxs-lookup"><span data-stu-id="13464-115">Permission type</span></span>      | <span data-ttu-id="13464-116">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="13464-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="13464-117">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="13464-117">Delegated (work or school account)</span></span> | <span data-ttu-id="13464-118">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="13464-118">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="13464-119">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="13464-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="13464-120">不支持。</span><span class="sxs-lookup"><span data-stu-id="13464-120">Not supported.</span></span>    |
|<span data-ttu-id="13464-121">应用程序</span><span class="sxs-lookup"><span data-stu-id="13464-121">Application</span></span> | <span data-ttu-id="13464-122">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="13464-122">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="13464-123">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="13464-123">HTTP Request</span></span>

<span data-ttu-id="13464-124">若要通过相对路径访问根 SharePoint 网站，请运行以下命令：</span><span class="sxs-lookup"><span data-stu-id="13464-124">To access the root SharePoint site with a relative path:</span></span>

<!-- { "blockType": "request", "name": "get-site-by-hostname-and-path", "scopes": "service.sharepoint sites.read.all" } -->

```http
GET /sites/{hostname}:/{relative-path}
```

## <a name="http-response"></a><span data-ttu-id="13464-125">HTTP 响应</span><span class="sxs-lookup"><span data-stu-id="13464-125">HTTP Response</span></span>

<span data-ttu-id="13464-126">此方法返回唯一标识符引用的网站的 [site][] 资源。</span><span class="sxs-lookup"><span data-stu-id="13464-126">This method returns a [site][] resource for the site referenced by the unique identifier.</span></span>

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
