---
title: 'user: findMeetingTimes'
description: 根据组织者和与会者的可用性以及指定为参数的时间或位置约束, 建议会议时间和位置。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 345b42690644fb94a2b6b2bdf6b3cfcc9ead6333
ms.sourcegitcommit: 539ed08adf3b7ad3253c98636d4ab303ce00176e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/15/2019
ms.locfileid: "30057055"
---
# <a name="user-findmeetingtimes"></a>user: findMeetingTimes

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

根据组织者和与会者的可用性以及指定为参数的时间或位置约束, 建议会议时间和位置。

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
| Prefer: outlook.timezone | 表示响应的具体时区的字符串，例如，“Pacific Standard Time”。可选。如果未指定此标头则使用 UTC。 |

## <a name="request-body"></a>请求正文
下面列出了支持的所有参数。根据你自己的方案，在请求正文中为各个必需参数指定 JSON 对象。 


| 参数    | 类型   |说明|
|:---------------|:--------|:----------|
|与会者|[attendeeDataModel](../resources/attendeedatamodel.md)集合|会议的与会者或资源的集合。 在对应的 **"类型**" 属性`required`中`optional` , 指定人员的`resource`或, 为会议室和资源 (如会议室) 指定或。 如果未指定, **** 则 findMeetingTimes `required`将假定为**type**属性。 空集合导致**findMeetingTimes**仅查找组织者的空闲时间段。 可选。|
|isOrganizerOptional|Edm.Boolean|如果组织者不必必须参加，则指定 `True`。默认值为 `false`。可选。|
|locationConstraint|[locationConstraints](../resources/locationconstraints.md)|组织者对会议地点的要求，如是否必须返回会议地点建议，或是否只能在特定地点举行会议。可选。|
|maxCandidates|Edm.Int32|要返回的会议时间建议数量上限。可选。|
|meetingDuration|Edm.Duration|会议的长度, 以[ISO 8601](https://www.iso.org/iso/iso8601)格式表示。 例如, 1 小时表示为 "PT1H", 其中 ' P ' 是持续时间指示器, ' t ' 是时间指示器, ' H ' 是小时指示符。 使用 M 指示持续时间的分钟数;例如, 2 小时零30分钟是 "PT2H30M"。 如果未指定会议持续时间, 则**findMeetingTimes**将使用默认值30分钟。 可选。|
|minimumAttendeePercentage|Edm.Double| 在响应中返回时间段所需的最低 [confidence](#the-confidence-of-a-meeting-suggestion)。这是一个介于 0 到 100 之间的百分比值。可选。|
|returnSuggestionReasons|Edm.Boolean|指定 `True` 可以在 **suggestionReason** 属性中返回每个会议建议的理由。默认为 `false`，即不返回此属性。可选。|
|timeConstraint|[findMeetingTimesTimeConstraints](../resources/findmeetingtimestimeconstraints.md)|会议的所有时间限制，可以包括会议性质（**activityDomain** 属性）和可能的会议时间段（**timeSlots** 属性）。如果未指定此参数，则 **findMeetingTimes** 将 **activityDomain** 假定为 `work`。可选。|

下表介绍了可以在 **timeConstraint** 参数中进一步指定的限制。

|timeConstraint 中的 activityDomain 值|会议时间建议|
|:-----|:-----|
|工时| 建议处于用户的工作时间（在用户的日历配置中定义该时间，并且可由用户或管理员自定义）内。默认工作时间是星期一到星期五的上午八点到下午五点（使用为邮箱设置的时区）。如果未指定 **activityDomain** 则此为默认值。 |
|personal| 建议处于用户的工作时间内及星期六和星期日。默认是星期一到星期日的上午八点到下午五点（使用邮箱的时区设置）。|
|unrestricted | 建议可以是全年任意一天的任意时间段。|
|unknown | 请勿使用此值，因为以后会弃用此值。当前其行为与 `work` 相同。根据需要将任何现有代码更改为使用 `work`、`personal`、或 `unrestricted`。|


根据指定的参数，**findMeetingTimes** 会检查组织者和与会者的主日历中的忙/闲状态。此操作会计算出最可行的会议时间，并返回所有会议时间建议。

## <a name="response"></a>响应

如果成功, 此方法在`200 OK`响应正文中返回响应代码和[findMeetingTimesResponse](../resources/findmeetingtimesresponse.md) 。 

**findMeetingTimesResponse**包括会议建议和**emptySuggestionsReason**属性的集合。 每个建议定义为[meetingTimeSuggestion](../resources/meetingtimesuggestion.md), 与会者的可信度平均为要参加的 50%, 或在**minimumAttendeePercentage**参数中指定的特定%。 

默认情况下，返回的每条会议时间建议的时区均为 UTC。 

如果 **findMeetingTimes** 无法返回任何会议时间建议，响应会在 **emptySuggestionsReason** 属性中指明原因。根据此值，可以更好地调整参数，并重新调用 **findMeetingTimes**。

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
|Samantha | 忙碌 | 0% |

会议时间建议的置信度为与会者出席可能性的平均值，即 (100% + 49% + 0%)/3 = 49.66%。

如果你在 **findMeetingTimes** 操作中将 **minimumAttendeePercentage** 指定为 80%，此操作将不会在响应中建议此时间，这是因为 49.66% < 80%。

## <a name="example"></a>示例

以下示例展示了如何查找预定地点会议的时间，并请求获得各条建议的理由，具体是通过在请求正文中指定以下参数：

- **attendees**
- **locationConstraint**
- **timeConstraint**
- **isOrganizerOptional**
- **meetingDuration**
- **returnSuggestionReasons**
- **minimumAttendeePercentage**

设置 **returnSuggestionReasons** 参数后，**suggestionReason** 属性中还会返回各条建议的理由（如果 **findMeetingTimes** 返回建议的话）。

请注意, 该请求指定了 PST 时区中的时间。 默认情况下, 响应将返回 UTC 格式的会议时间建议。 您可以使用`Prefer: outlook.timezone`请求标头为响应中的时间值指定 PST。

##### <a name="request"></a>请求
下面展示了示例请求。
<!-- {
  "blockType": "request",
  "name": "user_findmeetingtimes"
}-->
```http
POST https://graph.microsoft.com/beta/me/findMeetingTimes
Prefer: outlook.timezone="Pacific Standard Time"
Content-Type: application/json

{ 
  "attendees": [ 
    { 
      "type": "required",  
      "emailAddress": { 
        "name": "Alex Wilbur",
        "address": "alexw@contoso.onmicrosoft.com" 
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
    "activityDomain":"work", 
    "timeslots": [ 
      { 
        "start": { 
          "dateTime": "2019-04-16T09:00:00",  
          "timeZone": "Pacific Standard Time" 
        },  
        "end": { 
          "dateTime": "2019-04-18T17:00:00",  
          "timeZone": "Pacific Standard Time" 
        } 
      } 
    ] 
  },  
  "isOrganizerOptional": "false",
  "meetingDuration": "PT1H",
  "returnSuggestionReasons": "true",
  "minimumAttendeePercentage": "100"
}
```

##### <a name="response"></a>响应
下面展示了示例响应。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.findMeetingTimesResponse",
  "isCollection": false
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Preference-Applied: outlook.timezone="Pacific Standard Time"

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#microsoft.graph.findMeetingTimesResponse",
    "emptySuggestionsReason": "",
    "meetingTimeSuggestions": [
        {
            "confidence": 100,
            "organizerAvailability": "free",
            "suggestionReason": "Suggested because it is one of the nearest times when all attendees are available.",
            "attendeeAvailability": [
                {
                    "availability": "free",
                    "attendee": {
                        "emailAddress": {
                            "address": "alexw@contoso.onmicrosoft.com"
                        }
                    }
                }
            ],
            "locations": [
                {
                    "displayName": "Conf room Hood"
                }
            ],
            "meetingTimeSlot": {
                "start": {
                    "dateTime": "2019-04-18T08:00:00.0000000",
                    "timeZone": "Pacific Standard Time"
                },
                "end": {
                    "dateTime": "2019-04-18T09:00:00.0000000",
                    "timeZone": "Pacific Standard Time"
                }
            }
        },
        {
            "confidence": 100,
            "organizerAvailability": "free",
            "suggestionReason": "Suggested because it is one of the nearest times when all attendees are available.",
            "attendeeAvailability": [
                {
                    "availability": "free",
                    "attendee": {
                        "emailAddress": {
                            "address": "alexw@contoso.onmicrosoft.com"
                        }
                    }
                }
            ],
            "locations": [
                {
                    "displayName": "Conf room Hood"
                }
            ],
            "meetingTimeSlot": {
                "start": {
                    "dateTime": "2019-04-18T12:00:00.0000000",
                    "timeZone": "Pacific Standard Time"
                },
                "end": {
                    "dateTime": "2019-04-18T13:00:00.0000000",
                    "timeZone": "Pacific Standard Time"
                }
            }
        },
        {
            "confidence": 100,
            "organizerAvailability": "free",
            "suggestionReason": "Suggested because it is one of the nearest times when all attendees are available.",
            "attendeeAvailability": [
                {
                    "availability": "free",
                    "attendee": {
                        "emailAddress": {
                            "address": "alexw@contoso.onmicrosoft.com"
                        }
                    }
                }
            ],
            "locations": [
                {
                    "displayName": "Conf room Hood"
                }
            ],
            "meetingTimeSlot": {
                "start": {
                    "dateTime": "2019-04-18T16:00:00.0000000",
                    "timeZone": "Pacific Standard Time"
                },
                "end": {
                    "dateTime": "2019-04-18T17:00:00.0000000",
                    "timeZone": "Pacific Standard Time"
                }
            }
        }
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "user: findMeetingTimes",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Warning: /api-reference/beta/api/user_findmeetingtimes.md:\r\n      Failed to parse any rows out of table with headers: |activityDomain value|Suggestions for meeting times|",
    "Error: /api-reference/beta/api/user-findmeetingtimes.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
