---
title: educationSubmission 资源类型
description: 提交由工作分配拥有。 提交表示单个 (或组) 为分配提供的资源以及返回的评分/反馈。
author: dipakboyed
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 3a917a6d74b47b3e42d2457c5bf747abbf237cf4
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47979577"
---
# <a name="educationsubmission-resource-type"></a><span data-ttu-id="39037-104">educationSubmission 资源类型</span><span class="sxs-lookup"><span data-stu-id="39037-104">educationSubmission resource type</span></span>

<span data-ttu-id="39037-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="39037-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="39037-106">提交由工作分配拥有。</span><span class="sxs-lookup"><span data-stu-id="39037-106">Submissions are owned by an assignment.</span></span> <span data-ttu-id="39037-107">提交代表单个 (或组) 为工作分配提供的资源，以及与提交相关联的成绩)  (如成绩或反馈的结果。</span><span class="sxs-lookup"><span data-stu-id="39037-107">A submission represents the resources that an individual (or group) turn in for an assignment and the outcomes (such as grades or feedback) that are associated with the submission.</span></span>
<span data-ttu-id="39037-108">发布工作分配时，将自动创建提交。</span><span class="sxs-lookup"><span data-stu-id="39037-108">Submissions are automatically created when an assignment is published.</span></span> <span data-ttu-id="39037-109">提交内容拥有两个资源列表。</span><span class="sxs-lookup"><span data-stu-id="39037-109">The submission owns two lists of resources.</span></span> <span data-ttu-id="39037-110">资源表示用户/组工作区，而提交的资源代表学生已处于活动状态的资源。</span><span class="sxs-lookup"><span data-stu-id="39037-110">Resources represent the user/groups working area while the submitted resources represent the resources that have actively been turned in by students.</span></span>  

><span data-ttu-id="39037-111">**注意：** 状态为只读，该对象通过操作在工作流中移动。</span><span class="sxs-lookup"><span data-stu-id="39037-111">**Note:** The status is read-only and the object is moved through the workflow via actions.</span></span> 

## <a name="methods"></a><span data-ttu-id="39037-112">方法</span><span class="sxs-lookup"><span data-stu-id="39037-112">Methods</span></span>

| <span data-ttu-id="39037-113">方法</span><span class="sxs-lookup"><span data-stu-id="39037-113">Method</span></span>           | <span data-ttu-id="39037-114">返回类型</span><span class="sxs-lookup"><span data-stu-id="39037-114">Return Type</span></span>    |<span data-ttu-id="39037-115">说明</span><span class="sxs-lookup"><span data-stu-id="39037-115">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="39037-116">获取 educationSubmission</span><span class="sxs-lookup"><span data-stu-id="39037-116">Get educationSubmission</span></span>](../api/educationsubmission-get.md) | [<span data-ttu-id="39037-117">educationSubmission</span><span class="sxs-lookup"><span data-stu-id="39037-117">educationSubmission</span></span>](educationsubmission.md) |<span data-ttu-id="39037-118">读取 **educationSubmission** 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="39037-118">Read properties and relationships of an **educationSubmission** object.</span></span>|
|[<span data-ttu-id="39037-119">列出资源</span><span class="sxs-lookup"><span data-stu-id="39037-119">List resources</span></span>](../api/educationsubmission-list-resources.md) |<span data-ttu-id="39037-120">[educationSubmissionResource](educationsubmissionresource.md) 集合</span><span class="sxs-lookup"><span data-stu-id="39037-120">[educationSubmissionResource](educationsubmissionresource.md) collection</span></span>| <span data-ttu-id="39037-121">获取 **educationSubmissionResource** 对象集合。</span><span class="sxs-lookup"><span data-stu-id="39037-121">Get an **educationSubmissionResource** object collection.</span></span>|
|[<span data-ttu-id="39037-122">列出 submittedResources</span><span class="sxs-lookup"><span data-stu-id="39037-122">List submittedResources</span></span>](../api/educationsubmission-list-submittedresources.md) |<span data-ttu-id="39037-123">[educationSubmissionResource](educationsubmissionresource.md) 集合</span><span class="sxs-lookup"><span data-stu-id="39037-123">[educationSubmissionResource](educationsubmissionresource.md) collection</span></span>| <span data-ttu-id="39037-124">获取 **educationSubmissionResource** 对象集合。</span><span class="sxs-lookup"><span data-stu-id="39037-124">Get an **educationSubmissionResource** object collection.</span></span>|
|[<span data-ttu-id="39037-125">列表结果</span><span class="sxs-lookup"><span data-stu-id="39037-125">List outcomes</span></span>](../api/educationsubmission-list-outcomes.md) |<span data-ttu-id="39037-126">[educationOutcome](educationoutcome.md) 集合</span><span class="sxs-lookup"><span data-stu-id="39037-126">[educationOutcome](educationoutcome.md) collection</span></span>| <span data-ttu-id="39037-127">获取 **educationOutcome** 对象集合。</span><span class="sxs-lookup"><span data-stu-id="39037-127">Get an **educationOutcome** object collection.</span></span>|
|[<span data-ttu-id="39037-128">Return</span><span class="sxs-lookup"><span data-stu-id="39037-128">Return</span></span>](../api/educationsubmission-return.md)|[<span data-ttu-id="39037-129">educationSubmission</span><span class="sxs-lookup"><span data-stu-id="39037-129">educationSubmission</span></span>](educationsubmission.md)|<span data-ttu-id="39037-130">教师使用 return 来表示可以向学生显示成绩/反馈。</span><span class="sxs-lookup"><span data-stu-id="39037-130">A teacher uses return to indicate that the grades/feedback can be shown to the student.</span></span>|
|[<span data-ttu-id="39037-131">Submit</span><span class="sxs-lookup"><span data-stu-id="39037-131">Submit</span></span>](../api/educationsubmission-submit.md)|[<span data-ttu-id="39037-132">educationSubmission</span><span class="sxs-lookup"><span data-stu-id="39037-132">educationSubmission</span></span>](educationsubmission.md)|<span data-ttu-id="39037-133">学生使用提交来打开工作分配。</span><span class="sxs-lookup"><span data-stu-id="39037-133">A student uses submit to turn in the assignment.</span></span> <span data-ttu-id="39037-134">这将把资源复制到 **submittedResources** 文件夹进行评分并更新状态。</span><span class="sxs-lookup"><span data-stu-id="39037-134">This will copy the resources into the **submittedResources** folder for grading and updates the status.</span></span>|
|[<span data-ttu-id="39037-135">Unsubmit</span><span class="sxs-lookup"><span data-stu-id="39037-135">Unsubmit</span></span>](../api/educationsubmission-unsubmit.md)|[<span data-ttu-id="39037-136">educationSubmission</span><span class="sxs-lookup"><span data-stu-id="39037-136">educationSubmission</span></span>](educationsubmission.md)|<span data-ttu-id="39037-137">学生使用 unsubmit 将提交状态移动回 "正在运行"。</span><span class="sxs-lookup"><span data-stu-id="39037-137">A student uses the unsubmit to move the state of the submission from submitted back to working.</span></span> <span data-ttu-id="39037-138">这将把资源复制到 **workingResources** 文件夹进行评分并更新状态。</span><span class="sxs-lookup"><span data-stu-id="39037-138">This will copy the resources into the **workingResources** folder for grading and updates the status.</span></span>|

## <a name="properties"></a><span data-ttu-id="39037-139">属性</span><span class="sxs-lookup"><span data-stu-id="39037-139">Properties</span></span>
| <span data-ttu-id="39037-140">属性</span><span class="sxs-lookup"><span data-stu-id="39037-140">Property</span></span>     | <span data-ttu-id="39037-141">类型</span><span class="sxs-lookup"><span data-stu-id="39037-141">Type</span></span>   |<span data-ttu-id="39037-142">说明</span><span class="sxs-lookup"><span data-stu-id="39037-142">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="39037-143">recipient</span><span class="sxs-lookup"><span data-stu-id="39037-143">recipient</span></span>|[<span data-ttu-id="39037-144">educationSubmissionRecipient</span><span class="sxs-lookup"><span data-stu-id="39037-144">educationSubmissionRecipient</span></span>](educationsubmissionrecipient.md)|<span data-ttu-id="39037-145">此提交被分配到的所有者。</span><span class="sxs-lookup"><span data-stu-id="39037-145">Who this submission is assigned to.</span></span>|
|<span data-ttu-id="39037-146">releasedBy</span><span class="sxs-lookup"><span data-stu-id="39037-146">releasedBy</span></span>|[<span data-ttu-id="39037-147">identitySet</span><span class="sxs-lookup"><span data-stu-id="39037-147">identitySet</span></span>](identityset.md)|<span data-ttu-id="39037-148">将此提交的状态移动到 "已发布" 的用户。</span><span class="sxs-lookup"><span data-stu-id="39037-148">User who moved the status of this submission to released.</span></span>|
|<span data-ttu-id="39037-149">releasedDateTime</span><span class="sxs-lookup"><span data-stu-id="39037-149">releasedDateTime</span></span>|<span data-ttu-id="39037-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="39037-150">DateTimeOffset</span></span>|<span data-ttu-id="39037-151">提交发布的时间。</span><span class="sxs-lookup"><span data-stu-id="39037-151">Moment in time when the submission was released.</span></span> <span data-ttu-id="39037-152">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="39037-152">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="39037-153">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="39037-153">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="39037-154">returnedBy</span><span class="sxs-lookup"><span data-stu-id="39037-154">returnedBy</span></span>|[<span data-ttu-id="39037-155">identitySet</span><span class="sxs-lookup"><span data-stu-id="39037-155">identitySet</span></span>](identityset.md)|<span data-ttu-id="39037-156">将此提交的状态移动到 "已返回" 的用户。</span><span class="sxs-lookup"><span data-stu-id="39037-156">User who moved the status of this submission to returned.</span></span>|
|<span data-ttu-id="39037-157">returnedDateTime</span><span class="sxs-lookup"><span data-stu-id="39037-157">returnedDateTime</span></span>|<span data-ttu-id="39037-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="39037-158">DateTimeOffset</span></span>|<span data-ttu-id="39037-159">返回提交的时间点。</span><span class="sxs-lookup"><span data-stu-id="39037-159">Moment in time when the submission was returned.</span></span> <span data-ttu-id="39037-160">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="39037-160">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="39037-161">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="39037-161">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="39037-162">resourcesFolderUrl</span><span class="sxs-lookup"><span data-stu-id="39037-162">resourcesFolderUrl</span></span>|<span data-ttu-id="39037-163">String</span><span class="sxs-lookup"><span data-stu-id="39037-163">String</span></span>|<span data-ttu-id="39037-164">需要存储此提交的所有文件资源的文件夹。</span><span class="sxs-lookup"><span data-stu-id="39037-164">Folder where all file resources for this submission need to be stored.</span></span>|
|<span data-ttu-id="39037-165">状态</span><span class="sxs-lookup"><span data-stu-id="39037-165">status</span></span>|<span data-ttu-id="39037-166">string</span><span class="sxs-lookup"><span data-stu-id="39037-166">string</span></span>| <span data-ttu-id="39037-167">只读。</span><span class="sxs-lookup"><span data-stu-id="39037-167">Read-Only.</span></span> <span data-ttu-id="39037-168">可取值为：`working`、`submitted`、`released`、`returned`。</span><span class="sxs-lookup"><span data-stu-id="39037-168">Possible values are: `working`, `submitted`, `released`, `returned`.</span></span>|
|<span data-ttu-id="39037-169">submittedBy</span><span class="sxs-lookup"><span data-stu-id="39037-169">submittedBy</span></span>|[<span data-ttu-id="39037-170">identitySet</span><span class="sxs-lookup"><span data-stu-id="39037-170">identitySet</span></span>](identityset.md)|<span data-ttu-id="39037-171">将资源移动到已提交状态的用户。</span><span class="sxs-lookup"><span data-stu-id="39037-171">User who moved the resource into the submitted state.</span></span>|
|<span data-ttu-id="39037-172">submittedDateTime</span><span class="sxs-lookup"><span data-stu-id="39037-172">submittedDateTime</span></span>|<span data-ttu-id="39037-173">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="39037-173">DateTimeOffset</span></span>|<span data-ttu-id="39037-174">将提交状态移至提交状态的时间点。</span><span class="sxs-lookup"><span data-stu-id="39037-174">Moment in time when the submission was moved into the submitted state.</span></span> <span data-ttu-id="39037-175">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="39037-175">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="39037-176">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="39037-176">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="39037-177">unsubmittedBy</span><span class="sxs-lookup"><span data-stu-id="39037-177">unsubmittedBy</span></span>|[<span data-ttu-id="39037-178">identitySet</span><span class="sxs-lookup"><span data-stu-id="39037-178">identitySet</span></span>](identityset.md)|<span data-ttu-id="39037-179">移动资源的用户被提交到工作状态。</span><span class="sxs-lookup"><span data-stu-id="39037-179">User who moved the resource from submitted into the working state.</span></span>|
|<span data-ttu-id="39037-180">unsubmittedDateTime</span><span class="sxs-lookup"><span data-stu-id="39037-180">unsubmittedDateTime</span></span>|<span data-ttu-id="39037-181">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="39037-181">DateTimeOffset</span></span>|<span data-ttu-id="39037-182">将提交的提交时间从提交到工作状态的时刻。</span><span class="sxs-lookup"><span data-stu-id="39037-182">Moment in time when the submission was moved from submitted into the working state.</span></span> <span data-ttu-id="39037-183">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="39037-183">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="39037-184">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="39037-184">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|

## <a name="relationships"></a><span data-ttu-id="39037-185">关系</span><span class="sxs-lookup"><span data-stu-id="39037-185">Relationships</span></span>
| <span data-ttu-id="39037-186">关系</span><span class="sxs-lookup"><span data-stu-id="39037-186">Relationship</span></span> | <span data-ttu-id="39037-187">类型</span><span class="sxs-lookup"><span data-stu-id="39037-187">Type</span></span>   |<span data-ttu-id="39037-188">说明</span><span class="sxs-lookup"><span data-stu-id="39037-188">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="39037-189">resources</span><span class="sxs-lookup"><span data-stu-id="39037-189">resources</span></span>|<span data-ttu-id="39037-190">[educationSubmissionResource](educationsubmissionresource.md) 集合</span><span class="sxs-lookup"><span data-stu-id="39037-190">[educationSubmissionResource](educationsubmissionresource.md) collection</span></span>| <span data-ttu-id="39037-191">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="39037-191">Nullable.</span></span>|
|<span data-ttu-id="39037-192">submittedResources</span><span class="sxs-lookup"><span data-stu-id="39037-192">submittedResources</span></span>|<span data-ttu-id="39037-193">[educationSubmissionResource](educationsubmissionresource.md) 集合</span><span class="sxs-lookup"><span data-stu-id="39037-193">[educationSubmissionResource](educationsubmissionresource.md) collection</span></span>| <span data-ttu-id="39037-194">只读。</span><span class="sxs-lookup"><span data-stu-id="39037-194">Read-only.</span></span> <span data-ttu-id="39037-195">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="39037-195">Nullable.</span></span>|
|<span data-ttu-id="39037-196">成果</span><span class="sxs-lookup"><span data-stu-id="39037-196">outcomes</span></span>|<span data-ttu-id="39037-197">[educationOutcome](educationOutcome.md) 集合。</span><span class="sxs-lookup"><span data-stu-id="39037-197">[educationOutcome](educationOutcome.md) collection.</span></span> <span data-ttu-id="39037-198">保留教师为此提交分配的成绩、反馈和/或 rubrics 信息</span><span class="sxs-lookup"><span data-stu-id="39037-198">Holds grades, feedback and/or rubrics information the teacher assigns to this submission</span></span>|<span data-ttu-id="39037-199">读写。</span><span class="sxs-lookup"><span data-stu-id="39037-199">Read-Write.</span></span> <span data-ttu-id="39037-200">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="39037-200">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="39037-201">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="39037-201">JSON representation</span></span>

<span data-ttu-id="39037-202">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="39037-202">The following is a JSON representation of the resource.</span></span>

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


