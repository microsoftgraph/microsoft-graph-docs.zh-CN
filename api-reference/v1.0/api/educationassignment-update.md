---
title: 更新 educationassignment
description: 更新 educationAssigment 对象。
localization_priority: Normal
author: sharad-sharma-msft
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: d5a0015ae6c98e2a8a3355f0602027f15751c21e
ms.sourcegitcommit: e4461c7eb8c3d265fc1aa766125e81b58c6e1099
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2021
ms.locfileid: "52941443"
---
# <a name="update-educationassignment"></a><span data-ttu-id="5d084-103">更新 educationassignment</span><span class="sxs-lookup"><span data-stu-id="5d084-103">Update educationassignment</span></span>

<span data-ttu-id="5d084-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5d084-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="5d084-105">更新 educationAssigment 对象。</span><span class="sxs-lookup"><span data-stu-id="5d084-105">Update an educationAssigment object.</span></span> 

<span data-ttu-id="5d084-106">只有教师才能执行此操作。</span><span class="sxs-lookup"><span data-stu-id="5d084-106">Only teachers can perform this action.</span></span> 

<span data-ttu-id="5d084-107">或者，通过发布操作请求更改工作 [分配](../api/educationassignment-publish.md) 的状态。</span><span class="sxs-lookup"><span data-stu-id="5d084-107">Alternatively, request to change the status of an assignment with [publish](../api/educationassignment-publish.md) action.</span></span> <span data-ttu-id="5d084-108">请勿将 PATCH 操作用于此目的。</span><span class="sxs-lookup"><span data-stu-id="5d084-108">Don't use a PATCH operation for this purpose.</span></span>

## <a name="permissions"></a><span data-ttu-id="5d084-109">权限</span><span class="sxs-lookup"><span data-stu-id="5d084-109">Permissions</span></span>
<span data-ttu-id="5d084-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="5d084-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5d084-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="5d084-112">Permission type</span></span>      | <span data-ttu-id="5d084-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="5d084-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5d084-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5d084-114">Delegated (work or school account)</span></span> |  <span data-ttu-id="5d084-115">EduAssignments.ReadWriteBasic、EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5d084-115">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="5d084-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5d084-116">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="5d084-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="5d084-117">Not supported.</span></span>  |
|<span data-ttu-id="5d084-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="5d084-118">Application</span></span> | <span data-ttu-id="5d084-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="5d084-119">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="5d084-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5d084-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /education/classes/acdefc6b-2dc6-4e71-b1e9-6d9810ab1793/assignments/cf6005fc-9e13-44a2-a6ac-a53322006454
```
## <a name="request-headers"></a><span data-ttu-id="5d084-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="5d084-121">Request headers</span></span>
| <span data-ttu-id="5d084-122">标头</span><span class="sxs-lookup"><span data-stu-id="5d084-122">Header</span></span>       | <span data-ttu-id="5d084-123">值</span><span class="sxs-lookup"><span data-stu-id="5d084-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="5d084-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="5d084-124">Authorization</span></span>  | <span data-ttu-id="5d084-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="5d084-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="5d084-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="5d084-127">Content-Type</span></span>  | <span data-ttu-id="5d084-128">application/json</span><span class="sxs-lookup"><span data-stu-id="5d084-128">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="5d084-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="5d084-129">Request body</span></span>
<span data-ttu-id="5d084-130">在请求正文中，仅提供要更新的字段的值。</span><span class="sxs-lookup"><span data-stu-id="5d084-130">In the request body, supply only the values of the fields you want to update.</span></span> 

<span data-ttu-id="5d084-131">请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="5d084-131">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="5d084-132">为了获得最佳性能，请勿加入尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="5d084-132">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="5d084-133">属性</span><span class="sxs-lookup"><span data-stu-id="5d084-133">Property</span></span>     | <span data-ttu-id="5d084-134">类型</span><span class="sxs-lookup"><span data-stu-id="5d084-134">Type</span></span>   |<span data-ttu-id="5d084-135">说明</span><span class="sxs-lookup"><span data-stu-id="5d084-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5d084-136">addedStudentAction</span><span class="sxs-lookup"><span data-stu-id="5d084-136">addedStudentAction</span></span>|<span data-ttu-id="5d084-137">String</span><span class="sxs-lookup"><span data-stu-id="5d084-137">String</span></span>| <span data-ttu-id="5d084-138">描述是否应当将作业分发给在作业发布日期之后添加的学生。</span><span class="sxs-lookup"><span data-stu-id="5d084-138">Describes if the assignment should be distributed to students who are added after the assignment publication date.</span></span>|
|<span data-ttu-id="5d084-139">allowLateSubmissions</span><span class="sxs-lookup"><span data-stu-id="5d084-139">allowLateSubmissions</span></span>|<span data-ttu-id="5d084-140">Boolean</span><span class="sxs-lookup"><span data-stu-id="5d084-140">Boolean</span></span>| <span data-ttu-id="5d084-141">学生是否可以在截止日期后发送提交。</span><span class="sxs-lookup"><span data-stu-id="5d084-141">Whether students can send submission after the due date.</span></span>|
|<span data-ttu-id="5d084-142">allowStudentsToAddResourcesToSubmission</span><span class="sxs-lookup"><span data-stu-id="5d084-142">allowStudentsToAddResourcesToSubmission</span></span>|<span data-ttu-id="5d084-143">Boolean</span><span class="sxs-lookup"><span data-stu-id="5d084-143">Boolean</span></span>| <span data-ttu-id="5d084-144">学生是否可以向提交中添加资源。</span><span class="sxs-lookup"><span data-stu-id="5d084-144">Whether a student can add resources to a submission or not.</span></span> <span data-ttu-id="5d084-145">此外，指示提交中所有资源是否对应于工作分配资源列表。</span><span class="sxs-lookup"><span data-stu-id="5d084-145">Also, indicates whether all resources in the submission correspond to the assignment resource list.</span></span> |
|<span data-ttu-id="5d084-146">assignDateTime</span><span class="sxs-lookup"><span data-stu-id="5d084-146">assignDateTime</span></span>|<span data-ttu-id="5d084-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5d084-147">DateTimeOffset</span></span>| <span data-ttu-id="5d084-148">指示向学生发布作业的日期。</span><span class="sxs-lookup"><span data-stu-id="5d084-148">Indicates the date to publish the assignment to students.</span></span> |
|<span data-ttu-id="5d084-149">assignTo</span><span class="sxs-lookup"><span data-stu-id="5d084-149">assignTo</span></span>|<span data-ttu-id="5d084-150">educationAssignmentRecipient</span><span class="sxs-lookup"><span data-stu-id="5d084-150">educationAssignmentRecipient</span></span>| <span data-ttu-id="5d084-151">获得作业的学生。</span><span class="sxs-lookup"><span data-stu-id="5d084-151">Students who get the assignment.</span></span>|
|<span data-ttu-id="5d084-152">closeDateTime</span><span class="sxs-lookup"><span data-stu-id="5d084-152">closeDateTime</span></span>|<span data-ttu-id="5d084-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5d084-153">DateTimeOffset</span></span>| <span data-ttu-id="5d084-154">工作分配关闭提交的日期。</span><span class="sxs-lookup"><span data-stu-id="5d084-154">Date when the assignment will be closed for submissions.</span></span> <span data-ttu-id="5d084-155">如果分配不允许LateSubmissions或 closeDateTime 与 dueDateTime 相同，则该字段可以是 null 的可选字段，但如果指定，它必须大于或等于 dueDateTime。</span><span class="sxs-lookup"><span data-stu-id="5d084-155">This is an optional field that can be null if the assignment does not allowLateSubmissions or the closeDateTime is the same as the dueDateTime but if specified, it must be greater than or equal to the dueDateTime.</span></span>|
|<span data-ttu-id="5d084-156">displayName</span><span class="sxs-lookup"><span data-stu-id="5d084-156">displayName</span></span>|<span data-ttu-id="5d084-157">String</span><span class="sxs-lookup"><span data-stu-id="5d084-157">String</span></span>| <span data-ttu-id="5d084-158">工作分配的名称。</span><span class="sxs-lookup"><span data-stu-id="5d084-158">Name of assignment.</span></span> |
|<span data-ttu-id="5d084-159">dueDateTime</span><span class="sxs-lookup"><span data-stu-id="5d084-159">dueDateTime</span></span>|<span data-ttu-id="5d084-160">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5d084-160">DateTimeOffset</span></span>| <span data-ttu-id="5d084-161">日期分配到期。</span><span class="sxs-lookup"><span data-stu-id="5d084-161">Date assignment is due.</span></span> |
|<span data-ttu-id="5d084-162">一个</span><span class="sxs-lookup"><span data-stu-id="5d084-162">grading</span></span>|<span data-ttu-id="5d084-163">educationAssignmentGradeType</span><span class="sxs-lookup"><span data-stu-id="5d084-163">educationAssignmentGradeType</span></span>| <span data-ttu-id="5d084-164">如何对作业进行评分。</span><span class="sxs-lookup"><span data-stu-id="5d084-164">How the assignment will be graded.</span></span>|
|<span data-ttu-id="5d084-165">instructions</span><span class="sxs-lookup"><span data-stu-id="5d084-165">instructions</span></span>|<span data-ttu-id="5d084-166">itemBody</span><span class="sxs-lookup"><span data-stu-id="5d084-166">itemBody</span></span>| <span data-ttu-id="5d084-167">要与作业一起向学生提供的说明。</span><span class="sxs-lookup"><span data-stu-id="5d084-167">Instructions to be given to the students along with the assignment.</span></span> |
|<span data-ttu-id="5d084-168">notificationChannelUrl</span><span class="sxs-lookup"><span data-stu-id="5d084-168">notificationChannelUrl</span></span>|<span data-ttu-id="5d084-169">String</span><span class="sxs-lookup"><span data-stu-id="5d084-169">String</span></span>| <span data-ttu-id="5d084-170">与分配相关的通知通信的通道。</span><span class="sxs-lookup"><span data-stu-id="5d084-170">The channel to communicate notifications related to the assignment.</span></span> <span data-ttu-id="5d084-171">若要更改 URL，将值设置为 `assignTo` [educationAssignmentClassRecipient](../resources/educationassignmentclassrecipient.md)。</span><span class="sxs-lookup"><span data-stu-id="5d084-171">To change the URL, set the `assignTo` value to [educationAssignmentClassRecipient](../resources/educationassignmentclassrecipient.md).</span></span> <span data-ttu-id="5d084-172">频道 URL 在工作分配发布后不能更改。</span><span class="sxs-lookup"><span data-stu-id="5d084-172">The channel URL can't change after the publication of the assignment.</span></span>|

## <a name="response"></a><span data-ttu-id="5d084-173">响应</span><span class="sxs-lookup"><span data-stu-id="5d084-173">Response</span></span>
<span data-ttu-id="5d084-174">如果成功，此方法在响应正文中返回 响应代码和更新的 `200 OK` [educationAssignment](../resources/educationassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="5d084-174">If successful, this method returns a `200 OK` response code and an updated [educationAssignment](../resources/educationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5d084-175">示例</span><span class="sxs-lookup"><span data-stu-id="5d084-175">Example</span></span>

### <a name="request"></a><span data-ttu-id="5d084-176">请求</span><span class="sxs-lookup"><span data-stu-id="5d084-176">Request</span></span>
<span data-ttu-id="5d084-177">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="5d084-177">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "sampleKeys": ["ad8afb28-c138-4ad7-b7f5-a6986c2655a8"],
  "name": "update_educationassignment"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/education/classes/acdefc6b-2dc6-4e71-b1e9-6d9810ab1793/assignments/ad8afb28-c138-4ad7-b7f5-a6986c2655a8
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

### <a name="response"></a><span data-ttu-id="5d084-178">响应</span><span class="sxs-lookup"><span data-stu-id="5d084-178">Response</span></span>
<span data-ttu-id="5d084-179">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="5d084-179">The following is an example of the response.</span></span> 

><span data-ttu-id="5d084-180">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="5d084-180">**Note:** The response object shown here might be shortened for readability.</span></span>

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


