---
title: 删除用户 - Microsoft Graph API
description: 介绍删除 Microsoft Graph API (REST) 的用户资源（实体）的方法。
author: dkershaw10
localization_priority: Priority
ms.prod: microsoft-identity-platform
ms.openlocfilehash: fef9dc57e7630bb210868674a575dca993f1e8c8
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35460551"
---
# <a name="delete-a-user"></a><span data-ttu-id="1bbf0-103">删除用户</span><span class="sxs-lookup"><span data-stu-id="1bbf0-103">Delete a user</span></span>

<span data-ttu-id="1bbf0-104">删除用户。</span><span class="sxs-lookup"><span data-stu-id="1bbf0-104">Delete user.</span></span>  

<span data-ttu-id="1bbf0-105">删除时，将用户资源转移到存储时限为 30 日的临时容器中。</span><span class="sxs-lookup"><span data-stu-id="1bbf0-105">When deleted, user resources are moved to a temporary container and can be restored within 30 days.</span></span>  <span data-ttu-id="1bbf0-106">此后，它们将被永久删除。</span><span class="sxs-lookup"><span data-stu-id="1bbf0-106">After that time, they are permanently deleted.</span></span>  <span data-ttu-id="1bbf0-107">要了解详细信息，请参阅 [deletedItems](../resources/directory.md)。</span><span class="sxs-lookup"><span data-stu-id="1bbf0-107">To learn more, see [deletedItems](../resources/directory.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="1bbf0-108">权限</span><span class="sxs-lookup"><span data-stu-id="1bbf0-108">Permissions</span></span>

<span data-ttu-id="1bbf0-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="1bbf0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1bbf0-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="1bbf0-111">Permission type</span></span>      | <span data-ttu-id="1bbf0-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="1bbf0-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1bbf0-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1bbf0-113">Delegated (work or school account)</span></span> | <span data-ttu-id="1bbf0-114">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="1bbf0-114">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="1bbf0-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1bbf0-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1bbf0-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="1bbf0-116">Not supported.</span></span>    |
|<span data-ttu-id="1bbf0-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="1bbf0-117">Application</span></span> | <span data-ttu-id="1bbf0-118">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1bbf0-118">User.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="1bbf0-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1bbf0-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
DELETE /users/{id | userPrincipalName}
```

## <a name="request-headers"></a><span data-ttu-id="1bbf0-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="1bbf0-120">Request headers</span></span>

| <span data-ttu-id="1bbf0-121">标头</span><span class="sxs-lookup"><span data-stu-id="1bbf0-121">Header</span></span>       | <span data-ttu-id="1bbf0-122">值</span><span class="sxs-lookup"><span data-stu-id="1bbf0-122">Value</span></span>|
|:-----------|:------|
| <span data-ttu-id="1bbf0-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="1bbf0-123">Authorization</span></span>  | <span data-ttu-id="1bbf0-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="1bbf0-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="1bbf0-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="1bbf0-126">Request body</span></span>

<span data-ttu-id="1bbf0-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="1bbf0-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1bbf0-128">响应</span><span class="sxs-lookup"><span data-stu-id="1bbf0-128">Response</span></span>

<span data-ttu-id="1bbf0-p104">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="1bbf0-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1bbf0-131">示例</span><span class="sxs-lookup"><span data-stu-id="1bbf0-131">Example</span></span>

## <a name="request"></a><span data-ttu-id="1bbf0-132">请求</span><span class="sxs-lookup"><span data-stu-id="1bbf0-132">Request</span></span>

<span data-ttu-id="1bbf0-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="1bbf0-133">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="1bbf0-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="1bbf0-134">--Http</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_user"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/users/{user-id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="1bbf0-135">C#</span><span class="sxs-lookup"><span data-stu-id="1bbf0-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-user-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="1bbf0-136">Javascript</span><span class="sxs-lookup"><span data-stu-id="1bbf0-136">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-user-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="1bbf0-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1bbf0-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-user-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="1bbf0-138">响应</span><span class="sxs-lookup"><span data-stu-id="1bbf0-138">Response</span></span>

<span data-ttu-id="1bbf0-139">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="1bbf0-139">Here is an example of the response.</span></span> 
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
