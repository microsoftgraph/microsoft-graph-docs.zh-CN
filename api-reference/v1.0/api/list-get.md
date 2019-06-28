---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: 获取 SharePoint 列表
localization_priority: Priority
ms.prod: sharepoint
ms.openlocfilehash: 4f623aa940ad71a593d68df1d86e4d18360277b9
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35272056"
---
# <a name="get-metadata-for-a-list"></a><span data-ttu-id="bcce2-102">获取列表的元数据</span><span class="sxs-lookup"><span data-stu-id="bcce2-102">Get metadata for a list</span></span>

<span data-ttu-id="bcce2-103">返回[列表][]的元数据。</span><span class="sxs-lookup"><span data-stu-id="bcce2-103">Returns the metadata for a [list][].</span></span>

[列表]: ../resources/list.md
[list]: ../resources/list.md

## <a name="permissions"></a><span data-ttu-id="bcce2-105">权限</span><span class="sxs-lookup"><span data-stu-id="bcce2-105">Permissions</span></span>

<span data-ttu-id="bcce2-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="bcce2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bcce2-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="bcce2-108">Permission type</span></span>      | <span data-ttu-id="bcce2-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="bcce2-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bcce2-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="bcce2-110">Delegated (work or school account)</span></span> | <span data-ttu-id="bcce2-111">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bcce2-111">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="bcce2-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="bcce2-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bcce2-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="bcce2-113">Not supported.</span></span>    |
|<span data-ttu-id="bcce2-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="bcce2-114">Application</span></span> | <span data-ttu-id="bcce2-115">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bcce2-115">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="bcce2-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="bcce2-116">HTTP request</span></span>

```http
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}?expand=columns,items(expand=fields)
```

## <a name="request-body"></a><span data-ttu-id="bcce2-117">请求正文</span><span class="sxs-lookup"><span data-stu-id="bcce2-117">Request body</span></span>

<span data-ttu-id="bcce2-118">请勿为此方法提供请求正文。</span><span class="sxs-lookup"><span data-stu-id="bcce2-118">Do not supply a request body with this method.</span></span>

## <a name="example"></a><span data-ttu-id="bcce2-119">示例</span><span class="sxs-lookup"><span data-stu-id="bcce2-119">Example</span></span>

#### <a name="request"></a><span data-ttu-id="bcce2-120">请求</span><span class="sxs-lookup"><span data-stu-id="bcce2-120">Request</span></span>

<!-- { "blockType": "request", "name": "get-list", "scopes": "sites.read.all" } -->

```http
GET /sites/{site-id}/lists/{list-id}
```

#### <a name="response"></a><span data-ttu-id="bcce2-121">响应</span><span class="sxs-lookup"><span data-stu-id="bcce2-121">Response</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="bcce2-122">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="bcce2-122">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="bcce2-123">C#</span><span class="sxs-lookup"><span data-stu-id="bcce2-123">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get-list-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="bcce2-124">Javascript</span><span class="sxs-lookup"><span data-stu-id="bcce2-124">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get-list-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="bcce2-125">Objective-C</span><span class="sxs-lookup"><span data-stu-id="bcce2-125">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get-list-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<span data-ttu-id="bcce2-126">借助 `select` 和 `expand` 语句，可以通过单个请求中检索列表元数据、列定义和列表项。</span><span class="sxs-lookup"><span data-stu-id="bcce2-126">With `select` and `expand` statements, you can retrieve list metadata, column definitions, and list items in a single request.</span></span>

#### <a name="request"></a><span data-ttu-id="bcce2-127">请求</span><span class="sxs-lookup"><span data-stu-id="bcce2-127">Request</span></span>

<!-- { "blockType": "request", "name": "get-list-multi-expand", "scopes": "sites.read.all" } -->

```http
GET /sites/{site-id}/lists/{list-id}?select=id,name,lastModifiedDateTime&expand=columns(select=name,description),items(expand=fields(select=Name,Color,Quantity))
```

#### <a name="response"></a><span data-ttu-id="bcce2-128">响应</span><span class="sxs-lookup"><span data-stu-id="bcce2-128">Response</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="bcce2-129">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="bcce2-129">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="bcce2-130">C#</span><span class="sxs-lookup"><span data-stu-id="bcce2-130">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get-list-multi-expand-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="bcce2-131">Javascript</span><span class="sxs-lookup"><span data-stu-id="bcce2-131">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get-list-multi-expand-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="bcce2-132">Objective-C</span><span class="sxs-lookup"><span data-stu-id="bcce2-132">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get-list-multi-expand-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Lists/Get metadata",
  "suppressions": [
    "Error: /api-reference/v1.0/api/list-get.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/list-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/list-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/v1.0/api/list-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/list-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
} -->
