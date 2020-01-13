---
title: 列出 calendarView
description: '从用户的默认日历中，获取由时间范围定义的日历视图中的事件发生次数、异常和单个实例， '
localization_priority: Priority
doc_type: apiPageType
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 9cbb8c31605ac389fb4e9607795ca5108f50a1f3
ms.sourcegitcommit: 2a601cffdb8df375b2ee32a1f35b8f71e0ffd04f
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2020
ms.locfileid: "41023143"
---
# <a name="list-calendarview"></a><span data-ttu-id="0ace2-103">列出 calendarView</span><span class="sxs-lookup"><span data-stu-id="0ace2-103">List calendarView</span></span>

<span data-ttu-id="0ace2-104">从用户的默认日历或其他一些日历中，获取由时间范围定义的日历视图中的事件发生次数、异常和单个实例。</span><span class="sxs-lookup"><span data-stu-id="0ace2-104">Get the occurrences, exceptions, and single instances of events in a calendar view defined by a time range, from the user's default calendar, or from some other calendar of the user's.</span></span>
## <a name="permissions"></a><span data-ttu-id="0ace2-105">权限</span><span class="sxs-lookup"><span data-stu-id="0ace2-105">Permissions</span></span>
<span data-ttu-id="0ace2-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0ace2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0ace2-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="0ace2-108">Permission type</span></span>      | <span data-ttu-id="0ace2-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="0ace2-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0ace2-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0ace2-110">Delegated (work or school account)</span></span> | <span data-ttu-id="0ace2-111">Calendars.Read、Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0ace2-111">Calendars.Read, Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="0ace2-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0ace2-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0ace2-113">Calendars.Read、Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0ace2-113">Calendars.Read, Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="0ace2-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="0ace2-114">Application</span></span> | <span data-ttu-id="0ace2-115">Calendars.Read、Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0ace2-115">Calendars.Read, Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="0ace2-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0ace2-116">HTTP request</span></span>

<span data-ttu-id="0ace2-117">用户的默认 [calendar](../resources/calendar.md)。</span><span class="sxs-lookup"><span data-stu-id="0ace2-117">A user's default [calendar](../resources/calendar.md).</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/calendar/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
```

<span data-ttu-id="0ace2-118">默认 [calendarGroup](../resources/calendargroup.md) 中的用户 [calendar](../resources/calendar.md)。</span><span class="sxs-lookup"><span data-stu-id="0ace2-118">A user's [calendar](../resources/calendar.md) in the default [calendarGroup](../resources/calendargroup.md).</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}

GET /me/calendarGroup/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendarGroup/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
```

<span data-ttu-id="0ace2-119">指定 [calendarGroup](../resources/calendargroup.md) 中用户的 [日历](../resources/calendar.md)。</span><span class="sxs-lookup"><span data-stu-id="0ace2-119">A user's [calendar](../resources/calendar.md) in a specific [calendarGroup](../resources/calendargroup.md).</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/calendarGroups/{id}/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendarGroups/{id}/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
```

## <a name="query-parameters"></a><span data-ttu-id="0ace2-120">查询参数</span><span class="sxs-lookup"><span data-stu-id="0ace2-120">Query parameters</span></span>

<span data-ttu-id="0ace2-121">在请求 URL 中，提供以下必要查询参数的值。</span><span class="sxs-lookup"><span data-stu-id="0ace2-121">In the request URL, provide the following required query parameters with values.</span></span>

| <span data-ttu-id="0ace2-122">参数</span><span class="sxs-lookup"><span data-stu-id="0ace2-122">Parameter</span></span>     | <span data-ttu-id="0ace2-123">类型</span><span class="sxs-lookup"><span data-stu-id="0ace2-123">Type</span></span>   | <span data-ttu-id="0ace2-124">说明</span><span class="sxs-lookup"><span data-stu-id="0ace2-124">Description</span></span>                                                                                                            |
|:--------------|:-------|:-----------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="0ace2-125">startDateTime</span><span class="sxs-lookup"><span data-stu-id="0ace2-125">startDateTime</span></span> | <span data-ttu-id="0ace2-126">String</span><span class="sxs-lookup"><span data-stu-id="0ace2-126">String</span></span> | <span data-ttu-id="0ace2-p102">时间范围的开始日期和时间，以 ISO 8601 格式表示。例如，“2019-11-08T19:00:00-08:00”。</span><span class="sxs-lookup"><span data-stu-id="0ace2-p102">The start date and time of the time range, represented in ISO 8601 format. For example, "2015-11-08T19:00:00.0000000".</span></span> |
| <span data-ttu-id="0ace2-129">endDateTime</span><span class="sxs-lookup"><span data-stu-id="0ace2-129">endDateTime</span></span>   | <span data-ttu-id="0ace2-130">String</span><span class="sxs-lookup"><span data-stu-id="0ace2-130">String</span></span> | <span data-ttu-id="0ace2-p103">时间范围的结束日期和时间，以 ISO 8601 格式表示。例如，“2019-11-08T20:00:00-08:00”。</span><span class="sxs-lookup"><span data-stu-id="0ace2-p103">The end date and time of the time range, represented in ISO 8601 format. For example, "2015-11-08T20:00:00.0000000".</span></span>   |

<span data-ttu-id="0ace2-133">`startDateTime` 和 `endDateTime` 的值使用值中指定的时区偏移量进行解释，并且不受 `Prefer: outlook.timezone` 标头（若有）的值影响。</span><span class="sxs-lookup"><span data-stu-id="0ace2-133">The values of `startDateTime` and `endDateTime` are interpreted using the timezone offset specified in the value and are not impacted by the value of the `Prefer: outlook.timezone` header if present.</span></span> <span data-ttu-id="0ace2-134">如果值中未包含时区偏移量，则将其解释为 UTC。</span><span class="sxs-lookup"><span data-stu-id="0ace2-134">If no timezone offset is included in the value, it is interpreted as UTC.</span></span>

<span data-ttu-id="0ace2-135">此方法还支持一些 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="0ace2-135">This method also supports some of the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

> [!NOTE]
> <span data-ttu-id="0ace2-136">[事件](../resources/event.md)的 **createdDateTime** 和 **lastModifiedDateTime** 属性不支持 `$select`。</span><span class="sxs-lookup"><span data-stu-id="0ace2-136">The **createdDateTime** and **lastModifiedDateTime** properties of [event](../resources/event.md) do not support `$select`.</span></span> <span data-ttu-id="0ace2-137">若要获取它们的值，只需在 **calendarView** 上进行查询，而不应用 `$select`。</span><span class="sxs-lookup"><span data-stu-id="0ace2-137">To get their values, simply query on **calendarView** without applying `$select`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0ace2-138">请求标头</span><span class="sxs-lookup"><span data-stu-id="0ace2-138">Request headers</span></span>
| <span data-ttu-id="0ace2-139">名称</span><span class="sxs-lookup"><span data-stu-id="0ace2-139">Name</span></span>       | <span data-ttu-id="0ace2-140">类型</span><span class="sxs-lookup"><span data-stu-id="0ace2-140">Type</span></span> | <span data-ttu-id="0ace2-141">说明</span><span class="sxs-lookup"><span data-stu-id="0ace2-141">Description</span></span> |
|:---------------|:--------|:--------|
| <span data-ttu-id="0ace2-142">Authorization</span><span class="sxs-lookup"><span data-stu-id="0ace2-142">Authorization</span></span>  | <span data-ttu-id="0ace2-143">string</span><span class="sxs-lookup"><span data-stu-id="0ace2-143">string</span></span> | <span data-ttu-id="0ace2-p106">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="0ace2-p106">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="0ace2-146">Prefer: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="0ace2-146">Prefer: outlook.timezone</span></span>  | <span data-ttu-id="0ace2-147">string</span><span class="sxs-lookup"><span data-stu-id="0ace2-147">string</span></span> | <span data-ttu-id="0ace2-148">此选项可用于指定响应中开始时间和结束时间的时区。</span><span class="sxs-lookup"><span data-stu-id="0ace2-148">Use this to specify the time zone for start and end times in the response.</span></span> <span data-ttu-id="0ace2-149">如果未指定，返回的这些时间值采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="0ace2-149">If not specified, those time values are returned in UTC.</span></span> <span data-ttu-id="0ace2-150">可选。</span><span class="sxs-lookup"><span data-stu-id="0ace2-150">Optional.</span></span> |
| <span data-ttu-id="0ace2-151">Prefer: outlook.body-content-type</span><span class="sxs-lookup"><span data-stu-id="0ace2-151">Prefer: outlook.body-content-type</span></span> | <span data-ttu-id="0ace2-152">string</span><span class="sxs-lookup"><span data-stu-id="0ace2-152">string</span></span> | <span data-ttu-id="0ace2-153">要返回的 **body** 属性的格式。</span><span class="sxs-lookup"><span data-stu-id="0ace2-153">The format of the **body** property to be returned in.</span></span> <span data-ttu-id="0ace2-154">可取值为“text”或“html”。</span><span class="sxs-lookup"><span data-stu-id="0ace2-154">Values can be "text" or "html".</span></span> <span data-ttu-id="0ace2-155">如果指定此 `Preference-Applied` 头，返回 `Prefer` 头作为证明。</span><span class="sxs-lookup"><span data-stu-id="0ace2-155">A `Preference-Applied` header is returned as confirmation if this `Prefer` header is specified.</span></span> <span data-ttu-id="0ace2-156">如果未指定此头，采用 HTML 格式返回 **body** 属性。</span><span class="sxs-lookup"><span data-stu-id="0ace2-156">If the header is not specified, the **body** property is returned in HTML format.</span></span> <span data-ttu-id="0ace2-157">可选。</span><span class="sxs-lookup"><span data-stu-id="0ace2-157">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0ace2-158">请求正文</span><span class="sxs-lookup"><span data-stu-id="0ace2-158">Request body</span></span>
<span data-ttu-id="0ace2-159">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="0ace2-159">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0ace2-160">响应</span><span class="sxs-lookup"><span data-stu-id="0ace2-160">Response</span></span>

<span data-ttu-id="0ace2-161">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [event](../resources/event.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="0ace2-161">If successful, this method returns a `200 OK` response code and collection of [event](../resources/event.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="0ace2-162">示例</span><span class="sxs-lookup"><span data-stu-id="0ace2-162">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0ace2-163">请求</span><span class="sxs-lookup"><span data-stu-id="0ace2-163">Request</span></span>
<span data-ttu-id="0ace2-164">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="0ace2-164">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="0ace2-165">HTTP</span><span class="sxs-lookup"><span data-stu-id="0ace2-165">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_get_calendarview"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/calendarView?startDateTime=2020-01-01T19:00:00-08:00&endDateTime=2020-01-02T19:00:00-08:00
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="0ace2-166">C#</span><span class="sxs-lookup"><span data-stu-id="0ace2-166">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-get-calendarview-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="0ace2-167">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0ace2-167">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-get-calendarview-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="0ace2-168">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0ace2-168">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-get-calendarview-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="0ace2-169">Java</span><span class="sxs-lookup"><span data-stu-id="0ace2-169">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/user-get-calendarview-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="0ace2-170">响应</span><span class="sxs-lookup"><span data-stu-id="0ace2-170">Response</span></span>
<span data-ttu-id="0ace2-p109">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="0ace2-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.event",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 354

{
  "value": [
    {
      "originalStartTimeZone": "originalStartTimeZone-value",
      "originalEndTimeZone": "originalEndTimeZone-value",
      "responseStatus": {
        "response": "",
        "time": "datetime-value"
      },
      "iCalUId": "iCalUId-value",
      "reminderMinutesBeforeStart": 99,
      "isReminderOn": true
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
