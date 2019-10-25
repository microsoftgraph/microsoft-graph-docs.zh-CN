---
author: JeremyKelley
description: 获取列表中项的集合。
ms.date: 09/11/2017
title: 检索 SharePoint 列表中的项
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: 1cd2bdf856f89068708ac670c239b6d27fd7ded2
ms.sourcegitcommit: bbef506636bce5b72351ee3834123771c301b1b1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/25/2019
ms.locfileid: "37726297"
---
# <a name="enumerate-items-in-a-list"></a><span data-ttu-id="24cc1-103">枚举列表中的项</span><span class="sxs-lookup"><span data-stu-id="24cc1-103">Enumerate items in a list</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="24cc1-104">获取[列表][]中[项][item]的集合。</span><span class="sxs-lookup"><span data-stu-id="24cc1-104">Get the collection of [items][item] in a [list][].</span></span>

[list]: ../resources/list.md
[item]: ../resources/listitem.md

## <a name="permissions"></a><span data-ttu-id="24cc1-106">权限</span><span class="sxs-lookup"><span data-stu-id="24cc1-106">Permissions</span></span>

<span data-ttu-id="24cc1-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="24cc1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="24cc1-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="24cc1-109">Permission type</span></span>      | <span data-ttu-id="24cc1-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="24cc1-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="24cc1-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="24cc1-111">Delegated (work or school account)</span></span> | <span data-ttu-id="24cc1-112">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="24cc1-112">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="24cc1-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="24cc1-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="24cc1-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="24cc1-114">Not supported.</span></span>    |
|<span data-ttu-id="24cc1-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="24cc1-115">Application</span></span> | <span data-ttu-id="24cc1-116">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="24cc1-116">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="24cc1-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="24cc1-117">HTTP request</span></span>

```http
GET /sites/{site-id}/lists/{list-id}/items
GET /sites/{site-id}/lists/{list-id}/items?expand=fields
GET /sites/{site-id}/lists/{list-id}/items?expand=fields(select=Column1,Column2)
```

## <a name="example"></a><span data-ttu-id="24cc1-118">示例</span><span class="sxs-lookup"><span data-stu-id="24cc1-118">Example</span></span>

#### <a name="request"></a><span data-ttu-id="24cc1-119">请求</span><span class="sxs-lookup"><span data-stu-id="24cc1-119">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="24cc1-120">HTTP</span><span class="sxs-lookup"><span data-stu-id="24cc1-120">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-list-items" } -->

```msgraph-interactive
GET https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items?expand=fields(select=Name,Color,Quantity)
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="24cc1-121">C#</span><span class="sxs-lookup"><span data-stu-id="24cc1-121">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-list-items-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="24cc1-122">JavaScript</span><span class="sxs-lookup"><span data-stu-id="24cc1-122">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-list-items-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="24cc1-123">Objective-C</span><span class="sxs-lookup"><span data-stu-id="24cc1-123">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-list-items-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="24cc1-124">响应</span><span class="sxs-lookup"><span data-stu-id="24cc1-124">Response</span></span>

<!-- { "blockType": "response", "@odata.type": "Collection(microsoft.graph.listItem)", "truncated": true } -->

```json
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "2",
      "fields": {
        "Name": "Gadget",
        "Color": "Red",
        "Quantity": 503
       }
    },
    {
      "id": "4",
      "fields": {
        "Name": "Widget",
        "Color": "Blue",
        "Quantity": 2357
       }
    },
    {
      "id": "7",
      "fields": {
        "Name": "Gizmo",
        "Color": "Green",
        "Quantity": 92
       }
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
  "tocPath": "ListItem/Enumerate",
  "suppressions": [
  ]
}
-->
