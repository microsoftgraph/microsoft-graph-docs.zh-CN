---
title: educationSubmission 资源类型
description: 提交归工作分配所有。 提交表示单个用户或 (组) 为作业启用的资源以及返回的成绩/反馈。
author: dipakboyed
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 9450770a78b8effd1ad11717297a7e1ad7e6e874
ms.sourcegitcommit: d700b7e3b411e3226b5adf1f213539f05fe802e8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/19/2021
ms.locfileid: "52547674"
---
# <a name="educationsubmission-resource-type"></a><span data-ttu-id="fe24a-104">educationSubmission 资源类型</span><span class="sxs-lookup"><span data-stu-id="fe24a-104">educationSubmission resource type</span></span>

<span data-ttu-id="fe24a-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fe24a-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fe24a-106">提交表示单个 (或组) 为作业启用的资源，以及 (与提交关联的成绩或) 反馈等结果。</span><span class="sxs-lookup"><span data-stu-id="fe24a-106">A submission represents the resources that an individual (or group) turn in for an assignment and the outcomes (such as grades or feedback) that are associated with the submission.</span></span>

<span data-ttu-id="fe24a-107">提交归工作分配所有。</span><span class="sxs-lookup"><span data-stu-id="fe24a-107">Submissions are owned by an assignment.</span></span> <span data-ttu-id="fe24a-108">发布作业时将自动创建提交。</span><span class="sxs-lookup"><span data-stu-id="fe24a-108">Submissions are automatically created when an assignment is published.</span></span> <span data-ttu-id="fe24a-109">提交拥有两个资源列表。</span><span class="sxs-lookup"><span data-stu-id="fe24a-109">The submission owns two lists of resources.</span></span> <span data-ttu-id="fe24a-110">资源表示用户/组工作区，而提交的资源表示学生已主动启用的资源。</span><span class="sxs-lookup"><span data-stu-id="fe24a-110">Resources represent the user/groups working area while the submitted resources represent the resources that have actively been turned in by students.</span></span>  

<span data-ttu-id="fe24a-111">**status** 属性是只读的，并且对象通过操作在工作流中移动。</span><span class="sxs-lookup"><span data-stu-id="fe24a-111">The **status** property is read-only and the object is moved through the workflow via actions.</span></span> 

<span data-ttu-id="fe24a-112">如果尚未对 **educationSubmission** 资源调用 [setUpResourcesFolder，](../api/educationsubmission-setupResourcesFolder.md)**则 resourcesFolderUrl** 属性为 `null` 。</span><span class="sxs-lookup"><span data-stu-id="fe24a-112">If [setUpResourcesFolder](../api/educationsubmission-setupResourcesFolder.md) has not been called on an **educationSubmission** resource, the **resourcesFolderUrl** property is `null`.</span></span>

## <a name="methods"></a><span data-ttu-id="fe24a-113">方法</span><span class="sxs-lookup"><span data-stu-id="fe24a-113">Methods</span></span>

| <span data-ttu-id="fe24a-114">方法</span><span class="sxs-lookup"><span data-stu-id="fe24a-114">Method</span></span>           | <span data-ttu-id="fe24a-115">返回类型</span><span class="sxs-lookup"><span data-stu-id="fe24a-115">Return Type</span></span>    |<span data-ttu-id="fe24a-116">说明</span><span class="sxs-lookup"><span data-stu-id="fe24a-116">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="fe24a-117">获取 educationSubmission</span><span class="sxs-lookup"><span data-stu-id="fe24a-117">Get educationSubmission</span></span>](../api/educationsubmission-get.md) | [<span data-ttu-id="fe24a-118">educationSubmission</span><span class="sxs-lookup"><span data-stu-id="fe24a-118">educationSubmission</span></span>](educationsubmission.md) |<span data-ttu-id="fe24a-119">读取 **educationSubmission** 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="fe24a-119">Read properties and relationships of an **educationSubmission** object.</span></span>|
|[<span data-ttu-id="fe24a-120">列出资源</span><span class="sxs-lookup"><span data-stu-id="fe24a-120">List resources</span></span>](../api/educationsubmission-list-resources.md) |<span data-ttu-id="fe24a-121">[educationSubmissionResource](educationsubmissionresource.md) 集合</span><span class="sxs-lookup"><span data-stu-id="fe24a-121">[educationSubmissionResource](educationsubmissionresource.md) collection</span></span>| <span data-ttu-id="fe24a-122">获取 **educationSubmissionResource** 对象集合。</span><span class="sxs-lookup"><span data-stu-id="fe24a-122">Get an **educationSubmissionResource** object collection.</span></span>|
|[<span data-ttu-id="fe24a-123">列出 submittedResources</span><span class="sxs-lookup"><span data-stu-id="fe24a-123">List submittedResources</span></span>](../api/educationsubmission-list-submittedresources.md) |<span data-ttu-id="fe24a-124">[educationSubmissionResource](educationsubmissionresource.md) 集合</span><span class="sxs-lookup"><span data-stu-id="fe24a-124">[educationSubmissionResource](educationsubmissionresource.md) collection</span></span>| <span data-ttu-id="fe24a-125">获取 **educationSubmissionResource** 对象集合。</span><span class="sxs-lookup"><span data-stu-id="fe24a-125">Get an **educationSubmissionResource** object collection.</span></span>|
|[<span data-ttu-id="fe24a-126">列出结果</span><span class="sxs-lookup"><span data-stu-id="fe24a-126">List outcomes</span></span>](../api/educationsubmission-list-outcomes.md) |<span data-ttu-id="fe24a-127">[educationOutcome](educationoutcome.md) 集合</span><span class="sxs-lookup"><span data-stu-id="fe24a-127">[educationOutcome](educationoutcome.md) collection</span></span>| <span data-ttu-id="fe24a-128">获取 **educationOutcome** 对象集合。</span><span class="sxs-lookup"><span data-stu-id="fe24a-128">Get an **educationOutcome** object collection.</span></span>|
|[<span data-ttu-id="fe24a-129">return</span><span class="sxs-lookup"><span data-stu-id="fe24a-129">return</span></span>](../api/educationsubmission-return.md)|[<span data-ttu-id="fe24a-130">educationSubmission</span><span class="sxs-lookup"><span data-stu-id="fe24a-130">educationSubmission</span></span>](educationsubmission.md)|<span data-ttu-id="fe24a-131">教师使用返回来指示可以向学生显示成绩/反馈。</span><span class="sxs-lookup"><span data-stu-id="fe24a-131">A teacher uses return to indicate that the grades/feedback can be shown to the student.</span></span>|
|[<span data-ttu-id="fe24a-132">setUpResourcesFolder</span><span class="sxs-lookup"><span data-stu-id="fe24a-132">setUpResourcesFolder</span></span>](../api/educationsubmission-setupResourcesFolder.md) |[<span data-ttu-id="fe24a-133">educationSubmission</span><span class="sxs-lookup"><span data-stu-id="fe24a-133">educationSubmission</span></span>](educationsubmission.md) | <span data-ttu-id="fe24a-134">触发创建 SharePoint 资源文件夹，其中应针对给定提交 (Word、Excel 等) 所有基于文件的资源。</span><span class="sxs-lookup"><span data-stu-id="fe24a-134">Trigger the creation of the SharePoint resource folder where all file-based resources (Word, Excel, and so on) should be uploaded for a given submission.</span></span> |
|[<span data-ttu-id="fe24a-135">提交</span><span class="sxs-lookup"><span data-stu-id="fe24a-135">submit</span></span>](../api/educationsubmission-submit.md)|[<span data-ttu-id="fe24a-136">educationSubmission</span><span class="sxs-lookup"><span data-stu-id="fe24a-136">educationSubmission</span></span>](educationsubmission.md)|<span data-ttu-id="fe24a-137">学生使用 submit 提交提交作业。</span><span class="sxs-lookup"><span data-stu-id="fe24a-137">A student uses submit to turn in the assignment.</span></span> <span data-ttu-id="fe24a-138">这会将资源复制到 **submittedResources** 文件夹中进行评分并更新状态。</span><span class="sxs-lookup"><span data-stu-id="fe24a-138">This will copy the resources into the **submittedResources** folder for grading and updates the status.</span></span>|
|[<span data-ttu-id="fe24a-139">unsubmit</span><span class="sxs-lookup"><span data-stu-id="fe24a-139">unsubmit</span></span>](../api/educationsubmission-unsubmit.md)|[<span data-ttu-id="fe24a-140">educationSubmission</span><span class="sxs-lookup"><span data-stu-id="fe24a-140">educationSubmission</span></span>](educationsubmission.md)|<span data-ttu-id="fe24a-141">学生使用取消提交将提交状态从提交后移回工作。</span><span class="sxs-lookup"><span data-stu-id="fe24a-141">A student uses the unsubmit to move the state of the submission from submitted back to working.</span></span> <span data-ttu-id="fe24a-142">这会将资源复制到 **workingResources** 文件夹中进行评分并更新状态。</span><span class="sxs-lookup"><span data-stu-id="fe24a-142">This will copy the resources into the **workingResources** folder for grading and updates the status.</span></span>|

## <a name="properties"></a><span data-ttu-id="fe24a-143">属性</span><span class="sxs-lookup"><span data-stu-id="fe24a-143">Properties</span></span>
| <span data-ttu-id="fe24a-144">属性</span><span class="sxs-lookup"><span data-stu-id="fe24a-144">Property</span></span>     | <span data-ttu-id="fe24a-145">类型</span><span class="sxs-lookup"><span data-stu-id="fe24a-145">Type</span></span>   |<span data-ttu-id="fe24a-146">说明</span><span class="sxs-lookup"><span data-stu-id="fe24a-146">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fe24a-147">recipient</span><span class="sxs-lookup"><span data-stu-id="fe24a-147">recipient</span></span>|[<span data-ttu-id="fe24a-148">educationSubmissionRecipient</span><span class="sxs-lookup"><span data-stu-id="fe24a-148">educationSubmissionRecipient</span></span>](educationsubmissionrecipient.md)|<span data-ttu-id="fe24a-149">Who分配此提交。</span><span class="sxs-lookup"><span data-stu-id="fe24a-149">Who this submission is assigned to.</span></span>|
|<span data-ttu-id="fe24a-150">releasedBy (已弃) </span><span class="sxs-lookup"><span data-stu-id="fe24a-150">releasedBy (deprecated)</span></span>|[<span data-ttu-id="fe24a-151">identitySet</span><span class="sxs-lookup"><span data-stu-id="fe24a-151">identitySet</span></span>](identityset.md)|<span data-ttu-id="fe24a-152">将此提交的状态移至已发布的用户。</span><span class="sxs-lookup"><span data-stu-id="fe24a-152">User who moved the status of this submission to released.</span></span>|
|<span data-ttu-id="fe24a-153">releasedDateTime (弃用) </span><span class="sxs-lookup"><span data-stu-id="fe24a-153">releasedDateTime (deprecated)</span></span>|<span data-ttu-id="fe24a-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fe24a-154">DateTimeOffset</span></span>|<span data-ttu-id="fe24a-155">发布提交的时间。</span><span class="sxs-lookup"><span data-stu-id="fe24a-155">Moment in time when the submission was released.</span></span> <span data-ttu-id="fe24a-156">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="fe24a-156">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="fe24a-157">例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`</span><span class="sxs-lookup"><span data-stu-id="fe24a-157">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="fe24a-158">returnedBy</span><span class="sxs-lookup"><span data-stu-id="fe24a-158">returnedBy</span></span>|[<span data-ttu-id="fe24a-159">identitySet</span><span class="sxs-lookup"><span data-stu-id="fe24a-159">identitySet</span></span>](identityset.md)|<span data-ttu-id="fe24a-160">将此提交的状态移至已返回的用户。</span><span class="sxs-lookup"><span data-stu-id="fe24a-160">User who moved the status of this submission to returned.</span></span>|
|<span data-ttu-id="fe24a-161">returnedDateTime</span><span class="sxs-lookup"><span data-stu-id="fe24a-161">returnedDateTime</span></span>|<span data-ttu-id="fe24a-162">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fe24a-162">DateTimeOffset</span></span>|<span data-ttu-id="fe24a-163">提交返回的时间。</span><span class="sxs-lookup"><span data-stu-id="fe24a-163">Moment in time when the submission was returned.</span></span> <span data-ttu-id="fe24a-164">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="fe24a-164">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="fe24a-165">例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`</span><span class="sxs-lookup"><span data-stu-id="fe24a-165">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="fe24a-166">resourcesFolderUrl</span><span class="sxs-lookup"><span data-stu-id="fe24a-166">resourcesFolderUrl</span></span>|<span data-ttu-id="fe24a-167">String</span><span class="sxs-lookup"><span data-stu-id="fe24a-167">String</span></span>|<span data-ttu-id="fe24a-168">需要存储此提交的所有文件资源的文件夹。</span><span class="sxs-lookup"><span data-stu-id="fe24a-168">Folder where all file resources for this submission need to be stored.</span></span>|
|<span data-ttu-id="fe24a-169">状态</span><span class="sxs-lookup"><span data-stu-id="fe24a-169">status</span></span>|<span data-ttu-id="fe24a-170">string</span><span class="sxs-lookup"><span data-stu-id="fe24a-170">string</span></span>| <span data-ttu-id="fe24a-171">只读。</span><span class="sxs-lookup"><span data-stu-id="fe24a-171">Read-Only.</span></span> <span data-ttu-id="fe24a-172">可取值为：`working`、`submitted`、`released`、`returned`。</span><span class="sxs-lookup"><span data-stu-id="fe24a-172">Possible values are: `working`, `submitted`, `released`, `returned`.</span></span>|
|<span data-ttu-id="fe24a-173">submittedBy</span><span class="sxs-lookup"><span data-stu-id="fe24a-173">submittedBy</span></span>|[<span data-ttu-id="fe24a-174">identitySet</span><span class="sxs-lookup"><span data-stu-id="fe24a-174">identitySet</span></span>](identityset.md)|<span data-ttu-id="fe24a-175">将资源移动到已提交状态的用户。</span><span class="sxs-lookup"><span data-stu-id="fe24a-175">User who moved the resource into the submitted state.</span></span>|
|<span data-ttu-id="fe24a-176">submittedDateTime</span><span class="sxs-lookup"><span data-stu-id="fe24a-176">submittedDateTime</span></span>|<span data-ttu-id="fe24a-177">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fe24a-177">DateTimeOffset</span></span>|<span data-ttu-id="fe24a-178">提交移动到提交状态的时间。</span><span class="sxs-lookup"><span data-stu-id="fe24a-178">Moment in time when the submission was moved into the submitted state.</span></span> <span data-ttu-id="fe24a-179">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="fe24a-179">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="fe24a-180">例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`</span><span class="sxs-lookup"><span data-stu-id="fe24a-180">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="fe24a-181">unsubmittedBy</span><span class="sxs-lookup"><span data-stu-id="fe24a-181">unsubmittedBy</span></span>|[<span data-ttu-id="fe24a-182">identitySet</span><span class="sxs-lookup"><span data-stu-id="fe24a-182">identitySet</span></span>](identityset.md)|<span data-ttu-id="fe24a-183">将资源从提交移动到工作状态的用户。</span><span class="sxs-lookup"><span data-stu-id="fe24a-183">User who moved the resource from submitted into the working state.</span></span>|
|<span data-ttu-id="fe24a-184">unsubmittedDateTime</span><span class="sxs-lookup"><span data-stu-id="fe24a-184">unsubmittedDateTime</span></span>|<span data-ttu-id="fe24a-185">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fe24a-185">DateTimeOffset</span></span>|<span data-ttu-id="fe24a-186">将提交从提交移动到工作状态的时间。</span><span class="sxs-lookup"><span data-stu-id="fe24a-186">Moment in time when the submission was moved from submitted into the working state.</span></span> <span data-ttu-id="fe24a-187">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="fe24a-187">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="fe24a-188">例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`</span><span class="sxs-lookup"><span data-stu-id="fe24a-188">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|

## <a name="relationships"></a><span data-ttu-id="fe24a-189">关系</span><span class="sxs-lookup"><span data-stu-id="fe24a-189">Relationships</span></span>
| <span data-ttu-id="fe24a-190">关系</span><span class="sxs-lookup"><span data-stu-id="fe24a-190">Relationship</span></span> | <span data-ttu-id="fe24a-191">类型</span><span class="sxs-lookup"><span data-stu-id="fe24a-191">Type</span></span>   |<span data-ttu-id="fe24a-192">说明</span><span class="sxs-lookup"><span data-stu-id="fe24a-192">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fe24a-193">resources</span><span class="sxs-lookup"><span data-stu-id="fe24a-193">resources</span></span>|<span data-ttu-id="fe24a-194">[educationSubmissionResource](educationsubmissionresource.md) 集合</span><span class="sxs-lookup"><span data-stu-id="fe24a-194">[educationSubmissionResource](educationsubmissionresource.md) collection</span></span>| <span data-ttu-id="fe24a-195">可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="fe24a-195">Nullable.</span></span>|
|<span data-ttu-id="fe24a-196">submittedResources</span><span class="sxs-lookup"><span data-stu-id="fe24a-196">submittedResources</span></span>|<span data-ttu-id="fe24a-197">[educationSubmissionResource](educationsubmissionresource.md) 集合</span><span class="sxs-lookup"><span data-stu-id="fe24a-197">[educationSubmissionResource](educationsubmissionresource.md) collection</span></span>| <span data-ttu-id="fe24a-p110">只读。可为 Null。</span><span class="sxs-lookup"><span data-stu-id="fe24a-p110">Read-only. Nullable.</span></span>|
|<span data-ttu-id="fe24a-200">outcomes</span><span class="sxs-lookup"><span data-stu-id="fe24a-200">outcomes</span></span>|<span data-ttu-id="fe24a-201">[educationOutcome](educationOutcome.md) 集合。</span><span class="sxs-lookup"><span data-stu-id="fe24a-201">[educationOutcome](educationOutcome.md) collection.</span></span> <span data-ttu-id="fe24a-202">保留教师分配给此提交的成绩、反馈和/或评分标准信息</span><span class="sxs-lookup"><span data-stu-id="fe24a-202">Holds grades, feedback and/or rubrics information the teacher assigns to this submission</span></span>|<span data-ttu-id="fe24a-203">读写。</span><span class="sxs-lookup"><span data-stu-id="fe24a-203">Read-Write.</span></span> <span data-ttu-id="fe24a-204">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="fe24a-204">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="fe24a-205">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="fe24a-205">JSON representation</span></span>

<span data-ttu-id="fe24a-206">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="fe24a-206">The following is a JSON representation of the resource.</span></span>

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
    "unsubmittedDateTime":"String (timestamp)"
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


