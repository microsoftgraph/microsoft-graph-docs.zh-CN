---
title: educationSubmission： return
description: 向学生提供与此提交相关的成绩和反馈。
author: sharad-sharma-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: f7c33c7bd744984ab26efb8d922716b5bb85a654
ms.sourcegitcommit: f77c1385306fd40557aceb24fdfe4832cbb60a27
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/12/2021
ms.locfileid: "52912271"
---
# <a name="educationsubmission-return"></a><span data-ttu-id="36fe2-103">educationSubmission： return</span><span class="sxs-lookup"><span data-stu-id="36fe2-103">educationSubmission: return</span></span>

<span data-ttu-id="36fe2-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="36fe2-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="36fe2-105">向学生提供与此提交相关的成绩和反馈。</span><span class="sxs-lookup"><span data-stu-id="36fe2-105">Make the grade and feedback associated with this submission available to the student.</span></span> 

<span data-ttu-id="36fe2-106">此操作将提交状态从"已提交"更改为"已返回"，并指示提供了反馈或评分已完成。</span><span class="sxs-lookup"><span data-stu-id="36fe2-106">This action changes the status of the submission from "submitted" to "returned" and indicates that feedback is provided or grading is done.</span></span> <span data-ttu-id="36fe2-107">此操作仅能由教师执行。</span><span class="sxs-lookup"><span data-stu-id="36fe2-107">This action can only be done by the teacher.</span></span>

## <a name="permissions"></a><span data-ttu-id="36fe2-108">权限</span><span class="sxs-lookup"><span data-stu-id="36fe2-108">Permissions</span></span>
<span data-ttu-id="36fe2-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="36fe2-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="36fe2-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="36fe2-111">Permission type</span></span>      | <span data-ttu-id="36fe2-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="36fe2-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="36fe2-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="36fe2-113">Delegated (work or school account)</span></span> |  <span data-ttu-id="36fe2-114">EduAssignments.ReadWriteBasic、EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="36fe2-114">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>   |
|<span data-ttu-id="36fe2-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="36fe2-115">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="36fe2-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="36fe2-116">Not supported.</span></span>  |
|<span data-ttu-id="36fe2-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="36fe2-117">Application</span></span> | <span data-ttu-id="36fe2-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="36fe2-118">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="36fe2-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="36fe2-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/acdefc6b-2dc6-4e71-b1e9-6d9810ab1793/assignments/cf6005fc-9e13-44a2-a6ac-a53322006454/submissions/d1bee293-d8bb-48d4-af3e-c8cb0e3c7fe7/return
```
## <a name="request-headers"></a><span data-ttu-id="36fe2-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="36fe2-120">Request headers</span></span>
| <span data-ttu-id="36fe2-121">标头</span><span class="sxs-lookup"><span data-stu-id="36fe2-121">Header</span></span>       | <span data-ttu-id="36fe2-122">值</span><span class="sxs-lookup"><span data-stu-id="36fe2-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="36fe2-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="36fe2-123">Authorization</span></span>  | <span data-ttu-id="36fe2-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="36fe2-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="36fe2-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="36fe2-126">Request body</span></span>
<span data-ttu-id="36fe2-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="36fe2-127">Don't supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="36fe2-128">响应</span><span class="sxs-lookup"><span data-stu-id="36fe2-128">Response</span></span>
<span data-ttu-id="36fe2-p104">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="36fe2-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="36fe2-131">示例</span><span class="sxs-lookup"><span data-stu-id="36fe2-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="36fe2-132">请求</span><span class="sxs-lookup"><span data-stu-id="36fe2-132">Request</span></span>
<span data-ttu-id="36fe2-133">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="36fe2-133">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "educationsubmission_return"
}-->

```http
POST https://graph.microsoft.com/v1.0/education/classes/acdefc6b-2dc6-4e71-b1e9-6d9810ab1793/assignments/ad8afb28-c138-4ad7-b7f5-a6986c2655a8/submissions/fbe51c90-78b7-418a-b5f3-871bf8d8d21e/return
```

### <a name="response"></a><span data-ttu-id="36fe2-134">响应</span><span class="sxs-lookup"><span data-stu-id="36fe2-134">Response</span></span>
<span data-ttu-id="36fe2-135">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="36fe2-135">The following is an example of the response.</span></span>

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
  "description": "educationSubmission: return",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


