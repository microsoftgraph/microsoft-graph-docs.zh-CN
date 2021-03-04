---
title: 获取事件
description: 获取指定的 event 对象的属性和关系。
author: harini84
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 44007d0c4b8ad4feaf97cb3940fac388b9cca902
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50436230"
---
# <a name="get-event"></a><span data-ttu-id="f85ec-103">获取事件</span><span class="sxs-lookup"><span data-stu-id="f85ec-103">Get event</span></span>

<span data-ttu-id="f85ec-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f85ec-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f85ec-105">获取指定的 [event](../resources/event.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="f85ec-105">Get the properties and relationships of the specified [event](../resources/event.md) object.</span></span>

<span data-ttu-id="f85ec-106">如果：</span><span class="sxs-lookup"><span data-stu-id="f85ec-106">An app can get an event in another user's calendar if:</span></span>

* <span data-ttu-id="f85ec-107">应用具有应用程序权限</span><span class="sxs-lookup"><span data-stu-id="f85ec-107">The app has application permissions</span></span>
* <span data-ttu-id="f85ec-108">应用具有来自一个用户的适当委派[](#permissions)权限，另一个用户已与该用户共享日历，或已授予该用户委派访问权限。</span><span class="sxs-lookup"><span data-stu-id="f85ec-108">The app has the appropriate delegated [permissions](#permissions) from one user, and another user has shared a calendar with that user, or has given delegated access to that user.</span></span> <span data-ttu-id="f85ec-109">请参阅[详细信息和示例](/graph/outlook-get-shared-events-calendars)。</span><span class="sxs-lookup"><span data-stu-id="f85ec-109">See [details and an example](/graph/outlook-get-shared-events-calendars).</span></span>

<span data-ttu-id="f85ec-110">由于 **事件** 资源 [支持扩展](/graph/extensibility-overview)，因此您还可以使用该操作获取事件实例中的自定义属性 `GET` 和 **扩展** 数据。</span><span class="sxs-lookup"><span data-stu-id="f85ec-110">Because the **event** resource supports [extensions](/graph/extensibility-overview), you can also use the `GET` operation to get custom properties and extension data in an **event** instance.</span></span>


### <a name="support-various-time-zones"></a><span data-ttu-id="f85ec-111">支持不同时区</span><span class="sxs-lookup"><span data-stu-id="f85ec-111">Support various time zones</span></span>

<span data-ttu-id="f85ec-112">对于返回事件的所有 GET 操作，你可以使用 `Prefer: outlook.timezone` 标头在响应中指定事件开始和结束时间的时区。</span><span class="sxs-lookup"><span data-stu-id="f85ec-112">For all GET operations that return events, you can use the `Prefer: outlook.timezone` header to specify the time zone for the event start and end times in the response.</span></span> 

<span data-ttu-id="f85ec-113">例如，下面的 `Prefer: outlook.timezone` 标头将响应中的开始和结束时间设置为东部标准时间。</span><span class="sxs-lookup"><span data-stu-id="f85ec-113">For example, the following `Prefer: outlook.timezone` header sets the start and end times in the response to Eastern Standard Time.</span></span>
```http
Prefer: outlook.timezone="Eastern Standard Time"
```

<span data-ttu-id="f85ec-p102">如果该事件是在不同的时区中创建的，则根据 `Prefer` 标头中指定的时区调整开始和结束时间。请查看此 [列表](../resources/datetimetimezone.md) 了解支持的时区名称。如果未指定 `Prefer: outlook.timezone` 标头，则返回用 UTC 表示的开始和结束时间。</span><span class="sxs-lookup"><span data-stu-id="f85ec-p102">If the event was created in a different time zone, the start and end times will be adjusted to the time zone specified in that `Prefer` header. See this [list](../resources/datetimetimezone.md) for the supported time zone names. If the `Prefer: outlook.timezone` header is not specified, the start and end times are returned in UTC.</span></span>

<span data-ttu-id="f85ec-117">可以使用 **事件** 资源中的 **OriginalStartTimeZone** 和 **OriginalEndTimeZone** 属性来查找创建事件时使用的时区。</span><span class="sxs-lookup"><span data-stu-id="f85ec-117">You can use the **OriginalStartTimeZone** and **OriginalEndTimeZone** properties on the **event** resource to find out the time zone used when the event was created.</span></span>

## <a name="permissions"></a><span data-ttu-id="f85ec-118">权限</span><span class="sxs-lookup"><span data-stu-id="f85ec-118">Permissions</span></span>
<span data-ttu-id="f85ec-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f85ec-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f85ec-121">权限类型</span><span class="sxs-lookup"><span data-stu-id="f85ec-121">Permission type</span></span>      | <span data-ttu-id="f85ec-122">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f85ec-122">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f85ec-123">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f85ec-123">Delegated (work or school account)</span></span> | <span data-ttu-id="f85ec-124">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="f85ec-124">Calendars.Read</span></span>    |
|<span data-ttu-id="f85ec-125">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f85ec-125">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f85ec-126">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="f85ec-126">Calendars.Read</span></span>    |
|<span data-ttu-id="f85ec-127">应用程序</span><span class="sxs-lookup"><span data-stu-id="f85ec-127">Application</span></span> | <span data-ttu-id="f85ec-128">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="f85ec-128">Calendars.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="f85ec-129">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f85ec-129">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/events/{id}
GET /users/{id | userPrincipalName}/events/{id}
GET /groups/{id}/events/{id}

GET /me/calendar/events/{id}
GET /users/{id | userPrincipalName}/calendar/events/{id}
GET /groups/{id}/calendar/events/{id}

GET /me/calendars/{id}/events/{id}
GET /users/{id | userPrincipalName}/calendars/{id}/events/{id}

GET /me/calendargroups/{id}/calendars/{id}/events/{id}
GET /users/{id | userPrincipalName}/calendargroups/{id}/calendars/{id}/events/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="f85ec-130">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="f85ec-130">Optional query parameters</span></span>
<span data-ttu-id="f85ec-131">此方法支持使用 [OData 查询参数](/graph/query-parameters)来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="f85ec-131">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="f85ec-132">请求标头</span><span class="sxs-lookup"><span data-stu-id="f85ec-132">Request headers</span></span>
| <span data-ttu-id="f85ec-133">名称</span><span class="sxs-lookup"><span data-stu-id="f85ec-133">Name</span></span>       | <span data-ttu-id="f85ec-134">类型</span><span class="sxs-lookup"><span data-stu-id="f85ec-134">Type</span></span> | <span data-ttu-id="f85ec-135">说明</span><span class="sxs-lookup"><span data-stu-id="f85ec-135">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="f85ec-136">Authorization</span><span class="sxs-lookup"><span data-stu-id="f85ec-136">Authorization</span></span>  | <span data-ttu-id="f85ec-137">string</span><span class="sxs-lookup"><span data-stu-id="f85ec-137">string</span></span>  | <span data-ttu-id="f85ec-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="f85ec-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="f85ec-140">Prefer: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="f85ec-140">Prefer: outlook.timezone</span></span> | <span data-ttu-id="f85ec-141">string</span><span class="sxs-lookup"><span data-stu-id="f85ec-141">string</span></span> | <span data-ttu-id="f85ec-142">此选项可用于指定响应中开始时间和结束时间的时区。</span><span class="sxs-lookup"><span data-stu-id="f85ec-142">Use this to specify the time zone for start and end times in the response.</span></span> <span data-ttu-id="f85ec-143">如果未指定，返回的这些时间值采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="f85ec-143">If not specified, those time values are returned in UTC.</span></span> <span data-ttu-id="f85ec-144">可选。</span><span class="sxs-lookup"><span data-stu-id="f85ec-144">Optional.</span></span> |
| <span data-ttu-id="f85ec-145">Prefer: outlook.body-content-type</span><span class="sxs-lookup"><span data-stu-id="f85ec-145">Prefer: outlook.body-content-type</span></span> | <span data-ttu-id="f85ec-146">string</span><span class="sxs-lookup"><span data-stu-id="f85ec-146">string</span></span> | <span data-ttu-id="f85ec-147">要返回的 **body** 属性的格式。</span><span class="sxs-lookup"><span data-stu-id="f85ec-147">The format of the **body** property to be returned in.</span></span> <span data-ttu-id="f85ec-148">可取值为“text”或“html”。</span><span class="sxs-lookup"><span data-stu-id="f85ec-148">Values can be "text" or "html".</span></span> <span data-ttu-id="f85ec-149">如果指定此 `Preference-Applied` 头，返回 `Prefer` 头作为证明。</span><span class="sxs-lookup"><span data-stu-id="f85ec-149">A `Preference-Applied` header is returned as confirmation if this `Prefer` header is specified.</span></span> <span data-ttu-id="f85ec-150">如果未指定此头，采用 HTML 格式返回 **body** 属性。</span><span class="sxs-lookup"><span data-stu-id="f85ec-150">If the header is not specified, the **body** property is returned in HTML format.</span></span> <span data-ttu-id="f85ec-151">可选。</span><span class="sxs-lookup"><span data-stu-id="f85ec-151">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f85ec-152">请求正文</span><span class="sxs-lookup"><span data-stu-id="f85ec-152">Request body</span></span>
<span data-ttu-id="f85ec-153">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="f85ec-153">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f85ec-154">响应</span><span class="sxs-lookup"><span data-stu-id="f85ec-154">Response</span></span>

<span data-ttu-id="f85ec-155">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [event](../resources/event.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="f85ec-155">If successful, this method returns a `200 OK` response code and an [event](../resources/event.md) object in the response body.</span></span>
## <a name="examples"></a><span data-ttu-id="f85ec-156">示例</span><span class="sxs-lookup"><span data-stu-id="f85ec-156">Examples</span></span>

### <a name="example-1-get-a-specified-event"></a><span data-ttu-id="f85ec-157">示例 1：获取指定事件</span><span class="sxs-lookup"><span data-stu-id="f85ec-157">Example 1: Get a specified event</span></span>
#### <a name="request"></a><span data-ttu-id="f85ec-158">请求</span><span class="sxs-lookup"><span data-stu-id="f85ec-158">Request</span></span>
<span data-ttu-id="f85ec-159">以下示例获取指定的事件。</span><span class="sxs-lookup"><span data-stu-id="f85ec-159">The following example gets the specified event.</span></span> <span data-ttu-id="f85ec-160">它指定以下内容：</span><span class="sxs-lookup"><span data-stu-id="f85ec-160">It specifies the following:</span></span>

- <span data-ttu-id="f85ec-161">获取以太平洋标准时间格式返回的日期时间值的 `Prefer: outlook.timezone` 标头。</span><span class="sxs-lookup"><span data-stu-id="f85ec-161">A `Prefer: outlook.timezone` header to get date time values returned in Pacific Standard Time.</span></span> 
- <span data-ttu-id="f85ec-p108">返回特定属性的 `$select` 查询参数。如果没有 `$select` 参数，将返回所有事件属性。</span><span class="sxs-lookup"><span data-stu-id="f85ec-p108">A `$select` query parameter to return specific properties. Without a `$select` parameter, all of the event properties will be returned.</span></span>

<span data-ttu-id="f85ec-164">该请求未指定任何 `Prefer: outlook.body-content-type` 标头来指示返回的事件正文的特定格式。</span><span class="sxs-lookup"><span data-stu-id="f85ec-164">The request does not specify any `Prefer: outlook.body-content-type` header to indicate a specific format for the returned event body.</span></span> 


# <a name="http"></a>[<span data-ttu-id="f85ec-165">HTTP</span><span class="sxs-lookup"><span data-stu-id="f85ec-165">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_event"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/events/AAMkAGIAAAoZDOFAAA=/?$select=subject,body,bodyPreview,organizer,attendees,start,end,location,hideAttendees 
Prefer: outlook.timezone="Pacific Standard Time"
```
# <a name="c"></a>[<span data-ttu-id="f85ec-166">C#</span><span class="sxs-lookup"><span data-stu-id="f85ec-166">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-event-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f85ec-167">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f85ec-167">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-event-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f85ec-168">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f85ec-168">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-event-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f85ec-169">Java</span><span class="sxs-lookup"><span data-stu-id="f85ec-169">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-event-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="f85ec-170">响应</span><span class="sxs-lookup"><span data-stu-id="f85ec-170">Response</span></span>
<span data-ttu-id="f85ec-171">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="f85ec-171">Here is an example of the response.</span></span> <span data-ttu-id="f85ec-172">由于未指定任何 `Prefer: outlook.body-content-type` 标头，将以默认 HTML 格式返回 **body** 属性。</span><span class="sxs-lookup"><span data-stu-id="f85ec-172">Because no `Prefer: outlook.body-content-type` header was specified, the **body** property is returned in the default HTML format.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.event"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Preference-Applied: outlook.timezone="Pacific Standard Time"
Content-length: 1928

{
    "@odata.context":"https://graph.microsoft.com/beta/$metadata#users('cd209b0b-3f83-4c35-82d2-d88a61820480')/events(subject,body,bodyPreview,organizer,attendees,start,end,location,hideAttendees)/$entity",
    "@odata.etag":"W/\"ZlnW4RIAV06KYYwlrfNZvQAAKGWwbw==\"",
    "id":"AAMkAGIAAAoZDOFAAA=",
    "subject":"Orientation ",
    "bodyPreview":"Dana, this is the time you selected for our orientation. Please bring the notes I sent you.",
    "body":{
        "contentType":"html",
        "content":"<html><head></head><body><p>Dana, this is the time you selected for our orientation. Please bring the notes I sent you.</p></body></html>"
    },
    "start":{
        "dateTime":"2017-04-21T10:00:00.0000000",
        "timeZone":"Pacific Standard Time"
    },
    "end":{
        "dateTime":"2017-04-21T12:00:00.0000000",
        "timeZone":"Pacific Standard Time"
    },
    "location": {
        "displayName": "Assembly Hall",
        "locationType": "default",
        "uniqueId": "Assembly Hall",
        "uniqueIdType": "private"
    },
    "locations": [
        {
            "displayName": "Assembly Hall",
            "locationType": "default",
            "uniqueIdType": "unknown"
        }
    ],
    "attendees":[
        {
            "type":"required",
            "status":{
                "response":"none",
                "time":"0001-01-01T00:00:00Z"
            },
            "emailAddress":{
                "name":"Samantha Booth",
                "address":"samanthab@a830edad905084922E17020313.onmicrosoft.com"
            }
        },
        {
            "type":"required",
            "status":{
                "response":"tentativelyAccepted",
                "time":"0001-01-01T00:00:00Z"
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
            "emailAddress":{
                "name":"Dana Swope",
                "address":"danas@a830edad905084922E17020313.onmicrosoft.com"
            }
        }
    ],
    "hideAttendees": false,
    "organizer":{
        "emailAddress":{
            "name":"Samantha Booth",
            "address":"samanthab@a830edad905084922E17020313.onmicrosoft.com"
        }
    }
}
```
### <a name="example-2-get-the-body-property-in-text-format"></a><span data-ttu-id="f85ec-173">示例 2：获取文本格式的 body 属性</span><span class="sxs-lookup"><span data-stu-id="f85ec-173">Example 2: Get the body property in text format</span></span>
#### <a name="request"></a><span data-ttu-id="f85ec-174">请求</span><span class="sxs-lookup"><span data-stu-id="f85ec-174">Request</span></span>
<span data-ttu-id="f85ec-175">以下示例演示如何使用标头获取文本格式的 `Prefer: outlook.body-content-type="text"` 指定事件的 body属性。</span><span class="sxs-lookup"><span data-stu-id="f85ec-175">The following example shows how to use a `Prefer: outlook.body-content-type="text"` header to get the **body** property of the specified event in text format.</span></span>

<span data-ttu-id="f85ec-176">该请求还使用 `$select` 查询参数返回特定属性。</span><span class="sxs-lookup"><span data-stu-id="f85ec-176">The request also uses a `$select` query parameter to return specific properties.</span></span> <span data-ttu-id="f85ec-177">如果没有 `$select` 参数，将返回所有事件属性。</span><span class="sxs-lookup"><span data-stu-id="f85ec-177">Without a `$select` parameter, all of the event properties will be returned.</span></span>


# <a name="http"></a>[<span data-ttu-id="f85ec-178">HTTP</span><span class="sxs-lookup"><span data-stu-id="f85ec-178">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_event_in_text"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/events/AAMkAGI1AAAoZDOFAAA=/?$select=subject,body,bodyPreview
Prefer: outlook.body-content-type="text"
```
# <a name="c"></a>[<span data-ttu-id="f85ec-179">C#</span><span class="sxs-lookup"><span data-stu-id="f85ec-179">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-event-in-text-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f85ec-180">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f85ec-180">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-event-in-text-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f85ec-181">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f85ec-181">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-event-in-text-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f85ec-182">Java</span><span class="sxs-lookup"><span data-stu-id="f85ec-182">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-event-in-text-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="f85ec-183">响应</span><span class="sxs-lookup"><span data-stu-id="f85ec-183">Response</span></span>
<span data-ttu-id="f85ec-184">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="f85ec-184">Here is an example of the response.</span></span> <span data-ttu-id="f85ec-185">以文本格式返回 **body** 属性。</span><span class="sxs-lookup"><span data-stu-id="f85ec-185">The **body** property is returned in text format.</span></span> 

<!-- {
  "blockType": "response",
  "name": "get_event_in_text",
  "truncated": true,
  "@odata.type": "microsoft.graph.event"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Preference-Applied: outlook.body-content-type="text"
Content-length: 636

{
    "@odata.context":"https://graph.microsoft.com/beta/$metadata#users('cd209b0b-3f83-4c35-82d2-d88a61820480')/events(subject,body,bodyPreview)/$entity",
    "@odata.etag":"W/\"ZlnW4RIAV06KYYwlrfNZvQAAKGWwbw==\"",
    "id":"AAMkAGI1AAAoZDOFAAA=",
    "subject":"Orientation ",
    "bodyPreview":"Dana, this is the time you selected for our orientation. Please bring the notes I sent you.",
    "body":{
        "contentType":"text",
        "content":"Dana, this is the time you selected for our orientation. Please bring the notes I sent you.\r\n"
    }
}
```

### <a name="example-3-get-an-event-that-specifies-more-than-one-location"></a><span data-ttu-id="f85ec-186">示例 3：获取指定多个位置的事件</span><span class="sxs-lookup"><span data-stu-id="f85ec-186">Example 3: Get an event that specifies more than one location</span></span>
#### <a name="request"></a><span data-ttu-id="f85ec-187">请求</span><span class="sxs-lookup"><span data-stu-id="f85ec-187">Request</span></span>

<span data-ttu-id="f85ec-188">以下示例显示获取指定多个位置的事件。</span><span class="sxs-lookup"><span data-stu-id="f85ec-188">The following example shows getting an event that specifies more than one location.</span></span> <span data-ttu-id="f85ec-189">该请求指定返回特定属性的 `$select` 查询参数。</span><span class="sxs-lookup"><span data-stu-id="f85ec-189">The request specifies a `$select` query parameter to return specific properties.</span></span> 


# <a name="http"></a>[<span data-ttu-id="f85ec-190">HTTP</span><span class="sxs-lookup"><span data-stu-id="f85ec-190">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_event_multiple_locations"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/events/AAMkADAGAADDdm4NAAA=/?$select=subject,body,bodyPreview,organizer,attendees,start,end,location,locations
```
# <a name="c"></a>[<span data-ttu-id="f85ec-191">C#</span><span class="sxs-lookup"><span data-stu-id="f85ec-191">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-event-multiple-locations-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f85ec-192">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f85ec-192">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-event-multiple-locations-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f85ec-193">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f85ec-193">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-event-multiple-locations-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f85ec-194">Java</span><span class="sxs-lookup"><span data-stu-id="f85ec-194">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-event-multiple-locations-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="f85ec-195">响应</span><span class="sxs-lookup"><span data-stu-id="f85ec-195">Response</span></span>
<span data-ttu-id="f85ec-196">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="f85ec-196">Here is an example of the response.</span></span> <span data-ttu-id="f85ec-197">**locations** 属性包括组织事件的 3 个地点的详细信息。</span><span class="sxs-lookup"><span data-stu-id="f85ec-197">The **locations** property includes details for the 3 locations that the event is organized for.</span></span> 

<span data-ttu-id="f85ec-198">由于请求未指定任何或标头，因此起始和结束属性以默认的 UTC 时区显示，正文采用默认的 `Prefer: outlook.timezone` `Prefer: outlook.body-content-type` HTML 格式。  </span><span class="sxs-lookup"><span data-stu-id="f85ec-198">Because the request does not specify any `Prefer: outlook.timezone` or `Prefer: outlook.body-content-type` header, the **start** and **end** properties are displayed in the default UTC time zone, and the body is in the default HTML format.</span></span>  

<!-- {
  "blockType": "response",
  "name": "get_event_multiple_locations",
  "truncated": true,
  "@odata.type": "microsoft.graph.event"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 1992

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#users('d1a2fae9-db66-4cc9-8133-2184c77af1b8')/events(subject,body,bodyPreview,organizer,attendees,start,end,location,locations)/$entity",
  "@odata.etag":"W/\"y53lbKh6jkaxHzFwGhgyxgAAw5zhug==\"",
  "id":"AAMkADAGAADDdm4NAAA=",
  "subject":"Plan summer company picnic",
  "bodyPreview":"Let's kick-start this event planning!",
  "body":{
    "contentType":"html",
    "content":"<html>\r\n<head>\r\n</head>\r\n<body>\r\nLet's kick-start this event planning!\r\n</body>\r\n</html>\r\n"
  },
  "start":{
    "dateTime":"2017-08-30T11:00:00.0000000",
    "timeZone":"UTC"
  },
  "end":{
    "dateTime":"2017-08-30T12:00:00.0000000",
    "timeZone":"UTC"
  },
  "location":{
    "displayName":"Conf Room 3; Fourth Coffee; Home Office",
    "locationType":"default",
    "uniqueId":"Conf Room 3; Fourth Coffee; Home Office",
    "uniqueIdType":"private"
  },
  "locations":[
    {
      "displayName":"Conf Room 3",
      "locationType":"default",
      "uniqueIdType":"unknown"
    },
    {
      "displayName":"Fourth Coffee",
      "locationType":"default",
      "uniqueId":"Fourth Coffee",
      "uniqueIdType":"private",
      "address":{
        "type":"unknown",
        "street":"4567 Main St",
        "city":"Redmond",
        "state":"WA",
        "countryOrRegion":"US",
        "postalCode":"32008"
      },
      "coordinates":{
        "latitude":47.672,
        "longitude":-102.103
      }
    },
    {
      "displayName":"Home Office",
      "locationType":"default",
      "uniqueIdType":"unknown"
    }
  ],
  "attendees":[
    {
      "type":"required",
      "status":{
        "response":"none",
        "time":"0001-01-01T00:00:00Z"
      },
      "emailAddress":{
        "name":"Dana Swope",
        "address":"DanaS@contoso.onmicrosoft.com"
      }
    },
    {
      "type":"required",
      "status":{
        "response":"none",
        "time":"0001-01-01T00:00:00Z"
      },
      "emailAddress":{
        "name":"Alex Wilber",
        "address":"AlexW@contoso.onmicrosoft.com"
      }
    }
  ],
  "organizer":{
    "emailAddress":{
      "name":"Adele Vance",
      "address":"AdeleV@contoso.onmicrosoft.com"
    }
  }
}
```
### <a name="example-4-expand-a-series-master-event"></a><span data-ttu-id="f85ec-199">示例 4：展开系列主事件</span><span class="sxs-lookup"><span data-stu-id="f85ec-199">Example 4: Expand a series master event</span></span>
#### <a name="request"></a><span data-ttu-id="f85ec-200">请求</span><span class="sxs-lookup"><span data-stu-id="f85ec-200">Request</span></span>

<span data-ttu-id="f85ec-201">以下示例显示展开定期系列的系列主事件（发生异常和已取消）。</span><span class="sxs-lookup"><span data-stu-id="f85ec-201">The following example shows expanding a series master event of a recurring series with exceptions and cancelled occurences.</span></span> <span data-ttu-id="f85ec-202">该请求指定返回特定属性的 `$select` 查询参数。</span><span class="sxs-lookup"><span data-stu-id="f85ec-202">The request specifies a `$select` query parameter to return specific properties.</span></span> 

<!-- {
  "blockType": "request",
  "name": "get_event_seriesMaster_expansion"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/events/AAMkADAGAADDdm4NAAA=/?$select=subject,start,end,occurrenceId,exceptionOccurrences,cancelledOccurrences$expand=exceptionOccurrences
```
#### <a name="response"></a><span data-ttu-id="f85ec-203">响应</span><span class="sxs-lookup"><span data-stu-id="f85ec-203">Response</span></span>
<span data-ttu-id="f85ec-204">GET 操作返回系列主事件的选定属性。</span><span class="sxs-lookup"><span data-stu-id="f85ec-204">The GET operation returns the selected properties for the series master event.</span></span> <span data-ttu-id="f85ec-205">具体而言，对于 **exceptionOccurrences** 集合中的事件，操作返回 **id** 属性，以及 (**subject、start、end** **、occurrenceId**) 。  </span><span class="sxs-lookup"><span data-stu-id="f85ec-205">Specifically, for events in the **exceptionOccurrences** collection, the operation returns the **id** property, and the applicable, selected properties (**subject**, **start**, **end**, **occurrenceId**).</span></span> <span data-ttu-id="f85ec-206">对于 **cancelledOccurrences** 集合中的事件，由于事件不再存在，因此操作仅返回 **其 occurrenceId** 属性值。</span><span class="sxs-lookup"><span data-stu-id="f85ec-206">As for events in the **cancelledOccurrences** collection, because the events no longer exist, the operation returns only their **occurrenceId** property values.</span></span>

<!-- {
  "blockType": "response",
  "name": "get_event_seriesMaster_expansion",
  "truncated": true,
  "@odata.type": "microsoft.graph.event"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 1992

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#users('d1a2fae9-db66-4cc9-8133-2184c77af1b8')/events(subject,start,end,occurrenceId,exceptionOccurrences,cancelledOccurrences)/$entity",
  "@odata.etag":"W/\"y53lbKh6jkaxHzFwGhgyxgAAw5zhug==\"",
  "id":"AAMkADAGAADDdm4NAAA=",
  "subject": "Daily stand-up",
  "cancelledOccurrences": [
     "OID.AAMkADAGAADDdm4NAAA=.2020-04-30",
     "OID.AAMkADAGAADDdm4NAAA=.2020-05-07",
     "OID.AAMkADAGAADDdm4NAAA=.2020-05-14"
    ],
  "occurrenceId": null,
    "start": {
        "dateTime": "2020-04-23T11:30:00.0000000",
        "timeZone": "UTC"
    },
  "end": {
        "dateTime": "2020-04-23T12:00:00.0000000",
        "timeZone": "UTC"
    },
  "exceptionOccurrences": [
        {
            "id": "AAMkADM0ZGRhMjdjLTA==",
            "Subject": "SM update 24",
            "occurrenceId": "OID.AAMkADAGAADDdm4NAAA=.2020-05-21",
            "start": {
                "dateTime": "2020-05-21T11:30:00.0000000",
                "timeZone": "UTC"
            },
            "end": {
                "dateTime": "2020-05-21T12:00:00.0000000",
                "timeZone": "UTC"
            }
        }
    ]
}
```

## <a name="see-also"></a><span data-ttu-id="f85ec-207">另请参阅</span><span class="sxs-lookup"><span data-stu-id="f85ec-207">See also</span></span>

- [<span data-ttu-id="f85ec-208">使用扩展向资源添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="f85ec-208">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="f85ec-209">使用开放扩展向用户添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="f85ec-209">Add custom data to users using open extensions</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="f85ec-210">使用架构扩展向组添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="f85ec-210">Add custom data to groups using schema extensions</span></span>](/graph/extensibility-schema-groups)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get event",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


