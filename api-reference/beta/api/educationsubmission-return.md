---
title: educationSubmission： 返回
description: 此操作会使薪等级和学生向此提交操作相关联的反馈。
author: dipakboyed
ms.openlocfilehash: d73300328168baf9481b329b36f056aa27044b2e
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27350874"
---
# <a name="educationsubmission-return"></a><span data-ttu-id="8e376-103">educationSubmission： 返回</span><span class="sxs-lookup"><span data-stu-id="8e376-103">educationSubmission: return</span></span>

> <span data-ttu-id="8e376-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="8e376-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8e376-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="8e376-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="8e376-106">此操作会使薪等级和学生向此提交操作相关联的反馈。</span><span class="sxs-lookup"><span data-stu-id="8e376-106">This action makes the grade and feedback associated with this submission available to the student.</span></span> <span data-ttu-id="8e376-107">这将提交的状态从"提交"变为"返回"，并指示提供反馈或分级完成。</span><span class="sxs-lookup"><span data-stu-id="8e376-107">This will change the status of the submission from "submitted" to "returned" and indicates that feedback is provided or grading is done.</span></span> <span data-ttu-id="8e376-108">此操作仅可通过教师。</span><span class="sxs-lookup"><span data-stu-id="8e376-108">This action can only be done by the teacher.</span></span>

## <a name="permissions"></a><span data-ttu-id="8e376-109">权限</span><span class="sxs-lookup"><span data-stu-id="8e376-109">Permissions</span></span>
<span data-ttu-id="8e376-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8e376-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8e376-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="8e376-112">Permission type</span></span>      | <span data-ttu-id="8e376-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="8e376-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8e376-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8e376-114">Delegated (work or school account)</span></span> |  <span data-ttu-id="8e376-115">EduAssignments.ReadWriteBasic EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8e376-115">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>   |
|<span data-ttu-id="8e376-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8e376-116">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="8e376-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="8e376-117">Not supported.</span></span>  |
|<span data-ttu-id="8e376-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="8e376-118">Application</span></span> | <span data-ttu-id="8e376-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="8e376-119">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="8e376-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8e376-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/{id}/assignments/{id}/submissions/{id}/return

```
## <a name="request-headers"></a><span data-ttu-id="8e376-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="8e376-121">Request headers</span></span>
| <span data-ttu-id="8e376-122">标头</span><span class="sxs-lookup"><span data-stu-id="8e376-122">Header</span></span>       | <span data-ttu-id="8e376-123">值</span><span class="sxs-lookup"><span data-stu-id="8e376-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="8e376-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="8e376-124">Authorization</span></span>  | <span data-ttu-id="8e376-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="8e376-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="8e376-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="8e376-127">Request body</span></span>
<span data-ttu-id="8e376-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="8e376-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8e376-129">响应</span><span class="sxs-lookup"><span data-stu-id="8e376-129">Response</span></span>
<span data-ttu-id="8e376-p105">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="8e376-p105">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8e376-132">示例</span><span class="sxs-lookup"><span data-stu-id="8e376-132">Example</span></span>
<span data-ttu-id="8e376-133">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="8e376-133">The following example shows how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="8e376-134">请求</span><span class="sxs-lookup"><span data-stu-id="8e376-134">Request</span></span>
<span data-ttu-id="8e376-135">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="8e376-135">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "educationsubmission_return"
}-->

```http
POST https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/submissions/850f51b7/return
```

##### <a name="response"></a><span data-ttu-id="8e376-136">响应</span><span class="sxs-lookup"><span data-stu-id="8e376-136">Response</span></span>
<span data-ttu-id="8e376-137">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="8e376-137">The following is an example of the response.</span></span>

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
  "description": "educationSubmission: return",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->