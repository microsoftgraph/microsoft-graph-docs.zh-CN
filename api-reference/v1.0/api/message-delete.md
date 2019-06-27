---
title: 删除邮件
description: 删除指定用户的邮箱中的邮件, 或删除邮件的关系。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: b944cb586b7da4580cf8242b25275e7e70e518e7
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35275668"
---
# <a name="delete-message"></a><span data-ttu-id="ef2c6-103">删除邮件</span><span class="sxs-lookup"><span data-stu-id="ef2c6-103">Delete message</span></span>

<span data-ttu-id="ef2c6-104">删除指定用户的邮箱中的邮件, 或删除邮件的关系。</span><span class="sxs-lookup"><span data-stu-id="ef2c6-104">Delete a message in the specified user's mailbox, or delete a relationship of the message.</span></span>

><span data-ttu-id="ef2c6-105">**注释**您可能无法删除 "可恢复的项目删除" 文件夹中的项目 (由[已知文件夹名称](../resources/mailfolder.md) `recoverableitemsdeletions`表示)。</span><span class="sxs-lookup"><span data-stu-id="ef2c6-105">**Note** You may not be able to delete items in the recoverable items deletions folder (represented by the [well-known folder name](../resources/mailfolder.md) `recoverableitemsdeletions`).</span></span> <span data-ttu-id="ef2c6-106">有关详细信息, 请参阅[已删除邮件保留](https://docs.microsoft.com/en-us/exchange/policy-and-compliance/recoverable-items-folder/recoverable-items-folder#deleted-item-retention)和[清除已删除项目](https://docs.microsoft.com/en-us/exchange/policy-and-compliance/recoverable-items-folder/clean-up-deleted-items)。</span><span class="sxs-lookup"><span data-stu-id="ef2c6-106">See [Deleted item retention](https://docs.microsoft.com/en-us/exchange/policy-and-compliance/recoverable-items-folder/recoverable-items-folder#deleted-item-retention) and [Clean up deleted items](https://docs.microsoft.com/en-us/exchange/policy-and-compliance/recoverable-items-folder/clean-up-deleted-items) for more information.</span></span>

## <a name="permissions"></a><span data-ttu-id="ef2c6-107">权限</span><span class="sxs-lookup"><span data-stu-id="ef2c6-107">Permissions</span></span>
<span data-ttu-id="ef2c6-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ef2c6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ef2c6-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="ef2c6-110">Permission type</span></span>      | <span data-ttu-id="ef2c6-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ef2c6-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ef2c6-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ef2c6-112">Delegated (work or school account)</span></span> | <span data-ttu-id="ef2c6-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ef2c6-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="ef2c6-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ef2c6-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ef2c6-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ef2c6-115">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="ef2c6-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="ef2c6-116">Application</span></span> | <span data-ttu-id="ef2c6-117">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ef2c6-117">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="ef2c6-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ef2c6-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/messages/{id}
DELETE /users/{id | userPrincipalName}/messages/{id}
DELETE /me/mailFolders/{id}/messages/{id}
DELETE /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}
```
## <a name="request-headers"></a><span data-ttu-id="ef2c6-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="ef2c6-119">Request headers</span></span>
| <span data-ttu-id="ef2c6-120">名称</span><span class="sxs-lookup"><span data-stu-id="ef2c6-120">Name</span></span>       | <span data-ttu-id="ef2c6-121">类型</span><span class="sxs-lookup"><span data-stu-id="ef2c6-121">Type</span></span> | <span data-ttu-id="ef2c6-122">说明</span><span class="sxs-lookup"><span data-stu-id="ef2c6-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="ef2c6-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="ef2c6-123">Authorization</span></span>  | <span data-ttu-id="ef2c6-124">string</span><span class="sxs-lookup"><span data-stu-id="ef2c6-124">string</span></span>  | <span data-ttu-id="ef2c6-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="ef2c6-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ef2c6-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="ef2c6-127">Request body</span></span>
<span data-ttu-id="ef2c6-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="ef2c6-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ef2c6-129">响应</span><span class="sxs-lookup"><span data-stu-id="ef2c6-129">Response</span></span>

<span data-ttu-id="ef2c6-p104">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="ef2c6-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ef2c6-132">示例</span><span class="sxs-lookup"><span data-stu-id="ef2c6-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ef2c6-133">请求</span><span class="sxs-lookup"><span data-stu-id="ef2c6-133">Request</span></span>
<span data-ttu-id="ef2c6-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="ef2c6-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_message"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/me/messages/{id}
```
##### <a name="response"></a><span data-ttu-id="ef2c6-135">响应</span><span class="sxs-lookup"><span data-stu-id="ef2c6-135">Response</span></span>
<span data-ttu-id="ef2c6-136">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="ef2c6-136">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="ef2c6-137">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="ef2c6-137">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="ef2c6-138">C#</span><span class="sxs-lookup"><span data-stu-id="ef2c6-138">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/delete_message-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="ef2c6-139">Javascript</span><span class="sxs-lookup"><span data-stu-id="ef2c6-139">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/delete_message-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="ef2c6-140">目标-C</span><span class="sxs-lookup"><span data-stu-id="ef2c6-140">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/delete_message-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete message",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/message-delete.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/message-delete.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/message-delete.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
