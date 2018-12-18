---
title: 获取用户和资源的忙/闲日程安排（预览版）
description: 在工作或学校设置中，一种常见方案是查看用户何时有空参加会议，或浏览团队、会议室或设备在一段时间内的状态。
author: angelgolfer-ms
ms.openlocfilehash: 2f201ed552200f7c8dd55b368a504b4eca1e3ba5
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27317757"
---
# <a name="get-freebusy-schedule-of-users-and-resources-preview"></a><span data-ttu-id="5d87f-103">获取用户和资源的忙/闲日程安排（预览版）</span><span class="sxs-lookup"><span data-stu-id="5d87f-103">Get free/busy schedule of users and resources (preview)</span></span>

<span data-ttu-id="5d87f-104">在工作或学校设置中，一种常见方案是查看用户何时有空参加会议，或浏览团队、会议室或设备在一段时间内的状态。</span><span class="sxs-lookup"><span data-stu-id="5d87f-104">In a work or school setting, a common scenario is to see when a user is free for meeting, or to browse the availability of a team, room, or equipment for a time period.</span></span>

<span data-ttu-id="5d87f-105">使用 [getSchedule](/graph/api/calendar-getschedule?view=graph-rest-beta) 操作，可以获取一个或多个实体（用户、通讯组列表或资源）在特定时间段内的状态信息。</span><span class="sxs-lookup"><span data-stu-id="5d87f-105">The [getSchedule](/graph/api/calendar-getschedule?view=graph-rest-beta) action lets you get the availability information of one or more entities - users, distribution lists, or resources - for a specific period of time.</span></span> 

## <a name="example"></a><span data-ttu-id="5d87f-106">示例</span><span class="sxs-lookup"><span data-stu-id="5d87f-106">Example</span></span>

<span data-ttu-id="5d87f-107">下面的简单示例展示了如何查找同事 Alex 在某天上午 9 点到下午 6 点（太平洋标准时间）之间的忙/闲日程安排：</span><span class="sxs-lookup"><span data-stu-id="5d87f-107">A simple example is to find the free/busy schedule of a coworker, Alex, on a specific day, from 9am to 6pm, Pacitfic Standard Time:</span></span>

<!-- {
  "blockType": "ignored",
  "name": "calendar_getSchedule_concept"
}-->
```http
POST https://graph.microsoft.com/beta/me/calendar/getschedule 
Prefer: outlook.timezone="Pacific Standard Time"
Content-Type: application/json

{        
    "Schedules": ["AlexW@contoso.OnMicrosoft.com"],
    "StartTime": {
        "dateTime": "2018-08-06T09:00:00",
        "timeZone": "Pacific Standard Time"
    },
    "EndTime": {
        "dateTime": "2018-08-06T18:00:00",
        "timeZone": "Pacific Standard Time"
    },
    "availabilityViewInterval": "15"
}
```

<span data-ttu-id="5d87f-108">**getSchedule** 返回两个与 Alex 默认日历中现有事件匹配的日程安排项，同时显示每个事件的开始时间和结束时间及其忙/闲状态。</span><span class="sxs-lookup"><span data-stu-id="5d87f-108">**getSchedule** returns two schedule items that match existing events in Alex' default calendar, showing the start and end times of each event and its free/busy status.</span></span> <span data-ttu-id="5d87f-109">可以假定 Alex 在此日期/时间范围的剩余时间内是空闲的。</span><span class="sxs-lookup"><span data-stu-id="5d87f-109">You can assume Alex is free for the remaining time in that date/time range.</span></span>

<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.scheduleInformation",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context":"https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.scheduleInformation)",
    "value":[
        {
            "scheduleId":"AlexW@contoso.OnMicrosoft.com",
            "availabilityView":"111111002222222200000000000000000000",
            "scheduleItems":[
                {
                    "isPrivate":false,
                    "status":"Tentative",
                    "start":{
                        "dateTime":"2018-08-06T09:00:00.0000000",
                        "timeZone":"Pacific Standard Time"
                    },
                    "end":{
                        "dateTime":"2018-08-06T10:30:00.0000000",
                        "timeZone":"Pacific Standard Time"
                    }
                },
                {
                    "isPrivate":false,
                    "status":"Busy",
                    "start":{
                        "dateTime":"2018-08-06T11:00:00.0000000",
                        "timeZone":"Pacific Standard Time"
                    },
                    "end":{
                        "dateTime":"2018-08-06T13:00:00.0000000",
                        "timeZone":"Pacific Standard Time"
                    }
                }
            ],
            "workingHours":{
                "daysOfWeek":[
                    "monday",
                    "tuesday",
                    "wednesday",
                    "thursday",
                    "friday"
                ],
                "startTime":"08:00:00.0000000",
                "endTime":"17:00:00.0000000",
                "timeZone":{
                    "@odata.type":"#microsoft.graph.customTimeZone",
                    "bias":480,
                    "name":"Customized Time Zone",
                    "standardOffset":{
                        "time":"02:00:00.0000000",
                        "dayOccurrence":1,
                        "dayOfWeek":"sunday",
                        "month":11,
                        "year":0
                    },
                    "daylightOffset":{
                        "daylightBias":-60,
                        "time":"02:00:00.0000000",
                        "dayOccurrence":2,
                        "dayOfWeek":"sunday",
                        "month":3,
                        "year":0
                    }
                }
            }
        }
    ]
}

```

<span data-ttu-id="5d87f-110">除了 Alex 的忙/闲日程安排和工作时间之外，**getSchedule** 还返回 **availabilityView**，这是 Alex 这一天状态的合并视图。</span><span class="sxs-lookup"><span data-stu-id="5d87f-110">Apart from the free/busy schedule and working hours of Alex, **getSchedule** also returns **availabilityView**, which is a merged view of Alex' availability for that day.</span></span> <span data-ttu-id="5d87f-111">此合并视图是一个字符串，其中包含这一天的所有时间段，每个时间段都使用以下约定指明 Alex 的状态：</span><span class="sxs-lookup"><span data-stu-id="5d87f-111">The merged view is a string that consists of time slots covering that day, with each time slot indicating Alex' availability using the following convention:</span></span> 

- <span data-ttu-id="5d87f-112">`0`= 空闲</span><span class="sxs-lookup"><span data-stu-id="5d87f-112">`0`= free</span></span>
- <span data-ttu-id="5d87f-113">`1`= 暂定</span><span class="sxs-lookup"><span data-stu-id="5d87f-113">`1`= tentative</span></span>
- <span data-ttu-id="5d87f-114">`2`= 忙碌</span><span class="sxs-lookup"><span data-stu-id="5d87f-114">`2`= busy</span></span>
- <span data-ttu-id="5d87f-115">`3`= 外出</span><span class="sxs-lookup"><span data-stu-id="5d87f-115">`3`= out of office</span></span>
- <span data-ttu-id="5d87f-116">`4`= 在其他地方工作。</span><span class="sxs-lookup"><span data-stu-id="5d87f-116">`4`= working elsewhere.</span></span> 

<span data-ttu-id="5d87f-117">默认情况下，每个时间段的长度为 30 分钟。</span><span class="sxs-lookup"><span data-stu-id="5d87f-117">By default, the length of each time slot is 30 minutes.</span></span> <span data-ttu-id="5d87f-118">此示例使用 **availabilityViewInterval** 属性，将时间段自定义为 15 分钟。</span><span class="sxs-lookup"><span data-stu-id="5d87f-118">This example uses the **availabilityViewInterval** property to customize the time slot to be 15 minutes.</span></span>

## <a name="how-is-getschedule-different-from-findmeetingtimes"></a><span data-ttu-id="5d87f-119">getSchedule 与 findMeetingTimes 有何区别</span><span class="sxs-lookup"><span data-stu-id="5d87f-119">How is getSchedule different from findMeetingTimes</span></span>

<span data-ttu-id="5d87f-120">[findMeetingTimes](/graph/api/user-findmeetingtimes?view=graph-rest-1.0) 操作与 **getSchedule** 类似，两者都读取指定用户和资源的忙/闲状态和工作时间。</span><span class="sxs-lookup"><span data-stu-id="5d87f-120">The [findMeetingTimes](/graph/api/user-findmeetingtimes?view=graph-rest-1.0) action is similar to **getSchedule** in that both read the free/busy status and working hours of specified users and resources.</span></span> <span data-ttu-id="5d87f-121">这两项操作的区别主要在以下几方面。</span><span class="sxs-lookup"><span data-stu-id="5d87f-121">The two actions differ in a few major ways.</span></span>

### <a name="application"></a><span data-ttu-id="5d87f-122">用途</span><span class="sxs-lookup"><span data-stu-id="5d87f-122">Application</span></span>

<span data-ttu-id="5d87f-123">**findMeetingTimes** 应用特定业务逻辑来建议会议时间和地点，如：</span><span class="sxs-lookup"><span data-stu-id="5d87f-123">**findMeetingTimes** applies certain business logic to suggest meeting times and locations, such as:</span></span>

- <span data-ttu-id="5d87f-124">每个实体是自愿与会还是必须与会</span><span class="sxs-lookup"><span data-stu-id="5d87f-124">Optional or mandatory attendance of each entity</span></span>
- <span data-ttu-id="5d87f-125">一天内请求执行的活动的性质</span><span class="sxs-lookup"><span data-stu-id="5d87f-125">The nature of the requested activity for the time of the day</span></span>
- <span data-ttu-id="5d87f-126">会议仲裁要求的最少与会人数</span><span class="sxs-lookup"><span data-stu-id="5d87f-126">The minimum attendance required for a quorum for a meeting</span></span>

<span data-ttu-id="5d87f-127">它适用于依赖[简化约会预订](findmeetingtimes-example.md)的方案。</span><span class="sxs-lookup"><span data-stu-id="5d87f-127">It is appropriate for scenarios that depend on [streamlining appointment booking](findmeetingtimes-example.md).</span></span>

<span data-ttu-id="5d87f-128">**getSchedule** 只返回每个所需日历中现有事件在给定时间段内的忙/闲状态，并假定在此时间段的剩余时间内是空闲的。</span><span class="sxs-lookup"><span data-stu-id="5d87f-128">**getSchedule** simply returns the free/busy status of existing events in each of the requested calendars for a given time period, and assumes the remaining time in that time period tp be free.</span></span> <span data-ttu-id="5d87f-129">然后，应用其他业务逻辑来利用此类数据完成方案。</span><span class="sxs-lookup"><span data-stu-id="5d87f-129">You would then apply further business logic to make use of this data to complete your scenario.</span></span>

### <a name="app-only-support"></a><span data-ttu-id="5d87f-130">仅应用支持</span><span class="sxs-lookup"><span data-stu-id="5d87f-130">App-only support</span></span>

<span data-ttu-id="5d87f-131">**findmeetingtimes** 仅支持要求用户必须已登录应用的委托方案。</span><span class="sxs-lookup"><span data-stu-id="5d87f-131">**findmeetingtimes** supports only delegated scenarios which require a user to have signed in to the app.</span></span> <span data-ttu-id="5d87f-132">应用只能读取已登录用户可以访问的日历中的事件。</span><span class="sxs-lookup"><span data-stu-id="5d87f-132">The app can read events in only the calendars that the signed-in user can access.</span></span> <span data-ttu-id="5d87f-133">这可以包括其他用户已委托或已与登录用户共享的日历。</span><span class="sxs-lookup"><span data-stu-id="5d87f-133">This can include calendars that other users have delegated or shared with the signed-in user.</span></span>

<span data-ttu-id="5d87f-134">**getSchedule** 支持委托方案和仅应用方案。</span><span class="sxs-lookup"><span data-stu-id="5d87f-134">**getSchedule** supports both delegated and app-only scenarios.</span></span> <span data-ttu-id="5d87f-135">对于后者，管理员同意应用访问所有日历，即使没有已登录用户，也不例外。</span><span class="sxs-lookup"><span data-stu-id="5d87f-135">In the latter, an administrator consents the app to access all calendars without a signed-in user.</span></span>


### <a name="version-support"></a><span data-ttu-id="5d87f-136">版本支持</span><span class="sxs-lookup"><span data-stu-id="5d87f-136">Version support</span></span>

<span data-ttu-id="5d87f-137">**findmeetingtimes** 一般适用于所有应用。</span><span class="sxs-lookup"><span data-stu-id="5d87f-137">**findmeetingtimes** is generally available for all apps.</span></span> 

<span data-ttu-id="5d87f-138">**getSchedule** 暂处于[预览状态](versioning-and-support.md#beta-version)，因此不适用于生产应用。</span><span class="sxs-lookup"><span data-stu-id="5d87f-138">**getSchedule** is currently available [in preview status](versioning-and-support.md#beta-version), and therefore is not appropriate for use in production apps.</span></span>


## <a name="permissions"></a><span data-ttu-id="5d87f-139">权限</span><span class="sxs-lookup"><span data-stu-id="5d87f-139">Permissions</span></span>
<span data-ttu-id="5d87f-140">获取忙/闲信息所需的最低权限是 Calendar.Read。</span><span class="sxs-lookup"><span data-stu-id="5d87f-140">The least privileged permission you need to get free/busy information is Calendar.Read.</span></span> <span data-ttu-id="5d87f-141">根据应用方案，这可由已登录用户或管理员同意授予。</span><span class="sxs-lookup"><span data-stu-id="5d87f-141">Depending on your app scenario, this can be consented by the signed-in user or administrator.</span></span>
<span data-ttu-id="5d87f-142">除了所需实体的忙/闲状态和工作时间外，**getSchedule** 还可以返回事件的主题和地点，前提是：</span><span class="sxs-lookup"><span data-stu-id="5d87f-142">Other than the free/busy status and working hours of requested entities, **getSchedule** can also return the subject and location of an event, provided that:</span></span>

- <span data-ttu-id="5d87f-143">如果事件被标记为低敏感度级别（`normal` 或 `personal`），且符合以下一个或多个条件：</span><span class="sxs-lookup"><span data-stu-id="5d87f-143">If the event is marked with low sensitivity level - `normal` or `personal` AND one or more of the following conditions applies:</span></span>

- <span data-ttu-id="5d87f-144">所需用户的日历设置允许组织中的全部用户查看标题和地点</span><span class="sxs-lookup"><span data-stu-id="5d87f-144">The requested user’s calendar settings allow all the users in the organization to view titles and locations</span></span>
- <span data-ttu-id="5d87f-145">所需用户的日历与已登录用户共享</span><span class="sxs-lookup"><span data-stu-id="5d87f-145">The requested user’s calendar is shared with the signed-in user</span></span>
- <span data-ttu-id="5d87f-146">已登录用户是所需用户所在组织的管理员。</span><span class="sxs-lookup"><span data-stu-id="5d87f-146">The signed-in user is an administrator of the same organization as the requested user.</span></span>

## <a name="time-zone-representation"></a><span data-ttu-id="5d87f-147">时区表示</span><span class="sxs-lookup"><span data-stu-id="5d87f-147">Time zone representation</span></span>
<span data-ttu-id="5d87f-148">默认情况下，返回的日程安排项的开始时间和结束时间都采用 UTC。</span><span class="sxs-lookup"><span data-stu-id="5d87f-148">By default, the start and end times of the returned schedule items are represented in UTC.</span></span> <span data-ttu-id="5d87f-149">可使用 `Prefer` 头指定适合应用的时区。</span><span class="sxs-lookup"><span data-stu-id="5d87f-149">You can use a `Prefer` header to specify a time zone appropriate for your app.</span></span> <span data-ttu-id="5d87f-150">例如：</span><span class="sxs-lookup"><span data-stu-id="5d87f-150">As an example:</span></span> 
```
Prefer: outlook.timezone="Pacific Standard Time"
```

## <a name="limits-and-error-conditions"></a><span data-ttu-id="5d87f-151">限制和错误条件</span><span class="sxs-lookup"><span data-stu-id="5d87f-151">Limits and error conditions</span></span>
<span data-ttu-id="5d87f-152">请注意以下限制和错误条件：</span><span class="sxs-lookup"><span data-stu-id="5d87f-152">Be aware of the following limits and error condition:</span></span>

- <span data-ttu-id="5d87f-153">**getSchedule** 支持一次查找最多 20 个实体的忙/闲信息。</span><span class="sxs-lookup"><span data-stu-id="5d87f-153">**getSchedule** can support looking up free/busy information for up to 20 entities at once.</span></span> <span data-ttu-id="5d87f-154">标识为个人的用户数或标识为通讯组列表成员的用户数以及资源数都计入此限制。</span><span class="sxs-lookup"><span data-stu-id="5d87f-154">This limit applies to the number of users identified individually or as members of a distribution list, and to the number of resources as well.</span></span>
- <span data-ttu-id="5d87f-155">查找时间段不得长于 42 天。</span><span class="sxs-lookup"><span data-stu-id="5d87f-155">The time period to look up must be less than 42 days.</span></span>
- <span data-ttu-id="5d87f-156">如果 **getSchedule** 无法识别指定用户或资源，便会返回一个日程安排项并指明错误。</span><span class="sxs-lookup"><span data-stu-id="5d87f-156">If **getSchedule** cannot identify a specified user or resource, it returns a single schedule item and indicates the error.</span></span> 

## <a name="see-also"></a><span data-ttu-id="5d87f-157">另请参阅</span><span class="sxs-lookup"><span data-stu-id="5d87f-157">See also</span></span>
- [<span data-ttu-id="5d87f-158">权限参考</span><span class="sxs-lookup"><span data-stu-id="5d87f-158">Permissions reference</span></span>](permissions-reference.md#calendars-permissions)
- [<span data-ttu-id="5d87f-159">在 Outlook 日历上查找可能的会议时间</span><span class="sxs-lookup"><span data-stu-id="5d87f-159">Find possible meeting times on the Outlook calendar</span></span>](findmeetingtimes-example.md)
