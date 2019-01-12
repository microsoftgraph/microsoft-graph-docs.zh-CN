---
title: educationSubmission： 发行版
description: " 指示完成分级。 此操作仅可通过教师。"
author: dipakboyed
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 99a9580df194c5dcfa7c28d3634d4d3eb72ec298
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27955553"
---
# <a name="educationsubmission-release"></a><span data-ttu-id="640fc-104">educationSubmission： 发行版</span><span class="sxs-lookup"><span data-stu-id="640fc-104">educationSubmission: release</span></span>

> <span data-ttu-id="640fc-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="640fc-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="640fc-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="640fc-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="640fc-107">此操作会使薪等级和学生向此提交操作相关联的反馈。</span><span class="sxs-lookup"><span data-stu-id="640fc-107">This action makes the grade and feedback associated with this submission available to the student.</span></span> <span data-ttu-id="640fc-108">这将提交的状态从"提交"变为"发布"，并指示完成分级。</span><span class="sxs-lookup"><span data-stu-id="640fc-108">This will change the status of the submission from "submitted" to "released" and indicates that grading is done.</span></span> <span data-ttu-id="640fc-109">此操作仅可通过教师。</span><span class="sxs-lookup"><span data-stu-id="640fc-109">This action can only be done by the teacher.</span></span>

## <a name="permissions"></a><span data-ttu-id="640fc-110">权限</span><span class="sxs-lookup"><span data-stu-id="640fc-110">Permissions</span></span>
<span data-ttu-id="640fc-p104">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="640fc-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="640fc-113">权限类型</span><span class="sxs-lookup"><span data-stu-id="640fc-113">Permission type</span></span>      | <span data-ttu-id="640fc-114">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="640fc-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="640fc-115">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="640fc-115">Delegated (work or school account)</span></span> |  <span data-ttu-id="640fc-116">EduAssignments.ReadWriteBasic EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="640fc-116">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>   |
|<span data-ttu-id="640fc-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="640fc-117">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="640fc-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="640fc-118">Not supported.</span></span>  |
|<span data-ttu-id="640fc-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="640fc-119">Application</span></span> | <span data-ttu-id="640fc-120">不支持。</span><span class="sxs-lookup"><span data-stu-id="640fc-120">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="640fc-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="640fc-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/{id}/assignments/{id}/submissions/{id}/release

```
## <a name="request-headers"></a><span data-ttu-id="640fc-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="640fc-122">Request headers</span></span>
| <span data-ttu-id="640fc-123">标头</span><span class="sxs-lookup"><span data-stu-id="640fc-123">Header</span></span>       | <span data-ttu-id="640fc-124">值</span><span class="sxs-lookup"><span data-stu-id="640fc-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="640fc-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="640fc-125">Authorization</span></span>  | <span data-ttu-id="640fc-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="640fc-p105">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="640fc-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="640fc-128">Request body</span></span>
<span data-ttu-id="640fc-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="640fc-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="640fc-130">响应</span><span class="sxs-lookup"><span data-stu-id="640fc-130">Response</span></span>
<span data-ttu-id="640fc-p106">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="640fc-p106">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="640fc-133">示例</span><span class="sxs-lookup"><span data-stu-id="640fc-133">Example</span></span>
<span data-ttu-id="640fc-134">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="640fc-134">The following example shows how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="640fc-135">请求</span><span class="sxs-lookup"><span data-stu-id="640fc-135">Request</span></span>
<span data-ttu-id="640fc-136">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="640fc-136">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "educationsubmission_release"
}-->

```http
POST https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/submissions/850f51b7/release
```

##### <a name="response"></a><span data-ttu-id="640fc-137">响应</span><span class="sxs-lookup"><span data-stu-id="640fc-137">Response</span></span>
<span data-ttu-id="640fc-138">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="640fc-138">The following is an example of the response.</span></span>

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
  "description": "educationSubmission: release",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
