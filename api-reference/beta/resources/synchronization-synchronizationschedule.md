---
title: synchronizationSchedule 资源类型
description: 定义用于运行 synchronizationJob 的计划。
ms.openlocfilehash: c0435b3957f138751f34a1e0e522683b352294da
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27045232"
---
# <a name="synchronizationschedule-resource-type"></a><span data-ttu-id="aeece-103">synchronizationSchedule 资源类型</span><span class="sxs-lookup"><span data-stu-id="aeece-103">synchronizationSchedule resource type</span></span>

> <span data-ttu-id="aeece-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="aeece-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="aeece-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="aeece-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="aeece-106">定义用于运行[synchronizationJob](synchronization-synchronizationjob.md)的计划。</span><span class="sxs-lookup"><span data-stu-id="aeece-106">Defines the schedule used to run a [synchronizationJob](synchronization-synchronizationjob.md).</span></span>

## <a name="properties"></a><span data-ttu-id="aeece-107">属性</span><span class="sxs-lookup"><span data-stu-id="aeece-107">Properties</span></span>
| <span data-ttu-id="aeece-108">属性</span><span class="sxs-lookup"><span data-stu-id="aeece-108">Property</span></span>     | <span data-ttu-id="aeece-109">类型</span><span class="sxs-lookup"><span data-stu-id="aeece-109">Type</span></span>   |<span data-ttu-id="aeece-110">说明</span><span class="sxs-lookup"><span data-stu-id="aeece-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="aeece-111">过期</span><span class="sxs-lookup"><span data-stu-id="aeece-111">expiration</span></span>|<span data-ttu-id="aeece-112">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="aeece-112">DateTimeOffset</span></span>|<span data-ttu-id="aeece-113">日期和时间时，此作业将过期。</span><span class="sxs-lookup"><span data-stu-id="aeece-113">Date and time when this job will expire.</span></span> <span data-ttu-id="aeece-114">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="aeece-114">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="aeece-115">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。</span><span class="sxs-lookup"><span data-stu-id="aeece-115">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="aeece-116">interval</span><span class="sxs-lookup"><span data-stu-id="aeece-116">interval</span></span>|<span data-ttu-id="aeece-117">Duration</span><span class="sxs-lookup"><span data-stu-id="aeece-117">Duration</span></span>|<span data-ttu-id="aeece-118">同步迭代之间的间隔。</span><span class="sxs-lookup"><span data-stu-id="aeece-118">The interval between synchronization iterations.</span></span>|
|<span data-ttu-id="aeece-119">状态</span><span class="sxs-lookup"><span data-stu-id="aeece-119">state</span></span>|<span data-ttu-id="aeece-120">String</span><span class="sxs-lookup"><span data-stu-id="aeece-120">String</span></span>| <span data-ttu-id="aeece-121">可取值为：`Active`、`Disabled`。</span><span class="sxs-lookup"><span data-stu-id="aeece-121">Possible values are: `Active`, `Disabled`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="aeece-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="aeece-122">JSON representation</span></span>

<span data-ttu-id="aeece-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="aeece-123">The following is a JSON representation of the resource.</span></span>

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