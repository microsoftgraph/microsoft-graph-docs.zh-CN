---
title: synchronizationTaskExecution 资源类型
description: 总结了运行同步作业的结果。
ms.openlocfilehash: 4aefba4bdf9ab850892344e6e34683e81d1a1afa
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27045243"
---
# <a name="synchronizationtaskexecution-resource-type"></a><span data-ttu-id="a043a-103">synchronizationTaskExecution 资源类型</span><span class="sxs-lookup"><span data-stu-id="a043a-103">synchronizationTaskExecution resource type</span></span>

> <span data-ttu-id="a043a-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="a043a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a043a-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="a043a-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a043a-106">总结了运行同步作业的结果。</span><span class="sxs-lookup"><span data-stu-id="a043a-106">Summarizes the results of the synchronization job run.</span></span>

## <a name="properties"></a><span data-ttu-id="a043a-107">属性</span><span class="sxs-lookup"><span data-stu-id="a043a-107">Properties</span></span>
| <span data-ttu-id="a043a-108">属性</span><span class="sxs-lookup"><span data-stu-id="a043a-108">Property</span></span>     | <span data-ttu-id="a043a-109">类型</span><span class="sxs-lookup"><span data-stu-id="a043a-109">Type</span></span>   |<span data-ttu-id="a043a-110">说明</span><span class="sxs-lookup"><span data-stu-id="a043a-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a043a-111">activityIdentifier</span><span class="sxs-lookup"><span data-stu-id="a043a-111">activityIdentifier</span></span>           |<span data-ttu-id="a043a-112">字符串</span><span class="sxs-lookup"><span data-stu-id="a043a-112">String</span></span> |<span data-ttu-id="a043a-113">运行作业的标识符。</span><span class="sxs-lookup"><span data-stu-id="a043a-113">Identifier of the job run.</span></span>|
|<span data-ttu-id="a043a-114">countEntitled</span><span class="sxs-lookup"><span data-stu-id="a043a-114">countEntitled</span></span>                |<span data-ttu-id="a043a-115">Int64</span><span class="sxs-lookup"><span data-stu-id="a043a-115">Int64</span></span>  |<span data-ttu-id="a043a-116">处理已分配为此应用程序的条目数。</span><span class="sxs-lookup"><span data-stu-id="a043a-116">Count of processed entries that were assigned for this application.</span></span>|
|<span data-ttu-id="a043a-117">countEntitledForProvisioning</span><span class="sxs-lookup"><span data-stu-id="a043a-117">countEntitledForProvisioning</span></span> |<span data-ttu-id="a043a-118">Int64</span><span class="sxs-lookup"><span data-stu-id="a043a-118">Int64</span></span>  |<span data-ttu-id="a043a-119">处理已分配的资源调配的条目数。</span><span class="sxs-lookup"><span data-stu-id="a043a-119">Count of processed entries that were assigned for provisioning.</span></span>|
|<span data-ttu-id="a043a-120">countEscrowed</span><span class="sxs-lookup"><span data-stu-id="a043a-120">countEscrowed</span></span>                |<span data-ttu-id="a043a-121">Int64</span><span class="sxs-lookup"><span data-stu-id="a043a-121">Int64</span></span>  |<span data-ttu-id="a043a-122">保管 （错误） 的条目数。</span><span class="sxs-lookup"><span data-stu-id="a043a-122">Count of entries that were escrowed (errors).</span></span>|
|<span data-ttu-id="a043a-123">countEscrowedRaw</span><span class="sxs-lookup"><span data-stu-id="a043a-123">countEscrowedRaw</span></span>             |<span data-ttu-id="a043a-124">Int64</span><span class="sxs-lookup"><span data-stu-id="a043a-124">Int64</span></span>  |<span data-ttu-id="a043a-125">已保管，包括 escrows 系统生成的条目数。</span><span class="sxs-lookup"><span data-stu-id="a043a-125">Count of entries that were escrowed, including system-generated escrows.</span></span>|
|<span data-ttu-id="a043a-126">countExported</span><span class="sxs-lookup"><span data-stu-id="a043a-126">countExported</span></span>                |<span data-ttu-id="a043a-127">Int64</span><span class="sxs-lookup"><span data-stu-id="a043a-127">Int64</span></span>  |<span data-ttu-id="a043a-128">导出的条目数。</span><span class="sxs-lookup"><span data-stu-id="a043a-128">Count of exported entries.</span></span>|
|<span data-ttu-id="a043a-129">countExports</span><span class="sxs-lookup"><span data-stu-id="a043a-129">countExports</span></span>                 |<span data-ttu-id="a043a-130">Int64</span><span class="sxs-lookup"><span data-stu-id="a043a-130">Int64</span></span>  |<span data-ttu-id="a043a-131">预计要导出的条目数。</span><span class="sxs-lookup"><span data-stu-id="a043a-131">Count of entries that were expected to be exported.</span></span>|
|<span data-ttu-id="a043a-132">countImported</span><span class="sxs-lookup"><span data-stu-id="a043a-132">countImported</span></span>                |<span data-ttu-id="a043a-133">Int64</span><span class="sxs-lookup"><span data-stu-id="a043a-133">Int64</span></span>  |<span data-ttu-id="a043a-134">导入的项目数。</span><span class="sxs-lookup"><span data-stu-id="a043a-134">Count of imported entries.</span></span>|
|<span data-ttu-id="a043a-135">countImportedDeltas</span><span class="sxs-lookup"><span data-stu-id="a043a-135">countImportedDeltas</span></span>          |<span data-ttu-id="a043a-136">Int64</span><span class="sxs-lookup"><span data-stu-id="a043a-136">Int64</span></span>  |<span data-ttu-id="a043a-137">导入的增量更改的计数。</span><span class="sxs-lookup"><span data-stu-id="a043a-137">Count of imported delta-changes.</span></span>|
|<span data-ttu-id="a043a-138">countImportedReferenceDeltas</span><span class="sxs-lookup"><span data-stu-id="a043a-138">countImportedReferenceDeltas</span></span> |<span data-ttu-id="a043a-139">Int64</span><span class="sxs-lookup"><span data-stu-id="a043a-139">Int64</span></span>  |<span data-ttu-id="a043a-140">导入增量-更改与引用更改的计数。</span><span class="sxs-lookup"><span data-stu-id="a043a-140">Count of imported delta-changes pertaining to reference changes.</span></span>|
|<span data-ttu-id="a043a-141">error</span><span class="sxs-lookup"><span data-stu-id="a043a-141">error</span></span>                        |[<span data-ttu-id="a043a-142">synchronizationError</span><span class="sxs-lookup"><span data-stu-id="a043a-142">synchronizationError</span></span>](synchronization-synchronizationerror.md)|<span data-ttu-id="a043a-143">如果遇到错误，将包含一个**synchronizationError**详细信息。</span><span class="sxs-lookup"><span data-stu-id="a043a-143">If an error was encountered, contains a **synchronizationError** object with details.</span></span>|
|<span data-ttu-id="a043a-144">状态</span><span class="sxs-lookup"><span data-stu-id="a043a-144">state</span></span>                        |<span data-ttu-id="a043a-145">字符串</span><span class="sxs-lookup"><span data-stu-id="a043a-145">String</span></span> |<span data-ttu-id="a043a-146">汇总结果的此次运行的代码。</span><span class="sxs-lookup"><span data-stu-id="a043a-146">Code summarizing the result of this run.</span></span> <span data-ttu-id="a043a-147">可取值为：`Succeeded`、`Failed`、`EntryLevelErrors`。</span><span class="sxs-lookup"><span data-stu-id="a043a-147">Possible values are: `Succeeded`, `Failed`, `EntryLevelErrors`.</span></span>|
|<span data-ttu-id="a043a-148">timeBegan</span><span class="sxs-lookup"><span data-stu-id="a043a-148">timeBegan</span></span>                    |<span data-ttu-id="a043a-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a043a-149">DateTimeOffset</span></span>|<span data-ttu-id="a043a-150">开始此作业的运行时的时间。</span><span class="sxs-lookup"><span data-stu-id="a043a-150">Time when this job run began.</span></span> <span data-ttu-id="a043a-151">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="a043a-151">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="a043a-152">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。</span><span class="sxs-lookup"><span data-stu-id="a043a-152">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="a043a-153">timeEnded</span><span class="sxs-lookup"><span data-stu-id="a043a-153">timeEnded</span></span>                    |<span data-ttu-id="a043a-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a043a-154">DateTimeOffset</span></span>|<span data-ttu-id="a043a-155">结束此作业的运行时的时间。</span><span class="sxs-lookup"><span data-stu-id="a043a-155">Time when this job run ended.</span></span> <span data-ttu-id="a043a-156">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="a043a-156">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="a043a-157">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。</span><span class="sxs-lookup"><span data-stu-id="a043a-157">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a043a-158">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a043a-158">JSON representation</span></span>

<span data-ttu-id="a043a-159">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a043a-159">The following is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "synchronizationTaskExecution resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->