---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: 按路径获取 SharePoint 网站
localization_priority: Normal
ms.prod: sharepoint
description: 检索网站资源的属性和关系。
doc_type: apiPageType
ms.openlocfilehash: 5e6195ddb90578d31d4cf68f081aafebbd004e24
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36021471"
---
# <a name="get-a-site-resource-by-path"></a><span data-ttu-id="b8a89-103">按路径获取网站资源</span><span class="sxs-lookup"><span data-stu-id="b8a89-103">Get a site resource by path</span></span>

<span data-ttu-id="b8a89-p101">检索[网站][]资源的属性和关系。**网站**资源表示 SharePoint 中的团队网站。</span><span class="sxs-lookup"><span data-stu-id="b8a89-p101">Retrieve properties and relationships for a [site][] resource. A **site** resource represents a team site in SharePoint.</span></span>

[网站]: ../resources/site.md
[site]: ../resources/site.md

<span data-ttu-id="b8a89-107">除了可以[按 ID 检索网站](site-get.md)外，还可以按相对服务器 URL 路径检索网站。</span><span class="sxs-lookup"><span data-stu-id="b8a89-107">In addition to retrieving a [site by ID](site-get.md) you can retrieve a site based on server-relative URL path.</span></span>

* <span data-ttu-id="b8a89-108">网站集主机名 (contoso.sharepoint.com)</span><span class="sxs-lookup"><span data-stu-id="b8a89-108">Site collection hostname (contoso.sharepoint.com)</span></span>
* <span data-ttu-id="b8a89-109">相对服务器主机名的网站路径。</span><span class="sxs-lookup"><span data-stu-id="b8a89-109">Site path, relative to server hostname.</span></span>

<span data-ttu-id="b8a89-110">还有一个保留的网站标识符，即 `root`。它经常用于引用给定目标的根网站，如下所示：</span><span class="sxs-lookup"><span data-stu-id="b8a89-110">There is also a reserved site identifier, `root`, which always references the root site for a given target, as follows:</span></span>

* <span data-ttu-id="b8a89-111">`/sites/root`：租户根网站。</span><span class="sxs-lookup"><span data-stu-id="b8a89-111">`/sites/root`: The tenant root site.</span></span>
* <span data-ttu-id="b8a89-112">`/groups/{group-id}/sites/root`：该组的团队网站。</span><span class="sxs-lookup"><span data-stu-id="b8a89-112">`/groups/{group-id}/sites/root`: The group's team site.</span></span>

## <a name="permissions"></a><span data-ttu-id="b8a89-113">权限</span><span class="sxs-lookup"><span data-stu-id="b8a89-113">Permissions</span></span>

<span data-ttu-id="b8a89-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b8a89-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b8a89-116">权限类型</span><span class="sxs-lookup"><span data-stu-id="b8a89-116">Permission type</span></span>      | <span data-ttu-id="b8a89-117">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b8a89-117">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b8a89-118">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b8a89-118">Delegated (work or school account)</span></span> | <span data-ttu-id="b8a89-119">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b8a89-119">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="b8a89-120">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b8a89-120">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b8a89-121">不支持。</span><span class="sxs-lookup"><span data-stu-id="b8a89-121">Not supported.</span></span>    |
|<span data-ttu-id="b8a89-122">应用程序</span><span class="sxs-lookup"><span data-stu-id="b8a89-122">Application</span></span> | <span data-ttu-id="b8a89-123">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b8a89-123">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b8a89-124">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b8a89-124">HTTP Request</span></span>

<span data-ttu-id="b8a89-125">若要通过相对路径访问根 SharePoint 网站，请运行以下命令：</span><span class="sxs-lookup"><span data-stu-id="b8a89-125">To access the root SharePoint site with a relative path:</span></span>

<!-- { "blockType": "request", "name": "get-site-by-hostname-and-path", "scopes": "sites.read.all", "tags": "service.sharepoint" } -->

```http
GET /sites/{hostname}:/{relative-path}
```

## <a name="response"></a><span data-ttu-id="b8a89-126">响应</span><span class="sxs-lookup"><span data-stu-id="b8a89-126">Response</span></span>

<span data-ttu-id="b8a89-127">此方法返回唯一标识符引用的网站的 [site][] 资源。</span><span class="sxs-lookup"><span data-stu-id="b8a89-127">This method returns a [site][] resource for the site referenced by the unique identifier.</span></span>

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
    "Warning: Couldn't serialize request for path /sites/{var}/children/{var} into EDMX: System.InvalidOperationException: Uri path requires navigating into unknown object hierarchy: missing property 'children' on 'site'. Possible issues:
         1) Doc bug where 'children' isn't defined on the resource.      2) Doc bug where 'children' is an example key and should instead be replaced with a placeholder like {item-id} or declared in the sampleKeys annotation.       3) Doc bug where 'site' is supposed to be an entity type, but is being treated as a complex because it (and its ancestors) are missing the keyProperty annotation
     at ApiDocs.Publishing.CSDL.CsdlWriter.ParseRequestTargetType(String requestPath, MethodCollection requestMethodCollection, EntityFramework edmx, IssueLogger issues) in D:/src/mds2/ApiDocs.Publishing/CSDL/CsdlWriter.cs:line 982
     at ApiDocs.Publishing.CSDL.CsdlWriter.ProcessRestRequestPaths(EntityFramework edmx, String[] baseUrlsToRemove, IssueLogger issues) in D:/src/mds2/ApiDocs.Publishing/CSDL/CsdlWriter.cs:line 653"
  ],
  "tocPath": "Sites/Get by path"
} -->
