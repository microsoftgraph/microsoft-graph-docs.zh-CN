---
title: educationSubmission：未提交
description: 指示学生想要在作业提交后处理作业提交。
author: sharad-sharma-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 152d042656f106a84fb4a89ecf8704938c251a04
ms.sourcegitcommit: f77c1385306fd40557aceb24fdfe4832cbb60a27
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/12/2021
ms.locfileid: "52912261"
---
# <a name="educationsubmission-unsubmit"></a><span data-ttu-id="60fde-103">educationSubmission：未提交</span><span class="sxs-lookup"><span data-stu-id="60fde-103">educationSubmission: unsubmit</span></span>

<span data-ttu-id="60fde-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="60fde-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="60fde-105">指示学生想要在作业提交后处理作业提交。</span><span class="sxs-lookup"><span data-stu-id="60fde-105">Indicate that a student wants to work on the submission of the assignment after it was turned in.</span></span> 

<span data-ttu-id="60fde-106">此操作仅能由学生执行。</span><span class="sxs-lookup"><span data-stu-id="60fde-106">This action can only be taken by the student.</span></span> <span data-ttu-id="60fde-107">这会将提交状态从"已提交"更改为"正在工作"。</span><span class="sxs-lookup"><span data-stu-id="60fde-107">This will change the status of the submission from "submitted" to "working".</span></span> <span data-ttu-id="60fde-108">在提交过程中，所有资源都将从 submittedResources 复制到 workingResources 存储桶。</span><span class="sxs-lookup"><span data-stu-id="60fde-108">During the submit process, all the resources will be copied from submittedResources to the workingResources bucket.</span></span> <span data-ttu-id="60fde-109">教师将查看工作资源列表进行评分。</span><span class="sxs-lookup"><span data-stu-id="60fde-109">The teacher will be looking at the working resources list for grading.</span></span>

## <a name="permissions"></a><span data-ttu-id="60fde-110">权限</span><span class="sxs-lookup"><span data-stu-id="60fde-110">Permissions</span></span>
<span data-ttu-id="60fde-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="60fde-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="60fde-113">权限类型</span><span class="sxs-lookup"><span data-stu-id="60fde-113">Permission type</span></span>      | <span data-ttu-id="60fde-114">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="60fde-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="60fde-115">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="60fde-115">Delegated (work or school account)</span></span> |  <span data-ttu-id="60fde-116">EduAssignments.ReadWriteBasic、EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="60fde-116">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="60fde-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="60fde-117">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="60fde-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="60fde-118">Not supported.</span></span>  |
|<span data-ttu-id="60fde-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="60fde-119">Application</span></span> | <span data-ttu-id="60fde-120">不支持。</span><span class="sxs-lookup"><span data-stu-id="60fde-120">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="60fde-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="60fde-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/acdefc6b-2dc6-4e71-b1e9-6d9810ab1793/assignments/cf6005fc-9e13-44a2-a6ac-a53322006454/submissions/d1bee293-d8bb-48d4-af3e-c8cb0e3c7fe7/unsubmit

```
## <a name="request-headers"></a><span data-ttu-id="60fde-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="60fde-122">Request headers</span></span>
| <span data-ttu-id="60fde-123">标头</span><span class="sxs-lookup"><span data-stu-id="60fde-123">Header</span></span>       | <span data-ttu-id="60fde-124">值</span><span class="sxs-lookup"><span data-stu-id="60fde-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="60fde-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="60fde-125">Authorization</span></span>  | <span data-ttu-id="60fde-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="60fde-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="60fde-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="60fde-128">Request body</span></span>
<span data-ttu-id="60fde-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="60fde-129">Don't supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="60fde-130">响应</span><span class="sxs-lookup"><span data-stu-id="60fde-130">Response</span></span>
<span data-ttu-id="60fde-p104">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="60fde-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="60fde-133">示例</span><span class="sxs-lookup"><span data-stu-id="60fde-133">Example</span></span>
<span data-ttu-id="60fde-134">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="60fde-134">The following example shows how to call this API.</span></span>
### <a name="request"></a><span data-ttu-id="60fde-135">请求</span><span class="sxs-lookup"><span data-stu-id="60fde-135">Request</span></span>
<span data-ttu-id="60fde-136">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="60fde-136">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "educationsubmission_unsubmit"
}-->
```http
POST https://graph.microsoft.com/v1.0/education/classes/acdefc6b-2dc6-4e71-b1e9-6d9810ab1793/assignments/ad8afb28-c138-4ad7-b7f5-a6986c2655a8/submissions/fbe51c90-78b7-418a-b5f3-871bf8d8d21e/unsubmit
```

### <a name="response"></a><span data-ttu-id="60fde-137">响应</span><span class="sxs-lookup"><span data-stu-id="60fde-137">Response</span></span>
<span data-ttu-id="60fde-138">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="60fde-138">The following is an example of the response.</span></span>

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
  "description": "educationSubmission: unsubmit",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


