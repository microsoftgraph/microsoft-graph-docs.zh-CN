---
title: 列出事件
description: 检索日历中的事件列表。该列表包含单实例会议和系列主控事件。
author: angelgolfer-ms
localization_priority: Priority
ms.prod: outlook
ms.openlocfilehash: a8fbac941f4eb045d46572716242c03425b152c4
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35443810"
---
# <a name="list-events"></a><span data-ttu-id="cf6f4-104">列出事件</span><span class="sxs-lookup"><span data-stu-id="cf6f4-104">List events</span></span>

<span data-ttu-id="cf6f4-p102">检索日历中的事件列表。该列表包含单个实例会议和系列主控形状。</span><span class="sxs-lookup"><span data-stu-id="cf6f4-p102">Retrieve a list of events in a calendar.  The list contains single instance meetings and series masters.</span></span>

<span data-ttu-id="cf6f4-107">要获取扩展的事件实例，可以[获取日历视图](calendar-list-calendarview.md)，或者[获取事件的实例](event-list-instances.md)。</span><span class="sxs-lookup"><span data-stu-id="cf6f4-107">To get expanded event instances, you can [get the calendar view](calendar-list-calendarview.md), or [get the instances of an event](event-list-instances.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="cf6f4-108">权限</span><span class="sxs-lookup"><span data-stu-id="cf6f4-108">Permissions</span></span>
<span data-ttu-id="cf6f4-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="cf6f4-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cf6f4-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="cf6f4-111">Permission type</span></span>      | <span data-ttu-id="cf6f4-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="cf6f4-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cf6f4-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="cf6f4-113">Delegated (work or school account)</span></span> | <span data-ttu-id="cf6f4-114">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="cf6f4-114">Calendars.Read</span></span>    |
|<span data-ttu-id="cf6f4-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="cf6f4-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cf6f4-116">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="cf6f4-116">Calendars.Read</span></span>    |
|<span data-ttu-id="cf6f4-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="cf6f4-117">Application</span></span> | <span data-ttu-id="cf6f4-118">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="cf6f4-118">Calendars.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="cf6f4-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="cf6f4-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="cf6f4-120">用户或组的默认 [日历](../resources/calendar.md)。</span><span class="sxs-lookup"><span data-stu-id="cf6f4-120">A user's or group's default [calendar](../resources/calendar.md).</span></span>
```http
GET /me/calendar/events
GET /users/{id | userPrincipalName}/calendar/events
GET /groups/{id}/calendar/events
```
<span data-ttu-id="cf6f4-121">默认 [calendarGroup](../resources/calendargroup.md) 中用户的 [日历](../resources/calendar.md)。</span><span class="sxs-lookup"><span data-stu-id="cf6f4-121">A user's [calendar](../resources/calendar.md) in the default [calendarGroup](../resources/calendargroup.md).</span></span>
```http
GET /me/calendars/{id}/events
GET /users/{id | userPrincipalName}/calendars/{id}/events

GET /me/calendarGroup/calendars/{id}/events
GET /users/{id | userPrincipalName}/calendarGroup/calendars/{id}/events
```
<span data-ttu-id="cf6f4-122">指定 [calendarGroup](../resources/calendargroup.md) 中用户的 [日历](../resources/calendar.md)。</span><span class="sxs-lookup"><span data-stu-id="cf6f4-122">A user's [calendar](../resources/calendar.md) in a specific [calendarGroup](../resources/calendargroup.md).</span></span>
```http
GET /me/calendarGroups/{id}/calendars/{id}/events
GET /users/{id | userPrincipalName}/calendarGroups/{id}/calendars/{id}/events
```
## <a name="optional-query-parameters"></a><span data-ttu-id="cf6f4-123">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="cf6f4-123">Optional query parameters</span></span>
<span data-ttu-id="cf6f4-124">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="cf6f4-124">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="cf6f4-125">请求标头</span><span class="sxs-lookup"><span data-stu-id="cf6f4-125">Request headers</span></span>
| <span data-ttu-id="cf6f4-126">名称</span><span class="sxs-lookup"><span data-stu-id="cf6f4-126">Name</span></span>       | <span data-ttu-id="cf6f4-127">类型</span><span class="sxs-lookup"><span data-stu-id="cf6f4-127">Type</span></span> | <span data-ttu-id="cf6f4-128">说明</span><span class="sxs-lookup"><span data-stu-id="cf6f4-128">Description</span></span> |
|:---------------|:--------|:--------|
| <span data-ttu-id="cf6f4-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="cf6f4-129">Authorization</span></span>  | <span data-ttu-id="cf6f4-130">string</span><span class="sxs-lookup"><span data-stu-id="cf6f4-130">string</span></span> | <span data-ttu-id="cf6f4-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="cf6f4-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="cf6f4-133">Prefer: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="cf6f4-133">Prefer: outlook.timezone</span></span>  | <span data-ttu-id="cf6f4-134">string</span><span class="sxs-lookup"><span data-stu-id="cf6f4-134">string</span></span> | <span data-ttu-id="cf6f4-135">此选项可用于指定响应中开始时间和结束时间的时区。</span><span class="sxs-lookup"><span data-stu-id="cf6f4-135">Use this to specify the time zone for start and end times in the response.</span></span> <span data-ttu-id="cf6f4-136">如果未指定，返回的这些时间值采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="cf6f4-136">If not specified, those time values are returned in UTC.</span></span> <span data-ttu-id="cf6f4-137">可选。</span><span class="sxs-lookup"><span data-stu-id="cf6f4-137">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="cf6f4-138">请求正文</span><span class="sxs-lookup"><span data-stu-id="cf6f4-138">Request body</span></span>
<span data-ttu-id="cf6f4-139">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="cf6f4-139">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cf6f4-140">响应</span><span class="sxs-lookup"><span data-stu-id="cf6f4-140">Response</span></span>

<span data-ttu-id="cf6f4-141">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [Event](../resources/event.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="cf6f4-141">If successful, this method returns a `200 OK` response code and collection of [Event](../resources/event.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="cf6f4-142">示例</span><span class="sxs-lookup"><span data-stu-id="cf6f4-142">Example</span></span>
##### <a name="request"></a><span data-ttu-id="cf6f4-143">请求</span><span class="sxs-lookup"><span data-stu-id="cf6f4-143">Request</span></span>
<span data-ttu-id="cf6f4-144">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="cf6f4-144">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="cf6f4-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="cf6f4-145">--Http</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_events"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/calendar/events
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="cf6f4-146">C#</span><span class="sxs-lookup"><span data-stu-id="cf6f4-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-events-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="cf6f4-147">Javascript</span><span class="sxs-lookup"><span data-stu-id="cf6f4-147">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-events-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="cf6f4-148">Objective-C</span><span class="sxs-lookup"><span data-stu-id="cf6f4-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-events-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="cf6f4-149">响应</span><span class="sxs-lookup"><span data-stu-id="cf6f4-149">Response</span></span>
<span data-ttu-id="cf6f4-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="cf6f4-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "List events",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
