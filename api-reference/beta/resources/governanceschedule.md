---
title: governanceSchedule 资源类型
description: '代表 governanceRoleAssignmentRequest 的日程安排。 对于角色分配请求, 日程安排控制何时执行角色分配操作、何时停止角色分配以及执行角色分配操作的频率。 '
localization_priority: Normal
ms.openlocfilehash: 798b2a7f3e67ac466189f1ece55437214931056d
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33340287"
---
# <a name="governanceschedule-resource-type"></a><span data-ttu-id="a2712-104">governanceSchedule 资源类型</span><span class="sxs-lookup"><span data-stu-id="a2712-104">governanceSchedule resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a2712-105">代表[governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)的日程安排。</span><span class="sxs-lookup"><span data-stu-id="a2712-105">Represents the schedule for a [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md).</span></span> <span data-ttu-id="a2712-106">对于角色分配请求, 日程安排控制何时执行角色分配操作、何时停止角色分配以及执行角色分配操作的频率。</span><span class="sxs-lookup"><span data-stu-id="a2712-106">For a role assignment request, the schedule controls when to perform the role assignment operation, when to stop the role assignment, and how frequently to do the role assignment operation.</span></span> 



## <a name="properties"></a><span data-ttu-id="a2712-107">属性</span><span class="sxs-lookup"><span data-stu-id="a2712-107">Properties</span></span>
| <span data-ttu-id="a2712-108">属性</span><span class="sxs-lookup"><span data-stu-id="a2712-108">Property</span></span>     | <span data-ttu-id="a2712-109">类型</span><span class="sxs-lookup"><span data-stu-id="a2712-109">Type</span></span>   |<span data-ttu-id="a2712-110">说明</span><span class="sxs-lookup"><span data-stu-id="a2712-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a2712-111">startDateTime</span><span class="sxs-lookup"><span data-stu-id="a2712-111">startDateTime</span></span>|<span data-ttu-id="a2712-112">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a2712-112">DateTimeOffset</span></span>|<span data-ttu-id="a2712-113">角色分配的开始时间。</span><span class="sxs-lookup"><span data-stu-id="a2712-113">The start time of the role assignment.</span></span> <span data-ttu-id="a2712-114">时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="a2712-114">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="a2712-115">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="a2712-115">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="a2712-116">endDateTime</span><span class="sxs-lookup"><span data-stu-id="a2712-116">endDateTime</span></span>|<span data-ttu-id="a2712-117">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a2712-117">DateTimeOffset</span></span>|<span data-ttu-id="a2712-118">角色分配的结束时间。</span><span class="sxs-lookup"><span data-stu-id="a2712-118">The end time of the role assignment.</span></span> <span data-ttu-id="a2712-119">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="a2712-119">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="a2712-120">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。</span><span class="sxs-lookup"><span data-stu-id="a2712-120">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="a2712-121">*注意: 如果值为`null`, 则表示永久分配。*</span><span class="sxs-lookup"><span data-stu-id="a2712-121">*Note: if the value is `null`, it indicates a permanent assignment.*</span></span>|
|<span data-ttu-id="a2712-122">type</span><span class="sxs-lookup"><span data-stu-id="a2712-122">type</span></span>|<span data-ttu-id="a2712-123">String</span><span class="sxs-lookup"><span data-stu-id="a2712-123">String</span></span>|<span data-ttu-id="a2712-124">角色分配计划类型。</span><span class="sxs-lookup"><span data-stu-id="a2712-124">The role assignment schedule type.</span></span> <span data-ttu-id="a2712-125">目前`Once`仅支持。</span><span class="sxs-lookup"><span data-stu-id="a2712-125">Only `Once` is supported for now.</span></span>
|<span data-ttu-id="a2712-126">duration</span><span class="sxs-lookup"><span data-stu-id="a2712-126">duration</span></span>|<span data-ttu-id="a2712-127">持续时间</span><span class="sxs-lookup"><span data-stu-id="a2712-127">Duration</span></span>|<span data-ttu-id="a2712-128">角色分配的持续时间。</span><span class="sxs-lookup"><span data-stu-id="a2712-128">The duration of a role assignment.</span></span> <span data-ttu-id="a2712-129">它的格式为 TimeSpan。</span><span class="sxs-lookup"><span data-stu-id="a2712-129">It is in format of a TimeSpan.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a2712-130">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a2712-130">JSON representation</span></span>

<span data-ttu-id="a2712-131">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a2712-131">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.governanceSchedule"
}-->

```json
{
  "duration": "String (timespan)",
  "startDateTime": "String (timestamp)",
  "endDateTime": "String (timestamp)",
  "type": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "governanceSchedule",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
