---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: 列出 SharePoint 网站的子网站
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: f5037373ab914dabe33f11892f90a3bcfad77d5b
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32537242"
---
# <a name="enumerate-subsites"></a><span data-ttu-id="f08c7-102">枚举子网站</span><span class="sxs-lookup"><span data-stu-id="f08c7-102">Enumerate subsites</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f08c7-103">获取为 [网站][] 定义的子网站集合。</span><span class="sxs-lookup"><span data-stu-id="f08c7-103">Get a collection of subsites defined for a [site][].</span></span>

[网站]: ../resources/site.md
[site]: ../resources/site.md

## <a name="permissions"></a><span data-ttu-id="f08c7-105">权限</span><span class="sxs-lookup"><span data-stu-id="f08c7-105">Permissions</span></span>

<span data-ttu-id="f08c7-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f08c7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f08c7-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="f08c7-108">Permission type</span></span>      | <span data-ttu-id="f08c7-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f08c7-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f08c7-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f08c7-110">Delegated (work or school account)</span></span> | <span data-ttu-id="f08c7-111">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f08c7-111">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="f08c7-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f08c7-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f08c7-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="f08c7-113">Not supported.</span></span>    |
|<span data-ttu-id="f08c7-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="f08c7-114">Application</span></span> | <span data-ttu-id="f08c7-115">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f08c7-115">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f08c7-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f08c7-116">HTTP request</span></span>

<!-- { "blockType": "request", "name": "list-subsites", "scopes": "service.sharepoint sites.read.all" } -->

```http
GET https://graph.microsoft.com/beta/sites/{site-id}/sites
```

## <a name="response"></a><span data-ttu-id="f08c7-117">响应</span><span class="sxs-lookup"><span data-stu-id="f08c7-117">Response</span></span>

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

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Sites/List subsites",
  "suppressions": [
    "Error: /api-reference/beta/api/site-list-subsites.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
