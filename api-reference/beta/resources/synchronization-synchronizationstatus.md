---
title: synchronizationStatus 资源类型
description: 代表 synchronizationJob 的当前状态。
localization_priority: Normal
ms.openlocfilehash: 01f30338d7f6d4388554df08bf91655136c24a12
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27817029"
---
# <a name="synchronizationstatus-resource-type"></a><span data-ttu-id="26246-103">synchronizationStatus 资源类型</span><span class="sxs-lookup"><span data-stu-id="26246-103">synchronizationStatus resource type</span></span>

> <span data-ttu-id="26246-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="26246-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="26246-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="26246-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="26246-106">代表[synchronizationJob](synchronization-synchronizationjob.md)的当前状态。</span><span class="sxs-lookup"><span data-stu-id="26246-106">Represents the current status of the [synchronizationJob](synchronization-synchronizationjob.md).</span></span>

## <a name="properties"></a><span data-ttu-id="26246-107">属性</span><span class="sxs-lookup"><span data-stu-id="26246-107">Properties</span></span>

| <span data-ttu-id="26246-108">属性</span><span class="sxs-lookup"><span data-stu-id="26246-108">Property</span></span>                              | <span data-ttu-id="26246-109">类型</span><span class="sxs-lookup"><span data-stu-id="26246-109">Type</span></span>      | <span data-ttu-id="26246-110">说明</span><span class="sxs-lookup"><span data-stu-id="26246-110">Description</span></span>    |
|:--------------------------------------|:----------|:---------------|
|<span data-ttu-id="26246-111">code</span><span class="sxs-lookup"><span data-stu-id="26246-111">code</span></span>|<span data-ttu-id="26246-112">字符串</span><span class="sxs-lookup"><span data-stu-id="26246-112">String</span></span>|<span data-ttu-id="26246-113">高级状态代码的同步作业。</span><span class="sxs-lookup"><span data-stu-id="26246-113">High-level status code of the synchronization job.</span></span> <span data-ttu-id="26246-114">可取值为：`NotConfigured`、`NotRun`、`Active`、`Paused`、`Quarantine`。</span><span class="sxs-lookup"><span data-stu-id="26246-114">Possible values are: `NotConfigured`, `NotRun`, `Active`, `Paused`, `Quarantine`.</span></span>|
|<span data-ttu-id="26246-115">countSuccessiveCompleteFailures</span><span class="sxs-lookup"><span data-stu-id="26246-115">countSuccessiveCompleteFailures</span></span>|<span data-ttu-id="26246-116">Int64</span><span class="sxs-lookup"><span data-stu-id="26246-116">Int64</span></span>|<span data-ttu-id="26246-117">连续次数此作业失败。</span><span class="sxs-lookup"><span data-stu-id="26246-117">Number of consecutive times this job failed.</span></span>|
|<span data-ttu-id="26246-118">escrowsPruned</span><span class="sxs-lookup"><span data-stu-id="26246-118">escrowsPruned</span></span>|<span data-ttu-id="26246-119">布尔</span><span class="sxs-lookup"><span data-stu-id="26246-119">Boolean</span></span>|<span data-ttu-id="26246-120">`true`如果在初始同步期间已修剪作业的 escrows （对象级错误）。</span><span class="sxs-lookup"><span data-stu-id="26246-120">`true` if the job's escrows (object-level errors) were pruned during initial synchronization.</span></span> <span data-ttu-id="26246-121">如果在初始同步过程达到阈值通常会将作业放在隔离的错误，则可以修剪 escrows。</span><span class="sxs-lookup"><span data-stu-id="26246-121">Escrows can be pruned if during the initial synchronization, you reach the threshold of errors that would normally put the job in quarantine.</span></span> <span data-ttu-id="26246-122">而不是进入隔离，同步过程清除作业的错误，并将继续，直到完成初始同步。</span><span class="sxs-lookup"><span data-stu-id="26246-122">Instead of going into quarantine, the synchronization process clears the job's errors and continues until the initial synchronization is completed.</span></span> <span data-ttu-id="26246-123">完成初始同步后，此作业将暂停并等待客户清理错误。</span><span class="sxs-lookup"><span data-stu-id="26246-123">When the initial synchronization is completed, the job will pause and wait for the customer to clean up the errors.</span></span>|
|<span data-ttu-id="26246-124">lastExecution</span><span class="sxs-lookup"><span data-stu-id="26246-124">lastExecution</span></span>|[<span data-ttu-id="26246-125">synchronizationTaskExecution</span><span class="sxs-lookup"><span data-stu-id="26246-125">synchronizationTaskExecution</span></span>](synchronization-synchronizationtaskexecution.md)|<span data-ttu-id="26246-126">上次执行作业的详细信息。</span><span class="sxs-lookup"><span data-stu-id="26246-126">Details of the last execution of the job.</span></span>|
|<span data-ttu-id="26246-127">lastSuccessfulExecution</span><span class="sxs-lookup"><span data-stu-id="26246-127">lastSuccessfulExecution</span></span>|[<span data-ttu-id="26246-128">synchronizationTaskExecution</span><span class="sxs-lookup"><span data-stu-id="26246-128">synchronizationTaskExecution</span></span>](synchronization-synchronizationtaskexecution.md)|<span data-ttu-id="26246-129">上次执行此作业，没有任何错误的详细信息。</span><span class="sxs-lookup"><span data-stu-id="26246-129">Details of the last execution of this job, which didn't have any errors.</span></span>|
|<span data-ttu-id="26246-130">lastSuccessfulExecutionWithExports</span><span class="sxs-lookup"><span data-stu-id="26246-130">lastSuccessfulExecutionWithExports</span></span>|[<span data-ttu-id="26246-131">synchronizationTaskExecution</span><span class="sxs-lookup"><span data-stu-id="26246-131">synchronizationTaskExecution</span></span>](synchronization-synchronizationtaskexecution.md)|<span data-ttu-id="26246-132">导出到目标目录的对象的作业的上次执行的详细信息。</span><span class="sxs-lookup"><span data-stu-id="26246-132">Details of the last execution of the job, which exported objects into the target directory.</span></span>|
|<span data-ttu-id="26246-133">进度</span><span class="sxs-lookup"><span data-stu-id="26246-133">progress</span></span>|<span data-ttu-id="26246-134">[synchronizationProgress](synchronization-synchronizationprogress.md)集合</span><span class="sxs-lookup"><span data-stu-id="26246-134">[synchronizationProgress](synchronization-synchronizationprogress.md) collection</span></span>|<span data-ttu-id="26246-135">完成作业的进度的详细信息。</span><span class="sxs-lookup"><span data-stu-id="26246-135">Details of the progress of a job toward completion.</span></span>|
|<span data-ttu-id="26246-136">隔离</span><span class="sxs-lookup"><span data-stu-id="26246-136">quarantine</span></span>|[<span data-ttu-id="26246-137">synchronizationQuarantine</span><span class="sxs-lookup"><span data-stu-id="26246-137">synchronizationQuarantine</span></span>](synchronization-quarantine.md)|<span data-ttu-id="26246-138">如果作业在隔离，隔离详细信息。</span><span class="sxs-lookup"><span data-stu-id="26246-138">If job is in quarantine, quarantine details.</span></span>|
|<span data-ttu-id="26246-139">steadyStateFirstAchievedTime</span><span class="sxs-lookup"><span data-stu-id="26246-139">steadyStateFirstAchievedTime</span></span>|<span data-ttu-id="26246-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="26246-140">DateTimeOffset</span></span>|<span data-ttu-id="26246-141">首先达到稳定状态 （过程没有更多更改） 时间。</span><span class="sxs-lookup"><span data-stu-id="26246-141">The time when steady state (no more changes to the process) was first achieved.</span></span> <span data-ttu-id="26246-142">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="26246-142">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="26246-143">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。</span><span class="sxs-lookup"><span data-stu-id="26246-143">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="26246-144">steadyStateLastAchievedTime</span><span class="sxs-lookup"><span data-stu-id="26246-144">steadyStateLastAchievedTime</span></span>|<span data-ttu-id="26246-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="26246-145">DateTimeOffset</span></span>|<span data-ttu-id="26246-146">上次达到稳定状态 （过程没有更多更改） 时间。</span><span class="sxs-lookup"><span data-stu-id="26246-146">The time when steady state (no more changes to the process) was last achieved.</span></span> <span data-ttu-id="26246-147">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="26246-147">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="26246-148">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。</span><span class="sxs-lookup"><span data-stu-id="26246-148">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="26246-149">synchronizedEntryCountByType</span><span class="sxs-lookup"><span data-stu-id="26246-149">synchronizedEntryCountByType</span></span>|<span data-ttu-id="26246-150">[stringKeyLongValuePair](synchronization-stringkeylongvaluepair.md)集合</span><span class="sxs-lookup"><span data-stu-id="26246-150">[stringKeyLongValuePair](synchronization-stringkeylongvaluepair.md) collection</span></span>|<span data-ttu-id="26246-151">按对象类型列出的同步对象数。</span><span class="sxs-lookup"><span data-stu-id="26246-151">Count of synchronized objects, listed by object type.</span></span>|
|<span data-ttu-id="26246-152">troubleshootingUrl</span><span class="sxs-lookup"><span data-stu-id="26246-152">troubleshootingUrl</span></span>|<span data-ttu-id="26246-153">字符串</span><span class="sxs-lookup"><span data-stu-id="26246-153">String</span></span>|<span data-ttu-id="26246-154">发生错误，带有问题的疑难解答步骤的 URL。</span><span class="sxs-lookup"><span data-stu-id="26246-154">In the event of an error, the URL with the troubleshooting steps for the issue.</span></span>|

### <a name="synchronization-status-code-details"></a><span data-ttu-id="26246-155">同步状态代码的详细信息</span><span class="sxs-lookup"><span data-stu-id="26246-155">Synchronization status code details</span></span>

| <span data-ttu-id="26246-156">值</span><span class="sxs-lookup"><span data-stu-id="26246-156">Value</span></span>                              | <span data-ttu-id="26246-157">Description</span><span class="sxs-lookup"><span data-stu-id="26246-157">Description</span></span>    |
|:-----------------------------------|:---------------|
|<span data-ttu-id="26246-158">NotConfigured</span><span class="sxs-lookup"><span data-stu-id="26246-158">NotConfigured</span></span>                       |<span data-ttu-id="26246-159">作业已未配置，永远不会运行。</span><span class="sxs-lookup"><span data-stu-id="26246-159">Job was not configured and never run.</span></span> <span data-ttu-id="26246-160">提供未授权。</span><span class="sxs-lookup"><span data-stu-id="26246-160">No authorization was provided.</span></span> |
|<span data-ttu-id="26246-161">NotRun</span><span class="sxs-lookup"><span data-stu-id="26246-161">NotRun</span></span>                              |<span data-ttu-id="26246-162">作业已配置并可能启动，但尚未完成其第一个域。</span><span class="sxs-lookup"><span data-stu-id="26246-162">Job was configured, and possibly started, but hasn't completed its first run.</span></span>|
|<span data-ttu-id="26246-163">活动</span><span class="sxs-lookup"><span data-stu-id="26246-163">Active</span></span>                              |<span data-ttu-id="26246-164">定期运行作业。</span><span class="sxs-lookup"><span data-stu-id="26246-164">Job is running periodically.</span></span>|
|<span data-ttu-id="26246-165">暂停</span><span class="sxs-lookup"><span data-stu-id="26246-165">Paused</span></span>                              |<span data-ttu-id="26246-166">作业已暂停 （通常是由管理员） 和当前未运行，但保留作业的状态。</span><span class="sxs-lookup"><span data-stu-id="26246-166">Job was paused (usually by an administrator) and currently is not running, but the state of the job is preserved.</span></span>|
|<span data-ttu-id="26246-167">隔离</span><span class="sxs-lookup"><span data-stu-id="26246-167">Quarantine</span></span>                          |<span data-ttu-id="26246-168">作业处于隔离。</span><span class="sxs-lookup"><span data-stu-id="26246-168">Job is in quarantine.</span></span> <span data-ttu-id="26246-169">有大量的错误，或者关键错误，例如吊销过期凭据时，可能发生此错误。</span><span class="sxs-lookup"><span data-stu-id="26246-169">This might happen when there is a high volume of errors, or critical errors such as revoked/expired credentials.</span></span> <span data-ttu-id="26246-170">在隔离中同步过程将尝试减少频率运行作业。</span><span class="sxs-lookup"><span data-stu-id="26246-170">While in quarantine, the synchronization process will attempt to run the job with reduced frequency.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="26246-171">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="26246-171">JSON representation</span></span>

<span data-ttu-id="26246-172">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="26246-172">The following is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "synchronizationStatus resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
