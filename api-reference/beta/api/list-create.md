---
author: JeremyKelley
description: 在 site 中的创建新的 list。
ms.date: 09/11/2017
title: 创建 SharePoint 列表
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: bbc23b04fe38e61e7e7313ca34ea9c2800854e8b
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36347127"
---
# <a name="create-a-new-list"></a><span data-ttu-id="6fdee-103">创建新的列表</span><span class="sxs-lookup"><span data-stu-id="6fdee-103">Create a new list</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6fdee-104">在 [site][] 中的创建新的 [list][]。</span><span class="sxs-lookup"><span data-stu-id="6fdee-104">Create a new [list][] in a [site][].</span></span>

## <a name="permissions"></a><span data-ttu-id="6fdee-105">权限</span><span class="sxs-lookup"><span data-stu-id="6fdee-105">Permissions</span></span>

<span data-ttu-id="6fdee-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6fdee-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|            <span data-ttu-id="6fdee-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="6fdee-108">Permission type</span></span>             | <span data-ttu-id="6fdee-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="6fdee-109">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="6fdee-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6fdee-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="6fdee-111">Sites.Manage.All</span><span class="sxs-lookup"><span data-stu-id="6fdee-111">Sites.Manage.All</span></span>                            |
| <span data-ttu-id="6fdee-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6fdee-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6fdee-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="6fdee-113">Not supported.</span></span>                              |
| <span data-ttu-id="6fdee-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="6fdee-114">Application</span></span>                            | <span data-ttu-id="6fdee-115">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6fdee-115">Sites.ReadWrite.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="6fdee-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6fdee-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST https://graph.microsoft.com/beta/sites/{site-id}/lists
```

## <a name="request-body"></a><span data-ttu-id="6fdee-117">请求正文</span><span class="sxs-lookup"><span data-stu-id="6fdee-117">Request body</span></span>

<span data-ttu-id="6fdee-118">在请求正文中，提供要创建的 [list][] 资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6fdee-118">In the request body, supply a JSON representation of the [list][] resource to create.</span></span>

## <a name="example"></a><span data-ttu-id="6fdee-119">示例</span><span class="sxs-lookup"><span data-stu-id="6fdee-119">Example</span></span>

<span data-ttu-id="6fdee-120">下面的示例展示了如何创建新的泛型列表。</span><span class="sxs-lookup"><span data-stu-id="6fdee-120">Here is an example of how to create a new generic list.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="6fdee-121">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="6fdee-121">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="6fdee-122">C#</span><span class="sxs-lookup"><span data-stu-id="6fdee-122">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-list-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="6fdee-123">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6fdee-123">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-list-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="6fdee-124">目标-C</span><span class="sxs-lookup"><span data-stu-id="6fdee-124">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-list-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="6fdee-125">Java</span><span class="sxs-lookup"><span data-stu-id="6fdee-125">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-list-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="6fdee-126">**注意：** 自定义列都是可选的。</span><span class="sxs-lookup"><span data-stu-id="6fdee-126">**Note:** Custom columns are optional.</span></span>

<span data-ttu-id="6fdee-127">除了此处指定的任何列，还使用引用的**模板**中定义的列创建新列表。</span><span class="sxs-lookup"><span data-stu-id="6fdee-127">In addition to any columns specified here, new lists are created with columns defined in the referenced **template**.</span></span>
<span data-ttu-id="6fdee-128">如果未指定 **list** facet 或**模板**，则列表默认为 `genericList` 模板，其中包括“标题”__ 列。</span><span class="sxs-lookup"><span data-stu-id="6fdee-128">If the **list** facet or **template** is unspecified, the list defaults to the `genericList` template, which includes a _Title_ column.</span></span>

## <a name="response"></a><span data-ttu-id="6fdee-129">响应</span><span class="sxs-lookup"><span data-stu-id="6fdee-129">Response</span></span>

<span data-ttu-id="6fdee-130">如果成功，此方法在创建列表的响应正文中返回 [list][]。</span><span class="sxs-lookup"><span data-stu-id="6fdee-130">If successful, this method returns a [list][] in the response body for the created list.</span></span>

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

<span data-ttu-id="6fdee-131">**注意：** 为清楚起见，将截断 Response 对象。</span><span class="sxs-lookup"><span data-stu-id="6fdee-131">**Note:** The response object is truncated for clarity.</span></span>
<span data-ttu-id="6fdee-132">实际调用会返回默认属性。</span><span class="sxs-lookup"><span data-stu-id="6fdee-132">Default properties will be returned from the actual call.</span></span>

[list]: ../resources/list.md
[网站]: ../resources/site.md
[site]: ../resources/site.md

<!--
{
  "type": "#page.annotation",
  "description": "Create a new SharePoint list.",
  "keywords": "",
  "section": "documentation",
  "tocPath": "List/Create",
  "suppressions": [
  ]
}
-->
