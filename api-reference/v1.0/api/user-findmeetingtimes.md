---
title: 'user: findMeetingTimes'
description: 建议的会议时间内和基于组织者和与会者可用性和作为参数指定的时间或位置约束位置。
localization_priority: Priority
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: b1e2ced373cffec19ab0d945dbc27e24833e8059
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27923164"
---
# <a name="user-findmeetingtimes"></a>user: findMeetingTimes
建议的会议时间内和基于组织者和与会者可用性和作为参数指定的时间或位置约束位置。

如果 **findMeetingTimes** 无法返回任何会议时间建议，响应会在 **emptySuggestionsReason** 属性中指明原因。根据此值，可以更好地调整参数，并重新调用 **findMeetingTimes**。


## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） | Calendars.Read.Shared、Calendars.ReadWrite.Shared    |
|委派（个人 Microsoft 帐户） | 不支持。    |
|应用程序 | 不支持。 |

## <a name="http-request"></a>HTTP 请求
<!-- { "blockType": "ignored" } -->
```http
POST /me/findMeetingTimes
POST /users/{id|userPrincipalName}/findMeetingTimes
```
## <a name="request-headers"></a>请求标头
| 名称       | 值|
|:---------------|:----------|
| Authorization  | Bearer {token}。必需。 |
| Prefer: outlook.timezone | 表示响应的具体时区的字符串，例如，“Pacific Standard Time”。可选。如果未指定此标头则使用 UTC。|

## <a name="request-body"></a>请求正文
下面列出了支持的所有参数。根据你自己的方案，在请求正文中为各个必需参数指定 JSON 对象。 


| 参数    | 类型   |说明|
|:---------------|:--------|:----------|
|attendees|[attendeeBase](../resources/attendeebase.md) 集合|一组会议与会者或资源。由于 findMeetingTimes 假设始终需要具备与会人员，因此在对应的 **type** 属性中将人员指定为 `required` 而将资源指定为 `resource`。如果集合为空，则 **findMeetingTimes** 只会查找组织者的空闲时间段。可选。|
|isOrganizerOptional|Edm.Boolean|如果组织者不必必须参加，则指定 `True`。默认值为 `false`。可选。|
|locationConstraint|[locationConstraint](../resources/locationconstraint.md)|组织者对会议地点的要求，如是否必须返回会议地点建议，或是否只能在特定地点举行会议。可选。|
|maxCandidates|Edm.Int32|要返回的会议时间建议数量上限。可选。|
|meetingDuration|Edm.Duration|会议时长，以 [ISO8601](https://www.iso.org/iso/iso8601) 格式表示。例如，1 小时表示为“PT1H”，其中“P”是持续时间指示符，“T”是时间指示符，“H”是小时指示符。使用 M 指示时长的分钟数；例如，2 小时 30 分钟是“PT2H30M”。如果未指定会议持续时间，则 **findMeetingTimes** 使用默认值 30 分钟。可选。|
|minimumAttendeePercentage|Edm.Double| 在响应中返回时间段所需的最低 [confidence](#the-confidence-of-a-meeting-suggestion)。这是一个介于 0 到 100 之间的百分比值。可选。|
|returnSuggestionReasons|Edm.Boolean|指定 `True` 可以在 **suggestionReason** 属性中返回每个会议建议的理由。默认为 `false`，即不返回此属性。可选。|
|timeConstraint|[timeConstraint](../resources/timeconstraint.md)|会议的所有时间限制，可以包括会议性质（**activityDomain** 属性）和可能的会议时间段（**timeSlots** 属性）。如果未指定此参数，则 **findMeetingTimes** 将 **activityDomain** 假定为 `work`。可选。|

下表描述了**activityDomain**限制可以进一步**timeConstraint**参数中指定。

|activityDomain 值|会议时间建议|
|:-----|:-----|
|工时| 建议处于用户的工作时间（在用户的日历配置中定义该时间，并且可由用户或管理员自定义）内。默认工作时间是星期一到星期五的上午八点到下午五点（使用为邮箱设置的时区）。如果未指定 **activityDomain** 则此为默认值。 |
|personal| 建议处于用户的工作时间内及星期六和星期日。默认是星期一到星期日的上午八点到下午五点（使用邮箱的时区设置）。|
|unrestricted | 建议可以是全年任意一天的任意时间段。|
|unknown | 请勿使用此值，因为以后会弃用此值。当前其行为与 `work` 相同。根据需要将任何现有代码更改为使用 `work`、`personal`、或 `unrestricted`。


根据指定的参数，**findMeetingTimes** 会检查组织者和与会者的主日历中的忙/闲状态。此操作会计算出最可行的会议时间，并返回所有会议时间建议。

## <a name="response"></a>响应

如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [meetingTimeSuggestionsResult](../resources/meetingtimesuggestionsresult.md)。 

**meetingTimeSuggestionsResult** 包含一组会议时间建议和 **emptySuggestionsReason** 属性。每条建议都被定义为 [meetingTimeSuggestion](../resources/meetingtimesuggestion.md)，同时与会者出席置信度平均值为 50%，或为你在 **minimumAttendeePercentage** 参数中指定的特定百分比值。 

默认情况下，返回的每条会议时间建议的时区均为 UTC。 

如果 **findMeetingTimes** 无法返回任何会议时间建议，响应会在 **emptySuggestionsReason** 属性中指明原因。根据此值，可以更好地调整参数，并重新调用 **findMeetingTimes**。

### <a name="the-confidence-of-a-meeting-suggestion"></a>会议时间建议的置信度

**meetingTimeSuggestion** 的 **confidence** 属性值介于 0% 到 100% 之间，表示所有与会者出席会议的可能性（以每个人的忙/闲状态为依据）：

- 对于每个与会者，在指定的会议时间段内，空闲、未知和忙碌状态对应的与会者出席可能性分别为 100%、49% 和 0%。
- 会议时间建议的置信度是通过计算相应会议的所有指定与会者的出席可能性平均值而得出。
- 可以使用 **findMeetingTimes** 的可选参数 **minimumAttendeePercentage**，指定仅返回置信度不低于特定值的会议时间建议。例如，如果只想返回所有与会者的出席可能性不低于 80% 的会议时间建议，可以将 **minimumAttendeePercentage** 指定为 80%。如果未指定 **minimumAttendeePercentage**，**findMeetingTimes** 假定值为 50%。
- 如果有多条会议时间建议，**findMeetingTimes** 操作首先会按计算得出的置信度值由高到低对建议进行排序。如果会议时间建议的置信度相同，此操作会按时间顺序对建议进行排序。

例如，如果会议时间建议涉及 3 位与会者，他们的忙/闲状态如下：

|**与会者**|**忙/闲状态**|**出席可能性 (%)**|
|:-----|:-----|:-----|
|Dana | 空闲 | 100% |
|John | 未知 | 49% |
|Samantha | 忙碌 | 0% |

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
Prefer: outlook.timezone="Pacific Standard Time"
Content-Type: application/json

{ 
  "attendees": [ 
    { 
      "type": "required",  
      "emailAddress": { 
        "name": "Samantha Booth",
        "address": "samanthab@contoso.onmicrosoft.com" 
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
    "activityDomain":"unrestricted", 
    "timeslots": [ 
      { 
        "start": { 
          "dateTime": "2017-04-17T09:00:00",  
          "timeZone": "Pacific Standard Time" 
        },  
        "end": { 
          "dateTime": "2017-04-19T17:00:00",  
          "timeZone": "Pacific Standard Time" 
        } 
      } 
    ] 
  },  
  "meetingDuration": "PT2H",
  "returnSuggestionReasons": true,
  "minimumAttendeePercentage": 100.0
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
Preference-Applied: outlook.timezone="Pacific Standard Time"
Content-Length: 976

{
    "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#microsoft.graph.meetingTimeSuggestionsResult",
    "emptySuggestionsReason":"",
    "meetingTimeSuggestions":[
        {
            "confidence":100.0,
            "organizerAvailability":"free",
            "suggestionReason":"Suggested because it is one of the nearest times when all attendees are available.",
            "meetingTimeSlot":{
                "start":{
                    "dateTime":"2017-04-17T18:00:00.0000000",
                    "timeZone":"Pacific Standard Time"
                },
                "end":{
                    "dateTime":"2017-04-17T20:00:00.0000000",
                    "timeZone":"Pacific Standard Time"
                }
            },
            "attendeeAvailability":[
                {
                    "availability":"free",
                    "attendee":{
                        "type":"required",
                        "emailAddress":{
                            "address":"samanthab@contoso.onmicrosoft.com"
                        }
                    }
                }
            ],
            "locations":[
                {
                    "displayName":"Conf room Hood"
                }
            ]
        },
        {
            "confidence":100.0,
            "organizerAvailability":"free",
            "suggestionReason":"Suggested because it is one of the nearest times when all attendees are available.",
            "meetingTimeSlot":{
                "start":{
                    "dateTime":"2017-04-17T20:00:00.0000000",
                    "timeZone":"Pacific Standard Time"
                },
                "end":{
                    "dateTime":"2017-04-17T22:00:00.0000000",
                    "timeZone":"Pacific Standard Time"
                }
            },
            "attendeeAvailability":[
                {
                    "availability":"free",
                    "attendee":{
                        "type":"required",
                        "emailAddress":{
                            "address":"samanthab@contoso.onmicrosoft.com"
                        }
                    }
                }
            ],
            "locations":[
                {
                    "displayName":"Conf room Hood"
                }
            ]
        }
   ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "user: findMeetingTimes",
  "keywords": "",
  "section": "documentation",
  "suppressions": [
      "Warning: /api-reference/v1.0/api/user-findmeetingtimes.md:
      Failed to parse any rows out of table with headers: |activityDomain value|Suggestions for meeting times|"
  ],
  "tocPath": ""
}-->
