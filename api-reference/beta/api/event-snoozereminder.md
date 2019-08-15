---
title: 'event: snoozeReminder'
description: 将用户日历中的事件的提醒推迟到新时间。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 6e9d2fc688c14ee28f3405c1adc94383df0d69a3
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/15/2019
ms.locfileid: "36419914"
---
# <a name="event-snoozereminder"></a><span data-ttu-id="d2297-103">event: snoozeReminder</span><span class="sxs-lookup"><span data-stu-id="d2297-103">event: snoozeReminder</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d2297-104">将用户[日历](../resources/calendar.md)中的[事件](../resources/event.md)的提醒推迟到新时间。</span><span class="sxs-lookup"><span data-stu-id="d2297-104">Postpone a reminder for an [event](../resources/event.md) in a user [calendar](../resources/calendar.md) until a new time.</span></span>

## <a name="permissions"></a><span data-ttu-id="d2297-105">权限</span><span class="sxs-lookup"><span data-stu-id="d2297-105">Permissions</span></span>
<span data-ttu-id="d2297-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d2297-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d2297-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="d2297-108">Permission type</span></span>      | <span data-ttu-id="d2297-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d2297-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d2297-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d2297-110">Delegated (work or school account)</span></span> | <span data-ttu-id="d2297-111">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d2297-111">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="d2297-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d2297-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d2297-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d2297-113">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="d2297-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="d2297-114">Application</span></span> | <span data-ttu-id="d2297-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d2297-115">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="d2297-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d2297-116">HTTP request</span></span>
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
## <a name="request-headers"></a><span data-ttu-id="d2297-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="d2297-117">Request headers</span></span>
| <span data-ttu-id="d2297-118">名称</span><span class="sxs-lookup"><span data-stu-id="d2297-118">Name</span></span>       | <span data-ttu-id="d2297-119">类型</span><span class="sxs-lookup"><span data-stu-id="d2297-119">Type</span></span> | <span data-ttu-id="d2297-120">说明</span><span class="sxs-lookup"><span data-stu-id="d2297-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="d2297-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="d2297-121">Authorization</span></span>  | <span data-ttu-id="d2297-122">string</span><span class="sxs-lookup"><span data-stu-id="d2297-122">string</span></span>  | <span data-ttu-id="d2297-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="d2297-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="d2297-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d2297-125">Content-Type</span></span> | <span data-ttu-id="d2297-126">string</span><span class="sxs-lookup"><span data-stu-id="d2297-126">string</span></span>  | <span data-ttu-id="d2297-p103">实体正文中的数据性质。必需。</span><span class="sxs-lookup"><span data-stu-id="d2297-p103">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d2297-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="d2297-129">Request body</span></span>
<span data-ttu-id="d2297-130">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="d2297-130">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="d2297-131">参数</span><span class="sxs-lookup"><span data-stu-id="d2297-131">Parameter</span></span>    | <span data-ttu-id="d2297-132">类型</span><span class="sxs-lookup"><span data-stu-id="d2297-132">Type</span></span>   |<span data-ttu-id="d2297-133">说明</span><span class="sxs-lookup"><span data-stu-id="d2297-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d2297-134">newReminderTime</span><span class="sxs-lookup"><span data-stu-id="d2297-134">newReminderTime</span></span>|<span data-ttu-id="d2297-135">DateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="d2297-135">DateTimeTimeZone</span></span>|<span data-ttu-id="d2297-136">触发提醒的新日期和时间。</span><span class="sxs-lookup"><span data-stu-id="d2297-136">The new date and time to trigger the reminder.</span></span>|

## <a name="response"></a><span data-ttu-id="d2297-137">响应</span><span class="sxs-lookup"><span data-stu-id="d2297-137">Response</span></span>

<span data-ttu-id="d2297-p104">如果成功，此方法返回 `200 OK` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="d2297-p104">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d2297-140">示例</span><span class="sxs-lookup"><span data-stu-id="d2297-140">Example</span></span>
<span data-ttu-id="d2297-141">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="d2297-141">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="d2297-142">请求</span><span class="sxs-lookup"><span data-stu-id="d2297-142">Request</span></span>
<span data-ttu-id="d2297-143">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="d2297-143">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="d2297-144">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="d2297-144">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="d2297-145">C#</span><span class="sxs-lookup"><span data-stu-id="d2297-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/event-snoozereminder-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d2297-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d2297-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/event-snoozereminder-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="d2297-147">目标-C</span><span class="sxs-lookup"><span data-stu-id="d2297-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/event-snoozereminder-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="d2297-148">响应</span><span class="sxs-lookup"><span data-stu-id="d2297-148">Response</span></span>
<span data-ttu-id="d2297-149">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="d2297-149">Here is an example of the response.</span></span>
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
