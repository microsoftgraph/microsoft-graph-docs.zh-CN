---
title: 删除用户 - Microsoft Graph API
description: 介绍删除 Microsoft Graph API (REST) 的用户资源（实体）的方法。
author: krbain
localization_priority: Priority
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: 3a8b5110682815a54878a104b69ed0552ca6548e
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50132886"
---
# <a name="delete-a-user"></a><span data-ttu-id="2e88e-103">删除用户</span><span class="sxs-lookup"><span data-stu-id="2e88e-103">Delete a user</span></span>

<span data-ttu-id="2e88e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2e88e-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="2e88e-105">删除用户。</span><span class="sxs-lookup"><span data-stu-id="2e88e-105">Delete user.</span></span>  

<span data-ttu-id="2e88e-106">删除时，将用户资源转移到存储时限为 30 日的临时容器中。</span><span class="sxs-lookup"><span data-stu-id="2e88e-106">When deleted, user resources are moved to a temporary container and can be restored within 30 days.</span></span>  <span data-ttu-id="2e88e-107">此后，它们将被永久删除。</span><span class="sxs-lookup"><span data-stu-id="2e88e-107">After that time, they are permanently deleted.</span></span>  <span data-ttu-id="2e88e-108">要了解详细信息，请参阅 [deletedItems](../resources/directory.md)。</span><span class="sxs-lookup"><span data-stu-id="2e88e-108">To learn more, see [deletedItems](../resources/directory.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="2e88e-109">权限</span><span class="sxs-lookup"><span data-stu-id="2e88e-109">Permissions</span></span>

<span data-ttu-id="2e88e-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2e88e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2e88e-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="2e88e-112">Permission type</span></span>      | <span data-ttu-id="2e88e-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="2e88e-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2e88e-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2e88e-114">Delegated (work or school account)</span></span> | <span data-ttu-id="2e88e-115">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="2e88e-115">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="2e88e-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2e88e-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2e88e-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="2e88e-117">Not supported.</span></span>    |
|<span data-ttu-id="2e88e-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="2e88e-118">Application</span></span> | <span data-ttu-id="2e88e-119">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2e88e-119">User.ReadWrite.All</span></span> |

<span data-ttu-id="2e88e-120">工作或学校帐户必须具有以下角色之一：</span><span class="sxs-lookup"><span data-stu-id="2e88e-120">The work or school account must be in one of the following roles:</span></span>
+ <span data-ttu-id="2e88e-121">全局管理员</span><span class="sxs-lookup"><span data-stu-id="2e88e-121">Global Administrator</span></span>
+ <span data-ttu-id="2e88e-122">用户管理员</span><span class="sxs-lookup"><span data-stu-id="2e88e-122">User Administrator</span></span>

<span data-ttu-id="2e88e-123">只有全局管理员才能删除全局管理员角色的用户或删除租户中的 _任何_ 用户。</span><span class="sxs-lookup"><span data-stu-id="2e88e-123">Only a Global Administrator can delete a user in a Global Administrator role  or _any_ user in the tenant.</span></span> <span data-ttu-id="2e88e-124">用户管理员只能删除非管理员或特定有限角色的用户。</span><span class="sxs-lookup"><span data-stu-id="2e88e-124">A User Administrator can only delete users who are non-administrators or in specific limited roles.</span></span> <span data-ttu-id="2e88e-125">有关详细信息，请参阅 [Azure AD 中管理员角色权限](/azure/active-directory/roles/permissions-reference#available-roles)。</span><span class="sxs-lookup"><span data-stu-id="2e88e-125">For more details, see [Administrator role permissions in Azure AD](/azure/active-directory/roles/permissions-reference#available-roles).</span></span>

## <a name="http-request"></a><span data-ttu-id="2e88e-126">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2e88e-126">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
DELETE /users/{id | userPrincipalName}
```

## <a name="request-headers"></a><span data-ttu-id="2e88e-127">请求标头</span><span class="sxs-lookup"><span data-stu-id="2e88e-127">Request headers</span></span>

| <span data-ttu-id="2e88e-128">标头</span><span class="sxs-lookup"><span data-stu-id="2e88e-128">Header</span></span>       | <span data-ttu-id="2e88e-129">值</span><span class="sxs-lookup"><span data-stu-id="2e88e-129">Value</span></span>|
|:-----------|:------|
| <span data-ttu-id="2e88e-130">Authorization</span><span class="sxs-lookup"><span data-stu-id="2e88e-130">Authorization</span></span>  | <span data-ttu-id="2e88e-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="2e88e-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="2e88e-133">请求正文</span><span class="sxs-lookup"><span data-stu-id="2e88e-133">Request body</span></span>

<span data-ttu-id="2e88e-134">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="2e88e-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2e88e-135">响应</span><span class="sxs-lookup"><span data-stu-id="2e88e-135">Response</span></span>

<span data-ttu-id="2e88e-p105">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="2e88e-p105">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2e88e-138">示例</span><span class="sxs-lookup"><span data-stu-id="2e88e-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="2e88e-139">请求</span><span class="sxs-lookup"><span data-stu-id="2e88e-139">Request</span></span>

<span data-ttu-id="2e88e-140">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="2e88e-140">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="2e88e-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="2e88e-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_user"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/users/{user-id}
```
# <a name="c"></a>[<span data-ttu-id="2e88e-142">C#</span><span class="sxs-lookup"><span data-stu-id="2e88e-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-user-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2e88e-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2e88e-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-user-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2e88e-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2e88e-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-user-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="2e88e-145">Java</span><span class="sxs-lookup"><span data-stu-id="2e88e-145">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-user-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="2e88e-146">响应</span><span class="sxs-lookup"><span data-stu-id="2e88e-146">Response</span></span>

<span data-ttu-id="2e88e-147">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="2e88e-147">Here is an example of the response.</span></span> 
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

