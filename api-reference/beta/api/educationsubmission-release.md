---
title: educationSubmission： release
description: " 并指示已完成评分。 此操作仅可由教师完成。"
author: dipakboyed
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 5ac32d42367d68e405263c66a9bdd980bb652ae5
ms.sourcegitcommit: bbef506636bce5b72351ee3834123771c301b1b1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/25/2019
ms.locfileid: "37726191"
---
# <a name="educationsubmission-release"></a><span data-ttu-id="2bfca-104">educationSubmission： release</span><span class="sxs-lookup"><span data-stu-id="2bfca-104">educationSubmission: release</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2bfca-105">此操作将使[educationOutcome](../resources/educationoutcome.md) ，其中包括与此提交相关的任何成绩或反馈，以供学生使用。</span><span class="sxs-lookup"><span data-stu-id="2bfca-105">This action makes the [educationOutcome](../resources/educationoutcome.md) including any grades or feedback associated with this submission available to the student.</span></span> <span data-ttu-id="2bfca-106">这会将提交状态从 "已提交" 更改为 "已发布"，并指示已完成评分。</span><span class="sxs-lookup"><span data-stu-id="2bfca-106">This will change the status of the submission from "submitted" to "released" and indicates that grading is done.</span></span> <span data-ttu-id="2bfca-107">此操作仅可由教师完成。</span><span class="sxs-lookup"><span data-stu-id="2bfca-107">This action can only be done by the teacher.</span></span>

## <a name="permissions"></a><span data-ttu-id="2bfca-108">权限</span><span class="sxs-lookup"><span data-stu-id="2bfca-108">Permissions</span></span>
<span data-ttu-id="2bfca-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2bfca-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2bfca-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="2bfca-111">Permission type</span></span>      | <span data-ttu-id="2bfca-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="2bfca-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2bfca-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2bfca-113">Delegated (work or school account)</span></span> |  <span data-ttu-id="2bfca-114">EduAssignments、ReadWriteBasic、EduAssignments</span><span class="sxs-lookup"><span data-stu-id="2bfca-114">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>   |
|<span data-ttu-id="2bfca-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2bfca-115">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="2bfca-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="2bfca-116">Not supported.</span></span>  |
|<span data-ttu-id="2bfca-117">Application</span><span class="sxs-lookup"><span data-stu-id="2bfca-117">Application</span></span> | <span data-ttu-id="2bfca-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="2bfca-118">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="2bfca-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2bfca-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/{id}/assignments/{id}/submissions/{id}/release

```
## <a name="request-headers"></a><span data-ttu-id="2bfca-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="2bfca-120">Request headers</span></span>
| <span data-ttu-id="2bfca-121">标头</span><span class="sxs-lookup"><span data-stu-id="2bfca-121">Header</span></span>       | <span data-ttu-id="2bfca-122">值</span><span class="sxs-lookup"><span data-stu-id="2bfca-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="2bfca-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="2bfca-123">Authorization</span></span>  | <span data-ttu-id="2bfca-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="2bfca-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="2bfca-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="2bfca-126">Request body</span></span>
<span data-ttu-id="2bfca-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="2bfca-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2bfca-128">响应</span><span class="sxs-lookup"><span data-stu-id="2bfca-128">Response</span></span>
<span data-ttu-id="2bfca-p105">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="2bfca-p105">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2bfca-131">示例</span><span class="sxs-lookup"><span data-stu-id="2bfca-131">Example</span></span>
<span data-ttu-id="2bfca-132">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="2bfca-132">The following example shows how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="2bfca-133">请求</span><span class="sxs-lookup"><span data-stu-id="2bfca-133">Request</span></span>
<span data-ttu-id="2bfca-134">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="2bfca-134">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "educationsubmission_release"
}-->

```http
POST https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/submissions/850f51b7/release
```

##### <a name="response"></a><span data-ttu-id="2bfca-135">响应</span><span class="sxs-lookup"><span data-stu-id="2bfca-135">Response</span></span>
<span data-ttu-id="2bfca-136">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="2bfca-136">The following is an example of the response.</span></span>

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
  "description": "educationSubmission: release",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
