---
title: synchronizationJob 资源类型
description: 通过在后台定期运行、 轮询一个目录，并将其推送到另一个目录中的更改执行同步。 同步作业始终是特定于您的租户中的应用程序的特定实例。 作为同步作业设置的一部分，您需要提供读取和写入您的目标目录中的对象的授权和自定义的作业同步架构。
localization_priority: Normal
ms.openlocfilehash: 57515857ac6561e73ef0f67f91bdead98abfb937
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29510566"
---
# <a name="synchronizationjob-resource-type"></a><span data-ttu-id="3109e-105">synchronizationJob 资源类型</span><span class="sxs-lookup"><span data-stu-id="3109e-105">synchronizationJob resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3109e-106">通过在后台定期运行、 轮询一个目录，并将其推送到另一个目录中的更改执行同步。</span><span class="sxs-lookup"><span data-stu-id="3109e-106">Performs synchronization by periodically running in the background, polling for changes in one directory, and pushing them to another directory.</span></span> <span data-ttu-id="3109e-107">同步作业始终是特定于您的租户中的应用程序的特定实例。</span><span class="sxs-lookup"><span data-stu-id="3109e-107">The synchronization job is always specific to a particular instance of an application in your tenant.</span></span> <span data-ttu-id="3109e-108">作为同步作业设置的一部分，您需要提供读取和写入您的目标目录中的对象的授权和自定义的作业同步架构。</span><span class="sxs-lookup"><span data-stu-id="3109e-108">As part of the synchronization job setup, you need to give authorization to read and write objects in your target directory, and customize the job's synchronization schema.</span></span>

## <a name="methods"></a><span data-ttu-id="3109e-109">方法</span><span class="sxs-lookup"><span data-stu-id="3109e-109">Methods</span></span>

| <span data-ttu-id="3109e-110">方法</span><span class="sxs-lookup"><span data-stu-id="3109e-110">Method</span></span>        | <span data-ttu-id="3109e-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="3109e-111">Return Type</span></span>               | <span data-ttu-id="3109e-112">说明</span><span class="sxs-lookup"><span data-stu-id="3109e-112">Description</span></span>                  |
|:--------------|:--------------------------|:-----------------------------|
|[<span data-ttu-id="3109e-113">List</span><span class="sxs-lookup"><span data-stu-id="3109e-113">List</span></span>](../api/synchronization-synchronizationjob-list.md)             |<span data-ttu-id="3109e-114">[synchronizationJob](synchronization-synchronizationjob.md)集合</span><span class="sxs-lookup"><span data-stu-id="3109e-114">[synchronizationJob](synchronization-synchronizationjob.md) collection</span></span>  |<span data-ttu-id="3109e-115">列出现有作业的给定应用程序实例 （服务主体）。</span><span class="sxs-lookup"><span data-stu-id="3109e-115">List existing jobs for a given application instance (service principal).</span></span>|
|[<span data-ttu-id="3109e-116">获取 synchronizationJob</span><span class="sxs-lookup"><span data-stu-id="3109e-116">Get synchronizationJob</span></span>](../api/synchronization-synchronizationjob-get.md) | [<span data-ttu-id="3109e-117">synchronizationJob</span><span class="sxs-lookup"><span data-stu-id="3109e-117">synchronizationJob</span></span>](synchronization-synchronizationjob.md) |<span data-ttu-id="3109e-118">读取属性和 synchronizationJob 对象的关系。</span><span class="sxs-lookup"><span data-stu-id="3109e-118">Read properties and relationships of a synchronizationJob object.</span></span>|
|[<span data-ttu-id="3109e-119">Create</span><span class="sxs-lookup"><span data-stu-id="3109e-119">Create</span></span>](../api/synchronization-synchronizationjob-post.md)         |[<span data-ttu-id="3109e-120">synchronizationJob</span><span class="sxs-lookup"><span data-stu-id="3109e-120">synchronizationJob</span></span>](synchronization-synchronizationjob.md)   |<span data-ttu-id="3109e-121">创建新作业给定应用程序。</span><span class="sxs-lookup"><span data-stu-id="3109e-121">Create new job for a given application.</span></span>|
|[<span data-ttu-id="3109e-122">Start</span><span class="sxs-lookup"><span data-stu-id="3109e-122">Start</span></span>](../api/synchronization-synchronizationjob-start.md)          |<span data-ttu-id="3109e-123">无</span><span class="sxs-lookup"><span data-stu-id="3109e-123">None</span></span>   |<span data-ttu-id="3109e-124">启动同步。</span><span class="sxs-lookup"><span data-stu-id="3109e-124">Start synchronization.</span></span> <span data-ttu-id="3109e-125">如果该作业暂停状态，继续从该作业已暂停其中时间点。</span><span class="sxs-lookup"><span data-stu-id="3109e-125">If the job is in a paused state, it continues from the point where the job was paused.</span></span> <span data-ttu-id="3109e-126">如果该作业在隔离，清除隔离状态。</span><span class="sxs-lookup"><span data-stu-id="3109e-126">If the job is in quarantine, the quarantine status is cleared.</span></span>|
|[<span data-ttu-id="3109e-127">Restart</span><span class="sxs-lookup"><span data-stu-id="3109e-127">Restart</span></span>](../api/synchronization-synchronizationjob-restart.md)      |<span data-ttu-id="3109e-128">无</span><span class="sxs-lookup"><span data-stu-id="3109e-128">None</span></span>   |<span data-ttu-id="3109e-129">强制该作业重新开始重新处理的目录中的所有对象。</span><span class="sxs-lookup"><span data-stu-id="3109e-129">Force the job to start over and re-process all the objects in the directory.</span></span>|
|[<span data-ttu-id="3109e-130">Pause</span><span class="sxs-lookup"><span data-stu-id="3109e-130">Pause</span></span>](../api/synchronization-synchronizationjob-pause.md)          |<span data-ttu-id="3109e-131">无</span><span class="sxs-lookup"><span data-stu-id="3109e-131">None</span></span>   |<span data-ttu-id="3109e-132">暂时停止同步。</span><span class="sxs-lookup"><span data-stu-id="3109e-132">Temporarily stop synchronization.</span></span> <span data-ttu-id="3109e-133">所有的进度，包括作业状态保持不变，且该作业将继续从停止时[启动](../api/synchronization-synchronizationjob-start.md)调用的地方。</span><span class="sxs-lookup"><span data-stu-id="3109e-133">All the progress, including job state, is persisted, and the job will continue from where it left off when a [Start](../api/synchronization-synchronizationjob-start.md) call is made.</span></span>|
|[<span data-ttu-id="3109e-134">删除</span><span class="sxs-lookup"><span data-stu-id="3109e-134">Delete</span></span>](../api/synchronization-synchronizationjob-delete.md)        |<span data-ttu-id="3109e-135">无</span><span class="sxs-lookup"><span data-stu-id="3109e-135">None</span></span>   |<span data-ttu-id="3109e-136">停止同步并永久删除所有与作业相关联的状态。</span><span class="sxs-lookup"><span data-stu-id="3109e-136">Stop synchronization, and permanently delete all the state associated with the job.</span></span>|
|[<span data-ttu-id="3109e-137">获取 synchrnoizationSchema</span><span class="sxs-lookup"><span data-stu-id="3109e-137">Get synchrnoizationSchema</span></span>](../api/synchronization-synchronizationschema-get.md)    |[<span data-ttu-id="3109e-138">synchronizationSchema</span><span class="sxs-lookup"><span data-stu-id="3109e-138">synchronizationSchema</span></span>](synchronization-synchronizationschema.md)   |<span data-ttu-id="3109e-139">检索该作业的有效同步架构。</span><span class="sxs-lookup"><span data-stu-id="3109e-139">Retrieve the job's effective synchronization schema.</span></span>|
|[<span data-ttu-id="3109e-140">更新 synchroizationSchema</span><span class="sxs-lookup"><span data-stu-id="3109e-140">Update synchroizationSchema</span></span>](../api/synchronization-synchronizationschema-update.md)    |<span data-ttu-id="3109e-141">无</span><span class="sxs-lookup"><span data-stu-id="3109e-141">None</span></span>   |<span data-ttu-id="3109e-142">更新作业的同步架构。</span><span class="sxs-lookup"><span data-stu-id="3109e-142">Update the job's synchronization schema.</span></span> |
|[<span data-ttu-id="3109e-143">验证凭据</span><span class="sxs-lookup"><span data-stu-id="3109e-143">Validate credentials</span></span>](../api/synchronization-synchronizationjob-validatecredentials.md)|<span data-ttu-id="3109e-144">无</span><span class="sxs-lookup"><span data-stu-id="3109e-144">None</span></span>|<span data-ttu-id="3109e-145">测试针对目标目录提供的凭据。</span><span class="sxs-lookup"><span data-stu-id="3109e-145">Test provided credentials against target directory.</span></span>|

## <a name="properties"></a><span data-ttu-id="3109e-146">属性</span><span class="sxs-lookup"><span data-stu-id="3109e-146">Properties</span></span>

| <span data-ttu-id="3109e-147">属性</span><span class="sxs-lookup"><span data-stu-id="3109e-147">Property</span></span>      | <span data-ttu-id="3109e-148">类型</span><span class="sxs-lookup"><span data-stu-id="3109e-148">Type</span></span>      | <span data-ttu-id="3109e-149">说明</span><span class="sxs-lookup"><span data-stu-id="3109e-149">Description</span></span>    |
|:--------------|:----------|:---------------|
|<span data-ttu-id="3109e-150">id</span><span class="sxs-lookup"><span data-stu-id="3109e-150">id</span></span>             |<span data-ttu-id="3109e-151">String</span><span class="sxs-lookup"><span data-stu-id="3109e-151">String</span></span>                     |<span data-ttu-id="3109e-152">唯一同步作业标识符。</span><span class="sxs-lookup"><span data-stu-id="3109e-152">Unique synchronization job identifier.</span></span> <span data-ttu-id="3109e-153">只读。</span><span class="sxs-lookup"><span data-stu-id="3109e-153">Read-only.</span></span>|
|<span data-ttu-id="3109e-154">Schedule</span><span class="sxs-lookup"><span data-stu-id="3109e-154">schedule</span></span>       |[<span data-ttu-id="3109e-155">synchronizationSchedule</span><span class="sxs-lookup"><span data-stu-id="3109e-155">synchronizationSchedule</span></span>](synchronization-synchronizationschedule.md)|<span data-ttu-id="3109e-156">用于运行作业的计划。</span><span class="sxs-lookup"><span data-stu-id="3109e-156">Schedule used to run the job.</span></span> <span data-ttu-id="3109e-157">只读。</span><span class="sxs-lookup"><span data-stu-id="3109e-157">Read-only.</span></span>|
|<span data-ttu-id="3109e-158">status</span><span class="sxs-lookup"><span data-stu-id="3109e-158">status</span></span>         |[<span data-ttu-id="3109e-159">synchronizationStatus</span><span class="sxs-lookup"><span data-stu-id="3109e-159">synchronizationStatus</span></span>](synchronization-synchronizationstatus.md)     |<span data-ttu-id="3109e-160">作业，其中包括上次运行作业、 当前作业状态和错误的状态。</span><span class="sxs-lookup"><span data-stu-id="3109e-160">Status of the job, which includes when the job was last run, current job state, and errors.</span></span>|
|<span data-ttu-id="3109e-161">templateId</span><span class="sxs-lookup"><span data-stu-id="3109e-161">templateId</span></span>     |<span data-ttu-id="3109e-162">字符串</span><span class="sxs-lookup"><span data-stu-id="3109e-162">String</span></span>    |<span data-ttu-id="3109e-163">基于此作业[同步模板](synchronization-synchronizationtemplate.md)的标识符。</span><span class="sxs-lookup"><span data-stu-id="3109e-163">Identifier of the [synchronization template](synchronization-synchronizationtemplate.md) this job is based on.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3109e-164">关系</span><span class="sxs-lookup"><span data-stu-id="3109e-164">Relationships</span></span>
| <span data-ttu-id="3109e-165">关系</span><span class="sxs-lookup"><span data-stu-id="3109e-165">Relationship</span></span> | <span data-ttu-id="3109e-166">类型</span><span class="sxs-lookup"><span data-stu-id="3109e-166">Type</span></span>   |<span data-ttu-id="3109e-167">说明</span><span class="sxs-lookup"><span data-stu-id="3109e-167">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3109e-168">架构</span><span class="sxs-lookup"><span data-stu-id="3109e-168">schema</span></span>|[<span data-ttu-id="3109e-169">synchronizationSchema</span><span class="sxs-lookup"><span data-stu-id="3109e-169">synchronizationSchema</span></span>](synchronization-synchronizationschema.md)| <span data-ttu-id="3109e-170">配置作业同步架构。</span><span class="sxs-lookup"><span data-stu-id="3109e-170">The synchronization schema configured for the job.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="3109e-171">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="3109e-171">JSON representation</span></span>

<span data-ttu-id="3109e-172">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3109e-172">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.synchronizationJob"
}-->

```json
{
  "id": "String (identifier)",
  "schedule": {"@odata.type": "microsoft.graph.synchronizationSchedule"},
  "status": {"@odata.type": "microsoft.graph.synchronizationStatus"},
  "templateId": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "synchronizationJob resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/synchronization-synchronizationjob.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
