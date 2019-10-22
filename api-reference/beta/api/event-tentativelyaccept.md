---
title: 'event: tentativelyAccept'
description: 暂时接受用户日历中的指定事件。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: b9bdcd71033c1e1c21f7ba3768e357bbe5c70084
ms.sourcegitcommit: c9b9ff2c862f8d96d282a7bdf641cdb9c53a4600
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2019
ms.locfileid: "37621425"
---
# <a name="event-tentativelyaccept"></a><span data-ttu-id="db628-103">event: tentativelyAccept</span><span class="sxs-lookup"><span data-stu-id="db628-103">event: tentativelyAccept</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="db628-104">暂时接受用户[日历](../resources/calendar.md)中的指定[事件](../resources/event.md)。</span><span class="sxs-lookup"><span data-stu-id="db628-104">Tentatively accept the specified [event](../resources/event.md) in a user [calendar](../resources/calendar.md).</span></span>

<span data-ttu-id="db628-105">如果事件允许建议的新时间，在对事件做出响应时，被邀请者可以通过包含**proposedNewTime**参数来选择建议替代时间。</span><span class="sxs-lookup"><span data-stu-id="db628-105">If the event allows proposals for new times, on responding tentative to the event, an invitee can choose to suggest an alternative time by including the **proposedNewTime** parameter.</span></span> <span data-ttu-id="db628-106">有关如何建议时间以及如何接收和接受新时间建议的详细信息，请参阅[建议新会议时间](/graph/outlook-calendar-meeting-proposals)。</span><span class="sxs-lookup"><span data-stu-id="db628-106">For more information on how to propose a time, and how to receive and accept a new time proposal, see [Propose new meeting times](/graph/outlook-calendar-meeting-proposals).</span></span>

## <a name="permissions"></a><span data-ttu-id="db628-107">权限</span><span class="sxs-lookup"><span data-stu-id="db628-107">Permissions</span></span>
<span data-ttu-id="db628-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="db628-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="db628-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="db628-110">Permission type</span></span>      | <span data-ttu-id="db628-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="db628-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="db628-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="db628-112">Delegated (work or school account)</span></span> | <span data-ttu-id="db628-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="db628-113">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="db628-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="db628-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="db628-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="db628-115">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="db628-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="db628-116">Application</span></span> | <span data-ttu-id="db628-117">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="db628-117">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="db628-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="db628-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/events/{id}/tentativelyAccept
POST /users/{id | userPrincipalName}/events/{id}/tentativelyAccept

POST /me/calendar/events/{id}/tentativelyAccept
POST /users/{id | userPrincipalName}/calendar/events/{id}/tentativelyAccept

POST /me/calendars/{id}/events/{id}/tentativelyAccept
POST /users/{id | userPrincipalName}/calendars/{id}/events/{id}/tentativelyAccept

POST /me/calendargroup/calendars/{id}/events/{id}/tentativelyAccept
POST /users/{id | userPrincipalName}/calendargroup/calendars/{id}/events/{id}/tentativelyAccept

POST /me/calendargroups/{id}/calendars/{id}/events/{id}/tentativelyAccept
POST /users/{id | userPrincipalName}/calendargroups/{id}/calendars/{id}/events/{id}/tentativelyAccept
```
## <a name="request-headers"></a><span data-ttu-id="db628-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="db628-119">Request headers</span></span>
| <span data-ttu-id="db628-120">名称</span><span class="sxs-lookup"><span data-stu-id="db628-120">Name</span></span>       | <span data-ttu-id="db628-121">类型</span><span class="sxs-lookup"><span data-stu-id="db628-121">Type</span></span> | <span data-ttu-id="db628-122">说明</span><span class="sxs-lookup"><span data-stu-id="db628-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="db628-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="db628-123">Authorization</span></span>  | <span data-ttu-id="db628-124">string</span><span class="sxs-lookup"><span data-stu-id="db628-124">string</span></span>  | <span data-ttu-id="db628-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="db628-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="db628-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="db628-127">Content-Type</span></span> | <span data-ttu-id="db628-128">string</span><span class="sxs-lookup"><span data-stu-id="db628-128">string</span></span>  | <span data-ttu-id="db628-p104">实体正文中的数据性质。必需。</span><span class="sxs-lookup"><span data-stu-id="db628-p104">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="db628-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="db628-131">Request body</span></span>
<span data-ttu-id="db628-132">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="db628-132">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="db628-133">参数</span><span class="sxs-lookup"><span data-stu-id="db628-133">Parameter</span></span>    | <span data-ttu-id="db628-134">类型</span><span class="sxs-lookup"><span data-stu-id="db628-134">Type</span></span>   |<span data-ttu-id="db628-135">说明</span><span class="sxs-lookup"><span data-stu-id="db628-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="db628-136">注释</span><span class="sxs-lookup"><span data-stu-id="db628-136">comment</span></span>|<span data-ttu-id="db628-137">String</span><span class="sxs-lookup"><span data-stu-id="db628-137">String</span></span>|<span data-ttu-id="db628-p105">响应中包含的文本。可选。</span><span class="sxs-lookup"><span data-stu-id="db628-p105">Text included in the response. Optional.</span></span>|
|<span data-ttu-id="db628-140">sendResponse</span><span class="sxs-lookup"><span data-stu-id="db628-140">sendResponse</span></span>|<span data-ttu-id="db628-141">Boolean</span><span class="sxs-lookup"><span data-stu-id="db628-141">Boolean</span></span>|<span data-ttu-id="db628-p106">如果将响应发送给组织者，则值为 `true`；否则为 `false`。可选。默认值为 `true`。</span><span class="sxs-lookup"><span data-stu-id="db628-p106">`true` if a response is to be sent to the organizer; otherwise, `false`. Optional. Default is `true`.</span></span>|
|<span data-ttu-id="db628-145">proposedNewTime</span><span class="sxs-lookup"><span data-stu-id="db628-145">proposedNewTime</span></span>|[<span data-ttu-id="db628-146">timeSlot</span><span class="sxs-lookup"><span data-stu-id="db628-146">timeSlot</span></span>](../resources/timeslot.md)|<span data-ttu-id="db628-147">会议请求开始和结束时由被邀请者建议的备用日期/时间。</span><span class="sxs-lookup"><span data-stu-id="db628-147">An alternate date/time proposed by an invitee for a meeting request to start and end.</span></span> <span data-ttu-id="db628-148">仅对允许新时间建议的事件有效。</span><span class="sxs-lookup"><span data-stu-id="db628-148">Valid only for events that allow new time proposals.</span></span> <span data-ttu-id="db628-149">设置此参数需要将**sendResponse**设置`true`为。</span><span class="sxs-lookup"><span data-stu-id="db628-149">Setting this parameter requires setting **sendResponse** to `true`.</span></span> <span data-ttu-id="db628-150">可选。</span><span class="sxs-lookup"><span data-stu-id="db628-150">Optional.</span></span>|

## <a name="response"></a><span data-ttu-id="db628-151">响应</span><span class="sxs-lookup"><span data-stu-id="db628-151">Response</span></span>

<span data-ttu-id="db628-p108">如果成功，此方法返回 `202 Accepted` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="db628-p108">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

<span data-ttu-id="db628-154">如果出现以下一种或两种情况，此操作将返回 HTTP 400：</span><span class="sxs-lookup"><span data-stu-id="db628-154">This action returns HTTP 400 if one or both of the following occur:</span></span>

- <span data-ttu-id="db628-155">包含**proposedNewTime**参数，但**事件** `false`的**allowNewTimeProposals**属性为。</span><span class="sxs-lookup"><span data-stu-id="db628-155">The **proposedNewTime** parameter is included but the **allowNewTimeProposals** property of the **event** is `false`.</span></span> 
- <span data-ttu-id="db628-156">包含**proposedNewTime**参数，但**sendResponse**参数设置为`false`。</span><span class="sxs-lookup"><span data-stu-id="db628-156">The **proposedNewTime** parameter is included but the **sendResponse** parameter is set to `false`.</span></span>

## <a name="example"></a><span data-ttu-id="db628-157">示例</span><span class="sxs-lookup"><span data-stu-id="db628-157">Example</span></span>
<span data-ttu-id="db628-158">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="db628-158">Here is an example of how to call this API.</span></span>
### <a name="request"></a><span data-ttu-id="db628-159">请求</span><span class="sxs-lookup"><span data-stu-id="db628-159">Request</span></span>
<span data-ttu-id="db628-160">在下面的示例中，登录用户对指定事件的响应是暂定的，将**sendResponse** paremeter 设置为 true，并在**proposedNewTime**参数中包含一个替代时间。</span><span class="sxs-lookup"><span data-stu-id="db628-160">In the following example, the signed-in user responds tentative to the specified event, sets the **sendResponse** paremeter to true, and includes an alternative time in the **proposedNewTime** parameter.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="db628-161">HTTP</span><span class="sxs-lookup"><span data-stu-id="db628-161">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "event_tentativelyaccept"
}-->
```http
POST https://graph.microsoft.com/beta/me/events/{id}/tentativelyAccept
Content-type: application/json

{
  "comment": "I may not be able to make this week. How about next week?",
  "sendResponse": true,
  "proposedNewTime": {
      "start": { 
          "dateTime": "2019-12-02T18:00:00", 
          "timeZone": "Pacific Standard Time" 
      }, 
      "end": { 
          "dateTime": "2019-12-02T19:00:00", 
          "timeZone": "Pacific Standard Time" 
      }     
  }
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="db628-162">C#</span><span class="sxs-lookup"><span data-stu-id="db628-162">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/event-tentativelyaccept-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="db628-163">JavaScript</span><span class="sxs-lookup"><span data-stu-id="db628-163">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/event-tentativelyaccept-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="db628-164">Objective-C</span><span class="sxs-lookup"><span data-stu-id="db628-164">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/event-tentativelyaccept-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="db628-165">响应</span><span class="sxs-lookup"><span data-stu-id="db628-165">Response</span></span>
<span data-ttu-id="db628-166">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="db628-166">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "name": "event_tentativelyaccept",
  "truncated": true
} -->
```http
HTTP/1.1 202 Accepted
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "event: tentativelyAccept",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
