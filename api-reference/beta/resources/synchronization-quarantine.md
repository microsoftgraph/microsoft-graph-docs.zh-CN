---
title: synchronizationQuarantine 资源类型
description: 提供有关 synchronizationJob 的隔离状态信息。
ms.openlocfilehash: b29da9644968ffe17abb02010f8aa5c304ca7905
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27042272"
---
# <a name="synchronizationquarantine-resource-type"></a><span data-ttu-id="6d915-103">synchronizationQuarantine 资源类型</span><span class="sxs-lookup"><span data-stu-id="6d915-103">synchronizationQuarantine resource type</span></span>

> <span data-ttu-id="6d915-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="6d915-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6d915-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="6d915-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="6d915-106">提供有关[synchronizationJob](synchronization-synchronizationjob.md)的隔离状态信息。</span><span class="sxs-lookup"><span data-stu-id="6d915-106">Provides information about the quarantine state of a [synchronizationJob](synchronization-synchronizationjob.md).</span></span>

## <a name="properties"></a><span data-ttu-id="6d915-107">属性</span><span class="sxs-lookup"><span data-stu-id="6d915-107">Properties</span></span>
| <span data-ttu-id="6d915-108">属性</span><span class="sxs-lookup"><span data-stu-id="6d915-108">Property</span></span>     | <span data-ttu-id="6d915-109">类型</span><span class="sxs-lookup"><span data-stu-id="6d915-109">Type</span></span>   |<span data-ttu-id="6d915-110">说明</span><span class="sxs-lookup"><span data-stu-id="6d915-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6d915-111">currentBegan</span><span class="sxs-lookup"><span data-stu-id="6d915-111">currentBegan</span></span>|<span data-ttu-id="6d915-112">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6d915-112">DateTimeOffset</span></span>|<span data-ttu-id="6d915-113">日期和时间隔离上次计算施加。</span><span class="sxs-lookup"><span data-stu-id="6d915-113">Date and time when the quarantine was last evaluated and imposed.</span></span> <span data-ttu-id="6d915-114">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="6d915-114">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="6d915-115">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。</span><span class="sxs-lookup"><span data-stu-id="6d915-115">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="6d915-116">nextAttempt</span><span class="sxs-lookup"><span data-stu-id="6d915-116">nextAttempt</span></span>|<span data-ttu-id="6d915-117">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6d915-117">DateTimeOffset</span></span>|<span data-ttu-id="6d915-118">日期和时间时将进行下次尝试重新评估隔离邮箱。</span><span class="sxs-lookup"><span data-stu-id="6d915-118">Date and time when the next attempt to re-evaluate the quarantine will be made.</span></span> <span data-ttu-id="6d915-119">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="6d915-119">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="6d915-120">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。</span><span class="sxs-lookup"><span data-stu-id="6d915-120">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="6d915-121">原因</span><span class="sxs-lookup"><span data-stu-id="6d915-121">reason</span></span>|<span data-ttu-id="6d915-122">字符串</span><span class="sxs-lookup"><span data-stu-id="6d915-122">String</span></span>|<span data-ttu-id="6d915-123">表示隔离邮箱已施加为何代码。</span><span class="sxs-lookup"><span data-stu-id="6d915-123">A code that signifies why the quarantine was imposed.</span></span> <span data-ttu-id="6d915-124">可取值为：`EncounteredBaseEscrowThreshold`、`EncounteredTotalEscrowThreshold`、`EncounteredEscrowProportionThreshold`、`EncounteredQuarantineException`、`Unknown`。</span><span class="sxs-lookup"><span data-stu-id="6d915-124">Possible values are: `EncounteredBaseEscrowThreshold`, `EncounteredTotalEscrowThreshold`, `EncounteredEscrowProportionThreshold`, `EncounteredQuarantineException`, `Unknown`.</span></span>|
|<span data-ttu-id="6d915-125">seriesBegan</span><span class="sxs-lookup"><span data-stu-id="6d915-125">seriesBegan</span></span>|<span data-ttu-id="6d915-126">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6d915-126">DateTimeOffset</span></span>|<span data-ttu-id="6d915-127">日期和时间首先本系列 （series 启动时隔离首先施加，并将重置为提升隔离） 施加隔离邮箱。</span><span class="sxs-lookup"><span data-stu-id="6d915-127">Date and time when the quarantine was first imposed in this series (a series starts when a quarantine is first imposed, and is reset as soon as the quarantine is lifted).</span></span> <span data-ttu-id="6d915-128">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="6d915-128">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="6d915-129">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。</span><span class="sxs-lookup"><span data-stu-id="6d915-129">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="6d915-130">seriesCount</span><span class="sxs-lookup"><span data-stu-id="6d915-130">seriesCount</span></span>|<span data-ttu-id="6d915-131">Int64</span><span class="sxs-lookup"><span data-stu-id="6d915-131">Int64</span></span>|<span data-ttu-id="6d915-132">次数隔离此系列中的已被重新计算并左实际上 （系列启动时隔离首先施加，并将重置为提升隔离）。</span><span class="sxs-lookup"><span data-stu-id="6d915-132">Number of times in this series the quarantine was re-evaluated and left in effect (a series starts when quarantine is first imposed, and is reset as soon as quarantine is lifted).</span></span>|

## <a name="json-representation"></a><span data-ttu-id="6d915-133">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6d915-133">JSON representation</span></span>

<span data-ttu-id="6d915-134">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6d915-134">The following is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "synchronizationQuarantine resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->