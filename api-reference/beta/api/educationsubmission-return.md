---
title: 'educationSubmission: 返回'
description: 此操作使与此提交相关联的评分和反馈可供学生使用。
author: dipakboyed
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 8d86cb72b54acae5485125e5516e494baeeaccef
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33324850"
---
# <a name="educationsubmission-return"></a><span data-ttu-id="0b44e-103">educationSubmission: 返回</span><span class="sxs-lookup"><span data-stu-id="0b44e-103">educationSubmission: return</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0b44e-104">此操作使与此提交相关联的评分和反馈可供学生使用。</span><span class="sxs-lookup"><span data-stu-id="0b44e-104">This action makes the grade and feedback associated with this submission available to the student.</span></span> <span data-ttu-id="0b44e-105">这会将提交的状态从 "已提交" 更改为 "已返回", 并指示反馈已提供或已完成评分。</span><span class="sxs-lookup"><span data-stu-id="0b44e-105">This will change the status of the submission from "submitted" to "returned" and indicates that feedback is provided or grading is done.</span></span> <span data-ttu-id="0b44e-106">此操作仅可由教师完成。</span><span class="sxs-lookup"><span data-stu-id="0b44e-106">This action can only be done by the teacher.</span></span>

## <a name="permissions"></a><span data-ttu-id="0b44e-107">权限</span><span class="sxs-lookup"><span data-stu-id="0b44e-107">Permissions</span></span>
<span data-ttu-id="0b44e-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0b44e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0b44e-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="0b44e-110">Permission type</span></span>      | <span data-ttu-id="0b44e-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="0b44e-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0b44e-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0b44e-112">Delegated (work or school account)</span></span> |  <span data-ttu-id="0b44e-113">EduAssignments、ReadWriteBasic、EduAssignments</span><span class="sxs-lookup"><span data-stu-id="0b44e-113">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>   |
|<span data-ttu-id="0b44e-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0b44e-114">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="0b44e-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="0b44e-115">Not supported.</span></span>  |
|<span data-ttu-id="0b44e-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="0b44e-116">Application</span></span> | <span data-ttu-id="0b44e-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="0b44e-117">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="0b44e-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0b44e-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/{id}/assignments/{id}/submissions/{id}/return

```
## <a name="request-headers"></a><span data-ttu-id="0b44e-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="0b44e-119">Request headers</span></span>
| <span data-ttu-id="0b44e-120">标头</span><span class="sxs-lookup"><span data-stu-id="0b44e-120">Header</span></span>       | <span data-ttu-id="0b44e-121">值</span><span class="sxs-lookup"><span data-stu-id="0b44e-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="0b44e-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="0b44e-122">Authorization</span></span>  | <span data-ttu-id="0b44e-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="0b44e-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="0b44e-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="0b44e-125">Request body</span></span>
<span data-ttu-id="0b44e-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="0b44e-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0b44e-127">响应</span><span class="sxs-lookup"><span data-stu-id="0b44e-127">Response</span></span>
<span data-ttu-id="0b44e-p104">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="0b44e-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0b44e-130">示例</span><span class="sxs-lookup"><span data-stu-id="0b44e-130">Example</span></span>
<span data-ttu-id="0b44e-131">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="0b44e-131">The following example shows how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="0b44e-132">请求</span><span class="sxs-lookup"><span data-stu-id="0b44e-132">Request</span></span>
<span data-ttu-id="0b44e-133">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="0b44e-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "educationsubmission_return"
}-->

```http
POST https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/submissions/850f51b7/return
```

##### <a name="response"></a><span data-ttu-id="0b44e-134">响应</span><span class="sxs-lookup"><span data-stu-id="0b44e-134">Response</span></span>
<span data-ttu-id="0b44e-135">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="0b44e-135">The following is an example of the response.</span></span>

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
  "description": "educationSubmission: return",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
