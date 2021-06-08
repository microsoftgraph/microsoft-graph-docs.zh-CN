---
title: educationSubmission：未提交
description: '一种操作，指示学生想要在作业提交后进行作业提交。 此操作仅能由学生执行。 '
author: dipakboyed
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 23f6a2ec01dde64ec12ff8f3a378c40b1b3fd3cb
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/06/2021
ms.locfileid: "52787273"
---
# <a name="educationsubmission-unsubmit"></a><span data-ttu-id="98d44-104">educationSubmission：未提交</span><span class="sxs-lookup"><span data-stu-id="98d44-104">educationSubmission: unsubmit</span></span>

<span data-ttu-id="98d44-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="98d44-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="98d44-106">一种操作，指示学生想要在作业提交后进行作业提交。</span><span class="sxs-lookup"><span data-stu-id="98d44-106">An action that indicates that a student wants to work on the submission of the assignment after it was turned in.</span></span> <span data-ttu-id="98d44-107">此操作仅能由学生执行。</span><span class="sxs-lookup"><span data-stu-id="98d44-107">This action can only be taken by the student.</span></span> <span data-ttu-id="98d44-108">这会将提交状态从"已提交"更改为"正在工作"。</span><span class="sxs-lookup"><span data-stu-id="98d44-108">This will change the status of the submission from "submitted" to "working".</span></span> <span data-ttu-id="98d44-109">在提交过程中，所有资源都将从 submittedResources 复制到 workingResources 存储桶。</span><span class="sxs-lookup"><span data-stu-id="98d44-109">During the submit process, all the resources will be copied from submittedResources to the workingResources bucket.</span></span> <span data-ttu-id="98d44-110">教师将查看工作资源列表进行评分。</span><span class="sxs-lookup"><span data-stu-id="98d44-110">The teacher will be looking at the working resources list for grading.</span></span>

## <a name="permissions"></a><span data-ttu-id="98d44-111">权限</span><span class="sxs-lookup"><span data-stu-id="98d44-111">Permissions</span></span>
<span data-ttu-id="98d44-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="98d44-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="98d44-114">权限类型</span><span class="sxs-lookup"><span data-stu-id="98d44-114">Permission type</span></span>      | <span data-ttu-id="98d44-115">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="98d44-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="98d44-116">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="98d44-116">Delegated (work or school account)</span></span> |  <span data-ttu-id="98d44-117">EduAssignments.ReadWriteBasic、EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="98d44-117">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="98d44-118">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="98d44-118">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="98d44-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="98d44-119">Not supported.</span></span>  |
|<span data-ttu-id="98d44-120">应用程序</span><span class="sxs-lookup"><span data-stu-id="98d44-120">Application</span></span> | <span data-ttu-id="98d44-121">不支持。</span><span class="sxs-lookup"><span data-stu-id="98d44-121">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="98d44-122">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="98d44-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/{id}/assignments/{id}/submissions/{id}/unsubmit
```
## <a name="request-headers"></a><span data-ttu-id="98d44-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="98d44-123">Request headers</span></span>
| <span data-ttu-id="98d44-124">标头</span><span class="sxs-lookup"><span data-stu-id="98d44-124">Header</span></span>       | <span data-ttu-id="98d44-125">值</span><span class="sxs-lookup"><span data-stu-id="98d44-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="98d44-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="98d44-126">Authorization</span></span>  | <span data-ttu-id="98d44-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="98d44-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="98d44-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="98d44-129">Request body</span></span>
<span data-ttu-id="98d44-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="98d44-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="98d44-131">响应</span><span class="sxs-lookup"><span data-stu-id="98d44-131">Response</span></span>
<span data-ttu-id="98d44-p105">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="98d44-p105">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="98d44-134">示例</span><span class="sxs-lookup"><span data-stu-id="98d44-134">Example</span></span>
<span data-ttu-id="98d44-135">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="98d44-135">The following example shows how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="98d44-136">请求</span><span class="sxs-lookup"><span data-stu-id="98d44-136">Request</span></span>
<span data-ttu-id="98d44-137">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="98d44-137">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="98d44-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="98d44-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "educationsubmission_unsubmit"
}-->
```http
POST https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/submissions/850f51b7/unsubmit
```
# <a name="c"></a>[<span data-ttu-id="98d44-139">C#</span><span class="sxs-lookup"><span data-stu-id="98d44-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/educationsubmission-unsubmit-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="98d44-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="98d44-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/educationsubmission-unsubmit-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="98d44-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="98d44-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/educationsubmission-unsubmit-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="98d44-142">Java</span><span class="sxs-lookup"><span data-stu-id="98d44-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/educationsubmission-unsubmit-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="98d44-143">响应</span><span class="sxs-lookup"><span data-stu-id="98d44-143">Response</span></span>
<span data-ttu-id="98d44-144">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="98d44-144">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "educationSubmission: unsubmit",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


