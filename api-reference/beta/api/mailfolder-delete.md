---
title: 删除 mailFolder
description: 删除指定的 mailFolder 或 mailSearchFolder。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 023bce8ac1d03ffd557eb3a0fe15c67e5a784146
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35448802"
---
# <a name="delete-mailfolder"></a><span data-ttu-id="020a5-103">删除 mailFolder</span><span class="sxs-lookup"><span data-stu-id="020a5-103">Delete mailFolder</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="020a5-104">删除指定的[mailFolder](../resources/mailfolder.md)。</span><span class="sxs-lookup"><span data-stu-id="020a5-104">Delete the specified [mailFolder](../resources/mailfolder.md).</span></span> <span data-ttu-id="020a5-105">文件夹可以是[mailSearchFolder](../resources/mailsearchfolder.md)。</span><span class="sxs-lookup"><span data-stu-id="020a5-105">The folder can be a [mailSearchFolder](../resources/mailsearchfolder.md).</span></span>

<span data-ttu-id="020a5-106">可以按文件夹 ID 或[已知文件夹名称](../resources/mailfolder.md)指定邮件文件夹 (如果存在)。</span><span class="sxs-lookup"><span data-stu-id="020a5-106">You can specify a mail folder by its folder ID, or by its [well-known folder name](../resources/mailfolder.md), if one exists.</span></span> 

><span data-ttu-id="020a5-107">**注释**您可能无法删除 "可恢复的项目删除" 文件夹中的项目 (由已知文件夹名称`recoverableitemsdeletions`表示)。</span><span class="sxs-lookup"><span data-stu-id="020a5-107">**Note** You may not be able to delete items in the recoverable items deletions folder (represented by the well-known folder name `recoverableitemsdeletions`).</span></span> <span data-ttu-id="020a5-108">有关详细信息, 请参阅[已删除邮件保留](https://docs.microsoft.com/en-us/exchange/policy-and-compliance/recoverable-items-folder/recoverable-items-folder#deleted-item-retention)和[清除已删除项目](https://docs.microsoft.com/en-us/exchange/policy-and-compliance/recoverable-items-folder/clean-up-deleted-items)。</span><span class="sxs-lookup"><span data-stu-id="020a5-108">See [Deleted item retention](https://docs.microsoft.com/en-us/exchange/policy-and-compliance/recoverable-items-folder/recoverable-items-folder#deleted-item-retention) and [Clean up deleted items](https://docs.microsoft.com/en-us/exchange/policy-and-compliance/recoverable-items-folder/clean-up-deleted-items) for more information.</span></span>

## <a name="permissions"></a><span data-ttu-id="020a5-109">权限</span><span class="sxs-lookup"><span data-stu-id="020a5-109">Permissions</span></span>
<span data-ttu-id="020a5-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="020a5-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="020a5-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="020a5-112">Permission type</span></span>      | <span data-ttu-id="020a5-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="020a5-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="020a5-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="020a5-114">Delegated (work or school account)</span></span> | <span data-ttu-id="020a5-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="020a5-115">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="020a5-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="020a5-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="020a5-117">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="020a5-117">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="020a5-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="020a5-118">Application</span></span> | <span data-ttu-id="020a5-119">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="020a5-119">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="020a5-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="020a5-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/mailFolders/{id}
DELETE /users/{id | userPrincipalName}/mailFolders/{id}
```
## <a name="request-headers"></a><span data-ttu-id="020a5-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="020a5-121">Request headers</span></span>
| <span data-ttu-id="020a5-122">名称</span><span class="sxs-lookup"><span data-stu-id="020a5-122">Name</span></span>       | <span data-ttu-id="020a5-123">类型</span><span class="sxs-lookup"><span data-stu-id="020a5-123">Type</span></span> | <span data-ttu-id="020a5-124">说明</span><span class="sxs-lookup"><span data-stu-id="020a5-124">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="020a5-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="020a5-125">Authorization</span></span>  | <span data-ttu-id="020a5-126">string</span><span class="sxs-lookup"><span data-stu-id="020a5-126">string</span></span>  | <span data-ttu-id="020a5-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="020a5-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="020a5-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="020a5-129">Request body</span></span>
<span data-ttu-id="020a5-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="020a5-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="020a5-131">响应</span><span class="sxs-lookup"><span data-stu-id="020a5-131">Response</span></span>
<span data-ttu-id="020a5-p105">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="020a5-p105">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="020a5-134">示例</span><span class="sxs-lookup"><span data-stu-id="020a5-134">Example</span></span>
#### <a name="request"></a><span data-ttu-id="020a5-135">请求</span><span class="sxs-lookup"><span data-stu-id="020a5-135">Request</span></span>
<span data-ttu-id="020a5-136">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="020a5-136">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="020a5-137">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="020a5-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_mailfolder"
}-->
```http
DELETE https://graph.microsoft.com/beta/me/mailFolders/AAMkAGVmMDEzM/
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="020a5-138">C#</span><span class="sxs-lookup"><span data-stu-id="020a5-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-mailfolder-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="020a5-139">Javascript</span><span class="sxs-lookup"><span data-stu-id="020a5-139">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-mailfolder-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="020a5-140">目标-C</span><span class="sxs-lookup"><span data-stu-id="020a5-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-mailfolder-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="020a5-141">响应</span><span class="sxs-lookup"><span data-stu-id="020a5-141">Response</span></span>
<span data-ttu-id="020a5-142">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="020a5-142">The following is an example of the response.</span></span> 
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
  "description": "Delete mailFolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
