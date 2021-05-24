---
title: educationSubmission 资源类型
description: 提交归工作分配所有。 提交表示单个用户或 (组) 为作业启用的资源以及返回的成绩/反馈。
author: dipakboyed
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: f468e0715a07320233db1224c3fcee62e0c8fe63
ms.sourcegitcommit: 276a13a37c3772689dfc71f7cd47586c9581f27d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/24/2021
ms.locfileid: "52629439"
---
# <a name="educationsubmission-resource-type"></a><span data-ttu-id="d0f7f-104">educationSubmission 资源类型</span><span class="sxs-lookup"><span data-stu-id="d0f7f-104">educationSubmission resource type</span></span>

<span data-ttu-id="d0f7f-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d0f7f-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d0f7f-106">提交表示单个 (或组) 为作业启用的资源，以及 (与提交关联的成绩或) 反馈等结果。</span><span class="sxs-lookup"><span data-stu-id="d0f7f-106">A submission represents the resources that an individual (or group) turn in for an assignment and the outcomes (such as grades or feedback) that are associated with the submission.</span></span>

<span data-ttu-id="d0f7f-107">提交归工作分配所有。</span><span class="sxs-lookup"><span data-stu-id="d0f7f-107">Submissions are owned by an assignment.</span></span> <span data-ttu-id="d0f7f-108">发布作业时将自动创建提交。</span><span class="sxs-lookup"><span data-stu-id="d0f7f-108">Submissions are automatically created when an assignment is published.</span></span> <span data-ttu-id="d0f7f-109">提交拥有两个资源列表。</span><span class="sxs-lookup"><span data-stu-id="d0f7f-109">The submission owns two lists of resources.</span></span> <span data-ttu-id="d0f7f-110">资源表示用户/组工作区，而提交的资源表示学生已主动启用的资源。</span><span class="sxs-lookup"><span data-stu-id="d0f7f-110">Resources represent the user/groups working area while the submitted resources represent the resources that have actively been turned in by students.</span></span>  

<span data-ttu-id="d0f7f-111">**status** 属性是只读的，并且对象通过操作在工作流中移动。</span><span class="sxs-lookup"><span data-stu-id="d0f7f-111">The **status** property is read-only and the object is moved through the workflow via actions.</span></span> 

<span data-ttu-id="d0f7f-112">如果尚未对 **educationSubmission** 资源调用 [setUpResourcesFolder，](../api/educationsubmission-setupResourcesFolder.md)**则 resourcesFolderUrl** 属性为 `null` 。</span><span class="sxs-lookup"><span data-stu-id="d0f7f-112">If [setUpResourcesFolder](../api/educationsubmission-setupResourcesFolder.md) has not been called on an **educationSubmission** resource, the **resourcesFolderUrl** property is `null`.</span></span>

## <a name="methods"></a><span data-ttu-id="d0f7f-113">Methods</span><span class="sxs-lookup"><span data-stu-id="d0f7f-113">Methods</span></span>

| <span data-ttu-id="d0f7f-114">方法</span><span class="sxs-lookup"><span data-stu-id="d0f7f-114">Method</span></span>           | <span data-ttu-id="d0f7f-115">返回类型</span><span class="sxs-lookup"><span data-stu-id="d0f7f-115">Return Type</span></span>    |<span data-ttu-id="d0f7f-116">说明</span><span class="sxs-lookup"><span data-stu-id="d0f7f-116">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="d0f7f-117">获取 educationSubmission</span><span class="sxs-lookup"><span data-stu-id="d0f7f-117">Get educationSubmission</span></span>](../api/educationsubmission-get.md) | [<span data-ttu-id="d0f7f-118">educationSubmission</span><span class="sxs-lookup"><span data-stu-id="d0f7f-118">educationSubmission</span></span>](educationsubmission.md) |<span data-ttu-id="d0f7f-119">读取 **educationSubmission** 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="d0f7f-119">Read properties and relationships of an **educationSubmission** object.</span></span>|
|[<span data-ttu-id="d0f7f-120">列出资源</span><span class="sxs-lookup"><span data-stu-id="d0f7f-120">List resources</span></span>](../api/educationsubmission-list-resources.md) |<span data-ttu-id="d0f7f-121">[educationSubmissionResource](educationsubmissionresource.md) 集合</span><span class="sxs-lookup"><span data-stu-id="d0f7f-121">[educationSubmissionResource](educationsubmissionresource.md) collection</span></span>| <span data-ttu-id="d0f7f-122">获取 **educationSubmissionResource** 对象集合。</span><span class="sxs-lookup"><span data-stu-id="d0f7f-122">Get an **educationSubmissionResource** object collection.</span></span>|
|[<span data-ttu-id="d0f7f-123">列出 submittedResources</span><span class="sxs-lookup"><span data-stu-id="d0f7f-123">List submittedResources</span></span>](../api/educationsubmission-list-submittedresources.md) |<span data-ttu-id="d0f7f-124">[educationSubmissionResource](educationsubmissionresource.md) 集合</span><span class="sxs-lookup"><span data-stu-id="d0f7f-124">[educationSubmissionResource](educationsubmissionresource.md) collection</span></span>| <span data-ttu-id="d0f7f-125">获取 **educationSubmissionResource** 对象集合。</span><span class="sxs-lookup"><span data-stu-id="d0f7f-125">Get an **educationSubmissionResource** object collection.</span></span>|
|[<span data-ttu-id="d0f7f-126">列出结果</span><span class="sxs-lookup"><span data-stu-id="d0f7f-126">List outcomes</span></span>](../api/educationsubmission-list-outcomes.md) |<span data-ttu-id="d0f7f-127">[educationOutcome](educationoutcome.md) 集合</span><span class="sxs-lookup"><span data-stu-id="d0f7f-127">[educationOutcome](educationoutcome.md) collection</span></span>| <span data-ttu-id="d0f7f-128">获取 **educationOutcome** 对象集合。</span><span class="sxs-lookup"><span data-stu-id="d0f7f-128">Get an **educationOutcome** object collection.</span></span>|
|[<span data-ttu-id="d0f7f-129">return</span><span class="sxs-lookup"><span data-stu-id="d0f7f-129">return</span></span>](../api/educationsubmission-return.md)|[<span data-ttu-id="d0f7f-130">educationSubmission</span><span class="sxs-lookup"><span data-stu-id="d0f7f-130">educationSubmission</span></span>](educationsubmission.md)|<span data-ttu-id="d0f7f-131">教师使用返回来指示可以向学生显示成绩/反馈。</span><span class="sxs-lookup"><span data-stu-id="d0f7f-131">A teacher uses return to indicate that the grades/feedback can be shown to the student.</span></span>|
|[<span data-ttu-id="d0f7f-132">设置提交特定资源文件夹</span><span class="sxs-lookup"><span data-stu-id="d0f7f-132">Set up submission specific resources folder</span></span>](../api/educationsubmission-setupResourcesFolder.md) |[<span data-ttu-id="d0f7f-133">educationSubmission</span><span class="sxs-lookup"><span data-stu-id="d0f7f-133">educationSubmission</span></span>](educationsubmission.md) | <span data-ttu-id="d0f7f-134">在SharePoint位置 (创建一个) 文件夹，以将文件作为提交资源上载。</span><span class="sxs-lookup"><span data-stu-id="d0f7f-134">Create a SharePoint folder (under pre-defined location) to upload files as submission resources.</span></span> |
|[<span data-ttu-id="d0f7f-135">提交</span><span class="sxs-lookup"><span data-stu-id="d0f7f-135">submit</span></span>](../api/educationsubmission-submit.md)|[<span data-ttu-id="d0f7f-136">educationSubmission</span><span class="sxs-lookup"><span data-stu-id="d0f7f-136">educationSubmission</span></span>](educationsubmission.md)|<span data-ttu-id="d0f7f-137">学生使用 submit 提交提交作业。</span><span class="sxs-lookup"><span data-stu-id="d0f7f-137">A student uses submit to turn in the assignment.</span></span> <span data-ttu-id="d0f7f-138">这会将资源复制到 **submittedResources** 文件夹中进行评分并更新状态。</span><span class="sxs-lookup"><span data-stu-id="d0f7f-138">This will copy the resources into the **submittedResources** folder for grading and updates the status.</span></span>|
|[<span data-ttu-id="d0f7f-139">unsubmit</span><span class="sxs-lookup"><span data-stu-id="d0f7f-139">unsubmit</span></span>](../api/educationsubmission-unsubmit.md)|[<span data-ttu-id="d0f7f-140">educationSubmission</span><span class="sxs-lookup"><span data-stu-id="d0f7f-140">educationSubmission</span></span>](educationsubmission.md)|<span data-ttu-id="d0f7f-141">学生使用取消提交将提交状态从提交后移回工作。</span><span class="sxs-lookup"><span data-stu-id="d0f7f-141">A student uses the unsubmit to move the state of the submission from submitted back to working.</span></span> <span data-ttu-id="d0f7f-142">这会将资源复制到 **workingResources** 文件夹中进行评分并更新状态。</span><span class="sxs-lookup"><span data-stu-id="d0f7f-142">This will copy the resources into the **workingResources** folder for grading and updates the status.</span></span>|

## <a name="properties"></a><span data-ttu-id="d0f7f-143">属性</span><span class="sxs-lookup"><span data-stu-id="d0f7f-143">Properties</span></span>
| <span data-ttu-id="d0f7f-144">属性</span><span class="sxs-lookup"><span data-stu-id="d0f7f-144">Property</span></span>     | <span data-ttu-id="d0f7f-145">类型</span><span class="sxs-lookup"><span data-stu-id="d0f7f-145">Type</span></span>   |<span data-ttu-id="d0f7f-146">说明</span><span class="sxs-lookup"><span data-stu-id="d0f7f-146">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d0f7f-147">recipient</span><span class="sxs-lookup"><span data-stu-id="d0f7f-147">recipient</span></span>|[<span data-ttu-id="d0f7f-148">educationSubmissionRecipient</span><span class="sxs-lookup"><span data-stu-id="d0f7f-148">educationSubmissionRecipient</span></span>](educationsubmissionrecipient.md)|<span data-ttu-id="d0f7f-149">Who分配此提交。</span><span class="sxs-lookup"><span data-stu-id="d0f7f-149">Who this submission is assigned to.</span></span>|
|<span data-ttu-id="d0f7f-150">returnedBy</span><span class="sxs-lookup"><span data-stu-id="d0f7f-150">returnedBy</span></span>|[<span data-ttu-id="d0f7f-151">identitySet</span><span class="sxs-lookup"><span data-stu-id="d0f7f-151">identitySet</span></span>](identityset.md)|<span data-ttu-id="d0f7f-152">将此提交的状态移至已返回的用户。</span><span class="sxs-lookup"><span data-stu-id="d0f7f-152">User who moved the status of this submission to returned.</span></span>|
|<span data-ttu-id="d0f7f-153">returnedDateTime</span><span class="sxs-lookup"><span data-stu-id="d0f7f-153">returnedDateTime</span></span>|<span data-ttu-id="d0f7f-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d0f7f-154">DateTimeOffset</span></span>|<span data-ttu-id="d0f7f-155">提交返回的时间。</span><span class="sxs-lookup"><span data-stu-id="d0f7f-155">Moment in time when the submission was returned.</span></span> <span data-ttu-id="d0f7f-156">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="d0f7f-156">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="d0f7f-157">例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`</span><span class="sxs-lookup"><span data-stu-id="d0f7f-157">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="d0f7f-158">resourcesFolderUrl</span><span class="sxs-lookup"><span data-stu-id="d0f7f-158">resourcesFolderUrl</span></span>|<span data-ttu-id="d0f7f-159">String</span><span class="sxs-lookup"><span data-stu-id="d0f7f-159">String</span></span>|<span data-ttu-id="d0f7f-160">需要存储此提交的所有文件资源的文件夹。</span><span class="sxs-lookup"><span data-stu-id="d0f7f-160">Folder where all file resources for this submission need to be stored.</span></span>|
|<span data-ttu-id="d0f7f-161">状态</span><span class="sxs-lookup"><span data-stu-id="d0f7f-161">status</span></span>|<span data-ttu-id="d0f7f-162">string</span><span class="sxs-lookup"><span data-stu-id="d0f7f-162">string</span></span>| <span data-ttu-id="d0f7f-163">只读。</span><span class="sxs-lookup"><span data-stu-id="d0f7f-163">Read-Only.</span></span> <span data-ttu-id="d0f7f-164">可取值为：`working`、`submitted`、`released`、`returned`。</span><span class="sxs-lookup"><span data-stu-id="d0f7f-164">Possible values are: `working`, `submitted`, `released`, `returned`.</span></span>|
|<span data-ttu-id="d0f7f-165">submittedBy</span><span class="sxs-lookup"><span data-stu-id="d0f7f-165">submittedBy</span></span>|[<span data-ttu-id="d0f7f-166">identitySet</span><span class="sxs-lookup"><span data-stu-id="d0f7f-166">identitySet</span></span>](identityset.md)|<span data-ttu-id="d0f7f-167">将资源移动到已提交状态的用户。</span><span class="sxs-lookup"><span data-stu-id="d0f7f-167">User who moved the resource into the submitted state.</span></span>|
|<span data-ttu-id="d0f7f-168">submittedDateTime</span><span class="sxs-lookup"><span data-stu-id="d0f7f-168">submittedDateTime</span></span>|<span data-ttu-id="d0f7f-169">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d0f7f-169">DateTimeOffset</span></span>|<span data-ttu-id="d0f7f-170">提交移动到提交状态的时间。</span><span class="sxs-lookup"><span data-stu-id="d0f7f-170">Moment in time when the submission was moved into the submitted state.</span></span> <span data-ttu-id="d0f7f-171">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="d0f7f-171">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="d0f7f-172">例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`</span><span class="sxs-lookup"><span data-stu-id="d0f7f-172">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="d0f7f-173">unsubmittedBy</span><span class="sxs-lookup"><span data-stu-id="d0f7f-173">unsubmittedBy</span></span>|[<span data-ttu-id="d0f7f-174">identitySet</span><span class="sxs-lookup"><span data-stu-id="d0f7f-174">identitySet</span></span>](identityset.md)|<span data-ttu-id="d0f7f-175">将资源从提交移动到工作状态的用户。</span><span class="sxs-lookup"><span data-stu-id="d0f7f-175">User who moved the resource from submitted into the working state.</span></span>|
|<span data-ttu-id="d0f7f-176">unsubmittedDateTime</span><span class="sxs-lookup"><span data-stu-id="d0f7f-176">unsubmittedDateTime</span></span>|<span data-ttu-id="d0f7f-177">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d0f7f-177">DateTimeOffset</span></span>|<span data-ttu-id="d0f7f-178">将提交从提交移动到工作状态的时间。</span><span class="sxs-lookup"><span data-stu-id="d0f7f-178">Moment in time when the submission was moved from submitted into the working state.</span></span> <span data-ttu-id="d0f7f-179">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="d0f7f-179">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="d0f7f-180">例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`</span><span class="sxs-lookup"><span data-stu-id="d0f7f-180">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|

## <a name="relationships"></a><span data-ttu-id="d0f7f-181">关系</span><span class="sxs-lookup"><span data-stu-id="d0f7f-181">Relationships</span></span>
| <span data-ttu-id="d0f7f-182">关系</span><span class="sxs-lookup"><span data-stu-id="d0f7f-182">Relationship</span></span> | <span data-ttu-id="d0f7f-183">类型</span><span class="sxs-lookup"><span data-stu-id="d0f7f-183">Type</span></span>   |<span data-ttu-id="d0f7f-184">说明</span><span class="sxs-lookup"><span data-stu-id="d0f7f-184">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d0f7f-185">resources</span><span class="sxs-lookup"><span data-stu-id="d0f7f-185">resources</span></span>|<span data-ttu-id="d0f7f-186">[educationSubmissionResource](educationsubmissionresource.md) 集合</span><span class="sxs-lookup"><span data-stu-id="d0f7f-186">[educationSubmissionResource](educationsubmissionresource.md) collection</span></span>| <span data-ttu-id="d0f7f-187">可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="d0f7f-187">Nullable.</span></span>|
|<span data-ttu-id="d0f7f-188">submittedResources</span><span class="sxs-lookup"><span data-stu-id="d0f7f-188">submittedResources</span></span>|<span data-ttu-id="d0f7f-189">[educationSubmissionResource](educationsubmissionresource.md) 集合</span><span class="sxs-lookup"><span data-stu-id="d0f7f-189">[educationSubmissionResource](educationsubmissionresource.md) collection</span></span>| <span data-ttu-id="d0f7f-p109">只读。可为 Null。</span><span class="sxs-lookup"><span data-stu-id="d0f7f-p109">Read-only. Nullable.</span></span>|
|<span data-ttu-id="d0f7f-192">outcomes</span><span class="sxs-lookup"><span data-stu-id="d0f7f-192">outcomes</span></span>|<span data-ttu-id="d0f7f-193">[educationOutcome](educationOutcome.md) 集合。</span><span class="sxs-lookup"><span data-stu-id="d0f7f-193">[educationOutcome](educationOutcome.md) collection.</span></span> <span data-ttu-id="d0f7f-194">保留教师分配给此提交的成绩、反馈和/或评分标准信息</span><span class="sxs-lookup"><span data-stu-id="d0f7f-194">Holds grades, feedback and/or rubrics information the teacher assigns to this submission</span></span>|<span data-ttu-id="d0f7f-195">读写。</span><span class="sxs-lookup"><span data-stu-id="d0f7f-195">Read-Write.</span></span> <span data-ttu-id="d0f7f-196">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="d0f7f-196">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d0f7f-197">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d0f7f-197">JSON representation</span></span>

<span data-ttu-id="d0f7f-198">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d0f7f-198">The following is a JSON representation of the resource.</span></span>

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


