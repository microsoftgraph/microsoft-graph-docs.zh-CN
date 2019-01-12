---
title: 删除 mailFolder
description: 删除指定的 mailFolder 或 mailSearchFolder。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 6753eaac9e02e5b6c5ff92402f13484dc458b558
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27923864"
---
# <a name="delete-mailfolder"></a><span data-ttu-id="2715b-103">删除 mailFolder</span><span class="sxs-lookup"><span data-stu-id="2715b-103">Delete mailFolder</span></span>

> <span data-ttu-id="2715b-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="2715b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2715b-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="2715b-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="2715b-106">删除指定的[mailFolder](../resources/mailfolder.md)或[mailSearchFolder](../resources/mailsearchfolder.md)。</span><span class="sxs-lookup"><span data-stu-id="2715b-106">Delete the specified [mailFolder](../resources/mailfolder.md) or [mailSearchFolder](../resources/mailsearchfolder.md).</span></span>

<span data-ttu-id="2715b-107">如果存在，您可以指定由其文件夹 ID，或按[已知文件夹名称](../resources/mailfolder.md)的邮件文件夹。</span><span class="sxs-lookup"><span data-stu-id="2715b-107">You can specify a mail folder by its folder ID, or by its [well-known folder name](../resources/mailfolder.md), if one exists.</span></span> 

><span data-ttu-id="2715b-108">**注释**您可能不能删除可恢复邮件删除文件夹中的项目 (由已知文件夹名称`recoverableitemsdeletions`)。</span><span class="sxs-lookup"><span data-stu-id="2715b-108">**Note** You may not be able to delete items in the recoverable items deletions folder (represented by the well-known folder name `recoverableitemsdeletions`).</span></span> <span data-ttu-id="2715b-109">有关详细信息，请参阅[已删除邮件的保留期](https://docs.microsoft.com/en-us/exchange/policy-and-compliance/recoverable-items-folder/recoverable-items-folder#deleted-item-retention)和[清理已删除项目](https://docs.microsoft.com/en-us/exchange/policy-and-compliance/recoverable-items-folder/clean-up-deleted-items)。</span><span class="sxs-lookup"><span data-stu-id="2715b-109">See [Deleted item retention](https://docs.microsoft.com/en-us/exchange/policy-and-compliance/recoverable-items-folder/recoverable-items-folder#deleted-item-retention) and [Clean up deleted items](https://docs.microsoft.com/en-us/exchange/policy-and-compliance/recoverable-items-folder/clean-up-deleted-items) for more information.</span></span>

## <a name="permissions"></a><span data-ttu-id="2715b-110">权限</span><span class="sxs-lookup"><span data-stu-id="2715b-110">Permissions</span></span>
<span data-ttu-id="2715b-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2715b-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2715b-113">权限类型</span><span class="sxs-lookup"><span data-stu-id="2715b-113">Permission type</span></span>      | <span data-ttu-id="2715b-114">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="2715b-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2715b-115">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2715b-115">Delegated (work or school account)</span></span> | <span data-ttu-id="2715b-116">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2715b-116">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="2715b-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2715b-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2715b-118">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2715b-118">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="2715b-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="2715b-119">Application</span></span> | <span data-ttu-id="2715b-120">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2715b-120">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="2715b-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2715b-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/mailFolders/{id}
DELETE /users/{id | userPrincipalName}/mailFolders/{id}
```
## <a name="request-headers"></a><span data-ttu-id="2715b-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="2715b-122">Request headers</span></span>
| <span data-ttu-id="2715b-123">名称</span><span class="sxs-lookup"><span data-stu-id="2715b-123">Name</span></span>       | <span data-ttu-id="2715b-124">类型</span><span class="sxs-lookup"><span data-stu-id="2715b-124">Type</span></span> | <span data-ttu-id="2715b-125">说明</span><span class="sxs-lookup"><span data-stu-id="2715b-125">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="2715b-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="2715b-126">Authorization</span></span>  | <span data-ttu-id="2715b-127">string</span><span class="sxs-lookup"><span data-stu-id="2715b-127">string</span></span>  | <span data-ttu-id="2715b-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="2715b-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2715b-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="2715b-130">Request body</span></span>
<span data-ttu-id="2715b-131">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="2715b-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2715b-132">响应</span><span class="sxs-lookup"><span data-stu-id="2715b-132">Response</span></span>
<span data-ttu-id="2715b-p105">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="2715b-p105">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2715b-135">示例</span><span class="sxs-lookup"><span data-stu-id="2715b-135">Example</span></span>
#### <a name="request"></a><span data-ttu-id="2715b-136">请求</span><span class="sxs-lookup"><span data-stu-id="2715b-136">Request</span></span>
<span data-ttu-id="2715b-137">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="2715b-137">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_mailfolder"
}-->
```http
DELETE https://graph.microsoft.com/beta/me/mailFolders/AAMkAGVmMDEzM/
```

#### <a name="response"></a><span data-ttu-id="2715b-138">响应</span><span class="sxs-lookup"><span data-stu-id="2715b-138">Response</span></span>
<span data-ttu-id="2715b-139">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="2715b-139">The following is an example of the response.</span></span> 
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
  "tocPath": ""
}-->
