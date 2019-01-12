---
title: 列出 calendarView
description: 从群组的默认日历中，获取由时间范围定义的日历视图中的事件发生次数、异常和单个实例。
localization_priority: Normal
author: dkershaw10
ms.prod: groups
ms.openlocfilehash: c543526ce8c5bd1b8d0da2bf3d60a50f1437f118
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27931298"
---
# <a name="list-calendarview"></a><span data-ttu-id="903fa-103">列出 calendarView</span><span class="sxs-lookup"><span data-stu-id="903fa-103">List calendarView</span></span>

> <span data-ttu-id="903fa-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="903fa-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="903fa-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="903fa-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="903fa-106">从群组的默认日历中，获取由时间范围定义的日历视图中的事件发生次数、异常和单个实例。</span><span class="sxs-lookup"><span data-stu-id="903fa-106">Get the occurrences, exceptions, and single instances of events in a calendar view defined by a time range, from the default calendar of a group.</span></span>

## <a name="permissions"></a><span data-ttu-id="903fa-107">权限</span><span class="sxs-lookup"><span data-stu-id="903fa-107">Permissions</span></span>
<span data-ttu-id="903fa-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="903fa-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="903fa-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="903fa-110">Permission type</span></span>      | <span data-ttu-id="903fa-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="903fa-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="903fa-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="903fa-112">Delegated (work or school account)</span></span> | <span data-ttu-id="903fa-113">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="903fa-113">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="903fa-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="903fa-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="903fa-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="903fa-115">Not supported.</span></span>    |
|<span data-ttu-id="903fa-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="903fa-116">Application</span></span> | <span data-ttu-id="903fa-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="903fa-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="903fa-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="903fa-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
```

## <a name="query-parameters"></a><span data-ttu-id="903fa-119">查询参数</span><span class="sxs-lookup"><span data-stu-id="903fa-119">Query parameters</span></span>
<span data-ttu-id="903fa-120">在请求 URL 中，提供以下必要查询参数的值。</span><span class="sxs-lookup"><span data-stu-id="903fa-120">In the request URL, provide the following required query parameters with values.</span></span>

| <span data-ttu-id="903fa-121">参数</span><span class="sxs-lookup"><span data-stu-id="903fa-121">Parameter</span></span>    | <span data-ttu-id="903fa-122">类型</span><span class="sxs-lookup"><span data-stu-id="903fa-122">Type</span></span>   |<span data-ttu-id="903fa-123">说明</span><span class="sxs-lookup"><span data-stu-id="903fa-123">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="903fa-124">startDateTime</span><span class="sxs-lookup"><span data-stu-id="903fa-124">startDateTime</span></span>|<span data-ttu-id="903fa-125">字符串</span><span class="sxs-lookup"><span data-stu-id="903fa-125">String</span></span>|<span data-ttu-id="903fa-p103">时间范围的开始日期和时间以 ISO 8601 格式表示。例如，“2015-11-08T19:00:00.0000000”。</span><span class="sxs-lookup"><span data-stu-id="903fa-p103">The start date and time of the time range, represented in ISO 8601 format. For example, "2015-11-08T19:00:00.0000000".</span></span>|
|<span data-ttu-id="903fa-128">endDateTime</span><span class="sxs-lookup"><span data-stu-id="903fa-128">endDateTime</span></span>|<span data-ttu-id="903fa-129">字符串</span><span class="sxs-lookup"><span data-stu-id="903fa-129">String</span></span>|<span data-ttu-id="903fa-p104">时间范围的结束日期和时间以 ISO 8601 格式表示。例如，“2015-11-08T20:00:00.0000000”。</span><span class="sxs-lookup"><span data-stu-id="903fa-p104">The end date and time of the time range, represented in ISO 8601 format. For example, "2015-11-08T20:00:00.0000000".</span></span>|

<span data-ttu-id="903fa-132">此方法还支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="903fa-132">This method also supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="903fa-133">请求标头</span><span class="sxs-lookup"><span data-stu-id="903fa-133">Request headers</span></span>
| <span data-ttu-id="903fa-134">名称</span><span class="sxs-lookup"><span data-stu-id="903fa-134">Name</span></span>       | <span data-ttu-id="903fa-135">类型</span><span class="sxs-lookup"><span data-stu-id="903fa-135">Type</span></span> | <span data-ttu-id="903fa-136">说明</span><span class="sxs-lookup"><span data-stu-id="903fa-136">Description</span></span> |
|:---------------|:--------|:--------|
| <span data-ttu-id="903fa-137">Authorization</span><span class="sxs-lookup"><span data-stu-id="903fa-137">Authorization</span></span>  | <span data-ttu-id="903fa-138">string</span><span class="sxs-lookup"><span data-stu-id="903fa-138">string</span></span> | <span data-ttu-id="903fa-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="903fa-p105">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="903fa-141">Prefer: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="903fa-141">Prefer: outlook.timezone</span></span>  | <span data-ttu-id="903fa-142">string</span><span class="sxs-lookup"><span data-stu-id="903fa-142">string</span></span> | <span data-ttu-id="903fa-143">此选项可用于指定响应中开始时间和结束时间的时区。</span><span class="sxs-lookup"><span data-stu-id="903fa-143">Use this to specify the time zone for start and end times in the response.</span></span> <span data-ttu-id="903fa-144">如果未指定，返回的这些时间值采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="903fa-144">If not specified, those time values are returned in UTC.</span></span> <span data-ttu-id="903fa-145">可选。</span><span class="sxs-lookup"><span data-stu-id="903fa-145">Optional.</span></span> |
| <span data-ttu-id="903fa-146">Prefer: outlook.body-content-type</span><span class="sxs-lookup"><span data-stu-id="903fa-146">Prefer: outlook.body-content-type</span></span> | <span data-ttu-id="903fa-147">string</span><span class="sxs-lookup"><span data-stu-id="903fa-147">string</span></span> | <span data-ttu-id="903fa-148">要返回的 **body** 属性的格式。</span><span class="sxs-lookup"><span data-stu-id="903fa-148">The format of the **body** property to be returned in.</span></span> <span data-ttu-id="903fa-149">可取值为“text”或“html”。</span><span class="sxs-lookup"><span data-stu-id="903fa-149">Values can be "text" or "html".</span></span> <span data-ttu-id="903fa-150">如果指定此 `Preference-Applied` 头，返回 `Prefer` 头作为证明。</span><span class="sxs-lookup"><span data-stu-id="903fa-150">A `Preference-Applied` header is returned as confirmation if this `Prefer` header is specified.</span></span> <span data-ttu-id="903fa-151">如果未指定此头，采用 HTML 格式返回 **body** 属性。</span><span class="sxs-lookup"><span data-stu-id="903fa-151">If the header is not specified, the **body** property is returned in HTML format.</span></span> <span data-ttu-id="903fa-152">可选。</span><span class="sxs-lookup"><span data-stu-id="903fa-152">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="903fa-153">请求正文</span><span class="sxs-lookup"><span data-stu-id="903fa-153">Request body</span></span>
<span data-ttu-id="903fa-154">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="903fa-154">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="903fa-155">响应</span><span class="sxs-lookup"><span data-stu-id="903fa-155">Response</span></span>
<span data-ttu-id="903fa-156">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [event](../resources/event.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="903fa-156">If successful, this method returns a `200 OK` response code and collection of [event](../resources/event.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="903fa-157">示例</span><span class="sxs-lookup"><span data-stu-id="903fa-157">Example</span></span>
#### <a name="request"></a><span data-ttu-id="903fa-158">请求</span><span class="sxs-lookup"><span data-stu-id="903fa-158">Request</span></span>
<span data-ttu-id="903fa-159">下面的示例展示了如何请求采用文本格式返回事件主体。</span><span class="sxs-lookup"><span data-stu-id="903fa-159">The following example requests event bodies to be returned in text format.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_calendarviews"
}-->
```http
GET https://graph.microsoft.com/beta/groups/02bd9fd6-8f93-4758-87c3-1fb73740a315/calendarView?startDateTime=2017-01-01T19:00:00.0000000&endDateTime=2017-10-01T19:00:00.00
Prefer: outlook.body-content-type="text"
```

#### <a name="response"></a><span data-ttu-id="903fa-160">响应</span><span class="sxs-lookup"><span data-stu-id="903fa-160">Response</span></span>
<span data-ttu-id="903fa-161">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="903fa-161">The following is an example of the response.</span></span>
><span data-ttu-id="903fa-162">**注意：** 可能为便于阅读缩短如下所示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="903fa-162">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="903fa-163">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="903fa-163">All the properties will be returned from an actual call.</span></span>
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
    "@odata.context":"https://graph.microsoft.com/beta/$metadata#groups('02bd9fd6-8f93-4758-87c3-1fb73740a315')/calendarView",
    "@odata.nextLink":"https://graph.microsoft.com/beta/groups/02bd9fd6-8f93-4758-87c3-1fb73740a315/calendarView?startDateTime=2017-01-01T19%3a00%3a00.0000000&endDateTime=2017-10-01T19%3a00%3a00.00&$skip=10",
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
            "uid":"040000008200E00074C5B7101A82E00807E1080E824DDB122F0AD301000000000000000010000000824A8905B038D54AA7735F117B3442ED",
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
            "uid":"040000008200E00074C5B7101A82E00807E10810824DDB122F0AD301000000000000000010000000824A8905B038D54AA7735F117B3442ED",
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
