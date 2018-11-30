---
title: 'educationSubmission: unsubmit'
description: . 在提交过程中，所有资源将都复制从 submittedResources 到 workingResources 地址散列表元。 教师将看的分级工作资源列表。
ms.openlocfilehash: 610b5a69a06c29d2e2b9b1fa6eb501a56d59b076
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27042335"
---
# <a name="educationsubmission-unsubmit"></a><span data-ttu-id="5f2f9-105">educationSubmission: unsubmit</span><span class="sxs-lookup"><span data-stu-id="5f2f9-105">educationSubmission: unsubmit</span></span>

> <span data-ttu-id="5f2f9-106">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="5f2f9-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5f2f9-107">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="5f2f9-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="5f2f9-108">指示学生希望后没有打开从事的工作分配的提交操作。</span><span class="sxs-lookup"><span data-stu-id="5f2f9-108">An action that indicates that a student wants to work on the submission of the assignment after it was turned in.</span></span> <span data-ttu-id="5f2f9-109">仅可由学生执行此操作。</span><span class="sxs-lookup"><span data-stu-id="5f2f9-109">This action can only be taken by the student.</span></span> <span data-ttu-id="5f2f9-110">这将提交的状态从"提交"变为"工作"。</span><span class="sxs-lookup"><span data-stu-id="5f2f9-110">This will change the status of the submission from "submitted" to "working".</span></span> <span data-ttu-id="5f2f9-111">在提交过程中，所有资源将都复制从 submittedResources 到 workingResources 地址散列表元。</span><span class="sxs-lookup"><span data-stu-id="5f2f9-111">During the submit process, all the resources will be copied from submittedResources to the workingResources bucket.</span></span> <span data-ttu-id="5f2f9-112">教师将看的分级工作资源列表。</span><span class="sxs-lookup"><span data-stu-id="5f2f9-112">The teacher will be looking at the working resources list for grading.</span></span>

## <a name="permissions"></a><span data-ttu-id="5f2f9-113">权限</span><span class="sxs-lookup"><span data-stu-id="5f2f9-113">Permissions</span></span>
<span data-ttu-id="5f2f9-p104">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="5f2f9-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5f2f9-116">权限类型</span><span class="sxs-lookup"><span data-stu-id="5f2f9-116">Permission type</span></span>      | <span data-ttu-id="5f2f9-117">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="5f2f9-117">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5f2f9-118">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5f2f9-118">Delegated (work or school account)</span></span> |  <span data-ttu-id="5f2f9-119">EduAssignments.ReadWriteBasic EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5f2f9-119">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="5f2f9-120">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5f2f9-120">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="5f2f9-121">不支持。</span><span class="sxs-lookup"><span data-stu-id="5f2f9-121">Not supported.</span></span>  |
|<span data-ttu-id="5f2f9-122">应用程序</span><span class="sxs-lookup"><span data-stu-id="5f2f9-122">Application</span></span> | <span data-ttu-id="5f2f9-123">不支持。</span><span class="sxs-lookup"><span data-stu-id="5f2f9-123">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="5f2f9-124">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5f2f9-124">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/{id}/assignments/{id}/submissions/{id}/unsubmit

```
## <a name="request-headers"></a><span data-ttu-id="5f2f9-125">请求标头</span><span class="sxs-lookup"><span data-stu-id="5f2f9-125">Request headers</span></span>
| <span data-ttu-id="5f2f9-126">标头</span><span class="sxs-lookup"><span data-stu-id="5f2f9-126">Header</span></span>       | <span data-ttu-id="5f2f9-127">值</span><span class="sxs-lookup"><span data-stu-id="5f2f9-127">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="5f2f9-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="5f2f9-128">Authorization</span></span>  | <span data-ttu-id="5f2f9-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="5f2f9-p105">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="5f2f9-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="5f2f9-131">Request body</span></span>
<span data-ttu-id="5f2f9-132">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="5f2f9-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5f2f9-133">响应</span><span class="sxs-lookup"><span data-stu-id="5f2f9-133">Response</span></span>
<span data-ttu-id="5f2f9-p106">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="5f2f9-p106">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5f2f9-136">示例</span><span class="sxs-lookup"><span data-stu-id="5f2f9-136">Example</span></span>
<span data-ttu-id="5f2f9-137">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="5f2f9-137">The following example shows how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="5f2f9-138">请求</span><span class="sxs-lookup"><span data-stu-id="5f2f9-138">Request</span></span>
<span data-ttu-id="5f2f9-139">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="5f2f9-139">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "educationsubmission_unsubmit"
}-->
```http
POST https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/submissions/850f51b7/unsubmit
```

##### <a name="response"></a><span data-ttu-id="5f2f9-140">响应</span><span class="sxs-lookup"><span data-stu-id="5f2f9-140">Response</span></span>
<span data-ttu-id="5f2f9-141">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="5f2f9-141">The following is an example of the response.</span></span>

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
  "description": "educationSubmission: unsubmit",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
