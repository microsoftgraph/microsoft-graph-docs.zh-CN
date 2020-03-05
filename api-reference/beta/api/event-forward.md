---
title: 事件：前进
description: '此操作允许会议事件的组织者或与会者转发 '
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 139d88c083269d92077da57eca1a730dfe314081
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42422977"
---
# <a name="event-forward"></a><span data-ttu-id="f7724-103">事件：前进</span><span class="sxs-lookup"><span data-stu-id="f7724-103">event: forward</span></span>

<span data-ttu-id="f7724-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="f7724-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f7724-105">此操作允许会议[事件](../resources/event.md)的组织者或与会者将会议请求转发给新的收件人。</span><span class="sxs-lookup"><span data-stu-id="f7724-105">This action allows the organizer or attendee of a meeting [event](../resources/event.md) to forward the meeting request to a new recipient.</span></span> 

<span data-ttu-id="f7724-106">如果将会议事件从与会者的 Office 365 邮箱转发给另一个收件人，此操作还会发送一封邮件，通知组织者转发，并将该收件人添加到组织者的会议事件副本中。</span><span class="sxs-lookup"><span data-stu-id="f7724-106">If the meeting event is forwarded from an attendee's Office 365 mailbox to another recipient, this action also sends a message to notify the organizer of the forwarding, and adds the recipient to the organizer's copy of the meeting event.</span></span> <span data-ttu-id="f7724-107">从 Outlook.com 帐户进行转发时，此便利功能不可用。</span><span class="sxs-lookup"><span data-stu-id="f7724-107">This convenience is not available when forwarding from an Outlook.com account.</span></span>


## <a name="permissions"></a><span data-ttu-id="f7724-108">权限</span><span class="sxs-lookup"><span data-stu-id="f7724-108">Permissions</span></span>
<span data-ttu-id="f7724-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f7724-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f7724-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="f7724-111">Permission type</span></span>      | <span data-ttu-id="f7724-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f7724-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f7724-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f7724-113">Delegated (work or school account)</span></span> | <span data-ttu-id="f7724-114">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="f7724-114">Calendars.Read</span></span>    |
|<span data-ttu-id="f7724-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f7724-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f7724-116">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="f7724-116">Calendars.Read</span></span>    |
|<span data-ttu-id="f7724-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="f7724-117">Application</span></span> | <span data-ttu-id="f7724-118">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="f7724-118">Calendars.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="f7724-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f7724-119">HTTP request</span></span>
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
## <a name="request-headers"></a><span data-ttu-id="f7724-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="f7724-120">Request headers</span></span>
| <span data-ttu-id="f7724-121">名称</span><span class="sxs-lookup"><span data-stu-id="f7724-121">Name</span></span>       | <span data-ttu-id="f7724-122">类型</span><span class="sxs-lookup"><span data-stu-id="f7724-122">Type</span></span> | <span data-ttu-id="f7724-123">说明</span><span class="sxs-lookup"><span data-stu-id="f7724-123">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="f7724-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="f7724-124">Authorization</span></span>  | <span data-ttu-id="f7724-125">string</span><span class="sxs-lookup"><span data-stu-id="f7724-125">string</span></span>  | <span data-ttu-id="f7724-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="f7724-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="f7724-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f7724-128">Content-Type</span></span> | <span data-ttu-id="f7724-129">string</span><span class="sxs-lookup"><span data-stu-id="f7724-129">string</span></span>  | <span data-ttu-id="f7724-p104">实体正文中的数据性质。必需。</span><span class="sxs-lookup"><span data-stu-id="f7724-p104">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f7724-132">请求正文</span><span class="sxs-lookup"><span data-stu-id="f7724-132">Request body</span></span>
<span data-ttu-id="f7724-133">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="f7724-133">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="f7724-134">参数</span><span class="sxs-lookup"><span data-stu-id="f7724-134">Parameter</span></span>    | <span data-ttu-id="f7724-135">类型</span><span class="sxs-lookup"><span data-stu-id="f7724-135">Type</span></span>   |<span data-ttu-id="f7724-136">说明</span><span class="sxs-lookup"><span data-stu-id="f7724-136">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f7724-137">评论</span><span class="sxs-lookup"><span data-stu-id="f7724-137">Comment</span></span>|<span data-ttu-id="f7724-138">字符串</span><span class="sxs-lookup"><span data-stu-id="f7724-138">String</span></span>|<span data-ttu-id="f7724-p105">要包含的注释。可以为空字符串。</span><span class="sxs-lookup"><span data-stu-id="f7724-p105">A comment to include. Can be an empty string.</span></span>|
|<span data-ttu-id="f7724-141">ToRecipients</span><span class="sxs-lookup"><span data-stu-id="f7724-141">ToRecipients</span></span>|<span data-ttu-id="f7724-142">[recipient](../resources/recipient.md) collection</span><span class="sxs-lookup"><span data-stu-id="f7724-142">[recipient](../resources/recipient.md) collection</span></span>|<span data-ttu-id="f7724-143">要将事件转发到的收件人列表。</span><span class="sxs-lookup"><span data-stu-id="f7724-143">The list of recipients to forward the event to.</span></span>|

## <a name="response"></a><span data-ttu-id="f7724-144">响应</span><span class="sxs-lookup"><span data-stu-id="f7724-144">Response</span></span>

<span data-ttu-id="f7724-p106">如果成功，此方法返回 `202 Accepted` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="f7724-p106">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f7724-147">示例</span><span class="sxs-lookup"><span data-stu-id="f7724-147">Example</span></span>
<span data-ttu-id="f7724-148">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="f7724-148">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="f7724-149">请求</span><span class="sxs-lookup"><span data-stu-id="f7724-149">Request</span></span>
<span data-ttu-id="f7724-150">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="f7724-150">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="f7724-151">HTTP</span><span class="sxs-lookup"><span data-stu-id="f7724-151">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="f7724-152">C#</span><span class="sxs-lookup"><span data-stu-id="f7724-152">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/event-forward-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f7724-153">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f7724-153">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/event-forward-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f7724-154">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f7724-154">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/event-forward-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="f7724-155">响应</span><span class="sxs-lookup"><span data-stu-id="f7724-155">Response</span></span>
<span data-ttu-id="f7724-156">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="f7724-156">Here is an example of the response.</span></span>
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
