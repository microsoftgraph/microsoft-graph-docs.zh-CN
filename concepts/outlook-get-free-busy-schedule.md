# <a name="get-freebusy-schedule-of-users-and-resources-preview"></a>获取用户和资源的闲 / 忙计划（预览）

在工作或学校设置中，一个常见的应用方案是查看用户什么时候有时间参加会议，或者浏览某一团队、会议室或设备在一特定时段是否有时间以及是否可用。

[GetSchedule](../api-reference/beta/api/calendar_getschedule.md) 操作可以获取某一特定时段内诸如用户、通讯组列表或资源等一个或多个实体的可用性信息。 

## <a name="example"></a>示例

一个简单的示例是查看同事 Alex 在某一天自上午九点至下午六点（太平洋标准时间）的闲 / 忙计划。

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

**getSchedule** 返回两个与 Alex 默认日历现有事件相匹配的计划项，显示的每个事件的开始和结束时间以及事件的闲 / 忙状态。 可以假定在该日期 / 时间范围内的剩余时间 Alex 是有空的。

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

除了 Alex 的闲 / 忙计划和工作时间外， **getSchedule** 也会返回 **availabilityView**，即 Alex 在该天有时间的合并视图。 合并视图是一个字符串，由覆盖那一天的时间段构成，每个时间段使用以下约定指示 Alex 是否有空： 

- `0`= 空闲
- `1`= 暂定
- `2`= 忙碌
- `3`= 不在办公室
- `4`= 在其他位置工作。 

默认方式，每个时间段的长度为 30 分钟。 本示例使用 **availabilityViewInterval** 属性将时间段自定义为 15 分钟。

## <a name="how-is-getschedule-different-from-findmeetingtimes"></a>getSchedule 与 findMeetingTimes 有何不同

在读取指定的用户和资源的闲 / 忙状态和工作时间方面 [findMeetingTimes](../api-reference/v1.0/api/user_findmeetingtimes.md) 操作类似于 **getSchedule** 。 在几个主要方式上，两个操作是不同的。

### <a name="application"></a>应用程序

**findMeetingTimes** 应用某些业务逻辑来建议会议时间和地点，例如：

- 每个实体的可选或强制出席
- 那天那个时间请求活动的性质
- 会议法定人数要求的最少出席人数

适合依赖 [简化预约预定](findmeetingtimes_example.md) 的方案。

对于给定的时间段， **getSchedule** 只返回每个请求日历中现有事件的闲 / 忙状态，并假定该时间段的剩余时间为空闲。 然后，进一步应用业务逻辑，使用该数据完成方案。

### <a name="app-only-support"></a>仅限应用程序的支持

**findmeetingtimes** 仅支持需要用户已登录应用程序的委派方案。 应用程序只能读取已登录用户可以访问的日历中的事件。 这可以包括其他用户已委派或与登录用户共享的日历。

**getSchedule** 支持委派和仅应用程序的方案。 后者，管理员许可应用程序在没有已登录用户的情况下访问所有日历。


### <a name="version-support"></a>版本支持

**findmeetingtimes** 通常适用于所有应用程序。 

**getSchedule** 当前 [在预览状态](versioning_and_support.md#beta-version) 中可用，所以不适合生产应用。


## <a name="permissions"></a>权限
获取闲 / 忙信息所需的最低权限是 Calendar.Read。 根据应用方案，可由已登录的用户或管理员完成许可。
不同于请求实体的闲 / 忙状态和工作时间， **getSchedule** 也可以返回事件的主题和位置，前提是：

- 如果事件标记为低的敏感度级别 - `normal` 或 `personal` 且应用以下一个或多个条件：

- 请求的用户日历设置允许组织中的所有用户查看标题和位置
- 请求的用户日历与已登录的用户共享
- 已登录的用户是与请求用户同一组织的管理员。

## <a name="time-zone-representation"></a>时区表示形式
默认方式，在 UTC 中表示返回计划项目的开始和结束时间。 可以使用 `Prefer` 标头指定适合应用程序的时区。 示例： 
```
Prefer: outlook.timezone="Pacific Standard Time"
```

## <a name="limits-and-error-conditions"></a>限制和错误条件
注意以下限制和错误条件：

- **getSchedule** 一次可以查找最多 20 个实体的闲 / 忙信息。 此限制应用于单独或作为通讯组列表成员识别的用户数量，亦应用于资源数量。
- 查找的时间段必须小于 42 天。
- 如果 **getSchedule** 不能识别特定的用户或者资源，它将返回单个计划项目并指示错误。 

## <a name="see-also"></a>另请参阅
- [权限参考](permissions_reference.md#calendars-permissions)
- [在 Outlook 日历上找到可能的会议时间](findmeetingtimes_example.md)
