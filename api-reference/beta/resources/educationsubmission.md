---
title: educationSubmission 资源类型
description: 提交由工作分配拥有。 提交表示个人 (或组) 在工作分配和返回的评分/反馈中打开的资源。
author: dipakboyed
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 27467548339dc01f7c95fe55bda159c0569c38ba
ms.sourcegitcommit: 129e58f83fc566f9d9f36e26b0c0b8cdf81d27d9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/03/2019
ms.locfileid: "36173039"
---
# <a name="educationsubmission-resource-type"></a><span data-ttu-id="52474-104">educationSubmission 资源类型</span><span class="sxs-lookup"><span data-stu-id="52474-104">educationSubmission resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="52474-105">提交由工作分配拥有。</span><span class="sxs-lookup"><span data-stu-id="52474-105">Submissions are owned by an assignment.</span></span> <span data-ttu-id="52474-106">提交表示个人 (或组) 在工作分配和返回的评分/反馈中打开的资源。</span><span class="sxs-lookup"><span data-stu-id="52474-106">A submission represents the resources that an individual (or group) turn in for an assignment and the grade/feedback that is returned.</span></span>
<span data-ttu-id="52474-107">发布工作分配时, 将自动创建提交。</span><span class="sxs-lookup"><span data-stu-id="52474-107">Submissions are automatically created when an assignment is published.</span></span> <span data-ttu-id="52474-108">提交内容拥有两个资源列表。</span><span class="sxs-lookup"><span data-stu-id="52474-108">The submission owns two lists of resources.</span></span> <span data-ttu-id="52474-109">资源表示用户/组工作区, 而提交的资源代表学生已处于活动状态的资源。</span><span class="sxs-lookup"><span data-stu-id="52474-109">Resources represent the user/groups working area while the submitted resources represent the resources that have actively been turned in by students.</span></span>  

><span data-ttu-id="52474-110">**注意:** 状态为只读, 该对象通过操作在工作流中移动。</span><span class="sxs-lookup"><span data-stu-id="52474-110">**Note:** The status is read-only and the object is moved through the workflow via actions.</span></span> 

## <a name="methods"></a><span data-ttu-id="52474-111">方法</span><span class="sxs-lookup"><span data-stu-id="52474-111">Methods</span></span>

| <span data-ttu-id="52474-112">方法</span><span class="sxs-lookup"><span data-stu-id="52474-112">Method</span></span>           | <span data-ttu-id="52474-113">返回类型</span><span class="sxs-lookup"><span data-stu-id="52474-113">Return Type</span></span>    |<span data-ttu-id="52474-114">说明</span><span class="sxs-lookup"><span data-stu-id="52474-114">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="52474-115">获取 educationSubmission</span><span class="sxs-lookup"><span data-stu-id="52474-115">Get educationSubmission</span></span>](../api/educationsubmission-get.md) | [<span data-ttu-id="52474-116">educationSubmission</span><span class="sxs-lookup"><span data-stu-id="52474-116">educationSubmission</span></span>](educationsubmission.md) |<span data-ttu-id="52474-117">读取**educationSubmission**对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="52474-117">Read properties and relationships of an **educationSubmission** object.</span></span>|
|[<span data-ttu-id="52474-118">列出资源</span><span class="sxs-lookup"><span data-stu-id="52474-118">List resources</span></span>](../api/educationsubmission-list-resources.md) |<span data-ttu-id="52474-119">[educationSubmissionResource](educationsubmissionresource.md)集合</span><span class="sxs-lookup"><span data-stu-id="52474-119">[educationSubmissionResource](educationsubmissionresource.md) collection</span></span>| <span data-ttu-id="52474-120">获取**educationSubmissionResource**对象集合。</span><span class="sxs-lookup"><span data-stu-id="52474-120">Get an **educationSubmissionResource** object collection.</span></span>|
|[<span data-ttu-id="52474-121">列出 submittedResources</span><span class="sxs-lookup"><span data-stu-id="52474-121">List submittedResources</span></span>](../api/educationsubmission-list-submittedresources.md) |<span data-ttu-id="52474-122">[educationSubmissionResource](educationsubmissionresource.md)集合</span><span class="sxs-lookup"><span data-stu-id="52474-122">[educationSubmissionResource](educationsubmissionresource.md) collection</span></span>| <span data-ttu-id="52474-123">获取**educationSubmissionResource**对象集合。</span><span class="sxs-lookup"><span data-stu-id="52474-123">Get an **educationSubmissionResource** object collection.</span></span>|
|[<span data-ttu-id="52474-124">列表结果</span><span class="sxs-lookup"><span data-stu-id="52474-124">List outcomes</span></span>](../api/educationsubmission-list-outcomes.md) |<span data-ttu-id="52474-125">[educationOutcome](educationoutcome.md)集合</span><span class="sxs-lookup"><span data-stu-id="52474-125">[educationOutcome](educationoutcome.md) collection</span></span>| <span data-ttu-id="52474-126">获取**educationOutcome**对象集合。</span><span class="sxs-lookup"><span data-stu-id="52474-126">Get an **educationOutcome** object collection.</span></span>|
|[<span data-ttu-id="52474-127">更新</span><span class="sxs-lookup"><span data-stu-id="52474-127">Update</span></span>](../api/educationsubmission-update.md) | [<span data-ttu-id="52474-128">educationSubmission</span><span class="sxs-lookup"><span data-stu-id="52474-128">educationSubmission</span></span>](educationsubmission.md) |<span data-ttu-id="52474-129">更新**educationSubmission**对象。</span><span class="sxs-lookup"><span data-stu-id="52474-129">Update an **educationSubmission** object.</span></span> |
|[<span data-ttu-id="52474-130">Return</span><span class="sxs-lookup"><span data-stu-id="52474-130">Return</span></span>](../api/educationsubmission-return.md)|[<span data-ttu-id="52474-131">educationSubmission</span><span class="sxs-lookup"><span data-stu-id="52474-131">educationSubmission</span></span>](educationsubmission.md)|<span data-ttu-id="52474-132">教师使用 return 来表示可以向学生显示成绩/反馈。</span><span class="sxs-lookup"><span data-stu-id="52474-132">A teacher uses return to indicate that the grades/feedback can be shown to the student.</span></span>|
|[<span data-ttu-id="52474-133">Submit</span><span class="sxs-lookup"><span data-stu-id="52474-133">Submit</span></span>](../api/educationsubmission-submit.md)|[<span data-ttu-id="52474-134">educationSubmission</span><span class="sxs-lookup"><span data-stu-id="52474-134">educationSubmission</span></span>](educationsubmission.md)|<span data-ttu-id="52474-135">学生使用提交来打开工作分配。</span><span class="sxs-lookup"><span data-stu-id="52474-135">A student uses submit to turn in the assignment.</span></span> <span data-ttu-id="52474-136">这将把资源复制到**submittedResources**文件夹进行评分并更新状态。</span><span class="sxs-lookup"><span data-stu-id="52474-136">This will copy the resources into the **submittedResources** folder for grading and updates the status.</span></span>|
|[<span data-ttu-id="52474-137">Unsubmit</span><span class="sxs-lookup"><span data-stu-id="52474-137">Unsubmit</span></span>](../api/educationsubmission-unsubmit.md)|[<span data-ttu-id="52474-138">educationSubmission</span><span class="sxs-lookup"><span data-stu-id="52474-138">educationSubmission</span></span>](educationsubmission.md)|<span data-ttu-id="52474-139">学生使用 unsubmit 将提交状态移动回 "正在运行"。</span><span class="sxs-lookup"><span data-stu-id="52474-139">A student uses the unsubmit to move the state of the submission from submitted back to working.</span></span> <span data-ttu-id="52474-140">这将把资源复制到**workingResources**文件夹进行评分并更新状态。</span><span class="sxs-lookup"><span data-stu-id="52474-140">This will copy the resources into the **workingResources** folder for grading and updates the status.</span></span>|

## <a name="properties"></a><span data-ttu-id="52474-141">属性</span><span class="sxs-lookup"><span data-stu-id="52474-141">Properties</span></span>
| <span data-ttu-id="52474-142">属性</span><span class="sxs-lookup"><span data-stu-id="52474-142">Property</span></span>     | <span data-ttu-id="52474-143">类型</span><span class="sxs-lookup"><span data-stu-id="52474-143">Type</span></span>   |<span data-ttu-id="52474-144">说明</span><span class="sxs-lookup"><span data-stu-id="52474-144">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="52474-145">反馈</span><span class="sxs-lookup"><span data-stu-id="52474-145">feedback</span></span>|[<span data-ttu-id="52474-146">educationFeedback</span><span class="sxs-lookup"><span data-stu-id="52474-146">educationFeedback</span></span>](educationfeedback.md)|<span data-ttu-id="52474-147">保留反馈属性, 该属性将教师的备注存储回学生。</span><span class="sxs-lookup"><span data-stu-id="52474-147">Holds the feedback property which stores the teacher's notes back to students.</span></span>|
|<span data-ttu-id="52474-148">grade</span><span class="sxs-lookup"><span data-stu-id="52474-148">grade</span></span>|[<span data-ttu-id="52474-149">educationAssignmentGrade</span><span class="sxs-lookup"><span data-stu-id="52474-149">educationAssignmentGrade</span></span>](educationassignmentgrade.md)|<span data-ttu-id="52474-150">保留教师为此提交分配的年级信息。</span><span class="sxs-lookup"><span data-stu-id="52474-150">Holds the grade information a teacher assigns to this submission.</span></span>|
|<span data-ttu-id="52474-151">id</span><span class="sxs-lookup"><span data-stu-id="52474-151">id</span></span>|<span data-ttu-id="52474-152">String</span><span class="sxs-lookup"><span data-stu-id="52474-152">String</span></span>| <span data-ttu-id="52474-153">只读。</span><span class="sxs-lookup"><span data-stu-id="52474-153">Read-only.</span></span>|
|<span data-ttu-id="52474-154">recipient</span><span class="sxs-lookup"><span data-stu-id="52474-154">recipient</span></span>|[<span data-ttu-id="52474-155">educationSubmissionRecipient</span><span class="sxs-lookup"><span data-stu-id="52474-155">educationSubmissionRecipient</span></span>](educationsubmissionrecipient.md)|<span data-ttu-id="52474-156">此提交被分配到的所有者。</span><span class="sxs-lookup"><span data-stu-id="52474-156">Who this submission is assigned to.</span></span>|
|<span data-ttu-id="52474-157">releasedBy</span><span class="sxs-lookup"><span data-stu-id="52474-157">releasedBy</span></span>|[<span data-ttu-id="52474-158">identitySet</span><span class="sxs-lookup"><span data-stu-id="52474-158">identitySet</span></span>](identityset.md)|<span data-ttu-id="52474-159">将此提交的状态移动到 "已发布" 的用户。</span><span class="sxs-lookup"><span data-stu-id="52474-159">User who moved the status of this submission to released.</span></span>|
|<span data-ttu-id="52474-160">releasedDateTime</span><span class="sxs-lookup"><span data-stu-id="52474-160">releasedDateTime</span></span>|<span data-ttu-id="52474-161">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="52474-161">DateTimeOffset</span></span>|<span data-ttu-id="52474-162">提交发布的时间。</span><span class="sxs-lookup"><span data-stu-id="52474-162">Moment in time when the submission was released.</span></span> <span data-ttu-id="52474-163">时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="52474-163">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="52474-164">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="52474-164">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="52474-165">returnedBy</span><span class="sxs-lookup"><span data-stu-id="52474-165">returnedBy</span></span>|[<span data-ttu-id="52474-166">identitySet</span><span class="sxs-lookup"><span data-stu-id="52474-166">identitySet</span></span>](identityset.md)|<span data-ttu-id="52474-167">将此提交的状态移动到 "已返回" 的用户。</span><span class="sxs-lookup"><span data-stu-id="52474-167">User who moved the status of this submission to returned.</span></span>|
|<span data-ttu-id="52474-168">returnedDateTime</span><span class="sxs-lookup"><span data-stu-id="52474-168">returnedDateTime</span></span>|<span data-ttu-id="52474-169">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="52474-169">DateTimeOffset</span></span>|<span data-ttu-id="52474-170">返回提交的时间点。</span><span class="sxs-lookup"><span data-stu-id="52474-170">Moment in time when the submission was returned.</span></span> <span data-ttu-id="52474-171">时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="52474-171">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="52474-172">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="52474-172">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="52474-173">resourcesFolderUrl</span><span class="sxs-lookup"><span data-stu-id="52474-173">resourcesFolderUrl</span></span>|<span data-ttu-id="52474-174">String</span><span class="sxs-lookup"><span data-stu-id="52474-174">String</span></span>|<span data-ttu-id="52474-175">需要存储此提交的所有文件资源的文件夹。</span><span class="sxs-lookup"><span data-stu-id="52474-175">Folder where all file resources for this submission need to be stored.</span></span>|
|<span data-ttu-id="52474-176">状态</span><span class="sxs-lookup"><span data-stu-id="52474-176">status</span></span>|<span data-ttu-id="52474-177">string</span><span class="sxs-lookup"><span data-stu-id="52474-177">string</span></span>| <span data-ttu-id="52474-178">只读。</span><span class="sxs-lookup"><span data-stu-id="52474-178">Read-Only.</span></span> <span data-ttu-id="52474-179">可取值为：`working`、`submitted`、`released`、`returned`。</span><span class="sxs-lookup"><span data-stu-id="52474-179">Possible values are: `working`, `submitted`, `released`, `returned`.</span></span>|
|<span data-ttu-id="52474-180">submittedBy</span><span class="sxs-lookup"><span data-stu-id="52474-180">submittedBy</span></span>|[<span data-ttu-id="52474-181">identitySet</span><span class="sxs-lookup"><span data-stu-id="52474-181">identitySet</span></span>](identityset.md)|<span data-ttu-id="52474-182">将资源移动到已提交状态的用户。</span><span class="sxs-lookup"><span data-stu-id="52474-182">User who moved the resource into the submitted state.</span></span>|
|<span data-ttu-id="52474-183">submittedDateTime</span><span class="sxs-lookup"><span data-stu-id="52474-183">submittedDateTime</span></span>|<span data-ttu-id="52474-184">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="52474-184">DateTimeOffset</span></span>|<span data-ttu-id="52474-185">将提交状态移至提交状态的时间点。</span><span class="sxs-lookup"><span data-stu-id="52474-185">Moment in time when the submission was moved into the submitted state.</span></span> <span data-ttu-id="52474-186">时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="52474-186">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="52474-187">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="52474-187">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="52474-188">unsubmittedBy</span><span class="sxs-lookup"><span data-stu-id="52474-188">unsubmittedBy</span></span>|[<span data-ttu-id="52474-189">identitySet</span><span class="sxs-lookup"><span data-stu-id="52474-189">identitySet</span></span>](identityset.md)|<span data-ttu-id="52474-190">移动资源的用户被提交到工作状态。</span><span class="sxs-lookup"><span data-stu-id="52474-190">User who moved the resource from submitted into the working state.</span></span>|
|<span data-ttu-id="52474-191">unsubmittedDateTime</span><span class="sxs-lookup"><span data-stu-id="52474-191">unsubmittedDateTime</span></span>|<span data-ttu-id="52474-192">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="52474-192">DateTimeOffset</span></span>|<span data-ttu-id="52474-193">将提交的提交时间从提交到工作状态的时刻。</span><span class="sxs-lookup"><span data-stu-id="52474-193">Moment in time when the submission was moved from submitted into the working state.</span></span> <span data-ttu-id="52474-194">时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="52474-194">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="52474-195">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="52474-195">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|

## <a name="relationships"></a><span data-ttu-id="52474-196">关系</span><span class="sxs-lookup"><span data-stu-id="52474-196">Relationships</span></span>
| <span data-ttu-id="52474-197">关系</span><span class="sxs-lookup"><span data-stu-id="52474-197">Relationship</span></span> | <span data-ttu-id="52474-198">类型</span><span class="sxs-lookup"><span data-stu-id="52474-198">Type</span></span>   |<span data-ttu-id="52474-199">说明</span><span class="sxs-lookup"><span data-stu-id="52474-199">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="52474-200">resources</span><span class="sxs-lookup"><span data-stu-id="52474-200">resources</span></span>|<span data-ttu-id="52474-201">[educationSubmissionResource](educationsubmissionresource.md)集合</span><span class="sxs-lookup"><span data-stu-id="52474-201">[educationSubmissionResource](educationsubmissionresource.md) collection</span></span>| <span data-ttu-id="52474-202">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="52474-202">Nullable.</span></span>|
|<span data-ttu-id="52474-203">submittedResources</span><span class="sxs-lookup"><span data-stu-id="52474-203">submittedResources</span></span>|<span data-ttu-id="52474-204">[educationSubmissionResource](educationsubmissionresource.md)集合</span><span class="sxs-lookup"><span data-stu-id="52474-204">[educationSubmissionResource](educationsubmissionresource.md) collection</span></span>| <span data-ttu-id="52474-205">只读。</span><span class="sxs-lookup"><span data-stu-id="52474-205">Read-only.</span></span> <span data-ttu-id="52474-206">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="52474-206">Nullable.</span></span>|
|<span data-ttu-id="52474-207">成果</span><span class="sxs-lookup"><span data-stu-id="52474-207">outcomes</span></span>|<span data-ttu-id="52474-208">[educationOutcome](educationOutcome.md)集合</span><span class="sxs-lookup"><span data-stu-id="52474-208">[educationOutcome](educationOutcome.md) collection</span></span>|<span data-ttu-id="52474-p111">只读。可为空。</span><span class="sxs-lookup"><span data-stu-id="52474-p111">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="52474-211">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="52474-211">JSON representation</span></span>

<span data-ttu-id="52474-212">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="52474-212">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationSubmission"
}-->

```json
{
    "feedback":{"@odata.type":"microsoft.graph.educationFeedback"},
    "grade":{"@odata.type":"microsoft.graph.educationAssignmentGrade"},
    "id":"String (identifier)",
    "recipient":{"@odata.type":"microsoft.graph.educationSubmissionRecipient"},
    "returnedBy":{"@odata.type":"microsoft.graph.identitySet"},
    "returnedDateTime":"String (timestamp)",
    "resourcesFolderUrl":"String",
    "status":"string",
    "submittedBy":{"@odata.type":"microsoft.graph.identitySet"},
    "submittedDateTime":"String (timestamp)",
    "unsubmittedBy":{"@odata.type":"microsoft.graph.identitySet"},
    "unsubmittedDateTime":"String (timestamp)",
    "releasedBy":{"@odata.type":"microsoft.graph.identitySet"},
    "releasedDateTime":"String (timestamp)"
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
  "suppressions": []
}
-->
