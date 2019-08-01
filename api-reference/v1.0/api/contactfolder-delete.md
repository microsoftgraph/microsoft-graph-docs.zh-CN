---
title: 删除 contactFolder
description: 删除默认 contactFolder 以外的 contactFolder。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: be5f222fc59135ad992b11b2eee6d777a387f9c1
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36003222"
---
# <a name="delete-contactfolder"></a><span data-ttu-id="4e1f3-103">删除 contactFolder</span><span class="sxs-lookup"><span data-stu-id="4e1f3-103">Delete contactFolder</span></span>

<span data-ttu-id="4e1f3-104">删除默认 contactFolder 以外的 contactFolder。</span><span class="sxs-lookup"><span data-stu-id="4e1f3-104">Delete contactFolder other than the default contactFolder.</span></span>
## <a name="permissions"></a><span data-ttu-id="4e1f3-105">权限</span><span class="sxs-lookup"><span data-stu-id="4e1f3-105">Permissions</span></span>
<span data-ttu-id="4e1f3-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4e1f3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4e1f3-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="4e1f3-108">Permission type</span></span>      | <span data-ttu-id="4e1f3-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="4e1f3-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4e1f3-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4e1f3-110">Delegated (work or school account)</span></span> | <span data-ttu-id="4e1f3-111">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4e1f3-111">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="4e1f3-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4e1f3-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4e1f3-113">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4e1f3-113">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="4e1f3-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="4e1f3-114">Application</span></span> | <span data-ttu-id="4e1f3-115">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4e1f3-115">Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="4e1f3-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4e1f3-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/contactFolders/{id}
DELETE /users/{id | userPrincipalName}/contactFolders/{id}
```
## <a name="request-headers"></a><span data-ttu-id="4e1f3-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="4e1f3-117">Request headers</span></span>
| <span data-ttu-id="4e1f3-118">名称</span><span class="sxs-lookup"><span data-stu-id="4e1f3-118">Name</span></span>       | <span data-ttu-id="4e1f3-119">类型</span><span class="sxs-lookup"><span data-stu-id="4e1f3-119">Type</span></span> | <span data-ttu-id="4e1f3-120">说明</span><span class="sxs-lookup"><span data-stu-id="4e1f3-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="4e1f3-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="4e1f3-121">Authorization</span></span>  | <span data-ttu-id="4e1f3-122">string</span><span class="sxs-lookup"><span data-stu-id="4e1f3-122">string</span></span>  | <span data-ttu-id="4e1f3-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="4e1f3-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4e1f3-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="4e1f3-125">Request body</span></span>
<span data-ttu-id="4e1f3-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="4e1f3-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4e1f3-127">响应</span><span class="sxs-lookup"><span data-stu-id="4e1f3-127">Response</span></span>

<span data-ttu-id="4e1f3-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="4e1f3-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4e1f3-130">示例</span><span class="sxs-lookup"><span data-stu-id="4e1f3-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4e1f3-131">请求</span><span class="sxs-lookup"><span data-stu-id="4e1f3-131">Request</span></span>
<span data-ttu-id="4e1f3-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="4e1f3-132">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="4e1f3-133">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="4e1f3-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_contactfolder"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/me/contactFolders/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="4e1f3-134">C#</span><span class="sxs-lookup"><span data-stu-id="4e1f3-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-contactfolder-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="4e1f3-135">Javascript</span><span class="sxs-lookup"><span data-stu-id="4e1f3-135">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-contactfolder-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="4e1f3-136">目标-C</span><span class="sxs-lookup"><span data-stu-id="4e1f3-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-contactfolder-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="4e1f3-137">Java</span><span class="sxs-lookup"><span data-stu-id="4e1f3-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-contactfolder-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="4e1f3-138">响应</span><span class="sxs-lookup"><span data-stu-id="4e1f3-138">Response</span></span>
<span data-ttu-id="4e1f3-139">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="4e1f3-139">Here is an example of the response.</span></span> 
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
  "description": "Delete contactFolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
