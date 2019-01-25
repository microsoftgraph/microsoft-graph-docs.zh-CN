---
title: 更新 educationassignment
description: 更新的 assignment 对象。 仅教师类中的可以执行此操作。 请注意，您无法使用 PATCH 请求更改的工作分配状态。 使用发布操作更改的工作分配状态。
localization_priority: Normal
author: dipakboyed
ms.prod: education
ms.openlocfilehash: eb5762f86e1572f9a9d5876199c945154a25293b
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29524959"
---
# <a name="update-educationassignment"></a><span data-ttu-id="c5a5e-106">更新 educationassignment</span><span class="sxs-lookup"><span data-stu-id="c5a5e-106">Update educationassignment</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c5a5e-107">更新的 assignment 对象。</span><span class="sxs-lookup"><span data-stu-id="c5a5e-107">Update the assignment object.</span></span> <span data-ttu-id="c5a5e-108">仅教师类中的可以执行此操作。</span><span class="sxs-lookup"><span data-stu-id="c5a5e-108">Only teachers in the class can do this.</span></span> <span data-ttu-id="c5a5e-109">请注意，您无法使用 PATCH 请求更改的工作分配状态。</span><span class="sxs-lookup"><span data-stu-id="c5a5e-109">Note that you can't use a PATCH request to change the status of an assignment.</span></span> <span data-ttu-id="c5a5e-110">使用[发布](../api/educationassignment-publish.md)操作更改的工作分配状态。</span><span class="sxs-lookup"><span data-stu-id="c5a5e-110">Use the [publish](../api/educationassignment-publish.md) action to change the assignment status.</span></span>

## <a name="permissions"></a><span data-ttu-id="c5a5e-111">权限</span><span class="sxs-lookup"><span data-stu-id="c5a5e-111">Permissions</span></span>
<span data-ttu-id="c5a5e-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c5a5e-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c5a5e-114">权限类型</span><span class="sxs-lookup"><span data-stu-id="c5a5e-114">Permission type</span></span>      | <span data-ttu-id="c5a5e-115">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c5a5e-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c5a5e-116">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c5a5e-116">Delegated (work or school account)</span></span> |  <span data-ttu-id="c5a5e-117">EduAssignments.ReadWriteBasic EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c5a5e-117">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="c5a5e-118">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c5a5e-118">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="c5a5e-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="c5a5e-119">Not supported.</span></span>  |
|<span data-ttu-id="c5a5e-120">应用程序</span><span class="sxs-lookup"><span data-stu-id="c5a5e-120">Application</span></span> | <span data-ttu-id="c5a5e-121">不支持。</span><span class="sxs-lookup"><span data-stu-id="c5a5e-121">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="c5a5e-122">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c5a5e-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /education/classes/{id}/assignments/{id}
```
## <a name="request-headers"></a><span data-ttu-id="c5a5e-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="c5a5e-123">Request headers</span></span>
| <span data-ttu-id="c5a5e-124">标头</span><span class="sxs-lookup"><span data-stu-id="c5a5e-124">Header</span></span>       | <span data-ttu-id="c5a5e-125">值</span><span class="sxs-lookup"><span data-stu-id="c5a5e-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="c5a5e-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="c5a5e-126">Authorization</span></span>  | <span data-ttu-id="c5a5e-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="c5a5e-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="c5a5e-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c5a5e-129">Content-Type</span></span>  | <span data-ttu-id="c5a5e-130">application/json</span><span class="sxs-lookup"><span data-stu-id="c5a5e-130">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="c5a5e-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="c5a5e-131">Request body</span></span>
<span data-ttu-id="c5a5e-132">在请求正文中，提供应更新的相关字段的值。</span><span class="sxs-lookup"><span data-stu-id="c5a5e-132">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="c5a5e-133">请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="c5a5e-133">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="c5a5e-134">为了获得最佳性能，请勿加入尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="c5a5e-134">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="c5a5e-135">属性</span><span class="sxs-lookup"><span data-stu-id="c5a5e-135">Property</span></span>     | <span data-ttu-id="c5a5e-136">类型</span><span class="sxs-lookup"><span data-stu-id="c5a5e-136">Type</span></span>   |<span data-ttu-id="c5a5e-137">说明</span><span class="sxs-lookup"><span data-stu-id="c5a5e-137">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c5a5e-138">allowLateSubmissions</span><span class="sxs-lookup"><span data-stu-id="c5a5e-138">allowLateSubmissions</span></span>|<span data-ttu-id="c5a5e-139">Boolean</span><span class="sxs-lookup"><span data-stu-id="c5a5e-139">Boolean</span></span>| <span data-ttu-id="c5a5e-140">是否可以在截止日期之后提交提交。</span><span class="sxs-lookup"><span data-stu-id="c5a5e-140">Whether submissions can be submitted after the due date.</span></span>|
|<span data-ttu-id="c5a5e-141">allowStudentsToAddResourcesToSubmission</span><span class="sxs-lookup"><span data-stu-id="c5a5e-141">allowStudentsToAddResourcesToSubmission</span></span>|<span data-ttu-id="c5a5e-142">Boolean</span><span class="sxs-lookup"><span data-stu-id="c5a5e-142">Boolean</span></span>| <span data-ttu-id="c5a5e-143">是否学生可以将资源添加到提交。</span><span class="sxs-lookup"><span data-stu-id="c5a5e-143">Whether a student can add resources to a submission.</span></span> <span data-ttu-id="c5a5e-144">指示在提交的那些项目是否来自工作分配资源列表。</span><span class="sxs-lookup"><span data-stu-id="c5a5e-144">Indicated whether the only items on the submission came from the assignment resource list.</span></span> |
|<span data-ttu-id="c5a5e-145">assignDateTime</span><span class="sxs-lookup"><span data-stu-id="c5a5e-145">assignDateTime</span></span>|<span data-ttu-id="c5a5e-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c5a5e-146">DateTimeOffset</span></span>| <span data-ttu-id="c5a5e-147">应将工作分配发布到学生的日期。</span><span class="sxs-lookup"><span data-stu-id="c5a5e-147">Date the assignment should be published to students.</span></span> |
|<span data-ttu-id="c5a5e-148">assignTo</span><span class="sxs-lookup"><span data-stu-id="c5a5e-148">assignTo</span></span>|<span data-ttu-id="c5a5e-149">educationAssignmentRecipient</span><span class="sxs-lookup"><span data-stu-id="c5a5e-149">educationAssignmentRecipient</span></span>| <span data-ttu-id="c5a5e-150">获取工作分配的学生。</span><span class="sxs-lookup"><span data-stu-id="c5a5e-150">Students who get the assignment.</span></span>|
|<span data-ttu-id="c5a5e-151">displayName</span><span class="sxs-lookup"><span data-stu-id="c5a5e-151">displayName</span></span>|<span data-ttu-id="c5a5e-152">String</span><span class="sxs-lookup"><span data-stu-id="c5a5e-152">String</span></span>| <span data-ttu-id="c5a5e-153">工作分配的名称。</span><span class="sxs-lookup"><span data-stu-id="c5a5e-153">Name of assignment.</span></span> |
|<span data-ttu-id="c5a5e-154">dueDateTime</span><span class="sxs-lookup"><span data-stu-id="c5a5e-154">dueDateTime</span></span>|<span data-ttu-id="c5a5e-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c5a5e-155">DateTimeOffset</span></span>| <span data-ttu-id="c5a5e-156">截止日期工作分配。</span><span class="sxs-lookup"><span data-stu-id="c5a5e-156">Date assignment is due.</span></span> |
|<span data-ttu-id="c5a5e-157">分级</span><span class="sxs-lookup"><span data-stu-id="c5a5e-157">grading</span></span>|<span data-ttu-id="c5a5e-158">educationAssignmentGradeType</span><span class="sxs-lookup"><span data-stu-id="c5a5e-158">educationAssignmentGradeType</span></span>| <span data-ttu-id="c5a5e-159">如何将评分工作分配。</span><span class="sxs-lookup"><span data-stu-id="c5a5e-159">How the assignment will be graded.</span></span>|
|<span data-ttu-id="c5a5e-160">说明</span><span class="sxs-lookup"><span data-stu-id="c5a5e-160">instructions</span></span>|<span data-ttu-id="c5a5e-161">itemBody</span><span class="sxs-lookup"><span data-stu-id="c5a5e-161">itemBody</span></span>| <span data-ttu-id="c5a5e-162">要赋予以及工作分配学生的说明。</span><span class="sxs-lookup"><span data-stu-id="c5a5e-162">Instructions to be given to the students along with the assignment.</span></span> |

## <a name="response"></a><span data-ttu-id="c5a5e-163">响应</span><span class="sxs-lookup"><span data-stu-id="c5a5e-163">Response</span></span>
<span data-ttu-id="c5a5e-164">如果成功，此方法返回`200 OK`响应代码和响应正文中的更新的[educationAssignment](../resources/educationassignment.md)对象。</span><span class="sxs-lookup"><span data-stu-id="c5a5e-164">If successful, this method returns a `200 OK` response code and an updated [educationAssignment](../resources/educationassignment.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="c5a5e-165">示例</span><span class="sxs-lookup"><span data-stu-id="c5a5e-165">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c5a5e-166">请求</span><span class="sxs-lookup"><span data-stu-id="c5a5e-166">Request</span></span>
<span data-ttu-id="c5a5e-167">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="c5a5e-167">The following is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="c5a5e-168">响应</span><span class="sxs-lookup"><span data-stu-id="c5a5e-168">Response</span></span>
<span data-ttu-id="c5a5e-169">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="c5a5e-169">The following is an example of the response.</span></span> 

><span data-ttu-id="c5a5e-170">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="c5a5e-170">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="c5a5e-171">将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="c5a5e-171">All of the properties will be returned from an actual call.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "Update educationassignment",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/educationassignment-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
