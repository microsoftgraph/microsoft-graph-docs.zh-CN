---
author: JeremyKelley
description: 获取为网站定义的子网站集合。
ms.date: 09/10/2017
title: 列出 SharePoint 网站的子网站
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: 6aaed76ed3fc571d0af534943febc1decaca0f43
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42453225"
---
# <a name="enumerate-subsites"></a><span data-ttu-id="04558-103">枚举子网站</span><span class="sxs-lookup"><span data-stu-id="04558-103">Enumerate subsites</span></span>

<span data-ttu-id="04558-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="04558-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="04558-105">获取为 [网站][] 定义的子网站集合。</span><span class="sxs-lookup"><span data-stu-id="04558-105">Get a collection of subsites defined for a [site][].</span></span>

[网站]: ../resources/site.md
[site]: ../resources/site.md

## <a name="permissions"></a><span data-ttu-id="04558-107">权限</span><span class="sxs-lookup"><span data-stu-id="04558-107">Permissions</span></span>

<span data-ttu-id="04558-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="04558-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="04558-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="04558-110">Permission type</span></span>      | <span data-ttu-id="04558-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="04558-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="04558-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="04558-112">Delegated (work or school account)</span></span> | <span data-ttu-id="04558-113">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="04558-113">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="04558-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="04558-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="04558-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="04558-115">Not supported.</span></span>    |
|<span data-ttu-id="04558-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="04558-116">Application</span></span> | <span data-ttu-id="04558-117">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="04558-117">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="04558-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="04558-118">HTTP request</span></span>

```http
GET /sites/{site-id}/sites
```

# <a name="http"></a>[<span data-ttu-id="04558-119">HTTP</span><span class="sxs-lookup"><span data-stu-id="04558-119">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "list-subsites", "scopes": "service.sharepoint sites.read.all" } -->

```msgraph-interactive
GET https://graph.microsoft.com/beta/sites/{site-id}/sites
```
# <a name="c"></a>[<span data-ttu-id="04558-120">C#</span><span class="sxs-lookup"><span data-stu-id="04558-120">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-subsites-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="04558-121">JavaScript</span><span class="sxs-lookup"><span data-stu-id="04558-121">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-subsites-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="04558-122">Objective-C</span><span class="sxs-lookup"><span data-stu-id="04558-122">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-subsites-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


## <a name="response"></a><span data-ttu-id="04558-123">响应</span><span class="sxs-lookup"><span data-stu-id="04558-123">Response</span></span>

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
  ]
}
-->
