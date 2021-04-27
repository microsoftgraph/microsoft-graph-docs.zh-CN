---
title: 列出 calendarView
description: 从用户的默认日历中，获取由时间范围定义的日历视图中的事件发生次数、异常和单个实例，
localization_priority: Normal
doc_type: apiPageType
author: harini84
ms.prod: outlook
ms.openlocfilehash: bd5d907e6511309ddb7389b5f3ea0e4cf950aca6
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52048888"
---
# <a name="list-calendarview"></a><span data-ttu-id="a7392-103">列出 calendarView</span><span class="sxs-lookup"><span data-stu-id="a7392-103">List calendarView</span></span>

<span data-ttu-id="a7392-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a7392-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a7392-105">从用户的默认日历或其他一些日历中，获取由时间范围定义的日历视图中的事件发生次数、异常和单个实例。</span><span class="sxs-lookup"><span data-stu-id="a7392-105">Get the occurrences, exceptions, and single instances of events in a calendar view defined by a time range, from the user's default calendar, or from some other calendar of the user's.</span></span>
## <a name="permissions"></a><span data-ttu-id="a7392-106">权限</span><span class="sxs-lookup"><span data-stu-id="a7392-106">Permissions</span></span>
<span data-ttu-id="a7392-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a7392-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a7392-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="a7392-109">Permission type</span></span>      | <span data-ttu-id="a7392-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a7392-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a7392-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a7392-111">Delegated (work or school account)</span></span> | <span data-ttu-id="a7392-112">Calendars.Read、Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a7392-112">Calendars.Read, Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="a7392-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a7392-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a7392-114">Calendars.Read、Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a7392-114">Calendars.Read, Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="a7392-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="a7392-115">Application</span></span> | <span data-ttu-id="a7392-116">Calendars.Read、Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a7392-116">Calendars.Read, Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="a7392-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a7392-117">HTTP request</span></span>
<span data-ttu-id="a7392-118">用户的默认 [calendar](../resources/calendar.md)。</span><span class="sxs-lookup"><span data-stu-id="a7392-118">A user's default [calendar](../resources/calendar.md).</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/calendar/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
```

<span data-ttu-id="a7392-119">默认 [calendarGroup](../resources/calendargroup.md) 中的用户 [calendar](../resources/calendar.md)。</span><span class="sxs-lookup"><span data-stu-id="a7392-119">A user's [calendar](../resources/calendar.md) in the default [calendarGroup](../resources/calendargroup.md).</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
```

<span data-ttu-id="a7392-120">指定 [calendarGroup](../resources/calendargroup.md) 中用户的 [日历](../resources/calendar.md)。</span><span class="sxs-lookup"><span data-stu-id="a7392-120">A user's [calendar](../resources/calendar.md) in a specific [calendarGroup](../resources/calendargroup.md).</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/calendarGroups/{id}/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendarGroups/{id}/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
```

## <a name="query-parameters"></a><span data-ttu-id="a7392-121">查询参数</span><span class="sxs-lookup"><span data-stu-id="a7392-121">Query parameters</span></span>

<span data-ttu-id="a7392-122">在请求 URL 中，提供以下必要查询参数的值。</span><span class="sxs-lookup"><span data-stu-id="a7392-122">In the request URL, provide the following required query parameters with values.</span></span>

| <span data-ttu-id="a7392-123">参数</span><span class="sxs-lookup"><span data-stu-id="a7392-123">Parameter</span></span>     | <span data-ttu-id="a7392-124">类型</span><span class="sxs-lookup"><span data-stu-id="a7392-124">Type</span></span>   | <span data-ttu-id="a7392-125">说明</span><span class="sxs-lookup"><span data-stu-id="a7392-125">Description</span></span>                                                                                                            |
|:--------------|:-------|:-----------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="a7392-126">startDateTime</span><span class="sxs-lookup"><span data-stu-id="a7392-126">startDateTime</span></span> | <span data-ttu-id="a7392-127">String</span><span class="sxs-lookup"><span data-stu-id="a7392-127">String</span></span> | <span data-ttu-id="a7392-p102">时间范围的开始日期和时间，以 ISO 8601 格式表示。例如，“2019-11-08T19:00:00-08:00”。</span><span class="sxs-lookup"><span data-stu-id="a7392-p102">The start date and time of the time range, represented in ISO 8601 format. For example, "2019-11-08T19:00:00-08:00".</span></span> |
| <span data-ttu-id="a7392-130">endDateTime</span><span class="sxs-lookup"><span data-stu-id="a7392-130">endDateTime</span></span>   | <span data-ttu-id="a7392-131">String</span><span class="sxs-lookup"><span data-stu-id="a7392-131">String</span></span> | <span data-ttu-id="a7392-p103">时间范围的结束日期和时间，以 ISO 8601 格式表示。例如，“2019-11-08T20:00:00-08:00”。</span><span class="sxs-lookup"><span data-stu-id="a7392-p103">The end date and time of the time range, represented in ISO 8601 format. For example, "2019-11-08T20:00:00-08:00".</span></span>   |

<span data-ttu-id="a7392-134">`startDateTime` 和 `endDateTime` 的值使用值中指定的时区偏移量进行解释，并且不受 `Prefer: outlook.timezone` 标头（若有）的值影响。</span><span class="sxs-lookup"><span data-stu-id="a7392-134">The values of `startDateTime` and `endDateTime` are interpreted using the timezone offset specified in the value and are not impacted by the value of the `Prefer: outlook.timezone` header if present.</span></span> <span data-ttu-id="a7392-135">如果值中未包含时区偏移量，则将其解释为 UTC。</span><span class="sxs-lookup"><span data-stu-id="a7392-135">If no timezone offset is included in the value, it is interpreted as UTC.</span></span>

<span data-ttu-id="a7392-136">此方法还支持一些 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="a7392-136">This method also supports some of the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

> [!NOTE]
> <span data-ttu-id="a7392-137">[事件](../resources/event.md)的 **createdDateTime** 和 **lastModifiedDateTime** 属性不支持 `$select`。</span><span class="sxs-lookup"><span data-stu-id="a7392-137">The **createdDateTime** and **lastModifiedDateTime** properties of [event](../resources/event.md) do not support `$select`.</span></span> <span data-ttu-id="a7392-138">若要获取它们的值，只需在 **calendarView** 上进行查询，而不应用 `$select`。</span><span class="sxs-lookup"><span data-stu-id="a7392-138">To get their values, simply query on **calendarView** without applying `$select`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a7392-139">请求标头</span><span class="sxs-lookup"><span data-stu-id="a7392-139">Request headers</span></span>
| <span data-ttu-id="a7392-140">名称</span><span class="sxs-lookup"><span data-stu-id="a7392-140">Name</span></span>       | <span data-ttu-id="a7392-141">类型</span><span class="sxs-lookup"><span data-stu-id="a7392-141">Type</span></span> | <span data-ttu-id="a7392-142">说明</span><span class="sxs-lookup"><span data-stu-id="a7392-142">Description</span></span> |
|:---------------|:--------|:--------|
| <span data-ttu-id="a7392-143">Authorization</span><span class="sxs-lookup"><span data-stu-id="a7392-143">Authorization</span></span>  | <span data-ttu-id="a7392-144">string</span><span class="sxs-lookup"><span data-stu-id="a7392-144">string</span></span> | <span data-ttu-id="a7392-p106">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="a7392-p106">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="a7392-147">Prefer: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="a7392-147">Prefer: outlook.timezone</span></span>  | <span data-ttu-id="a7392-148">string</span><span class="sxs-lookup"><span data-stu-id="a7392-148">string</span></span> | <span data-ttu-id="a7392-149">此选项可用于指定响应中开始时间和结束时间的时区。</span><span class="sxs-lookup"><span data-stu-id="a7392-149">Use this to specify the time zone for start and end times in the response.</span></span> <span data-ttu-id="a7392-150">如果未指定，返回的这些时间值采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="a7392-150">If not specified, those time values are returned in UTC.</span></span> <span data-ttu-id="a7392-151">可选。</span><span class="sxs-lookup"><span data-stu-id="a7392-151">Optional.</span></span> |
| <span data-ttu-id="a7392-152">Prefer: outlook.body-content-type</span><span class="sxs-lookup"><span data-stu-id="a7392-152">Prefer: outlook.body-content-type</span></span> | <span data-ttu-id="a7392-153">string</span><span class="sxs-lookup"><span data-stu-id="a7392-153">string</span></span> | <span data-ttu-id="a7392-154">要返回的 **body** 属性的格式。</span><span class="sxs-lookup"><span data-stu-id="a7392-154">The format of the **body** property to be returned in.</span></span> <span data-ttu-id="a7392-155">可取值为“text”或“html”。</span><span class="sxs-lookup"><span data-stu-id="a7392-155">Values can be "text" or "html".</span></span> <span data-ttu-id="a7392-156">如果指定此 `Preference-Applied` 头，返回 `Prefer` 头作为证明。</span><span class="sxs-lookup"><span data-stu-id="a7392-156">A `Preference-Applied` header is returned as confirmation if this `Prefer` header is specified.</span></span> <span data-ttu-id="a7392-157">如果未指定此头，采用 HTML 格式返回 **body** 属性。</span><span class="sxs-lookup"><span data-stu-id="a7392-157">If the header is not specified, the **body** property is returned in HTML format.</span></span> <span data-ttu-id="a7392-158">可选。</span><span class="sxs-lookup"><span data-stu-id="a7392-158">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a7392-159">请求正文</span><span class="sxs-lookup"><span data-stu-id="a7392-159">Request body</span></span>
<span data-ttu-id="a7392-160">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="a7392-160">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a7392-161">响应</span><span class="sxs-lookup"><span data-stu-id="a7392-161">Response</span></span>

<span data-ttu-id="a7392-162">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [event](../resources/event.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="a7392-162">If successful, this method returns a `200 OK` response code and collection of [event](../resources/event.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="a7392-163">示例</span><span class="sxs-lookup"><span data-stu-id="a7392-163">Example</span></span>
### <a name="request"></a><span data-ttu-id="a7392-164">请求</span><span class="sxs-lookup"><span data-stu-id="a7392-164">Request</span></span>
<span data-ttu-id="a7392-165">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="a7392-165">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="a7392-166">HTTP</span><span class="sxs-lookup"><span data-stu-id="a7392-166">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_get_calendarview"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/calendarView?startDateTime=2020-01-01T19:00:00-08:00&endDateTime=2020-01-02T19:00:00-08:00
```
# <a name="c"></a>[<span data-ttu-id="a7392-167">C#</span><span class="sxs-lookup"><span data-stu-id="a7392-167">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-get-calendarview-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a7392-168">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a7392-168">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-get-calendarview-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a7392-169">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a7392-169">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-get-calendarview-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a7392-170">Java</span><span class="sxs-lookup"><span data-stu-id="a7392-170">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/user-get-calendarview-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="a7392-171">响应</span><span class="sxs-lookup"><span data-stu-id="a7392-171">Response</span></span>
<span data-ttu-id="a7392-172">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="a7392-172">Here is an example of the response.</span></span> <span data-ttu-id="a7392-173">注意：为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="a7392-173">Note: The response object shown here might be shortened for readability.</span></span>
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
      "originalStartTimeZone": "Pacific Standard Time",
      "originalEndTimeZone": "Pacific Standard Time",
      "responseStatus": {
        "response": "accepted",
        "time": "2016-10-19T10:37:00Z"
      },
      "uid": "040000008200E00074C5B7101A82E00800000000D3D70B8A6A17D70100000000000000001000000074665914A06C3F49BB4B7D7EEE4304DA",
      "reminderMinutesBeforeStart": 15,
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
