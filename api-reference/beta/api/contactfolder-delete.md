---
title: 删除 contactFolder
description: 删除默认 contactFolder 以外的 contactFolder。
author: kevinbellinger
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 11b8c41506d260702237f4330b449c6f6a6458d5
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43381966"
---
# <a name="delete-contactfolder"></a><span data-ttu-id="71c3d-103">删除 contactFolder</span><span class="sxs-lookup"><span data-stu-id="71c3d-103">Delete contactFolder</span></span>

<span data-ttu-id="71c3d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="71c3d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="71c3d-105">删除默认 contactFolder 以外的 contactFolder。</span><span class="sxs-lookup"><span data-stu-id="71c3d-105">Delete contactFolder other than the default contactFolder.</span></span>
## <a name="permissions"></a><span data-ttu-id="71c3d-106">权限</span><span class="sxs-lookup"><span data-stu-id="71c3d-106">Permissions</span></span>
<span data-ttu-id="71c3d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="71c3d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="71c3d-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="71c3d-109">Permission type</span></span>      | <span data-ttu-id="71c3d-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="71c3d-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="71c3d-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="71c3d-111">Delegated (work or school account)</span></span> | <span data-ttu-id="71c3d-112">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="71c3d-112">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="71c3d-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="71c3d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="71c3d-114">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="71c3d-114">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="71c3d-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="71c3d-115">Application</span></span> | <span data-ttu-id="71c3d-116">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="71c3d-116">Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="71c3d-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="71c3d-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/contactFolders/{id}
DELETE /users/{id | userPrincipalName}/contactFolders/{id}
```
## <a name="request-headers"></a><span data-ttu-id="71c3d-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="71c3d-118">Request headers</span></span>
| <span data-ttu-id="71c3d-119">名称</span><span class="sxs-lookup"><span data-stu-id="71c3d-119">Name</span></span>       | <span data-ttu-id="71c3d-120">类型</span><span class="sxs-lookup"><span data-stu-id="71c3d-120">Type</span></span> | <span data-ttu-id="71c3d-121">说明</span><span class="sxs-lookup"><span data-stu-id="71c3d-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="71c3d-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="71c3d-122">Authorization</span></span>  | <span data-ttu-id="71c3d-123">string</span><span class="sxs-lookup"><span data-stu-id="71c3d-123">string</span></span>  | <span data-ttu-id="71c3d-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="71c3d-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="71c3d-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="71c3d-126">Request body</span></span>
<span data-ttu-id="71c3d-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="71c3d-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="71c3d-128">响应</span><span class="sxs-lookup"><span data-stu-id="71c3d-128">Response</span></span>

<span data-ttu-id="71c3d-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="71c3d-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="71c3d-131">示例</span><span class="sxs-lookup"><span data-stu-id="71c3d-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="71c3d-132">请求</span><span class="sxs-lookup"><span data-stu-id="71c3d-132">Request</span></span>
<span data-ttu-id="71c3d-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="71c3d-133">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="71c3d-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="71c3d-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_contactfolder"
}-->
```http
DELETE https://graph.microsoft.com/beta/me/contactFolders/{id}
```
# <a name="c"></a>[<span data-ttu-id="71c3d-135">C#</span><span class="sxs-lookup"><span data-stu-id="71c3d-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-contactfolder-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="71c3d-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="71c3d-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-contactfolder-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="71c3d-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="71c3d-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-contactfolder-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="71c3d-138">响应</span><span class="sxs-lookup"><span data-stu-id="71c3d-138">Response</span></span>
<span data-ttu-id="71c3d-139">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="71c3d-139">Here is an example of the response.</span></span> 
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
  "description": "Delete contactFolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
