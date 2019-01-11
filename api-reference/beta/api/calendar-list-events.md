---
title: 列出事件
description: 检索日历中的事件列表。该列表包含单个实例会议和系列主控形状。
author: angelgolfer-ms
localization_priority: Normal
ms.openlocfilehash: 7d3f4110b33cb401126200eadc57c14fef379f9e
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27814229"
---
# <a name="list-events"></a><span data-ttu-id="6e3f6-104">列出事件</span><span class="sxs-lookup"><span data-stu-id="6e3f6-104">List events</span></span>

> <span data-ttu-id="6e3f6-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="6e3f6-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6e3f6-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="6e3f6-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="6e3f6-p103">检索日历中的事件列表。该列表包含单个实例会议和系列主控形状。</span><span class="sxs-lookup"><span data-stu-id="6e3f6-p103">Retrieve a list of events in a calendar.  The list contains single instance meetings and series masters.</span></span>

<span data-ttu-id="6e3f6-109">要获取扩展的事件实例，可以[获取日历视图](calendar-list-calendarview.md)，或者[获取事件的实例](event-list-instances.md)。</span><span class="sxs-lookup"><span data-stu-id="6e3f6-109">To get expanded event instances, you can [get the calendar view](calendar-list-calendarview.md), or [get the instances of an event](event-list-instances.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="6e3f6-110">权限</span><span class="sxs-lookup"><span data-stu-id="6e3f6-110">Permissions</span></span>
<span data-ttu-id="6e3f6-p104">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6e3f6-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6e3f6-113">权限类型</span><span class="sxs-lookup"><span data-stu-id="6e3f6-113">Permission type</span></span>      | <span data-ttu-id="6e3f6-114">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="6e3f6-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6e3f6-115">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6e3f6-115">Delegated (work or school account)</span></span> | <span data-ttu-id="6e3f6-116">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="6e3f6-116">Calendars.Read</span></span>    |
|<span data-ttu-id="6e3f6-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6e3f6-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6e3f6-118">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="6e3f6-118">Calendars.Read</span></span>    |
|<span data-ttu-id="6e3f6-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="6e3f6-119">Application</span></span> | <span data-ttu-id="6e3f6-120">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="6e3f6-120">Calendars.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="6e3f6-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6e3f6-121">HTTP request</span></span>
<span data-ttu-id="6e3f6-122"><!-- { "blockType": "ignored" } -->用户或组的默认[日历](../resources/calendar.md)。</span><span class="sxs-lookup"><span data-stu-id="6e3f6-122"><!-- { "blockType": "ignored" } --> A user's or group's default [calendar](../resources/calendar.md).</span></span>
```http
GET /me/calendar/events
GET /users/{id | userPrincipalName}/calendar/events
GET /groups/{id}/calendar/events
```
<span data-ttu-id="6e3f6-123">默认 [calendarGroup](../resources/calendargroup.md) 中的用户 [calendar](../resources/calendar.md)。</span><span class="sxs-lookup"><span data-stu-id="6e3f6-123">A user's [calendar](../resources/calendar.md) in the default [calendarGroup](../resources/calendargroup.md).</span></span>
```http
GET /me/calendars/{id}/events
GET /users/{id | userPrincipalName}/calendars/{id}/events

GET /me/calendarGroup/calendars/{id}/events
GET /users/{id | userPrincipalName}/calendarGroup/calendars/{id}/events
```
<span data-ttu-id="6e3f6-124">指定 [calendarGroup](../resources/calendargroup.md) 中用户的 [日历](../resources/calendar.md)。</span><span class="sxs-lookup"><span data-stu-id="6e3f6-124">A user's [calendar](../resources/calendar.md) in a specific [calendarGroup](../resources/calendargroup.md).</span></span>
```http
GET /me/calendarGroups/{id}/calendars/{id}/events
GET /users/{id | userPrincipalName}/calendarGroups/{id}/calendars/{id}/events
```
## <a name="optional-query-parameters"></a><span data-ttu-id="6e3f6-125">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="6e3f6-125">Optional query parameters</span></span>
<span data-ttu-id="6e3f6-126">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="6e3f6-126">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="6e3f6-127">请求标头</span><span class="sxs-lookup"><span data-stu-id="6e3f6-127">Request headers</span></span>
| <span data-ttu-id="6e3f6-128">名称</span><span class="sxs-lookup"><span data-stu-id="6e3f6-128">Name</span></span>       | <span data-ttu-id="6e3f6-129">类型</span><span class="sxs-lookup"><span data-stu-id="6e3f6-129">Type</span></span> | <span data-ttu-id="6e3f6-130">说明</span><span class="sxs-lookup"><span data-stu-id="6e3f6-130">Description</span></span> |
|:---------------|:--------|:--------|
| <span data-ttu-id="6e3f6-131">Authorization</span><span class="sxs-lookup"><span data-stu-id="6e3f6-131">Authorization</span></span>  | <span data-ttu-id="6e3f6-132">string</span><span class="sxs-lookup"><span data-stu-id="6e3f6-132">string</span></span> | <span data-ttu-id="6e3f6-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="6e3f6-p105">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="6e3f6-135">Prefer: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="6e3f6-135">Prefer: outlook.timezone</span></span>  | <span data-ttu-id="6e3f6-136">string</span><span class="sxs-lookup"><span data-stu-id="6e3f6-136">string</span></span> | <span data-ttu-id="6e3f6-137">此选项可用于指定响应中开始时间和结束时间的时区。</span><span class="sxs-lookup"><span data-stu-id="6e3f6-137">Use this to specify the time zone for start and end times in the response.</span></span> <span data-ttu-id="6e3f6-138">如果未指定，返回的这些时间值采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="6e3f6-138">If not specified, those time values are returned in UTC.</span></span> <span data-ttu-id="6e3f6-139">可选。</span><span class="sxs-lookup"><span data-stu-id="6e3f6-139">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6e3f6-140">请求正文</span><span class="sxs-lookup"><span data-stu-id="6e3f6-140">Request body</span></span>
<span data-ttu-id="6e3f6-141">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="6e3f6-141">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6e3f6-142">响应</span><span class="sxs-lookup"><span data-stu-id="6e3f6-142">Response</span></span>

<span data-ttu-id="6e3f6-143">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [Event](../resources/event.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="6e3f6-143">If successful, this method returns a `200 OK` response code and collection of [Event](../resources/event.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="6e3f6-144">示例</span><span class="sxs-lookup"><span data-stu-id="6e3f6-144">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6e3f6-145">请求</span><span class="sxs-lookup"><span data-stu-id="6e3f6-145">Request</span></span>
<span data-ttu-id="6e3f6-146">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="6e3f6-146">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_events"
}-->
```http
GET https://graph.microsoft.com/beta/me/calendar/events
```
##### <a name="response"></a><span data-ttu-id="6e3f6-147">响应</span><span class="sxs-lookup"><span data-stu-id="6e3f6-147">Response</span></span>
<span data-ttu-id="6e3f6-p107">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="6e3f6-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "List events",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
