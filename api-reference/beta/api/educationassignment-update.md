---
title: 更新 educationassignment
description: 更新工作分配对象。 只有课堂中的教师才能执行此操作。 请注意, 不能使用 PATCH 请求来更改工作分配的状态。 使用 "发布" 操作可更改工作分配状态。
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 8c3537a6c14e144147f848dc3cd77388387c3765
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35955696"
---
# <a name="update-educationassignment"></a><span data-ttu-id="b19a8-106">更新 educationassignment</span><span class="sxs-lookup"><span data-stu-id="b19a8-106">Update educationassignment</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b19a8-107">更新工作分配对象。</span><span class="sxs-lookup"><span data-stu-id="b19a8-107">Update the assignment object.</span></span> <span data-ttu-id="b19a8-108">只有课堂中的教师才能执行此操作。</span><span class="sxs-lookup"><span data-stu-id="b19a8-108">Only teachers in the class can do this.</span></span> <span data-ttu-id="b19a8-109">请注意, 不能使用 PATCH 请求来更改工作分配的状态。</span><span class="sxs-lookup"><span data-stu-id="b19a8-109">Note that you can't use a PATCH request to change the status of an assignment.</span></span> <span data-ttu-id="b19a8-110">使用 "[发布](../api/educationassignment-publish.md)" 操作可更改工作分配状态。</span><span class="sxs-lookup"><span data-stu-id="b19a8-110">Use the [publish](../api/educationassignment-publish.md) action to change the assignment status.</span></span>

## <a name="permissions"></a><span data-ttu-id="b19a8-111">权限</span><span class="sxs-lookup"><span data-stu-id="b19a8-111">Permissions</span></span>
<span data-ttu-id="b19a8-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b19a8-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b19a8-114">权限类型</span><span class="sxs-lookup"><span data-stu-id="b19a8-114">Permission type</span></span>      | <span data-ttu-id="b19a8-115">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b19a8-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b19a8-116">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b19a8-116">Delegated (work or school account)</span></span> |  <span data-ttu-id="b19a8-117">EduAssignments、ReadWriteBasic、EduAssignments</span><span class="sxs-lookup"><span data-stu-id="b19a8-117">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="b19a8-118">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b19a8-118">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="b19a8-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="b19a8-119">Not supported.</span></span>  |
|<span data-ttu-id="b19a8-120">应用程序</span><span class="sxs-lookup"><span data-stu-id="b19a8-120">Application</span></span> | <span data-ttu-id="b19a8-121">不支持。</span><span class="sxs-lookup"><span data-stu-id="b19a8-121">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="b19a8-122">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b19a8-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /education/classes/{id}/assignments/{id}
```
## <a name="request-headers"></a><span data-ttu-id="b19a8-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="b19a8-123">Request headers</span></span>
| <span data-ttu-id="b19a8-124">标头</span><span class="sxs-lookup"><span data-stu-id="b19a8-124">Header</span></span>       | <span data-ttu-id="b19a8-125">值</span><span class="sxs-lookup"><span data-stu-id="b19a8-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="b19a8-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="b19a8-126">Authorization</span></span>  | <span data-ttu-id="b19a8-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="b19a8-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="b19a8-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b19a8-129">Content-Type</span></span>  | <span data-ttu-id="b19a8-130">application/json</span><span class="sxs-lookup"><span data-stu-id="b19a8-130">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="b19a8-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="b19a8-131">Request body</span></span>
<span data-ttu-id="b19a8-132">在请求正文中，提供应更新的相关字段的值。</span><span class="sxs-lookup"><span data-stu-id="b19a8-132">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="b19a8-133">请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="b19a8-133">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="b19a8-134">为了获得最佳性能，请勿加入尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="b19a8-134">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="b19a8-135">属性</span><span class="sxs-lookup"><span data-stu-id="b19a8-135">Property</span></span>     | <span data-ttu-id="b19a8-136">类型</span><span class="sxs-lookup"><span data-stu-id="b19a8-136">Type</span></span>   |<span data-ttu-id="b19a8-137">说明</span><span class="sxs-lookup"><span data-stu-id="b19a8-137">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b19a8-138">allowLateSubmissions</span><span class="sxs-lookup"><span data-stu-id="b19a8-138">allowLateSubmissions</span></span>|<span data-ttu-id="b19a8-139">Boolean</span><span class="sxs-lookup"><span data-stu-id="b19a8-139">Boolean</span></span>| <span data-ttu-id="b19a8-140">提交在截止日期之后是否可以提交。</span><span class="sxs-lookup"><span data-stu-id="b19a8-140">Whether submissions can be submitted after the due date.</span></span>|
|<span data-ttu-id="b19a8-141">allowStudentsToAddResourcesToSubmission</span><span class="sxs-lookup"><span data-stu-id="b19a8-141">allowStudentsToAddResourcesToSubmission</span></span>|<span data-ttu-id="b19a8-142">Boolean</span><span class="sxs-lookup"><span data-stu-id="b19a8-142">Boolean</span></span>| <span data-ttu-id="b19a8-143">学生是否可以将资源添加到提交。</span><span class="sxs-lookup"><span data-stu-id="b19a8-143">Whether a student can add resources to a submission.</span></span> <span data-ttu-id="b19a8-144">指示提交的唯一项目是否来自工作分配资源列表。</span><span class="sxs-lookup"><span data-stu-id="b19a8-144">Indicated whether the only items on the submission came from the assignment resource list.</span></span> |
|<span data-ttu-id="b19a8-145">assignDateTime</span><span class="sxs-lookup"><span data-stu-id="b19a8-145">assignDateTime</span></span>|<span data-ttu-id="b19a8-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b19a8-146">DateTimeOffset</span></span>| <span data-ttu-id="b19a8-147">应将分配发布给学生的日期。</span><span class="sxs-lookup"><span data-stu-id="b19a8-147">Date the assignment should be published to students.</span></span> |
|<span data-ttu-id="b19a8-148">assignTo</span><span class="sxs-lookup"><span data-stu-id="b19a8-148">assignTo</span></span>|<span data-ttu-id="b19a8-149">educationAssignmentRecipient</span><span class="sxs-lookup"><span data-stu-id="b19a8-149">educationAssignmentRecipient</span></span>| <span data-ttu-id="b19a8-150">获取工作分配的学生。</span><span class="sxs-lookup"><span data-stu-id="b19a8-150">Students who get the assignment.</span></span>|
|<span data-ttu-id="b19a8-151">displayName</span><span class="sxs-lookup"><span data-stu-id="b19a8-151">displayName</span></span>|<span data-ttu-id="b19a8-152">String</span><span class="sxs-lookup"><span data-stu-id="b19a8-152">String</span></span>| <span data-ttu-id="b19a8-153">分配的名称。</span><span class="sxs-lookup"><span data-stu-id="b19a8-153">Name of assignment.</span></span> |
|<span data-ttu-id="b19a8-154">dueDateTime</span><span class="sxs-lookup"><span data-stu-id="b19a8-154">dueDateTime</span></span>|<span data-ttu-id="b19a8-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b19a8-155">DateTimeOffset</span></span>| <span data-ttu-id="b19a8-156">日期工作分配到期。</span><span class="sxs-lookup"><span data-stu-id="b19a8-156">Date assignment is due.</span></span> |
|<span data-ttu-id="b19a8-157">评分</span><span class="sxs-lookup"><span data-stu-id="b19a8-157">grading</span></span>|<span data-ttu-id="b19a8-158">educationAssignmentGradeType</span><span class="sxs-lookup"><span data-stu-id="b19a8-158">educationAssignmentGradeType</span></span>| <span data-ttu-id="b19a8-159">将如何对工作分配进行评分。</span><span class="sxs-lookup"><span data-stu-id="b19a8-159">How the assignment will be graded.</span></span>|
|<span data-ttu-id="b19a8-160">指令</span><span class="sxs-lookup"><span data-stu-id="b19a8-160">instructions</span></span>|<span data-ttu-id="b19a8-161">itemBody</span><span class="sxs-lookup"><span data-stu-id="b19a8-161">itemBody</span></span>| <span data-ttu-id="b19a8-162">向学生分配的说明以及工作分配。</span><span class="sxs-lookup"><span data-stu-id="b19a8-162">Instructions to be given to the students along with the assignment.</span></span> |

## <a name="response"></a><span data-ttu-id="b19a8-163">响应</span><span class="sxs-lookup"><span data-stu-id="b19a8-163">Response</span></span>
<span data-ttu-id="b19a8-164">如果成功, 此方法在响应`200 OK`正文中返回响应代码和更新的[educationAssignment](../resources/educationassignment.md)对象。</span><span class="sxs-lookup"><span data-stu-id="b19a8-164">If successful, this method returns a `200 OK` response code and an updated [educationAssignment](../resources/educationassignment.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="b19a8-165">示例</span><span class="sxs-lookup"><span data-stu-id="b19a8-165">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b19a8-166">请求</span><span class="sxs-lookup"><span data-stu-id="b19a8-166">Request</span></span>
<span data-ttu-id="b19a8-167">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="b19a8-167">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="b19a8-168">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="b19a8-168">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="b19a8-169">C#</span><span class="sxs-lookup"><span data-stu-id="b19a8-169">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-educationassignment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b19a8-170">Javascript</span><span class="sxs-lookup"><span data-stu-id="b19a8-170">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-educationassignment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="b19a8-171">目标-C</span><span class="sxs-lookup"><span data-stu-id="b19a8-171">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-educationassignment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="b19a8-172">Java</span><span class="sxs-lookup"><span data-stu-id="b19a8-172">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-educationassignment-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="b19a8-173">响应</span><span class="sxs-lookup"><span data-stu-id="b19a8-173">Response</span></span>
<span data-ttu-id="b19a8-174">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="b19a8-174">The following is an example of the response.</span></span> 

><span data-ttu-id="b19a8-175">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="b19a8-175">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="b19a8-176">将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="b19a8-176">All of the properties will be returned from an actual call.</span></span>

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
  ]
}
-->
