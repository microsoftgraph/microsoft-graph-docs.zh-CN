---
title: 删除 educationClass
description: 删除课程。 课程也是通用组，因此删除课程时也会删除组。
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: 594b3ba4676ae054e038747cb7797ffcdaa99ab6
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35436093"
---
# <a name="delete-educationclass"></a><span data-ttu-id="82e62-104">删除 educationClass</span><span class="sxs-lookup"><span data-stu-id="82e62-104">Delete educationClass</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="82e62-105">删除课程。</span><span class="sxs-lookup"><span data-stu-id="82e62-105">Delete a class.</span></span> <span data-ttu-id="82e62-106">课程也是通用组，因此删除课程时也会删除组。</span><span class="sxs-lookup"><span data-stu-id="82e62-106">Because a class is also a universal group, deleting a class deletes the group.</span></span>

## <a name="permissions"></a><span data-ttu-id="82e62-107">权限</span><span class="sxs-lookup"><span data-stu-id="82e62-107">Permissions</span></span>
<span data-ttu-id="82e62-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="82e62-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="82e62-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="82e62-110">Permission type</span></span>      | <span data-ttu-id="82e62-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="82e62-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="82e62-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="82e62-112">Delegated (work or school account)</span></span> |  <span data-ttu-id="82e62-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="82e62-113">Not supported.</span></span>  |
|<span data-ttu-id="82e62-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="82e62-114">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="82e62-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="82e62-115">Not supported.</span></span>  |
|<span data-ttu-id="82e62-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="82e62-116">Application</span></span> | <span data-ttu-id="82e62-117">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="82e62-117">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="82e62-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="82e62-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /education/classes/{id}

```
## <a name="request-headers"></a><span data-ttu-id="82e62-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="82e62-119">Request headers</span></span>
| <span data-ttu-id="82e62-120">标头</span><span class="sxs-lookup"><span data-stu-id="82e62-120">Header</span></span>       | <span data-ttu-id="82e62-121">值</span><span class="sxs-lookup"><span data-stu-id="82e62-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="82e62-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="82e62-122">Authorization</span></span>  | <span data-ttu-id="82e62-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="82e62-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="82e62-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="82e62-125">Request body</span></span>
<span data-ttu-id="82e62-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="82e62-126">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="82e62-127">响应</span><span class="sxs-lookup"><span data-stu-id="82e62-127">Response</span></span>
<span data-ttu-id="82e62-p105">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="82e62-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="82e62-130">示例</span><span class="sxs-lookup"><span data-stu-id="82e62-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="82e62-131">请求</span><span class="sxs-lookup"><span data-stu-id="82e62-131">Request</span></span>
<span data-ttu-id="82e62-132">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="82e62-132">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="82e62-133">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="82e62-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_educationclass"
}-->
```http
DELETE https://graph.microsoft.com/beta/education/classes/11022
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="82e62-134">C#</span><span class="sxs-lookup"><span data-stu-id="82e62-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-educationclass-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="82e62-135">Javascript</span><span class="sxs-lookup"><span data-stu-id="82e62-135">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-educationclass-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="82e62-136">目标-C</span><span class="sxs-lookup"><span data-stu-id="82e62-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-educationclass-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="82e62-137">响应</span><span class="sxs-lookup"><span data-stu-id="82e62-137">Response</span></span>
<span data-ttu-id="82e62-138">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="82e62-138">The following is an example of the response.</span></span> 

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
  "description": "Delete educationClass",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
