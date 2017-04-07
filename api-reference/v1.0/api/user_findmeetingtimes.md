# <a name="user-findmeetingtimes"></a>user: findMeetingTimes
根据组织者和与会者忙/闲状态以及指定为参数的时间或地点约束，查找会议时间建议。

如果 **findMeetingTimes** 无法返回任何会议时间建议，响应会在 **emptySuggestionsReason** 属性中指明原因。根据此值，可以更好地调整参数，并重新调用 **findMeetingTimes**。

**注意**

**findMeetingTimes** 当前假设：

- 所有 [attendee](../resources/attendee.md) 都是必需的人员（而不是资源）。因此，在 **attendees** 集合参数中，在相应的 **type** 属性中为人员指定 `required`，为资源指定 `resource`。
- 所有会议时间建议都不会超出组织者或与会者的工作时间。可以忽略指定 [timeConstraint](../resources/timeConstraint.md) 的 **activityDomain** 属性。 


## <a name="prerequisites"></a>先决条件
若要执行此 API，必须有以下**范围**之一：*Calendars.Read.Shared* 或 *Calendars.ReadWrite.Shared*
## <a name="http-request"></a>HTTP 请求
<!-- { "blockType": "ignored" } -->
```http
POST /me/findMeetingTimes
POST /users/{id|userPrincipalName}/findMeetingTimes
```
## <a name="request-headers"></a>请求标头
| 名称       | 值|
|:---------------|:----------|
| Authorization  | Bearer <code>|
| Prefer: outlook.timezone | 表示响应的具体时区的字符串，例如，“Pacific Standard Time”。 |


## <a name="request-body"></a>请求正文
下面列出了支持的所有参数。根据你自己的方案，在请求正文中为各个必需参数指定 JSON 对象。根据指定的参数，**findMeetingTimes** 会检查组织者和与会者的主日历中的忙/闲状态。此操作会计算出最可行的会议时间，并返回所有会议时间建议。


| 参数       | 类型    |说明|
|:---------------|:--------|:----------|
|attendees|[attendeeBase](../resources/attendeebase.md) 集合|一组会议与会者或资源。若集合为空，**findMeetingTimes** 只会查找组织者的空闲时间段。|
|locationConstraint|[locationConstraint](../resources/locationconstraint.md)|组织者对会议地点的要求，如是否必须返回会议地点建议，或是否只能在特定地点举行会议。|
|timeConstraint|[timeConstraint](../resources/timeconstraint.md)|会议开始时间和结束时间范围。可以在此参数的 **start** 和 **end** 属性中指定时区。不过，此时区只影响 **timeConstraint** 参数；如果响应中返回了时间值（若有），仍默认采用 UTC。可以使用 `Prefer: outlook.timezone` 请求头为响应中的时间值指定具体时区。 |
|meetingDuration|Edm.Duration|会议时长，以 [ISO8601](http://www.iso.org/iso/iso8601) 格式表示。例如，1 小时表示为“PT1H”，其中“P”是持续时间指示符，“T”是时间指示符，“H”是小时指示符。如果未指定会议持续时间，**findMeetingTimes** 使用默认值 30 分钟。 |
|maxCandidates|Edm.Int32|要返回的会议时间建议数量上限。|
|isOrganizerOptional|Edm.Boolean|若为 `True`，表示组织者不一定要出席；若为 `false`，表示组织者一定要出席。|
|returnSuggestionReasons|Edm.Boolean|若为 `True`，表示在 **suggestionReason** 属性中返回每个会议时间建议的理由。默认为 `false`，即不返回此属性。|
|minimumAttendeePercentage|Edm.Double| 在响应中返回时间段所需的最低 [confidence](#the-confidence-of-a-meeting-suggestion)。这是一个介于 0 到 100 之间的百分比值。 |

## <a name="response"></a>响应
如果成功，此方法在响应正文中返回 `200, OK` 响应代码和 [meetingTimeSuggestionsResult](../resources/meetingTimeSuggestionsResult.md)。 

**meetingTimeSuggestionsResult** 包含一组会议时间建议和 **emptySuggestionsReason** 属性。每条建议都被定义为 [meetingTimeSuggestion](../resources/meetingTimeSuggestion.md)，同时与会者出席置信度平均值为 50%，或为你在 **minimumAttendeePercentage** 参数中指定的特定百分比值。 

默认情况下，返回的每条会议时间建议的时区均为 UTC。 

### <a name="the-confidence-of-a-meeting-suggestion"></a>会议时间建议的置信度

**meetingTimeSuggestion** 的 **confidence** 属性值介于 0% 到 100% 之间，表示所有与会者出席会议的可能性（以每个人的忙/闲状态为依据）：

- 对于每个与会者，在指定的会议时间段内，空闲、未知和忙碌状态对应的与会者出席可能性分别为 100%、49% 和 0%。
- 会议时间建议的置信度是通过计算相应会议的所有指定与会者的出席可能性平均值而得出。
- 如果有多条会议时间建议，**findMeetingTimes** 操作首先会按计算得出的置信度值由高到低对建议进行排序。如果会议时间建议的置信度相同，此操作会按时间顺序对建议进行排序。
- 可以使用 **findMeetingTimes** 的可选参数 **minimumAttendeePercentage**，指定仅返回置信度不低于特定值的会议时间建议。例如，如果只想返回所有与会者的出席可能性不低于 80% 的会议时间建议，可以将 **minimumAttendeePercentage** 指定为 80%。如果未指定 **minimumAttendeePercentage**，**findMeetingTimes** 假定值为 50%。

例如，如果会议时间建议涉及 3 位与会者，他们的忙/闲状态如下：

|**与会者**|**忙/闲状态**|**出席可能性 (%)**|
|:-----|:-----|:-----|
|Dana | 空闲 | 100% |
|John | 未知 | 49% |
|Fanny | 忙碌 | 0% |

会议时间建议的置信度为与会者出席可能性的平均值，即 (100% + 49% + 0%)/3 = 49.66%。

如果你在 **findMeetingTimes** 操作中将 **minimumAttendeePercentage** 指定为 80%，此操作将不会在响应中建议此时间，这是因为 49.66% < 80%。

## <a name="example"></a>示例

以下示例展示了如何查找预定地点会议的时间，并请求获得各条建议的理由，具体是通过在请求正文中指定以下参数：

- **attendees**
- **locationConstraint**
- **timeConstraint**
- **meetingDuration**
- **returnSuggestionReasons**
- **minimumAttendeePercentage**

设置 **returnSuggestionReasons** 参数后，**suggestionReason** 属性中还会返回各条建议的理由（如果 **findMeetingTimes** 返回建议的话）。

请注意，请求指定的是 PST 时区时间，而响应返回的会议时间建议默认采用 UTC。可以使用 `Prefer: outlook.timezone` 请求头也为响应中的时间值指定 PST 时区。

##### <a name="request"></a>请求
下面展示了示例请求。
<!-- {
  "blockType": "request",
  "name": "user_findmeetingtimes"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/findMeetingTimes
Content-type: application/json

{ 
  "attendees": [ 
    { 
      "type": "required",  
      "emailAddress": { 
        "name": "Fanny Downs",
        "address": "fannyd@a830edad905084922E16072013.onmicrosoft.com" 
      } 
    },
    { 
      "type": "optional",  
      "emailAddress": { 
        "name": "Dana Swope",
        "address": "danas@a830edad905084922E16072013.onmicrosoft.com" 
      } 
    } 
  ],  
  "locationConstraint": { 
    "isRequired": "false",  
    "suggestLocation": "false",  
    "locations": [ 
      { 
        "resolveAvailability": "false",
        "displayName": "Conf room Hood" 
      } 
    ] 
  },  
  "timeConstraint": { 
    "timeslots": [ 
      { 
        "start": { 
          "dateTime": "2016-10-20T07:00:00",  
          "timeZone": "Pacific Standard Time" 
        },  
        "end": { 
          "dateTime": "2016-10-20T17:00:00",  
          "timeZone": "Pacific Standard Time" 
        } 
      } 
    ] 
  },  
  "meetingDuration": "PT2H",
  "returnSuggestionReasons": "true",
  "minimumAttendeePercentage": "60"
}
```

##### <a name="response"></a>响应
下面展示了示例响应。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.meetingTimeSuggestionsResult",
  "isCollection": false
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json


{
   "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#microsoft.graph.meetingTimeSuggestionsResult",
   "meetingTimeSuggestions":[
      {
         "meetingTimeSlot":{
            "start":{
               "dateTime":"2016-10-20T15:00:00.0000000",
               "timeZone":"UTC"
            },
            "end":{
               "dateTime":"2016-10-20T17:00:00.0000000",
               "timeZone":"UTC"
            }
         },
         "confidence":100,
         "organizerAvailability":"free",
         "attendeeAvailability":[
            {
               "attendee":{
                  "type":"required",
                  "emailAddress":{
                    "name": "Fanny Downs",
                    "address": "fannyd@a830edad905084922E16072013.onmicrosoft.com" 
                  }
               },
               "availability":"free"
            },
            {
               "attendee":{
                  "type":"required",
                  "emailAddress":{
                    "name": "Dana Swope",
                    "address": "danas@a830edad905084922E16072013.onmicrosoft.com" 
                  }
               },
               "availability":"free"
            }
         ],
         "locations":[
            {
               "displayName":"Conf room Hood"
            }
         ],
         "suggestionReason":"Suggested because it is one of the nearest times when all attendees are available."
      },
      {
         "meetingTimeSlot":{
            "start":{
               "dateTime":"2016-10-20T17:00:00.0000000",
               "timeZone":"UTC"
            },
            "end":{
               "dateTime":"2016-10-20T19:00:00.0000000",
               "timeZone":"UTC"
            }
         },
         "confidence":100,
         "organizerAvailability":"free",
         "attendeeAvailability":[
            {
               "attendee":{
                  "type":"required",
                  "emailAddress":{
                    "name": "Fanny Downs",
                    "address": "fannyd@a830edad905084922E16072013.onmicrosoft.com" 
                  }
               },
               "availability":"free"
            },
            {
               "attendee":{
                  "type":"required",
                  "emailAddress":{
                    "name": "Dana Swope",
                    "address": "danas@a830edad905084922E16072013.onmicrosoft.com" 
                  }
               },
               "availability":"unknown"
            }
         ],
         "locations":[
            {
               "displayName":"Conf room Hood"
            }
         ],
         "suggestionReason":"Suggested because it is one of the nearest times when all attendees are available."
      }
   ],
   "emptySuggestionsReason":""
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "user: findMeetingTimes",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->