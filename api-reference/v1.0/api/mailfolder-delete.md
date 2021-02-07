---
title: 删除 mailFolder
description: 删除指定的 mailFolder。
author: abheek-das
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 50a33046e9f3e0006a5dbc419f303ecf6aedb185
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50133299"
---
# <a name="delete-mailfolder"></a><span data-ttu-id="8df2d-103">删除 mailFolder</span><span class="sxs-lookup"><span data-stu-id="8df2d-103">Delete mailFolder</span></span>

<span data-ttu-id="8df2d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8df2d-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="8df2d-105">删除指定的 [mailFolder](../resources/mailfolder.md)。</span><span class="sxs-lookup"><span data-stu-id="8df2d-105">Delete the specified [mailFolder](../resources/mailfolder.md).</span></span> <span data-ttu-id="8df2d-106">该文件夹可以是 [mailSearchFolder](../resources/mailsearchfolder.md)。</span><span class="sxs-lookup"><span data-stu-id="8df2d-106">The folder can be a [mailSearchFolder](../resources/mailsearchfolder.md).</span></span>

<span data-ttu-id="8df2d-107">您可以按文件夹 ID 或已知文件夹名称（如果存在）指定[](../resources/mailfolder.md)邮件文件夹。</span><span class="sxs-lookup"><span data-stu-id="8df2d-107">You can specify a mail folder by its folder ID, or by its [well-known folder name](../resources/mailfolder.md), if one exists.</span></span>

><span data-ttu-id="8df2d-108">**注意** 你可能无法删除"可恢复的项目删除"文件夹中 (由已知文件夹名称表示 `recoverableitemsdeletions`) 。</span><span class="sxs-lookup"><span data-stu-id="8df2d-108">**Note** You may not be able to delete items in the recoverable items deletions folder (represented by the well-known folder name `recoverableitemsdeletions`).</span></span> <span data-ttu-id="8df2d-109">有关详细信息[，请参阅"已删除](/exchange/policy-and-compliance/recoverable-items-folder/recoverable-items-folder#deleted-item-retention)邮件[](/exchange/policy-and-compliance/recoverable-items-folder/clean-up-deleted-items)保留和清理已删除项目"。</span><span class="sxs-lookup"><span data-stu-id="8df2d-109">See [Deleted item retention](/exchange/policy-and-compliance/recoverable-items-folder/recoverable-items-folder#deleted-item-retention) and [Clean up deleted items](/exchange/policy-and-compliance/recoverable-items-folder/clean-up-deleted-items) for more information.</span></span>

## <a name="permissions"></a><span data-ttu-id="8df2d-110">Permissions</span><span class="sxs-lookup"><span data-stu-id="8df2d-110">Permissions</span></span>
<span data-ttu-id="8df2d-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8df2d-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8df2d-113">权限类型</span><span class="sxs-lookup"><span data-stu-id="8df2d-113">Permission type</span></span>      | <span data-ttu-id="8df2d-114">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="8df2d-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8df2d-115">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8df2d-115">Delegated (work or school account)</span></span> | <span data-ttu-id="8df2d-116">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8df2d-116">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="8df2d-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8df2d-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8df2d-118">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8df2d-118">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="8df2d-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="8df2d-119">Application</span></span> | <span data-ttu-id="8df2d-120">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8df2d-120">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="8df2d-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8df2d-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/mailFolders/{id}
DELETE /users/{id | userPrincipalName}/mailFolders/{id}
```
## <a name="request-headers"></a><span data-ttu-id="8df2d-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="8df2d-122">Request headers</span></span>
| <span data-ttu-id="8df2d-123">名称</span><span class="sxs-lookup"><span data-stu-id="8df2d-123">Name</span></span>       | <span data-ttu-id="8df2d-124">类型</span><span class="sxs-lookup"><span data-stu-id="8df2d-124">Type</span></span> | <span data-ttu-id="8df2d-125">说明</span><span class="sxs-lookup"><span data-stu-id="8df2d-125">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="8df2d-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="8df2d-126">Authorization</span></span>  | <span data-ttu-id="8df2d-127">string</span><span class="sxs-lookup"><span data-stu-id="8df2d-127">string</span></span>  | <span data-ttu-id="8df2d-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="8df2d-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8df2d-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="8df2d-130">Request body</span></span>
<span data-ttu-id="8df2d-131">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="8df2d-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8df2d-132">响应</span><span class="sxs-lookup"><span data-stu-id="8df2d-132">Response</span></span>

<span data-ttu-id="8df2d-p105">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="8df2d-p105">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8df2d-135">示例</span><span class="sxs-lookup"><span data-stu-id="8df2d-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8df2d-136">请求</span><span class="sxs-lookup"><span data-stu-id="8df2d-136">Request</span></span>
<span data-ttu-id="8df2d-137">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="8df2d-137">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="8df2d-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="8df2d-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_mailfolder"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/me/mailFolders/{id}
```
# <a name="c"></a>[<span data-ttu-id="8df2d-139">C#</span><span class="sxs-lookup"><span data-stu-id="8df2d-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-mailfolder-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8df2d-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8df2d-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-mailfolder-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8df2d-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8df2d-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-mailfolder-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8df2d-142">Java</span><span class="sxs-lookup"><span data-stu-id="8df2d-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-mailfolder-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="8df2d-143">响应</span><span class="sxs-lookup"><span data-stu-id="8df2d-143">Response</span></span>
<span data-ttu-id="8df2d-144">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="8df2d-144">Here is an example of the response.</span></span>
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
  "description": "Delete mailFolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

