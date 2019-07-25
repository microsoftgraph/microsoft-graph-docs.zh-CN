---
title: 删除 rejectedSender
description: 从 "拒绝的发件人" 列表中删除用户或组。
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 9eccda8c9fce5a8582215d1bf296fcbf3adafda2
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35858839"
---
# <a name="remove-rejectedsender"></a><span data-ttu-id="b4acf-103">删除 rejectedSender</span><span class="sxs-lookup"><span data-stu-id="b4acf-103">Remove rejectedSender</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b4acf-104">从指定组的 "拒绝的发件人" 列表中删除用户或组。</span><span class="sxs-lookup"><span data-stu-id="b4acf-104">Remove a user or group from the rejected-senders list of the specified group.</span></span>

## <a name="permissions"></a><span data-ttu-id="b4acf-105">权限</span><span class="sxs-lookup"><span data-stu-id="b4acf-105">Permissions</span></span>
<span data-ttu-id="b4acf-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b4acf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b4acf-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="b4acf-108">Permission type</span></span>                        | <span data-ttu-id="b4acf-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b4acf-109">Permissions (from least to most privileged)</span></span>  |
|:---------------------------------------|:-------------------------------------------- |
| <span data-ttu-id="b4acf-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b4acf-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="b4acf-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b4acf-111">Group.ReadWrite.All</span></span>  |  
| <span data-ttu-id="b4acf-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b4acf-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b4acf-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="b4acf-113">Not supported.</span></span> |
| <span data-ttu-id="b4acf-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="b4acf-114">Application</span></span>                            | <span data-ttu-id="b4acf-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="b4acf-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b4acf-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b4acf-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}/rejectedSenders/$ref?$id={id}
```

## <a name="request-headers"></a><span data-ttu-id="b4acf-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="b4acf-117">Request headers</span></span>

| <span data-ttu-id="b4acf-118">标头</span><span class="sxs-lookup"><span data-stu-id="b4acf-118">Header</span></span>         | <span data-ttu-id="b4acf-119">值</span><span class="sxs-lookup"><span data-stu-id="b4acf-119">Value</span></span>                      |
|:---------------|:---------------------------|
| <span data-ttu-id="b4acf-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="b4acf-120">Authorization</span></span>  | <span data-ttu-id="b4acf-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="b4acf-p102">Bearer {token}. Required.</span></span>  

## <a name="request-body"></a><span data-ttu-id="b4acf-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="b4acf-123">Request body</span></span>
<span data-ttu-id="b4acf-124">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="b4acf-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b4acf-125">响应</span><span class="sxs-lookup"><span data-stu-id="b4acf-125">Response</span></span>
<span data-ttu-id="b4acf-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="b4acf-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="b4acf-128">示例</span><span class="sxs-lookup"><span data-stu-id="b4acf-128">Examples</span></span>
### <a name="example-1-remove-a-user-from-the-rejected-senders-list-of-the-group"></a><span data-ttu-id="b4acf-129">示例 1: 从组的 "拒绝的发件人" 列表中删除用户。</span><span class="sxs-lookup"><span data-stu-id="b4acf-129">Example 1: Remove a user from the rejected-senders list of the group.</span></span>
#### <a name="request"></a><span data-ttu-id="b4acf-130">请求</span><span class="sxs-lookup"><span data-stu-id="b4acf-130">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="b4acf-131">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="b4acf-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "remove_user_from_rejectedsenderslist_of_group"
}-->
```http
DELETE https://graph.microsoft.com/beta/groups/{id}/rejectedSenders/$ref?$id=https://graph.microsoft.com/beta/users/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="b4acf-132">C#</span><span class="sxs-lookup"><span data-stu-id="b4acf-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/remove-user-from-rejectedsenderslist-of-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b4acf-133">Javascript</span><span class="sxs-lookup"><span data-stu-id="b4acf-133">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/remove-user-from-rejectedsenderslist-of-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="b4acf-134">目标-C</span><span class="sxs-lookup"><span data-stu-id="b4acf-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/remove-user-from-rejectedsenderslist-of-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="b4acf-135">Java</span><span class="sxs-lookup"><span data-stu-id="b4acf-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/remove-user-from-rejectedsenderslist-of-group-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="b4acf-136">响应</span><span class="sxs-lookup"><span data-stu-id="b4acf-136">Response</span></span>
<span data-ttu-id="b4acf-137">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="b4acf-137">The following is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

### <a name="example-2-remove-a-group-from-the-rejected-senders-list-of-the-group"></a><span data-ttu-id="b4acf-138">示例 2: 从组的 "拒绝-发件人" 列表中删除组。</span><span class="sxs-lookup"><span data-stu-id="b4acf-138">Example 2: Remove a group from the rejected-senders list of the group.</span></span>
#### <a name="request"></a><span data-ttu-id="b4acf-139">请求</span><span class="sxs-lookup"><span data-stu-id="b4acf-139">Request</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="b4acf-140">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="b4acf-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "remove_group_from_rejectedsenderslist_of_group"
}-->
```http
DELETE https://graph.microsoft.com/beta/groups/{id}/rejectedSenders/$ref?$id=https://graph.microsoft.com/beta/groups/{other-group-id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="b4acf-141">C#</span><span class="sxs-lookup"><span data-stu-id="b4acf-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/remove-group-from-rejectedsenderslist-of-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b4acf-142">Javascript</span><span class="sxs-lookup"><span data-stu-id="b4acf-142">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/remove-group-from-rejectedsenderslist-of-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="b4acf-143">目标-C</span><span class="sxs-lookup"><span data-stu-id="b4acf-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/remove-group-from-rejectedsenderslist-of-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="b4acf-144">Java</span><span class="sxs-lookup"><span data-stu-id="b4acf-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/remove-group-from-rejectedsenderslist-of-group-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="b4acf-145">响应</span><span class="sxs-lookup"><span data-stu-id="b4acf-145">Response</span></span>
<span data-ttu-id="b4acf-146">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="b4acf-146">The following is an example of the response.</span></span> 
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
