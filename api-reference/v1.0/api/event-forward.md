---
title: event： forward
description: '此操作允许会议事件的组织者或与会者转发 '
author: harini84
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 624312256cbca37529eb55eececa136df04d69fe
ms.sourcegitcommit: 0cde389d4d6dbec1568dab14490f0fd6297d5aa4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/19/2020
ms.locfileid: "49720743"
---
# <a name="event-forward"></a><span data-ttu-id="9321f-103">event： forward</span><span class="sxs-lookup"><span data-stu-id="9321f-103">event: forward</span></span>

<span data-ttu-id="9321f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9321f-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="9321f-105">此操作允许会议事件的组织者或与会者将会议请求[](../resources/event.md)转发给新收件人。</span><span class="sxs-lookup"><span data-stu-id="9321f-105">This action allows the organizer or attendee of a meeting [event](../resources/event.md) to forward the meeting request to a new recipient.</span></span> 

<span data-ttu-id="9321f-106">如果会议事件从与会者的 Microsoft 365 邮箱转发到另一个收件人，此操作还会发送一条消息，通知组织者转发，并将收件人添加到会议事件的组织者副本中。</span><span class="sxs-lookup"><span data-stu-id="9321f-106">If the meeting event is forwarded from an attendee's Microsoft 365 mailbox to another recipient, this action also sends a message to notify the organizer of the forwarding, and adds the recipient to the organizer's copy of the meeting event.</span></span> <span data-ttu-id="9321f-107">从帐户转发时，这种便利Outlook.com可用。</span><span class="sxs-lookup"><span data-stu-id="9321f-107">This convenience is not available when forwarding from an Outlook.com account.</span></span>

## <a name="permissions"></a><span data-ttu-id="9321f-108">权限</span><span class="sxs-lookup"><span data-stu-id="9321f-108">Permissions</span></span>
<span data-ttu-id="9321f-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9321f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9321f-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="9321f-111">Permission type</span></span>      | <span data-ttu-id="9321f-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="9321f-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9321f-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9321f-113">Delegated (work or school account)</span></span> | <span data-ttu-id="9321f-114">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="9321f-114">Calendars.Read</span></span>    |
|<span data-ttu-id="9321f-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9321f-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9321f-116">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="9321f-116">Calendars.Read</span></span>    |
|<span data-ttu-id="9321f-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="9321f-117">Application</span></span> | <span data-ttu-id="9321f-118">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="9321f-118">Calendars.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="9321f-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9321f-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/events/{id}/forward
POST /users/{id | userPrincipalName}/events/{id}/forward
POST /groups/{id}/events/{id}/forward

POST /me/calendar/events/{id}/forward
POST /users/{id | userPrincipalName}/calendar/events/{id}/forward
POST /groups/{id}/calendar/events/{id}/forward

POST /me/calendars/{id}/events/{id}/forward
POST /users/{id | userPrincipalName}/calendars/{id}/events/{id}/forward

POST /me/calendargroup/calendars/{id}/events/{id}/forward
POST /users/{id | userPrincipalName}/calendargroup/calendars/{id}/events/{id}/forward

POST /me/calendargroups/{id}/calendars/{id}/events/{id}/forward
POST /users/{id | userPrincipalName}/calendargroups/{id}/calendars/{id}/events/{id}/forward
```
## <a name="request-headers"></a><span data-ttu-id="9321f-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="9321f-120">Request headers</span></span>
| <span data-ttu-id="9321f-121">名称</span><span class="sxs-lookup"><span data-stu-id="9321f-121">Name</span></span>       | <span data-ttu-id="9321f-122">类型</span><span class="sxs-lookup"><span data-stu-id="9321f-122">Type</span></span> | <span data-ttu-id="9321f-123">说明</span><span class="sxs-lookup"><span data-stu-id="9321f-123">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="9321f-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="9321f-124">Authorization</span></span>  | <span data-ttu-id="9321f-125">string</span><span class="sxs-lookup"><span data-stu-id="9321f-125">string</span></span>  | <span data-ttu-id="9321f-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="9321f-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="9321f-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="9321f-128">Content-Type</span></span> | <span data-ttu-id="9321f-129">string</span><span class="sxs-lookup"><span data-stu-id="9321f-129">string</span></span>  | <span data-ttu-id="9321f-p104">实体正文中的数据性质。必需。</span><span class="sxs-lookup"><span data-stu-id="9321f-p104">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9321f-132">请求正文</span><span class="sxs-lookup"><span data-stu-id="9321f-132">Request body</span></span>
<span data-ttu-id="9321f-133">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="9321f-133">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="9321f-134">参数</span><span class="sxs-lookup"><span data-stu-id="9321f-134">Parameter</span></span>    | <span data-ttu-id="9321f-135">类型</span><span class="sxs-lookup"><span data-stu-id="9321f-135">Type</span></span>   |<span data-ttu-id="9321f-136">说明</span><span class="sxs-lookup"><span data-stu-id="9321f-136">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9321f-137">评论</span><span class="sxs-lookup"><span data-stu-id="9321f-137">Comment</span></span>|<span data-ttu-id="9321f-138">字符串</span><span class="sxs-lookup"><span data-stu-id="9321f-138">String</span></span>|<span data-ttu-id="9321f-p105">要包含的注释。可以为空字符串。</span><span class="sxs-lookup"><span data-stu-id="9321f-p105">A comment to include. Can be an empty string.</span></span>|
|<span data-ttu-id="9321f-141">ToRecipients</span><span class="sxs-lookup"><span data-stu-id="9321f-141">ToRecipients</span></span>|<span data-ttu-id="9321f-142">[recipient](../resources/recipient.md) collection</span><span class="sxs-lookup"><span data-stu-id="9321f-142">[recipient](../resources/recipient.md) collection</span></span>|<span data-ttu-id="9321f-143">将事件转发到的收件人列表。</span><span class="sxs-lookup"><span data-stu-id="9321f-143">The list of recipients to forward the event to.</span></span>|

## <a name="response"></a><span data-ttu-id="9321f-144">响应</span><span class="sxs-lookup"><span data-stu-id="9321f-144">Response</span></span>

<span data-ttu-id="9321f-p106">如果成功，此方法返回 `202 Accepted` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="9321f-p106">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9321f-147">示例</span><span class="sxs-lookup"><span data-stu-id="9321f-147">Example</span></span>
<span data-ttu-id="9321f-148">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="9321f-148">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="9321f-149">请求</span><span class="sxs-lookup"><span data-stu-id="9321f-149">Request</span></span>
<span data-ttu-id="9321f-150">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="9321f-150">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "event_forward"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/events/{id}/forward
Content-type: application/json
Content-length: 56

{
  "ToRecipients":[
      {
        "emailAddress": {
          "address":"danas@contoso.onmicrosoft.com",
          "name":"Dana Swope"
        }
      }
     ],
  "Comment": "Dana, hope you can make this meeting." 
}

```


##### <a name="response"></a><span data-ttu-id="9321f-151">响应</span><span class="sxs-lookup"><span data-stu-id="9321f-151">Response</span></span>
<span data-ttu-id="9321f-152">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="9321f-152">Here is an example of the response.</span></span>
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
  "description": "event: forward",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
