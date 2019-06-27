---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: 创建 SharePoint 列表
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 7a1333cee432c04bbc127298e005350fc21eb525
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35272098"
---
# <a name="create-a-new-list"></a><span data-ttu-id="6c9f2-102">创建新的列表</span><span class="sxs-lookup"><span data-stu-id="6c9f2-102">Create a new list</span></span>

<span data-ttu-id="6c9f2-103">在 [site][] 中的创建新的 [list][]。</span><span class="sxs-lookup"><span data-stu-id="6c9f2-103">Create a new [list][] in a [site][].</span></span>

## <a name="permissions"></a><span data-ttu-id="6c9f2-104">权限</span><span class="sxs-lookup"><span data-stu-id="6c9f2-104">Permissions</span></span>

<span data-ttu-id="6c9f2-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6c9f2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|            <span data-ttu-id="6c9f2-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="6c9f2-107">Permission type</span></span>             | <span data-ttu-id="6c9f2-108">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="6c9f2-108">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="6c9f2-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6c9f2-109">Delegated (work or school account)</span></span>     | <span data-ttu-id="6c9f2-110">Sites.Manage.All</span><span class="sxs-lookup"><span data-stu-id="6c9f2-110">Sites.Manage.All</span></span>                            |
| <span data-ttu-id="6c9f2-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6c9f2-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6c9f2-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="6c9f2-112">Not supported.</span></span>                              |
| <span data-ttu-id="6c9f2-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="6c9f2-113">Application</span></span>                            | <span data-ttu-id="6c9f2-114">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6c9f2-114">Sites.ReadWrite.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="6c9f2-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6c9f2-115">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST https://graph.microsoft.com/v1.0/sites/{site-id}/lists
```

## <a name="request-body"></a><span data-ttu-id="6c9f2-116">请求正文</span><span class="sxs-lookup"><span data-stu-id="6c9f2-116">Request body</span></span>

<span data-ttu-id="6c9f2-117">在请求正文中，提供要创建的 [list][] 资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6c9f2-117">In the request body, supply a JSON representation of the [list][] resource to create.</span></span>

## <a name="example"></a><span data-ttu-id="6c9f2-118">示例</span><span class="sxs-lookup"><span data-stu-id="6c9f2-118">Example</span></span>

<span data-ttu-id="6c9f2-119">下面的示例展示了如何创建新的泛型列表。</span><span class="sxs-lookup"><span data-stu-id="6c9f2-119">Here is an example of how to create a new generic list.</span></span>

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

<span data-ttu-id="6c9f2-120">**注意：** 自定义列都是可选的。</span><span class="sxs-lookup"><span data-stu-id="6c9f2-120">**Note:** Custom columns are optional.</span></span>

<span data-ttu-id="6c9f2-121">除了此处指定的任何列，还使用引用的**模板**中定义的列创建新列表。</span><span class="sxs-lookup"><span data-stu-id="6c9f2-121">In addition to any columns specified here, new lists are created with columns defined in the referenced **template**.</span></span>
<span data-ttu-id="6c9f2-122">如果未指定 **list** facet 或**模板**，则列表默认为 `genericList` 模板，其中包括“标题”__ 列。</span><span class="sxs-lookup"><span data-stu-id="6c9f2-122">If the **list** facet or **template** is unspecified, the list defaults to the `genericList` template, which includes a _Title_ column.</span></span>

## <a name="response"></a><span data-ttu-id="6c9f2-123">响应</span><span class="sxs-lookup"><span data-stu-id="6c9f2-123">Response</span></span>

<span data-ttu-id="6c9f2-124">如果成功，此方法在创建列表的响应正文中返回 [list][]。</span><span class="sxs-lookup"><span data-stu-id="6c9f2-124">If successful, this method returns a [list][] in the response body for the created list.</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="6c9f2-125">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="6c9f2-125">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="6c9f2-126">C#</span><span class="sxs-lookup"><span data-stu-id="6c9f2-126">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/create-list-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="6c9f2-127">Javascript</span><span class="sxs-lookup"><span data-stu-id="6c9f2-127">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create-list-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="6c9f2-128">目标-C</span><span class="sxs-lookup"><span data-stu-id="6c9f2-128">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/create-list-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<span data-ttu-id="6c9f2-129">**注意：** 为清楚起见，将截断 Response 对象。</span><span class="sxs-lookup"><span data-stu-id="6c9f2-129">**Note:** The response object is truncated for clarity.</span></span>
<span data-ttu-id="6c9f2-130">实际调用会返回默认属性。</span><span class="sxs-lookup"><span data-stu-id="6c9f2-130">Default properties will be returned from the actual call.</span></span>

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
    "Error: /api-reference/v1.0/api/list-create.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/list-create.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/list-create.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
} -->
