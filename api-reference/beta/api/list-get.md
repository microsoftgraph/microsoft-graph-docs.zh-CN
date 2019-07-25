---
author: JeremyKelley
title: 获取列表的元数据
description: 返回 [列表] [] 的元数据。
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: b60b5b1d6190738d133a030c96149688fc9fc88b
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35880343"
---
# <a name="get-metadata-for-a-list"></a><span data-ttu-id="770bf-103">获取列表的元数据</span><span class="sxs-lookup"><span data-stu-id="770bf-103">Get metadata for a list</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="770bf-104">返回[列表][]的元数据。</span><span class="sxs-lookup"><span data-stu-id="770bf-104">Return the metadata for a [list][].</span></span>

[列表]: ../resources/list.md
[list]: ../resources/list.md

## <a name="permissions"></a><span data-ttu-id="770bf-106">权限</span><span class="sxs-lookup"><span data-stu-id="770bf-106">Permissions</span></span>

<span data-ttu-id="770bf-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="770bf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="770bf-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="770bf-109">Permission type</span></span>      | <span data-ttu-id="770bf-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="770bf-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="770bf-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="770bf-111">Delegated (work or school account)</span></span> | <span data-ttu-id="770bf-112">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="770bf-112">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="770bf-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="770bf-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="770bf-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="770bf-114">Not supported.</span></span>    |
|<span data-ttu-id="770bf-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="770bf-115">Application</span></span> | <span data-ttu-id="770bf-116">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="770bf-116">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="770bf-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="770bf-117">HTTP request</span></span>

```http
GET https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}
GET https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}?expand=columns,items(expand=fields)
```

## <a name="request-body"></a><span data-ttu-id="770bf-118">请求正文</span><span class="sxs-lookup"><span data-stu-id="770bf-118">Request body</span></span>

<span data-ttu-id="770bf-119">请勿为此方法提供请求正文。</span><span class="sxs-lookup"><span data-stu-id="770bf-119">Do not supply a request body with this method.</span></span>

## <a name="example"></a><span data-ttu-id="770bf-120">示例</span><span class="sxs-lookup"><span data-stu-id="770bf-120">Example</span></span>

#### <a name="request"></a><span data-ttu-id="770bf-121">请求</span><span class="sxs-lookup"><span data-stu-id="770bf-121">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="770bf-122">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="770bf-122">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-list" } -->

```http
GET /sites/{site-id}/lists/{list-id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="770bf-123">C#</span><span class="sxs-lookup"><span data-stu-id="770bf-123">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-list-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="770bf-124">Javascript</span><span class="sxs-lookup"><span data-stu-id="770bf-124">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-list-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="770bf-125">目标-C</span><span class="sxs-lookup"><span data-stu-id="770bf-125">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-list-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="770bf-126">Java</span><span class="sxs-lookup"><span data-stu-id="770bf-126">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-list-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="770bf-127">响应</span><span class="sxs-lookup"><span data-stu-id="770bf-127">Response</span></span>

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

<span data-ttu-id="770bf-128">借助 `select` 和 `expand` 语句，可以通过单个请求中检索列表元数据、列定义和列表项。</span><span class="sxs-lookup"><span data-stu-id="770bf-128">With `select` and `expand` statements, you can retrieve list metadata, column definitions, and list items in a single request.</span></span>

#### <a name="request"></a><span data-ttu-id="770bf-129">请求</span><span class="sxs-lookup"><span data-stu-id="770bf-129">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="770bf-130">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="770bf-130">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-list-multi-expand" } -->

```http
GET /sites/{site-id}/lists/{list-id}?select=name,lastModifiedDateTime&expand=columns(select=name,description),items(expand=fields(select=Name,Color,Quantity))
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="770bf-131">C#</span><span class="sxs-lookup"><span data-stu-id="770bf-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-list-multi-expand-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="770bf-132">Javascript</span><span class="sxs-lookup"><span data-stu-id="770bf-132">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-list-multi-expand-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="770bf-133">目标-C</span><span class="sxs-lookup"><span data-stu-id="770bf-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-list-multi-expand-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="770bf-134">Java</span><span class="sxs-lookup"><span data-stu-id="770bf-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-list-multi-expand-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="770bf-135">响应</span><span class="sxs-lookup"><span data-stu-id="770bf-135">Response</span></span>

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
#### <a name="request"></a><span data-ttu-id="770bf-136">请求</span><span class="sxs-lookup"><span data-stu-id="770bf-136">Request</span></span>

<!-- { "blockType": "request", "name": "get-list-multi-expand" } -->

<span data-ttu-id="770bf-137">下面的示例演示如何获取包含三列的列表的元数据: 名称、数量和类别。</span><span class="sxs-lookup"><span data-stu-id="770bf-137">The following example shows how to get metadata for a list that contains three columns: Name, Quantity, and Category.</span></span>
<span data-ttu-id="770bf-138">[托管元数据](https://docs.microsoft.com/en-us/sharepoint/managed-metadata)列```Category``` , 如作为术语 ID 和术语名称对的返回值。</span><span class="sxs-lookup"><span data-stu-id="770bf-138">[Managed Metadata](https://docs.microsoft.com/en-us/sharepoint/managed-metadata) columns like ```Category``` return values as term ID and term name pair.</span></span>
```http
GET /sites/{site-id}/lists/{list-id}?select=name,lastModifiedDateTime&expand=columns(select=name,description),items(expand=fields(select=Name,Quantity,Category))
```

#### <a name="response"></a><span data-ttu-id="770bf-139">响应</span><span class="sxs-lookup"><span data-stu-id="770bf-139">Response</span></span>

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
