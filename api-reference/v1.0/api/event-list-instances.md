---
title: 列出实例
description: '获取指定的时间范围内的事件的实例 （匹配项）。 如果该事件是`SeriesMaster`类型，这将返回 '
localization_priority: Normal
ms.openlocfilehash: 194d911b6c5ea05eb0d3f797287773c516da9ee3
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27811394"
---
# <a name="list-instances"></a><span data-ttu-id="c826c-104">列出实例</span><span class="sxs-lookup"><span data-stu-id="c826c-104">List instances</span></span>

<span data-ttu-id="c826c-p102">获取指定的时间范围的事件的实例（发生次数）。如果事件的类型是 `SeriesMaster`，这将返回在指定的时间范围内事件的发生次数和异常。</span><span class="sxs-lookup"><span data-stu-id="c826c-p102">Get the instances (occurrences) of an event for a specified time range. If the event is a `SeriesMaster` type, this returns the occurrences and exceptions of the event in the specified time range.</span></span>

## <a name="permissions"></a><span data-ttu-id="c826c-107">权限</span><span class="sxs-lookup"><span data-stu-id="c826c-107">Permissions</span></span>
<span data-ttu-id="c826c-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c826c-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c826c-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="c826c-110">Permission type</span></span>      | <span data-ttu-id="c826c-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c826c-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c826c-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c826c-112">Delegated (work or school account)</span></span> | <span data-ttu-id="c826c-113">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="c826c-113">Calendars.Read</span></span>    |
|<span data-ttu-id="c826c-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c826c-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c826c-115">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="c826c-115">Calendars.Read</span></span>    |
|<span data-ttu-id="c826c-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="c826c-116">Application</span></span> | <span data-ttu-id="c826c-117">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="c826c-117">Calendars.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="c826c-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c826c-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/events/{id}/instances?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/events/{id}/instances?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /groups/{id}/events/{id}/instances?startDateTime={start_datetime}&endDateTime={end_datetime}

GET /me/calendar/events/{id}/instances?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendar/events/{id}/instances?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /groups/{id}/calendar/events/{id}/instances?startDateTime={start_datetime}&endDateTime={end_datetime}

GET /me/calendars/{id}/events/{id}/instances?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendars/{id}/events/{id}/instances?startDateTime={start_datetime}&endDateTime={end_datetime}

GET /me/calendargroup/calendars/{id}/events/{id}/instances?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendargroup/calendars/{id}/events/{id}/instances?startDateTime={start_datetime}&endDateTime={end_datetime}

GET /me/calendargroups/{id}/calendars/{id}/events/{id}/instances?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendargroups/{id}/calendars/{id}/events/{id}/instances?startDateTime={start_datetime}&endDateTime={end_datetime}
```
## <a name="query-parameters"></a><span data-ttu-id="c826c-119">查询参数</span><span class="sxs-lookup"><span data-stu-id="c826c-119">Query parameters</span></span>

<span data-ttu-id="c826c-120">在请求 URL 中，提供以下必要查询参数的值。</span><span class="sxs-lookup"><span data-stu-id="c826c-120">In the request URL, provide the following required query parameters with values.</span></span>

| <span data-ttu-id="c826c-121">参数</span><span class="sxs-lookup"><span data-stu-id="c826c-121">Parameter</span></span>    | <span data-ttu-id="c826c-122">类型</span><span class="sxs-lookup"><span data-stu-id="c826c-122">Type</span></span>   |<span data-ttu-id="c826c-123">说明</span><span class="sxs-lookup"><span data-stu-id="c826c-123">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c826c-124">startDateTime</span><span class="sxs-lookup"><span data-stu-id="c826c-124">startDateTime</span></span>|<span data-ttu-id="c826c-125">字符串</span><span class="sxs-lookup"><span data-stu-id="c826c-125">String</span></span>|<span data-ttu-id="c826c-p104">时间范围的开始日期和时间以 ISO 8601 格式表示。例如，“2015-11-08T19:00:00.0000000”。</span><span class="sxs-lookup"><span data-stu-id="c826c-p104">The start date and time of the time range, represented in ISO 8601 format. For example, "2015-11-08T19:00:00.0000000".</span></span>|
|<span data-ttu-id="c826c-128">endDateTime</span><span class="sxs-lookup"><span data-stu-id="c826c-128">endDateTime</span></span>|<span data-ttu-id="c826c-129">字符串</span><span class="sxs-lookup"><span data-stu-id="c826c-129">String</span></span>|<span data-ttu-id="c826c-p105">时间范围的结束日期和时间以 ISO 8601 格式表示。例如，“2015-11-08T20:00:00.0000000”。</span><span class="sxs-lookup"><span data-stu-id="c826c-p105">The end date and time of the time range, represented in ISO 8601 format. For example, "2015-11-08T20:00:00.0000000".</span></span>|

<span data-ttu-id="c826c-132">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="c826c-132">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="c826c-133">请求标头</span><span class="sxs-lookup"><span data-stu-id="c826c-133">Request headers</span></span>
| <span data-ttu-id="c826c-134">名称</span><span class="sxs-lookup"><span data-stu-id="c826c-134">Name</span></span>       | <span data-ttu-id="c826c-135">类型</span><span class="sxs-lookup"><span data-stu-id="c826c-135">Type</span></span> | <span data-ttu-id="c826c-136">说明</span><span class="sxs-lookup"><span data-stu-id="c826c-136">Description</span></span> |
|:---------------|:--------|:--------|
| <span data-ttu-id="c826c-137">Authorization</span><span class="sxs-lookup"><span data-stu-id="c826c-137">Authorization</span></span>  | <span data-ttu-id="c826c-138">string</span><span class="sxs-lookup"><span data-stu-id="c826c-138">string</span></span> | <span data-ttu-id="c826c-p106">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="c826c-p106">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="c826c-141">Prefer: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="c826c-141">Prefer: outlook.timezone</span></span>  | <span data-ttu-id="c826c-142">string</span><span class="sxs-lookup"><span data-stu-id="c826c-142">string</span></span> | <span data-ttu-id="c826c-143">此选项可用于指定响应中开始时间和结束时间的时区。</span><span class="sxs-lookup"><span data-stu-id="c826c-143">Use this to specify the time zone for start and end times in the response.</span></span> <span data-ttu-id="c826c-144">如果未指定，返回的这些时间值采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="c826c-144">If not specified, those time values are returned in UTC.</span></span> <span data-ttu-id="c826c-145">可选。</span><span class="sxs-lookup"><span data-stu-id="c826c-145">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c826c-146">请求正文</span><span class="sxs-lookup"><span data-stu-id="c826c-146">Request body</span></span>
<span data-ttu-id="c826c-147">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="c826c-147">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c826c-148">响应</span><span class="sxs-lookup"><span data-stu-id="c826c-148">Response</span></span>

<span data-ttu-id="c826c-149">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [Event](../resources/event.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="c826c-149">If successful, this method returns a `200 OK` response code and collection of [Event](../resources/event.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="c826c-150">示例</span><span class="sxs-lookup"><span data-stu-id="c826c-150">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c826c-151">请求</span><span class="sxs-lookup"><span data-stu-id="c826c-151">Request</span></span>
<span data-ttu-id="c826c-152">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="c826c-152">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_instances"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/events/{id}/instances
```
##### <a name="response"></a><span data-ttu-id="c826c-153">响应</span><span class="sxs-lookup"><span data-stu-id="c826c-153">Response</span></span>
<span data-ttu-id="c826c-p108">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="c826c-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "List instances",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
