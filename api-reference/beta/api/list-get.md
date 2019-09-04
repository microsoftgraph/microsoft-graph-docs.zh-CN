---
author: JeremyKelley
title: 获取列表的元数据
description: 返回列表的元数据。
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: c3561808ed48fdf40438c8a2d862b15401e37d5b
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/04/2019
ms.locfileid: "36726177"
---
# <a name="get-metadata-for-a-list"></a><span data-ttu-id="239de-103">获取列表的元数据</span><span class="sxs-lookup"><span data-stu-id="239de-103">Get metadata for a list</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="239de-104">返回[列表][]的元数据。</span><span class="sxs-lookup"><span data-stu-id="239de-104">Return the metadata for a [list][].</span></span>

[列表]: ../resources/list.md
[list]: ../resources/list.md

## <a name="permissions"></a><span data-ttu-id="239de-106">权限</span><span class="sxs-lookup"><span data-stu-id="239de-106">Permissions</span></span>

<span data-ttu-id="239de-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="239de-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="239de-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="239de-109">Permission type</span></span>      | <span data-ttu-id="239de-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="239de-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="239de-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="239de-111">Delegated (work or school account)</span></span> | <span data-ttu-id="239de-112">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="239de-112">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="239de-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="239de-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="239de-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="239de-114">Not supported.</span></span>    |
|<span data-ttu-id="239de-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="239de-115">Application</span></span> | <span data-ttu-id="239de-116">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="239de-116">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="239de-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="239de-117">HTTP request</span></span>

```http
GET https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}
GET https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}?expand=columns,items(expand=fields)
```

## <a name="request-body"></a><span data-ttu-id="239de-118">请求正文</span><span class="sxs-lookup"><span data-stu-id="239de-118">Request body</span></span>

<span data-ttu-id="239de-119">请勿为此方法提供请求正文。</span><span class="sxs-lookup"><span data-stu-id="239de-119">Do not supply a request body with this method.</span></span>

## <a name="example"></a><span data-ttu-id="239de-120">示例</span><span class="sxs-lookup"><span data-stu-id="239de-120">Example</span></span>

#### <a name="request"></a><span data-ttu-id="239de-121">请求</span><span class="sxs-lookup"><span data-stu-id="239de-121">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="239de-122">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="239de-122">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-list" } -->

```msgraph-interactive
GET /sites/{site-id}/lists/{list-id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="239de-123">C#</span><span class="sxs-lookup"><span data-stu-id="239de-123">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-list-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="239de-124">JavaScript</span><span class="sxs-lookup"><span data-stu-id="239de-124">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-list-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="239de-125">目标-C</span><span class="sxs-lookup"><span data-stu-id="239de-125">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-list-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="239de-126">响应</span><span class="sxs-lookup"><span data-stu-id="239de-126">Response</span></span>

<!-- { "blockType": "response", "@type": "microsoft.graph.list", "truncated": true, "scopes": "sites.read.all service.sharepoint" } -->

```json
HTTP/1.1 200 OK
Content-type: application/json

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
```

<span data-ttu-id="239de-127">借助 `select` 和 `expand` 语句，可以通过单个请求中检索列表元数据、列定义和列表项。</span><span class="sxs-lookup"><span data-stu-id="239de-127">With `select` and `expand` statements, you can retrieve list metadata, column definitions, and list items in a single request.</span></span>

#### <a name="request"></a><span data-ttu-id="239de-128">请求</span><span class="sxs-lookup"><span data-stu-id="239de-128">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="239de-129">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="239de-129">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-list-multi-expand" } -->

```msgraph-interactive
GET /sites/{site-id}/lists/{list-id}?select=name,lastModifiedDateTime&expand=columns(select=name,description),items(expand=fields(select=Name,Color,Quantity))
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="239de-130">C#</span><span class="sxs-lookup"><span data-stu-id="239de-130">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-list-multi-expand-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="239de-131">JavaScript</span><span class="sxs-lookup"><span data-stu-id="239de-131">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-list-multi-expand-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="239de-132">目标-C</span><span class="sxs-lookup"><span data-stu-id="239de-132">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-list-multi-expand-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="239de-133">响应</span><span class="sxs-lookup"><span data-stu-id="239de-133">Response</span></span>

<!-- { "blockType": "response", "@type": "microsoft.graph.list", "truncated": true, "scopes": "sites.read.all service.sharepoint" } -->

```json
HTTP/1.1 200 OK
Content-type: application/json

{
  "name": "Inventory",
  "lastModifiedDateTime": "2016-08-30T08:32:00Z",
  "columns": [
    {
      "name": "Name",
      "description": "Customer-facing name of the SKU"
    },
    {
      "name": "Color",
      "description": "Color of the item in stock"
    },
    {
      "name": "Quantity",
      "description": "Number of items in stock"
    }
  ],
  "items": [
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
#### <a name="request"></a><span data-ttu-id="239de-134">请求</span><span class="sxs-lookup"><span data-stu-id="239de-134">Request</span></span>

<!-- { "blockType": "request", "name": "get-list-multi-expand" } -->

<span data-ttu-id="239de-135">下面的示例演示如何获取包含三列的列表的元数据: 名称、数量和类别。</span><span class="sxs-lookup"><span data-stu-id="239de-135">The following example shows how to get metadata for a list that contains three columns: Name, Quantity, and Category.</span></span>
<span data-ttu-id="239de-136">[托管元数据](https://docs.microsoft.com/en-us/sharepoint/managed-metadata)列```Category``` , 如作为术语 ID 和术语名称对的返回值。</span><span class="sxs-lookup"><span data-stu-id="239de-136">[Managed Metadata](https://docs.microsoft.com/en-us/sharepoint/managed-metadata) columns like ```Category``` return values as term ID and term name pair.</span></span>
```http
GET /sites/{site-id}/lists/{list-id}?select=name,lastModifiedDateTime&expand=columns(select=name,description),items(expand=fields(select=Name,Quantity,Category))
```

#### <a name="response"></a><span data-ttu-id="239de-137">响应</span><span class="sxs-lookup"><span data-stu-id="239de-137">Response</span></span>

<!-- { "blockType": "response", "@type": "microsoft.graph.list", "truncated": true, "scopes": "sites.read.all service.sharepoint" } -->

```json
HTTP/1.1 200 OK
Content-type: application/json

{
  "name": "Inventory",
  "lastModifiedDateTime": "2016-08-30T08:32:00Z",
  "columns": [
    {
      "name": "Name",
      "description": "Customer-facing name of the SKU"
    },
    {
      "name": "Quantity",
      "description": "Number of items in stock"
    },
    {
      "name": "Category",
      "description": "Category of the item"
    }
  ],
  "items": [
    {
      "id": "2",
      "fields": {
        "Name": "Gadget",
        "Quantity": 503,
        "Category": {
          "termId": "791d537a-9c1c-3b05-97b0-1ce7ece7e1a4",
          "name": "Tool"
         }
       }
    },
    {
      "id": "4",
      "fields": {
        "Name": "Widget",
        "Quantity": 2357,
        "Category": {
          "termId": "902e568b-9b2d-4d06-87c2-2cf8ecf9f2b5" ,
          "name": "Mechanical Device"
         }
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
  "tocPath": "Lists/Get metadata",
  "suppressions": [
  ]
}
-->
