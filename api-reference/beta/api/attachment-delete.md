---
title: 删除附件
description: 从日历事件、 邮件、 Outlook 任务或公告中删除附件。
localization_priority: Normal
ms.openlocfilehash: c8af55d2237dd481e89b888d9bc025e6a1093695
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27824939"
---
# <a name="delete-attachment"></a><span data-ttu-id="f1760-103">删除附件</span><span class="sxs-lookup"><span data-stu-id="f1760-103">Delete attachment</span></span>

> <span data-ttu-id="f1760-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="f1760-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f1760-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="f1760-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f1760-106">从日历[事件](../resources/event.md)、[消息](../resources/message.md)、 [Outlook 任务](../resources/outlooktask.md)或[发布](../resources/post.md)删除附件。</span><span class="sxs-lookup"><span data-stu-id="f1760-106">Delete an attachment from a calendar [event](../resources/event.md), [message](../resources/message.md), [Outlook task](../resources/outlooktask.md), or [post](../resources/post.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="f1760-107">权限</span><span class="sxs-lookup"><span data-stu-id="f1760-107">Permissions</span></span>

<span data-ttu-id="f1760-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f1760-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

* <span data-ttu-id="f1760-110">如果访问邮件中的附件： Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f1760-110">If accessing attachments in messages: Mail.ReadWrite</span></span>
* <span data-ttu-id="f1760-111">如果访问事件中的附件： Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f1760-111">If accessing attachments in events: Calendars.ReadWrite</span></span>
* <span data-ttu-id="f1760-112">如果访问 Outlook 任务中的附件： Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f1760-112">If accessing attachments in Outlook tasks: Tasks.ReadWrite</span></span>
* <span data-ttu-id="f1760-113">如果访问组文章中的附件： Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f1760-113">If accessing attachments in group posts: Group.ReadWrite.All</span></span>

<!--
* If accessing attachments in Group Events or Posts: Group.ReadWrite.All
-->

## <a name="http-request"></a><span data-ttu-id="f1760-114">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f1760-114">HTTP request</span></span>

<span data-ttu-id="f1760-115">[事件](../resources/event.md)的附件。</span><span class="sxs-lookup"><span data-stu-id="f1760-115">Attachments for an [event](../resources/event.md).</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /me/events/{id}/attachments/{id}
DELETE /users/{id | userPrincipalName}/events/{id}/attachments/{id}
```

<!--
DELETE /groups/{id}/events/{id}/attachments/{id}
-->

<span data-ttu-id="f1760-116">用户邮箱中的 [邮件](../resources/message.md) 附件。</span><span class="sxs-lookup"><span data-stu-id="f1760-116">Attachments for a [message](../resources/message.md) in a user's mailbox.</span></span>
<!-- { "blockType": "ignored" } -->

```http
DELETE /me/messages/{id}/attachments/{id}
DELETE /users/{id | userPrincipalName}/messages/{id}/attachments/{id}
```

<span data-ttu-id="f1760-117">用户邮箱的顶级 [mailFolder](../resources/mailfolder.md) 中包含的 [邮件](../resources/message.md) 附件。</span><span class="sxs-lookup"><span data-stu-id="f1760-117">Attachments for a [message](../resources/message.md) contained in a top level [mailFolder](../resources/mailfolder.md) in a user's mailbox.</span></span>
<!-- { "blockType": "ignored" } -->

```http
DELETE /me/mailFolders/{id}/messages/{id}/attachments/{id}
DELETE /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/attachments/{id}
```

<span data-ttu-id="f1760-118">[邮件](../resources/message.md)的用户的邮箱中[mailFolder](../resources/mailfolder.md)子文件夹中包含的附件。</span><span class="sxs-lookup"><span data-stu-id="f1760-118">Attachments for a [message](../resources/message.md) contained in a child folder of a [mailFolder](../resources/mailfolder.md) in a user's mailbox.</span></span>  <span data-ttu-id="f1760-119">下面的示例演示一个级别的嵌套，但一条消息可以位于子级的子级，依此类推。</span><span class="sxs-lookup"><span data-stu-id="f1760-119">The example below shows one level of nesting, but a message can be located in a child of a child and so on.</span></span>
<!-- { "blockType": "ignored" } -->

```http
DELETE /me/mailFolders/{id}/childFolders/{id}/.../messages/{id}/attachments/{id}
DELETE /users/{id | userPrincipalName}/mailFolders/{id}/childFolders/{id}/messages/{id}/attachments/{id}
```

<span data-ttu-id="f1760-120">为[Outlook 任务](../resources/outlooktask.md)的附件。</span><span class="sxs-lookup"><span data-stu-id="f1760-120">Attachments for an [Outlook task](../resources/outlooktask.md).</span></span>
<!-- { "blockType": "ignored" } -->

```http
DELETE /me/outlook/tasks/<id>/attachments/{id}
DELETE /users/<id>/outlook/tasks/<id>/attachments/{id}
```

<span data-ttu-id="f1760-121">属于组的 [对话](../resources/conversation.md) 的 [线程](../resources/conversationthread.md) 中的 [帖子](../resources/post.md) 附件。</span><span class="sxs-lookup"><span data-stu-id="f1760-121">Attachments for a [post](../resources/post.md) in a [thread](../resources/conversationthread.md) belonging to a [conversation](../resources/conversation.md) of a group.</span></span>
<!-- { "blockType": "ignored" } -->

```http
DELETE /groups/{id}/threads/{id}/posts/{id}/attachments/{id}
DELETE /groups/{id}/conversations/{id}/threads/{id}/posts/{id}/attachments/{id}
```

## <a name="request-headers"></a><span data-ttu-id="f1760-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="f1760-122">Request headers</span></span>

| <span data-ttu-id="f1760-123">名称</span><span class="sxs-lookup"><span data-stu-id="f1760-123">Name</span></span>       | <span data-ttu-id="f1760-124">类型</span><span class="sxs-lookup"><span data-stu-id="f1760-124">Type</span></span> | <span data-ttu-id="f1760-125">说明</span><span class="sxs-lookup"><span data-stu-id="f1760-125">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="f1760-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="f1760-126">Authorization</span></span>  | <span data-ttu-id="f1760-127">string</span><span class="sxs-lookup"><span data-stu-id="f1760-127">string</span></span>  | <span data-ttu-id="f1760-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="f1760-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f1760-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="f1760-130">Request body</span></span>

<span data-ttu-id="f1760-131">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="f1760-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f1760-132">响应</span><span class="sxs-lookup"><span data-stu-id="f1760-132">Response</span></span>

<span data-ttu-id="f1760-p105">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="f1760-p105">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f1760-135">示例</span><span class="sxs-lookup"><span data-stu-id="f1760-135">Example</span></span>

### <a name="request"></a><span data-ttu-id="f1760-136">请求</span><span class="sxs-lookup"><span data-stu-id="f1760-136">Request</span></span>

<span data-ttu-id="f1760-137">下面的示例展示了用于删除事件的附件的请求。</span><span class="sxs-lookup"><span data-stu-id="f1760-137">Here is an example of the request to delete an attachment on an event.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_attachment"
}-->

```http
DELETE https://graph.microsoft.com/beta/me/events/{id}/attachments/{id}
```

### <a name="response"></a><span data-ttu-id="f1760-138">响应</span><span class="sxs-lookup"><span data-stu-id="f1760-138">Response</span></span>

<span data-ttu-id="f1760-139">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="f1760-139">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete attachment",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
