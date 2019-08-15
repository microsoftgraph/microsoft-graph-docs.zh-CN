---
title: 删除附件
description: 从日历事件、邮件、Outlook 任务或帖子中删除附件。
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ''
ms.openlocfilehash: 53a56b720ed1b1b2def64916f25831473cc79555
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/15/2019
ms.locfileid: "36408185"
---
# <a name="delete-attachment"></a><span data-ttu-id="d5049-103">删除附件</span><span class="sxs-lookup"><span data-stu-id="d5049-103">Delete attachment</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d5049-104">从日历[事件](../resources/event.md)、[邮件](../resources/message.md)、 [Outlook 任务](../resources/outlooktask.md)或[帖子](../resources/post.md)中删除附件。</span><span class="sxs-lookup"><span data-stu-id="d5049-104">Delete an attachment from a calendar [event](../resources/event.md), [message](../resources/message.md), [Outlook task](../resources/outlooktask.md), or [post](../resources/post.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="d5049-105">权限</span><span class="sxs-lookup"><span data-stu-id="d5049-105">Permissions</span></span>

<span data-ttu-id="d5049-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d5049-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

* <span data-ttu-id="d5049-108">如果访问邮件中的附件: Mail. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d5049-108">If accessing attachments in messages: Mail.ReadWrite</span></span>
* <span data-ttu-id="d5049-109">如果访问事件中的附件: 日历. 读写</span><span class="sxs-lookup"><span data-stu-id="d5049-109">If accessing attachments in events: Calendars.ReadWrite</span></span>
* <span data-ttu-id="d5049-110">如果访问 Outlook 任务中的附件: Tasks. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d5049-110">If accessing attachments in Outlook tasks: Tasks.ReadWrite</span></span>
* <span data-ttu-id="d5049-111">如果访问组帖子中的附件: Group. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="d5049-111">If accessing attachments in group posts: Group.ReadWrite.All</span></span>

<!--
* If accessing attachments in Group Events or Posts: Group.ReadWrite.All
-->

## <a name="http-request"></a><span data-ttu-id="d5049-112">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d5049-112">HTTP request</span></span>

<span data-ttu-id="d5049-113">[事件](../resources/event.md)的附件。</span><span class="sxs-lookup"><span data-stu-id="d5049-113">Attachments for an [event](../resources/event.md).</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /me/events/{id}/attachments/{id}
DELETE /users/{id | userPrincipalName}/events/{id}/attachments/{id}
```

<!--
DELETE /groups/{id}/events/{id}/attachments/{id}
-->

<span data-ttu-id="d5049-114">用户邮箱中的 [邮件](../resources/message.md) 附件。</span><span class="sxs-lookup"><span data-stu-id="d5049-114">Attachments for a [message](../resources/message.md) in a user's mailbox.</span></span>
<!-- { "blockType": "ignored" } -->

```http
DELETE /me/messages/{id}/attachments/{id}
DELETE /users/{id | userPrincipalName}/messages/{id}/attachments/{id}
```

<span data-ttu-id="d5049-115">用户邮箱的顶级 [mailFolder](../resources/mailfolder.md) 中包含的 [邮件](../resources/message.md) 附件。</span><span class="sxs-lookup"><span data-stu-id="d5049-115">Attachments for a [message](../resources/message.md) contained in a top level [mailFolder](../resources/mailfolder.md) in a user's mailbox.</span></span>
<!-- { "blockType": "ignored" } -->

```http
DELETE /me/mailFolders/{id}/messages/{id}/attachments/{id}
DELETE /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/attachments/{id}
```

<span data-ttu-id="d5049-p102">用户邮箱的 [mailFolder](../resources/mailfolder.md) 的子文件夹中包含的 [邮件](../resources/message.md) 附件。下面的示例显示了一个嵌套级别，但邮件可能位于子级的子级中，诸如此类。</span><span class="sxs-lookup"><span data-stu-id="d5049-p102">Attachments for a [message](../resources/message.md) contained in a child folder of a [mailFolder](../resources/mailfolder.md) in a user's mailbox.  The example below shows one level of nesting, but a message can be located in a child of a child and so on. </span></span><!-- { "blockType": "ignored" } -->

```http
DELETE /me/mailFolders/{id}/childFolders/{id}/.../messages/{id}/attachments/{id}
DELETE /users/{id | userPrincipalName}/mailFolders/{id}/childFolders/{id}/messages/{id}/attachments/{id}
```

<span data-ttu-id="d5049-118">[Outlook 任务](../resources/outlooktask.md)的附件。</span><span class="sxs-lookup"><span data-stu-id="d5049-118">Attachments for an [Outlook task](../resources/outlooktask.md).</span></span>
<!-- { "blockType": "ignored" } -->

```http
DELETE /me/outlook/tasks/{id}/attachments/{id}
DELETE /users/{id}/outlook/tasks/{id}/attachments/{id}
```

<span data-ttu-id="d5049-119">属于组的 [对话](../resources/conversation.md) 的 [线程](../resources/conversationthread.md) 中的 [帖子](../resources/post.md) 附件。</span><span class="sxs-lookup"><span data-stu-id="d5049-119">Attachments for a [post](../resources/post.md) in a [thread](../resources/conversationthread.md) belonging to a [conversation](../resources/conversation.md) of a group.</span></span>
<!-- { "blockType": "ignored" } -->

```http
DELETE /groups/{id}/threads/{id}/posts/{id}/attachments/{id}
DELETE /groups/{id}/conversations/{id}/threads/{id}/posts/{id}/attachments/{id}
```

## <a name="request-headers"></a><span data-ttu-id="d5049-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="d5049-120">Request headers</span></span>

| <span data-ttu-id="d5049-121">名称</span><span class="sxs-lookup"><span data-stu-id="d5049-121">Name</span></span>       | <span data-ttu-id="d5049-122">类型</span><span class="sxs-lookup"><span data-stu-id="d5049-122">Type</span></span> | <span data-ttu-id="d5049-123">说明</span><span class="sxs-lookup"><span data-stu-id="d5049-123">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="d5049-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="d5049-124">Authorization</span></span>  | <span data-ttu-id="d5049-125">string</span><span class="sxs-lookup"><span data-stu-id="d5049-125">string</span></span>  | <span data-ttu-id="d5049-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="d5049-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d5049-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="d5049-128">Request body</span></span>

<span data-ttu-id="d5049-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="d5049-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d5049-130">响应</span><span class="sxs-lookup"><span data-stu-id="d5049-130">Response</span></span>

<span data-ttu-id="d5049-p104">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="d5049-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d5049-133">示例</span><span class="sxs-lookup"><span data-stu-id="d5049-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="d5049-134">请求</span><span class="sxs-lookup"><span data-stu-id="d5049-134">Request</span></span>

<span data-ttu-id="d5049-135">下面的示例展示了用于删除事件的附件的请求。</span><span class="sxs-lookup"><span data-stu-id="d5049-135">Here is an example of the request to delete an attachment on an event.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="d5049-136">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="d5049-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_attachment"
}-->

```http
DELETE https://graph.microsoft.com/beta/me/events/{id}/attachments/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="d5049-137">C#</span><span class="sxs-lookup"><span data-stu-id="d5049-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-attachment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d5049-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d5049-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-attachment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="d5049-139">目标-C</span><span class="sxs-lookup"><span data-stu-id="d5049-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-attachment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="d5049-140">响应</span><span class="sxs-lookup"><span data-stu-id="d5049-140">Response</span></span>

<span data-ttu-id="d5049-141">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="d5049-141">Here is an example of the response.</span></span>
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
