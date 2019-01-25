---
title: synchronizationStatus 资源类型
description: 代表 synchronizationJob 的当前状态。
localization_priority: Normal
ms.openlocfilehash: 404fe4f7f58b8189b3059c212aa1ce858350bb01
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29523762"
---
# <a name="synchronizationstatus-resource-type"></a><span data-ttu-id="906be-103">synchronizationStatus 资源类型</span><span class="sxs-lookup"><span data-stu-id="906be-103">synchronizationStatus resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="906be-104">代表[synchronizationJob](synchronization-synchronizationjob.md)的当前状态。</span><span class="sxs-lookup"><span data-stu-id="906be-104">Represents the current status of the [synchronizationJob](synchronization-synchronizationjob.md).</span></span>

## <a name="properties"></a><span data-ttu-id="906be-105">属性</span><span class="sxs-lookup"><span data-stu-id="906be-105">Properties</span></span>

| <span data-ttu-id="906be-106">属性</span><span class="sxs-lookup"><span data-stu-id="906be-106">Property</span></span>                              | <span data-ttu-id="906be-107">类型</span><span class="sxs-lookup"><span data-stu-id="906be-107">Type</span></span>      | <span data-ttu-id="906be-108">描述</span><span class="sxs-lookup"><span data-stu-id="906be-108">Description</span></span>    |
|:--------------------------------------|:----------|:---------------|
|<span data-ttu-id="906be-109">code</span><span class="sxs-lookup"><span data-stu-id="906be-109">code</span></span>|<span data-ttu-id="906be-110">String</span><span class="sxs-lookup"><span data-stu-id="906be-110">String</span></span>|<span data-ttu-id="906be-111">高级状态代码的同步作业。</span><span class="sxs-lookup"><span data-stu-id="906be-111">High-level status code of the synchronization job.</span></span> <span data-ttu-id="906be-112">可取值为：`NotConfigured`、`NotRun`、`Active`、`Paused`、`Quarantine`。</span><span class="sxs-lookup"><span data-stu-id="906be-112">Possible values are: `NotConfigured`, `NotRun`, `Active`, `Paused`, `Quarantine`.</span></span>|
|<span data-ttu-id="906be-113">countSuccessiveCompleteFailures</span><span class="sxs-lookup"><span data-stu-id="906be-113">countSuccessiveCompleteFailures</span></span>|<span data-ttu-id="906be-114">Int64</span><span class="sxs-lookup"><span data-stu-id="906be-114">Int64</span></span>|<span data-ttu-id="906be-115">连续次数此作业失败。</span><span class="sxs-lookup"><span data-stu-id="906be-115">Number of consecutive times this job failed.</span></span>|
|<span data-ttu-id="906be-116">escrowsPruned</span><span class="sxs-lookup"><span data-stu-id="906be-116">escrowsPruned</span></span>|<span data-ttu-id="906be-117">Boolean</span><span class="sxs-lookup"><span data-stu-id="906be-117">Boolean</span></span>|<span data-ttu-id="906be-118">`true`如果在初始同步期间已修剪作业的 escrows （对象级错误）。</span><span class="sxs-lookup"><span data-stu-id="906be-118">`true` if the job's escrows (object-level errors) were pruned during initial synchronization.</span></span> <span data-ttu-id="906be-119">如果在初始同步过程达到阈值通常会将作业放在隔离的错误，则可以修剪 escrows。</span><span class="sxs-lookup"><span data-stu-id="906be-119">Escrows can be pruned if during the initial synchronization, you reach the threshold of errors that would normally put the job in quarantine.</span></span> <span data-ttu-id="906be-120">而不是进入隔离，同步过程清除作业的错误，并将继续，直到完成初始同步。</span><span class="sxs-lookup"><span data-stu-id="906be-120">Instead of going into quarantine, the synchronization process clears the job's errors and continues until the initial synchronization is completed.</span></span> <span data-ttu-id="906be-121">完成初始同步后，此作业将暂停并等待客户清理错误。</span><span class="sxs-lookup"><span data-stu-id="906be-121">When the initial synchronization is completed, the job will pause and wait for the customer to clean up the errors.</span></span>|
|<span data-ttu-id="906be-122">lastExecution</span><span class="sxs-lookup"><span data-stu-id="906be-122">lastExecution</span></span>|[<span data-ttu-id="906be-123">synchronizationTaskExecution</span><span class="sxs-lookup"><span data-stu-id="906be-123">synchronizationTaskExecution</span></span>](synchronization-synchronizationtaskexecution.md)|<span data-ttu-id="906be-124">上次执行作业的详细信息。</span><span class="sxs-lookup"><span data-stu-id="906be-124">Details of the last execution of the job.</span></span>|
|<span data-ttu-id="906be-125">lastSuccessfulExecution</span><span class="sxs-lookup"><span data-stu-id="906be-125">lastSuccessfulExecution</span></span>|[<span data-ttu-id="906be-126">synchronizationTaskExecution</span><span class="sxs-lookup"><span data-stu-id="906be-126">synchronizationTaskExecution</span></span>](synchronization-synchronizationtaskexecution.md)|<span data-ttu-id="906be-127">上次执行此作业，没有任何错误的详细信息。</span><span class="sxs-lookup"><span data-stu-id="906be-127">Details of the last execution of this job, which didn't have any errors.</span></span>|
|<span data-ttu-id="906be-128">lastSuccessfulExecutionWithExports</span><span class="sxs-lookup"><span data-stu-id="906be-128">lastSuccessfulExecutionWithExports</span></span>|[<span data-ttu-id="906be-129">synchronizationTaskExecution</span><span class="sxs-lookup"><span data-stu-id="906be-129">synchronizationTaskExecution</span></span>](synchronization-synchronizationtaskexecution.md)|<span data-ttu-id="906be-130">导出到目标目录的对象的作业的上次执行的详细信息。</span><span class="sxs-lookup"><span data-stu-id="906be-130">Details of the last execution of the job, which exported objects into the target directory.</span></span>|
|<span data-ttu-id="906be-131">Progress</span><span class="sxs-lookup"><span data-stu-id="906be-131">progress</span></span>|<span data-ttu-id="906be-132">[synchronizationProgress](synchronization-synchronizationprogress.md)集合</span><span class="sxs-lookup"><span data-stu-id="906be-132">[synchronizationProgress](synchronization-synchronizationprogress.md) collection</span></span>|<span data-ttu-id="906be-133">完成作业的进度的详细信息。</span><span class="sxs-lookup"><span data-stu-id="906be-133">Details of the progress of a job toward completion.</span></span>|
|<span data-ttu-id="906be-134">隔离</span><span class="sxs-lookup"><span data-stu-id="906be-134">quarantine</span></span>|[<span data-ttu-id="906be-135">synchronizationQuarantine</span><span class="sxs-lookup"><span data-stu-id="906be-135">synchronizationQuarantine</span></span>](synchronization-quarantine.md)|<span data-ttu-id="906be-136">如果作业在隔离，隔离详细信息。</span><span class="sxs-lookup"><span data-stu-id="906be-136">If job is in quarantine, quarantine details.</span></span>|
|<span data-ttu-id="906be-137">steadyStateFirstAchievedTime</span><span class="sxs-lookup"><span data-stu-id="906be-137">steadyStateFirstAchievedTime</span></span>|<span data-ttu-id="906be-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="906be-138">DateTimeOffset</span></span>|<span data-ttu-id="906be-139">首先达到稳定状态 （过程没有更多更改） 时间。</span><span class="sxs-lookup"><span data-stu-id="906be-139">The time when steady state (no more changes to the process) was first achieved.</span></span> <span data-ttu-id="906be-140">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="906be-140">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="906be-141">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。</span><span class="sxs-lookup"><span data-stu-id="906be-141">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="906be-142">steadyStateLastAchievedTime</span><span class="sxs-lookup"><span data-stu-id="906be-142">steadyStateLastAchievedTime</span></span>|<span data-ttu-id="906be-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="906be-143">DateTimeOffset</span></span>|<span data-ttu-id="906be-144">上次达到稳定状态 （过程没有更多更改） 时间。</span><span class="sxs-lookup"><span data-stu-id="906be-144">The time when steady state (no more changes to the process) was last achieved.</span></span> <span data-ttu-id="906be-145">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="906be-145">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="906be-146">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。</span><span class="sxs-lookup"><span data-stu-id="906be-146">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="906be-147">synchronizedEntryCountByType</span><span class="sxs-lookup"><span data-stu-id="906be-147">synchronizedEntryCountByType</span></span>|<span data-ttu-id="906be-148">[stringKeyLongValuePair](synchronization-stringkeylongvaluepair.md)集合</span><span class="sxs-lookup"><span data-stu-id="906be-148">[stringKeyLongValuePair](synchronization-stringkeylongvaluepair.md) collection</span></span>|<span data-ttu-id="906be-149">按对象类型列出的同步对象数。</span><span class="sxs-lookup"><span data-stu-id="906be-149">Count of synchronized objects, listed by object type.</span></span>|
|<span data-ttu-id="906be-150">troubleshootingUrl</span><span class="sxs-lookup"><span data-stu-id="906be-150">troubleshootingUrl</span></span>|<span data-ttu-id="906be-151">String</span><span class="sxs-lookup"><span data-stu-id="906be-151">String</span></span>|<span data-ttu-id="906be-152">发生错误，带有问题的疑难解答步骤的 URL。</span><span class="sxs-lookup"><span data-stu-id="906be-152">In the event of an error, the URL with the troubleshooting steps for the issue.</span></span>|

### <a name="synchronization-status-code-details"></a><span data-ttu-id="906be-153">同步状态代码的详细信息</span><span class="sxs-lookup"><span data-stu-id="906be-153">Synchronization status code details</span></span>

| <span data-ttu-id="906be-154">值</span><span class="sxs-lookup"><span data-stu-id="906be-154">Value</span></span>                              | <span data-ttu-id="906be-155">说明</span><span class="sxs-lookup"><span data-stu-id="906be-155">Description</span></span>    |
|:-----------------------------------|:---------------|
|<span data-ttu-id="906be-156">NotConfigured</span><span class="sxs-lookup"><span data-stu-id="906be-156">NotConfigured</span></span>                       |<span data-ttu-id="906be-157">作业已未配置，永远不会运行。</span><span class="sxs-lookup"><span data-stu-id="906be-157">Job was not configured and never run.</span></span> <span data-ttu-id="906be-158">提供未授权。</span><span class="sxs-lookup"><span data-stu-id="906be-158">No authorization was provided.</span></span> |
|<span data-ttu-id="906be-159">NotRun</span><span class="sxs-lookup"><span data-stu-id="906be-159">NotRun</span></span>                              |<span data-ttu-id="906be-160">作业已配置并可能启动，但尚未完成其第一个域。</span><span class="sxs-lookup"><span data-stu-id="906be-160">Job was configured, and possibly started, but hasn't completed its first run.</span></span>|
|<span data-ttu-id="906be-161">活动</span><span class="sxs-lookup"><span data-stu-id="906be-161">Active</span></span>                              |<span data-ttu-id="906be-162">定期运行作业。</span><span class="sxs-lookup"><span data-stu-id="906be-162">Job is running periodically.</span></span>|
|<span data-ttu-id="906be-163">暂停</span><span class="sxs-lookup"><span data-stu-id="906be-163">Paused</span></span>                              |<span data-ttu-id="906be-164">作业已暂停 （通常是由管理员） 和当前未运行，但保留作业的状态。</span><span class="sxs-lookup"><span data-stu-id="906be-164">Job was paused (usually by an administrator) and currently is not running, but the state of the job is preserved.</span></span>|
|<span data-ttu-id="906be-165">隔离</span><span class="sxs-lookup"><span data-stu-id="906be-165">Quarantine</span></span>                          |<span data-ttu-id="906be-166">作业处于隔离。</span><span class="sxs-lookup"><span data-stu-id="906be-166">Job is in quarantine.</span></span> <span data-ttu-id="906be-167">有大量的错误，或者关键错误，例如吊销过期凭据时，可能发生此错误。</span><span class="sxs-lookup"><span data-stu-id="906be-167">This might happen when there is a high volume of errors, or critical errors such as revoked/expired credentials.</span></span> <span data-ttu-id="906be-168">在隔离中同步过程将尝试减少频率运行作业。</span><span class="sxs-lookup"><span data-stu-id="906be-168">While in quarantine, the synchronization process will attempt to run the job with reduced frequency.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="906be-169">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="906be-169">JSON representation</span></span>

<span data-ttu-id="906be-170">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="906be-170">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.synchronizationStatus"
}-->

```json
{
  "code": "String",
  "countSuccessiveCompleteFailures": 1024,
  "escrowsPruned": true,
  "lastExecution": {"@odata.type": "microsoft.graph.synchronizationTaskExecution"},
  "lastSuccessfulExecution": {"@odata.type": "microsoft.graph.synchronizationTaskExecution"},
  "lastSuccessfulExecutionWithExports": {"@odata.type": "microsoft.graph.synchronizationTaskExecution"},
  "progress": [{"@odata.type": "microsoft.graph.synchronizationProgress"}],
  "quarantine": {"@odata.type": "microsoft.graph.synchronizationQuarantine"},
  "steadyStateFirstAchievedTime": "String (timestamp)",
  "steadyStateLastAchievedTime": "String (timestamp)",
  "synchronizedEntryCountByType": [{"@odata.type": "microsoft.graph.stringKeyLongValuePair"}],
  "troubleshootingUrl": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "synchronizationStatus resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/synchronization-synchronizationstatus.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
