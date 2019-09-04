---
author: JeremyKelley
description: 返回列表中某个项的元数据。
ms.date: 09/11/2017
title: 从 SharePoint 列表中获取条目
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: b86348b7c1648a7246a9414a2f8d96e694692fd2
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/04/2019
ms.locfileid: "36726163"
---
# <a name="get-an-item-in-a-list"></a><span data-ttu-id="59226-103">获取列表中的项</span><span class="sxs-lookup"><span data-stu-id="59226-103">Get an item in a list</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="59226-104">返回[列表][]中某个[项][]的元数据。</span><span class="sxs-lookup"><span data-stu-id="59226-104">Returns the metadata for an [item][] in a [list][].</span></span>

[列表]: ../resources/list.md
[list]: ../resources/list.md
[项]: ../resources/listitem.md
[item]: ../resources/listitem.md

## <a name="permissions"></a><span data-ttu-id="59226-107">权限</span><span class="sxs-lookup"><span data-stu-id="59226-107">Permissions</span></span>

<span data-ttu-id="59226-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="59226-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="59226-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="59226-110">Permission type</span></span>      | <span data-ttu-id="59226-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="59226-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="59226-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="59226-112">Delegated (work or school account)</span></span> | <span data-ttu-id="59226-113">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="59226-113">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="59226-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="59226-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="59226-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="59226-115">Not supported.</span></span>    |
|<span data-ttu-id="59226-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="59226-116">Application</span></span> | <span data-ttu-id="59226-117">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="59226-117">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="59226-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="59226-118">HTTP request</span></span>

```http
GET https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items/{item-id}
GET https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items/{item-id}?expand=fields
GET https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items/{item-id}?expand=fields(select=Column1,Column2)
```

## <a name="example"></a><span data-ttu-id="59226-119">示例</span><span class="sxs-lookup"><span data-stu-id="59226-119">Example</span></span>

##### <a name="request"></a><span data-ttu-id="59226-120">请求</span><span class="sxs-lookup"><span data-stu-id="59226-120">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="59226-121">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="59226-121">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-list-item" } -->

```msgraph-interactive
GET https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items/{item-id}?expand=fields
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="59226-122">C#</span><span class="sxs-lookup"><span data-stu-id="59226-122">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-list-item-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="59226-123">JavaScript</span><span class="sxs-lookup"><span data-stu-id="59226-123">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-list-item-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="59226-124">目标-C</span><span class="sxs-lookup"><span data-stu-id="59226-124">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-list-item-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="59226-125">响应</span><span class="sxs-lookup"><span data-stu-id="59226-125">Response</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.listItem", "truncated": true } -->

```json
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "d14922d8-43e6-4c8a-b029-e35c5b4e0d63",
  "listItemId": 2,
  "fields": {
    "Name": "Widget",
    "Color": "Blue",
    "Quantity": 2357
    }
}
```

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "ListItem/Get metadata",
  "suppressions": [
  ]
}
-->
