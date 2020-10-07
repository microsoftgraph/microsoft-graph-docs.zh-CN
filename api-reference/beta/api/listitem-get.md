---
author: JeremyKelley
description: 返回列表中某个项的元数据。
ms.date: 09/11/2017
title: 从 SharePoint 列表中获取条目
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: 25d0a055840055c822814799346136a6bda6c660
ms.sourcegitcommit: c20276369a8834a259f24038e7ee5c33de02660b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/07/2020
ms.locfileid: "48373564"
---
# <a name="get-an-item-in-a-list"></a><span data-ttu-id="3c83c-103">获取列表中的项</span><span class="sxs-lookup"><span data-stu-id="3c83c-103">Get an item in a list</span></span>

<span data-ttu-id="3c83c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3c83c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3c83c-105">返回[列表][]中某个[项][]的元数据。</span><span class="sxs-lookup"><span data-stu-id="3c83c-105">Returns the metadata for an [item][] in a [list][].</span></span>

[列表]: ../resources/list.md
[list]: ../resources/list.md
[项]: ../resources/listitem.md
[item]: ../resources/listitem.md

## <a name="permissions"></a><span data-ttu-id="3c83c-108">权限</span><span class="sxs-lookup"><span data-stu-id="3c83c-108">Permissions</span></span>

<span data-ttu-id="3c83c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="3c83c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3c83c-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="3c83c-111">Permission type</span></span>      | <span data-ttu-id="3c83c-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="3c83c-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3c83c-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3c83c-113">Delegated (work or school account)</span></span> | <span data-ttu-id="3c83c-114">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3c83c-114">Sites.Read.All, Sites.ReadWrite.All</span></span> |
|<span data-ttu-id="3c83c-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3c83c-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3c83c-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="3c83c-116">Not supported.</span></span>    |
|<span data-ttu-id="3c83c-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="3c83c-117">Application</span></span> | <span data-ttu-id="3c83c-118">"全部"、"全部"、"站点"、"所有"。</span><span class="sxs-lookup"><span data-stu-id="3c83c-118">Sites.Read.All, Sites.ReadWrite.All, Sites.Manage.All</span></span> |

> <span data-ttu-id="3c83c-119">**注意**：应用程序权限网站。如果 SharePoint 列表启用了内容审批设置，则必须进行管理。</span><span class="sxs-lookup"><span data-stu-id="3c83c-119">**Note**: The application permission Sites.Manage.All is required if the SharePoint list has content approval settings turned on.</span></span> <span data-ttu-id="3c83c-120">否则，Microsoft Graph 将不会检索审批状态不是 "已批准" 的列表项。</span><span class="sxs-lookup"><span data-stu-id="3c83c-120">Otherwise, Microsoft Graph won't retrieve list items that have an approval status other than Approved.</span></span>

## <a name="http-request"></a><span data-ttu-id="3c83c-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3c83c-121">HTTP request</span></span>

```http
GET /sites/{site-id}/lists/{list-id}/items/{item-id}
GET /sites/{site-id}/lists/{list-id}/items/{item-id}?expand=fields
GET /sites/{site-id}/lists/{list-id}/items/{item-id}?expand=fields(select=Column1,Column2)
```

## <a name="example"></a><span data-ttu-id="3c83c-122">示例</span><span class="sxs-lookup"><span data-stu-id="3c83c-122">Example</span></span>

##### <a name="request"></a><span data-ttu-id="3c83c-123">请求</span><span class="sxs-lookup"><span data-stu-id="3c83c-123">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="3c83c-124">HTTP</span><span class="sxs-lookup"><span data-stu-id="3c83c-124">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-list-item" } -->

```msgraph-interactive
GET https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items/{item-id}?expand=fields
```
# <a name="c"></a>[<span data-ttu-id="3c83c-125">C#</span><span class="sxs-lookup"><span data-stu-id="3c83c-125">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-list-item-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3c83c-126">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3c83c-126">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-list-item-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3c83c-127">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3c83c-127">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-list-item-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="3c83c-128">响应</span><span class="sxs-lookup"><span data-stu-id="3c83c-128">Response</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.listItem", "truncated": true } -->

```json
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "d14922d8-43e6-4c8a-b029-e35c5b4e0d63",
  "listItemId": 2,
  "fields": {
    "Name": "Widget",
    "Color": "Blue",
    "Quantity": 2357
    }
}
```

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "ListItem/Get metadata",
  "suppressions": [
  ]
}
-->


