---
title: 删除邮件
description: 删除指定用户的邮箱中的邮件，或删除邮件的关系。
localization_priority: Normal
author: svpsiva
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 014cbcbeb9d7ac34fa4ab038377363e2c3e6286c
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48019073"
---
# <a name="delete-message"></a><span data-ttu-id="6e9fa-103">删除邮件</span><span class="sxs-lookup"><span data-stu-id="6e9fa-103">Delete message</span></span>

<span data-ttu-id="6e9fa-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6e9fa-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="6e9fa-105">删除指定用户的邮箱中的邮件，或删除邮件的关系。</span><span class="sxs-lookup"><span data-stu-id="6e9fa-105">Delete a message in the specified user's mailbox, or delete a relationship of the message.</span></span>

><span data-ttu-id="6e9fa-106">**注释** 您可能无法删除 "可恢复的项目" 删除文件夹中的项目 (由 [已知文件夹名称](../resources/mailfolder.md) `recoverableitemsdeletions`) 所表示。</span><span class="sxs-lookup"><span data-stu-id="6e9fa-106">**Note** You may not be able to delete items in the recoverable items deletions folder (represented by the [well-known folder name](../resources/mailfolder.md) `recoverableitemsdeletions`).</span></span> <span data-ttu-id="6e9fa-107">有关详细信息，请参阅 [已删除邮件保留](/exchange/policy-and-compliance/recoverable-items-folder/recoverable-items-folder#deleted-item-retention) 和 [清除已删除项目](/exchange/policy-and-compliance/recoverable-items-folder/clean-up-deleted-items) 。</span><span class="sxs-lookup"><span data-stu-id="6e9fa-107">See [Deleted item retention](/exchange/policy-and-compliance/recoverable-items-folder/recoverable-items-folder#deleted-item-retention) and [Clean up deleted items](/exchange/policy-and-compliance/recoverable-items-folder/clean-up-deleted-items) for more information.</span></span>

## <a name="permissions"></a><span data-ttu-id="6e9fa-108">权限</span><span class="sxs-lookup"><span data-stu-id="6e9fa-108">Permissions</span></span>
<span data-ttu-id="6e9fa-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6e9fa-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6e9fa-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="6e9fa-111">Permission type</span></span>      | <span data-ttu-id="6e9fa-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="6e9fa-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6e9fa-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6e9fa-113">Delegated (work or school account)</span></span> | <span data-ttu-id="6e9fa-114">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6e9fa-114">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="6e9fa-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6e9fa-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6e9fa-116">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6e9fa-116">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="6e9fa-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="6e9fa-117">Application</span></span> | <span data-ttu-id="6e9fa-118">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6e9fa-118">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="6e9fa-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6e9fa-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/messages/{id}
DELETE /users/{id | userPrincipalName}/messages/{id}
DELETE /me/mailFolders/{id}/messages/{id}
DELETE /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}
```
## <a name="request-headers"></a><span data-ttu-id="6e9fa-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="6e9fa-120">Request headers</span></span>
| <span data-ttu-id="6e9fa-121">名称</span><span class="sxs-lookup"><span data-stu-id="6e9fa-121">Name</span></span>       | <span data-ttu-id="6e9fa-122">类型</span><span class="sxs-lookup"><span data-stu-id="6e9fa-122">Type</span></span> | <span data-ttu-id="6e9fa-123">说明</span><span class="sxs-lookup"><span data-stu-id="6e9fa-123">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="6e9fa-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="6e9fa-124">Authorization</span></span>  | <span data-ttu-id="6e9fa-125">string</span><span class="sxs-lookup"><span data-stu-id="6e9fa-125">string</span></span>  | <span data-ttu-id="6e9fa-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="6e9fa-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6e9fa-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="6e9fa-128">Request body</span></span>
<span data-ttu-id="6e9fa-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="6e9fa-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6e9fa-130">响应</span><span class="sxs-lookup"><span data-stu-id="6e9fa-130">Response</span></span>

<span data-ttu-id="6e9fa-p104">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="6e9fa-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6e9fa-133">示例</span><span class="sxs-lookup"><span data-stu-id="6e9fa-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6e9fa-134">请求</span><span class="sxs-lookup"><span data-stu-id="6e9fa-134">Request</span></span>
<span data-ttu-id="6e9fa-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="6e9fa-135">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="6e9fa-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="6e9fa-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_message"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/me/messages/{id}
```
# <a name="c"></a>[<span data-ttu-id="6e9fa-137">C#</span><span class="sxs-lookup"><span data-stu-id="6e9fa-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-message-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6e9fa-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6e9fa-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-message-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6e9fa-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6e9fa-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-message-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="6e9fa-140">Java</span><span class="sxs-lookup"><span data-stu-id="6e9fa-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-message-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="6e9fa-141">响应</span><span class="sxs-lookup"><span data-stu-id="6e9fa-141">Response</span></span>
<span data-ttu-id="6e9fa-142">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="6e9fa-142">Here is an example of the response.</span></span>
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
  "tocPath": "",
  "suppressions": [
  ]
}-->

