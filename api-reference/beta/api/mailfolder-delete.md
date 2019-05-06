---
title: 删除 mailFolder
description: 删除指定的 mailFolder 或 mailSearchFolder。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 4e8363198b3856e87ad9279d36effbc5d522bf93
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2019
ms.locfileid: "33598365"
---
# <a name="delete-mailfolder"></a><span data-ttu-id="71c53-103">删除 mailFolder</span><span class="sxs-lookup"><span data-stu-id="71c53-103">Delete mailFolder</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="71c53-104">删除指定的[mailFolder](../resources/mailfolder.md)或[mailSearchFolder](../resources/mailsearchfolder.md)。</span><span class="sxs-lookup"><span data-stu-id="71c53-104">Delete the specified [mailFolder](../resources/mailfolder.md) or [mailSearchFolder](../resources/mailsearchfolder.md).</span></span>

<span data-ttu-id="71c53-105">可以按文件夹 ID 或[已知文件夹名称](../resources/mailfolder.md)指定邮件文件夹 (如果存在)。</span><span class="sxs-lookup"><span data-stu-id="71c53-105">You can specify a mail folder by its folder ID, or by its [well-known folder name](../resources/mailfolder.md), if one exists.</span></span> 

><span data-ttu-id="71c53-106">**注释**您可能无法删除 "可恢复的项目删除" 文件夹中的项目 (由已知文件夹名称`recoverableitemsdeletions`表示)。</span><span class="sxs-lookup"><span data-stu-id="71c53-106">**Note** You may not be able to delete items in the recoverable items deletions folder (represented by the well-known folder name `recoverableitemsdeletions`).</span></span> <span data-ttu-id="71c53-107">有关详细信息, 请参阅[已删除邮件保留](https://docs.microsoft.com/en-us/exchange/policy-and-compliance/recoverable-items-folder/recoverable-items-folder#deleted-item-retention)和[清除已删除项目](https://docs.microsoft.com/en-us/exchange/policy-and-compliance/recoverable-items-folder/clean-up-deleted-items)。</span><span class="sxs-lookup"><span data-stu-id="71c53-107">See [Deleted item retention](https://docs.microsoft.com/en-us/exchange/policy-and-compliance/recoverable-items-folder/recoverable-items-folder#deleted-item-retention) and [Clean up deleted items](https://docs.microsoft.com/en-us/exchange/policy-and-compliance/recoverable-items-folder/clean-up-deleted-items) for more information.</span></span>

## <a name="permissions"></a><span data-ttu-id="71c53-108">权限</span><span class="sxs-lookup"><span data-stu-id="71c53-108">Permissions</span></span>
<span data-ttu-id="71c53-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="71c53-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="71c53-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="71c53-111">Permission type</span></span>      | <span data-ttu-id="71c53-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="71c53-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="71c53-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="71c53-113">Delegated (work or school account)</span></span> | <span data-ttu-id="71c53-114">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="71c53-114">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="71c53-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="71c53-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="71c53-116">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="71c53-116">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="71c53-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="71c53-117">Application</span></span> | <span data-ttu-id="71c53-118">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="71c53-118">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="71c53-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="71c53-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/mailFolders/{id}
DELETE /users/{id | userPrincipalName}/mailFolders/{id}
```
## <a name="request-headers"></a><span data-ttu-id="71c53-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="71c53-120">Request headers</span></span>
| <span data-ttu-id="71c53-121">名称</span><span class="sxs-lookup"><span data-stu-id="71c53-121">Name</span></span>       | <span data-ttu-id="71c53-122">类型</span><span class="sxs-lookup"><span data-stu-id="71c53-122">Type</span></span> | <span data-ttu-id="71c53-123">说明</span><span class="sxs-lookup"><span data-stu-id="71c53-123">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="71c53-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="71c53-124">Authorization</span></span>  | <span data-ttu-id="71c53-125">string</span><span class="sxs-lookup"><span data-stu-id="71c53-125">string</span></span>  | <span data-ttu-id="71c53-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="71c53-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="71c53-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="71c53-128">Request body</span></span>
<span data-ttu-id="71c53-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="71c53-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="71c53-130">响应</span><span class="sxs-lookup"><span data-stu-id="71c53-130">Response</span></span>
<span data-ttu-id="71c53-p104">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="71c53-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="71c53-133">示例</span><span class="sxs-lookup"><span data-stu-id="71c53-133">Example</span></span>
#### <a name="request"></a><span data-ttu-id="71c53-134">请求</span><span class="sxs-lookup"><span data-stu-id="71c53-134">Request</span></span>
<span data-ttu-id="71c53-135">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="71c53-135">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_mailfolder"
}-->
```http
DELETE https://graph.microsoft.com/beta/me/mailFolders/AAMkAGVmMDEzM/
```

#### <a name="response"></a><span data-ttu-id="71c53-136">响应</span><span class="sxs-lookup"><span data-stu-id="71c53-136">Response</span></span>
<span data-ttu-id="71c53-137">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="71c53-137">The following is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="71c53-138">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="71c53-138">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="71c53-139">语言</span><span class="sxs-lookup"><span data-stu-id="71c53-139">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/delete_mailfolder-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="71c53-140">Javascript</span><span class="sxs-lookup"><span data-stu-id="71c53-140">Javascript</span></span>](#tab/javascript)
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
