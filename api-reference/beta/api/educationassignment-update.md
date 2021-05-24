---
title: 更新 educationassignment
description: 更新分配对象。 只有班级中的教师可以这样做。 请注意，你不能使用 PATCH 请求更改工作分配的状态。 使用发布操作可更改工作分配状态。
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: fcaed5b3c73039aeac6c1861a8b1ddcd4e5f19d8
ms.sourcegitcommit: 276a13a37c3772689dfc71f7cd47586c9581f27d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/24/2021
ms.locfileid: "52629180"
---
# <a name="update-educationassignment"></a><span data-ttu-id="d0953-106">更新 educationassignment</span><span class="sxs-lookup"><span data-stu-id="d0953-106">Update educationassignment</span></span>

<span data-ttu-id="d0953-107">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d0953-107">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d0953-108">更新分配对象。</span><span class="sxs-lookup"><span data-stu-id="d0953-108">Update the assignment object.</span></span> <span data-ttu-id="d0953-109">只有班级中的教师可以这样做。</span><span class="sxs-lookup"><span data-stu-id="d0953-109">Only teachers in the class can do this.</span></span> <span data-ttu-id="d0953-110">请注意，你不能使用 PATCH 请求更改工作分配的状态。</span><span class="sxs-lookup"><span data-stu-id="d0953-110">Note that you can't use a PATCH request to change the status of an assignment.</span></span> <span data-ttu-id="d0953-111">使用 [发布](../api/educationassignment-publish.md) 操作可更改工作分配状态。</span><span class="sxs-lookup"><span data-stu-id="d0953-111">Use the [publish](../api/educationassignment-publish.md) action to change the assignment status.</span></span>

## <a name="permissions"></a><span data-ttu-id="d0953-112">Permissions</span><span class="sxs-lookup"><span data-stu-id="d0953-112">Permissions</span></span>
<span data-ttu-id="d0953-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d0953-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d0953-115">权限类型</span><span class="sxs-lookup"><span data-stu-id="d0953-115">Permission type</span></span>      | <span data-ttu-id="d0953-116">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d0953-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d0953-117">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d0953-117">Delegated (work or school account)</span></span> |  <span data-ttu-id="d0953-118">EduAssignments.ReadWriteBasic、EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d0953-118">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="d0953-119">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d0953-119">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="d0953-120">不支持。</span><span class="sxs-lookup"><span data-stu-id="d0953-120">Not supported.</span></span>  |
|<span data-ttu-id="d0953-121">应用程序</span><span class="sxs-lookup"><span data-stu-id="d0953-121">Application</span></span> | <span data-ttu-id="d0953-122">不支持。</span><span class="sxs-lookup"><span data-stu-id="d0953-122">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="d0953-123">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d0953-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /education/classes/{id}/assignments/{id}
```
## <a name="request-headers"></a><span data-ttu-id="d0953-124">请求标头</span><span class="sxs-lookup"><span data-stu-id="d0953-124">Request headers</span></span>
| <span data-ttu-id="d0953-125">标头</span><span class="sxs-lookup"><span data-stu-id="d0953-125">Header</span></span>       | <span data-ttu-id="d0953-126">值</span><span class="sxs-lookup"><span data-stu-id="d0953-126">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="d0953-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="d0953-127">Authorization</span></span>  | <span data-ttu-id="d0953-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="d0953-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="d0953-130">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d0953-130">Content-Type</span></span>  | <span data-ttu-id="d0953-131">application/json</span><span class="sxs-lookup"><span data-stu-id="d0953-131">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="d0953-132">请求正文</span><span class="sxs-lookup"><span data-stu-id="d0953-132">Request body</span></span>
<span data-ttu-id="d0953-133">在请求正文中，提供应更新的相关字段的值。</span><span class="sxs-lookup"><span data-stu-id="d0953-133">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="d0953-134">请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="d0953-134">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="d0953-135">为了获得最佳性能，请勿加入尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="d0953-135">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="d0953-136">属性</span><span class="sxs-lookup"><span data-stu-id="d0953-136">Property</span></span>     | <span data-ttu-id="d0953-137">类型</span><span class="sxs-lookup"><span data-stu-id="d0953-137">Type</span></span>   |<span data-ttu-id="d0953-138">说明</span><span class="sxs-lookup"><span data-stu-id="d0953-138">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d0953-139">addedStudentAction</span><span class="sxs-lookup"><span data-stu-id="d0953-139">addedStudentAction</span></span>|<span data-ttu-id="d0953-140">String</span><span class="sxs-lookup"><span data-stu-id="d0953-140">String</span></span>| <span data-ttu-id="d0953-141">控制在作业发布后添加的学生的行为。</span><span class="sxs-lookup"><span data-stu-id="d0953-141">Controls the behavior for students who are added after the assignment is published.</span></span>|
|<span data-ttu-id="d0953-142">allowLateSubmissions</span><span class="sxs-lookup"><span data-stu-id="d0953-142">allowLateSubmissions</span></span>|<span data-ttu-id="d0953-143">布尔值</span><span class="sxs-lookup"><span data-stu-id="d0953-143">Boolean</span></span>| <span data-ttu-id="d0953-144">提交是否可在截止日期后提交。</span><span class="sxs-lookup"><span data-stu-id="d0953-144">Whether submissions can be submitted after the due date.</span></span>|
|<span data-ttu-id="d0953-145">allowStudentsToAddResourcesToSubmission</span><span class="sxs-lookup"><span data-stu-id="d0953-145">allowStudentsToAddResourcesToSubmission</span></span>|<span data-ttu-id="d0953-146">布尔值</span><span class="sxs-lookup"><span data-stu-id="d0953-146">Boolean</span></span>| <span data-ttu-id="d0953-147">学生是否可以向提交中添加资源。</span><span class="sxs-lookup"><span data-stu-id="d0953-147">Whether a student can add resources to a submission.</span></span> <span data-ttu-id="d0953-148">指示提交中的唯一项目是否来自工作分配资源列表。</span><span class="sxs-lookup"><span data-stu-id="d0953-148">Indicated whether the only items on the submission came from the assignment resource list.</span></span> |
|<span data-ttu-id="d0953-149">assignDateTime</span><span class="sxs-lookup"><span data-stu-id="d0953-149">assignDateTime</span></span>|<span data-ttu-id="d0953-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d0953-150">DateTimeOffset</span></span>| <span data-ttu-id="d0953-151">作业应发布到学生的日期。</span><span class="sxs-lookup"><span data-stu-id="d0953-151">Date the assignment should be published to students.</span></span> |
|<span data-ttu-id="d0953-152">assignTo</span><span class="sxs-lookup"><span data-stu-id="d0953-152">assignTo</span></span>|<span data-ttu-id="d0953-153">educationAssignmentRecipient</span><span class="sxs-lookup"><span data-stu-id="d0953-153">educationAssignmentRecipient</span></span>| <span data-ttu-id="d0953-154">获得作业的学生。</span><span class="sxs-lookup"><span data-stu-id="d0953-154">Students who get the assignment.</span></span>|
|<span data-ttu-id="d0953-155">closeDateTime</span><span class="sxs-lookup"><span data-stu-id="d0953-155">closeDateTime</span></span>|<span data-ttu-id="d0953-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d0953-156">DateTimeOffset</span></span>| <span data-ttu-id="d0953-157">工作分配关闭提交的日期。</span><span class="sxs-lookup"><span data-stu-id="d0953-157">Date when the assignment will be closed for submissions.</span></span> <span data-ttu-id="d0953-158">如果分配不允许LateSubmissions或 closeDateTime 与 dueDateTime 相同，则该字段可以是 null 的可选字段，但如果指定，它必须大于或等于 dueDateTime。</span><span class="sxs-lookup"><span data-stu-id="d0953-158">This is an optional field that can be null if the assignment does not allowLateSubmissions or the closeDateTime is the same as the dueDateTime but if specified, it must be greater than or equal to the dueDateTime.</span></span>|
|<span data-ttu-id="d0953-159">displayName</span><span class="sxs-lookup"><span data-stu-id="d0953-159">displayName</span></span>|<span data-ttu-id="d0953-160">String</span><span class="sxs-lookup"><span data-stu-id="d0953-160">String</span></span>| <span data-ttu-id="d0953-161">工作分配的名称。</span><span class="sxs-lookup"><span data-stu-id="d0953-161">Name of assignment.</span></span> |
|<span data-ttu-id="d0953-162">dueDateTime</span><span class="sxs-lookup"><span data-stu-id="d0953-162">dueDateTime</span></span>|<span data-ttu-id="d0953-163">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d0953-163">DateTimeOffset</span></span>| <span data-ttu-id="d0953-164">日期分配到期。</span><span class="sxs-lookup"><span data-stu-id="d0953-164">Date assignment is due.</span></span> |
|<span data-ttu-id="d0953-165">一个</span><span class="sxs-lookup"><span data-stu-id="d0953-165">grading</span></span>|<span data-ttu-id="d0953-166">educationAssignmentGradeType</span><span class="sxs-lookup"><span data-stu-id="d0953-166">educationAssignmentGradeType</span></span>| <span data-ttu-id="d0953-167">如何对作业进行评分。</span><span class="sxs-lookup"><span data-stu-id="d0953-167">How the assignment will be graded.</span></span>|
|<span data-ttu-id="d0953-168">instructions</span><span class="sxs-lookup"><span data-stu-id="d0953-168">instructions</span></span>|<span data-ttu-id="d0953-169">itemBody</span><span class="sxs-lookup"><span data-stu-id="d0953-169">itemBody</span></span>| <span data-ttu-id="d0953-170">要与作业一起向学生提供的说明。</span><span class="sxs-lookup"><span data-stu-id="d0953-170">Instructions to be given to the students along with the assignment.</span></span> |
|<span data-ttu-id="d0953-171">notificationChannelUrl</span><span class="sxs-lookup"><span data-stu-id="d0953-171">notificationChannelUrl</span></span>|<span data-ttu-id="d0953-172">String</span><span class="sxs-lookup"><span data-stu-id="d0953-172">String</span></span>| <span data-ttu-id="d0953-173">发布工作分配发布通知的频道。</span><span class="sxs-lookup"><span data-stu-id="d0953-173">Channel to post assignment publish notification.</span></span> <span data-ttu-id="d0953-174">发布分配后不允许更新通道 URL，并且仅在 **assignTo** 值为 [educationAssignmentClassRecipient 时允许更新](../resources/educationassignmentclassrecipient.md)。</span><span class="sxs-lookup"><span data-stu-id="d0953-174">Updating the channel URL is not allowed after the assignment has been published and is only allowed when the **assignTo** value is [educationAssignmentClassRecipient](../resources/educationassignmentclassrecipient.md).</span></span>|

## <a name="response"></a><span data-ttu-id="d0953-175">响应</span><span class="sxs-lookup"><span data-stu-id="d0953-175">Response</span></span>
<span data-ttu-id="d0953-176">如果成功，此方法在响应正文中返回 响应代码和更新的 `200 OK` [educationAssignment](../resources/educationassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="d0953-176">If successful, this method returns a `200 OK` response code and an updated [educationAssignment](../resources/educationassignment.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="d0953-177">示例</span><span class="sxs-lookup"><span data-stu-id="d0953-177">Example</span></span>
### <a name="request"></a><span data-ttu-id="d0953-178">请求</span><span class="sxs-lookup"><span data-stu-id="d0953-178">Request</span></span>
<span data-ttu-id="d0953-179">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="d0953-179">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="d0953-180">HTTP</span><span class="sxs-lookup"><span data-stu-id="d0953-180">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="d0953-181">C#</span><span class="sxs-lookup"><span data-stu-id="d0953-181">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-educationassignment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d0953-182">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d0953-182">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-educationassignment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d0953-183">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d0953-183">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-educationassignment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d0953-184">Java</span><span class="sxs-lookup"><span data-stu-id="d0953-184">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-educationassignment-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="d0953-185">响应</span><span class="sxs-lookup"><span data-stu-id="d0953-185">Response</span></span>
<span data-ttu-id="d0953-186">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="d0953-186">The following is an example of the response.</span></span> 

><span data-ttu-id="d0953-187">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="d0953-187">**Note:** The response object shown here might be shortened for readability.</span></span>

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
  "assignedDateTime": "2014-01-01T00:00:00Z",
  "resourcesFolderUrl": "https://graph.microsoft.com/v1.0/drives/b!0sGAoOieeE6iSj1WXCV-nYYTuh2luKRDvUVGQBLOmvYpRzc5ARnCRorRht6P3MhU/items/01N74NOEZL7P3VK22SQFDKBZ3PHVPKDVAQ",
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


