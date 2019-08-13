---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: 从 SharePoint 列表中删除条目
localization_priority: Normal
ms.prod: sharepoint
description: 从 list 中删除项。
doc_type: apiPageType
ms.openlocfilehash: ac07e03892476ad160f76dd49ced3b2bcb63ace6
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36374017"
---
# <a name="delete-an-item-from-a-list"></a><span data-ttu-id="e74c4-103">从列表中删除项</span><span class="sxs-lookup"><span data-stu-id="e74c4-103">Delete an item from a list</span></span>

<span data-ttu-id="e74c4-104">从 [list][] 中删除项。</span><span class="sxs-lookup"><span data-stu-id="e74c4-104">Removes an item from a [list][].</span></span>

[列表]: ../resources/list.md
[list]: ../resources/list.md

## <a name="permissions"></a><span data-ttu-id="e74c4-106">权限</span><span class="sxs-lookup"><span data-stu-id="e74c4-106">Permissions</span></span>

<span data-ttu-id="e74c4-107">应用程序必须拥有用户授予的对要删除的项的写入权限，才能删除项。</span><span class="sxs-lookup"><span data-stu-id="e74c4-107">To delete an item, the user must have granted the application write access to the item to be deleted.</span></span>

<span data-ttu-id="e74c4-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e74c4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e74c4-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="e74c4-110">Permission type</span></span>      | <span data-ttu-id="e74c4-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e74c4-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e74c4-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e74c4-112">Delegated (work or school account)</span></span> | <span data-ttu-id="e74c4-113">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e74c4-113">Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="e74c4-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e74c4-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e74c4-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="e74c4-115">Not supported.</span></span>    |
|<span data-ttu-id="e74c4-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="e74c4-116">Application</span></span> | <span data-ttu-id="e74c4-117">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e74c4-117">Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e74c4-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e74c4-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items/{item-id}
```

## <a name="optional-request-headers"></a><span data-ttu-id="e74c4-119">可选的请求标头</span><span class="sxs-lookup"><span data-stu-id="e74c4-119">Optional request headers</span></span>

| <span data-ttu-id="e74c4-120">名称</span><span class="sxs-lookup"><span data-stu-id="e74c4-120">Name</span></span>       | <span data-ttu-id="e74c4-121">值</span><span class="sxs-lookup"><span data-stu-id="e74c4-121">Value</span></span> | <span data-ttu-id="e74c4-122">说明</span><span class="sxs-lookup"><span data-stu-id="e74c4-122">Description</span></span>
|:-----------|:------|:--------------------------------------------------------
| <span data-ttu-id="e74c4-123">_if-match_</span><span class="sxs-lookup"><span data-stu-id="e74c4-123">_if-match_</span></span> | <span data-ttu-id="e74c4-124">etag</span><span class="sxs-lookup"><span data-stu-id="e74c4-124">etag</span></span>  | <span data-ttu-id="e74c4-125">如果包含此请求标头，且提供的 eTag 与项中的当前标记不匹配，则返回 `412 Precondition Failed` 响应，并且不会删除该项。</span><span class="sxs-lookup"><span data-stu-id="e74c4-125">If this request header is included and the eTag provided does not match the current tag on the item, a `412 Precondition Failed` response is returned and the item will not be deleted.</span></span>

## <a name="request-body"></a><span data-ttu-id="e74c4-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="e74c4-126">Request body</span></span>

<span data-ttu-id="e74c4-127">请勿为此方法提供请求正文。</span><span class="sxs-lookup"><span data-stu-id="e74c4-127">Do not supply a request body with this method.</span></span>

## <a name="example"></a><span data-ttu-id="e74c4-128">示例</span><span class="sxs-lookup"><span data-stu-id="e74c4-128">Example</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="e74c4-129">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="e74c4-129">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "delete-item-site", "scopes": "files.readwrite sites.readwrite.all" } -->

```http
DELETE https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items/{item-id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="e74c4-130">C#</span><span class="sxs-lookup"><span data-stu-id="e74c4-130">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-item-site-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e74c4-131">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e74c4-131">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-item-site-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="e74c4-132">目标-C</span><span class="sxs-lookup"><span data-stu-id="e74c4-132">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-item-site-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="e74c4-133">Java</span><span class="sxs-lookup"><span data-stu-id="e74c4-133">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-item-site-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


## <a name="response"></a><span data-ttu-id="e74c4-134">响应</span><span class="sxs-lookup"><span data-stu-id="e74c4-134">Response</span></span>

<span data-ttu-id="e74c4-135">如果成功，此调用将返回 `204 No Content` 响应，表示资源已被删除，没有可返回的内容。</span><span class="sxs-lookup"><span data-stu-id="e74c4-135">If successful, this call returns a `204 No Content` response to indicate that resource was deleted and there was nothing to return.</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No Content
```

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "ListItem/Delete",
  "suppressions": [
  ]
} -->
