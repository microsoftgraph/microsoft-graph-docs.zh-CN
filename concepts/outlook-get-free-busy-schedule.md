---
title: 获取闲/忙安排的用户和资源 （预览）
description: 在工作或学校设置中，一个常见方案是当用户参加的会议，请参阅或浏览团队、 会议室或时间段内的设备的可用性。
ms.openlocfilehash: 8a2dd9318bdd806c99d525ee41f46d78d1963b47
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27091896"
---
# <a name="get-freebusy-schedule-of-users-and-resources-preview"></a><span data-ttu-id="51a2f-103">获取闲/忙安排的用户和资源 （预览）</span><span class="sxs-lookup"><span data-stu-id="51a2f-103">Get free/busy schedule of users and resources (preview)</span></span>

<span data-ttu-id="51a2f-104">在工作或学校设置中，一个常见方案是当用户参加的会议，请参阅或浏览团队、 会议室或时间段内的设备的可用性。</span><span class="sxs-lookup"><span data-stu-id="51a2f-104">In a work or school setting, a common scenario is to see when a user is free for meeting, or to browse the availability of a team, room, or equipment for a time period.</span></span>

<span data-ttu-id="51a2f-105">[GetSchedule](/graph/api/calendar-getschedule?view=graph-rest-beta)操作允许您在特定时间内的一个或多个实体的用户、 通讯组列表或资源的可用性信息。</span><span class="sxs-lookup"><span data-stu-id="51a2f-105">The [getSchedule](/graph/api/calendar-getschedule?view=graph-rest-beta) action lets you get the availability information of one or more entities - users, distribution lists, or resources - for a specific period of time.</span></span> 

## <a name="example"></a><span data-ttu-id="51a2f-106">示例</span><span class="sxs-lookup"><span data-stu-id="51a2f-106">Example</span></span>

<span data-ttu-id="51a2f-107">一个简单的示例是同事的查找某一天，上午 9 点到下午 6 点，Pacitfic 标准时间，Alex 的忙/闲计划：</span><span class="sxs-lookup"><span data-stu-id="51a2f-107">A simple example is to find the free/busy schedule of a coworker, Alex, on a specific day, from 9am to 6pm, Pacitfic Standard Time:</span></span>

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

<span data-ttu-id="51a2f-108">**getSchedule**返回两个安排匹配 Alex 中的现有事件的项默认日历，显示的每个事件以及其忙/闲状态的开始和结束时间。</span><span class="sxs-lookup"><span data-stu-id="51a2f-108">**getSchedule** returns two schedule items that match existing events in Alex' default calendar, showing the start and end times of each event and its free/busy status.</span></span> <span data-ttu-id="51a2f-109">您可以假定该日期/时间范围内的剩余时间是免费 Alex。</span><span class="sxs-lookup"><span data-stu-id="51a2f-109">You can assume Alex is free for the remaining time in that date/time range.</span></span>

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

<span data-ttu-id="51a2f-110">除了的闲/忙安排和工作时间的 Alex， **getSchedule**也会返回**availabilityView**，即 Alex 的合并的视图该天的可用性。</span><span class="sxs-lookup"><span data-stu-id="51a2f-110">Apart from the free/busy schedule and working hours of Alex, **getSchedule** also returns **availabilityView**, which is a merged view of Alex' availability for that day.</span></span> <span data-ttu-id="51a2f-111">合并的视图是一个字符串，包含与每个时间段，指示 Alex 涵盖的一天的时间段可用性使用以下约定：</span><span class="sxs-lookup"><span data-stu-id="51a2f-111">The merged view is a string that consists of time slots covering that day, with each time slot indicating Alex' availability using the following convention:</span></span> 

- <span data-ttu-id="51a2f-112">`0`免费 =</span><span class="sxs-lookup"><span data-stu-id="51a2f-112">`0`= free</span></span>
- <span data-ttu-id="51a2f-113">`1`暂定 =</span><span class="sxs-lookup"><span data-stu-id="51a2f-113">`1`= tentative</span></span>
- <span data-ttu-id="51a2f-114">`2`= 忙</span><span class="sxs-lookup"><span data-stu-id="51a2f-114">`2`= busy</span></span>
- <span data-ttu-id="51a2f-115">`3`外出 =</span><span class="sxs-lookup"><span data-stu-id="51a2f-115">`3`= out of office</span></span>
- <span data-ttu-id="51a2f-116">`4`= 使用其他位置。</span><span class="sxs-lookup"><span data-stu-id="51a2f-116">`4`= working elsewhere.</span></span> 

<span data-ttu-id="51a2f-117">默认情况下，每个时间段的长度为 30 分钟。</span><span class="sxs-lookup"><span data-stu-id="51a2f-117">By default, the length of each time slot is 30 minutes.</span></span> <span data-ttu-id="51a2f-118">本示例使用**availabilityViewInterval**属性自定义为 15 分钟的时间段。</span><span class="sxs-lookup"><span data-stu-id="51a2f-118">This example uses the **availabilityViewInterval** property to customize the time slot to be 15 minutes.</span></span>

## <a name="how-is-getschedule-different-from-findmeetingtimes"></a><span data-ttu-id="51a2f-119">如何为不同 findMeetingTimes getSchedule</span><span class="sxs-lookup"><span data-stu-id="51a2f-119">How is getSchedule different from findMeetingTimes</span></span>

<span data-ttu-id="51a2f-120">同时读取忙/闲状态和指定的用户和资源的工作时间[findMeetingTimes](/graph/api/user-findmeetingtimes?view=graph-rest-1.0)操作类似于**getSchedule** 。</span><span class="sxs-lookup"><span data-stu-id="51a2f-120">The [findMeetingTimes](/graph/api/user-findmeetingtimes?view=graph-rest-1.0) action is similar to **getSchedule** in that both read the free/busy status and working hours of specified users and resources.</span></span> <span data-ttu-id="51a2f-121">在几个主要的方法，两个操作会有所不同。</span><span class="sxs-lookup"><span data-stu-id="51a2f-121">The two actions differ in a few major ways.</span></span>

### <a name="application"></a><span data-ttu-id="51a2f-122">应用程序</span><span class="sxs-lookup"><span data-stu-id="51a2f-122">Application</span></span>

<span data-ttu-id="51a2f-123">**findMeetingTimes**应用特定业务逻辑以建议的会议时间和位置，例如：</span><span class="sxs-lookup"><span data-stu-id="51a2f-123">**findMeetingTimes** applies certain business logic to suggest meeting times and locations, such as:</span></span>

- <span data-ttu-id="51a2f-124">每个实体的可选或强制对现时</span><span class="sxs-lookup"><span data-stu-id="51a2f-124">Optional or mandatory attendance of each entity</span></span>
- <span data-ttu-id="51a2f-125">请求活动的时间的性质</span><span class="sxs-lookup"><span data-stu-id="51a2f-125">The nature of the requested activity for the time of the day</span></span>
- <span data-ttu-id="51a2f-126">最小出席所需的仲裁会议</span><span class="sxs-lookup"><span data-stu-id="51a2f-126">The minimum attendance required for a quorum for a meeting</span></span>

<span data-ttu-id="51a2f-127">它是适用于取决于[简化约会预定](findmeetingtimes-example.md)的方案。</span><span class="sxs-lookup"><span data-stu-id="51a2f-127">It is appropriate for scenarios that depend on [streamlining appointment booking](findmeetingtimes-example.md).</span></span>

<span data-ttu-id="51a2f-128">**getSchedule**只返回在每个请求的日历忙/闲状态的现有事件给定的时间段，并假定 tp 有空的时间段的剩余时间。</span><span class="sxs-lookup"><span data-stu-id="51a2f-128">**getSchedule** simply returns the free/busy status of existing events in each of the requested calendars for a given time period, and assumes the remaining time in that time period tp be free.</span></span> <span data-ttu-id="51a2f-129">然后，您将应用进一步业务逻辑，以使此数据的用于完成您的方案。</span><span class="sxs-lookup"><span data-stu-id="51a2f-129">You would then apply further business logic to make use of this data to complete your scenario.</span></span>

### <a name="app-only-support"></a><span data-ttu-id="51a2f-130">仅限应用程序的支持</span><span class="sxs-lookup"><span data-stu-id="51a2f-130">App-only support</span></span>

<span data-ttu-id="51a2f-131">**findmeetingtimes**支持仅委派的方案需要用户已登录到应用程序中。</span><span class="sxs-lookup"><span data-stu-id="51a2f-131">**findmeetingtimes** supports only delegated scenarios which require a user to have signed in to the app.</span></span> <span data-ttu-id="51a2f-132">应用程序可以读取的已登录的用户可以访问日历事件。</span><span class="sxs-lookup"><span data-stu-id="51a2f-132">The app can read events in only the calendars that the signed-in user can access.</span></span> <span data-ttu-id="51a2f-133">这可能包括其他用户已委派或与登录用户共享的日历。</span><span class="sxs-lookup"><span data-stu-id="51a2f-133">This can include calendars that other users have delegated or shared with the signed-in user.</span></span>

<span data-ttu-id="51a2f-134">**getSchedule**支持委派和仅应用程序的方案。</span><span class="sxs-lookup"><span data-stu-id="51a2f-134">**getSchedule** supports both delegated and app-only scenarios.</span></span> <span data-ttu-id="51a2f-135">后者，管理员同意应用程序以访问已登录的用户的情况下的所有日历。</span><span class="sxs-lookup"><span data-stu-id="51a2f-135">In the latter, an administrator consents the app to access all calendars without a signed-in user.</span></span>


### <a name="version-support"></a><span data-ttu-id="51a2f-136">版本支持</span><span class="sxs-lookup"><span data-stu-id="51a2f-136">Version support</span></span>

<span data-ttu-id="51a2f-137">**findmeetingtimes**是通常适用于所有应用程序。</span><span class="sxs-lookup"><span data-stu-id="51a2f-137">**findmeetingtimes** is generally available for all apps.</span></span> 

<span data-ttu-id="51a2f-138">**getSchedule**目前[处于预览状态](versioning-and-support.md#beta-version)，并因此不适合在生产应用程序中使用。</span><span class="sxs-lookup"><span data-stu-id="51a2f-138">**getSchedule** is currently available [in preview status](versioning-and-support.md#beta-version), and therefore is not appropriate for use in production apps.</span></span>


## <a name="permissions"></a><span data-ttu-id="51a2f-139">Permissions</span><span class="sxs-lookup"><span data-stu-id="51a2f-139">Permissions</span></span>
<span data-ttu-id="51a2f-140">若要获取忙/闲信息所需的最小特权的权限是 Calendar.Read。</span><span class="sxs-lookup"><span data-stu-id="51a2f-140">The least privileged permission you need to get free/busy information is Calendar.Read.</span></span> <span data-ttu-id="51a2f-141">根据您的应用程序的方案，这可以由已登录的用户或管理员许可。</span><span class="sxs-lookup"><span data-stu-id="51a2f-141">Depending on your app scenario, this can be consented by the signed-in user or administrator.</span></span>
<span data-ttu-id="51a2f-142">以外的忙/闲状态和工作时间请求实体， **getSchedule**也可以返回的主题和发生的事件，前提是该位置：</span><span class="sxs-lookup"><span data-stu-id="51a2f-142">Other than the free/busy status and working hours of requested entities, **getSchedule** can also return the subject and location of an event, provided that:</span></span>

- <span data-ttu-id="51a2f-143">如果事件标记为低的敏感度级别-`normal`或`personal`和一个或多个以下条件适用：</span><span class="sxs-lookup"><span data-stu-id="51a2f-143">If the event is marked with low sensitivity level - `normal` or `personal` AND one or more of the following conditions applies:</span></span>

- <span data-ttu-id="51a2f-144">所请求的用户的日历设置允许查看标题和位置组织中的所有用户</span><span class="sxs-lookup"><span data-stu-id="51a2f-144">The requested user’s calendar settings allow all the users in the organization to view titles and locations</span></span>
- <span data-ttu-id="51a2f-145">与已登录的用户共享请求的用户的日历</span><span class="sxs-lookup"><span data-stu-id="51a2f-145">The requested user’s calendar is shared with the signed-in user</span></span>
- <span data-ttu-id="51a2f-146">已登录的用户是为请求的用户的同一组织的管理员。</span><span class="sxs-lookup"><span data-stu-id="51a2f-146">The signed-in user is an administrator of the same organization as the requested user.</span></span>

## <a name="time-zone-representation"></a><span data-ttu-id="51a2f-147">时区表示形式</span><span class="sxs-lookup"><span data-stu-id="51a2f-147">Time zone representation</span></span>
<span data-ttu-id="51a2f-148">默认情况下，以 UTC 表示的返回的计划项目的开始和结束时间。</span><span class="sxs-lookup"><span data-stu-id="51a2f-148">By default, the start and end times of the returned schedule items are represented in UTC.</span></span> <span data-ttu-id="51a2f-149">您可以使用`Prefer`标头以指定适合您的应用程序所在的时区。</span><span class="sxs-lookup"><span data-stu-id="51a2f-149">You can use a `Prefer` header to specify a time zone appropriate for your app.</span></span> <span data-ttu-id="51a2f-150">示例：</span><span class="sxs-lookup"><span data-stu-id="51a2f-150">As an example:</span></span> 
```
Prefer: outlook.timezone="Pacific Standard Time"
```

## <a name="limits-and-error-conditions"></a><span data-ttu-id="51a2f-151">限制和错误条件</span><span class="sxs-lookup"><span data-stu-id="51a2f-151">Limits and error conditions</span></span>
<span data-ttu-id="51a2f-152">注意以下限制和错误情况：</span><span class="sxs-lookup"><span data-stu-id="51a2f-152">Be aware of the following limits and error condition:</span></span>

- <span data-ttu-id="51a2f-153">**getSchedule**可以查找忙/闲信息的最多为 20 实体同时支持。</span><span class="sxs-lookup"><span data-stu-id="51a2f-153">**getSchedule** can support looking up free/busy information for up to 20 entities at once.</span></span> <span data-ttu-id="51a2f-154">此限制适用于单独或作为成员的通讯组列表，标识的用户数和资源以及数。</span><span class="sxs-lookup"><span data-stu-id="51a2f-154">This limit applies to the number of users identified individually or as members of a distribution list, and to the number of resources as well.</span></span>
- <span data-ttu-id="51a2f-155">若要查找的时间段必须小于 42 天。</span><span class="sxs-lookup"><span data-stu-id="51a2f-155">The time period to look up must be less than 42 days.</span></span>
- <span data-ttu-id="51a2f-156">如果指定的用户或资源不能识别**getSchedule** ，它将返回单个计划项目并指示错误。</span><span class="sxs-lookup"><span data-stu-id="51a2f-156">If **getSchedule** cannot identify a specified user or resource, it returns a single schedule item and indicates the error.</span></span> 

## <a name="see-also"></a><span data-ttu-id="51a2f-157">另请参阅</span><span class="sxs-lookup"><span data-stu-id="51a2f-157">See also</span></span>
- [<span data-ttu-id="51a2f-158">权限参考 （英文）</span><span class="sxs-lookup"><span data-stu-id="51a2f-158">Permissions reference</span></span>](permissions-reference.md#calendars-permissions)
- [<span data-ttu-id="51a2f-159">在 Outlook 日历上找到可能的会议时间</span><span class="sxs-lookup"><span data-stu-id="51a2f-159">Find possible meeting times on the Outlook calendar</span></span>](findmeetingtimes-example.md)
