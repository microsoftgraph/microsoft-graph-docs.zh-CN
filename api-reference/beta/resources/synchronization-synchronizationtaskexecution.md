---
title: synchronizationTaskExecution 资源类型
description: 汇总同步作业运行的结果。
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: applications
ms.openlocfilehash: ac42a91ec35c1d81d81efa52f4306bbd1cfb2f55
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50135035"
---
# <a name="synchronizationtaskexecution-resource-type"></a><span data-ttu-id="0be67-103">synchronizationTaskExecution 资源类型</span><span class="sxs-lookup"><span data-stu-id="0be67-103">synchronizationTaskExecution resource type</span></span>

<span data-ttu-id="0be67-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0be67-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0be67-105">汇总同步作业运行的结果。</span><span class="sxs-lookup"><span data-stu-id="0be67-105">Summarizes the results of the synchronization job run.</span></span>

## <a name="properties"></a><span data-ttu-id="0be67-106">属性</span><span class="sxs-lookup"><span data-stu-id="0be67-106">Properties</span></span>
| <span data-ttu-id="0be67-107">属性</span><span class="sxs-lookup"><span data-stu-id="0be67-107">Property</span></span>     | <span data-ttu-id="0be67-108">类型</span><span class="sxs-lookup"><span data-stu-id="0be67-108">Type</span></span>   |<span data-ttu-id="0be67-109">说明</span><span class="sxs-lookup"><span data-stu-id="0be67-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0be67-110">activityIdentifier</span><span class="sxs-lookup"><span data-stu-id="0be67-110">activityIdentifier</span></span>           |<span data-ttu-id="0be67-111">字符串</span><span class="sxs-lookup"><span data-stu-id="0be67-111">String</span></span> |<span data-ttu-id="0be67-112">作业运行的标识符。</span><span class="sxs-lookup"><span data-stu-id="0be67-112">Identifier of the job run.</span></span>|
|<span data-ttu-id="0be67-113">countEntitled</span><span class="sxs-lookup"><span data-stu-id="0be67-113">countEntitled</span></span>                |<span data-ttu-id="0be67-114">Int64</span><span class="sxs-lookup"><span data-stu-id="0be67-114">Int64</span></span>  |<span data-ttu-id="0be67-115">为此应用程序分配的已处理条目计数。</span><span class="sxs-lookup"><span data-stu-id="0be67-115">Count of processed entries that were assigned for this application.</span></span>|
|<span data-ttu-id="0be67-116">countEntitledForProvisioning</span><span class="sxs-lookup"><span data-stu-id="0be67-116">countEntitledForProvisioning</span></span> |<span data-ttu-id="0be67-117">Int64</span><span class="sxs-lookup"><span data-stu-id="0be67-117">Int64</span></span>  |<span data-ttu-id="0be67-118">已分配用于预配的已处理条目计数。</span><span class="sxs-lookup"><span data-stu-id="0be67-118">Count of processed entries that were assigned for provisioning.</span></span>|
|<span data-ttu-id="0be67-119">countEscrowed</span><span class="sxs-lookup"><span data-stu-id="0be67-119">countEscrowed</span></span>                |<span data-ttu-id="0be67-120">Int64</span><span class="sxs-lookup"><span data-stu-id="0be67-120">Int64</span></span>  |<span data-ttu-id="0be67-121">托管的条目数 (错误) 。</span><span class="sxs-lookup"><span data-stu-id="0be67-121">Count of entries that were escrowed (errors).</span></span>|
|<span data-ttu-id="0be67-122">countEscrowedRaw</span><span class="sxs-lookup"><span data-stu-id="0be67-122">countEscrowedRaw</span></span>             |<span data-ttu-id="0be67-123">Int64</span><span class="sxs-lookup"><span data-stu-id="0be67-123">Int64</span></span>  |<span data-ttu-id="0be67-124">托管的条目计数，包括系统生成的托管。</span><span class="sxs-lookup"><span data-stu-id="0be67-124">Count of entries that were escrowed, including system-generated escrows.</span></span>|
|<span data-ttu-id="0be67-125">countExported</span><span class="sxs-lookup"><span data-stu-id="0be67-125">countExported</span></span>                |<span data-ttu-id="0be67-126">Int64</span><span class="sxs-lookup"><span data-stu-id="0be67-126">Int64</span></span>  |<span data-ttu-id="0be67-127">已导出条目的计数。</span><span class="sxs-lookup"><span data-stu-id="0be67-127">Count of exported entries.</span></span>|
|<span data-ttu-id="0be67-128">countExports</span><span class="sxs-lookup"><span data-stu-id="0be67-128">countExports</span></span>                 |<span data-ttu-id="0be67-129">Int64</span><span class="sxs-lookup"><span data-stu-id="0be67-129">Int64</span></span>  |<span data-ttu-id="0be67-130">预期要导出的条目计数。</span><span class="sxs-lookup"><span data-stu-id="0be67-130">Count of entries that were expected to be exported.</span></span>|
|<span data-ttu-id="0be67-131">countImported</span><span class="sxs-lookup"><span data-stu-id="0be67-131">countImported</span></span>                |<span data-ttu-id="0be67-132">Int64</span><span class="sxs-lookup"><span data-stu-id="0be67-132">Int64</span></span>  |<span data-ttu-id="0be67-133">导入的条目计数。</span><span class="sxs-lookup"><span data-stu-id="0be67-133">Count of imported entries.</span></span>|
|<span data-ttu-id="0be67-134">countImportedDeltas</span><span class="sxs-lookup"><span data-stu-id="0be67-134">countImportedDeltas</span></span>          |<span data-ttu-id="0be67-135">Int64</span><span class="sxs-lookup"><span data-stu-id="0be67-135">Int64</span></span>  |<span data-ttu-id="0be67-136">导入的增量更改计数。</span><span class="sxs-lookup"><span data-stu-id="0be67-136">Count of imported delta-changes.</span></span>|
|<span data-ttu-id="0be67-137">countImportedReferenceDeltas</span><span class="sxs-lookup"><span data-stu-id="0be67-137">countImportedReferenceDeltas</span></span> |<span data-ttu-id="0be67-138">Int64</span><span class="sxs-lookup"><span data-stu-id="0be67-138">Int64</span></span>  |<span data-ttu-id="0be67-139">与引用更改相关的导入增量更改计数。</span><span class="sxs-lookup"><span data-stu-id="0be67-139">Count of imported delta-changes pertaining to reference changes.</span></span>|
|<span data-ttu-id="0be67-140">error</span><span class="sxs-lookup"><span data-stu-id="0be67-140">error</span></span>                        |[<span data-ttu-id="0be67-141">synchronizationError</span><span class="sxs-lookup"><span data-stu-id="0be67-141">synchronizationError</span></span>](synchronization-synchronizationerror.md)|<span data-ttu-id="0be67-142">如果遇到错误，则包含包含详细信息的 **synchronizationError** 对象。</span><span class="sxs-lookup"><span data-stu-id="0be67-142">If an error was encountered, contains a **synchronizationError** object with details.</span></span>|
|<span data-ttu-id="0be67-143">state</span><span class="sxs-lookup"><span data-stu-id="0be67-143">state</span></span>                        |<span data-ttu-id="0be67-144">String</span><span class="sxs-lookup"><span data-stu-id="0be67-144">String</span></span> |<span data-ttu-id="0be67-145">汇总此运行结果的代码。</span><span class="sxs-lookup"><span data-stu-id="0be67-145">Code summarizing the result of this run.</span></span> <span data-ttu-id="0be67-146">可取值为：`Succeeded`、`Failed`、`EntryLevelErrors`。</span><span class="sxs-lookup"><span data-stu-id="0be67-146">Possible values are: `Succeeded`, `Failed`, `EntryLevelErrors`.</span></span>|
|<span data-ttu-id="0be67-147">timeBegan</span><span class="sxs-lookup"><span data-stu-id="0be67-147">timeBegan</span></span>                    |<span data-ttu-id="0be67-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0be67-148">DateTimeOffset</span></span>|<span data-ttu-id="0be67-149">此作业运行开始的时间。</span><span class="sxs-lookup"><span data-stu-id="0be67-149">Time when this job run began.</span></span> <span data-ttu-id="0be67-150">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="0be67-150">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="0be67-151">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。</span><span class="sxs-lookup"><span data-stu-id="0be67-151">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="0be67-152">timeEnded</span><span class="sxs-lookup"><span data-stu-id="0be67-152">timeEnded</span></span>                    |<span data-ttu-id="0be67-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0be67-153">DateTimeOffset</span></span>|<span data-ttu-id="0be67-154">此作业运行结束的时间。</span><span class="sxs-lookup"><span data-stu-id="0be67-154">Time when this job run ended.</span></span> <span data-ttu-id="0be67-155">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="0be67-155">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="0be67-156">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。</span><span class="sxs-lookup"><span data-stu-id="0be67-156">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0be67-157">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0be67-157">JSON representation</span></span>

<span data-ttu-id="0be67-158">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0be67-158">The following is a JSON representation of the resource.</span></span>

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


