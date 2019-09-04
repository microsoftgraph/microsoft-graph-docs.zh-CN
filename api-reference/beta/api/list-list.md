---
author: JeremyKelley
description: 获取 site 的 lists 的集合。
ms.date: 09/11/2017
title: 列出网站中的 SharePoint 列表
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: 8175f3c30f481c937529879932a8cb60799184ca
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/04/2019
ms.locfileid: "36724006"
---
# <a name="enumerate-lists-in-a-site"></a><span data-ttu-id="262c1-103">枚举网站中的列表</span><span class="sxs-lookup"><span data-stu-id="262c1-103">Enumerate lists in a site</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="262c1-104">获取 [site][] 的 [lists][] 的集合。</span><span class="sxs-lookup"><span data-stu-id="262c1-104">Get the collection of [lists][] for a [site][].</span></span>

[lists]: ../resources/list.md
[site]: ../resources/site.md

## <a name="permissions"></a><span data-ttu-id="262c1-107">权限</span><span class="sxs-lookup"><span data-stu-id="262c1-107">Permissions</span></span>

<span data-ttu-id="262c1-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="262c1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="262c1-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="262c1-110">Permission type</span></span>      | <span data-ttu-id="262c1-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="262c1-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="262c1-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="262c1-112">Delegated (work or school account)</span></span> | <span data-ttu-id="262c1-113">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="262c1-113">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="262c1-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="262c1-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="262c1-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="262c1-115">Not supported.</span></span>    |
|<span data-ttu-id="262c1-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="262c1-116">Application</span></span> | <span data-ttu-id="262c1-117">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="262c1-117">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="262c1-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="262c1-118">HTTP request</span></span>

```http
GET https://graph.microsoft.com/beta/sites/{site-id}/lists
```

## <a name="example"></a><span data-ttu-id="262c1-119">示例</span><span class="sxs-lookup"><span data-stu-id="262c1-119">Example</span></span>

#### <a name="request"></a><span data-ttu-id="262c1-120">请求</span><span class="sxs-lookup"><span data-stu-id="262c1-120">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="262c1-121">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="262c1-121">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "enum-lists", "scopes": "sites.read.all service.sharepoint" } -->

```msgraph-interactive
GET https://graph.microsoft.com/beta/sites/{site-id}/lists
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="262c1-122">C#</span><span class="sxs-lookup"><span data-stu-id="262c1-122">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/enum-lists-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="262c1-123">JavaScript</span><span class="sxs-lookup"><span data-stu-id="262c1-123">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/enum-lists-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="262c1-124">目标-C</span><span class="sxs-lookup"><span data-stu-id="262c1-124">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/enum-lists-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="262c1-125">响应</span><span class="sxs-lookup"><span data-stu-id="262c1-125">Response</span></span>

<!-- { "blockType": "response", "@type": "microsoft.graph.list", "isCollection": true, "truncated": true } -->

```json
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "b57af081-936c-4803-a120-d94887b03864",
      "name": "Documents",
      "createdDateTime": "2016-08-30T08:32:00Z",
      "lastModifiedDateTime": "2016-08-30T08:32:00Z",
      "list": {
        "hidden": false,
        "template": "documentLibrary"
       }
    },
    {
      "id": "1234-112-112-4",
      "name": "MicroFeed",
      "createdDateTime": "2016-08-30T08:32:00Z",
      "lastModifiedDateTime": "2016-08-30T08:32:00Z",
      "list": {
        "hidden": false,
        "template": "genericList"
       }
    }
  ]
}
```

## <a name="remarks"></a><span data-ttu-id="262c1-126">注解</span><span class="sxs-lookup"><span data-stu-id="262c1-126">Remarks</span></span>

<span data-ttu-id="262c1-127">默认情况下，将隐藏包含 [system][] Facet 的列表。</span><span class="sxs-lookup"><span data-stu-id="262c1-127">Lists with the [system][] facet are hidden by default.</span></span>
<span data-ttu-id="262c1-128">若要列出它们，请在 `$select` 语句中添加 `system`。</span><span class="sxs-lookup"><span data-stu-id="262c1-128">To list them, include `system` in your `$select` statement.</span></span>

[system]: ../resources/systemfacet.md

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Lists/Enumerate",
  "suppressions": [
  ]
}
-->
