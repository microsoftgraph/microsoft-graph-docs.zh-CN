---
title: educationSubmission： submit
description: 指示学生已完成工作并准备好处理作业的操作。 此操作仅能由学生执行。
author: sharad-sharma-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 1c455b022fef11b82935471a3eb90fd2b253bbd7
ms.sourcegitcommit: f77c1385306fd40557aceb24fdfe4832cbb60a27
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/12/2021
ms.locfileid: "52912344"
---
# <a name="educationsubmission-submit"></a><span data-ttu-id="3fbe1-104">educationSubmission： submit</span><span class="sxs-lookup"><span data-stu-id="3fbe1-104">educationSubmission: submit</span></span>

<span data-ttu-id="3fbe1-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3fbe1-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="3fbe1-106">指示学生已完成工作并准备好处理作业。</span><span class="sxs-lookup"><span data-stu-id="3fbe1-106">Indicate that a student is done with the work and is ready to hand in the assignment.</span></span> 

<span data-ttu-id="3fbe1-107">此操作仅能由学生执行。</span><span class="sxs-lookup"><span data-stu-id="3fbe1-107">This action can only be taken by the student.</span></span> <span data-ttu-id="3fbe1-108">这会将提交状态从"正在工作"更改为"已提交"。</span><span class="sxs-lookup"><span data-stu-id="3fbe1-108">This will change the status of the submission from "working" to "submitted".</span></span> <span data-ttu-id="3fbe1-109">在提交过程中，所有资源都将复制到 **submittedResources** 存储桶。</span><span class="sxs-lookup"><span data-stu-id="3fbe1-109">During the submit process, all the resources will be copied to the **submittedResources** bucket.</span></span> <span data-ttu-id="3fbe1-110">教师将查看提交的资源列表进行评分。</span><span class="sxs-lookup"><span data-stu-id="3fbe1-110">The teacher will be looking at the submitted resources list for grading.</span></span>

## <a name="permissions"></a><span data-ttu-id="3fbe1-111">权限</span><span class="sxs-lookup"><span data-stu-id="3fbe1-111">Permissions</span></span>
<span data-ttu-id="3fbe1-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="3fbe1-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3fbe1-114">权限类型</span><span class="sxs-lookup"><span data-stu-id="3fbe1-114">Permission type</span></span>      | <span data-ttu-id="3fbe1-115">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="3fbe1-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3fbe1-116">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3fbe1-116">Delegated (work or school account)</span></span> |  <span data-ttu-id="3fbe1-117">EduAssignments.ReadWriteBasic、EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3fbe1-117">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="3fbe1-118">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3fbe1-118">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="3fbe1-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="3fbe1-119">Not supported.</span></span>  |
|<span data-ttu-id="3fbe1-120">应用程序</span><span class="sxs-lookup"><span data-stu-id="3fbe1-120">Application</span></span> | <span data-ttu-id="3fbe1-121">不支持。</span><span class="sxs-lookup"><span data-stu-id="3fbe1-121">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="3fbe1-122">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3fbe1-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/acdefc6b-2dc6-4e71-b1e9-6d9810ab1793/assignments/cf6005fc-9e13-44a2-a6ac-a53322006454/submissions/d1bee293-d8bb-48d4-af3e-c8cb0e3c7fe7/submit
```

## <a name="request-headers"></a><span data-ttu-id="3fbe1-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="3fbe1-123">Request headers</span></span>
| <span data-ttu-id="3fbe1-124">标头</span><span class="sxs-lookup"><span data-stu-id="3fbe1-124">Header</span></span>       | <span data-ttu-id="3fbe1-125">值</span><span class="sxs-lookup"><span data-stu-id="3fbe1-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="3fbe1-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="3fbe1-126">Authorization</span></span>  | <span data-ttu-id="3fbe1-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="3fbe1-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="3fbe1-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="3fbe1-129">Request body</span></span>
<span data-ttu-id="3fbe1-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="3fbe1-130">Don't supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3fbe1-131">响应</span><span class="sxs-lookup"><span data-stu-id="3fbe1-131">Response</span></span>
<span data-ttu-id="3fbe1-p105">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="3fbe1-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3fbe1-134">示例</span><span class="sxs-lookup"><span data-stu-id="3fbe1-134">Example</span></span>
<span data-ttu-id="3fbe1-135">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="3fbe1-135">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="3fbe1-136">请求</span><span class="sxs-lookup"><span data-stu-id="3fbe1-136">Request</span></span>
<span data-ttu-id="3fbe1-137">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="3fbe1-137">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "educationsubmission_submit"
}-->
```http
POST https://graph.microsoft.com/v1.0/education/classes/acdefc6b-2dc6-4e71-b1e9-6d9810ab1793/assignments/ad8afb28-c138-4ad7-b7f5-a6986c2655a8/submissions/fbe51c90-78b7-418a-b5f3-871bf8d8d21e/submit
```

### <a name="response"></a><span data-ttu-id="3fbe1-138">响应</span><span class="sxs-lookup"><span data-stu-id="3fbe1-138">Response</span></span>
<span data-ttu-id="3fbe1-139">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="3fbe1-139">The following is an example of the response.</span></span>

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


