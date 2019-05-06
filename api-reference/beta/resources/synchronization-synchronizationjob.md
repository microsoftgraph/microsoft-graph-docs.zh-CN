---
title: synchronizationJob 资源类型
description: 通过定期在后台运行、轮询一个目录中的更改并将它们推送到另一个目录来执行同步。 同步作业始终特定于租户中的应用程序的特定实例。 作为同步作业安装程序的一部分, 您需要授予在目标目录中读取和写入对象的权限, 并自定义作业的同步架构。
localization_priority: Normal
ms.openlocfilehash: 186df51b9a2a941d6c27cda03895423e311fb0b0
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2019
ms.locfileid: "33620827"
---
# <a name="synchronizationjob-resource-type"></a><span data-ttu-id="60d50-105">synchronizationJob 资源类型</span><span class="sxs-lookup"><span data-stu-id="60d50-105">synchronizationJob resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="60d50-106">通过定期在后台运行、轮询一个目录中的更改并将它们推送到另一个目录来执行同步。</span><span class="sxs-lookup"><span data-stu-id="60d50-106">Performs synchronization by periodically running in the background, polling for changes in one directory, and pushing them to another directory.</span></span> <span data-ttu-id="60d50-107">同步作业始终特定于租户中的应用程序的特定实例。</span><span class="sxs-lookup"><span data-stu-id="60d50-107">The synchronization job is always specific to a particular instance of an application in your tenant.</span></span> <span data-ttu-id="60d50-108">作为同步作业安装程序的一部分, 您需要授予在目标目录中读取和写入对象的权限, 并自定义作业的同步架构。</span><span class="sxs-lookup"><span data-stu-id="60d50-108">As part of the synchronization job setup, you need to give authorization to read and write objects in your target directory, and customize the job's synchronization schema.</span></span>

## <a name="methods"></a><span data-ttu-id="60d50-109">方法</span><span class="sxs-lookup"><span data-stu-id="60d50-109">Methods</span></span>

| <span data-ttu-id="60d50-110">方法</span><span class="sxs-lookup"><span data-stu-id="60d50-110">Method</span></span>        | <span data-ttu-id="60d50-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="60d50-111">Return Type</span></span>               | <span data-ttu-id="60d50-112">说明</span><span class="sxs-lookup"><span data-stu-id="60d50-112">Description</span></span>                  |
|:--------------|:--------------------------|:-----------------------------|
|[<span data-ttu-id="60d50-113">List</span><span class="sxs-lookup"><span data-stu-id="60d50-113">List</span></span>](../api/synchronization-synchronizationjob-list.md)             |<span data-ttu-id="60d50-114">[synchronizationJob](synchronization-synchronizationjob.md)集合</span><span class="sxs-lookup"><span data-stu-id="60d50-114">[synchronizationJob](synchronization-synchronizationjob.md) collection</span></span>  |<span data-ttu-id="60d50-115">列出给定应用程序实例 (服务主体) 的现有作业。</span><span class="sxs-lookup"><span data-stu-id="60d50-115">List existing jobs for a given application instance (service principal).</span></span>|
|[<span data-ttu-id="60d50-116">获取 synchronizationJob</span><span class="sxs-lookup"><span data-stu-id="60d50-116">Get synchronizationJob</span></span>](../api/synchronization-synchronizationjob-get.md) | [<span data-ttu-id="60d50-117">synchronizationJob</span><span class="sxs-lookup"><span data-stu-id="60d50-117">synchronizationJob</span></span>](synchronization-synchronizationjob.md) |<span data-ttu-id="60d50-118">读取 synchronizationJob 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="60d50-118">Read properties and relationships of a synchronizationJob object.</span></span>|
|[<span data-ttu-id="60d50-119">Create</span><span class="sxs-lookup"><span data-stu-id="60d50-119">Create</span></span>](../api/synchronization-synchronizationjob-post.md)         |[<span data-ttu-id="60d50-120">synchronizationJob</span><span class="sxs-lookup"><span data-stu-id="60d50-120">synchronizationJob</span></span>](synchronization-synchronizationjob.md)   |<span data-ttu-id="60d50-121">为给定应用程序创建新作业。</span><span class="sxs-lookup"><span data-stu-id="60d50-121">Create new job for a given application.</span></span>|
|[<span data-ttu-id="60d50-122">Start</span><span class="sxs-lookup"><span data-stu-id="60d50-122">Start</span></span>](../api/synchronization-synchronizationjob-start.md)          |<span data-ttu-id="60d50-123">无</span><span class="sxs-lookup"><span data-stu-id="60d50-123">None</span></span>   |<span data-ttu-id="60d50-124">启动同步。</span><span class="sxs-lookup"><span data-stu-id="60d50-124">Start synchronization.</span></span> <span data-ttu-id="60d50-125">如果作业处于暂停状态, 则它将从作业暂停的点继续。</span><span class="sxs-lookup"><span data-stu-id="60d50-125">If the job is in a paused state, it continues from the point where the job was paused.</span></span> <span data-ttu-id="60d50-126">如果作业处于隔离状态, 则隔离状态为 "已清除"。</span><span class="sxs-lookup"><span data-stu-id="60d50-126">If the job is in quarantine, the quarantine status is cleared.</span></span>|
|[<span data-ttu-id="60d50-127">Restart</span><span class="sxs-lookup"><span data-stu-id="60d50-127">Restart</span></span>](../api/synchronization-synchronizationjob-restart.md)      |<span data-ttu-id="60d50-128">无</span><span class="sxs-lookup"><span data-stu-id="60d50-128">None</span></span>   |<span data-ttu-id="60d50-129">强制作业重新启动并重新处理目录中的所有对象。</span><span class="sxs-lookup"><span data-stu-id="60d50-129">Force the job to start over and re-process all the objects in the directory.</span></span>|
|[<span data-ttu-id="60d50-130">Pause</span><span class="sxs-lookup"><span data-stu-id="60d50-130">Pause</span></span>](../api/synchronization-synchronizationjob-pause.md)          |<span data-ttu-id="60d50-131">无</span><span class="sxs-lookup"><span data-stu-id="60d50-131">None</span></span>   |<span data-ttu-id="60d50-132">临时停止同步。</span><span class="sxs-lookup"><span data-stu-id="60d50-132">Temporarily stop synchronization.</span></span> <span data-ttu-id="60d50-133">所有进度 (包括作业状态) 均保持不变, 作业将从[开始](../api/synchronization-synchronizationjob-start.md)调用时停止的位置继续。</span><span class="sxs-lookup"><span data-stu-id="60d50-133">All the progress, including job state, is persisted, and the job will continue from where it left off when a [Start](../api/synchronization-synchronizationjob-start.md) call is made.</span></span>|
|[<span data-ttu-id="60d50-134">删除</span><span class="sxs-lookup"><span data-stu-id="60d50-134">Delete</span></span>](../api/synchronization-synchronizationjob-delete.md)        |<span data-ttu-id="60d50-135">无</span><span class="sxs-lookup"><span data-stu-id="60d50-135">None</span></span>   |<span data-ttu-id="60d50-136">停止同步, 并永久删除与作业关联的所有状态。</span><span class="sxs-lookup"><span data-stu-id="60d50-136">Stop synchronization, and permanently delete all the state associated with the job.</span></span>|
|[<span data-ttu-id="60d50-137">获取 synchronizationSchema</span><span class="sxs-lookup"><span data-stu-id="60d50-137">Get synchronizationSchema</span></span>](../api/synchronization-synchronizationschema-get.md)    |[<span data-ttu-id="60d50-138">synchronizationSchema</span><span class="sxs-lookup"><span data-stu-id="60d50-138">synchronizationSchema</span></span>](synchronization-synchronizationschema.md)   |<span data-ttu-id="60d50-139">检索作业的有效同步架构。</span><span class="sxs-lookup"><span data-stu-id="60d50-139">Retrieve the job's effective synchronization schema.</span></span>|
|[<span data-ttu-id="60d50-140">更新 synchronizationSchema</span><span class="sxs-lookup"><span data-stu-id="60d50-140">Update synchronizationSchema</span></span>](../api/synchronization-synchronizationschema-update.md)    |<span data-ttu-id="60d50-141">无</span><span class="sxs-lookup"><span data-stu-id="60d50-141">None</span></span>   |<span data-ttu-id="60d50-142">更新作业的同步架构。</span><span class="sxs-lookup"><span data-stu-id="60d50-142">Update the job's synchronization schema.</span></span> |
|[<span data-ttu-id="60d50-143">验证凭据</span><span class="sxs-lookup"><span data-stu-id="60d50-143">Validate credentials</span></span>](../api/synchronization-synchronizationjob-validatecredentials.md)|<span data-ttu-id="60d50-144">无</span><span class="sxs-lookup"><span data-stu-id="60d50-144">None</span></span>|<span data-ttu-id="60d50-145">测试提供的针对目标目录的凭据。</span><span class="sxs-lookup"><span data-stu-id="60d50-145">Test provided credentials against target directory.</span></span>|

## <a name="properties"></a><span data-ttu-id="60d50-146">属性</span><span class="sxs-lookup"><span data-stu-id="60d50-146">Properties</span></span>

| <span data-ttu-id="60d50-147">属性</span><span class="sxs-lookup"><span data-stu-id="60d50-147">Property</span></span>      | <span data-ttu-id="60d50-148">类型</span><span class="sxs-lookup"><span data-stu-id="60d50-148">Type</span></span>      | <span data-ttu-id="60d50-149">说明</span><span class="sxs-lookup"><span data-stu-id="60d50-149">Description</span></span>    |
|:--------------|:----------|:---------------|
|<span data-ttu-id="60d50-150">id</span><span class="sxs-lookup"><span data-stu-id="60d50-150">id</span></span>             |<span data-ttu-id="60d50-151">字符串</span><span class="sxs-lookup"><span data-stu-id="60d50-151">String</span></span>                     |<span data-ttu-id="60d50-152">唯一的同步作业标识符。</span><span class="sxs-lookup"><span data-stu-id="60d50-152">Unique synchronization job identifier.</span></span> <span data-ttu-id="60d50-153">只读。</span><span class="sxs-lookup"><span data-stu-id="60d50-153">Read-only.</span></span>|
|<span data-ttu-id="60d50-154">schedule</span><span class="sxs-lookup"><span data-stu-id="60d50-154">schedule</span></span>       |[<span data-ttu-id="60d50-155">synchronizationSchedule</span><span class="sxs-lookup"><span data-stu-id="60d50-155">synchronizationSchedule</span></span>](synchronization-synchronizationschedule.md)|<span data-ttu-id="60d50-156">用于运行作业的计划。</span><span class="sxs-lookup"><span data-stu-id="60d50-156">Schedule used to run the job.</span></span> <span data-ttu-id="60d50-157">只读。</span><span class="sxs-lookup"><span data-stu-id="60d50-157">Read-only.</span></span>|
|<span data-ttu-id="60d50-158">status</span><span class="sxs-lookup"><span data-stu-id="60d50-158">status</span></span>         |[<span data-ttu-id="60d50-159">synchronizationStatus</span><span class="sxs-lookup"><span data-stu-id="60d50-159">synchronizationStatus</span></span>](synchronization-synchronizationstatus.md)     |<span data-ttu-id="60d50-160">作业的状态, 包括上次运行作业的时间、当前作业状态和错误。</span><span class="sxs-lookup"><span data-stu-id="60d50-160">Status of the job, which includes when the job was last run, current job state, and errors.</span></span>|
|<span data-ttu-id="60d50-161">templateId</span><span class="sxs-lookup"><span data-stu-id="60d50-161">templateId</span></span>     |<span data-ttu-id="60d50-162">字符串</span><span class="sxs-lookup"><span data-stu-id="60d50-162">String</span></span>    |<span data-ttu-id="60d50-163">此作业所基于的[同步模板](synchronization-synchronizationtemplate.md)的标识符。</span><span class="sxs-lookup"><span data-stu-id="60d50-163">Identifier of the [synchronization template](synchronization-synchronizationtemplate.md) this job is based on.</span></span>|

## <a name="relationships"></a><span data-ttu-id="60d50-164">关系</span><span class="sxs-lookup"><span data-stu-id="60d50-164">Relationships</span></span>
| <span data-ttu-id="60d50-165">关系</span><span class="sxs-lookup"><span data-stu-id="60d50-165">Relationship</span></span> | <span data-ttu-id="60d50-166">类型</span><span class="sxs-lookup"><span data-stu-id="60d50-166">Type</span></span>   |<span data-ttu-id="60d50-167">说明</span><span class="sxs-lookup"><span data-stu-id="60d50-167">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="60d50-168">架构</span><span class="sxs-lookup"><span data-stu-id="60d50-168">schema</span></span>|[<span data-ttu-id="60d50-169">synchronizationSchema</span><span class="sxs-lookup"><span data-stu-id="60d50-169">synchronizationSchema</span></span>](synchronization-synchronizationschema.md)| <span data-ttu-id="60d50-170">为作业配置的同步架构。</span><span class="sxs-lookup"><span data-stu-id="60d50-170">The synchronization schema configured for the job.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="60d50-171">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="60d50-171">JSON representation</span></span>

<span data-ttu-id="60d50-172">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="60d50-172">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "keyProperty": "id",
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
  "suppressions": []
}
-->
