---
title: educationSubmission： 发行版
description: " 指示完成分级。 此操作仅可通过教师。"
author: dipakboyed
localization_priority: Normal
ms.openlocfilehash: a2723684f734a9e31dc08fb97d1e184400cac387
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27859008"
---
# <a name="educationsubmission-release"></a><span data-ttu-id="6e01e-104">educationSubmission： 发行版</span><span class="sxs-lookup"><span data-stu-id="6e01e-104">educationSubmission: release</span></span>

> <span data-ttu-id="6e01e-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="6e01e-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6e01e-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="6e01e-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="6e01e-107">此操作会使薪等级和学生向此提交操作相关联的反馈。</span><span class="sxs-lookup"><span data-stu-id="6e01e-107">This action makes the grade and feedback associated with this submission available to the student.</span></span> <span data-ttu-id="6e01e-108">这将提交的状态从"提交"变为"发布"，并指示完成分级。</span><span class="sxs-lookup"><span data-stu-id="6e01e-108">This will change the status of the submission from "submitted" to "released" and indicates that grading is done.</span></span> <span data-ttu-id="6e01e-109">此操作仅可通过教师。</span><span class="sxs-lookup"><span data-stu-id="6e01e-109">This action can only be done by the teacher.</span></span>

## <a name="permissions"></a><span data-ttu-id="6e01e-110">权限</span><span class="sxs-lookup"><span data-stu-id="6e01e-110">Permissions</span></span>
<span data-ttu-id="6e01e-p104">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6e01e-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6e01e-113">权限类型</span><span class="sxs-lookup"><span data-stu-id="6e01e-113">Permission type</span></span>      | <span data-ttu-id="6e01e-114">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="6e01e-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6e01e-115">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6e01e-115">Delegated (work or school account)</span></span> |  <span data-ttu-id="6e01e-116">EduAssignments.ReadWriteBasic EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6e01e-116">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>   |
|<span data-ttu-id="6e01e-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6e01e-117">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="6e01e-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="6e01e-118">Not supported.</span></span>  |
|<span data-ttu-id="6e01e-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="6e01e-119">Application</span></span> | <span data-ttu-id="6e01e-120">不支持。</span><span class="sxs-lookup"><span data-stu-id="6e01e-120">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="6e01e-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6e01e-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/{id}/assignments/{id}/submissions/{id}/release

```
## <a name="request-headers"></a><span data-ttu-id="6e01e-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="6e01e-122">Request headers</span></span>
| <span data-ttu-id="6e01e-123">标头</span><span class="sxs-lookup"><span data-stu-id="6e01e-123">Header</span></span>       | <span data-ttu-id="6e01e-124">值</span><span class="sxs-lookup"><span data-stu-id="6e01e-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="6e01e-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="6e01e-125">Authorization</span></span>  | <span data-ttu-id="6e01e-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="6e01e-p105">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="6e01e-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="6e01e-128">Request body</span></span>
<span data-ttu-id="6e01e-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="6e01e-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6e01e-130">响应</span><span class="sxs-lookup"><span data-stu-id="6e01e-130">Response</span></span>
<span data-ttu-id="6e01e-p106">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="6e01e-p106">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6e01e-133">示例</span><span class="sxs-lookup"><span data-stu-id="6e01e-133">Example</span></span>
<span data-ttu-id="6e01e-134">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="6e01e-134">The following example shows how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="6e01e-135">请求</span><span class="sxs-lookup"><span data-stu-id="6e01e-135">Request</span></span>
<span data-ttu-id="6e01e-136">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="6e01e-136">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "educationsubmission_release"
}-->

```http
POST https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/submissions/850f51b7/release
```

##### <a name="response"></a><span data-ttu-id="6e01e-137">响应</span><span class="sxs-lookup"><span data-stu-id="6e01e-137">Response</span></span>
<span data-ttu-id="6e01e-138">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="6e01e-138">The following is an example of the response.</span></span>

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
