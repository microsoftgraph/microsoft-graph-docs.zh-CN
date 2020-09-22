---
title: 'event: snoozeReminder'
description: 将用户日历中的事件的提醒推迟到新时间。
author: harini84
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 7ee337c31a27f3eb4b55d82e7c5f3434025d6dc6
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48006935"
---
# <a name="event-snoozereminder"></a><span data-ttu-id="e9f0b-103">event: snoozeReminder</span><span class="sxs-lookup"><span data-stu-id="e9f0b-103">event: snoozeReminder</span></span>

<span data-ttu-id="e9f0b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e9f0b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e9f0b-105">将用户[日历](../resources/calendar.md)中的[事件](../resources/event.md)的提醒推迟到新时间。</span><span class="sxs-lookup"><span data-stu-id="e9f0b-105">Postpone a reminder for an [event](../resources/event.md) in a user [calendar](../resources/calendar.md) until a new time.</span></span>

## <a name="permissions"></a><span data-ttu-id="e9f0b-106">权限</span><span class="sxs-lookup"><span data-stu-id="e9f0b-106">Permissions</span></span>
<span data-ttu-id="e9f0b-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e9f0b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e9f0b-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="e9f0b-109">Permission type</span></span>      | <span data-ttu-id="e9f0b-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e9f0b-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e9f0b-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e9f0b-111">Delegated (work or school account)</span></span> | <span data-ttu-id="e9f0b-112">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e9f0b-112">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="e9f0b-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e9f0b-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e9f0b-114">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e9f0b-114">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="e9f0b-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="e9f0b-115">Application</span></span> | <span data-ttu-id="e9f0b-116">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e9f0b-116">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="e9f0b-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e9f0b-117">HTTP request</span></span>
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
## <a name="request-headers"></a><span data-ttu-id="e9f0b-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="e9f0b-118">Request headers</span></span>
| <span data-ttu-id="e9f0b-119">名称</span><span class="sxs-lookup"><span data-stu-id="e9f0b-119">Name</span></span>       | <span data-ttu-id="e9f0b-120">类型</span><span class="sxs-lookup"><span data-stu-id="e9f0b-120">Type</span></span> | <span data-ttu-id="e9f0b-121">说明</span><span class="sxs-lookup"><span data-stu-id="e9f0b-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="e9f0b-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="e9f0b-122">Authorization</span></span>  | <span data-ttu-id="e9f0b-123">string</span><span class="sxs-lookup"><span data-stu-id="e9f0b-123">string</span></span>  | <span data-ttu-id="e9f0b-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="e9f0b-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="e9f0b-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e9f0b-126">Content-Type</span></span> | <span data-ttu-id="e9f0b-127">string</span><span class="sxs-lookup"><span data-stu-id="e9f0b-127">string</span></span>  | <span data-ttu-id="e9f0b-p103">实体正文中的数据性质。必需。</span><span class="sxs-lookup"><span data-stu-id="e9f0b-p103">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e9f0b-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="e9f0b-130">Request body</span></span>
<span data-ttu-id="e9f0b-131">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="e9f0b-131">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="e9f0b-132">参数</span><span class="sxs-lookup"><span data-stu-id="e9f0b-132">Parameter</span></span>    | <span data-ttu-id="e9f0b-133">类型</span><span class="sxs-lookup"><span data-stu-id="e9f0b-133">Type</span></span>   |<span data-ttu-id="e9f0b-134">说明</span><span class="sxs-lookup"><span data-stu-id="e9f0b-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e9f0b-135">newReminderTime</span><span class="sxs-lookup"><span data-stu-id="e9f0b-135">newReminderTime</span></span>|<span data-ttu-id="e9f0b-136">DateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="e9f0b-136">DateTimeTimeZone</span></span>|<span data-ttu-id="e9f0b-137">触发提醒的新日期和时间。</span><span class="sxs-lookup"><span data-stu-id="e9f0b-137">The new date and time to trigger the reminder.</span></span>|

## <a name="response"></a><span data-ttu-id="e9f0b-138">响应</span><span class="sxs-lookup"><span data-stu-id="e9f0b-138">Response</span></span>

<span data-ttu-id="e9f0b-p104">如果成功，此方法返回 `200 OK` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="e9f0b-p104">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e9f0b-141">示例</span><span class="sxs-lookup"><span data-stu-id="e9f0b-141">Example</span></span>
<span data-ttu-id="e9f0b-142">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="e9f0b-142">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="e9f0b-143">请求</span><span class="sxs-lookup"><span data-stu-id="e9f0b-143">Request</span></span>
<span data-ttu-id="e9f0b-144">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="e9f0b-144">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="e9f0b-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="e9f0b-145">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="e9f0b-146">C#</span><span class="sxs-lookup"><span data-stu-id="e9f0b-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/event-snoozereminder-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e9f0b-147">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e9f0b-147">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/event-snoozereminder-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e9f0b-148">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e9f0b-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/event-snoozereminder-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="e9f0b-149">响应</span><span class="sxs-lookup"><span data-stu-id="e9f0b-149">Response</span></span>
<span data-ttu-id="e9f0b-150">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="e9f0b-150">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "event: snoozeReminder",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


