---
author: JeremyKelley
description: 从 list 中删除项。
ms.date: 09/11/2017
title: 从 SharePoint 列表中删除条目
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: f392ec8699fb2e079446c6f72c12c844db62852c
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42457132"
---
# <a name="delete-an-item-from-a-list"></a><span data-ttu-id="124ea-103">从列表中删除项</span><span class="sxs-lookup"><span data-stu-id="124ea-103">Delete an item from a list</span></span>

<span data-ttu-id="124ea-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="124ea-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="124ea-105">从 [list][] 中删除项。</span><span class="sxs-lookup"><span data-stu-id="124ea-105">Removes an item from a [list][].</span></span>

[list]: ../resources/list.md

## <a name="permissions"></a><span data-ttu-id="124ea-107">权限</span><span class="sxs-lookup"><span data-stu-id="124ea-107">Permissions</span></span>

<span data-ttu-id="124ea-108">应用程序必须拥有用户授予的对要删除的项的写入权限，才能删除项。</span><span class="sxs-lookup"><span data-stu-id="124ea-108">To delete an item, the user must have granted the application write access to the item to be deleted.</span></span>

<span data-ttu-id="124ea-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="124ea-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="124ea-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="124ea-111">Permission type</span></span>      | <span data-ttu-id="124ea-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="124ea-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="124ea-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="124ea-113">Delegated (work or school account)</span></span> | <span data-ttu-id="124ea-114">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="124ea-114">Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="124ea-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="124ea-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="124ea-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="124ea-116">Not supported.</span></span>    |
|<span data-ttu-id="124ea-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="124ea-117">Application</span></span> | <span data-ttu-id="124ea-118">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="124ea-118">Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="124ea-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="124ea-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /sites/{site-id}/lists/{list-id}/items/{item-id}
```

## <a name="optional-request-headers"></a><span data-ttu-id="124ea-120">可选的请求标头</span><span class="sxs-lookup"><span data-stu-id="124ea-120">Optional request headers</span></span>

| <span data-ttu-id="124ea-121">名称</span><span class="sxs-lookup"><span data-stu-id="124ea-121">Name</span></span>       | <span data-ttu-id="124ea-122">值</span><span class="sxs-lookup"><span data-stu-id="124ea-122">Value</span></span> | <span data-ttu-id="124ea-123">说明</span><span class="sxs-lookup"><span data-stu-id="124ea-123">Description</span></span>
|:-----------|:------|:--------------------------------------------------------
| <span data-ttu-id="124ea-124">_if-match_</span><span class="sxs-lookup"><span data-stu-id="124ea-124">_if-match_</span></span> | <span data-ttu-id="124ea-125">etag</span><span class="sxs-lookup"><span data-stu-id="124ea-125">etag</span></span>  | <span data-ttu-id="124ea-126">如果包含此请求标头，且提供的 eTag 与项中的当前标记不匹配，则返回 `412 Precondition Failed` 响应，并且不会删除该项。</span><span class="sxs-lookup"><span data-stu-id="124ea-126">If this request header is included and the eTag provided does not match the current tag on the item, a `412 Precondition Failed` response is returned and the item will not be deleted.</span></span>

## <a name="request-body"></a><span data-ttu-id="124ea-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="124ea-127">Request body</span></span>

<span data-ttu-id="124ea-128">请勿为此方法提供请求正文。</span><span class="sxs-lookup"><span data-stu-id="124ea-128">Do not supply a request body with this method.</span></span>

## <a name="example"></a><span data-ttu-id="124ea-129">示例</span><span class="sxs-lookup"><span data-stu-id="124ea-129">Example</span></span>


# <a name="http"></a>[<span data-ttu-id="124ea-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="124ea-130">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "delete-item", "scopes": "files.readwrite" } -->

```http
DELETE https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items/{item-id}
```
# <a name="c"></a>[<span data-ttu-id="124ea-131">C#</span><span class="sxs-lookup"><span data-stu-id="124ea-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-item-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="124ea-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="124ea-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-item-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="124ea-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="124ea-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-item-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


## <a name="response"></a><span data-ttu-id="124ea-134">响应</span><span class="sxs-lookup"><span data-stu-id="124ea-134">Response</span></span>

<span data-ttu-id="124ea-135">如果成功，此调用将返回 `204 No Content` 响应，表示资源已被删除，没有可返回的内容。</span><span class="sxs-lookup"><span data-stu-id="124ea-135">If successful, this call returns a `204 No Content` response to indicate that resource was deleted and there was nothing to return.</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No Content
```

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "ListItem/Delete",
  "suppressions": [
  ]
}
-->
