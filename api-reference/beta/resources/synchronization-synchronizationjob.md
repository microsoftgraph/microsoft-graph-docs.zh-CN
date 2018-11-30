---
title: synchronizationJob 资源类型
description: 通过在后台定期运行、 轮询一个目录，并将其推送到另一个目录中的更改执行同步。 同步作业始终是特定于您的租户中的应用程序的特定实例。 作为同步作业设置的一部分，您需要提供读取和写入您的目标目录中的对象的授权和自定义的作业同步架构。
ms.openlocfilehash: 0e6428f2a088e5326f4412e743489c4d94b10296
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27048909"
---
# <a name="synchronizationjob-resource-type"></a><span data-ttu-id="f6a63-105">synchronizationJob 资源类型</span><span class="sxs-lookup"><span data-stu-id="f6a63-105">synchronizationJob resource type</span></span>

> <span data-ttu-id="f6a63-106">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="f6a63-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f6a63-107">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="f6a63-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f6a63-108">通过在后台定期运行、 轮询一个目录，并将其推送到另一个目录中的更改执行同步。</span><span class="sxs-lookup"><span data-stu-id="f6a63-108">Performs synchronization by periodically running in the background, polling for changes in one directory, and pushing them to another directory.</span></span> <span data-ttu-id="f6a63-109">同步作业始终是特定于您的租户中的应用程序的特定实例。</span><span class="sxs-lookup"><span data-stu-id="f6a63-109">The synchronization job is always specific to a particular instance of an application in your tenant.</span></span> <span data-ttu-id="f6a63-110">作为同步作业设置的一部分，您需要提供读取和写入您的目标目录中的对象的授权和自定义的作业同步架构。</span><span class="sxs-lookup"><span data-stu-id="f6a63-110">As part of the synchronization job setup, you need to give authorization to read and write objects in your target directory, and customize the job's synchronization schema.</span></span>

## <a name="methods"></a><span data-ttu-id="f6a63-111">方法</span><span class="sxs-lookup"><span data-stu-id="f6a63-111">Methods</span></span>

| <span data-ttu-id="f6a63-112">方法</span><span class="sxs-lookup"><span data-stu-id="f6a63-112">Method</span></span>        | <span data-ttu-id="f6a63-113">返回类型</span><span class="sxs-lookup"><span data-stu-id="f6a63-113">Return Type</span></span>               | <span data-ttu-id="f6a63-114">说明</span><span class="sxs-lookup"><span data-stu-id="f6a63-114">Description</span></span>                  |
|:--------------|:--------------------------|:-----------------------------|
|[<span data-ttu-id="f6a63-115">List</span><span class="sxs-lookup"><span data-stu-id="f6a63-115">List</span></span>](../api/synchronization-synchronizationjob-list.md)             |<span data-ttu-id="f6a63-116">[synchronizationJob](synchronization-synchronizationjob.md)集合</span><span class="sxs-lookup"><span data-stu-id="f6a63-116">[synchronizationJob](synchronization-synchronizationjob.md) collection</span></span>  |<span data-ttu-id="f6a63-117">列出现有作业的给定应用程序实例 （服务主体）。</span><span class="sxs-lookup"><span data-stu-id="f6a63-117">List existing jobs for a given application instance (service principal).</span></span>|
|[<span data-ttu-id="f6a63-118">获取 synchronizationJob</span><span class="sxs-lookup"><span data-stu-id="f6a63-118">Get synchronizationJob</span></span>](../api/synchronization-synchronizationjob-get.md) | [<span data-ttu-id="f6a63-119">synchronizationJob</span><span class="sxs-lookup"><span data-stu-id="f6a63-119">synchronizationJob</span></span>](synchronization-synchronizationjob.md) |<span data-ttu-id="f6a63-120">读取属性和 synchronizationJob 对象的关系。</span><span class="sxs-lookup"><span data-stu-id="f6a63-120">Read properties and relationships of a synchronizationJob object.</span></span>|
|[<span data-ttu-id="f6a63-121">Create</span><span class="sxs-lookup"><span data-stu-id="f6a63-121">Create</span></span>](../api/synchronization-synchronizationjob-post.md)         |[<span data-ttu-id="f6a63-122">synchronizationJob</span><span class="sxs-lookup"><span data-stu-id="f6a63-122">synchronizationJob</span></span>](synchronization-synchronizationjob.md)   |<span data-ttu-id="f6a63-123">创建新作业给定应用程序。</span><span class="sxs-lookup"><span data-stu-id="f6a63-123">Create new job for a given application.</span></span>|
|[<span data-ttu-id="f6a63-124">Start</span><span class="sxs-lookup"><span data-stu-id="f6a63-124">Start</span></span>](../api/synchronization-synchronizationjob-start.md)          |<span data-ttu-id="f6a63-125">无</span><span class="sxs-lookup"><span data-stu-id="f6a63-125">None</span></span>   |<span data-ttu-id="f6a63-126">启动同步。</span><span class="sxs-lookup"><span data-stu-id="f6a63-126">Start synchronization.</span></span> <span data-ttu-id="f6a63-127">如果该作业暂停状态，继续从该作业已暂停其中时间点。</span><span class="sxs-lookup"><span data-stu-id="f6a63-127">If the job is in a paused state, it continues from the point where the job was paused.</span></span> <span data-ttu-id="f6a63-128">如果该作业在隔离，清除隔离状态。</span><span class="sxs-lookup"><span data-stu-id="f6a63-128">If the job is in quarantine, the quarantine status is cleared.</span></span>|
|[<span data-ttu-id="f6a63-129">Restart</span><span class="sxs-lookup"><span data-stu-id="f6a63-129">Restart</span></span>](../api/synchronization-synchronizationjob-restart.md)      |<span data-ttu-id="f6a63-130">无</span><span class="sxs-lookup"><span data-stu-id="f6a63-130">None</span></span>   |<span data-ttu-id="f6a63-131">强制该作业重新开始重新处理的目录中的所有对象。</span><span class="sxs-lookup"><span data-stu-id="f6a63-131">Force the job to start over and re-process all the objects in the directory.</span></span>|
|[<span data-ttu-id="f6a63-132">Pause</span><span class="sxs-lookup"><span data-stu-id="f6a63-132">Pause</span></span>](../api/synchronization-synchronizationjob-pause.md)          |<span data-ttu-id="f6a63-133">无</span><span class="sxs-lookup"><span data-stu-id="f6a63-133">None</span></span>   |<span data-ttu-id="f6a63-134">暂时停止同步。</span><span class="sxs-lookup"><span data-stu-id="f6a63-134">Temporarily stop synchronization.</span></span> <span data-ttu-id="f6a63-135">所有的进度，包括作业状态保持不变，且该作业将继续从停止时[启动](../api/synchronization-synchronizationjob-start.md)调用的地方。</span><span class="sxs-lookup"><span data-stu-id="f6a63-135">All the progress, including job state, is persisted, and the job will continue from where it left off when a [Start](../api/synchronization-synchronizationjob-start.md) call is made.</span></span>|
|[<span data-ttu-id="f6a63-136">删除</span><span class="sxs-lookup"><span data-stu-id="f6a63-136">Delete</span></span>](../api/synchronization-synchronizationjob-delete.md)        |<span data-ttu-id="f6a63-137">无</span><span class="sxs-lookup"><span data-stu-id="f6a63-137">None</span></span>   |<span data-ttu-id="f6a63-138">停止同步并永久删除所有与作业相关联的状态。</span><span class="sxs-lookup"><span data-stu-id="f6a63-138">Stop synchronization, and permanently delete all the state associated with the job.</span></span>|
|[<span data-ttu-id="f6a63-139">获取 synchrnoizationSchema</span><span class="sxs-lookup"><span data-stu-id="f6a63-139">Get synchrnoizationSchema</span></span>](../api/synchronization-synchronizationschema-get.md)    |[<span data-ttu-id="f6a63-140">synchronizationSchema</span><span class="sxs-lookup"><span data-stu-id="f6a63-140">synchronizationSchema</span></span>](synchronization-synchronizationschema.md)   |<span data-ttu-id="f6a63-141">检索该作业的有效同步架构。</span><span class="sxs-lookup"><span data-stu-id="f6a63-141">Retrieve the job's effective synchronization schema.</span></span>|
|[<span data-ttu-id="f6a63-142">更新 synchroizationSchema</span><span class="sxs-lookup"><span data-stu-id="f6a63-142">Update synchroizationSchema</span></span>](../api/synchronization-synchronizationschema-update.md)    |<span data-ttu-id="f6a63-143">无</span><span class="sxs-lookup"><span data-stu-id="f6a63-143">None</span></span>   |<span data-ttu-id="f6a63-144">更新作业的同步架构。</span><span class="sxs-lookup"><span data-stu-id="f6a63-144">Update the job's synchronization schema.</span></span> |
|[<span data-ttu-id="f6a63-145">验证凭据</span><span class="sxs-lookup"><span data-stu-id="f6a63-145">Validate credentials</span></span>](../api/synchronization-synchronizationjob-validatecredentials.md)|<span data-ttu-id="f6a63-146">无</span><span class="sxs-lookup"><span data-stu-id="f6a63-146">None</span></span>|<span data-ttu-id="f6a63-147">测试针对目标目录提供的凭据。</span><span class="sxs-lookup"><span data-stu-id="f6a63-147">Test provided credentials against target directory.</span></span>|

## <a name="properties"></a><span data-ttu-id="f6a63-148">属性</span><span class="sxs-lookup"><span data-stu-id="f6a63-148">Properties</span></span>

| <span data-ttu-id="f6a63-149">属性</span><span class="sxs-lookup"><span data-stu-id="f6a63-149">Property</span></span>      | <span data-ttu-id="f6a63-150">类型</span><span class="sxs-lookup"><span data-stu-id="f6a63-150">Type</span></span>      | <span data-ttu-id="f6a63-151">说明</span><span class="sxs-lookup"><span data-stu-id="f6a63-151">Description</span></span>    |
|:--------------|:----------|:---------------|
|<span data-ttu-id="f6a63-152">id</span><span class="sxs-lookup"><span data-stu-id="f6a63-152">id</span></span>             |<span data-ttu-id="f6a63-153">字符串</span><span class="sxs-lookup"><span data-stu-id="f6a63-153">String</span></span>                     |<span data-ttu-id="f6a63-154">唯一同步作业标识符。</span><span class="sxs-lookup"><span data-stu-id="f6a63-154">Unique synchronization job identifier.</span></span> <span data-ttu-id="f6a63-155">只读。</span><span class="sxs-lookup"><span data-stu-id="f6a63-155">Read-only.</span></span>|
|<span data-ttu-id="f6a63-156">计划</span><span class="sxs-lookup"><span data-stu-id="f6a63-156">schedule</span></span>       |[<span data-ttu-id="f6a63-157">synchronizationSchedule</span><span class="sxs-lookup"><span data-stu-id="f6a63-157">synchronizationSchedule</span></span>](synchronization-synchronizationschedule.md)|<span data-ttu-id="f6a63-158">用于运行作业的计划。</span><span class="sxs-lookup"><span data-stu-id="f6a63-158">Schedule used to run the job.</span></span> <span data-ttu-id="f6a63-159">只读。</span><span class="sxs-lookup"><span data-stu-id="f6a63-159">Read-only.</span></span>|
|<span data-ttu-id="f6a63-160">状态</span><span class="sxs-lookup"><span data-stu-id="f6a63-160">status</span></span>         |[<span data-ttu-id="f6a63-161">synchronizationStatus</span><span class="sxs-lookup"><span data-stu-id="f6a63-161">synchronizationStatus</span></span>](synchronization-synchronizationstatus.md)     |<span data-ttu-id="f6a63-162">作业，其中包括上次运行作业、 当前作业状态和错误的状态。</span><span class="sxs-lookup"><span data-stu-id="f6a63-162">Status of the job, which includes when the job was last run, current job state, and errors.</span></span>|
|<span data-ttu-id="f6a63-163">templateId</span><span class="sxs-lookup"><span data-stu-id="f6a63-163">templateId</span></span>     |<span data-ttu-id="f6a63-164">字符串</span><span class="sxs-lookup"><span data-stu-id="f6a63-164">String</span></span>    |<span data-ttu-id="f6a63-165">基于此作业[同步模板](synchronization-synchronizationtemplate.md)的标识符。</span><span class="sxs-lookup"><span data-stu-id="f6a63-165">Identifier of the [synchronization template](synchronization-synchronizationtemplate.md) this job is based on.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f6a63-166">Relationships</span><span class="sxs-lookup"><span data-stu-id="f6a63-166">Relationships</span></span>
| <span data-ttu-id="f6a63-167">关系</span><span class="sxs-lookup"><span data-stu-id="f6a63-167">Relationship</span></span> | <span data-ttu-id="f6a63-168">类型</span><span class="sxs-lookup"><span data-stu-id="f6a63-168">Type</span></span>   |<span data-ttu-id="f6a63-169">说明</span><span class="sxs-lookup"><span data-stu-id="f6a63-169">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f6a63-170">架构</span><span class="sxs-lookup"><span data-stu-id="f6a63-170">schema</span></span>|[<span data-ttu-id="f6a63-171">synchronizationSchema</span><span class="sxs-lookup"><span data-stu-id="f6a63-171">synchronizationSchema</span></span>](synchronization-synchronizationschema.md)| <span data-ttu-id="f6a63-172">配置作业同步架构。</span><span class="sxs-lookup"><span data-stu-id="f6a63-172">The synchronization schema configured for the job.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f6a63-173">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f6a63-173">JSON representation</span></span>

<span data-ttu-id="f6a63-174">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f6a63-174">The following is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "synchronizationJob resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->