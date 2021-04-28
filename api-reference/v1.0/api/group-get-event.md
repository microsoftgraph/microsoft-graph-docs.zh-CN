---
title: 获取事件
description: 获取 event 对象。
author: yyuank
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: f69c592a0739f654781d136999ab52cc9ee8bf54
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52050470"
---
# <a name="get-event"></a><span data-ttu-id="b54bf-103">获取事件</span><span class="sxs-lookup"><span data-stu-id="b54bf-103">Get event</span></span>

<span data-ttu-id="b54bf-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b54bf-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="b54bf-105">获取 [event](../resources/event.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="b54bf-105">Get an [event](../resources/event.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="b54bf-106">权限</span><span class="sxs-lookup"><span data-stu-id="b54bf-106">Permissions</span></span>
<span data-ttu-id="b54bf-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b54bf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b54bf-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="b54bf-109">Permission type</span></span>      | <span data-ttu-id="b54bf-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b54bf-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b54bf-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b54bf-111">Delegated (work or school account)</span></span> | <span data-ttu-id="b54bf-112">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b54bf-112">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="b54bf-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b54bf-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b54bf-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="b54bf-114">Not supported.</span></span>    |
|<span data-ttu-id="b54bf-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="b54bf-115">Application</span></span> | <span data-ttu-id="b54bf-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="b54bf-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b54bf-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b54bf-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/events/{id}
GET /groups/{id}/calendar/events/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b54bf-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="b54bf-118">Optional query parameters</span></span>
<span data-ttu-id="b54bf-119">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="b54bf-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b54bf-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="b54bf-120">Request headers</span></span>
| <span data-ttu-id="b54bf-121">名称</span><span class="sxs-lookup"><span data-stu-id="b54bf-121">Name</span></span>       | <span data-ttu-id="b54bf-122">类型</span><span class="sxs-lookup"><span data-stu-id="b54bf-122">Type</span></span> | <span data-ttu-id="b54bf-123">说明</span><span class="sxs-lookup"><span data-stu-id="b54bf-123">Description</span></span> |
|:---------------|:--------|:--------|
| <span data-ttu-id="b54bf-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="b54bf-124">Authorization</span></span>  | <span data-ttu-id="b54bf-125">string</span><span class="sxs-lookup"><span data-stu-id="b54bf-125">string</span></span> | <span data-ttu-id="b54bf-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="b54bf-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="b54bf-128">Prefer: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="b54bf-128">Prefer: outlook.timezone</span></span>  | <span data-ttu-id="b54bf-129">string</span><span class="sxs-lookup"><span data-stu-id="b54bf-129">string</span></span> | <span data-ttu-id="b54bf-130">此选项可用于指定响应中开始时间和结束时间的时区。</span><span class="sxs-lookup"><span data-stu-id="b54bf-130">Use this to specify the time zone for start and end times in the response.</span></span> <span data-ttu-id="b54bf-131">如果未指定，返回的这些时间值采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="b54bf-131">If not specified, those time values are returned in UTC.</span></span> <span data-ttu-id="b54bf-132">可选。</span><span class="sxs-lookup"><span data-stu-id="b54bf-132">Optional.</span></span> |
| <span data-ttu-id="b54bf-133">Prefer: outlook.body-content-type</span><span class="sxs-lookup"><span data-stu-id="b54bf-133">Prefer: outlook.body-content-type</span></span> | <span data-ttu-id="b54bf-134">string</span><span class="sxs-lookup"><span data-stu-id="b54bf-134">string</span></span> | <span data-ttu-id="b54bf-135">要返回的 **body** 属性的格式。</span><span class="sxs-lookup"><span data-stu-id="b54bf-135">The format of the **body** property to be returned in.</span></span> <span data-ttu-id="b54bf-136">可取值为“text”或“html”。</span><span class="sxs-lookup"><span data-stu-id="b54bf-136">Values can be "text" or "html".</span></span> <span data-ttu-id="b54bf-137">如果指定此 `Preference-Applied` 头，返回 `Prefer` 头作为证明。</span><span class="sxs-lookup"><span data-stu-id="b54bf-137">A `Preference-Applied` header is returned as confirmation if this `Prefer` header is specified.</span></span> <span data-ttu-id="b54bf-138">如果未指定此头，采用 HTML 格式返回 **body** 属性。</span><span class="sxs-lookup"><span data-stu-id="b54bf-138">If the header is not specified, the **body** property is returned in HTML format.</span></span> <span data-ttu-id="b54bf-139">可选。</span><span class="sxs-lookup"><span data-stu-id="b54bf-139">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b54bf-140">请求正文</span><span class="sxs-lookup"><span data-stu-id="b54bf-140">Request body</span></span>
<span data-ttu-id="b54bf-141">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="b54bf-141">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b54bf-142">响应</span><span class="sxs-lookup"><span data-stu-id="b54bf-142">Response</span></span>
<span data-ttu-id="b54bf-143">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [event](../resources/event.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="b54bf-143">If successful, this method returns a `200 OK` response code and an [event](../resources/event.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b54bf-144">示例</span><span class="sxs-lookup"><span data-stu-id="b54bf-144">Example</span></span>
#### <a name="request"></a><span data-ttu-id="b54bf-145">请求</span><span class="sxs-lookup"><span data-stu-id="b54bf-145">Request</span></span>
<span data-ttu-id="b54bf-146">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="b54bf-146">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="b54bf-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="b54bf-147">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["02bd9fd6-8f93-4758-87c3-1fb73740a315", "AQMkAGI5MWY5ZmUyLTJiNzYtNDE0ZC04OWEwLWM3M2FjYmM3NwAzZWYARgAAA_b2VnUAiWNLj0xeSOs499YHAMT2RdsuOqRIlQZ4vOzp66YAAAIBDQAAAMT2RdsuOqRIlQZ4vOzp66YAAAIJOgAAAA=="],
  "name": "get_group_event"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groups/02bd9fd6-8f93-4758-87c3-1fb73740a315/events/AQMkAGI5MWY5ZmUyLTJiNzYtNDE0ZC04OWEwLWM3M2FjYmM3NwAzZWYARgAAA_b2VnUAiWNLj0xeSOs499YHAMT2RdsuOqRIlQZ4vOzp66YAAAIBDQAAAMT2RdsuOqRIlQZ4vOzp66YAAAIJOgAAAA==
```
# <a name="c"></a>[<span data-ttu-id="b54bf-148">C#</span><span class="sxs-lookup"><span data-stu-id="b54bf-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-group-event-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b54bf-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b54bf-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-group-event-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b54bf-150">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b54bf-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-group-event-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b54bf-151">Java</span><span class="sxs-lookup"><span data-stu-id="b54bf-151">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-group-event-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="b54bf-152">响应</span><span class="sxs-lookup"><span data-stu-id="b54bf-152">Response</span></span>
<span data-ttu-id="b54bf-153">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="b54bf-153">The following is an example of the response.</span></span>
><span data-ttu-id="b54bf-154">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="b54bf-154">**Note:** The response object shown here might be shortened for readability.</span></span>

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
    "iCalUId": "040000008200E00074C5B7101A82E00800000000B23663002F0AD301000000000000000010000000B7C936D4C2FEC749824EE24B2FD7DA62",
    "reminderMinutesBeforeStart": 15,
    "isReminderOn": true,
    "hasAttachments": false,
    "subject": "Continuing Education Sync",
    "bodyPreview": "Higher Education Planning.\r\n\r\n\r\n\r\nJoin Microsoft Teams Online Meeting<https://teams.microsoft.com/l/meetup-join/19%3acc89e82c01e349d4998655891d93e12e%40thread.skype/1501527510806?tenantId=dcd219dd-bc68-4b9b-bf0b-4a33a796be35>",
    "importance": "normal",
    "sensitivity": "normal",
    "isAllDay": false,
    "isCancelled": false,
    "isDraft": false,
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
  "tocPath": "",
  "suppressions": [
  ]
}-->

