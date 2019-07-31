---
title: synchronizationQuarantine 资源类型
description: 提供有关 synchronizationJob 的隔离状态的信息。
localization_priority: Normal
doc_type: resourcePageType
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: d63082dbe4e8e952d41032a74467cd4c301a857b
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35964699"
---
# <a name="synchronizationquarantine-resource-type"></a><span data-ttu-id="29b5b-103">synchronizationQuarantine 资源类型</span><span class="sxs-lookup"><span data-stu-id="29b5b-103">synchronizationQuarantine resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="29b5b-104">提供有关[synchronizationJob](synchronization-synchronizationjob.md)的隔离状态的信息。</span><span class="sxs-lookup"><span data-stu-id="29b5b-104">Provides information about the quarantine state of a [synchronizationJob](synchronization-synchronizationjob.md).</span></span>

## <a name="properties"></a><span data-ttu-id="29b5b-105">属性</span><span class="sxs-lookup"><span data-stu-id="29b5b-105">Properties</span></span>
| <span data-ttu-id="29b5b-106">属性</span><span class="sxs-lookup"><span data-stu-id="29b5b-106">Property</span></span>     | <span data-ttu-id="29b5b-107">类型</span><span class="sxs-lookup"><span data-stu-id="29b5b-107">Type</span></span>   |<span data-ttu-id="29b5b-108">说明</span><span class="sxs-lookup"><span data-stu-id="29b5b-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="29b5b-109">currentBegan</span><span class="sxs-lookup"><span data-stu-id="29b5b-109">currentBegan</span></span>|<span data-ttu-id="29b5b-110">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="29b5b-110">DateTimeOffset</span></span>|<span data-ttu-id="29b5b-111">上次评估和实施隔离的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="29b5b-111">Date and time when the quarantine was last evaluated and imposed.</span></span> <span data-ttu-id="29b5b-112">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="29b5b-112">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="29b5b-113">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。</span><span class="sxs-lookup"><span data-stu-id="29b5b-113">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="29b5b-114">nextAttempt</span><span class="sxs-lookup"><span data-stu-id="29b5b-114">nextAttempt</span></span>|<span data-ttu-id="29b5b-115">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="29b5b-115">DateTimeOffset</span></span>|<span data-ttu-id="29b5b-116">将进行下次尝试重新评估隔离的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="29b5b-116">Date and time when the next attempt to re-evaluate the quarantine will be made.</span></span> <span data-ttu-id="29b5b-117">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="29b5b-117">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="29b5b-118">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。</span><span class="sxs-lookup"><span data-stu-id="29b5b-118">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="29b5b-119">在于</span><span class="sxs-lookup"><span data-stu-id="29b5b-119">reason</span></span>|<span data-ttu-id="29b5b-120">String</span><span class="sxs-lookup"><span data-stu-id="29b5b-120">String</span></span>|<span data-ttu-id="29b5b-121">表示为什么强制实施隔离的代码。</span><span class="sxs-lookup"><span data-stu-id="29b5b-121">A code that signifies why the quarantine was imposed.</span></span> <span data-ttu-id="29b5b-122">可取值为：`EncounteredBaseEscrowThreshold`、`EncounteredTotalEscrowThreshold`、`EncounteredEscrowProportionThreshold`、`EncounteredQuarantineException`、`Unknown`。</span><span class="sxs-lookup"><span data-stu-id="29b5b-122">Possible values are: `EncounteredBaseEscrowThreshold`, `EncounteredTotalEscrowThreshold`, `EncounteredEscrowProportionThreshold`, `EncounteredQuarantineException`, `Unknown`.</span></span>|
|<span data-ttu-id="29b5b-123">seriesBegan</span><span class="sxs-lookup"><span data-stu-id="29b5b-123">seriesBegan</span></span>|<span data-ttu-id="29b5b-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="29b5b-124">DateTimeOffset</span></span>|<span data-ttu-id="29b5b-125">本系列首次实施隔离的日期和时间 (在首次实施隔离时, 系列会启动, 并且在提升隔离后立即重置)。</span><span class="sxs-lookup"><span data-stu-id="29b5b-125">Date and time when the quarantine was first imposed in this series (a series starts when a quarantine is first imposed, and is reset as soon as the quarantine is lifted).</span></span> <span data-ttu-id="29b5b-126">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="29b5b-126">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="29b5b-127">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。</span><span class="sxs-lookup"><span data-stu-id="29b5b-127">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="29b5b-128">seriesCount</span><span class="sxs-lookup"><span data-stu-id="29b5b-128">seriesCount</span></span>|<span data-ttu-id="29b5b-129">Int64</span><span class="sxs-lookup"><span data-stu-id="29b5b-129">Int64</span></span>|<span data-ttu-id="29b5b-130">本系列中的次数隔离已重新评估并生效 (当第一次实施隔离时, 系列会启动, 并在提升隔离后立即重置)。</span><span class="sxs-lookup"><span data-stu-id="29b5b-130">Number of times in this series the quarantine was re-evaluated and left in effect (a series starts when quarantine is first imposed, and is reset as soon as quarantine is lifted).</span></span>|

## <a name="json-representation"></a><span data-ttu-id="29b5b-131">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="29b5b-131">JSON representation</span></span>

<span data-ttu-id="29b5b-132">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="29b5b-132">The following is a JSON representation of the resource.</span></span>

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
  "suppressions": []
}
-->
