---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: 列出 SharePoint 网站的子网站
localization_priority: Priority
ms.prod: sharepoint
ms.openlocfilehash: a14a44700ee3167759af6f484615494a8675cca6
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35885488"
---
# <a name="enumerate-subsites"></a><span data-ttu-id="dc4b8-102">枚举子网站</span><span class="sxs-lookup"><span data-stu-id="dc4b8-102">Enumerate subsites</span></span>

<span data-ttu-id="dc4b8-103">获取为 [网站][] 定义的子网站集合。</span><span class="sxs-lookup"><span data-stu-id="dc4b8-103">Get a collection of subsites defined for a [site][].</span></span>

[网站]: ../resources/site.md
[site]: ../resources/site.md

## <a name="permissions"></a><span data-ttu-id="dc4b8-105">权限</span><span class="sxs-lookup"><span data-stu-id="dc4b8-105">Permissions</span></span>

<span data-ttu-id="dc4b8-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="dc4b8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dc4b8-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="dc4b8-108">Permission type</span></span>      | <span data-ttu-id="dc4b8-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="dc4b8-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="dc4b8-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="dc4b8-110">Delegated (work or school account)</span></span> | <span data-ttu-id="dc4b8-111">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dc4b8-111">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="dc4b8-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="dc4b8-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dc4b8-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="dc4b8-113">Not supported.</span></span>    |
|<span data-ttu-id="dc4b8-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="dc4b8-114">Application</span></span> | <span data-ttu-id="dc4b8-115">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dc4b8-115">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="dc4b8-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="dc4b8-116">HTTP request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="dc4b8-117">HTTP</span><span class="sxs-lookup"><span data-stu-id="dc4b8-117">--Http</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "list-subsites", "scopes": "sites.read.all", "tags": "service.sharepoint" } -->

```http
GET https://graph.microsoft.com/v1.0/sites/{site-id}/sites
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="dc4b8-118">C#</span><span class="sxs-lookup"><span data-stu-id="dc4b8-118">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-subsites-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="dc4b8-119">Javascript</span><span class="sxs-lookup"><span data-stu-id="dc4b8-119">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-subsites-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="dc4b8-120">Objective-C</span><span class="sxs-lookup"><span data-stu-id="dc4b8-120">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-subsites-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="dc4b8-121">Java</span><span class="sxs-lookup"><span data-stu-id="dc4b8-121">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-subsites-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


## <a name="response"></a><span data-ttu-id="dc4b8-122">响应</span><span class="sxs-lookup"><span data-stu-id="dc4b8-122">Response</span></span>

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
  "tocPath": "Sites/List subsites",
  "suppressions": [
  ]
} -->
