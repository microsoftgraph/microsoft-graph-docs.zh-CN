---
title: 更新 educationassignment
description: 更新工作分配对象。 只有课堂中的教师才能执行此操作。 请注意，不能使用 PATCH 请求来更改工作分配的状态。 使用 "发布" 操作可更改工作分配状态。
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 5d9dba365e554f317d4c085bc51e1967b7d0ab78
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48002541"
---
# <a name="update-educationassignment"></a><span data-ttu-id="ff666-106">更新 educationassignment</span><span class="sxs-lookup"><span data-stu-id="ff666-106">Update educationassignment</span></span>

<span data-ttu-id="ff666-107">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ff666-107">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ff666-108">更新工作分配对象。</span><span class="sxs-lookup"><span data-stu-id="ff666-108">Update the assignment object.</span></span> <span data-ttu-id="ff666-109">只有课堂中的教师才能执行此操作。</span><span class="sxs-lookup"><span data-stu-id="ff666-109">Only teachers in the class can do this.</span></span> <span data-ttu-id="ff666-110">请注意，不能使用 PATCH 请求来更改工作分配的状态。</span><span class="sxs-lookup"><span data-stu-id="ff666-110">Note that you can't use a PATCH request to change the status of an assignment.</span></span> <span data-ttu-id="ff666-111">使用 " [发布](../api/educationassignment-publish.md) " 操作可更改工作分配状态。</span><span class="sxs-lookup"><span data-stu-id="ff666-111">Use the [publish](../api/educationassignment-publish.md) action to change the assignment status.</span></span>

## <a name="permissions"></a><span data-ttu-id="ff666-112">权限</span><span class="sxs-lookup"><span data-stu-id="ff666-112">Permissions</span></span>
<span data-ttu-id="ff666-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ff666-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ff666-115">权限类型</span><span class="sxs-lookup"><span data-stu-id="ff666-115">Permission type</span></span>      | <span data-ttu-id="ff666-116">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ff666-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ff666-117">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ff666-117">Delegated (work or school account)</span></span> |  <span data-ttu-id="ff666-118">EduAssignments、ReadWriteBasic、EduAssignments</span><span class="sxs-lookup"><span data-stu-id="ff666-118">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="ff666-119">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ff666-119">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="ff666-120">不支持。</span><span class="sxs-lookup"><span data-stu-id="ff666-120">Not supported.</span></span>  |
|<span data-ttu-id="ff666-121">应用程序</span><span class="sxs-lookup"><span data-stu-id="ff666-121">Application</span></span> | <span data-ttu-id="ff666-122">不支持。</span><span class="sxs-lookup"><span data-stu-id="ff666-122">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="ff666-123">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ff666-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /education/classes/{id}/assignments/{id}
```
## <a name="request-headers"></a><span data-ttu-id="ff666-124">请求标头</span><span class="sxs-lookup"><span data-stu-id="ff666-124">Request headers</span></span>
| <span data-ttu-id="ff666-125">标头</span><span class="sxs-lookup"><span data-stu-id="ff666-125">Header</span></span>       | <span data-ttu-id="ff666-126">值</span><span class="sxs-lookup"><span data-stu-id="ff666-126">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="ff666-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="ff666-127">Authorization</span></span>  | <span data-ttu-id="ff666-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="ff666-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="ff666-130">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ff666-130">Content-Type</span></span>  | <span data-ttu-id="ff666-131">application/json</span><span class="sxs-lookup"><span data-stu-id="ff666-131">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="ff666-132">请求正文</span><span class="sxs-lookup"><span data-stu-id="ff666-132">Request body</span></span>
<span data-ttu-id="ff666-133">在请求正文中，提供应更新的相关字段的值。</span><span class="sxs-lookup"><span data-stu-id="ff666-133">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="ff666-134">请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="ff666-134">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="ff666-135">为了获得最佳性能，请勿加入尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="ff666-135">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="ff666-136">属性</span><span class="sxs-lookup"><span data-stu-id="ff666-136">Property</span></span>     | <span data-ttu-id="ff666-137">类型</span><span class="sxs-lookup"><span data-stu-id="ff666-137">Type</span></span>   |<span data-ttu-id="ff666-138">说明</span><span class="sxs-lookup"><span data-stu-id="ff666-138">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ff666-139">allowLateSubmissions</span><span class="sxs-lookup"><span data-stu-id="ff666-139">allowLateSubmissions</span></span>|<span data-ttu-id="ff666-140">Boolean</span><span class="sxs-lookup"><span data-stu-id="ff666-140">Boolean</span></span>| <span data-ttu-id="ff666-141">提交在截止日期之后是否可以提交。</span><span class="sxs-lookup"><span data-stu-id="ff666-141">Whether submissions can be submitted after the due date.</span></span>|
|<span data-ttu-id="ff666-142">allowStudentsToAddResourcesToSubmission</span><span class="sxs-lookup"><span data-stu-id="ff666-142">allowStudentsToAddResourcesToSubmission</span></span>|<span data-ttu-id="ff666-143">Boolean</span><span class="sxs-lookup"><span data-stu-id="ff666-143">Boolean</span></span>| <span data-ttu-id="ff666-144">学生是否可以将资源添加到提交。</span><span class="sxs-lookup"><span data-stu-id="ff666-144">Whether a student can add resources to a submission.</span></span> <span data-ttu-id="ff666-145">指示提交的唯一项目是否来自工作分配资源列表。</span><span class="sxs-lookup"><span data-stu-id="ff666-145">Indicated whether the only items on the submission came from the assignment resource list.</span></span> |
|<span data-ttu-id="ff666-146">assignDateTime</span><span class="sxs-lookup"><span data-stu-id="ff666-146">assignDateTime</span></span>|<span data-ttu-id="ff666-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ff666-147">DateTimeOffset</span></span>| <span data-ttu-id="ff666-148">应将分配发布给学生的日期。</span><span class="sxs-lookup"><span data-stu-id="ff666-148">Date the assignment should be published to students.</span></span> |
|<span data-ttu-id="ff666-149">assignTo</span><span class="sxs-lookup"><span data-stu-id="ff666-149">assignTo</span></span>|<span data-ttu-id="ff666-150">educationAssignmentRecipient</span><span class="sxs-lookup"><span data-stu-id="ff666-150">educationAssignmentRecipient</span></span>| <span data-ttu-id="ff666-151">获取工作分配的学生。</span><span class="sxs-lookup"><span data-stu-id="ff666-151">Students who get the assignment.</span></span>|
|<span data-ttu-id="ff666-152">closeDateTime</span><span class="sxs-lookup"><span data-stu-id="ff666-152">closeDateTime</span></span>|<span data-ttu-id="ff666-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ff666-153">DateTimeOffset</span></span>| <span data-ttu-id="ff666-154">将为提交关闭工作分配的日期。</span><span class="sxs-lookup"><span data-stu-id="ff666-154">Date when the assignment will be closed for submissions.</span></span> <span data-ttu-id="ff666-155">这是可选字段，如果工作分配不 allowLateSubmissions 或 closeDateTime 与 dueDateTime 相同，则可以为 null，但如果指定，则它必须大于或等于 dueDateTime。</span><span class="sxs-lookup"><span data-stu-id="ff666-155">This is an optional field that can be null if the assignment does not allowLateSubmissions or the closeDateTime is the same as the dueDateTime but if specified, it must be greater than or equal to the dueDateTime.</span></span>|
|<span data-ttu-id="ff666-156">displayName</span><span class="sxs-lookup"><span data-stu-id="ff666-156">displayName</span></span>|<span data-ttu-id="ff666-157">String</span><span class="sxs-lookup"><span data-stu-id="ff666-157">String</span></span>| <span data-ttu-id="ff666-158">分配的名称。</span><span class="sxs-lookup"><span data-stu-id="ff666-158">Name of assignment.</span></span> |
|<span data-ttu-id="ff666-159">dueDateTime</span><span class="sxs-lookup"><span data-stu-id="ff666-159">dueDateTime</span></span>|<span data-ttu-id="ff666-160">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ff666-160">DateTimeOffset</span></span>| <span data-ttu-id="ff666-161">日期工作分配到期。</span><span class="sxs-lookup"><span data-stu-id="ff666-161">Date assignment is due.</span></span> |
|<span data-ttu-id="ff666-162">评分</span><span class="sxs-lookup"><span data-stu-id="ff666-162">grading</span></span>|<span data-ttu-id="ff666-163">educationAssignmentGradeType</span><span class="sxs-lookup"><span data-stu-id="ff666-163">educationAssignmentGradeType</span></span>| <span data-ttu-id="ff666-164">将如何对工作分配进行评分。</span><span class="sxs-lookup"><span data-stu-id="ff666-164">How the assignment will be graded.</span></span>|
|<span data-ttu-id="ff666-165">指令</span><span class="sxs-lookup"><span data-stu-id="ff666-165">instructions</span></span>|<span data-ttu-id="ff666-166">itemBody</span><span class="sxs-lookup"><span data-stu-id="ff666-166">itemBody</span></span>| <span data-ttu-id="ff666-167">向学生分配的说明以及工作分配。</span><span class="sxs-lookup"><span data-stu-id="ff666-167">Instructions to be given to the students along with the assignment.</span></span> |

## <a name="response"></a><span data-ttu-id="ff666-168">响应</span><span class="sxs-lookup"><span data-stu-id="ff666-168">Response</span></span>
<span data-ttu-id="ff666-169">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和更新的 [educationAssignment](../resources/educationassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="ff666-169">If successful, this method returns a `200 OK` response code and an updated [educationAssignment](../resources/educationassignment.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="ff666-170">示例</span><span class="sxs-lookup"><span data-stu-id="ff666-170">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ff666-171">请求</span><span class="sxs-lookup"><span data-stu-id="ff666-171">Request</span></span>
<span data-ttu-id="ff666-172">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="ff666-172">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="ff666-173">HTTP</span><span class="sxs-lookup"><span data-stu-id="ff666-173">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_educationassignment"
}-->
```http
PATCH https://graph.microsoft.com/beta/education/classes/11021/assignments/19002
Content-type: application/json
Content-length: 279

{
  "displayName": "Week 1 reading assignment",
  "instructions": {
    "contentType": "Text",
    "content": "Read chapters 1 through 3"
  },
  "dueDateTime": "2014-02-01T00:00:00Z"
}
```
# <a name="c"></a>[<span data-ttu-id="ff666-174">C#</span><span class="sxs-lookup"><span data-stu-id="ff666-174">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-educationassignment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ff666-175">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ff666-175">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-educationassignment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ff666-176">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ff666-176">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-educationassignment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="ff666-177">响应</span><span class="sxs-lookup"><span data-stu-id="ff666-177">Response</span></span>
<span data-ttu-id="ff666-178">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="ff666-178">The following is an example of the response.</span></span> 

><span data-ttu-id="ff666-179">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="ff666-179">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="ff666-180">将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="ff666-180">All of the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationAssignment"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 279

{
  "classId": "11021",
  "displayName": "Week 1 reading assignment",
  "instructions": {
    "contentType": "Text",
    "content": "Read chapters 1 through 3"
  },
  "closeDateTime": "2014-02-11T00:00:00Z",
  "dueDateTime": "2014-02-01T00:00:00Z",
  "assignDateTime": "2014-01-01T00:00:00Z",
  "assignedDateTime": "2014-01-01T00:00:00Z"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update educationassignment",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


