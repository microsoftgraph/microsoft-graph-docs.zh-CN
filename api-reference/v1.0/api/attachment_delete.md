# <a name="delete-attachment"></a><span data-ttu-id="a1262-101">删除附件</span><span class="sxs-lookup"><span data-stu-id="a1262-101">Delete attachment</span></span>

<span data-ttu-id="a1262-102">从日历事件、电子邮件或组帖子中删除附件。</span><span class="sxs-lookup"><span data-stu-id="a1262-102">Delete an attachment from a calendar event, mail message, or group post.</span></span>
## <a name="permissions"></a><span data-ttu-id="a1262-103">权限</span><span class="sxs-lookup"><span data-stu-id="a1262-103">Permissions</span></span>
<span data-ttu-id="a1262-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="a1262-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

* <span data-ttu-id="a1262-106">如果访问邮件中的附件：Mail.ReadWrite。</span><span class="sxs-lookup"><span data-stu-id="a1262-106">If accessing attachments in Messages: Mail.ReadWrite.</span></span>
* <span data-ttu-id="a1262-107">如果访问事件中的附件：Calendars.ReadWrite。</span><span class="sxs-lookup"><span data-stu-id="a1262-107">If accessing attachments in Events: Calendars.ReadWrite.</span></span>
* <span data-ttu-id="a1262-108">如果访问组文章中的附件：Group.ReadWrite.All。</span><span class="sxs-lookup"><span data-stu-id="a1262-108">If accessing attachments in group posts: Group.ReadWrite.All.</span></span>

<!--
* If accessing attachments in Group Events or Posts: Group.ReadWrite.All.
-->

## <a name="http-request"></a><span data-ttu-id="a1262-109">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a1262-109">HTTP request</span></span>
<span data-ttu-id="a1262-110">用户或组的默认 [日历](../resources/calendar.md) 中的 [事件](../resources/event.md) 附件。</span><span class="sxs-lookup"><span data-stu-id="a1262-110">Attachments for an [event](../resources/event.md) in the user's or group's default [calendar](../resources/calendar.md).</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/events/{id}/attachments/{id}
DELETE /users/{id | userPrincipalName}/events/{id}/attachments/{id}

DELETE /me/calendar/{id}/events/{id}/attachments/{id}
DELETE /users/{id | userPrincipalName}/calendar/events/{id}/attachments/{id}
```

<!--
DELETE /groups/{id}/events/{id}/attachments/{id}
DELETE /groups/{id}/calendar/events/{id}/attachments/{id}
-->

<span data-ttu-id="a1262-111">属于用户的默认 [calendarGroup](../resources/calendargroup.md) 的 [日历](../resources/calendar.md) 中的 [事件](../resources/event.md) 附件。</span><span class="sxs-lookup"><span data-stu-id="a1262-111">Attachments for an [event](../resources/event.md) in a [calendar](../resources/calendar.md) belonging to the user's default [calendarGroup](../resources/calendargroup.md).</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/calendars/{id}/events/{id}/attachments/{id}
DELETE /users/{id | userPrincipalName}/calendars/{id}/events/{id}/attachments/{id}

DELETE /me/calendargroup/calendars/{id}/events/{id}/attachments/{id}
DELETE /users/{id | userPrincipalName}/calendargroup/calendars/{id}/events/{id}/attachments/{id}
```
<span data-ttu-id="a1262-112">属于用户的 [calendarGroup](../resources/calendargroup.md) 的 [日历](../resources/calendar.md) 中的 [事件](../resources/event.md) 附件。</span><span class="sxs-lookup"><span data-stu-id="a1262-112">Attachments for an [event](../resources/event.md) in a [calendar](../resources/calendar.md) belonging to a user's [calendarGroup](../resources/calendargroup.md).</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/calendargroups/{id}/calendars/{id}/events/{id}/attachments/{id}
DELETE /users/{id | userPrincipalName}/calendargroups/{id}/calendars/{id}/events/{id}/attachments/{id}
```
<span data-ttu-id="a1262-113">用户邮箱中的 [邮件](../resources/message.md) 附件。</span><span class="sxs-lookup"><span data-stu-id="a1262-113">Attachments for a [message](../resources/message.md) in a user's mailbox.</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/messages/{id}/attachments/{id}
DELETE /users/{id | userPrincipalName}/messages/{id}/attachments/{id}
```
<span data-ttu-id="a1262-114">用户邮箱的顶级 [mailFolder](../resources/mailfolder.md) 中包含的 [邮件](../resources/message.md)附件。</span><span class="sxs-lookup"><span data-stu-id="a1262-114">Attachments for a [message](../resources/message.md) contained in a top level [mailFolder](../resources/mailfolder.md) in a user's mailbox.</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/mailFolders/{id}/messages/{id}/attachments/{id}
DELETE /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/attachments/{id}
```
<span data-ttu-id="a1262-115">用户邮箱的子文件夹 [mailFolder](../resources/mailfolder.md) 中包含的 [邮件](../resources/message.md)附件。</span><span class="sxs-lookup"><span data-stu-id="a1262-115">Attachments for a [message](../resources/message.md) contained in a top level [mailFolder](../resources/mailfolder.md) in a user's mailbox.</span></span>  <span data-ttu-id="a1262-116">下面的示例显示了一个嵌套级别，但联系人可能位于子级的子级中，诸如此类。</span><span class="sxs-lookup"><span data-stu-id="a1262-116">A contact contained in a child folder of a contactFolder. The example below shows one level of nesting, but a contact can be located in a child of a child and so on.</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/mailFolders/{id}/childFolders/{id}/.../messages/{id}/attachments/{id}
DELETE /users/{id | userPrincipalName}/mailFolders/{id}/childFolders/{id}/messages/{id}/attachments/{id}
```
<span data-ttu-id="a1262-117">属于组的 [对话](../resources/conversation.md)的 [线程](../resources/conversationthread.md)中的 [帖子](../resources/post.md)附件。</span><span class="sxs-lookup"><span data-stu-id="a1262-117">Attachments for a [post](../resources/post.md) in a [thread](../resources/conversationthread.md) belonging to a [conversation](../resources/conversation.md) of a group.</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}/threads/{id}/posts/{id}/attachments/{id}
DELETE /groups/{id}/conversations/{id}/threads/{id}/posts/{id}/attachments/{id}
```
## <a name="request-headers"></a><span data-ttu-id="a1262-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="a1262-118">Request headers</span></span>
| <span data-ttu-id="a1262-119">名称</span><span class="sxs-lookup"><span data-stu-id="a1262-119">Name</span></span>       | <span data-ttu-id="a1262-120">类型</span><span class="sxs-lookup"><span data-stu-id="a1262-120">Type</span></span> | <span data-ttu-id="a1262-121">说明</span><span class="sxs-lookup"><span data-stu-id="a1262-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="a1262-122">授权</span><span class="sxs-lookup"><span data-stu-id="a1262-122">Authorization</span></span>  | <span data-ttu-id="a1262-123">字符串</span><span class="sxs-lookup"><span data-stu-id="a1262-123">string</span></span>  | <span data-ttu-id="a1262-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="a1262-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a1262-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="a1262-126">Request body</span></span>
<span data-ttu-id="a1262-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="a1262-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a1262-128">响应</span><span class="sxs-lookup"><span data-stu-id="a1262-128">Response</span></span>

<span data-ttu-id="a1262-p104">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="a1262-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a1262-131">示例</span><span class="sxs-lookup"><span data-stu-id="a1262-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a1262-132">请求</span><span class="sxs-lookup"><span data-stu-id="a1262-132">Request</span></span>
<span data-ttu-id="a1262-133">下面的示例展示了用于删除事件的附件的请求。</span><span class="sxs-lookup"><span data-stu-id="a1262-133">Here is an example of the request to delete an attachment on an event.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_attachment"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/me/events/{id}/attachments/{id}
```
##### <a name="response"></a><span data-ttu-id="a1262-134">响应</span><span class="sxs-lookup"><span data-stu-id="a1262-134">Response</span></span>
<span data-ttu-id="a1262-135">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="a1262-135">Here is an example of the response.</span></span>
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
