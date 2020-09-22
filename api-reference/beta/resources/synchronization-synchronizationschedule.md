---
title: synchronizationSchedule 资源类型
description: 定义用于运行 synchronizationJob 的计划。
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 70b44acb7f00e55bf4082ac064950e819cb33f2f
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48046736"
---
# <a name="synchronizationschedule-resource-type"></a><span data-ttu-id="3eddf-103">synchronizationSchedule 资源类型</span><span class="sxs-lookup"><span data-stu-id="3eddf-103">synchronizationSchedule resource type</span></span>

<span data-ttu-id="3eddf-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3eddf-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3eddf-105">定义用于运行 [synchronizationJob](synchronization-synchronizationjob.md)的计划。</span><span class="sxs-lookup"><span data-stu-id="3eddf-105">Defines the schedule used to run a [synchronizationJob](synchronization-synchronizationjob.md).</span></span>

## <a name="properties"></a><span data-ttu-id="3eddf-106">属性</span><span class="sxs-lookup"><span data-stu-id="3eddf-106">Properties</span></span>
| <span data-ttu-id="3eddf-107">属性</span><span class="sxs-lookup"><span data-stu-id="3eddf-107">Property</span></span>     | <span data-ttu-id="3eddf-108">类型</span><span class="sxs-lookup"><span data-stu-id="3eddf-108">Type</span></span>   |<span data-ttu-id="3eddf-109">说明</span><span class="sxs-lookup"><span data-stu-id="3eddf-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3eddf-110">时间</span><span class="sxs-lookup"><span data-stu-id="3eddf-110">expiration</span></span>|<span data-ttu-id="3eddf-111">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3eddf-111">DateTimeOffset</span></span>|<span data-ttu-id="3eddf-112">此作业将到期的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="3eddf-112">Date and time when this job will expire.</span></span> <span data-ttu-id="3eddf-113">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="3eddf-113">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="3eddf-114">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。</span><span class="sxs-lookup"><span data-stu-id="3eddf-114">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="3eddf-115">interval</span><span class="sxs-lookup"><span data-stu-id="3eddf-115">interval</span></span>|<span data-ttu-id="3eddf-116">持续时间</span><span class="sxs-lookup"><span data-stu-id="3eddf-116">Duration</span></span>|<span data-ttu-id="3eddf-117">同步迭代之间的时间间隔。</span><span class="sxs-lookup"><span data-stu-id="3eddf-117">The interval between synchronization iterations.</span></span>|
|<span data-ttu-id="3eddf-118">state</span><span class="sxs-lookup"><span data-stu-id="3eddf-118">state</span></span>|<span data-ttu-id="3eddf-119">String</span><span class="sxs-lookup"><span data-stu-id="3eddf-119">String</span></span>| <span data-ttu-id="3eddf-120">可取值为：`Active`、`Disabled`。</span><span class="sxs-lookup"><span data-stu-id="3eddf-120">Possible values are: `Active`, `Disabled`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="3eddf-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="3eddf-121">JSON representation</span></span>

<span data-ttu-id="3eddf-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3eddf-122">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.synchronizationSchedule"
}-->

```json
{
  "expiration": "String (timestamp)",
  "interval": "String (duration)",
  "state": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "synchronizationSchedule resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


