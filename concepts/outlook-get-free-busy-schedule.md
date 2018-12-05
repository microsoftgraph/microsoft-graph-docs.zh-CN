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
# <a name="get-freebusy-schedule-of-users-and-resources-preview"></a>获取闲/忙安排的用户和资源 （预览）

在工作或学校设置中，一个常见方案是当用户参加的会议，请参阅或浏览团队、 会议室或时间段内的设备的可用性。

[GetSchedule](/graph/api/calendar-getschedule?view=graph-rest-beta)操作允许您在特定时间内的一个或多个实体的用户、 通讯组列表或资源的可用性信息。 

## <a name="example"></a>示例

一个简单的示例是同事的查找某一天，上午 9 点到下午 6 点，Pacitfic 标准时间，Alex 的忙/闲计划：

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

**getSchedule**返回两个安排匹配 Alex 中的现有事件的项默认日历，显示的每个事件以及其忙/闲状态的开始和结束时间。 您可以假定该日期/时间范围内的剩余时间是免费 Alex。

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

除了的闲/忙安排和工作时间的 Alex， **getSchedule**也会返回**availabilityView**，即 Alex 的合并的视图该天的可用性。 合并的视图是一个字符串，包含与每个时间段，指示 Alex 涵盖的一天的时间段可用性使用以下约定： 

- `0`免费 =
- `1`暂定 =
- `2`= 忙
- `3`外出 =
- `4`= 使用其他位置。 

默认情况下，每个时间段的长度为 30 分钟。 本示例使用**availabilityViewInterval**属性自定义为 15 分钟的时间段。

## <a name="how-is-getschedule-different-from-findmeetingtimes"></a>如何为不同 findMeetingTimes getSchedule

同时读取忙/闲状态和指定的用户和资源的工作时间[findMeetingTimes](/graph/api/user-findmeetingtimes?view=graph-rest-1.0)操作类似于**getSchedule** 。 在几个主要的方法，两个操作会有所不同。

### <a name="application"></a>应用程序

**findMeetingTimes**应用特定业务逻辑以建议的会议时间和位置，例如：

- 每个实体的可选或强制对现时
- 请求活动的时间的性质
- 最小出席所需的仲裁会议

它是适用于取决于[简化约会预定](findmeetingtimes-example.md)的方案。

**getSchedule**只返回在每个请求的日历忙/闲状态的现有事件给定的时间段，并假定 tp 有空的时间段的剩余时间。 然后，您将应用进一步业务逻辑，以使此数据的用于完成您的方案。

### <a name="app-only-support"></a>仅限应用程序的支持

**findmeetingtimes**支持仅委派的方案需要用户已登录到应用程序中。 应用程序可以读取的已登录的用户可以访问日历事件。 这可能包括其他用户已委派或与登录用户共享的日历。

**getSchedule**支持委派和仅应用程序的方案。 后者，管理员同意应用程序以访问已登录的用户的情况下的所有日历。


### <a name="version-support"></a>版本支持

**findmeetingtimes**是通常适用于所有应用程序。 

**getSchedule**目前[处于预览状态](versioning-and-support.md#beta-version)，并因此不适合在生产应用程序中使用。


## <a name="permissions"></a>Permissions
若要获取忙/闲信息所需的最小特权的权限是 Calendar.Read。 根据您的应用程序的方案，这可以由已登录的用户或管理员许可。
以外的忙/闲状态和工作时间请求实体， **getSchedule**也可以返回的主题和发生的事件，前提是该位置：

- 如果事件标记为低的敏感度级别-`normal`或`personal`和一个或多个以下条件适用：

- 所请求的用户的日历设置允许查看标题和位置组织中的所有用户
- 与已登录的用户共享请求的用户的日历
- 已登录的用户是为请求的用户的同一组织的管理员。

## <a name="time-zone-representation"></a>时区表示形式
默认情况下，以 UTC 表示的返回的计划项目的开始和结束时间。 您可以使用`Prefer`标头以指定适合您的应用程序所在的时区。 示例： 
```
Prefer: outlook.timezone="Pacific Standard Time"
```

## <a name="limits-and-error-conditions"></a>限制和错误条件
注意以下限制和错误情况：

- **getSchedule**可以查找忙/闲信息的最多为 20 实体同时支持。 此限制适用于单独或作为成员的通讯组列表，标识的用户数和资源以及数。
- 若要查找的时间段必须小于 42 天。
- 如果指定的用户或资源不能识别**getSchedule** ，它将返回单个计划项目并指示错误。 

## <a name="see-also"></a>另请参阅
- [权限参考 （英文）](permissions-reference.md#calendars-permissions)
- [在 Outlook 日历上找到可能的会议时间](findmeetingtimes-example.md)
