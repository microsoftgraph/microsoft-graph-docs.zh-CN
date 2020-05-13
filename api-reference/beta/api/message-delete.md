---
title: 删除邮件
description: 删除指定用户的邮箱中的邮件，或删除邮件的关系。
localization_priority: Normal
author: svpsiva
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 3f69c123b72dfb876a7ed60d427b76674e1556f6
ms.sourcegitcommit: d4114bac58628527611e83e436132c6581a19c52
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/13/2020
ms.locfileid: "43448611"
---
# <a name="delete-message"></a><span data-ttu-id="3e3b5-103">删除邮件</span><span class="sxs-lookup"><span data-stu-id="3e3b5-103">Delete message</span></span>

<span data-ttu-id="3e3b5-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3e3b5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3e3b5-105">删除指定用户的邮箱中的邮件，或删除邮件的关系。</span><span class="sxs-lookup"><span data-stu-id="3e3b5-105">Delete a message in the specified user's mailbox, or delete a relationship of the message.</span></span>

<span data-ttu-id="3e3b5-106">例如，您可以在邮件中删除特定的[@-提及](../resources/mention.md)指定用户。</span><span class="sxs-lookup"><span data-stu-id="3e3b5-106">For example, you can delete a specific [@-mention](../resources/mention.md) of the specified user in the message.</span></span>

><span data-ttu-id="3e3b5-107">**注释**您可能无法删除 "可恢复的项目删除" 文件夹中的项目（由[已知文件夹名称](../resources/mailfolder.md)表示 `recoverableitemsdeletions` ）。</span><span class="sxs-lookup"><span data-stu-id="3e3b5-107">**Note** You may not be able to delete items in the recoverable items deletions folder (represented by the [well-known folder name](../resources/mailfolder.md) `recoverableitemsdeletions`).</span></span> <span data-ttu-id="3e3b5-108">有关详细信息，请参阅[已删除邮件保留](/exchange/policy-and-compliance/recoverable-items-folder/recoverable-items-folder#deleted-item-retention)和[清除已删除项目](/exchange/policy-and-compliance/recoverable-items-folder/clean-up-deleted-items)。</span><span class="sxs-lookup"><span data-stu-id="3e3b5-108">See [Deleted item retention](/exchange/policy-and-compliance/recoverable-items-folder/recoverable-items-folder#deleted-item-retention) and [Clean up deleted items](/exchange/policy-and-compliance/recoverable-items-folder/clean-up-deleted-items) for more information.</span></span>

## <a name="permissions"></a><span data-ttu-id="3e3b5-109">权限</span><span class="sxs-lookup"><span data-stu-id="3e3b5-109">Permissions</span></span>
<span data-ttu-id="3e3b5-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="3e3b5-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3e3b5-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="3e3b5-112">Permission type</span></span>      | <span data-ttu-id="3e3b5-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="3e3b5-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3e3b5-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3e3b5-114">Delegated (work or school account)</span></span> | <span data-ttu-id="3e3b5-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3e3b5-115">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="3e3b5-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3e3b5-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3e3b5-117">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3e3b5-117">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="3e3b5-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="3e3b5-118">Application</span></span> | <span data-ttu-id="3e3b5-119">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3e3b5-119">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="3e3b5-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3e3b5-120">HTTP request</span></span>

<span data-ttu-id="3e3b5-121">要删除指定的邮件，请执行以下操作：</span><span class="sxs-lookup"><span data-stu-id="3e3b5-121">To delete the specified message:</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/messages/{id}
DELETE /users/{id | userPrincipalName}/messages/{id}
DELETE /me/mailFolders/{id}/messages/{id}
DELETE /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}
```

<span data-ttu-id="3e3b5-122">删除邮件中的特定[提及](../resources/mention.md)：</span><span class="sxs-lookup"><span data-stu-id="3e3b5-122">To delete a specific [mention](../resources/mention.md) in a message:</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/messages/{id}/mentions/{id}
DELETE /users/{id | userPrincipalName}/messages/{id}/mentions/{id}
DELETE /me/mailFolders/{id}/messages/{id}/mentions/{id}
DELETE /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/mentions/{id}
```

## <a name="request-headers"></a><span data-ttu-id="3e3b5-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="3e3b5-123">Request headers</span></span>
| <span data-ttu-id="3e3b5-124">名称</span><span class="sxs-lookup"><span data-stu-id="3e3b5-124">Name</span></span>       | <span data-ttu-id="3e3b5-125">类型</span><span class="sxs-lookup"><span data-stu-id="3e3b5-125">Type</span></span> | <span data-ttu-id="3e3b5-126">说明</span><span class="sxs-lookup"><span data-stu-id="3e3b5-126">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="3e3b5-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="3e3b5-127">Authorization</span></span>  | <span data-ttu-id="3e3b5-128">string</span><span class="sxs-lookup"><span data-stu-id="3e3b5-128">string</span></span>  | <span data-ttu-id="3e3b5-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="3e3b5-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3e3b5-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="3e3b5-131">Request body</span></span>
<span data-ttu-id="3e3b5-132">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="3e3b5-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3e3b5-133">响应</span><span class="sxs-lookup"><span data-stu-id="3e3b5-133">Response</span></span>

<span data-ttu-id="3e3b5-p104">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="3e3b5-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3e3b5-136">示例</span><span class="sxs-lookup"><span data-stu-id="3e3b5-136">Example</span></span>
##### <a name="request-1"></a><span data-ttu-id="3e3b5-137">请求 1</span><span class="sxs-lookup"><span data-stu-id="3e3b5-137">Request 1</span></span>
<span data-ttu-id="3e3b5-138">第一个示例删除指定的邮件。</span><span class="sxs-lookup"><span data-stu-id="3e3b5-138">The first example deletes the specified message.</span></span>

# <a name="http"></a>[<span data-ttu-id="3e3b5-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="3e3b5-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_message"
}-->
```http
DELETE https://graph.microsoft.com/beta/me/messages/{id}
```
# <a name="c"></a>[<span data-ttu-id="3e3b5-140">C#</span><span class="sxs-lookup"><span data-stu-id="3e3b5-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-message-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3e3b5-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3e3b5-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-message-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3e3b5-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3e3b5-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-message-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response-1"></a><span data-ttu-id="3e3b5-143">响应 1</span><span class="sxs-lookup"><span data-stu-id="3e3b5-143">Response 1</span></span>
<span data-ttu-id="3e3b5-144">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="3e3b5-144">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

##### <a name="request-2"></a><span data-ttu-id="3e3b5-145">请求 2</span><span class="sxs-lookup"><span data-stu-id="3e3b5-145">Request 2</span></span>
<span data-ttu-id="3e3b5-146">下一个示例将删除指定邮件中的某个**提到**。</span><span class="sxs-lookup"><span data-stu-id="3e3b5-146">The next example deletes a certain **mention** in the specified message.</span></span>

# <a name="http"></a>[<span data-ttu-id="3e3b5-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="3e3b5-147">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_mention_in_message"
}-->
```http
DELETE https://graph.microsoft.com/beta/me/messages/{id}/mentions/{id}
```
# <a name="c"></a>[<span data-ttu-id="3e3b5-148">C#</span><span class="sxs-lookup"><span data-stu-id="3e3b5-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-mention-in-message-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3e3b5-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3e3b5-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-mention-in-message-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3e3b5-150">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3e3b5-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-mention-in-message-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response-2"></a><span data-ttu-id="3e3b5-151">响应 2</span><span class="sxs-lookup"><span data-stu-id="3e3b5-151">Response 2</span></span>
<span data-ttu-id="3e3b5-152">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="3e3b5-152">Here is an example of the response.</span></span>
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
