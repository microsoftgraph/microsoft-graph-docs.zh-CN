---
title: synchronizationTaskExecution 资源类型
description: 概述同步作业的运行结果。
localization_priority: Normal
ms.openlocfilehash: a9008dd7d51a1d07be75c5b9bbad34d636fff74c
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33339823"
---
# <a name="synchronizationtaskexecution-resource-type"></a><span data-ttu-id="6b48f-103">synchronizationTaskExecution 资源类型</span><span class="sxs-lookup"><span data-stu-id="6b48f-103">synchronizationTaskExecution resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6b48f-104">概述同步作业的运行结果。</span><span class="sxs-lookup"><span data-stu-id="6b48f-104">Summarizes the results of the synchronization job run.</span></span>

## <a name="properties"></a><span data-ttu-id="6b48f-105">属性</span><span class="sxs-lookup"><span data-stu-id="6b48f-105">Properties</span></span>
| <span data-ttu-id="6b48f-106">属性</span><span class="sxs-lookup"><span data-stu-id="6b48f-106">Property</span></span>     | <span data-ttu-id="6b48f-107">类型</span><span class="sxs-lookup"><span data-stu-id="6b48f-107">Type</span></span>   |<span data-ttu-id="6b48f-108">说明</span><span class="sxs-lookup"><span data-stu-id="6b48f-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6b48f-109">activityIdentifier</span><span class="sxs-lookup"><span data-stu-id="6b48f-109">activityIdentifier</span></span>           |<span data-ttu-id="6b48f-110">String</span><span class="sxs-lookup"><span data-stu-id="6b48f-110">String</span></span> |<span data-ttu-id="6b48f-111">作业运行的标识符。</span><span class="sxs-lookup"><span data-stu-id="6b48f-111">Identifier of the job run.</span></span>|
|<span data-ttu-id="6b48f-112">countEntitled</span><span class="sxs-lookup"><span data-stu-id="6b48f-112">countEntitled</span></span>                |<span data-ttu-id="6b48f-113">Int64</span><span class="sxs-lookup"><span data-stu-id="6b48f-113">Int64</span></span>  |<span data-ttu-id="6b48f-114">为此应用程序分配的已处理项的计数。</span><span class="sxs-lookup"><span data-stu-id="6b48f-114">Count of processed entries that were assigned for this application.</span></span>|
|<span data-ttu-id="6b48f-115">countEntitledForProvisioning</span><span class="sxs-lookup"><span data-stu-id="6b48f-115">countEntitledForProvisioning</span></span> |<span data-ttu-id="6b48f-116">Int64</span><span class="sxs-lookup"><span data-stu-id="6b48f-116">Int64</span></span>  |<span data-ttu-id="6b48f-117">为设置分配的已处理项的计数。</span><span class="sxs-lookup"><span data-stu-id="6b48f-117">Count of processed entries that were assigned for provisioning.</span></span>|
|<span data-ttu-id="6b48f-118">countEscrowed</span><span class="sxs-lookup"><span data-stu-id="6b48f-118">countEscrowed</span></span>                |<span data-ttu-id="6b48f-119">Int64</span><span class="sxs-lookup"><span data-stu-id="6b48f-119">Int64</span></span>  |<span data-ttu-id="6b48f-120">escrowed (错误) 的项的计数。</span><span class="sxs-lookup"><span data-stu-id="6b48f-120">Count of entries that were escrowed (errors).</span></span>|
|<span data-ttu-id="6b48f-121">countEscrowedRaw</span><span class="sxs-lookup"><span data-stu-id="6b48f-121">countEscrowedRaw</span></span>             |<span data-ttu-id="6b48f-122">Int64</span><span class="sxs-lookup"><span data-stu-id="6b48f-122">Int64</span></span>  |<span data-ttu-id="6b48f-123">escrowed 的条目数, 包括系统生成的 escrows。</span><span class="sxs-lookup"><span data-stu-id="6b48f-123">Count of entries that were escrowed, including system-generated escrows.</span></span>|
|<span data-ttu-id="6b48f-124">countExported</span><span class="sxs-lookup"><span data-stu-id="6b48f-124">countExported</span></span>                |<span data-ttu-id="6b48f-125">Int64</span><span class="sxs-lookup"><span data-stu-id="6b48f-125">Int64</span></span>  |<span data-ttu-id="6b48f-126">已导出条目的计数。</span><span class="sxs-lookup"><span data-stu-id="6b48f-126">Count of exported entries.</span></span>|
|<span data-ttu-id="6b48f-127">countExports</span><span class="sxs-lookup"><span data-stu-id="6b48f-127">countExports</span></span>                 |<span data-ttu-id="6b48f-128">Int64</span><span class="sxs-lookup"><span data-stu-id="6b48f-128">Int64</span></span>  |<span data-ttu-id="6b48f-129">预期要导出的条目数。</span><span class="sxs-lookup"><span data-stu-id="6b48f-129">Count of entries that were expected to be exported.</span></span>|
|<span data-ttu-id="6b48f-130">countImported</span><span class="sxs-lookup"><span data-stu-id="6b48f-130">countImported</span></span>                |<span data-ttu-id="6b48f-131">Int64</span><span class="sxs-lookup"><span data-stu-id="6b48f-131">Int64</span></span>  |<span data-ttu-id="6b48f-132">导入的条目数。</span><span class="sxs-lookup"><span data-stu-id="6b48f-132">Count of imported entries.</span></span>|
|<span data-ttu-id="6b48f-133">countImportedDeltas</span><span class="sxs-lookup"><span data-stu-id="6b48f-133">countImportedDeltas</span></span>          |<span data-ttu-id="6b48f-134">Int64</span><span class="sxs-lookup"><span data-stu-id="6b48f-134">Int64</span></span>  |<span data-ttu-id="6b48f-135">导入的增量更改的计数。</span><span class="sxs-lookup"><span data-stu-id="6b48f-135">Count of imported delta-changes.</span></span>|
|<span data-ttu-id="6b48f-136">countImportedReferenceDeltas</span><span class="sxs-lookup"><span data-stu-id="6b48f-136">countImportedReferenceDeltas</span></span> |<span data-ttu-id="6b48f-137">Int64</span><span class="sxs-lookup"><span data-stu-id="6b48f-137">Int64</span></span>  |<span data-ttu-id="6b48f-138">与引用更改相关的导入的 delta 更改的计数。</span><span class="sxs-lookup"><span data-stu-id="6b48f-138">Count of imported delta-changes pertaining to reference changes.</span></span>|
|<span data-ttu-id="6b48f-139">error</span><span class="sxs-lookup"><span data-stu-id="6b48f-139">error</span></span>                        |[<span data-ttu-id="6b48f-140">synchronizationError</span><span class="sxs-lookup"><span data-stu-id="6b48f-140">synchronizationError</span></span>](synchronization-synchronizationerror.md)|<span data-ttu-id="6b48f-141">如果遇到错误, 则包含包含详细信息的**synchronizationError**对象。</span><span class="sxs-lookup"><span data-stu-id="6b48f-141">If an error was encountered, contains a **synchronizationError** object with details.</span></span>|
|<span data-ttu-id="6b48f-142">state</span><span class="sxs-lookup"><span data-stu-id="6b48f-142">state</span></span>                        |<span data-ttu-id="6b48f-143">String</span><span class="sxs-lookup"><span data-stu-id="6b48f-143">String</span></span> |<span data-ttu-id="6b48f-144">对此运行的结果进行汇总的代码。</span><span class="sxs-lookup"><span data-stu-id="6b48f-144">Code summarizing the result of this run.</span></span> <span data-ttu-id="6b48f-145">可取值为：`Succeeded`、`Failed`、`EntryLevelErrors`。</span><span class="sxs-lookup"><span data-stu-id="6b48f-145">Possible values are: `Succeeded`, `Failed`, `EntryLevelErrors`.</span></span>|
|<span data-ttu-id="6b48f-146">timeBegan</span><span class="sxs-lookup"><span data-stu-id="6b48f-146">timeBegan</span></span>                    |<span data-ttu-id="6b48f-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6b48f-147">DateTimeOffset</span></span>|<span data-ttu-id="6b48f-148">开始运行此作业的时间。</span><span class="sxs-lookup"><span data-stu-id="6b48f-148">Time when this job run began.</span></span> <span data-ttu-id="6b48f-149">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="6b48f-149">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="6b48f-150">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。</span><span class="sxs-lookup"><span data-stu-id="6b48f-150">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="6b48f-151">timeEnded</span><span class="sxs-lookup"><span data-stu-id="6b48f-151">timeEnded</span></span>                    |<span data-ttu-id="6b48f-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6b48f-152">DateTimeOffset</span></span>|<span data-ttu-id="6b48f-153">此作业运行结束的时间。</span><span class="sxs-lookup"><span data-stu-id="6b48f-153">Time when this job run ended.</span></span> <span data-ttu-id="6b48f-154">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="6b48f-154">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="6b48f-155">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。</span><span class="sxs-lookup"><span data-stu-id="6b48f-155">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="6b48f-156">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6b48f-156">JSON representation</span></span>

<span data-ttu-id="6b48f-157">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6b48f-157">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.synchronizationTaskExecution"
}-->

```json
{
  "activityIdentifier": "String",
  "countEntitled": 1024,
  "countEntitledForProvisioning": 1024,
  "countEscrowed": 1024,
  "countEscrowedRaw": 1024,
  "countExported": 1024,
  "countExports": 1024,
  "countImported": 1024,
  "countImportedDeltas": 1024,
  "countImportedReferenceDeltas": 1024,
  "error": {"@odata.type": "microsoft.graph.synchronizationError"},
  "state": "String",
  "timeBegan": "String (timestamp)",
  "timeEnded": "String (timestamp)"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "synchronizationTaskExecution resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
