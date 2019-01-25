---
title: 删除邮件
description: 删除指定的用户邮箱中的邮件或删除邮件的关系。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 1237ba7e4aa5ab0439af9f07902705e7b4061374
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29513541"
---
# <a name="delete-message"></a><span data-ttu-id="6dadc-103">删除邮件</span><span class="sxs-lookup"><span data-stu-id="6dadc-103">Delete message</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6dadc-104">删除指定的用户邮箱中的邮件或删除邮件的关系。</span><span class="sxs-lookup"><span data-stu-id="6dadc-104">Delete a message in the specified user's mailbox, or delete a relationship of the message.</span></span>

<span data-ttu-id="6dadc-105">例如，您可以删除某个特定的[@ 提及](../resources/mention.md)的消息中指定的用户。</span><span class="sxs-lookup"><span data-stu-id="6dadc-105">For example, you can delete a specific [@-mention](../resources/mention.md) of the specified user in the message.</span></span>

><span data-ttu-id="6dadc-106">**注释**您可能不能删除可恢复邮件删除文件夹中的项目 (由[已知文件夹名称](../resources/mailfolder.md) `recoverableitemsdeletions`)。</span><span class="sxs-lookup"><span data-stu-id="6dadc-106">**Note** You may not be able to delete items in the recoverable items deletions folder (represented by the [well-known folder name](../resources/mailfolder.md) `recoverableitemsdeletions`).</span></span> <span data-ttu-id="6dadc-107">有关详细信息，请参阅[已删除邮件的保留期](https://docs.microsoft.com/en-us/exchange/policy-and-compliance/recoverable-items-folder/recoverable-items-folder#deleted-item-retention)和[清理已删除项目](https://docs.microsoft.com/en-us/exchange/policy-and-compliance/recoverable-items-folder/clean-up-deleted-items)。</span><span class="sxs-lookup"><span data-stu-id="6dadc-107">See [Deleted item retention](https://docs.microsoft.com/en-us/exchange/policy-and-compliance/recoverable-items-folder/recoverable-items-folder#deleted-item-retention) and [Clean up deleted items](https://docs.microsoft.com/en-us/exchange/policy-and-compliance/recoverable-items-folder/clean-up-deleted-items) for more information.</span></span>

## <a name="permissions"></a><span data-ttu-id="6dadc-108">权限</span><span class="sxs-lookup"><span data-stu-id="6dadc-108">Permissions</span></span>
<span data-ttu-id="6dadc-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6dadc-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6dadc-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="6dadc-111">Permission type</span></span>      | <span data-ttu-id="6dadc-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="6dadc-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6dadc-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6dadc-113">Delegated (work or school account)</span></span> | <span data-ttu-id="6dadc-114">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6dadc-114">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="6dadc-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6dadc-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6dadc-116">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6dadc-116">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="6dadc-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="6dadc-117">Application</span></span> | <span data-ttu-id="6dadc-118">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6dadc-118">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="6dadc-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6dadc-119">HTTP request</span></span>

<span data-ttu-id="6dadc-120">删除指定的消息：<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="6dadc-120">To delete the specified message: <!-- { "blockType": "ignored" } --></span></span>
```http
DELETE /me/messages/{id}
DELETE /users/{id | userPrincipalName}/messages/{id}
DELETE /me/mailFolders/{id}/messages/{id}
DELETE /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}
```

<span data-ttu-id="6dadc-121">删除特定[提及](../resources/mention.md)邮件中：<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="6dadc-121">To delete a specific [mention](../resources/mention.md) in a message: <!-- { "blockType": "ignored" } --></span></span>
```http
DELETE /me/messages/{id}/mentions/{id}
DELETE /users/{id | userPrincipalName}/messages/{id}/mentions/{id}
DELETE /me/mailFolders/{id}/messages/{id}/mentions/{id}
DELETE /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/mentions/{id}
```

## <a name="request-headers"></a><span data-ttu-id="6dadc-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="6dadc-122">Request headers</span></span>
| <span data-ttu-id="6dadc-123">名称</span><span class="sxs-lookup"><span data-stu-id="6dadc-123">Name</span></span>       | <span data-ttu-id="6dadc-124">类型</span><span class="sxs-lookup"><span data-stu-id="6dadc-124">Type</span></span> | <span data-ttu-id="6dadc-125">说明</span><span class="sxs-lookup"><span data-stu-id="6dadc-125">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="6dadc-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="6dadc-126">Authorization</span></span>  | <span data-ttu-id="6dadc-127">string</span><span class="sxs-lookup"><span data-stu-id="6dadc-127">string</span></span>  | <span data-ttu-id="6dadc-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="6dadc-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6dadc-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="6dadc-130">Request body</span></span>
<span data-ttu-id="6dadc-131">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="6dadc-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6dadc-132">响应</span><span class="sxs-lookup"><span data-stu-id="6dadc-132">Response</span></span>

<span data-ttu-id="6dadc-p104">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="6dadc-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6dadc-135">示例</span><span class="sxs-lookup"><span data-stu-id="6dadc-135">Example</span></span>
##### <a name="request-1"></a><span data-ttu-id="6dadc-136">请求 1</span><span class="sxs-lookup"><span data-stu-id="6dadc-136">Request 1</span></span>
<span data-ttu-id="6dadc-137">第一个示例删除指定的消息。</span><span class="sxs-lookup"><span data-stu-id="6dadc-137">The first example deletes the specified message.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_message"
}-->
```http
DELETE https://graph.microsoft.com/beta/me/messages/{id}
```
##### <a name="response-1"></a><span data-ttu-id="6dadc-138">响应 1</span><span class="sxs-lookup"><span data-stu-id="6dadc-138">Response 1</span></span>
<span data-ttu-id="6dadc-139">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="6dadc-139">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

##### <a name="request-2"></a><span data-ttu-id="6dadc-140">请求 2</span><span class="sxs-lookup"><span data-stu-id="6dadc-140">Request 2</span></span>
<span data-ttu-id="6dadc-141">下一个示例删除某些**提及**中指定的消息。</span><span class="sxs-lookup"><span data-stu-id="6dadc-141">The next example deletes a certain **mention** in the specified message.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_mention_in_message"
}-->
```http
DELETE https://graph.microsoft.com/beta/me/messages/{id}/mentions/{id}
```
##### <a name="response-2"></a><span data-ttu-id="6dadc-142">响应 2</span><span class="sxs-lookup"><span data-stu-id="6dadc-142">Response 2</span></span>
<span data-ttu-id="6dadc-143">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="6dadc-143">Here is an example of the response.</span></span> 
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
    "Error: /api-reference/beta/api/message-delete.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
