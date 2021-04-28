---
title: 列出 calendarView
description: 获取由时间范围定义的日历视图中的事件发生次数、异常和单个实例，
localization_priority: Normal
author: yyuank
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 8c0eb3dc633c11e47cca189d449e46923d30a4d2
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52052339"
---
# <a name="list-calendarview"></a><span data-ttu-id="37eae-103">列出 calendarView</span><span class="sxs-lookup"><span data-stu-id="37eae-103">List calendarView</span></span>

<span data-ttu-id="37eae-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="37eae-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="37eae-105">从群组的默认日历中，获取由时间范围定义的日历视图中的事件发生次数、异常和单个实例。</span><span class="sxs-lookup"><span data-stu-id="37eae-105">Get the occurrences, exceptions, and single instances of events in a calendar view defined by a time range, from the default calendar of a group.</span></span>

## <a name="permissions"></a><span data-ttu-id="37eae-106">权限</span><span class="sxs-lookup"><span data-stu-id="37eae-106">Permissions</span></span>
<span data-ttu-id="37eae-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="37eae-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="37eae-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="37eae-109">Permission type</span></span>      | <span data-ttu-id="37eae-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="37eae-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="37eae-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="37eae-111">Delegated (work or school account)</span></span> | <span data-ttu-id="37eae-112">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="37eae-112">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="37eae-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="37eae-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="37eae-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="37eae-114">Not supported.</span></span>    |
|<span data-ttu-id="37eae-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="37eae-115">Application</span></span> | <span data-ttu-id="37eae-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="37eae-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="37eae-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="37eae-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
```

## <a name="query-parameters"></a><span data-ttu-id="37eae-118">查询参数</span><span class="sxs-lookup"><span data-stu-id="37eae-118">Query parameters</span></span>
<span data-ttu-id="37eae-119">在请求 URL 中，提供以下必要查询参数的值。</span><span class="sxs-lookup"><span data-stu-id="37eae-119">In the request URL, provide the following required query parameters with values.</span></span>

| <span data-ttu-id="37eae-120">参数</span><span class="sxs-lookup"><span data-stu-id="37eae-120">Parameter</span></span>     | <span data-ttu-id="37eae-121">类型</span><span class="sxs-lookup"><span data-stu-id="37eae-121">Type</span></span>   | <span data-ttu-id="37eae-122">说明</span><span class="sxs-lookup"><span data-stu-id="37eae-122">Description</span></span>                                                                                                            |
|:--------------|:-------|:-----------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="37eae-123">startDateTime</span><span class="sxs-lookup"><span data-stu-id="37eae-123">startDateTime</span></span> | <span data-ttu-id="37eae-124">String</span><span class="sxs-lookup"><span data-stu-id="37eae-124">String</span></span> | <span data-ttu-id="37eae-p102">时间范围的开始日期和时间，以 ISO 8601 格式表示。例如，“2019-11-08T19:00:00-08:00”。</span><span class="sxs-lookup"><span data-stu-id="37eae-p102">The start date and time of the time range, represented in ISO 8601 format. For example, "2019-11-08T19:00:00-08:00".</span></span> |
| <span data-ttu-id="37eae-127">endDateTime</span><span class="sxs-lookup"><span data-stu-id="37eae-127">endDateTime</span></span>   | <span data-ttu-id="37eae-128">String</span><span class="sxs-lookup"><span data-stu-id="37eae-128">String</span></span> | <span data-ttu-id="37eae-p103">时间范围的结束日期和时间，以 ISO 8601 格式表示。例如，“2019-11-08T20:00:00-08:00”。</span><span class="sxs-lookup"><span data-stu-id="37eae-p103">The end date and time of the time range, represented in ISO 8601 format. For example, "2019-11-08T20:00:00-08:00".</span></span>   |

<span data-ttu-id="37eae-131">`startDateTime` 和 `endDateTime` 的值使用值中指定的时区偏移量进行解释，并且不受 `Prefer: outlook.timezone` 标头（若有）的值影响。</span><span class="sxs-lookup"><span data-stu-id="37eae-131">The values of `startDateTime` and `endDateTime` are interpreted using the timezone offset specified in the value and are not impacted by the value of the `Prefer: outlook.timezone` header if present.</span></span> <span data-ttu-id="37eae-132">如果值中未包含时区偏移量，则将其解释为 UTC。</span><span class="sxs-lookup"><span data-stu-id="37eae-132">If no timezone offset is included in the value, it is interpreted as UTC.</span></span>

<span data-ttu-id="37eae-133">此方法还支持一些 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="37eae-133">This method also supports some of the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

> [!NOTE]
> <span data-ttu-id="37eae-134">[事件](../resources/event.md)的 **createdDateTime** 和 **lastModifiedDateTime** 属性不支持 `$select`。</span><span class="sxs-lookup"><span data-stu-id="37eae-134">The **createdDateTime** and **lastModifiedDateTime** properties of [event](../resources/event.md) do not support `$select`.</span></span> <span data-ttu-id="37eae-135">若要获取它们的值，只需在 **calendarView** 上进行查询，而不应用 `$select`。</span><span class="sxs-lookup"><span data-stu-id="37eae-135">To get their values, simply query on **calendarView** without applying `$select`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="37eae-136">请求标头</span><span class="sxs-lookup"><span data-stu-id="37eae-136">Request headers</span></span>
| <span data-ttu-id="37eae-137">名称</span><span class="sxs-lookup"><span data-stu-id="37eae-137">Name</span></span>       | <span data-ttu-id="37eae-138">类型</span><span class="sxs-lookup"><span data-stu-id="37eae-138">Type</span></span> | <span data-ttu-id="37eae-139">说明</span><span class="sxs-lookup"><span data-stu-id="37eae-139">Description</span></span> |
|:---------------|:--------|:--------|
| <span data-ttu-id="37eae-140">Authorization</span><span class="sxs-lookup"><span data-stu-id="37eae-140">Authorization</span></span>  | <span data-ttu-id="37eae-141">string</span><span class="sxs-lookup"><span data-stu-id="37eae-141">string</span></span> | <span data-ttu-id="37eae-p106">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="37eae-p106">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="37eae-144">Prefer: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="37eae-144">Prefer: outlook.timezone</span></span>  | <span data-ttu-id="37eae-145">string</span><span class="sxs-lookup"><span data-stu-id="37eae-145">string</span></span> | <span data-ttu-id="37eae-146">此选项可用于指定响应中开始时间和结束时间的时区。</span><span class="sxs-lookup"><span data-stu-id="37eae-146">Use this to specify the time zone for start and end times in the response.</span></span> <span data-ttu-id="37eae-147">如果未指定，返回的这些时间值采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="37eae-147">If not specified, those time values are returned in UTC.</span></span> <span data-ttu-id="37eae-148">可选。</span><span class="sxs-lookup"><span data-stu-id="37eae-148">Optional.</span></span> |
| <span data-ttu-id="37eae-149">Prefer: outlook.body-content-type</span><span class="sxs-lookup"><span data-stu-id="37eae-149">Prefer: outlook.body-content-type</span></span> | <span data-ttu-id="37eae-150">string</span><span class="sxs-lookup"><span data-stu-id="37eae-150">string</span></span> | <span data-ttu-id="37eae-151">要返回的 **body** 属性的格式。</span><span class="sxs-lookup"><span data-stu-id="37eae-151">The format of the **body** property to be returned in.</span></span> <span data-ttu-id="37eae-152">可取值为“text”或“html”。</span><span class="sxs-lookup"><span data-stu-id="37eae-152">Values can be "text" or "html".</span></span> <span data-ttu-id="37eae-153">如果指定此 `Preference-Applied` 头，返回 `Prefer` 头作为证明。</span><span class="sxs-lookup"><span data-stu-id="37eae-153">A `Preference-Applied` header is returned as confirmation if this `Prefer` header is specified.</span></span> <span data-ttu-id="37eae-154">如果未指定此头，采用 HTML 格式返回 **body** 属性。</span><span class="sxs-lookup"><span data-stu-id="37eae-154">If the header is not specified, the **body** property is returned in HTML format.</span></span> <span data-ttu-id="37eae-155">可选。</span><span class="sxs-lookup"><span data-stu-id="37eae-155">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="37eae-156">请求正文</span><span class="sxs-lookup"><span data-stu-id="37eae-156">Request body</span></span>
<span data-ttu-id="37eae-157">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="37eae-157">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="37eae-158">响应</span><span class="sxs-lookup"><span data-stu-id="37eae-158">Response</span></span>
<span data-ttu-id="37eae-159">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [event](../resources/event.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="37eae-159">If successful, this method returns a `200 OK` response code and collection of [event](../resources/event.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="37eae-160">示例</span><span class="sxs-lookup"><span data-stu-id="37eae-160">Example</span></span>
#### <a name="request"></a><span data-ttu-id="37eae-161">请求</span><span class="sxs-lookup"><span data-stu-id="37eae-161">Request</span></span>
<span data-ttu-id="37eae-162">下面的示例展示了如何请求采用文本格式返回事件主体。</span><span class="sxs-lookup"><span data-stu-id="37eae-162">The following example requests event bodies to be returned in text format.</span></span>

# <a name="http"></a>[<span data-ttu-id="37eae-163">HTTP</span><span class="sxs-lookup"><span data-stu-id="37eae-163">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["02bd9fd6-8f93-4758-87c3-1fb73740a315"],
  "name": "group_get_calendarview"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groups/02bd9fd6-8f93-4758-87c3-1fb73740a315/calendarView?startDateTime=2017-01-01T19:00:00-08:00&endDateTime=2017-10-01T19:00:00.00-08:00
Prefer: outlook.body-content-type="text"
```
# <a name="c"></a>[<span data-ttu-id="37eae-164">C#</span><span class="sxs-lookup"><span data-stu-id="37eae-164">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-get-calendarview-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="37eae-165">JavaScript</span><span class="sxs-lookup"><span data-stu-id="37eae-165">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-get-calendarview-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="37eae-166">Objective-C</span><span class="sxs-lookup"><span data-stu-id="37eae-166">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-get-calendarview-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="37eae-167">Java</span><span class="sxs-lookup"><span data-stu-id="37eae-167">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/group-get-calendarview-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="37eae-168">响应</span><span class="sxs-lookup"><span data-stu-id="37eae-168">Response</span></span>
<span data-ttu-id="37eae-169">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="37eae-169">The following is an example of the response.</span></span>
><span data-ttu-id="37eae-170">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="37eae-170">**Note:** The response object shown here might be shortened for readability.</span></span>
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
  "tocPath": "",
  "suppressions": [
  ]
}-->
