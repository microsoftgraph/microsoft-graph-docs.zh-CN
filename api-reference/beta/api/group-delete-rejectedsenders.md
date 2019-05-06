---
title: 删除 rejectedSender
description: 从 "拒绝的发件人" 列表中删除用户或组。
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 309a859fd45152fc4cd5e29e3d84db7e8c07664e
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2019
ms.locfileid: "33593303"
---
# <a name="remove-rejectedsender"></a><span data-ttu-id="bcdc0-103">删除 rejectedSender</span><span class="sxs-lookup"><span data-stu-id="bcdc0-103">Remove rejectedSender</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bcdc0-104">从指定组的 "拒绝的发件人" 列表中删除用户或组。</span><span class="sxs-lookup"><span data-stu-id="bcdc0-104">Remove a user or group from the rejected-senders list of the specified group.</span></span>

## <a name="permissions"></a><span data-ttu-id="bcdc0-105">权限</span><span class="sxs-lookup"><span data-stu-id="bcdc0-105">Permissions</span></span>
<span data-ttu-id="bcdc0-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="bcdc0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="bcdc0-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="bcdc0-108">Permission type</span></span>                        | <span data-ttu-id="bcdc0-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="bcdc0-109">Permissions (from least to most privileged)</span></span>  |
|:---------------------------------------|:-------------------------------------------- |
| <span data-ttu-id="bcdc0-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="bcdc0-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="bcdc0-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bcdc0-111">Group.ReadWrite.All</span></span>  |  
| <span data-ttu-id="bcdc0-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="bcdc0-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bcdc0-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="bcdc0-113">Not supported.</span></span> |
| <span data-ttu-id="bcdc0-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="bcdc0-114">Application</span></span>                            | <span data-ttu-id="bcdc0-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="bcdc0-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="bcdc0-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="bcdc0-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}/rejectedSenders/$ref?$id={id}
```

## <a name="request-headers"></a><span data-ttu-id="bcdc0-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="bcdc0-117">Request headers</span></span>

| <span data-ttu-id="bcdc0-118">标头</span><span class="sxs-lookup"><span data-stu-id="bcdc0-118">Header</span></span>         | <span data-ttu-id="bcdc0-119">值</span><span class="sxs-lookup"><span data-stu-id="bcdc0-119">Value</span></span>                      |
|:---------------|:---------------------------|
| <span data-ttu-id="bcdc0-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="bcdc0-120">Authorization</span></span>  | <span data-ttu-id="bcdc0-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="bcdc0-p102">Bearer {token}. Required.</span></span>  

## <a name="request-body"></a><span data-ttu-id="bcdc0-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="bcdc0-123">Request body</span></span>
<span data-ttu-id="bcdc0-124">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="bcdc0-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bcdc0-125">响应</span><span class="sxs-lookup"><span data-stu-id="bcdc0-125">Response</span></span>
<span data-ttu-id="bcdc0-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="bcdc0-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="bcdc0-128">示例</span><span class="sxs-lookup"><span data-stu-id="bcdc0-128">Examples</span></span>
### <a name="example-1-remove-a-user-from-the-rejected-senders-list-of-the-group"></a><span data-ttu-id="bcdc0-129">示例 1: 从组的 "拒绝的发件人" 列表中删除用户。</span><span class="sxs-lookup"><span data-stu-id="bcdc0-129">Example 1: Remove a user from the rejected-senders list of the group.</span></span>
#### <a name="request"></a><span data-ttu-id="bcdc0-130">请求</span><span class="sxs-lookup"><span data-stu-id="bcdc0-130">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "remove_user_from_rejectedsenderslist_of_group"
}-->
```http
DELETE https://graph.microsoft.com/beta/groups/{id}/rejectedSenders/$ref?$id=https://graph.microsoft.com/beta/users/{id}
```
#### <a name="response"></a><span data-ttu-id="bcdc0-131">响应</span><span class="sxs-lookup"><span data-stu-id="bcdc0-131">Response</span></span>
<span data-ttu-id="bcdc0-132">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="bcdc0-132">The following is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="bcdc0-133">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="bcdc0-133">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="bcdc0-134">语言</span><span class="sxs-lookup"><span data-stu-id="bcdc0-134">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/remove_user_from_rejectedsenderslist_of_group-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="bcdc0-135">Javascript</span><span class="sxs-lookup"><span data-stu-id="bcdc0-135">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/remove_user_from_rejectedsenderslist_of_group-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

### <a name="example-2-remove-a-group-from-the-rejected-senders-list-of-the-group"></a><span data-ttu-id="bcdc0-136">示例 2: 从组的 "拒绝-发件人" 列表中删除组。</span><span class="sxs-lookup"><span data-stu-id="bcdc0-136">Example 2: Remove a group from the rejected-senders list of the group.</span></span>
#### <a name="request"></a><span data-ttu-id="bcdc0-137">请求</span><span class="sxs-lookup"><span data-stu-id="bcdc0-137">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "remove_group_from_rejectedsenderslist_of_group"
}-->
```http
DELETE https://graph.microsoft.com/beta/groups/{id}/rejectedSenders/$ref?$id=https://graph.microsoft.com/beta/groups/{other-group-id}
```

#### <a name="response"></a><span data-ttu-id="bcdc0-138">响应</span><span class="sxs-lookup"><span data-stu-id="bcdc0-138">Response</span></span>
<span data-ttu-id="bcdc0-139">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="bcdc0-139">The following is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="bcdc0-140">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="bcdc0-140">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="bcdc0-141">语言</span><span class="sxs-lookup"><span data-stu-id="bcdc0-141">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/remove_group_from_rejectedsenderslist_of_group-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="bcdc0-142">Javascript</span><span class="sxs-lookup"><span data-stu-id="bcdc0-142">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/remove_group_from_rejectedsenderslist_of_group-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/group-delete-rejectedsenders.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/group-delete-rejectedsenders.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/group-delete-rejectedsenders.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/group-delete-rejectedsenders.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
