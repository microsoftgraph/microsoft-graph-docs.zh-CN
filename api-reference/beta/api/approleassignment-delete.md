---
title: 删除 appRoleAssignment
description: 删除 appRoleAssignment。
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: psignoret
ms.openlocfilehash: 2c42171863f336e25e298d0b807839d83376d83d
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "40868318"
---
# <a name="delete-approleassignment"></a><span data-ttu-id="6ea68-103">删除 appRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="6ea68-103">Delete appRoleAssignment</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6ea68-104">删除 appRoleAssignment。</span><span class="sxs-lookup"><span data-stu-id="6ea68-104">Delete appRoleAssignment.</span></span>
## <a name="permissions"></a><span data-ttu-id="6ea68-105">权限</span><span class="sxs-lookup"><span data-stu-id="6ea68-105">Permissions</span></span>
<span data-ttu-id="6ea68-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6ea68-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6ea68-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="6ea68-108">Permission type</span></span>      | <span data-ttu-id="6ea68-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="6ea68-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6ea68-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6ea68-110">Delegated (work or school account)</span></span> | <span data-ttu-id="6ea68-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="6ea68-111">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="6ea68-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6ea68-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6ea68-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="6ea68-113">Not supported.</span></span>    |
|<span data-ttu-id="6ea68-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="6ea68-114">Application</span></span> | <span data-ttu-id="6ea68-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="6ea68-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="6ea68-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6ea68-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /users/{id | userPrincipalName}/appRoleAssignments/{id}
DELETE /groups/{id}/appRoleAssignments/{id}
DELETE /servicePrincipals/{id}/appRoleAssignments/{id}
DELETE /servicePrincipals/{id}/appRoleAssignedTo/{id}

```
## <a name="request-headers"></a><span data-ttu-id="6ea68-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="6ea68-117">Request headers</span></span>
| <span data-ttu-id="6ea68-118">名称</span><span class="sxs-lookup"><span data-stu-id="6ea68-118">Name</span></span>       | <span data-ttu-id="6ea68-119">类型</span><span class="sxs-lookup"><span data-stu-id="6ea68-119">Type</span></span> | <span data-ttu-id="6ea68-120">说明</span><span class="sxs-lookup"><span data-stu-id="6ea68-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="6ea68-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="6ea68-121">Authorization</span></span>  | <span data-ttu-id="6ea68-122">string</span><span class="sxs-lookup"><span data-stu-id="6ea68-122">string</span></span>  | <span data-ttu-id="6ea68-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="6ea68-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6ea68-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="6ea68-125">Request body</span></span>
<span data-ttu-id="6ea68-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="6ea68-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6ea68-127">响应</span><span class="sxs-lookup"><span data-stu-id="6ea68-127">Response</span></span>

<span data-ttu-id="6ea68-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="6ea68-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6ea68-130">示例</span><span class="sxs-lookup"><span data-stu-id="6ea68-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6ea68-131">请求</span><span class="sxs-lookup"><span data-stu-id="6ea68-131">Request</span></span>
<span data-ttu-id="6ea68-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="6ea68-132">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="6ea68-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="6ea68-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_approleassignment"
}-->
```http
DELETE https://graph.microsoft.com/beta/servicePrincipals/{id}/appRoleAssignedTo/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="6ea68-134">C#</span><span class="sxs-lookup"><span data-stu-id="6ea68-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-approleassignment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="6ea68-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6ea68-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-approleassignment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="6ea68-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6ea68-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-approleassignment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="6ea68-137">响应</span><span class="sxs-lookup"><span data-stu-id="6ea68-137">Response</span></span>
<span data-ttu-id="6ea68-138">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="6ea68-138">Here is an example of the response.</span></span> 
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
  "description": "Delete appRoleAssignment",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
