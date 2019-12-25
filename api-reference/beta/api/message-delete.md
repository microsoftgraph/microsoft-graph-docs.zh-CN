---
title: 删除邮件
description: 删除指定用户的邮箱中的邮件，或删除邮件的关系。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 70854305f87546f716b56fdc53122b11c7b56dec
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "40867811"
---
# <a name="delete-message"></a><span data-ttu-id="8ba84-103">删除邮件</span><span class="sxs-lookup"><span data-stu-id="8ba84-103">Delete message</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8ba84-104">删除指定用户的邮箱中的邮件，或删除邮件的关系。</span><span class="sxs-lookup"><span data-stu-id="8ba84-104">Delete a message in the specified user's mailbox, or delete a relationship of the message.</span></span>

<span data-ttu-id="8ba84-105">例如，您可以在邮件中删除特定的[@-提及](../resources/mention.md)指定用户。</span><span class="sxs-lookup"><span data-stu-id="8ba84-105">For example, you can delete a specific [@-mention](../resources/mention.md) of the specified user in the message.</span></span>

><span data-ttu-id="8ba84-106">**注释**您可能无法删除 "可恢复的项目删除" 文件夹中的项目（由[已知文件夹名称](../resources/mailfolder.md) `recoverableitemsdeletions`表示）。</span><span class="sxs-lookup"><span data-stu-id="8ba84-106">**Note** You may not be able to delete items in the recoverable items deletions folder (represented by the [well-known folder name](../resources/mailfolder.md) `recoverableitemsdeletions`).</span></span> <span data-ttu-id="8ba84-107">有关详细信息，请参阅[已删除邮件保留](/exchange/policy-and-compliance/recoverable-items-folder/recoverable-items-folder#deleted-item-retention)和[清除已删除项目](/exchange/policy-and-compliance/recoverable-items-folder/clean-up-deleted-items)。</span><span class="sxs-lookup"><span data-stu-id="8ba84-107">See [Deleted item retention](/exchange/policy-and-compliance/recoverable-items-folder/recoverable-items-folder#deleted-item-retention) and [Clean up deleted items](/exchange/policy-and-compliance/recoverable-items-folder/clean-up-deleted-items) for more information.</span></span>

## <a name="permissions"></a><span data-ttu-id="8ba84-108">权限</span><span class="sxs-lookup"><span data-stu-id="8ba84-108">Permissions</span></span>
<span data-ttu-id="8ba84-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8ba84-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8ba84-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="8ba84-111">Permission type</span></span>      | <span data-ttu-id="8ba84-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="8ba84-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8ba84-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8ba84-113">Delegated (work or school account)</span></span> | <span data-ttu-id="8ba84-114">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8ba84-114">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="8ba84-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8ba84-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8ba84-116">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8ba84-116">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="8ba84-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="8ba84-117">Application</span></span> | <span data-ttu-id="8ba84-118">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8ba84-118">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="8ba84-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8ba84-119">HTTP request</span></span>

<span data-ttu-id="8ba84-120">要删除指定的邮件，请执行以下操作：</span><span class="sxs-lookup"><span data-stu-id="8ba84-120">To delete the specified message:</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/messages/{id}
DELETE /users/{id | userPrincipalName}/messages/{id}
DELETE /me/mailFolders/{id}/messages/{id}
DELETE /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}
```

<span data-ttu-id="8ba84-121">删除邮件中的特定[提及](../resources/mention.md)：</span><span class="sxs-lookup"><span data-stu-id="8ba84-121">To delete a specific [mention](../resources/mention.md) in a message:</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/messages/{id}/mentions/{id}
DELETE /users/{id | userPrincipalName}/messages/{id}/mentions/{id}
DELETE /me/mailFolders/{id}/messages/{id}/mentions/{id}
DELETE /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/mentions/{id}
```

## <a name="request-headers"></a><span data-ttu-id="8ba84-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="8ba84-122">Request headers</span></span>
| <span data-ttu-id="8ba84-123">名称</span><span class="sxs-lookup"><span data-stu-id="8ba84-123">Name</span></span>       | <span data-ttu-id="8ba84-124">类型</span><span class="sxs-lookup"><span data-stu-id="8ba84-124">Type</span></span> | <span data-ttu-id="8ba84-125">说明</span><span class="sxs-lookup"><span data-stu-id="8ba84-125">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="8ba84-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="8ba84-126">Authorization</span></span>  | <span data-ttu-id="8ba84-127">string</span><span class="sxs-lookup"><span data-stu-id="8ba84-127">string</span></span>  | <span data-ttu-id="8ba84-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="8ba84-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8ba84-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="8ba84-130">Request body</span></span>
<span data-ttu-id="8ba84-131">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="8ba84-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8ba84-132">响应</span><span class="sxs-lookup"><span data-stu-id="8ba84-132">Response</span></span>

<span data-ttu-id="8ba84-p104">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="8ba84-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8ba84-135">示例</span><span class="sxs-lookup"><span data-stu-id="8ba84-135">Example</span></span>
##### <a name="request-1"></a><span data-ttu-id="8ba84-136">请求 1</span><span class="sxs-lookup"><span data-stu-id="8ba84-136">Request 1</span></span>
<span data-ttu-id="8ba84-137">第一个示例删除指定的邮件。</span><span class="sxs-lookup"><span data-stu-id="8ba84-137">The first example deletes the specified message.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="8ba84-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="8ba84-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_message"
}-->
```http
DELETE https://graph.microsoft.com/beta/me/messages/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="8ba84-139">C#</span><span class="sxs-lookup"><span data-stu-id="8ba84-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-message-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="8ba84-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8ba84-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-message-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="8ba84-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8ba84-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-message-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response-1"></a><span data-ttu-id="8ba84-142">响应 1</span><span class="sxs-lookup"><span data-stu-id="8ba84-142">Response 1</span></span>
<span data-ttu-id="8ba84-143">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="8ba84-143">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

##### <a name="request-2"></a><span data-ttu-id="8ba84-144">请求 2</span><span class="sxs-lookup"><span data-stu-id="8ba84-144">Request 2</span></span>
<span data-ttu-id="8ba84-145">下一个示例将删除指定邮件中的某个**提到**。</span><span class="sxs-lookup"><span data-stu-id="8ba84-145">The next example deletes a certain **mention** in the specified message.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="8ba84-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="8ba84-146">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_mention_in_message"
}-->
```http
DELETE https://graph.microsoft.com/beta/me/messages/{id}/mentions/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="8ba84-147">C#</span><span class="sxs-lookup"><span data-stu-id="8ba84-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-mention-in-message-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="8ba84-148">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8ba84-148">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-mention-in-message-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="8ba84-149">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8ba84-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-mention-in-message-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response-2"></a><span data-ttu-id="8ba84-150">响应 2</span><span class="sxs-lookup"><span data-stu-id="8ba84-150">Response 2</span></span>
<span data-ttu-id="8ba84-151">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="8ba84-151">Here is an example of the response.</span></span>
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
