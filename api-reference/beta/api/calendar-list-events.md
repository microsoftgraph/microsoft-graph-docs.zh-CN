---
title: 列出事件
description: 检索日历中的事件列表。该列表包含单实例会议和系列主控事件。
author: harini84
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 1f1a292024772c2504bd4b72231e4154a4679abc
ms.sourcegitcommit: a9f0fde9924ad184d315bb2de43c2610002409f3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/30/2020
ms.locfileid: "48313114"
---
# <a name="list-events"></a><span data-ttu-id="8e79a-104">列出事件</span><span class="sxs-lookup"><span data-stu-id="8e79a-104">List events</span></span>

<span data-ttu-id="8e79a-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8e79a-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8e79a-106">检索日历中的事件列表。</span><span class="sxs-lookup"><span data-stu-id="8e79a-106">Retrieve a list of events in a calendar.</span></span>  <span data-ttu-id="8e79a-107">可以是[用户](../resources/user.md)的日历，也可以是 Microsoft 365 [组](../resources/group.md)的默认日历。</span><span class="sxs-lookup"><span data-stu-id="8e79a-107">The calendar can be one for a [user](../resources/user.md), or the default calendar of a Microsoft 365 [group](../resources/group.md).</span></span> <span data-ttu-id="8e79a-108">事件列表包含单个实例会议和系列母版。</span><span class="sxs-lookup"><span data-stu-id="8e79a-108">The list of events contains single instance meetings and series masters.</span></span>

<span data-ttu-id="8e79a-109">要获取扩展的事件实例，可以[获取日历视图](calendar-list-calendarview.md)，或者[获取事件的实例](event-list-instances.md)。</span><span class="sxs-lookup"><span data-stu-id="8e79a-109">To get expanded event instances, you can [get the calendar view](calendar-list-calendarview.md), or [get the instances of an event](event-list-instances.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="8e79a-110">权限</span><span class="sxs-lookup"><span data-stu-id="8e79a-110">Permissions</span></span>
<span data-ttu-id="8e79a-111">根据事件所处的日历类型和所请求的权限类型（委派型或应用程序），需要下列某一权限来调用此 API。</span><span class="sxs-lookup"><span data-stu-id="8e79a-111">Depending on the type of calendar that the events are in and the permission type (delegated or application) requested, one of the following permissions is required to call this API.</span></span> <span data-ttu-id="8e79a-112">要了解详细信息（包括如何选择权限），请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8e79a-112">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="8e79a-113">日历</span><span class="sxs-lookup"><span data-stu-id="8e79a-113">Calendar</span></span> | <span data-ttu-id="8e79a-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8e79a-114">Delegated (work or school account)</span></span> | <span data-ttu-id="8e79a-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8e79a-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8e79a-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="8e79a-116">Application</span></span> |
|:-----|:-----|:-----|:-----|
| <span data-ttu-id="8e79a-117">用户日历</span><span class="sxs-lookup"><span data-stu-id="8e79a-117">user calendar</span></span> | <span data-ttu-id="8e79a-118">Calendars.Read、Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8e79a-118">Calendars.Read, Calendars.ReadWrite</span></span> | <span data-ttu-id="8e79a-119">Calendars.Read、Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8e79a-119">Calendars.Read, Calendars.ReadWrite</span></span> | <span data-ttu-id="8e79a-120">Calendars.Read、Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8e79a-120">Calendars.Read, Calendars.ReadWrite</span></span> |
| <span data-ttu-id="8e79a-121">组日历</span><span class="sxs-lookup"><span data-stu-id="8e79a-121">group calendar</span></span> | <span data-ttu-id="8e79a-122">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8e79a-122">Group.Read.All, Group.ReadWrite.All</span></span> | <span data-ttu-id="8e79a-123">不支持。</span><span class="sxs-lookup"><span data-stu-id="8e79a-123">Not supported.</span></span> | <span data-ttu-id="8e79a-124">不支持。</span><span class="sxs-lookup"><span data-stu-id="8e79a-124">Not supported.</span></span> |


## <a name="http-request"></a><span data-ttu-id="8e79a-125">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8e79a-125">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="8e79a-126">用户或组的默认 [日历](../resources/calendar.md)。</span><span class="sxs-lookup"><span data-stu-id="8e79a-126">A user's or group's default [calendar](../resources/calendar.md).</span></span>
```http
GET /me/calendar/events
GET /users/{id | userPrincipalName}/calendar/events
GET /groups/{id}/calendar/events
```
<span data-ttu-id="8e79a-127">默认 [calendarGroup](../resources/calendargroup.md) 中用户的 [日历](../resources/calendar.md)。</span><span class="sxs-lookup"><span data-stu-id="8e79a-127">A user's [calendar](../resources/calendar.md) in the default [calendarGroup](../resources/calendargroup.md).</span></span>
```http
GET /me/calendars/{id}/events
GET /users/{id | userPrincipalName}/calendars/{id}/events

GET /me/calendarGroup/calendars/{id}/events
GET /users/{id | userPrincipalName}/calendarGroup/calendars/{id}/events
```
<span data-ttu-id="8e79a-128">指定 [calendarGroup](../resources/calendargroup.md) 中用户的 [日历](../resources/calendar.md)。</span><span class="sxs-lookup"><span data-stu-id="8e79a-128">A user's [calendar](../resources/calendar.md) in a specific [calendarGroup](../resources/calendargroup.md).</span></span>
```http
GET /me/calendarGroups/{id}/calendars/{id}/events
GET /users/{id | userPrincipalName}/calendarGroups/{id}/calendars/{id}/events
```
## <a name="optional-query-parameters"></a><span data-ttu-id="8e79a-129">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="8e79a-129">Optional query parameters</span></span>
<span data-ttu-id="8e79a-130">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="8e79a-130">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="8e79a-131">请求标头</span><span class="sxs-lookup"><span data-stu-id="8e79a-131">Request headers</span></span>
| <span data-ttu-id="8e79a-132">名称</span><span class="sxs-lookup"><span data-stu-id="8e79a-132">Name</span></span>       | <span data-ttu-id="8e79a-133">类型</span><span class="sxs-lookup"><span data-stu-id="8e79a-133">Type</span></span> | <span data-ttu-id="8e79a-134">说明</span><span class="sxs-lookup"><span data-stu-id="8e79a-134">Description</span></span> |
|:---------------|:--------|:--------|
| <span data-ttu-id="8e79a-135">Authorization</span><span class="sxs-lookup"><span data-stu-id="8e79a-135">Authorization</span></span>  | <span data-ttu-id="8e79a-136">string</span><span class="sxs-lookup"><span data-stu-id="8e79a-136">string</span></span> | <span data-ttu-id="8e79a-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="8e79a-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="8e79a-139">Prefer: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="8e79a-139">Prefer: outlook.timezone</span></span>  | <span data-ttu-id="8e79a-140">string</span><span class="sxs-lookup"><span data-stu-id="8e79a-140">string</span></span> | <span data-ttu-id="8e79a-141">此选项可用于指定响应中开始时间和结束时间的时区。</span><span class="sxs-lookup"><span data-stu-id="8e79a-141">Use this to specify the time zone for start and end times in the response.</span></span> <span data-ttu-id="8e79a-142">如果未指定，返回的这些时间值采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="8e79a-142">If not specified, those time values are returned in UTC.</span></span> <span data-ttu-id="8e79a-143">可选。</span><span class="sxs-lookup"><span data-stu-id="8e79a-143">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8e79a-144">请求正文</span><span class="sxs-lookup"><span data-stu-id="8e79a-144">Request body</span></span>
<span data-ttu-id="8e79a-145">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="8e79a-145">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8e79a-146">响应</span><span class="sxs-lookup"><span data-stu-id="8e79a-146">Response</span></span>

<span data-ttu-id="8e79a-147">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [Event](../resources/event.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="8e79a-147">If successful, this method returns a `200 OK` response code and collection of [Event](../resources/event.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="8e79a-148">示例</span><span class="sxs-lookup"><span data-stu-id="8e79a-148">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8e79a-149">请求</span><span class="sxs-lookup"><span data-stu-id="8e79a-149">Request</span></span>
<span data-ttu-id="8e79a-150">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="8e79a-150">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="8e79a-151">HTTP</span><span class="sxs-lookup"><span data-stu-id="8e79a-151">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "calendar_get_events"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/calendar/events
```
# <a name="c"></a>[<span data-ttu-id="8e79a-152">C#</span><span class="sxs-lookup"><span data-stu-id="8e79a-152">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/calendar-get-events-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8e79a-153">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8e79a-153">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/calendar-get-events-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8e79a-154">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8e79a-154">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/calendar-get-events-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="8e79a-155">响应</span><span class="sxs-lookup"><span data-stu-id="8e79a-155">Response</span></span>
<span data-ttu-id="8e79a-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="8e79a-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "List events",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->