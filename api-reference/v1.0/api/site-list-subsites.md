---
author: JeremyKelley
ms.date: 09/10/2017
title: 列出 SharePoint 网站的子网站
localization_priority: Priority
ms.prod: sharepoint
description: 获取为网站定义的子网站集合。
doc_type: apiPageType
ms.openlocfilehash: 8032f070f54ac8945444d70fe7fc189de7ddf983
ms.sourcegitcommit: 5b0aab5422e0619ce8806664c479479d223129ec
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/14/2021
ms.locfileid: "50238489"
---
# <a name="enumerate-subsites"></a><span data-ttu-id="0d6eb-103">枚举子网站</span><span class="sxs-lookup"><span data-stu-id="0d6eb-103">Enumerate subsites</span></span>

<span data-ttu-id="0d6eb-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0d6eb-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="0d6eb-105">获取为 [网站][] 定义的子网站集合。</span><span class="sxs-lookup"><span data-stu-id="0d6eb-105">Get a collection of subsites defined for a [site][].</span></span>

[网站]: ../resources/site.md
[site]: ../resources/site.md

## <a name="permissions"></a><span data-ttu-id="0d6eb-107">权限</span><span class="sxs-lookup"><span data-stu-id="0d6eb-107">Permissions</span></span>

<span data-ttu-id="0d6eb-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0d6eb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0d6eb-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="0d6eb-110">Permission type</span></span>      | <span data-ttu-id="0d6eb-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="0d6eb-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0d6eb-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0d6eb-112">Delegated (work or school account)</span></span> | <span data-ttu-id="0d6eb-113">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0d6eb-113">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="0d6eb-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0d6eb-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0d6eb-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="0d6eb-115">Not supported.</span></span>    |
|<span data-ttu-id="0d6eb-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="0d6eb-116">Application</span></span> | <span data-ttu-id="0d6eb-117">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0d6eb-117">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="0d6eb-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0d6eb-118">HTTP request</span></span>


# <a name="http"></a>[<span data-ttu-id="0d6eb-119">HTTP</span><span class="sxs-lookup"><span data-stu-id="0d6eb-119">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "list-subsites", "scopes": "sites.read.all", "tags": "service.sharepoint" } -->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/sites/{site-id}/sites
```
# <a name="c"></a>[<span data-ttu-id="0d6eb-120">C#</span><span class="sxs-lookup"><span data-stu-id="0d6eb-120">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-subsites-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0d6eb-121">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0d6eb-121">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-subsites-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0d6eb-122">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0d6eb-122">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-subsites-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="0d6eb-123">Java</span><span class="sxs-lookup"><span data-stu-id="0d6eb-123">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-subsites-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


## <a name="response"></a><span data-ttu-id="0d6eb-124">响应</span><span class="sxs-lookup"><span data-stu-id="0d6eb-124">Response</span></span>

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

