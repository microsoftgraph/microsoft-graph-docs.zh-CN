---
title: 删除 outlookTaskFolder
description: 删除指定的 Outlook 任务文件夹。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 4c526c937f7d92b6e2b0482193f6c0327f4870c1
ms.sourcegitcommit: a17ad12b05fbad86fc21ea4384c36e3b14e543c3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/27/2019
ms.locfileid: "30869384"
---
# <a name="delete-outlooktaskfolder"></a><span data-ttu-id="92dde-103">删除 outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="92dde-103">Delete outlookTaskFolder</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="92dde-104">删除指定的 Outlook 任务文件夹。</span><span class="sxs-lookup"><span data-stu-id="92dde-104">Delete the specified Outlook task folder.</span></span>
## <a name="permissions"></a><span data-ttu-id="92dde-105">权限</span><span class="sxs-lookup"><span data-stu-id="92dde-105">Permissions</span></span>
<span data-ttu-id="92dde-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="92dde-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="92dde-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="92dde-108">Permission type</span></span>      | <span data-ttu-id="92dde-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="92dde-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="92dde-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="92dde-110">Delegated (work or school account)</span></span> | <span data-ttu-id="92dde-111">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="92dde-111">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="92dde-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="92dde-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="92dde-113">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="92dde-113">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="92dde-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="92dde-114">Application</span></span> | <span data-ttu-id="92dde-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="92dde-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="92dde-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="92dde-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/outlook/taskFolders/{id}
DELETE /me/outlook/taskGroups/{id}/taskFolders/{id}
DELETE /users/{id|userPrincipalName}/outlook/taskFolders/{id}
DELETE /users/{id|userPrincipalName}/outlook/taskGroups/{id}/taskFolders/{id}
```
## <a name="request-headers"></a><span data-ttu-id="92dde-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="92dde-117">Request headers</span></span>
| <span data-ttu-id="92dde-118">名称</span><span class="sxs-lookup"><span data-stu-id="92dde-118">Name</span></span>       | <span data-ttu-id="92dde-119">说明</span><span class="sxs-lookup"><span data-stu-id="92dde-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="92dde-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="92dde-120">Authorization</span></span>  | <span data-ttu-id="92dde-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="92dde-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="92dde-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="92dde-123">Request body</span></span>
<span data-ttu-id="92dde-124">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="92dde-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="92dde-125">响应</span><span class="sxs-lookup"><span data-stu-id="92dde-125">Response</span></span>

<span data-ttu-id="92dde-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="92dde-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="92dde-128">示例</span><span class="sxs-lookup"><span data-stu-id="92dde-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="92dde-129">请求</span><span class="sxs-lookup"><span data-stu-id="92dde-129">Request</span></span>
<span data-ttu-id="92dde-130">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="92dde-130">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_outlooktaskfolder"
}-->
```http
DELETE https://graph.microsoft.com/beta/me/outlook/taskFolders('AAMkADIyAAAhrbPXAAA=')
```
##### <a name="response"></a><span data-ttu-id="92dde-131">响应</span><span class="sxs-lookup"><span data-stu-id="92dde-131">Response</span></span>
<span data-ttu-id="92dde-132">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="92dde-132">Here is an example of the response.</span></span> 
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
  "description": "Delete outlookTaskFolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/outlooktaskfolder-delete.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
