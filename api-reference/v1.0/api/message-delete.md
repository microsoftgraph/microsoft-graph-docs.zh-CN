---
title: 删除邮件
description: 删除指定的用户邮箱中的邮件或删除邮件的关系。
ms.openlocfilehash: 5bfcb57f3f9c82f79147c30c982f59172e48b51f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27010719"
---
# <a name="delete-message"></a><span data-ttu-id="9660f-103">删除邮件</span><span class="sxs-lookup"><span data-stu-id="9660f-103">Delete message</span></span>

<span data-ttu-id="9660f-104">删除指定的用户邮箱中的邮件或删除邮件的关系。</span><span class="sxs-lookup"><span data-stu-id="9660f-104">Delete a message in the specified user's mailbox, or delete a relationship of the message.</span></span>

><span data-ttu-id="9660f-105">**注释**您可能不能删除可恢复邮件删除文件夹中的项目 (由[已知文件夹名称](../resources/mailfolder.md) `recoverableitemsdeletions`)。</span><span class="sxs-lookup"><span data-stu-id="9660f-105">**Note** You may not be able to delete items in the recoverable items deletions folder (represented by the [well-known folder name](../resources/mailfolder.md) `recoverableitemsdeletions`).</span></span> <span data-ttu-id="9660f-106">有关详细信息，请参阅[已删除邮件的保留期](https://docs.microsoft.com/en-us/exchange/policy-and-compliance/recoverable-items-folder/recoverable-items-folder#deleted-item-retention)和[清理已删除项目](https://docs.microsoft.com/en-us/exchange/policy-and-compliance/recoverable-items-folder/clean-up-deleted-items)。</span><span class="sxs-lookup"><span data-stu-id="9660f-106">See [Deleted item retention](https://docs.microsoft.com/en-us/exchange/policy-and-compliance/recoverable-items-folder/recoverable-items-folder#deleted-item-retention) and [Clean up deleted items](https://docs.microsoft.com/en-us/exchange/policy-and-compliance/recoverable-items-folder/clean-up-deleted-items) for more information.</span></span>

## <a name="permissions"></a><span data-ttu-id="9660f-107">权限</span><span class="sxs-lookup"><span data-stu-id="9660f-107">Permissions</span></span>
<span data-ttu-id="9660f-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9660f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9660f-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="9660f-110">Permission type</span></span>      | <span data-ttu-id="9660f-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="9660f-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9660f-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9660f-112">Delegated (work or school account)</span></span> | <span data-ttu-id="9660f-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9660f-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="9660f-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9660f-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9660f-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9660f-115">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="9660f-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="9660f-116">Application</span></span> | <span data-ttu-id="9660f-117">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9660f-117">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="9660f-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9660f-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/messages/{id}
DELETE /users/{id | userPrincipalName}/messages/{id}
DELETE /me/mailFolders/{id}/messages/{id}
DELETE /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}
```
## <a name="request-headers"></a><span data-ttu-id="9660f-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="9660f-119">Request headers</span></span>
| <span data-ttu-id="9660f-120">名称</span><span class="sxs-lookup"><span data-stu-id="9660f-120">Name</span></span>       | <span data-ttu-id="9660f-121">类型</span><span class="sxs-lookup"><span data-stu-id="9660f-121">Type</span></span> | <span data-ttu-id="9660f-122">说明</span><span class="sxs-lookup"><span data-stu-id="9660f-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="9660f-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="9660f-123">Authorization</span></span>  | <span data-ttu-id="9660f-124">string</span><span class="sxs-lookup"><span data-stu-id="9660f-124">string</span></span>  | <span data-ttu-id="9660f-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="9660f-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9660f-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="9660f-127">Request body</span></span>
<span data-ttu-id="9660f-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="9660f-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9660f-129">响应</span><span class="sxs-lookup"><span data-stu-id="9660f-129">Response</span></span>

<span data-ttu-id="9660f-p104">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="9660f-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9660f-132">示例</span><span class="sxs-lookup"><span data-stu-id="9660f-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9660f-133">请求</span><span class="sxs-lookup"><span data-stu-id="9660f-133">Request</span></span>
<span data-ttu-id="9660f-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="9660f-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_message"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/me/messages/{id}
```
##### <a name="response"></a><span data-ttu-id="9660f-135">响应</span><span class="sxs-lookup"><span data-stu-id="9660f-135">Response</span></span>
<span data-ttu-id="9660f-136">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="9660f-136">Here is an example of the response.</span></span> 
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