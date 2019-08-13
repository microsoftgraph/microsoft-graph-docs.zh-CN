---
title: 删除附件
description: 从日历事件、邮件、Outlook 任务或帖子中删除附件。
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ''
ms.openlocfilehash: 774043c030594ea60c80eb952acbae00e00c47c0
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36318528"
---
# <a name="delete-attachment"></a><span data-ttu-id="097bd-103">删除附件</span><span class="sxs-lookup"><span data-stu-id="097bd-103">Delete attachment</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="097bd-104">从日历[事件](../resources/event.md)、[邮件](../resources/message.md)、 [Outlook 任务](../resources/outlooktask.md)或[帖子](../resources/post.md)中删除附件。</span><span class="sxs-lookup"><span data-stu-id="097bd-104">Delete an attachment from a calendar [event](../resources/event.md), [message](../resources/message.md), [Outlook task](../resources/outlooktask.md), or [post](../resources/post.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="097bd-105">权限</span><span class="sxs-lookup"><span data-stu-id="097bd-105">Permissions</span></span>

<span data-ttu-id="097bd-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="097bd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

* <span data-ttu-id="097bd-108">如果访问邮件中的附件: Mail. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="097bd-108">If accessing attachments in messages: Mail.ReadWrite</span></span>
* <span data-ttu-id="097bd-109">如果访问事件中的附件: 日历. 读写</span><span class="sxs-lookup"><span data-stu-id="097bd-109">If accessing attachments in events: Calendars.ReadWrite</span></span>
* <span data-ttu-id="097bd-110">如果访问 Outlook 任务中的附件: Tasks. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="097bd-110">If accessing attachments in Outlook tasks: Tasks.ReadWrite</span></span>
* <span data-ttu-id="097bd-111">如果访问组帖子中的附件: Group. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="097bd-111">If accessing attachments in group posts: Group.ReadWrite.All</span></span>

<!--
* If accessing attachments in Group Events or Posts: Group.ReadWrite.All
-->

## <a name="http-request"></a><span data-ttu-id="097bd-112">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="097bd-112">HTTP request</span></span>

<span data-ttu-id="097bd-113">[事件](../resources/event.md)的附件。</span><span class="sxs-lookup"><span data-stu-id="097bd-113">Attachments for an [event](../resources/event.md).</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /me/events/{id}/attachments/{id}
DELETE /users/{id | userPrincipalName}/events/{id}/attachments/{id}
```

<!--
DELETE /groups/{id}/events/{id}/attachments/{id}
-->

<span data-ttu-id="097bd-114">用户邮箱中的 [邮件](../resources/message.md) 附件。</span><span class="sxs-lookup"><span data-stu-id="097bd-114">Attachments for a [message](../resources/message.md) in a user's mailbox.</span></span>
<!-- { "blockType": "ignored" } -->

```http
DELETE /me/messages/{id}/attachments/{id}
DELETE /users/{id | userPrincipalName}/messages/{id}/attachments/{id}
```

<span data-ttu-id="097bd-115">用户邮箱的顶级 [mailFolder](../resources/mailfolder.md) 中包含的 [邮件](../resources/message.md) 附件。</span><span class="sxs-lookup"><span data-stu-id="097bd-115">Attachments for a [message](../resources/message.md) contained in a top level [mailFolder](../resources/mailfolder.md) in a user's mailbox.</span></span>
<!-- { "blockType": "ignored" } -->

```http
DELETE /me/mailFolders/{id}/messages/{id}/attachments/{id}
DELETE /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/attachments/{id}
```

<span data-ttu-id="097bd-p102">用户邮箱的 [mailFolder](../resources/mailfolder.md) 的子文件夹中包含的 [邮件](../resources/message.md) 附件。下面的示例显示了一个嵌套级别，但邮件可能位于子级的子级中，诸如此类。</span><span class="sxs-lookup"><span data-stu-id="097bd-p102">Attachments for a [message](../resources/message.md) contained in a child folder of a [mailFolder](../resources/mailfolder.md) in a user's mailbox.  The example below shows one level of nesting, but a message can be located in a child of a child and so on. </span></span><!-- { "blockType": "ignored" } -->

```http
DELETE /me/mailFolders/{id}/childFolders/{id}/.../messages/{id}/attachments/{id}
DELETE /users/{id | userPrincipalName}/mailFolders/{id}/childFolders/{id}/messages/{id}/attachments/{id}
```

<span data-ttu-id="097bd-118">[Outlook 任务](../resources/outlooktask.md)的附件。</span><span class="sxs-lookup"><span data-stu-id="097bd-118">Attachments for an [Outlook task](../resources/outlooktask.md).</span></span>
<!-- { "blockType": "ignored" } -->

```http
DELETE /me/outlook/tasks/<id>/attachments/{id}
DELETE /users/<id>/outlook/tasks/<id>/attachments/{id}
```

<span data-ttu-id="097bd-119">属于组的 [对话](../resources/conversation.md) 的 [线程](../resources/conversationthread.md) 中的 [帖子](../resources/post.md) 附件。</span><span class="sxs-lookup"><span data-stu-id="097bd-119">Attachments for a [post](../resources/post.md) in a [thread](../resources/conversationthread.md) belonging to a [conversation](../resources/conversation.md) of a group.</span></span>
<!-- { "blockType": "ignored" } -->

```http
DELETE /groups/{id}/threads/{id}/posts/{id}/attachments/{id}
DELETE /groups/{id}/conversations/{id}/threads/{id}/posts/{id}/attachments/{id}
```

## <a name="request-headers"></a><span data-ttu-id="097bd-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="097bd-120">Request headers</span></span>

| <span data-ttu-id="097bd-121">名称</span><span class="sxs-lookup"><span data-stu-id="097bd-121">Name</span></span>       | <span data-ttu-id="097bd-122">类型</span><span class="sxs-lookup"><span data-stu-id="097bd-122">Type</span></span> | <span data-ttu-id="097bd-123">说明</span><span class="sxs-lookup"><span data-stu-id="097bd-123">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="097bd-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="097bd-124">Authorization</span></span>  | <span data-ttu-id="097bd-125">string</span><span class="sxs-lookup"><span data-stu-id="097bd-125">string</span></span>  | <span data-ttu-id="097bd-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="097bd-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="097bd-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="097bd-128">Request body</span></span>

<span data-ttu-id="097bd-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="097bd-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="097bd-130">响应</span><span class="sxs-lookup"><span data-stu-id="097bd-130">Response</span></span>

<span data-ttu-id="097bd-p104">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="097bd-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="097bd-133">示例</span><span class="sxs-lookup"><span data-stu-id="097bd-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="097bd-134">请求</span><span class="sxs-lookup"><span data-stu-id="097bd-134">Request</span></span>

<span data-ttu-id="097bd-135">下面的示例展示了用于删除事件的附件的请求。</span><span class="sxs-lookup"><span data-stu-id="097bd-135">Here is an example of the request to delete an attachment on an event.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="097bd-136">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="097bd-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_attachment"
}-->

```http
DELETE https://graph.microsoft.com/beta/me/events/{id}/attachments/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="097bd-137">C#</span><span class="sxs-lookup"><span data-stu-id="097bd-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-attachment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="097bd-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="097bd-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-attachment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="097bd-139">目标-C</span><span class="sxs-lookup"><span data-stu-id="097bd-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-attachment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="097bd-140">Java</span><span class="sxs-lookup"><span data-stu-id="097bd-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-attachment-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="097bd-141">响应</span><span class="sxs-lookup"><span data-stu-id="097bd-141">Response</span></span>

<span data-ttu-id="097bd-142">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="097bd-142">Here is an example of the response.</span></span>
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
