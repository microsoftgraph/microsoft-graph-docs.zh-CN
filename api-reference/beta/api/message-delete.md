---
title: 删除邮件
description: 删除指定用户的邮箱中的邮件, 或删除邮件的关系。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: cd4141dbf6ab8f55990ff494fc61167f1ea8758c
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35448248"
---
# <a name="delete-message"></a><span data-ttu-id="fe504-103">删除邮件</span><span class="sxs-lookup"><span data-stu-id="fe504-103">Delete message</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fe504-104">删除指定用户的邮箱中的邮件, 或删除邮件的关系。</span><span class="sxs-lookup"><span data-stu-id="fe504-104">Delete a message in the specified user's mailbox, or delete a relationship of the message.</span></span>

<span data-ttu-id="fe504-105">例如, 您可以在邮件中删除特定的[@-提及](../resources/mention.md)指定用户。</span><span class="sxs-lookup"><span data-stu-id="fe504-105">For example, you can delete a specific [@-mention](../resources/mention.md) of the specified user in the message.</span></span>

><span data-ttu-id="fe504-106">**注释**您可能无法删除 "可恢复的项目删除" 文件夹中的项目 (由[已知文件夹名称](../resources/mailfolder.md) `recoverableitemsdeletions`表示)。</span><span class="sxs-lookup"><span data-stu-id="fe504-106">**Note** You may not be able to delete items in the recoverable items deletions folder (represented by the [well-known folder name](../resources/mailfolder.md) `recoverableitemsdeletions`).</span></span> <span data-ttu-id="fe504-107">有关详细信息, 请参阅[已删除邮件保留](https://docs.microsoft.com/en-us/exchange/policy-and-compliance/recoverable-items-folder/recoverable-items-folder#deleted-item-retention)和[清除已删除项目](https://docs.microsoft.com/en-us/exchange/policy-and-compliance/recoverable-items-folder/clean-up-deleted-items)。</span><span class="sxs-lookup"><span data-stu-id="fe504-107">See [Deleted item retention](https://docs.microsoft.com/en-us/exchange/policy-and-compliance/recoverable-items-folder/recoverable-items-folder#deleted-item-retention) and [Clean up deleted items](https://docs.microsoft.com/en-us/exchange/policy-and-compliance/recoverable-items-folder/clean-up-deleted-items) for more information.</span></span>

## <a name="permissions"></a><span data-ttu-id="fe504-108">权限</span><span class="sxs-lookup"><span data-stu-id="fe504-108">Permissions</span></span>
<span data-ttu-id="fe504-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="fe504-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fe504-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="fe504-111">Permission type</span></span>      | <span data-ttu-id="fe504-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="fe504-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fe504-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="fe504-113">Delegated (work or school account)</span></span> | <span data-ttu-id="fe504-114">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="fe504-114">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="fe504-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="fe504-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fe504-116">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="fe504-116">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="fe504-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="fe504-117">Application</span></span> | <span data-ttu-id="fe504-118">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="fe504-118">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="fe504-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="fe504-119">HTTP request</span></span>

<span data-ttu-id="fe504-120">要删除指定的邮件, 请执行以下操作:</span><span class="sxs-lookup"><span data-stu-id="fe504-120">To delete the specified message:</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/messages/{id}
DELETE /users/{id | userPrincipalName}/messages/{id}
DELETE /me/mailFolders/{id}/messages/{id}
DELETE /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}
```

<span data-ttu-id="fe504-121">删除邮件中的特定[提及](../resources/mention.md):</span><span class="sxs-lookup"><span data-stu-id="fe504-121">To delete a specific [mention](../resources/mention.md) in a message:</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/messages/{id}/mentions/{id}
DELETE /users/{id | userPrincipalName}/messages/{id}/mentions/{id}
DELETE /me/mailFolders/{id}/messages/{id}/mentions/{id}
DELETE /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/mentions/{id}
```

## <a name="request-headers"></a><span data-ttu-id="fe504-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="fe504-122">Request headers</span></span>
| <span data-ttu-id="fe504-123">名称</span><span class="sxs-lookup"><span data-stu-id="fe504-123">Name</span></span>       | <span data-ttu-id="fe504-124">类型</span><span class="sxs-lookup"><span data-stu-id="fe504-124">Type</span></span> | <span data-ttu-id="fe504-125">说明</span><span class="sxs-lookup"><span data-stu-id="fe504-125">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="fe504-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="fe504-126">Authorization</span></span>  | <span data-ttu-id="fe504-127">string</span><span class="sxs-lookup"><span data-stu-id="fe504-127">string</span></span>  | <span data-ttu-id="fe504-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="fe504-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="fe504-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="fe504-130">Request body</span></span>
<span data-ttu-id="fe504-131">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="fe504-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fe504-132">响应</span><span class="sxs-lookup"><span data-stu-id="fe504-132">Response</span></span>

<span data-ttu-id="fe504-p104">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="fe504-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fe504-135">示例</span><span class="sxs-lookup"><span data-stu-id="fe504-135">Example</span></span>
##### <a name="request-1"></a><span data-ttu-id="fe504-136">请求 1</span><span class="sxs-lookup"><span data-stu-id="fe504-136">Request 1</span></span>
<span data-ttu-id="fe504-137">第一个示例删除指定的邮件。</span><span class="sxs-lookup"><span data-stu-id="fe504-137">The first example deletes the specified message.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="fe504-138">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="fe504-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_message"
}-->
```http
DELETE https://graph.microsoft.com/beta/me/messages/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="fe504-139">C#</span><span class="sxs-lookup"><span data-stu-id="fe504-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-message-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="fe504-140">Javascript</span><span class="sxs-lookup"><span data-stu-id="fe504-140">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-message-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="fe504-141">目标-C</span><span class="sxs-lookup"><span data-stu-id="fe504-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-message-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response-1"></a><span data-ttu-id="fe504-142">响应 1</span><span class="sxs-lookup"><span data-stu-id="fe504-142">Response 1</span></span>
<span data-ttu-id="fe504-143">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="fe504-143">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

##### <a name="request-2"></a><span data-ttu-id="fe504-144">请求 2</span><span class="sxs-lookup"><span data-stu-id="fe504-144">Request 2</span></span>
<span data-ttu-id="fe504-145">下一个示例将删除指定邮件中的某个**提到**。</span><span class="sxs-lookup"><span data-stu-id="fe504-145">The next example deletes a certain **mention** in the specified message.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="fe504-146">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="fe504-146">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_mention_in_message"
}-->
```http
DELETE https://graph.microsoft.com/beta/me/messages/{id}/mentions/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="fe504-147">C#</span><span class="sxs-lookup"><span data-stu-id="fe504-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-mention-in-message-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="fe504-148">Javascript</span><span class="sxs-lookup"><span data-stu-id="fe504-148">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-mention-in-message-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="fe504-149">目标-C</span><span class="sxs-lookup"><span data-stu-id="fe504-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-mention-in-message-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response-2"></a><span data-ttu-id="fe504-150">响应 2</span><span class="sxs-lookup"><span data-stu-id="fe504-150">Response 2</span></span>
<span data-ttu-id="fe504-151">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="fe504-151">Here is an example of the response.</span></span> 
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
  "description": "Delete message",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
