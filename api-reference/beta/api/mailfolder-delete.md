---
title: 删除 mailFolder
description: 删除指定的 mailFolder 或 mailSearchFolder。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 9064febf261c240ef51dd704f98fc2e502acdd24
ms.sourcegitcommit: b742da101a3a232356bf748c42da3ba08a7539d3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/10/2019
ms.locfileid: "34812591"
---
# <a name="delete-mailfolder"></a><span data-ttu-id="5f005-103">删除 mailFolder</span><span class="sxs-lookup"><span data-stu-id="5f005-103">Delete mailFolder</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5f005-104">删除指定的[mailFolder](../resources/mailfolder.md)。</span><span class="sxs-lookup"><span data-stu-id="5f005-104">Delete the specified [mailFolder](../resources/mailfolder.md).</span></span> <span data-ttu-id="5f005-105">文件夹可以是[mailSearchFolder](../resources/mailsearchfolder.md)。</span><span class="sxs-lookup"><span data-stu-id="5f005-105">The folder can be a [mailSearchFolder](../resources/mailsearchfolder.md).</span></span>

<span data-ttu-id="5f005-106">可以按文件夹 ID 或[已知文件夹名称](../resources/mailfolder.md)指定邮件文件夹 (如果存在)。</span><span class="sxs-lookup"><span data-stu-id="5f005-106">You can specify a mail folder by its folder ID, or by its [well-known folder name](../resources/mailfolder.md), if one exists.</span></span> 

><span data-ttu-id="5f005-107">**注释**您可能无法删除 "可恢复的项目删除" 文件夹中的项目 (由已知文件夹名称`recoverableitemsdeletions`表示)。</span><span class="sxs-lookup"><span data-stu-id="5f005-107">**Note** You may not be able to delete items in the recoverable items deletions folder (represented by the well-known folder name `recoverableitemsdeletions`).</span></span> <span data-ttu-id="5f005-108">有关详细信息, 请参阅[已删除邮件保留](https://docs.microsoft.com/en-us/exchange/policy-and-compliance/recoverable-items-folder/recoverable-items-folder#deleted-item-retention)和[清除已删除项目](https://docs.microsoft.com/en-us/exchange/policy-and-compliance/recoverable-items-folder/clean-up-deleted-items)。</span><span class="sxs-lookup"><span data-stu-id="5f005-108">See [Deleted item retention](https://docs.microsoft.com/en-us/exchange/policy-and-compliance/recoverable-items-folder/recoverable-items-folder#deleted-item-retention) and [Clean up deleted items](https://docs.microsoft.com/en-us/exchange/policy-and-compliance/recoverable-items-folder/clean-up-deleted-items) for more information.</span></span>

## <a name="permissions"></a><span data-ttu-id="5f005-109">权限</span><span class="sxs-lookup"><span data-stu-id="5f005-109">Permissions</span></span>
<span data-ttu-id="5f005-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="5f005-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5f005-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="5f005-112">Permission type</span></span>      | <span data-ttu-id="5f005-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="5f005-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5f005-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5f005-114">Delegated (work or school account)</span></span> | <span data-ttu-id="5f005-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5f005-115">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="5f005-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5f005-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5f005-117">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5f005-117">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="5f005-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="5f005-118">Application</span></span> | <span data-ttu-id="5f005-119">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5f005-119">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="5f005-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5f005-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/mailFolders/{id}
DELETE /users/{id | userPrincipalName}/mailFolders/{id}
```
## <a name="request-headers"></a><span data-ttu-id="5f005-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="5f005-121">Request headers</span></span>
| <span data-ttu-id="5f005-122">名称</span><span class="sxs-lookup"><span data-stu-id="5f005-122">Name</span></span>       | <span data-ttu-id="5f005-123">类型</span><span class="sxs-lookup"><span data-stu-id="5f005-123">Type</span></span> | <span data-ttu-id="5f005-124">说明</span><span class="sxs-lookup"><span data-stu-id="5f005-124">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="5f005-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="5f005-125">Authorization</span></span>  | <span data-ttu-id="5f005-126">string</span><span class="sxs-lookup"><span data-stu-id="5f005-126">string</span></span>  | <span data-ttu-id="5f005-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="5f005-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5f005-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="5f005-129">Request body</span></span>
<span data-ttu-id="5f005-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="5f005-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5f005-131">响应</span><span class="sxs-lookup"><span data-stu-id="5f005-131">Response</span></span>
<span data-ttu-id="5f005-p105">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="5f005-p105">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5f005-134">示例</span><span class="sxs-lookup"><span data-stu-id="5f005-134">Example</span></span>
#### <a name="request"></a><span data-ttu-id="5f005-135">请求</span><span class="sxs-lookup"><span data-stu-id="5f005-135">Request</span></span>
<span data-ttu-id="5f005-136">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="5f005-136">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_mailfolder"
}-->
```http
DELETE https://graph.microsoft.com/beta/me/mailFolders/AAMkAGVmMDEzM/
```

#### <a name="response"></a><span data-ttu-id="5f005-137">响应</span><span class="sxs-lookup"><span data-stu-id="5f005-137">Response</span></span>
<span data-ttu-id="5f005-138">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="5f005-138">The following is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="5f005-139">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="5f005-139">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="5f005-140">C#</span><span class="sxs-lookup"><span data-stu-id="5f005-140">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/delete_mailfolder-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="5f005-141">Javascript</span><span class="sxs-lookup"><span data-stu-id="5f005-141">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/delete_mailfolder-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete mailFolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/mailfolder-delete.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/mailfolder-delete.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
