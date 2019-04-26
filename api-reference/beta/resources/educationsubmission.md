---
title: educationSubmission 资源类型
description: 提交由工作分配拥有。 提交表示个人 (或组) 在工作分配和返回的评分/反馈中打开的资源。
author: dipakboyed
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 39adc3f394d106860406b3dd22bbf9a1c600280f
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33334126"
---
# <a name="educationsubmission-resource-type"></a><span data-ttu-id="39ffa-104">educationSubmission 资源类型</span><span class="sxs-lookup"><span data-stu-id="39ffa-104">educationSubmission resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="39ffa-105">提交由工作分配拥有。</span><span class="sxs-lookup"><span data-stu-id="39ffa-105">Submissions are owned by an assignment.</span></span> <span data-ttu-id="39ffa-106">提交表示个人 (或组) 在工作分配和返回的评分/反馈中打开的资源。</span><span class="sxs-lookup"><span data-stu-id="39ffa-106">A submission represents the resources that an individual (or group) turn in for an assignment and the grade/feedback that is returned.</span></span>
<span data-ttu-id="39ffa-107">发布工作分配时, 将自动创建提交。</span><span class="sxs-lookup"><span data-stu-id="39ffa-107">Submissions are automatically created when an assignment is published.</span></span> <span data-ttu-id="39ffa-108">提交内容拥有两个资源列表。</span><span class="sxs-lookup"><span data-stu-id="39ffa-108">The submission owns two lists of resources.</span></span> <span data-ttu-id="39ffa-109">资源表示用户/组工作区, 而提交的资源代表学生已处于活动状态的资源。</span><span class="sxs-lookup"><span data-stu-id="39ffa-109">Resources represent the user/groups working area while the submitted resources represent the resources that have actively been turned in by students.</span></span>  

><span data-ttu-id="39ffa-110">**注意:** 状态为只读, 该对象通过操作在工作流中移动。</span><span class="sxs-lookup"><span data-stu-id="39ffa-110">**Note:** The status is read-only and the object is moved through the workflow via actions.</span></span> 

## <a name="methods"></a><span data-ttu-id="39ffa-111">方法</span><span class="sxs-lookup"><span data-stu-id="39ffa-111">Methods</span></span>

| <span data-ttu-id="39ffa-112">方法</span><span class="sxs-lookup"><span data-stu-id="39ffa-112">Method</span></span>           | <span data-ttu-id="39ffa-113">返回类型</span><span class="sxs-lookup"><span data-stu-id="39ffa-113">Return Type</span></span>    |<span data-ttu-id="39ffa-114">说明</span><span class="sxs-lookup"><span data-stu-id="39ffa-114">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="39ffa-115">获取 educationSubmission</span><span class="sxs-lookup"><span data-stu-id="39ffa-115">Get educationSubmission</span></span>](../api/educationsubmission-get.md) | [<span data-ttu-id="39ffa-116">educationSubmission</span><span class="sxs-lookup"><span data-stu-id="39ffa-116">educationSubmission</span></span>](educationsubmission.md) |<span data-ttu-id="39ffa-117">读取**educationSubmission**对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="39ffa-117">Read properties and relationships of an **educationSubmission** object.</span></span>|
|[<span data-ttu-id="39ffa-118">列出资源</span><span class="sxs-lookup"><span data-stu-id="39ffa-118">List resources</span></span>](../api/educationsubmission-list-resources.md) |<span data-ttu-id="39ffa-119">[educationSubmissionResource](educationsubmissionresource.md)集合</span><span class="sxs-lookup"><span data-stu-id="39ffa-119">[educationSubmissionResource](educationsubmissionresource.md) collection</span></span>| <span data-ttu-id="39ffa-120">获取**educationSubmissionResource**对象集合。</span><span class="sxs-lookup"><span data-stu-id="39ffa-120">Get an **educationSubmissionResource** object collection.</span></span>|
|[<span data-ttu-id="39ffa-121">列出 submittedResources</span><span class="sxs-lookup"><span data-stu-id="39ffa-121">List submittedResources</span></span>](../api/educationsubmission-list-submittedresources.md) |<span data-ttu-id="39ffa-122">[educationSubmissionResource](educationsubmissionresource.md)集合</span><span class="sxs-lookup"><span data-stu-id="39ffa-122">[educationSubmissionResource](educationsubmissionresource.md) collection</span></span>| <span data-ttu-id="39ffa-123">获取**educationSubmissionResource**对象集合。</span><span class="sxs-lookup"><span data-stu-id="39ffa-123">Get an **educationSubmissionResource** object collection.</span></span>|
|[<span data-ttu-id="39ffa-124">更新</span><span class="sxs-lookup"><span data-stu-id="39ffa-124">Update</span></span>](../api/educationsubmission-update.md) | [<span data-ttu-id="39ffa-125">educationSubmission</span><span class="sxs-lookup"><span data-stu-id="39ffa-125">educationSubmission</span></span>](educationsubmission.md) |<span data-ttu-id="39ffa-126">更新**educationSubmission**对象。</span><span class="sxs-lookup"><span data-stu-id="39ffa-126">Update an **educationSubmission** object.</span></span> |
|[<span data-ttu-id="39ffa-127">Return</span><span class="sxs-lookup"><span data-stu-id="39ffa-127">Return</span></span>](../api/educationsubmission-return.md)|[<span data-ttu-id="39ffa-128">educationSubmission</span><span class="sxs-lookup"><span data-stu-id="39ffa-128">educationSubmission</span></span>](educationsubmission.md)|<span data-ttu-id="39ffa-129">教师使用 return 来表示可以向学生显示成绩/反馈。</span><span class="sxs-lookup"><span data-stu-id="39ffa-129">A teacher uses return to indicate that the grades/feedback can be shown to the student.</span></span>|
|[<span data-ttu-id="39ffa-130">Submit</span><span class="sxs-lookup"><span data-stu-id="39ffa-130">Submit</span></span>](../api/educationsubmission-submit.md)|[<span data-ttu-id="39ffa-131">educationSubmission</span><span class="sxs-lookup"><span data-stu-id="39ffa-131">educationSubmission</span></span>](educationsubmission.md)|<span data-ttu-id="39ffa-132">学生使用提交来打开工作分配。</span><span class="sxs-lookup"><span data-stu-id="39ffa-132">A student uses submit to turn in the assignment.</span></span> <span data-ttu-id="39ffa-133">这将把资源复制到**submittedResources**文件夹进行评分并更新状态。</span><span class="sxs-lookup"><span data-stu-id="39ffa-133">This will copy the resources into the **submittedResources** folder for grading and updates the status.</span></span>|
|[<span data-ttu-id="39ffa-134">Unsubmit</span><span class="sxs-lookup"><span data-stu-id="39ffa-134">Unsubmit</span></span>](../api/educationsubmission-unsubmit.md)|[<span data-ttu-id="39ffa-135">educationSubmission</span><span class="sxs-lookup"><span data-stu-id="39ffa-135">educationSubmission</span></span>](educationsubmission.md)|<span data-ttu-id="39ffa-136">学生使用 unsubmit 将提交状态移动回 "正在运行"。</span><span class="sxs-lookup"><span data-stu-id="39ffa-136">A student uses the unsubmit to move the state of the submission from submitted back to working.</span></span> <span data-ttu-id="39ffa-137">这将把资源复制到**workingResources**文件夹进行评分并更新状态。</span><span class="sxs-lookup"><span data-stu-id="39ffa-137">This will copy the resources into the **workingResources** folder for grading and updates the status.</span></span>|

## <a name="properties"></a><span data-ttu-id="39ffa-138">属性</span><span class="sxs-lookup"><span data-stu-id="39ffa-138">Properties</span></span>
| <span data-ttu-id="39ffa-139">属性</span><span class="sxs-lookup"><span data-stu-id="39ffa-139">Property</span></span>     | <span data-ttu-id="39ffa-140">类型</span><span class="sxs-lookup"><span data-stu-id="39ffa-140">Type</span></span>   |<span data-ttu-id="39ffa-141">说明</span><span class="sxs-lookup"><span data-stu-id="39ffa-141">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="39ffa-142">征求</span><span class="sxs-lookup"><span data-stu-id="39ffa-142">feedback</span></span>|[<span data-ttu-id="39ffa-143">educationFeedback</span><span class="sxs-lookup"><span data-stu-id="39ffa-143">educationFeedback</span></span>](educationfeedback.md)|<span data-ttu-id="39ffa-144">保留反馈属性, 该属性将教师的备注存储回学生。</span><span class="sxs-lookup"><span data-stu-id="39ffa-144">Holds the feedback property which stores the teacher's notes back to students.</span></span>|
|<span data-ttu-id="39ffa-145">grade</span><span class="sxs-lookup"><span data-stu-id="39ffa-145">grade</span></span>|[<span data-ttu-id="39ffa-146">educationAssignmentGrade</span><span class="sxs-lookup"><span data-stu-id="39ffa-146">educationAssignmentGrade</span></span>](educationassignmentgrade.md)|<span data-ttu-id="39ffa-147">保留教师为此提交分配的年级信息。</span><span class="sxs-lookup"><span data-stu-id="39ffa-147">Holds the grade information a teacher assigns to this submission.</span></span>|
|<span data-ttu-id="39ffa-148">id</span><span class="sxs-lookup"><span data-stu-id="39ffa-148">id</span></span>|<span data-ttu-id="39ffa-149">String</span><span class="sxs-lookup"><span data-stu-id="39ffa-149">String</span></span>| <span data-ttu-id="39ffa-150">只读。</span><span class="sxs-lookup"><span data-stu-id="39ffa-150">Read-only.</span></span>|
|<span data-ttu-id="39ffa-151">recipient</span><span class="sxs-lookup"><span data-stu-id="39ffa-151">recipient</span></span>|[<span data-ttu-id="39ffa-152">educationSubmissionRecipient</span><span class="sxs-lookup"><span data-stu-id="39ffa-152">educationSubmissionRecipient</span></span>](educationsubmissionrecipient.md)|<span data-ttu-id="39ffa-153">此提交被分配到的所有者。</span><span class="sxs-lookup"><span data-stu-id="39ffa-153">Who this submission is assigned to.</span></span>|
|<span data-ttu-id="39ffa-154">releasedBy</span><span class="sxs-lookup"><span data-stu-id="39ffa-154">releasedBy</span></span>|[<span data-ttu-id="39ffa-155">identitySet</span><span class="sxs-lookup"><span data-stu-id="39ffa-155">identitySet</span></span>](identityset.md)|<span data-ttu-id="39ffa-156">将此提交的状态移动到 "已发布" 的用户。</span><span class="sxs-lookup"><span data-stu-id="39ffa-156">User who moved the status of this submission to released.</span></span>|
|<span data-ttu-id="39ffa-157">releasedDateTime</span><span class="sxs-lookup"><span data-stu-id="39ffa-157">releasedDateTime</span></span>|<span data-ttu-id="39ffa-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="39ffa-158">DateTimeOffset</span></span>|<span data-ttu-id="39ffa-159">提交发布的时间。</span><span class="sxs-lookup"><span data-stu-id="39ffa-159">Moment in time when the submission was released.</span></span> <span data-ttu-id="39ffa-160">时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="39ffa-160">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="39ffa-161">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="39ffa-161">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="39ffa-162">returnedBy</span><span class="sxs-lookup"><span data-stu-id="39ffa-162">returnedBy</span></span>|[<span data-ttu-id="39ffa-163">identitySet</span><span class="sxs-lookup"><span data-stu-id="39ffa-163">identitySet</span></span>](identityset.md)|<span data-ttu-id="39ffa-164">将此提交的状态移动到 "已返回" 的用户。</span><span class="sxs-lookup"><span data-stu-id="39ffa-164">User who moved the status of this submission to returned.</span></span>|
|<span data-ttu-id="39ffa-165">returnedDateTime</span><span class="sxs-lookup"><span data-stu-id="39ffa-165">returnedDateTime</span></span>|<span data-ttu-id="39ffa-166">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="39ffa-166">DateTimeOffset</span></span>|<span data-ttu-id="39ffa-167">返回提交的时间点。</span><span class="sxs-lookup"><span data-stu-id="39ffa-167">Moment in time when the submission was returned.</span></span> <span data-ttu-id="39ffa-168">时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="39ffa-168">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="39ffa-169">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="39ffa-169">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="39ffa-170">resourcesFolderUrl</span><span class="sxs-lookup"><span data-stu-id="39ffa-170">resourcesFolderUrl</span></span>|<span data-ttu-id="39ffa-171">String</span><span class="sxs-lookup"><span data-stu-id="39ffa-171">String</span></span>|<span data-ttu-id="39ffa-172">需要存储此提交的所有文件资源的文件夹。</span><span class="sxs-lookup"><span data-stu-id="39ffa-172">Folder where all file resources for this submission need to be stored.</span></span>|
|<span data-ttu-id="39ffa-173">状态</span><span class="sxs-lookup"><span data-stu-id="39ffa-173">status</span></span>|<span data-ttu-id="39ffa-174">string</span><span class="sxs-lookup"><span data-stu-id="39ffa-174">string</span></span>| <span data-ttu-id="39ffa-175">只读。</span><span class="sxs-lookup"><span data-stu-id="39ffa-175">Read-Only.</span></span> <span data-ttu-id="39ffa-176">可取值为：`working`、`submitted`、`released`、`returned`。</span><span class="sxs-lookup"><span data-stu-id="39ffa-176">Possible values are: `working`, `submitted`, `released`, `returned`.</span></span>|
|<span data-ttu-id="39ffa-177">submittedBy</span><span class="sxs-lookup"><span data-stu-id="39ffa-177">submittedBy</span></span>|[<span data-ttu-id="39ffa-178">identitySet</span><span class="sxs-lookup"><span data-stu-id="39ffa-178">identitySet</span></span>](identityset.md)|<span data-ttu-id="39ffa-179">将资源移动到已提交状态的用户。</span><span class="sxs-lookup"><span data-stu-id="39ffa-179">User who moved the resource into the submitted state.</span></span>|
|<span data-ttu-id="39ffa-180">submittedDateTime</span><span class="sxs-lookup"><span data-stu-id="39ffa-180">submittedDateTime</span></span>|<span data-ttu-id="39ffa-181">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="39ffa-181">DateTimeOffset</span></span>|<span data-ttu-id="39ffa-182">将提交状态移至提交状态的时间点。</span><span class="sxs-lookup"><span data-stu-id="39ffa-182">Moment in time when the submission was moved into the submitted state.</span></span> <span data-ttu-id="39ffa-183">时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="39ffa-183">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="39ffa-184">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="39ffa-184">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="39ffa-185">unsubmittedBy</span><span class="sxs-lookup"><span data-stu-id="39ffa-185">unsubmittedBy</span></span>|[<span data-ttu-id="39ffa-186">identitySet</span><span class="sxs-lookup"><span data-stu-id="39ffa-186">identitySet</span></span>](identityset.md)|<span data-ttu-id="39ffa-187">移动资源的用户被提交到工作状态。</span><span class="sxs-lookup"><span data-stu-id="39ffa-187">User who moved the resource from submitted into the working state.</span></span>|
|<span data-ttu-id="39ffa-188">unsubmittedDateTime</span><span class="sxs-lookup"><span data-stu-id="39ffa-188">unsubmittedDateTime</span></span>|<span data-ttu-id="39ffa-189">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="39ffa-189">DateTimeOffset</span></span>|<span data-ttu-id="39ffa-190">将提交的提交时间从提交到工作状态的时刻。</span><span class="sxs-lookup"><span data-stu-id="39ffa-190">Moment in time when the submission was moved from submitted into the working state.</span></span> <span data-ttu-id="39ffa-191">时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="39ffa-191">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="39ffa-192">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="39ffa-192">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|

## <a name="relationships"></a><span data-ttu-id="39ffa-193">关系</span><span class="sxs-lookup"><span data-stu-id="39ffa-193">Relationships</span></span>
| <span data-ttu-id="39ffa-194">关系</span><span class="sxs-lookup"><span data-stu-id="39ffa-194">Relationship</span></span> | <span data-ttu-id="39ffa-195">类型</span><span class="sxs-lookup"><span data-stu-id="39ffa-195">Type</span></span>   |<span data-ttu-id="39ffa-196">说明</span><span class="sxs-lookup"><span data-stu-id="39ffa-196">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="39ffa-197">资源</span><span class="sxs-lookup"><span data-stu-id="39ffa-197">resources</span></span>|<span data-ttu-id="39ffa-198">[educationSubmissionResource](educationsubmissionresource.md)集合</span><span class="sxs-lookup"><span data-stu-id="39ffa-198">[educationSubmissionResource](educationsubmissionresource.md) collection</span></span>| <span data-ttu-id="39ffa-199">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="39ffa-199">Nullable.</span></span>|
|<span data-ttu-id="39ffa-200">submittedResources</span><span class="sxs-lookup"><span data-stu-id="39ffa-200">submittedResources</span></span>|<span data-ttu-id="39ffa-201">[educationSubmissionResource](educationsubmissionresource.md)集合</span><span class="sxs-lookup"><span data-stu-id="39ffa-201">[educationSubmissionResource](educationsubmissionresource.md) collection</span></span>| <span data-ttu-id="39ffa-p110">只读。可为空。</span><span class="sxs-lookup"><span data-stu-id="39ffa-p110">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="39ffa-204">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="39ffa-204">JSON representation</span></span>

<span data-ttu-id="39ffa-205">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="39ffa-205">The following is a JSON representation of the resource.</span></span>

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
