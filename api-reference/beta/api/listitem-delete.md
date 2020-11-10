---
author: JeremyKelley
description: 从 list 中删除项。
ms.date: 09/11/2017
title: 从 SharePoint 列表中删除条目
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: 1493a5cc46bb0824709fa2b0cf7e37f251ee3697
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48971377"
---
# <a name="delete-an-item-from-a-list"></a><span data-ttu-id="9c119-103">从列表中删除项</span><span class="sxs-lookup"><span data-stu-id="9c119-103">Delete an item from a list</span></span>

<span data-ttu-id="9c119-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9c119-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9c119-105">从 [list][] 中删除项。</span><span class="sxs-lookup"><span data-stu-id="9c119-105">Removes an item from a [list][].</span></span>

[list]: ../resources/list.md

## <a name="permissions"></a><span data-ttu-id="9c119-107">权限</span><span class="sxs-lookup"><span data-stu-id="9c119-107">Permissions</span></span>

<span data-ttu-id="9c119-108">应用程序必须拥有用户授予的对要删除的项的写入权限，才能删除项。</span><span class="sxs-lookup"><span data-stu-id="9c119-108">To delete an item, the user must have granted the application write access to the item to be deleted.</span></span>

<span data-ttu-id="9c119-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9c119-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9c119-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="9c119-111">Permission type</span></span>      | <span data-ttu-id="9c119-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="9c119-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9c119-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9c119-113">Delegated (work or school account)</span></span> | <span data-ttu-id="9c119-114">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9c119-114">Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="9c119-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9c119-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9c119-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="9c119-116">Not supported.</span></span>    |
|<span data-ttu-id="9c119-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="9c119-117">Application</span></span> | <span data-ttu-id="9c119-118">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9c119-118">Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="9c119-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9c119-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /sites/{site-id}/lists/{list-id}/items/{item-id}
```

## <a name="optional-request-headers"></a><span data-ttu-id="9c119-120">可选的请求标头</span><span class="sxs-lookup"><span data-stu-id="9c119-120">Optional request headers</span></span>

| <span data-ttu-id="9c119-121">名称</span><span class="sxs-lookup"><span data-stu-id="9c119-121">Name</span></span>       | <span data-ttu-id="9c119-122">值</span><span class="sxs-lookup"><span data-stu-id="9c119-122">Value</span></span> | <span data-ttu-id="9c119-123">说明</span><span class="sxs-lookup"><span data-stu-id="9c119-123">Description</span></span>
|:-----------|:------|:--------------------------------------------------------
| <span data-ttu-id="9c119-124">_if-match_</span><span class="sxs-lookup"><span data-stu-id="9c119-124">_if-match_</span></span> | <span data-ttu-id="9c119-125">etag</span><span class="sxs-lookup"><span data-stu-id="9c119-125">etag</span></span>  | <span data-ttu-id="9c119-126">如果包含此请求标头，且提供的 eTag 与项中的当前标记不匹配，则返回 `412 Precondition Failed` 响应，并且不会删除该项。</span><span class="sxs-lookup"><span data-stu-id="9c119-126">If this request header is included and the eTag provided does not match the current tag on the item, a `412 Precondition Failed` response is returned and the item will not be deleted.</span></span>

## <a name="request-body"></a><span data-ttu-id="9c119-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="9c119-127">Request body</span></span>

<span data-ttu-id="9c119-128">请勿为此方法提供请求正文。</span><span class="sxs-lookup"><span data-stu-id="9c119-128">Do not supply a request body with this method.</span></span>

## <a name="example"></a><span data-ttu-id="9c119-129">示例</span><span class="sxs-lookup"><span data-stu-id="9c119-129">Example</span></span>


# <a name="http"></a>[<span data-ttu-id="9c119-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="9c119-130">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "delete-item", "scopes": "files.readwrite" } -->

```http
DELETE https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items/{item-id}
```
# <a name="c"></a>[<span data-ttu-id="9c119-131">C#</span><span class="sxs-lookup"><span data-stu-id="9c119-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-item-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9c119-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9c119-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-item-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9c119-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9c119-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-item-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="9c119-134">Java</span><span class="sxs-lookup"><span data-stu-id="9c119-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-item-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


## <a name="response"></a><span data-ttu-id="9c119-135">响应</span><span class="sxs-lookup"><span data-stu-id="9c119-135">Response</span></span>

<span data-ttu-id="9c119-136">如果成功，此调用将返回 `204 No Content` 响应，表示资源已被删除，没有可返回的内容。</span><span class="sxs-lookup"><span data-stu-id="9c119-136">If successful, this call returns a `204 No Content` response to indicate that resource was deleted and there was nothing to return.</span></span>

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


