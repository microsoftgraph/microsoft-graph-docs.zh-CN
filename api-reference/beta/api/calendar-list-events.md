---
title: 列出事件
description: 检索日历中的事件列表。该列表包含单实例会议和系列主控事件。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 20393a541505ddc5e1640cbcc6738efa3d32d05d
ms.sourcegitcommit: eb5f63deafcdd6db44e791f2d1f4c46604ab06fc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/07/2019
ms.locfileid: "36245618"
---
# <a name="list-events"></a><span data-ttu-id="d455f-104">列出事件</span><span class="sxs-lookup"><span data-stu-id="d455f-104">List events</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d455f-105">检索日历中的事件列表。</span><span class="sxs-lookup"><span data-stu-id="d455f-105">Retrieve a list of events in a calendar.</span></span>  <span data-ttu-id="d455f-106">可以是[用户](../resources/user.md)的日历，也可以是 Office 365 [组](../resources/group.md)的默认日历。</span><span class="sxs-lookup"><span data-stu-id="d455f-106">The calendar can be one for a [user](../resources/user.md), or the default calendar of an Office 365 [group](../resources/group.md).</span></span> <span data-ttu-id="d455f-107">事件列表包含单实例会议和系列主控形状。</span><span class="sxs-lookup"><span data-stu-id="d455f-107">The list of events contains single instance meetings and series masters.</span></span>

<span data-ttu-id="d455f-108">要获取扩展的事件实例，可以[获取日历视图](calendar-list-calendarview.md)，或者[获取事件的实例](event-list-instances.md)。</span><span class="sxs-lookup"><span data-stu-id="d455f-108">To get expanded event instances, you can [get the calendar view](calendar-list-calendarview.md), or [get the instances of an event](event-list-instances.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="d455f-109">权限</span><span class="sxs-lookup"><span data-stu-id="d455f-109">Permissions</span></span>
<span data-ttu-id="d455f-110">根据事件所在的日历类型以及请求的权限类型 (委派或应用程序), 需要以下权限之一才能调用此 API。</span><span class="sxs-lookup"><span data-stu-id="d455f-110">Depending on the type of calendar that the events are in and the permission type (delegated or application) requested, one of the following permissions is required to call this API.</span></span> <span data-ttu-id="d455f-111">若要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d455f-111">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d455f-112">日历</span><span class="sxs-lookup"><span data-stu-id="d455f-112">Calendar</span></span> | <span data-ttu-id="d455f-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d455f-113">Delegated (work or school account)</span></span> | <span data-ttu-id="d455f-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d455f-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d455f-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="d455f-115">Application</span></span> |
|:-----|:-----|:-----|:-----|
| <span data-ttu-id="d455f-116">用户日历</span><span class="sxs-lookup"><span data-stu-id="d455f-116">user calendar</span></span> | <span data-ttu-id="d455f-117">Calendars.Read、Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d455f-117">Calendars.Read, Calendars.ReadWrite</span></span> | <span data-ttu-id="d455f-118">Calendars.Read、Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d455f-118">Calendars.Read, Calendars.ReadWrite</span></span> | <span data-ttu-id="d455f-119">Calendars.Read、Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d455f-119">Calendars.Read, Calendars.ReadWrite</span></span> |
| <span data-ttu-id="d455f-120">组 日历</span><span class="sxs-lookup"><span data-stu-id="d455f-120">group calendar</span></span> | <span data-ttu-id="d455f-121">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d455f-121">Group.Read.All, Group.ReadWrite.All</span></span> | <span data-ttu-id="d455f-122">不支持。</span><span class="sxs-lookup"><span data-stu-id="d455f-122">Not supported.</span></span> | <span data-ttu-id="d455f-123">不支持。</span><span class="sxs-lookup"><span data-stu-id="d455f-123">Not supported.</span></span> |


## <a name="http-request"></a><span data-ttu-id="d455f-124">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d455f-124">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="d455f-125">用户或组的默认 [日历](../resources/calendar.md)。</span><span class="sxs-lookup"><span data-stu-id="d455f-125">A user's or group's default [calendar](../resources/calendar.md).</span></span>
```http
GET /me/calendar/events
GET /users/{id | userPrincipalName}/calendar/events
GET /groups/{id}/calendar/events
```
<span data-ttu-id="d455f-126">默认 [calendarGroup](../resources/calendargroup.md) 中用户的 [日历](../resources/calendar.md)。</span><span class="sxs-lookup"><span data-stu-id="d455f-126">A user's [calendar](../resources/calendar.md) in the default [calendarGroup](../resources/calendargroup.md).</span></span>
```http
GET /me/calendars/{id}/events
GET /users/{id | userPrincipalName}/calendars/{id}/events

GET /me/calendarGroup/calendars/{id}/events
GET /users/{id | userPrincipalName}/calendarGroup/calendars/{id}/events
```
<span data-ttu-id="d455f-127">指定 [calendarGroup](../resources/calendargroup.md) 中用户的 [日历](../resources/calendar.md)。</span><span class="sxs-lookup"><span data-stu-id="d455f-127">A user's [calendar](../resources/calendar.md) in a specific [calendarGroup](../resources/calendargroup.md).</span></span>
```http
GET /me/calendarGroups/{id}/calendars/{id}/events
GET /users/{id | userPrincipalName}/calendarGroups/{id}/calendars/{id}/events
```
## <a name="optional-query-parameters"></a><span data-ttu-id="d455f-128">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="d455f-128">Optional query parameters</span></span>
<span data-ttu-id="d455f-129">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="d455f-129">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="d455f-130">请求标头</span><span class="sxs-lookup"><span data-stu-id="d455f-130">Request headers</span></span>
| <span data-ttu-id="d455f-131">名称</span><span class="sxs-lookup"><span data-stu-id="d455f-131">Name</span></span>       | <span data-ttu-id="d455f-132">类型</span><span class="sxs-lookup"><span data-stu-id="d455f-132">Type</span></span> | <span data-ttu-id="d455f-133">说明</span><span class="sxs-lookup"><span data-stu-id="d455f-133">Description</span></span> |
|:---------------|:--------|:--------|
| <span data-ttu-id="d455f-134">Authorization</span><span class="sxs-lookup"><span data-stu-id="d455f-134">Authorization</span></span>  | <span data-ttu-id="d455f-135">string</span><span class="sxs-lookup"><span data-stu-id="d455f-135">string</span></span> | <span data-ttu-id="d455f-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="d455f-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="d455f-138">Prefer: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="d455f-138">Prefer: outlook.timezone</span></span>  | <span data-ttu-id="d455f-139">string</span><span class="sxs-lookup"><span data-stu-id="d455f-139">string</span></span> | <span data-ttu-id="d455f-140">此选项可用于指定响应中开始时间和结束时间的时区。</span><span class="sxs-lookup"><span data-stu-id="d455f-140">Use this to specify the time zone for start and end times in the response.</span></span> <span data-ttu-id="d455f-141">如果未指定，返回的这些时间值采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="d455f-141">If not specified, those time values are returned in UTC.</span></span> <span data-ttu-id="d455f-142">可选。</span><span class="sxs-lookup"><span data-stu-id="d455f-142">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d455f-143">请求正文</span><span class="sxs-lookup"><span data-stu-id="d455f-143">Request body</span></span>
<span data-ttu-id="d455f-144">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="d455f-144">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d455f-145">响应</span><span class="sxs-lookup"><span data-stu-id="d455f-145">Response</span></span>

<span data-ttu-id="d455f-146">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [Event](../resources/event.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="d455f-146">If successful, this method returns a `200 OK` response code and collection of [Event](../resources/event.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="d455f-147">示例</span><span class="sxs-lookup"><span data-stu-id="d455f-147">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d455f-148">请求</span><span class="sxs-lookup"><span data-stu-id="d455f-148">Request</span></span>
<span data-ttu-id="d455f-149">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="d455f-149">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="d455f-150">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="d455f-150">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "calendar_get_events"
}-->
```http
GET https://graph.microsoft.com/beta/me/calendar/events
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="d455f-151">C#</span><span class="sxs-lookup"><span data-stu-id="d455f-151">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/calendar-get-events-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d455f-152">Javascript</span><span class="sxs-lookup"><span data-stu-id="d455f-152">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/calendar-get-events-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="d455f-153">目标-C</span><span class="sxs-lookup"><span data-stu-id="d455f-153">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/calendar-get-events-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="d455f-154">Java</span><span class="sxs-lookup"><span data-stu-id="d455f-154">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/calendar-get-events-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="d455f-155">响应</span><span class="sxs-lookup"><span data-stu-id="d455f-155">Response</span></span>
<span data-ttu-id="d455f-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="d455f-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
