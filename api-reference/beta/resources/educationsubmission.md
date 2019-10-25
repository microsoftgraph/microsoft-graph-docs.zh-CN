---
title: educationSubmission 资源类型
description: 提交由工作分配拥有。 提交表示个人（或组）在工作分配和返回的评分/反馈中打开的资源。
author: dipakboyed
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 325eb9772e350848dbf35f9832282cb92a7fda86
ms.sourcegitcommit: bbef506636bce5b72351ee3834123771c301b1b1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/25/2019
ms.locfileid: "37726385"
---
# <a name="educationsubmission-resource-type"></a><span data-ttu-id="ac1e0-104">educationSubmission 资源类型</span><span class="sxs-lookup"><span data-stu-id="ac1e0-104">educationSubmission resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ac1e0-105">提交由工作分配拥有。</span><span class="sxs-lookup"><span data-stu-id="ac1e0-105">Submissions are owned by an assignment.</span></span> <span data-ttu-id="ac1e0-106">提交表示个人（或组）为工作分配以及与提交相关联的结果（如成绩或反馈）所转的资源。</span><span class="sxs-lookup"><span data-stu-id="ac1e0-106">A submission represents the resources that an individual (or group) turn in for an assignment and the outcomes (such as grades or feedback) that are associated with the submission.</span></span>
<span data-ttu-id="ac1e0-107">发布工作分配时，将自动创建提交。</span><span class="sxs-lookup"><span data-stu-id="ac1e0-107">Submissions are automatically created when an assignment is published.</span></span> <span data-ttu-id="ac1e0-108">提交内容拥有两个资源列表。</span><span class="sxs-lookup"><span data-stu-id="ac1e0-108">The submission owns two lists of resources.</span></span> <span data-ttu-id="ac1e0-109">资源表示用户/组工作区，而提交的资源代表学生已处于活动状态的资源。</span><span class="sxs-lookup"><span data-stu-id="ac1e0-109">Resources represent the user/groups working area while the submitted resources represent the resources that have actively been turned in by students.</span></span>  

><span data-ttu-id="ac1e0-110">**注意：** 状态为只读，该对象通过操作在工作流中移动。</span><span class="sxs-lookup"><span data-stu-id="ac1e0-110">**Note:** The status is read-only and the object is moved through the workflow via actions.</span></span> 

## <a name="methods"></a><span data-ttu-id="ac1e0-111">方法</span><span class="sxs-lookup"><span data-stu-id="ac1e0-111">Methods</span></span>

| <span data-ttu-id="ac1e0-112">方法</span><span class="sxs-lookup"><span data-stu-id="ac1e0-112">Method</span></span>           | <span data-ttu-id="ac1e0-113">返回类型</span><span class="sxs-lookup"><span data-stu-id="ac1e0-113">Return Type</span></span>    |<span data-ttu-id="ac1e0-114">说明</span><span class="sxs-lookup"><span data-stu-id="ac1e0-114">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="ac1e0-115">获取 educationSubmission</span><span class="sxs-lookup"><span data-stu-id="ac1e0-115">Get educationSubmission</span></span>](../api/educationsubmission-get.md) | [<span data-ttu-id="ac1e0-116">educationSubmission</span><span class="sxs-lookup"><span data-stu-id="ac1e0-116">educationSubmission</span></span>](educationsubmission.md) |<span data-ttu-id="ac1e0-117">读取**educationSubmission**对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="ac1e0-117">Read properties and relationships of an **educationSubmission** object.</span></span>|
|[<span data-ttu-id="ac1e0-118">列出资源</span><span class="sxs-lookup"><span data-stu-id="ac1e0-118">List resources</span></span>](../api/educationsubmission-list-resources.md) |<span data-ttu-id="ac1e0-119">[educationSubmissionResource](educationsubmissionresource.md)集合</span><span class="sxs-lookup"><span data-stu-id="ac1e0-119">[educationSubmissionResource](educationsubmissionresource.md) collection</span></span>| <span data-ttu-id="ac1e0-120">获取**educationSubmissionResource**对象集合。</span><span class="sxs-lookup"><span data-stu-id="ac1e0-120">Get an **educationSubmissionResource** object collection.</span></span>|
|[<span data-ttu-id="ac1e0-121">列出 submittedResources</span><span class="sxs-lookup"><span data-stu-id="ac1e0-121">List submittedResources</span></span>](../api/educationsubmission-list-submittedresources.md) |<span data-ttu-id="ac1e0-122">[educationSubmissionResource](educationsubmissionresource.md)集合</span><span class="sxs-lookup"><span data-stu-id="ac1e0-122">[educationSubmissionResource](educationsubmissionresource.md) collection</span></span>| <span data-ttu-id="ac1e0-123">获取**educationSubmissionResource**对象集合。</span><span class="sxs-lookup"><span data-stu-id="ac1e0-123">Get an **educationSubmissionResource** object collection.</span></span>|
|[<span data-ttu-id="ac1e0-124">列表结果</span><span class="sxs-lookup"><span data-stu-id="ac1e0-124">List outcomes</span></span>](../api/educationsubmission-list-outcomes.md) |<span data-ttu-id="ac1e0-125">[educationOutcome](educationoutcome.md)集合</span><span class="sxs-lookup"><span data-stu-id="ac1e0-125">[educationOutcome](educationoutcome.md) collection</span></span>| <span data-ttu-id="ac1e0-126">获取**educationOutcome**对象集合。</span><span class="sxs-lookup"><span data-stu-id="ac1e0-126">Get an **educationOutcome** object collection.</span></span>|
|[<span data-ttu-id="ac1e0-127">Return</span><span class="sxs-lookup"><span data-stu-id="ac1e0-127">Return</span></span>](../api/educationsubmission-return.md)|[<span data-ttu-id="ac1e0-128">educationSubmission</span><span class="sxs-lookup"><span data-stu-id="ac1e0-128">educationSubmission</span></span>](educationsubmission.md)|<span data-ttu-id="ac1e0-129">教师使用 return 来表示可以向学生显示成绩/反馈。</span><span class="sxs-lookup"><span data-stu-id="ac1e0-129">A teacher uses return to indicate that the grades/feedback can be shown to the student.</span></span>|
|[<span data-ttu-id="ac1e0-130">Submit</span><span class="sxs-lookup"><span data-stu-id="ac1e0-130">Submit</span></span>](../api/educationsubmission-submit.md)|[<span data-ttu-id="ac1e0-131">educationSubmission</span><span class="sxs-lookup"><span data-stu-id="ac1e0-131">educationSubmission</span></span>](educationsubmission.md)|<span data-ttu-id="ac1e0-132">学生使用提交来打开工作分配。</span><span class="sxs-lookup"><span data-stu-id="ac1e0-132">A student uses submit to turn in the assignment.</span></span> <span data-ttu-id="ac1e0-133">这将把资源复制到**submittedResources**文件夹进行评分并更新状态。</span><span class="sxs-lookup"><span data-stu-id="ac1e0-133">This will copy the resources into the **submittedResources** folder for grading and updates the status.</span></span>|
|[<span data-ttu-id="ac1e0-134">Unsubmit</span><span class="sxs-lookup"><span data-stu-id="ac1e0-134">Unsubmit</span></span>](../api/educationsubmission-unsubmit.md)|[<span data-ttu-id="ac1e0-135">educationSubmission</span><span class="sxs-lookup"><span data-stu-id="ac1e0-135">educationSubmission</span></span>](educationsubmission.md)|<span data-ttu-id="ac1e0-136">学生使用 unsubmit 将提交状态移动回 "正在运行"。</span><span class="sxs-lookup"><span data-stu-id="ac1e0-136">A student uses the unsubmit to move the state of the submission from submitted back to working.</span></span> <span data-ttu-id="ac1e0-137">这将把资源复制到**workingResources**文件夹进行评分并更新状态。</span><span class="sxs-lookup"><span data-stu-id="ac1e0-137">This will copy the resources into the **workingResources** folder for grading and updates the status.</span></span>|

## <a name="properties"></a><span data-ttu-id="ac1e0-138">属性</span><span class="sxs-lookup"><span data-stu-id="ac1e0-138">Properties</span></span>
| <span data-ttu-id="ac1e0-139">属性</span><span class="sxs-lookup"><span data-stu-id="ac1e0-139">Property</span></span>     | <span data-ttu-id="ac1e0-140">类型</span><span class="sxs-lookup"><span data-stu-id="ac1e0-140">Type</span></span>   |<span data-ttu-id="ac1e0-141">说明</span><span class="sxs-lookup"><span data-stu-id="ac1e0-141">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ac1e0-142">recipient</span><span class="sxs-lookup"><span data-stu-id="ac1e0-142">recipient</span></span>|[<span data-ttu-id="ac1e0-143">educationSubmissionRecipient</span><span class="sxs-lookup"><span data-stu-id="ac1e0-143">educationSubmissionRecipient</span></span>](educationsubmissionrecipient.md)|<span data-ttu-id="ac1e0-144">此提交被分配到的所有者。</span><span class="sxs-lookup"><span data-stu-id="ac1e0-144">Who this submission is assigned to.</span></span>|
|<span data-ttu-id="ac1e0-145">releasedBy</span><span class="sxs-lookup"><span data-stu-id="ac1e0-145">releasedBy</span></span>|[<span data-ttu-id="ac1e0-146">identitySet</span><span class="sxs-lookup"><span data-stu-id="ac1e0-146">identitySet</span></span>](identityset.md)|<span data-ttu-id="ac1e0-147">将此提交的状态移动到 "已发布" 的用户。</span><span class="sxs-lookup"><span data-stu-id="ac1e0-147">User who moved the status of this submission to released.</span></span>|
|<span data-ttu-id="ac1e0-148">releasedDateTime</span><span class="sxs-lookup"><span data-stu-id="ac1e0-148">releasedDateTime</span></span>|<span data-ttu-id="ac1e0-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ac1e0-149">DateTimeOffset</span></span>|<span data-ttu-id="ac1e0-150">提交发布的时间。</span><span class="sxs-lookup"><span data-stu-id="ac1e0-150">Moment in time when the submission was released.</span></span> <span data-ttu-id="ac1e0-151">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="ac1e0-151">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="ac1e0-152">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="ac1e0-152">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="ac1e0-153">returnedBy</span><span class="sxs-lookup"><span data-stu-id="ac1e0-153">returnedBy</span></span>|[<span data-ttu-id="ac1e0-154">identitySet</span><span class="sxs-lookup"><span data-stu-id="ac1e0-154">identitySet</span></span>](identityset.md)|<span data-ttu-id="ac1e0-155">将此提交的状态移动到 "已返回" 的用户。</span><span class="sxs-lookup"><span data-stu-id="ac1e0-155">User who moved the status of this submission to returned.</span></span>|
|<span data-ttu-id="ac1e0-156">returnedDateTime</span><span class="sxs-lookup"><span data-stu-id="ac1e0-156">returnedDateTime</span></span>|<span data-ttu-id="ac1e0-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ac1e0-157">DateTimeOffset</span></span>|<span data-ttu-id="ac1e0-158">返回提交的时间点。</span><span class="sxs-lookup"><span data-stu-id="ac1e0-158">Moment in time when the submission was returned.</span></span> <span data-ttu-id="ac1e0-159">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="ac1e0-159">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="ac1e0-160">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="ac1e0-160">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="ac1e0-161">resourcesFolderUrl</span><span class="sxs-lookup"><span data-stu-id="ac1e0-161">resourcesFolderUrl</span></span>|<span data-ttu-id="ac1e0-162">字符串</span><span class="sxs-lookup"><span data-stu-id="ac1e0-162">String</span></span>|<span data-ttu-id="ac1e0-163">需要存储此提交的所有文件资源的文件夹。</span><span class="sxs-lookup"><span data-stu-id="ac1e0-163">Folder where all file resources for this submission need to be stored.</span></span>|
|<span data-ttu-id="ac1e0-164">状态</span><span class="sxs-lookup"><span data-stu-id="ac1e0-164">status</span></span>|<span data-ttu-id="ac1e0-165">string</span><span class="sxs-lookup"><span data-stu-id="ac1e0-165">string</span></span>| <span data-ttu-id="ac1e0-166">只读。</span><span class="sxs-lookup"><span data-stu-id="ac1e0-166">Read-Only.</span></span> <span data-ttu-id="ac1e0-167">可取值为：`working`、`submitted`、`released`、`returned`。</span><span class="sxs-lookup"><span data-stu-id="ac1e0-167">Possible values are: `working`, `submitted`, `released`, `returned`.</span></span>|
|<span data-ttu-id="ac1e0-168">submittedBy</span><span class="sxs-lookup"><span data-stu-id="ac1e0-168">submittedBy</span></span>|[<span data-ttu-id="ac1e0-169">identitySet</span><span class="sxs-lookup"><span data-stu-id="ac1e0-169">identitySet</span></span>](identityset.md)|<span data-ttu-id="ac1e0-170">将资源移动到已提交状态的用户。</span><span class="sxs-lookup"><span data-stu-id="ac1e0-170">User who moved the resource into the submitted state.</span></span>|
|<span data-ttu-id="ac1e0-171">submittedDateTime</span><span class="sxs-lookup"><span data-stu-id="ac1e0-171">submittedDateTime</span></span>|<span data-ttu-id="ac1e0-172">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ac1e0-172">DateTimeOffset</span></span>|<span data-ttu-id="ac1e0-173">将提交状态移至提交状态的时间点。</span><span class="sxs-lookup"><span data-stu-id="ac1e0-173">Moment in time when the submission was moved into the submitted state.</span></span> <span data-ttu-id="ac1e0-174">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="ac1e0-174">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="ac1e0-175">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="ac1e0-175">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="ac1e0-176">unsubmittedBy</span><span class="sxs-lookup"><span data-stu-id="ac1e0-176">unsubmittedBy</span></span>|[<span data-ttu-id="ac1e0-177">identitySet</span><span class="sxs-lookup"><span data-stu-id="ac1e0-177">identitySet</span></span>](identityset.md)|<span data-ttu-id="ac1e0-178">移动资源的用户被提交到工作状态。</span><span class="sxs-lookup"><span data-stu-id="ac1e0-178">User who moved the resource from submitted into the working state.</span></span>|
|<span data-ttu-id="ac1e0-179">unsubmittedDateTime</span><span class="sxs-lookup"><span data-stu-id="ac1e0-179">unsubmittedDateTime</span></span>|<span data-ttu-id="ac1e0-180">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ac1e0-180">DateTimeOffset</span></span>|<span data-ttu-id="ac1e0-181">将提交的提交时间从提交到工作状态的时刻。</span><span class="sxs-lookup"><span data-stu-id="ac1e0-181">Moment in time when the submission was moved from submitted into the working state.</span></span> <span data-ttu-id="ac1e0-182">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="ac1e0-182">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="ac1e0-183">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="ac1e0-183">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|

## <a name="relationships"></a><span data-ttu-id="ac1e0-184">关系</span><span class="sxs-lookup"><span data-stu-id="ac1e0-184">Relationships</span></span>
| <span data-ttu-id="ac1e0-185">关系</span><span class="sxs-lookup"><span data-stu-id="ac1e0-185">Relationship</span></span> | <span data-ttu-id="ac1e0-186">类型</span><span class="sxs-lookup"><span data-stu-id="ac1e0-186">Type</span></span>   |<span data-ttu-id="ac1e0-187">说明</span><span class="sxs-lookup"><span data-stu-id="ac1e0-187">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ac1e0-188">resources</span><span class="sxs-lookup"><span data-stu-id="ac1e0-188">resources</span></span>|<span data-ttu-id="ac1e0-189">[educationSubmissionResource](educationsubmissionresource.md)集合</span><span class="sxs-lookup"><span data-stu-id="ac1e0-189">[educationSubmissionResource](educationsubmissionresource.md) collection</span></span>| <span data-ttu-id="ac1e0-190">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="ac1e0-190">Nullable.</span></span>|
|<span data-ttu-id="ac1e0-191">submittedResources</span><span class="sxs-lookup"><span data-stu-id="ac1e0-191">submittedResources</span></span>|<span data-ttu-id="ac1e0-192">[educationSubmissionResource](educationsubmissionresource.md)集合</span><span class="sxs-lookup"><span data-stu-id="ac1e0-192">[educationSubmissionResource](educationsubmissionresource.md) collection</span></span>| <span data-ttu-id="ac1e0-193">只读。</span><span class="sxs-lookup"><span data-stu-id="ac1e0-193">Read-only.</span></span> <span data-ttu-id="ac1e0-194">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="ac1e0-194">Nullable.</span></span>|
|<span data-ttu-id="ac1e0-195">成果</span><span class="sxs-lookup"><span data-stu-id="ac1e0-195">outcomes</span></span>|<span data-ttu-id="ac1e0-196">[educationOutcome](educationOutcome.md)集合。</span><span class="sxs-lookup"><span data-stu-id="ac1e0-196">[educationOutcome](educationOutcome.md) collection.</span></span> <span data-ttu-id="ac1e0-197">保留教师为此提交分配的成绩、反馈和/或 rubrics 信息</span><span class="sxs-lookup"><span data-stu-id="ac1e0-197">Holds grades, feedback and/or rubrics information the teacher assigns to this submission</span></span>|<span data-ttu-id="ac1e0-198">读写。</span><span class="sxs-lookup"><span data-stu-id="ac1e0-198">Read-Write.</span></span> <span data-ttu-id="ac1e0-199">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="ac1e0-199">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ac1e0-200">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ac1e0-200">JSON representation</span></span>

<span data-ttu-id="ac1e0-201">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ac1e0-201">The following is a JSON representation of the resource.</span></span>

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
