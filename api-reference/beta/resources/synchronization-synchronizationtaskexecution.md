---
title: synchronizationTaskExecution 资源类型
description: 概述同步作业的运行结果。
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 5d777a575290699c2a936902614aa8ef0e8b042d
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48094909"
---
# <a name="synchronizationtaskexecution-resource-type"></a><span data-ttu-id="f0bd4-103">synchronizationTaskExecution 资源类型</span><span class="sxs-lookup"><span data-stu-id="f0bd4-103">synchronizationTaskExecution resource type</span></span>

<span data-ttu-id="f0bd4-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f0bd4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f0bd4-105">概述同步作业的运行结果。</span><span class="sxs-lookup"><span data-stu-id="f0bd4-105">Summarizes the results of the synchronization job run.</span></span>

## <a name="properties"></a><span data-ttu-id="f0bd4-106">属性</span><span class="sxs-lookup"><span data-stu-id="f0bd4-106">Properties</span></span>
| <span data-ttu-id="f0bd4-107">属性</span><span class="sxs-lookup"><span data-stu-id="f0bd4-107">Property</span></span>     | <span data-ttu-id="f0bd4-108">类型</span><span class="sxs-lookup"><span data-stu-id="f0bd4-108">Type</span></span>   |<span data-ttu-id="f0bd4-109">说明</span><span class="sxs-lookup"><span data-stu-id="f0bd4-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f0bd4-110">activityIdentifier</span><span class="sxs-lookup"><span data-stu-id="f0bd4-110">activityIdentifier</span></span>           |<span data-ttu-id="f0bd4-111">字符串</span><span class="sxs-lookup"><span data-stu-id="f0bd4-111">String</span></span> |<span data-ttu-id="f0bd4-112">作业运行的标识符。</span><span class="sxs-lookup"><span data-stu-id="f0bd4-112">Identifier of the job run.</span></span>|
|<span data-ttu-id="f0bd4-113">countEntitled</span><span class="sxs-lookup"><span data-stu-id="f0bd4-113">countEntitled</span></span>                |<span data-ttu-id="f0bd4-114">Int64</span><span class="sxs-lookup"><span data-stu-id="f0bd4-114">Int64</span></span>  |<span data-ttu-id="f0bd4-115">为此应用程序分配的已处理项的计数。</span><span class="sxs-lookup"><span data-stu-id="f0bd4-115">Count of processed entries that were assigned for this application.</span></span>|
|<span data-ttu-id="f0bd4-116">countEntitledForProvisioning</span><span class="sxs-lookup"><span data-stu-id="f0bd4-116">countEntitledForProvisioning</span></span> |<span data-ttu-id="f0bd4-117">Int64</span><span class="sxs-lookup"><span data-stu-id="f0bd4-117">Int64</span></span>  |<span data-ttu-id="f0bd4-118">为设置分配的已处理项的计数。</span><span class="sxs-lookup"><span data-stu-id="f0bd4-118">Count of processed entries that were assigned for provisioning.</span></span>|
|<span data-ttu-id="f0bd4-119">countEscrowed</span><span class="sxs-lookup"><span data-stu-id="f0bd4-119">countEscrowed</span></span>                |<span data-ttu-id="f0bd4-120">Int64</span><span class="sxs-lookup"><span data-stu-id="f0bd4-120">Int64</span></span>  |<span data-ttu-id="f0bd4-121">Escrowed (错误) 的条目数。</span><span class="sxs-lookup"><span data-stu-id="f0bd4-121">Count of entries that were escrowed (errors).</span></span>|
|<span data-ttu-id="f0bd4-122">countEscrowedRaw</span><span class="sxs-lookup"><span data-stu-id="f0bd4-122">countEscrowedRaw</span></span>             |<span data-ttu-id="f0bd4-123">Int64</span><span class="sxs-lookup"><span data-stu-id="f0bd4-123">Int64</span></span>  |<span data-ttu-id="f0bd4-124">Escrowed 的条目数，包括系统生成的 escrows。</span><span class="sxs-lookup"><span data-stu-id="f0bd4-124">Count of entries that were escrowed, including system-generated escrows.</span></span>|
|<span data-ttu-id="f0bd4-125">countExported</span><span class="sxs-lookup"><span data-stu-id="f0bd4-125">countExported</span></span>                |<span data-ttu-id="f0bd4-126">Int64</span><span class="sxs-lookup"><span data-stu-id="f0bd4-126">Int64</span></span>  |<span data-ttu-id="f0bd4-127">已导出条目的计数。</span><span class="sxs-lookup"><span data-stu-id="f0bd4-127">Count of exported entries.</span></span>|
|<span data-ttu-id="f0bd4-128">countExports</span><span class="sxs-lookup"><span data-stu-id="f0bd4-128">countExports</span></span>                 |<span data-ttu-id="f0bd4-129">Int64</span><span class="sxs-lookup"><span data-stu-id="f0bd4-129">Int64</span></span>  |<span data-ttu-id="f0bd4-130">预期要导出的条目数。</span><span class="sxs-lookup"><span data-stu-id="f0bd4-130">Count of entries that were expected to be exported.</span></span>|
|<span data-ttu-id="f0bd4-131">countImported</span><span class="sxs-lookup"><span data-stu-id="f0bd4-131">countImported</span></span>                |<span data-ttu-id="f0bd4-132">Int64</span><span class="sxs-lookup"><span data-stu-id="f0bd4-132">Int64</span></span>  |<span data-ttu-id="f0bd4-133">导入的条目数。</span><span class="sxs-lookup"><span data-stu-id="f0bd4-133">Count of imported entries.</span></span>|
|<span data-ttu-id="f0bd4-134">countImportedDeltas</span><span class="sxs-lookup"><span data-stu-id="f0bd4-134">countImportedDeltas</span></span>          |<span data-ttu-id="f0bd4-135">Int64</span><span class="sxs-lookup"><span data-stu-id="f0bd4-135">Int64</span></span>  |<span data-ttu-id="f0bd4-136">导入的增量更改的计数。</span><span class="sxs-lookup"><span data-stu-id="f0bd4-136">Count of imported delta-changes.</span></span>|
|<span data-ttu-id="f0bd4-137">countImportedReferenceDeltas</span><span class="sxs-lookup"><span data-stu-id="f0bd4-137">countImportedReferenceDeltas</span></span> |<span data-ttu-id="f0bd4-138">Int64</span><span class="sxs-lookup"><span data-stu-id="f0bd4-138">Int64</span></span>  |<span data-ttu-id="f0bd4-139">与引用更改相关的导入的 delta 更改的计数。</span><span class="sxs-lookup"><span data-stu-id="f0bd4-139">Count of imported delta-changes pertaining to reference changes.</span></span>|
|<span data-ttu-id="f0bd4-140">error</span><span class="sxs-lookup"><span data-stu-id="f0bd4-140">error</span></span>                        |[<span data-ttu-id="f0bd4-141">synchronizationError</span><span class="sxs-lookup"><span data-stu-id="f0bd4-141">synchronizationError</span></span>](synchronization-synchronizationerror.md)|<span data-ttu-id="f0bd4-142">如果遇到错误，则包含包含详细信息的 **synchronizationError** 对象。</span><span class="sxs-lookup"><span data-stu-id="f0bd4-142">If an error was encountered, contains a **synchronizationError** object with details.</span></span>|
|<span data-ttu-id="f0bd4-143">state</span><span class="sxs-lookup"><span data-stu-id="f0bd4-143">state</span></span>                        |<span data-ttu-id="f0bd4-144">String</span><span class="sxs-lookup"><span data-stu-id="f0bd4-144">String</span></span> |<span data-ttu-id="f0bd4-145">对此运行的结果进行汇总的代码。</span><span class="sxs-lookup"><span data-stu-id="f0bd4-145">Code summarizing the result of this run.</span></span> <span data-ttu-id="f0bd4-146">可取值为：`Succeeded`、`Failed`、`EntryLevelErrors`。</span><span class="sxs-lookup"><span data-stu-id="f0bd4-146">Possible values are: `Succeeded`, `Failed`, `EntryLevelErrors`.</span></span>|
|<span data-ttu-id="f0bd4-147">timeBegan</span><span class="sxs-lookup"><span data-stu-id="f0bd4-147">timeBegan</span></span>                    |<span data-ttu-id="f0bd4-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f0bd4-148">DateTimeOffset</span></span>|<span data-ttu-id="f0bd4-149">开始运行此作业的时间。</span><span class="sxs-lookup"><span data-stu-id="f0bd4-149">Time when this job run began.</span></span> <span data-ttu-id="f0bd4-150">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="f0bd4-150">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="f0bd4-151">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。</span><span class="sxs-lookup"><span data-stu-id="f0bd4-151">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="f0bd4-152">timeEnded</span><span class="sxs-lookup"><span data-stu-id="f0bd4-152">timeEnded</span></span>                    |<span data-ttu-id="f0bd4-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f0bd4-153">DateTimeOffset</span></span>|<span data-ttu-id="f0bd4-154">此作业运行结束的时间。</span><span class="sxs-lookup"><span data-stu-id="f0bd4-154">Time when this job run ended.</span></span> <span data-ttu-id="f0bd4-155">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="f0bd4-155">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="f0bd4-156">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。</span><span class="sxs-lookup"><span data-stu-id="f0bd4-156">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f0bd4-157">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f0bd4-157">JSON representation</span></span>

<span data-ttu-id="f0bd4-158">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f0bd4-158">The following is a JSON representation of the resource.</span></span>

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


