---
title: 获取 Outlook 日历用户和资源的忙/闲计划
description: 使用 getSchedule 操作获取一个或多个用户、通讯组列表或资源在特定时间段内的状态信息。
author: tariq-sharif
ms.localizationpriority: high
ms.prod: outlook
ms.openlocfilehash: 263e3b5462b688f0dff98714bd646a247dde9765
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/29/2022
ms.locfileid: "66439030"
---
# <a name="get-freebusy-schedule-of-outlook-calendar-users-and-resources"></a>获取 Outlook 日历用户和资源的忙/闲计划

在工作或学校设置中，一种常见方案是查看用户何时有空参加会议，或浏览团队、会议室或设备在一段时间内的状态。

使用 [getSchedule](/graph/api/calendar-getschedule) 操作，可以获取一个或多个实体&mdash;用户、通讯组列表或资源&mdash;在特定时间段内的状态信息。

## <a name="example"></a>示例

下面的简单示例展示了如何查找同事 Alex 在某天上午 9 点到下午 6 点（太平洋标准时间）之间的忙/闲日程安排：

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

**getSchedule** 返回两个与 Alex 默认日历中现有事件匹配的日程安排项，同时显示每个事件的开始时间和结束时间及其忙/闲状态。 可以假定 Alex 在此日期/时间范围的剩余时间内是空闲的。

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

除了 Alex 的忙/闲日程安排和工作时间之外，**getSchedule** 还返回 **availabilityView**，这是 Alex 这一天状态的合并视图。 此合并视图是一个字符串，其中包含这一天的所有时间段，每个时间段都使用以下约定指明 Alex 的状态： 

- `0`= 空闲
- `1`= 暂定
- `2`= 忙碌
- `3`= 外出
- `4`= 在其他地方工作。 

默认情况下，每个时间段的长度为 30 分钟。 此示例使用 **availabilityViewInterval** 属性，将时间段自定义为 15 分钟。

## <a name="how-does-getschedule-compare-with-findmeetingtimes"></a>getSchedule 如何与 findMeetingTimes 进行比较

[findMeetingTimes](/graph/api/user-findmeetingtimes) 操作与 **getSchedule** 类似，两者都读取指定用户和资源的忙/闲状态和工作时间。 这两项操作的区别主要在以下几方面。

### <a name="application"></a>用途

**findMeetingTimes** 应用特定业务逻辑来建议会议时间和地点，如：

- 每个实体是自愿与会还是必须与会
- 一天内请求执行的活动的性质
- 会议仲裁要求的最少与会人数

它适用于依赖[简化约会预订](findmeetingtimes-example.md)的方案。

**getSchedule** 只返回每个所需日历中现有事件在给定时间段内的忙/闲状态，并假定在此时间段的剩余时间内是空闲的。 然后，应用其他业务逻辑来利用此类数据完成方案。

### <a name="app-only-support"></a>仅应用支持

**findmeetingtimes** 仅支持要求用户必须已登录应用的委托方案。 应用只能读取已登录用户可以访问的日历中的事件。 这可以包括其他用户已委托或已与登录用户共享的日历。

**getSchedule** 支持委托方案和仅应用方案。 对于后者，管理员同意应用访问所有日历，即使没有已登录用户，也不例外。

### <a name="permissions"></a>权限
**findmeetingtimes** 所需的最低特权权限为 Calendars.Read.Shared。

**getSchedule** 所需的最低特权权限为 Calendars.Read。 

### <a name="version-support"></a>版本支持

**findmeetingtimes** 和 **getSchedule** 均已正式发布且适用于生产应用。


## <a name="event-data-returned"></a>返回的事件数据
要使应用能够获取忙/闲信息，**getSchedule** 所需的最低特权权限为 Calendars.Read。 根据应用方案，这可由已登录用户或管理员同意授予。

虽然借助同意后授予的权限，应用可通过 Outlook 在所请求用户的日历上使用 **getSchedule** 但所请求的用户可控制该 **getSchedule** 返回的事件数据（若有）。 

例如，**getSchedule** 可返回所请求用户的忙/闲状态和工作时间，还能返回事件的 **subject**、**location** 和 **isPrivate**，但前提是：

- 事件被标记为低敏感度级别（`normal` 或 `personal`），且符合以下一个或多个条件：

  - 所请求的用户的日历设置允许用户登录后查看主题行和位置
  - 所请求的用户的日历与已登录用户共享

无论已登录用户是否是组织中的管理员，都需遵循这些条件。 所请求的用户可控制返回的事件数据。

## <a name="time-zone-representation"></a>时区表示
默认情况下，返回的日程安排项的开始时间和结束时间都采用 UTC。 可使用 `Prefer` 头指定适合应用的时区。 例如： 
``` http
Prefer: outlook.timezone="Pacific Standard Time"
```

## <a name="limits-and-error-conditions"></a>限制和错误条件
请注意以下限制和错误条件：

- **getSchedule** 支持一次查找最多 20 个实体的忙/闲信息。 标识为个人的用户数或标识为通讯组列表成员的用户数以及资源数都计入此限制。
- 查找时间段不得长于 42 天。
- 如果 **getSchedule** 无法识别指定用户或资源，便会返回一个日程安排项并指明错误。 


## <a name="see-also"></a>另请参阅
- [权限参考](permissions-reference.md#calendars-permissions)
- [在 Outlook 日历上查找可能的会议时间](findmeetingtimes-example.md)
