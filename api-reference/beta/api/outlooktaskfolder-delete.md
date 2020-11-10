---
title: 删除 outlookTaskFolder
description: 删除指定的 Outlook 任务文件夹。
author: mashriv
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: ceeb91c23181c7fcadf13aaf64153b6494e6a4e5
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48974832"
---
# <a name="delete-outlooktaskfolder-deprecated"></a><span data-ttu-id="dc005-103">删除 outlookTaskFolder (弃用) </span><span class="sxs-lookup"><span data-stu-id="dc005-103">Delete outlookTaskFolder (deprecated)</span></span>

<span data-ttu-id="dc005-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dc005-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [outlooktask-deprecate-allup](../../includes/outlooktask-deprecate-allup.md)]


<span data-ttu-id="dc005-105">删除指定的 Outlook 任务文件夹。</span><span class="sxs-lookup"><span data-stu-id="dc005-105">Delete the specified Outlook task folder.</span></span>
## <a name="permissions"></a><span data-ttu-id="dc005-106">权限</span><span class="sxs-lookup"><span data-stu-id="dc005-106">Permissions</span></span>
<span data-ttu-id="dc005-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="dc005-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dc005-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="dc005-109">Permission type</span></span>      | <span data-ttu-id="dc005-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="dc005-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="dc005-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="dc005-111">Delegated (work or school account)</span></span> | <span data-ttu-id="dc005-112">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="dc005-112">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="dc005-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="dc005-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dc005-114">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="dc005-114">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="dc005-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="dc005-115">Application</span></span> | <span data-ttu-id="dc005-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="dc005-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="dc005-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="dc005-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/outlook/taskFolders/{id}
DELETE /me/outlook/taskGroups/{id}/taskFolders/{id}
DELETE /users/{id|userPrincipalName}/outlook/taskFolders/{id}
DELETE /users/{id|userPrincipalName}/outlook/taskGroups/{id}/taskFolders/{id}
```
## <a name="request-headers"></a><span data-ttu-id="dc005-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="dc005-118">Request headers</span></span>
| <span data-ttu-id="dc005-119">名称</span><span class="sxs-lookup"><span data-stu-id="dc005-119">Name</span></span>       | <span data-ttu-id="dc005-120">说明</span><span class="sxs-lookup"><span data-stu-id="dc005-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="dc005-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="dc005-121">Authorization</span></span>  | <span data-ttu-id="dc005-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="dc005-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="dc005-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="dc005-124">Request body</span></span>
<span data-ttu-id="dc005-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="dc005-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="dc005-126">响应</span><span class="sxs-lookup"><span data-stu-id="dc005-126">Response</span></span>

<span data-ttu-id="dc005-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="dc005-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dc005-129">示例</span><span class="sxs-lookup"><span data-stu-id="dc005-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="dc005-130">请求</span><span class="sxs-lookup"><span data-stu-id="dc005-130">Request</span></span>
<span data-ttu-id="dc005-131">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="dc005-131">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="dc005-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="dc005-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_outlooktaskfolder"
}-->
```http
DELETE https://graph.microsoft.com/beta/me/outlook/taskFolders/AAMkADIyAAAhrbPXAAA=
```
# <a name="c"></a>[<span data-ttu-id="dc005-133">C#</span><span class="sxs-lookup"><span data-stu-id="dc005-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-outlooktaskfolder-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="dc005-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="dc005-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-outlooktaskfolder-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="dc005-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="dc005-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-outlooktaskfolder-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="dc005-136">Java</span><span class="sxs-lookup"><span data-stu-id="dc005-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-outlooktaskfolder-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="dc005-137">响应</span><span class="sxs-lookup"><span data-stu-id="dc005-137">Response</span></span>
<span data-ttu-id="dc005-138">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="dc005-138">Here is an example of the response.</span></span> 
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
  ]
}
-->


