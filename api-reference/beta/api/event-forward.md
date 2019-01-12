---
title: 事件： 转接
description: '此操作允许组织者或与会者的会议事件转发 '
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: fe8d108ebeb15c2684e1997b8a02cc28a99101b1
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27990669"
---
# <a name="event-forward"></a><span data-ttu-id="47126-103">事件： 转接</span><span class="sxs-lookup"><span data-stu-id="47126-103">event: forward</span></span>

> <span data-ttu-id="47126-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="47126-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="47126-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="47126-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="47126-106">此操作允许组织者或与会者的会议[事件](../resources/event.md)，将会议请求转发到新的收件人。</span><span class="sxs-lookup"><span data-stu-id="47126-106">This action allows the organizer or attendee of a meeting [event](../resources/event.md) to forward the meeting request to a new recipient.</span></span> 

<span data-ttu-id="47126-107">如果从与会者的 Office 365 邮箱到另一个收件人转发会议事件时，此操作将还发送一条消息，通知的转发，组织者，并将收件人添加到的会议事件的组织者的副本。</span><span class="sxs-lookup"><span data-stu-id="47126-107">If the meeting event is forwarded from an attendee's Office 365 mailbox to another recipient, this action also sends a message to notify the organizer of the forwarding, and adds the recipient to the organizer's copy of the meeting event.</span></span> <span data-ttu-id="47126-108">转发 Outlook.com 帐户时，这种便利不可用。</span><span class="sxs-lookup"><span data-stu-id="47126-108">This convenience is not available when forwarding from an Outlook.com account.</span></span>


## <a name="permissions"></a><span data-ttu-id="47126-109">权限</span><span class="sxs-lookup"><span data-stu-id="47126-109">Permissions</span></span>
<span data-ttu-id="47126-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="47126-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="47126-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="47126-112">Permission type</span></span>      | <span data-ttu-id="47126-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="47126-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="47126-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="47126-114">Delegated (work or school account)</span></span> | <span data-ttu-id="47126-115">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="47126-115">Calendars.Read</span></span>    |
|<span data-ttu-id="47126-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="47126-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="47126-117">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="47126-117">Calendars.Read</span></span>    |
|<span data-ttu-id="47126-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="47126-118">Application</span></span> | <span data-ttu-id="47126-119">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="47126-119">Calendars.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="47126-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="47126-120">HTTP request</span></span>
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
## <a name="request-headers"></a><span data-ttu-id="47126-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="47126-121">Request headers</span></span>
| <span data-ttu-id="47126-122">名称</span><span class="sxs-lookup"><span data-stu-id="47126-122">Name</span></span>       | <span data-ttu-id="47126-123">类型</span><span class="sxs-lookup"><span data-stu-id="47126-123">Type</span></span> | <span data-ttu-id="47126-124">说明</span><span class="sxs-lookup"><span data-stu-id="47126-124">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="47126-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="47126-125">Authorization</span></span>  | <span data-ttu-id="47126-126">string</span><span class="sxs-lookup"><span data-stu-id="47126-126">string</span></span>  | <span data-ttu-id="47126-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="47126-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="47126-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="47126-129">Content-Type</span></span> | <span data-ttu-id="47126-130">string</span><span class="sxs-lookup"><span data-stu-id="47126-130">string</span></span>  | <span data-ttu-id="47126-p105">实体正文中的数据性质。必需。</span><span class="sxs-lookup"><span data-stu-id="47126-p105">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="47126-133">请求正文</span><span class="sxs-lookup"><span data-stu-id="47126-133">Request body</span></span>
<span data-ttu-id="47126-134">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="47126-134">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="47126-135">参数</span><span class="sxs-lookup"><span data-stu-id="47126-135">Parameter</span></span>    | <span data-ttu-id="47126-136">类型</span><span class="sxs-lookup"><span data-stu-id="47126-136">Type</span></span>   |<span data-ttu-id="47126-137">说明</span><span class="sxs-lookup"><span data-stu-id="47126-137">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="47126-138">Comment</span><span class="sxs-lookup"><span data-stu-id="47126-138">Comment</span></span>|<span data-ttu-id="47126-139">String</span><span class="sxs-lookup"><span data-stu-id="47126-139">String</span></span>|<span data-ttu-id="47126-p106">要包含的注释。可以为空字符串。</span><span class="sxs-lookup"><span data-stu-id="47126-p106">A comment to include. Can be an empty string.</span></span>|
|<span data-ttu-id="47126-142">ToRecipients</span><span class="sxs-lookup"><span data-stu-id="47126-142">ToRecipients</span></span>|<span data-ttu-id="47126-143">[recipient](../resources/recipient.md) collection</span><span class="sxs-lookup"><span data-stu-id="47126-143">[recipient](../resources/recipient.md) collection</span></span>|<span data-ttu-id="47126-144">要转接到的事件的收件人列表。</span><span class="sxs-lookup"><span data-stu-id="47126-144">The list of recipients to forward the event to.</span></span>|

## <a name="response"></a><span data-ttu-id="47126-145">响应</span><span class="sxs-lookup"><span data-stu-id="47126-145">Response</span></span>

<span data-ttu-id="47126-p107">如果成功，此方法返回 `202 Accepted` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="47126-p107">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="47126-148">示例</span><span class="sxs-lookup"><span data-stu-id="47126-148">Example</span></span>
<span data-ttu-id="47126-149">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="47126-149">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="47126-150">请求</span><span class="sxs-lookup"><span data-stu-id="47126-150">Request</span></span>
<span data-ttu-id="47126-151">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="47126-151">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "event_forward"
}-->
```http
POST https://graph.microsoft.com/beta/me/events/{id}/forward
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

##### <a name="response"></a><span data-ttu-id="47126-152">响应</span><span class="sxs-lookup"><span data-stu-id="47126-152">Response</span></span>
<span data-ttu-id="47126-153">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="47126-153">Here is an example of the response.</span></span>
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
  "description": "event: forward",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
