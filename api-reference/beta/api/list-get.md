---
author: JeremyKelley
title: 获取列表的元数据
description: 返回列表的元数据。
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: 6225e85c751e47cd6c0e499eba2aff4e892fb3f0
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2021
ms.locfileid: "50472907"
---
# <a name="get-metadata-for-a-list"></a><span data-ttu-id="5e2b6-103">获取列表的元数据</span><span class="sxs-lookup"><span data-stu-id="5e2b6-103">Get metadata for a list</span></span>

<span data-ttu-id="5e2b6-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5e2b6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5e2b6-105">返回列表的 [元数据][]。</span><span class="sxs-lookup"><span data-stu-id="5e2b6-105">Return the metadata for a [list][].</span></span>

[list]: ../resources/list.md

## <a name="permissions"></a><span data-ttu-id="5e2b6-107">权限</span><span class="sxs-lookup"><span data-stu-id="5e2b6-107">Permissions</span></span>

<span data-ttu-id="5e2b6-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="5e2b6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="5e2b6-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="5e2b6-110">Permission type</span></span>                        | <span data-ttu-id="5e2b6-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="5e2b6-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="5e2b6-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5e2b6-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="5e2b6-113">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5e2b6-113">Sites.Read.All, Sites.ReadWrite.All</span></span>         |
| <span data-ttu-id="5e2b6-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5e2b6-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5e2b6-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="5e2b6-115">Not supported.</span></span>                              |
| <span data-ttu-id="5e2b6-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="5e2b6-116">Application</span></span>                            | <span data-ttu-id="5e2b6-117">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5e2b6-117">Sites.Read.All, Sites.ReadWrite.All</span></span>         |

## <a name="http-request"></a><span data-ttu-id="5e2b6-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5e2b6-118">HTTP request</span></span>

```http
GET https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}
GET https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-title}
GET https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}?expand=columns,items(expand=fields)
```

## <a name="request-body"></a><span data-ttu-id="5e2b6-119">请求正文</span><span class="sxs-lookup"><span data-stu-id="5e2b6-119">Request body</span></span>

<span data-ttu-id="5e2b6-120">请勿为此方法提供请求正文。</span><span class="sxs-lookup"><span data-stu-id="5e2b6-120">Do not supply a request body with this method.</span></span>

## <a name="example"></a><span data-ttu-id="5e2b6-121">示例</span><span class="sxs-lookup"><span data-stu-id="5e2b6-121">Example</span></span>

#### <a name="request"></a><span data-ttu-id="5e2b6-122">请求</span><span class="sxs-lookup"><span data-stu-id="5e2b6-122">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="5e2b6-123">HTTP</span><span class="sxs-lookup"><span data-stu-id="5e2b6-123">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-list" } -->

```msgraph-interactive
GET /sites/{site-id}/lists/{list-id}
```
# <a name="c"></a>[<span data-ttu-id="5e2b6-124">C#</span><span class="sxs-lookup"><span data-stu-id="5e2b6-124">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-list-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5e2b6-125">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5e2b6-125">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-list-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5e2b6-126">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5e2b6-126">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-list-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="5e2b6-127">Java</span><span class="sxs-lookup"><span data-stu-id="5e2b6-127">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-list-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="5e2b6-128">响应</span><span class="sxs-lookup"><span data-stu-id="5e2b6-128">Response</span></span>

<!-- { "blockType": "response", "@type": "microsoft.graph.list", "truncated": true, "scopes": "sites.read.all service.sharepoint" } -->

```http
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

<span data-ttu-id="5e2b6-129">借助 `select` 和 `expand` 语句，可以通过单个请求中检索列表元数据、列定义和列表项。</span><span class="sxs-lookup"><span data-stu-id="5e2b6-129">With `select` and `expand` statements, you can retrieve list metadata, column definitions, and list items in a single request.</span></span>

#### <a name="request"></a><span data-ttu-id="5e2b6-130">请求</span><span class="sxs-lookup"><span data-stu-id="5e2b6-130">Request</span></span>
<span data-ttu-id="5e2b6-131">下面示例演示如何从 SharePoint Online 列表标题获取列表。</span><span class="sxs-lookup"><span data-stu-id="5e2b6-131">The following example shows how to get a list from a SharePoint Online list title.</span></span>

# <a name="http"></a>[<span data-ttu-id="5e2b6-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="5e2b6-132">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-list" } -->

```msgraph-interactive
GET /sites/{site-id}/lists/{list-title}
```
# <a name="c"></a>[<span data-ttu-id="5e2b6-133">C#</span><span class="sxs-lookup"><span data-stu-id="5e2b6-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-list-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5e2b6-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5e2b6-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-list-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5e2b6-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5e2b6-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-list-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="5e2b6-136">Java</span><span class="sxs-lookup"><span data-stu-id="5e2b6-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-list-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="5e2b6-137">响应</span><span class="sxs-lookup"><span data-stu-id="5e2b6-137">Response</span></span>

<!-- { "blockType": "response", "@type": "microsoft.graph.list", "truncated": true, "scopes": "sites.read.all service.sharepoint" } -->

```http
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

<span data-ttu-id="5e2b6-138">借助 `select` 和 `expand` 语句，可以通过单个请求中检索列表元数据、列定义和列表项。</span><span class="sxs-lookup"><span data-stu-id="5e2b6-138">With `select` and `expand` statements, you can retrieve list metadata, column definitions, and list items in a single request.</span></span>

#### <a name="request"></a><span data-ttu-id="5e2b6-139">请求</span><span class="sxs-lookup"><span data-stu-id="5e2b6-139">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="5e2b6-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="5e2b6-140">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-list-multi-expand" } -->

```msgraph-interactive
GET /sites/{site-id}/lists/{list-id}?select=name,lastModifiedDateTime&expand=columns(select=name,description),items(expand=fields(select=Name,Color,Quantity))
```
# <a name="c"></a>[<span data-ttu-id="5e2b6-141">C#</span><span class="sxs-lookup"><span data-stu-id="5e2b6-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-list-multi-expand-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5e2b6-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5e2b6-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-list-multi-expand-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5e2b6-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5e2b6-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-list-multi-expand-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="5e2b6-144">Java</span><span class="sxs-lookup"><span data-stu-id="5e2b6-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-list-multi-expand-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="5e2b6-145">响应</span><span class="sxs-lookup"><span data-stu-id="5e2b6-145">Response</span></span>

<!-- { "blockType": "response", "@type": "microsoft.graph.list", "truncated": true, "scopes": "sites.read.all service.sharepoint" } -->

```http
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
#### <a name="request"></a><span data-ttu-id="5e2b6-146">请求</span><span class="sxs-lookup"><span data-stu-id="5e2b6-146">Request</span></span>

<!-- { "blockType": "request", "name": "get-list-multi-expand" } -->

<span data-ttu-id="5e2b6-147">以下示例演示如何获取包含三列的列表的元数据：名称、数量和类别。</span><span class="sxs-lookup"><span data-stu-id="5e2b6-147">The following example shows how to get metadata for a list that contains three columns: Name, Quantity, and Category.</span></span>
<span data-ttu-id="5e2b6-148">[托管元数据](/sharepoint/managed-metadata) 列， ```Category``` 如作为术语 ID 和术语名称对的返回值。</span><span class="sxs-lookup"><span data-stu-id="5e2b6-148">[Managed Metadata](/sharepoint/managed-metadata) columns like ```Category``` return values as term ID and term name pair.</span></span>
```http
GET /sites/{site-id}/lists/{list-id}?select=name,lastModifiedDateTime&expand=columns(select=name,description),items(expand=fields(select=Name,Quantity,Category))
```

#### <a name="response"></a><span data-ttu-id="5e2b6-149">响应</span><span class="sxs-lookup"><span data-stu-id="5e2b6-149">Response</span></span>

<!-- { "blockType": "response", "@type": "microsoft.graph.list", "truncated": true, "scopes": "sites.read.all service.sharepoint" } -->

```http
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


