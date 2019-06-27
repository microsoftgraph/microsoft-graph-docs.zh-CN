---
title: '事件: 取消'
description: '此操作允许会议组织者发送取消邮件并取消事件。 '
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 1442ca958e3238148ac257e54f7a135b6b4b8b47
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35259295"
---
# <a name="event-cancel"></a><span data-ttu-id="15589-103">事件: 取消</span><span class="sxs-lookup"><span data-stu-id="15589-103">event: cancel</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="15589-104">此操作允许会议组织者发送取消邮件并取消事件。</span><span class="sxs-lookup"><span data-stu-id="15589-104">This action allows the organizer of a meeting to send a cancellation message and cancel the event.</span></span> 

<span data-ttu-id="15589-105">该操作会将事件移动到 "已删除邮件" 文件夹中。</span><span class="sxs-lookup"><span data-stu-id="15589-105">The action moves the event to the Deleted Items folder.</span></span> <span data-ttu-id="15589-106">组织者还可以通过提供发生事件 ID 来取消定期会议的事件。</span><span class="sxs-lookup"><span data-stu-id="15589-106">The organizer can also cancel an occurrence of a recurring meeting by providing the occurrence event ID.</span></span> <span data-ttu-id="15589-107">调用此操作的与会者将收到错误 (HTTP 400 错误请求), 并提供以下错误消息:</span><span class="sxs-lookup"><span data-stu-id="15589-107">An attendee calling this action gets an error (HTTP 400 Bad Request), with the following error message:</span></span>

<span data-ttu-id="15589-108">无法完成您的请求。</span><span class="sxs-lookup"><span data-stu-id="15589-108">"Your request can't be completed.</span></span> <span data-ttu-id="15589-109">您必须是组织者才能取消会议。 "</span><span class="sxs-lookup"><span data-stu-id="15589-109">You need to be an organizer to cancel a meeting."</span></span>

<span data-ttu-id="15589-110">此操作与中的 "删除" 不同, "**取消**" 中的 "[删除](event-delete.md)" 仅对组织者可用, 并允许组织者向与会者发送有关取消的自定义消息。</span><span class="sxs-lookup"><span data-stu-id="15589-110">This action differs from [Delete](event-delete.md) in that **Cancel** is available to only the organizer, and lets the organizer send a custom message to the attendees about the cancellation.</span></span>

## <a name="permissions"></a><span data-ttu-id="15589-111">权限</span><span class="sxs-lookup"><span data-stu-id="15589-111">Permissions</span></span>
<span data-ttu-id="15589-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="15589-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="15589-114">权限类型</span><span class="sxs-lookup"><span data-stu-id="15589-114">Permission type</span></span>      | <span data-ttu-id="15589-115">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="15589-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="15589-116">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="15589-116">Delegated (work or school account)</span></span> | <span data-ttu-id="15589-117">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="15589-117">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="15589-118">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="15589-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="15589-119">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="15589-119">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="15589-120">应用程序</span><span class="sxs-lookup"><span data-stu-id="15589-120">Application</span></span> | <span data-ttu-id="15589-121">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="15589-121">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="15589-122">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="15589-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/events/{id}/cancel
POST /users/{id | userPrincipalName}/events/{id}/cancel
POST /groups/{id}/events/{id}/cancel

POST /me/calendar/events/{id}/cancel
POST /users/{id | userPrincipalName}/calendar/events/{id}/cancel
POST /groups/{id}/calendar/events/{id}/cancel

POST /me/calendars/{id}/events/{id}/cancel
POST /users/{id | userPrincipalName}/calendars/{id}/events/{id}/cancel

POST /me/calendargroup/calendars/{id}/events/{id}/cancel
POST /users/{id | userPrincipalName}/calendargroup/calendars/{id}/events/{id}/cancel

POST /me/calendargroups/{id}/calendars/{id}/events/{id}/cancel
POST /users/{id | userPrincipalName}/calendargroups/{id}/calendars/{id}/events/{id}/cancel
```
## <a name="request-headers"></a><span data-ttu-id="15589-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="15589-123">Request headers</span></span>
| <span data-ttu-id="15589-124">名称</span><span class="sxs-lookup"><span data-stu-id="15589-124">Name</span></span>       | <span data-ttu-id="15589-125">类型</span><span class="sxs-lookup"><span data-stu-id="15589-125">Type</span></span> | <span data-ttu-id="15589-126">说明</span><span class="sxs-lookup"><span data-stu-id="15589-126">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="15589-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="15589-127">Authorization</span></span>  | <span data-ttu-id="15589-128">string</span><span class="sxs-lookup"><span data-stu-id="15589-128">string</span></span>  | <span data-ttu-id="15589-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="15589-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="15589-131">Content-Type</span><span class="sxs-lookup"><span data-stu-id="15589-131">Content-Type</span></span> | <span data-ttu-id="15589-132">string</span><span class="sxs-lookup"><span data-stu-id="15589-132">string</span></span>  | <span data-ttu-id="15589-p105">实体正文中的数据性质。必需。</span><span class="sxs-lookup"><span data-stu-id="15589-p105">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="15589-135">请求正文</span><span class="sxs-lookup"><span data-stu-id="15589-135">Request body</span></span>
<span data-ttu-id="15589-136">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="15589-136">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="15589-137">参数</span><span class="sxs-lookup"><span data-stu-id="15589-137">Parameter</span></span>    | <span data-ttu-id="15589-138">类型</span><span class="sxs-lookup"><span data-stu-id="15589-138">Type</span></span>   |<span data-ttu-id="15589-139">说明</span><span class="sxs-lookup"><span data-stu-id="15589-139">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="15589-140">注释</span><span class="sxs-lookup"><span data-stu-id="15589-140">comment</span></span>|<span data-ttu-id="15589-141">String</span><span class="sxs-lookup"><span data-stu-id="15589-141">String</span></span>|<span data-ttu-id="15589-142">有关向所有与会者发送的取消的注释。</span><span class="sxs-lookup"><span data-stu-id="15589-142">A comment about the cancellation sent to all the attendees.</span></span> <span data-ttu-id="15589-143">可选。</span><span class="sxs-lookup"><span data-stu-id="15589-143">Optional.</span></span>|

## <a name="response"></a><span data-ttu-id="15589-144">响应</span><span class="sxs-lookup"><span data-stu-id="15589-144">Response</span></span>

<span data-ttu-id="15589-p107">如果成功，此方法返回 `202 Accepted` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="15589-p107">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="15589-147">示例</span><span class="sxs-lookup"><span data-stu-id="15589-147">Example</span></span>
<span data-ttu-id="15589-148">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="15589-148">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="15589-149">请求</span><span class="sxs-lookup"><span data-stu-id="15589-149">Request</span></span>
<span data-ttu-id="15589-150">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="15589-150">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "event_cancel"
}-->
```http
POST https://graph.microsoft.com/beta/me/events/{id}/cancel
Content-type: application/json

{
  "Comment": "Cancelling for this week due to all hands"
}
```

##### <a name="response"></a><span data-ttu-id="15589-151">响应</span><span class="sxs-lookup"><span data-stu-id="15589-151">Response</span></span>
<span data-ttu-id="15589-152">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="15589-152">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 202 Accepted
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="15589-153">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="15589-153">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="15589-154">C#</span><span class="sxs-lookup"><span data-stu-id="15589-154">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/event_cancel-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="15589-155">Javascript</span><span class="sxs-lookup"><span data-stu-id="15589-155">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/event_cancel-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="15589-156">目标-C</span><span class="sxs-lookup"><span data-stu-id="15589-156">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/event_cancel-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "event: cancel",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/event-cancel.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/event-cancel.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/event-cancel.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
