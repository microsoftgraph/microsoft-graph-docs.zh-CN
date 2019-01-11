---
title: 列出实例
description: 获取指定的时间范围内的事件的实例 （匹配项）。 如果该事件是`SeriesMaster`类型，这将返回
localization_priority: Normal
ms.openlocfilehash: 79f6f5832a30f37a4f66e07eb44c2d31a39f7546
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27843440"
---
# <a name="list-instances"></a><span data-ttu-id="99f68-104">列表实例</span><span class="sxs-lookup"><span data-stu-id="99f68-104">List instances</span></span>

> <span data-ttu-id="99f68-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="99f68-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="99f68-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="99f68-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="99f68-p103">获取指定的时间范围的事件的实例（发生次数）。如果事件的类型是 `SeriesMaster`，这将返回在指定的时间范围内事件的发生次数和异常。</span><span class="sxs-lookup"><span data-stu-id="99f68-p103">Get the instances (occurrences) of an event for a specified time range. If the event is a `SeriesMaster` type, this returns the occurrences and exceptions of the event in the specified time range.</span></span>

## <a name="permissions"></a><span data-ttu-id="99f68-109">权限</span><span class="sxs-lookup"><span data-stu-id="99f68-109">Permissions</span></span>
<span data-ttu-id="99f68-p104">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="99f68-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="99f68-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="99f68-112">Permission type</span></span>      | <span data-ttu-id="99f68-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="99f68-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="99f68-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="99f68-114">Delegated (work or school account)</span></span> | <span data-ttu-id="99f68-115">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="99f68-115">Calendars.Read</span></span>    |
|<span data-ttu-id="99f68-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="99f68-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="99f68-117">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="99f68-117">Calendars.Read</span></span>    |
|<span data-ttu-id="99f68-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="99f68-118">Application</span></span> | <span data-ttu-id="99f68-119">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="99f68-119">Calendars.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="99f68-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="99f68-120">HTTP request</span></span>
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
## <a name="query-parameters"></a><span data-ttu-id="99f68-121">查询参数</span><span class="sxs-lookup"><span data-stu-id="99f68-121">Query parameters</span></span>

<span data-ttu-id="99f68-122">在请求 URL 中，提供以下必要查询参数的值。</span><span class="sxs-lookup"><span data-stu-id="99f68-122">In the request URL, provide the following required query parameters with values.</span></span>

| <span data-ttu-id="99f68-123">参数</span><span class="sxs-lookup"><span data-stu-id="99f68-123">Parameter</span></span>    | <span data-ttu-id="99f68-124">类型</span><span class="sxs-lookup"><span data-stu-id="99f68-124">Type</span></span>   |<span data-ttu-id="99f68-125">说明</span><span class="sxs-lookup"><span data-stu-id="99f68-125">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="99f68-126">startDateTime</span><span class="sxs-lookup"><span data-stu-id="99f68-126">startDateTime</span></span>|<span data-ttu-id="99f68-127">字符串</span><span class="sxs-lookup"><span data-stu-id="99f68-127">String</span></span>|<span data-ttu-id="99f68-p105">时间范围的开始日期和时间以 ISO 8601 格式表示。例如，“2015-11-08T19:00:00.0000000”。</span><span class="sxs-lookup"><span data-stu-id="99f68-p105">The start date and time of the time range, represented in ISO 8601 format. For example, "2015-11-08T19:00:00.0000000".</span></span>|
|<span data-ttu-id="99f68-130">endDateTime</span><span class="sxs-lookup"><span data-stu-id="99f68-130">endDateTime</span></span>|<span data-ttu-id="99f68-131">字符串</span><span class="sxs-lookup"><span data-stu-id="99f68-131">String</span></span>|<span data-ttu-id="99f68-p106">时间范围的结束日期和时间以 ISO 8601 格式表示。例如，“2015-11-08T20:00:00.0000000”。</span><span class="sxs-lookup"><span data-stu-id="99f68-p106">The end date and time of the time range, represented in ISO 8601 format. For example, "2015-11-08T20:00:00.0000000".</span></span>|

<span data-ttu-id="99f68-134">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="99f68-134">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="99f68-135">请求标头</span><span class="sxs-lookup"><span data-stu-id="99f68-135">Request headers</span></span>
| <span data-ttu-id="99f68-136">名称</span><span class="sxs-lookup"><span data-stu-id="99f68-136">Name</span></span>       | <span data-ttu-id="99f68-137">类型</span><span class="sxs-lookup"><span data-stu-id="99f68-137">Type</span></span> | <span data-ttu-id="99f68-138">说明</span><span class="sxs-lookup"><span data-stu-id="99f68-138">Description</span></span> |
|:---------------|:--------|:--------|
| <span data-ttu-id="99f68-139">Authorization</span><span class="sxs-lookup"><span data-stu-id="99f68-139">Authorization</span></span>  | <span data-ttu-id="99f68-140">string</span><span class="sxs-lookup"><span data-stu-id="99f68-140">string</span></span> | <span data-ttu-id="99f68-p107">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="99f68-p107">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="99f68-143">Prefer: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="99f68-143">Prefer: outlook.timezone</span></span>  | <span data-ttu-id="99f68-144">string</span><span class="sxs-lookup"><span data-stu-id="99f68-144">string</span></span> | <span data-ttu-id="99f68-145">此选项可用于指定响应中开始时间和结束时间的时区。</span><span class="sxs-lookup"><span data-stu-id="99f68-145">Use this to specify the time zone for start and end times in the response.</span></span> <span data-ttu-id="99f68-146">如果未指定，返回的这些时间值采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="99f68-146">If not specified, those time values are returned in UTC.</span></span> <span data-ttu-id="99f68-147">可选。</span><span class="sxs-lookup"><span data-stu-id="99f68-147">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="99f68-148">请求正文</span><span class="sxs-lookup"><span data-stu-id="99f68-148">Request body</span></span>
<span data-ttu-id="99f68-149">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="99f68-149">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="99f68-150">响应</span><span class="sxs-lookup"><span data-stu-id="99f68-150">Response</span></span>

<span data-ttu-id="99f68-151">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [Event](../resources/event.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="99f68-151">If successful, this method returns a `200 OK` response code and collection of [Event](../resources/event.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="99f68-152">示例</span><span class="sxs-lookup"><span data-stu-id="99f68-152">Example</span></span>
##### <a name="request"></a><span data-ttu-id="99f68-153">请求</span><span class="sxs-lookup"><span data-stu-id="99f68-153">Request</span></span>
<span data-ttu-id="99f68-154">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="99f68-154">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_instances"
}-->
```http
GET https://graph.microsoft.com/beta/me/events/{id}/instances
```
##### <a name="response"></a><span data-ttu-id="99f68-155">响应</span><span class="sxs-lookup"><span data-stu-id="99f68-155">Response</span></span>
<span data-ttu-id="99f68-p109">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="99f68-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "List instances",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
