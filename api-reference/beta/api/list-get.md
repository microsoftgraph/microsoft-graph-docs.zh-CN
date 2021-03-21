---
author: JeremyKelley
title: 获取列表的元数据
description: 返回列表的元数据。
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: 5091e8de36ff357b00a9b2517fab968f4a99cd41
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50958020"
---
# <a name="get-metadata-for-a-list"></a><span data-ttu-id="9cb2f-103">获取列表的元数据</span><span class="sxs-lookup"><span data-stu-id="9cb2f-103">Get metadata for a list</span></span>

<span data-ttu-id="9cb2f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9cb2f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9cb2f-105">返回列表的 [元数据][]。</span><span class="sxs-lookup"><span data-stu-id="9cb2f-105">Return the metadata for a [list][].</span></span>

[列表]: ../resources/list.md
[list]: ../resources/list.md

## <a name="permissions"></a><span data-ttu-id="9cb2f-107">权限</span><span class="sxs-lookup"><span data-stu-id="9cb2f-107">Permissions</span></span>

<span data-ttu-id="9cb2f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9cb2f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="9cb2f-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="9cb2f-110">Permission type</span></span>                        | <span data-ttu-id="9cb2f-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="9cb2f-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="9cb2f-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9cb2f-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="9cb2f-113">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9cb2f-113">Sites.Read.All, Sites.ReadWrite.All</span></span>         |
| <span data-ttu-id="9cb2f-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9cb2f-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9cb2f-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="9cb2f-115">Not supported.</span></span>                              |
| <span data-ttu-id="9cb2f-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="9cb2f-116">Application</span></span>                            | <span data-ttu-id="9cb2f-117">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9cb2f-117">Sites.Read.All, Sites.ReadWrite.All</span></span>         |

## <a name="http-request"></a><span data-ttu-id="9cb2f-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9cb2f-118">HTTP request</span></span>

```http
GET https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}
GET https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-title}
GET https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}?expand=columns,items(expand=fields)
```

## <a name="request-body"></a><span data-ttu-id="9cb2f-119">请求正文</span><span class="sxs-lookup"><span data-stu-id="9cb2f-119">Request body</span></span>

<span data-ttu-id="9cb2f-120">请勿为此方法提供请求正文。</span><span class="sxs-lookup"><span data-stu-id="9cb2f-120">Do not supply a request body with this method.</span></span>

## <a name="example"></a><span data-ttu-id="9cb2f-121">示例</span><span class="sxs-lookup"><span data-stu-id="9cb2f-121">Example</span></span>

#### <a name="request"></a><span data-ttu-id="9cb2f-122">请求</span><span class="sxs-lookup"><span data-stu-id="9cb2f-122">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="9cb2f-123">HTTP</span><span class="sxs-lookup"><span data-stu-id="9cb2f-123">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-list-1" } -->

```msgraph-interactive
GET /sites/{site-id}/lists/{list-id}
```
# <a name="c"></a>[<span data-ttu-id="9cb2f-124">C#</span><span class="sxs-lookup"><span data-stu-id="9cb2f-124">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-list-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9cb2f-125">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9cb2f-125">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-list-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9cb2f-126">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9cb2f-126">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-list-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="9cb2f-127">Java</span><span class="sxs-lookup"><span data-stu-id="9cb2f-127">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-list-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="9cb2f-128">响应</span><span class="sxs-lookup"><span data-stu-id="9cb2f-128">Response</span></span>

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

<span data-ttu-id="9cb2f-129">借助 `select` 和 `expand` 语句，可以通过单个请求中检索列表元数据、列定义和列表项。</span><span class="sxs-lookup"><span data-stu-id="9cb2f-129">With `select` and `expand` statements, you can retrieve list metadata, column definitions, and list items in a single request.</span></span>

#### <a name="request"></a><span data-ttu-id="9cb2f-130">请求</span><span class="sxs-lookup"><span data-stu-id="9cb2f-130">Request</span></span>
<span data-ttu-id="9cb2f-131">下面示例演示如何从 SharePoint Online 列表标题获取列表。</span><span class="sxs-lookup"><span data-stu-id="9cb2f-131">The following example shows how to get a list from a SharePoint Online list title.</span></span>

# <a name="http"></a>[<span data-ttu-id="9cb2f-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="9cb2f-132">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-list-2" } -->

```msgraph-interactive
GET /sites/{site-id}/lists/{list-title}
```
# <a name="c"></a>[<span data-ttu-id="9cb2f-133">C#</span><span class="sxs-lookup"><span data-stu-id="9cb2f-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-list-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9cb2f-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9cb2f-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-list-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9cb2f-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9cb2f-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-list-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="9cb2f-136">Java</span><span class="sxs-lookup"><span data-stu-id="9cb2f-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-list-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="9cb2f-137">响应</span><span class="sxs-lookup"><span data-stu-id="9cb2f-137">Response</span></span>

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

<span data-ttu-id="9cb2f-138">借助 `select` 和 `expand` 语句，可以通过单个请求中检索列表元数据、列定义和列表项。</span><span class="sxs-lookup"><span data-stu-id="9cb2f-138">With `select` and `expand` statements, you can retrieve list metadata, column definitions, and list items in a single request.</span></span>

#### <a name="request"></a><span data-ttu-id="9cb2f-139">请求</span><span class="sxs-lookup"><span data-stu-id="9cb2f-139">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="9cb2f-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="9cb2f-140">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-list-multi-expand" } -->

```msgraph-interactive
GET /sites/{site-id}/lists/{list-id}?select=name,lastModifiedDateTime&expand=columns(select=name,description),items(expand=fields(select=Name,Color,Quantity))
```
# <a name="c"></a>[<span data-ttu-id="9cb2f-141">C#</span><span class="sxs-lookup"><span data-stu-id="9cb2f-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-list-multi-expand-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9cb2f-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9cb2f-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-list-multi-expand-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9cb2f-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9cb2f-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-list-multi-expand-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="9cb2f-144">Java</span><span class="sxs-lookup"><span data-stu-id="9cb2f-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-list-multi-expand-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="9cb2f-145">响应</span><span class="sxs-lookup"><span data-stu-id="9cb2f-145">Response</span></span>

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
#### <a name="request"></a><span data-ttu-id="9cb2f-146">请求</span><span class="sxs-lookup"><span data-stu-id="9cb2f-146">Request</span></span>

<!-- { "blockType": "request", "name": "get-list-multi-expand" } -->

<span data-ttu-id="9cb2f-147">以下示例演示如何获取包含三列的列表的元数据：名称、数量和类别。</span><span class="sxs-lookup"><span data-stu-id="9cb2f-147">The following example shows how to get metadata for a list that contains three columns: Name, Quantity, and Category.</span></span>
<span data-ttu-id="9cb2f-148">[托管元数据](/sharepoint/managed-metadata) 列， ```Category``` 如作为术语 ID 和术语名称对的返回值。</span><span class="sxs-lookup"><span data-stu-id="9cb2f-148">[Managed Metadata](/sharepoint/managed-metadata) columns like ```Category``` return values as term ID and term name pair.</span></span>
```http
GET /sites/{site-id}/lists/{list-id}?select=name,lastModifiedDateTime&expand=columns(select=name,description),items(expand=fields(select=Name,Quantity,Category))
```

#### <a name="response"></a><span data-ttu-id="9cb2f-149">响应</span><span class="sxs-lookup"><span data-stu-id="9cb2f-149">Response</span></span>

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


