---
title: educationSubmission： 提交
description: 指示学生完成的工作，并且已准备好分配中分发操作。 仅可由学生执行此操作。
author: dipakboyed
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: d1fd41c66e3f54898f6086a9bf14a0b53763df88
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27915807"
---
# <a name="educationsubmission-submit"></a><span data-ttu-id="b98ff-104">educationSubmission： 提交</span><span class="sxs-lookup"><span data-stu-id="b98ff-104">educationSubmission: submit</span></span>

> <span data-ttu-id="b98ff-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="b98ff-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b98ff-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="b98ff-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="b98ff-107">指示学生完成的工作，并且已准备好分配中分发操作。</span><span class="sxs-lookup"><span data-stu-id="b98ff-107">An action that indicates that a student is done with the work and is ready to hand in the assignment.</span></span> <span data-ttu-id="b98ff-108">仅可由学生执行此操作。</span><span class="sxs-lookup"><span data-stu-id="b98ff-108">This action can only be taken by the student.</span></span> <span data-ttu-id="b98ff-109">这将更改从"工作"到"提交"提交的状态。</span><span class="sxs-lookup"><span data-stu-id="b98ff-109">This will change the status of the submission from "working" to "submitted".</span></span> <span data-ttu-id="b98ff-110">在提交过程中，所有资源将都复制到 submittedResources 地址散列表元中。</span><span class="sxs-lookup"><span data-stu-id="b98ff-110">During the submit process, all the resources will be copied to the submittedResources bucket.</span></span> <span data-ttu-id="b98ff-111">教师将看评分的提交的资源列表。</span><span class="sxs-lookup"><span data-stu-id="b98ff-111">The teacher will be looking at the submitted resources list for grading.</span></span>

## <a name="permissions"></a><span data-ttu-id="b98ff-112">权限</span><span class="sxs-lookup"><span data-stu-id="b98ff-112">Permissions</span></span>
<span data-ttu-id="b98ff-p104">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b98ff-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b98ff-115">权限类型</span><span class="sxs-lookup"><span data-stu-id="b98ff-115">Permission type</span></span>      | <span data-ttu-id="b98ff-116">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b98ff-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b98ff-117">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b98ff-117">Delegated (work or school account)</span></span> |  <span data-ttu-id="b98ff-118">EduAssignments.ReadWriteBasic EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b98ff-118">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="b98ff-119">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b98ff-119">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="b98ff-120">不支持。</span><span class="sxs-lookup"><span data-stu-id="b98ff-120">Not supported.</span></span>  |
|<span data-ttu-id="b98ff-121">应用程序</span><span class="sxs-lookup"><span data-stu-id="b98ff-121">Application</span></span> | <span data-ttu-id="b98ff-122">不支持。</span><span class="sxs-lookup"><span data-stu-id="b98ff-122">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="b98ff-123">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b98ff-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/{id}/assignments/{id}/submissions/{id}/submit

```
## <a name="request-headers"></a><span data-ttu-id="b98ff-124">请求标头</span><span class="sxs-lookup"><span data-stu-id="b98ff-124">Request headers</span></span>
| <span data-ttu-id="b98ff-125">标头</span><span class="sxs-lookup"><span data-stu-id="b98ff-125">Header</span></span>       | <span data-ttu-id="b98ff-126">值</span><span class="sxs-lookup"><span data-stu-id="b98ff-126">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="b98ff-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="b98ff-127">Authorization</span></span>  | <span data-ttu-id="b98ff-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="b98ff-p105">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="b98ff-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="b98ff-130">Request body</span></span>
<span data-ttu-id="b98ff-131">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="b98ff-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b98ff-132">响应</span><span class="sxs-lookup"><span data-stu-id="b98ff-132">Response</span></span>
<span data-ttu-id="b98ff-p106">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="b98ff-p106">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b98ff-135">示例</span><span class="sxs-lookup"><span data-stu-id="b98ff-135">Example</span></span>
<span data-ttu-id="b98ff-136">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="b98ff-136">The following example shows how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="b98ff-137">请求</span><span class="sxs-lookup"><span data-stu-id="b98ff-137">Request</span></span>
<span data-ttu-id="b98ff-138">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="b98ff-138">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "educationsubmission_submit"
}-->
```http
POST https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/submissions/850f51b7/submit
```

##### <a name="response"></a><span data-ttu-id="b98ff-139">响应</span><span class="sxs-lookup"><span data-stu-id="b98ff-139">Response</span></span>
<span data-ttu-id="b98ff-140">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="b98ff-140">The following is an example of the response.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "educationSubmission: submit",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
