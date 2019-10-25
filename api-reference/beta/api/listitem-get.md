---
author: JeremyKelley
description: 返回列表中某个项的元数据。
ms.date: 09/11/2017
title: 从 SharePoint 列表中获取条目
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: 537785e9f9dcb6f8c991d0564dc7be1fbc4d06b7
ms.sourcegitcommit: bbef506636bce5b72351ee3834123771c301b1b1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/25/2019
ms.locfileid: "37726301"
---
# <a name="get-an-item-in-a-list"></a><span data-ttu-id="078bd-103">获取列表中的项</span><span class="sxs-lookup"><span data-stu-id="078bd-103">Get an item in a list</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="078bd-104">返回[列表][]中某个[项][]的元数据。</span><span class="sxs-lookup"><span data-stu-id="078bd-104">Returns the metadata for an [item][] in a [list][].</span></span>

[列表]: ../resources/list.md
[list]: ../resources/list.md
[项]: ../resources/listitem.md
[item]: ../resources/listitem.md

## <a name="permissions"></a><span data-ttu-id="078bd-107">权限</span><span class="sxs-lookup"><span data-stu-id="078bd-107">Permissions</span></span>

<span data-ttu-id="078bd-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="078bd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="078bd-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="078bd-110">Permission type</span></span>      | <span data-ttu-id="078bd-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="078bd-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="078bd-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="078bd-112">Delegated (work or school account)</span></span> | <span data-ttu-id="078bd-113">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="078bd-113">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="078bd-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="078bd-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="078bd-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="078bd-115">Not supported.</span></span>    |
|<span data-ttu-id="078bd-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="078bd-116">Application</span></span> | <span data-ttu-id="078bd-117">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="078bd-117">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="078bd-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="078bd-118">HTTP request</span></span>

```http
GET /sites/{site-id}/lists/{list-id}/items/{item-id}
GET /sites/{site-id}/lists/{list-id}/items/{item-id}?expand=fields
GET /sites/{site-id}/lists/{list-id}/items/{item-id}?expand=fields(select=Column1,Column2)
```

## <a name="example"></a><span data-ttu-id="078bd-119">示例</span><span class="sxs-lookup"><span data-stu-id="078bd-119">Example</span></span>

##### <a name="request"></a><span data-ttu-id="078bd-120">请求</span><span class="sxs-lookup"><span data-stu-id="078bd-120">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="078bd-121">HTTP</span><span class="sxs-lookup"><span data-stu-id="078bd-121">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-list-item" } -->

```msgraph-interactive
GET https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items/{item-id}?expand=fields
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="078bd-122">C#</span><span class="sxs-lookup"><span data-stu-id="078bd-122">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-list-item-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="078bd-123">JavaScript</span><span class="sxs-lookup"><span data-stu-id="078bd-123">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-list-item-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="078bd-124">Objective-C</span><span class="sxs-lookup"><span data-stu-id="078bd-124">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-list-item-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="078bd-125">响应</span><span class="sxs-lookup"><span data-stu-id="078bd-125">Response</span></span>

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
