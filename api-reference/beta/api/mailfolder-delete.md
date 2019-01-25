---
title: 删除 mailFolder
description: 删除指定的 mailFolder 或 mailSearchFolder。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: e993d4cb770db546a11e80aa9b9fe24501e2b281
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29512995"
---
# <a name="delete-mailfolder"></a><span data-ttu-id="68ee0-103">删除 mailFolder</span><span class="sxs-lookup"><span data-stu-id="68ee0-103">Delete mailFolder</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="68ee0-104">删除指定的[mailFolder](../resources/mailfolder.md)或[mailSearchFolder](../resources/mailsearchfolder.md)。</span><span class="sxs-lookup"><span data-stu-id="68ee0-104">Delete the specified [mailFolder](../resources/mailfolder.md) or [mailSearchFolder](../resources/mailsearchfolder.md).</span></span>

<span data-ttu-id="68ee0-105">如果存在，您可以指定由其文件夹 ID，或按[已知文件夹名称](../resources/mailfolder.md)的邮件文件夹。</span><span class="sxs-lookup"><span data-stu-id="68ee0-105">You can specify a mail folder by its folder ID, or by its [well-known folder name](../resources/mailfolder.md), if one exists.</span></span> 

><span data-ttu-id="68ee0-106">**注释**您可能不能删除可恢复邮件删除文件夹中的项目 (由已知文件夹名称`recoverableitemsdeletions`)。</span><span class="sxs-lookup"><span data-stu-id="68ee0-106">**Note** You may not be able to delete items in the recoverable items deletions folder (represented by the well-known folder name `recoverableitemsdeletions`).</span></span> <span data-ttu-id="68ee0-107">有关详细信息，请参阅[已删除邮件的保留期](https://docs.microsoft.com/en-us/exchange/policy-and-compliance/recoverable-items-folder/recoverable-items-folder#deleted-item-retention)和[清理已删除项目](https://docs.microsoft.com/en-us/exchange/policy-and-compliance/recoverable-items-folder/clean-up-deleted-items)。</span><span class="sxs-lookup"><span data-stu-id="68ee0-107">See [Deleted item retention](https://docs.microsoft.com/en-us/exchange/policy-and-compliance/recoverable-items-folder/recoverable-items-folder#deleted-item-retention) and [Clean up deleted items](https://docs.microsoft.com/en-us/exchange/policy-and-compliance/recoverable-items-folder/clean-up-deleted-items) for more information.</span></span>

## <a name="permissions"></a><span data-ttu-id="68ee0-108">权限</span><span class="sxs-lookup"><span data-stu-id="68ee0-108">Permissions</span></span>
<span data-ttu-id="68ee0-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="68ee0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="68ee0-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="68ee0-111">Permission type</span></span>      | <span data-ttu-id="68ee0-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="68ee0-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="68ee0-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="68ee0-113">Delegated (work or school account)</span></span> | <span data-ttu-id="68ee0-114">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="68ee0-114">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="68ee0-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="68ee0-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="68ee0-116">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="68ee0-116">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="68ee0-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="68ee0-117">Application</span></span> | <span data-ttu-id="68ee0-118">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="68ee0-118">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="68ee0-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="68ee0-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/mailFolders/{id}
DELETE /users/{id | userPrincipalName}/mailFolders/{id}
```
## <a name="request-headers"></a><span data-ttu-id="68ee0-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="68ee0-120">Request headers</span></span>
| <span data-ttu-id="68ee0-121">名称</span><span class="sxs-lookup"><span data-stu-id="68ee0-121">Name</span></span>       | <span data-ttu-id="68ee0-122">类型</span><span class="sxs-lookup"><span data-stu-id="68ee0-122">Type</span></span> | <span data-ttu-id="68ee0-123">说明</span><span class="sxs-lookup"><span data-stu-id="68ee0-123">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="68ee0-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="68ee0-124">Authorization</span></span>  | <span data-ttu-id="68ee0-125">string</span><span class="sxs-lookup"><span data-stu-id="68ee0-125">string</span></span>  | <span data-ttu-id="68ee0-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="68ee0-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="68ee0-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="68ee0-128">Request body</span></span>
<span data-ttu-id="68ee0-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="68ee0-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="68ee0-130">响应</span><span class="sxs-lookup"><span data-stu-id="68ee0-130">Response</span></span>
<span data-ttu-id="68ee0-p104">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="68ee0-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="68ee0-133">示例</span><span class="sxs-lookup"><span data-stu-id="68ee0-133">Example</span></span>
#### <a name="request"></a><span data-ttu-id="68ee0-134">请求</span><span class="sxs-lookup"><span data-stu-id="68ee0-134">Request</span></span>
<span data-ttu-id="68ee0-135">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="68ee0-135">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_mailfolder"
}-->
```http
DELETE https://graph.microsoft.com/beta/me/mailFolders/AAMkAGVmMDEzM/
```

#### <a name="response"></a><span data-ttu-id="68ee0-136">响应</span><span class="sxs-lookup"><span data-stu-id="68ee0-136">Response</span></span>
<span data-ttu-id="68ee0-137">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="68ee0-137">The following is an example of the response.</span></span> 
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
    "Error: /api-reference/beta/api/mailfolder-delete.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
