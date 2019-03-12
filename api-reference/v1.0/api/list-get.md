---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: 获取 SharePoint 列表
localization_priority: Priority
ms.prod: sharepoint
ms.openlocfilehash: 9e667055b47568d712349c6725bd4ebc70aa63fd
ms.sourcegitcommit: b877a8dc9aeaf74f975ca495b401ffff001d7699
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2019
ms.locfileid: "30482348"
---
# <a name="get-metadata-for-a-list"></a><span data-ttu-id="5a7a6-102">获取列表的元数据</span><span class="sxs-lookup"><span data-stu-id="5a7a6-102">Get metadata for a list</span></span>

<span data-ttu-id="5a7a6-103">返回[列表][]的元数据。</span><span class="sxs-lookup"><span data-stu-id="5a7a6-103">Returns the metadata for a [list][].</span></span>

[列表]: ../resources/list.md
[list]: ../resources/list.md

## <a name="permissions"></a><span data-ttu-id="5a7a6-105">权限</span><span class="sxs-lookup"><span data-stu-id="5a7a6-105">Permissions</span></span>

<span data-ttu-id="5a7a6-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="5a7a6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5a7a6-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="5a7a6-108">Permission type</span></span>      | <span data-ttu-id="5a7a6-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="5a7a6-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5a7a6-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5a7a6-110">Delegated (work or school account)</span></span> | <span data-ttu-id="5a7a6-111">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5a7a6-111">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="5a7a6-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5a7a6-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5a7a6-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="5a7a6-113">Not supported.</span></span>    |
|<span data-ttu-id="5a7a6-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="5a7a6-114">Application</span></span> | <span data-ttu-id="5a7a6-115">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5a7a6-115">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="5a7a6-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5a7a6-116">HTTP request</span></span>

```http
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}?expand=columns,items(expand=fields)
```

## <a name="request-body"></a><span data-ttu-id="5a7a6-117">请求正文</span><span class="sxs-lookup"><span data-stu-id="5a7a6-117">Request body</span></span>

<span data-ttu-id="5a7a6-118">请勿为此方法提供请求正文。</span><span class="sxs-lookup"><span data-stu-id="5a7a6-118">Do not supply a request body with this method.</span></span>

## <a name="example"></a><span data-ttu-id="5a7a6-119">示例</span><span class="sxs-lookup"><span data-stu-id="5a7a6-119">Example</span></span>

#### <a name="request"></a><span data-ttu-id="5a7a6-120">请求</span><span class="sxs-lookup"><span data-stu-id="5a7a6-120">Request</span></span>

<!-- { "blockType": "request", "name": "get-list", "scopes": "sites.read.all" } -->

```http
GET /sites/{site-id}/lists/{list-id}
```

#### <a name="response"></a><span data-ttu-id="5a7a6-121">响应</span><span class="sxs-lookup"><span data-stu-id="5a7a6-121">Response</span></span>

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

<span data-ttu-id="5a7a6-122">借助 `select` 和 `expand` 语句，可以通过单个请求中检索列表元数据、列定义和列表项。</span><span class="sxs-lookup"><span data-stu-id="5a7a6-122">With `select` and `expand` statements, you can retrieve list metadata, column definitions, and list items in a single request.</span></span>

#### <a name="request"></a><span data-ttu-id="5a7a6-123">请求</span><span class="sxs-lookup"><span data-stu-id="5a7a6-123">Request</span></span>

<!-- { "blockType": "request", "name": "get-list-multi-expand", "scopes": "sites.read.all" } -->

```http
GET /sites/{site-id}/lists/{list-id}?select=id,name,lastModifiedDateTime&expand=columns(select=name,description),items(expand=fields(select=Name,Color,Quantity))
```

#### <a name="response"></a><span data-ttu-id="5a7a6-124">响应</span><span class="sxs-lookup"><span data-stu-id="5a7a6-124">Response</span></span>

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
  "tocPath": "Lists/Get metadata"
} -->
