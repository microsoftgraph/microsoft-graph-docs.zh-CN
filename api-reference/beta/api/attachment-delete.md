---
title: 删除附件
description: 从日历事件、邮件、Outlook 任务或帖子中删除附件。
localization_priority: Normal
doc_type: apiPageType
ms.prod: outlook
author: angelgolfer-ms
ms.openlocfilehash: f3e4a06e86ef5da90851a84055e3162ae475129f
ms.sourcegitcommit: 83a053067f6248fb49ec5d473738ab1555fb4295
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/24/2019
ms.locfileid: "36622556"
---
# <a name="delete-attachment"></a><span data-ttu-id="6a1f5-103">删除附件</span><span class="sxs-lookup"><span data-stu-id="6a1f5-103">Delete attachment</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6a1f5-104">删除用户日历[事件](../resources/event.md)、[邮件](../resources/message.md)、 [Outlook 任务](../resources/outlooktask.md)或[帖子](../resources/post.md)中的附件。</span><span class="sxs-lookup"><span data-stu-id="6a1f5-104">Delete an attachment from a user calendar [event](../resources/event.md), [message](../resources/message.md), [Outlook task](../resources/outlooktask.md), or [post](../resources/post.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="6a1f5-105">权限</span><span class="sxs-lookup"><span data-stu-id="6a1f5-105">Permissions</span></span>

<span data-ttu-id="6a1f5-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6a1f5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

* <span data-ttu-id="6a1f5-108">如果访问邮件中的附件: Mail. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6a1f5-108">If accessing attachments in messages: Mail.ReadWrite</span></span>
* <span data-ttu-id="6a1f5-109">如果访问事件中的附件: 日历. 读写</span><span class="sxs-lookup"><span data-stu-id="6a1f5-109">If accessing attachments in events: Calendars.ReadWrite</span></span>
* <span data-ttu-id="6a1f5-110">如果访问 Outlook 任务中的附件: Tasks. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6a1f5-110">If accessing attachments in Outlook tasks: Tasks.ReadWrite</span></span>
* <span data-ttu-id="6a1f5-111">如果访问组帖子中的附件: Group. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="6a1f5-111">If accessing attachments in group posts: Group.ReadWrite.All</span></span>

<!--
* If accessing attachments in Group Events or Posts: Group.ReadWrite.All
-->

## <a name="http-request"></a><span data-ttu-id="6a1f5-112">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6a1f5-112">HTTP request</span></span>

<span data-ttu-id="6a1f5-113">用户的默认[日历](../resources/calendar.md)中的[事件](../resources/event.md)的附件。</span><span class="sxs-lookup"><span data-stu-id="6a1f5-113">Attachments for an [event](../resources/event.md) in the user's default [calendar](../resources/calendar.md).</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/events/{id}/attachments/{id}
DELETE /users/{id | userPrincipalName}/events/{id}/attachments/{id}

DELETE /me/calendar/events/{id}/attachments/{id}
DELETE /users/{id | userPrincipalName}/calendar/events/{id}/attachments/{id}
```

<span data-ttu-id="6a1f5-114">属于用户的指定[日历](../resources/calendar.md)中的[事件](../resources/event.md)的附件。</span><span class="sxs-lookup"><span data-stu-id="6a1f5-114">Attachments for an [event](../resources/event.md) in the specified [calendar](../resources/calendar.md) belonging to the user.</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/calendars/{id}/events/{id}/attachments/{id}
DELETE /users/{id | userPrincipalName}/calendars/{id}/events/{id}/attachments/{id}
```

<!-- Tried adding and getting group event with attachment, event exists but without attachment. Group event attachment not supported.
DELETE /groups/{id}/events/{id}/attachments/{id}
DELETE /groups/{id}/calendar/events/{id}/attachments/{id}
-->

<span data-ttu-id="6a1f5-115">属于用户的默认 [calendarGroup](../resources/calendargroup.md) 的 [日历](../resources/calendar.md) 中的 [事件](../resources/event.md) 附件。</span><span class="sxs-lookup"><span data-stu-id="6a1f5-115">Attachments for an [event](../resources/event.md) in a [calendar](../resources/calendar.md) belonging to the user's default [calendarGroup](../resources/calendargroup.md).</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/calendars/{id}/events/{id}/attachments/{id}
DELETE /users/{id | userPrincipalName}/calendars/{id}/events/{id}/attachments/{id}

DELETE /me/calendargroup/calendars/{id}/events/{id}/attachments/{id}
DELETE /users/{id | userPrincipalName}/calendargroup/calendars/{id}/events/{id}/attachments/{id}
```
<span data-ttu-id="6a1f5-116">属于用户的 [calendarGroup](../resources/calendargroup.md) 的 [日历](../resources/calendar.md) 中的 [事件](../resources/event.md) 附件。</span><span class="sxs-lookup"><span data-stu-id="6a1f5-116">Attachments for an [event](../resources/event.md) in a [calendar](../resources/calendar.md) belonging to a user's [calendarGroup](../resources/calendargroup.md).</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/calendargroups/{id}/calendars/{id}/events/{id}/attachments/{id}
DELETE /users/{id | userPrincipalName}/calendargroups/{id}/calendars/{id}/events/{id}/attachments/{id}

Attachments for a [message](../resources/message.md) in a user's mailbox.
<!-- { "blockType": "ignored" } -->

```http
DELETE /me/messages/{id}/attachments/{id}
DELETE /users/{id | userPrincipalName}/messages/{id}/attachments/{id}
```

<span data-ttu-id="6a1f5-117">用户邮箱的顶级 [mailFolder](../resources/mailfolder.md) 中包含的 [邮件](../resources/message.md) 附件。</span><span class="sxs-lookup"><span data-stu-id="6a1f5-117">Attachments for a [message](../resources/message.md) contained in a top level [mailFolder](../resources/mailfolder.md) in a user's mailbox.</span></span>
<!-- { "blockType": "ignored" } -->

```http
DELETE /me/mailFolders/{id}/messages/{id}/attachments/{id}
DELETE /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/attachments/{id}
```

<span data-ttu-id="6a1f5-p102">用户邮箱的 [mailFolder](../resources/mailfolder.md) 的子文件夹中包含的 [邮件](../resources/message.md) 附件。下面的示例显示了一个嵌套级别，但邮件可能位于子级的子级中，诸如此类。</span><span class="sxs-lookup"><span data-stu-id="6a1f5-p102">Attachments for a [message](../resources/message.md) contained in a child folder of a [mailFolder](../resources/mailfolder.md) in a user's mailbox.  The example below shows one level of nesting, but a message can be located in a child of a child and so on. </span></span><!-- { "blockType": "ignored" } -->

```http
DELETE /me/mailFolders/{id}/childFolders/{id}/.../messages/{id}/attachments/{id}
DELETE /users/{id | userPrincipalName}/mailFolders/{id}/childFolders/{id}/messages/{id}/attachments/{id}
```

<span data-ttu-id="6a1f5-120">[Outlook 任务](../resources/outlooktask.md)的附件。</span><span class="sxs-lookup"><span data-stu-id="6a1f5-120">Attachments for an [Outlook task](../resources/outlooktask.md).</span></span>
<!-- { "blockType": "ignored" } -->

```http
DELETE /me/outlook/tasks/{id}/attachments/{id}
DELETE /users/{id}/outlook/tasks/{id}/attachments/{id}
```

<span data-ttu-id="6a1f5-121">属于组的 [对话](../resources/conversation.md) 的 [线程](../resources/conversationthread.md) 中的 [帖子](../resources/post.md) 附件。</span><span class="sxs-lookup"><span data-stu-id="6a1f5-121">Attachments for a [post](../resources/post.md) in a [thread](../resources/conversationthread.md) belonging to a [conversation](../resources/conversation.md) of a group.</span></span>
<!-- { "blockType": "ignored" } -->

```http
DELETE /groups/{id}/threads/{id}/posts/{id}/attachments/{id}
DELETE /groups/{id}/conversations/{id}/threads/{id}/posts/{id}/attachments/{id}
```

## <a name="request-headers"></a><span data-ttu-id="6a1f5-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="6a1f5-122">Request headers</span></span>

| <span data-ttu-id="6a1f5-123">名称</span><span class="sxs-lookup"><span data-stu-id="6a1f5-123">Name</span></span>       | <span data-ttu-id="6a1f5-124">类型</span><span class="sxs-lookup"><span data-stu-id="6a1f5-124">Type</span></span> | <span data-ttu-id="6a1f5-125">说明</span><span class="sxs-lookup"><span data-stu-id="6a1f5-125">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="6a1f5-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="6a1f5-126">Authorization</span></span>  | <span data-ttu-id="6a1f5-127">string</span><span class="sxs-lookup"><span data-stu-id="6a1f5-127">string</span></span>  | <span data-ttu-id="6a1f5-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="6a1f5-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6a1f5-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="6a1f5-130">Request body</span></span>

<span data-ttu-id="6a1f5-131">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="6a1f5-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6a1f5-132">响应</span><span class="sxs-lookup"><span data-stu-id="6a1f5-132">Response</span></span>

<span data-ttu-id="6a1f5-p104">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="6a1f5-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6a1f5-135">示例</span><span class="sxs-lookup"><span data-stu-id="6a1f5-135">Example</span></span>

### <a name="request"></a><span data-ttu-id="6a1f5-136">请求</span><span class="sxs-lookup"><span data-stu-id="6a1f5-136">Request</span></span>

<span data-ttu-id="6a1f5-137">下面的示例展示了用于删除事件的附件的请求。</span><span class="sxs-lookup"><span data-stu-id="6a1f5-137">Here is an example of the request to delete an attachment on an event.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="6a1f5-138">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="6a1f5-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_attachment"
}-->

```http
DELETE https://graph.microsoft.com/beta/me/events/{id}/attachments/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="6a1f5-139">C#</span><span class="sxs-lookup"><span data-stu-id="6a1f5-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-attachment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="6a1f5-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6a1f5-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-attachment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="6a1f5-141">目标-C</span><span class="sxs-lookup"><span data-stu-id="6a1f5-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-attachment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="6a1f5-142">响应</span><span class="sxs-lookup"><span data-stu-id="6a1f5-142">Response</span></span>

<span data-ttu-id="6a1f5-143">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="6a1f5-143">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete attachment",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
