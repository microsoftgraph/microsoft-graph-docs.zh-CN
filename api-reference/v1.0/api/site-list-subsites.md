---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: 列出 SharePoint 网站的子网站
localization_priority: Priority
ms.prod: sharepoint
ms.openlocfilehash: 59cede94bbdf5c26f3082fd96c93580fbcd03b3c
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35279238"
---
# <a name="enumerate-subsites"></a><span data-ttu-id="07d41-102">枚举子网站</span><span class="sxs-lookup"><span data-stu-id="07d41-102">Enumerate subsites</span></span>

<span data-ttu-id="07d41-103">获取为 [网站][] 定义的子网站集合。</span><span class="sxs-lookup"><span data-stu-id="07d41-103">Get a collection of subsites defined for a [site][].</span></span>

[网站]: ../resources/site.md
[site]: ../resources/site.md

## <a name="permissions"></a><span data-ttu-id="07d41-105">权限</span><span class="sxs-lookup"><span data-stu-id="07d41-105">Permissions</span></span>

<span data-ttu-id="07d41-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="07d41-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="07d41-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="07d41-108">Permission type</span></span>      | <span data-ttu-id="07d41-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="07d41-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="07d41-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="07d41-110">Delegated (work or school account)</span></span> | <span data-ttu-id="07d41-111">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="07d41-111">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="07d41-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="07d41-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="07d41-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="07d41-113">Not supported.</span></span>    |
|<span data-ttu-id="07d41-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="07d41-114">Application</span></span> | <span data-ttu-id="07d41-115">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="07d41-115">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="07d41-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="07d41-116">HTTP request</span></span>

<!-- { "blockType": "request", "name": "list-subsites", "scopes": "sites.read.all", "tags": "service.sharepoint" } -->

```http
GET https://graph.microsoft.com/v1.0/sites/{site-id}/sites
```

## <a name="response"></a><span data-ttu-id="07d41-117">响应</span><span class="sxs-lookup"><span data-stu-id="07d41-117">Response</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="07d41-118">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="07d41-118">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="07d41-119">C#</span><span class="sxs-lookup"><span data-stu-id="07d41-119">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/list-subsites-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="07d41-120">Javascript</span><span class="sxs-lookup"><span data-stu-id="07d41-120">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/list-subsites-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="07d41-121">Objective-C</span><span class="sxs-lookup"><span data-stu-id="07d41-121">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/list-subsites-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Sites/List subsites",
  "suppressions": [
    "Error: /api-reference/v1.0/api/site-list-subsites.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/site-list-subsites.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/site-list-subsites.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
} -->
