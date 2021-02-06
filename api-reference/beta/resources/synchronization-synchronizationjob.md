---
title: synchronizationJob 资源类型
description: 通过定期在后台运行、轮询一个目录中的更改，以及将它们推送到另一个目录执行同步。
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: applications
ms.openlocfilehash: 0f0036cd26a72effba41085d9a4638647fd4060e
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50132039"
---
# <a name="synchronizationjob-resource-type"></a><span data-ttu-id="e5abd-103">synchronizationJob 资源类型</span><span class="sxs-lookup"><span data-stu-id="e5abd-103">synchronizationJob resource type</span></span>

<span data-ttu-id="e5abd-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e5abd-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e5abd-105">通过定期在后台运行、轮询一个目录中的更改，以及将它们推送到另一个目录执行同步。</span><span class="sxs-lookup"><span data-stu-id="e5abd-105">Performs synchronization by periodically running in the background, polling for changes in one directory, and pushing them to another directory.</span></span> <span data-ttu-id="e5abd-106">同步作业始终特定于租户中应用程序的特定实例。</span><span class="sxs-lookup"><span data-stu-id="e5abd-106">The synchronization job is always specific to a particular instance of an application in your tenant.</span></span> <span data-ttu-id="e5abd-107">作为同步作业设置的一部分，您需要授权读取和写入目标目录中的对象，并自定义作业的同步架构。</span><span class="sxs-lookup"><span data-stu-id="e5abd-107">As part of the synchronization job setup, you need to give authorization to read and write objects in your target directory, and customize the job's synchronization schema.</span></span>

## <a name="methods"></a><span data-ttu-id="e5abd-108">方法</span><span class="sxs-lookup"><span data-stu-id="e5abd-108">Methods</span></span>

| <span data-ttu-id="e5abd-109">方法</span><span class="sxs-lookup"><span data-stu-id="e5abd-109">Method</span></span>        | <span data-ttu-id="e5abd-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="e5abd-110">Return Type</span></span>               | <span data-ttu-id="e5abd-111">Description</span><span class="sxs-lookup"><span data-stu-id="e5abd-111">Description</span></span>                  |
|:--------------|:--------------------------|:-----------------------------|
|[<span data-ttu-id="e5abd-112">List</span><span class="sxs-lookup"><span data-stu-id="e5abd-112">List</span></span>](../api/synchronization-synchronizationjob-list.md)             |<span data-ttu-id="e5abd-113">[synchronizationJob](synchronization-synchronizationjob.md) 集合</span><span class="sxs-lookup"><span data-stu-id="e5abd-113">[synchronizationJob](synchronization-synchronizationjob.md) collection</span></span>  |<span data-ttu-id="e5abd-114">列出给定应用程序实例的现有作业 (服务主体) 。</span><span class="sxs-lookup"><span data-stu-id="e5abd-114">List existing jobs for a given application instance (service principal).</span></span>|
|[<span data-ttu-id="e5abd-115">获取 synchronizationJob</span><span class="sxs-lookup"><span data-stu-id="e5abd-115">Get synchronizationJob</span></span>](../api/synchronization-synchronizationjob-get.md) | [<span data-ttu-id="e5abd-116">synchronizationJob</span><span class="sxs-lookup"><span data-stu-id="e5abd-116">synchronizationJob</span></span>](synchronization-synchronizationjob.md) |<span data-ttu-id="e5abd-117">读取 synchronizationJob 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="e5abd-117">Read properties and relationships of a synchronizationJob object.</span></span>|
|[<span data-ttu-id="e5abd-118">创建</span><span class="sxs-lookup"><span data-stu-id="e5abd-118">Create</span></span>](../api/synchronization-synchronizationjob-post.md)         |[<span data-ttu-id="e5abd-119">synchronizationJob</span><span class="sxs-lookup"><span data-stu-id="e5abd-119">synchronizationJob</span></span>](synchronization-synchronizationjob.md)   |<span data-ttu-id="e5abd-120">为给定应用程序创建新作业。</span><span class="sxs-lookup"><span data-stu-id="e5abd-120">Create new job for a given application.</span></span>|
|[<span data-ttu-id="e5abd-121">开始</span><span class="sxs-lookup"><span data-stu-id="e5abd-121">Start</span></span>](../api/synchronization-synchronizationjob-start.md)          |<span data-ttu-id="e5abd-122">无</span><span class="sxs-lookup"><span data-stu-id="e5abd-122">None</span></span>   |<span data-ttu-id="e5abd-123">启动同步。</span><span class="sxs-lookup"><span data-stu-id="e5abd-123">Start synchronization.</span></span> <span data-ttu-id="e5abd-124">如果作业已暂停，则从作业暂停时开始继续。</span><span class="sxs-lookup"><span data-stu-id="e5abd-124">If the job is in a paused state, it continues from the point where the job was paused.</span></span> <span data-ttu-id="e5abd-125">如果作业被隔离，则清除隔离状态。</span><span class="sxs-lookup"><span data-stu-id="e5abd-125">If the job is in quarantine, the quarantine status is cleared.</span></span>|
|[<span data-ttu-id="e5abd-126">Restart</span><span class="sxs-lookup"><span data-stu-id="e5abd-126">Restart</span></span>](../api/synchronization-synchronizationjob-restart.md)      |<span data-ttu-id="e5abd-127">无</span><span class="sxs-lookup"><span data-stu-id="e5abd-127">None</span></span>   |<span data-ttu-id="e5abd-128">强制作业重新开始并重新处理目录中的所有对象。</span><span class="sxs-lookup"><span data-stu-id="e5abd-128">Force the job to start over and re-process all the objects in the directory.</span></span>|
|[<span data-ttu-id="e5abd-129">Pause</span><span class="sxs-lookup"><span data-stu-id="e5abd-129">Pause</span></span>](../api/synchronization-synchronizationjob-pause.md)          |<span data-ttu-id="e5abd-130">无</span><span class="sxs-lookup"><span data-stu-id="e5abd-130">None</span></span>   |<span data-ttu-id="e5abd-131">暂时停止同步。</span><span class="sxs-lookup"><span data-stu-id="e5abd-131">Temporarily stop synchronization.</span></span> <span data-ttu-id="e5abd-132">所有进度（包括作业状态）都将保持，并且作业将在启动调用时从它离开的地方继续。 [](../api/synchronization-synchronizationjob-start.md)</span><span class="sxs-lookup"><span data-stu-id="e5abd-132">All the progress, including job state, is persisted, and the job will continue from where it left off when a [Start](../api/synchronization-synchronizationjob-start.md) call is made.</span></span>|
|[<span data-ttu-id="e5abd-133">删除</span><span class="sxs-lookup"><span data-stu-id="e5abd-133">Delete</span></span>](../api/synchronization-synchronizationjob-delete.md)        |<span data-ttu-id="e5abd-134">无</span><span class="sxs-lookup"><span data-stu-id="e5abd-134">None</span></span>   |<span data-ttu-id="e5abd-135">停止同步，并永久删除与作业关联的所有状态。</span><span class="sxs-lookup"><span data-stu-id="e5abd-135">Stop synchronization, and permanently delete all the state associated with the job.</span></span>|
|[<span data-ttu-id="e5abd-136">获取 synchronizationSchema</span><span class="sxs-lookup"><span data-stu-id="e5abd-136">Get synchronizationSchema</span></span>](../api/synchronization-synchronizationschema-get.md)    |[<span data-ttu-id="e5abd-137">synchronizationSchema</span><span class="sxs-lookup"><span data-stu-id="e5abd-137">synchronizationSchema</span></span>](synchronization-synchronizationschema.md)   |<span data-ttu-id="e5abd-138">检索作业的有效同步架构。</span><span class="sxs-lookup"><span data-stu-id="e5abd-138">Retrieve the job's effective synchronization schema.</span></span>|
|[<span data-ttu-id="e5abd-139">更新 synchronizationSchema</span><span class="sxs-lookup"><span data-stu-id="e5abd-139">Update synchronizationSchema</span></span>](../api/synchronization-synchronizationschema-update.md)    |<span data-ttu-id="e5abd-140">无</span><span class="sxs-lookup"><span data-stu-id="e5abd-140">None</span></span>   |<span data-ttu-id="e5abd-141">更新作业的同步架构。</span><span class="sxs-lookup"><span data-stu-id="e5abd-141">Update the job's synchronization schema.</span></span> |
|[<span data-ttu-id="e5abd-142">验证凭据</span><span class="sxs-lookup"><span data-stu-id="e5abd-142">Validate credentials</span></span>](../api/synchronization-synchronizationjob-validatecredentials.md)|<span data-ttu-id="e5abd-143">无</span><span class="sxs-lookup"><span data-stu-id="e5abd-143">None</span></span>|<span data-ttu-id="e5abd-144">针对目标目录测试提供的凭据。</span><span class="sxs-lookup"><span data-stu-id="e5abd-144">Test provided credentials against target directory.</span></span>|
|[<span data-ttu-id="e5abd-145">provisionOnDemand</span><span class="sxs-lookup"><span data-stu-id="e5abd-145">provisionOnDemand</span></span>](../api/synchronization-synchronizationjob-provision-on-demand.md)|<span data-ttu-id="e5abd-146">[synchronizationJobApplicationParameters](../resources/synchronization-synchronizationjobapplicationparameters.md) 集合</span><span class="sxs-lookup"><span data-stu-id="e5abd-146">[synchronizationJobApplicationParameters](../resources/synchronization-synchronizationjobapplicationparameters.md) collection</span></span>|<span data-ttu-id="e5abd-147">表示将设置的对象和执行同步规则。</span><span class="sxs-lookup"><span data-stu-id="e5abd-147">Represents the objects that will be provisioned and the synchronization rules executed.</span></span> <span data-ttu-id="e5abd-148">资源主要用于按需预配。</span><span class="sxs-lookup"><span data-stu-id="e5abd-148">The resource is primarily used for on-demand provisioning.</span></span> |
## <a name="properties"></a><span data-ttu-id="e5abd-149">属性</span><span class="sxs-lookup"><span data-stu-id="e5abd-149">Properties</span></span>

| <span data-ttu-id="e5abd-150">属性</span><span class="sxs-lookup"><span data-stu-id="e5abd-150">Property</span></span>      | <span data-ttu-id="e5abd-151">类型</span><span class="sxs-lookup"><span data-stu-id="e5abd-151">Type</span></span>      | <span data-ttu-id="e5abd-152">说明</span><span class="sxs-lookup"><span data-stu-id="e5abd-152">Description</span></span>    |
|:--------------|:----------|:---------------|
|<span data-ttu-id="e5abd-153">id</span><span class="sxs-lookup"><span data-stu-id="e5abd-153">id</span></span>             |<span data-ttu-id="e5abd-154">字符串</span><span class="sxs-lookup"><span data-stu-id="e5abd-154">String</span></span>                     |<span data-ttu-id="e5abd-155">唯一同步作业标识符。</span><span class="sxs-lookup"><span data-stu-id="e5abd-155">Unique synchronization job identifier.</span></span> <span data-ttu-id="e5abd-156">只读。</span><span class="sxs-lookup"><span data-stu-id="e5abd-156">Read-only.</span></span>|
|<span data-ttu-id="e5abd-157">schedule</span><span class="sxs-lookup"><span data-stu-id="e5abd-157">schedule</span></span>       |[<span data-ttu-id="e5abd-158">synchronizationSchedule</span><span class="sxs-lookup"><span data-stu-id="e5abd-158">synchronizationSchedule</span></span>](synchronization-synchronizationschedule.md)|<span data-ttu-id="e5abd-159">用于运行作业的计划。</span><span class="sxs-lookup"><span data-stu-id="e5abd-159">Schedule used to run the job.</span></span> <span data-ttu-id="e5abd-160">只读。</span><span class="sxs-lookup"><span data-stu-id="e5abd-160">Read-only.</span></span>|
|<span data-ttu-id="e5abd-161">status</span><span class="sxs-lookup"><span data-stu-id="e5abd-161">status</span></span>         |[<span data-ttu-id="e5abd-162">synchronizationStatus</span><span class="sxs-lookup"><span data-stu-id="e5abd-162">synchronizationStatus</span></span>](synchronization-synchronizationstatus.md)     |<span data-ttu-id="e5abd-163">作业的状态，包括上次运行作业时、当前作业状态和错误。</span><span class="sxs-lookup"><span data-stu-id="e5abd-163">Status of the job, which includes when the job was last run, current job state, and errors.</span></span>|
|<span data-ttu-id="e5abd-164">synchronizationJobSettings</span><span class="sxs-lookup"><span data-stu-id="e5abd-164">synchronizationJobSettings</span></span>   |[<span data-ttu-id="e5abd-165">keyValuePair</span><span class="sxs-lookup"><span data-stu-id="e5abd-165">keyValuePair</span></span>](keyvaluepair.md)    |<span data-ttu-id="e5abd-166">与作业关联的设置。</span><span class="sxs-lookup"><span data-stu-id="e5abd-166">Settings associated with the job.</span></span> <span data-ttu-id="e5abd-167">某些设置是从模板继承的。</span><span class="sxs-lookup"><span data-stu-id="e5abd-167">Some settings are inherited from the template.</span></span>|
|<span data-ttu-id="e5abd-168">templateId</span><span class="sxs-lookup"><span data-stu-id="e5abd-168">templateId</span></span>     |<span data-ttu-id="e5abd-169">字符串</span><span class="sxs-lookup"><span data-stu-id="e5abd-169">String</span></span>    |<span data-ttu-id="e5abd-170">此作业 [所基于的](synchronization-synchronizationtemplate.md) 同步模板的标识符。</span><span class="sxs-lookup"><span data-stu-id="e5abd-170">Identifier of the [synchronization template](synchronization-synchronizationtemplate.md) this job is based on.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e5abd-171">关系</span><span class="sxs-lookup"><span data-stu-id="e5abd-171">Relationships</span></span>
| <span data-ttu-id="e5abd-172">关系</span><span class="sxs-lookup"><span data-stu-id="e5abd-172">Relationship</span></span> | <span data-ttu-id="e5abd-173">类型</span><span class="sxs-lookup"><span data-stu-id="e5abd-173">Type</span></span>   |<span data-ttu-id="e5abd-174">说明</span><span class="sxs-lookup"><span data-stu-id="e5abd-174">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e5abd-175">架构</span><span class="sxs-lookup"><span data-stu-id="e5abd-175">schema</span></span>|[<span data-ttu-id="e5abd-176">synchronizationSchema</span><span class="sxs-lookup"><span data-stu-id="e5abd-176">synchronizationSchema</span></span>](synchronization-synchronizationschema.md)| <span data-ttu-id="e5abd-177">为作业配置的同步架构。</span><span class="sxs-lookup"><span data-stu-id="e5abd-177">The synchronization schema configured for the job.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e5abd-178">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e5abd-178">JSON representation</span></span>

<span data-ttu-id="e5abd-179">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e5abd-179">The following is a JSON representation of the resource.</span></span>

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


