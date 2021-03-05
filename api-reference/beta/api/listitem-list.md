---
author: JeremyKelley
description: 获取列表中项的集合。
ms.date: 09/11/2017
title: 检索 SharePoint 列表中的项
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: 91a6682b2fd9d9a339332982cb1a89bfca163c8c
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2021
ms.locfileid: "50475848"
---
# <a name="enumerate-items-in-a-list"></a><span data-ttu-id="4153b-103">枚举列表中的项</span><span class="sxs-lookup"><span data-stu-id="4153b-103">Enumerate items in a list</span></span>

<span data-ttu-id="4153b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4153b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4153b-105">获取[列表][]中[项][item]的集合。</span><span class="sxs-lookup"><span data-stu-id="4153b-105">Get the collection of [items][item] in a [list][].</span></span>

[list]: ../resources/list.md
[item]: ../resources/listitem.md

## <a name="permissions"></a><span data-ttu-id="4153b-107">权限</span><span class="sxs-lookup"><span data-stu-id="4153b-107">Permissions</span></span>

<span data-ttu-id="4153b-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4153b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4153b-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="4153b-110">Permission type</span></span>      | <span data-ttu-id="4153b-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="4153b-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4153b-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4153b-112">Delegated (work or school account)</span></span> | <span data-ttu-id="4153b-113">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4153b-113">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="4153b-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4153b-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4153b-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="4153b-115">Not supported.</span></span>    |
|<span data-ttu-id="4153b-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="4153b-116">Application</span></span> | <span data-ttu-id="4153b-117">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4153b-117">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4153b-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4153b-118">HTTP request</span></span>

```http
GET /sites/{site-id}/lists/{list-id}/items
GET /sites/{site-id}/lists/{list-id}/items?expand=fields
GET /sites/{site-id}/lists/{list-id}/items?expand=fields(select=Column1,Column2)
```

## <a name="example"></a><span data-ttu-id="4153b-119">示例</span><span class="sxs-lookup"><span data-stu-id="4153b-119">Example</span></span>

#### <a name="request"></a><span data-ttu-id="4153b-120">请求</span><span class="sxs-lookup"><span data-stu-id="4153b-120">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="4153b-121">HTTP</span><span class="sxs-lookup"><span data-stu-id="4153b-121">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-list-items" } -->

```msgraph-interactive
GET https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items?expand=fields(select=Name,Color,Quantity)
```
# <a name="c"></a>[<span data-ttu-id="4153b-122">C#</span><span class="sxs-lookup"><span data-stu-id="4153b-122">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-list-items-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4153b-123">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4153b-123">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-list-items-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4153b-124">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4153b-124">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-list-items-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="4153b-125">Java</span><span class="sxs-lookup"><span data-stu-id="4153b-125">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-list-items-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="4153b-126">响应</span><span class="sxs-lookup"><span data-stu-id="4153b-126">Response</span></span>

<!-- { "blockType": "response", "@odata.type": "Collection(microsoft.graph.listItem)", "truncated": true } -->

```http
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


