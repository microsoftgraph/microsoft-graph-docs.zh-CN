---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: 从 SharePoint 列表中删除条目
localization_priority: Normal
ms.prod: sharepoint
description: 从 list 中删除项。
doc_type: apiPageType
ms.openlocfilehash: f62360dec348e80cc2f54bc2d06afdc20abf19c0
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42511710"
---
# <a name="delete-an-item-from-a-list"></a><span data-ttu-id="bebeb-103">从列表中删除项</span><span class="sxs-lookup"><span data-stu-id="bebeb-103">Delete an item from a list</span></span>

<span data-ttu-id="bebeb-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bebeb-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="bebeb-105">从 [list][] 中删除项。</span><span class="sxs-lookup"><span data-stu-id="bebeb-105">Removes an item from a [list][].</span></span>

[list]: ../resources/list.md

## <a name="permissions"></a><span data-ttu-id="bebeb-107">权限</span><span class="sxs-lookup"><span data-stu-id="bebeb-107">Permissions</span></span>

<span data-ttu-id="bebeb-108">应用程序必须拥有用户授予的对要删除的项的写入权限，才能删除项。</span><span class="sxs-lookup"><span data-stu-id="bebeb-108">To delete an item, the user must have granted the application write access to the item to be deleted.</span></span>

<span data-ttu-id="bebeb-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="bebeb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bebeb-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="bebeb-111">Permission type</span></span>      | <span data-ttu-id="bebeb-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="bebeb-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bebeb-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="bebeb-113">Delegated (work or school account)</span></span> | <span data-ttu-id="bebeb-114">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bebeb-114">Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="bebeb-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="bebeb-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bebeb-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="bebeb-116">Not supported.</span></span>    |
|<span data-ttu-id="bebeb-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="bebeb-117">Application</span></span> | <span data-ttu-id="bebeb-118">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bebeb-118">Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="bebeb-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="bebeb-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items/{item-id}
```

## <a name="optional-request-headers"></a><span data-ttu-id="bebeb-120">可选的请求标头</span><span class="sxs-lookup"><span data-stu-id="bebeb-120">Optional request headers</span></span>

| <span data-ttu-id="bebeb-121">名称</span><span class="sxs-lookup"><span data-stu-id="bebeb-121">Name</span></span>       | <span data-ttu-id="bebeb-122">值</span><span class="sxs-lookup"><span data-stu-id="bebeb-122">Value</span></span> | <span data-ttu-id="bebeb-123">说明</span><span class="sxs-lookup"><span data-stu-id="bebeb-123">Description</span></span>
|:-----------|:------|:--------------------------------------------------------
| <span data-ttu-id="bebeb-124">_if-match_</span><span class="sxs-lookup"><span data-stu-id="bebeb-124">_if-match_</span></span> | <span data-ttu-id="bebeb-125">etag</span><span class="sxs-lookup"><span data-stu-id="bebeb-125">etag</span></span>  | <span data-ttu-id="bebeb-126">如果包含此请求标头，且提供的 eTag 与项中的当前标记不匹配，则返回 `412 Precondition Failed` 响应，并且不会删除该项。</span><span class="sxs-lookup"><span data-stu-id="bebeb-126">If this request header is included and the eTag provided does not match the current tag on the item, a `412 Precondition Failed` response is returned and the item will not be deleted.</span></span>

## <a name="request-body"></a><span data-ttu-id="bebeb-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="bebeb-127">Request body</span></span>

<span data-ttu-id="bebeb-128">请勿为此方法提供请求正文。</span><span class="sxs-lookup"><span data-stu-id="bebeb-128">Do not supply a request body with this method.</span></span>

## <a name="example"></a><span data-ttu-id="bebeb-129">示例</span><span class="sxs-lookup"><span data-stu-id="bebeb-129">Example</span></span>


# <a name="http"></a>[<span data-ttu-id="bebeb-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="bebeb-130">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "delete-item-site", "scopes": "files.readwrite sites.readwrite.all" } -->

```http
DELETE https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items/{item-id}
```
# <a name="c"></a>[<span data-ttu-id="bebeb-131">C#</span><span class="sxs-lookup"><span data-stu-id="bebeb-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-item-site-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="bebeb-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="bebeb-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-item-site-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="bebeb-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="bebeb-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-item-site-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="bebeb-134">Java</span><span class="sxs-lookup"><span data-stu-id="bebeb-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-item-site-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


## <a name="response"></a><span data-ttu-id="bebeb-135">响应</span><span class="sxs-lookup"><span data-stu-id="bebeb-135">Response</span></span>

<span data-ttu-id="bebeb-136">如果成功，此调用将返回 `204 No Content` 响应，表示资源已被删除，没有可返回的内容。</span><span class="sxs-lookup"><span data-stu-id="bebeb-136">If successful, this call returns a `204 No Content` response to indicate that resource was deleted and there was nothing to return.</span></span>

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
