---
title: educationSubmission 资源类型
description: 提交归工作分配。 提交表示的资源的个人 （或组） 打开中的工作分配和返回薪等级/反馈。
author: dipakboyed
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: aeeb1355da2ffcb0ebf561af2ecd15ac93221e26
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29521423"
---
# <a name="educationsubmission-resource-type"></a><span data-ttu-id="350ef-104">educationSubmission 资源类型</span><span class="sxs-lookup"><span data-stu-id="350ef-104">educationSubmission resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="350ef-105">提交归工作分配。</span><span class="sxs-lookup"><span data-stu-id="350ef-105">Submissions are owned by an assignment.</span></span> <span data-ttu-id="350ef-106">提交表示的资源的个人 （或组） 打开中的工作分配和返回薪等级/反馈。</span><span class="sxs-lookup"><span data-stu-id="350ef-106">A submission represents the resources that an individual (or group) turn in for an assignment and the grade/feedback that is returned.</span></span>
<span data-ttu-id="350ef-107">发布工作分配时，会自动创建提交。</span><span class="sxs-lookup"><span data-stu-id="350ef-107">Submissions are automatically created when an assignment is published.</span></span> <span data-ttu-id="350ef-108">提交拥有资源的两个的列表。</span><span class="sxs-lookup"><span data-stu-id="350ef-108">The submission owns two lists of resources.</span></span> <span data-ttu-id="350ef-109">资源表示工作区域时的提交的资源表示主动已打开学生的资源的用户/组。</span><span class="sxs-lookup"><span data-stu-id="350ef-109">Resources represent the user/groups working area while the submitted resources represent the resources that have actively been turned in by students.</span></span>  

><span data-ttu-id="350ef-110">**注意：** 状态是只读的并通过操作在工作流移动对象。</span><span class="sxs-lookup"><span data-stu-id="350ef-110">**Note:** The status is read-only and the object is moved through the workflow via actions.</span></span> 

## <a name="methods"></a><span data-ttu-id="350ef-111">方法</span><span class="sxs-lookup"><span data-stu-id="350ef-111">Methods</span></span>

| <span data-ttu-id="350ef-112">方法</span><span class="sxs-lookup"><span data-stu-id="350ef-112">Method</span></span>           | <span data-ttu-id="350ef-113">返回类型</span><span class="sxs-lookup"><span data-stu-id="350ef-113">Return Type</span></span>    |<span data-ttu-id="350ef-114">说明</span><span class="sxs-lookup"><span data-stu-id="350ef-114">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="350ef-115">获取 educationSubmission</span><span class="sxs-lookup"><span data-stu-id="350ef-115">Get educationSubmission</span></span>](../api/educationsubmission-get.md) | [<span data-ttu-id="350ef-116">educationSubmission</span><span class="sxs-lookup"><span data-stu-id="350ef-116">educationSubmission</span></span>](educationsubmission.md) |<span data-ttu-id="350ef-117">读取属性和**educationSubmission**对象的关系。</span><span class="sxs-lookup"><span data-stu-id="350ef-117">Read properties and relationships of an **educationSubmission** object.</span></span>|
|[<span data-ttu-id="350ef-118">列表资源</span><span class="sxs-lookup"><span data-stu-id="350ef-118">List resources</span></span>](../api/educationsubmission-list-resources.md) |<span data-ttu-id="350ef-119">[educationSubmissionResource](educationsubmissionresource.md)集合</span><span class="sxs-lookup"><span data-stu-id="350ef-119">[educationSubmissionResource](educationsubmissionresource.md) collection</span></span>| <span data-ttu-id="350ef-120">获取**educationSubmissionResource**对象集合。</span><span class="sxs-lookup"><span data-stu-id="350ef-120">Get an **educationSubmissionResource** object collection.</span></span>|
|[<span data-ttu-id="350ef-121">列表 submittedResources</span><span class="sxs-lookup"><span data-stu-id="350ef-121">List submittedResources</span></span>](../api/educationsubmission-list-submittedresources.md) |<span data-ttu-id="350ef-122">[educationSubmissionResource](educationsubmissionresource.md)集合</span><span class="sxs-lookup"><span data-stu-id="350ef-122">[educationSubmissionResource](educationsubmissionresource.md) collection</span></span>| <span data-ttu-id="350ef-123">获取**educationSubmissionResource**对象集合。</span><span class="sxs-lookup"><span data-stu-id="350ef-123">Get an **educationSubmissionResource** object collection.</span></span>|
|[<span data-ttu-id="350ef-124">Update</span><span class="sxs-lookup"><span data-stu-id="350ef-124">Update</span></span>](../api/educationsubmission-update.md) | [<span data-ttu-id="350ef-125">educationSubmission</span><span class="sxs-lookup"><span data-stu-id="350ef-125">educationSubmission</span></span>](educationsubmission.md) |<span data-ttu-id="350ef-126">更新**educationSubmission**对象。</span><span class="sxs-lookup"><span data-stu-id="350ef-126">Update an **educationSubmission** object.</span></span> |
|[<span data-ttu-id="350ef-127">Return</span><span class="sxs-lookup"><span data-stu-id="350ef-127">Return</span></span>](../api/educationsubmission-return.md)|[<span data-ttu-id="350ef-128">educationSubmission</span><span class="sxs-lookup"><span data-stu-id="350ef-128">educationSubmission</span></span>](educationsubmission.md)|<span data-ttu-id="350ef-129">教师使用返回指示可以向学生显示薪等级/反馈。</span><span class="sxs-lookup"><span data-stu-id="350ef-129">A teacher uses return to indicate that the grades/feedback can be shown to the student.</span></span>|
|[<span data-ttu-id="350ef-130">Submit</span><span class="sxs-lookup"><span data-stu-id="350ef-130">Submit</span></span>](../api/educationsubmission-submit.md)|[<span data-ttu-id="350ef-131">educationSubmission</span><span class="sxs-lookup"><span data-stu-id="350ef-131">educationSubmission</span></span>](educationsubmission.md)|<span data-ttu-id="350ef-132">使用提交以分配中启用的学生。</span><span class="sxs-lookup"><span data-stu-id="350ef-132">A student uses submit to turn in the assignment.</span></span> <span data-ttu-id="350ef-133">这会将资源复制到评分的**submittedResources**文件夹，并更新状态。</span><span class="sxs-lookup"><span data-stu-id="350ef-133">This will copy the resources into the **submittedResources** folder for grading and updates the status.</span></span>|
|[<span data-ttu-id="350ef-134">Unsubmit</span><span class="sxs-lookup"><span data-stu-id="350ef-134">Unsubmit</span></span>](../api/educationsubmission-unsubmit.md)|[<span data-ttu-id="350ef-135">educationSubmission</span><span class="sxs-lookup"><span data-stu-id="350ef-135">educationSubmission</span></span>](educationsubmission.md)|<span data-ttu-id="350ef-136">学生使用 unsubmit 将提交的状态从提交后移至工作。</span><span class="sxs-lookup"><span data-stu-id="350ef-136">A student uses the unsubmit to move the state of the submission from submitted back to working.</span></span> <span data-ttu-id="350ef-137">这会将资源复制到评分的**workingResources**文件夹，并更新状态。</span><span class="sxs-lookup"><span data-stu-id="350ef-137">This will copy the resources into the **workingResources** folder for grading and updates the status.</span></span>|

## <a name="properties"></a><span data-ttu-id="350ef-138">属性</span><span class="sxs-lookup"><span data-stu-id="350ef-138">Properties</span></span>
| <span data-ttu-id="350ef-139">属性</span><span class="sxs-lookup"><span data-stu-id="350ef-139">Property</span></span>     | <span data-ttu-id="350ef-140">类型</span><span class="sxs-lookup"><span data-stu-id="350ef-140">Type</span></span>   |<span data-ttu-id="350ef-141">说明</span><span class="sxs-lookup"><span data-stu-id="350ef-141">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="350ef-142">反馈</span><span class="sxs-lookup"><span data-stu-id="350ef-142">feedback</span></span>|[<span data-ttu-id="350ef-143">educationFeedback</span><span class="sxs-lookup"><span data-stu-id="350ef-143">educationFeedback</span></span>](educationfeedback.md)|<span data-ttu-id="350ef-144">保留反馈属性存储回学生教师的注释。</span><span class="sxs-lookup"><span data-stu-id="350ef-144">Holds the feedback property which stores the teacher's notes back to students.</span></span>|
|<span data-ttu-id="350ef-145">grade</span><span class="sxs-lookup"><span data-stu-id="350ef-145">grade</span></span>|[<span data-ttu-id="350ef-146">educationAssignmentGrade</span><span class="sxs-lookup"><span data-stu-id="350ef-146">educationAssignmentGrade</span></span>](educationassignmentgrade.md)|<span data-ttu-id="350ef-147">包含教师将分配给此提交的薪等级信息。</span><span class="sxs-lookup"><span data-stu-id="350ef-147">Holds the grade information a teacher assigns to this submission.</span></span>|
|<span data-ttu-id="350ef-148">id</span><span class="sxs-lookup"><span data-stu-id="350ef-148">id</span></span>|<span data-ttu-id="350ef-149">String</span><span class="sxs-lookup"><span data-stu-id="350ef-149">String</span></span>| <span data-ttu-id="350ef-150">只读。</span><span class="sxs-lookup"><span data-stu-id="350ef-150">Read-only.</span></span>|
|<span data-ttu-id="350ef-151">recipient</span><span class="sxs-lookup"><span data-stu-id="350ef-151">recipient</span></span>|[<span data-ttu-id="350ef-152">educationSubmissionRecipient</span><span class="sxs-lookup"><span data-stu-id="350ef-152">educationSubmissionRecipient</span></span>](educationsubmissionrecipient.md)|<span data-ttu-id="350ef-153">此提交被分配到。</span><span class="sxs-lookup"><span data-stu-id="350ef-153">Who this submission is assigned to.</span></span>|
|<span data-ttu-id="350ef-154">releasedBy</span><span class="sxs-lookup"><span data-stu-id="350ef-154">releasedBy</span></span>|[<span data-ttu-id="350ef-155">identitySet</span><span class="sxs-lookup"><span data-stu-id="350ef-155">identitySet</span></span>](identityset.md)|<span data-ttu-id="350ef-156">移动此提交释放的状态的用户。</span><span class="sxs-lookup"><span data-stu-id="350ef-156">User who moved the status of this submission to released.</span></span>|
|<span data-ttu-id="350ef-157">releasedDateTime</span><span class="sxs-lookup"><span data-stu-id="350ef-157">releasedDateTime</span></span>|<span data-ttu-id="350ef-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="350ef-158">DateTimeOffset</span></span>|<span data-ttu-id="350ef-159">发布提交时时刻。</span><span class="sxs-lookup"><span data-stu-id="350ef-159">Moment in time when the submission was released.</span></span> <span data-ttu-id="350ef-160">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="350ef-160">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="350ef-161">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="350ef-161">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="350ef-162">returnedBy</span><span class="sxs-lookup"><span data-stu-id="350ef-162">returnedBy</span></span>|[<span data-ttu-id="350ef-163">identitySet</span><span class="sxs-lookup"><span data-stu-id="350ef-163">identitySet</span></span>](identityset.md)|<span data-ttu-id="350ef-164">移动此提交返回的状态的用户。</span><span class="sxs-lookup"><span data-stu-id="350ef-164">User who moved the status of this submission to returned.</span></span>|
|<span data-ttu-id="350ef-165">returnedDateTime</span><span class="sxs-lookup"><span data-stu-id="350ef-165">returnedDateTime</span></span>|<span data-ttu-id="350ef-166">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="350ef-166">DateTimeOffset</span></span>|<span data-ttu-id="350ef-167">返回提交了时刻。</span><span class="sxs-lookup"><span data-stu-id="350ef-167">Moment in time when the submission was returned.</span></span> <span data-ttu-id="350ef-168">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="350ef-168">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="350ef-169">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="350ef-169">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="350ef-170">resourcesFolderUrl</span><span class="sxs-lookup"><span data-stu-id="350ef-170">resourcesFolderUrl</span></span>|<span data-ttu-id="350ef-171">String</span><span class="sxs-lookup"><span data-stu-id="350ef-171">String</span></span>|<span data-ttu-id="350ef-172">此提交的所有文件资源都需要存储的文件夹。</span><span class="sxs-lookup"><span data-stu-id="350ef-172">Folder where all file resources for this submission need to be stored.</span></span>|
|<span data-ttu-id="350ef-173">status</span><span class="sxs-lookup"><span data-stu-id="350ef-173">status</span></span>|<span data-ttu-id="350ef-174">string</span><span class="sxs-lookup"><span data-stu-id="350ef-174">string</span></span>| <span data-ttu-id="350ef-175">只读。</span><span class="sxs-lookup"><span data-stu-id="350ef-175">Read-Only.</span></span> <span data-ttu-id="350ef-176">可取值为：`working`、`submitted`、`released`、`returned`。</span><span class="sxs-lookup"><span data-stu-id="350ef-176">Possible values are: `working`, `submitted`, `released`, `returned`.</span></span>|
|<span data-ttu-id="350ef-177">submittedBy</span><span class="sxs-lookup"><span data-stu-id="350ef-177">submittedBy</span></span>|[<span data-ttu-id="350ef-178">identitySet</span><span class="sxs-lookup"><span data-stu-id="350ef-178">identitySet</span></span>](identityset.md)|<span data-ttu-id="350ef-179">移至提交状态的资源的用户。</span><span class="sxs-lookup"><span data-stu-id="350ef-179">User who moved the resource into the submitted state.</span></span>|
|<span data-ttu-id="350ef-180">submittedDateTime</span><span class="sxs-lookup"><span data-stu-id="350ef-180">submittedDateTime</span></span>|<span data-ttu-id="350ef-181">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="350ef-181">DateTimeOffset</span></span>|<span data-ttu-id="350ef-182">当提交已移至提交状态时刻。</span><span class="sxs-lookup"><span data-stu-id="350ef-182">Moment in time when the submission was moved into the submitted state.</span></span> <span data-ttu-id="350ef-183">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="350ef-183">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="350ef-184">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="350ef-184">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="350ef-185">unsubmittedBy</span><span class="sxs-lookup"><span data-stu-id="350ef-185">unsubmittedBy</span></span>|[<span data-ttu-id="350ef-186">identitySet</span><span class="sxs-lookup"><span data-stu-id="350ef-186">identitySet</span></span>](identityset.md)|<span data-ttu-id="350ef-187">移动资源的用户从提交到运行状态。</span><span class="sxs-lookup"><span data-stu-id="350ef-187">User who moved the resource from submitted into the working state.</span></span>|
|<span data-ttu-id="350ef-188">unsubmittedDateTime</span><span class="sxs-lookup"><span data-stu-id="350ef-188">unsubmittedDateTime</span></span>|<span data-ttu-id="350ef-189">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="350ef-189">DateTimeOffset</span></span>|<span data-ttu-id="350ef-190">当提交已移动从提交到工作状态时刻。</span><span class="sxs-lookup"><span data-stu-id="350ef-190">Moment in time when the submission was moved from submitted into the working state.</span></span> <span data-ttu-id="350ef-191">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="350ef-191">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="350ef-192">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="350ef-192">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|

## <a name="relationships"></a><span data-ttu-id="350ef-193">关系</span><span class="sxs-lookup"><span data-stu-id="350ef-193">Relationships</span></span>
| <span data-ttu-id="350ef-194">关系</span><span class="sxs-lookup"><span data-stu-id="350ef-194">Relationship</span></span> | <span data-ttu-id="350ef-195">类型</span><span class="sxs-lookup"><span data-stu-id="350ef-195">Type</span></span>   |<span data-ttu-id="350ef-196">说明</span><span class="sxs-lookup"><span data-stu-id="350ef-196">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="350ef-197">resources</span><span class="sxs-lookup"><span data-stu-id="350ef-197">resources</span></span>|<span data-ttu-id="350ef-198">[educationSubmissionResource](educationsubmissionresource.md)集合</span><span class="sxs-lookup"><span data-stu-id="350ef-198">[educationSubmissionResource](educationsubmissionresource.md) collection</span></span>| <span data-ttu-id="350ef-199">可为空。</span><span class="sxs-lookup"><span data-stu-id="350ef-199">Nullable.</span></span>|
|<span data-ttu-id="350ef-200">submittedResources</span><span class="sxs-lookup"><span data-stu-id="350ef-200">submittedResources</span></span>|<span data-ttu-id="350ef-201">[educationSubmissionResource](educationsubmissionresource.md)集合</span><span class="sxs-lookup"><span data-stu-id="350ef-201">[educationSubmissionResource](educationsubmissionresource.md) collection</span></span>| <span data-ttu-id="350ef-p110">只读。可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="350ef-p110">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="350ef-204">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="350ef-204">JSON representation</span></span>

<span data-ttu-id="350ef-205">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="350ef-205">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationSubmission"
}-->

```json
{
  "feedback": {"@odata.type": "microsoft.graph.educationFeedback"},
  "grade": {"@odata.type": "microsoft.graph.educationAssignmentGrade"},
  "id": "String (identifier)",
  "recipient": {"@odata.type": "microsoft.graph.educationSubmissionRecipient"},
  "returnedBy": {"@odata.type": "microsoft.graph.identitySet"},
  "returnedDateTime": "String (timestamp)",
  "resourcesFolderUrl": "String",
  "status": "string",
  "submittedBy": {"@odata.type": "microsoft.graph.identitySet"},
  "submittedDateTime": "String (timestamp)",
  "unsubmittedBy": {"@odata.type": "microsoft.graph.identitySet"},
  "unsubmittedDateTime": "String (timestamp)"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "educationSubmission resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/educationsubmission.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
