---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: 创建 SharePoint 列表
ms.openlocfilehash: a1e247722e9e8874a78a1951619e08bff9bd36e8
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27048857"
---
# <a name="create-a-new-list"></a><span data-ttu-id="bf608-102">创建新的列表</span><span class="sxs-lookup"><span data-stu-id="bf608-102">Create a new list</span></span>

> <span data-ttu-id="bf608-103">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="bf608-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="bf608-104">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="bf608-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="bf608-105">在 [site][] 中的创建新的 [list][]。</span><span class="sxs-lookup"><span data-stu-id="bf608-105">Create a new [list][] in a [site][].</span></span>

## <a name="permissions"></a><span data-ttu-id="bf608-106">权限</span><span class="sxs-lookup"><span data-stu-id="bf608-106">Permissions</span></span>

<span data-ttu-id="bf608-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="bf608-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|            <span data-ttu-id="bf608-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="bf608-109">Permission type</span></span>             | <span data-ttu-id="bf608-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="bf608-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="bf608-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="bf608-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="bf608-112">Sites.Manage.All</span><span class="sxs-lookup"><span data-stu-id="bf608-112">Sites.Manage.All</span></span>                            |
| <span data-ttu-id="bf608-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="bf608-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bf608-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="bf608-114">Not supported.</span></span>                              |
| <span data-ttu-id="bf608-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="bf608-115">Application</span></span>                            | <span data-ttu-id="bf608-116">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bf608-116">Sites.ReadWrite.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="bf608-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="bf608-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST https://graph.microsoft.com/beta/sites/{site-id}/lists
```

## <a name="request-body"></a><span data-ttu-id="bf608-118">请求正文</span><span class="sxs-lookup"><span data-stu-id="bf608-118">Request body</span></span>

<span data-ttu-id="bf608-119">在请求正文中，提供要创建的 [list][] 资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="bf608-119">In the request body, supply a JSON representation of the [list][] resource to create.</span></span>

## <a name="example"></a><span data-ttu-id="bf608-120">示例</span><span class="sxs-lookup"><span data-stu-id="bf608-120">Example</span></span>

<span data-ttu-id="bf608-121">下面的示例展示了如何创建新的泛型列表。</span><span class="sxs-lookup"><span data-stu-id="bf608-121">Here is an example of how to create a new generic list.</span></span>

<!-- { "blockType": "request", "name": "create-list", "scopes": "sites.readwrite.all" } -->

```http
POST /sites/{site-id}/lists
Content-Type: application/json

{
  "name": "Books",
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

<span data-ttu-id="bf608-122">**注意：** 自定义列都是可选的。</span><span class="sxs-lookup"><span data-stu-id="bf608-122">**Note:** Custom columns are optional.</span></span>

<span data-ttu-id="bf608-123">除了此处指定的任何列，还使用引用的**模板**中定义的列创建新列表。</span><span class="sxs-lookup"><span data-stu-id="bf608-123">In addition to any columns specified here, new lists are created with columns defined in the referenced **template**.</span></span>
<span data-ttu-id="bf608-124">如果未指定 **list** facet 或**模板**，则列表默认为 `genericList` 模板，其中包括“标题”__ 列。</span><span class="sxs-lookup"><span data-stu-id="bf608-124">If the **list** facet or **template** is unspecified, the list defaults to the `genericList` template, which includes a _Title_ column.</span></span>

## <a name="response"></a><span data-ttu-id="bf608-125">响应</span><span class="sxs-lookup"><span data-stu-id="bf608-125">Response</span></span>

<span data-ttu-id="bf608-126">如果成功，此方法在创建列表的响应正文中返回 [list][]。</span><span class="sxs-lookup"><span data-stu-id="bf608-126">If successful, this method returns a [list][] in the response body for the created list.</span></span>

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

<span data-ttu-id="bf608-127">**注意：** 为清楚起见，将截断 Response 对象。</span><span class="sxs-lookup"><span data-stu-id="bf608-127">**Note:** The response object is truncated for clarity.</span></span>
<span data-ttu-id="bf608-128">实际调用会返回默认属性。</span><span class="sxs-lookup"><span data-stu-id="bf608-128">Default properties will be returned from the actual call.</span></span>

[list]: ../resources/list.md
[site]: ../resources/site.md

<!-- {
  "type": "#page.annotation",
  "description": "Create a new SharePoint list.",
  "keywords": "",
  "section": "documentation",
  "tocPath": "List/Create"
} -->
