---
title: educationSubmission： release
description: " 并指示已完成评分。 此操作仅可由教师完成。"
author: dipakboyed
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 3cb2c5a8388ca10f3c2819d84957cf26eb75f2f6
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48007239"
---
# <a name="educationsubmission-release"></a><span data-ttu-id="88d74-104">educationSubmission： release</span><span class="sxs-lookup"><span data-stu-id="88d74-104">educationSubmission: release</span></span>

<span data-ttu-id="88d74-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="88d74-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="88d74-106">此操作将使 [educationOutcome](../resources/educationoutcome.md) ，其中包括与此提交相关的任何成绩或反馈，以供学生使用。</span><span class="sxs-lookup"><span data-stu-id="88d74-106">This action makes the [educationOutcome](../resources/educationoutcome.md) including any grades or feedback associated with this submission available to the student.</span></span> <span data-ttu-id="88d74-107">这会将提交状态从 "已提交" 更改为 "已发布"，并指示已完成评分。</span><span class="sxs-lookup"><span data-stu-id="88d74-107">This will change the status of the submission from "submitted" to "released" and indicates that grading is done.</span></span> <span data-ttu-id="88d74-108">此操作仅可由教师完成。</span><span class="sxs-lookup"><span data-stu-id="88d74-108">This action can only be done by the teacher.</span></span>

## <a name="permissions"></a><span data-ttu-id="88d74-109">权限</span><span class="sxs-lookup"><span data-stu-id="88d74-109">Permissions</span></span>
<span data-ttu-id="88d74-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="88d74-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="88d74-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="88d74-112">Permission type</span></span>      | <span data-ttu-id="88d74-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="88d74-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="88d74-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="88d74-114">Delegated (work or school account)</span></span> |  <span data-ttu-id="88d74-115">EduAssignments、ReadWriteBasic、EduAssignments</span><span class="sxs-lookup"><span data-stu-id="88d74-115">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>   |
|<span data-ttu-id="88d74-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="88d74-116">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="88d74-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="88d74-117">Not supported.</span></span>  |
|<span data-ttu-id="88d74-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="88d74-118">Application</span></span> | <span data-ttu-id="88d74-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="88d74-119">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="88d74-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="88d74-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/{id}/assignments/{id}/submissions/{id}/release

```
## <a name="request-headers"></a><span data-ttu-id="88d74-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="88d74-121">Request headers</span></span>
| <span data-ttu-id="88d74-122">标头</span><span class="sxs-lookup"><span data-stu-id="88d74-122">Header</span></span>       | <span data-ttu-id="88d74-123">值</span><span class="sxs-lookup"><span data-stu-id="88d74-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="88d74-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="88d74-124">Authorization</span></span>  | <span data-ttu-id="88d74-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="88d74-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="88d74-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="88d74-127">Request body</span></span>
<span data-ttu-id="88d74-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="88d74-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="88d74-129">响应</span><span class="sxs-lookup"><span data-stu-id="88d74-129">Response</span></span>
<span data-ttu-id="88d74-p105">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="88d74-p105">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="88d74-132">示例</span><span class="sxs-lookup"><span data-stu-id="88d74-132">Example</span></span>
<span data-ttu-id="88d74-133">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="88d74-133">The following example shows how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="88d74-134">请求</span><span class="sxs-lookup"><span data-stu-id="88d74-134">Request</span></span>
<span data-ttu-id="88d74-135">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="88d74-135">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "educationsubmission_release"
}-->

```http
POST https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/submissions/850f51b7/release
```

##### <a name="response"></a><span data-ttu-id="88d74-136">响应</span><span class="sxs-lookup"><span data-stu-id="88d74-136">Response</span></span>
<span data-ttu-id="88d74-137">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="88d74-137">The following is an example of the response.</span></span>

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


