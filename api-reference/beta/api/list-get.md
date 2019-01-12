---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: 获取 SharePoint 列表
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: f9744ec25d852359246e84c83ba3bd1dec92ff17
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27927952"
---
# <a name="get-metadata-for-a-list"></a><span data-ttu-id="f07c5-102">获取列表的元数据</span><span class="sxs-lookup"><span data-stu-id="f07c5-102">Get metadata for a list</span></span>

> <span data-ttu-id="f07c5-103">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="f07c5-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f07c5-104">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="f07c5-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f07c5-105">返回[列表][]的元数据。</span><span class="sxs-lookup"><span data-stu-id="f07c5-105">Returns the metadata for a [list][].</span></span>

[列表]: ../resources/list.md
[list]: ../resources/list.md

## <a name="permissions"></a><span data-ttu-id="f07c5-107">权限</span><span class="sxs-lookup"><span data-stu-id="f07c5-107">Permissions</span></span>

<span data-ttu-id="f07c5-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f07c5-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f07c5-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="f07c5-110">Permission type</span></span>      | <span data-ttu-id="f07c5-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f07c5-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f07c5-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f07c5-112">Delegated (work or school account)</span></span> | <span data-ttu-id="f07c5-113">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f07c5-113">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="f07c5-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f07c5-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f07c5-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="f07c5-115">Not supported.</span></span>    |
|<span data-ttu-id="f07c5-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="f07c5-116">Application</span></span> | <span data-ttu-id="f07c5-117">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f07c5-117">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f07c5-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f07c5-118">HTTP request</span></span>

```http
GET https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}
GET https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}?expand=columns,items(expand=fields)
```

## <a name="request-body"></a><span data-ttu-id="f07c5-119">请求正文</span><span class="sxs-lookup"><span data-stu-id="f07c5-119">Request body</span></span>

<span data-ttu-id="f07c5-120">请勿为此方法提供请求正文。</span><span class="sxs-lookup"><span data-stu-id="f07c5-120">Do not supply a request body with this method.</span></span>

## <a name="example"></a><span data-ttu-id="f07c5-121">示例</span><span class="sxs-lookup"><span data-stu-id="f07c5-121">Example</span></span>

#### <a name="request"></a><span data-ttu-id="f07c5-122">请求</span><span class="sxs-lookup"><span data-stu-id="f07c5-122">Request</span></span>

<!-- { "blockType": "request", "name": "get-list" } -->

```http
GET /sites/{site-id}/lists/{list-id}
```

#### <a name="response"></a><span data-ttu-id="f07c5-123">响应</span><span class="sxs-lookup"><span data-stu-id="f07c5-123">Response</span></span>

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

<span data-ttu-id="f07c5-124">借助 `select` 和 `expand` 语句，可以通过单个请求中检索列表元数据、列定义和列表项。</span><span class="sxs-lookup"><span data-stu-id="f07c5-124">With `select` and `expand` statements, you can retrieve list metadata, column definitions, and list items in a single request.</span></span>

#### <a name="request"></a><span data-ttu-id="f07c5-125">请求</span><span class="sxs-lookup"><span data-stu-id="f07c5-125">Request</span></span>

<!-- { "blockType": "request", "name": "get-list-multi-expand" } -->

```http
GET /sites/{site-id}/lists/{list-id}?select=name,lastModifiedDateTime&expand=columns(select=name,description),items(expand=fields(select=Name,Color,Quantity))
```

#### <a name="response"></a><span data-ttu-id="f07c5-126">响应</span><span class="sxs-lookup"><span data-stu-id="f07c5-126">Response</span></span>

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

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Lists/Get metadata"
} -->
