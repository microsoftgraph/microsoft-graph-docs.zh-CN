---
title: educationSubmission： submit
description: 指示学生已完成工作并准备好处理作业的操作。 此操作仅能由学生执行。
author: sharad-sharma-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: d63392079ad66d715c735ab5d6ddd989336fa958
ms.sourcegitcommit: 979fe005c74eb99cd971df6b9511b2d3f7fe3cd4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/17/2021
ms.locfileid: "52993300"
---
# <a name="educationsubmission-submit"></a><span data-ttu-id="9ab9f-104">educationSubmission： submit</span><span class="sxs-lookup"><span data-stu-id="9ab9f-104">educationSubmission: submit</span></span>

<span data-ttu-id="9ab9f-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9ab9f-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="9ab9f-106">指示学生已完成工作并准备好处理作业。</span><span class="sxs-lookup"><span data-stu-id="9ab9f-106">Indicate that a student is done with the work and is ready to hand in the assignment.</span></span> 

<span data-ttu-id="9ab9f-107">此操作仅能由学生执行。</span><span class="sxs-lookup"><span data-stu-id="9ab9f-107">This action can only be taken by the student.</span></span> <span data-ttu-id="9ab9f-108">这会将提交状态从"正在工作"更改为"已提交"。</span><span class="sxs-lookup"><span data-stu-id="9ab9f-108">This will change the status of the submission from "working" to "submitted".</span></span> <span data-ttu-id="9ab9f-109">在提交过程中，所有资源都将复制到 **submittedResources** 存储桶。</span><span class="sxs-lookup"><span data-stu-id="9ab9f-109">During the submit process, all the resources will be copied to the **submittedResources** bucket.</span></span> <span data-ttu-id="9ab9f-110">教师将查看提交的资源列表进行评分。</span><span class="sxs-lookup"><span data-stu-id="9ab9f-110">The teacher will be looking at the submitted resources list for grading.</span></span>

## <a name="permissions"></a><span data-ttu-id="9ab9f-111">权限</span><span class="sxs-lookup"><span data-stu-id="9ab9f-111">Permissions</span></span>
<span data-ttu-id="9ab9f-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9ab9f-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9ab9f-114">权限类型</span><span class="sxs-lookup"><span data-stu-id="9ab9f-114">Permission type</span></span>      | <span data-ttu-id="9ab9f-115">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="9ab9f-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9ab9f-116">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9ab9f-116">Delegated (work or school account)</span></span> |  <span data-ttu-id="9ab9f-117">EduAssignments.ReadWriteBasic、EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9ab9f-117">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="9ab9f-118">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9ab9f-118">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="9ab9f-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="9ab9f-119">Not supported.</span></span>  |
|<span data-ttu-id="9ab9f-120">应用程序</span><span class="sxs-lookup"><span data-stu-id="9ab9f-120">Application</span></span> | <span data-ttu-id="9ab9f-121">不支持。</span><span class="sxs-lookup"><span data-stu-id="9ab9f-121">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="9ab9f-122">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9ab9f-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/acdefc6b-2dc6-4e71-b1e9-6d9810ab1793/assignments/cf6005fc-9e13-44a2-a6ac-a53322006454/submissions/d1bee293-d8bb-48d4-af3e-c8cb0e3c7fe7/submit
```

## <a name="request-headers"></a><span data-ttu-id="9ab9f-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="9ab9f-123">Request headers</span></span>
| <span data-ttu-id="9ab9f-124">标头</span><span class="sxs-lookup"><span data-stu-id="9ab9f-124">Header</span></span>       | <span data-ttu-id="9ab9f-125">值</span><span class="sxs-lookup"><span data-stu-id="9ab9f-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="9ab9f-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="9ab9f-126">Authorization</span></span>  | <span data-ttu-id="9ab9f-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="9ab9f-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="9ab9f-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="9ab9f-129">Request body</span></span>
<span data-ttu-id="9ab9f-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="9ab9f-130">Don't supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9ab9f-131">响应</span><span class="sxs-lookup"><span data-stu-id="9ab9f-131">Response</span></span>
<span data-ttu-id="9ab9f-p105">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="9ab9f-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9ab9f-134">示例</span><span class="sxs-lookup"><span data-stu-id="9ab9f-134">Example</span></span>
<span data-ttu-id="9ab9f-135">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="9ab9f-135">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="9ab9f-136">请求</span><span class="sxs-lookup"><span data-stu-id="9ab9f-136">Request</span></span>
<span data-ttu-id="9ab9f-137">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="9ab9f-137">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="9ab9f-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="9ab9f-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "educationsubmission_submit"
}-->
```http
POST https://graph.microsoft.com/v1.0/education/classes/acdefc6b-2dc6-4e71-b1e9-6d9810ab1793/assignments/ad8afb28-c138-4ad7-b7f5-a6986c2655a8/submissions/fbe51c90-78b7-418a-b5f3-871bf8d8d21e/submit
```
# <a name="c"></a>[<span data-ttu-id="9ab9f-139">C#</span><span class="sxs-lookup"><span data-stu-id="9ab9f-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/educationsubmission-submit-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9ab9f-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9ab9f-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/educationsubmission-submit-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9ab9f-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9ab9f-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/educationsubmission-submit-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="9ab9f-142">Java</span><span class="sxs-lookup"><span data-stu-id="9ab9f-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/educationsubmission-submit-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="9ab9f-143">响应</span><span class="sxs-lookup"><span data-stu-id="9ab9f-143">Response</span></span>
<span data-ttu-id="9ab9f-144">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="9ab9f-144">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationAssignment"
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
  "description": "educationSubmission: submit",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


