---
title: 删除 educationUser
description: 删除用户。
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: bc1946d9155227df0bd1d6c7489161faf9c5c4b6
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35459452"
---
# <a name="delete-educationuser"></a><span data-ttu-id="c97b1-103">删除 educationUser</span><span class="sxs-lookup"><span data-stu-id="c97b1-103">Delete educationUser</span></span>

<span data-ttu-id="c97b1-104">删除用户。</span><span class="sxs-lookup"><span data-stu-id="c97b1-104">Delete a user.</span></span>


## <a name="permissions"></a><span data-ttu-id="c97b1-105">权限</span><span class="sxs-lookup"><span data-stu-id="c97b1-105">Permissions</span></span>
<span data-ttu-id="c97b1-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c97b1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c97b1-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="c97b1-108">Permission type</span></span>      | <span data-ttu-id="c97b1-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c97b1-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c97b1-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c97b1-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="c97b1-111">不支持。</span><span class="sxs-lookup"><span data-stu-id="c97b1-111">Not supported.</span></span>  |
|<span data-ttu-id="c97b1-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c97b1-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="c97b1-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="c97b1-113">Not supported.</span></span>  |
|<span data-ttu-id="c97b1-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="c97b1-114">Application</span></span> | <span data-ttu-id="c97b1-115">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c97b1-115">EduRoster.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c97b1-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c97b1-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /education/users/{id}
```
## <a name="request-headers"></a><span data-ttu-id="c97b1-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="c97b1-117">Request headers</span></span>
| <span data-ttu-id="c97b1-118">标头</span><span class="sxs-lookup"><span data-stu-id="c97b1-118">Header</span></span>       | <span data-ttu-id="c97b1-119">值</span><span class="sxs-lookup"><span data-stu-id="c97b1-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="c97b1-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="c97b1-120">Authorization</span></span>  | <span data-ttu-id="c97b1-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="c97b1-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="c97b1-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="c97b1-123">Request body</span></span>
<span data-ttu-id="c97b1-124">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="c97b1-124">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="c97b1-125">响应</span><span class="sxs-lookup"><span data-stu-id="c97b1-125">Response</span></span>
<span data-ttu-id="c97b1-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="c97b1-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c97b1-128">示例</span><span class="sxs-lookup"><span data-stu-id="c97b1-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c97b1-129">请求</span><span class="sxs-lookup"><span data-stu-id="c97b1-129">Request</span></span>
<span data-ttu-id="c97b1-130">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="c97b1-130">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="c97b1-131">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="c97b1-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_educationuser"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/education/users/{user-id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="c97b1-132">C#</span><span class="sxs-lookup"><span data-stu-id="c97b1-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-educationuser-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c97b1-133">Javascript</span><span class="sxs-lookup"><span data-stu-id="c97b1-133">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-educationuser-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="c97b1-134">目标-C</span><span class="sxs-lookup"><span data-stu-id="c97b1-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-educationuser-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="c97b1-135">响应</span><span class="sxs-lookup"><span data-stu-id="c97b1-135">Response</span></span>
<span data-ttu-id="c97b1-136">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="c97b1-136">The following is an example of the response.</span></span> 
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
  "description": "Delete educationUser",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
