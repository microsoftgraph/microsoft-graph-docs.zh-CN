---
title: 删除邮件
description: 删除指定用户邮箱中的邮件，或删除邮件的关系。
localization_priority: Normal
author: abheek-das
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 71ab17fa25dee8c5158d5ef166de68ca934d7ae5
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50132816"
---
# <a name="delete-message"></a><span data-ttu-id="9771b-103">删除邮件</span><span class="sxs-lookup"><span data-stu-id="9771b-103">Delete message</span></span>

<span data-ttu-id="9771b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9771b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9771b-105">删除指定用户邮箱中的邮件，或删除邮件的关系。</span><span class="sxs-lookup"><span data-stu-id="9771b-105">Delete a message in the specified user's mailbox, or delete a relationship of the message.</span></span>

<span data-ttu-id="9771b-106">例如，可以在邮件中删除指定用户的特定[@-mention。](../resources/mention.md)</span><span class="sxs-lookup"><span data-stu-id="9771b-106">For example, you can delete a specific [@-mention](../resources/mention.md) of the specified user in the message.</span></span>

><span data-ttu-id="9771b-107">**注意** 你可能无法删除由已知文件夹名称 (文件夹名称表示的可恢复邮件删除文件夹中 [](../resources/mailfolder.md) `recoverableitemsdeletions`) 。</span><span class="sxs-lookup"><span data-stu-id="9771b-107">**Note** You may not be able to delete items in the recoverable items deletions folder (represented by the [well-known folder name](../resources/mailfolder.md) `recoverableitemsdeletions`).</span></span> <span data-ttu-id="9771b-108">有关详细信息[，请参阅"已删除](/exchange/policy-and-compliance/recoverable-items-folder/recoverable-items-folder#deleted-item-retention)邮件[](/exchange/policy-and-compliance/recoverable-items-folder/clean-up-deleted-items)保留和清理已删除项目"。</span><span class="sxs-lookup"><span data-stu-id="9771b-108">See [Deleted item retention](/exchange/policy-and-compliance/recoverable-items-folder/recoverable-items-folder#deleted-item-retention) and [Clean up deleted items](/exchange/policy-and-compliance/recoverable-items-folder/clean-up-deleted-items) for more information.</span></span>

## <a name="permissions"></a><span data-ttu-id="9771b-109">权限</span><span class="sxs-lookup"><span data-stu-id="9771b-109">Permissions</span></span>
<span data-ttu-id="9771b-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9771b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9771b-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="9771b-112">Permission type</span></span>      | <span data-ttu-id="9771b-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="9771b-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9771b-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9771b-114">Delegated (work or school account)</span></span> | <span data-ttu-id="9771b-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9771b-115">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="9771b-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9771b-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9771b-117">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9771b-117">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="9771b-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="9771b-118">Application</span></span> | <span data-ttu-id="9771b-119">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9771b-119">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="9771b-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9771b-120">HTTP request</span></span>

<span data-ttu-id="9771b-121">若要删除指定邮件，请执行以下操作：</span><span class="sxs-lookup"><span data-stu-id="9771b-121">To delete the specified message:</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/messages/{id}
DELETE /users/{id | userPrincipalName}/messages/{id}
DELETE /me/mailFolders/{id}/messages/{id}
DELETE /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}
```

<span data-ttu-id="9771b-122">若要删除邮件 [中的](../resources/mention.md) 特定提及内容，请执行：</span><span class="sxs-lookup"><span data-stu-id="9771b-122">To delete a specific [mention](../resources/mention.md) in a message:</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/messages/{id}/mentions/{id}
DELETE /users/{id | userPrincipalName}/messages/{id}/mentions/{id}
DELETE /me/mailFolders/{id}/messages/{id}/mentions/{id}
DELETE /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/mentions/{id}
```

## <a name="request-headers"></a><span data-ttu-id="9771b-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="9771b-123">Request headers</span></span>
| <span data-ttu-id="9771b-124">名称</span><span class="sxs-lookup"><span data-stu-id="9771b-124">Name</span></span>       | <span data-ttu-id="9771b-125">类型</span><span class="sxs-lookup"><span data-stu-id="9771b-125">Type</span></span> | <span data-ttu-id="9771b-126">说明</span><span class="sxs-lookup"><span data-stu-id="9771b-126">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="9771b-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="9771b-127">Authorization</span></span>  | <span data-ttu-id="9771b-128">string</span><span class="sxs-lookup"><span data-stu-id="9771b-128">string</span></span>  | <span data-ttu-id="9771b-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="9771b-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9771b-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="9771b-131">Request body</span></span>
<span data-ttu-id="9771b-132">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="9771b-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9771b-133">响应</span><span class="sxs-lookup"><span data-stu-id="9771b-133">Response</span></span>

<span data-ttu-id="9771b-p104">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="9771b-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9771b-136">示例</span><span class="sxs-lookup"><span data-stu-id="9771b-136">Example</span></span>
##### <a name="request-1"></a><span data-ttu-id="9771b-137">请求 1</span><span class="sxs-lookup"><span data-stu-id="9771b-137">Request 1</span></span>
<span data-ttu-id="9771b-138">第一个示例删除指定的邮件。</span><span class="sxs-lookup"><span data-stu-id="9771b-138">The first example deletes the specified message.</span></span>

# <a name="http"></a>[<span data-ttu-id="9771b-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="9771b-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_message"
}-->
```http
DELETE https://graph.microsoft.com/beta/me/messages/{id}
```
# <a name="c"></a>[<span data-ttu-id="9771b-140">C#</span><span class="sxs-lookup"><span data-stu-id="9771b-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-message-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9771b-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9771b-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-message-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9771b-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9771b-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-message-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="9771b-143">Java</span><span class="sxs-lookup"><span data-stu-id="9771b-143">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-message-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response-1"></a><span data-ttu-id="9771b-144">响应 1</span><span class="sxs-lookup"><span data-stu-id="9771b-144">Response 1</span></span>
<span data-ttu-id="9771b-145">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="9771b-145">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

##### <a name="request-2"></a><span data-ttu-id="9771b-146">请求 2</span><span class="sxs-lookup"><span data-stu-id="9771b-146">Request 2</span></span>
<span data-ttu-id="9771b-147">下一个示例删除 **指定邮件中的** 特定提及内容。</span><span class="sxs-lookup"><span data-stu-id="9771b-147">The next example deletes a certain **mention** in the specified message.</span></span>

# <a name="http"></a>[<span data-ttu-id="9771b-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="9771b-148">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_mention_in_message"
}-->
```http
DELETE https://graph.microsoft.com/beta/me/messages/{id}/mentions/{id}
```
# <a name="c"></a>[<span data-ttu-id="9771b-149">C#</span><span class="sxs-lookup"><span data-stu-id="9771b-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-mention-in-message-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9771b-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9771b-150">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-mention-in-message-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9771b-151">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9771b-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-mention-in-message-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="9771b-152">Java</span><span class="sxs-lookup"><span data-stu-id="9771b-152">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-mention-in-message-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response-2"></a><span data-ttu-id="9771b-153">响应 2</span><span class="sxs-lookup"><span data-stu-id="9771b-153">Response 2</span></span>
<span data-ttu-id="9771b-154">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="9771b-154">Here is an example of the response.</span></span>
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


