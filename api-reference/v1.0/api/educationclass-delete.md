---
title: 删除 educationClass
description: 删除课程。 课程也是通用组，因此删除课程时也会删除组。
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 2f4920ec1d1db2603122fdc72961e758d8222d87
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36370492"
---
# <a name="delete-educationclass"></a><span data-ttu-id="4397f-104">删除 educationClass</span><span class="sxs-lookup"><span data-stu-id="4397f-104">Delete educationClass</span></span>

<span data-ttu-id="4397f-105">删除课程。</span><span class="sxs-lookup"><span data-stu-id="4397f-105">Delete a class.</span></span> <span data-ttu-id="4397f-106">课程也是通用组，因此删除课程时也会删除组。</span><span class="sxs-lookup"><span data-stu-id="4397f-106">Because a class is also a universal group, deleting a class deletes the group.</span></span>

## <a name="permissions"></a><span data-ttu-id="4397f-107">权限</span><span class="sxs-lookup"><span data-stu-id="4397f-107">Permissions</span></span>
<span data-ttu-id="4397f-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4397f-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4397f-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="4397f-110">Permission type</span></span>      | <span data-ttu-id="4397f-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="4397f-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4397f-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4397f-112">Delegated (work or school account)</span></span> |  <span data-ttu-id="4397f-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="4397f-113">Not supported.</span></span>  |
|<span data-ttu-id="4397f-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4397f-114">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="4397f-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="4397f-115">Not supported.</span></span>  |
|<span data-ttu-id="4397f-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="4397f-116">Application</span></span> | <span data-ttu-id="4397f-117">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4397f-117">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="4397f-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4397f-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /education/classes/{id}

```
## <a name="request-headers"></a><span data-ttu-id="4397f-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="4397f-119">Request headers</span></span>
| <span data-ttu-id="4397f-120">标头</span><span class="sxs-lookup"><span data-stu-id="4397f-120">Header</span></span>       | <span data-ttu-id="4397f-121">值</span><span class="sxs-lookup"><span data-stu-id="4397f-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="4397f-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="4397f-122">Authorization</span></span>  | <span data-ttu-id="4397f-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="4397f-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="4397f-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="4397f-125">Request body</span></span>
<span data-ttu-id="4397f-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="4397f-126">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="4397f-127">响应</span><span class="sxs-lookup"><span data-stu-id="4397f-127">Response</span></span>
<span data-ttu-id="4397f-p105">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="4397f-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4397f-130">示例</span><span class="sxs-lookup"><span data-stu-id="4397f-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4397f-131">请求</span><span class="sxs-lookup"><span data-stu-id="4397f-131">Request</span></span>
<span data-ttu-id="4397f-132">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="4397f-132">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="4397f-133">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="4397f-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_educationclass"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/education/classes/{class-id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="4397f-134">C#</span><span class="sxs-lookup"><span data-stu-id="4397f-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-educationclass-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="4397f-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4397f-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-educationclass-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="4397f-136">目标-C</span><span class="sxs-lookup"><span data-stu-id="4397f-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-educationclass-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="4397f-137">Java</span><span class="sxs-lookup"><span data-stu-id="4397f-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-educationclass-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="4397f-138">响应</span><span class="sxs-lookup"><span data-stu-id="4397f-138">Response</span></span>
<span data-ttu-id="4397f-139">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="4397f-139">The following is an example of the response.</span></span> 

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
  "description": "Delete educationClass",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
