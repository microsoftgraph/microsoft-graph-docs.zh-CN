---
title: 计划资源类型
description: 团队中的 schedulingGroups、倒班、timeOffReasons 和 timesOff 的集合。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: de3662fcf3c5a8e50493e365f6a10a8641a451df
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32563104"
---
# <a name="schedule-resource-type"></a><span data-ttu-id="512fa-103">计划资源类型</span><span class="sxs-lookup"><span data-stu-id="512fa-103">schedule resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="512fa-104">一个[团队](../resources/team.md)中的[schedulingGroup](schedulinggroup.md)对象、 [shift](shift.md)对象、 [timeOffReason](timeoffreason.md)对象和[timeOff](timeoff.md)对象的集合。</span><span class="sxs-lookup"><span data-stu-id="512fa-104">A collection of [schedulingGroup](schedulinggroup.md) objects, [shift](shift.md) objects, [timeOffReason](timeoffreason.md) objects, and [timeOff](timeoff.md) objects within a [team](../resources/team.md).</span></span> 

## <a name="methods"></a><span data-ttu-id="512fa-105">方法</span><span class="sxs-lookup"><span data-stu-id="512fa-105">Methods</span></span>

| <span data-ttu-id="512fa-106">方法</span><span class="sxs-lookup"><span data-stu-id="512fa-106">Method</span></span>       | <span data-ttu-id="512fa-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="512fa-107">Return Type</span></span>  |<span data-ttu-id="512fa-108">说明</span><span class="sxs-lookup"><span data-stu-id="512fa-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="512fa-109">创建或替换计划</span><span class="sxs-lookup"><span data-stu-id="512fa-109">Create or replace schedule</span></span>](../api/team-put-schedule.md) | [<span data-ttu-id="512fa-110">设定</span><span class="sxs-lookup"><span data-stu-id="512fa-110">schedule</span></span>](schedule.md) | <span data-ttu-id="512fa-111">创建或替换`schedule`。</span><span class="sxs-lookup"><span data-stu-id="512fa-111">Create or replace a `schedule`.</span></span>|
|[<span data-ttu-id="512fa-112">获取日程安排</span><span class="sxs-lookup"><span data-stu-id="512fa-112">Get schedule</span></span>](../api/schedule-get.md) | [<span data-ttu-id="512fa-113">设定</span><span class="sxs-lookup"><span data-stu-id="512fa-113">schedule</span></span>](schedule.md) | <span data-ttu-id="512fa-114">获取`schedule`。</span><span class="sxs-lookup"><span data-stu-id="512fa-114">Get a `schedule`.</span></span>|
|[<span data-ttu-id="512fa-115">share</span><span class="sxs-lookup"><span data-stu-id="512fa-115">share</span></span>](../api/schedule-share.md) | <span data-ttu-id="512fa-116">无</span><span class="sxs-lookup"><span data-stu-id="512fa-116">None</span></span> | <span data-ttu-id="512fa-117">与 schedule `schedule`成员共享时间范围。</span><span class="sxs-lookup"><span data-stu-id="512fa-117">Share a `schedule` time range with schedule members.</span></span>|

## <a name="properties"></a><span data-ttu-id="512fa-118">属性</span><span class="sxs-lookup"><span data-stu-id="512fa-118">Properties</span></span>
|<span data-ttu-id="512fa-119">名称</span><span class="sxs-lookup"><span data-stu-id="512fa-119">Name</span></span>                   |<span data-ttu-id="512fa-120">类型</span><span class="sxs-lookup"><span data-stu-id="512fa-120">Type</span></span>           |<span data-ttu-id="512fa-121">说明</span><span class="sxs-lookup"><span data-stu-id="512fa-121">Description</span></span>                                                                                                                                      |
|-----------------------|---------------|-------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="512fa-122">id</span><span class="sxs-lookup"><span data-stu-id="512fa-122">id</span></span>                    |`string`  |<span data-ttu-id="512fa-123">`schedule` 的 ID。</span><span class="sxs-lookup"><span data-stu-id="512fa-123">ID of the `schedule`.</span></span>|
| <span data-ttu-id="512fa-124">enabled</span><span class="sxs-lookup"><span data-stu-id="512fa-124">enabled</span></span>               |`bool`    | <span data-ttu-id="512fa-125">指示是否为团队启用了计划。</span><span class="sxs-lookup"><span data-stu-id="512fa-125">Indicates whether the schedule is enabled for the team.</span></span> <span data-ttu-id="512fa-126">必需。</span><span class="sxs-lookup"><span data-stu-id="512fa-126">Required.</span></span>|
| <span data-ttu-id="512fa-127">timeZone</span><span class="sxs-lookup"><span data-stu-id="512fa-127">timeZone</span></span>              |`string`  | <span data-ttu-id="512fa-128">指示使用 tz 数据库格式的日程安排团队的时区。</span><span class="sxs-lookup"><span data-stu-id="512fa-128">Indicates the time zone of the schedule team using tz database format.</span></span> <span data-ttu-id="512fa-129">必需。</span><span class="sxs-lookup"><span data-stu-id="512fa-129">Required.</span></span>|
| <span data-ttu-id="512fa-130">provisionStatus</span><span class="sxs-lookup"><span data-stu-id="512fa-130">provisionStatus</span></span>       |`enum`    | <span data-ttu-id="512fa-131">调度设置的状态。</span><span class="sxs-lookup"><span data-stu-id="512fa-131">The status of the schedule provisioning.</span></span> |
| <span data-ttu-id="512fa-132">provisionStatusCode</span><span class="sxs-lookup"><span data-stu-id="512fa-132">provisionStatusCode</span></span>   |`string`  | <span data-ttu-id="512fa-133">有关计划设置失败原因的其他信息。</span><span class="sxs-lookup"><span data-stu-id="512fa-133">Additional information about why schedule provisioning failed.</span></span> |


## <a name="relationships"></a><span data-ttu-id="512fa-134">关系</span><span class="sxs-lookup"><span data-stu-id="512fa-134">Relationships</span></span>
|<span data-ttu-id="512fa-135">名称</span><span class="sxs-lookup"><span data-stu-id="512fa-135">Name</span></span>                   |<span data-ttu-id="512fa-136">类型</span><span class="sxs-lookup"><span data-stu-id="512fa-136">Type</span></span>           |<span data-ttu-id="512fa-137">说明</span><span class="sxs-lookup"><span data-stu-id="512fa-137">Description</span></span>                                                                                                                                      |
|-----------------------|---------------|-------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="512fa-138">发生</span><span class="sxs-lookup"><span data-stu-id="512fa-138">shifts</span></span>   |`collection(shift)`  | <span data-ttu-id="512fa-139">日程中的班次。</span><span class="sxs-lookup"><span data-stu-id="512fa-139">The shifts in the schedule.</span></span> |
| <span data-ttu-id="512fa-140">timesOff</span><span class="sxs-lookup"><span data-stu-id="512fa-140">timesOff</span></span>   |`collection(timeOff)`  | <span data-ttu-id="512fa-141">计划中的超时实例。</span><span class="sxs-lookup"><span data-stu-id="512fa-141">The instances of times off in the schedule.</span></span> |
| <span data-ttu-id="512fa-142">timeOffReasons</span><span class="sxs-lookup"><span data-stu-id="512fa-142">timeOffReasons</span></span>   |`collection(timeOffReason)`  | <span data-ttu-id="512fa-143">时间安排中的时间的一组原因。</span><span class="sxs-lookup"><span data-stu-id="512fa-143">The set of reasons for a time off in the schedule.</span></span> |
| <span data-ttu-id="512fa-144">schedulingGroups</span><span class="sxs-lookup"><span data-stu-id="512fa-144">schedulingGroups</span></span>   |`collection(schedulingGroup)`  | <span data-ttu-id="512fa-145">按日程安排的用户的逻辑分组 (通常按角色)。</span><span class="sxs-lookup"><span data-stu-id="512fa-145">The logical grouping of users in the schedule (usually by role).</span></span> |


## <a name="json-representation"></a><span data-ttu-id="512fa-146">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="512fa-146">JSON representation</span></span>

<span data-ttu-id="512fa-147">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="512fa-147">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.schedule"
}-->

```json
{
  "id": "833fc4df-c88b-4398-992f-d8afcfe41df2",
  "enabled": true,
  "timeZone": "America/Chicago",
  "provisionStatus": "Completed",
  "provisionStatusCode": null
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "schedule resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/schedule.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
