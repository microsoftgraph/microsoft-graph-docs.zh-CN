---
title: 删除附件
description: 从日历事件、电子邮件或组帖子中删除附件。
localization_priority: Normal
author: abheek-das
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: f97441b7b258c16ae38c46019cc070810c9ba1ad
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50137053"
---
# <a name="delete-attachment"></a><span data-ttu-id="c8786-103">删除附件</span><span class="sxs-lookup"><span data-stu-id="c8786-103">Delete attachment</span></span>

<span data-ttu-id="c8786-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c8786-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="c8786-105">从用户日历事件、邮件或组帖子中删除附件。</span><span class="sxs-lookup"><span data-stu-id="c8786-105">Delete an attachment from a user calendar event, mail message, or group post.</span></span>
## <a name="permissions"></a><span data-ttu-id="c8786-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="c8786-106">Permissions</span></span>

<span data-ttu-id="c8786-107">根据 **附件所附加到** 的资源 **(** 事件、邮件 **、outlookTask** 或 post) 以及请求的权限类型 (委派或应用程序) ，下表中指定的权限是调用此 API 所需的最小特权。</span><span class="sxs-lookup"><span data-stu-id="c8786-107">Depending on the resource (**event**, **message**, **outlookTask**, or **post**) that the attachment is attached to and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="c8786-108">若要了解其他信息， [在](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) 特权权限之前要特别小心，在"权限" [中搜索](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c8786-108">To learn more, including [taking caution](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) before choosing more privileged permissions, search for the following permissions in [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="c8786-109">支持的资源</span><span class="sxs-lookup"><span data-stu-id="c8786-109">Supported resource</span></span> | <span data-ttu-id="c8786-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c8786-110">Delegated (work or school account)</span></span> | <span data-ttu-id="c8786-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c8786-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c8786-112">应用程序</span><span class="sxs-lookup"><span data-stu-id="c8786-112">Application</span></span> |
|:-----|:-----|:-----|:-----|
| [<span data-ttu-id="c8786-113">事件</span><span class="sxs-lookup"><span data-stu-id="c8786-113">event</span></span>](../resources/event.md) | <span data-ttu-id="c8786-114">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c8786-114">Calendars.ReadWrite</span></span> | <span data-ttu-id="c8786-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c8786-115">Calendars.ReadWrite</span></span> | <span data-ttu-id="c8786-116">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c8786-116">Calendars.ReadWrite</span></span> |
| [<span data-ttu-id="c8786-117">邮件</span><span class="sxs-lookup"><span data-stu-id="c8786-117">message</span></span>](../resources/message.md) | <span data-ttu-id="c8786-118">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c8786-118">Mail.ReadWrite</span></span> | <span data-ttu-id="c8786-119">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c8786-119">Mail.ReadWrite</span></span> | <span data-ttu-id="c8786-120">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c8786-120">Mail.ReadWrite</span></span> |
| [<span data-ttu-id="c8786-121">帖子</span><span class="sxs-lookup"><span data-stu-id="c8786-121">post</span></span>](../resources/post.md) | <span data-ttu-id="c8786-122">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c8786-122">Group.ReadWrite.All</span></span> | <span data-ttu-id="c8786-123">不支持</span><span class="sxs-lookup"><span data-stu-id="c8786-123">Not supported</span></span> | <span data-ttu-id="c8786-124">不支持</span><span class="sxs-lookup"><span data-stu-id="c8786-124">Not supported</span></span> |


<!--
* If accessing attachments in Group Events or Posts: Group.ReadWrite.All.
-->

## <a name="http-request"></a><span data-ttu-id="c8786-125">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c8786-125">HTTP request</span></span>
<span data-ttu-id="c8786-126">用户的默认[日历](../resources/calendar.md)中的[事件](../resources/event.md)附件。</span><span class="sxs-lookup"><span data-stu-id="c8786-126">Attachments for an [event](../resources/event.md) in the user's default [calendar](../resources/calendar.md).</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/events/{id}/attachments/{id}
DELETE /users/{id | userPrincipalName}/events/{id}/attachments/{id}

DELETE /me/calendar/events/{id}/attachments/{id}
DELETE /users/{id | userPrincipalName}/calendar/events/{id}/attachments/{id}
```

<span data-ttu-id="c8786-127">属于[用户的指定](../resources/event.md)[日历中的](../resources/calendar.md)事件的附件。</span><span class="sxs-lookup"><span data-stu-id="c8786-127">Attachments for an [event](../resources/event.md) in the specified [calendar](../resources/calendar.md) belonging to the user.</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/calendars/{id}/events/{id}/attachments/{id}
DELETE /users/{id | userPrincipalName}/calendars/{id}/events/{id}/attachments/{id}
```

<!-- Tried adding and getting group event with attachment, event exists but without attachment. Assume group event attachment not supported.
DELETE /groups/{id}/events/{id}/attachments/{id}
DELETE /groups/{id}/calendar/events/{id}/attachments/{id}
-->

<span data-ttu-id="c8786-128">属于用户的默认 [calendarGroup](../resources/calendargroup.md) 的 [日历](../resources/calendar.md) 中的 [事件](../resources/event.md) 附件。</span><span class="sxs-lookup"><span data-stu-id="c8786-128">Attachments for an [event](../resources/event.md) in a [calendar](../resources/calendar.md) belonging to the user's default [calendarGroup](../resources/calendargroup.md).</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/calendars/{id}/events/{id}/attachments/{id}
DELETE /users/{id | userPrincipalName}/calendars/{id}/events/{id}/attachments/{id}

DELETE /me/calendargroup/calendars/{id}/events/{id}/attachments/{id}
DELETE /users/{id | userPrincipalName}/calendargroup/calendars/{id}/events/{id}/attachments/{id}
```
<span data-ttu-id="c8786-129">属于用户的 [calendarGroup](../resources/calendargroup.md) 的 [日历](../resources/calendar.md) 中的 [事件](../resources/event.md) 附件。</span><span class="sxs-lookup"><span data-stu-id="c8786-129">Attachments for an [event](../resources/event.md) in a [calendar](../resources/calendar.md) belonging to a user's [calendarGroup](../resources/calendargroup.md).</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/calendargroups/{id}/calendars/{id}/events/{id}/attachments/{id}
DELETE /users/{id | userPrincipalName}/calendargroups/{id}/calendars/{id}/events/{id}/attachments/{id}
```
<span data-ttu-id="c8786-130">用户邮箱中的 [邮件](../resources/message.md) 附件。</span><span class="sxs-lookup"><span data-stu-id="c8786-130">Attachments for a [message](../resources/message.md) in a user's mailbox.</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/messages/{id}/attachments/{id}
DELETE /users/{id | userPrincipalName}/messages/{id}/attachments/{id}
```
<span data-ttu-id="c8786-131">用户邮箱的顶级 [mailFolder](../resources/mailfolder.md) 中包含的 [邮件](../resources/message.md) 附件。</span><span class="sxs-lookup"><span data-stu-id="c8786-131">Attachments for a [message](../resources/message.md) contained in a top level [mailFolder](../resources/mailfolder.md) in a user's mailbox.</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/mailFolders/{id}/messages/{id}/attachments/{id}
DELETE /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/attachments/{id}
```
<span data-ttu-id="c8786-p102">用户邮箱的 [mailFolder](../resources/mailfolder.md) 的子文件夹中包含的 [邮件](../resources/message.md) 附件。下面的示例显示了一个嵌套级别，但邮件可能位于子级的子级中，诸如此类。 </span><span class="sxs-lookup"><span data-stu-id="c8786-p102">Attachments for a [message](../resources/message.md) contained in a child folder of a [mailFolder](../resources/mailfolder.md) in a user's mailbox.  The example below shows one level of nesting, but a message can be located in a child of a child and so on. </span></span><!-- { "blockType": "ignored" } -->
```http
DELETE /me/mailFolders/{id}/childFolders/{id}/.../messages/{id}/attachments/{id}
DELETE /users/{id | userPrincipalName}/mailFolders/{id}/childFolders/{id}/messages/{id}/attachments/{id}
```
<span data-ttu-id="c8786-134">属于组的 [对话](../resources/conversation.md) 的 [线程](../resources/conversationthread.md) 中的 [帖子](../resources/post.md) 附件。</span><span class="sxs-lookup"><span data-stu-id="c8786-134">Attachments for a [post](../resources/post.md) in a [thread](../resources/conversationthread.md) belonging to a [conversation](../resources/conversation.md) of a group.</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}/threads/{id}/posts/{id}/attachments/{id}
DELETE /groups/{id}/conversations/{id}/threads/{id}/posts/{id}/attachments/{id}
```
## <a name="request-headers"></a><span data-ttu-id="c8786-135">请求标头</span><span class="sxs-lookup"><span data-stu-id="c8786-135">Request headers</span></span>
| <span data-ttu-id="c8786-136">名称</span><span class="sxs-lookup"><span data-stu-id="c8786-136">Name</span></span>       | <span data-ttu-id="c8786-137">类型</span><span class="sxs-lookup"><span data-stu-id="c8786-137">Type</span></span> | <span data-ttu-id="c8786-138">说明</span><span class="sxs-lookup"><span data-stu-id="c8786-138">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="c8786-139">Authorization</span><span class="sxs-lookup"><span data-stu-id="c8786-139">Authorization</span></span>  | <span data-ttu-id="c8786-140">string</span><span class="sxs-lookup"><span data-stu-id="c8786-140">string</span></span>  | <span data-ttu-id="c8786-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="c8786-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c8786-143">请求正文</span><span class="sxs-lookup"><span data-stu-id="c8786-143">Request body</span></span>
<span data-ttu-id="c8786-144">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="c8786-144">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c8786-145">响应</span><span class="sxs-lookup"><span data-stu-id="c8786-145">Response</span></span>

<span data-ttu-id="c8786-p104">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="c8786-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c8786-148">示例</span><span class="sxs-lookup"><span data-stu-id="c8786-148">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c8786-149">请求</span><span class="sxs-lookup"><span data-stu-id="c8786-149">Request</span></span>
<span data-ttu-id="c8786-150">下面的示例展示了用于删除事件的附件的请求。</span><span class="sxs-lookup"><span data-stu-id="c8786-150">Here is an example of the request to delete an attachment on an event.</span></span>

# <a name="http"></a>[<span data-ttu-id="c8786-151">HTTP</span><span class="sxs-lookup"><span data-stu-id="c8786-151">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_attachment"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/me/events/{id}/attachments/{id}
```
# <a name="c"></a>[<span data-ttu-id="c8786-152">C#</span><span class="sxs-lookup"><span data-stu-id="c8786-152">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-attachment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c8786-153">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c8786-153">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-attachment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c8786-154">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c8786-154">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-attachment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c8786-155">Java</span><span class="sxs-lookup"><span data-stu-id="c8786-155">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-attachment-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="c8786-156">响应</span><span class="sxs-lookup"><span data-stu-id="c8786-156">Response</span></span>
<span data-ttu-id="c8786-157">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="c8786-157">Here is an example of the response.</span></span>
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
  "tocPath": "",
  "suppressions": [
  ]
}-->

