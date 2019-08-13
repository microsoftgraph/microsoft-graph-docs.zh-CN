---
title: 删除用户 - Microsoft Graph API
description: 介绍删除 Microsoft Graph API (REST) 的用户资源（实体）的方法。
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: d1dc586596fe6f46861094b1f1913787f49ccfd6
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36362486"
---
# <a name="delete-a-user"></a><span data-ttu-id="ec197-103">删除用户</span><span class="sxs-lookup"><span data-stu-id="ec197-103">Delete a user</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ec197-104">删除用户。</span><span class="sxs-lookup"><span data-stu-id="ec197-104">Delete user.</span></span>  

<span data-ttu-id="ec197-105">删除时，将用户资源转移到存储时限为 30 日的临时容器中。</span><span class="sxs-lookup"><span data-stu-id="ec197-105">When deleted, user resources are moved to a temporary container and can be restored within 30 days.</span></span>  <span data-ttu-id="ec197-106">此后，它们将被永久删除。</span><span class="sxs-lookup"><span data-stu-id="ec197-106">After that time, they are permanently deleted.</span></span>  <span data-ttu-id="ec197-107">要了解详细信息，请参阅 [deletedItems](../resources/directory.md)。</span><span class="sxs-lookup"><span data-stu-id="ec197-107">To learn more, see [deletedItems](../resources/directory.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="ec197-108">权限</span><span class="sxs-lookup"><span data-stu-id="ec197-108">Permissions</span></span>

<span data-ttu-id="ec197-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ec197-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ec197-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="ec197-111">Permission type</span></span>      | <span data-ttu-id="ec197-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ec197-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ec197-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ec197-113">Delegated (work or school account)</span></span> | <span data-ttu-id="ec197-114">User.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="ec197-114">User.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="ec197-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ec197-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ec197-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="ec197-116">Not supported.</span></span>    |
|<span data-ttu-id="ec197-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="ec197-117">Application</span></span> | <span data-ttu-id="ec197-118">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ec197-118">User.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ec197-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ec197-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
DELETE /users/{id | userPrincipalName}
```

## <a name="request-headers"></a><span data-ttu-id="ec197-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="ec197-120">Request headers</span></span>

| <span data-ttu-id="ec197-121">标头</span><span class="sxs-lookup"><span data-stu-id="ec197-121">Header</span></span>       | <span data-ttu-id="ec197-122">值</span><span class="sxs-lookup"><span data-stu-id="ec197-122">Value</span></span>|
|:-----------|:------|
| <span data-ttu-id="ec197-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="ec197-123">Authorization</span></span>  | <span data-ttu-id="ec197-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="ec197-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="ec197-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="ec197-126">Request body</span></span>

<span data-ttu-id="ec197-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="ec197-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ec197-128">响应</span><span class="sxs-lookup"><span data-stu-id="ec197-128">Response</span></span>

<span data-ttu-id="ec197-p104">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="ec197-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ec197-131">示例</span><span class="sxs-lookup"><span data-stu-id="ec197-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="ec197-132">请求</span><span class="sxs-lookup"><span data-stu-id="ec197-132">Request</span></span>

<span data-ttu-id="ec197-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="ec197-133">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="ec197-134">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="ec197-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_user"
}-->
```http
DELETE https://graph.microsoft.com/beta/users/ba9a3254-9f18-4209-aeb3-9e42a35b5be4 
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="ec197-135">C#</span><span class="sxs-lookup"><span data-stu-id="ec197-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-user-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="ec197-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ec197-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-user-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="ec197-137">目标-C</span><span class="sxs-lookup"><span data-stu-id="ec197-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-user-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="ec197-138">Java</span><span class="sxs-lookup"><span data-stu-id="ec197-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-user-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="ec197-139">响应</span><span class="sxs-lookup"><span data-stu-id="ec197-139">Response</span></span>

<span data-ttu-id="ec197-140">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="ec197-140">Here is an example of the response.</span></span> 
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
  "description": "Delete user",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
