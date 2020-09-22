---
title: 计划资源类型
description: 团队中的 schedulingGroups、倒班、timeOffReasons 和 timesOff 的集合。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: f0b3f621028c0e15634203e34d92c4d8abb6f6bb
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47985837"
---
# <a name="schedule-resource-type"></a><span data-ttu-id="873d9-103">计划资源类型</span><span class="sxs-lookup"><span data-stu-id="873d9-103">schedule resource type</span></span>

<span data-ttu-id="873d9-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="873d9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="873d9-105">一个[团队](../resources/team.md)中的[schedulingGroup](schedulinggroup.md)对象、 [shift](shift.md)对象、 [timeOffReason](timeoffreason.md)对象和[timeOff](timeoff.md)对象的集合。</span><span class="sxs-lookup"><span data-stu-id="873d9-105">A collection of [schedulingGroup](schedulinggroup.md) objects, [shift](shift.md) objects, [timeOffReason](timeoffreason.md) objects, and [timeOff](timeoff.md) objects within a [team](../resources/team.md).</span></span> 

## <a name="methods"></a><span data-ttu-id="873d9-106">方法</span><span class="sxs-lookup"><span data-stu-id="873d9-106">Methods</span></span>

| <span data-ttu-id="873d9-107">方法</span><span class="sxs-lookup"><span data-stu-id="873d9-107">Method</span></span>       | <span data-ttu-id="873d9-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="873d9-108">Return Type</span></span>  |<span data-ttu-id="873d9-109">说明</span><span class="sxs-lookup"><span data-stu-id="873d9-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="873d9-110">创建或替换计划</span><span class="sxs-lookup"><span data-stu-id="873d9-110">Create or replace schedule</span></span>](../api/team-put-schedule.md) | [<span data-ttu-id="873d9-111">日程安排</span><span class="sxs-lookup"><span data-stu-id="873d9-111">schedule</span></span>](schedule.md) | <span data-ttu-id="873d9-112">创建或替换计划。</span><span class="sxs-lookup"><span data-stu-id="873d9-112">Create or replace a schedule.</span></span>|
|[<span data-ttu-id="873d9-113">获取日程安排</span><span class="sxs-lookup"><span data-stu-id="873d9-113">Get schedule</span></span>](../api/schedule-get.md) | [<span data-ttu-id="873d9-114">日程安排</span><span class="sxs-lookup"><span data-stu-id="873d9-114">schedule</span></span>](schedule.md) | <span data-ttu-id="873d9-115">获取日程安排。</span><span class="sxs-lookup"><span data-stu-id="873d9-115">Get a schedule.</span></span>|
|[<span data-ttu-id="873d9-116">共享</span><span class="sxs-lookup"><span data-stu-id="873d9-116">Share</span></span>](../api/schedule-share.md) | <span data-ttu-id="873d9-117">无</span><span class="sxs-lookup"><span data-stu-id="873d9-117">None</span></span> | <span data-ttu-id="873d9-118">与 schedule 成员共享计划时间范围。</span><span class="sxs-lookup"><span data-stu-id="873d9-118">Share a schedule time range with schedule members.</span></span>|

## <a name="properties"></a><span data-ttu-id="873d9-119">属性</span><span class="sxs-lookup"><span data-stu-id="873d9-119">Properties</span></span>
|<span data-ttu-id="873d9-120">名称</span><span class="sxs-lookup"><span data-stu-id="873d9-120">Name</span></span>                   |<span data-ttu-id="873d9-121">类型</span><span class="sxs-lookup"><span data-stu-id="873d9-121">Type</span></span>           |<span data-ttu-id="873d9-122">说明</span><span class="sxs-lookup"><span data-stu-id="873d9-122">Description</span></span>                                                                                                                                      |
|-----------------------|---------------|-------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="873d9-123">id</span><span class="sxs-lookup"><span data-stu-id="873d9-123">id</span></span>                    |<span data-ttu-id="873d9-124">string</span><span class="sxs-lookup"><span data-stu-id="873d9-124">string</span></span>  |<span data-ttu-id="873d9-125">计划的 ID。</span><span class="sxs-lookup"><span data-stu-id="873d9-125">ID of the schedule.</span></span>|
| <span data-ttu-id="873d9-126">enabled</span><span class="sxs-lookup"><span data-stu-id="873d9-126">enabled</span></span>               |<span data-ttu-id="873d9-127">Boolean</span><span class="sxs-lookup"><span data-stu-id="873d9-127">Boolean</span></span>    | <span data-ttu-id="873d9-128">指示是否为团队启用了计划。</span><span class="sxs-lookup"><span data-stu-id="873d9-128">Indicates whether the schedule is enabled for the team.</span></span> <span data-ttu-id="873d9-129">必需。</span><span class="sxs-lookup"><span data-stu-id="873d9-129">Required.</span></span>|
| <span data-ttu-id="873d9-130">timeZone</span><span class="sxs-lookup"><span data-stu-id="873d9-130">timeZone</span></span>              |<span data-ttu-id="873d9-131">string</span><span class="sxs-lookup"><span data-stu-id="873d9-131">string</span></span>  | <span data-ttu-id="873d9-132">指示使用 tz 数据库格式的日程安排团队的时区。</span><span class="sxs-lookup"><span data-stu-id="873d9-132">Indicates the time zone of the schedule team using tz database format.</span></span> <span data-ttu-id="873d9-133">必需。</span><span class="sxs-lookup"><span data-stu-id="873d9-133">Required.</span></span>|
| <span data-ttu-id="873d9-134">provisionStatus</span><span class="sxs-lookup"><span data-stu-id="873d9-134">provisionStatus</span></span>       |<span data-ttu-id="873d9-135">operationStatus</span><span class="sxs-lookup"><span data-stu-id="873d9-135">operationStatus</span></span>    | <span data-ttu-id="873d9-136">调度设置的状态。</span><span class="sxs-lookup"><span data-stu-id="873d9-136">The status of the schedule provisioning.</span></span> <span data-ttu-id="873d9-137">可能的值为 `notStarted` 、 `running` 、 `completed` 、 `failed` 。</span><span class="sxs-lookup"><span data-stu-id="873d9-137">The possible values are `notStarted`, `running`, `completed`, `failed`.</span></span> |
| <span data-ttu-id="873d9-138">provisionStatusCode</span><span class="sxs-lookup"><span data-stu-id="873d9-138">provisionStatusCode</span></span>   |<span data-ttu-id="873d9-139">字符串</span><span class="sxs-lookup"><span data-stu-id="873d9-139">string</span></span>  | <span data-ttu-id="873d9-140">有关计划设置失败原因的其他信息。</span><span class="sxs-lookup"><span data-stu-id="873d9-140">Additional information about why schedule provisioning failed.</span></span> |
| <span data-ttu-id="873d9-141">timeClockEnabled</span><span class="sxs-lookup"><span data-stu-id="873d9-141">timeClockEnabled</span></span>                  |<span data-ttu-id="873d9-142">Boolean</span><span class="sxs-lookup"><span data-stu-id="873d9-142">Boolean</span></span>  | <span data-ttu-id="873d9-143">指示是否为计划启用了时间时钟。</span><span class="sxs-lookup"><span data-stu-id="873d9-143">Indicates whether time clock is enabled for the schedule.</span></span>             |
| <span data-ttu-id="873d9-144">openShiftsEnabled</span><span class="sxs-lookup"><span data-stu-id="873d9-144">openShiftsEnabled</span></span>                 |<span data-ttu-id="873d9-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="873d9-145">Boolean</span></span>  | <span data-ttu-id="873d9-146">指示是否为计划启用打开的班次。</span><span class="sxs-lookup"><span data-stu-id="873d9-146">Indicates whether open shifts are enabled for the schedule.</span></span>             | 
| <span data-ttu-id="873d9-147">swapShiftsRequestsEnabled</span><span class="sxs-lookup"><span data-stu-id="873d9-147">swapShiftsRequestsEnabled</span></span>                 |<span data-ttu-id="873d9-148">Boolean</span><span class="sxs-lookup"><span data-stu-id="873d9-148">Boolean</span></span>| <span data-ttu-id="873d9-149">指示是否为计划启用交换倒班请求。</span><span class="sxs-lookup"><span data-stu-id="873d9-149">Indicates whether swap shifts requests are enabled for the schedule.</span></span>             |
| <span data-ttu-id="873d9-150">offerShiftRequestsEnabled</span><span class="sxs-lookup"><span data-stu-id="873d9-150">offerShiftRequestsEnabled</span></span>                 |<span data-ttu-id="873d9-151">Boolean</span><span class="sxs-lookup"><span data-stu-id="873d9-151">Boolean</span></span>  | <span data-ttu-id="873d9-152">指示是否为计划启用了提供倒班请求。</span><span class="sxs-lookup"><span data-stu-id="873d9-152">Indicates whether offer shift requests are enabled for the schedule.</span></span>             | 
| <span data-ttu-id="873d9-153">timeOffRequestsEnabled</span><span class="sxs-lookup"><span data-stu-id="873d9-153">timeOffRequestsEnabled</span></span>                    |<span data-ttu-id="873d9-154">Boolean</span><span class="sxs-lookup"><span data-stu-id="873d9-154">Boolean</span></span> | <span data-ttu-id="873d9-155">指示是否为计划启用时间关请求。</span><span class="sxs-lookup"><span data-stu-id="873d9-155">Indicates whether time off requests are enabled for the schedule.</span></span>             | 



## <a name="relationships"></a><span data-ttu-id="873d9-156">关系</span><span class="sxs-lookup"><span data-stu-id="873d9-156">Relationships</span></span>
|<span data-ttu-id="873d9-157">名称</span><span class="sxs-lookup"><span data-stu-id="873d9-157">Name</span></span>                   |<span data-ttu-id="873d9-158">类型</span><span class="sxs-lookup"><span data-stu-id="873d9-158">Type</span></span>           |<span data-ttu-id="873d9-159">说明</span><span class="sxs-lookup"><span data-stu-id="873d9-159">Description</span></span>                                                                                                                                      |
|-----------------------|---------------|-------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="873d9-160">发生</span><span class="sxs-lookup"><span data-stu-id="873d9-160">shifts</span></span>   | <span data-ttu-id="873d9-161">[shift](shift.md) 集合</span><span class="sxs-lookup"><span data-stu-id="873d9-161">[shift](shift.md) collection</span></span>  | <span data-ttu-id="873d9-162">日程中的班次。</span><span class="sxs-lookup"><span data-stu-id="873d9-162">The shifts in the schedule.</span></span> |
| <span data-ttu-id="873d9-163">timesOff</span><span class="sxs-lookup"><span data-stu-id="873d9-163">timesOff</span></span>   |<span data-ttu-id="873d9-164">[timeOff](timeoff.md) 集合</span><span class="sxs-lookup"><span data-stu-id="873d9-164">[timeOff](timeoff.md) collection</span></span>  | <span data-ttu-id="873d9-165">计划中的超时实例。</span><span class="sxs-lookup"><span data-stu-id="873d9-165">The instances of times off in the schedule.</span></span> |
| <span data-ttu-id="873d9-166">timeOffReasons</span><span class="sxs-lookup"><span data-stu-id="873d9-166">timeOffReasons</span></span>   |<span data-ttu-id="873d9-167">[timeOffReason](timeoffreason.md) 集合</span><span class="sxs-lookup"><span data-stu-id="873d9-167">[timeOffReason](timeoffreason.md) collection</span></span>  | <span data-ttu-id="873d9-168">时间安排中的时间的一组原因。</span><span class="sxs-lookup"><span data-stu-id="873d9-168">The set of reasons for a time off in the schedule.</span></span> |
| <span data-ttu-id="873d9-169">schedulingGroups</span><span class="sxs-lookup"><span data-stu-id="873d9-169">schedulingGroups</span></span>   |<span data-ttu-id="873d9-170">[schedulingGroup](schedulinggroup.md) 集合</span><span class="sxs-lookup"><span data-stu-id="873d9-170">[schedulingGroup](schedulinggroup.md) collection</span></span>  | <span data-ttu-id="873d9-171"> (通常由角色) 的日程安排中的用户的逻辑分组。</span><span class="sxs-lookup"><span data-stu-id="873d9-171">The logical grouping of users in the schedule (usually by role).</span></span> |
| <span data-ttu-id="873d9-172">openshifts</span><span class="sxs-lookup"><span data-stu-id="873d9-172">openshifts</span></span>   |<span data-ttu-id="873d9-173">[openShift](openshift.md) 集合</span><span class="sxs-lookup"><span data-stu-id="873d9-173">[openShift](openshift.md) collection</span></span> | <span data-ttu-id="873d9-174">计划组中的一组打开的班次。</span><span class="sxs-lookup"><span data-stu-id="873d9-174">The set of open shifts in a scheduling group in the schedule.</span></span> |
| <span data-ttu-id="873d9-175">workforceintegrations</span><span class="sxs-lookup"><span data-stu-id="873d9-175">workforceintegrations</span></span>   |<span data-ttu-id="873d9-176">[workforceIntegration](workforceintegration.md) 集合</span><span class="sxs-lookup"><span data-stu-id="873d9-176">[workforceIntegration](workforceintegration.md) collection</span></span>  | <span data-ttu-id="873d9-177">每个团队的劳动力集成实例，在同步更改通知中对受支持的实体的出站数据流 () 。</span><span class="sxs-lookup"><span data-stu-id="873d9-177">An instance of a workforce integration per team with outbound data flow on synchronous change notifications (for supported entities).</span></span> |
| <span data-ttu-id="873d9-178">swapshiftchangerequests</span><span class="sxs-lookup"><span data-stu-id="873d9-178">swapshiftchangerequests</span></span>   |<span data-ttu-id="873d9-179">[swapShiftsChangeRequest](swapshiftschangerequest.md) 集合</span><span class="sxs-lookup"><span data-stu-id="873d9-179">[swapShiftsChangeRequest](swapshiftschangerequest.md) collection</span></span>  | <span data-ttu-id="873d9-180">计划中倒班的交换请求。</span><span class="sxs-lookup"><span data-stu-id="873d9-180">The swap requests for shifts in the schedule.</span></span> |
| <span data-ttu-id="873d9-181">openshiftchangerequests</span><span class="sxs-lookup"><span data-stu-id="873d9-181">openshiftchangerequests</span></span>   |<span data-ttu-id="873d9-182">[openShiftChangeRequest](openshiftchangerequest.md) 集合</span><span class="sxs-lookup"><span data-stu-id="873d9-182">[openShiftChangeRequest](openshiftchangerequest.md) collection</span></span>  | <span data-ttu-id="873d9-183">计划中打开的班次请求。</span><span class="sxs-lookup"><span data-stu-id="873d9-183">The open shift requests in the schedule.</span></span> |
| <span data-ttu-id="873d9-184">timeoffrequest</span><span class="sxs-lookup"><span data-stu-id="873d9-184">timeoffrequest</span></span>   |<span data-ttu-id="873d9-185">[timeOffRequest](timeoffrequest.md) 集合</span><span class="sxs-lookup"><span data-stu-id="873d9-185">[timeOffRequest](timeoffrequest.md) collection</span></span>  | <span data-ttu-id="873d9-186">计划中的休息时间请求。</span><span class="sxs-lookup"><span data-stu-id="873d9-186">The time off requests in the schedule.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="873d9-187">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="873d9-187">JSON representation</span></span>

<span data-ttu-id="873d9-188">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="873d9-188">The following is a JSON representation of the resource.</span></span>

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


