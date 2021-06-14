---
title: educationSubmission 资源类型
description: 提交表示单个 (或组) 为作业启用的资源，以及 (与提交关联的成绩或) 反馈等结果。
author: sharad-sharma-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: e0539d1ddd44e505c77172ffb4c95a335418f478
ms.sourcegitcommit: f77c1385306fd40557aceb24fdfe4832cbb60a27
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/12/2021
ms.locfileid: "52912305"
---
# <a name="educationsubmission-resource-type"></a><span data-ttu-id="5fa91-103">educationSubmission 资源类型</span><span class="sxs-lookup"><span data-stu-id="5fa91-103">educationSubmission resource type</span></span>

<span data-ttu-id="5fa91-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5fa91-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="5fa91-105">提交表示单个 (或组) 为作业启用的资源，以及 (与提交关联的成绩或) 反馈等结果。</span><span class="sxs-lookup"><span data-stu-id="5fa91-105">A submission represents the resources that an individual (or group) turn in for an assignment and the outcomes (such as grades or feedback) that are associated with the submission.</span></span>

<span data-ttu-id="5fa91-106">提交归工作分配所有。</span><span class="sxs-lookup"><span data-stu-id="5fa91-106">Submissions are owned by an assignment.</span></span> <span data-ttu-id="5fa91-107">发布作业时将自动创建提交。</span><span class="sxs-lookup"><span data-stu-id="5fa91-107">Submissions are automatically created when an assignment is published.</span></span> <span data-ttu-id="5fa91-108">提交拥有两个资源列表。</span><span class="sxs-lookup"><span data-stu-id="5fa91-108">The submission owns two lists of resources.</span></span> <span data-ttu-id="5fa91-109">资源表示用户/组工作区，而提交的资源表示学生已主动启用的资源。</span><span class="sxs-lookup"><span data-stu-id="5fa91-109">Resources represent the user/groups working area while the submitted resources represent the resources that have actively been turned in by students.</span></span>  

<span data-ttu-id="5fa91-110">**status** 属性是只读的，并且对象通过操作在工作流中移动。</span><span class="sxs-lookup"><span data-stu-id="5fa91-110">The **status** property is read-only and the object is moved through the workflow via actions.</span></span> 

<span data-ttu-id="5fa91-111">如果尚未对 **educationSubmission** 资源调用 [setUpResourcesFolder，](../api/educationsubmission-setupResourcesFolder.md)**则 resourcesFolderUrl** 属性为 `null` 。</span><span class="sxs-lookup"><span data-stu-id="5fa91-111">If [setUpResourcesFolder](../api/educationsubmission-setupResourcesFolder.md) has not been called on an **educationSubmission** resource, the **resourcesFolderUrl** property is `null`.</span></span>

## <a name="methods"></a><span data-ttu-id="5fa91-112">方法</span><span class="sxs-lookup"><span data-stu-id="5fa91-112">Methods</span></span>

| <span data-ttu-id="5fa91-113">方法</span><span class="sxs-lookup"><span data-stu-id="5fa91-113">Method</span></span>           | <span data-ttu-id="5fa91-114">返回类型</span><span class="sxs-lookup"><span data-stu-id="5fa91-114">Return Type</span></span>    |<span data-ttu-id="5fa91-115">说明</span><span class="sxs-lookup"><span data-stu-id="5fa91-115">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="5fa91-116">获取 educationSubmission</span><span class="sxs-lookup"><span data-stu-id="5fa91-116">Get educationSubmission</span></span>](../api/educationsubmission-get.md) | [<span data-ttu-id="5fa91-117">educationSubmission</span><span class="sxs-lookup"><span data-stu-id="5fa91-117">educationSubmission</span></span>](educationsubmission.md) |<span data-ttu-id="5fa91-118">读取 **educationSubmission** 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="5fa91-118">Read properties and relationships of an **educationSubmission** object.</span></span>|
|[<span data-ttu-id="5fa91-119">列出资源</span><span class="sxs-lookup"><span data-stu-id="5fa91-119">List resources</span></span>](../api/educationsubmission-list-resources.md) |<span data-ttu-id="5fa91-120">[educationSubmissionResource](educationsubmissionresource.md) 集合</span><span class="sxs-lookup"><span data-stu-id="5fa91-120">[educationSubmissionResource](educationsubmissionresource.md) collection</span></span>| <span data-ttu-id="5fa91-121">获取 **educationSubmissionResource** 对象集合。</span><span class="sxs-lookup"><span data-stu-id="5fa91-121">Get an **educationSubmissionResource** object collection.</span></span>|
|[<span data-ttu-id="5fa91-122">列出 submittedResources</span><span class="sxs-lookup"><span data-stu-id="5fa91-122">List submittedResources</span></span>](../api/educationsubmission-list-submittedresources.md) |<span data-ttu-id="5fa91-123">[educationSubmissionResource](educationsubmissionresource.md) 集合</span><span class="sxs-lookup"><span data-stu-id="5fa91-123">[educationSubmissionResource](educationsubmissionresource.md) collection</span></span>| <span data-ttu-id="5fa91-124">获取 **educationSubmissionResource** 对象集合。</span><span class="sxs-lookup"><span data-stu-id="5fa91-124">Get an **educationSubmissionResource** object collection.</span></span>|
|[<span data-ttu-id="5fa91-125">列出结果</span><span class="sxs-lookup"><span data-stu-id="5fa91-125">List outcomes</span></span>](../api/educationsubmission-list-outcomes.md) |<span data-ttu-id="5fa91-126">[educationOutcome](educationoutcome.md) 集合</span><span class="sxs-lookup"><span data-stu-id="5fa91-126">[educationOutcome](educationoutcome.md) collection</span></span>| <span data-ttu-id="5fa91-127">获取 **educationOutcome** 对象集合。</span><span class="sxs-lookup"><span data-stu-id="5fa91-127">Get an **educationOutcome** object collection.</span></span>|
|[<span data-ttu-id="5fa91-128">return</span><span class="sxs-lookup"><span data-stu-id="5fa91-128">return</span></span>](../api/educationsubmission-return.md)|[<span data-ttu-id="5fa91-129">educationSubmission</span><span class="sxs-lookup"><span data-stu-id="5fa91-129">educationSubmission</span></span>](educationsubmission.md)|<span data-ttu-id="5fa91-130">教师使用返回来指示可以向学生显示成绩/反馈。</span><span class="sxs-lookup"><span data-stu-id="5fa91-130">A teacher uses return to indicate that the grades/feedback can be shown to the student.</span></span>|
|[<span data-ttu-id="5fa91-131">设置提交特定资源文件夹</span><span class="sxs-lookup"><span data-stu-id="5fa91-131">Set up submission specific resources folder</span></span>](../api/educationsubmission-setupResourcesFolder.md) |[<span data-ttu-id="5fa91-132">educationSubmission</span><span class="sxs-lookup"><span data-stu-id="5fa91-132">educationSubmission</span></span>](educationsubmission.md) | <span data-ttu-id="5fa91-133">在SharePoint位置 (创建一个) 文件夹，以将文件作为提交资源上载。</span><span class="sxs-lookup"><span data-stu-id="5fa91-133">Create a SharePoint folder (under pre-defined location) to upload files as submission resources.</span></span> |
|[<span data-ttu-id="5fa91-134">提交</span><span class="sxs-lookup"><span data-stu-id="5fa91-134">submit</span></span>](../api/educationsubmission-submit.md)|[<span data-ttu-id="5fa91-135">educationSubmission</span><span class="sxs-lookup"><span data-stu-id="5fa91-135">educationSubmission</span></span>](educationsubmission.md)|<span data-ttu-id="5fa91-136">学生使用 submit 提交提交作业。</span><span class="sxs-lookup"><span data-stu-id="5fa91-136">A student uses submit to turn in the assignment.</span></span> <span data-ttu-id="5fa91-137">这会将资源复制到 **submittedResources** 文件夹中进行评分并更新状态。</span><span class="sxs-lookup"><span data-stu-id="5fa91-137">This will copy the resources into the **submittedResources** folder for grading and updates the status.</span></span>|
|[<span data-ttu-id="5fa91-138">unsubmit</span><span class="sxs-lookup"><span data-stu-id="5fa91-138">unsubmit</span></span>](../api/educationsubmission-unsubmit.md)|[<span data-ttu-id="5fa91-139">educationSubmission</span><span class="sxs-lookup"><span data-stu-id="5fa91-139">educationSubmission</span></span>](educationsubmission.md)|<span data-ttu-id="5fa91-140">学生使用取消提交将提交状态从提交后移回工作。</span><span class="sxs-lookup"><span data-stu-id="5fa91-140">A student uses the unsubmit to move the state of the submission from submitted back to working.</span></span> <span data-ttu-id="5fa91-141">这会将资源复制到 **workingResources** 文件夹中进行评分并更新状态。</span><span class="sxs-lookup"><span data-stu-id="5fa91-141">This will copy the resources into the **workingResources** folder for grading and updates the status.</span></span>|

## <a name="properties"></a><span data-ttu-id="5fa91-142">属性</span><span class="sxs-lookup"><span data-stu-id="5fa91-142">Properties</span></span>
| <span data-ttu-id="5fa91-143">属性</span><span class="sxs-lookup"><span data-stu-id="5fa91-143">Property</span></span>     | <span data-ttu-id="5fa91-144">类型</span><span class="sxs-lookup"><span data-stu-id="5fa91-144">Type</span></span>   |<span data-ttu-id="5fa91-145">说明</span><span class="sxs-lookup"><span data-stu-id="5fa91-145">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5fa91-146">recipient</span><span class="sxs-lookup"><span data-stu-id="5fa91-146">recipient</span></span>|[<span data-ttu-id="5fa91-147">educationSubmissionRecipient</span><span class="sxs-lookup"><span data-stu-id="5fa91-147">educationSubmissionRecipient</span></span>](educationsubmissionrecipient.md)|<span data-ttu-id="5fa91-148">Who分配此提交。</span><span class="sxs-lookup"><span data-stu-id="5fa91-148">Who this submission is assigned to.</span></span>|
|<span data-ttu-id="5fa91-149">returnedBy</span><span class="sxs-lookup"><span data-stu-id="5fa91-149">returnedBy</span></span>|[<span data-ttu-id="5fa91-150">identitySet</span><span class="sxs-lookup"><span data-stu-id="5fa91-150">identitySet</span></span>](identityset.md)|<span data-ttu-id="5fa91-151">将此提交的状态移至已返回的用户。</span><span class="sxs-lookup"><span data-stu-id="5fa91-151">User who moved the status of this submission to returned.</span></span>|
|<span data-ttu-id="5fa91-152">returnedDateTime</span><span class="sxs-lookup"><span data-stu-id="5fa91-152">returnedDateTime</span></span>|<span data-ttu-id="5fa91-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5fa91-153">DateTimeOffset</span></span>|<span data-ttu-id="5fa91-154">提交返回的时间。</span><span class="sxs-lookup"><span data-stu-id="5fa91-154">Moment in time when the submission was returned.</span></span> <span data-ttu-id="5fa91-155">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="5fa91-155">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="5fa91-156">例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`</span><span class="sxs-lookup"><span data-stu-id="5fa91-156">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="5fa91-157">resourcesFolderUrl</span><span class="sxs-lookup"><span data-stu-id="5fa91-157">resourcesFolderUrl</span></span>|<span data-ttu-id="5fa91-158">String</span><span class="sxs-lookup"><span data-stu-id="5fa91-158">String</span></span>|<span data-ttu-id="5fa91-159">需要存储此提交的所有文件资源的文件夹。</span><span class="sxs-lookup"><span data-stu-id="5fa91-159">Folder where all file resources for this submission need to be stored.</span></span>|
|<span data-ttu-id="5fa91-160">状态</span><span class="sxs-lookup"><span data-stu-id="5fa91-160">status</span></span>|<span data-ttu-id="5fa91-161">string</span><span class="sxs-lookup"><span data-stu-id="5fa91-161">string</span></span>| <span data-ttu-id="5fa91-162">只读。</span><span class="sxs-lookup"><span data-stu-id="5fa91-162">Read-Only.</span></span> <span data-ttu-id="5fa91-163">可取值为：`working`、`submitted`、`released`、`returned`。</span><span class="sxs-lookup"><span data-stu-id="5fa91-163">Possible values are: `working`, `submitted`, `released`, `returned`.</span></span>|
|<span data-ttu-id="5fa91-164">submittedBy</span><span class="sxs-lookup"><span data-stu-id="5fa91-164">submittedBy</span></span>|[<span data-ttu-id="5fa91-165">identitySet</span><span class="sxs-lookup"><span data-stu-id="5fa91-165">identitySet</span></span>](identityset.md)|<span data-ttu-id="5fa91-166">将资源移动到已提交状态的用户。</span><span class="sxs-lookup"><span data-stu-id="5fa91-166">User who moved the resource into the submitted state.</span></span>|
|<span data-ttu-id="5fa91-167">submittedDateTime</span><span class="sxs-lookup"><span data-stu-id="5fa91-167">submittedDateTime</span></span>|<span data-ttu-id="5fa91-168">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5fa91-168">DateTimeOffset</span></span>|<span data-ttu-id="5fa91-169">提交移动到提交状态的时间。</span><span class="sxs-lookup"><span data-stu-id="5fa91-169">Moment in time when the submission was moved into the submitted state.</span></span> <span data-ttu-id="5fa91-170">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="5fa91-170">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="5fa91-171">例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`</span><span class="sxs-lookup"><span data-stu-id="5fa91-171">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="5fa91-172">unsubmittedBy</span><span class="sxs-lookup"><span data-stu-id="5fa91-172">unsubmittedBy</span></span>|[<span data-ttu-id="5fa91-173">identitySet</span><span class="sxs-lookup"><span data-stu-id="5fa91-173">identitySet</span></span>](identityset.md)|<span data-ttu-id="5fa91-174">将资源从提交移动到工作状态的用户。</span><span class="sxs-lookup"><span data-stu-id="5fa91-174">User who moved the resource from submitted into the working state.</span></span>|
|<span data-ttu-id="5fa91-175">unsubmittedDateTime</span><span class="sxs-lookup"><span data-stu-id="5fa91-175">unsubmittedDateTime</span></span>|<span data-ttu-id="5fa91-176">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5fa91-176">DateTimeOffset</span></span>|<span data-ttu-id="5fa91-177">将提交从提交移动到工作状态的时间。</span><span class="sxs-lookup"><span data-stu-id="5fa91-177">Moment in time when the submission was moved from submitted into the working state.</span></span> <span data-ttu-id="5fa91-178">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="5fa91-178">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="5fa91-179">例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`</span><span class="sxs-lookup"><span data-stu-id="5fa91-179">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|

## <a name="relationships"></a><span data-ttu-id="5fa91-180">关系</span><span class="sxs-lookup"><span data-stu-id="5fa91-180">Relationships</span></span>
| <span data-ttu-id="5fa91-181">关系</span><span class="sxs-lookup"><span data-stu-id="5fa91-181">Relationship</span></span> | <span data-ttu-id="5fa91-182">类型</span><span class="sxs-lookup"><span data-stu-id="5fa91-182">Type</span></span>   |<span data-ttu-id="5fa91-183">说明</span><span class="sxs-lookup"><span data-stu-id="5fa91-183">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5fa91-184">resources</span><span class="sxs-lookup"><span data-stu-id="5fa91-184">resources</span></span>|<span data-ttu-id="5fa91-185">[educationSubmissionResource](educationsubmissionresource.md) 集合</span><span class="sxs-lookup"><span data-stu-id="5fa91-185">[educationSubmissionResource](educationsubmissionresource.md) collection</span></span>| <span data-ttu-id="5fa91-186">可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="5fa91-186">Nullable.</span></span>|
|<span data-ttu-id="5fa91-187">submittedResources</span><span class="sxs-lookup"><span data-stu-id="5fa91-187">submittedResources</span></span>|<span data-ttu-id="5fa91-188">[educationSubmissionResource](educationsubmissionresource.md) 集合</span><span class="sxs-lookup"><span data-stu-id="5fa91-188">[educationSubmissionResource](educationsubmissionresource.md) collection</span></span>| <span data-ttu-id="5fa91-p108">只读。可为 Null。</span><span class="sxs-lookup"><span data-stu-id="5fa91-p108">Read-only. Nullable.</span></span>|
|<span data-ttu-id="5fa91-191">outcomes</span><span class="sxs-lookup"><span data-stu-id="5fa91-191">outcomes</span></span>|<span data-ttu-id="5fa91-192">[educationOutcome](educationOutcome.md) 集合。</span><span class="sxs-lookup"><span data-stu-id="5fa91-192">[educationOutcome](educationOutcome.md) collection.</span></span> <span data-ttu-id="5fa91-193">保留教师分配给此提交的成绩、反馈和/或评分标准信息</span><span class="sxs-lookup"><span data-stu-id="5fa91-193">Holds grades, feedback and/or rubrics information the teacher assigns to this submission</span></span>|<span data-ttu-id="5fa91-194">读写。</span><span class="sxs-lookup"><span data-stu-id="5fa91-194">Read-Write.</span></span> <span data-ttu-id="5fa91-195">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="5fa91-195">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="5fa91-196">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5fa91-196">JSON representation</span></span>

<span data-ttu-id="5fa91-197">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5fa91-197">The following is a JSON representation of the resource.</span></span>

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


