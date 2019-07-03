---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: 从 SharePoint 列表中获取条目
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 0864650701f9f6d4ee195373b5875dfe5a86b46a
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35449160"
---
# <a name="get-an-item-in-a-list"></a><span data-ttu-id="856f0-102">获取列表中的项</span><span class="sxs-lookup"><span data-stu-id="856f0-102">Get an item in a list</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="856f0-103">返回[列表][]中某个[项][]的元数据。</span><span class="sxs-lookup"><span data-stu-id="856f0-103">Returns the metadata for an [item][] in a [list][].</span></span>

[列表]: ../resources/list.md
[list]: ../resources/list.md
[项]: ../resources/listitem.md
[item]: ../resources/listitem.md

## <a name="permissions"></a><span data-ttu-id="856f0-106">权限</span><span class="sxs-lookup"><span data-stu-id="856f0-106">Permissions</span></span>

<span data-ttu-id="856f0-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="856f0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="856f0-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="856f0-109">Permission type</span></span>      | <span data-ttu-id="856f0-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="856f0-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="856f0-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="856f0-111">Delegated (work or school account)</span></span> | <span data-ttu-id="856f0-112">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="856f0-112">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="856f0-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="856f0-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="856f0-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="856f0-114">Not supported.</span></span>    |
|<span data-ttu-id="856f0-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="856f0-115">Application</span></span> | <span data-ttu-id="856f0-116">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="856f0-116">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="856f0-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="856f0-117">HTTP request</span></span>

```http
GET https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items/{item-id}
GET https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items/{item-id}?expand=fields
GET https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items/{item-id}?expand=fields(select=Column1,Column2)
```

## <a name="example"></a><span data-ttu-id="856f0-118">示例</span><span class="sxs-lookup"><span data-stu-id="856f0-118">Example</span></span>

##### <a name="request"></a><span data-ttu-id="856f0-119">请求</span><span class="sxs-lookup"><span data-stu-id="856f0-119">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="856f0-120">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="856f0-120">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-list-item" } -->

```http
GET https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items/{item-id}?expand=fields
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="856f0-121">C#</span><span class="sxs-lookup"><span data-stu-id="856f0-121">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-list-item-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="856f0-122">Javascript</span><span class="sxs-lookup"><span data-stu-id="856f0-122">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-list-item-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="856f0-123">目标-C</span><span class="sxs-lookup"><span data-stu-id="856f0-123">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-list-item-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="856f0-124">响应</span><span class="sxs-lookup"><span data-stu-id="856f0-124">Response</span></span>

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
