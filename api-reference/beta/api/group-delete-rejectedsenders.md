---
title: 删除 rejectedSender
description: 从拒绝的发件人列表中删除用户或组。
author: Jordanndahl
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 14bdcef8d41d204e3c3ae6f3de08a3d1cc53a5ff
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/27/2021
ms.locfileid: "52681832"
---
# <a name="remove-rejectedsender"></a><span data-ttu-id="ecdc4-103">删除 rejectedSender</span><span class="sxs-lookup"><span data-stu-id="ecdc4-103">Remove rejectedSender</span></span>

<span data-ttu-id="ecdc4-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ecdc4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ecdc4-105">从指定组的拒绝发件人列表中删除用户或组。</span><span class="sxs-lookup"><span data-stu-id="ecdc4-105">Remove a user or group from the rejected-senders list of the specified group.</span></span>

## <a name="permissions"></a><span data-ttu-id="ecdc4-106">权限</span><span class="sxs-lookup"><span data-stu-id="ecdc4-106">Permissions</span></span>
<span data-ttu-id="ecdc4-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ecdc4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ecdc4-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="ecdc4-109">Permission type</span></span>                        | <span data-ttu-id="ecdc4-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ecdc4-110">Permissions (from least to most privileged)</span></span>  |
|:---------------------------------------|:-------------------------------------------- |
| <span data-ttu-id="ecdc4-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ecdc4-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="ecdc4-112">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ecdc4-112">Group.ReadWrite.All</span></span>  |  
| <span data-ttu-id="ecdc4-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ecdc4-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ecdc4-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="ecdc4-114">Not supported.</span></span> |
| <span data-ttu-id="ecdc4-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="ecdc4-115">Application</span></span>                            | <span data-ttu-id="ecdc4-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="ecdc4-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ecdc4-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ecdc4-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}/rejectedSenders/$ref?$id={id}
```

## <a name="request-headers"></a><span data-ttu-id="ecdc4-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="ecdc4-118">Request headers</span></span>

| <span data-ttu-id="ecdc4-119">标头</span><span class="sxs-lookup"><span data-stu-id="ecdc4-119">Header</span></span>         | <span data-ttu-id="ecdc4-120">值</span><span class="sxs-lookup"><span data-stu-id="ecdc4-120">Value</span></span>                      |
|:---------------|:---------------------------|
| <span data-ttu-id="ecdc4-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="ecdc4-121">Authorization</span></span>  | <span data-ttu-id="ecdc4-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="ecdc4-p102">Bearer {token}. Required.</span></span>  

## <a name="request-body"></a><span data-ttu-id="ecdc4-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="ecdc4-124">Request body</span></span>
<span data-ttu-id="ecdc4-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="ecdc4-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ecdc4-126">响应</span><span class="sxs-lookup"><span data-stu-id="ecdc4-126">Response</span></span>
<span data-ttu-id="ecdc4-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="ecdc4-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="ecdc4-129">示例</span><span class="sxs-lookup"><span data-stu-id="ecdc4-129">Examples</span></span>
### <a name="example-1-remove-a-user-from-the-rejected-senders-list-of-the-group"></a><span data-ttu-id="ecdc4-130">示例 1：从组的拒绝发件人列表中删除用户。</span><span class="sxs-lookup"><span data-stu-id="ecdc4-130">Example 1: Remove a user from the rejected-senders list of the group.</span></span>
#### <a name="request"></a><span data-ttu-id="ecdc4-131">请求</span><span class="sxs-lookup"><span data-stu-id="ecdc4-131">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="ecdc4-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="ecdc4-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "remove_user_from_rejectedsenderslist_of_group"
}-->
```http
DELETE https://graph.microsoft.com/beta/groups/{id}/rejectedSenders/$ref?$id=https://graph.microsoft.com/beta/users/{id}
```
# <a name="c"></a>[<span data-ttu-id="ecdc4-133">C#</span><span class="sxs-lookup"><span data-stu-id="ecdc4-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/remove-user-from-rejectedsenderslist-of-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ecdc4-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ecdc4-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/remove-user-from-rejectedsenderslist-of-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ecdc4-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ecdc4-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/remove-user-from-rejectedsenderslist-of-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ecdc4-136">Java</span><span class="sxs-lookup"><span data-stu-id="ecdc4-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/remove-user-from-rejectedsenderslist-of-group-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="ecdc4-137">响应</span><span class="sxs-lookup"><span data-stu-id="ecdc4-137">Response</span></span>
<span data-ttu-id="ecdc4-138">下面介绍响应示例。</span><span class="sxs-lookup"><span data-stu-id="ecdc4-138">The following is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

### <a name="example-2-remove-a-group-from-the-rejected-senders-list-of-the-group"></a><span data-ttu-id="ecdc4-139">示例 2：从该组的拒绝发件人列表中删除组。</span><span class="sxs-lookup"><span data-stu-id="ecdc4-139">Example 2: Remove a group from the rejected-senders list of the group.</span></span>
#### <a name="request"></a><span data-ttu-id="ecdc4-140">请求</span><span class="sxs-lookup"><span data-stu-id="ecdc4-140">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="ecdc4-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="ecdc4-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "remove_group_from_rejectedsenderslist_of_group"
}-->
```http
DELETE https://graph.microsoft.com/beta/groups/{id}/rejectedSenders/$ref?$id=https://graph.microsoft.com/beta/groups/{other-group-id}
```
# <a name="c"></a>[<span data-ttu-id="ecdc4-142">C#</span><span class="sxs-lookup"><span data-stu-id="ecdc4-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/remove-group-from-rejectedsenderslist-of-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ecdc4-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ecdc4-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/remove-group-from-rejectedsenderslist-of-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ecdc4-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ecdc4-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/remove-group-from-rejectedsenderslist-of-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ecdc4-145">Java</span><span class="sxs-lookup"><span data-stu-id="ecdc4-145">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/remove-group-from-rejectedsenderslist-of-group-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="ecdc4-146">响应</span><span class="sxs-lookup"><span data-stu-id="ecdc4-146">Response</span></span>
<span data-ttu-id="ecdc4-147">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="ecdc4-147">The following is an example of the response.</span></span> 
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
  "description": "Remove rejectedSender",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


