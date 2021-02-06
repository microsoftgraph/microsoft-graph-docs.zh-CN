---
title: synchronizationStatus 资源类型
description: 表示 synchronizationJob 的当前状态。
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: applications
ms.openlocfilehash: bb832fa8d62f2c666b430c242a49bd9138de1b57
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50135049"
---
# <a name="synchronizationstatus-resource-type"></a><span data-ttu-id="45e71-103">synchronizationStatus 资源类型</span><span class="sxs-lookup"><span data-stu-id="45e71-103">synchronizationStatus resource type</span></span>

<span data-ttu-id="45e71-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="45e71-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="45e71-105">表示 [synchronizationJob 的当前状态](synchronization-synchronizationjob.md)。</span><span class="sxs-lookup"><span data-stu-id="45e71-105">Represents the current status of the [synchronizationJob](synchronization-synchronizationjob.md).</span></span>

## <a name="properties"></a><span data-ttu-id="45e71-106">属性</span><span class="sxs-lookup"><span data-stu-id="45e71-106">Properties</span></span>

| <span data-ttu-id="45e71-107">属性</span><span class="sxs-lookup"><span data-stu-id="45e71-107">Property</span></span>                              | <span data-ttu-id="45e71-108">类型</span><span class="sxs-lookup"><span data-stu-id="45e71-108">Type</span></span>      | <span data-ttu-id="45e71-109">说明</span><span class="sxs-lookup"><span data-stu-id="45e71-109">Description</span></span>    |
|:--------------------------------------|:----------|:---------------|
|<span data-ttu-id="45e71-110">code</span><span class="sxs-lookup"><span data-stu-id="45e71-110">code</span></span>|<span data-ttu-id="45e71-111">字符串</span><span class="sxs-lookup"><span data-stu-id="45e71-111">String</span></span>|<span data-ttu-id="45e71-112">同步作业的高级别状态代码。</span><span class="sxs-lookup"><span data-stu-id="45e71-112">High-level status code of the synchronization job.</span></span> <span data-ttu-id="45e71-113">可取值为：`NotConfigured`、`NotRun`、`Active`、`Paused`、`Quarantine`。</span><span class="sxs-lookup"><span data-stu-id="45e71-113">Possible values are: `NotConfigured`, `NotRun`, `Active`, `Paused`, `Quarantine`.</span></span>|
|<span data-ttu-id="45e71-114">countSuccessiveCompleteFailures</span><span class="sxs-lookup"><span data-stu-id="45e71-114">countSuccessiveCompleteFailures</span></span>|<span data-ttu-id="45e71-115">Int64</span><span class="sxs-lookup"><span data-stu-id="45e71-115">Int64</span></span>|<span data-ttu-id="45e71-116">此作业失败的连续次数。</span><span class="sxs-lookup"><span data-stu-id="45e71-116">Number of consecutive times this job failed.</span></span>|
|<span data-ttu-id="45e71-117">escrowsPruned</span><span class="sxs-lookup"><span data-stu-id="45e71-117">escrowsPruned</span></span>|<span data-ttu-id="45e71-118">Boolean</span><span class="sxs-lookup"><span data-stu-id="45e71-118">Boolean</span></span>|<span data-ttu-id="45e71-119">`true` 如果作业的托管 (对象级错误) 初始同步期间被修剪。</span><span class="sxs-lookup"><span data-stu-id="45e71-119">`true` if the job's escrows (object-level errors) were pruned during initial synchronization.</span></span> <span data-ttu-id="45e71-120">如果在初始同步期间达到通常将作业置于隔离状态的错误阈值，可以删除托管。</span><span class="sxs-lookup"><span data-stu-id="45e71-120">Escrows can be pruned if during the initial synchronization, you reach the threshold of errors that would normally put the job in quarantine.</span></span> <span data-ttu-id="45e71-121">同步过程不会进入隔离区，而是清除作业的错误并继续，直到初始同步完成。</span><span class="sxs-lookup"><span data-stu-id="45e71-121">Instead of going into quarantine, the synchronization process clears the job's errors and continues until the initial synchronization is completed.</span></span> <span data-ttu-id="45e71-122">初始同步完成后，作业将暂停并等待客户清理错误。</span><span class="sxs-lookup"><span data-stu-id="45e71-122">When the initial synchronization is completed, the job will pause and wait for the customer to clean up the errors.</span></span>|
|<span data-ttu-id="45e71-123">lastExecution</span><span class="sxs-lookup"><span data-stu-id="45e71-123">lastExecution</span></span>|[<span data-ttu-id="45e71-124">synchronizationTaskExecution</span><span class="sxs-lookup"><span data-stu-id="45e71-124">synchronizationTaskExecution</span></span>](synchronization-synchronizationtaskexecution.md)|<span data-ttu-id="45e71-125">上次执行作业的详细信息。</span><span class="sxs-lookup"><span data-stu-id="45e71-125">Details of the last execution of the job.</span></span>|
|<span data-ttu-id="45e71-126">lastSuccessfulExecution</span><span class="sxs-lookup"><span data-stu-id="45e71-126">lastSuccessfulExecution</span></span>|[<span data-ttu-id="45e71-127">synchronizationTaskExecution</span><span class="sxs-lookup"><span data-stu-id="45e71-127">synchronizationTaskExecution</span></span>](synchronization-synchronizationtaskexecution.md)|<span data-ttu-id="45e71-128">上次执行此作业的详细信息，没有任何错误。</span><span class="sxs-lookup"><span data-stu-id="45e71-128">Details of the last execution of this job, which didn't have any errors.</span></span>|
|<span data-ttu-id="45e71-129">lastSuccessfulExecutionWithExports</span><span class="sxs-lookup"><span data-stu-id="45e71-129">lastSuccessfulExecutionWithExports</span></span>|[<span data-ttu-id="45e71-130">synchronizationTaskExecution</span><span class="sxs-lookup"><span data-stu-id="45e71-130">synchronizationTaskExecution</span></span>](synchronization-synchronizationtaskexecution.md)|<span data-ttu-id="45e71-131">上次执行作业的详细信息，该作业将对象导出到目标目录中。</span><span class="sxs-lookup"><span data-stu-id="45e71-131">Details of the last execution of the job, which exported objects into the target directory.</span></span>|
|<span data-ttu-id="45e71-132">progress</span><span class="sxs-lookup"><span data-stu-id="45e71-132">progress</span></span>|<span data-ttu-id="45e71-133">[synchronizationProgress](synchronization-synchronizationprogress.md) 集合</span><span class="sxs-lookup"><span data-stu-id="45e71-133">[synchronizationProgress](synchronization-synchronizationprogress.md) collection</span></span>|<span data-ttu-id="45e71-134">完成作业的进度的详细信息。</span><span class="sxs-lookup"><span data-stu-id="45e71-134">Details of the progress of a job toward completion.</span></span>|
|<span data-ttu-id="45e71-135">隔离</span><span class="sxs-lookup"><span data-stu-id="45e71-135">quarantine</span></span>|[<span data-ttu-id="45e71-136">synchronizationQuarantine</span><span class="sxs-lookup"><span data-stu-id="45e71-136">synchronizationQuarantine</span></span>](synchronization-quarantine.md)|<span data-ttu-id="45e71-137">如果作业位于隔离区中，则隔离详细信息。</span><span class="sxs-lookup"><span data-stu-id="45e71-137">If job is in quarantine, quarantine details.</span></span>|
|<span data-ttu-id="45e71-138">steadyStateFirstAchievedTime</span><span class="sxs-lookup"><span data-stu-id="45e71-138">steadyStateFirstAchievedTime</span></span>|<span data-ttu-id="45e71-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="45e71-139">DateTimeOffset</span></span>|<span data-ttu-id="45e71-140">达到稳定状态 (第一次实现) 更改的时间。</span><span class="sxs-lookup"><span data-stu-id="45e71-140">The time when steady state (no more changes to the process) was first achieved.</span></span> <span data-ttu-id="45e71-141">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="45e71-141">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="45e71-142">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。</span><span class="sxs-lookup"><span data-stu-id="45e71-142">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="45e71-143">steadyStateLastAchievedTime</span><span class="sxs-lookup"><span data-stu-id="45e71-143">steadyStateLastAchievedTime</span></span>|<span data-ttu-id="45e71-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="45e71-144">DateTimeOffset</span></span>|<span data-ttu-id="45e71-145">上次达到稳定 (对进程更改) 的时间。</span><span class="sxs-lookup"><span data-stu-id="45e71-145">The time when steady state (no more changes to the process) was last achieved.</span></span> <span data-ttu-id="45e71-146">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="45e71-146">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="45e71-147">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。</span><span class="sxs-lookup"><span data-stu-id="45e71-147">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="45e71-148">synchronizedEntryCountByType</span><span class="sxs-lookup"><span data-stu-id="45e71-148">synchronizedEntryCountByType</span></span>|<span data-ttu-id="45e71-149">[stringKeyLongValuePair](synchronization-stringkeylongvaluepair.md) 集合</span><span class="sxs-lookup"><span data-stu-id="45e71-149">[stringKeyLongValuePair](synchronization-stringkeylongvaluepair.md) collection</span></span>|<span data-ttu-id="45e71-150">同步对象计数，按对象类型。</span><span class="sxs-lookup"><span data-stu-id="45e71-150">Count of synchronized objects, listed by object type.</span></span>|
|<span data-ttu-id="45e71-151">troubleshootingUrl</span><span class="sxs-lookup"><span data-stu-id="45e71-151">troubleshootingUrl</span></span>|<span data-ttu-id="45e71-152">字符串</span><span class="sxs-lookup"><span data-stu-id="45e71-152">String</span></span>|<span data-ttu-id="45e71-153">如果出现错误，URL 将包含问题的疑难解答步骤。</span><span class="sxs-lookup"><span data-stu-id="45e71-153">In the event of an error, the URL with the troubleshooting steps for the issue.</span></span>|

### <a name="synchronization-status-code-details"></a><span data-ttu-id="45e71-154">同步状态代码详细信息</span><span class="sxs-lookup"><span data-stu-id="45e71-154">Synchronization status code details</span></span>

| <span data-ttu-id="45e71-155">值</span><span class="sxs-lookup"><span data-stu-id="45e71-155">Value</span></span>                              | <span data-ttu-id="45e71-156">说明</span><span class="sxs-lookup"><span data-stu-id="45e71-156">Description</span></span>    |
|:-----------------------------------|:---------------|
|<span data-ttu-id="45e71-157">NotConfigured</span><span class="sxs-lookup"><span data-stu-id="45e71-157">NotConfigured</span></span>                       |<span data-ttu-id="45e71-158">作业未配置且从不运行。</span><span class="sxs-lookup"><span data-stu-id="45e71-158">Job was not configured and never run.</span></span> <span data-ttu-id="45e71-159">未提供授权。</span><span class="sxs-lookup"><span data-stu-id="45e71-159">No authorization was provided.</span></span> |
|<span data-ttu-id="45e71-160">NotRun</span><span class="sxs-lookup"><span data-stu-id="45e71-160">NotRun</span></span>                              |<span data-ttu-id="45e71-161">作业已配置，可能已启动，但尚未完成首次运行。</span><span class="sxs-lookup"><span data-stu-id="45e71-161">Job was configured, and possibly started, but hasn't completed its first run.</span></span>|
|<span data-ttu-id="45e71-162">活动</span><span class="sxs-lookup"><span data-stu-id="45e71-162">Active</span></span>                              |<span data-ttu-id="45e71-163">作业定期运行。</span><span class="sxs-lookup"><span data-stu-id="45e71-163">Job is running periodically.</span></span>|
|<span data-ttu-id="45e71-164">暂停</span><span class="sxs-lookup"><span data-stu-id="45e71-164">Paused</span></span>                              |<span data-ttu-id="45e71-165">作业已暂停 (管理员) 当前未运行，但保留作业的状态。</span><span class="sxs-lookup"><span data-stu-id="45e71-165">Job was paused (usually by an administrator) and currently is not running, but the state of the job is preserved.</span></span>|
|<span data-ttu-id="45e71-166">Quarantine</span><span class="sxs-lookup"><span data-stu-id="45e71-166">Quarantine</span></span>                          |<span data-ttu-id="45e71-167">作业被隔离。</span><span class="sxs-lookup"><span data-stu-id="45e71-167">Job is in quarantine.</span></span> <span data-ttu-id="45e71-168">当存在大量错误或关键错误（如吊销/过期的凭据）时，可能会发生这种情况。</span><span class="sxs-lookup"><span data-stu-id="45e71-168">This might happen when there is a high volume of errors, or critical errors such as revoked/expired credentials.</span></span> <span data-ttu-id="45e71-169">隔离时，同步过程将尝试以降低的频率运行作业。</span><span class="sxs-lookup"><span data-stu-id="45e71-169">While in quarantine, the synchronization process will attempt to run the job with reduced frequency.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="45e71-170">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="45e71-170">JSON representation</span></span>

<span data-ttu-id="45e71-171">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="45e71-171">The following is a JSON representation of the resource.</span></span>

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


