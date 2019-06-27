---
title: 删除用户 - Microsoft Graph API
description: 介绍删除 Microsoft Graph API (REST) 的用户资源（实体）的方法。
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 4ee725065269313e2b596305888d157edecdcc5f
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35270376"
---
# <a name="delete-a-user"></a><span data-ttu-id="02a42-103">删除用户</span><span class="sxs-lookup"><span data-stu-id="02a42-103">Delete a user</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="02a42-104">删除用户。</span><span class="sxs-lookup"><span data-stu-id="02a42-104">Delete user.</span></span>  

<span data-ttu-id="02a42-105">删除时，将用户资源转移到存储时限为 30 日的临时容器中。</span><span class="sxs-lookup"><span data-stu-id="02a42-105">When deleted, user resources are moved to a temporary container and can be restored within 30 days.</span></span>  <span data-ttu-id="02a42-106">此后，它们将被永久删除。</span><span class="sxs-lookup"><span data-stu-id="02a42-106">After that time, they are permanently deleted.</span></span>  <span data-ttu-id="02a42-107">要了解详细信息，请参阅 [deletedItems](../resources/directory.md)。</span><span class="sxs-lookup"><span data-stu-id="02a42-107">To learn more, see [deletedItems](../resources/directory.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="02a42-108">权限</span><span class="sxs-lookup"><span data-stu-id="02a42-108">Permissions</span></span>

<span data-ttu-id="02a42-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="02a42-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="02a42-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="02a42-111">Permission type</span></span>      | <span data-ttu-id="02a42-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="02a42-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="02a42-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="02a42-113">Delegated (work or school account)</span></span> | <span data-ttu-id="02a42-114">User.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="02a42-114">User.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="02a42-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="02a42-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="02a42-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="02a42-116">Not supported.</span></span>    |
|<span data-ttu-id="02a42-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="02a42-117">Application</span></span> | <span data-ttu-id="02a42-118">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="02a42-118">User.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="02a42-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="02a42-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
DELETE /users/{id | userPrincipalName}
```

## <a name="request-headers"></a><span data-ttu-id="02a42-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="02a42-120">Request headers</span></span>

| <span data-ttu-id="02a42-121">标头</span><span class="sxs-lookup"><span data-stu-id="02a42-121">Header</span></span>       | <span data-ttu-id="02a42-122">值</span><span class="sxs-lookup"><span data-stu-id="02a42-122">Value</span></span>|
|:-----------|:------|
| <span data-ttu-id="02a42-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="02a42-123">Authorization</span></span>  | <span data-ttu-id="02a42-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="02a42-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="02a42-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="02a42-126">Request body</span></span>

<span data-ttu-id="02a42-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="02a42-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="02a42-128">响应</span><span class="sxs-lookup"><span data-stu-id="02a42-128">Response</span></span>

<span data-ttu-id="02a42-p104">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="02a42-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="02a42-131">示例</span><span class="sxs-lookup"><span data-stu-id="02a42-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="02a42-132">请求</span><span class="sxs-lookup"><span data-stu-id="02a42-132">Request</span></span>

<span data-ttu-id="02a42-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="02a42-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_user"
}-->
```http
DELETE https://graph.microsoft.com/beta/users/ba9a3254-9f18-4209-aeb3-9e42a35b5be4 
```
### <a name="response"></a><span data-ttu-id="02a42-134">响应</span><span class="sxs-lookup"><span data-stu-id="02a42-134">Response</span></span>

<span data-ttu-id="02a42-135">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="02a42-135">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="02a42-136">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="02a42-136">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="02a42-137">C#</span><span class="sxs-lookup"><span data-stu-id="02a42-137">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/delete_user-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="02a42-138">Javascript</span><span class="sxs-lookup"><span data-stu-id="02a42-138">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/delete_user-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="02a42-139">目标-C</span><span class="sxs-lookup"><span data-stu-id="02a42-139">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/delete_user-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/user-delete.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/user-delete.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/user-delete.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
