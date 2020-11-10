---
title: 删除 educationClass
description: 删除课程。 课程也是通用组，因此删除课程时也会删除组。
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 84ac58abc25a8cf0d7559179692372db9e1b936a
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48966362"
---
# <a name="delete-educationclass"></a><span data-ttu-id="bd67f-104">删除 educationClass</span><span class="sxs-lookup"><span data-stu-id="bd67f-104">Delete educationClass</span></span>

<span data-ttu-id="bd67f-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bd67f-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bd67f-106">删除课程。</span><span class="sxs-lookup"><span data-stu-id="bd67f-106">Delete a class.</span></span> <span data-ttu-id="bd67f-107">课程也是通用组，因此删除课程时也会删除组。</span><span class="sxs-lookup"><span data-stu-id="bd67f-107">Because a class is also a universal group, deleting a class deletes the group.</span></span>

## <a name="permissions"></a><span data-ttu-id="bd67f-108">权限</span><span class="sxs-lookup"><span data-stu-id="bd67f-108">Permissions</span></span>
<span data-ttu-id="bd67f-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="bd67f-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bd67f-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="bd67f-111">Permission type</span></span>      | <span data-ttu-id="bd67f-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="bd67f-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bd67f-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="bd67f-113">Delegated (work or school account)</span></span> |  <span data-ttu-id="bd67f-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="bd67f-114">Not supported.</span></span>  |
|<span data-ttu-id="bd67f-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="bd67f-115">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="bd67f-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="bd67f-116">Not supported.</span></span>  |
|<span data-ttu-id="bd67f-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="bd67f-117">Application</span></span> | <span data-ttu-id="bd67f-118">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bd67f-118">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="bd67f-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="bd67f-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /education/classes/{id}

```
## <a name="request-headers"></a><span data-ttu-id="bd67f-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="bd67f-120">Request headers</span></span>
| <span data-ttu-id="bd67f-121">标头</span><span class="sxs-lookup"><span data-stu-id="bd67f-121">Header</span></span>       | <span data-ttu-id="bd67f-122">值</span><span class="sxs-lookup"><span data-stu-id="bd67f-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="bd67f-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="bd67f-123">Authorization</span></span>  | <span data-ttu-id="bd67f-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="bd67f-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="bd67f-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="bd67f-126">Request body</span></span>
<span data-ttu-id="bd67f-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="bd67f-127">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="bd67f-128">响应</span><span class="sxs-lookup"><span data-stu-id="bd67f-128">Response</span></span>
<span data-ttu-id="bd67f-p105">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="bd67f-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bd67f-131">示例</span><span class="sxs-lookup"><span data-stu-id="bd67f-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="bd67f-132">请求</span><span class="sxs-lookup"><span data-stu-id="bd67f-132">Request</span></span>
<span data-ttu-id="bd67f-133">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="bd67f-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="bd67f-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="bd67f-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_educationclass"
}-->
```http
DELETE https://graph.microsoft.com/beta/education/classes/11022
```
# <a name="c"></a>[<span data-ttu-id="bd67f-135">C#</span><span class="sxs-lookup"><span data-stu-id="bd67f-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-educationclass-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="bd67f-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="bd67f-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-educationclass-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="bd67f-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="bd67f-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-educationclass-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="bd67f-138">Java</span><span class="sxs-lookup"><span data-stu-id="bd67f-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-educationclass-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="bd67f-139">响应</span><span class="sxs-lookup"><span data-stu-id="bd67f-139">Response</span></span>
<span data-ttu-id="bd67f-140">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="bd67f-140">The following is an example of the response.</span></span> 

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


