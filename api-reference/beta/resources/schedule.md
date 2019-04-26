---
title: 计划资源类型
description: 团队中的 schedulingGroups、倒班、timeOffReasons 和 timesOff 的集合。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 48b3b5c118a39442469bc6155068664fcebe0ec2
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33343519"
---
# <a name="schedule-resource-type"></a><span data-ttu-id="95e67-103">计划资源类型</span><span class="sxs-lookup"><span data-stu-id="95e67-103">schedule resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="95e67-104">一个[团队](../resources/team.md)中的[schedulingGroup](schedulinggroup.md)对象、 [shift](shift.md)对象、 [timeOffReason](timeoffreason.md)对象和[timeOff](timeoff.md)对象的集合。</span><span class="sxs-lookup"><span data-stu-id="95e67-104">A collection of [schedulingGroup](schedulinggroup.md) objects, [shift](shift.md) objects, [timeOffReason](timeoffreason.md) objects, and [timeOff](timeoff.md) objects within a [team](../resources/team.md).</span></span> 

## <a name="methods"></a><span data-ttu-id="95e67-105">方法</span><span class="sxs-lookup"><span data-stu-id="95e67-105">Methods</span></span>

| <span data-ttu-id="95e67-106">方法</span><span class="sxs-lookup"><span data-stu-id="95e67-106">Method</span></span>       | <span data-ttu-id="95e67-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="95e67-107">Return Type</span></span>  |<span data-ttu-id="95e67-108">说明</span><span class="sxs-lookup"><span data-stu-id="95e67-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="95e67-109">创建或替换计划</span><span class="sxs-lookup"><span data-stu-id="95e67-109">Create or replace schedule</span></span>](../api/team-put-schedule.md) | [<span data-ttu-id="95e67-110">设定</span><span class="sxs-lookup"><span data-stu-id="95e67-110">schedule</span></span>](schedule.md) | <span data-ttu-id="95e67-111">创建或替换`schedule`。</span><span class="sxs-lookup"><span data-stu-id="95e67-111">Create or replace a `schedule`.</span></span>|
|[<span data-ttu-id="95e67-112">获取日程安排</span><span class="sxs-lookup"><span data-stu-id="95e67-112">Get schedule</span></span>](../api/schedule-get.md) | [<span data-ttu-id="95e67-113">设定</span><span class="sxs-lookup"><span data-stu-id="95e67-113">schedule</span></span>](schedule.md) | <span data-ttu-id="95e67-114">获取`schedule`。</span><span class="sxs-lookup"><span data-stu-id="95e67-114">Get a `schedule`.</span></span>|
|[<span data-ttu-id="95e67-115">share</span><span class="sxs-lookup"><span data-stu-id="95e67-115">share</span></span>](../api/schedule-share.md) | <span data-ttu-id="95e67-116">无</span><span class="sxs-lookup"><span data-stu-id="95e67-116">None</span></span> | <span data-ttu-id="95e67-117">与 schedule `schedule`成员共享时间范围。</span><span class="sxs-lookup"><span data-stu-id="95e67-117">Share a `schedule` time range with schedule members.</span></span>|

## <a name="properties"></a><span data-ttu-id="95e67-118">属性</span><span class="sxs-lookup"><span data-stu-id="95e67-118">Properties</span></span>
|<span data-ttu-id="95e67-119">名称</span><span class="sxs-lookup"><span data-stu-id="95e67-119">Name</span></span>                   |<span data-ttu-id="95e67-120">类型</span><span class="sxs-lookup"><span data-stu-id="95e67-120">Type</span></span>           |<span data-ttu-id="95e67-121">说明</span><span class="sxs-lookup"><span data-stu-id="95e67-121">Description</span></span>                                                                                                                                      |
|-----------------------|---------------|-------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="95e67-122">id</span><span class="sxs-lookup"><span data-stu-id="95e67-122">id</span></span>                    |`string`  |<span data-ttu-id="95e67-123">`schedule` 的 ID。</span><span class="sxs-lookup"><span data-stu-id="95e67-123">ID of the `schedule`.</span></span>|
| <span data-ttu-id="95e67-124">enabled</span><span class="sxs-lookup"><span data-stu-id="95e67-124">enabled</span></span>               |`bool`    | <span data-ttu-id="95e67-125">指示是否为团队启用了计划。</span><span class="sxs-lookup"><span data-stu-id="95e67-125">Indicates whether the schedule is enabled for the team.</span></span> <span data-ttu-id="95e67-126">必需。</span><span class="sxs-lookup"><span data-stu-id="95e67-126">Required.</span></span>|
| <span data-ttu-id="95e67-127">timeZone</span><span class="sxs-lookup"><span data-stu-id="95e67-127">timeZone</span></span>              |`string`  | <span data-ttu-id="95e67-128">指示使用 tz 数据库格式的日程安排团队的时区。</span><span class="sxs-lookup"><span data-stu-id="95e67-128">Indicates the time zone of the schedule team using tz database format.</span></span> <span data-ttu-id="95e67-129">必需。</span><span class="sxs-lookup"><span data-stu-id="95e67-129">Required.</span></span>|
| <span data-ttu-id="95e67-130">provisionStatus</span><span class="sxs-lookup"><span data-stu-id="95e67-130">provisionStatus</span></span>       |`operationStatus`    | <span data-ttu-id="95e67-131">调度设置的状态。</span><span class="sxs-lookup"><span data-stu-id="95e67-131">The status of the schedule provisioning.</span></span> <span data-ttu-id="95e67-132">可能的值为`notStarted`、 `running`、 `completed`、 `failed`。</span><span class="sxs-lookup"><span data-stu-id="95e67-132">The possible values are `notStarted`, `running`, `completed`, `failed`.</span></span> |
| <span data-ttu-id="95e67-133">provisionStatusCode</span><span class="sxs-lookup"><span data-stu-id="95e67-133">provisionStatusCode</span></span>   |`string`  | <span data-ttu-id="95e67-134">有关计划设置失败原因的其他信息。</span><span class="sxs-lookup"><span data-stu-id="95e67-134">Additional information about why schedule provisioning failed.</span></span> |


## <a name="relationships"></a><span data-ttu-id="95e67-135">关系</span><span class="sxs-lookup"><span data-stu-id="95e67-135">Relationships</span></span>
|<span data-ttu-id="95e67-136">名称</span><span class="sxs-lookup"><span data-stu-id="95e67-136">Name</span></span>                   |<span data-ttu-id="95e67-137">类型</span><span class="sxs-lookup"><span data-stu-id="95e67-137">Type</span></span>           |<span data-ttu-id="95e67-138">说明</span><span class="sxs-lookup"><span data-stu-id="95e67-138">Description</span></span>                                                                                                                                      |
|-----------------------|---------------|-------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="95e67-139">发生</span><span class="sxs-lookup"><span data-stu-id="95e67-139">shifts</span></span>   |`collection(shift)`  | <span data-ttu-id="95e67-140">日程中的班次。</span><span class="sxs-lookup"><span data-stu-id="95e67-140">The shifts in the schedule.</span></span> |
| <span data-ttu-id="95e67-141">timesOff</span><span class="sxs-lookup"><span data-stu-id="95e67-141">timesOff</span></span>   |`collection(timeOff)`  | <span data-ttu-id="95e67-142">计划中的超时实例。</span><span class="sxs-lookup"><span data-stu-id="95e67-142">The instances of times off in the schedule.</span></span> |
| <span data-ttu-id="95e67-143">timeOffReasons</span><span class="sxs-lookup"><span data-stu-id="95e67-143">timeOffReasons</span></span>   |`collection(timeOffReason)`  | <span data-ttu-id="95e67-144">时间安排中的时间的一组原因。</span><span class="sxs-lookup"><span data-stu-id="95e67-144">The set of reasons for a time off in the schedule.</span></span> |
| <span data-ttu-id="95e67-145">schedulingGroups</span><span class="sxs-lookup"><span data-stu-id="95e67-145">schedulingGroups</span></span>   |`collection(schedulingGroup)`  | <span data-ttu-id="95e67-146">按日程安排的用户的逻辑分组 (通常按角色)。</span><span class="sxs-lookup"><span data-stu-id="95e67-146">The logical grouping of users in the schedule (usually by role).</span></span> |


## <a name="json-representation"></a><span data-ttu-id="95e67-147">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="95e67-147">JSON representation</span></span>

<span data-ttu-id="95e67-148">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="95e67-148">Here is a JSON representation of the resource.</span></span>

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
  "suppressions": []
}
-->
