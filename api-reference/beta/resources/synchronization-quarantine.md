---
title: synchronizationQuarantine 资源类型
description: 提供有关 synchronizationJob 的隔离状态的信息。
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: dd2641c7327ce0670d3b13ab05701c7da5eb0de6
ms.sourcegitcommit: bdef75943ade3f1080120f555b67d5ebb3245699
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/10/2020
ms.locfileid: "43217596"
---
# <a name="synchronizationquarantine-resource-type"></a><span data-ttu-id="1dca1-103">synchronizationQuarantine 资源类型</span><span class="sxs-lookup"><span data-stu-id="1dca1-103">synchronizationQuarantine resource type</span></span>

<span data-ttu-id="1dca1-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1dca1-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1dca1-105">提供有关[synchronizationJob](synchronization-synchronizationjob.md)的隔离状态的信息。</span><span class="sxs-lookup"><span data-stu-id="1dca1-105">Provides information about the quarantine state of a [synchronizationJob](synchronization-synchronizationjob.md).</span></span>

## <a name="properties"></a><span data-ttu-id="1dca1-106">属性</span><span class="sxs-lookup"><span data-stu-id="1dca1-106">Properties</span></span>
| <span data-ttu-id="1dca1-107">属性</span><span class="sxs-lookup"><span data-stu-id="1dca1-107">Property</span></span>     | <span data-ttu-id="1dca1-108">类型</span><span class="sxs-lookup"><span data-stu-id="1dca1-108">Type</span></span>   |<span data-ttu-id="1dca1-109">说明</span><span class="sxs-lookup"><span data-stu-id="1dca1-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1dca1-110">currentBegan</span><span class="sxs-lookup"><span data-stu-id="1dca1-110">currentBegan</span></span>|<span data-ttu-id="1dca1-111">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1dca1-111">DateTimeOffset</span></span>|<span data-ttu-id="1dca1-112">上次评估和实施隔离的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="1dca1-112">Date and time when the quarantine was last evaluated and imposed.</span></span> <span data-ttu-id="1dca1-113">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="1dca1-113">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="1dca1-114">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。</span><span class="sxs-lookup"><span data-stu-id="1dca1-114">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="1dca1-115">nextAttempt</span><span class="sxs-lookup"><span data-stu-id="1dca1-115">nextAttempt</span></span>|<span data-ttu-id="1dca1-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1dca1-116">DateTimeOffset</span></span>|<span data-ttu-id="1dca1-117">将进行下次尝试重新评估隔离的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="1dca1-117">Date and time when the next attempt to re-evaluate the quarantine will be made.</span></span> <span data-ttu-id="1dca1-118">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="1dca1-118">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="1dca1-119">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。</span><span class="sxs-lookup"><span data-stu-id="1dca1-119">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="1dca1-120">reason</span><span class="sxs-lookup"><span data-stu-id="1dca1-120">reason</span></span>|<span data-ttu-id="1dca1-121">字符串</span><span class="sxs-lookup"><span data-stu-id="1dca1-121">String</span></span>|<span data-ttu-id="1dca1-122">表示为什么强制实施隔离的代码。</span><span class="sxs-lookup"><span data-stu-id="1dca1-122">A code that signifies why the quarantine was imposed.</span></span> <span data-ttu-id="1dca1-123">可取值为：`EncounteredBaseEscrowThreshold`、`EncounteredTotalEscrowThreshold`、`EncounteredEscrowProportionThreshold`、`EncounteredQuarantineException`、`QuarantinedOnDemand`、`TooManyDeletes` 或 `Unknown`。</span><span class="sxs-lookup"><span data-stu-id="1dca1-123">Possible values are: `EncounteredBaseEscrowThreshold`, `EncounteredTotalEscrowThreshold`, `EncounteredEscrowProportionThreshold`, `EncounteredQuarantineException`, `QuarantinedOnDemand`, `TooManyDeletes`, `Unknown`.</span></span>|
|<span data-ttu-id="1dca1-124">seriesBegan</span><span class="sxs-lookup"><span data-stu-id="1dca1-124">seriesBegan</span></span>|<span data-ttu-id="1dca1-125">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1dca1-125">DateTimeOffset</span></span>|<span data-ttu-id="1dca1-126">本系列首次实施隔离的日期和时间（在首次实施隔离时，系列会启动，并且在提升隔离后立即重置）。</span><span class="sxs-lookup"><span data-stu-id="1dca1-126">Date and time when the quarantine was first imposed in this series (a series starts when a quarantine is first imposed, and is reset as soon as the quarantine is lifted).</span></span> <span data-ttu-id="1dca1-127">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="1dca1-127">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="1dca1-128">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。</span><span class="sxs-lookup"><span data-stu-id="1dca1-128">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="1dca1-129">seriesCount</span><span class="sxs-lookup"><span data-stu-id="1dca1-129">seriesCount</span></span>|<span data-ttu-id="1dca1-130">Int64</span><span class="sxs-lookup"><span data-stu-id="1dca1-130">Int64</span></span>|<span data-ttu-id="1dca1-131">本系列中的次数隔离已重新评估并生效（当第一次实施隔离时，系列会启动，并在提升隔离后立即重置）。</span><span class="sxs-lookup"><span data-stu-id="1dca1-131">Number of times in this series the quarantine was re-evaluated and left in effect (a series starts when quarantine is first imposed, and is reset as soon as quarantine is lifted).</span></span>|
|<span data-ttu-id="1dca1-132">error</span><span class="sxs-lookup"><span data-stu-id="1dca1-132">error</span></span>|[<span data-ttu-id="1dca1-133">synchronizationError</span><span class="sxs-lookup"><span data-stu-id="1dca1-133">synchronizationError</span></span>](synchronization-synchronizationerror.md)|<span data-ttu-id="1dca1-134">描述将同步作业放入隔离时出现的错误。</span><span class="sxs-lookup"><span data-stu-id="1dca1-134">Describes the error(s) that occurred when putting the synchronization job into quarantine.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="1dca1-135">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1dca1-135">JSON representation</span></span>

<span data-ttu-id="1dca1-136">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1dca1-136">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.synchronizationQuarantine"
}-->

```json
{
  "error": {"@odata.type": "microsoft.graph.synchronizationError"},
  "currentBegan": "String (timestamp)",
  "nextAttempt": "String (timestamp)",
  "reason": "String",
  "seriesBegan": "String (timestamp)",
  "seriesCount": 1024
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "synchronizationQuarantine resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
