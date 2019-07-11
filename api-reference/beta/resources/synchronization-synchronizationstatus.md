---
title: synchronizationStatus 资源类型
description: 表示 synchronizationJob 的当前状态。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: fb7c3337933af763ee4f08412ee1b85085f0d380
ms.sourcegitcommit: 121c0fad692fb3c5c01dc051481b5249e4491b48
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/11/2019
ms.locfileid: "35620673"
---
# <a name="synchronizationstatus-resource-type"></a><span data-ttu-id="5513d-103">synchronizationStatus 资源类型</span><span class="sxs-lookup"><span data-stu-id="5513d-103">synchronizationStatus resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5513d-104">表示[synchronizationJob](synchronization-synchronizationjob.md)的当前状态。</span><span class="sxs-lookup"><span data-stu-id="5513d-104">Represents the current status of the [synchronizationJob](synchronization-synchronizationjob.md).</span></span>

## <a name="properties"></a><span data-ttu-id="5513d-105">属性</span><span class="sxs-lookup"><span data-stu-id="5513d-105">Properties</span></span>

| <span data-ttu-id="5513d-106">属性</span><span class="sxs-lookup"><span data-stu-id="5513d-106">Property</span></span>                              | <span data-ttu-id="5513d-107">类型</span><span class="sxs-lookup"><span data-stu-id="5513d-107">Type</span></span>      | <span data-ttu-id="5513d-108">说明</span><span class="sxs-lookup"><span data-stu-id="5513d-108">Description</span></span>    |
|:--------------------------------------|:----------|:---------------|
|<span data-ttu-id="5513d-109">code</span><span class="sxs-lookup"><span data-stu-id="5513d-109">code</span></span>|<span data-ttu-id="5513d-110">String</span><span class="sxs-lookup"><span data-stu-id="5513d-110">String</span></span>|<span data-ttu-id="5513d-111">同步作业的高级别状态代码。</span><span class="sxs-lookup"><span data-stu-id="5513d-111">High-level status code of the synchronization job.</span></span> <span data-ttu-id="5513d-112">可取值为：`NotConfigured`、`NotRun`、`Active`、`Paused`、`Quarantine`。</span><span class="sxs-lookup"><span data-stu-id="5513d-112">Possible values are: `NotConfigured`, `NotRun`, `Active`, `Paused`, `Quarantine`.</span></span>|
|<span data-ttu-id="5513d-113">countSuccessiveCompleteFailures</span><span class="sxs-lookup"><span data-stu-id="5513d-113">countSuccessiveCompleteFailures</span></span>|<span data-ttu-id="5513d-114">Int64</span><span class="sxs-lookup"><span data-stu-id="5513d-114">Int64</span></span>|<span data-ttu-id="5513d-115">此作业连续失败的次数。</span><span class="sxs-lookup"><span data-stu-id="5513d-115">Number of consecutive times this job failed.</span></span>|
|<span data-ttu-id="5513d-116">escrowsPruned</span><span class="sxs-lookup"><span data-stu-id="5513d-116">escrowsPruned</span></span>|<span data-ttu-id="5513d-117">Boolean</span><span class="sxs-lookup"><span data-stu-id="5513d-117">Boolean</span></span>|<span data-ttu-id="5513d-118">`true`在初始同步过程中, 如果作业的 escrows (对象级错误) 被修剪。</span><span class="sxs-lookup"><span data-stu-id="5513d-118">`true` if the job's escrows (object-level errors) were pruned during initial synchronization.</span></span> <span data-ttu-id="5513d-119">在初始同步过程中, 可以对 Escrows 进行修剪, 从而达到通常会将作业放入隔离的错误阈值。</span><span class="sxs-lookup"><span data-stu-id="5513d-119">Escrows can be pruned if during the initial synchronization, you reach the threshold of errors that would normally put the job in quarantine.</span></span> <span data-ttu-id="5513d-120">同步过程不会进入隔离, 而是清除作业的错误并继续, 直到初始同步完成。</span><span class="sxs-lookup"><span data-stu-id="5513d-120">Instead of going into quarantine, the synchronization process clears the job's errors and continues until the initial synchronization is completed.</span></span> <span data-ttu-id="5513d-121">初始同步完成后, 作业将暂停, 并等待客户清除错误。</span><span class="sxs-lookup"><span data-stu-id="5513d-121">When the initial synchronization is completed, the job will pause and wait for the customer to clean up the errors.</span></span>|
|<span data-ttu-id="5513d-122">lastExecution</span><span class="sxs-lookup"><span data-stu-id="5513d-122">lastExecution</span></span>|[<span data-ttu-id="5513d-123">synchronizationTaskExecution</span><span class="sxs-lookup"><span data-stu-id="5513d-123">synchronizationTaskExecution</span></span>](synchronization-synchronizationtaskexecution.md)|<span data-ttu-id="5513d-124">上次执行作业的详细信息。</span><span class="sxs-lookup"><span data-stu-id="5513d-124">Details of the last execution of the job.</span></span>|
|<span data-ttu-id="5513d-125">lastSuccessfulExecution</span><span class="sxs-lookup"><span data-stu-id="5513d-125">lastSuccessfulExecution</span></span>|[<span data-ttu-id="5513d-126">synchronizationTaskExecution</span><span class="sxs-lookup"><span data-stu-id="5513d-126">synchronizationTaskExecution</span></span>](synchronization-synchronizationtaskexecution.md)|<span data-ttu-id="5513d-127">此作业的最后一次执行的详细信息, 其中未包含任何错误。</span><span class="sxs-lookup"><span data-stu-id="5513d-127">Details of the last execution of this job, which didn't have any errors.</span></span>|
|<span data-ttu-id="5513d-128">lastSuccessfulExecutionWithExports</span><span class="sxs-lookup"><span data-stu-id="5513d-128">lastSuccessfulExecutionWithExports</span></span>|[<span data-ttu-id="5513d-129">synchronizationTaskExecution</span><span class="sxs-lookup"><span data-stu-id="5513d-129">synchronizationTaskExecution</span></span>](synchronization-synchronizationtaskexecution.md)|<span data-ttu-id="5513d-130">上次执行作业的详细信息, 该作业将对象导出到目标目录中。</span><span class="sxs-lookup"><span data-stu-id="5513d-130">Details of the last execution of the job, which exported objects into the target directory.</span></span>|
|<span data-ttu-id="5513d-131">progress</span><span class="sxs-lookup"><span data-stu-id="5513d-131">progress</span></span>|<span data-ttu-id="5513d-132">[synchronizationProgress](synchronization-synchronizationprogress.md)集合</span><span class="sxs-lookup"><span data-stu-id="5513d-132">[synchronizationProgress](synchronization-synchronizationprogress.md) collection</span></span>|<span data-ttu-id="5513d-133">完成作业进度的详细信息。</span><span class="sxs-lookup"><span data-stu-id="5513d-133">Details of the progress of a job toward completion.</span></span>|
|<span data-ttu-id="5513d-134">隔离</span><span class="sxs-lookup"><span data-stu-id="5513d-134">quarantine</span></span>|[<span data-ttu-id="5513d-135">synchronizationQuarantine</span><span class="sxs-lookup"><span data-stu-id="5513d-135">synchronizationQuarantine</span></span>](synchronization-quarantine.md)|<span data-ttu-id="5513d-136">如果作业在隔离中, 则隔离详细信息。</span><span class="sxs-lookup"><span data-stu-id="5513d-136">If job is in quarantine, quarantine details.</span></span>|
|<span data-ttu-id="5513d-137">steadyStateFirstAchievedTime</span><span class="sxs-lookup"><span data-stu-id="5513d-137">steadyStateFirstAchievedTime</span></span>|<span data-ttu-id="5513d-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5513d-138">DateTimeOffset</span></span>|<span data-ttu-id="5513d-139">稳定状态 (不再对进程所做的更改) 第一次实现的时间。</span><span class="sxs-lookup"><span data-stu-id="5513d-139">The time when steady state (no more changes to the process) was first achieved.</span></span> <span data-ttu-id="5513d-140">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="5513d-140">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="5513d-141">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。</span><span class="sxs-lookup"><span data-stu-id="5513d-141">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="5513d-142">steadyStateLastAchievedTime</span><span class="sxs-lookup"><span data-stu-id="5513d-142">steadyStateLastAchievedTime</span></span>|<span data-ttu-id="5513d-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5513d-143">DateTimeOffset</span></span>|<span data-ttu-id="5513d-144">上次达到稳定状态 (不再对进程所做的更改) 的时间。</span><span class="sxs-lookup"><span data-stu-id="5513d-144">The time when steady state (no more changes to the process) was last achieved.</span></span> <span data-ttu-id="5513d-145">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="5513d-145">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="5513d-146">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。</span><span class="sxs-lookup"><span data-stu-id="5513d-146">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="5513d-147">synchronizedEntryCountByType</span><span class="sxs-lookup"><span data-stu-id="5513d-147">synchronizedEntryCountByType</span></span>|<span data-ttu-id="5513d-148">[stringKeyLongValuePair](synchronization-stringkeylongvaluepair.md)集合</span><span class="sxs-lookup"><span data-stu-id="5513d-148">[stringKeyLongValuePair](synchronization-stringkeylongvaluepair.md) collection</span></span>|<span data-ttu-id="5513d-149">按对象类型列出的已同步对象的计数。</span><span class="sxs-lookup"><span data-stu-id="5513d-149">Count of synchronized objects, listed by object type.</span></span>|
|<span data-ttu-id="5513d-150">troubleshootingUrl</span><span class="sxs-lookup"><span data-stu-id="5513d-150">troubleshootingUrl</span></span>|<span data-ttu-id="5513d-151">String</span><span class="sxs-lookup"><span data-stu-id="5513d-151">String</span></span>|<span data-ttu-id="5513d-152">出现错误时, 将包含问题的故障排除步骤的 URL。</span><span class="sxs-lookup"><span data-stu-id="5513d-152">In the event of an error, the URL with the troubleshooting steps for the issue.</span></span>|

### <a name="synchronization-status-code-details"></a><span data-ttu-id="5513d-153">同步状态代码详细信息</span><span class="sxs-lookup"><span data-stu-id="5513d-153">Synchronization status code details</span></span>

| <span data-ttu-id="5513d-154">值</span><span class="sxs-lookup"><span data-stu-id="5513d-154">Value</span></span>                              | <span data-ttu-id="5513d-155">说明</span><span class="sxs-lookup"><span data-stu-id="5513d-155">Description</span></span>    |
|:-----------------------------------|:---------------|
|<span data-ttu-id="5513d-156">NotConfigured</span><span class="sxs-lookup"><span data-stu-id="5513d-156">NotConfigured</span></span>                       |<span data-ttu-id="5513d-157">作业未配置且从未运行。</span><span class="sxs-lookup"><span data-stu-id="5513d-157">Job was not configured and never run.</span></span> <span data-ttu-id="5513d-158">未提供任何授权。</span><span class="sxs-lookup"><span data-stu-id="5513d-158">No authorization was provided.</span></span> |
|<span data-ttu-id="5513d-159">NotRun</span><span class="sxs-lookup"><span data-stu-id="5513d-159">NotRun</span></span>                              |<span data-ttu-id="5513d-160">作业已配置且可能已启动, 但尚未完成其第一次运行。</span><span class="sxs-lookup"><span data-stu-id="5513d-160">Job was configured, and possibly started, but hasn't completed its first run.</span></span>|
|<span data-ttu-id="5513d-161">活动</span><span class="sxs-lookup"><span data-stu-id="5513d-161">Active</span></span>                              |<span data-ttu-id="5513d-162">作业正在定期运行。</span><span class="sxs-lookup"><span data-stu-id="5513d-162">Job is running periodically.</span></span>|
|<span data-ttu-id="5513d-163">暂停</span><span class="sxs-lookup"><span data-stu-id="5513d-163">Paused</span></span>                              |<span data-ttu-id="5513d-164">作业已暂停 (通常由管理员执行), 当前未在运行, 但保留作业的状态。</span><span class="sxs-lookup"><span data-stu-id="5513d-164">Job was paused (usually by an administrator) and currently is not running, but the state of the job is preserved.</span></span>|
|<span data-ttu-id="5513d-165">隔离</span><span class="sxs-lookup"><span data-stu-id="5513d-165">Quarantine</span></span>                          |<span data-ttu-id="5513d-166">作业处于隔离中。</span><span class="sxs-lookup"><span data-stu-id="5513d-166">Job is in quarantine.</span></span> <span data-ttu-id="5513d-167">当出现大量错误或严重错误 (如已吊销/已过期的凭据) 时, 可能会发生这种情况。</span><span class="sxs-lookup"><span data-stu-id="5513d-167">This might happen when there is a high volume of errors, or critical errors such as revoked/expired credentials.</span></span> <span data-ttu-id="5513d-168">在隔离过程中, 同步过程将尝试以降低的频率运行作业。</span><span class="sxs-lookup"><span data-stu-id="5513d-168">While in quarantine, the synchronization process will attempt to run the job with reduced frequency.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="5513d-169">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5513d-169">JSON representation</span></span>

<span data-ttu-id="5513d-170">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5513d-170">The following is a JSON representation of the resource.</span></span>

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
  "suppressions": []
}
-->
