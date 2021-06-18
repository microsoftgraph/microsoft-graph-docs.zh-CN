---
title: 删除 educationCategory
description: 从此 educationAssignment 中删除现有 educationCategory
localization_priority: Normal
author: sharad-sharma-msft
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 70bde8c8549486347542ff90f9088f1c78bde14a
ms.sourcegitcommit: 979fe005c74eb99cd971df6b9511b2d3f7fe3cd4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/17/2021
ms.locfileid: "52992469"
---
# <a name="remove-educationcategory"></a><span data-ttu-id="0cd2f-103">删除 educationCategory</span><span class="sxs-lookup"><span data-stu-id="0cd2f-103">Remove educationCategory</span></span>

<span data-ttu-id="0cd2f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0cd2f-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="0cd2f-105">从[educationAssignment](../resources/educationcategory.md)中删除[educationCategory。](../resources/educationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="0cd2f-105">Remove an [educationCategory](../resources/educationcategory.md) from an [educationAssignment](../resources/educationassignment.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="0cd2f-106">权限</span><span class="sxs-lookup"><span data-stu-id="0cd2f-106">Permissions</span></span>
<span data-ttu-id="0cd2f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0cd2f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0cd2f-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="0cd2f-109">Permission type</span></span>      | <span data-ttu-id="0cd2f-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="0cd2f-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0cd2f-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0cd2f-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="0cd2f-112">EduAssignments.ReadWriteBasic、EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0cd2f-112">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="0cd2f-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0cd2f-113">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="0cd2f-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="0cd2f-114">Not supported.</span></span>  |
|<span data-ttu-id="0cd2f-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="0cd2f-115">Application</span></span> | <span data-ttu-id="0cd2f-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="0cd2f-116">Not supported.</span></span>  | 

## <a name="http-request"></a><span data-ttu-id="0cd2f-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0cd2f-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /education/classes/{id}/assignments/{id}/categories/{id}/$ref
```
## <a name="request-headers"></a><span data-ttu-id="0cd2f-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="0cd2f-118">Request headers</span></span>
| <span data-ttu-id="0cd2f-119">标头</span><span class="sxs-lookup"><span data-stu-id="0cd2f-119">Header</span></span>       | <span data-ttu-id="0cd2f-120">值</span><span class="sxs-lookup"><span data-stu-id="0cd2f-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="0cd2f-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="0cd2f-121">Authorization</span></span>  | <span data-ttu-id="0cd2f-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="0cd2f-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="0cd2f-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="0cd2f-124">Content-Type</span></span>  | <span data-ttu-id="0cd2f-125">application/json</span><span class="sxs-lookup"><span data-stu-id="0cd2f-125">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="0cd2f-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="0cd2f-126">Request body</span></span>
<span data-ttu-id="0cd2f-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="0cd2f-127">Don't supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0cd2f-128">响应</span><span class="sxs-lookup"><span data-stu-id="0cd2f-128">Response</span></span>
<span data-ttu-id="0cd2f-129">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="0cd2f-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="0cd2f-130">示例</span><span class="sxs-lookup"><span data-stu-id="0cd2f-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="0cd2f-131">请求</span><span class="sxs-lookup"><span data-stu-id="0cd2f-131">Request</span></span>
<span data-ttu-id="0cd2f-132">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="0cd2f-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="0cd2f-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="0cd2f-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["ec98f158-341d-4fea-9f8c-14a250d489ac"],
  "name": "add_educationcategory_to_educationassignment"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/education/classes/acdefc6b-2dc6-4e71-b1e9-6d9810ab1793/assignments/ad8afb28-c138-4ad7-b7f5-a6986c2655a8/categories/ec98f158-341d-4fea-9f8c-14a250d489ac/$ref
```
# <a name="c"></a>[<span data-ttu-id="0cd2f-134">C#</span><span class="sxs-lookup"><span data-stu-id="0cd2f-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/add-educationcategory-to-educationassignment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0cd2f-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0cd2f-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/add-educationcategory-to-educationassignment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0cd2f-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0cd2f-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/add-educationcategory-to-educationassignment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="0cd2f-137">Java</span><span class="sxs-lookup"><span data-stu-id="0cd2f-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/add-educationcategory-to-educationassignment-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="0cd2f-138">响应</span><span class="sxs-lookup"><span data-stu-id="0cd2f-138">Response</span></span>
<span data-ttu-id="0cd2f-139">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="0cd2f-139">The following is an example of the response.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationAssignmentResource"
} -->
```http
HTTP/1.1 204 No Content

{
}
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Remove an educationCategory from an educationAssignment",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


