---
author: JeremyKelley
description: 返回列表中某个项的元数据。
ms.date: 09/11/2017
title: 从 SharePoint 列表中获取条目
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: 32d3fe8c2aecedb31c50fd3ea805cabd2e63dca7
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36347099"
---
# <a name="get-an-item-in-a-list"></a><span data-ttu-id="037e8-103">获取列表中的项</span><span class="sxs-lookup"><span data-stu-id="037e8-103">Get an item in a list</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="037e8-104">返回[列表][]中某个[项][]的元数据。</span><span class="sxs-lookup"><span data-stu-id="037e8-104">Returns the metadata for an [item][] in a [list][].</span></span>

[列表]: ../resources/list.md
[list]: ../resources/list.md
[项]: ../resources/listitem.md
[item]: ../resources/listitem.md

## <a name="permissions"></a><span data-ttu-id="037e8-107">权限</span><span class="sxs-lookup"><span data-stu-id="037e8-107">Permissions</span></span>

<span data-ttu-id="037e8-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="037e8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="037e8-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="037e8-110">Permission type</span></span>      | <span data-ttu-id="037e8-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="037e8-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="037e8-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="037e8-112">Delegated (work or school account)</span></span> | <span data-ttu-id="037e8-113">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="037e8-113">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="037e8-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="037e8-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="037e8-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="037e8-115">Not supported.</span></span>    |
|<span data-ttu-id="037e8-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="037e8-116">Application</span></span> | <span data-ttu-id="037e8-117">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="037e8-117">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="037e8-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="037e8-118">HTTP request</span></span>

```http
GET https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items/{item-id}
GET https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items/{item-id}?expand=fields
GET https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items/{item-id}?expand=fields(select=Column1,Column2)
```

## <a name="example"></a><span data-ttu-id="037e8-119">示例</span><span class="sxs-lookup"><span data-stu-id="037e8-119">Example</span></span>

##### <a name="request"></a><span data-ttu-id="037e8-120">请求</span><span class="sxs-lookup"><span data-stu-id="037e8-120">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="037e8-121">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="037e8-121">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-list-item" } -->

```http
GET https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items/{item-id}?expand=fields
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="037e8-122">C#</span><span class="sxs-lookup"><span data-stu-id="037e8-122">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-list-item-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="037e8-123">JavaScript</span><span class="sxs-lookup"><span data-stu-id="037e8-123">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-list-item-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="037e8-124">目标-C</span><span class="sxs-lookup"><span data-stu-id="037e8-124">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-list-item-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="037e8-125">Java</span><span class="sxs-lookup"><span data-stu-id="037e8-125">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-list-item-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="037e8-126">响应</span><span class="sxs-lookup"><span data-stu-id="037e8-126">Response</span></span>

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
