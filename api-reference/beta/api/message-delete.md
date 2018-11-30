---
title: 删除邮件
description: 删除指定的用户邮箱中的邮件或删除邮件的关系。
ms.openlocfilehash: 8f7429dfa4ee586f7bb6c263bdbb80971416d006
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27049067"
---
# <a name="delete-message"></a><span data-ttu-id="41d6d-103">删除邮件</span><span class="sxs-lookup"><span data-stu-id="41d6d-103">Delete message</span></span>

> <span data-ttu-id="41d6d-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="41d6d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="41d6d-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="41d6d-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="41d6d-106">删除指定的用户邮箱中的邮件或删除邮件的关系。</span><span class="sxs-lookup"><span data-stu-id="41d6d-106">Delete a message in the specified user's mailbox, or delete a relationship of the message.</span></span>

<span data-ttu-id="41d6d-107">例如，您可以删除某个特定的[@ 提及](../resources/mention.md)的消息中指定的用户。</span><span class="sxs-lookup"><span data-stu-id="41d6d-107">For example, you can delete a specific [@-mention](../resources/mention.md) of the specified user in the message.</span></span>

><span data-ttu-id="41d6d-108">**注释**您可能不能删除可恢复邮件删除文件夹中的项目 (由[已知文件夹名称](../resources/mailfolder.md) `recoverableitemsdeletions`)。</span><span class="sxs-lookup"><span data-stu-id="41d6d-108">**Note** You may not be able to delete items in the recoverable items deletions folder (represented by the [well-known folder name](../resources/mailfolder.md) `recoverableitemsdeletions`).</span></span> <span data-ttu-id="41d6d-109">有关详细信息，请参阅[已删除邮件的保留期](https://docs.microsoft.com/en-us/exchange/policy-and-compliance/recoverable-items-folder/recoverable-items-folder#deleted-item-retention)和[清理已删除项目](https://docs.microsoft.com/en-us/exchange/policy-and-compliance/recoverable-items-folder/clean-up-deleted-items)。</span><span class="sxs-lookup"><span data-stu-id="41d6d-109">See [Deleted item retention](https://docs.microsoft.com/en-us/exchange/policy-and-compliance/recoverable-items-folder/recoverable-items-folder#deleted-item-retention) and [Clean up deleted items](https://docs.microsoft.com/en-us/exchange/policy-and-compliance/recoverable-items-folder/clean-up-deleted-items) for more information.</span></span>

## <a name="permissions"></a><span data-ttu-id="41d6d-110">权限</span><span class="sxs-lookup"><span data-stu-id="41d6d-110">Permissions</span></span>
<span data-ttu-id="41d6d-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="41d6d-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="41d6d-113">权限类型</span><span class="sxs-lookup"><span data-stu-id="41d6d-113">Permission type</span></span>      | <span data-ttu-id="41d6d-114">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="41d6d-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="41d6d-115">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="41d6d-115">Delegated (work or school account)</span></span> | <span data-ttu-id="41d6d-116">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="41d6d-116">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="41d6d-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="41d6d-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="41d6d-118">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="41d6d-118">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="41d6d-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="41d6d-119">Application</span></span> | <span data-ttu-id="41d6d-120">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="41d6d-120">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="41d6d-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="41d6d-121">HTTP request</span></span>

<span data-ttu-id="41d6d-122">删除指定的消息：<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="41d6d-122">To delete the specified message: <!-- { "blockType": "ignored" } --></span></span>
```http
DELETE /me/messages/{id}
DELETE /users/{id | userPrincipalName}/messages/{id}
DELETE /me/mailFolders/{id}/messages/{id}
DELETE /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}
```

<span data-ttu-id="41d6d-123">删除特定[提及](../resources/mention.md)邮件中：<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="41d6d-123">To delete a specific [mention](../resources/mention.md) in a message: <!-- { "blockType": "ignored" } --></span></span>
```http
DELETE /me/messages/{id}/mentions/{id}
DELETE /users/{id | userPrincipalName}/messages/{id}/mentions/{id}
DELETE /me/mailFolders/{id}/messages/{id}/mentions/{id}
DELETE /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/mentions/{id}
```

## <a name="request-headers"></a><span data-ttu-id="41d6d-124">请求标头</span><span class="sxs-lookup"><span data-stu-id="41d6d-124">Request headers</span></span>
| <span data-ttu-id="41d6d-125">名称</span><span class="sxs-lookup"><span data-stu-id="41d6d-125">Name</span></span>       | <span data-ttu-id="41d6d-126">类型</span><span class="sxs-lookup"><span data-stu-id="41d6d-126">Type</span></span> | <span data-ttu-id="41d6d-127">说明</span><span class="sxs-lookup"><span data-stu-id="41d6d-127">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="41d6d-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="41d6d-128">Authorization</span></span>  | <span data-ttu-id="41d6d-129">string</span><span class="sxs-lookup"><span data-stu-id="41d6d-129">string</span></span>  | <span data-ttu-id="41d6d-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="41d6d-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="41d6d-132">请求正文</span><span class="sxs-lookup"><span data-stu-id="41d6d-132">Request body</span></span>
<span data-ttu-id="41d6d-133">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="41d6d-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="41d6d-134">响应</span><span class="sxs-lookup"><span data-stu-id="41d6d-134">Response</span></span>

<span data-ttu-id="41d6d-p105">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="41d6d-p105">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="41d6d-137">示例</span><span class="sxs-lookup"><span data-stu-id="41d6d-137">Example</span></span>
##### <a name="request-1"></a><span data-ttu-id="41d6d-138">请求 1</span><span class="sxs-lookup"><span data-stu-id="41d6d-138">Request 1</span></span>
<span data-ttu-id="41d6d-139">第一个示例删除指定的消息。</span><span class="sxs-lookup"><span data-stu-id="41d6d-139">The first example deletes the specified message.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_message"
}-->
```http
DELETE https://graph.microsoft.com/beta/me/messages/{id}
```
##### <a name="response-1"></a><span data-ttu-id="41d6d-140">响应 1</span><span class="sxs-lookup"><span data-stu-id="41d6d-140">Response 1</span></span>
<span data-ttu-id="41d6d-141">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="41d6d-141">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

##### <a name="request-2"></a><span data-ttu-id="41d6d-142">请求 2</span><span class="sxs-lookup"><span data-stu-id="41d6d-142">Request 2</span></span>
<span data-ttu-id="41d6d-143">下一个示例删除某些**提及**中指定的消息。</span><span class="sxs-lookup"><span data-stu-id="41d6d-143">The next example deletes a certain **mention** in the specified message.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_mention_in_message"
}-->
```http
DELETE https://graph.microsoft.com/beta/me/messages/{id}/mentions/{id}
```
##### <a name="response-2"></a><span data-ttu-id="41d6d-144">响应 2</span><span class="sxs-lookup"><span data-stu-id="41d6d-144">Response 2</span></span>
<span data-ttu-id="41d6d-145">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="41d6d-145">Here is an example of the response.</span></span> 
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
  "description": "Delete message",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->