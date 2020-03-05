---
title: 事件：取消
description: '此操作允许会议组织者发送取消邮件并取消事件。 '
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 0558bc37421391cd565e197e76365840aa8a97a0
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42423390"
---
# <a name="event-cancel"></a><span data-ttu-id="21cd2-103">事件：取消</span><span class="sxs-lookup"><span data-stu-id="21cd2-103">event: cancel</span></span>

<span data-ttu-id="21cd2-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="21cd2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="21cd2-105">此操作允许会议组织者发送取消邮件并取消事件。</span><span class="sxs-lookup"><span data-stu-id="21cd2-105">This action allows the organizer of a meeting to send a cancellation message and cancel the event.</span></span> 

<span data-ttu-id="21cd2-106">该操作会将事件移动到 "已删除邮件" 文件夹中。</span><span class="sxs-lookup"><span data-stu-id="21cd2-106">The action moves the event to the Deleted Items folder.</span></span> <span data-ttu-id="21cd2-107">组织者还可以通过提供发生事件 ID 来取消定期会议的事件。</span><span class="sxs-lookup"><span data-stu-id="21cd2-107">The organizer can also cancel an occurrence of a recurring meeting by providing the occurrence event ID.</span></span> <span data-ttu-id="21cd2-108">调用此操作的与会者将收到错误（HTTP 400 错误请求），并提供以下错误消息：</span><span class="sxs-lookup"><span data-stu-id="21cd2-108">An attendee calling this action gets an error (HTTP 400 Bad Request), with the following error message:</span></span>

<span data-ttu-id="21cd2-109">无法完成您的请求。</span><span class="sxs-lookup"><span data-stu-id="21cd2-109">"Your request can't be completed.</span></span> <span data-ttu-id="21cd2-110">您必须是组织者才能取消会议。 "</span><span class="sxs-lookup"><span data-stu-id="21cd2-110">You need to be an organizer to cancel a meeting."</span></span>

<span data-ttu-id="21cd2-111">此操作与中的 "删除" 不同，"**取消**" 中的 "[删除](event-delete.md)" 仅对组织者可用，并允许组织者向与会者发送有关取消的自定义消息。</span><span class="sxs-lookup"><span data-stu-id="21cd2-111">This action differs from [Delete](event-delete.md) in that **Cancel** is available to only the organizer, and lets the organizer send a custom message to the attendees about the cancellation.</span></span>

## <a name="permissions"></a><span data-ttu-id="21cd2-112">权限</span><span class="sxs-lookup"><span data-stu-id="21cd2-112">Permissions</span></span>
<span data-ttu-id="21cd2-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="21cd2-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="21cd2-115">权限类型</span><span class="sxs-lookup"><span data-stu-id="21cd2-115">Permission type</span></span>      | <span data-ttu-id="21cd2-116">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="21cd2-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="21cd2-117">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="21cd2-117">Delegated (work or school account)</span></span> | <span data-ttu-id="21cd2-118">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="21cd2-118">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="21cd2-119">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="21cd2-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="21cd2-120">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="21cd2-120">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="21cd2-121">应用程序</span><span class="sxs-lookup"><span data-stu-id="21cd2-121">Application</span></span> | <span data-ttu-id="21cd2-122">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="21cd2-122">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="21cd2-123">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="21cd2-123">HTTP request</span></span>
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
## <a name="request-headers"></a><span data-ttu-id="21cd2-124">请求标头</span><span class="sxs-lookup"><span data-stu-id="21cd2-124">Request headers</span></span>
| <span data-ttu-id="21cd2-125">名称</span><span class="sxs-lookup"><span data-stu-id="21cd2-125">Name</span></span>       | <span data-ttu-id="21cd2-126">类型</span><span class="sxs-lookup"><span data-stu-id="21cd2-126">Type</span></span> | <span data-ttu-id="21cd2-127">说明</span><span class="sxs-lookup"><span data-stu-id="21cd2-127">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="21cd2-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="21cd2-128">Authorization</span></span>  | <span data-ttu-id="21cd2-129">string</span><span class="sxs-lookup"><span data-stu-id="21cd2-129">string</span></span>  | <span data-ttu-id="21cd2-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="21cd2-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="21cd2-132">Content-Type</span><span class="sxs-lookup"><span data-stu-id="21cd2-132">Content-Type</span></span> | <span data-ttu-id="21cd2-133">string</span><span class="sxs-lookup"><span data-stu-id="21cd2-133">string</span></span>  | <span data-ttu-id="21cd2-p105">实体正文中的数据性质。必需。</span><span class="sxs-lookup"><span data-stu-id="21cd2-p105">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="21cd2-136">请求正文</span><span class="sxs-lookup"><span data-stu-id="21cd2-136">Request body</span></span>
<span data-ttu-id="21cd2-137">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="21cd2-137">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="21cd2-138">参数</span><span class="sxs-lookup"><span data-stu-id="21cd2-138">Parameter</span></span>    | <span data-ttu-id="21cd2-139">类型</span><span class="sxs-lookup"><span data-stu-id="21cd2-139">Type</span></span>   |<span data-ttu-id="21cd2-140">说明</span><span class="sxs-lookup"><span data-stu-id="21cd2-140">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="21cd2-141">注释</span><span class="sxs-lookup"><span data-stu-id="21cd2-141">comment</span></span>|<span data-ttu-id="21cd2-142">String</span><span class="sxs-lookup"><span data-stu-id="21cd2-142">String</span></span>|<span data-ttu-id="21cd2-143">有关向所有与会者发送的取消的注释。</span><span class="sxs-lookup"><span data-stu-id="21cd2-143">A comment about the cancellation sent to all the attendees.</span></span> <span data-ttu-id="21cd2-144">可选。</span><span class="sxs-lookup"><span data-stu-id="21cd2-144">Optional.</span></span>|

## <a name="response"></a><span data-ttu-id="21cd2-145">响应</span><span class="sxs-lookup"><span data-stu-id="21cd2-145">Response</span></span>

<span data-ttu-id="21cd2-p107">如果成功，此方法返回 `202 Accepted` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="21cd2-p107">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="21cd2-148">示例</span><span class="sxs-lookup"><span data-stu-id="21cd2-148">Example</span></span>
<span data-ttu-id="21cd2-149">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="21cd2-149">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="21cd2-150">请求</span><span class="sxs-lookup"><span data-stu-id="21cd2-150">Request</span></span>
<span data-ttu-id="21cd2-151">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="21cd2-151">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="21cd2-152">HTTP</span><span class="sxs-lookup"><span data-stu-id="21cd2-152">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="21cd2-153">C#</span><span class="sxs-lookup"><span data-stu-id="21cd2-153">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/event-cancel-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="21cd2-154">JavaScript</span><span class="sxs-lookup"><span data-stu-id="21cd2-154">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/event-cancel-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="21cd2-155">Objective-C</span><span class="sxs-lookup"><span data-stu-id="21cd2-155">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/event-cancel-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="21cd2-156">响应</span><span class="sxs-lookup"><span data-stu-id="21cd2-156">Response</span></span>
<span data-ttu-id="21cd2-157">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="21cd2-157">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
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
  "description": "event: cancel",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
