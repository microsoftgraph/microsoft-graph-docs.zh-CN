---
title: 列出 calendarView
description: 获取由一个时间范围，从用户的默认日历中，定义日历视图中的匹配项、 例外和事件的单个实例
localization_priority: Normal
ms.openlocfilehash: 8db54c6ad12254957fd2c95509ddbebd34813906
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27876074"
---
# <a name="list-calendarview"></a><span data-ttu-id="25af7-103">列出 calendarView</span><span class="sxs-lookup"><span data-stu-id="25af7-103">List calendarView</span></span>

> <span data-ttu-id="25af7-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="25af7-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="25af7-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="25af7-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="25af7-106">从用户的默认日历或其他一些日历中，获取由时间范围定义的日历视图中的事件发生次数、异常和单个实例。</span><span class="sxs-lookup"><span data-stu-id="25af7-106">Get the occurrences, exceptions, and single instances of events in a calendar view defined by a time range, from the user's default calendar, or from some other calendar of the user's.</span></span>
## <a name="permissions"></a><span data-ttu-id="25af7-107">权限</span><span class="sxs-lookup"><span data-stu-id="25af7-107">Permissions</span></span>
<span data-ttu-id="25af7-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="25af7-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="25af7-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="25af7-110">Permission type</span></span>      | <span data-ttu-id="25af7-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="25af7-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="25af7-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="25af7-112">Delegated (work or school account)</span></span> | <span data-ttu-id="25af7-113">Calendars.Read、Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="25af7-113">Calendars.Read, Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="25af7-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="25af7-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="25af7-115">Calendars.Read、Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="25af7-115">Calendars.Read, Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="25af7-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="25af7-116">Application</span></span> | <span data-ttu-id="25af7-117">Calendars.Read、Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="25af7-117">Calendars.Read, Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="25af7-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="25af7-118">HTTP request</span></span>
<span data-ttu-id="25af7-119">用户的默认 [calendar](../resources/calendar.md)。</span><span class="sxs-lookup"><span data-stu-id="25af7-119">A user's default [calendar](../resources/calendar.md).</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/calendar/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
```

<span data-ttu-id="25af7-120">默认 [calendarGroup](../resources/calendargroup.md) 中的用户 [calendar](../resources/calendar.md)。</span><span class="sxs-lookup"><span data-stu-id="25af7-120">A user's [calendar](../resources/calendar.md) in the default [calendarGroup](../resources/calendargroup.md).</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}

GET /me/calendarGroup/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendarGroup/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
```

<span data-ttu-id="25af7-121">指定 [calendarGroup](../resources/calendargroup.md) 中用户的 [日历](../resources/calendar.md)。</span><span class="sxs-lookup"><span data-stu-id="25af7-121">A user's [calendar](../resources/calendar.md) in a specific [calendarGroup](../resources/calendargroup.md).</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/calendarGroups/{id}/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendarGroups/{id}/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
```

## <a name="query-parameters"></a><span data-ttu-id="25af7-122">查询参数</span><span class="sxs-lookup"><span data-stu-id="25af7-122">Query parameters</span></span>

<span data-ttu-id="25af7-123">在请求 URL 中，提供以下必要查询参数的值。</span><span class="sxs-lookup"><span data-stu-id="25af7-123">In the request URL, provide the following required query parameters with values.</span></span>

| <span data-ttu-id="25af7-124">参数</span><span class="sxs-lookup"><span data-stu-id="25af7-124">Parameter</span></span>    | <span data-ttu-id="25af7-125">类型</span><span class="sxs-lookup"><span data-stu-id="25af7-125">Type</span></span>   |<span data-ttu-id="25af7-126">说明</span><span class="sxs-lookup"><span data-stu-id="25af7-126">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="25af7-127">startDateTime</span><span class="sxs-lookup"><span data-stu-id="25af7-127">startDateTime</span></span>|<span data-ttu-id="25af7-128">字符串</span><span class="sxs-lookup"><span data-stu-id="25af7-128">String</span></span>|<span data-ttu-id="25af7-p103">时间范围的开始日期和时间以 ISO 8601 格式表示。例如，“2015-11-08T19:00:00.0000000”。</span><span class="sxs-lookup"><span data-stu-id="25af7-p103">The start date and time of the time range, represented in ISO 8601 format. For example, "2015-11-08T19:00:00.0000000".</span></span>|
|<span data-ttu-id="25af7-131">endDateTime</span><span class="sxs-lookup"><span data-stu-id="25af7-131">endDateTime</span></span>|<span data-ttu-id="25af7-132">字符串</span><span class="sxs-lookup"><span data-stu-id="25af7-132">String</span></span>|<span data-ttu-id="25af7-p104">时间范围的结束日期和时间以 ISO 8601 格式表示。例如，“2015-11-08T20:00:00.0000000”。</span><span class="sxs-lookup"><span data-stu-id="25af7-p104">The end date and time of the time range, represented in ISO 8601 format. For example, "2015-11-08T20:00:00.0000000".</span></span>|

<span data-ttu-id="25af7-135">此方法还支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="25af7-135">This method also supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="25af7-136">请求标头</span><span class="sxs-lookup"><span data-stu-id="25af7-136">Request headers</span></span>
| <span data-ttu-id="25af7-137">名称</span><span class="sxs-lookup"><span data-stu-id="25af7-137">Name</span></span>       | <span data-ttu-id="25af7-138">类型</span><span class="sxs-lookup"><span data-stu-id="25af7-138">Type</span></span> | <span data-ttu-id="25af7-139">说明</span><span class="sxs-lookup"><span data-stu-id="25af7-139">Description</span></span> |
|:---------------|:--------|:--------|
| <span data-ttu-id="25af7-140">Authorization</span><span class="sxs-lookup"><span data-stu-id="25af7-140">Authorization</span></span>  | <span data-ttu-id="25af7-141">string</span><span class="sxs-lookup"><span data-stu-id="25af7-141">string</span></span> | <span data-ttu-id="25af7-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="25af7-p105">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="25af7-144">Prefer: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="25af7-144">Prefer: outlook.timezone</span></span>  | <span data-ttu-id="25af7-145">string</span><span class="sxs-lookup"><span data-stu-id="25af7-145">string</span></span> | <span data-ttu-id="25af7-146">此选项可用于指定响应中开始时间和结束时间的时区。</span><span class="sxs-lookup"><span data-stu-id="25af7-146">Use this to specify the time zone for start and end times in the response.</span></span> <span data-ttu-id="25af7-147">如果未指定，返回的这些时间值采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="25af7-147">If not specified, those time values are returned in UTC.</span></span> <span data-ttu-id="25af7-148">可选。</span><span class="sxs-lookup"><span data-stu-id="25af7-148">Optional.</span></span> |
| <span data-ttu-id="25af7-149">Prefer: outlook.body-content-type</span><span class="sxs-lookup"><span data-stu-id="25af7-149">Prefer: outlook.body-content-type</span></span> | <span data-ttu-id="25af7-150">string</span><span class="sxs-lookup"><span data-stu-id="25af7-150">string</span></span> | <span data-ttu-id="25af7-151">要返回的 **body** 属性的格式。</span><span class="sxs-lookup"><span data-stu-id="25af7-151">The format of the **body** property to be returned in.</span></span> <span data-ttu-id="25af7-152">可取值为“text”或“html”。</span><span class="sxs-lookup"><span data-stu-id="25af7-152">Values can be "text" or "html".</span></span> <span data-ttu-id="25af7-153">如果指定此 `Preference-Applied` 头，返回 `Prefer` 头作为证明。</span><span class="sxs-lookup"><span data-stu-id="25af7-153">A `Preference-Applied` header is returned as confirmation if this `Prefer` header is specified.</span></span> <span data-ttu-id="25af7-154">如果未指定此头，采用 HTML 格式返回 **body** 属性。</span><span class="sxs-lookup"><span data-stu-id="25af7-154">If the header is not specified, the **body** property is returned in HTML format.</span></span> <span data-ttu-id="25af7-155">可选。</span><span class="sxs-lookup"><span data-stu-id="25af7-155">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="25af7-156">请求正文</span><span class="sxs-lookup"><span data-stu-id="25af7-156">Request body</span></span>
<span data-ttu-id="25af7-157">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="25af7-157">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="25af7-158">响应</span><span class="sxs-lookup"><span data-stu-id="25af7-158">Response</span></span>

<span data-ttu-id="25af7-159">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [Event](../resources/event.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="25af7-159">If successful, this method returns a `200 OK` response code and collection of [Event](../resources/event.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="25af7-160">示例</span><span class="sxs-lookup"><span data-stu-id="25af7-160">Example</span></span>
##### <a name="request"></a><span data-ttu-id="25af7-161">请求</span><span class="sxs-lookup"><span data-stu-id="25af7-161">Request</span></span>
<span data-ttu-id="25af7-162">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="25af7-162">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_calendarview"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/calendarView?startDateTime=2016-01-01T19:00:00.0000000&endDateTime=2016-10-01T19:00:00.0000000
```
##### <a name="response"></a><span data-ttu-id="25af7-163">响应</span><span class="sxs-lookup"><span data-stu-id="25af7-163">Response</span></span>
<span data-ttu-id="25af7-p108">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="25af7-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
        "time": "2016-10-19T10:37:00Z"
      },
      "uid": "iCalUId-value",
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
  "keywords": "calendar",
  "section": "documentation",
  "tocPath": ""
}-->
