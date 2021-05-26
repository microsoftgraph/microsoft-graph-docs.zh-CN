---
title: 删除 educationSubmissionResource
description: 从提交中删除资源。 此操作仅能由学生完成。 如果从工作分配复制了资源，将在删除当前副本后创建资源的新副本。
author: dipakboyed
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: f989c1854ee952b53bfd5df123e425bd25a0d2ca
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/26/2021
ms.locfileid: "52664753"
---
# <a name="delete-educationsubmissionresource"></a><span data-ttu-id="2c7ab-105">删除 educationSubmissionResource</span><span class="sxs-lookup"><span data-stu-id="2c7ab-105">Delete educationSubmissionResource</span></span>

<span data-ttu-id="2c7ab-106">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2c7ab-106">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2c7ab-107">从提交中删除资源。</span><span class="sxs-lookup"><span data-stu-id="2c7ab-107">Deletes a resource from the submission.</span></span> <span data-ttu-id="2c7ab-108">此操作仅能由学生完成。</span><span class="sxs-lookup"><span data-stu-id="2c7ab-108">This can only be done by the student.</span></span> <span data-ttu-id="2c7ab-109">如果从工作分配复制了资源，将在删除当前副本后创建资源的新副本。</span><span class="sxs-lookup"><span data-stu-id="2c7ab-109">If the resource was copied from the assignment, a new copy of the resource will be created after the current copy is deleted.</span></span> <span data-ttu-id="2c7ab-110">这允许您将资源"重置"到其原始状态。</span><span class="sxs-lookup"><span data-stu-id="2c7ab-110">This allows you to "reset" the resource to its original state.</span></span> <span data-ttu-id="2c7ab-111">如果资源不是从作业中复制的，而是从学生添加的，则只会删除该资源。</span><span class="sxs-lookup"><span data-stu-id="2c7ab-111">If the resource was not copied from the assignment but was added from the student, the resource is simply deleted.</span></span>

## <a name="permissions"></a><span data-ttu-id="2c7ab-112">权限</span><span class="sxs-lookup"><span data-stu-id="2c7ab-112">Permissions</span></span>
<span data-ttu-id="2c7ab-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2c7ab-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2c7ab-115">权限类型</span><span class="sxs-lookup"><span data-stu-id="2c7ab-115">Permission type</span></span>      | <span data-ttu-id="2c7ab-116">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="2c7ab-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2c7ab-117">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2c7ab-117">Delegated (work or school account)</span></span> |  <span data-ttu-id="2c7ab-118">EduAssignments.ReadWriteBasic、EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2c7ab-118">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="2c7ab-119">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2c7ab-119">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="2c7ab-120">不支持。</span><span class="sxs-lookup"><span data-stu-id="2c7ab-120">Not supported.</span></span>  |
|<span data-ttu-id="2c7ab-121">应用程序</span><span class="sxs-lookup"><span data-stu-id="2c7ab-121">Application</span></span> | <span data-ttu-id="2c7ab-122">不支持。</span><span class="sxs-lookup"><span data-stu-id="2c7ab-122">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="2c7ab-123">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2c7ab-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /education/classes/{id}/assignments/{id}/submissions/{id}/resources/{id}
```

## <a name="request-headers"></a><span data-ttu-id="2c7ab-124">请求标头</span><span class="sxs-lookup"><span data-stu-id="2c7ab-124">Request headers</span></span>
| <span data-ttu-id="2c7ab-125">标头</span><span class="sxs-lookup"><span data-stu-id="2c7ab-125">Header</span></span>       | <span data-ttu-id="2c7ab-126">值</span><span class="sxs-lookup"><span data-stu-id="2c7ab-126">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="2c7ab-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="2c7ab-127">Authorization</span></span>  | <span data-ttu-id="2c7ab-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="2c7ab-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="2c7ab-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="2c7ab-130">Request body</span></span>
<span data-ttu-id="2c7ab-131">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="2c7ab-131">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="2c7ab-132">响应</span><span class="sxs-lookup"><span data-stu-id="2c7ab-132">Response</span></span>
<span data-ttu-id="2c7ab-p105">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="2c7ab-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2c7ab-135">示例</span><span class="sxs-lookup"><span data-stu-id="2c7ab-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2c7ab-136">请求</span><span class="sxs-lookup"><span data-stu-id="2c7ab-136">Request</span></span>
<span data-ttu-id="2c7ab-137">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="2c7ab-137">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="2c7ab-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="2c7ab-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_educationsubmissionresource"
}-->
```http
DELETE https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/submissions/850f51b7/resources/f2387c3b-ec39-4bf2-a399-d7242677f024
```
# <a name="c"></a>[<span data-ttu-id="2c7ab-139">C#</span><span class="sxs-lookup"><span data-stu-id="2c7ab-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-educationsubmissionresource-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2c7ab-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2c7ab-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-educationsubmissionresource-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2c7ab-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2c7ab-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-educationsubmissionresource-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="2c7ab-142">Java</span><span class="sxs-lookup"><span data-stu-id="2c7ab-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-educationsubmissionresource-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="2c7ab-143">响应</span><span class="sxs-lookup"><span data-stu-id="2c7ab-143">Response</span></span>
<span data-ttu-id="2c7ab-144">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="2c7ab-144">The following is an example of the response.</span></span> 

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
  "description": "Delete educationSubmissionResource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


