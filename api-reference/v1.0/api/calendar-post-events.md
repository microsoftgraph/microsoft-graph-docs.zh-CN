---
title: 创建事件
description: 使用此 API 在默认或指定的日历中创建新事件。
ms.openlocfilehash: da06df89ab4a62a1b767635e3daa928f84f29d9e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27009975"
---
# <a name="create-event"></a><span data-ttu-id="21afc-103">创建事件</span><span class="sxs-lookup"><span data-stu-id="21afc-103">Create Event</span></span>

<span data-ttu-id="21afc-104">使用此 API 在默认或指定的日历中创建新事件。</span><span class="sxs-lookup"><span data-stu-id="21afc-104">Use this API to create a new Event in the default or the specified calendar.</span></span>
## <a name="permissions"></a><span data-ttu-id="21afc-105">权限</span><span class="sxs-lookup"><span data-stu-id="21afc-105">Permissions</span></span>
<span data-ttu-id="21afc-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="21afc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="21afc-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="21afc-108">Permission type</span></span>      | <span data-ttu-id="21afc-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="21afc-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="21afc-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="21afc-110">Delegated (work or school account)</span></span> | <span data-ttu-id="21afc-111">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="21afc-111">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="21afc-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="21afc-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="21afc-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="21afc-113">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="21afc-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="21afc-114">Application</span></span> | <span data-ttu-id="21afc-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="21afc-115">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="21afc-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="21afc-116">HTTP request</span></span>
<span data-ttu-id="21afc-117"><!-- { "blockType": "ignored" } -->用户或组的默认[日历](../resources/calendar.md)。</span><span class="sxs-lookup"><span data-stu-id="21afc-117"><!-- { "blockType": "ignored" } --> A user's or group's default [calendar](../resources/calendar.md).</span></span>
```http
POST /me/calendar/events
POST /users/{id | userPrincipalName}/calendar/events
POST /groups/{id}/calendar/events
```
<span data-ttu-id="21afc-118">默认 [calendarGroup](../resources/calendargroup.md) 中的用户 [calendar](../resources/calendar.md)。</span><span class="sxs-lookup"><span data-stu-id="21afc-118">A user's [calendar](../resources/calendar.md) in the default [calendarGroup](../resources/calendargroup.md).</span></span>
```http
POST /me/calendars/{id}/events
POST /users/{id | userPrincipalName}/calendars/{id}/events

POST /me/calendarGroup/calendars/{id}/events
POST /users/{id | userPrincipalName}/calendarGroup/calendars/{id}/events
```
<span data-ttu-id="21afc-119">指定 [calendarGroup](../resources/calendargroup.md) 中用户的 [日历](../resources/calendar.md)。</span><span class="sxs-lookup"><span data-stu-id="21afc-119">A user's [calendar](../resources/calendar.md) in a specific [calendarGroup](../resources/calendargroup.md).</span></span>
```http
POST /me/calendarGroups/{id}/calendars/{id}/events
POST /users/{id | userPrincipalName}/calendarGroups/{id}/calendars/{id}/events
```
## <a name="request-headers"></a><span data-ttu-id="21afc-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="21afc-120">Request headers</span></span>
| <span data-ttu-id="21afc-121">标头</span><span class="sxs-lookup"><span data-stu-id="21afc-121">Header</span></span>       | <span data-ttu-id="21afc-122">值</span><span class="sxs-lookup"><span data-stu-id="21afc-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="21afc-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="21afc-123">Authorization</span></span>  | <span data-ttu-id="21afc-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="21afc-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="21afc-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="21afc-126">Content-Type</span></span>  | <span data-ttu-id="21afc-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="21afc-p103">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="21afc-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="21afc-129">Request body</span></span>
<span data-ttu-id="21afc-130">在请求正文中，提供 [Event](../resources/event.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="21afc-130">In the request body, supply a JSON representation of [Event](../resources/event.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="21afc-131">响应</span><span class="sxs-lookup"><span data-stu-id="21afc-131">Response</span></span>

<span data-ttu-id="21afc-132">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [Event](../resources/event.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="21afc-132">If successful, this method returns `201 Created` response code and [Event](../resources/event.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="21afc-133">示例</span><span class="sxs-lookup"><span data-stu-id="21afc-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="21afc-134">请求</span><span class="sxs-lookup"><span data-stu-id="21afc-134">Request</span></span>
<span data-ttu-id="21afc-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="21afc-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_event_from_calendar"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/calendar/events
Content-type: application/json
Content-length: 285

{
  "originalStartTimeZone": "originalStartTimeZone-value",
  "originalEndTimeZone": "originalEndTimeZone-value",
  "responseStatus": {
    "response": "",
    "time": "datetime-value"
  },
  "reminderMinutesBeforeStart": 99,
  "isReminderOn": true
}
```
<span data-ttu-id="21afc-136">在请求正文中，提供 [Event](../resources/event.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="21afc-136">In the request body, supply a JSON representation of [event](../resources/event.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="21afc-137">响应</span><span class="sxs-lookup"><span data-stu-id="21afc-137">Response</span></span>
<span data-ttu-id="21afc-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="21afc-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.event"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 285

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
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create Event",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
