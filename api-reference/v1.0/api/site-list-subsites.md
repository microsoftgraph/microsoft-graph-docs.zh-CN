---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: 列出 SharePoint 网站的子网站
ms.openlocfilehash: a26c2f592c11760b822c80a7e37749823a5172aa
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27008718"
---
# <a name="enumerate-subsites"></a><span data-ttu-id="4ddad-102">枚举子网站</span><span class="sxs-lookup"><span data-stu-id="4ddad-102">Enumerate subsites</span></span>

<span data-ttu-id="4ddad-103">获取为 [网站][] 定义的子网站集合。</span><span class="sxs-lookup"><span data-stu-id="4ddad-103">Get a collection of subsites defined for a [site][].</span></span>

[网站]: ../resources/site.md
[site]: ../resources/site.md

## <a name="permissions"></a><span data-ttu-id="4ddad-105">权限</span><span class="sxs-lookup"><span data-stu-id="4ddad-105">Permissions</span></span>

<span data-ttu-id="4ddad-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4ddad-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4ddad-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="4ddad-108">Permission type</span></span>      | <span data-ttu-id="4ddad-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="4ddad-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4ddad-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4ddad-110">Delegated (work or school account)</span></span> | <span data-ttu-id="4ddad-111">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4ddad-111">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="4ddad-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4ddad-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4ddad-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="4ddad-113">Not supported.</span></span>    |
|<span data-ttu-id="4ddad-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="4ddad-114">Application</span></span> | <span data-ttu-id="4ddad-115">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4ddad-115">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4ddad-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4ddad-116">HTTP request</span></span>

<!-- { "blockType": "request", "name": "list-subsites", "scopes": "sites.read.all", "tags": "service.sharepoint" } -->

```http
GET https://graph.microsoft.com/v1.0/sites/{site-id}/sites
```

## <a name="response"></a><span data-ttu-id="4ddad-117">响应</span><span class="sxs-lookup"><span data-stu-id="4ddad-117">Response</span></span>

<!-- { "blockType": "response", "@type": "microsoft.graph.site", "isCollection": true, "truncated": true } -->

```json
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "contoso.sharepoint.com,da60e844-ba1d-49bc-b4d4-d5e36bae9019,712a596e-90a1-49e3-9b48-bfa80bee8740",
      "name": "Team A Subsite",
      "description": "",
      "createdDateTime": "2016-10-18T03:05:59Z",
      "lastModifiedDateTime": "2016-10-18T10:40:59Z",
      "webUrl": "https://contoso.sharepoint.com/sites/site/subsiteA"
    },
    {
      "id": "contoso.sharepoint.com,da60e844-ba1d-49bc-b4d4-d5e36bae9019,0271110f-634f-4300-a841-3a8a2e851851",
      "name": "Team B Subsite",
      "description": "",
      "createdDateTime": "2016-10-18T03:05:59Z",
      "lastModifiedDateTime": "2016-10-18T10:40:59Z",
      "webUrl": "https://contoso.sharepoint.com/sites/site/subsiteB"
    }
  ]
}
```

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Sites/List subsites"
} -->
