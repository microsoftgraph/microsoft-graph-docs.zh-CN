---
author: JeremyKelley
ms.author: JeremyKelley
title: 获取 SharePoint 列表
localization_priority: Priority
ms.prod: sharepoint
description: 返回列表的元数据。
doc_type: apiPageType
ms.openlocfilehash: 5739c4cf84bd308c113f88a0bbacbaf28aff7214
ms.sourcegitcommit: 53a57f19a5b16029b540e61ddfba6c2b4e45cfc5
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/06/2020
ms.locfileid: "44593651"
---
# <a name="get-metadata-for-a-list"></a><span data-ttu-id="c958b-103">获取列表的元数据</span><span class="sxs-lookup"><span data-stu-id="c958b-103">Get metadata for a list</span></span>

<span data-ttu-id="c958b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c958b-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="c958b-105">返回[列表][]的元数据。</span><span class="sxs-lookup"><span data-stu-id="c958b-105">Returns the metadata for a [list][].</span></span>

[列表]: ../resources/list.md
[list]: ../resources/list.md

## <a name="permissions"></a><span data-ttu-id="c958b-107">权限</span><span class="sxs-lookup"><span data-stu-id="c958b-107">Permissions</span></span>

<span data-ttu-id="c958b-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c958b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="c958b-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="c958b-110">Permission type</span></span>                        | <span data-ttu-id="c958b-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c958b-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="c958b-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c958b-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="c958b-113">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c958b-113">Sites.Read.All, Sites.ReadWrite.All</span></span>         |
| <span data-ttu-id="c958b-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c958b-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c958b-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="c958b-115">Not supported.</span></span>                              |
| <span data-ttu-id="c958b-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="c958b-116">Application</span></span>                            | <span data-ttu-id="c958b-117">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c958b-117">Sites.Read.All, Sites.ReadWrite.All</span></span>         |

## <a name="http-request"></a><span data-ttu-id="c958b-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c958b-118">HTTP request</span></span>

```http
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-title}
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}?expand=columns,items(expand=fields)
```

## <a name="request-body"></a><span data-ttu-id="c958b-119">请求正文</span><span class="sxs-lookup"><span data-stu-id="c958b-119">Request body</span></span>

<span data-ttu-id="c958b-120">请勿为此方法提供请求正文。</span><span class="sxs-lookup"><span data-stu-id="c958b-120">Do not supply a request body with this method.</span></span>

## <a name="example"></a><span data-ttu-id="c958b-121">示例</span><span class="sxs-lookup"><span data-stu-id="c958b-121">Example</span></span>

#### <a name="request"></a><span data-ttu-id="c958b-122">请求</span><span class="sxs-lookup"><span data-stu-id="c958b-122">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="c958b-123">HTTP</span><span class="sxs-lookup"><span data-stu-id="c958b-123">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-list", "scopes": "sites.read.all" } -->

```msgraph-interactive
GET /sites/{site-id}/lists/{list-id}
```
# <a name="c"></a>[<span data-ttu-id="c958b-124">C#</span><span class="sxs-lookup"><span data-stu-id="c958b-124">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-list-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c958b-125">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c958b-125">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-list-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c958b-126">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c958b-126">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-list-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c958b-127">Java</span><span class="sxs-lookup"><span data-stu-id="c958b-127">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-list-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="c958b-128">响应</span><span class="sxs-lookup"><span data-stu-id="c958b-128">Response</span></span>

<!-- { "blockType": "response", "@type": "microsoft.graph.list", "truncated": true, "scopes": "sites.read.all", "tags": "service.sharepoint" } -->

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

<span data-ttu-id="c958b-129">借助 `select` 和 `expand` 语句，可以通过单个请求中检索列表元数据、列定义和列表项。</span><span class="sxs-lookup"><span data-stu-id="c958b-129">With `select` and `expand` statements, you can retrieve list metadata, column definitions, and list items in a single request.</span></span>

#### <a name="request"></a><span data-ttu-id="c958b-130">请求</span><span class="sxs-lookup"><span data-stu-id="c958b-130">Request</span></span>
<span data-ttu-id="c958b-131">下面示例演示如何从 SharePoint Online 列表标题获取列表。</span><span class="sxs-lookup"><span data-stu-id="c958b-131">The following example shows how to get a list from a SharePoint Online list title.</span></span>

# <a name="http"></a>[<span data-ttu-id="c958b-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="c958b-132">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-list", "scopes": "sites.read.all" } -->

```msgraph-interactive
GET /sites/{site-id}/lists/{list-title}
```
# <a name="c"></a>[<span data-ttu-id="c958b-133">C#</span><span class="sxs-lookup"><span data-stu-id="c958b-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-list-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c958b-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c958b-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-list-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c958b-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c958b-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-list-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c958b-136">Java</span><span class="sxs-lookup"><span data-stu-id="c958b-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-list-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="c958b-137">响应</span><span class="sxs-lookup"><span data-stu-id="c958b-137">Response</span></span>

<!-- { "blockType": "response", "@type": "microsoft.graph.list", "truncated": true, "scopes": "sites.read.all", "tags": "service.sharepoint" } -->

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

<span data-ttu-id="c958b-138">借助 `select` 和 `expand` 语句，可以通过单个请求中检索列表元数据、列定义和列表项。</span><span class="sxs-lookup"><span data-stu-id="c958b-138">With `select` and `expand` statements, you can retrieve list metadata, column definitions, and list items in a single request.</span></span>

#### <a name="request"></a><span data-ttu-id="c958b-139">请求</span><span class="sxs-lookup"><span data-stu-id="c958b-139">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="c958b-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="c958b-140">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-list-multi-expand", "scopes": "sites.read.all" } -->

```msgraph-interactive
GET /sites/{site-id}/lists/{list-id}?select=id,name,lastModifiedDateTime&expand=columns(select=name,description),items(expand=fields(select=Name,Color,Quantity))
```
# <a name="c"></a>[<span data-ttu-id="c958b-141">C#</span><span class="sxs-lookup"><span data-stu-id="c958b-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-list-multi-expand-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c958b-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c958b-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-list-multi-expand-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c958b-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c958b-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-list-multi-expand-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c958b-144">Java</span><span class="sxs-lookup"><span data-stu-id="c958b-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-list-multi-expand-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="c958b-145">响应</span><span class="sxs-lookup"><span data-stu-id="c958b-145">Response</span></span>

<!-- { "blockType": "response", "@type": "microsoft.graph.list", "truncated": true, "scopes": "sites.read.all", "tags": "service.sharepoint" } -->

```json
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "1234-112-112-4",
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

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Lists/Get metadata",
  "suppressions": [
  ]
} -->
