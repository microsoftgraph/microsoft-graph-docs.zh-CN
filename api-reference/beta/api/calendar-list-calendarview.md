---
title: 列出 calendarView
description: 获取由时间范围定义的日历视图中的事件发生次数、异常和单个实例，
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: a2b16788e4c312816d2a8336f002e0a30fafb109
ms.sourcegitcommit: 2a601cffdb8df375b2ee32a1f35b8f71e0ffd04f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2020
ms.locfileid: "41023066"
---
# <a name="list-calendarview"></a><span data-ttu-id="5eed1-103">列出 calendarView</span><span class="sxs-lookup"><span data-stu-id="5eed1-103">List calendarView</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5eed1-104">从用户的默认日历 `(../me/calendarview)` 或其他一些日历中，获取由时间范围定义的日历视图中的事件发生次数、异常和单个实例。</span><span class="sxs-lookup"><span data-stu-id="5eed1-104">Get the occurrences, exceptions, and single instances of events in a calendar view defined by a time range, from a user's default calendar `(../me/calendarview)` or some other calendar of the user's.</span></span>

## <a name="permissions"></a><span data-ttu-id="5eed1-105">权限</span><span class="sxs-lookup"><span data-stu-id="5eed1-105">Permissions</span></span>
<span data-ttu-id="5eed1-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="5eed1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5eed1-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="5eed1-108">Permission type</span></span>      | <span data-ttu-id="5eed1-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="5eed1-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5eed1-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5eed1-110">Delegated (work or school account)</span></span> | <span data-ttu-id="5eed1-111">Calendars.Read、Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5eed1-111">Calendars.Read, Calendars.ReadWrite</span></span> |
|<span data-ttu-id="5eed1-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5eed1-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5eed1-113">Calendars.Read、Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5eed1-113">Calendars.Read, Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="5eed1-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="5eed1-114">Application</span></span> | <span data-ttu-id="5eed1-115">Calendars.Read、Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5eed1-115">Calendars.Read, Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="5eed1-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5eed1-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="5eed1-117">用户的默认 [calendar](../resources/calendar.md)。</span><span class="sxs-lookup"><span data-stu-id="5eed1-117">A user's default [calendar](../resources/calendar.md).</span></span>
```http
GET /me/calendar/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendar/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
```

<span data-ttu-id="5eed1-118">默认 [calendarGroup](../resources/calendargroup.md) 中的用户 [calendar](../resources/calendar.md)。</span><span class="sxs-lookup"><span data-stu-id="5eed1-118">A user's [calendar](../resources/calendar.md) in the default [calendarGroup](../resources/calendargroup.md).</span></span>
```http
GET /me/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}

GET /me/calendarGroup/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendarGroup/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
```

<span data-ttu-id="5eed1-119">指定 [calendarGroup](../resources/calendargroup.md) 中用户的 [日历](../resources/calendar.md)。</span><span class="sxs-lookup"><span data-stu-id="5eed1-119">A user's [calendar](../resources/calendar.md) in a specific [calendarGroup](../resources/calendargroup.md).</span></span>
```http
GET /me/calendarGroups/{id}/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendarGroups/{id}/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
```

## <a name="query-parameters"></a><span data-ttu-id="5eed1-120">查询参数</span><span class="sxs-lookup"><span data-stu-id="5eed1-120">Query parameters</span></span>

<span data-ttu-id="5eed1-121">在请求 URL 中，提供以下必要查询参数的值。</span><span class="sxs-lookup"><span data-stu-id="5eed1-121">In the request URL, provide the following required query parameters with values.</span></span>

| <span data-ttu-id="5eed1-122">参数</span><span class="sxs-lookup"><span data-stu-id="5eed1-122">Parameter</span></span>     | <span data-ttu-id="5eed1-123">类型</span><span class="sxs-lookup"><span data-stu-id="5eed1-123">Type</span></span>   | <span data-ttu-id="5eed1-124">说明</span><span class="sxs-lookup"><span data-stu-id="5eed1-124">Description</span></span>                                                                                                            |
|:--------------|:-------|:-----------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="5eed1-125">startDateTime</span><span class="sxs-lookup"><span data-stu-id="5eed1-125">startDateTime</span></span> | <span data-ttu-id="5eed1-126">String</span><span class="sxs-lookup"><span data-stu-id="5eed1-126">String</span></span> | <span data-ttu-id="5eed1-p102">时间范围的开始日期和时间，以 ISO 8601 格式表示。例如，"2019-11-08T19：00： 00-08： 00"。</span><span class="sxs-lookup"><span data-stu-id="5eed1-p102">The start date and time of the time range, represented in ISO 8601 format. For example, "2019-11-08T19:00:00-08:00".</span></span> |
| <span data-ttu-id="5eed1-129">endDateTime</span><span class="sxs-lookup"><span data-stu-id="5eed1-129">endDateTime</span></span>   | <span data-ttu-id="5eed1-130">String</span><span class="sxs-lookup"><span data-stu-id="5eed1-130">String</span></span> | <span data-ttu-id="5eed1-p103">时间范围的结束日期和时间，以 ISO 8601 格式表示。例如，"2019-11-08T20：00： 00-08： 00"。</span><span class="sxs-lookup"><span data-stu-id="5eed1-p103">The end date and time of the time range, represented in ISO 8601 format. For example, "2019-11-08T20:00:00-08:00".</span></span>   |

<span data-ttu-id="5eed1-133">`startDateTime`和的值使用`endDateTime`值中指定的时区偏移量进行解释，如果存在，则不受`Prefer: outlook.timezone`标头值的影响。</span><span class="sxs-lookup"><span data-stu-id="5eed1-133">The values of `startDateTime` and `endDateTime` are interpreted using the timezone offset specified in the value and are not impacted by the value of the `Prefer: outlook.timezone` header if present.</span></span> <span data-ttu-id="5eed1-134">如果值中不包含任何时区偏移量，则它将被解释为 UTC。</span><span class="sxs-lookup"><span data-stu-id="5eed1-134">If no timezone offset is included in the value, it is interpreted as UTC.</span></span>

<span data-ttu-id="5eed1-135">此方法还支持一些 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="5eed1-135">This method also supports some of the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

> [!NOTE]
> <span data-ttu-id="5eed1-136">[事件](../resources/event.md)的 **createdDateTime** 和 **lastModifiedDateTime** 属性不支持 `$select`。</span><span class="sxs-lookup"><span data-stu-id="5eed1-136">The **createdDateTime** and **lastModifiedDateTime** properties of [event](../resources/event.md) do not support `$select`.</span></span> <span data-ttu-id="5eed1-137">若要获取它们的值，只需在 **calendarView** 上进行查询，而不应用 `$select`。</span><span class="sxs-lookup"><span data-stu-id="5eed1-137">To get their values, simply query on **calendarView** without applying `$select`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5eed1-138">请求标头</span><span class="sxs-lookup"><span data-stu-id="5eed1-138">Request headers</span></span>
| <span data-ttu-id="5eed1-139">名称</span><span class="sxs-lookup"><span data-stu-id="5eed1-139">Name</span></span>       | <span data-ttu-id="5eed1-140">类型</span><span class="sxs-lookup"><span data-stu-id="5eed1-140">Type</span></span> | <span data-ttu-id="5eed1-141">说明</span><span class="sxs-lookup"><span data-stu-id="5eed1-141">Description</span></span> |
|:---------------|:--------|:--------|
| <span data-ttu-id="5eed1-142">Authorization</span><span class="sxs-lookup"><span data-stu-id="5eed1-142">Authorization</span></span>  | <span data-ttu-id="5eed1-143">string</span><span class="sxs-lookup"><span data-stu-id="5eed1-143">string</span></span> | <span data-ttu-id="5eed1-p106">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="5eed1-p106">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="5eed1-146">Prefer: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="5eed1-146">Prefer: outlook.timezone</span></span>  | <span data-ttu-id="5eed1-147">string</span><span class="sxs-lookup"><span data-stu-id="5eed1-147">string</span></span> | <span data-ttu-id="5eed1-148">此选项可用于指定响应中开始时间和结束时间的时区。</span><span class="sxs-lookup"><span data-stu-id="5eed1-148">Use this to specify the time zone for start and end times in the response.</span></span> <span data-ttu-id="5eed1-149">如果未指定，返回的这些时间值采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="5eed1-149">If not specified, those time values are returned in UTC.</span></span> <span data-ttu-id="5eed1-150">可选。</span><span class="sxs-lookup"><span data-stu-id="5eed1-150">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5eed1-151">请求正文</span><span class="sxs-lookup"><span data-stu-id="5eed1-151">Request body</span></span>
<span data-ttu-id="5eed1-152">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="5eed1-152">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5eed1-153">响应</span><span class="sxs-lookup"><span data-stu-id="5eed1-153">Response</span></span>

<span data-ttu-id="5eed1-154">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [event](../resources/event.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="5eed1-154">If successful, this method returns a `200 OK` response code and collection of [event](../resources/event.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="5eed1-155">示例</span><span class="sxs-lookup"><span data-stu-id="5eed1-155">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5eed1-156">请求</span><span class="sxs-lookup"><span data-stu-id="5eed1-156">Request</span></span>
<span data-ttu-id="5eed1-157">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="5eed1-157">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="5eed1-158">HTTP</span><span class="sxs-lookup"><span data-stu-id="5eed1-158">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_calendarview"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/calendar/calendarView?startDateTime=2017-01-01T19:00:00-08:00&endDateTime=2017-01-07T19:00:00-08:00
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="5eed1-159">C#</span><span class="sxs-lookup"><span data-stu-id="5eed1-159">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-calendarview-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="5eed1-160">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5eed1-160">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-calendarview-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="5eed1-161">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5eed1-161">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-calendarview-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="5eed1-162">响应</span><span class="sxs-lookup"><span data-stu-id="5eed1-162">Response</span></span>
<span data-ttu-id="5eed1-p108">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="5eed1-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
