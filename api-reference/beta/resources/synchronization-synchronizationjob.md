---
title: synchronizationJob 资源类型
description: 通过定期在后台运行、轮询一个目录中的更改并将它们推送到另一个目录来执行同步。
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 18c8076a55643289e8ef33fa4316cd224abfe02e
ms.sourcegitcommit: bdef75943ade3f1080120f555b67d5ebb3245699
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/10/2020
ms.locfileid: "43217540"
---
# <a name="synchronizationjob-resource-type"></a><span data-ttu-id="5e1bc-103">synchronizationJob 资源类型</span><span class="sxs-lookup"><span data-stu-id="5e1bc-103">synchronizationJob resource type</span></span>

<span data-ttu-id="5e1bc-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5e1bc-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5e1bc-105">通过定期在后台运行、轮询一个目录中的更改并将它们推送到另一个目录来执行同步。</span><span class="sxs-lookup"><span data-stu-id="5e1bc-105">Performs synchronization by periodically running in the background, polling for changes in one directory, and pushing them to another directory.</span></span> <span data-ttu-id="5e1bc-106">同步作业始终特定于租户中的应用程序的特定实例。</span><span class="sxs-lookup"><span data-stu-id="5e1bc-106">The synchronization job is always specific to a particular instance of an application in your tenant.</span></span> <span data-ttu-id="5e1bc-107">作为同步作业安装程序的一部分，您需要授予在目标目录中读取和写入对象的权限，并自定义作业的同步架构。</span><span class="sxs-lookup"><span data-stu-id="5e1bc-107">As part of the synchronization job setup, you need to give authorization to read and write objects in your target directory, and customize the job's synchronization schema.</span></span>

## <a name="methods"></a><span data-ttu-id="5e1bc-108">Methods</span><span class="sxs-lookup"><span data-stu-id="5e1bc-108">Methods</span></span>

| <span data-ttu-id="5e1bc-109">方法</span><span class="sxs-lookup"><span data-stu-id="5e1bc-109">Method</span></span>        | <span data-ttu-id="5e1bc-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="5e1bc-110">Return Type</span></span>               | <span data-ttu-id="5e1bc-111">说明</span><span class="sxs-lookup"><span data-stu-id="5e1bc-111">Description</span></span>                  |
|:--------------|:--------------------------|:-----------------------------|
|[<span data-ttu-id="5e1bc-112">List</span><span class="sxs-lookup"><span data-stu-id="5e1bc-112">List</span></span>](../api/synchronization-synchronizationjob-list.md)             |<span data-ttu-id="5e1bc-113">[synchronizationJob](synchronization-synchronizationjob.md)集合</span><span class="sxs-lookup"><span data-stu-id="5e1bc-113">[synchronizationJob](synchronization-synchronizationjob.md) collection</span></span>  |<span data-ttu-id="5e1bc-114">列出给定应用程序实例（服务主体）的现有作业。</span><span class="sxs-lookup"><span data-stu-id="5e1bc-114">List existing jobs for a given application instance (service principal).</span></span>|
|[<span data-ttu-id="5e1bc-115">获取 synchronizationJob</span><span class="sxs-lookup"><span data-stu-id="5e1bc-115">Get synchronizationJob</span></span>](../api/synchronization-synchronizationjob-get.md) | [<span data-ttu-id="5e1bc-116">synchronizationJob</span><span class="sxs-lookup"><span data-stu-id="5e1bc-116">synchronizationJob</span></span>](synchronization-synchronizationjob.md) |<span data-ttu-id="5e1bc-117">读取 synchronizationJob 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="5e1bc-117">Read properties and relationships of a synchronizationJob object.</span></span>|
|[<span data-ttu-id="5e1bc-118">创建</span><span class="sxs-lookup"><span data-stu-id="5e1bc-118">Create</span></span>](../api/synchronization-synchronizationjob-post.md)         |[<span data-ttu-id="5e1bc-119">synchronizationJob</span><span class="sxs-lookup"><span data-stu-id="5e1bc-119">synchronizationJob</span></span>](synchronization-synchronizationjob.md)   |<span data-ttu-id="5e1bc-120">为给定应用程序创建新作业。</span><span class="sxs-lookup"><span data-stu-id="5e1bc-120">Create new job for a given application.</span></span>|
|[<span data-ttu-id="5e1bc-121">开始</span><span class="sxs-lookup"><span data-stu-id="5e1bc-121">Start</span></span>](../api/synchronization-synchronizationjob-start.md)          |<span data-ttu-id="5e1bc-122">无</span><span class="sxs-lookup"><span data-stu-id="5e1bc-122">None</span></span>   |<span data-ttu-id="5e1bc-123">启动同步。</span><span class="sxs-lookup"><span data-stu-id="5e1bc-123">Start synchronization.</span></span> <span data-ttu-id="5e1bc-124">如果作业处于暂停状态，则它将从作业暂停的点继续。</span><span class="sxs-lookup"><span data-stu-id="5e1bc-124">If the job is in a paused state, it continues from the point where the job was paused.</span></span> <span data-ttu-id="5e1bc-125">如果作业处于隔离状态，则隔离状态为 "已清除"。</span><span class="sxs-lookup"><span data-stu-id="5e1bc-125">If the job is in quarantine, the quarantine status is cleared.</span></span>|
|[<span data-ttu-id="5e1bc-126">Restart</span><span class="sxs-lookup"><span data-stu-id="5e1bc-126">Restart</span></span>](../api/synchronization-synchronizationjob-restart.md)      |<span data-ttu-id="5e1bc-127">无</span><span class="sxs-lookup"><span data-stu-id="5e1bc-127">None</span></span>   |<span data-ttu-id="5e1bc-128">强制作业重新启动并重新处理目录中的所有对象。</span><span class="sxs-lookup"><span data-stu-id="5e1bc-128">Force the job to start over and re-process all the objects in the directory.</span></span>|
|[<span data-ttu-id="5e1bc-129">Pause</span><span class="sxs-lookup"><span data-stu-id="5e1bc-129">Pause</span></span>](../api/synchronization-synchronizationjob-pause.md)          |<span data-ttu-id="5e1bc-130">无</span><span class="sxs-lookup"><span data-stu-id="5e1bc-130">None</span></span>   |<span data-ttu-id="5e1bc-131">临时停止同步。</span><span class="sxs-lookup"><span data-stu-id="5e1bc-131">Temporarily stop synchronization.</span></span> <span data-ttu-id="5e1bc-132">所有进度（包括作业状态）均保持不变，作业将从[开始](../api/synchronization-synchronizationjob-start.md)调用时停止的位置继续。</span><span class="sxs-lookup"><span data-stu-id="5e1bc-132">All the progress, including job state, is persisted, and the job will continue from where it left off when a [Start](../api/synchronization-synchronizationjob-start.md) call is made.</span></span>|
|[<span data-ttu-id="5e1bc-133">删除</span><span class="sxs-lookup"><span data-stu-id="5e1bc-133">Delete</span></span>](../api/synchronization-synchronizationjob-delete.md)        |<span data-ttu-id="5e1bc-134">无</span><span class="sxs-lookup"><span data-stu-id="5e1bc-134">None</span></span>   |<span data-ttu-id="5e1bc-135">停止同步，并永久删除与作业关联的所有状态。</span><span class="sxs-lookup"><span data-stu-id="5e1bc-135">Stop synchronization, and permanently delete all the state associated with the job.</span></span>|
|[<span data-ttu-id="5e1bc-136">获取 synchronizationSchema</span><span class="sxs-lookup"><span data-stu-id="5e1bc-136">Get synchronizationSchema</span></span>](../api/synchronization-synchronizationschema-get.md)    |[<span data-ttu-id="5e1bc-137">synchronizationSchema</span><span class="sxs-lookup"><span data-stu-id="5e1bc-137">synchronizationSchema</span></span>](synchronization-synchronizationschema.md)   |<span data-ttu-id="5e1bc-138">检索作业的有效同步架构。</span><span class="sxs-lookup"><span data-stu-id="5e1bc-138">Retrieve the job's effective synchronization schema.</span></span>|
|[<span data-ttu-id="5e1bc-139">更新 synchronizationSchema</span><span class="sxs-lookup"><span data-stu-id="5e1bc-139">Update synchronizationSchema</span></span>](../api/synchronization-synchronizationschema-update.md)    |<span data-ttu-id="5e1bc-140">无</span><span class="sxs-lookup"><span data-stu-id="5e1bc-140">None</span></span>   |<span data-ttu-id="5e1bc-141">更新作业的同步架构。</span><span class="sxs-lookup"><span data-stu-id="5e1bc-141">Update the job's synchronization schema.</span></span> |
|[<span data-ttu-id="5e1bc-142">验证凭据</span><span class="sxs-lookup"><span data-stu-id="5e1bc-142">Validate credentials</span></span>](../api/synchronization-synchronizationjob-validatecredentials.md)|<span data-ttu-id="5e1bc-143">无</span><span class="sxs-lookup"><span data-stu-id="5e1bc-143">None</span></span>|<span data-ttu-id="5e1bc-144">测试提供的针对目标目录的凭据。</span><span class="sxs-lookup"><span data-stu-id="5e1bc-144">Test provided credentials against target directory.</span></span>|

## <a name="properties"></a><span data-ttu-id="5e1bc-145">属性</span><span class="sxs-lookup"><span data-stu-id="5e1bc-145">Properties</span></span>

| <span data-ttu-id="5e1bc-146">属性</span><span class="sxs-lookup"><span data-stu-id="5e1bc-146">Property</span></span>      | <span data-ttu-id="5e1bc-147">类型</span><span class="sxs-lookup"><span data-stu-id="5e1bc-147">Type</span></span>      | <span data-ttu-id="5e1bc-148">说明</span><span class="sxs-lookup"><span data-stu-id="5e1bc-148">Description</span></span>    |
|:--------------|:----------|:---------------|
|<span data-ttu-id="5e1bc-149">id</span><span class="sxs-lookup"><span data-stu-id="5e1bc-149">id</span></span>             |<span data-ttu-id="5e1bc-150">字符串</span><span class="sxs-lookup"><span data-stu-id="5e1bc-150">String</span></span>                     |<span data-ttu-id="5e1bc-151">唯一的同步作业标识符。</span><span class="sxs-lookup"><span data-stu-id="5e1bc-151">Unique synchronization job identifier.</span></span> <span data-ttu-id="5e1bc-152">只读。</span><span class="sxs-lookup"><span data-stu-id="5e1bc-152">Read-only.</span></span>|
|<span data-ttu-id="5e1bc-153">schedule</span><span class="sxs-lookup"><span data-stu-id="5e1bc-153">schedule</span></span>       |[<span data-ttu-id="5e1bc-154">synchronizationSchedule</span><span class="sxs-lookup"><span data-stu-id="5e1bc-154">synchronizationSchedule</span></span>](synchronization-synchronizationschedule.md)|<span data-ttu-id="5e1bc-155">用于运行作业的计划。</span><span class="sxs-lookup"><span data-stu-id="5e1bc-155">Schedule used to run the job.</span></span> <span data-ttu-id="5e1bc-156">只读。</span><span class="sxs-lookup"><span data-stu-id="5e1bc-156">Read-only.</span></span>|
|<span data-ttu-id="5e1bc-157">状态</span><span class="sxs-lookup"><span data-stu-id="5e1bc-157">status</span></span>         |[<span data-ttu-id="5e1bc-158">synchronizationStatus</span><span class="sxs-lookup"><span data-stu-id="5e1bc-158">synchronizationStatus</span></span>](synchronization-synchronizationstatus.md)     |<span data-ttu-id="5e1bc-159">作业的状态，包括上次运行作业的时间、当前作业状态和错误。</span><span class="sxs-lookup"><span data-stu-id="5e1bc-159">Status of the job, which includes when the job was last run, current job state, and errors.</span></span>|
|<span data-ttu-id="5e1bc-160">synchronizationJobSettings</span><span class="sxs-lookup"><span data-stu-id="5e1bc-160">synchronizationJobSettings</span></span>   |[<span data-ttu-id="5e1bc-161">keyValuePair</span><span class="sxs-lookup"><span data-stu-id="5e1bc-161">keyValuePair</span></span>](keyvaluepair.md)    |<span data-ttu-id="5e1bc-162">与作业相关联的设置。</span><span class="sxs-lookup"><span data-stu-id="5e1bc-162">Settings associated with the job.</span></span> <span data-ttu-id="5e1bc-163">某些设置是从模板继承的。</span><span class="sxs-lookup"><span data-stu-id="5e1bc-163">Some settings are inherited from the template.</span></span>|
|<span data-ttu-id="5e1bc-164">templateId</span><span class="sxs-lookup"><span data-stu-id="5e1bc-164">templateId</span></span>     |<span data-ttu-id="5e1bc-165">字符串</span><span class="sxs-lookup"><span data-stu-id="5e1bc-165">String</span></span>    |<span data-ttu-id="5e1bc-166">此作业所基于的[同步模板](synchronization-synchronizationtemplate.md)的标识符。</span><span class="sxs-lookup"><span data-stu-id="5e1bc-166">Identifier of the [synchronization template](synchronization-synchronizationtemplate.md) this job is based on.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5e1bc-167">关系</span><span class="sxs-lookup"><span data-stu-id="5e1bc-167">Relationships</span></span>
| <span data-ttu-id="5e1bc-168">关系</span><span class="sxs-lookup"><span data-stu-id="5e1bc-168">Relationship</span></span> | <span data-ttu-id="5e1bc-169">类型</span><span class="sxs-lookup"><span data-stu-id="5e1bc-169">Type</span></span>   |<span data-ttu-id="5e1bc-170">说明</span><span class="sxs-lookup"><span data-stu-id="5e1bc-170">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5e1bc-171">架构</span><span class="sxs-lookup"><span data-stu-id="5e1bc-171">schema</span></span>|[<span data-ttu-id="5e1bc-172">synchronizationSchema</span><span class="sxs-lookup"><span data-stu-id="5e1bc-172">synchronizationSchema</span></span>](synchronization-synchronizationschema.md)| <span data-ttu-id="5e1bc-173">为作业配置的同步架构。</span><span class="sxs-lookup"><span data-stu-id="5e1bc-173">The synchronization schema configured for the job.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="5e1bc-174">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5e1bc-174">JSON representation</span></span>

<span data-ttu-id="5e1bc-175">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5e1bc-175">The following is a JSON representation of the resource.</span></span>

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
  "synchronizationJobSettings": {"@odata.type": "microsoft.graph.keyValuePair"},
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
