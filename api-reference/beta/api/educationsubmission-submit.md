---
title: educationSubmission：提交
description: 指示学生完成工作并准备好在工作分配中进行准备的操作。 仅学生可以执行此操作。
author: dipakboyed
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 948793527423a93f05bf890708651fd9e60bca56
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48007264"
---
# <a name="educationsubmission-submit"></a><span data-ttu-id="91f82-104">educationSubmission：提交</span><span class="sxs-lookup"><span data-stu-id="91f82-104">educationSubmission: submit</span></span>

<span data-ttu-id="91f82-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="91f82-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="91f82-106">指示学生完成工作并准备好在工作分配中进行准备的操作。</span><span class="sxs-lookup"><span data-stu-id="91f82-106">An action that indicates that a student is done with the work and is ready to hand in the assignment.</span></span> <span data-ttu-id="91f82-107">仅学生可以执行此操作。</span><span class="sxs-lookup"><span data-stu-id="91f82-107">This action can only be taken by the student.</span></span> <span data-ttu-id="91f82-108">这会将提交状态从 "正在运行" 更改为 "已提交"。</span><span class="sxs-lookup"><span data-stu-id="91f82-108">This will change the status of the submission from "working" to "submitted".</span></span> <span data-ttu-id="91f82-109">在提交过程中，所有资源都将复制到 submittedResources 存储桶中。</span><span class="sxs-lookup"><span data-stu-id="91f82-109">During the submit process, all the resources will be copied to the submittedResources bucket.</span></span> <span data-ttu-id="91f82-110">教师将在 "已提交的资源" 列表中查找评分。</span><span class="sxs-lookup"><span data-stu-id="91f82-110">The teacher will be looking at the submitted resources list for grading.</span></span>

## <a name="permissions"></a><span data-ttu-id="91f82-111">权限</span><span class="sxs-lookup"><span data-stu-id="91f82-111">Permissions</span></span>
<span data-ttu-id="91f82-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="91f82-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="91f82-114">权限类型</span><span class="sxs-lookup"><span data-stu-id="91f82-114">Permission type</span></span>      | <span data-ttu-id="91f82-115">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="91f82-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="91f82-116">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="91f82-116">Delegated (work or school account)</span></span> |  <span data-ttu-id="91f82-117">EduAssignments、ReadWriteBasic、EduAssignments</span><span class="sxs-lookup"><span data-stu-id="91f82-117">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="91f82-118">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="91f82-118">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="91f82-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="91f82-119">Not supported.</span></span>  |
|<span data-ttu-id="91f82-120">应用程序</span><span class="sxs-lookup"><span data-stu-id="91f82-120">Application</span></span> | <span data-ttu-id="91f82-121">不支持。</span><span class="sxs-lookup"><span data-stu-id="91f82-121">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="91f82-122">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="91f82-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/{id}/assignments/{id}/submissions/{id}/submit

```
## <a name="request-headers"></a><span data-ttu-id="91f82-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="91f82-123">Request headers</span></span>
| <span data-ttu-id="91f82-124">标头</span><span class="sxs-lookup"><span data-stu-id="91f82-124">Header</span></span>       | <span data-ttu-id="91f82-125">值</span><span class="sxs-lookup"><span data-stu-id="91f82-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="91f82-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="91f82-126">Authorization</span></span>  | <span data-ttu-id="91f82-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="91f82-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="91f82-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="91f82-129">Request body</span></span>
<span data-ttu-id="91f82-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="91f82-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="91f82-131">响应</span><span class="sxs-lookup"><span data-stu-id="91f82-131">Response</span></span>
<span data-ttu-id="91f82-p105">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="91f82-p105">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="91f82-134">示例</span><span class="sxs-lookup"><span data-stu-id="91f82-134">Example</span></span>
<span data-ttu-id="91f82-135">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="91f82-135">The following example shows how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="91f82-136">请求</span><span class="sxs-lookup"><span data-stu-id="91f82-136">Request</span></span>
<span data-ttu-id="91f82-137">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="91f82-137">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="91f82-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="91f82-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "educationsubmission_submit"
}-->
```http
POST https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/submissions/850f51b7/submit
```
# <a name="c"></a>[<span data-ttu-id="91f82-139">C#</span><span class="sxs-lookup"><span data-stu-id="91f82-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/educationsubmission-submit-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="91f82-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="91f82-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/educationsubmission-submit-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="91f82-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="91f82-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/educationsubmission-submit-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="91f82-142">响应</span><span class="sxs-lookup"><span data-stu-id="91f82-142">Response</span></span>
<span data-ttu-id="91f82-143">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="91f82-143">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationAssignment"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "educationSubmission: submit",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


