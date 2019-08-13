---
author: JeremyKelley
description: 在列表中创建新的 listItem。
ms.date: 09/11/2017
title: 在 SharePoint 列表中创建新条目
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: 8b1b4ba187c204769d55355bebbfd5468aa6956c
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36342997"
---
# <a name="create-a-new-item-in-a-list"></a><span data-ttu-id="bb8f7-103">在列表中创建新项</span><span class="sxs-lookup"><span data-stu-id="bb8f7-103">Create a new item in a list</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bb8f7-104">在[列表][]中创建新的 [listItem][]。</span><span class="sxs-lookup"><span data-stu-id="bb8f7-104">Create a new [listItem][] in a [list][].</span></span>

## <a name="permissions"></a><span data-ttu-id="bb8f7-105">权限</span><span class="sxs-lookup"><span data-stu-id="bb8f7-105">Permissions</span></span>

<span data-ttu-id="bb8f7-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="bb8f7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bb8f7-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="bb8f7-108">Permission type</span></span>      | <span data-ttu-id="bb8f7-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="bb8f7-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bb8f7-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="bb8f7-110">Delegated (work or school account)</span></span> | <span data-ttu-id="bb8f7-111">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bb8f7-111">Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="bb8f7-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="bb8f7-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bb8f7-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="bb8f7-113">Not supported.</span></span>    |
|<span data-ttu-id="bb8f7-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="bb8f7-114">Application</span></span> | <span data-ttu-id="bb8f7-115">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bb8f7-115">Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="bb8f7-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="bb8f7-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items
```

## <a name="request-body"></a><span data-ttu-id="bb8f7-117">请求正文</span><span class="sxs-lookup"><span data-stu-id="bb8f7-117">Request body</span></span>

<span data-ttu-id="bb8f7-118">在请求正文中，提供要创建的 [listItem][] 资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="bb8f7-118">In the request body, supply a JSON representation of the [listItem][] resource to create.</span></span>

## <a name="example"></a><span data-ttu-id="bb8f7-119">示例</span><span class="sxs-lookup"><span data-stu-id="bb8f7-119">Example</span></span>

<span data-ttu-id="bb8f7-120">下面的示例展示了如何创建新的泛型列表项。</span><span class="sxs-lookup"><span data-stu-id="bb8f7-120">Here is an example of how to create a new generic list item.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="bb8f7-121">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="bb8f7-121">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "create-listitem", "scopes": "sites.readwrite.all" } -->

```json
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="bb8f7-122">C#</span><span class="sxs-lookup"><span data-stu-id="bb8f7-122">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-listitem-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="bb8f7-123">JavaScript</span><span class="sxs-lookup"><span data-stu-id="bb8f7-123">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-listitem-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="bb8f7-124">目标-C</span><span class="sxs-lookup"><span data-stu-id="bb8f7-124">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-listitem-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="bb8f7-125">Java</span><span class="sxs-lookup"><span data-stu-id="bb8f7-125">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-listitem-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


## <a name="response"></a><span data-ttu-id="bb8f7-126">响应</span><span class="sxs-lookup"><span data-stu-id="bb8f7-126">Response</span></span>

<span data-ttu-id="bb8f7-127">如果成功，此方法在已创建列表项的响应正文中返回 [listItem][]。</span><span class="sxs-lookup"><span data-stu-id="bb8f7-127">If successful, this method returns a [listItem][] in the response body for the created list item.</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.listItem", "truncated": true } -->

```json
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

<span data-ttu-id="bb8f7-128">**注意：** 为清楚起见，将截断 Response 对象。</span><span class="sxs-lookup"><span data-stu-id="bb8f7-128">**Note:** The response object is truncated for clarity.</span></span> <span data-ttu-id="bb8f7-129">实际调用会返回默认属性。</span><span class="sxs-lookup"><span data-stu-id="bb8f7-129">Default properties will be returned from the actual call.</span></span>

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
