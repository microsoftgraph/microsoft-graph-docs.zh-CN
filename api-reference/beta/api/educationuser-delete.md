---
title: 删除 educationUser
description: 删除用户。
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 87f94494c88ae4869d4aaa56b422cfe66695ce92
ms.sourcegitcommit: e4b0211db9b20dfea8be964003661cd99fe064d1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/10/2019
ms.locfileid: "37439795"
---
# <a name="delete-educationuser"></a><span data-ttu-id="249f6-103">删除 educationUser</span><span class="sxs-lookup"><span data-stu-id="249f6-103">Delete educationUser</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="249f6-104">删除用户。</span><span class="sxs-lookup"><span data-stu-id="249f6-104">Delete a user.</span></span>

## <a name="permissions"></a><span data-ttu-id="249f6-105">权限</span><span class="sxs-lookup"><span data-stu-id="249f6-105">Permissions</span></span>

<span data-ttu-id="249f6-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="249f6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="249f6-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="249f6-108">Permission type</span></span>                        | <span data-ttu-id="249f6-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="249f6-109">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="249f6-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="249f6-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="249f6-111">不支持。</span><span class="sxs-lookup"><span data-stu-id="249f6-111">Not supported.</span></span>                              |
| <span data-ttu-id="249f6-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="249f6-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="249f6-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="249f6-113">Not supported.</span></span>                              |
| <span data-ttu-id="249f6-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="249f6-114">Application</span></span>                            | <span data-ttu-id="249f6-115">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="249f6-115">EduRoster.ReadWrite.All</span></span>                     |

## <a name="http-request"></a><span data-ttu-id="249f6-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="249f6-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /education/users/{id}
```

## <a name="request-headers"></a><span data-ttu-id="249f6-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="249f6-117">Request headers</span></span>

| <span data-ttu-id="249f6-118">标头</span><span class="sxs-lookup"><span data-stu-id="249f6-118">Header</span></span>        | <span data-ttu-id="249f6-119">值</span><span class="sxs-lookup"><span data-stu-id="249f6-119">Value</span></span>                     |
| :------------ | :------------------------ |
| <span data-ttu-id="249f6-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="249f6-120">Authorization</span></span> | <span data-ttu-id="249f6-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="249f6-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="249f6-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="249f6-123">Request body</span></span>

<span data-ttu-id="249f6-124">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="249f6-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="249f6-125">响应</span><span class="sxs-lookup"><span data-stu-id="249f6-125">Response</span></span>

<span data-ttu-id="249f6-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="249f6-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="249f6-128">示例</span><span class="sxs-lookup"><span data-stu-id="249f6-128">Example</span></span>

##### <a name="request"></a><span data-ttu-id="249f6-129">请求</span><span class="sxs-lookup"><span data-stu-id="249f6-129">Request</span></span>

<span data-ttu-id="249f6-130">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="249f6-130">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="249f6-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="249f6-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_educationuser"
}-->
```http
DELETE https://graph.microsoft.com/beta/education/users/13019
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="249f6-132">C#</span><span class="sxs-lookup"><span data-stu-id="249f6-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-educationuser-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="249f6-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="249f6-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-educationuser-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="249f6-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="249f6-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-educationuser-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="249f6-135">响应</span><span class="sxs-lookup"><span data-stu-id="249f6-135">Response</span></span>

<span data-ttu-id="249f6-136">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="249f6-136">The following is an example of the response.</span></span> 
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
