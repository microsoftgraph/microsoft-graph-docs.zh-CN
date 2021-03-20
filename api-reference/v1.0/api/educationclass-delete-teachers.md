---
title: 删除 teacher
description: 从课程中删除教师。
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 8905fec82f2db5ad9605481dee54e36b4b5fb208
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50943545"
---
# <a name="remove-teacher"></a><span data-ttu-id="464c5-103">删除教师</span><span class="sxs-lookup"><span data-stu-id="464c5-103">Remove teacher</span></span>

<span data-ttu-id="464c5-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="464c5-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="464c5-105">从课程中删除教师。</span><span class="sxs-lookup"><span data-stu-id="464c5-105">Remove a teacher from a class.</span></span>

## <a name="permissions"></a><span data-ttu-id="464c5-106">权限</span><span class="sxs-lookup"><span data-stu-id="464c5-106">Permissions</span></span>
<span data-ttu-id="464c5-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="464c5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="464c5-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="464c5-109">Permission type</span></span>      | <span data-ttu-id="464c5-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="464c5-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="464c5-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="464c5-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="464c5-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="464c5-112">Not supported.</span></span>  |
|<span data-ttu-id="464c5-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="464c5-113">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="464c5-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="464c5-114">Not supported.</span></span>  |
|<span data-ttu-id="464c5-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="464c5-115">Application</span></span> | <span data-ttu-id="464c5-116">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="464c5-116">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="464c5-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="464c5-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /education/classes/{id}/teachers/{userId}/$ref
```
## <a name="request-headers"></a><span data-ttu-id="464c5-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="464c5-118">Request headers</span></span>
| <span data-ttu-id="464c5-119">标头</span><span class="sxs-lookup"><span data-stu-id="464c5-119">Header</span></span>       | <span data-ttu-id="464c5-120">值</span><span class="sxs-lookup"><span data-stu-id="464c5-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="464c5-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="464c5-121">Authorization</span></span>  | <span data-ttu-id="464c5-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="464c5-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="464c5-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="464c5-124">Request body</span></span>
<span data-ttu-id="464c5-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="464c5-125">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="464c5-126">响应</span><span class="sxs-lookup"><span data-stu-id="464c5-126">Response</span></span>
<span data-ttu-id="464c5-127">如果成功，此方法将返回 `204 No Content` 响应代码和空响应正文。</span><span class="sxs-lookup"><span data-stu-id="464c5-127">If successful, this method returns a `204 No Content` response code and an empty response body.</span></span>

## <a name="example"></a><span data-ttu-id="464c5-128">示例</span><span class="sxs-lookup"><span data-stu-id="464c5-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="464c5-129">请求</span><span class="sxs-lookup"><span data-stu-id="464c5-129">Request</span></span>
<span data-ttu-id="464c5-130">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="464c5-130">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="464c5-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="464c5-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_educationclass_from_educationschool_2"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/education/classes/{class-id}/teachers/{teacher-id}
```
# <a name="c"></a>[<span data-ttu-id="464c5-132">C#</span><span class="sxs-lookup"><span data-stu-id="464c5-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-educationclass-from-educationschool-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="464c5-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="464c5-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-educationclass-from-educationschool-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="464c5-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="464c5-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-educationclass-from-educationschool-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="464c5-135">Java</span><span class="sxs-lookup"><span data-stu-id="464c5-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-educationclass-from-educationschool-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="464c5-136">响应</span><span class="sxs-lookup"><span data-stu-id="464c5-136">Response</span></span>
<span data-ttu-id="464c5-137">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="464c5-137">The following is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationClass"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create educationClass",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

