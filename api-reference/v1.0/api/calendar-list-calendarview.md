---
title: 列出 calendarView
description: 获取由时间范围定义的日历视图中的事件发生次数、异常和单个实例，
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: dfc0d378a48716f70753b38d1970f0d4017a13a7
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32570601"
---
# <a name="list-calendarview"></a><span data-ttu-id="fe0e9-103">列出 calendarView</span><span class="sxs-lookup"><span data-stu-id="fe0e9-103">List calendarView</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fe0e9-104">从用户或群组的默认日历 `(../me/calendarview)` 或用户的其他一些日历中，获取由时间范围定义的日历视图中的事件发生次数、异常和单个实例。</span><span class="sxs-lookup"><span data-stu-id="fe0e9-104">Get the occurrences, exceptions, and single instances of events in a calendar view defined by a time range, from the default calendar `(../me/calendarview)` of a user or group, or some other calendar of the user's.</span></span>

## <a name="permissions"></a><span data-ttu-id="fe0e9-105">权限</span><span class="sxs-lookup"><span data-stu-id="fe0e9-105">Permissions</span></span>
<span data-ttu-id="fe0e9-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="fe0e9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

* <span data-ttu-id="fe0e9-108">用户日历中的事件：Calendars.Read 或 Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="fe0e9-108">Events in a user's calendar: Calendars.Read or Calendars.ReadWrite</span></span>
* <span data-ttu-id="fe0e9-109">群组日历中的事件：Group.Read.All 或 Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fe0e9-109">Events in a group calendar: Group.Read.All or Group.ReadWrite.All</span></span>

## <a name="http-request"></a><span data-ttu-id="fe0e9-110">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="fe0e9-110">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="fe0e9-111">用户或组的默认 [日历](../resources/calendar.md)。</span><span class="sxs-lookup"><span data-stu-id="fe0e9-111">A user's or group's default [calendar](../resources/calendar.md).</span></span>
```http
GET /me/calendar/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendar/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /groups/{id}/calendar/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
```

<span data-ttu-id="fe0e9-112">默认 [calendarGroup](../resources/calendargroup.md) 中用户的 [日历](../resources/calendar.md)。</span><span class="sxs-lookup"><span data-stu-id="fe0e9-112">A user's [calendar](../resources/calendar.md) in the default [calendarGroup](../resources/calendargroup.md).</span></span>
```http
GET /me/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}

GET /me/calendarGroup/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendarGroup/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
```

<span data-ttu-id="fe0e9-113">指定 [calendarGroup](../resources/calendargroup.md) 中用户的 [日历](../resources/calendar.md)。</span><span class="sxs-lookup"><span data-stu-id="fe0e9-113">A user's [calendar](../resources/calendar.md) in a specific [calendarGroup](../resources/calendargroup.md).</span></span>
```http
GET /me/calendarGroups/{id}/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendarGroups/{id}/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
```

## <a name="query-parameters"></a><span data-ttu-id="fe0e9-114">查询参数</span><span class="sxs-lookup"><span data-stu-id="fe0e9-114">Query parameters</span></span>

<span data-ttu-id="fe0e9-115">在请求 URL 中，提供以下必要查询参数的值。</span><span class="sxs-lookup"><span data-stu-id="fe0e9-115">In the request URL, provide the following required query parameters with values.</span></span>

| <span data-ttu-id="fe0e9-116">参数</span><span class="sxs-lookup"><span data-stu-id="fe0e9-116">Parameter</span></span>    | <span data-ttu-id="fe0e9-117">类型</span><span class="sxs-lookup"><span data-stu-id="fe0e9-117">Type</span></span>   |<span data-ttu-id="fe0e9-118">说明</span><span class="sxs-lookup"><span data-stu-id="fe0e9-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fe0e9-119">startDateTime</span><span class="sxs-lookup"><span data-stu-id="fe0e9-119">startDateTime</span></span>|<span data-ttu-id="fe0e9-120">String</span><span class="sxs-lookup"><span data-stu-id="fe0e9-120">String</span></span>|<span data-ttu-id="fe0e9-p102">时间范围的开始日期和时间以 ISO 8601 格式表示。例如，“2015-11-08T19:00:00.0000000”。</span><span class="sxs-lookup"><span data-stu-id="fe0e9-p102">The start date and time of the time range, represented in ISO 8601 format. For example, "2015-11-08T19:00:00.0000000".</span></span>|
|<span data-ttu-id="fe0e9-123">endDateTime</span><span class="sxs-lookup"><span data-stu-id="fe0e9-123">endDateTime</span></span>|<span data-ttu-id="fe0e9-124">String</span><span class="sxs-lookup"><span data-stu-id="fe0e9-124">String</span></span>|<span data-ttu-id="fe0e9-p103">时间范围的结束日期和时间以 ISO 8601 格式表示。例如，“2015-11-08T20:00:00.0000000”。</span><span class="sxs-lookup"><span data-stu-id="fe0e9-p103">The end date and time of the time range, represented in ISO 8601 format. For example, "2015-11-08T20:00:00.0000000".</span></span>|

<span data-ttu-id="fe0e9-127">此方法还支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="fe0e9-127">This method also supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="fe0e9-128">请求标头</span><span class="sxs-lookup"><span data-stu-id="fe0e9-128">Request headers</span></span>
| <span data-ttu-id="fe0e9-129">名称</span><span class="sxs-lookup"><span data-stu-id="fe0e9-129">Name</span></span>       | <span data-ttu-id="fe0e9-130">类型</span><span class="sxs-lookup"><span data-stu-id="fe0e9-130">Type</span></span> | <span data-ttu-id="fe0e9-131">说明</span><span class="sxs-lookup"><span data-stu-id="fe0e9-131">Description</span></span> |
|:---------------|:--------|:--------|
| <span data-ttu-id="fe0e9-132">Authorization</span><span class="sxs-lookup"><span data-stu-id="fe0e9-132">Authorization</span></span>  | <span data-ttu-id="fe0e9-133">string</span><span class="sxs-lookup"><span data-stu-id="fe0e9-133">string</span></span> | <span data-ttu-id="fe0e9-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="fe0e9-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="fe0e9-136">Prefer: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="fe0e9-136">Prefer: outlook.timezone</span></span>  | <span data-ttu-id="fe0e9-137">string</span><span class="sxs-lookup"><span data-stu-id="fe0e9-137">string</span></span> | <span data-ttu-id="fe0e9-138">此选项可用于指定响应中开始时间和结束时间的时区。</span><span class="sxs-lookup"><span data-stu-id="fe0e9-138">Use this to specify the time zone for start and end times in the response.</span></span> <span data-ttu-id="fe0e9-139">如果未指定，返回的这些时间值采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="fe0e9-139">If not specified, those time values are returned in UTC.</span></span> <span data-ttu-id="fe0e9-140">可选。</span><span class="sxs-lookup"><span data-stu-id="fe0e9-140">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="fe0e9-141">请求正文</span><span class="sxs-lookup"><span data-stu-id="fe0e9-141">Request body</span></span>
<span data-ttu-id="fe0e9-142">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="fe0e9-142">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fe0e9-143">响应</span><span class="sxs-lookup"><span data-stu-id="fe0e9-143">Response</span></span>

<span data-ttu-id="fe0e9-144">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [Event](../resources/event.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="fe0e9-144">If successful, this method returns a `200 OK` response code and collection of [Event](../resources/event.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="fe0e9-145">示例</span><span class="sxs-lookup"><span data-stu-id="fe0e9-145">Example</span></span>
##### <a name="request"></a><span data-ttu-id="fe0e9-146">请求</span><span class="sxs-lookup"><span data-stu-id="fe0e9-146">Request</span></span>
<span data-ttu-id="fe0e9-147">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="fe0e9-147">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_calendarview"
}-->
```http
GET https://graph.microsoft.com/beta/me/calendar/calendarView?startDateTime=2017-01-01T19:00:00.0000000&endDateTime=2017-01-07T19:00:00.0000000
```
##### <a name="response"></a><span data-ttu-id="fe0e9-148">响应</span><span class="sxs-lookup"><span data-stu-id="fe0e9-148">Response</span></span>
<span data-ttu-id="fe0e9-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="fe0e9-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
        "response": "response-value",
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
<!--
{
  "type": "#page.annotation",
  "description": "List calendarView",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
