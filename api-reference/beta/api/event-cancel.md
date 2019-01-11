---
title: 事件： 取消
description: '此操作允许组织者的会议发送取消邮件和取消事件。 '
author: angelgolfer-ms
localization_priority: Normal
ms.openlocfilehash: 482804d58078f148ed321a0c3489954fc9144f8e
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27864622"
---
# <a name="event-cancel"></a><span data-ttu-id="73201-103">事件： 取消</span><span class="sxs-lookup"><span data-stu-id="73201-103">event: cancel</span></span>

> <span data-ttu-id="73201-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="73201-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="73201-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="73201-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="73201-106">此操作允许组织者的会议发送取消邮件和取消事件。</span><span class="sxs-lookup"><span data-stu-id="73201-106">This action allows the organizer of a meeting to send a cancellation message and cancel the event.</span></span> 

<span data-ttu-id="73201-107">操作将事件移到已删除邮件文件夹中。</span><span class="sxs-lookup"><span data-stu-id="73201-107">The action moves the event to the Deleted Items folder.</span></span> <span data-ttu-id="73201-108">组织者还可以取消的定期会议通过提供出现事件 id。</span><span class="sxs-lookup"><span data-stu-id="73201-108">The organizer can also cancel an occurrence of a recurring meeting by providing the occurrence event ID.</span></span> <span data-ttu-id="73201-109">调用此操作与会者获取错误 （HTTP 400 错误请求），与以下错误消息：</span><span class="sxs-lookup"><span data-stu-id="73201-109">An attendee calling this action gets an error (HTTP 400 Bad Request), with the following error message:</span></span>

<span data-ttu-id="73201-110">"无法完成您的请求。</span><span class="sxs-lookup"><span data-stu-id="73201-110">"Your request can't be completed.</span></span> <span data-ttu-id="73201-111">您需要取消会议组织者。"</span><span class="sxs-lookup"><span data-stu-id="73201-111">You need to be an organizer to cancel a meeting."</span></span>

<span data-ttu-id="73201-112">此操作与[删除](event-delete.md)区别在于**取消**可供仅组织者，并允许组织者向取消有关与会者发送自定义消息。</span><span class="sxs-lookup"><span data-stu-id="73201-112">This action differs from [Delete](event-delete.md) in that **Cancel** is available to only the organizer, and lets the organizer send a custom message to the attendees about the cancellation.</span></span>

## <a name="permissions"></a><span data-ttu-id="73201-113">权限</span><span class="sxs-lookup"><span data-stu-id="73201-113">Permissions</span></span>
<span data-ttu-id="73201-p104">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="73201-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="73201-116">权限类型</span><span class="sxs-lookup"><span data-stu-id="73201-116">Permission type</span></span>      | <span data-ttu-id="73201-117">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="73201-117">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="73201-118">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="73201-118">Delegated (work or school account)</span></span> | <span data-ttu-id="73201-119">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="73201-119">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="73201-120">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="73201-120">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="73201-121">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="73201-121">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="73201-122">应用程序</span><span class="sxs-lookup"><span data-stu-id="73201-122">Application</span></span> | <span data-ttu-id="73201-123">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="73201-123">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="73201-124">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="73201-124">HTTP request</span></span>
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
## <a name="request-headers"></a><span data-ttu-id="73201-125">请求标头</span><span class="sxs-lookup"><span data-stu-id="73201-125">Request headers</span></span>
| <span data-ttu-id="73201-126">名称</span><span class="sxs-lookup"><span data-stu-id="73201-126">Name</span></span>       | <span data-ttu-id="73201-127">类型</span><span class="sxs-lookup"><span data-stu-id="73201-127">Type</span></span> | <span data-ttu-id="73201-128">说明</span><span class="sxs-lookup"><span data-stu-id="73201-128">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="73201-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="73201-129">Authorization</span></span>  | <span data-ttu-id="73201-130">string</span><span class="sxs-lookup"><span data-stu-id="73201-130">string</span></span>  | <span data-ttu-id="73201-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="73201-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="73201-133">Content-Type</span><span class="sxs-lookup"><span data-stu-id="73201-133">Content-Type</span></span> | <span data-ttu-id="73201-134">string</span><span class="sxs-lookup"><span data-stu-id="73201-134">string</span></span>  | <span data-ttu-id="73201-p106">实体正文中的数据性质。必需。</span><span class="sxs-lookup"><span data-stu-id="73201-p106">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="73201-137">请求正文</span><span class="sxs-lookup"><span data-stu-id="73201-137">Request body</span></span>
<span data-ttu-id="73201-138">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="73201-138">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="73201-139">参数</span><span class="sxs-lookup"><span data-stu-id="73201-139">Parameter</span></span>    | <span data-ttu-id="73201-140">类型</span><span class="sxs-lookup"><span data-stu-id="73201-140">Type</span></span>   |<span data-ttu-id="73201-141">说明</span><span class="sxs-lookup"><span data-stu-id="73201-141">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="73201-142">注释</span><span class="sxs-lookup"><span data-stu-id="73201-142">comment</span></span>|<span data-ttu-id="73201-143">String</span><span class="sxs-lookup"><span data-stu-id="73201-143">String</span></span>|<span data-ttu-id="73201-144">有关取消发送给所有与会者的注释。</span><span class="sxs-lookup"><span data-stu-id="73201-144">A comment about the cancellation sent to all the attendees.</span></span> <span data-ttu-id="73201-145">可选。</span><span class="sxs-lookup"><span data-stu-id="73201-145">Optional.</span></span>|

## <a name="response"></a><span data-ttu-id="73201-146">响应</span><span class="sxs-lookup"><span data-stu-id="73201-146">Response</span></span>

<span data-ttu-id="73201-p108">如果成功，此方法返回 `202 Accepted` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="73201-p108">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="73201-149">示例</span><span class="sxs-lookup"><span data-stu-id="73201-149">Example</span></span>
<span data-ttu-id="73201-150">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="73201-150">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="73201-151">请求</span><span class="sxs-lookup"><span data-stu-id="73201-151">Request</span></span>
<span data-ttu-id="73201-152">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="73201-152">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="73201-153">响应</span><span class="sxs-lookup"><span data-stu-id="73201-153">Response</span></span>
<span data-ttu-id="73201-154">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="73201-154">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 202 Accepted
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "event: cancel",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
