---
title: synchronizationTaskExecution 资源类型
description: 概述同步作业的运行结果。
localization_priority: Normal
ms.openlocfilehash: 37a0fd57269cef6d3cb03c5cc5c38d3024fe198d
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32453861"
---
# <a name="synchronizationtaskexecution-resource-type"></a><span data-ttu-id="c4ff3-103">synchronizationTaskExecution 资源类型</span><span class="sxs-lookup"><span data-stu-id="c4ff3-103">synchronizationTaskExecution resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c4ff3-104">概述同步作业的运行结果。</span><span class="sxs-lookup"><span data-stu-id="c4ff3-104">Summarizes the results of the synchronization job run.</span></span>

## <a name="properties"></a><span data-ttu-id="c4ff3-105">属性</span><span class="sxs-lookup"><span data-stu-id="c4ff3-105">Properties</span></span>
| <span data-ttu-id="c4ff3-106">属性</span><span class="sxs-lookup"><span data-stu-id="c4ff3-106">Property</span></span>     | <span data-ttu-id="c4ff3-107">类型</span><span class="sxs-lookup"><span data-stu-id="c4ff3-107">Type</span></span>   |<span data-ttu-id="c4ff3-108">描述</span><span class="sxs-lookup"><span data-stu-id="c4ff3-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c4ff3-109">activityIdentifier</span><span class="sxs-lookup"><span data-stu-id="c4ff3-109">activityIdentifier</span></span>           |<span data-ttu-id="c4ff3-110">字符串</span><span class="sxs-lookup"><span data-stu-id="c4ff3-110">String</span></span> |<span data-ttu-id="c4ff3-111">作业运行的标识符。</span><span class="sxs-lookup"><span data-stu-id="c4ff3-111">Identifier of the job run.</span></span>|
|<span data-ttu-id="c4ff3-112">countEntitled</span><span class="sxs-lookup"><span data-stu-id="c4ff3-112">countEntitled</span></span>                |<span data-ttu-id="c4ff3-113">Int64</span><span class="sxs-lookup"><span data-stu-id="c4ff3-113">Int64</span></span>  |<span data-ttu-id="c4ff3-114">为此应用程序分配的已处理项的计数。</span><span class="sxs-lookup"><span data-stu-id="c4ff3-114">Count of processed entries that were assigned for this application.</span></span>|
|<span data-ttu-id="c4ff3-115">countEntitledForProvisioning</span><span class="sxs-lookup"><span data-stu-id="c4ff3-115">countEntitledForProvisioning</span></span> |<span data-ttu-id="c4ff3-116">Int64</span><span class="sxs-lookup"><span data-stu-id="c4ff3-116">Int64</span></span>  |<span data-ttu-id="c4ff3-117">为设置分配的已处理项的计数。</span><span class="sxs-lookup"><span data-stu-id="c4ff3-117">Count of processed entries that were assigned for provisioning.</span></span>|
|<span data-ttu-id="c4ff3-118">countEscrowed</span><span class="sxs-lookup"><span data-stu-id="c4ff3-118">countEscrowed</span></span>                |<span data-ttu-id="c4ff3-119">Int64</span><span class="sxs-lookup"><span data-stu-id="c4ff3-119">Int64</span></span>  |<span data-ttu-id="c4ff3-120">escrowed (错误) 的项的计数。</span><span class="sxs-lookup"><span data-stu-id="c4ff3-120">Count of entries that were escrowed (errors).</span></span>|
|<span data-ttu-id="c4ff3-121">countEscrowedRaw</span><span class="sxs-lookup"><span data-stu-id="c4ff3-121">countEscrowedRaw</span></span>             |<span data-ttu-id="c4ff3-122">Int64</span><span class="sxs-lookup"><span data-stu-id="c4ff3-122">Int64</span></span>  |<span data-ttu-id="c4ff3-123">escrowed 的条目数, 包括系统生成的 escrows。</span><span class="sxs-lookup"><span data-stu-id="c4ff3-123">Count of entries that were escrowed, including system-generated escrows.</span></span>|
|<span data-ttu-id="c4ff3-124">countExported</span><span class="sxs-lookup"><span data-stu-id="c4ff3-124">countExported</span></span>                |<span data-ttu-id="c4ff3-125">Int64</span><span class="sxs-lookup"><span data-stu-id="c4ff3-125">Int64</span></span>  |<span data-ttu-id="c4ff3-126">已导出条目的计数。</span><span class="sxs-lookup"><span data-stu-id="c4ff3-126">Count of exported entries.</span></span>|
|<span data-ttu-id="c4ff3-127">countExports</span><span class="sxs-lookup"><span data-stu-id="c4ff3-127">countExports</span></span>                 |<span data-ttu-id="c4ff3-128">Int64</span><span class="sxs-lookup"><span data-stu-id="c4ff3-128">Int64</span></span>  |<span data-ttu-id="c4ff3-129">预期要导出的条目数。</span><span class="sxs-lookup"><span data-stu-id="c4ff3-129">Count of entries that were expected to be exported.</span></span>|
|<span data-ttu-id="c4ff3-130">countImported</span><span class="sxs-lookup"><span data-stu-id="c4ff3-130">countImported</span></span>                |<span data-ttu-id="c4ff3-131">Int64</span><span class="sxs-lookup"><span data-stu-id="c4ff3-131">Int64</span></span>  |<span data-ttu-id="c4ff3-132">导入的条目数。</span><span class="sxs-lookup"><span data-stu-id="c4ff3-132">Count of imported entries.</span></span>|
|<span data-ttu-id="c4ff3-133">countImportedDeltas</span><span class="sxs-lookup"><span data-stu-id="c4ff3-133">countImportedDeltas</span></span>          |<span data-ttu-id="c4ff3-134">Int64</span><span class="sxs-lookup"><span data-stu-id="c4ff3-134">Int64</span></span>  |<span data-ttu-id="c4ff3-135">导入的增量更改的计数。</span><span class="sxs-lookup"><span data-stu-id="c4ff3-135">Count of imported delta-changes.</span></span>|
|<span data-ttu-id="c4ff3-136">countImportedReferenceDeltas</span><span class="sxs-lookup"><span data-stu-id="c4ff3-136">countImportedReferenceDeltas</span></span> |<span data-ttu-id="c4ff3-137">Int64</span><span class="sxs-lookup"><span data-stu-id="c4ff3-137">Int64</span></span>  |<span data-ttu-id="c4ff3-138">与引用更改相关的导入的 delta 更改的计数。</span><span class="sxs-lookup"><span data-stu-id="c4ff3-138">Count of imported delta-changes pertaining to reference changes.</span></span>|
|<span data-ttu-id="c4ff3-139">error</span><span class="sxs-lookup"><span data-stu-id="c4ff3-139">error</span></span>                        |[<span data-ttu-id="c4ff3-140">synchronizationError</span><span class="sxs-lookup"><span data-stu-id="c4ff3-140">synchronizationError</span></span>](synchronization-synchronizationerror.md)|<span data-ttu-id="c4ff3-141">如果遇到错误, 则包含包含详细信息的**synchronizationError**对象。</span><span class="sxs-lookup"><span data-stu-id="c4ff3-141">If an error was encountered, contains a **synchronizationError** object with details.</span></span>|
|<span data-ttu-id="c4ff3-142">state</span><span class="sxs-lookup"><span data-stu-id="c4ff3-142">state</span></span>                        |<span data-ttu-id="c4ff3-143">String</span><span class="sxs-lookup"><span data-stu-id="c4ff3-143">String</span></span> |<span data-ttu-id="c4ff3-144">对此运行的结果进行汇总的代码。</span><span class="sxs-lookup"><span data-stu-id="c4ff3-144">Code summarizing the result of this run.</span></span> <span data-ttu-id="c4ff3-145">可取值为：`Succeeded`、`Failed`、`EntryLevelErrors`。</span><span class="sxs-lookup"><span data-stu-id="c4ff3-145">Possible values are: `Succeeded`, `Failed`, `EntryLevelErrors`.</span></span>|
|<span data-ttu-id="c4ff3-146">timeBegan</span><span class="sxs-lookup"><span data-stu-id="c4ff3-146">timeBegan</span></span>                    |<span data-ttu-id="c4ff3-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c4ff3-147">DateTimeOffset</span></span>|<span data-ttu-id="c4ff3-148">开始运行此作业的时间。</span><span class="sxs-lookup"><span data-stu-id="c4ff3-148">Time when this job run began.</span></span> <span data-ttu-id="c4ff3-149">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="c4ff3-149">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="c4ff3-150">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。</span><span class="sxs-lookup"><span data-stu-id="c4ff3-150">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="c4ff3-151">timeEnded</span><span class="sxs-lookup"><span data-stu-id="c4ff3-151">timeEnded</span></span>                    |<span data-ttu-id="c4ff3-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c4ff3-152">DateTimeOffset</span></span>|<span data-ttu-id="c4ff3-153">此作业运行结束的时间。</span><span class="sxs-lookup"><span data-stu-id="c4ff3-153">Time when this job run ended.</span></span> <span data-ttu-id="c4ff3-154">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="c4ff3-154">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="c4ff3-155">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。</span><span class="sxs-lookup"><span data-stu-id="c4ff3-155">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c4ff3-156">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c4ff3-156">JSON representation</span></span>

<span data-ttu-id="c4ff3-157">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c4ff3-157">The following is a JSON representation of the resource.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/synchronization-synchronizationtaskexecution.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
