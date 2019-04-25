---
title: 列出 calendarView
description: 在由时间范围定义的日历视图中获取事件的具体值、异常和单个实例,
localization_priority: Normal
author: dkershaw10
ms.prod: groups
ms.openlocfilehash: db4c448176f21fc2a2d691e9155f9b7bba45d873
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32583590"
---
# <a name="list-calendarview"></a><span data-ttu-id="8c82a-103">列出 calendarView</span><span class="sxs-lookup"><span data-stu-id="8c82a-103">List calendarView</span></span>
<span data-ttu-id="8c82a-104">从群组的默认日历中，获取由时间范围定义的日历视图中的事件发生次数、异常和单个实例。</span><span class="sxs-lookup"><span data-stu-id="8c82a-104">Get the occurrences, exceptions, and single instances of events in a calendar view defined by a time range, from the default calendar of a group.</span></span>

## <a name="permissions"></a><span data-ttu-id="8c82a-105">权限</span><span class="sxs-lookup"><span data-stu-id="8c82a-105">Permissions</span></span>
<span data-ttu-id="8c82a-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8c82a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8c82a-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="8c82a-108">Permission type</span></span>      | <span data-ttu-id="8c82a-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="8c82a-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8c82a-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8c82a-110">Delegated (work or school account)</span></span> | <span data-ttu-id="8c82a-111">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8c82a-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="8c82a-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8c82a-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8c82a-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="8c82a-113">Not supported.</span></span>    |
|<span data-ttu-id="8c82a-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="8c82a-114">Application</span></span> | <span data-ttu-id="8c82a-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="8c82a-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="8c82a-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8c82a-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
```

## <a name="query-parameters"></a><span data-ttu-id="8c82a-117">查询参数</span><span class="sxs-lookup"><span data-stu-id="8c82a-117">Query parameters</span></span>
<span data-ttu-id="8c82a-118">在请求 URL 中，提供以下必要查询参数的值。</span><span class="sxs-lookup"><span data-stu-id="8c82a-118">In the request URL, provide the following required query parameters with values.</span></span>

| <span data-ttu-id="8c82a-119">参数</span><span class="sxs-lookup"><span data-stu-id="8c82a-119">Parameter</span></span>    | <span data-ttu-id="8c82a-120">类型</span><span class="sxs-lookup"><span data-stu-id="8c82a-120">Type</span></span>   |<span data-ttu-id="8c82a-121">说明</span><span class="sxs-lookup"><span data-stu-id="8c82a-121">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8c82a-122">startDateTime</span><span class="sxs-lookup"><span data-stu-id="8c82a-122">startDateTime</span></span>|<span data-ttu-id="8c82a-123">String</span><span class="sxs-lookup"><span data-stu-id="8c82a-123">String</span></span>|<span data-ttu-id="8c82a-p102">时间范围的开始日期和时间以 ISO 8601 格式表示。例如，“2015-11-08T19:00:00.0000000”。</span><span class="sxs-lookup"><span data-stu-id="8c82a-p102">The start date and time of the time range, represented in ISO 8601 format. For example, "2015-11-08T19:00:00.0000000".</span></span>|
|<span data-ttu-id="8c82a-126">endDateTime</span><span class="sxs-lookup"><span data-stu-id="8c82a-126">endDateTime</span></span>|<span data-ttu-id="8c82a-127">String</span><span class="sxs-lookup"><span data-stu-id="8c82a-127">String</span></span>|<span data-ttu-id="8c82a-p103">时间范围的结束日期和时间以 ISO 8601 格式表示。例如，“2015-11-08T20:00:00.0000000”。</span><span class="sxs-lookup"><span data-stu-id="8c82a-p103">The end date and time of the time range, represented in ISO 8601 format. For example, "2015-11-08T20:00:00.0000000".</span></span>|

<span data-ttu-id="8c82a-130">此方法还支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="8c82a-130">This method also supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8c82a-131">请求头</span><span class="sxs-lookup"><span data-stu-id="8c82a-131">Request headers</span></span>
| <span data-ttu-id="8c82a-132">名称</span><span class="sxs-lookup"><span data-stu-id="8c82a-132">Name</span></span>       | <span data-ttu-id="8c82a-133">类型</span><span class="sxs-lookup"><span data-stu-id="8c82a-133">Type</span></span> | <span data-ttu-id="8c82a-134">说明</span><span class="sxs-lookup"><span data-stu-id="8c82a-134">Description</span></span> |
|:---------------|:--------|:--------|
| <span data-ttu-id="8c82a-135">Authorization</span><span class="sxs-lookup"><span data-stu-id="8c82a-135">Authorization</span></span>  | <span data-ttu-id="8c82a-136">string</span><span class="sxs-lookup"><span data-stu-id="8c82a-136">string</span></span> | <span data-ttu-id="8c82a-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="8c82a-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="8c82a-139">Prefer: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="8c82a-139">Prefer: outlook.timezone</span></span>  | <span data-ttu-id="8c82a-140">string</span><span class="sxs-lookup"><span data-stu-id="8c82a-140">string</span></span> | <span data-ttu-id="8c82a-141">此选项可用于指定响应中开始时间和结束时间的时区。</span><span class="sxs-lookup"><span data-stu-id="8c82a-141">Use this to specify the time zone for start and end times in the response.</span></span> <span data-ttu-id="8c82a-142">如果未指定，返回的这些时间值采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="8c82a-142">If not specified, those time values are returned in UTC.</span></span> <span data-ttu-id="8c82a-143">可选。</span><span class="sxs-lookup"><span data-stu-id="8c82a-143">Optional.</span></span> |
| <span data-ttu-id="8c82a-144">Prefer: outlook.body-content-type</span><span class="sxs-lookup"><span data-stu-id="8c82a-144">Prefer: outlook.body-content-type</span></span> | <span data-ttu-id="8c82a-145">string</span><span class="sxs-lookup"><span data-stu-id="8c82a-145">string</span></span> | <span data-ttu-id="8c82a-146">要返回的 **body** 属性的格式。</span><span class="sxs-lookup"><span data-stu-id="8c82a-146">The format of the **body** property to be returned in.</span></span> <span data-ttu-id="8c82a-147">可取值为“text”或“html”。</span><span class="sxs-lookup"><span data-stu-id="8c82a-147">Values can be "text" or "html".</span></span> <span data-ttu-id="8c82a-148">如果指定此 `Preference-Applied` 头，返回 `Prefer` 头作为证明。</span><span class="sxs-lookup"><span data-stu-id="8c82a-148">A `Preference-Applied` header is returned as confirmation if this `Prefer` header is specified.</span></span> <span data-ttu-id="8c82a-149">如果未指定此头，采用 HTML 格式返回 **body** 属性。</span><span class="sxs-lookup"><span data-stu-id="8c82a-149">If the header is not specified, the **body** property is returned in HTML format.</span></span> <span data-ttu-id="8c82a-150">可选。</span><span class="sxs-lookup"><span data-stu-id="8c82a-150">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8c82a-151">请求正文</span><span class="sxs-lookup"><span data-stu-id="8c82a-151">Request body</span></span>
<span data-ttu-id="8c82a-152">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="8c82a-152">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8c82a-153">响应</span><span class="sxs-lookup"><span data-stu-id="8c82a-153">Response</span></span>
<span data-ttu-id="8c82a-154">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [event](../resources/event.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="8c82a-154">If successful, this method returns a `200 OK` response code and collection of [event](../resources/event.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8c82a-155">示例</span><span class="sxs-lookup"><span data-stu-id="8c82a-155">Example</span></span>
#### <a name="request"></a><span data-ttu-id="8c82a-156">请求</span><span class="sxs-lookup"><span data-stu-id="8c82a-156">Request</span></span>
<span data-ttu-id="8c82a-157">下面的示例展示了如何请求采用文本格式返回事件主体。</span><span class="sxs-lookup"><span data-stu-id="8c82a-157">The following example requests event bodies to be returned in text format.</span></span>
<!-- {
  "blockType": "request",
  "sampleKeys": ["02bd9fd6-8f93-4758-87c3-1fb73740a315"],
  "name": "get_calendarview"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/02bd9fd6-8f93-4758-87c3-1fb73740a315/calendarView?startDateTime=2017-01-01T19:00:00.0000000&endDateTime=2017-10-01T19:00:00.00
Prefer: outlook.body-content-type="text"
```

#### <a name="response"></a><span data-ttu-id="8c82a-158">响应</span><span class="sxs-lookup"><span data-stu-id="8c82a-158">Response</span></span>
<span data-ttu-id="8c82a-159">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="8c82a-159">The following is an example of the response.</span></span>
><span data-ttu-id="8c82a-160">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="8c82a-160">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="8c82a-161">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="8c82a-161">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.event",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 1354
Preference-Applied: outlook.body-content-type="text"

{
    "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#groups('02bd9fd6-8f93-4758-87c3-1fb73740a315')/calendarView",
    "@odata.nextLink":"https://graph.microsoft.com/v1.0/groups/02bd9fd6-8f93-4758-87c3-1fb73740a315/calendarView?startDateTime=2017-01-01T19%3a00%3a00.0000000&endDateTime=2017-10-01T19%3a00%3a00.00&$skip=10",
    "value":[
        {
            "@odata.etag":"W/\"xPZF2y46pEiVBni87OnrpgAAFq78Xw==\"",
            "id":"AAMkAGI5MWYJOwAAEA==",
            "createdDateTime":"2017-07-31T18:59:01.982289Z",
            "lastModifiedDateTime":"2017-09-06T04:29:38.6647687Z",
            "changeKey":"xPZF2y46pEiVBni87OnrpgAAFq78Xw==",
            "categories":[

            ],
            "originalStartTimeZone":"Eastern Standard Time",
            "originalEndTimeZone":"Eastern Standard Time",
            "iCalUId":"040000008200E00074C5B7101A82E00807E1080E824DDB122F0AD301000000000000000010000000824A8905B038D54AA7735F117B3442ED",
            "reminderMinutesBeforeStart":15,
            "isReminderOn":true,
            "hasAttachments":false,
            "subject":"New Training Plans",
            "bodyPreview":"Meeting to plan new trainings.\r\n\r\n\r\n\r\nJoin Microsoft Teams Online Meeting<https://teams.microsoft.com/l/meetup-join/19%3a900876baa3134907b0dcb41a0d220e31%40thread.skype/1501527539926?tenantId=dcd219dd-bc68-4b9b-bf0b-4a33a796be35>",
            "importance":"normal",
            "sensitivity":"normal",
            "isAllDay":false,
            "isCancelled":false,
            "isOrganizer":true,
            "responseRequested":true,
            "seriesMasterId":null,
            "showAs":"busy",
            "type":"singleInstance",
            "webLink":"https://outlook.office365.com/owa/?itemid=AAMkAGI5MWYJOwAAEA%3D%3D&exvsurl=1&path=/calendar/item",
            "onlineMeetingUrl":null,
            "responseStatus":{
                "response":"organizer",
                "time":"0001-01-01T00:00:00Z"
            },
            "body":{
                "contentType":"text",
                "content":"Meeting to plan new trainings.\r\n\r\n\r\n\r\nJoin Microsoft Teams Online Meeting<https://teams.microsoft.com/l/meetup-join/19%3a900876baa3134907b0dcb41a0d220e31%40thread.skype/1501527539926?tenantId=dcd219dd-bc68-4b9b-bf0b-4a33a796be35>\r\n"
            },
            "start":{
                "dateTime":"2017-08-14T21:00:00.0000000",
                "timeZone":"UTC"
            },
            "end":{
                "dateTime":"2017-08-14T22:00:00.0000000",
                "timeZone":"UTC"
            },
            "location":{
                "displayName":"HR Taskforce / Facilities"
            },
            "recurrence":null,
            "attendees":[
                 {
                    "type":"required",
                    "status":{
                        "response":"none",
                        "time":"0001-01-01T00:00:00Z"
                    },
                    "emailAddress":{
                        "name":"HR Taskforce",
                        "address":"HRTaskforce@contoso.onmicrosoft.com"
                    }
                },
                {
                    "type":"required",
                    "status":{
                        "response":"none",
                        "time":"0001-01-01T00:00:00Z"
                    },
                    "emailAddress":{
                        "name":"Megan Bowen",
                        "address":"MeganB@contoso.onmicrosoft.com"
                    }
                }
             ],
            "organizer":{
                "emailAddress":{
                    "name":"HR Taskforce",
                    "address":"HRTaskforce@contoso.onmicrosoft.com"
                }
            }
        },
        {
            "@odata.etag":"W/\"xPZF2y46pEiVBni87OnrpgAAFq78Xw==\"",
            "id":"AAMkAGI5MWYJOwAAEA==",
            "createdDateTime":"2017-07-31T18:59:01.982289Z",
            "lastModifiedDateTime":"2017-09-06T04:29:38.6647687Z",
            "changeKey":"xPZF2y46pEiVBni87OnrpgAAFq78Xw==",
            "categories":[

            ],
            "originalStartTimeZone":"Eastern Standard Time",
            "originalEndTimeZone":"Eastern Standard Time",
            "iCalUId":"040000008200E00074C5B7101A82E00807E10810824DDB122F0AD301000000000000000010000000824A8905B038D54AA7735F117B3442ED",
            "reminderMinutesBeforeStart":15,
            "isReminderOn":true,
            "hasAttachments":false,
            "subject":"New Training Plans",
            "bodyPreview":"Follow-up meeting to plan new trainings.\r\n\r\n\r\n\r\nJoin Microsoft Teams Online Meeting<https://teams.microsoft.com/l/meetup-join/19%3a900876baa3134907b0dcb41a0d220e31%40thread.skype/1501527539926?tenantId=dcd219dd-bc68-4b9b-bf0b-4a33a796be35>",
            "importance":"normal",
            "sensitivity":"normal",
            "isAllDay":false,
            "isCancelled":false,
            "isOrganizer":true,
            "responseRequested":true,
            "seriesMasterId":null,
            "showAs":"busy",
            "type":"singleInstance",
            "webLink":"https://outlook.office365.com/owa/?itemid=AAMkAGI5MWYJOwAAEA%3D%3D&exvsurl=1&path=/calendar/item",
            "onlineMeetingUrl":null,
            "responseStatus":{
                "response":"organizer",
                "time":"0001-01-01T00:00:00Z"
            },
            "body":{
                "contentType":"text",
                "content":"Meeting to plan new trainings.\r\n\r\n\r\n\r\nJoin Microsoft Teams Online Meeting<https://teams.microsoft.com/l/meetup-join/19%3a900876baa3134907b0dcb41a0d220e31%40thread.skype/1501527539926?tenantId=dcd219dd-bc68-4b9b-bf0b-4a33a796be35>\r\n"
            },
            "start":{
                "dateTime":"2017-08-16T21:00:00.0000000",
                "timeZone":"UTC"
            },
            "end":{
                "dateTime":"2017-08-16T22:00:00.0000000",
                "timeZone":"UTC"
            },
            "location":{
                "displayName":"HR Taskforce / Facilities"
            },
            "recurrence":null,
            "attendees":[
                {
                    "type":"required",
                    "status":{
                        "response":"none",
                        "time":"0001-01-01T00:00:00Z"
                    },
                    "emailAddress":{
                        "name":"HR Taskforce",
                        "address":"HRTaskforce@contoso.onmicrosoft.com"
                    }
                },
                {
                    "type":"required",
                    "status":{
                        "response":"none",
                        "time":"0001-01-01T00:00:00Z"
                    },
                    "emailAddress":{
                        "name":"Megan Bowen",
                        "address":"MeganB@contoso.onmicrosoft.com"
                    }
                }
            ],
            "organizer":{
                "emailAddress":{
                    "name":"HR Taskforce",
                    "address":"HRTaskforce@contoso.onmicrosoft.com"
                }
            }
        }
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List calendarView",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
