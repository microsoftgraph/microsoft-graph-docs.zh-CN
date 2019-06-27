---
title: 列出 calendarView
description: '从用户的默认日历中，获取由时间范围定义的日历视图中的事件发生次数、异常和单个实例， '
localization_priority: Priority
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: e2420580d22d2e3f7c60412472d7586c1ceceb2a
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35277943"
---
# <a name="list-calendarview"></a><span data-ttu-id="f2826-103">列出 calendarView</span><span class="sxs-lookup"><span data-stu-id="f2826-103">List calendarView</span></span>

<span data-ttu-id="f2826-104">从用户的默认日历或其他一些日历中，获取由时间范围定义的日历视图中的事件发生次数、异常和单个实例。</span><span class="sxs-lookup"><span data-stu-id="f2826-104">Get the occurrences, exceptions, and single instances of events in a calendar view defined by a time range, from the user's default calendar, or from some other calendar of the user's.</span></span>
## <a name="permissions"></a><span data-ttu-id="f2826-105">权限</span><span class="sxs-lookup"><span data-stu-id="f2826-105">Permissions</span></span>
<span data-ttu-id="f2826-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f2826-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f2826-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="f2826-108">Permission type</span></span>      | <span data-ttu-id="f2826-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f2826-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f2826-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f2826-110">Delegated (work or school account)</span></span> | <span data-ttu-id="f2826-111">Calendars.Read、Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f2826-111">Calendars.Read, Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="f2826-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f2826-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f2826-113">Calendars.Read、Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f2826-113">Calendars.Read, Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="f2826-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="f2826-114">Application</span></span> | <span data-ttu-id="f2826-115">Calendars.Read、Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f2826-115">Calendars.Read, Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="f2826-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f2826-116">HTTP request</span></span>

<span data-ttu-id="f2826-117">用户的默认 [calendar](../resources/calendar.md)。</span><span class="sxs-lookup"><span data-stu-id="f2826-117">A user's default [calendar](../resources/calendar.md).</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/calendar/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
```

<span data-ttu-id="f2826-118">默认 [calendarGroup](../resources/calendargroup.md) 中的用户 [calendar](../resources/calendar.md)。</span><span class="sxs-lookup"><span data-stu-id="f2826-118">A user's [calendar](../resources/calendar.md) in the default [calendarGroup](../resources/calendargroup.md).</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}

GET /me/calendarGroup/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendarGroup/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
```

<span data-ttu-id="f2826-119">指定 [calendarGroup](../resources/calendargroup.md) 中用户的 [日历](../resources/calendar.md)。</span><span class="sxs-lookup"><span data-stu-id="f2826-119">A user's [calendar](../resources/calendar.md) in a specific [calendarGroup](../resources/calendargroup.md).</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/calendarGroups/{id}/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendarGroups/{id}/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
```

## <a name="query-parameters"></a><span data-ttu-id="f2826-120">查询参数</span><span class="sxs-lookup"><span data-stu-id="f2826-120">Query parameters</span></span>

<span data-ttu-id="f2826-121">在请求 URL 中，提供以下必要查询参数的值。</span><span class="sxs-lookup"><span data-stu-id="f2826-121">In the request URL, provide the following required query parameters with values.</span></span>

| <span data-ttu-id="f2826-122">参数</span><span class="sxs-lookup"><span data-stu-id="f2826-122">Parameter</span></span>    | <span data-ttu-id="f2826-123">类型</span><span class="sxs-lookup"><span data-stu-id="f2826-123">Type</span></span>   |<span data-ttu-id="f2826-124">说明</span><span class="sxs-lookup"><span data-stu-id="f2826-124">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f2826-125">startDateTime</span><span class="sxs-lookup"><span data-stu-id="f2826-125">startDateTime</span></span>|<span data-ttu-id="f2826-126">String</span><span class="sxs-lookup"><span data-stu-id="f2826-126">String</span></span>|<span data-ttu-id="f2826-p102">时间范围的开始日期和时间以 ISO 8601 格式表示。例如，“2015-11-08T19:00:00.0000000”。</span><span class="sxs-lookup"><span data-stu-id="f2826-p102">The start date and time of the time range, represented in ISO 8601 format. For example, "2015-11-08T19:00:00.0000000".</span></span>|
|<span data-ttu-id="f2826-129">endDateTime</span><span class="sxs-lookup"><span data-stu-id="f2826-129">endDateTime</span></span>|<span data-ttu-id="f2826-130">String</span><span class="sxs-lookup"><span data-stu-id="f2826-130">String</span></span>|<span data-ttu-id="f2826-p103">时间范围的结束日期和时间以 ISO 8601 格式表示。例如，“2015-11-08T20:00:00.0000000”。</span><span class="sxs-lookup"><span data-stu-id="f2826-p103">The end date and time of the time range, represented in ISO 8601 format. For example, "2015-11-08T20:00:00.0000000".</span></span>|

<span data-ttu-id="f2826-133">此方法还支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="f2826-133">This method also supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="f2826-134">请求标头</span><span class="sxs-lookup"><span data-stu-id="f2826-134">Request headers</span></span>
| <span data-ttu-id="f2826-135">名称</span><span class="sxs-lookup"><span data-stu-id="f2826-135">Name</span></span>       | <span data-ttu-id="f2826-136">类型</span><span class="sxs-lookup"><span data-stu-id="f2826-136">Type</span></span> | <span data-ttu-id="f2826-137">说明</span><span class="sxs-lookup"><span data-stu-id="f2826-137">Description</span></span> |
|:---------------|:--------|:--------|
| <span data-ttu-id="f2826-138">Authorization</span><span class="sxs-lookup"><span data-stu-id="f2826-138">Authorization</span></span>  | <span data-ttu-id="f2826-139">string</span><span class="sxs-lookup"><span data-stu-id="f2826-139">string</span></span> | <span data-ttu-id="f2826-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="f2826-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="f2826-142">Prefer: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="f2826-142">Prefer: outlook.timezone</span></span>  | <span data-ttu-id="f2826-143">string</span><span class="sxs-lookup"><span data-stu-id="f2826-143">string</span></span> | <span data-ttu-id="f2826-144">此选项可用于指定响应中开始时间和结束时间的时区。</span><span class="sxs-lookup"><span data-stu-id="f2826-144">Use this to specify the time zone for start and end times in the response.</span></span> <span data-ttu-id="f2826-145">如果未指定，返回的这些时间值采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="f2826-145">If not specified, those time values are returned in UTC.</span></span> <span data-ttu-id="f2826-146">可选。</span><span class="sxs-lookup"><span data-stu-id="f2826-146">Optional.</span></span> |
| <span data-ttu-id="f2826-147">Prefer: outlook.body-content-type</span><span class="sxs-lookup"><span data-stu-id="f2826-147">Prefer: outlook.body-content-type</span></span> | <span data-ttu-id="f2826-148">string</span><span class="sxs-lookup"><span data-stu-id="f2826-148">string</span></span> | <span data-ttu-id="f2826-149">要返回的 **body** 属性的格式。</span><span class="sxs-lookup"><span data-stu-id="f2826-149">The format of the **body** property to be returned in.</span></span> <span data-ttu-id="f2826-150">可取值为“text”或“html”。</span><span class="sxs-lookup"><span data-stu-id="f2826-150">Values can be "text" or "html".</span></span> <span data-ttu-id="f2826-151">如果指定此 `Preference-Applied` 头，返回 `Prefer` 头作为证明。</span><span class="sxs-lookup"><span data-stu-id="f2826-151">A `Preference-Applied` header is returned as confirmation if this `Prefer` header is specified.</span></span> <span data-ttu-id="f2826-152">如果未指定此头，采用 HTML 格式返回 **body** 属性。</span><span class="sxs-lookup"><span data-stu-id="f2826-152">If the header is not specified, the **body** property is returned in HTML format.</span></span> <span data-ttu-id="f2826-153">可选。</span><span class="sxs-lookup"><span data-stu-id="f2826-153">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f2826-154">请求正文</span><span class="sxs-lookup"><span data-stu-id="f2826-154">Request body</span></span>
<span data-ttu-id="f2826-155">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="f2826-155">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f2826-156">响应</span><span class="sxs-lookup"><span data-stu-id="f2826-156">Response</span></span>

<span data-ttu-id="f2826-157">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [Event](../resources/event.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="f2826-157">If successful, this method returns a `200 OK` response code and collection of [Event](../resources/event.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="f2826-158">示例</span><span class="sxs-lookup"><span data-stu-id="f2826-158">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f2826-159">请求</span><span class="sxs-lookup"><span data-stu-id="f2826-159">Request</span></span>
<span data-ttu-id="f2826-160">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="f2826-160">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_calendarview"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/calendarView?startDateTime=2016-01-01T19:00:00.0000000&endDateTime=2016-10-01T19:00:00.0000000 
```
##### <a name="response"></a><span data-ttu-id="f2826-161">响应</span><span class="sxs-lookup"><span data-stu-id="f2826-161">Response</span></span>
<span data-ttu-id="f2826-p107">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="f2826-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="f2826-165">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="f2826-165">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="f2826-166">C#</span><span class="sxs-lookup"><span data-stu-id="f2826-166">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_calendarview-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f2826-167">Javascript</span><span class="sxs-lookup"><span data-stu-id="f2826-167">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_calendarview-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="f2826-168">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f2826-168">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_calendarview-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List calendarView",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/user-list-calendarview.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/user-list-calendarview.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/user-list-calendarview.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
