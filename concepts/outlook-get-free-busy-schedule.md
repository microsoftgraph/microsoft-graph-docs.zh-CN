---
title: 获取用户和资源的忙/闲日程安排（预览版）
description: 在工作或学校设置中，一种常见方案是查看用户何时有空参加会议，或浏览团队、会议室或设备在一段时间内的状态。
ms.openlocfilehash: 8a2dd9318bdd806c99d525ee41f46d78d1963b47
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27091896"
---
# <a name="get-freebusy-schedule-of-users-and-resources-preview"></a>获取用户和资源的忙/闲日程安排（预览版）

在工作或学校设置中，一种常见方案是查看用户何时有空参加会议，或浏览团队、会议室或设备在一段时间内的状态。

使用 [getSchedule](/graph/api/calendar-getschedule?view=graph-rest-beta) 操作，可以获取一个或多个实体（用户、通讯组列表或资源）在特定时间段内的状态信息。 

## <a name="example"></a>示例

下面的简单示例展示了如何查找同事 Alex 在某天上午 9 点到下午 6 点（太平洋标准时间）之间的忙/闲日程安排：

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

除了 Alex 的忙/闲日程安排和工作时间之外，**getSchedule** 还返回 **availabilityView**，这是 Alex 这一天状态的合并视图。 此合并视图是一个字符串，其中包含这一天的所有时间段，每个时间段都使用以下约定指明 Alex 的状态： 

- `0`= 空闲
- `1`= 暂定
- `2`= 忙碌
- `3`= 外出
- `4`= 在其他地方工作。 

默认情况下，每个时间段的长度为 30 分钟。 此示例使用 **availabilityViewInterval** 属性，将时间段自定义为 15 分钟。

## <a name="how-is-getschedule-different-from-findmeetingtimes"></a>getSchedule 与 findMeetingTimes 有何区别

[findMeetingTimes](/graph/api/user-findmeetingtimes?view=graph-rest-1.0) 操作与 **getSchedule** 类似，两者都读取指定用户和资源的忙/闲状态和工作时间。 这两项操作的区别主要在以下几方面。

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


### <a name="version-support"></a>版本支持

**findmeetingtimes** 一般适用于所有应用。 

**getSchedule** 暂处于[预览状态](versioning-and-support.md#beta-version)，因此不适用于生产应用。


## <a name="permissions"></a>权限
获取忙/闲信息所需的最低权限是 Calendar.Read。 根据应用方案，这可由已登录用户或管理员同意授予。
除了所需实体的忙/闲状态和工作时间外，**getSchedule** 还可以返回事件的主题和地点，前提是：

- 如果事件被标记为低敏感度级别（`normal` 或 `personal`），且符合以下一个或多个条件：

- 所需用户的日历设置允许组织中的全部用户查看标题和地点
- 所需用户的日历与已登录用户共享
- 已登录用户是所需用户所在组织的管理员。

## <a name="time-zone-representation"></a>时区表示
默认情况下，返回的日程安排项的开始时间和结束时间都采用 UTC。 可使用 `Prefer` 头指定适合应用的时区。 例如： 
```
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
