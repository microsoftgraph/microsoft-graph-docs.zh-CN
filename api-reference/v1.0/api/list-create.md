---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: 创建 SharePoint 列表
localization_priority: Normal
ms.prod: sharepoint
description: 在 site 中的创建新的 list。
doc_type: apiPageType
ms.openlocfilehash: 96ab4b1f80ea85a6c17c7ad1d22214dac4bf687e
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48038464"
---
# <a name="create-a-new-list"></a><span data-ttu-id="ad072-103">创建新列表</span><span class="sxs-lookup"><span data-stu-id="ad072-103">Create a new list</span></span>

<span data-ttu-id="ad072-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ad072-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ad072-105">在 [site][] 中的创建新的 [list][]。</span><span class="sxs-lookup"><span data-stu-id="ad072-105">Create a new [list][] in a [site][].</span></span>

## <a name="permissions"></a><span data-ttu-id="ad072-106">权限</span><span class="sxs-lookup"><span data-stu-id="ad072-106">Permissions</span></span>

<span data-ttu-id="ad072-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ad072-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|            <span data-ttu-id="ad072-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="ad072-109">Permission type</span></span>             | <span data-ttu-id="ad072-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ad072-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="ad072-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ad072-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="ad072-112">Sites.Manage.All</span><span class="sxs-lookup"><span data-stu-id="ad072-112">Sites.Manage.All</span></span>                            |
| <span data-ttu-id="ad072-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ad072-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ad072-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="ad072-114">Not supported.</span></span>                              |
| <span data-ttu-id="ad072-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="ad072-115">Application</span></span>                            | <span data-ttu-id="ad072-116">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ad072-116">Sites.ReadWrite.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="ad072-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ad072-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST https://graph.microsoft.com/v1.0/sites/{site-id}/lists
```

## <a name="request-body"></a><span data-ttu-id="ad072-118">请求正文</span><span class="sxs-lookup"><span data-stu-id="ad072-118">Request body</span></span>

<span data-ttu-id="ad072-119">在请求正文中，提供要创建的 [list][] 资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ad072-119">In the request body, supply a JSON representation of the [list][] resource to create.</span></span>

## <a name="example"></a><span data-ttu-id="ad072-120">示例</span><span class="sxs-lookup"><span data-stu-id="ad072-120">Example</span></span>

<span data-ttu-id="ad072-121">下面的示例展示了如何创建新的泛型列表。</span><span class="sxs-lookup"><span data-stu-id="ad072-121">Here is an example of how to create a new generic list.</span></span>


# <a name="http"></a>[<span data-ttu-id="ad072-122">HTTP</span><span class="sxs-lookup"><span data-stu-id="ad072-122">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "create-list", "scopes": "sites.readwrite.all" } -->

```http
POST /sites/{site-id}/lists
Content-Type: application/json

{
  "displayName": "Books",
  "columns": [
    {
      "name": "Author",
      "text": { }
    },
    {
      "name": "PageCount",
      "number": { }
    }
  ],
  "list": {
    "template": "genericList"
  }
}
```
# <a name="c"></a>[<span data-ttu-id="ad072-123">C#</span><span class="sxs-lookup"><span data-stu-id="ad072-123">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-list-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ad072-124">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ad072-124">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-list-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ad072-125">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ad072-125">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-list-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ad072-126">Java</span><span class="sxs-lookup"><span data-stu-id="ad072-126">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-list-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="ad072-127">**注意：** 自定义列都是可选的。</span><span class="sxs-lookup"><span data-stu-id="ad072-127">**Note:** Custom columns are optional.</span></span>

<span data-ttu-id="ad072-128">除了此处指定的任何列，还使用引用的**模板**中定义的列创建新列表。</span><span class="sxs-lookup"><span data-stu-id="ad072-128">In addition to any columns specified here, new lists are created with columns defined in the referenced **template**.</span></span>
<span data-ttu-id="ad072-129">如果未指定 **list** facet 或**模板**，则列表默认为 `genericList` 模板，其中包括“标题”__ 列。</span><span class="sxs-lookup"><span data-stu-id="ad072-129">If the **list** facet or **template** is unspecified, the list defaults to the `genericList` template, which includes a _Title_ column.</span></span>

## <a name="response"></a><span data-ttu-id="ad072-130">响应</span><span class="sxs-lookup"><span data-stu-id="ad072-130">Response</span></span>

<span data-ttu-id="ad072-131">如果成功，此方法在创建列表的响应正文中返回 [list][]。</span><span class="sxs-lookup"><span data-stu-id="ad072-131">If successful, this method returns a [list][] in the response body for the created list.</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.list", "truncated": true } -->

```json
HTTP/1.1 201 Created
Content-type: application/json

{
  "id": "22e03ef3-6ef4-424d-a1d3-92a337807c30",
  "createdDateTime": "2017-04-30T01:21:00Z",
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

<span data-ttu-id="ad072-132">**注意：** 为清楚起见，将截断 Response 对象。</span><span class="sxs-lookup"><span data-stu-id="ad072-132">**Note:** The response object is truncated for clarity.</span></span>
<span data-ttu-id="ad072-133">实际调用会返回默认属性。</span><span class="sxs-lookup"><span data-stu-id="ad072-133">Default properties will be returned from the actual call.</span></span>

[列表]: ../resources/list.md
[list]: ../resources/list.md
[网站]: ../resources/site.md
[site]: ../resources/site.md

<!-- {
  "type": "#page.annotation",
  "description": "Create a new SharePoint list.",
  "keywords": "",
  "section": "documentation",
  "tocPath": "List/Create",
  "suppressions": [
  ]
} -->

