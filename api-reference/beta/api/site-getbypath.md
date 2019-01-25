---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: 按路径获取 SharePoint 网站
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: c81e025f8cee7acfc4eb9761d2168c200d0d4d5a
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29508802"
---
# <a name="get-a-site-resource-by-path"></a><span data-ttu-id="e48bd-102">按路径获取 site 资源</span><span class="sxs-lookup"><span data-stu-id="e48bd-102">Get a site resource by path</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e48bd-p101">检索[网站][]资源的属性和关系。**网站**资源表示 SharePoint 中的团队网站。</span><span class="sxs-lookup"><span data-stu-id="e48bd-p101">Retrieve properties and relationships for a [site][] resource. A **site** resource represents a team site in SharePoint.</span></span>

[site]: ../resources/site.md

<span data-ttu-id="e48bd-106">除了可以[按 ID 检索网站](site-get.md)外，还可以按相对服务器 URL 路径检索网站。</span><span class="sxs-lookup"><span data-stu-id="e48bd-106">In addition to retrieving a [site by ID](site-get.md) you can retrieve a site based on server-relative URL path.</span></span>

* <span data-ttu-id="e48bd-107">网站集主机名 (contoso.sharepoint.com)</span><span class="sxs-lookup"><span data-stu-id="e48bd-107">Site collection hostname (contoso.sharepoint.com)</span></span>
* <span data-ttu-id="e48bd-108">相对服务器主机名的网站路径。</span><span class="sxs-lookup"><span data-stu-id="e48bd-108">Site path, relative to server hostname.</span></span>

<span data-ttu-id="e48bd-109">还有一个保留的网站标识符，即 `root`。它经常用于引用给定目标的根网站，如下所示：</span><span class="sxs-lookup"><span data-stu-id="e48bd-109">There is also a reserved site identifier, `root`, which always references the root site for a given target, as follows:</span></span>

* <span data-ttu-id="e48bd-110">`/sites/root`：租户根网站。</span><span class="sxs-lookup"><span data-stu-id="e48bd-110">`/sites/root`: The tenant root site.</span></span>
* <span data-ttu-id="e48bd-111">`/groups/{group-id}/sites/root`：该组的团队网站。</span><span class="sxs-lookup"><span data-stu-id="e48bd-111">`/groups/{group-id}/sites/root`: The group's team site.</span></span>

## <a name="permissions"></a><span data-ttu-id="e48bd-112">权限</span><span class="sxs-lookup"><span data-stu-id="e48bd-112">Permissions</span></span>

<span data-ttu-id="e48bd-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e48bd-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e48bd-115">权限类型</span><span class="sxs-lookup"><span data-stu-id="e48bd-115">Permission type</span></span>      | <span data-ttu-id="e48bd-116">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e48bd-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e48bd-117">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e48bd-117">Delegated (work or school account)</span></span> | <span data-ttu-id="e48bd-118">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e48bd-118">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="e48bd-119">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e48bd-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e48bd-120">不支持。</span><span class="sxs-lookup"><span data-stu-id="e48bd-120">Not supported.</span></span>    |
|<span data-ttu-id="e48bd-121">应用程序</span><span class="sxs-lookup"><span data-stu-id="e48bd-121">Application</span></span> | <span data-ttu-id="e48bd-122">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e48bd-122">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e48bd-123">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e48bd-123">HTTP Request</span></span>

<span data-ttu-id="e48bd-124">若要通过相对路径访问根 SharePoint 网站，请运行以下命令：</span><span class="sxs-lookup"><span data-stu-id="e48bd-124">To access the root SharePoint site with a relative path:</span></span>

<!-- { "blockType": "request", "name": "get-site-by-hostname-and-path", "scopes": "service.sharepoint sites.read.all" } -->

```http
GET /sites/{hostname}:/{relative-path}
```

## <a name="response"></a><span data-ttu-id="e48bd-125">响应</span><span class="sxs-lookup"><span data-stu-id="e48bd-125">Response</span></span>

<span data-ttu-id="e48bd-126">此方法返回唯一标识符引用的网站的 [网站][] 资源。</span><span class="sxs-lookup"><span data-stu-id="e48bd-126">This method returns a [site][] resource for the site referenced by the unique identifier.</span></span>

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

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Sites/Get by path",
  "suppressions": [
    "Error: /api-reference/beta/api/site-getbypath.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
