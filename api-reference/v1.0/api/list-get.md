---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: 获取 SharePoint 列表
localization_priority: Priority
ms.prod: sharepoint
description: 返回列表的元数据。
doc_type: apiPageType
ms.openlocfilehash: 93c007a761b431131236b9c3ba66f36f071ab250
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36023172"
---
# <a name="get-metadata-for-a-list"></a><span data-ttu-id="ca7b8-103">获取列表的元数据</span><span class="sxs-lookup"><span data-stu-id="ca7b8-103">Get metadata for a list</span></span>

<span data-ttu-id="ca7b8-104">返回[列表][]的元数据。</span><span class="sxs-lookup"><span data-stu-id="ca7b8-104">Returns the metadata for a [list][].</span></span>

[列表]: ../resources/list.md
[list]: ../resources/list.md

## <a name="permissions"></a><span data-ttu-id="ca7b8-106">权限</span><span class="sxs-lookup"><span data-stu-id="ca7b8-106">Permissions</span></span>

<span data-ttu-id="ca7b8-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ca7b8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ca7b8-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="ca7b8-109">Permission type</span></span>      | <span data-ttu-id="ca7b8-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ca7b8-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ca7b8-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ca7b8-111">Delegated (work or school account)</span></span> | <span data-ttu-id="ca7b8-112">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ca7b8-112">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="ca7b8-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ca7b8-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ca7b8-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="ca7b8-114">Not supported.</span></span>    |
|<span data-ttu-id="ca7b8-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="ca7b8-115">Application</span></span> | <span data-ttu-id="ca7b8-116">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ca7b8-116">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ca7b8-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ca7b8-117">HTTP request</span></span>

```http
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}?expand=columns,items(expand=fields)
```

## <a name="request-body"></a><span data-ttu-id="ca7b8-118">请求正文</span><span class="sxs-lookup"><span data-stu-id="ca7b8-118">Request body</span></span>

<span data-ttu-id="ca7b8-119">请勿为此方法提供请求正文。</span><span class="sxs-lookup"><span data-stu-id="ca7b8-119">Do not supply a request body with this method.</span></span>

## <a name="example"></a><span data-ttu-id="ca7b8-120">示例</span><span class="sxs-lookup"><span data-stu-id="ca7b8-120">Example</span></span>

#### <a name="request"></a><span data-ttu-id="ca7b8-121">请求</span><span class="sxs-lookup"><span data-stu-id="ca7b8-121">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="ca7b8-122">HTTP</span><span class="sxs-lookup"><span data-stu-id="ca7b8-122">--Http</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-list", "scopes": "sites.read.all" } -->

```http
GET /sites/{site-id}/lists/{list-id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="ca7b8-123">C#</span><span class="sxs-lookup"><span data-stu-id="ca7b8-123">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-list-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="ca7b8-124">Javascript</span><span class="sxs-lookup"><span data-stu-id="ca7b8-124">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-list-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="ca7b8-125">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ca7b8-125">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-list-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="ca7b8-126">Java</span><span class="sxs-lookup"><span data-stu-id="ca7b8-126">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-list-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="ca7b8-127">响应</span><span class="sxs-lookup"><span data-stu-id="ca7b8-127">Response</span></span>

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

<span data-ttu-id="ca7b8-128">借助 `select` 和 `expand` 语句，可以通过单个请求中检索列表元数据、列定义和列表项。</span><span class="sxs-lookup"><span data-stu-id="ca7b8-128">With `select` and `expand` statements, you can retrieve list metadata, column definitions, and list items in a single request.</span></span>

#### <a name="request"></a><span data-ttu-id="ca7b8-129">请求</span><span class="sxs-lookup"><span data-stu-id="ca7b8-129">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="ca7b8-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="ca7b8-130">--Http</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-list-multi-expand", "scopes": "sites.read.all" } -->

```http
GET /sites/{site-id}/lists/{list-id}?select=id,name,lastModifiedDateTime&expand=columns(select=name,description),items(expand=fields(select=Name,Color,Quantity))
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="ca7b8-131">C#</span><span class="sxs-lookup"><span data-stu-id="ca7b8-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-list-multi-expand-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="ca7b8-132">Javascript</span><span class="sxs-lookup"><span data-stu-id="ca7b8-132">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-list-multi-expand-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="ca7b8-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ca7b8-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-list-multi-expand-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="ca7b8-134">Java</span><span class="sxs-lookup"><span data-stu-id="ca7b8-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-list-multi-expand-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="ca7b8-135">响应</span><span class="sxs-lookup"><span data-stu-id="ca7b8-135">Response</span></span>

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
