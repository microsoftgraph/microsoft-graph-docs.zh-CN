---
title: 'event: tentativelyAccept'
description: 暂时接受用户日历中的指定事件。
author: harini84
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 183742e6f6402b6ba00a749f80ae934a421ea1a4
ms.sourcegitcommit: 20b951f8bd245bb3a2bc7d3f5533e8619e9db084
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/27/2020
ms.locfileid: "45427107"
---
# <a name="event-tentativelyaccept"></a><span data-ttu-id="78719-103">event: tentativelyAccept</span><span class="sxs-lookup"><span data-stu-id="78719-103">event: tentativelyAccept</span></span>

<span data-ttu-id="78719-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="78719-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="78719-105">暂时接受用户[日历](../resources/calendar.md)中的指定[事件](../resources/event.md)。</span><span class="sxs-lookup"><span data-stu-id="78719-105">Tentatively accept the specified [event](../resources/event.md) in a user [calendar](../resources/calendar.md).</span></span>

<span data-ttu-id="78719-106">如果事件允许建议的新时间，在对事件做出响应时，被邀请者可以通过包含**proposedNewTime**参数来选择建议替代时间。</span><span class="sxs-lookup"><span data-stu-id="78719-106">If the event allows proposals for new times, on responding tentative to the event, an invitee can choose to suggest an alternative time by including the **proposedNewTime** parameter.</span></span> <span data-ttu-id="78719-107">有关如何建议时间以及如何接收和接受新时间建议的详细信息，请参阅[建议新会议时间](/graph/outlook-calendar-meeting-proposals)。</span><span class="sxs-lookup"><span data-stu-id="78719-107">For more information on how to propose a time, and how to receive and accept a new time proposal, see [Propose new meeting times](/graph/outlook-calendar-meeting-proposals).</span></span>

## <a name="permissions"></a><span data-ttu-id="78719-108">权限</span><span class="sxs-lookup"><span data-stu-id="78719-108">Permissions</span></span>
<span data-ttu-id="78719-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="78719-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="78719-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="78719-111">Permission type</span></span>      | <span data-ttu-id="78719-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="78719-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="78719-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="78719-113">Delegated (work or school account)</span></span> | <span data-ttu-id="78719-114">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="78719-114">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="78719-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="78719-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="78719-116">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="78719-116">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="78719-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="78719-117">Application</span></span> | <span data-ttu-id="78719-118">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="78719-118">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="78719-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="78719-119">HTTP request</span></span>
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
## <a name="request-headers"></a><span data-ttu-id="78719-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="78719-120">Request headers</span></span>
| <span data-ttu-id="78719-121">名称</span><span class="sxs-lookup"><span data-stu-id="78719-121">Name</span></span>       | <span data-ttu-id="78719-122">类型</span><span class="sxs-lookup"><span data-stu-id="78719-122">Type</span></span> | <span data-ttu-id="78719-123">说明</span><span class="sxs-lookup"><span data-stu-id="78719-123">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="78719-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="78719-124">Authorization</span></span>  | <span data-ttu-id="78719-125">string</span><span class="sxs-lookup"><span data-stu-id="78719-125">string</span></span>  | <span data-ttu-id="78719-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="78719-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="78719-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="78719-128">Content-Type</span></span> | <span data-ttu-id="78719-129">string</span><span class="sxs-lookup"><span data-stu-id="78719-129">string</span></span>  | <span data-ttu-id="78719-p104">实体正文中的数据性质。必需。</span><span class="sxs-lookup"><span data-stu-id="78719-p104">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="78719-132">请求正文</span><span class="sxs-lookup"><span data-stu-id="78719-132">Request body</span></span>
<span data-ttu-id="78719-133">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="78719-133">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="78719-134">参数</span><span class="sxs-lookup"><span data-stu-id="78719-134">Parameter</span></span>    | <span data-ttu-id="78719-135">类型</span><span class="sxs-lookup"><span data-stu-id="78719-135">Type</span></span>   |<span data-ttu-id="78719-136">说明</span><span class="sxs-lookup"><span data-stu-id="78719-136">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="78719-137">注释</span><span class="sxs-lookup"><span data-stu-id="78719-137">comment</span></span>|<span data-ttu-id="78719-138">String</span><span class="sxs-lookup"><span data-stu-id="78719-138">String</span></span>|<span data-ttu-id="78719-p105">响应中包含的文本。可选。</span><span class="sxs-lookup"><span data-stu-id="78719-p105">Text included in the response. Optional.</span></span>|
|<span data-ttu-id="78719-141">proposedNewTime</span><span class="sxs-lookup"><span data-stu-id="78719-141">proposedNewTime</span></span>|[<span data-ttu-id="78719-142">timeSlot</span><span class="sxs-lookup"><span data-stu-id="78719-142">timeSlot</span></span>](../resources/timeslot.md)|<span data-ttu-id="78719-143">会议请求开始和结束时由被邀请者建议的备用日期/时间。</span><span class="sxs-lookup"><span data-stu-id="78719-143">An alternate date/time proposed by an invitee for a meeting request to start and end.</span></span> <span data-ttu-id="78719-144">仅对允许新时间建议的事件有效。</span><span class="sxs-lookup"><span data-stu-id="78719-144">Valid only for events that allow new time proposals.</span></span> <span data-ttu-id="78719-145">设置此参数需要将**sendResponse**设置为 `true` 。</span><span class="sxs-lookup"><span data-stu-id="78719-145">Setting this parameter requires setting **sendResponse** to `true`.</span></span> <span data-ttu-id="78719-146">可选。</span><span class="sxs-lookup"><span data-stu-id="78719-146">Optional.</span></span>|
|<span data-ttu-id="78719-147">sendResponse</span><span class="sxs-lookup"><span data-stu-id="78719-147">sendResponse</span></span>|<span data-ttu-id="78719-148">Boolean</span><span class="sxs-lookup"><span data-stu-id="78719-148">Boolean</span></span>|<span data-ttu-id="78719-p107">如果将响应发送给组织者，则值为 `true`；否则为 `false`。可选。默认值为 `true`。</span><span class="sxs-lookup"><span data-stu-id="78719-p107">`true` if a response is to be sent to the organizer; otherwise, `false`. Optional. Default is `true`.</span></span>|

## <a name="response"></a><span data-ttu-id="78719-152">响应</span><span class="sxs-lookup"><span data-stu-id="78719-152">Response</span></span>

<span data-ttu-id="78719-p108">如果成功，此方法返回 `202 Accepted` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="78719-p108">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

<span data-ttu-id="78719-155">如果出现以下一种或两种情况，此操作将返回 HTTP 400：</span><span class="sxs-lookup"><span data-stu-id="78719-155">This action returns HTTP 400 if one or both of the following occur:</span></span>

- <span data-ttu-id="78719-156">包含**proposedNewTime**参数，但**事件**的**allowNewTimeProposals**属性为 `false` 。</span><span class="sxs-lookup"><span data-stu-id="78719-156">The **proposedNewTime** parameter is included but the **allowNewTimeProposals** property of the **event** is `false`.</span></span> 
- <span data-ttu-id="78719-157">包含**proposedNewTime**参数，但**sendResponse**参数设置为 `false` 。</span><span class="sxs-lookup"><span data-stu-id="78719-157">The **proposedNewTime** parameter is included but the **sendResponse** parameter is set to `false`.</span></span>

## <a name="example"></a><span data-ttu-id="78719-158">示例</span><span class="sxs-lookup"><span data-stu-id="78719-158">Example</span></span>
<span data-ttu-id="78719-159">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="78719-159">Here is an example of how to call this API.</span></span>
### <a name="request"></a><span data-ttu-id="78719-160">请求</span><span class="sxs-lookup"><span data-stu-id="78719-160">Request</span></span>
<span data-ttu-id="78719-161">在下面的示例中，登录用户对指定事件的响应是暂定的，将**sendResponse** paremeter 设置为 true，并在**proposedNewTime**参数中包含一个替代时间。</span><span class="sxs-lookup"><span data-stu-id="78719-161">In the following example, the signed-in user responds tentative to the specified event, sets the **sendResponse** paremeter to true, and includes an alternative time in the **proposedNewTime** parameter.</span></span>

# <a name="http"></a>[<span data-ttu-id="78719-162">HTTP</span><span class="sxs-lookup"><span data-stu-id="78719-162">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "event_tentativelyaccept"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/events/{id}/tentativelyAccept
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
# <a name="c"></a>[<span data-ttu-id="78719-163">C#</span><span class="sxs-lookup"><span data-stu-id="78719-163">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/event-tentativelyaccept-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="78719-164">JavaScript</span><span class="sxs-lookup"><span data-stu-id="78719-164">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/event-tentativelyaccept-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="78719-165">Objective-C</span><span class="sxs-lookup"><span data-stu-id="78719-165">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/event-tentativelyaccept-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="78719-166">Java</span><span class="sxs-lookup"><span data-stu-id="78719-166">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/event-tentativelyaccept-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="78719-167">响应</span><span class="sxs-lookup"><span data-stu-id="78719-167">Response</span></span>
<span data-ttu-id="78719-168">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="78719-168">Here is an example of the response.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "event: tentativelyAccept",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
