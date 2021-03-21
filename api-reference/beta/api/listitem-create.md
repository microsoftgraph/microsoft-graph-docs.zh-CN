---
author: JeremyKelley
description: 在列表中创建新的 listItem。
ms.date: 09/11/2017
title: 在 SharePoint 列表中创建新条目
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: e1d99d99fd29599853c214eda82ceddb49af24fc
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50957959"
---
# <a name="create-a-new-item-in-a-list"></a><span data-ttu-id="00dbb-103">在列表中创建新项</span><span class="sxs-lookup"><span data-stu-id="00dbb-103">Create a new item in a list</span></span>

<span data-ttu-id="00dbb-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="00dbb-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="00dbb-105">在[列表][]中创建新的 [listItem][]。</span><span class="sxs-lookup"><span data-stu-id="00dbb-105">Create a new [listItem][] in a [list][].</span></span>

## <a name="permissions"></a><span data-ttu-id="00dbb-106">权限</span><span class="sxs-lookup"><span data-stu-id="00dbb-106">Permissions</span></span>

<span data-ttu-id="00dbb-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="00dbb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="00dbb-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="00dbb-109">Permission type</span></span>      | <span data-ttu-id="00dbb-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="00dbb-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="00dbb-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="00dbb-111">Delegated (work or school account)</span></span> | <span data-ttu-id="00dbb-112">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="00dbb-112">Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="00dbb-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="00dbb-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="00dbb-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="00dbb-114">Not supported.</span></span>    |
|<span data-ttu-id="00dbb-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="00dbb-115">Application</span></span> | <span data-ttu-id="00dbb-116">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="00dbb-116">Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="00dbb-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="00dbb-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /sites/{site-id}/lists/{list-id}/items
```

## <a name="request-body"></a><span data-ttu-id="00dbb-118">请求正文</span><span class="sxs-lookup"><span data-stu-id="00dbb-118">Request body</span></span>

<span data-ttu-id="00dbb-119">在请求正文中，提供要创建的 [listItem][] 资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="00dbb-119">In the request body, supply a JSON representation of the [listItem][] resource to create.</span></span>

## <a name="example"></a><span data-ttu-id="00dbb-120">示例</span><span class="sxs-lookup"><span data-stu-id="00dbb-120">Example</span></span>

<span data-ttu-id="00dbb-121">下面的示例展示了如何创建新的泛型列表项。</span><span class="sxs-lookup"><span data-stu-id="00dbb-121">Here is an example of how to create a new generic list item.</span></span>


# <a name="http"></a>[<span data-ttu-id="00dbb-122">HTTP</span><span class="sxs-lookup"><span data-stu-id="00dbb-122">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "create-listitem-1", "scopes": "sites.readwrite.all" } -->

```http
POST https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items
Content-Type: application/json

{
  "fields": {
    "Title": "Widget",
    "Color": "Purple",
    "Weight": 32
  }
}
```
# <a name="c"></a>[<span data-ttu-id="00dbb-123">C#</span><span class="sxs-lookup"><span data-stu-id="00dbb-123">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-listitem-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="00dbb-124">JavaScript</span><span class="sxs-lookup"><span data-stu-id="00dbb-124">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-listitem-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="00dbb-125">Objective-C</span><span class="sxs-lookup"><span data-stu-id="00dbb-125">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-listitem-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


## <a name="response"></a><span data-ttu-id="00dbb-126">响应</span><span class="sxs-lookup"><span data-stu-id="00dbb-126">Response</span></span>

<span data-ttu-id="00dbb-127">如果成功，此方法在已创建列表项的响应正文中返回 [listItem][]。</span><span class="sxs-lookup"><span data-stu-id="00dbb-127">If successful, this method returns a [listItem][] in the response body for the created list item.</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.listItem", "truncated": true } -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "id": "20",
  "createdDateTime": "2016-08-30T08:26:00Z",
  "createdBy": {
    "user": {
      "displayName": "Ryan Gregg",
      "id": "8606e4d5-d582-4f5f-aeba-7d7c18b20cfd"
    }
  },
  "lastModifiedDateTime": "2016-08-30T08:26:00Z",
  "lastModifiedBy": {
    "user": {
      "displayName": "Ryan Gregg",
      "id": "8606e4d5-d582-4f5f-aeba-7d7c18b20cfd"
    }
  }
}
```

<span data-ttu-id="00dbb-128">**注意：** 为清楚起见，将截断 Response 对象。</span><span class="sxs-lookup"><span data-stu-id="00dbb-128">**Note:** The response object is truncated for clarity.</span></span> <span data-ttu-id="00dbb-129">实际调用会返回默认属性。</span><span class="sxs-lookup"><span data-stu-id="00dbb-129">Default properties will be returned from the actual call.</span></span>

[列表]: ../resources/list.md
[list]: ../resources/list.md
[listItem]: ../resources/listitem.md

<!--
{
  "type": "#page.annotation",
  "description": "Add a new item to a SharePoint list.",
  "keywords": "",
  "section": "documentation",
  "tocPath": "ListItem/Create",
  "suppressions": [
  ]
}
-->


