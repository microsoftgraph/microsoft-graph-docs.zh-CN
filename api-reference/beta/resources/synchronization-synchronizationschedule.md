---
title: synchronizationSchedule 资源类型
description: 定义用于运行 synchronizationJob 的计划。
localization_priority: Normal
doc_type: resourcePageType
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 5ffbc327d40edb071c70336032506b5f97c9e083
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35964625"
---
# <a name="synchronizationschedule-resource-type"></a><span data-ttu-id="84240-103">synchronizationSchedule 资源类型</span><span class="sxs-lookup"><span data-stu-id="84240-103">synchronizationSchedule resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="84240-104">定义用于运行[synchronizationJob](synchronization-synchronizationjob.md)的计划。</span><span class="sxs-lookup"><span data-stu-id="84240-104">Defines the schedule used to run a [synchronizationJob](synchronization-synchronizationjob.md).</span></span>

## <a name="properties"></a><span data-ttu-id="84240-105">属性</span><span class="sxs-lookup"><span data-stu-id="84240-105">Properties</span></span>
| <span data-ttu-id="84240-106">属性</span><span class="sxs-lookup"><span data-stu-id="84240-106">Property</span></span>     | <span data-ttu-id="84240-107">类型</span><span class="sxs-lookup"><span data-stu-id="84240-107">Type</span></span>   |<span data-ttu-id="84240-108">说明</span><span class="sxs-lookup"><span data-stu-id="84240-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="84240-109">时间</span><span class="sxs-lookup"><span data-stu-id="84240-109">expiration</span></span>|<span data-ttu-id="84240-110">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="84240-110">DateTimeOffset</span></span>|<span data-ttu-id="84240-111">此作业将到期的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="84240-111">Date and time when this job will expire.</span></span> <span data-ttu-id="84240-112">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="84240-112">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="84240-113">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。</span><span class="sxs-lookup"><span data-stu-id="84240-113">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="84240-114">interval</span><span class="sxs-lookup"><span data-stu-id="84240-114">interval</span></span>|<span data-ttu-id="84240-115">持续时间</span><span class="sxs-lookup"><span data-stu-id="84240-115">Duration</span></span>|<span data-ttu-id="84240-116">同步迭代之间的时间间隔。</span><span class="sxs-lookup"><span data-stu-id="84240-116">The interval between synchronization iterations.</span></span>|
|<span data-ttu-id="84240-117">state</span><span class="sxs-lookup"><span data-stu-id="84240-117">state</span></span>|<span data-ttu-id="84240-118">String</span><span class="sxs-lookup"><span data-stu-id="84240-118">String</span></span>| <span data-ttu-id="84240-119">可取值为：`Active`、`Disabled`。</span><span class="sxs-lookup"><span data-stu-id="84240-119">Possible values are: `Active`, `Disabled`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="84240-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="84240-120">JSON representation</span></span>

<span data-ttu-id="84240-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="84240-121">The following is a JSON representation of the resource.</span></span>

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
