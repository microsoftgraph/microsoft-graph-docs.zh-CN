---
title: synchronizationSchedule 资源类型
description: 定义用于运行 synchronizationJob 的计划。
localization_priority: Normal
ms.openlocfilehash: b59c36a36d837c21c147033dff8de66b85c863a1
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27877866"
---
# <a name="synchronizationschedule-resource-type"></a><span data-ttu-id="5e693-103">synchronizationSchedule 资源类型</span><span class="sxs-lookup"><span data-stu-id="5e693-103">synchronizationSchedule resource type</span></span>

> <span data-ttu-id="5e693-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="5e693-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5e693-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="5e693-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="5e693-106">定义用于运行[synchronizationJob](synchronization-synchronizationjob.md)的计划。</span><span class="sxs-lookup"><span data-stu-id="5e693-106">Defines the schedule used to run a [synchronizationJob](synchronization-synchronizationjob.md).</span></span>

## <a name="properties"></a><span data-ttu-id="5e693-107">属性</span><span class="sxs-lookup"><span data-stu-id="5e693-107">Properties</span></span>
| <span data-ttu-id="5e693-108">属性</span><span class="sxs-lookup"><span data-stu-id="5e693-108">Property</span></span>     | <span data-ttu-id="5e693-109">类型</span><span class="sxs-lookup"><span data-stu-id="5e693-109">Type</span></span>   |<span data-ttu-id="5e693-110">Description</span><span class="sxs-lookup"><span data-stu-id="5e693-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5e693-111">过期</span><span class="sxs-lookup"><span data-stu-id="5e693-111">expiration</span></span>|<span data-ttu-id="5e693-112">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5e693-112">DateTimeOffset</span></span>|<span data-ttu-id="5e693-113">日期和时间时，此作业将过期。</span><span class="sxs-lookup"><span data-stu-id="5e693-113">Date and time when this job will expire.</span></span> <span data-ttu-id="5e693-114">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="5e693-114">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="5e693-115">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。</span><span class="sxs-lookup"><span data-stu-id="5e693-115">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="5e693-116">interval</span><span class="sxs-lookup"><span data-stu-id="5e693-116">interval</span></span>|<span data-ttu-id="5e693-117">Duration</span><span class="sxs-lookup"><span data-stu-id="5e693-117">Duration</span></span>|<span data-ttu-id="5e693-118">同步迭代之间的间隔。</span><span class="sxs-lookup"><span data-stu-id="5e693-118">The interval between synchronization iterations.</span></span>|
|<span data-ttu-id="5e693-119">state</span><span class="sxs-lookup"><span data-stu-id="5e693-119">state</span></span>|<span data-ttu-id="5e693-120">String</span><span class="sxs-lookup"><span data-stu-id="5e693-120">String</span></span>| <span data-ttu-id="5e693-121">可取值为：`Active`、`Disabled`。</span><span class="sxs-lookup"><span data-stu-id="5e693-121">Possible values are: `Active`, `Disabled`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="5e693-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5e693-122">JSON representation</span></span>

<span data-ttu-id="5e693-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5e693-123">The following is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "synchronizationSchedule resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
