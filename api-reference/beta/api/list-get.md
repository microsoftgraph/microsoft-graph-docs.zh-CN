---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: 获取 SharePoint 列表
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: bb5b99b273a60ccd68622e4d4625c7afd21037be
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35449251"
---
# <a name="get-metadata-for-a-list"></a><span data-ttu-id="2fda6-102">获取列表的元数据</span><span class="sxs-lookup"><span data-stu-id="2fda6-102">Get metadata for a list</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2fda6-103">返回[列表][]的元数据。</span><span class="sxs-lookup"><span data-stu-id="2fda6-103">Returns the metadata for a [list][].</span></span>

[列表]: ../resources/list.md
[list]: ../resources/list.md

## <a name="permissions"></a><span data-ttu-id="2fda6-105">权限</span><span class="sxs-lookup"><span data-stu-id="2fda6-105">Permissions</span></span>

<span data-ttu-id="2fda6-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2fda6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2fda6-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="2fda6-108">Permission type</span></span>      | <span data-ttu-id="2fda6-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="2fda6-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2fda6-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2fda6-110">Delegated (work or school account)</span></span> | <span data-ttu-id="2fda6-111">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2fda6-111">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="2fda6-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2fda6-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2fda6-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="2fda6-113">Not supported.</span></span>    |
|<span data-ttu-id="2fda6-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="2fda6-114">Application</span></span> | <span data-ttu-id="2fda6-115">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2fda6-115">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="2fda6-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2fda6-116">HTTP request</span></span>

```http
GET https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}
GET https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}?expand=columns,items(expand=fields)
```

## <a name="request-body"></a><span data-ttu-id="2fda6-117">请求正文</span><span class="sxs-lookup"><span data-stu-id="2fda6-117">Request body</span></span>

<span data-ttu-id="2fda6-118">请勿为此方法提供请求正文。</span><span class="sxs-lookup"><span data-stu-id="2fda6-118">Do not supply a request body with this method.</span></span>

## <a name="example"></a><span data-ttu-id="2fda6-119">示例</span><span class="sxs-lookup"><span data-stu-id="2fda6-119">Example</span></span>

#### <a name="request"></a><span data-ttu-id="2fda6-120">请求</span><span class="sxs-lookup"><span data-stu-id="2fda6-120">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="2fda6-121">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="2fda6-121">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-list" } -->

```http
GET /sites/{site-id}/lists/{list-id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="2fda6-122">C#</span><span class="sxs-lookup"><span data-stu-id="2fda6-122">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-list-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="2fda6-123">Javascript</span><span class="sxs-lookup"><span data-stu-id="2fda6-123">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-list-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="2fda6-124">目标-C</span><span class="sxs-lookup"><span data-stu-id="2fda6-124">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-list-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="2fda6-125">响应</span><span class="sxs-lookup"><span data-stu-id="2fda6-125">Response</span></span>

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

<span data-ttu-id="2fda6-126">借助 `select` 和 `expand` 语句，可以通过单个请求中检索列表元数据、列定义和列表项。</span><span class="sxs-lookup"><span data-stu-id="2fda6-126">With `select` and `expand` statements, you can retrieve list metadata, column definitions, and list items in a single request.</span></span>

#### <a name="request"></a><span data-ttu-id="2fda6-127">请求</span><span class="sxs-lookup"><span data-stu-id="2fda6-127">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="2fda6-128">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="2fda6-128">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-list-multi-expand" } -->

```http
GET /sites/{site-id}/lists/{list-id}?select=name,lastModifiedDateTime&expand=columns(select=name,description),items(expand=fields(select=Name,Color,Quantity))
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="2fda6-129">C#</span><span class="sxs-lookup"><span data-stu-id="2fda6-129">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-list-multi-expand-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="2fda6-130">Javascript</span><span class="sxs-lookup"><span data-stu-id="2fda6-130">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-list-multi-expand-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="2fda6-131">目标-C</span><span class="sxs-lookup"><span data-stu-id="2fda6-131">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-list-multi-expand-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="2fda6-132">响应</span><span class="sxs-lookup"><span data-stu-id="2fda6-132">Response</span></span>

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
