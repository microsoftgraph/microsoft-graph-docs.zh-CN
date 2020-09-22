---
title: 删除 rejectedSender
description: 从 "拒绝的发件人" 列表中删除用户或组。
author: yyuank
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 0844e05da10dda1888309d90591153b443614915
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48094814"
---
# <a name="remove-rejectedsender"></a><span data-ttu-id="4e1e0-103">删除 rejectedSender</span><span class="sxs-lookup"><span data-stu-id="4e1e0-103">Remove rejectedSender</span></span>

<span data-ttu-id="4e1e0-104">命名空间： microsoft. graph 从拒绝的发件人列表中删除用户或组。</span><span class="sxs-lookup"><span data-stu-id="4e1e0-104">Namespace: microsoft.graph Remove a user or group from the rejected-senders list.</span></span>

## <a name="permissions"></a><span data-ttu-id="4e1e0-105">权限</span><span class="sxs-lookup"><span data-stu-id="4e1e0-105">Permissions</span></span>
<span data-ttu-id="4e1e0-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4e1e0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="4e1e0-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="4e1e0-108">Permission type</span></span>                        | <span data-ttu-id="4e1e0-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="4e1e0-109">Permissions (from least to most privileged)</span></span>  |
|:---------------------------------------|:-------------------------------------------- |
| <span data-ttu-id="4e1e0-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4e1e0-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="4e1e0-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4e1e0-111">Group.ReadWrite.All</span></span> |
| <span data-ttu-id="4e1e0-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4e1e0-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4e1e0-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="4e1e0-113">Not supported.</span></span> |
| <span data-ttu-id="4e1e0-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="4e1e0-114">Application</span></span>                            | <span data-ttu-id="4e1e0-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="4e1e0-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="4e1e0-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4e1e0-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}/rejectedSenders/$ref?$id=https://graph.microsoft.com/v1.0/users/{user-id}
DELETE /groups/{id}/rejectedSenders/$ref?$id=https://graph.microsoft.com/v1.0/groups/{other-group-id}
```

## <a name="request-headers"></a><span data-ttu-id="4e1e0-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="4e1e0-117">Request headers</span></span>

| <span data-ttu-id="4e1e0-118">标头</span><span class="sxs-lookup"><span data-stu-id="4e1e0-118">Header</span></span>         | <span data-ttu-id="4e1e0-119">值</span><span class="sxs-lookup"><span data-stu-id="4e1e0-119">Value</span></span>                      |
|:---------------|:---------------------------|
| <span data-ttu-id="4e1e0-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="4e1e0-120">Authorization</span></span>  | <span data-ttu-id="4e1e0-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="4e1e0-p102">Bearer {token}. Required.</span></span> 

## <a name="request-body"></a><span data-ttu-id="4e1e0-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="4e1e0-123">Request body</span></span>
<span data-ttu-id="4e1e0-124">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="4e1e0-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4e1e0-125">响应</span><span class="sxs-lookup"><span data-stu-id="4e1e0-125">Response</span></span>
<span data-ttu-id="4e1e0-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="4e1e0-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4e1e0-128">示例</span><span class="sxs-lookup"><span data-stu-id="4e1e0-128">Example</span></span>
#### <a name="request"></a><span data-ttu-id="4e1e0-129">请求</span><span class="sxs-lookup"><span data-stu-id="4e1e0-129">Request</span></span>
<span data-ttu-id="4e1e0-130">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="4e1e0-130">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="4e1e0-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="4e1e0-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "remove_rejectedSender_from_group"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/groups/{id}/rejectedSenders/$ref?$id=https://graph.microsoft.com/v1.0/users/{user-id}
```
# <a name="c"></a>[<span data-ttu-id="4e1e0-132">C#</span><span class="sxs-lookup"><span data-stu-id="4e1e0-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/remove-rejectedsender-from-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4e1e0-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4e1e0-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/remove-rejectedsender-from-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4e1e0-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4e1e0-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/remove-rejectedsender-from-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="4e1e0-135">Java</span><span class="sxs-lookup"><span data-stu-id="4e1e0-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/remove-rejectedsender-from-group-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="4e1e0-136">响应</span><span class="sxs-lookup"><span data-stu-id="4e1e0-136">Response</span></span>
<span data-ttu-id="4e1e0-137">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="4e1e0-137">The following is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Remove rejectedSender",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

