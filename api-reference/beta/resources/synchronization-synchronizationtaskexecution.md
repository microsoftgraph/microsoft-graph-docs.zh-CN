---
title: synchronizationTaskExecution 资源类型
description: 概述同步作业的运行结果。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 2aeb64d0ef08d25a8be9b2ed711d6deabfe522a1
ms.sourcegitcommit: 121c0fad692fb3c5c01dc051481b5249e4491b48
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/11/2019
ms.locfileid: "35620659"
---
# <a name="synchronizationtaskexecution-resource-type"></a><span data-ttu-id="831e4-103">synchronizationTaskExecution 资源类型</span><span class="sxs-lookup"><span data-stu-id="831e4-103">synchronizationTaskExecution resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="831e4-104">概述同步作业的运行结果。</span><span class="sxs-lookup"><span data-stu-id="831e4-104">Summarizes the results of the synchronization job run.</span></span>

## <a name="properties"></a><span data-ttu-id="831e4-105">属性</span><span class="sxs-lookup"><span data-stu-id="831e4-105">Properties</span></span>
| <span data-ttu-id="831e4-106">属性</span><span class="sxs-lookup"><span data-stu-id="831e4-106">Property</span></span>     | <span data-ttu-id="831e4-107">类型</span><span class="sxs-lookup"><span data-stu-id="831e4-107">Type</span></span>   |<span data-ttu-id="831e4-108">说明</span><span class="sxs-lookup"><span data-stu-id="831e4-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="831e4-109">activityIdentifier</span><span class="sxs-lookup"><span data-stu-id="831e4-109">activityIdentifier</span></span>           |<span data-ttu-id="831e4-110">String</span><span class="sxs-lookup"><span data-stu-id="831e4-110">String</span></span> |<span data-ttu-id="831e4-111">作业运行的标识符。</span><span class="sxs-lookup"><span data-stu-id="831e4-111">Identifier of the job run.</span></span>|
|<span data-ttu-id="831e4-112">countEntitled</span><span class="sxs-lookup"><span data-stu-id="831e4-112">countEntitled</span></span>                |<span data-ttu-id="831e4-113">Int64</span><span class="sxs-lookup"><span data-stu-id="831e4-113">Int64</span></span>  |<span data-ttu-id="831e4-114">为此应用程序分配的已处理项的计数。</span><span class="sxs-lookup"><span data-stu-id="831e4-114">Count of processed entries that were assigned for this application.</span></span>|
|<span data-ttu-id="831e4-115">countEntitledForProvisioning</span><span class="sxs-lookup"><span data-stu-id="831e4-115">countEntitledForProvisioning</span></span> |<span data-ttu-id="831e4-116">Int64</span><span class="sxs-lookup"><span data-stu-id="831e4-116">Int64</span></span>  |<span data-ttu-id="831e4-117">为设置分配的已处理项的计数。</span><span class="sxs-lookup"><span data-stu-id="831e4-117">Count of processed entries that were assigned for provisioning.</span></span>|
|<span data-ttu-id="831e4-118">countEscrowed</span><span class="sxs-lookup"><span data-stu-id="831e4-118">countEscrowed</span></span>                |<span data-ttu-id="831e4-119">Int64</span><span class="sxs-lookup"><span data-stu-id="831e4-119">Int64</span></span>  |<span data-ttu-id="831e4-120">Escrowed (错误) 的项的计数。</span><span class="sxs-lookup"><span data-stu-id="831e4-120">Count of entries that were escrowed (errors).</span></span>|
|<span data-ttu-id="831e4-121">countEscrowedRaw</span><span class="sxs-lookup"><span data-stu-id="831e4-121">countEscrowedRaw</span></span>             |<span data-ttu-id="831e4-122">Int64</span><span class="sxs-lookup"><span data-stu-id="831e4-122">Int64</span></span>  |<span data-ttu-id="831e4-123">Escrowed 的条目数, 包括系统生成的 escrows。</span><span class="sxs-lookup"><span data-stu-id="831e4-123">Count of entries that were escrowed, including system-generated escrows.</span></span>|
|<span data-ttu-id="831e4-124">countExported</span><span class="sxs-lookup"><span data-stu-id="831e4-124">countExported</span></span>                |<span data-ttu-id="831e4-125">Int64</span><span class="sxs-lookup"><span data-stu-id="831e4-125">Int64</span></span>  |<span data-ttu-id="831e4-126">已导出条目的计数。</span><span class="sxs-lookup"><span data-stu-id="831e4-126">Count of exported entries.</span></span>|
|<span data-ttu-id="831e4-127">countExports</span><span class="sxs-lookup"><span data-stu-id="831e4-127">countExports</span></span>                 |<span data-ttu-id="831e4-128">Int64</span><span class="sxs-lookup"><span data-stu-id="831e4-128">Int64</span></span>  |<span data-ttu-id="831e4-129">预期要导出的条目数。</span><span class="sxs-lookup"><span data-stu-id="831e4-129">Count of entries that were expected to be exported.</span></span>|
|<span data-ttu-id="831e4-130">countImported</span><span class="sxs-lookup"><span data-stu-id="831e4-130">countImported</span></span>                |<span data-ttu-id="831e4-131">Int64</span><span class="sxs-lookup"><span data-stu-id="831e4-131">Int64</span></span>  |<span data-ttu-id="831e4-132">导入的条目数。</span><span class="sxs-lookup"><span data-stu-id="831e4-132">Count of imported entries.</span></span>|
|<span data-ttu-id="831e4-133">countImportedDeltas</span><span class="sxs-lookup"><span data-stu-id="831e4-133">countImportedDeltas</span></span>          |<span data-ttu-id="831e4-134">Int64</span><span class="sxs-lookup"><span data-stu-id="831e4-134">Int64</span></span>  |<span data-ttu-id="831e4-135">导入的增量更改的计数。</span><span class="sxs-lookup"><span data-stu-id="831e4-135">Count of imported delta-changes.</span></span>|
|<span data-ttu-id="831e4-136">countImportedReferenceDeltas</span><span class="sxs-lookup"><span data-stu-id="831e4-136">countImportedReferenceDeltas</span></span> |<span data-ttu-id="831e4-137">Int64</span><span class="sxs-lookup"><span data-stu-id="831e4-137">Int64</span></span>  |<span data-ttu-id="831e4-138">与引用更改相关的导入的 delta 更改的计数。</span><span class="sxs-lookup"><span data-stu-id="831e4-138">Count of imported delta-changes pertaining to reference changes.</span></span>|
|<span data-ttu-id="831e4-139">error</span><span class="sxs-lookup"><span data-stu-id="831e4-139">error</span></span>                        |[<span data-ttu-id="831e4-140">synchronizationError</span><span class="sxs-lookup"><span data-stu-id="831e4-140">synchronizationError</span></span>](synchronization-synchronizationerror.md)|<span data-ttu-id="831e4-141">如果遇到错误, 则包含包含详细信息的**synchronizationError**对象。</span><span class="sxs-lookup"><span data-stu-id="831e4-141">If an error was encountered, contains a **synchronizationError** object with details.</span></span>|
|<span data-ttu-id="831e4-142">state</span><span class="sxs-lookup"><span data-stu-id="831e4-142">state</span></span>                        |<span data-ttu-id="831e4-143">String</span><span class="sxs-lookup"><span data-stu-id="831e4-143">String</span></span> |<span data-ttu-id="831e4-144">对此运行的结果进行汇总的代码。</span><span class="sxs-lookup"><span data-stu-id="831e4-144">Code summarizing the result of this run.</span></span> <span data-ttu-id="831e4-145">可取值为：`Succeeded`、`Failed`、`EntryLevelErrors`。</span><span class="sxs-lookup"><span data-stu-id="831e4-145">Possible values are: `Succeeded`, `Failed`, `EntryLevelErrors`.</span></span>|
|<span data-ttu-id="831e4-146">timeBegan</span><span class="sxs-lookup"><span data-stu-id="831e4-146">timeBegan</span></span>                    |<span data-ttu-id="831e4-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="831e4-147">DateTimeOffset</span></span>|<span data-ttu-id="831e4-148">开始运行此作业的时间。</span><span class="sxs-lookup"><span data-stu-id="831e4-148">Time when this job run began.</span></span> <span data-ttu-id="831e4-149">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="831e4-149">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="831e4-150">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。</span><span class="sxs-lookup"><span data-stu-id="831e4-150">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="831e4-151">timeEnded</span><span class="sxs-lookup"><span data-stu-id="831e4-151">timeEnded</span></span>                    |<span data-ttu-id="831e4-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="831e4-152">DateTimeOffset</span></span>|<span data-ttu-id="831e4-153">此作业运行结束的时间。</span><span class="sxs-lookup"><span data-stu-id="831e4-153">Time when this job run ended.</span></span> <span data-ttu-id="831e4-154">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="831e4-154">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="831e4-155">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。</span><span class="sxs-lookup"><span data-stu-id="831e4-155">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="831e4-156">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="831e4-156">JSON representation</span></span>

<span data-ttu-id="831e4-157">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="831e4-157">The following is a JSON representation of the resource.</span></span>

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
