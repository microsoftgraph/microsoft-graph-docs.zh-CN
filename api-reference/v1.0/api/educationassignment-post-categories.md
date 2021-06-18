---
title: 创建 educationCategories
description: 将现有 educationCategory 添加到 educationAssignment
localization_priority: Normal
author: sharad-sharma-msft
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: daf3999953439e383dd5da6b71907aa963b2a13c
ms.sourcegitcommit: 979fe005c74eb99cd971df6b9511b2d3f7fe3cd4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/17/2021
ms.locfileid: "52991308"
---
# <a name="create-educationcategories"></a><span data-ttu-id="662d8-103">创建 educationCategories</span><span class="sxs-lookup"><span data-stu-id="662d8-103">Create educationCategories</span></span>

<span data-ttu-id="662d8-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="662d8-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="662d8-105">将一个或多个现有的 [educationCategory](../resources/educationcategory.md) 对象添加到指定的  [educationAssignment](../resources/educationassignment.md)。</span><span class="sxs-lookup"><span data-stu-id="662d8-105">Add one or more existing [educationCategory](../resources/educationcategory.md) objects to the specified  [educationAssignment](../resources/educationassignment.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="662d8-106">权限</span><span class="sxs-lookup"><span data-stu-id="662d8-106">Permissions</span></span>
<span data-ttu-id="662d8-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="662d8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="662d8-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="662d8-109">Permission type</span></span>      | <span data-ttu-id="662d8-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="662d8-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="662d8-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="662d8-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="662d8-112">EduAssignments.ReadWriteBasic、EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="662d8-112">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="662d8-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="662d8-113">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="662d8-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="662d8-114">Not supported.</span></span>  |
|<span data-ttu-id="662d8-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="662d8-115">Application</span></span> | <span data-ttu-id="662d8-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="662d8-116">Not supported.</span></span>  | 

## <a name="http-request"></a><span data-ttu-id="662d8-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="662d8-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/{id}/assignments/{id}/categories/$ref
```
## <a name="request-headers"></a><span data-ttu-id="662d8-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="662d8-118">Request headers</span></span>
| <span data-ttu-id="662d8-119">标头</span><span class="sxs-lookup"><span data-stu-id="662d8-119">Header</span></span>       | <span data-ttu-id="662d8-120">值</span><span class="sxs-lookup"><span data-stu-id="662d8-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="662d8-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="662d8-121">Authorization</span></span>  | <span data-ttu-id="662d8-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="662d8-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="662d8-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="662d8-124">Content-Type</span></span>  | <span data-ttu-id="662d8-125">application/json</span><span class="sxs-lookup"><span data-stu-id="662d8-125">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="662d8-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="662d8-126">Request body</span></span>
<span data-ttu-id="662d8-127">在请求正文中，odata.id 现有 [educationCategory](../resources/educationcategory.md) () 添加到此分配。</span><span class="sxs-lookup"><span data-stu-id="662d8-127">In the request body, supply the odata.id of the existing [educationCategory](../resources/educationcategory.md) object(s) to add to this assignment.</span></span>


## <a name="response"></a><span data-ttu-id="662d8-128">响应</span><span class="sxs-lookup"><span data-stu-id="662d8-128">Response</span></span>
<span data-ttu-id="662d8-129">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="662d8-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="662d8-130">示例</span><span class="sxs-lookup"><span data-stu-id="662d8-130">Example</span></span>
### <a name="request"></a><span data-ttu-id="662d8-131">请求</span><span class="sxs-lookup"><span data-stu-id="662d8-131">Request</span></span>
<span data-ttu-id="662d8-132">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="662d8-132">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="662d8-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="662d8-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "add_educationcategory_to_educationassignment"
}-->

```http
POST https://graph.microsoft.com/v1.0/education/classes/acdefc6b-2dc6-4e71-b1e9-6d9810ab1793/assignments/ad8afb28-c138-4ad7-b7f5-a6986c2655a8/categories/$ref
Content-type: application/json
Content-length: 212

{
  "@odata.id": "https://graph.microsoft.com/v1.0/education/classes/acdefc6b-2dc6-4e71-b1e9-6d9810ab1793/assignmentCategories/ec98f158-341d-4fea-9f8c-14a250d489ac"
}

```
# <a name="c"></a>[<span data-ttu-id="662d8-134">C#</span><span class="sxs-lookup"><span data-stu-id="662d8-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/add-educationcategory-to-educationassignment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="662d8-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="662d8-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/add-educationcategory-to-educationassignment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="662d8-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="662d8-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/add-educationcategory-to-educationassignment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="662d8-137">Java</span><span class="sxs-lookup"><span data-stu-id="662d8-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/add-educationcategory-to-educationassignment-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="662d8-138">在请求正文中，odata.id 要添加到此分配的现有 [educationCategory](../resources/educationcategory.md) 对象的组。</span><span class="sxs-lookup"><span data-stu-id="662d8-138">In the request body, supply the odata.id of the existing [educationCategory](../resources/educationcategory.md) object to add to this assignment.</span></span>

### <a name="response"></a><span data-ttu-id="662d8-139">响应</span><span class="sxs-lookup"><span data-stu-id="662d8-139">Response</span></span>
<span data-ttu-id="662d8-140">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="662d8-140">The following is an example of the response.</span></span> 

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
  "description": "Add educationCategory to educationAssignment",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


