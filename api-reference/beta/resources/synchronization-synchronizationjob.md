---
title: synchronizationJob 资源类型
description: 通过定期在后台运行、轮询一个目录中的更改并将它们推送到另一个目录来执行同步。 同步作业始终特定于租户中的应用程序的特定实例。 作为同步作业安装程序的一部分, 您需要授予在目标目录中读取和写入对象的权限, 并自定义作业的同步架构。
localization_priority: Normal
ms.openlocfilehash: 57515857ac6561e73ef0f67f91bdead98abfb937
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32580657"
---
# <a name="synchronizationjob-resource-type"></a><span data-ttu-id="1c140-105">synchronizationJob 资源类型</span><span class="sxs-lookup"><span data-stu-id="1c140-105">synchronizationJob resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1c140-106">通过定期在后台运行、轮询一个目录中的更改并将它们推送到另一个目录来执行同步。</span><span class="sxs-lookup"><span data-stu-id="1c140-106">Performs synchronization by periodically running in the background, polling for changes in one directory, and pushing them to another directory.</span></span> <span data-ttu-id="1c140-107">同步作业始终特定于租户中的应用程序的特定实例。</span><span class="sxs-lookup"><span data-stu-id="1c140-107">The synchronization job is always specific to a particular instance of an application in your tenant.</span></span> <span data-ttu-id="1c140-108">作为同步作业安装程序的一部分, 您需要授予在目标目录中读取和写入对象的权限, 并自定义作业的同步架构。</span><span class="sxs-lookup"><span data-stu-id="1c140-108">As part of the synchronization job setup, you need to give authorization to read and write objects in your target directory, and customize the job's synchronization schema.</span></span>

## <a name="methods"></a><span data-ttu-id="1c140-109">方法</span><span class="sxs-lookup"><span data-stu-id="1c140-109">Methods</span></span>

| <span data-ttu-id="1c140-110">方法</span><span class="sxs-lookup"><span data-stu-id="1c140-110">Method</span></span>        | <span data-ttu-id="1c140-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="1c140-111">Return Type</span></span>               | <span data-ttu-id="1c140-112">说明</span><span class="sxs-lookup"><span data-stu-id="1c140-112">Description</span></span>                  |
|:--------------|:--------------------------|:-----------------------------|
|[<span data-ttu-id="1c140-113">List</span><span class="sxs-lookup"><span data-stu-id="1c140-113">List</span></span>](../api/synchronization-synchronizationjob-list.md)             |<span data-ttu-id="1c140-114">[synchronizationJob](synchronization-synchronizationjob.md)集合</span><span class="sxs-lookup"><span data-stu-id="1c140-114">[synchronizationJob](synchronization-synchronizationjob.md) collection</span></span>  |<span data-ttu-id="1c140-115">列出给定应用程序实例 (服务主体) 的现有作业。</span><span class="sxs-lookup"><span data-stu-id="1c140-115">List existing jobs for a given application instance (service principal).</span></span>|
|[<span data-ttu-id="1c140-116">获取 synchronizationJob</span><span class="sxs-lookup"><span data-stu-id="1c140-116">Get synchronizationJob</span></span>](../api/synchronization-synchronizationjob-get.md) | [<span data-ttu-id="1c140-117">synchronizationJob</span><span class="sxs-lookup"><span data-stu-id="1c140-117">synchronizationJob</span></span>](synchronization-synchronizationjob.md) |<span data-ttu-id="1c140-118">读取 synchronizationJob 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="1c140-118">Read properties and relationships of a synchronizationJob object.</span></span>|
|[<span data-ttu-id="1c140-119">创建</span><span class="sxs-lookup"><span data-stu-id="1c140-119">Create</span></span>](../api/synchronization-synchronizationjob-post.md)         |[<span data-ttu-id="1c140-120">synchronizationJob</span><span class="sxs-lookup"><span data-stu-id="1c140-120">synchronizationJob</span></span>](synchronization-synchronizationjob.md)   |<span data-ttu-id="1c140-121">为给定应用程序创建新作业。</span><span class="sxs-lookup"><span data-stu-id="1c140-121">Create new job for a given application.</span></span>|
|[<span data-ttu-id="1c140-122">Start</span><span class="sxs-lookup"><span data-stu-id="1c140-122">Start</span></span>](../api/synchronization-synchronizationjob-start.md)          |<span data-ttu-id="1c140-123">无</span><span class="sxs-lookup"><span data-stu-id="1c140-123">None</span></span>   |<span data-ttu-id="1c140-124">启动同步。</span><span class="sxs-lookup"><span data-stu-id="1c140-124">Start synchronization.</span></span> <span data-ttu-id="1c140-125">如果作业处于暂停状态, 则它将从作业暂停的点继续。</span><span class="sxs-lookup"><span data-stu-id="1c140-125">If the job is in a paused state, it continues from the point where the job was paused.</span></span> <span data-ttu-id="1c140-126">如果作业处于隔离状态, 则隔离状态为 "已清除"。</span><span class="sxs-lookup"><span data-stu-id="1c140-126">If the job is in quarantine, the quarantine status is cleared.</span></span>|
|[<span data-ttu-id="1c140-127">Restart</span><span class="sxs-lookup"><span data-stu-id="1c140-127">Restart</span></span>](../api/synchronization-synchronizationjob-restart.md)      |<span data-ttu-id="1c140-128">无</span><span class="sxs-lookup"><span data-stu-id="1c140-128">None</span></span>   |<span data-ttu-id="1c140-129">强制作业重新启动并重新处理目录中的所有对象。</span><span class="sxs-lookup"><span data-stu-id="1c140-129">Force the job to start over and re-process all the objects in the directory.</span></span>|
|[<span data-ttu-id="1c140-130">Pause</span><span class="sxs-lookup"><span data-stu-id="1c140-130">Pause</span></span>](../api/synchronization-synchronizationjob-pause.md)          |<span data-ttu-id="1c140-131">无</span><span class="sxs-lookup"><span data-stu-id="1c140-131">None</span></span>   |<span data-ttu-id="1c140-132">临时停止同步。</span><span class="sxs-lookup"><span data-stu-id="1c140-132">Temporarily stop synchronization.</span></span> <span data-ttu-id="1c140-133">所有进度 (包括作业状态) 均保持不变, 作业将从[开始](../api/synchronization-synchronizationjob-start.md)调用时停止的位置继续。</span><span class="sxs-lookup"><span data-stu-id="1c140-133">All the progress, including job state, is persisted, and the job will continue from where it left off when a [Start](../api/synchronization-synchronizationjob-start.md) call is made.</span></span>|
|[<span data-ttu-id="1c140-134">删除</span><span class="sxs-lookup"><span data-stu-id="1c140-134">Delete</span></span>](../api/synchronization-synchronizationjob-delete.md)        |<span data-ttu-id="1c140-135">无</span><span class="sxs-lookup"><span data-stu-id="1c140-135">None</span></span>   |<span data-ttu-id="1c140-136">停止同步, 并永久删除与作业关联的所有状态。</span><span class="sxs-lookup"><span data-stu-id="1c140-136">Stop synchronization, and permanently delete all the state associated with the job.</span></span>|
|[<span data-ttu-id="1c140-137">获取 synchrnoizationSchema</span><span class="sxs-lookup"><span data-stu-id="1c140-137">Get synchrnoizationSchema</span></span>](../api/synchronization-synchronizationschema-get.md)    |[<span data-ttu-id="1c140-138">synchronizationSchema</span><span class="sxs-lookup"><span data-stu-id="1c140-138">synchronizationSchema</span></span>](synchronization-synchronizationschema.md)   |<span data-ttu-id="1c140-139">检索作业的有效同步架构。</span><span class="sxs-lookup"><span data-stu-id="1c140-139">Retrieve the job's effective synchronization schema.</span></span>|
|[<span data-ttu-id="1c140-140">更新 synchroizationSchema</span><span class="sxs-lookup"><span data-stu-id="1c140-140">Update synchroizationSchema</span></span>](../api/synchronization-synchronizationschema-update.md)    |<span data-ttu-id="1c140-141">无</span><span class="sxs-lookup"><span data-stu-id="1c140-141">None</span></span>   |<span data-ttu-id="1c140-142">更新作业的同步架构。</span><span class="sxs-lookup"><span data-stu-id="1c140-142">Update the job's synchronization schema.</span></span> |
|[<span data-ttu-id="1c140-143">验证凭据</span><span class="sxs-lookup"><span data-stu-id="1c140-143">Validate credentials</span></span>](../api/synchronization-synchronizationjob-validatecredentials.md)|<span data-ttu-id="1c140-144">无</span><span class="sxs-lookup"><span data-stu-id="1c140-144">None</span></span>|<span data-ttu-id="1c140-145">测试提供的针对目标目录的凭据。</span><span class="sxs-lookup"><span data-stu-id="1c140-145">Test provided credentials against target directory.</span></span>|

## <a name="properties"></a><span data-ttu-id="1c140-146">属性</span><span class="sxs-lookup"><span data-stu-id="1c140-146">Properties</span></span>

| <span data-ttu-id="1c140-147">属性</span><span class="sxs-lookup"><span data-stu-id="1c140-147">Property</span></span>      | <span data-ttu-id="1c140-148">类型</span><span class="sxs-lookup"><span data-stu-id="1c140-148">Type</span></span>      | <span data-ttu-id="1c140-149">说明</span><span class="sxs-lookup"><span data-stu-id="1c140-149">Description</span></span>    |
|:--------------|:----------|:---------------|
|<span data-ttu-id="1c140-150">id</span><span class="sxs-lookup"><span data-stu-id="1c140-150">id</span></span>             |<span data-ttu-id="1c140-151">String</span><span class="sxs-lookup"><span data-stu-id="1c140-151">String</span></span>                     |<span data-ttu-id="1c140-152">唯一的同步作业标识符。</span><span class="sxs-lookup"><span data-stu-id="1c140-152">Unique synchronization job identifier.</span></span> <span data-ttu-id="1c140-153">只读。</span><span class="sxs-lookup"><span data-stu-id="1c140-153">Read-only.</span></span>|
|<span data-ttu-id="1c140-154">设定</span><span class="sxs-lookup"><span data-stu-id="1c140-154">schedule</span></span>       |[<span data-ttu-id="1c140-155">synchronizationSchedule</span><span class="sxs-lookup"><span data-stu-id="1c140-155">synchronizationSchedule</span></span>](synchronization-synchronizationschedule.md)|<span data-ttu-id="1c140-156">用于运行作业的计划。</span><span class="sxs-lookup"><span data-stu-id="1c140-156">Schedule used to run the job.</span></span> <span data-ttu-id="1c140-157">只读。</span><span class="sxs-lookup"><span data-stu-id="1c140-157">Read-only.</span></span>|
|<span data-ttu-id="1c140-158">状态</span><span class="sxs-lookup"><span data-stu-id="1c140-158">status</span></span>         |[<span data-ttu-id="1c140-159">synchronizationStatus</span><span class="sxs-lookup"><span data-stu-id="1c140-159">synchronizationStatus</span></span>](synchronization-synchronizationstatus.md)     |<span data-ttu-id="1c140-160">作业的状态, 包括上次运行作业的时间、当前作业状态和错误。</span><span class="sxs-lookup"><span data-stu-id="1c140-160">Status of the job, which includes when the job was last run, current job state, and errors.</span></span>|
|<span data-ttu-id="1c140-161">templateId</span><span class="sxs-lookup"><span data-stu-id="1c140-161">templateId</span></span>     |<span data-ttu-id="1c140-162">String</span><span class="sxs-lookup"><span data-stu-id="1c140-162">String</span></span>    |<span data-ttu-id="1c140-163">此作业所基于的[同步模板](synchronization-synchronizationtemplate.md)的标识符。</span><span class="sxs-lookup"><span data-stu-id="1c140-163">Identifier of the [synchronization template](synchronization-synchronizationtemplate.md) this job is based on.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1c140-164">关系</span><span class="sxs-lookup"><span data-stu-id="1c140-164">Relationships</span></span>
| <span data-ttu-id="1c140-165">关系</span><span class="sxs-lookup"><span data-stu-id="1c140-165">Relationship</span></span> | <span data-ttu-id="1c140-166">类型</span><span class="sxs-lookup"><span data-stu-id="1c140-166">Type</span></span>   |<span data-ttu-id="1c140-167">说明</span><span class="sxs-lookup"><span data-stu-id="1c140-167">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1c140-168">架构</span><span class="sxs-lookup"><span data-stu-id="1c140-168">schema</span></span>|[<span data-ttu-id="1c140-169">synchronizationSchema</span><span class="sxs-lookup"><span data-stu-id="1c140-169">synchronizationSchema</span></span>](synchronization-synchronizationschema.md)| <span data-ttu-id="1c140-170">为作业配置的同步架构。</span><span class="sxs-lookup"><span data-stu-id="1c140-170">The synchronization schema configured for the job.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="1c140-171">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1c140-171">JSON representation</span></span>

<span data-ttu-id="1c140-172">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1c140-172">The following is a JSON representation of the resource.</span></span>

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
