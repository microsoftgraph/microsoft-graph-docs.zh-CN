---
title: 'event: snoozeReminder'
description: 将用户日历中的事件的提醒推迟到新时间。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 6de413d937f87820f3fbad497198e0c1b74628da
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42422808"
---
# <a name="event-snoozereminder"></a><span data-ttu-id="50671-103">event: snoozeReminder</span><span class="sxs-lookup"><span data-stu-id="50671-103">event: snoozeReminder</span></span>

<span data-ttu-id="50671-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="50671-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="50671-105">将用户[日历](../resources/calendar.md)中的[事件](../resources/event.md)的提醒推迟到新时间。</span><span class="sxs-lookup"><span data-stu-id="50671-105">Postpone a reminder for an [event](../resources/event.md) in a user [calendar](../resources/calendar.md) until a new time.</span></span>

## <a name="permissions"></a><span data-ttu-id="50671-106">权限</span><span class="sxs-lookup"><span data-stu-id="50671-106">Permissions</span></span>
<span data-ttu-id="50671-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="50671-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="50671-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="50671-109">Permission type</span></span>      | <span data-ttu-id="50671-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="50671-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="50671-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="50671-111">Delegated (work or school account)</span></span> | <span data-ttu-id="50671-112">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="50671-112">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="50671-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="50671-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="50671-114">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="50671-114">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="50671-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="50671-115">Application</span></span> | <span data-ttu-id="50671-116">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="50671-116">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="50671-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="50671-117">HTTP request</span></span>
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
## <a name="request-headers"></a><span data-ttu-id="50671-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="50671-118">Request headers</span></span>
| <span data-ttu-id="50671-119">名称</span><span class="sxs-lookup"><span data-stu-id="50671-119">Name</span></span>       | <span data-ttu-id="50671-120">类型</span><span class="sxs-lookup"><span data-stu-id="50671-120">Type</span></span> | <span data-ttu-id="50671-121">说明</span><span class="sxs-lookup"><span data-stu-id="50671-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="50671-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="50671-122">Authorization</span></span>  | <span data-ttu-id="50671-123">string</span><span class="sxs-lookup"><span data-stu-id="50671-123">string</span></span>  | <span data-ttu-id="50671-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="50671-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="50671-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="50671-126">Content-Type</span></span> | <span data-ttu-id="50671-127">string</span><span class="sxs-lookup"><span data-stu-id="50671-127">string</span></span>  | <span data-ttu-id="50671-p103">实体正文中的数据性质。必需。</span><span class="sxs-lookup"><span data-stu-id="50671-p103">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="50671-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="50671-130">Request body</span></span>
<span data-ttu-id="50671-131">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="50671-131">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="50671-132">参数</span><span class="sxs-lookup"><span data-stu-id="50671-132">Parameter</span></span>    | <span data-ttu-id="50671-133">类型</span><span class="sxs-lookup"><span data-stu-id="50671-133">Type</span></span>   |<span data-ttu-id="50671-134">说明</span><span class="sxs-lookup"><span data-stu-id="50671-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="50671-135">newReminderTime</span><span class="sxs-lookup"><span data-stu-id="50671-135">newReminderTime</span></span>|<span data-ttu-id="50671-136">DateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="50671-136">DateTimeTimeZone</span></span>|<span data-ttu-id="50671-137">触发提醒的新日期和时间。</span><span class="sxs-lookup"><span data-stu-id="50671-137">The new date and time to trigger the reminder.</span></span>|

## <a name="response"></a><span data-ttu-id="50671-138">响应</span><span class="sxs-lookup"><span data-stu-id="50671-138">Response</span></span>

<span data-ttu-id="50671-p104">如果成功，此方法返回 `200 OK` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="50671-p104">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="50671-141">示例</span><span class="sxs-lookup"><span data-stu-id="50671-141">Example</span></span>
<span data-ttu-id="50671-142">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="50671-142">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="50671-143">请求</span><span class="sxs-lookup"><span data-stu-id="50671-143">Request</span></span>
<span data-ttu-id="50671-144">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="50671-144">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="50671-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="50671-145">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="50671-146">C#</span><span class="sxs-lookup"><span data-stu-id="50671-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/event-snoozereminder-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="50671-147">JavaScript</span><span class="sxs-lookup"><span data-stu-id="50671-147">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/event-snoozereminder-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="50671-148">Objective-C</span><span class="sxs-lookup"><span data-stu-id="50671-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/event-snoozereminder-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="50671-149">响应</span><span class="sxs-lookup"><span data-stu-id="50671-149">Response</span></span>
<span data-ttu-id="50671-150">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="50671-150">Here is an example of the response.</span></span>
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
