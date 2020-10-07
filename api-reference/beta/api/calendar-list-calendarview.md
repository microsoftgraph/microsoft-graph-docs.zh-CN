---
title: 列出 calendarView
description: 获取由时间范围定义的日历视图中的事件发生次数、异常和单个实例，
localization_priority: Normal
author: harini84
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 36509a1983ff9398bc438ed7c8e6b5ebefae1541
ms.sourcegitcommit: c20276369a8834a259f24038e7ee5c33de02660b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/07/2020
ms.locfileid: "48372157"
---
# <a name="list-calendarview"></a><span data-ttu-id="ed3a6-103">列出 calendarView</span><span class="sxs-lookup"><span data-stu-id="ed3a6-103">List calendarView</span></span>

<span data-ttu-id="ed3a6-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ed3a6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ed3a6-105">从用户的默认日历 `(../me/calendarview)` 或其他一些日历中，获取由时间范围定义的日历视图中的事件发生次数、异常和单个实例。</span><span class="sxs-lookup"><span data-stu-id="ed3a6-105">Get the occurrences, exceptions, and single instances of events in a calendar view defined by a time range, from a user's default calendar `(../me/calendarview)` or some other calendar of the user's.</span></span>

## <a name="permissions"></a><span data-ttu-id="ed3a6-106">权限</span><span class="sxs-lookup"><span data-stu-id="ed3a6-106">Permissions</span></span>
<span data-ttu-id="ed3a6-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ed3a6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ed3a6-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="ed3a6-109">Permission type</span></span>      | <span data-ttu-id="ed3a6-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ed3a6-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ed3a6-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ed3a6-111">Delegated (work or school account)</span></span> | <span data-ttu-id="ed3a6-112">Calendars.Read、Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ed3a6-112">Calendars.Read, Calendars.ReadWrite</span></span> |
|<span data-ttu-id="ed3a6-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ed3a6-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ed3a6-114">Calendars.Read、Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ed3a6-114">Calendars.Read, Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="ed3a6-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="ed3a6-115">Application</span></span> | <span data-ttu-id="ed3a6-116">Calendars.Read、Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ed3a6-116">Calendars.Read, Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="ed3a6-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ed3a6-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="ed3a6-118">用户的默认 [calendar](../resources/calendar.md)。</span><span class="sxs-lookup"><span data-stu-id="ed3a6-118">A user's default [calendar](../resources/calendar.md).</span></span>
```http
GET /me/calendar/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendar/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
```

<span data-ttu-id="ed3a6-119">默认 [calendarGroup](../resources/calendargroup.md) 中的用户 [calendar](../resources/calendar.md)。</span><span class="sxs-lookup"><span data-stu-id="ed3a6-119">A user's [calendar](../resources/calendar.md) in the default [calendarGroup](../resources/calendargroup.md).</span></span>
```http
GET /me/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}

GET /me/calendarGroup/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendarGroup/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
```

<span data-ttu-id="ed3a6-120">指定 [calendarGroup](../resources/calendargroup.md) 中用户的 [日历](../resources/calendar.md)。</span><span class="sxs-lookup"><span data-stu-id="ed3a6-120">A user's [calendar](../resources/calendar.md) in a specific [calendarGroup](../resources/calendargroup.md).</span></span>
```http
GET /me/calendarGroups/{id}/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendarGroups/{id}/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
```

## <a name="query-parameters"></a><span data-ttu-id="ed3a6-121">查询参数</span><span class="sxs-lookup"><span data-stu-id="ed3a6-121">Query parameters</span></span>

<span data-ttu-id="ed3a6-122">在请求 URL 中，提供以下必要查询参数的值。</span><span class="sxs-lookup"><span data-stu-id="ed3a6-122">In the request URL, provide the following required query parameters with values.</span></span>

| <span data-ttu-id="ed3a6-123">参数</span><span class="sxs-lookup"><span data-stu-id="ed3a6-123">Parameter</span></span>     | <span data-ttu-id="ed3a6-124">类型</span><span class="sxs-lookup"><span data-stu-id="ed3a6-124">Type</span></span>   | <span data-ttu-id="ed3a6-125">说明</span><span class="sxs-lookup"><span data-stu-id="ed3a6-125">Description</span></span>                                                                                                            |
|:--------------|:-------|:-----------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="ed3a6-126">startDateTime</span><span class="sxs-lookup"><span data-stu-id="ed3a6-126">startDateTime</span></span> | <span data-ttu-id="ed3a6-127">String</span><span class="sxs-lookup"><span data-stu-id="ed3a6-127">String</span></span> | <span data-ttu-id="ed3a6-p102">时间范围的开始日期和时间，以 ISO 8601 格式表示。例如，“2019-11-08T19:00:00-08:00”。</span><span class="sxs-lookup"><span data-stu-id="ed3a6-p102">The start date and time of the time range, represented in ISO 8601 format. For example, "2019-11-08T19:00:00-08:00".</span></span> |
| <span data-ttu-id="ed3a6-130">endDateTime</span><span class="sxs-lookup"><span data-stu-id="ed3a6-130">endDateTime</span></span>   | <span data-ttu-id="ed3a6-131">String</span><span class="sxs-lookup"><span data-stu-id="ed3a6-131">String</span></span> | <span data-ttu-id="ed3a6-p103">时间范围的结束日期和时间，以 ISO 8601 格式表示。例如，“2019-11-08T20:00:00-08:00”。</span><span class="sxs-lookup"><span data-stu-id="ed3a6-p103">The end date and time of the time range, represented in ISO 8601 format. For example, "2019-11-08T20:00:00-08:00".</span></span>   |

<span data-ttu-id="ed3a6-134">`startDateTime` 和 `endDateTime` 的值使用值中指定的时区偏移量进行解释，并且不受 `Prefer: outlook.timezone` 标头（若有）的值影响。</span><span class="sxs-lookup"><span data-stu-id="ed3a6-134">The values of `startDateTime` and `endDateTime` are interpreted using the timezone offset specified in the value and are not impacted by the value of the `Prefer: outlook.timezone` header if present.</span></span> <span data-ttu-id="ed3a6-135">如果值中未包含时区偏移量，则将其解释为 UTC。</span><span class="sxs-lookup"><span data-stu-id="ed3a6-135">If no timezone offset is included in the value, it is interpreted as UTC.</span></span>

<span data-ttu-id="ed3a6-136">此方法还支持一些 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="ed3a6-136">This method also supports some of the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

> [!NOTE]
> <span data-ttu-id="ed3a6-137">[事件](../resources/event.md)的 **createdDateTime** 和 **lastModifiedDateTime** 属性不支持 `$select`。</span><span class="sxs-lookup"><span data-stu-id="ed3a6-137">The **createdDateTime** and **lastModifiedDateTime** properties of [event](../resources/event.md) do not support `$select`.</span></span> <span data-ttu-id="ed3a6-138">若要获取它们的值，只需在 **calendarView** 上进行查询，而不应用 `$select`。</span><span class="sxs-lookup"><span data-stu-id="ed3a6-138">To get their values, simply query on **calendarView** without applying `$select`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ed3a6-139">请求标头</span><span class="sxs-lookup"><span data-stu-id="ed3a6-139">Request headers</span></span>
| <span data-ttu-id="ed3a6-140">名称</span><span class="sxs-lookup"><span data-stu-id="ed3a6-140">Name</span></span>       | <span data-ttu-id="ed3a6-141">类型</span><span class="sxs-lookup"><span data-stu-id="ed3a6-141">Type</span></span> | <span data-ttu-id="ed3a6-142">说明</span><span class="sxs-lookup"><span data-stu-id="ed3a6-142">Description</span></span> |
|:---------------|:--------|:--------|
| <span data-ttu-id="ed3a6-143">Authorization</span><span class="sxs-lookup"><span data-stu-id="ed3a6-143">Authorization</span></span>  | <span data-ttu-id="ed3a6-144">string</span><span class="sxs-lookup"><span data-stu-id="ed3a6-144">string</span></span> | <span data-ttu-id="ed3a6-p106">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="ed3a6-p106">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="ed3a6-147">Prefer: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="ed3a6-147">Prefer: outlook.timezone</span></span>  | <span data-ttu-id="ed3a6-148">string</span><span class="sxs-lookup"><span data-stu-id="ed3a6-148">string</span></span> | <span data-ttu-id="ed3a6-149">此选项可用于指定响应中开始时间和结束时间的时区。</span><span class="sxs-lookup"><span data-stu-id="ed3a6-149">Use this to specify the time zone for start and end times in the response.</span></span> <span data-ttu-id="ed3a6-150">如果未指定，返回的这些时间值采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="ed3a6-150">If not specified, those time values are returned in UTC.</span></span> <span data-ttu-id="ed3a6-151">可选。</span><span class="sxs-lookup"><span data-stu-id="ed3a6-151">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ed3a6-152">请求正文</span><span class="sxs-lookup"><span data-stu-id="ed3a6-152">Request body</span></span>
<span data-ttu-id="ed3a6-153">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="ed3a6-153">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ed3a6-154">响应</span><span class="sxs-lookup"><span data-stu-id="ed3a6-154">Response</span></span>

<span data-ttu-id="ed3a6-155">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [event](../resources/event.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="ed3a6-155">If successful, this method returns a `200 OK` response code and collection of [event](../resources/event.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="ed3a6-156">示例</span><span class="sxs-lookup"><span data-stu-id="ed3a6-156">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ed3a6-157">请求</span><span class="sxs-lookup"><span data-stu-id="ed3a6-157">Request</span></span>
<span data-ttu-id="ed3a6-158">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="ed3a6-158">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="ed3a6-159">HTTP</span><span class="sxs-lookup"><span data-stu-id="ed3a6-159">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_calendarview"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/calendar/calendarView?startDateTime=2017-01-01T19:00:00-08:00&endDateTime=2017-01-07T19:00:00-08:00
```
# <a name="c"></a>[<span data-ttu-id="ed3a6-160">C#</span><span class="sxs-lookup"><span data-stu-id="ed3a6-160">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-calendarview-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ed3a6-161">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ed3a6-161">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-calendarview-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ed3a6-162">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ed3a6-162">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-calendarview-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="ed3a6-163">响应</span><span class="sxs-lookup"><span data-stu-id="ed3a6-163">Response</span></span>
<span data-ttu-id="ed3a6-p108">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="ed3a6-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  ]
}
-->
