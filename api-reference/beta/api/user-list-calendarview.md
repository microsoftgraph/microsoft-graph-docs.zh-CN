---
title: 列出 calendarView
description: 从用户的默认日历中，获取由时间范围定义的日历视图中的事件发生次数、异常和单个实例，
localization_priority: Normal
doc_type: apiPageType
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 9ec7e3ab963bca6b2710b17cf9c5777ef04bb349
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36362285"
---
# <a name="list-calendarview"></a><span data-ttu-id="da71d-103">列出 calendarView</span><span class="sxs-lookup"><span data-stu-id="da71d-103">List calendarView</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="da71d-104">从用户的默认日历或其他一些日历中，获取由时间范围定义的日历视图中的事件发生次数、异常和单个实例。</span><span class="sxs-lookup"><span data-stu-id="da71d-104">Get the occurrences, exceptions, and single instances of events in a calendar view defined by a time range, from the user's default calendar, or from some other calendar of the user's.</span></span>
## <a name="permissions"></a><span data-ttu-id="da71d-105">权限</span><span class="sxs-lookup"><span data-stu-id="da71d-105">Permissions</span></span>
<span data-ttu-id="da71d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="da71d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="da71d-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="da71d-108">Permission type</span></span>      | <span data-ttu-id="da71d-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="da71d-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="da71d-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="da71d-110">Delegated (work or school account)</span></span> | <span data-ttu-id="da71d-111">Calendars.Read、Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="da71d-111">Calendars.Read, Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="da71d-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="da71d-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="da71d-113">Calendars.Read、Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="da71d-113">Calendars.Read, Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="da71d-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="da71d-114">Application</span></span> | <span data-ttu-id="da71d-115">Calendars.Read、Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="da71d-115">Calendars.Read, Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="da71d-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="da71d-116">HTTP request</span></span>
<span data-ttu-id="da71d-117">用户的默认 [calendar](../resources/calendar.md)。</span><span class="sxs-lookup"><span data-stu-id="da71d-117">A user's default [calendar](../resources/calendar.md).</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/calendar/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
```

<span data-ttu-id="da71d-118">默认 [calendarGroup](../resources/calendargroup.md) 中的用户 [calendar](../resources/calendar.md)。</span><span class="sxs-lookup"><span data-stu-id="da71d-118">A user's [calendar](../resources/calendar.md) in the default [calendarGroup](../resources/calendargroup.md).</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}

GET /me/calendarGroup/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendarGroup/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
```

<span data-ttu-id="da71d-119">指定 [calendarGroup](../resources/calendargroup.md) 中用户的 [日历](../resources/calendar.md)。</span><span class="sxs-lookup"><span data-stu-id="da71d-119">A user's [calendar](../resources/calendar.md) in a specific [calendarGroup](../resources/calendargroup.md).</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/calendarGroups/{id}/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendarGroups/{id}/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
```

## <a name="query-parameters"></a><span data-ttu-id="da71d-120">查询参数</span><span class="sxs-lookup"><span data-stu-id="da71d-120">Query parameters</span></span>

<span data-ttu-id="da71d-121">在请求 URL 中，提供以下必要查询参数的值。</span><span class="sxs-lookup"><span data-stu-id="da71d-121">In the request URL, provide the following required query parameters with values.</span></span>

| <span data-ttu-id="da71d-122">参数</span><span class="sxs-lookup"><span data-stu-id="da71d-122">Parameter</span></span>    | <span data-ttu-id="da71d-123">类型</span><span class="sxs-lookup"><span data-stu-id="da71d-123">Type</span></span>   |<span data-ttu-id="da71d-124">说明</span><span class="sxs-lookup"><span data-stu-id="da71d-124">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="da71d-125">startDateTime</span><span class="sxs-lookup"><span data-stu-id="da71d-125">startDateTime</span></span>|<span data-ttu-id="da71d-126">String</span><span class="sxs-lookup"><span data-stu-id="da71d-126">String</span></span>|<span data-ttu-id="da71d-p102">时间范围的开始日期和时间以 ISO 8601 格式表示。例如，“2015-11-08T19:00:00.0000000”。</span><span class="sxs-lookup"><span data-stu-id="da71d-p102">The start date and time of the time range, represented in ISO 8601 format. For example, "2015-11-08T19:00:00.0000000".</span></span>|
|<span data-ttu-id="da71d-129">endDateTime</span><span class="sxs-lookup"><span data-stu-id="da71d-129">endDateTime</span></span>|<span data-ttu-id="da71d-130">String</span><span class="sxs-lookup"><span data-stu-id="da71d-130">String</span></span>|<span data-ttu-id="da71d-p103">时间范围的结束日期和时间以 ISO 8601 格式表示。例如，“2015-11-08T20:00:00.0000000”。</span><span class="sxs-lookup"><span data-stu-id="da71d-p103">The end date and time of the time range, represented in ISO 8601 format. For example, "2015-11-08T20:00:00.0000000".</span></span>|

<span data-ttu-id="da71d-133">此方法还支持某些[OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters)来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="da71d-133">This method also supports some of the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

> [!NOTE] 
> <span data-ttu-id="da71d-134">[事件](../resources/event.md)的`$select` **createdDateTime**和**lastModifiedDateTime**属性不支持。</span><span class="sxs-lookup"><span data-stu-id="da71d-134">The **createdDateTime** and **lastModifiedDateTime** properties of [event](../resources/event.md) do not support `$select`.</span></span> <span data-ttu-id="da71d-135">若要获取它们的值, 只\*\*\*\* 需查询 calendarView `$select`而无需应用。</span><span class="sxs-lookup"><span data-stu-id="da71d-135">To get their values, simply query on **calendarView** without applying `$select`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="da71d-136">请求标头</span><span class="sxs-lookup"><span data-stu-id="da71d-136">Request headers</span></span>
| <span data-ttu-id="da71d-137">名称</span><span class="sxs-lookup"><span data-stu-id="da71d-137">Name</span></span>       | <span data-ttu-id="da71d-138">类型</span><span class="sxs-lookup"><span data-stu-id="da71d-138">Type</span></span> | <span data-ttu-id="da71d-139">说明</span><span class="sxs-lookup"><span data-stu-id="da71d-139">Description</span></span> |
|:---------------|:--------|:--------|
| <span data-ttu-id="da71d-140">Authorization</span><span class="sxs-lookup"><span data-stu-id="da71d-140">Authorization</span></span>  | <span data-ttu-id="da71d-141">字符串</span><span class="sxs-lookup"><span data-stu-id="da71d-141">string</span></span> | <span data-ttu-id="da71d-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="da71d-p105">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="da71d-144">Prefer: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="da71d-144">Prefer: outlook.timezone</span></span>  | <span data-ttu-id="da71d-145">string</span><span class="sxs-lookup"><span data-stu-id="da71d-145">string</span></span> | <span data-ttu-id="da71d-146">此选项可用于指定响应中开始时间和结束时间的时区。</span><span class="sxs-lookup"><span data-stu-id="da71d-146">Use this to specify the time zone for start and end times in the response.</span></span> <span data-ttu-id="da71d-147">如果未指定，返回的这些时间值采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="da71d-147">If not specified, those time values are returned in UTC.</span></span> <span data-ttu-id="da71d-148">可选。</span><span class="sxs-lookup"><span data-stu-id="da71d-148">Optional.</span></span> |
| <span data-ttu-id="da71d-149">Prefer: outlook.body-content-type</span><span class="sxs-lookup"><span data-stu-id="da71d-149">Prefer: outlook.body-content-type</span></span> | <span data-ttu-id="da71d-150">string</span><span class="sxs-lookup"><span data-stu-id="da71d-150">string</span></span> | <span data-ttu-id="da71d-151">要返回的 **body** 属性的格式。</span><span class="sxs-lookup"><span data-stu-id="da71d-151">The format of the **body** property to be returned in.</span></span> <span data-ttu-id="da71d-152">可取值为“text”或“html”。</span><span class="sxs-lookup"><span data-stu-id="da71d-152">Values can be "text" or "html".</span></span> <span data-ttu-id="da71d-153">如果指定此 `Preference-Applied` 头，返回 `Prefer` 头作为证明。</span><span class="sxs-lookup"><span data-stu-id="da71d-153">A `Preference-Applied` header is returned as confirmation if this `Prefer` header is specified.</span></span> <span data-ttu-id="da71d-154">如果未指定此头，采用 HTML 格式返回 **body** 属性。</span><span class="sxs-lookup"><span data-stu-id="da71d-154">If the header is not specified, the **body** property is returned in HTML format.</span></span> <span data-ttu-id="da71d-155">可选。</span><span class="sxs-lookup"><span data-stu-id="da71d-155">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="da71d-156">请求正文</span><span class="sxs-lookup"><span data-stu-id="da71d-156">Request body</span></span>
<span data-ttu-id="da71d-157">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="da71d-157">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="da71d-158">响应</span><span class="sxs-lookup"><span data-stu-id="da71d-158">Response</span></span>

<span data-ttu-id="da71d-159">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [event](../resources/event.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="da71d-159">If successful, this method returns a `200 OK` response code and collection of [event](../resources/event.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="da71d-160">示例</span><span class="sxs-lookup"><span data-stu-id="da71d-160">Example</span></span>
##### <a name="request"></a><span data-ttu-id="da71d-161">请求</span><span class="sxs-lookup"><span data-stu-id="da71d-161">Request</span></span>
<span data-ttu-id="da71d-162">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="da71d-162">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="da71d-163">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="da71d-163">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_get_calendarview"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/calendarView?startDateTime=2016-01-01T19:00:00.0000000&endDateTime=2016-10-01T19:00:00.0000000
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="da71d-164">C#</span><span class="sxs-lookup"><span data-stu-id="da71d-164">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-get-calendarview-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="da71d-165">JavaScript</span><span class="sxs-lookup"><span data-stu-id="da71d-165">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-get-calendarview-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="da71d-166">目标-C</span><span class="sxs-lookup"><span data-stu-id="da71d-166">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-get-calendarview-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="da71d-167">Java</span><span class="sxs-lookup"><span data-stu-id="da71d-167">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/user-get-calendarview-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="da71d-168">响应</span><span class="sxs-lookup"><span data-stu-id="da71d-168">Response</span></span>
<span data-ttu-id="da71d-p108">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="da71d-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "List calendarView",
  "keywords": "calendar",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
