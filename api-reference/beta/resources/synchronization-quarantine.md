---
title: synchronizationQuarantine 资源类型
description: 提供有关 synchronizationJob 的隔离状态的信息。
localization_priority: Normal
ms.openlocfilehash: 6d5d5c3cbe96eda6b39833287e8efb6e0771b19a
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32523213"
---
# <a name="synchronizationquarantine-resource-type"></a><span data-ttu-id="5b02b-103">synchronizationQuarantine 资源类型</span><span class="sxs-lookup"><span data-stu-id="5b02b-103">synchronizationQuarantine resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5b02b-104">提供有关[synchronizationJob](synchronization-synchronizationjob.md)的隔离状态的信息。</span><span class="sxs-lookup"><span data-stu-id="5b02b-104">Provides information about the quarantine state of a [synchronizationJob](synchronization-synchronizationjob.md).</span></span>

## <a name="properties"></a><span data-ttu-id="5b02b-105">属性</span><span class="sxs-lookup"><span data-stu-id="5b02b-105">Properties</span></span>
| <span data-ttu-id="5b02b-106">属性</span><span class="sxs-lookup"><span data-stu-id="5b02b-106">Property</span></span>     | <span data-ttu-id="5b02b-107">类型</span><span class="sxs-lookup"><span data-stu-id="5b02b-107">Type</span></span>   |<span data-ttu-id="5b02b-108">说明</span><span class="sxs-lookup"><span data-stu-id="5b02b-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5b02b-109">currentBegan</span><span class="sxs-lookup"><span data-stu-id="5b02b-109">currentBegan</span></span>|<span data-ttu-id="5b02b-110">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5b02b-110">DateTimeOffset</span></span>|<span data-ttu-id="5b02b-111">上次评估和实施隔离的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="5b02b-111">Date and time when the quarantine was last evaluated and imposed.</span></span> <span data-ttu-id="5b02b-112">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="5b02b-112">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="5b02b-113">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。</span><span class="sxs-lookup"><span data-stu-id="5b02b-113">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="5b02b-114">nextAttempt</span><span class="sxs-lookup"><span data-stu-id="5b02b-114">nextAttempt</span></span>|<span data-ttu-id="5b02b-115">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5b02b-115">DateTimeOffset</span></span>|<span data-ttu-id="5b02b-116">将进行下次尝试重新评估隔离的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="5b02b-116">Date and time when the next attempt to re-evaluate the quarantine will be made.</span></span> <span data-ttu-id="5b02b-117">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="5b02b-117">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="5b02b-118">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。</span><span class="sxs-lookup"><span data-stu-id="5b02b-118">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="5b02b-119">在于</span><span class="sxs-lookup"><span data-stu-id="5b02b-119">reason</span></span>|<span data-ttu-id="5b02b-120">String</span><span class="sxs-lookup"><span data-stu-id="5b02b-120">String</span></span>|<span data-ttu-id="5b02b-121">表示为什么强制实施隔离的代码。</span><span class="sxs-lookup"><span data-stu-id="5b02b-121">A code that signifies why the quarantine was imposed.</span></span> <span data-ttu-id="5b02b-122">可取值为：`EncounteredBaseEscrowThreshold`、`EncounteredTotalEscrowThreshold`、`EncounteredEscrowProportionThreshold`、`EncounteredQuarantineException` 或 `Unknown`。</span><span class="sxs-lookup"><span data-stu-id="5b02b-122">Possible values are: `EncounteredBaseEscrowThreshold`, `EncounteredTotalEscrowThreshold`, `EncounteredEscrowProportionThreshold`, `EncounteredQuarantineException`, `Unknown`.</span></span>|
|<span data-ttu-id="5b02b-123">seriesBegan</span><span class="sxs-lookup"><span data-stu-id="5b02b-123">seriesBegan</span></span>|<span data-ttu-id="5b02b-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5b02b-124">DateTimeOffset</span></span>|<span data-ttu-id="5b02b-125">本系列首次实施隔离的日期和时间 (在首次实施隔离时, 系列会启动, 并且在提升隔离后立即重置)。</span><span class="sxs-lookup"><span data-stu-id="5b02b-125">Date and time when the quarantine was first imposed in this series (a series starts when a quarantine is first imposed, and is reset as soon as the quarantine is lifted).</span></span> <span data-ttu-id="5b02b-126">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="5b02b-126">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="5b02b-127">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。</span><span class="sxs-lookup"><span data-stu-id="5b02b-127">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="5b02b-128">seriesCount</span><span class="sxs-lookup"><span data-stu-id="5b02b-128">seriesCount</span></span>|<span data-ttu-id="5b02b-129">Int64</span><span class="sxs-lookup"><span data-stu-id="5b02b-129">Int64</span></span>|<span data-ttu-id="5b02b-130">本系列中的次数隔离已重新评估并生效 (当第一次实施隔离时, 系列会启动, 并在提升隔离后立即重置)。</span><span class="sxs-lookup"><span data-stu-id="5b02b-130">Number of times in this series the quarantine was re-evaluated and left in effect (a series starts when quarantine is first imposed, and is reset as soon as quarantine is lifted).</span></span>|

## <a name="json-representation"></a><span data-ttu-id="5b02b-131">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5b02b-131">JSON representation</span></span>

<span data-ttu-id="5b02b-132">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5b02b-132">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.synchronizationQuarantine"
}-->

```json
{
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
  "suppressions": [
    "Error: /api-reference/beta/resources/synchronization-quarantine.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
