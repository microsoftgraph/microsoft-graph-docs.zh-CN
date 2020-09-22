---
title: 删除用户 - Microsoft Graph API
description: 介绍删除 Microsoft Graph API (REST) 的用户资源（实体）的方法。
author: krbain
localization_priority: Priority
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: b4ecb9ebf2b022ebdddd41e5b63595b55ca49154
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48037946"
---
# <a name="delete-a-user"></a><span data-ttu-id="840aa-103">删除用户</span><span class="sxs-lookup"><span data-stu-id="840aa-103">Delete a user</span></span>

<span data-ttu-id="840aa-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="840aa-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="840aa-105">删除用户。</span><span class="sxs-lookup"><span data-stu-id="840aa-105">Delete user.</span></span>  

<span data-ttu-id="840aa-106">删除时，将用户资源转移到存储时限为 30 日的临时容器中。</span><span class="sxs-lookup"><span data-stu-id="840aa-106">When deleted, user resources are moved to a temporary container and can be restored within 30 days.</span></span>  <span data-ttu-id="840aa-107">此后，它们将被永久删除。</span><span class="sxs-lookup"><span data-stu-id="840aa-107">After that time, they are permanently deleted.</span></span>  <span data-ttu-id="840aa-108">要了解详细信息，请参阅 [deletedItems](../resources/directory.md)。</span><span class="sxs-lookup"><span data-stu-id="840aa-108">To learn more, see [deletedItems](../resources/directory.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="840aa-109">权限</span><span class="sxs-lookup"><span data-stu-id="840aa-109">Permissions</span></span>

<span data-ttu-id="840aa-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="840aa-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="840aa-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="840aa-112">Permission type</span></span>      | <span data-ttu-id="840aa-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="840aa-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="840aa-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="840aa-114">Delegated (work or school account)</span></span> | <span data-ttu-id="840aa-115">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="840aa-115">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="840aa-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="840aa-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="840aa-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="840aa-117">Not supported.</span></span>    |
|<span data-ttu-id="840aa-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="840aa-118">Application</span></span> | <span data-ttu-id="840aa-119">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="840aa-119">User.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="840aa-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="840aa-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
DELETE /users/{id | userPrincipalName}
```

## <a name="request-headers"></a><span data-ttu-id="840aa-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="840aa-121">Request headers</span></span>

| <span data-ttu-id="840aa-122">标头</span><span class="sxs-lookup"><span data-stu-id="840aa-122">Header</span></span>       | <span data-ttu-id="840aa-123">值</span><span class="sxs-lookup"><span data-stu-id="840aa-123">Value</span></span>|
|:-----------|:------|
| <span data-ttu-id="840aa-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="840aa-124">Authorization</span></span>  | <span data-ttu-id="840aa-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="840aa-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="840aa-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="840aa-127">Request body</span></span>

<span data-ttu-id="840aa-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="840aa-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="840aa-129">响应</span><span class="sxs-lookup"><span data-stu-id="840aa-129">Response</span></span>

<span data-ttu-id="840aa-p104">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="840aa-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="840aa-132">示例</span><span class="sxs-lookup"><span data-stu-id="840aa-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="840aa-133">请求</span><span class="sxs-lookup"><span data-stu-id="840aa-133">Request</span></span>

<span data-ttu-id="840aa-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="840aa-134">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="840aa-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="840aa-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_user"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/users/{user-id}
```
# <a name="c"></a>[<span data-ttu-id="840aa-136">C#</span><span class="sxs-lookup"><span data-stu-id="840aa-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-user-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="840aa-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="840aa-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-user-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="840aa-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="840aa-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-user-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="840aa-139">Java</span><span class="sxs-lookup"><span data-stu-id="840aa-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-user-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="840aa-140">响应</span><span class="sxs-lookup"><span data-stu-id="840aa-140">Response</span></span>

<span data-ttu-id="840aa-141">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="840aa-141">Here is an example of the response.</span></span> 
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
  "description": "Delete user",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

