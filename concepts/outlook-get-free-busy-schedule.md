# <a name="get-freebusy-schedule-for-users-and-resources-preview"></a><span data-ttu-id="eb5cd-101">获取用户和资源的闲 / 忙计划（预览）</span><span class="sxs-lookup"><span data-stu-id="eb5cd-101">Get free/busy schedule for users and resources (preview)</span></span>

<span data-ttu-id="eb5cd-102">在工作或学校设置中，一个常见的应用方案是查看用户什么时候有时间参加会议，或者浏览某一团队、会议室或设备在一特定时段是否有时间以及是否可用。</span><span class="sxs-lookup"><span data-stu-id="eb5cd-102">In a work or school setting, a common scenario is to see when a user is free for meeting, or to browse the availability of a team, room, or equipment for a time period.</span></span>

<span data-ttu-id="eb5cd-103"> [GetSchedule](../api-reference/beta/api/calendar_getschedule.md) 操作可以获取某一特定时段内诸如用户、通讯组列表或资源等一个或多个实体的可用性信息。</span><span class="sxs-lookup"><span data-stu-id="eb5cd-103">The [getSchedule](../api-reference/beta/api/calendar_getschedule.md) action lets you get the availability information of one or more entities - users, distribution lists, or resources - for a specific period of time.</span></span> 

## <a name="example"></a><span data-ttu-id="eb5cd-104">示例</span><span class="sxs-lookup"><span data-stu-id="eb5cd-104">Example</span></span>

<span data-ttu-id="eb5cd-105">一个简单的示例是查看同事 Alex 在某一天自上午九点至下午六点（太平洋标准时间）的闲 / 忙计划。</span><span class="sxs-lookup"><span data-stu-id="eb5cd-105">A simple example is to find the free/busy schedule of a coworker, Alex, on a specific day, from 9am to 6pm, Pacitfic Standard Time:</span></span>

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

<span data-ttu-id="eb5cd-106">**getSchedule** 返回两个与 Alex 默认日历现有事件相匹配的计划项，显示的每个事件的开始和结束时间以及事件的闲 / 忙状态。</span><span class="sxs-lookup"><span data-stu-id="eb5cd-106">**getSchedule** returns two schedule items that match existing events in Alex' default calendar, showing the start and end times of each event and its free/busy status.</span></span> <span data-ttu-id="eb5cd-107">可以假定在该日期 / 时间范围内的剩余时间 Alex 是有空的。</span><span class="sxs-lookup"><span data-stu-id="eb5cd-107">You can assume Alex is free for the remaining time in that date/time range.</span></span>

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

<span data-ttu-id="eb5cd-108">除了 Alex 的闲 / 忙计划和工作时间外， **getSchedule** 也会返回 **availabilityView**，即 Alex 在该天有时间的合并视图。</span><span class="sxs-lookup"><span data-stu-id="eb5cd-108">Apart from the free/busy schedule and working hours of Alex, **getSchedule** also returns **availabilityView**, which is a merged view of Alex' availability for that day.</span></span> <span data-ttu-id="eb5cd-109">合并视图是一个字符串，由覆盖那一天的时间段构成，每个时间段使用以下约定指示 Alex 是否有空：</span><span class="sxs-lookup"><span data-stu-id="eb5cd-109">The merged view is a string that consists of time slots covering that day, with each time slot indicating Alex' availability using the following convention:</span></span> 

- <span data-ttu-id="eb5cd-110">`0`= 空闲</span><span class="sxs-lookup"><span data-stu-id="eb5cd-110">`0`= free</span></span>
- <span data-ttu-id="eb5cd-111">`1`= 暂定</span><span class="sxs-lookup"><span data-stu-id="eb5cd-111">`1`= tentative</span></span>
- <span data-ttu-id="eb5cd-112">`2`= 忙碌</span><span class="sxs-lookup"><span data-stu-id="eb5cd-112">`2`= busy</span></span>
- <span data-ttu-id="eb5cd-113">`3`= 不在办公室</span><span class="sxs-lookup"><span data-stu-id="eb5cd-113">`3`= out of office</span></span>
- <span data-ttu-id="eb5cd-114">`4`= 在其他位置工作。</span><span class="sxs-lookup"><span data-stu-id="eb5cd-114">`4`= working elsewhere.</span></span> 

<span data-ttu-id="eb5cd-115">默认方式，每个时间段的长度为 30 分钟。</span><span class="sxs-lookup"><span data-stu-id="eb5cd-115">Specifies the length of each time slot in minutes. Default is 30 minutes.</span></span> <span data-ttu-id="eb5cd-116">本示例使用 **availabilityViewInterval** 属性将时间段自定义为 15 分钟。</span><span class="sxs-lookup"><span data-stu-id="eb5cd-116">This example uses the **availabilityViewInterval** property to customize the time slot to be 15 minutes.</span></span>

## <a name="how-is-getschedule-different-from-findmeetingtimes"></a><span data-ttu-id="eb5cd-117">getSchedule 与 findMeetingTimes 有何不同</span><span class="sxs-lookup"><span data-stu-id="eb5cd-117">How is getSchedule different from findMeetingTimes</span></span>

<span data-ttu-id="eb5cd-118">在读取指定的用户和资源的闲 / 忙状态和工作时间方面 [findMeetingTimes](../api-reference/v1.0/api/user_findmeetingtimes.md) 操作类似于 **getSchedule** 。</span><span class="sxs-lookup"><span data-stu-id="eb5cd-118">The [findMeetingTimes](../api-reference/v1.0/api/user_findmeetingtimes.md) action is similar to **getSchedule** in that both read the free/busy status and working hours of specified users and resources.</span></span> <span data-ttu-id="eb5cd-119">在几个主要方式上，两个操作是不同的。</span><span class="sxs-lookup"><span data-stu-id="eb5cd-119">The two actions differ in a few major ways.</span></span>

### <a name="application"></a><span data-ttu-id="eb5cd-120">应用程序</span><span class="sxs-lookup"><span data-stu-id="eb5cd-120">Application</span></span>

<span data-ttu-id="eb5cd-121">**findMeetingTimes** 应用某些业务逻辑来建议会议时间和地点，例如：</span><span class="sxs-lookup"><span data-stu-id="eb5cd-121">**findMeetingTimes** applies certain business logic to suggest meeting times and locations, such as:</span></span>

- <span data-ttu-id="eb5cd-122">每个实体的可选或强制出席</span><span class="sxs-lookup"><span data-stu-id="eb5cd-122">Optional or mandatory attendance of each entity</span></span>
- <span data-ttu-id="eb5cd-123">那天那个时间请求活动的性质</span><span class="sxs-lookup"><span data-stu-id="eb5cd-123">The nature of the requested activity for the time of the day</span></span>
- <span data-ttu-id="eb5cd-124">会议法定人数要求的最少出席人数</span><span class="sxs-lookup"><span data-stu-id="eb5cd-124">The minimum attendance required for a quorum for a meeting</span></span>

<span data-ttu-id="eb5cd-125">适合依赖 [简化预约预定](findmeetingtimes_example.md) 的方案。</span><span class="sxs-lookup"><span data-stu-id="eb5cd-125">It is appropriate for scenarios that depend on [streamlining appointment booking](findmeetingtimes_example.md).</span></span>

<span data-ttu-id="eb5cd-126">对于给定的时间段， **getSchedule** 只返回每个请求日历中现有事件的闲 / 忙状态，并假定该时间段的剩余时间为空闲。</span><span class="sxs-lookup"><span data-stu-id="eb5cd-126">**getSchedule** simply returns the free/busy status of existing events in each of the requested calendars for a given time period, and assumes the remaining time in that time period tp be free.</span></span> <span data-ttu-id="eb5cd-127">然后，进一步应用业务逻辑，使用该数据完成方案。</span><span class="sxs-lookup"><span data-stu-id="eb5cd-127">You would then apply further business logic to make use of this data to complete your scenario.</span></span>

### <a name="app-only-support"></a><span data-ttu-id="eb5cd-128">仅限应用程序的支持</span><span class="sxs-lookup"><span data-stu-id="eb5cd-128">App-only support</span></span>

<span data-ttu-id="eb5cd-129">**findmeetingtimes** 仅支持需要用户已登录应用程序的委派方案。</span><span class="sxs-lookup"><span data-stu-id="eb5cd-129">**findmeetingtimes** supports only delegated scenarios which require a user to have signed in to the app.</span></span> <span data-ttu-id="eb5cd-130">应用程序只能读取已登录用户可以访问的日历中的事件。</span><span class="sxs-lookup"><span data-stu-id="eb5cd-130">The app can read events in only the calendars that the signed-in user can access.</span></span> <span data-ttu-id="eb5cd-131">这可以包括其他用户已委派或与登录用户共享的日历。</span><span class="sxs-lookup"><span data-stu-id="eb5cd-131">This can include calendars that other users have delegated or shared with the signed-in user.</span></span>

<span data-ttu-id="eb5cd-132">**getSchedule** 支持委派和仅应用程序的方案。</span><span class="sxs-lookup"><span data-stu-id="eb5cd-132">**getSchedule** supports both delegated and app-only scenarios.</span></span> <span data-ttu-id="eb5cd-133">后者，管理员许可应用程序在没有已登录用户的情况下访问所有日历。</span><span class="sxs-lookup"><span data-stu-id="eb5cd-133">In the latter, an administrator consents the app to access all calendars without a signed-in user.</span></span>


### <a name="version-support"></a><span data-ttu-id="eb5cd-134">版本支持</span><span class="sxs-lookup"><span data-stu-id="eb5cd-134">Version support</span></span>

<span data-ttu-id="eb5cd-135">**findmeetingtimes** 通常适用于所有应用程序。</span><span class="sxs-lookup"><span data-stu-id="eb5cd-135">**findmeetingtimes** is generally available for all apps.</span></span> 

<span data-ttu-id="eb5cd-136">**getSchedule** 当前 [在预览状态](versioning_and_support.md#beta-version) 中可用，所以不适合生产应用。</span><span class="sxs-lookup"><span data-stu-id="eb5cd-136">**getSchedule** is currently available [in preview status](versioning_and_support.md#beta-version), and therefore is not appropriate for use in production apps.</span></span>


## <a name="permissions"></a><span data-ttu-id="eb5cd-137">权限</span><span class="sxs-lookup"><span data-stu-id="eb5cd-137">Permissions</span></span>
<span data-ttu-id="eb5cd-138">获取闲 / 忙信息所需的最低权限是 Calendar.Read。</span><span class="sxs-lookup"><span data-stu-id="eb5cd-138">The least privileged permission you need to get free/busy information is Calendar.Read.</span></span> <span data-ttu-id="eb5cd-139">根据应用方案，可由已登录的用户或管理员完成许可。</span><span class="sxs-lookup"><span data-stu-id="eb5cd-139">Depending on your app scenario, this can be consented by the signed-in user or administrator.</span></span>
<span data-ttu-id="eb5cd-140">不同于请求实体的闲 / 忙状态和工作时间， **getSchedule** 也可以返回事件的主题和位置，前提是：</span><span class="sxs-lookup"><span data-stu-id="eb5cd-140">Other than the free/busy status and working hours of requested entities, **getSchedule** can also return the subject and location of an event, provided that:</span></span>

- <span data-ttu-id="eb5cd-141">如果事件标记为低的敏感度级别 - `normal` 或 `personal` 且应用以下一个或多个条件：</span><span class="sxs-lookup"><span data-stu-id="eb5cd-141">If the event is marked with low sensitivity level - `normal` or `personal` AND one or more of the following conditions applies:</span></span>

- <span data-ttu-id="eb5cd-142">请求的用户日历设置允许组织中的所有用户查看标题和位置</span><span class="sxs-lookup"><span data-stu-id="eb5cd-142">The requested user’s calendar settings allow all the users in the organization to view titles and locations</span></span>
- <span data-ttu-id="eb5cd-143">请求的用户日历与已登录的用户共享</span><span class="sxs-lookup"><span data-stu-id="eb5cd-143">The requested user’s calendar is shared with the signed-in user</span></span>
- <span data-ttu-id="eb5cd-144">已登录的用户是与请求用户同一组织的管理员。</span><span class="sxs-lookup"><span data-stu-id="eb5cd-144">The signed-in user is an administrator of the same organization as the requested user.</span></span>

## <a name="time-zone-representation"></a><span data-ttu-id="eb5cd-145">时区表示形式</span><span class="sxs-lookup"><span data-stu-id="eb5cd-145">Time zone representation</span></span>
<span data-ttu-id="eb5cd-146">默认方式，在 UTC 中表示返回计划项目的开始和结束时间。</span><span class="sxs-lookup"><span data-stu-id="eb5cd-146">By default, the start and end times of the returned schedule items are represented in UTC.</span></span> <span data-ttu-id="eb5cd-147">可以使用 `Prefer` 标头指定适合应用程序的时区。</span><span class="sxs-lookup"><span data-stu-id="eb5cd-147">You can use a `Prefer` header to specify a time zone appropriate for your app.</span></span> <span data-ttu-id="eb5cd-148">示例：</span><span class="sxs-lookup"><span data-stu-id="eb5cd-148">As an example:</span></span> 
```
Prefer: outlook.timezone="Pacific Standard Time"
```

## <a name="limits-and-error-conditions"></a><span data-ttu-id="eb5cd-149">限制和错误条件</span><span class="sxs-lookup"><span data-stu-id="eb5cd-149">Limits and error conditions</span></span>
<span data-ttu-id="eb5cd-150">注意以下限制和错误条件：</span><span class="sxs-lookup"><span data-stu-id="eb5cd-150">Be aware of the following limits and error condition:</span></span>

- <span data-ttu-id="eb5cd-151">**getSchedule** 一次可以查找最多 20 个实体的闲 / 忙信息。</span><span class="sxs-lookup"><span data-stu-id="eb5cd-151">**getSchedule** can support looking up free/busy information for up to 20 entities at once.</span></span> <span data-ttu-id="eb5cd-152">此限制应用于单独或作为通讯组列表成员识别的用户数量，亦应用于资源数量。</span><span class="sxs-lookup"><span data-stu-id="eb5cd-152">This limit applies to the number of users identified individually or as members of a distribution list, and to the number of resources as well.</span></span>
- <span data-ttu-id="eb5cd-153">查找的时间段必须小于 42 天。</span><span class="sxs-lookup"><span data-stu-id="eb5cd-153">The time period to look up must be less than 42 days.</span></span>
- <span data-ttu-id="eb5cd-154">如果 **getSchedule** 不能识别特定的用户或者资源，它将返回单个计划项目并指示错误。</span><span class="sxs-lookup"><span data-stu-id="eb5cd-154">If **getSchedule** cannot identify a specified user or resource, it returns a single schedule item and indicates the error.</span></span> 

## <a name="see-also"></a><span data-ttu-id="eb5cd-155">另请参阅</span><span class="sxs-lookup"><span data-stu-id="eb5cd-155">See also</span></span>
- [<span data-ttu-id="eb5cd-156">权限参考</span><span class="sxs-lookup"><span data-stu-id="eb5cd-156">Permissions reference</span></span>](permissions_reference.md#calendars-permissions)
- [<span data-ttu-id="eb5cd-157">在 Outlook 日历上查找可能的会议时间</span><span class="sxs-lookup"><span data-stu-id="eb5cd-157">Find possible meeting times on the Outlook calendar</span></span>](findmeetingtimes_example.md)
