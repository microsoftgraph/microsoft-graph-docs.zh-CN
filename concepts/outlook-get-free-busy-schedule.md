---
title: 获取用户和资源的忙/闲日程安排
description: 在工作或学校设置中，一种常见方案是查看用户何时有空参加会议，或浏览团队、会议室或设备在一段时间内的状态。
author: tariq-sharif
localization_priority: Priority
ms.prod: outlook
ms.openlocfilehash: d3d8379f05d6e19505bdf3c45cca0863a685423d
ms.sourcegitcommit: ada6eab637b9b318129aefb98edbe7316399d9ba
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/07/2021
ms.locfileid: "53317129"
---
# <a name="get-freebusy-schedule-of-users-and-resources"></a><span data-ttu-id="82ad1-103">获取用户和资源的忙/闲日程安排</span><span class="sxs-lookup"><span data-stu-id="82ad1-103">Get free/busy schedule of users and resources</span></span>

<span data-ttu-id="82ad1-104">在工作或学校设置中，一种常见方案是查看用户何时有空参加会议，或浏览团队、会议室或设备在一段时间内的状态。</span><span class="sxs-lookup"><span data-stu-id="82ad1-104">In a work or school setting, a common scenario is to see when a user is free for meeting, or to browse the availability of a team, room, or equipment for a time period.</span></span>

<span data-ttu-id="82ad1-105">使用 [getSchedule](/graph/api/calendar-getschedule?view=graph-rest-1.0) 操作，可以获取一个或多个实体（用户、通讯组列表或资源）在特定时间段内的状态信息。</span><span class="sxs-lookup"><span data-stu-id="82ad1-105">The [getSchedule](/graph/api/calendar-getschedule?view=graph-rest-1.0) action lets you get the availability information of one or more entities - users, distribution lists, or resources - for a specific period of time.</span></span> 

## <a name="example"></a><span data-ttu-id="82ad1-106">示例</span><span class="sxs-lookup"><span data-stu-id="82ad1-106">Example</span></span>

<span data-ttu-id="82ad1-107">下面的简单示例展示了如何查找同事 Alex 在某天上午 9 点到下午 6 点（太平洋标准时间）之间的忙/闲日程安排：</span><span class="sxs-lookup"><span data-stu-id="82ad1-107">A simple example is to find the free/busy schedule of a coworker, Alex, on a specific day, from 9am to 6pm, Pacific Standard Time:</span></span>

<!-- {
  "blockType": "ignored",
  "name": "calendar_getSchedule_concept"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/calendar/getschedule 
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

<span data-ttu-id="82ad1-108">**getSchedule** 返回两个与 Alex 默认日历中现有事件匹配的日程安排项，同时显示每个事件的开始时间和结束时间及其忙/闲状态。</span><span class="sxs-lookup"><span data-stu-id="82ad1-108">**getSchedule** returns two schedule items that match existing events in Alex' default calendar, showing the start and end times of each event and its free/busy status.</span></span> <span data-ttu-id="82ad1-109">可以假定 Alex 在此日期/时间范围的剩余时间内是空闲的。</span><span class="sxs-lookup"><span data-stu-id="82ad1-109">You can assume Alex is free for the remaining time in that date/time range.</span></span>

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
    "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#Collection(microsoft.graph.scheduleInformation)",
    "value":[
        {
            "scheduleId":"AlexW@contoso.OnMicrosoft.com",
            "availabilityView":"111111002222222200000000000000000000",
            "scheduleItems":[
                {
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

<span data-ttu-id="82ad1-110">除了 Alex 的忙/闲日程安排和工作时间之外，**getSchedule** 还返回 **availabilityView**，这是 Alex 这一天状态的合并视图。</span><span class="sxs-lookup"><span data-stu-id="82ad1-110">Apart from the free/busy schedule and working hours of Alex, **getSchedule** also returns **availabilityView**, which is a merged view of Alex' availability for that day.</span></span> <span data-ttu-id="82ad1-111">此合并视图是一个字符串，其中包含这一天的所有时间段，每个时间段都使用以下约定指明 Alex 的状态：</span><span class="sxs-lookup"><span data-stu-id="82ad1-111">The merged view is a string that consists of time slots covering that day, with each time slot indicating Alex' availability using the following convention:</span></span> 

- <span data-ttu-id="82ad1-112">`0`= 空闲</span><span class="sxs-lookup"><span data-stu-id="82ad1-112">`0`= free</span></span>
- <span data-ttu-id="82ad1-113">`1`= 暂定</span><span class="sxs-lookup"><span data-stu-id="82ad1-113">`1`= tentative</span></span>
- <span data-ttu-id="82ad1-114">`2`= 忙碌</span><span class="sxs-lookup"><span data-stu-id="82ad1-114">`2`= busy</span></span>
- <span data-ttu-id="82ad1-115">`3`= 外出</span><span class="sxs-lookup"><span data-stu-id="82ad1-115">`3`= out of office</span></span>
- <span data-ttu-id="82ad1-116">`4`= 在其他地方工作。</span><span class="sxs-lookup"><span data-stu-id="82ad1-116">`4`= working elsewhere.</span></span> 

<span data-ttu-id="82ad1-117">默认情况下，每个时间段的长度为 30 分钟。</span><span class="sxs-lookup"><span data-stu-id="82ad1-117">By default, the length of each time slot is 30 minutes.</span></span> <span data-ttu-id="82ad1-118">此示例使用 **availabilityViewInterval** 属性，将时间段自定义为 15 分钟。</span><span class="sxs-lookup"><span data-stu-id="82ad1-118">This example uses the **availabilityViewInterval** property to customize the time slot to be 15 minutes.</span></span>

## <a name="how-does-getschedule-compare-with-findmeetingtimes"></a><span data-ttu-id="82ad1-119">getSchedule 如何与 findMeetingTimes 进行比较</span><span class="sxs-lookup"><span data-stu-id="82ad1-119">How does getSchedule compare with findMeetingTimes</span></span>

<span data-ttu-id="82ad1-120">[findMeetingTimes](/graph/api/user-findmeetingtimes?view=graph-rest-1.0) 操作与 **getSchedule** 类似，两者都读取指定用户和资源的忙/闲状态和工作时间。</span><span class="sxs-lookup"><span data-stu-id="82ad1-120">The [findMeetingTimes](/graph/api/user-findmeetingtimes?view=graph-rest-1.0) action is similar to **getSchedule** in that both read the free/busy status and working hours of specified users and resources.</span></span> <span data-ttu-id="82ad1-121">这两项操作的区别主要在以下几方面。</span><span class="sxs-lookup"><span data-stu-id="82ad1-121">The two actions differ in a few major ways.</span></span>

### <a name="application"></a><span data-ttu-id="82ad1-122">用途</span><span class="sxs-lookup"><span data-stu-id="82ad1-122">Application</span></span>

<span data-ttu-id="82ad1-123">**findMeetingTimes** 应用特定业务逻辑来建议会议时间和地点，如：</span><span class="sxs-lookup"><span data-stu-id="82ad1-123">**findMeetingTimes** applies certain business logic to suggest meeting times and locations, such as:</span></span>

- <span data-ttu-id="82ad1-124">每个实体是自愿与会还是必须与会</span><span class="sxs-lookup"><span data-stu-id="82ad1-124">Optional or mandatory attendance of each entity</span></span>
- <span data-ttu-id="82ad1-125">一天内请求执行的活动的性质</span><span class="sxs-lookup"><span data-stu-id="82ad1-125">The nature of the requested activity for the time of the day</span></span>
- <span data-ttu-id="82ad1-126">会议仲裁要求的最少与会人数</span><span class="sxs-lookup"><span data-stu-id="82ad1-126">The minimum attendance required for a quorum for a meeting</span></span>

<span data-ttu-id="82ad1-127">它适用于依赖[简化约会预订](findmeetingtimes-example.md)的方案。</span><span class="sxs-lookup"><span data-stu-id="82ad1-127">It is appropriate for scenarios that depend on [streamlining appointment booking](findmeetingtimes-example.md).</span></span>

<span data-ttu-id="82ad1-128">**getSchedule** 只返回每个所需日历中现有事件在给定时间段内的忙/闲状态，并假定在此时间段的剩余时间内是空闲的。</span><span class="sxs-lookup"><span data-stu-id="82ad1-128">**getSchedule** simply returns the free/busy status of existing events in each of the requested calendars for a given time period, and assumes the remaining time in that time period to be free.</span></span> <span data-ttu-id="82ad1-129">然后，应用其他业务逻辑来利用此类数据完成方案。</span><span class="sxs-lookup"><span data-stu-id="82ad1-129">You would then apply further business logic to make use of this data to complete your scenario.</span></span>

### <a name="app-only-support"></a><span data-ttu-id="82ad1-130">仅应用支持</span><span class="sxs-lookup"><span data-stu-id="82ad1-130">App-only support</span></span>

<span data-ttu-id="82ad1-131">**findmeetingtimes** 仅支持要求用户必须已登录应用的委托方案。</span><span class="sxs-lookup"><span data-stu-id="82ad1-131">**findmeetingtimes** supports only delegated scenarios which require a user to have signed in to the app.</span></span> <span data-ttu-id="82ad1-132">应用只能读取已登录用户可以访问的日历中的事件。</span><span class="sxs-lookup"><span data-stu-id="82ad1-132">The app can read events in only the calendars that the signed-in user can access.</span></span> <span data-ttu-id="82ad1-133">这可以包括其他用户已委托或已与登录用户共享的日历。</span><span class="sxs-lookup"><span data-stu-id="82ad1-133">This can include calendars that other users have delegated or shared with the signed-in user.</span></span>

<span data-ttu-id="82ad1-134">**getSchedule** 支持委托方案和仅应用方案。</span><span class="sxs-lookup"><span data-stu-id="82ad1-134">**getSchedule** supports both delegated and app-only scenarios.</span></span> <span data-ttu-id="82ad1-135">对于后者，管理员同意应用访问所有日历，即使没有已登录用户，也不例外。</span><span class="sxs-lookup"><span data-stu-id="82ad1-135">In the latter, an administrator consents the app to access all calendars without a signed-in user.</span></span>

### <a name="permissions"></a><span data-ttu-id="82ad1-136">权限</span><span class="sxs-lookup"><span data-stu-id="82ad1-136">Permissions</span></span>
<span data-ttu-id="82ad1-137">**findmeetingtimes** 所需的最低特权权限为 Calendars.Read.Shared。</span><span class="sxs-lookup"><span data-stu-id="82ad1-137">The least privileged permissions required by **findmeetingtimes** is Calendars.Read.Shared.</span></span>

<span data-ttu-id="82ad1-138">**getSchedule** 所需的最低特权权限为 Calendars.Read。</span><span class="sxs-lookup"><span data-stu-id="82ad1-138">The least privileged permission required by **getSchedule** is Calendars.Read.</span></span> 

### <a name="version-support"></a><span data-ttu-id="82ad1-139">版本支持</span><span class="sxs-lookup"><span data-stu-id="82ad1-139">Version support</span></span>

<span data-ttu-id="82ad1-140">**findmeetingtimes** 和 **getSchedule** 均已正式发布且适用于生产应用。</span><span class="sxs-lookup"><span data-stu-id="82ad1-140">**findmeetingtimes** and **getSchedule** are both generally available and appropriate for use in production apps.</span></span>


## <a name="event-data-returned"></a><span data-ttu-id="82ad1-141">返回的事件数据</span><span class="sxs-lookup"><span data-stu-id="82ad1-141">Event data returned</span></span>
<span data-ttu-id="82ad1-142">要使应用能够获取忙/闲信息，**getSchedule** 所需的最低特权权限为 Calendars.Read。</span><span class="sxs-lookup"><span data-stu-id="82ad1-142">The least privileged permission required by **getSchedule** for an app to get free/busy information is Calendars.Read.</span></span> <span data-ttu-id="82ad1-143">根据应用方案，这可由已登录用户或管理员同意授予。</span><span class="sxs-lookup"><span data-stu-id="82ad1-143">Depending on your app scenario, this can be consented by the signed-in user or administrator.</span></span>

<span data-ttu-id="82ad1-144">虽然借助同意后授予的权限，应用可通过 Outlook 在所请求用户的日历上使用 **getSchedule** 但所请求的用户可控制该 **getSchedule** 返回的事件数据（若有）。</span><span class="sxs-lookup"><span data-stu-id="82ad1-144">While the consented permission lets an app use **getSchedule** on the requested users' calendars, through Outlook, the requested user controls which event data, if any, that **getSchedule** returns.</span></span> 

<span data-ttu-id="82ad1-145">例如，**getSchedule** 可返回所请求用户的忙/闲状态和工作时间，还能返回事件的 **subject**、**location** 和 **isPrivate**，但前提是：</span><span class="sxs-lookup"><span data-stu-id="82ad1-145">For example, **getSchedule** can return the free/busy status and working hours of the requested users, or it can also return the **subject**, **location**, and **isPrivate** properties of an event, provided that:</span></span>

- <span data-ttu-id="82ad1-146">事件被标记为低敏感度级别（`normal` 或 `personal`），且符合以下一个或多个条件：</span><span class="sxs-lookup"><span data-stu-id="82ad1-146">The event is marked with low sensitivity level - `normal` or `personal` - AND one or more of the following conditions apply:</span></span>

  - <span data-ttu-id="82ad1-147">所请求的用户的日历设置允许用户登录后查看主题行和位置</span><span class="sxs-lookup"><span data-stu-id="82ad1-147">The requested user’s calendar settings allow the signed-in user to view subject lines and locations</span></span>
  - <span data-ttu-id="82ad1-148">所请求的用户的日历与已登录用户共享</span><span class="sxs-lookup"><span data-stu-id="82ad1-148">The requested user’s calendar is shared with the signed-in user</span></span>

<span data-ttu-id="82ad1-149">无论已登录用户是否是组织中的管理员，都需遵循这些条件。</span><span class="sxs-lookup"><span data-stu-id="82ad1-149">These conditions apply regardless of whether the signed-in user is an administrator in the organization.</span></span> <span data-ttu-id="82ad1-150">所请求的用户可控制返回的事件数据。</span><span class="sxs-lookup"><span data-stu-id="82ad1-150">The requested user has control over the event data returned.</span></span>

## <a name="time-zone-representation"></a><span data-ttu-id="82ad1-151">时区表示</span><span class="sxs-lookup"><span data-stu-id="82ad1-151">Time zone representation</span></span>
<span data-ttu-id="82ad1-152">默认情况下，返回的日程安排项的开始时间和结束时间都采用 UTC。</span><span class="sxs-lookup"><span data-stu-id="82ad1-152">By default, the start and end times of the returned schedule items are represented in UTC.</span></span> <span data-ttu-id="82ad1-153">可使用 `Prefer` 头指定适合应用的时区。</span><span class="sxs-lookup"><span data-stu-id="82ad1-153">You can use a `Prefer` header to specify a time zone appropriate for your app.</span></span> <span data-ttu-id="82ad1-154">例如：</span><span class="sxs-lookup"><span data-stu-id="82ad1-154">As an example:</span></span> 
``` http
Prefer: outlook.timezone="Pacific Standard Time"
```

## <a name="limits-and-error-conditions"></a><span data-ttu-id="82ad1-155">限制和错误条件</span><span class="sxs-lookup"><span data-stu-id="82ad1-155">Limits and error conditions</span></span>
<span data-ttu-id="82ad1-156">请注意以下限制和错误条件：</span><span class="sxs-lookup"><span data-stu-id="82ad1-156">Be aware of the following limits and error condition:</span></span>

- <span data-ttu-id="82ad1-157">**getSchedule** 支持一次查找最多 20 个实体的忙/闲信息。</span><span class="sxs-lookup"><span data-stu-id="82ad1-157">**getSchedule** can support looking up free/busy information for up to 20 entities at once.</span></span> <span data-ttu-id="82ad1-158">标识为个人的用户数或标识为通讯组列表成员的用户数以及资源数都计入此限制。</span><span class="sxs-lookup"><span data-stu-id="82ad1-158">This limit applies to the number of users identified individually or as members of a distribution list, and to the number of resources as well.</span></span>
- <span data-ttu-id="82ad1-159">查找时间段不得长于 42 天。</span><span class="sxs-lookup"><span data-stu-id="82ad1-159">The time period to look up must be less than 42 days.</span></span>
- <span data-ttu-id="82ad1-160">如果 **getSchedule** 无法识别指定用户或资源，便会返回一个日程安排项并指明错误。</span><span class="sxs-lookup"><span data-stu-id="82ad1-160">If **getSchedule** cannot identify a specified user or resource, it returns a single schedule item and indicates the error.</span></span> 


## <a name="see-also"></a><span data-ttu-id="82ad1-161">另请参阅</span><span class="sxs-lookup"><span data-stu-id="82ad1-161">See also</span></span>
- [<span data-ttu-id="82ad1-162">权限参考</span><span class="sxs-lookup"><span data-stu-id="82ad1-162">Permissions reference</span></span>](permissions-reference.md#calendars-permissions)
- [<span data-ttu-id="82ad1-163">在 Outlook 日历上查找可能的会议时间</span><span class="sxs-lookup"><span data-stu-id="82ad1-163">Find possible meeting times on the Outlook calendar</span></span>](findmeetingtimes-example.md)
