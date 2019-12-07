---
title: 计划资源类型
description: 团队中的 schedulingGroups、倒班、timeOffReasons 和 timesOff 的集合。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType_
ms.openlocfilehash: 6bc92b18bd0529066ef9ade2df9c6ccee9628add
ms.sourcegitcommit: 2ddc63c889fc2f4666aa55bca7ce0221ab899abf
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/07/2019
ms.locfileid: "39895376"
---
# <a name="schedule-resource-type"></a><span data-ttu-id="e3301-103">计划资源类型</span><span class="sxs-lookup"><span data-stu-id="e3301-103">schedule resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e3301-104">一个[团队](../resources/team.md)中的[schedulingGroup](schedulinggroup.md)对象、 [shift](shift.md)对象、 [timeOffReason](timeoffreason.md)对象和[timeOff](timeoff.md)对象的集合。</span><span class="sxs-lookup"><span data-stu-id="e3301-104">A collection of [schedulingGroup](schedulinggroup.md) objects, [shift](shift.md) objects, [timeOffReason](timeoffreason.md) objects, and [timeOff](timeoff.md) objects within a [team](../resources/team.md).</span></span> 

## <a name="methods"></a><span data-ttu-id="e3301-105">方法</span><span class="sxs-lookup"><span data-stu-id="e3301-105">Methods</span></span>

| <span data-ttu-id="e3301-106">方法</span><span class="sxs-lookup"><span data-stu-id="e3301-106">Method</span></span>       | <span data-ttu-id="e3301-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="e3301-107">Return Type</span></span>  |<span data-ttu-id="e3301-108">说明</span><span class="sxs-lookup"><span data-stu-id="e3301-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="e3301-109">创建或替换计划</span><span class="sxs-lookup"><span data-stu-id="e3301-109">Create or replace schedule</span></span>](../api/team-put-schedule.md) | [<span data-ttu-id="e3301-110">日程安排</span><span class="sxs-lookup"><span data-stu-id="e3301-110">schedule</span></span>](schedule.md) | <span data-ttu-id="e3301-111">创建或替换计划。</span><span class="sxs-lookup"><span data-stu-id="e3301-111">Create or replace a schedule.</span></span>|
|[<span data-ttu-id="e3301-112">获取日程安排</span><span class="sxs-lookup"><span data-stu-id="e3301-112">Get schedule</span></span>](../api/schedule-get.md) | [<span data-ttu-id="e3301-113">日程安排</span><span class="sxs-lookup"><span data-stu-id="e3301-113">schedule</span></span>](schedule.md) | <span data-ttu-id="e3301-114">获取日程安排。</span><span class="sxs-lookup"><span data-stu-id="e3301-114">Get a schedule.</span></span>|
|[<span data-ttu-id="e3301-115">共享</span><span class="sxs-lookup"><span data-stu-id="e3301-115">Share</span></span>](../api/schedule-share.md) | <span data-ttu-id="e3301-116">None</span><span class="sxs-lookup"><span data-stu-id="e3301-116">None</span></span> | <span data-ttu-id="e3301-117">与 schedule 成员共享计划时间范围。</span><span class="sxs-lookup"><span data-stu-id="e3301-117">Share a schedule time range with schedule members.</span></span>|

## <a name="properties"></a><span data-ttu-id="e3301-118">属性</span><span class="sxs-lookup"><span data-stu-id="e3301-118">Properties</span></span>
|<span data-ttu-id="e3301-119">名称</span><span class="sxs-lookup"><span data-stu-id="e3301-119">Name</span></span>                   |<span data-ttu-id="e3301-120">类型</span><span class="sxs-lookup"><span data-stu-id="e3301-120">Type</span></span>           |<span data-ttu-id="e3301-121">说明</span><span class="sxs-lookup"><span data-stu-id="e3301-121">Description</span></span>                                                                                                                                      |
|-----------------------|---------------|-------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="e3301-122">id</span><span class="sxs-lookup"><span data-stu-id="e3301-122">id</span></span>                    |<span data-ttu-id="e3301-123">string</span><span class="sxs-lookup"><span data-stu-id="e3301-123">string</span></span>  |<span data-ttu-id="e3301-124">计划的 ID。</span><span class="sxs-lookup"><span data-stu-id="e3301-124">ID of the schedule.</span></span>|
| <span data-ttu-id="e3301-125">enabled</span><span class="sxs-lookup"><span data-stu-id="e3301-125">enabled</span></span>               |<span data-ttu-id="e3301-126">Boolean</span><span class="sxs-lookup"><span data-stu-id="e3301-126">Boolean</span></span>    | <span data-ttu-id="e3301-127">指示是否为团队启用了计划。</span><span class="sxs-lookup"><span data-stu-id="e3301-127">Indicates whether the schedule is enabled for the team.</span></span> <span data-ttu-id="e3301-128">必需。</span><span class="sxs-lookup"><span data-stu-id="e3301-128">Required.</span></span>|
| <span data-ttu-id="e3301-129">timeZone</span><span class="sxs-lookup"><span data-stu-id="e3301-129">timeZone</span></span>              |<span data-ttu-id="e3301-130">string</span><span class="sxs-lookup"><span data-stu-id="e3301-130">string</span></span>  | <span data-ttu-id="e3301-131">指示使用 tz 数据库格式的日程安排团队的时区。</span><span class="sxs-lookup"><span data-stu-id="e3301-131">Indicates the time zone of the schedule team using tz database format.</span></span> <span data-ttu-id="e3301-132">必需。</span><span class="sxs-lookup"><span data-stu-id="e3301-132">Required.</span></span>|
| <span data-ttu-id="e3301-133">provisionStatus</span><span class="sxs-lookup"><span data-stu-id="e3301-133">provisionStatus</span></span>       |<span data-ttu-id="e3301-134">operationStatus</span><span class="sxs-lookup"><span data-stu-id="e3301-134">operationStatus</span></span>    | <span data-ttu-id="e3301-135">调度设置的状态。</span><span class="sxs-lookup"><span data-stu-id="e3301-135">The status of the schedule provisioning.</span></span> <span data-ttu-id="e3301-136">可能的值为`notStarted`、 `running`、 `completed`、 `failed`。</span><span class="sxs-lookup"><span data-stu-id="e3301-136">The possible values are `notStarted`, `running`, `completed`, `failed`.</span></span> |
| <span data-ttu-id="e3301-137">provisionStatusCode</span><span class="sxs-lookup"><span data-stu-id="e3301-137">provisionStatusCode</span></span>   |<span data-ttu-id="e3301-138">string</span><span class="sxs-lookup"><span data-stu-id="e3301-138">string</span></span>  | <span data-ttu-id="e3301-139">有关计划设置失败原因的其他信息。</span><span class="sxs-lookup"><span data-stu-id="e3301-139">Additional information about why schedule provisioning failed.</span></span> |
| <span data-ttu-id="e3301-140">timeClockEnabled</span><span class="sxs-lookup"><span data-stu-id="e3301-140">timeClockEnabled</span></span>                  |<span data-ttu-id="e3301-141">Boolean</span><span class="sxs-lookup"><span data-stu-id="e3301-141">Boolean</span></span>  | <span data-ttu-id="e3301-142">指示是否为计划启用了时间时钟。</span><span class="sxs-lookup"><span data-stu-id="e3301-142">Indicates whether time clock is enabled for the schedule.</span></span>             |
| <span data-ttu-id="e3301-143">openShiftsEnabled</span><span class="sxs-lookup"><span data-stu-id="e3301-143">openShiftsEnabled</span></span>                 |<span data-ttu-id="e3301-144">Boolean</span><span class="sxs-lookup"><span data-stu-id="e3301-144">Boolean</span></span>  | <span data-ttu-id="e3301-145">指示是否为计划启用打开的班次。</span><span class="sxs-lookup"><span data-stu-id="e3301-145">Indicates whether open shifts are enabled for the schedule.</span></span>             | 
| <span data-ttu-id="e3301-146">swapShiftsRequestsEnabled</span><span class="sxs-lookup"><span data-stu-id="e3301-146">swapShiftsRequestsEnabled</span></span>                 |<span data-ttu-id="e3301-147">Boolean</span><span class="sxs-lookup"><span data-stu-id="e3301-147">Boolean</span></span>| <span data-ttu-id="e3301-148">指示是否为计划启用交换倒班请求。</span><span class="sxs-lookup"><span data-stu-id="e3301-148">Indicates whether swap shifts requests are enabled for the schedule.</span></span>             |
| <span data-ttu-id="e3301-149">offerShiftRequestsEnabled</span><span class="sxs-lookup"><span data-stu-id="e3301-149">offerShiftRequestsEnabled</span></span>                 |<span data-ttu-id="e3301-150">Boolean</span><span class="sxs-lookup"><span data-stu-id="e3301-150">Boolean</span></span>  | <span data-ttu-id="e3301-151">指示是否为计划启用了提供倒班请求。</span><span class="sxs-lookup"><span data-stu-id="e3301-151">Indicates whether offer shift requests are enabled for the schedule.</span></span>             | 
| <span data-ttu-id="e3301-152">timeOffRequestsEnabled</span><span class="sxs-lookup"><span data-stu-id="e3301-152">timeOffRequestsEnabled</span></span>                    |<span data-ttu-id="e3301-153">Boolean</span><span class="sxs-lookup"><span data-stu-id="e3301-153">Boolean</span></span> | <span data-ttu-id="e3301-154">指示是否为计划启用时间关请求。</span><span class="sxs-lookup"><span data-stu-id="e3301-154">Indicates whether time off requests are enabled for the schedule.</span></span>             | 



## <a name="relationships"></a><span data-ttu-id="e3301-155">关系</span><span class="sxs-lookup"><span data-stu-id="e3301-155">Relationships</span></span>
|<span data-ttu-id="e3301-156">名称</span><span class="sxs-lookup"><span data-stu-id="e3301-156">Name</span></span>                   |<span data-ttu-id="e3301-157">类型</span><span class="sxs-lookup"><span data-stu-id="e3301-157">Type</span></span>           |<span data-ttu-id="e3301-158">说明</span><span class="sxs-lookup"><span data-stu-id="e3301-158">Description</span></span>                                                                                                                                      |
|-----------------------|---------------|-------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="e3301-159">发生</span><span class="sxs-lookup"><span data-stu-id="e3301-159">shifts</span></span>   | <span data-ttu-id="e3301-160">[shift](shift.md)集合</span><span class="sxs-lookup"><span data-stu-id="e3301-160">[shift](shift.md) collection</span></span>  | <span data-ttu-id="e3301-161">日程中的班次。</span><span class="sxs-lookup"><span data-stu-id="e3301-161">The shifts in the schedule.</span></span> |
| <span data-ttu-id="e3301-162">timesOff</span><span class="sxs-lookup"><span data-stu-id="e3301-162">timesOff</span></span>   |<span data-ttu-id="e3301-163">[timeOff](timeoff.md)集合</span><span class="sxs-lookup"><span data-stu-id="e3301-163">[timeOff](timeoff.md) collection</span></span>  | <span data-ttu-id="e3301-164">计划中的超时实例。</span><span class="sxs-lookup"><span data-stu-id="e3301-164">The instances of times off in the schedule.</span></span> |
| <span data-ttu-id="e3301-165">timeOffReasons</span><span class="sxs-lookup"><span data-stu-id="e3301-165">timeOffReasons</span></span>   |<span data-ttu-id="e3301-166">[timeOffReason](timeoffreason.md)集合</span><span class="sxs-lookup"><span data-stu-id="e3301-166">[timeOffReason](timeoffreason.md) collection</span></span>  | <span data-ttu-id="e3301-167">时间安排中的时间的一组原因。</span><span class="sxs-lookup"><span data-stu-id="e3301-167">The set of reasons for a time off in the schedule.</span></span> |
| <span data-ttu-id="e3301-168">schedulingGroups</span><span class="sxs-lookup"><span data-stu-id="e3301-168">schedulingGroups</span></span>   |<span data-ttu-id="e3301-169">[schedulingGroup](schedulinggroup.md) 集合</span><span class="sxs-lookup"><span data-stu-id="e3301-169">[schedulingGroup](schedulinggroup.md) collection</span></span>  | <span data-ttu-id="e3301-170">按日程安排的用户的逻辑分组（通常按角色）。</span><span class="sxs-lookup"><span data-stu-id="e3301-170">The logical grouping of users in the schedule (usually by role).</span></span> |
| <span data-ttu-id="e3301-171">openshifts</span><span class="sxs-lookup"><span data-stu-id="e3301-171">openshifts</span></span>   |<span data-ttu-id="e3301-172">[openShift](openshift.md)集合</span><span class="sxs-lookup"><span data-stu-id="e3301-172">[openShift](openshift.md) collection</span></span> | <span data-ttu-id="e3301-173">计划组中的一组打开的班次。</span><span class="sxs-lookup"><span data-stu-id="e3301-173">The set of open shifts in a scheduling group in the schedule.</span></span> |
| <span data-ttu-id="e3301-174">workforceintegrations</span><span class="sxs-lookup"><span data-stu-id="e3301-174">workforceintegrations</span></span>   |<span data-ttu-id="e3301-175">[workforceIntegration](workforceintegration.md)集合</span><span class="sxs-lookup"><span data-stu-id="e3301-175">[workforceIntegration](workforceintegration.md) collection</span></span>  | <span data-ttu-id="e3301-176">在同步更改通知（针对受支持的实体）中，每个团队的劳动力集成实例（针对受支持的实体的出站数据流）。</span><span class="sxs-lookup"><span data-stu-id="e3301-176">An instance of a workforce integration per team with outbound data flow on synchronous change notifications (for supported entities).</span></span> |
| <span data-ttu-id="e3301-177">swapshiftchangerequests</span><span class="sxs-lookup"><span data-stu-id="e3301-177">swapshiftchangerequests</span></span>   |<span data-ttu-id="e3301-178">[swapShiftsChangeRequest](swapshiftschangerequest.md)集合</span><span class="sxs-lookup"><span data-stu-id="e3301-178">[swapShiftsChangeRequest](swapshiftschangerequest.md) collection</span></span>  | <span data-ttu-id="e3301-179">计划中倒班的交换请求。</span><span class="sxs-lookup"><span data-stu-id="e3301-179">The swap requests for shifts in the schedule.</span></span> |
| <span data-ttu-id="e3301-180">openshiftchangerequests</span><span class="sxs-lookup"><span data-stu-id="e3301-180">openshiftchangerequests</span></span>   |<span data-ttu-id="e3301-181">[openShiftChangeRequest](openshiftchangerequest.md)集合</span><span class="sxs-lookup"><span data-stu-id="e3301-181">[openShiftChangeRequest](openshiftchangerequest.md) collection</span></span>  | <span data-ttu-id="e3301-182">计划中打开的班次请求。</span><span class="sxs-lookup"><span data-stu-id="e3301-182">The open shift requests in the schedule.</span></span> |
| <span data-ttu-id="e3301-183">timeoffrequest</span><span class="sxs-lookup"><span data-stu-id="e3301-183">timeoffrequest</span></span>   |<span data-ttu-id="e3301-184">[timeOffRequest](timeoffrequest.md)集合</span><span class="sxs-lookup"><span data-stu-id="e3301-184">[timeOffRequest](timeoffrequest.md) collection</span></span>  | <span data-ttu-id="e3301-185">计划中的休息时间请求。</span><span class="sxs-lookup"><span data-stu-id="e3301-185">The time off requests in the schedule.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="e3301-186">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e3301-186">JSON representation</span></span>

<span data-ttu-id="e3301-187">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e3301-187">The following is a JSON representation of the resource.</span></span>

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
