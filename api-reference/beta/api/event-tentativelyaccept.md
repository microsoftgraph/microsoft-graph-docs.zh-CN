---
title: 'event: tentativelyAccept'
description: 暂时接受用户日历中的指定事件。
author: harini84
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 36786332fdbd0b84a6107106cf346153f8be55c8
ms.sourcegitcommit: 979fe005c74eb99cd971df6b9511b2d3f7fe3cd4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/17/2021
ms.locfileid: "52992238"
---
# <a name="event-tentativelyaccept"></a><span data-ttu-id="2f4eb-103">event: tentativelyAccept</span><span class="sxs-lookup"><span data-stu-id="2f4eb-103">event: tentativelyAccept</span></span>

<span data-ttu-id="2f4eb-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2f4eb-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2f4eb-105">暂时接受用户 [日历中的](../resources/event.md) 指定 [事件](../resources/calendar.md)。</span><span class="sxs-lookup"><span data-stu-id="2f4eb-105">Tentatively accept the specified [event](../resources/event.md) in a user [calendar](../resources/calendar.md).</span></span>

<span data-ttu-id="2f4eb-106">如果事件允许针对新时间的建议，则当对事件做出暂定响应时，被邀请者可以选择通过包含 **proposedNewTime** 参数来建议备选时间。</span><span class="sxs-lookup"><span data-stu-id="2f4eb-106">If the event allows proposals for new times, on responding tentative to the event, an invitee can choose to suggest an alternative time by including the **proposedNewTime** parameter.</span></span> <span data-ttu-id="2f4eb-107">若要详细了解如何建议时间，以及如何接收和接受新时间建议，请参阅 [建议新的会议时间](/graph/outlook-calendar-meeting-proposals)。</span><span class="sxs-lookup"><span data-stu-id="2f4eb-107">For more information on how to propose a time, and how to receive and accept a new time proposal, see [Propose new meeting times](/graph/outlook-calendar-meeting-proposals).</span></span>

## <a name="permissions"></a><span data-ttu-id="2f4eb-108">权限</span><span class="sxs-lookup"><span data-stu-id="2f4eb-108">Permissions</span></span>
<span data-ttu-id="2f4eb-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2f4eb-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2f4eb-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="2f4eb-111">Permission type</span></span>      | <span data-ttu-id="2f4eb-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="2f4eb-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2f4eb-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2f4eb-113">Delegated (work or school account)</span></span> | <span data-ttu-id="2f4eb-114">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2f4eb-114">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="2f4eb-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2f4eb-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2f4eb-116">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2f4eb-116">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="2f4eb-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="2f4eb-117">Application</span></span> | <span data-ttu-id="2f4eb-118">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2f4eb-118">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="2f4eb-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2f4eb-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/events/{id}/tentativelyAccept
POST /users/{id | userPrincipalName}/events/{id}/tentativelyAccept

POST /me/calendar/events/{id}/tentativelyAccept
POST /users/{id | userPrincipalName}/calendar/events/{id}/tentativelyAccept

POST /me/calendars/{id}/events/{id}/tentativelyAccept
POST /users/{id | userPrincipalName}/calendars/{id}/events/{id}/tentativelyAccept

POST /me/calendargroups/{id}/calendars/{id}/events/{id}/tentativelyAccept
POST /users/{id | userPrincipalName}/calendargroups/{id}/calendars/{id}/events/{id}/tentativelyAccept
```
## <a name="request-headers"></a><span data-ttu-id="2f4eb-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="2f4eb-120">Request headers</span></span>
| <span data-ttu-id="2f4eb-121">名称</span><span class="sxs-lookup"><span data-stu-id="2f4eb-121">Name</span></span>       | <span data-ttu-id="2f4eb-122">类型</span><span class="sxs-lookup"><span data-stu-id="2f4eb-122">Type</span></span> | <span data-ttu-id="2f4eb-123">说明</span><span class="sxs-lookup"><span data-stu-id="2f4eb-123">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="2f4eb-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="2f4eb-124">Authorization</span></span>  | <span data-ttu-id="2f4eb-125">string</span><span class="sxs-lookup"><span data-stu-id="2f4eb-125">string</span></span>  | <span data-ttu-id="2f4eb-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="2f4eb-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="2f4eb-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="2f4eb-128">Content-Type</span></span> | <span data-ttu-id="2f4eb-129">string</span><span class="sxs-lookup"><span data-stu-id="2f4eb-129">string</span></span>  | <span data-ttu-id="2f4eb-p104">实体正文中的数据性质。必需。</span><span class="sxs-lookup"><span data-stu-id="2f4eb-p104">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2f4eb-132">请求正文</span><span class="sxs-lookup"><span data-stu-id="2f4eb-132">Request body</span></span>
<span data-ttu-id="2f4eb-133">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="2f4eb-133">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="2f4eb-134">参数</span><span class="sxs-lookup"><span data-stu-id="2f4eb-134">Parameter</span></span>    | <span data-ttu-id="2f4eb-135">类型</span><span class="sxs-lookup"><span data-stu-id="2f4eb-135">Type</span></span>   |<span data-ttu-id="2f4eb-136">说明</span><span class="sxs-lookup"><span data-stu-id="2f4eb-136">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2f4eb-137">注释</span><span class="sxs-lookup"><span data-stu-id="2f4eb-137">comment</span></span>|<span data-ttu-id="2f4eb-138">String</span><span class="sxs-lookup"><span data-stu-id="2f4eb-138">String</span></span>|<span data-ttu-id="2f4eb-p105">响应中包含的文本。可选。</span><span class="sxs-lookup"><span data-stu-id="2f4eb-p105">Text included in the response. Optional.</span></span>|
|<span data-ttu-id="2f4eb-141">sendResponse</span><span class="sxs-lookup"><span data-stu-id="2f4eb-141">sendResponse</span></span>|<span data-ttu-id="2f4eb-142">Boolean</span><span class="sxs-lookup"><span data-stu-id="2f4eb-142">Boolean</span></span>|<span data-ttu-id="2f4eb-p106">如果将响应发送给组织者，则值为 `true`；否则为 `false`。可选。默认值为 `true`。</span><span class="sxs-lookup"><span data-stu-id="2f4eb-p106">`true` if a response is to be sent to the organizer; otherwise, `false`. Optional. Default is `true`.</span></span>|
|<span data-ttu-id="2f4eb-146">proposedNewTime</span><span class="sxs-lookup"><span data-stu-id="2f4eb-146">proposedNewTime</span></span>|[<span data-ttu-id="2f4eb-147">timeSlot</span><span class="sxs-lookup"><span data-stu-id="2f4eb-147">timeSlot</span></span>](../resources/timeslot.md)|<span data-ttu-id="2f4eb-148">被邀请者为开始和结束会议请求建议的备用日期/时间。</span><span class="sxs-lookup"><span data-stu-id="2f4eb-148">An alternate date/time proposed by an invitee for a meeting request to start and end.</span></span> <span data-ttu-id="2f4eb-149">仅对允许新时间建议的事件有效。</span><span class="sxs-lookup"><span data-stu-id="2f4eb-149">Valid only for events that allow new time proposals.</span></span> <span data-ttu-id="2f4eb-150">设置此参数需要将 **sendResponse 设置为** `true` 。</span><span class="sxs-lookup"><span data-stu-id="2f4eb-150">Setting this parameter requires setting **sendResponse** to `true`.</span></span> <span data-ttu-id="2f4eb-151">可选。</span><span class="sxs-lookup"><span data-stu-id="2f4eb-151">Optional.</span></span>|

## <a name="response"></a><span data-ttu-id="2f4eb-152">响应</span><span class="sxs-lookup"><span data-stu-id="2f4eb-152">Response</span></span>

<span data-ttu-id="2f4eb-p108">如果成功，此方法返回 `202 Accepted` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="2f4eb-p108">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

<span data-ttu-id="2f4eb-155">如果发生以下一个或两个情况，此操作将返回 HTTP 400：</span><span class="sxs-lookup"><span data-stu-id="2f4eb-155">This action returns HTTP 400 if one or both of the following occur:</span></span>

- <span data-ttu-id="2f4eb-156">**包含 proposedNewTime** 参数，但 **事件的 allowNewTimeProposals** 属性 **为** `false` 。</span><span class="sxs-lookup"><span data-stu-id="2f4eb-156">The **proposedNewTime** parameter is included but the **allowNewTimeProposals** property of the **event** is `false`.</span></span> 
- <span data-ttu-id="2f4eb-157">包含 **proposedNewTime** 参数，但 **sendResponse** 参数设置为 `false` 。</span><span class="sxs-lookup"><span data-stu-id="2f4eb-157">The **proposedNewTime** parameter is included but the **sendResponse** parameter is set to `false`.</span></span>

## <a name="example"></a><span data-ttu-id="2f4eb-158">示例</span><span class="sxs-lookup"><span data-stu-id="2f4eb-158">Example</span></span>
<span data-ttu-id="2f4eb-159">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="2f4eb-159">Here is an example of how to call this API.</span></span>
### <a name="request"></a><span data-ttu-id="2f4eb-160">请求</span><span class="sxs-lookup"><span data-stu-id="2f4eb-160">Request</span></span>
<span data-ttu-id="2f4eb-161">在下面的示例中，登录用户对指定事件做出暂定响应，将 **sendResponse** 参数设置为 true，并包括 **proposedNewTime** 参数中的备选时间。</span><span class="sxs-lookup"><span data-stu-id="2f4eb-161">In the following example, the signed-in user responds tentative to the specified event, sets the **sendResponse** parameter to true, and includes an alternative time in the **proposedNewTime** parameter.</span></span>

# <a name="http"></a>[<span data-ttu-id="2f4eb-162">HTTP</span><span class="sxs-lookup"><span data-stu-id="2f4eb-162">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="2f4eb-163">C#</span><span class="sxs-lookup"><span data-stu-id="2f4eb-163">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/event-tentativelyaccept-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2f4eb-164">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2f4eb-164">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/event-tentativelyaccept-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2f4eb-165">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2f4eb-165">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/event-tentativelyaccept-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="2f4eb-166">Java</span><span class="sxs-lookup"><span data-stu-id="2f4eb-166">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/event-tentativelyaccept-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="2f4eb-167">响应</span><span class="sxs-lookup"><span data-stu-id="2f4eb-167">Response</span></span>
<span data-ttu-id="2f4eb-168">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="2f4eb-168">Here is an example of the response.</span></span>
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


