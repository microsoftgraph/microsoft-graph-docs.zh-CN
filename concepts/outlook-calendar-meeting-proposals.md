---
title: 在 Outlook 中建议新的会议时间
description: 在 Outlook 中，会议组织者可以允许被邀请者建议备选会议时间。
author: harini84
localization_priority: Priority
ms.prod: outlook
ms.openlocfilehash: a09c7bec65c69cd1f5058cae5eddc1b99a22e694
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2021
ms.locfileid: "50472312"
---
# <a name="propose-new-meeting-times-in-outlook"></a><span data-ttu-id="5f30e-103">在 Outlook 中建议新的会议时间</span><span class="sxs-lookup"><span data-stu-id="5f30e-103">Propose new meeting times in Outlook</span></span>

<span data-ttu-id="5f30e-104">在 Outlook 中，如果被邀请者无法在原始设置的日期/时间参加会议并暂定接受或拒绝，则会议组织者可以允许被邀请者建议备选会议时间。</span><span class="sxs-lookup"><span data-stu-id="5f30e-104">In Outlook, a meeting organizer can allow invitees to propose alternative meeting times, if they cannot meet at the original set date/time and accept tentatively or decline.</span></span> <span data-ttu-id="5f30e-105">组织者可通过适当调整会议时间来接受建议。</span><span class="sxs-lookup"><span data-stu-id="5f30e-105">The organizer can accept a proposal by adjusting the meeting time as appropriate.</span></span>

## <a name="example-attendee-responds-tentative-and-suggests-a-different-datetime"></a><span data-ttu-id="5f30e-106">示例：与会者做出暂定响应并建议不同的日期/时间</span><span class="sxs-lookup"><span data-stu-id="5f30e-106">Example: attendee responds tentative and suggests a different date/time</span></span>
<span data-ttu-id="5f30e-107">下面是一个示例，其中 Alex 邀请 Adele 共进午餐，Adele 暂定接受并建议备选日期和时间，然后 Alex 通过相应地调整会议来接受建议：</span><span class="sxs-lookup"><span data-stu-id="5f30e-107">The following is an example where Alex invites Adele to lunch, Adele tentatively accepts and proposes an alternative date and time, and Alex accepts the proposal by adjusting the meeting accordingly:</span></span>

1. <span data-ttu-id="5f30e-108">作为组织者，Alex 向 Adele 发送了一个会议请求。</span><span class="sxs-lookup"><span data-stu-id="5f30e-108">As the organizer, Alex sends a meeting request to Adele.</span></span> <span data-ttu-id="5f30e-109">他将 [event](/graph/api/resources/event?view=graph-rest-1.0) 的 **allowNewTimeProposals** 属性设置为 `true`，以便让 Adele 在需要时建议另一个时间。</span><span class="sxs-lookup"><span data-stu-id="5f30e-109">He sets the **allowNewTimeProposals** property of the [event](/graph/api/resources/event?view=graph-rest-1.0) to `true` to let Adele suggest another time if she needs to.</span></span>

    <!-- {
      "blockType": "request",
      "name": "create_event"
    }-->
    ```http
    POST https://graph.microsoft.com/v1.0/me/events
    Prefer: outlook.timezone="Pacific Standard Time"
    Content-type: application/json

    {
      "subject": "Let's go for lunch",
      "body": {
        "contentType": "HTML",
        "content": "Does noon work for you?"
      },
      "start": {
          "dateTime": "2019-08-15T12:00:00",
          "timeZone": "Pacific Standard Time"
      },
      "end": {
          "dateTime": "2019-08-15T14:00:00",
          "timeZone": "Pacific Standard Time"
      },
      "allowNewTimeProposals": true,
      "location":{
          "displayName":"Harry's Bar"
      },
      "attendees": [
        {
          "emailAddress": {
          "address":"AdeleV@contoso.OnMicrosoft.com",
          "name": "Adele Vance"
          },
          "type": "required"
        }
      ]
    }
    ```

    <span data-ttu-id="5f30e-110">Alex 获得以下响应：</span><span class="sxs-lookup"><span data-stu-id="5f30e-110">Alex gets the following response:</span></span> 
    <!-- {
      "blockType": "response",
      "name": "create_event",
      "truncated": true,
      "@odata.type": "microsoft.graph.event"
    } -->
    ```http
    HTTP/1.1 201 Created
    Content-type: application/json

    {
      "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users('64339082-ed84-4b0b-b4ab-004ae54f3747')/events/$entity",
      "@odata.etag": "W/\"NEXywgsVrkeNsFsyVyRrtAAAAhBhkg==\"",
      "id": "AAMkADAwJXJGu0AAACEhWOAAA=",
      "createdDateTime": "2019-08-01T06:41:07.805128Z",
      "lastModifiedDateTime": "2019-08-01T06:41:08.3298275Z",
      "changeKey": "NEXywgsVrkeNsFsyVyRrtAAAAhBhkg==",
      "categories": [],
      "originalStartTimeZone": "Pacific Standard Time",
      "originalEndTimeZone": "Pacific Standard Time",
      "uid": "0400000082008A9979A0BD16",
      "reminderMinutesBeforeStart": 15,
      "isReminderOn": true,
      "hasAttachments": false,
      "subject": "Let's go for lunch",
      "bodyPreview": "Does noon work for you?",
      "importance": "normal",
      "sensitivity": "normal",
      "isAllDay": false,
      "isCancelled": false,
      "isOrganizer": true,
      "responseRequested": true,
      "seriesMasterId": null,
      "showAs": "busy",
      "type": "singleInstance",
      "webLink": "https://outlook.office365.com/owa/?itemid=AAMkADAwJXJGu0AAACEhWOAAA%3D&exvsurl=1&path=/calendar/item",
      "onlineMeetingUrl": null,
      "allowNewTimeProposals": true,
      "recurrence": null,
      "responseStatus": {
        "response": "organizer",
        "time": "0001-01-01T00:00:00Z"
      },
      "body": {
        "contentType": "html",
        "content": "<html>\r\n<head>\r\n<meta http-equiv=\"Content-Type\" content=\"text/html; charset=utf-8\">\r\n<meta content=\"text/html; charset=us-ascii\">\r\n</head>\r\n<body>\r\nDoes late morning work for you?\r\n</body>\r\n</html>\r\n"
      },
      "start": {
        "dateTime": "2019-08-15T12:00:00.0000000",
        "timeZone": "Pacific Standard Time"
      },
      "end": {
        "dateTime": "2019-08-15T14:00:00.0000000",
        "timeZone": "Pacific Standard Time"
      },
      "location": {
        "displayName": "Harry's Bar",
        "locationType": "default",
        "uniqueId": "Harry's Bar",
        "uniqueIdType": "private"
      },
     "locations": [
        {
            "displayName": "Harry's Bar",
            "locationType": "default",
            "uniqueId": "Harry's Bar",
            "uniqueIdType": "private"
        }
      ],
      "attendees": [
        {
            "type": "required",
            "status": {
                "response": "none",
                "time": "0001-01-01T00:00:00Z"
            },
            "emailAddress": {
                "name": "Adele Vance",
                "address": "AdeleV@contoso.OnMicrosoft.com"
            }
        }
      ],
      "organizer": {
        "emailAddress": {
            "name": "Alex Wilber",
            "address": "AlexW@contoso.OnMicrosoft.com"
        }
      }
    }
    ```

2. <span data-ttu-id="5f30e-111">Adele 在她的收件箱中以 [eventMessageRequest](/graph/api/resources/eventmessagerequest?view=graph-rest-1.0) 的形式接收邀请。</span><span class="sxs-lookup"><span data-stu-id="5f30e-111">Adele receives the invitation in her Inbox as an [eventMessageRequest](/graph/api/resources/eventmessagerequest?view=graph-rest-1.0).</span></span> <span data-ttu-id="5f30e-112">她注意到 **allowNewTimeProposals** 属性已设置。</span><span class="sxs-lookup"><span data-stu-id="5f30e-112">She notices the **allowNewTimeProposals** property is set.</span></span> <span data-ttu-id="5f30e-113">[使用与此 **eventMessageRequest** 相关联的 **event**](/graph/api/eventmessage-get?view=graph-rest-1.0#example-2)，她做了一个暂定性答复，并在 **proposedNewTime** 正文参数中将日期建议为次日的同一时间。</span><span class="sxs-lookup"><span data-stu-id="5f30e-113">[Using the **event** associated](/graph/api/eventmessage-get?view=graph-rest-1.0#example-2) with this **eventMessageRequest**, she makes a tentative reply and proposes the next day at the same time, in the **proposedNewTime** body parameter.</span></span> <span data-ttu-id="5f30e-114">她还将 **sendResponse** 参数设置为 true。</span><span class="sxs-lookup"><span data-stu-id="5f30e-114">She also sets the **sendResponse** parameter to true.</span></span>

    <!-- {
      "blockType": "request",
      "name": "event_tentativelyaccept"
    }-->
    ```http
    POST https://graph.microsoft.com/v1.0/me/events/AAMkADU5NRaRqdoI4oeRpAAAB_woNAAA=/tentativelyAccept
    Content-type: application/json

    { 
      "comment": "Can you make the next day instead?", 
      "sendResponse": "true", 
      "proposedNewTime": {
         "Start": { 
              "DateTime": "2019-08-16T12:00:00", 
              "TimeZone": "Pacific Standard Time" 
         }, 
         "End": { 
              "DateTime": "2019-08-16T14:00:00", 
              "TimeZone": "Pacific Standard Time" 
         }
      }
    } 
    ```

    <span data-ttu-id="5f30e-115">Adele 成功进行了回复，并收到以下响应：</span><span class="sxs-lookup"><span data-stu-id="5f30e-115">Adele's reply succeeds and she gets the following response:</span></span>

    <!-- {
      "blockType": "response",
      "name": "event_tentativelyaccept"
      "truncated": true
    } -->
    ```http
    HTTP/1.1 202 Accepted
    ```

3. <span data-ttu-id="5f30e-116">Alex 收到一封 [eventMessageResponse](/graph/api/resources/eventmessageresponse?view=graph-rest-1.0) 类型的电子邮件。</span><span class="sxs-lookup"><span data-stu-id="5f30e-116">Alex receives an email of the [eventMessageResponse](/graph/api/resources/eventmessageresponse?view=graph-rest-1.0) type.</span></span> <span data-ttu-id="5f30e-117">他注意到了以下内容：</span><span class="sxs-lookup"><span data-stu-id="5f30e-117">He notices the following:</span></span>

   - <span data-ttu-id="5f30e-118">主题包含一个前缀，上面写着“已建议新时间：让我们共进午餐吧”</span><span class="sxs-lookup"><span data-stu-id="5f30e-118">The subject includes a prefix and says "New Time Proposed: Let's go for lunch"</span></span>
   - <span data-ttu-id="5f30e-119">发送者是 Adele Vance</span><span class="sxs-lookup"><span data-stu-id="5f30e-119">The sender is Adele Vance</span></span>
   - <span data-ttu-id="5f30e-120">**responseType** 是 `tentativelyAccepted`</span><span class="sxs-lookup"><span data-stu-id="5f30e-120">The **responseType** is `tentativelyAccepted`</span></span>
   - <span data-ttu-id="5f30e-121">Adele 的建议位于 **eventMessageResponse** 的 **proposedNewTime** 属性中</span><span class="sxs-lookup"><span data-stu-id="5f30e-121">Adele's proposal is in the **proposedNewTime** property of the **eventMessageResponse**</span></span>

    <!-- {
      "blockType": "request",
      "name": "get_messages"
    }-->
    ```http
    GET https://graph.microsoft.com/v1.0/me/messages?$top=1
    Prefer: outlook.timezone="Pacific Standard Time"
    ```

    <span data-ttu-id="5f30e-122">出于演示目的，假设 Adele 的回复是 Alex 邮箱中的最新消息，则 Alex 可以简单地请求该最新消息。</span><span class="sxs-lookup"><span data-stu-id="5f30e-122">For demonstration purpose, assume Adele's reply is the latest message in Alex' mailbox, and Alex can simply request that latest message.</span></span>

    <!-- {
      "blockType": "response",
      "name": "get_messages",
      "truncated": true,
      "@odata.type": "microsoft.graph.message",
      "isCollection": true
    } -->
    ```http
    HTTP/1.1 200 OK
    Content-type: application/json
    Preference-Applied: outlook.timezone="Pacific Standard Time"

    {
       "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users('64339082-ed84-4b0b-b4ab-004ae54f3747')/messages",
       "@odata.nextLink": "https://graph.microsoft.com/v1.0/me/messages?$top=1&$skip=4"",
       "value": [
          {
            "@odata.type": "#microsoft.graph.eventMessageResponse",
            "@odata.etag": "W/\"DAAAABYAAAA0RfLCCxWuR42wWzJXJGu0AAACEGHC\"",
            "id": "AAMkADAwJXJGu0AAACEiVAAAA=",
            "createdDateTime": "2019-08-01T07:06:27Z",
            "lastModifiedDateTime": "2019-08-01T07:06:28Z",
            "changeKey": "DAAAABYAAAA0RfLCCxWuR42wWzJXJGu0AAACEGHC",
            "categories": [],
            "receivedDateTime": "2019-08-01T07:06:28Z",
            "sentDateTime": "2019-08-01T07:06:24Z",
            "hasAttachments": false,
            "internetMessageId": "<BY5PR17MB38759D33B8925D525A476F33D9DE0@contoso.outlook.com>",
            "subject": "New Time Proposed: Let's go for lunch",
            "bodyPreview": "Can you make the next day instead?",
            "importance": "normal",
            "parentFolderId": "AQMkADAwQAAAIBDAAAAA==",
            "conversationId": "AAQkADAwQAQAMkh89RO3QpBiUCETTtVbIo=",
            "conversationIndex": "AdVINBlgySHz1E7dCkGJQIRNO1VsigAA4n6R",
            "isDeliveryReceiptRequested": null,
            "isReadReceiptRequested": false,
            "isRead": false,
            "isDraft": false,
            "webLink": "https://outlook.office365.com/owa/?ItemID=AAMkADAwJXJGu0AAACEiVAAAA%3D&exvsurl=1&viewmodel=ReadMessageItem",
            "inferenceClassification": "focused",
            "unsubscribeData": [],
            "unsubscribeEnabled": false,
            "meetingMessageType": "meetingTentativelyAccepted",
            "type": "singleInstance",
            "isOutOfDate": false,
            "isAllDay": false,
            "isDelegated": false,
            "responseType": "tentativelyAccepted",
            "recurrence": null,
            "body": {
                "contentType": "html",
                "content": "<html>\r\n<head>\r\n<meta http-equiv=\"Content-Type\" content=\"text/html; charset=utf-8\">\r\n<meta content=\"text/html; charset=us-ascii\">\r\n</head>\r\n<body>\r\nCan you make the next day instead?\r\n</body>\r\n</html>\r\n"
            },
            "sender": {
                "emailAddress": {
                    "name": "Adele Vance",
                    "address": "AdeleV@contoso.OnMicrosoft.com"
                }
            },
            "from": {
                "emailAddress": {
                    "name": "Adele Vance",
                    "address": "AdeleV@contoso.OnMicrosoft.com"
                }
            },
            "toRecipients": [
                {
                    "emailAddress": {
                        "name": "Alex Wilber",
                        "address": "AlexW@contoso.OnMicrosoft.com"
                    }
                }
            ],
            "ccRecipients": [],
            "bccRecipients": [],
            "replyTo": [],
            "flag": {
                "flagStatus": "notFlagged"
            },
            "startDateTime": {
                "dateTime": "2019-08-15T12:00:00.0000000",
                "timeZone": "Pacific Standard Time"
            },
            "endDateTime": {
                "dateTime": "2019-08-15T14:00:00.0000000",
                "timeZone": "Pacific Standard Time"
            },
            "location": {
                "displayName": "Harry's Bar",
                "locationType": "default",
                "uniqueIdType": "unknown"
            },
            "proposedNewTime": {
                "start": {
                    "dateTime": "2019-08-16T12:00:00", 
                    "timeZone": "Pacific Standard Time"
                },
                "end": {
                    "dateTime": "2019-08-16T14:00:00", 
                    "timeZone": "Pacific Standard Time"
                }
            }
         }
        ]
    }
    ```

4. <span data-ttu-id="5f30e-123">Alex 还注意到，午餐的 **event** 现在包括一个指示 Adele 建议的 **proposedNewTime** 属性。</span><span class="sxs-lookup"><span data-stu-id="5f30e-123">Alex also notices the **event** for the lunch now includes a **proposedNewTime** property that indicates Adele's proposal.</span></span> <span data-ttu-id="5f30e-124">如果相应的与会者建议了备选会议时间，则此属性仅在 [attendee ](/graph/api/resources/attendee?view=graph-rest-1.0) 实例中出现。</span><span class="sxs-lookup"><span data-stu-id="5f30e-124">This property is only present as part of an [attendee](/graph/api/resources/attendee?view=graph-rest-1.0) instance if the corresponding attendee has suggested an alternative meeting time.</span></span> 

    <!-- {
      "blockType": "request",
      "name": "event_get"
    }-->
    ```http
    GET https://graph.microsoft.com/v1.0/me/events/AAMkADAwJXJGu0AAACEhWOAAA=?$select=subject,allowNewTimeProposals,start,end,attendees,organizer
    Prefer: outlook.timezone="Pacific Standard Time"
    ```

    <!-- {
      "blockType": "response",
      "name": "event_get",
      "truncated": true,
      "@odata.type": "microsoft.graph.event"
    } -->
    ```http
    HTTP/1.1 200 Ok

    {
        "@odata.context": "https://graph.microsoft.com/testexchangev1.0/$metadata#users('64339082-ed84-4b0b-b4ab-004ae54f3747')/events(subject,allowNewTimeProposals,start,end,attendees,organizer)/$entity",
        "@odata.etag": "W/\"NEXywgsVrkeNsFsyVyRrtAAAAhEDMA==\"",
        "id": "AAMkADAwJXJGu0AAACEhWOAAA=",
        "subject": "Let's go for lunch",
        "allowNewTimeProposals": true,
        "start": {
            "dateTime": "2019-08-15T12:00:00.0000000",
            "timeZone": "Pacific Standard Time"
        },
        "end": {
            "dateTime": "2019-08-15T14:00:00.0000000",
            "timeZone": "Pacific Standard Time"
        },
        "attendees": [
            {
                "type": "required",
                "status": {
                    "response": "tentativelyAccepted",
                    "time": "2019-08-01T07:06:24.5046431Z"
                },
                "proposedNewTime": {
                    "start": {
                        "dateTime": "2019-08-16T12:00:00.0000000",
                        "timeZone": "Pacific Standard Time"
                    },
                    "end": {
                        "dateTime": "2019-08-16T14:00:00.0000000",
                        "timeZone": "Pacific Standard Time"
                    }
                },
                "emailAddress": {
                    "name": "Adele Vance",
                    "address": "AdeleV@contoso.OnMicrosoft.com"
                }
            }
        ],
        "organizer": {
            "emailAddress": {
                "name": "Alex Wilber",
                "address": "AlexW@contoso.OnMicrosoft.com"
            }
        }
    }
    ```


5. <span data-ttu-id="5f30e-125">Alex 决定通过将 **event** 更新为建议的 **start** 和 **end** 日期/时间来接受 Adele 的建议。</span><span class="sxs-lookup"><span data-stu-id="5f30e-125">Alex decides to accept Adele's proposal by updating the **event** to the proposed **start** and **end** date/time.</span></span>

    <!-- {
      "blockType": "request",
      "name": "event_update"
    }-->
    ```http
    PATCH https://graph.microsoft.com/v1.0/me/events/AAMkADAwJXJGu0AAACEhWOAAA=
    Prefer: outlook.timezone="Pacific Standard Time"
    Content-type: application/json

    {
        "start": {
            "dateTime": "2019-08-16T12:00:00.0000000",
            "timeZone": "Pacific Standard Time"
        },
        "end": {
            "dateTime": "2019-08-16T14:00:00.0000000",
            "timeZone": "Pacific Standard Time"
        }
    }
    ```

    <span data-ttu-id="5f30e-126">Adele 成功进行了更新，并收到以下响应。</span><span class="sxs-lookup"><span data-stu-id="5f30e-126">Alex's update succeeds and gets the following response.</span></span>

    <!-- {
      "blockType": "response",
      "name": "event_update",
      "truncated": true,
      "@odata.type": "microsoft.graph.event"
    } -->
    ```http
    HTTP/1.1 200 Ok

    {
      "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users('64339082-ed84-4b0b-b4ab-004ae54f3747')/events/$entity",
      "@odata.etag": "W/\"NEXywgsVrkeNsFsyVyRrtAAAAhBizA==\"",
      "id": "AAMkADAwJXJGu0AAACEhWOAAA=",
      "createdDateTime": "2019-08-01T06:41:07.805128Z",
      "lastModifiedDateTime": "2019-08-01T08:21:43.5696529Z",
      "changeKey": "NEXywgsVrkeNsFsyVyRrtAAAAhBizA==",
      "categories": [],
      "originalStartTimeZone": "Pacific Standard Time",
      "originalEndTimeZone": "Pacific Standard Time",
      "uid": "0400000082008A9979A0BD16",
      "reminderMinutesBeforeStart": 15,
      "isReminderOn": true,
      "hasAttachments": false,
      "subject": "Let's go for lunch",
      "bodyPreview": "Does noon work for you?",
      "importance": "normal",
      "sensitivity": "normal",
      "isAllDay": false,
      "isCancelled": false,
      "isOrganizer": true,
      "responseRequested": true,
      "seriesMasterId": null,
      "showAs": "busy",
      "type": "singleInstance",
      "webLink": "https://outlook.office365.com/owa/?itemid=AAMkADAwJXJGu0AAACEhWOAAA%3D&exvsurl=1&path=/calendar/item",
      "onlineMeetingUrl": null,
      "allowNewTimeProposals": true,
      "recurrence": null,
      "responseStatus": {
        "response": "organizer",
        "time": "0001-01-01T00:00:00Z"
      },
      "body": {
        "contentType": "html",
        "content": "<html>\r\n<head>\r\n<meta http-equiv=\"Content-Type\" content=\"text/html; charset=utf-8\">\r\n<meta content=\"text/html; charset=us-ascii\">\r\n</head>\r\n<body>\r\nDoes noon work for you?\r\n</body>\r\n</html>\r\n"
      },
      "start": {
        "dateTime": "2019-08-16T12:00:00.0000000",
        "timeZone": "Pacific Standard Time"
      },
      "end": {
        "dateTime": "2019-08-16T14:00:00.0000000",
        "timeZone": "Pacific Standard Time"
      },
      "location": {
        "displayName": "Harry's Bar",
        "locationType": "default",
        "uniqueId": "Harry's Bar",
        "uniqueIdType": "private"
      },
      "locations": [
        {
            "displayName": "Harry's Bar",
            "locationType": "default",
            "uniqueId": "Harry's Bar",
            "uniqueIdType": "private"
        }
      ],
      "attendees": [
        {
            "type": "required",
            "status": {
                "response": "notResponded",
                "time": "4501-01-01T00:00:00Z"
            },
            "emailAddress": {
                "name": "Adele Vance",
                "address": "AdeleV@contoso.OnMicrosoft.com"
            }
        }
      ],
      "organizer": {
        "emailAddress": {
            "name": "Alex Wilber",
            "address": "AlexW@contoso.OnMicrosoft.com"
        }
      }
    }
    ```


## <a name="no-attendee-proposes-alternative-time"></a><span data-ttu-id="5f30e-127">无与会者建议备选时间</span><span class="sxs-lookup"><span data-stu-id="5f30e-127">No attendee proposes alternative time</span></span>

<span data-ttu-id="5f30e-128">在步骤 2 中，如果 Adele 回答暂定或拒绝，并且没有提出不同的日期/时间，则会发生以下情况：</span><span class="sxs-lookup"><span data-stu-id="5f30e-128">In step 2, if Adele replied tentative or declined, and did not propose a different date/time, then the following would happen:</span></span>

- <span data-ttu-id="5f30e-129">在步骤 3 中，Alex 将收到 **responseType** 属性设置为 `tentativelyAccepted` 的 **eventMessageResponse**（如果 Adele 拒绝，则设置为 `decline`）。</span><span class="sxs-lookup"><span data-stu-id="5f30e-129">In step 3, Alex would receive an **eventMessageResponse** with the **responseType** property set to `tentativelyAccepted` (or `decline` if Adele declined).</span></span> <span data-ttu-id="5f30e-130">在此 **eventMessageResponse** 实例中，Alex 将找不到 **proposedNewTime** 属性。</span><span class="sxs-lookup"><span data-stu-id="5f30e-130">Alex would not find a **proposedNewTime** property in this instance of **eventMessageResponse**.</span></span>
- <span data-ttu-id="5f30e-131">在步骤 4 中，Alex 在关联的 **event** 中也找不到 **proposedNewTime** 属性。</span><span class="sxs-lookup"><span data-stu-id="5f30e-131">In step 4, Alex would not find a **proposedNewTime** property in the associated **event** either.</span></span>

## <a name="see-also"></a><span data-ttu-id="5f30e-132">另请参阅</span><span class="sxs-lookup"><span data-stu-id="5f30e-132">See also</span></span>
- [<span data-ttu-id="5f30e-133">在 Outlook 日历中查找可能会议时间</span><span class="sxs-lookup"><span data-stu-id="5f30e-133">Finding possible meeting times on the Outlook calendar</span></span>](findmeetingtimes-example.md)
- [<span data-ttu-id="5f30e-134">获取用户和资源的忙/闲日程安排</span><span class="sxs-lookup"><span data-stu-id="5f30e-134">Getting the free/busy schedule for users and resources</span></span>](outlook-get-free-busy-schedule.md)
- [<span data-ttu-id="5f30e-135">在 Outlook 中将重复约会安排为定期事件</span><span class="sxs-lookup"><span data-stu-id="5f30e-135">Scheduling repeating appointments as recurring events in Outlook</span></span>](outlook-schedule-recurring-events.md)