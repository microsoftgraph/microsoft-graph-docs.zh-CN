---
title: event： cancel
description: '此操作允许会议的组织者发送取消消息并取消事件。 '
author: harini84
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: a0d9c8dae2998d38bb9bde56fcf2cd0d49e691b9
ms.sourcegitcommit: 0cde389d4d6dbec1568dab14490f0fd6297d5aa4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/19/2020
ms.locfileid: "49720734"
---
# <a name="event-cancel"></a><span data-ttu-id="f5d04-103">event： cancel</span><span class="sxs-lookup"><span data-stu-id="f5d04-103">event: cancel</span></span>

<span data-ttu-id="f5d04-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f5d04-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="f5d04-105">此操作允许会议的组织者发送取消消息并取消事件。</span><span class="sxs-lookup"><span data-stu-id="f5d04-105">This action allows the organizer of a meeting to send a cancellation message and cancel the event.</span></span> 

<span data-ttu-id="f5d04-106">该操作将事件移动到"已删除邮件"文件夹。</span><span class="sxs-lookup"><span data-stu-id="f5d04-106">The action moves the event to the Deleted Items folder.</span></span> <span data-ttu-id="f5d04-107">组织者还可以通过提供定期会议的事件 ID 来取消定期会议。</span><span class="sxs-lookup"><span data-stu-id="f5d04-107">The organizer can also cancel an occurrence of a recurring meeting by providing the occurrence event ID.</span></span> <span data-ttu-id="f5d04-108">调用此操作的与会者 (HTTP 400 错误) 错误，并出现以下错误消息：</span><span class="sxs-lookup"><span data-stu-id="f5d04-108">An attendee calling this action gets an error (HTTP 400 Bad Request), with the following error message:</span></span>

<span data-ttu-id="f5d04-109">"您的请求无法完成。</span><span class="sxs-lookup"><span data-stu-id="f5d04-109">"Your request can't be completed.</span></span> <span data-ttu-id="f5d04-110">你需要是组织者来取消会议。"</span><span class="sxs-lookup"><span data-stu-id="f5d04-110">You need to be an organizer to cancel a meeting."</span></span>

<span data-ttu-id="f5d04-111">此操作与 ["](event-delete.md) 删除"不同， **即** "取消"仅对组织者可用，并且允许组织者向与会者发送有关取消的自定义消息。</span><span class="sxs-lookup"><span data-stu-id="f5d04-111">This action differs from [Delete](event-delete.md) in that **Cancel** is available to only the organizer, and lets the organizer send a custom message to the attendees about the cancellation.</span></span>

## <a name="permissions"></a><span data-ttu-id="f5d04-112">权限</span><span class="sxs-lookup"><span data-stu-id="f5d04-112">Permissions</span></span>
<span data-ttu-id="f5d04-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f5d04-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f5d04-115">权限类型</span><span class="sxs-lookup"><span data-stu-id="f5d04-115">Permission type</span></span>      | <span data-ttu-id="f5d04-116">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f5d04-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f5d04-117">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f5d04-117">Delegated (work or school account)</span></span> | <span data-ttu-id="f5d04-118">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f5d04-118">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="f5d04-119">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f5d04-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f5d04-120">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f5d04-120">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="f5d04-121">应用程序</span><span class="sxs-lookup"><span data-stu-id="f5d04-121">Application</span></span> | <span data-ttu-id="f5d04-122">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f5d04-122">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="f5d04-123">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f5d04-123">HTTP request</span></span>
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
## <a name="request-headers"></a><span data-ttu-id="f5d04-124">请求标头</span><span class="sxs-lookup"><span data-stu-id="f5d04-124">Request headers</span></span>
| <span data-ttu-id="f5d04-125">名称</span><span class="sxs-lookup"><span data-stu-id="f5d04-125">Name</span></span>       | <span data-ttu-id="f5d04-126">类型</span><span class="sxs-lookup"><span data-stu-id="f5d04-126">Type</span></span> | <span data-ttu-id="f5d04-127">说明</span><span class="sxs-lookup"><span data-stu-id="f5d04-127">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="f5d04-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="f5d04-128">Authorization</span></span>  | <span data-ttu-id="f5d04-129">string</span><span class="sxs-lookup"><span data-stu-id="f5d04-129">string</span></span>  | <span data-ttu-id="f5d04-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="f5d04-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="f5d04-132">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f5d04-132">Content-Type</span></span> | <span data-ttu-id="f5d04-133">string</span><span class="sxs-lookup"><span data-stu-id="f5d04-133">string</span></span>  | <span data-ttu-id="f5d04-p105">实体正文中的数据性质。必需。</span><span class="sxs-lookup"><span data-stu-id="f5d04-p105">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f5d04-136">请求正文</span><span class="sxs-lookup"><span data-stu-id="f5d04-136">Request body</span></span>
<span data-ttu-id="f5d04-137">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="f5d04-137">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="f5d04-138">参数</span><span class="sxs-lookup"><span data-stu-id="f5d04-138">Parameter</span></span>    | <span data-ttu-id="f5d04-139">类型</span><span class="sxs-lookup"><span data-stu-id="f5d04-139">Type</span></span>   |<span data-ttu-id="f5d04-140">说明</span><span class="sxs-lookup"><span data-stu-id="f5d04-140">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f5d04-141">注释</span><span class="sxs-lookup"><span data-stu-id="f5d04-141">comment</span></span>|<span data-ttu-id="f5d04-142">String</span><span class="sxs-lookup"><span data-stu-id="f5d04-142">String</span></span>|<span data-ttu-id="f5d04-143">有关发送给所有与会者的取消的注释。</span><span class="sxs-lookup"><span data-stu-id="f5d04-143">A comment about the cancellation sent to all the attendees.</span></span> <span data-ttu-id="f5d04-144">可选。</span><span class="sxs-lookup"><span data-stu-id="f5d04-144">Optional.</span></span>|

## <a name="response"></a><span data-ttu-id="f5d04-145">响应</span><span class="sxs-lookup"><span data-stu-id="f5d04-145">Response</span></span>

<span data-ttu-id="f5d04-p107">如果成功，此方法返回 `202 Accepted` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="f5d04-p107">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f5d04-148">示例</span><span class="sxs-lookup"><span data-stu-id="f5d04-148">Example</span></span>
<span data-ttu-id="f5d04-149">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="f5d04-149">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="f5d04-150">请求</span><span class="sxs-lookup"><span data-stu-id="f5d04-150">Request</span></span>
<span data-ttu-id="f5d04-151">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="f5d04-151">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "event_cancel"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/events/{id}/cancel
Content-type: application/json

{
  "Comment": "Cancelling for this week due to all hands"
}
```


##### <a name="response"></a><span data-ttu-id="f5d04-152">响应</span><span class="sxs-lookup"><span data-stu-id="f5d04-152">Response</span></span>
<span data-ttu-id="f5d04-153">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="f5d04-153">Here is an example of the response.</span></span>
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
