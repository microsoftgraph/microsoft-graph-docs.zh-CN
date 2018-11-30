---
title: 更新 educationassignment
description: 更新的 assignment 对象。 仅教师类中的可以执行此操作。 请注意，您无法使用 PATCH 请求更改的工作分配状态。 使用发布操作更改的工作分配状态。
ms.openlocfilehash: 8b23b7ac4b971856ed7a96b4991fca2e5220d069
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27044226"
---
# <a name="update-educationassignment"></a><span data-ttu-id="b8bcc-106">更新 educationassignment</span><span class="sxs-lookup"><span data-stu-id="b8bcc-106">Update educationassignment</span></span>

> <span data-ttu-id="b8bcc-107">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="b8bcc-107">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b8bcc-108">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="b8bcc-108">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="b8bcc-109">更新的 assignment 对象。</span><span class="sxs-lookup"><span data-stu-id="b8bcc-109">Update the assignment object.</span></span> <span data-ttu-id="b8bcc-110">仅教师类中的可以执行此操作。</span><span class="sxs-lookup"><span data-stu-id="b8bcc-110">Only teachers in the class can do this.</span></span> <span data-ttu-id="b8bcc-111">请注意，您无法使用 PATCH 请求更改的工作分配状态。</span><span class="sxs-lookup"><span data-stu-id="b8bcc-111">Note that you can't use a PATCH request to change the status of an assignment.</span></span> <span data-ttu-id="b8bcc-112">使用[发布](../api/educationassignment-publish.md)操作更改的工作分配状态。</span><span class="sxs-lookup"><span data-stu-id="b8bcc-112">Use the [publish](../api/educationassignment-publish.md) action to change the assignment status.</span></span>

## <a name="permissions"></a><span data-ttu-id="b8bcc-113">权限</span><span class="sxs-lookup"><span data-stu-id="b8bcc-113">Permissions</span></span>
<span data-ttu-id="b8bcc-p104">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b8bcc-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b8bcc-116">权限类型</span><span class="sxs-lookup"><span data-stu-id="b8bcc-116">Permission type</span></span>      | <span data-ttu-id="b8bcc-117">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b8bcc-117">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b8bcc-118">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b8bcc-118">Delegated (work or school account)</span></span> |  <span data-ttu-id="b8bcc-119">EduAssignments.ReadWriteBasic EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b8bcc-119">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="b8bcc-120">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b8bcc-120">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="b8bcc-121">不支持。</span><span class="sxs-lookup"><span data-stu-id="b8bcc-121">Not supported.</span></span>  |
|<span data-ttu-id="b8bcc-122">应用程序</span><span class="sxs-lookup"><span data-stu-id="b8bcc-122">Application</span></span> | <span data-ttu-id="b8bcc-123">不支持。</span><span class="sxs-lookup"><span data-stu-id="b8bcc-123">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="b8bcc-124">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b8bcc-124">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /education/classes/{id}/assignments/{id}
```
## <a name="request-headers"></a><span data-ttu-id="b8bcc-125">请求标头</span><span class="sxs-lookup"><span data-stu-id="b8bcc-125">Request headers</span></span>
| <span data-ttu-id="b8bcc-126">标头</span><span class="sxs-lookup"><span data-stu-id="b8bcc-126">Header</span></span>       | <span data-ttu-id="b8bcc-127">值</span><span class="sxs-lookup"><span data-stu-id="b8bcc-127">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="b8bcc-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="b8bcc-128">Authorization</span></span>  | <span data-ttu-id="b8bcc-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="b8bcc-p105">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="b8bcc-131">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b8bcc-131">Content-Type</span></span>  | <span data-ttu-id="b8bcc-132">application/json</span><span class="sxs-lookup"><span data-stu-id="b8bcc-132">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="b8bcc-133">请求正文</span><span class="sxs-lookup"><span data-stu-id="b8bcc-133">Request body</span></span>
<span data-ttu-id="b8bcc-134">在请求正文中，提供应更新的相关字段的值。</span><span class="sxs-lookup"><span data-stu-id="b8bcc-134">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="b8bcc-135">请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="b8bcc-135">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="b8bcc-136">为了获得最佳性能，请勿加入尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="b8bcc-136">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="b8bcc-137">属性</span><span class="sxs-lookup"><span data-stu-id="b8bcc-137">Property</span></span>     | <span data-ttu-id="b8bcc-138">类型</span><span class="sxs-lookup"><span data-stu-id="b8bcc-138">Type</span></span>   |<span data-ttu-id="b8bcc-139">说明</span><span class="sxs-lookup"><span data-stu-id="b8bcc-139">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b8bcc-140">allowLateSubmissions</span><span class="sxs-lookup"><span data-stu-id="b8bcc-140">allowLateSubmissions</span></span>|<span data-ttu-id="b8bcc-141">布尔</span><span class="sxs-lookup"><span data-stu-id="b8bcc-141">Boolean</span></span>| <span data-ttu-id="b8bcc-142">是否可以在截止日期之后提交提交。</span><span class="sxs-lookup"><span data-stu-id="b8bcc-142">Whether submissions can be submitted after the due date.</span></span>|
|<span data-ttu-id="b8bcc-143">allowStudentsToAddResourcesToSubmission</span><span class="sxs-lookup"><span data-stu-id="b8bcc-143">allowStudentsToAddResourcesToSubmission</span></span>|<span data-ttu-id="b8bcc-144">布尔</span><span class="sxs-lookup"><span data-stu-id="b8bcc-144">Boolean</span></span>| <span data-ttu-id="b8bcc-145">是否学生可以将资源添加到提交。</span><span class="sxs-lookup"><span data-stu-id="b8bcc-145">Whether a student can add resources to a submission.</span></span> <span data-ttu-id="b8bcc-146">指示在提交的那些项目是否来自工作分配资源列表。</span><span class="sxs-lookup"><span data-stu-id="b8bcc-146">Indicated whether the only items on the submission came from the assignment resource list.</span></span> |
|<span data-ttu-id="b8bcc-147">assignDateTime</span><span class="sxs-lookup"><span data-stu-id="b8bcc-147">assignDateTime</span></span>|<span data-ttu-id="b8bcc-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b8bcc-148">DateTimeOffset</span></span>| <span data-ttu-id="b8bcc-149">应将工作分配发布到学生的日期。</span><span class="sxs-lookup"><span data-stu-id="b8bcc-149">Date the assignment should be published to students.</span></span> |
|<span data-ttu-id="b8bcc-150">assignTo</span><span class="sxs-lookup"><span data-stu-id="b8bcc-150">assignTo</span></span>|<span data-ttu-id="b8bcc-151">educationAssignmentRecipient</span><span class="sxs-lookup"><span data-stu-id="b8bcc-151">educationAssignmentRecipient</span></span>| <span data-ttu-id="b8bcc-152">获取工作分配的学生。</span><span class="sxs-lookup"><span data-stu-id="b8bcc-152">Students who get the assignment.</span></span>|
|<span data-ttu-id="b8bcc-153">displayName</span><span class="sxs-lookup"><span data-stu-id="b8bcc-153">displayName</span></span>|<span data-ttu-id="b8bcc-154">字符串</span><span class="sxs-lookup"><span data-stu-id="b8bcc-154">String</span></span>| <span data-ttu-id="b8bcc-155">工作分配的名称。</span><span class="sxs-lookup"><span data-stu-id="b8bcc-155">Name of assignment.</span></span> |
|<span data-ttu-id="b8bcc-156">dueDateTime</span><span class="sxs-lookup"><span data-stu-id="b8bcc-156">dueDateTime</span></span>|<span data-ttu-id="b8bcc-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b8bcc-157">DateTimeOffset</span></span>| <span data-ttu-id="b8bcc-158">截止日期工作分配。</span><span class="sxs-lookup"><span data-stu-id="b8bcc-158">Date assignment is due.</span></span> |
|<span data-ttu-id="b8bcc-159">分级</span><span class="sxs-lookup"><span data-stu-id="b8bcc-159">grading</span></span>|<span data-ttu-id="b8bcc-160">educationAssignmentGradeType</span><span class="sxs-lookup"><span data-stu-id="b8bcc-160">educationAssignmentGradeType</span></span>| <span data-ttu-id="b8bcc-161">如何将评分工作分配。</span><span class="sxs-lookup"><span data-stu-id="b8bcc-161">How the assignment will be graded.</span></span>|
|<span data-ttu-id="b8bcc-162">说明</span><span class="sxs-lookup"><span data-stu-id="b8bcc-162">instructions</span></span>|<span data-ttu-id="b8bcc-163">itemBody</span><span class="sxs-lookup"><span data-stu-id="b8bcc-163">itemBody</span></span>| <span data-ttu-id="b8bcc-164">要赋予以及工作分配学生的说明。</span><span class="sxs-lookup"><span data-stu-id="b8bcc-164">Instructions to be given to the students along with the assignment.</span></span> |

## <a name="response"></a><span data-ttu-id="b8bcc-165">响应</span><span class="sxs-lookup"><span data-stu-id="b8bcc-165">Response</span></span>
<span data-ttu-id="b8bcc-166">如果成功，此方法返回`200 OK`响应代码和响应正文中的更新的[educationAssignment](../resources/educationassignment.md)对象。</span><span class="sxs-lookup"><span data-stu-id="b8bcc-166">If successful, this method returns a `200 OK` response code and an updated [educationAssignment](../resources/educationassignment.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="b8bcc-167">示例</span><span class="sxs-lookup"><span data-stu-id="b8bcc-167">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b8bcc-168">请求</span><span class="sxs-lookup"><span data-stu-id="b8bcc-168">Request</span></span>
<span data-ttu-id="b8bcc-169">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="b8bcc-169">The following is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="b8bcc-170">响应</span><span class="sxs-lookup"><span data-stu-id="b8bcc-170">Response</span></span>
<span data-ttu-id="b8bcc-171">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="b8bcc-171">The following is an example of the response.</span></span> 

><span data-ttu-id="b8bcc-172">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="b8bcc-172">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="b8bcc-173">将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="b8bcc-173">All of the properties will be returned from an actual call.</span></span>

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
  "dueDateTime": "2014-02-01T00:00:00Z",
  "assignDateTime": "2014-01-01T00:00:00Z",
  "assignedDateTime": "2014-01-01T00:00:00Z"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update educationassignment",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->