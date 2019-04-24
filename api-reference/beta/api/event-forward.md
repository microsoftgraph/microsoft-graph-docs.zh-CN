---
title: '事件: 前进'
description: '此操作允许会议事件的组织者或与会者转发 '
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 6f1b3e1f089d927aeb21ca80ff77edda63121c60
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32464340"
---
# <a name="event-forward"></a><span data-ttu-id="39b55-103">事件: 前进</span><span class="sxs-lookup"><span data-stu-id="39b55-103">event: forward</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="39b55-104">此操作允许会议[事件](../resources/event.md)的组织者或与会者将会议请求转发给新的收件人。</span><span class="sxs-lookup"><span data-stu-id="39b55-104">This action allows the organizer or attendee of a meeting [event](../resources/event.md) to forward the meeting request to a new recipient.</span></span> 

<span data-ttu-id="39b55-105">如果将会议事件从与会者的 Office 365 邮箱转发给另一个收件人, 此操作还会发送一封邮件, 通知组织者转发, 并将该收件人添加到组织者的会议事件副本中。</span><span class="sxs-lookup"><span data-stu-id="39b55-105">If the meeting event is forwarded from an attendee's Office 365 mailbox to another recipient, this action also sends a message to notify the organizer of the forwarding, and adds the recipient to the organizer's copy of the meeting event.</span></span> <span data-ttu-id="39b55-106">从 Outlook.com 帐户进行转发时, 此便利功能不可用。</span><span class="sxs-lookup"><span data-stu-id="39b55-106">This convenience is not available when forwarding from an Outlook.com account.</span></span>


## <a name="permissions"></a><span data-ttu-id="39b55-107">权限</span><span class="sxs-lookup"><span data-stu-id="39b55-107">Permissions</span></span>
<span data-ttu-id="39b55-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="39b55-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="39b55-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="39b55-110">Permission type</span></span>      | <span data-ttu-id="39b55-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="39b55-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="39b55-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="39b55-112">Delegated (work or school account)</span></span> | <span data-ttu-id="39b55-113">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="39b55-113">Calendars.Read</span></span>    |
|<span data-ttu-id="39b55-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="39b55-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="39b55-115">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="39b55-115">Calendars.Read</span></span>    |
|<span data-ttu-id="39b55-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="39b55-116">Application</span></span> | <span data-ttu-id="39b55-117">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="39b55-117">Calendars.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="39b55-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="39b55-118">HTTP request</span></span>
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
## <a name="request-headers"></a><span data-ttu-id="39b55-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="39b55-119">Request headers</span></span>
| <span data-ttu-id="39b55-120">名称</span><span class="sxs-lookup"><span data-stu-id="39b55-120">Name</span></span>       | <span data-ttu-id="39b55-121">类型</span><span class="sxs-lookup"><span data-stu-id="39b55-121">Type</span></span> | <span data-ttu-id="39b55-122">说明</span><span class="sxs-lookup"><span data-stu-id="39b55-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="39b55-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="39b55-123">Authorization</span></span>  | <span data-ttu-id="39b55-124">string</span><span class="sxs-lookup"><span data-stu-id="39b55-124">string</span></span>  | <span data-ttu-id="39b55-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="39b55-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="39b55-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="39b55-127">Content-Type</span></span> | <span data-ttu-id="39b55-128">string</span><span class="sxs-lookup"><span data-stu-id="39b55-128">string</span></span>  | <span data-ttu-id="39b55-p104">实体正文中的数据性质。必需。</span><span class="sxs-lookup"><span data-stu-id="39b55-p104">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="39b55-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="39b55-131">Request body</span></span>
<span data-ttu-id="39b55-132">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="39b55-132">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="39b55-133">参数</span><span class="sxs-lookup"><span data-stu-id="39b55-133">Parameter</span></span>    | <span data-ttu-id="39b55-134">类型</span><span class="sxs-lookup"><span data-stu-id="39b55-134">Type</span></span>   |<span data-ttu-id="39b55-135">说明</span><span class="sxs-lookup"><span data-stu-id="39b55-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="39b55-136">Comment</span><span class="sxs-lookup"><span data-stu-id="39b55-136">Comment</span></span>|<span data-ttu-id="39b55-137">String</span><span class="sxs-lookup"><span data-stu-id="39b55-137">String</span></span>|<span data-ttu-id="39b55-p105">要包含的注释。可以为空字符串。</span><span class="sxs-lookup"><span data-stu-id="39b55-p105">A comment to include. Can be an empty string.</span></span>|
|<span data-ttu-id="39b55-140">ToRecipients</span><span class="sxs-lookup"><span data-stu-id="39b55-140">ToRecipients</span></span>|<span data-ttu-id="39b55-141">[recipient](../resources/recipient.md) collection</span><span class="sxs-lookup"><span data-stu-id="39b55-141">[recipient](../resources/recipient.md) collection</span></span>|<span data-ttu-id="39b55-142">要将事件转发到的收件人列表。</span><span class="sxs-lookup"><span data-stu-id="39b55-142">The list of recipients to forward the event to.</span></span>|

## <a name="response"></a><span data-ttu-id="39b55-143">响应</span><span class="sxs-lookup"><span data-stu-id="39b55-143">Response</span></span>

<span data-ttu-id="39b55-p106">如果成功，此方法返回 `202 Accepted` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="39b55-p106">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="39b55-146">示例</span><span class="sxs-lookup"><span data-stu-id="39b55-146">Example</span></span>
<span data-ttu-id="39b55-147">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="39b55-147">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="39b55-148">请求</span><span class="sxs-lookup"><span data-stu-id="39b55-148">Request</span></span>
<span data-ttu-id="39b55-149">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="39b55-149">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="39b55-150">响应</span><span class="sxs-lookup"><span data-stu-id="39b55-150">Response</span></span>
<span data-ttu-id="39b55-151">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="39b55-151">Here is an example of the response.</span></span>
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
    "Error: /api-reference/beta/api/event-forward.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
