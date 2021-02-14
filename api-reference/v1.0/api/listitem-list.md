---
author: JeremyKelley
ms.date: 09/11/2017
title: 检索 SharePoint 列表中的项
localization_priority: Priority
ms.prod: sharepoint
description: 获取列表中项的集合。
doc_type: apiPageType
ms.openlocfilehash: d554e92d6118fdb590f17d78d0d05ef712814546
ms.sourcegitcommit: 5b0aab5422e0619ce8806664c479479d223129ec
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/14/2021
ms.locfileid: "50238762"
---
# <a name="enumerate-items-in-a-list"></a><span data-ttu-id="96996-103">枚举列表中的项</span><span class="sxs-lookup"><span data-stu-id="96996-103">Enumerate items in a list</span></span>

<span data-ttu-id="96996-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="96996-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="96996-105">获取[列表][]中[项][item]的集合。</span><span class="sxs-lookup"><span data-stu-id="96996-105">Get the collection of [items][item] in a [list][].</span></span>

[list]: ../resources/list.md
[item]: ../resources/listitem.md

## <a name="permissions"></a><span data-ttu-id="96996-107">权限</span><span class="sxs-lookup"><span data-stu-id="96996-107">Permissions</span></span>

<span data-ttu-id="96996-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="96996-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="96996-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="96996-110">Permission type</span></span>      | <span data-ttu-id="96996-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="96996-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="96996-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="96996-112">Delegated (work or school account)</span></span> | <span data-ttu-id="96996-113">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="96996-113">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="96996-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="96996-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="96996-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="96996-115">Not supported.</span></span>    |
|<span data-ttu-id="96996-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="96996-116">Application</span></span> | <span data-ttu-id="96996-117">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="96996-117">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="96996-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="96996-118">HTTP request</span></span>

```http
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items?expand=fields
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items?expand=fields(select=Column1,Column2)
```

## <a name="example"></a><span data-ttu-id="96996-119">示例</span><span class="sxs-lookup"><span data-stu-id="96996-119">Example</span></span>

#### <a name="request"></a><span data-ttu-id="96996-120">请求</span><span class="sxs-lookup"><span data-stu-id="96996-120">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="96996-121">HTTP</span><span class="sxs-lookup"><span data-stu-id="96996-121">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-list-items", "scopes": "sites.read.all" } -->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items?expand=fields(select=Name,Color,Quantity)
```
# <a name="c"></a>[<span data-ttu-id="96996-122">C#</span><span class="sxs-lookup"><span data-stu-id="96996-122">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-list-items-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="96996-123">JavaScript</span><span class="sxs-lookup"><span data-stu-id="96996-123">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-list-items-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="96996-124">Objective-C</span><span class="sxs-lookup"><span data-stu-id="96996-124">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-list-items-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="96996-125">Java</span><span class="sxs-lookup"><span data-stu-id="96996-125">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-list-items-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="96996-126">响应</span><span class="sxs-lookup"><span data-stu-id="96996-126">Response</span></span>

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

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "ListItem/Enumerate",
  "suppressions": [
  ]
} -->

