---
title: educationSubmission 资源类型
description: 提交归工作分配所有。 提交表示单个用户或 (组) 工作分配所需的资源以及返回的成绩/反馈。
author: dipakboyed
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: fccb8c691d5398bd95cc3ebc7eca1fc3028443a5
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/11/2021
ms.locfileid: "50722156"
---
# <a name="educationsubmission-resource-type"></a><span data-ttu-id="6c0cb-104">educationSubmission 资源类型</span><span class="sxs-lookup"><span data-stu-id="6c0cb-104">educationSubmission resource type</span></span>

<span data-ttu-id="6c0cb-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6c0cb-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6c0cb-106">提交归工作分配所有。</span><span class="sxs-lookup"><span data-stu-id="6c0cb-106">Submissions are owned by an assignment.</span></span> <span data-ttu-id="6c0cb-107">提交表示单个 (组) 为作业启用的资源，以及结果 (如成绩或) 与提交关联的反馈。</span><span class="sxs-lookup"><span data-stu-id="6c0cb-107">A submission represents the resources that an individual (or group) turn in for an assignment and the outcomes (such as grades or feedback) that are associated with the submission.</span></span>
<span data-ttu-id="6c0cb-108">发布工作分配时将自动创建提交。</span><span class="sxs-lookup"><span data-stu-id="6c0cb-108">Submissions are automatically created when an assignment is published.</span></span> <span data-ttu-id="6c0cb-109">提交拥有两个资源列表。</span><span class="sxs-lookup"><span data-stu-id="6c0cb-109">The submission owns two lists of resources.</span></span> <span data-ttu-id="6c0cb-110">资源表示用户/组工作区，而提交的资源表示学生已主动启用的资源。</span><span class="sxs-lookup"><span data-stu-id="6c0cb-110">Resources represent the user/groups working area while the submitted resources represent the resources that have actively been turned in by students.</span></span>  

><span data-ttu-id="6c0cb-111">**注意：** 状态为只读，并且对象通过操作在工作流中移动。</span><span class="sxs-lookup"><span data-stu-id="6c0cb-111">**Note:** The status is read-only and the object is moved through the workflow via actions.</span></span> 

## <a name="methods"></a><span data-ttu-id="6c0cb-112">方法</span><span class="sxs-lookup"><span data-stu-id="6c0cb-112">Methods</span></span>

| <span data-ttu-id="6c0cb-113">方法</span><span class="sxs-lookup"><span data-stu-id="6c0cb-113">Method</span></span>           | <span data-ttu-id="6c0cb-114">返回类型</span><span class="sxs-lookup"><span data-stu-id="6c0cb-114">Return Type</span></span>    |<span data-ttu-id="6c0cb-115">说明</span><span class="sxs-lookup"><span data-stu-id="6c0cb-115">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="6c0cb-116">获取 educationSubmission</span><span class="sxs-lookup"><span data-stu-id="6c0cb-116">Get educationSubmission</span></span>](../api/educationsubmission-get.md) | [<span data-ttu-id="6c0cb-117">educationSubmission</span><span class="sxs-lookup"><span data-stu-id="6c0cb-117">educationSubmission</span></span>](educationsubmission.md) |<span data-ttu-id="6c0cb-118">读取 **educationSubmission 对象的属性和** 关系。</span><span class="sxs-lookup"><span data-stu-id="6c0cb-118">Read properties and relationships of an **educationSubmission** object.</span></span>|
|[<span data-ttu-id="6c0cb-119">列出资源</span><span class="sxs-lookup"><span data-stu-id="6c0cb-119">List resources</span></span>](../api/educationsubmission-list-resources.md) |<span data-ttu-id="6c0cb-120">[educationSubmissionResource](educationsubmissionresource.md) 集合</span><span class="sxs-lookup"><span data-stu-id="6c0cb-120">[educationSubmissionResource](educationsubmissionresource.md) collection</span></span>| <span data-ttu-id="6c0cb-121">获取 **educationSubmissionResource** 对象集合。</span><span class="sxs-lookup"><span data-stu-id="6c0cb-121">Get an **educationSubmissionResource** object collection.</span></span>|
|[<span data-ttu-id="6c0cb-122">列出 submittedResources</span><span class="sxs-lookup"><span data-stu-id="6c0cb-122">List submittedResources</span></span>](../api/educationsubmission-list-submittedresources.md) |<span data-ttu-id="6c0cb-123">[educationSubmissionResource](educationsubmissionresource.md) 集合</span><span class="sxs-lookup"><span data-stu-id="6c0cb-123">[educationSubmissionResource](educationsubmissionresource.md) collection</span></span>| <span data-ttu-id="6c0cb-124">获取 **educationSubmissionResource** 对象集合。</span><span class="sxs-lookup"><span data-stu-id="6c0cb-124">Get an **educationSubmissionResource** object collection.</span></span>|
|[<span data-ttu-id="6c0cb-125">列出结果</span><span class="sxs-lookup"><span data-stu-id="6c0cb-125">List outcomes</span></span>](../api/educationsubmission-list-outcomes.md) |<span data-ttu-id="6c0cb-126">[educationOutcome](educationoutcome.md) 集合</span><span class="sxs-lookup"><span data-stu-id="6c0cb-126">[educationOutcome](educationoutcome.md) collection</span></span>| <span data-ttu-id="6c0cb-127">获取 **educationOutcome** 对象集合。</span><span class="sxs-lookup"><span data-stu-id="6c0cb-127">Get an **educationOutcome** object collection.</span></span>|
|[<span data-ttu-id="6c0cb-128">Return</span><span class="sxs-lookup"><span data-stu-id="6c0cb-128">Return</span></span>](../api/educationsubmission-return.md)|[<span data-ttu-id="6c0cb-129">educationSubmission</span><span class="sxs-lookup"><span data-stu-id="6c0cb-129">educationSubmission</span></span>](educationsubmission.md)|<span data-ttu-id="6c0cb-130">教师使用返回指示可以向学生显示成绩/反馈。</span><span class="sxs-lookup"><span data-stu-id="6c0cb-130">A teacher uses return to indicate that the grades/feedback can be shown to the student.</span></span>|
|[<span data-ttu-id="6c0cb-131">Submit</span><span class="sxs-lookup"><span data-stu-id="6c0cb-131">Submit</span></span>](../api/educationsubmission-submit.md)|[<span data-ttu-id="6c0cb-132">educationSubmission</span><span class="sxs-lookup"><span data-stu-id="6c0cb-132">educationSubmission</span></span>](educationsubmission.md)|<span data-ttu-id="6c0cb-133">学生使用提交来提交作业。</span><span class="sxs-lookup"><span data-stu-id="6c0cb-133">A student uses submit to turn in the assignment.</span></span> <span data-ttu-id="6c0cb-134">这会将资源复制到 **submittedResources** 文件夹中进行评分并更新状态。</span><span class="sxs-lookup"><span data-stu-id="6c0cb-134">This will copy the resources into the **submittedResources** folder for grading and updates the status.</span></span>|
|[<span data-ttu-id="6c0cb-135">取消提交</span><span class="sxs-lookup"><span data-stu-id="6c0cb-135">Unsubmit</span></span>](../api/educationsubmission-unsubmit.md)|[<span data-ttu-id="6c0cb-136">educationSubmission</span><span class="sxs-lookup"><span data-stu-id="6c0cb-136">educationSubmission</span></span>](educationsubmission.md)|<span data-ttu-id="6c0cb-137">学生使用取消提交将提交状态从提交状态移回工作状态。</span><span class="sxs-lookup"><span data-stu-id="6c0cb-137">A student uses the unsubmit to move the state of the submission from submitted back to working.</span></span> <span data-ttu-id="6c0cb-138">这会将资源复制到 **workingResources** 文件夹中进行评分并更新状态。</span><span class="sxs-lookup"><span data-stu-id="6c0cb-138">This will copy the resources into the **workingResources** folder for grading and updates the status.</span></span>|

## <a name="properties"></a><span data-ttu-id="6c0cb-139">属性</span><span class="sxs-lookup"><span data-stu-id="6c0cb-139">Properties</span></span>
| <span data-ttu-id="6c0cb-140">属性</span><span class="sxs-lookup"><span data-stu-id="6c0cb-140">Property</span></span>     | <span data-ttu-id="6c0cb-141">类型</span><span class="sxs-lookup"><span data-stu-id="6c0cb-141">Type</span></span>   |<span data-ttu-id="6c0cb-142">说明</span><span class="sxs-lookup"><span data-stu-id="6c0cb-142">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6c0cb-143">recipient</span><span class="sxs-lookup"><span data-stu-id="6c0cb-143">recipient</span></span>|[<span data-ttu-id="6c0cb-144">educationSubmissionRecipient</span><span class="sxs-lookup"><span data-stu-id="6c0cb-144">educationSubmissionRecipient</span></span>](educationsubmissionrecipient.md)|<span data-ttu-id="6c0cb-145">此提交将分配给谁。</span><span class="sxs-lookup"><span data-stu-id="6c0cb-145">Who this submission is assigned to.</span></span>|
|<span data-ttu-id="6c0cb-146">releasedBy</span><span class="sxs-lookup"><span data-stu-id="6c0cb-146">releasedBy</span></span>|[<span data-ttu-id="6c0cb-147">identitySet</span><span class="sxs-lookup"><span data-stu-id="6c0cb-147">identitySet</span></span>](identityset.md)|<span data-ttu-id="6c0cb-148">将此提交的状态移动到已发布的用户。</span><span class="sxs-lookup"><span data-stu-id="6c0cb-148">User who moved the status of this submission to released.</span></span>|
|<span data-ttu-id="6c0cb-149">releasedDateTime</span><span class="sxs-lookup"><span data-stu-id="6c0cb-149">releasedDateTime</span></span>|<span data-ttu-id="6c0cb-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6c0cb-150">DateTimeOffset</span></span>|<span data-ttu-id="6c0cb-151">提交发布的时间。</span><span class="sxs-lookup"><span data-stu-id="6c0cb-151">Moment in time when the submission was released.</span></span> <span data-ttu-id="6c0cb-152">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="6c0cb-152">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="6c0cb-153">例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`</span><span class="sxs-lookup"><span data-stu-id="6c0cb-153">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="6c0cb-154">returnedBy</span><span class="sxs-lookup"><span data-stu-id="6c0cb-154">returnedBy</span></span>|[<span data-ttu-id="6c0cb-155">identitySet</span><span class="sxs-lookup"><span data-stu-id="6c0cb-155">identitySet</span></span>](identityset.md)|<span data-ttu-id="6c0cb-156">将此提交的状态移动到返回的用户。</span><span class="sxs-lookup"><span data-stu-id="6c0cb-156">User who moved the status of this submission to returned.</span></span>|
|<span data-ttu-id="6c0cb-157">returnedDateTime</span><span class="sxs-lookup"><span data-stu-id="6c0cb-157">returnedDateTime</span></span>|<span data-ttu-id="6c0cb-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6c0cb-158">DateTimeOffset</span></span>|<span data-ttu-id="6c0cb-159">提交返回的时间。</span><span class="sxs-lookup"><span data-stu-id="6c0cb-159">Moment in time when the submission was returned.</span></span> <span data-ttu-id="6c0cb-160">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="6c0cb-160">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="6c0cb-161">例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`</span><span class="sxs-lookup"><span data-stu-id="6c0cb-161">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="6c0cb-162">resourcesFolderUrl</span><span class="sxs-lookup"><span data-stu-id="6c0cb-162">resourcesFolderUrl</span></span>|<span data-ttu-id="6c0cb-163">String</span><span class="sxs-lookup"><span data-stu-id="6c0cb-163">String</span></span>|<span data-ttu-id="6c0cb-164">需要存储此提交的所有文件资源的文件夹。</span><span class="sxs-lookup"><span data-stu-id="6c0cb-164">Folder where all file resources for this submission need to be stored.</span></span>|
|<span data-ttu-id="6c0cb-165">状态</span><span class="sxs-lookup"><span data-stu-id="6c0cb-165">status</span></span>|<span data-ttu-id="6c0cb-166">string</span><span class="sxs-lookup"><span data-stu-id="6c0cb-166">string</span></span>| <span data-ttu-id="6c0cb-167">只读。</span><span class="sxs-lookup"><span data-stu-id="6c0cb-167">Read-Only.</span></span> <span data-ttu-id="6c0cb-168">可取值为：`working`、`submitted`、`released`、`returned`。</span><span class="sxs-lookup"><span data-stu-id="6c0cb-168">Possible values are: `working`, `submitted`, `released`, `returned`.</span></span>|
|<span data-ttu-id="6c0cb-169">submittedBy</span><span class="sxs-lookup"><span data-stu-id="6c0cb-169">submittedBy</span></span>|[<span data-ttu-id="6c0cb-170">identitySet</span><span class="sxs-lookup"><span data-stu-id="6c0cb-170">identitySet</span></span>](identityset.md)|<span data-ttu-id="6c0cb-171">将资源移动到已提交状态的用户。</span><span class="sxs-lookup"><span data-stu-id="6c0cb-171">User who moved the resource into the submitted state.</span></span>|
|<span data-ttu-id="6c0cb-172">submittedDateTime</span><span class="sxs-lookup"><span data-stu-id="6c0cb-172">submittedDateTime</span></span>|<span data-ttu-id="6c0cb-173">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6c0cb-173">DateTimeOffset</span></span>|<span data-ttu-id="6c0cb-174">提交移动到提交状态的时间。</span><span class="sxs-lookup"><span data-stu-id="6c0cb-174">Moment in time when the submission was moved into the submitted state.</span></span> <span data-ttu-id="6c0cb-175">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="6c0cb-175">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="6c0cb-176">例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`</span><span class="sxs-lookup"><span data-stu-id="6c0cb-176">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="6c0cb-177">unsubmittedBy</span><span class="sxs-lookup"><span data-stu-id="6c0cb-177">unsubmittedBy</span></span>|[<span data-ttu-id="6c0cb-178">identitySet</span><span class="sxs-lookup"><span data-stu-id="6c0cb-178">identitySet</span></span>](identityset.md)|<span data-ttu-id="6c0cb-179">将资源从提交移动到工作状态的用户。</span><span class="sxs-lookup"><span data-stu-id="6c0cb-179">User who moved the resource from submitted into the working state.</span></span>|
|<span data-ttu-id="6c0cb-180">unsubmittedDateTime</span><span class="sxs-lookup"><span data-stu-id="6c0cb-180">unsubmittedDateTime</span></span>|<span data-ttu-id="6c0cb-181">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6c0cb-181">DateTimeOffset</span></span>|<span data-ttu-id="6c0cb-182">将提交从提交移动到工作状态的时间。</span><span class="sxs-lookup"><span data-stu-id="6c0cb-182">Moment in time when the submission was moved from submitted into the working state.</span></span> <span data-ttu-id="6c0cb-183">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="6c0cb-183">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="6c0cb-184">例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`</span><span class="sxs-lookup"><span data-stu-id="6c0cb-184">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|

## <a name="relationships"></a><span data-ttu-id="6c0cb-185">关系</span><span class="sxs-lookup"><span data-stu-id="6c0cb-185">Relationships</span></span>
| <span data-ttu-id="6c0cb-186">关系</span><span class="sxs-lookup"><span data-stu-id="6c0cb-186">Relationship</span></span> | <span data-ttu-id="6c0cb-187">类型</span><span class="sxs-lookup"><span data-stu-id="6c0cb-187">Type</span></span>   |<span data-ttu-id="6c0cb-188">说明</span><span class="sxs-lookup"><span data-stu-id="6c0cb-188">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6c0cb-189">resources</span><span class="sxs-lookup"><span data-stu-id="6c0cb-189">resources</span></span>|<span data-ttu-id="6c0cb-190">[educationSubmissionResource](educationsubmissionresource.md) 集合</span><span class="sxs-lookup"><span data-stu-id="6c0cb-190">[educationSubmissionResource](educationsubmissionresource.md) collection</span></span>| <span data-ttu-id="6c0cb-191">可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="6c0cb-191">Nullable.</span></span>|
|<span data-ttu-id="6c0cb-192">submittedResources</span><span class="sxs-lookup"><span data-stu-id="6c0cb-192">submittedResources</span></span>|<span data-ttu-id="6c0cb-193">[educationSubmissionResource](educationsubmissionresource.md) 集合</span><span class="sxs-lookup"><span data-stu-id="6c0cb-193">[educationSubmissionResource](educationsubmissionresource.md) collection</span></span>| <span data-ttu-id="6c0cb-194">只读。</span><span class="sxs-lookup"><span data-stu-id="6c0cb-194">Read-only.</span></span> <span data-ttu-id="6c0cb-195">可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="6c0cb-195">Nullable.</span></span>|
|<span data-ttu-id="6c0cb-196">outcomes</span><span class="sxs-lookup"><span data-stu-id="6c0cb-196">outcomes</span></span>|<span data-ttu-id="6c0cb-197">[educationOutcome](educationOutcome.md) 集合。</span><span class="sxs-lookup"><span data-stu-id="6c0cb-197">[educationOutcome](educationOutcome.md) collection.</span></span> <span data-ttu-id="6c0cb-198">保留教师分配给此提交的成绩、反馈和/或评分标准信息</span><span class="sxs-lookup"><span data-stu-id="6c0cb-198">Holds grades, feedback and/or rubrics information the teacher assigns to this submission</span></span>|<span data-ttu-id="6c0cb-199">读/写。</span><span class="sxs-lookup"><span data-stu-id="6c0cb-199">Read-Write.</span></span> <span data-ttu-id="6c0cb-200">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="6c0cb-200">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="6c0cb-201">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6c0cb-201">JSON representation</span></span>

<span data-ttu-id="6c0cb-202">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6c0cb-202">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationSubmission"
}-->

```json
{
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


