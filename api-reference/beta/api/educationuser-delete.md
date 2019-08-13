---
title: 删除 educationUser
description: 删除用户。
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 11d79b905b687f94e3cd5e7fc089cba90b18ac0d
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36323802"
---
# <a name="delete-educationuser"></a><span data-ttu-id="9c8a7-103">删除 educationUser</span><span class="sxs-lookup"><span data-stu-id="9c8a7-103">Delete educationUser</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9c8a7-104">删除用户。</span><span class="sxs-lookup"><span data-stu-id="9c8a7-104">Delete a user.</span></span>


## <a name="permissions"></a><span data-ttu-id="9c8a7-105">权限</span><span class="sxs-lookup"><span data-stu-id="9c8a7-105">Permissions</span></span>
<span data-ttu-id="9c8a7-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9c8a7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9c8a7-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="9c8a7-108">Permission type</span></span>      | <span data-ttu-id="9c8a7-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="9c8a7-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9c8a7-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9c8a7-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="9c8a7-111">不支持。</span><span class="sxs-lookup"><span data-stu-id="9c8a7-111">Not supported.</span></span>  |
|<span data-ttu-id="9c8a7-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9c8a7-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="9c8a7-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="9c8a7-113">Not supported.</span></span>  |
|<span data-ttu-id="9c8a7-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="9c8a7-114">Application</span></span> | <span data-ttu-id="9c8a7-115">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9c8a7-115">EduRoster.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="9c8a7-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9c8a7-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /education/users/{id}
```
## <a name="request-headers"></a><span data-ttu-id="9c8a7-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="9c8a7-117">Request headers</span></span>
| <span data-ttu-id="9c8a7-118">标头</span><span class="sxs-lookup"><span data-stu-id="9c8a7-118">Header</span></span>       | <span data-ttu-id="9c8a7-119">值</span><span class="sxs-lookup"><span data-stu-id="9c8a7-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="9c8a7-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="9c8a7-120">Authorization</span></span>  | <span data-ttu-id="9c8a7-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="9c8a7-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="9c8a7-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="9c8a7-123">Request body</span></span>
<span data-ttu-id="9c8a7-124">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="9c8a7-124">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="9c8a7-125">响应</span><span class="sxs-lookup"><span data-stu-id="9c8a7-125">Response</span></span>
<span data-ttu-id="9c8a7-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="9c8a7-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9c8a7-128">示例</span><span class="sxs-lookup"><span data-stu-id="9c8a7-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9c8a7-129">请求</span><span class="sxs-lookup"><span data-stu-id="9c8a7-129">Request</span></span>
<span data-ttu-id="9c8a7-130">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="9c8a7-130">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="9c8a7-131">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="9c8a7-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_educationuser"
}-->
```http
DELETE https://graph.microsoft.com/beta/education/users/13019
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="9c8a7-132">C#</span><span class="sxs-lookup"><span data-stu-id="9c8a7-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-educationuser-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="9c8a7-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9c8a7-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-educationuser-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="9c8a7-134">目标-C</span><span class="sxs-lookup"><span data-stu-id="9c8a7-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-educationuser-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="9c8a7-135">Java</span><span class="sxs-lookup"><span data-stu-id="9c8a7-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-educationuser-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="9c8a7-136">响应</span><span class="sxs-lookup"><span data-stu-id="9c8a7-136">Response</span></span>
<span data-ttu-id="9c8a7-137">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="9c8a7-137">The following is an example of the response.</span></span> 
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
  "description": "Delete educationUser",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
