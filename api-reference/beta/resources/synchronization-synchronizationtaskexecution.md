---
title: synchronizationTaskExecution 资源类型
description: 总结了运行同步作业的结果。
localization_priority: Normal
ms.openlocfilehash: 37a0fd57269cef6d3cb03c5cc5c38d3024fe198d
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29510552"
---
# <a name="synchronizationtaskexecution-resource-type"></a><span data-ttu-id="25663-103">synchronizationTaskExecution 资源类型</span><span class="sxs-lookup"><span data-stu-id="25663-103">synchronizationTaskExecution resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="25663-104">总结了运行同步作业的结果。</span><span class="sxs-lookup"><span data-stu-id="25663-104">Summarizes the results of the synchronization job run.</span></span>

## <a name="properties"></a><span data-ttu-id="25663-105">属性</span><span class="sxs-lookup"><span data-stu-id="25663-105">Properties</span></span>
| <span data-ttu-id="25663-106">属性</span><span class="sxs-lookup"><span data-stu-id="25663-106">Property</span></span>     | <span data-ttu-id="25663-107">类型</span><span class="sxs-lookup"><span data-stu-id="25663-107">Type</span></span>   |<span data-ttu-id="25663-108">说明</span><span class="sxs-lookup"><span data-stu-id="25663-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="25663-109">activityIdentifier</span><span class="sxs-lookup"><span data-stu-id="25663-109">activityIdentifier</span></span>           |<span data-ttu-id="25663-110">String</span><span class="sxs-lookup"><span data-stu-id="25663-110">String</span></span> |<span data-ttu-id="25663-111">运行作业的标识符。</span><span class="sxs-lookup"><span data-stu-id="25663-111">Identifier of the job run.</span></span>|
|<span data-ttu-id="25663-112">countEntitled</span><span class="sxs-lookup"><span data-stu-id="25663-112">countEntitled</span></span>                |<span data-ttu-id="25663-113">Int64</span><span class="sxs-lookup"><span data-stu-id="25663-113">Int64</span></span>  |<span data-ttu-id="25663-114">处理已分配为此应用程序的条目数。</span><span class="sxs-lookup"><span data-stu-id="25663-114">Count of processed entries that were assigned for this application.</span></span>|
|<span data-ttu-id="25663-115">countEntitledForProvisioning</span><span class="sxs-lookup"><span data-stu-id="25663-115">countEntitledForProvisioning</span></span> |<span data-ttu-id="25663-116">Int64</span><span class="sxs-lookup"><span data-stu-id="25663-116">Int64</span></span>  |<span data-ttu-id="25663-117">处理已分配的资源调配的条目数。</span><span class="sxs-lookup"><span data-stu-id="25663-117">Count of processed entries that were assigned for provisioning.</span></span>|
|<span data-ttu-id="25663-118">countEscrowed</span><span class="sxs-lookup"><span data-stu-id="25663-118">countEscrowed</span></span>                |<span data-ttu-id="25663-119">Int64</span><span class="sxs-lookup"><span data-stu-id="25663-119">Int64</span></span>  |<span data-ttu-id="25663-120">保管 （错误） 的条目数。</span><span class="sxs-lookup"><span data-stu-id="25663-120">Count of entries that were escrowed (errors).</span></span>|
|<span data-ttu-id="25663-121">countEscrowedRaw</span><span class="sxs-lookup"><span data-stu-id="25663-121">countEscrowedRaw</span></span>             |<span data-ttu-id="25663-122">Int64</span><span class="sxs-lookup"><span data-stu-id="25663-122">Int64</span></span>  |<span data-ttu-id="25663-123">已保管，包括 escrows 系统生成的条目数。</span><span class="sxs-lookup"><span data-stu-id="25663-123">Count of entries that were escrowed, including system-generated escrows.</span></span>|
|<span data-ttu-id="25663-124">countExported</span><span class="sxs-lookup"><span data-stu-id="25663-124">countExported</span></span>                |<span data-ttu-id="25663-125">Int64</span><span class="sxs-lookup"><span data-stu-id="25663-125">Int64</span></span>  |<span data-ttu-id="25663-126">导出的条目数。</span><span class="sxs-lookup"><span data-stu-id="25663-126">Count of exported entries.</span></span>|
|<span data-ttu-id="25663-127">countExports</span><span class="sxs-lookup"><span data-stu-id="25663-127">countExports</span></span>                 |<span data-ttu-id="25663-128">Int64</span><span class="sxs-lookup"><span data-stu-id="25663-128">Int64</span></span>  |<span data-ttu-id="25663-129">预计要导出的条目数。</span><span class="sxs-lookup"><span data-stu-id="25663-129">Count of entries that were expected to be exported.</span></span>|
|<span data-ttu-id="25663-130">countImported</span><span class="sxs-lookup"><span data-stu-id="25663-130">countImported</span></span>                |<span data-ttu-id="25663-131">Int64</span><span class="sxs-lookup"><span data-stu-id="25663-131">Int64</span></span>  |<span data-ttu-id="25663-132">导入的项目数。</span><span class="sxs-lookup"><span data-stu-id="25663-132">Count of imported entries.</span></span>|
|<span data-ttu-id="25663-133">countImportedDeltas</span><span class="sxs-lookup"><span data-stu-id="25663-133">countImportedDeltas</span></span>          |<span data-ttu-id="25663-134">Int64</span><span class="sxs-lookup"><span data-stu-id="25663-134">Int64</span></span>  |<span data-ttu-id="25663-135">导入的增量更改的计数。</span><span class="sxs-lookup"><span data-stu-id="25663-135">Count of imported delta-changes.</span></span>|
|<span data-ttu-id="25663-136">countImportedReferenceDeltas</span><span class="sxs-lookup"><span data-stu-id="25663-136">countImportedReferenceDeltas</span></span> |<span data-ttu-id="25663-137">Int64</span><span class="sxs-lookup"><span data-stu-id="25663-137">Int64</span></span>  |<span data-ttu-id="25663-138">导入增量-更改与引用更改的计数。</span><span class="sxs-lookup"><span data-stu-id="25663-138">Count of imported delta-changes pertaining to reference changes.</span></span>|
|<span data-ttu-id="25663-139">error</span><span class="sxs-lookup"><span data-stu-id="25663-139">error</span></span>                        |[<span data-ttu-id="25663-140">synchronizationError</span><span class="sxs-lookup"><span data-stu-id="25663-140">synchronizationError</span></span>](synchronization-synchronizationerror.md)|<span data-ttu-id="25663-141">如果遇到错误，将包含一个**synchronizationError**详细信息。</span><span class="sxs-lookup"><span data-stu-id="25663-141">If an error was encountered, contains a **synchronizationError** object with details.</span></span>|
|<span data-ttu-id="25663-142">state</span><span class="sxs-lookup"><span data-stu-id="25663-142">state</span></span>                        |<span data-ttu-id="25663-143">String</span><span class="sxs-lookup"><span data-stu-id="25663-143">String</span></span> |<span data-ttu-id="25663-144">汇总结果的此次运行的代码。</span><span class="sxs-lookup"><span data-stu-id="25663-144">Code summarizing the result of this run.</span></span> <span data-ttu-id="25663-145">可取值为：`Succeeded`、`Failed`、`EntryLevelErrors`。</span><span class="sxs-lookup"><span data-stu-id="25663-145">Possible values are: `Succeeded`, `Failed`, `EntryLevelErrors`.</span></span>|
|<span data-ttu-id="25663-146">timeBegan</span><span class="sxs-lookup"><span data-stu-id="25663-146">timeBegan</span></span>                    |<span data-ttu-id="25663-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="25663-147">DateTimeOffset</span></span>|<span data-ttu-id="25663-148">开始此作业的运行时的时间。</span><span class="sxs-lookup"><span data-stu-id="25663-148">Time when this job run began.</span></span> <span data-ttu-id="25663-149">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="25663-149">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="25663-150">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。</span><span class="sxs-lookup"><span data-stu-id="25663-150">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="25663-151">timeEnded</span><span class="sxs-lookup"><span data-stu-id="25663-151">timeEnded</span></span>                    |<span data-ttu-id="25663-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="25663-152">DateTimeOffset</span></span>|<span data-ttu-id="25663-153">结束此作业的运行时的时间。</span><span class="sxs-lookup"><span data-stu-id="25663-153">Time when this job run ended.</span></span> <span data-ttu-id="25663-154">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="25663-154">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="25663-155">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。</span><span class="sxs-lookup"><span data-stu-id="25663-155">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="25663-156">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="25663-156">JSON representation</span></span>

<span data-ttu-id="25663-157">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="25663-157">The following is a JSON representation of the resource.</span></span>

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
