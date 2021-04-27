---
title: 删除 plannerBucket
description: 删除 **plannerBucket**。
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: apiPageType
ms.openlocfilehash: a136237632781f4bb9cb050bcb1fdf82dc098aca
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52055328"
---
# <a name="delete-plannerbucket"></a><span data-ttu-id="ce52a-103">删除 plannerBucket</span><span class="sxs-lookup"><span data-stu-id="ce52a-103">Delete plannerBucket</span></span>

<span data-ttu-id="ce52a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ce52a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ce52a-105">删除 **plannerBucket**。</span><span class="sxs-lookup"><span data-stu-id="ce52a-105">Delete **plannerBucket**.</span></span>
## <a name="permissions"></a><span data-ttu-id="ce52a-106">权限</span><span class="sxs-lookup"><span data-stu-id="ce52a-106">Permissions</span></span>
<span data-ttu-id="ce52a-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ce52a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ce52a-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="ce52a-109">Permission type</span></span>      | <span data-ttu-id="ce52a-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ce52a-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ce52a-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ce52a-111">Delegated (work or school account)</span></span> | <span data-ttu-id="ce52a-112">Tasks.ReadWrite，Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ce52a-112">Tasks.ReadWrite, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="ce52a-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ce52a-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ce52a-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="ce52a-114">Not supported.</span></span>    |
|<span data-ttu-id="ce52a-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="ce52a-115">Application</span></span> | <span data-ttu-id="ce52a-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="ce52a-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ce52a-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ce52a-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /planner/buckets/{id}
```
## <a name="request-headers"></a><span data-ttu-id="ce52a-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="ce52a-118">Request headers</span></span>
| <span data-ttu-id="ce52a-119">名称</span><span class="sxs-lookup"><span data-stu-id="ce52a-119">Name</span></span>       | <span data-ttu-id="ce52a-120">说明</span><span class="sxs-lookup"><span data-stu-id="ce52a-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="ce52a-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="ce52a-121">Authorization</span></span>  | <span data-ttu-id="ce52a-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="ce52a-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="ce52a-124">If-Match</span><span class="sxs-lookup"><span data-stu-id="ce52a-124">If-Match</span></span>  | <span data-ttu-id="ce52a-p103">要删除的 **plannerBucket** 的上次已知 ETag 值。必需。</span><span class="sxs-lookup"><span data-stu-id="ce52a-p103">Last known ETag value for the **plannerBucket** to be deleted. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="ce52a-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="ce52a-127">Request body</span></span>
<span data-ttu-id="ce52a-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="ce52a-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ce52a-129">响应</span><span class="sxs-lookup"><span data-stu-id="ce52a-129">Response</span></span>

<span data-ttu-id="ce52a-p104">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="ce52a-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

<span data-ttu-id="ce52a-p105">此方法可以返回任何 [HTTP 状态代码](/graph/errors)。应用应当为此方法处理的最常见的错误为 400、403、404、409 和 412 响应。有关这些错误的详细信息，请参阅[常见规划器错误情况](../resources/planner-overview.md#common-planner-error-conditions)。</span><span class="sxs-lookup"><span data-stu-id="ce52a-p105">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 400, 403, 404, 409, and 412 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="ce52a-135">示例</span><span class="sxs-lookup"><span data-stu-id="ce52a-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ce52a-136">请求</span><span class="sxs-lookup"><span data-stu-id="ce52a-136">Request</span></span>
<span data-ttu-id="ce52a-137">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="ce52a-137">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="ce52a-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="ce52a-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_plannerbucket"
}-->
```http
DELETE https://graph.microsoft.com/beta/planner/buckets/{id}
If-Match: W/"JzEtVGFzayAgQEBAQEBAQEBAQEBAQEBAWCc="
```
# <a name="c"></a>[<span data-ttu-id="ce52a-139">C#</span><span class="sxs-lookup"><span data-stu-id="ce52a-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-plannerbucket-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ce52a-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ce52a-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-plannerbucket-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ce52a-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ce52a-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-plannerbucket-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ce52a-142">Java</span><span class="sxs-lookup"><span data-stu-id="ce52a-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-plannerbucket-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="ce52a-143">响应</span><span class="sxs-lookup"><span data-stu-id="ce52a-143">Response</span></span>
<span data-ttu-id="ce52a-144">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="ce52a-144">Here is an example of the response.</span></span> <span data-ttu-id="ce52a-145">注意：为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="ce52a-145">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete plannerBucket",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


