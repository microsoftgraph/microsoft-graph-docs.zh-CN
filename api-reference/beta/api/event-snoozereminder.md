---
title: 'event: snoozeReminder'
description: 推迟事件提醒用户日历中的新时间之前。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 4197a231872341b7ba9c14057e32569b5c0f0c8e
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27966074"
---
# <a name="event-snoozereminder"></a><span data-ttu-id="c5a46-103">event: snoozeReminder</span><span class="sxs-lookup"><span data-stu-id="c5a46-103">event: snoozeReminder</span></span>

> <span data-ttu-id="c5a46-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="c5a46-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c5a46-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="c5a46-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c5a46-106">推迟新时间之前提醒用户[日历](../resources/calendar.md)中的[事件](../resources/event.md)。</span><span class="sxs-lookup"><span data-stu-id="c5a46-106">Postpone a reminder for an [event](../resources/event.md) in a user [calendar](../resources/calendar.md) until a new time.</span></span>

## <a name="permissions"></a><span data-ttu-id="c5a46-107">权限</span><span class="sxs-lookup"><span data-stu-id="c5a46-107">Permissions</span></span>
<span data-ttu-id="c5a46-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c5a46-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c5a46-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="c5a46-110">Permission type</span></span>      | <span data-ttu-id="c5a46-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c5a46-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c5a46-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c5a46-112">Delegated (work or school account)</span></span> | <span data-ttu-id="c5a46-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c5a46-113">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="c5a46-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c5a46-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c5a46-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c5a46-115">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="c5a46-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="c5a46-116">Application</span></span> | <span data-ttu-id="c5a46-117">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c5a46-117">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="c5a46-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c5a46-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/events/{id}/snoozeReminder
POST /users/{id | userPrincipalName}/events/{id}/snoozeReminder

POST /me/calendar/events/{id}/snoozeReminder
POST /users/{id | userPrincipalName}/calendar/events/{id}/snoozeReminder

POST /me/calendars/{id}/events/{id}/snoozeReminder
POST /users/{id | userPrincipalName}/calendars/{id}/events/{id}/snoozeReminder

POST /me/calendargroup/calendars/{id}/events/{id}/snoozeReminder
POST /users/{id | userPrincipalName}/calendargroup/calendars/{id}/events/{id}/snoozeReminder

POST /me/calendargroups/{id}/calendars/{id}/events/{id}/snoozeReminder
POST /users/{id | userPrincipalName}/calendargroups/{id}/calendars/{id}/events/{id}/snoozeReminder
```
## <a name="request-headers"></a><span data-ttu-id="c5a46-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="c5a46-119">Request headers</span></span>
| <span data-ttu-id="c5a46-120">名称</span><span class="sxs-lookup"><span data-stu-id="c5a46-120">Name</span></span>       | <span data-ttu-id="c5a46-121">类型</span><span class="sxs-lookup"><span data-stu-id="c5a46-121">Type</span></span> | <span data-ttu-id="c5a46-122">说明</span><span class="sxs-lookup"><span data-stu-id="c5a46-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="c5a46-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c5a46-123">Authorization</span></span>  | <span data-ttu-id="c5a46-124">string</span><span class="sxs-lookup"><span data-stu-id="c5a46-124">string</span></span>  | <span data-ttu-id="c5a46-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="c5a46-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="c5a46-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c5a46-127">Content-Type</span></span> | <span data-ttu-id="c5a46-128">string</span><span class="sxs-lookup"><span data-stu-id="c5a46-128">string</span></span>  | <span data-ttu-id="c5a46-p104">实体正文中的数据性质。必需。</span><span class="sxs-lookup"><span data-stu-id="c5a46-p104">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c5a46-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="c5a46-131">Request body</span></span>
<span data-ttu-id="c5a46-132">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="c5a46-132">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="c5a46-133">参数</span><span class="sxs-lookup"><span data-stu-id="c5a46-133">Parameter</span></span>    | <span data-ttu-id="c5a46-134">类型</span><span class="sxs-lookup"><span data-stu-id="c5a46-134">Type</span></span>   |<span data-ttu-id="c5a46-135">说明</span><span class="sxs-lookup"><span data-stu-id="c5a46-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c5a46-136">newReminderTime</span><span class="sxs-lookup"><span data-stu-id="c5a46-136">newReminderTime</span></span>|<span data-ttu-id="c5a46-137">DateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="c5a46-137">DateTimeTimeZone</span></span>|<span data-ttu-id="c5a46-138">触发提醒的新日期和时间。</span><span class="sxs-lookup"><span data-stu-id="c5a46-138">The new date and time to trigger the reminder.</span></span>|

## <a name="response"></a><span data-ttu-id="c5a46-139">响应</span><span class="sxs-lookup"><span data-stu-id="c5a46-139">Response</span></span>

<span data-ttu-id="c5a46-p105">如果成功，此方法返回 `200 OK` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="c5a46-p105">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c5a46-142">示例</span><span class="sxs-lookup"><span data-stu-id="c5a46-142">Example</span></span>
<span data-ttu-id="c5a46-143">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="c5a46-143">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="c5a46-144">请求</span><span class="sxs-lookup"><span data-stu-id="c5a46-144">Request</span></span>
<span data-ttu-id="c5a46-145">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="c5a46-145">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "event_snoozereminder"
}-->
```http
POST https://graph.microsoft.com/beta/me/events/{id}/snoozeReminder
Content-type: application/json
Content-length: 97

{
  "newReminderTime": {
    "dateTime": "2016-10-19T10:37:00Z",
    "timeZone": "timeZone-value"
  }
}
```

##### <a name="response"></a><span data-ttu-id="c5a46-146">响应</span><span class="sxs-lookup"><span data-stu-id="c5a46-146">Response</span></span>
<span data-ttu-id="c5a46-147">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="c5a46-147">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "event: snoozeReminder",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
