---
title: 删除 mailFolder
description: 删除指定的 mailFolder。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 56b1fc45b79172f64ceb1bf9b0d6f69da1695bcf
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32565462"
---
# <a name="delete-mailfolder"></a><span data-ttu-id="8e1a8-103">删除 mailFolder</span><span class="sxs-lookup"><span data-stu-id="8e1a8-103">Delete mailFolder</span></span>

<span data-ttu-id="8e1a8-104">删除指定的[mailFolder](../resources/mailfolder.md)。</span><span class="sxs-lookup"><span data-stu-id="8e1a8-104">Delete the specified [mailFolder](../resources/mailfolder.md).</span></span>

<span data-ttu-id="8e1a8-105">可以按文件夹 ID 或[已知文件夹名称](../resources/mailfolder.md)指定邮件文件夹 (如果存在)。</span><span class="sxs-lookup"><span data-stu-id="8e1a8-105">You can specify a mail folder by its folder ID, or by its [well-known folder name](../resources/mailfolder.md), if one exists.</span></span> 

><span data-ttu-id="8e1a8-106">**注释**您可能无法删除 "可恢复的项目删除" 文件夹中的项目 (由已知文件夹名称`recoverableitemsdeletions`表示)。</span><span class="sxs-lookup"><span data-stu-id="8e1a8-106">**Note** You may not be able to delete items in the recoverable items deletions folder (represented by the well-known folder name `recoverableitemsdeletions`).</span></span> <span data-ttu-id="8e1a8-107">有关详细信息, 请参阅[已删除邮件保留](https://docs.microsoft.com/en-us/exchange/policy-and-compliance/recoverable-items-folder/recoverable-items-folder#deleted-item-retention)和[清除已删除项目](https://docs.microsoft.com/en-us/exchange/policy-and-compliance/recoverable-items-folder/clean-up-deleted-items)。</span><span class="sxs-lookup"><span data-stu-id="8e1a8-107">See [Deleted item retention](https://docs.microsoft.com/en-us/exchange/policy-and-compliance/recoverable-items-folder/recoverable-items-folder#deleted-item-retention) and [Clean up deleted items](https://docs.microsoft.com/en-us/exchange/policy-and-compliance/recoverable-items-folder/clean-up-deleted-items) for more information.</span></span>

## <a name="permissions"></a><span data-ttu-id="8e1a8-108">权限</span><span class="sxs-lookup"><span data-stu-id="8e1a8-108">Permissions</span></span>
<span data-ttu-id="8e1a8-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8e1a8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8e1a8-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="8e1a8-111">Permission type</span></span>      | <span data-ttu-id="8e1a8-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="8e1a8-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8e1a8-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8e1a8-113">Delegated (work or school account)</span></span> | <span data-ttu-id="8e1a8-114">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8e1a8-114">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="8e1a8-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8e1a8-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8e1a8-116">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8e1a8-116">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="8e1a8-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="8e1a8-117">Application</span></span> | <span data-ttu-id="8e1a8-118">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8e1a8-118">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="8e1a8-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8e1a8-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/mailFolders/{id}
DELETE /users/{id | userPrincipalName}/mailFolders/{id}
```
## <a name="request-headers"></a><span data-ttu-id="8e1a8-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="8e1a8-120">Request headers</span></span>
| <span data-ttu-id="8e1a8-121">名称</span><span class="sxs-lookup"><span data-stu-id="8e1a8-121">Name</span></span>       | <span data-ttu-id="8e1a8-122">类型</span><span class="sxs-lookup"><span data-stu-id="8e1a8-122">Type</span></span> | <span data-ttu-id="8e1a8-123">说明</span><span class="sxs-lookup"><span data-stu-id="8e1a8-123">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="8e1a8-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="8e1a8-124">Authorization</span></span>  | <span data-ttu-id="8e1a8-125">string</span><span class="sxs-lookup"><span data-stu-id="8e1a8-125">string</span></span>  | <span data-ttu-id="8e1a8-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="8e1a8-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8e1a8-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="8e1a8-128">Request body</span></span>
<span data-ttu-id="8e1a8-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="8e1a8-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8e1a8-130">响应</span><span class="sxs-lookup"><span data-stu-id="8e1a8-130">Response</span></span>

<span data-ttu-id="8e1a8-p104">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="8e1a8-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8e1a8-133">示例</span><span class="sxs-lookup"><span data-stu-id="8e1a8-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8e1a8-134">请求</span><span class="sxs-lookup"><span data-stu-id="8e1a8-134">Request</span></span>
<span data-ttu-id="8e1a8-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="8e1a8-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_mailfolder"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/me/mailFolders/{id}
```
##### <a name="response"></a><span data-ttu-id="8e1a8-136">响应</span><span class="sxs-lookup"><span data-stu-id="8e1a8-136">Response</span></span>
<span data-ttu-id="8e1a8-137">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="8e1a8-137">Here is an example of the response.</span></span> 
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
