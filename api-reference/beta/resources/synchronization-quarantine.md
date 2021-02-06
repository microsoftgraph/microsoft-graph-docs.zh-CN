---
title: synchronizationQuarantine 资源类型
description: 提供有关 synchronizationJob 的隔离状态的信息。
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: applications
ms.openlocfilehash: 1673da71c0fbeaa952bccb89e6edd2c029fad4a6
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50133131"
---
# <a name="synchronizationquarantine-resource-type"></a><span data-ttu-id="853dc-103">synchronizationQuarantine 资源类型</span><span class="sxs-lookup"><span data-stu-id="853dc-103">synchronizationQuarantine resource type</span></span>

<span data-ttu-id="853dc-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="853dc-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="853dc-105">提供有关 [synchronizationJob](synchronization-synchronizationjob.md)的隔离状态的信息。</span><span class="sxs-lookup"><span data-stu-id="853dc-105">Provides information about the quarantine state of a [synchronizationJob](synchronization-synchronizationjob.md).</span></span>

## <a name="properties"></a><span data-ttu-id="853dc-106">属性</span><span class="sxs-lookup"><span data-stu-id="853dc-106">Properties</span></span>
| <span data-ttu-id="853dc-107">属性</span><span class="sxs-lookup"><span data-stu-id="853dc-107">Property</span></span>     | <span data-ttu-id="853dc-108">类型</span><span class="sxs-lookup"><span data-stu-id="853dc-108">Type</span></span>   |<span data-ttu-id="853dc-109">说明</span><span class="sxs-lookup"><span data-stu-id="853dc-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="853dc-110">currentBegan</span><span class="sxs-lookup"><span data-stu-id="853dc-110">currentBegan</span></span>|<span data-ttu-id="853dc-111">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="853dc-111">DateTimeOffset</span></span>|<span data-ttu-id="853dc-112">上次评估并强制隔离的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="853dc-112">Date and time when the quarantine was last evaluated and imposed.</span></span> <span data-ttu-id="853dc-113">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="853dc-113">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="853dc-114">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。</span><span class="sxs-lookup"><span data-stu-id="853dc-114">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="853dc-115">nextAttempt</span><span class="sxs-lookup"><span data-stu-id="853dc-115">nextAttempt</span></span>|<span data-ttu-id="853dc-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="853dc-116">DateTimeOffset</span></span>|<span data-ttu-id="853dc-117">下一次尝试重新评估隔离的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="853dc-117">Date and time when the next attempt to re-evaluate the quarantine will be made.</span></span> <span data-ttu-id="853dc-118">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="853dc-118">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="853dc-119">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。</span><span class="sxs-lookup"><span data-stu-id="853dc-119">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="853dc-120">reason</span><span class="sxs-lookup"><span data-stu-id="853dc-120">reason</span></span>|<span data-ttu-id="853dc-121">字符串</span><span class="sxs-lookup"><span data-stu-id="853dc-121">String</span></span>|<span data-ttu-id="853dc-122">一个代码，它表示为何实施隔离。</span><span class="sxs-lookup"><span data-stu-id="853dc-122">A code that signifies why the quarantine was imposed.</span></span> <span data-ttu-id="853dc-123">可取值为：`EncounteredBaseEscrowThreshold`、`EncounteredTotalEscrowThreshold`、`EncounteredEscrowProportionThreshold`、`EncounteredQuarantineException`、`QuarantinedOnDemand`、`TooManyDeletes` 或 `Unknown`。</span><span class="sxs-lookup"><span data-stu-id="853dc-123">Possible values are: `EncounteredBaseEscrowThreshold`, `EncounteredTotalEscrowThreshold`, `EncounteredEscrowProportionThreshold`, `EncounteredQuarantineException`, `QuarantinedOnDemand`, `TooManyDeletes`, `Unknown`.</span></span>|
|<span data-ttu-id="853dc-124">seriesBegan</span><span class="sxs-lookup"><span data-stu-id="853dc-124">seriesBegan</span></span>|<span data-ttu-id="853dc-125">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="853dc-125">DateTimeOffset</span></span>|<span data-ttu-id="853dc-126">在本系列中首次隔离的日期和时间 (一系列从首次隔离时开始，一旦解除隔离，就会) 。</span><span class="sxs-lookup"><span data-stu-id="853dc-126">Date and time when the quarantine was first imposed in this series (a series starts when a quarantine is first imposed, and is reset as soon as the quarantine is lifted).</span></span> <span data-ttu-id="853dc-127">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="853dc-127">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="853dc-128">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。</span><span class="sxs-lookup"><span data-stu-id="853dc-128">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="853dc-129">seriesCount</span><span class="sxs-lookup"><span data-stu-id="853dc-129">seriesCount</span></span>|<span data-ttu-id="853dc-130">Int64</span><span class="sxs-lookup"><span data-stu-id="853dc-130">Int64</span></span>|<span data-ttu-id="853dc-131">此系列中对隔离进行重新评估并留有效 (一系列在首次实施隔离时开始，一旦解除隔离，就会重置) 。</span><span class="sxs-lookup"><span data-stu-id="853dc-131">Number of times in this series the quarantine was re-evaluated and left in effect (a series starts when quarantine is first imposed, and is reset as soon as quarantine is lifted).</span></span>|
|<span data-ttu-id="853dc-132">error</span><span class="sxs-lookup"><span data-stu-id="853dc-132">error</span></span>|[<span data-ttu-id="853dc-133">synchronizationError</span><span class="sxs-lookup"><span data-stu-id="853dc-133">synchronizationError</span></span>](synchronization-synchronizationerror.md)|<span data-ttu-id="853dc-134">描述将 (隔离) 时发生的错误。</span><span class="sxs-lookup"><span data-stu-id="853dc-134">Describes the error(s) that occurred when putting the synchronization job into quarantine.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="853dc-135">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="853dc-135">JSON representation</span></span>

<span data-ttu-id="853dc-136">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="853dc-136">The following is a JSON representation of the resource.</span></span>

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


