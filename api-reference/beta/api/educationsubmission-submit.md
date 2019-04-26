---
title: 'educationSubmission: 提交'
description: 指示学生完成工作并准备好在工作分配中进行准备的操作。 仅学生可以执行此操作。
author: dipakboyed
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: fd340c126c1a2b05bf71e2d91727ad3d9eee375c
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33324705"
---
# <a name="educationsubmission-submit"></a><span data-ttu-id="1b6bb-104">educationSubmission: 提交</span><span class="sxs-lookup"><span data-stu-id="1b6bb-104">educationSubmission: submit</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1b6bb-105">指示学生完成工作并准备好在工作分配中进行准备的操作。</span><span class="sxs-lookup"><span data-stu-id="1b6bb-105">An action that indicates that a student is done with the work and is ready to hand in the assignment.</span></span> <span data-ttu-id="1b6bb-106">仅学生可以执行此操作。</span><span class="sxs-lookup"><span data-stu-id="1b6bb-106">This action can only be taken by the student.</span></span> <span data-ttu-id="1b6bb-107">这会将提交状态从 "正在运行" 更改为 "已提交"。</span><span class="sxs-lookup"><span data-stu-id="1b6bb-107">This will change the status of the submission from "working" to "submitted".</span></span> <span data-ttu-id="1b6bb-108">在提交过程中, 所有资源都将复制到 submittedResources 存储桶中。</span><span class="sxs-lookup"><span data-stu-id="1b6bb-108">During the submit process, all the resources will be copied to the submittedResources bucket.</span></span> <span data-ttu-id="1b6bb-109">教师将在 "已提交的资源" 列表中查找评分。</span><span class="sxs-lookup"><span data-stu-id="1b6bb-109">The teacher will be looking at the submitted resources list for grading.</span></span>

## <a name="permissions"></a><span data-ttu-id="1b6bb-110">权限</span><span class="sxs-lookup"><span data-stu-id="1b6bb-110">Permissions</span></span>
<span data-ttu-id="1b6bb-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="1b6bb-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1b6bb-113">权限类型</span><span class="sxs-lookup"><span data-stu-id="1b6bb-113">Permission type</span></span>      | <span data-ttu-id="1b6bb-114">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="1b6bb-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1b6bb-115">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1b6bb-115">Delegated (work or school account)</span></span> |  <span data-ttu-id="1b6bb-116">EduAssignments、ReadWriteBasic、EduAssignments</span><span class="sxs-lookup"><span data-stu-id="1b6bb-116">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="1b6bb-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1b6bb-117">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="1b6bb-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="1b6bb-118">Not supported.</span></span>  |
|<span data-ttu-id="1b6bb-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="1b6bb-119">Application</span></span> | <span data-ttu-id="1b6bb-120">不支持。</span><span class="sxs-lookup"><span data-stu-id="1b6bb-120">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="1b6bb-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1b6bb-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/{id}/assignments/{id}/submissions/{id}/submit

```
## <a name="request-headers"></a><span data-ttu-id="1b6bb-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="1b6bb-122">Request headers</span></span>
| <span data-ttu-id="1b6bb-123">标头</span><span class="sxs-lookup"><span data-stu-id="1b6bb-123">Header</span></span>       | <span data-ttu-id="1b6bb-124">值</span><span class="sxs-lookup"><span data-stu-id="1b6bb-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="1b6bb-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="1b6bb-125">Authorization</span></span>  | <span data-ttu-id="1b6bb-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="1b6bb-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="1b6bb-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="1b6bb-128">Request body</span></span>
<span data-ttu-id="1b6bb-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="1b6bb-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1b6bb-130">响应</span><span class="sxs-lookup"><span data-stu-id="1b6bb-130">Response</span></span>
<span data-ttu-id="1b6bb-p105">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="1b6bb-p105">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1b6bb-133">示例</span><span class="sxs-lookup"><span data-stu-id="1b6bb-133">Example</span></span>
<span data-ttu-id="1b6bb-134">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="1b6bb-134">The following example shows how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="1b6bb-135">请求</span><span class="sxs-lookup"><span data-stu-id="1b6bb-135">Request</span></span>
<span data-ttu-id="1b6bb-136">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="1b6bb-136">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "educationsubmission_submit"
}-->
```http
POST https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/submissions/850f51b7/submit
```

##### <a name="response"></a><span data-ttu-id="1b6bb-137">响应</span><span class="sxs-lookup"><span data-stu-id="1b6bb-137">Response</span></span>
<span data-ttu-id="1b6bb-138">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="1b6bb-138">The following is an example of the response.</span></span>

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
  "suppressions": []
}
-->
