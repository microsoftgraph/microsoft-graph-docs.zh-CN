---
title: 获取事件
description: 获取 event 对象。
ms.openlocfilehash: f67c7aef7203f86edf963e6b3d0add1f0260dfcc
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27042644"
---
# <a name="get-event"></a><span data-ttu-id="ae9b3-103">获取事件</span><span class="sxs-lookup"><span data-stu-id="ae9b3-103">Get event</span></span>

> <span data-ttu-id="ae9b3-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="ae9b3-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ae9b3-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="ae9b3-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="ae9b3-106">获取 [event](../resources/event.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="ae9b3-106">Get an [event](../resources/event.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="ae9b3-107">权限</span><span class="sxs-lookup"><span data-stu-id="ae9b3-107">Permissions</span></span>
<span data-ttu-id="ae9b3-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ae9b3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ae9b3-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="ae9b3-110">Permission type</span></span>      | <span data-ttu-id="ae9b3-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ae9b3-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ae9b3-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ae9b3-112">Delegated (work or school account)</span></span> | <span data-ttu-id="ae9b3-113">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ae9b3-113">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="ae9b3-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ae9b3-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ae9b3-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="ae9b3-115">Not supported.</span></span>    |
|<span data-ttu-id="ae9b3-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="ae9b3-116">Application</span></span> | <span data-ttu-id="ae9b3-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="ae9b3-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ae9b3-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ae9b3-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/events/{id}
GET /groups/{id}/calendar/events/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ae9b3-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="ae9b3-119">Optional query parameters</span></span>
<span data-ttu-id="ae9b3-120">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="ae9b3-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ae9b3-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="ae9b3-121">Request headers</span></span>
| <span data-ttu-id="ae9b3-122">名称</span><span class="sxs-lookup"><span data-stu-id="ae9b3-122">Name</span></span>       | <span data-ttu-id="ae9b3-123">类型</span><span class="sxs-lookup"><span data-stu-id="ae9b3-123">Type</span></span> | <span data-ttu-id="ae9b3-124">说明</span><span class="sxs-lookup"><span data-stu-id="ae9b3-124">Description</span></span> |
|:---------------|:--------|:--------|
| <span data-ttu-id="ae9b3-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="ae9b3-125">Authorization</span></span>  | <span data-ttu-id="ae9b3-126">string</span><span class="sxs-lookup"><span data-stu-id="ae9b3-126">string</span></span> | <span data-ttu-id="ae9b3-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="ae9b3-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="ae9b3-129">Prefer: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="ae9b3-129">Prefer: outlook.timezone</span></span>  | <span data-ttu-id="ae9b3-130">string</span><span class="sxs-lookup"><span data-stu-id="ae9b3-130">string</span></span> | <span data-ttu-id="ae9b3-131">此选项可用于指定响应中开始时间和结束时间的时区。</span><span class="sxs-lookup"><span data-stu-id="ae9b3-131">Use this to specify the time zone for start and end times in the response.</span></span> <span data-ttu-id="ae9b3-132">如果未指定，返回的这些时间值采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="ae9b3-132">If not specified, those time values are returned in UTC.</span></span> <span data-ttu-id="ae9b3-133">可选。</span><span class="sxs-lookup"><span data-stu-id="ae9b3-133">Optional.</span></span> |
| <span data-ttu-id="ae9b3-134">Prefer: outlook.body-content-type</span><span class="sxs-lookup"><span data-stu-id="ae9b3-134">Prefer: outlook.body-content-type</span></span> | <span data-ttu-id="ae9b3-135">string</span><span class="sxs-lookup"><span data-stu-id="ae9b3-135">string</span></span> | <span data-ttu-id="ae9b3-136">要返回的 **body** 属性的格式。</span><span class="sxs-lookup"><span data-stu-id="ae9b3-136">The format of the **body** property to be returned in.</span></span> <span data-ttu-id="ae9b3-137">可取值为“text”或“html”。</span><span class="sxs-lookup"><span data-stu-id="ae9b3-137">Values can be "text" or "html".</span></span> <span data-ttu-id="ae9b3-138">如果指定此 `Preference-Applied` 头，返回 `Prefer` 头作为证明。</span><span class="sxs-lookup"><span data-stu-id="ae9b3-138">A `Preference-Applied` header is returned as confirmation if this `Prefer` header is specified.</span></span> <span data-ttu-id="ae9b3-139">如果未指定此头，采用 HTML 格式返回 **body** 属性。</span><span class="sxs-lookup"><span data-stu-id="ae9b3-139">If the header is not specified, the **body** property is returned in HTML format.</span></span> <span data-ttu-id="ae9b3-140">可选。</span><span class="sxs-lookup"><span data-stu-id="ae9b3-140">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ae9b3-141">请求正文</span><span class="sxs-lookup"><span data-stu-id="ae9b3-141">Request body</span></span>
<span data-ttu-id="ae9b3-142">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="ae9b3-142">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ae9b3-143">响应</span><span class="sxs-lookup"><span data-stu-id="ae9b3-143">Response</span></span>
<span data-ttu-id="ae9b3-144">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [event](../resources/event.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="ae9b3-144">If successful, this method returns a `200 OK` response code and an [event](../resources/event.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ae9b3-145">示例</span><span class="sxs-lookup"><span data-stu-id="ae9b3-145">Example</span></span>
#### <a name="request"></a><span data-ttu-id="ae9b3-146">请求</span><span class="sxs-lookup"><span data-stu-id="ae9b3-146">Request</span></span>
<span data-ttu-id="ae9b3-147">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="ae9b3-147">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_group_event"
}-->
```http
GET https://graph.microsoft.com/beta/groups/02bd9fd6-8f93-4758-87c3-1fb73740a315/events/AQMkAGI5MWY5ZmUyLTJiNzYtNDE0ZC04OWEwLWM3M2FjYmM3NwAzZWYARgAAA_b2VnUAiWNLj0xeSOs499YHAMT2RdsuOqRIlQZ4vOzp66YAAAIBDQAAAMT2RdsuOqRIlQZ4vOzp66YAAAIJOgAAAA==
```

#### <a name="response"></a><span data-ttu-id="ae9b3-148">响应</span><span class="sxs-lookup"><span data-stu-id="ae9b3-148">Response</span></span>
<span data-ttu-id="ae9b3-149">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="ae9b3-149">The following is an example of the response.</span></span>
><span data-ttu-id="ae9b3-p106">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="ae9b3-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.event"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 1728

{
    "id": "AQMkAGI5MWY5ZmUyLTJiNzYtNDE0ZC04OWEwLWM3M2FjYmM3NwAzZWYARgAAA_b2VnUAiWNLj0xeSOs499YHAMT2RdsuOqRIlQZ4vOzp66YAAAIBDQAAAMT2RdsuOqRIlQZ4vOzp66YAAAIJOgAAAA==",
    "createdDateTime": "2017-07-31T18:58:31.011909Z",
    "lastModifiedDateTime": "2017-07-31T18:58:35.418473Z",
    "changeKey": "xPZF2y46pEiVBni87OnrpgAAAAAJTg==",
    "categories": [],
    "originalStartTimeZone": "Eastern Standard Time",
    "originalEndTimeZone": "Eastern Standard Time",
    "uid": "040000008200E00074C5B7101A82E00800000000B23663002F0AD301000000000000000010000000B7C936D4C2FEC749824EE24B2FD7DA62",
    "reminderMinutesBeforeStart": 15,
    "isReminderOn": true,
    "hasAttachments": false,
    "subject": "Continuing Education Sync",
    "bodyPreview": "Higher Education Planning.\r\n\r\n\r\n\r\nJoin Microsoft Teams Online Meeting<https://teams.microsoft.com/l/meetup-join/19%3acc89e82c01e349d4998655891d93e12e%40thread.skype/1501527510806?tenantId=dcd219dd-bc68-4b9b-bf0b-4a33a796be35>",
    "importance": "normal",
    "sensitivity": "normal",
    "isAllDay": false,
    "isCancelled": false,
    "isOrganizer": true,
    "responseRequested": true,
    "seriesMasterId": null,
    "showAs": "busy",
    "type": "seriesMaster",
    "webLink": "https://outlook.office365.com/owa/?itemid=AQMkAGI5MWY5ZmUyLTJiNzYtNDE0ZC04OWEwLWM3M2FjYmM3NwAzZWYARgAAA%2Bb2VnUAiWNLj0xeSOs499YHAMT2RdsuOqRIlQZ4vOzp66YAAAIBDQAAAMT2RdsuOqRIlQZ4vOzp66YAAAIJOgAAAA%3D%3D&exvsurl=1&path=/calendar/item",
    "onlineMeetingUrl": null,
    "responseStatus": {
        "response": "organizer",
        "time": "0001-01-01T00:00:00Z"
    },
    "body": {
        "contentType": "html",
        "content": "<html>\r\n<head>\r\n<meta http-equiv=\"Content-Type\" content=\"text/html; charset=utf-8\">\r\n</head>\r\n<body>\r\n<div>Higher Education Planning.</div>\r\n<div><br>\r\n<br>\r\n<br>\r\n<a href=\"https://teams.microsoft.com/l/meetup-join/19%3acc89e82c01e349d4998655891d93e12e%40thread.skype/1501527510806?tenantId=dcd219dd-bc68-4b9b-bf0b-4a33a796be35\">Join Microsoft Teams Online Meeting</a></div>\r\n</body>\r\n</html>\r\n"
    },
    "start": {
        "dateTime": "2017-08-15T14:30:00.0000000",
        "timeZone": "UTC"
    },
    "end": {
        "dateTime": "2017-08-15T15:30:00.0000000",
        "timeZone": "UTC"
    },
    "location": {
        "displayName": "HR Taskforce / Benefits"
    },
    "recurrence": {
        "pattern": {
            "type": "weekly",
            "interval": 1,
            "month": 0,
            "dayOfMonth": 0,
            "daysOfWeek": [
                "tuesday",
                "thursday"
            ],
            "firstDayOfWeek": "sunday",
            "index": "first"
        },
        "range": {
            "type": "noEnd",
            "startDate": "2017-08-15",
            "endDate": "0001-01-01",
            "recurrenceTimeZone": "Eastern Standard Time",
            "numberOfOccurrences": 0
        }
    },
    "attendees": [
        {
            "type": "required",
            "status": {
                "response": "accepted",
                "time": "2017-07-31T18:58:34.3298022Z"
            },
            "emailAddress": {
                "name": "Lidia Holloway",
                "address": "LidiaH@contoso.com"
            }
        },
        {
            "type": "required",
            "status": {
                "response": "none",
                "time": "0001-01-01T00:00:00Z"
            },
            "emailAddress": {
                "name": "HR Taskforce",
                "address": "HRTaskforce@contoso.com"
            }
        },
        {
            "type": "required",
            "status": {
                "response": "none",
                "time": "0001-01-01T00:00:00Z"
            },
            "emailAddress": {
                "name": "Diego Siciliani",
                "address": "DiegoS@contoso.com"
            }
        },
        {
            "type": "required",
            "status": {
                "response": "none",
                "time": "0001-01-01T00:00:00Z"
            },
            "emailAddress": {
                "name": "Johanna Lorenz",
                "address": "JohannaL@contoso.com"
            }
        },
        {
            "type": "required",
            "status": {
                "response": "none",
                "time": "0001-01-01T00:00:00Z"
            },
            "emailAddress": {
                "name": "Megan Bowen",
                "address": "MeganB@contoso.com"
            }
        }
    ],
    "organizer": {
        "emailAddress": {
            "name": "HR Taskforce",
            "address": "HRTaskforce@contoso.com"
        }
    }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get event",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
