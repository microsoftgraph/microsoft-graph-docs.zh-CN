---
title: 列出 calendarView
description: 获取由一个时间范围，定义日历视图中的匹配项、 例外和事件的单个实例
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: b360d47c99de387daf5b421623f926ad7912b912
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29520891"
---
# <a name="list-calendarview"></a><span data-ttu-id="8eddf-103">列出 calendarView</span><span class="sxs-lookup"><span data-stu-id="8eddf-103">List calendarView</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8eddf-104">从用户或群组的默认日历 `(../me/calendarview)` 或用户的其他一些日历中，获取由时间范围定义的日历视图中的事件发生次数、异常和单个实例。</span><span class="sxs-lookup"><span data-stu-id="8eddf-104">Get the occurrences, exceptions, and single instances of events in a calendar view defined by a time range, from the default calendar `(../me/calendarview)` of a user or group, or some other calendar of the user's.</span></span>

## <a name="permissions"></a><span data-ttu-id="8eddf-105">权限</span><span class="sxs-lookup"><span data-stu-id="8eddf-105">Permissions</span></span>
<span data-ttu-id="8eddf-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8eddf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

* <span data-ttu-id="8eddf-108">用户日历中的事件：Calendars.Read 或 Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8eddf-108">Events in a user's calendar: Calendars.Read or Calendars.ReadWrite</span></span>
* <span data-ttu-id="8eddf-109">群组日历中的事件：Group.Read.All 或 Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8eddf-109">Events in a group calendar: Group.Read.All or Group.ReadWrite.All</span></span>

## <a name="http-request"></a><span data-ttu-id="8eddf-110">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8eddf-110">HTTP request</span></span>
<span data-ttu-id="8eddf-111"><!-- { "blockType": "ignored" } -->用户或组的默认[日历](../resources/calendar.md)。</span><span class="sxs-lookup"><span data-stu-id="8eddf-111"><!-- { "blockType": "ignored" } --> A user's or group's default [calendar](../resources/calendar.md).</span></span>
```http
GET /me/calendar/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendar/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /groups/{id}/calendar/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
```

<span data-ttu-id="8eddf-112">默认 [calendarGroup](../resources/calendargroup.md) 中的用户 [calendar](../resources/calendar.md)。</span><span class="sxs-lookup"><span data-stu-id="8eddf-112">A user's [calendar](../resources/calendar.md) in the default [calendarGroup](../resources/calendargroup.md).</span></span>
```http
GET /me/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}

GET /me/calendarGroup/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendarGroup/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
```

<span data-ttu-id="8eddf-113">指定 [calendarGroup](../resources/calendargroup.md) 中用户的 [日历](../resources/calendar.md)。</span><span class="sxs-lookup"><span data-stu-id="8eddf-113">A user's [calendar](../resources/calendar.md) in a specific [calendarGroup](../resources/calendargroup.md).</span></span>
```http
GET /me/calendarGroups/{id}/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendarGroups/{id}/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
```

## <a name="query-parameters"></a><span data-ttu-id="8eddf-114">查询参数</span><span class="sxs-lookup"><span data-stu-id="8eddf-114">Query parameters</span></span>

<span data-ttu-id="8eddf-115">在请求 URL 中，提供以下必要查询参数的值。</span><span class="sxs-lookup"><span data-stu-id="8eddf-115">In the request URL, provide the following required query parameters with values.</span></span>

| <span data-ttu-id="8eddf-116">参数</span><span class="sxs-lookup"><span data-stu-id="8eddf-116">Parameter</span></span>    | <span data-ttu-id="8eddf-117">类型</span><span class="sxs-lookup"><span data-stu-id="8eddf-117">Type</span></span>   |<span data-ttu-id="8eddf-118">说明</span><span class="sxs-lookup"><span data-stu-id="8eddf-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8eddf-119">startDateTime</span><span class="sxs-lookup"><span data-stu-id="8eddf-119">startDateTime</span></span>|<span data-ttu-id="8eddf-120">String</span><span class="sxs-lookup"><span data-stu-id="8eddf-120">String</span></span>|<span data-ttu-id="8eddf-p102">时间范围的开始日期和时间以 ISO 8601 格式表示。例如，“2015-11-08T19:00:00.0000000”。</span><span class="sxs-lookup"><span data-stu-id="8eddf-p102">The start date and time of the time range, represented in ISO 8601 format. For example, "2015-11-08T19:00:00.0000000".</span></span>|
|<span data-ttu-id="8eddf-123">endDateTime</span><span class="sxs-lookup"><span data-stu-id="8eddf-123">endDateTime</span></span>|<span data-ttu-id="8eddf-124">String</span><span class="sxs-lookup"><span data-stu-id="8eddf-124">String</span></span>|<span data-ttu-id="8eddf-p103">时间范围的结束日期和时间以 ISO 8601 格式表示。例如，“2015-11-08T20:00:00.0000000”。</span><span class="sxs-lookup"><span data-stu-id="8eddf-p103">The end date and time of the time range, represented in ISO 8601 format. For example, "2015-11-08T20:00:00.0000000".</span></span>|

<span data-ttu-id="8eddf-127">此方法还支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="8eddf-127">This method also supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="8eddf-128">请求标头</span><span class="sxs-lookup"><span data-stu-id="8eddf-128">Request headers</span></span>
| <span data-ttu-id="8eddf-129">名称</span><span class="sxs-lookup"><span data-stu-id="8eddf-129">Name</span></span>       | <span data-ttu-id="8eddf-130">类型</span><span class="sxs-lookup"><span data-stu-id="8eddf-130">Type</span></span> | <span data-ttu-id="8eddf-131">说明</span><span class="sxs-lookup"><span data-stu-id="8eddf-131">Description</span></span> |
|:---------------|:--------|:--------|
| <span data-ttu-id="8eddf-132">Authorization</span><span class="sxs-lookup"><span data-stu-id="8eddf-132">Authorization</span></span>  | <span data-ttu-id="8eddf-133">string</span><span class="sxs-lookup"><span data-stu-id="8eddf-133">string</span></span> | <span data-ttu-id="8eddf-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="8eddf-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="8eddf-136">Prefer: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="8eddf-136">Prefer: outlook.timezone</span></span>  | <span data-ttu-id="8eddf-137">string</span><span class="sxs-lookup"><span data-stu-id="8eddf-137">string</span></span> | <span data-ttu-id="8eddf-138">此选项可用于指定响应中开始时间和结束时间的时区。</span><span class="sxs-lookup"><span data-stu-id="8eddf-138">Use this to specify the time zone for start and end times in the response.</span></span> <span data-ttu-id="8eddf-139">如果未指定，返回的这些时间值采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="8eddf-139">If not specified, those time values are returned in UTC.</span></span> <span data-ttu-id="8eddf-140">可选。</span><span class="sxs-lookup"><span data-stu-id="8eddf-140">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8eddf-141">请求正文</span><span class="sxs-lookup"><span data-stu-id="8eddf-141">Request body</span></span>
<span data-ttu-id="8eddf-142">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="8eddf-142">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8eddf-143">响应</span><span class="sxs-lookup"><span data-stu-id="8eddf-143">Response</span></span>

<span data-ttu-id="8eddf-144">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [Event](../resources/event.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="8eddf-144">If successful, this method returns a `200 OK` response code and collection of [Event](../resources/event.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="8eddf-145">示例</span><span class="sxs-lookup"><span data-stu-id="8eddf-145">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8eddf-146">请求</span><span class="sxs-lookup"><span data-stu-id="8eddf-146">Request</span></span>
<span data-ttu-id="8eddf-147">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="8eddf-147">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_calendarview"
}-->
```http
GET https://graph.microsoft.com/beta/me/calendar/calendarView?startDateTime=2017-01-01T19:00:00.0000000&endDateTime=2017-01-07T19:00:00.0000000
```
##### <a name="response"></a><span data-ttu-id="8eddf-148">响应</span><span class="sxs-lookup"><span data-stu-id="8eddf-148">Response</span></span>
<span data-ttu-id="8eddf-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="8eddf-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "suppressions": [
    "Error: /api-reference/beta/api/calendar-list-calendarview.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
