---
title: 删除 educationSubmissionResource
description: 从提交中删除资源。 仅学生可以执行此操作。 如果资源是从分配中复制的, 则在删除当前副本后将创建该资源的新副本。
author: dipakboyed
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 74cb61fe4e486a8837542f24efeccab5de295e87
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/15/2019
ms.locfileid: "36416035"
---
# <a name="delete-educationsubmissionresource"></a><span data-ttu-id="36688-105">删除 educationSubmissionResource</span><span class="sxs-lookup"><span data-stu-id="36688-105">Delete educationSubmissionResource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="36688-106">从提交中删除资源。</span><span class="sxs-lookup"><span data-stu-id="36688-106">Deletes a resource from the submission.</span></span> <span data-ttu-id="36688-107">仅学生可以执行此操作。</span><span class="sxs-lookup"><span data-stu-id="36688-107">This can only be done by the student.</span></span> <span data-ttu-id="36688-108">如果资源是从分配中复制的, 则在删除当前副本后将创建该资源的新副本。</span><span class="sxs-lookup"><span data-stu-id="36688-108">If the resource was copied from the assignment, a new copy of the resource will be created after the current copy is deleted.</span></span> <span data-ttu-id="36688-109">这使您可以将资源 "重置" 为其原始状态。</span><span class="sxs-lookup"><span data-stu-id="36688-109">This allows you to "reset" the resource to its original state.</span></span> <span data-ttu-id="36688-110">如果资源不是从分配中复制的, 而是从学生添加的, 则只会删除该资源。</span><span class="sxs-lookup"><span data-stu-id="36688-110">If the resource was not copied from the assignment but was added from the student, the resource is simply deleted.</span></span>

## <a name="permissions"></a><span data-ttu-id="36688-111">权限</span><span class="sxs-lookup"><span data-stu-id="36688-111">Permissions</span></span>
<span data-ttu-id="36688-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="36688-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="36688-114">权限类型</span><span class="sxs-lookup"><span data-stu-id="36688-114">Permission type</span></span>      | <span data-ttu-id="36688-115">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="36688-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="36688-116">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="36688-116">Delegated (work or school account)</span></span> |  <span data-ttu-id="36688-117">EduAssignments、ReadWriteBasic、EduAssignments</span><span class="sxs-lookup"><span data-stu-id="36688-117">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="36688-118">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="36688-118">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="36688-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="36688-119">Not supported.</span></span>  |
|<span data-ttu-id="36688-120">应用程序</span><span class="sxs-lookup"><span data-stu-id="36688-120">Application</span></span> | <span data-ttu-id="36688-121">不支持。</span><span class="sxs-lookup"><span data-stu-id="36688-121">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="36688-122">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="36688-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /educationClasses/assignments/{id}/submissions/{id}/resources/{id}

```
## <a name="request-headers"></a><span data-ttu-id="36688-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="36688-123">Request headers</span></span>
| <span data-ttu-id="36688-124">标头</span><span class="sxs-lookup"><span data-stu-id="36688-124">Header</span></span>       | <span data-ttu-id="36688-125">值</span><span class="sxs-lookup"><span data-stu-id="36688-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="36688-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="36688-126">Authorization</span></span>  | <span data-ttu-id="36688-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="36688-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="36688-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="36688-129">Request body</span></span>
<span data-ttu-id="36688-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="36688-130">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="36688-131">响应</span><span class="sxs-lookup"><span data-stu-id="36688-131">Response</span></span>
<span data-ttu-id="36688-p105">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="36688-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="36688-134">示例</span><span class="sxs-lookup"><span data-stu-id="36688-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="36688-135">请求</span><span class="sxs-lookup"><span data-stu-id="36688-135">Request</span></span>
<span data-ttu-id="36688-136">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="36688-136">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="36688-137">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="36688-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_educationsubmissionresource"
}-->
```http
DELETE https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/submissions/850f51b7/resources/f2387c3b-ec39-4bf2-a399-d7242677f024
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="36688-138">C#</span><span class="sxs-lookup"><span data-stu-id="36688-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-educationsubmissionresource-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="36688-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="36688-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-educationsubmissionresource-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="36688-140">目标-C</span><span class="sxs-lookup"><span data-stu-id="36688-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-educationsubmissionresource-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="36688-141">响应</span><span class="sxs-lookup"><span data-stu-id="36688-141">Response</span></span>
<span data-ttu-id="36688-142">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="36688-142">The following is an example of the response.</span></span> 

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
