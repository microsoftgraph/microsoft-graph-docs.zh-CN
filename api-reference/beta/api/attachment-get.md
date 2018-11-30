---
title: Get attachment
description: '读取的属性和附件，附加到事件的关系 '
ms.openlocfilehash: a432e4f3fb98062a701e4c6e7b177145faa65e1e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27043031"
---
# <a name="get-attachment"></a><span data-ttu-id="e690c-103">Get attachment</span><span class="sxs-lookup"><span data-stu-id="e690c-103">Get attachment</span></span>

> <span data-ttu-id="e690c-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="e690c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e690c-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="e690c-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e690c-106">读取的属性和附件，附加到[事件](../resources/event.md)、[消息](../resources/message.md)、 [Outlook 任务](../resources/outlooktask.md)或[发布](../resources/post.md)的关系。</span><span class="sxs-lookup"><span data-stu-id="e690c-106">Read the properties and relationships of an attachment, attached to an [event](../resources/event.md), [message](../resources/message.md), [Outlook task](../resources/outlooktask.md), or [post](../resources/post.md).</span></span> 

<span data-ttu-id="e690c-107">附件可以是下列类型之一：</span><span class="sxs-lookup"><span data-stu-id="e690c-107">An attachment can be one of the following types:</span></span>

* <span data-ttu-id="e690c-108">文件（[fileAttachment](../resources/fileattachment.md) 资源）。</span><span class="sxs-lookup"><span data-stu-id="e690c-108">A file ([fileAttachment](../resources/fileattachment.md) resource).</span></span>
* <span data-ttu-id="e690c-p102">项（由 [itemAttachment](../resources/itemattachment.md) 资源表示的联系人、事件或邮件）。可以使用 `$expand` 来进一步获取该项的属性。请参阅以下[示例](#request-2)。</span><span class="sxs-lookup"><span data-stu-id="e690c-p102">An item (contact, event or message, represented by an [itemAttachment](../resources/itemattachment.md) resource). You can use `$expand` to further get the properties of that item. See an [example](#request-2) below.</span></span>
* <span data-ttu-id="e690c-112">文件链接（[referenceAttachment](../resources/referenceattachment.md) 资源）。</span><span class="sxs-lookup"><span data-stu-id="e690c-112">A link to a file ([referenceAttachment](../resources/referenceattachment.md) resource).</span></span>

<span data-ttu-id="e690c-113">所有这些类型的 attachment 资源均派生自 [attachment](../resources/attachment.md) 资源。</span><span class="sxs-lookup"><span data-stu-id="e690c-113">All these types of attachment resources are derived from the [attachment](../resources/attachment.md) resource.</span></span> 

## <a name="permissions"></a><span data-ttu-id="e690c-114">权限</span><span class="sxs-lookup"><span data-stu-id="e690c-114">Permissions</span></span>
<span data-ttu-id="e690c-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e690c-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

* <span data-ttu-id="e690c-117">如果访问邮件中的附件： Mail.Read</span><span class="sxs-lookup"><span data-stu-id="e690c-117">If accessing attachments in messages: Mail.Read</span></span>
* <span data-ttu-id="e690c-118">如果访问事件中的附件： Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="e690c-118">If accessing attachments in events: Calendars.Read</span></span>
* <span data-ttu-id="e690c-119">如果访问 Outlook 任务中的附件： Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="e690c-119">If accessing attachments in Outlook tasks: Tasks.Read</span></span>
* <span data-ttu-id="e690c-120">如果访问组文章中的附件： Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="e690c-120">If accessing attachments in group posts: Group.Read.All</span></span>
<!--
* If accessing attachments in group events or posts: Group.Read.All
-->

## <a name="http-request"></a><span data-ttu-id="e690c-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e690c-121">HTTP request</span></span>
<span data-ttu-id="e690c-122">[事件](../resources/event.md)在用户的默认[日历](../resources/calendar.md)中的附件。</span><span class="sxs-lookup"><span data-stu-id="e690c-122">Attachments for an [event](../resources/event.md) in the user's default [calendar](../resources/calendar.md).</span></span>

<!--
Attachments for an [event](../resources/event.md) in the user's or group's default [calendar](../resources/calendar.md).
-->
<!-- { "blockType": "ignored" } -->
```http
GET /me/events/{id}/attachments/{id}
GET /users/{id | userPrincipalName}/events/{id}/attachments/{id}

GET /me/calendar/{id}/events/{id}/attachments/{id}
GET /users/{id | userPrincipalName}/calendar/events/{id}/attachments/{id}
```

<!--
GET /groups/{id}/events/{id}/attachments/{id}
GET /groups/{id}/calendar/events/{id}/attachments/{id}
-->

<span data-ttu-id="e690c-123">属于用户的默认 [calendarGroup](../resources/calendargroup.md) 的 [日历](../resources/calendar.md) 中的 [事件](../resources/event.md) 附件。</span><span class="sxs-lookup"><span data-stu-id="e690c-123">Attachments for an [event](../resources/event.md) in a [calendar](../resources/calendar.md) belonging to the user's default [calendarGroup](../resources/calendargroup.md).</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/calendars/{id}/events/{id}/attachments/{id}
GET /users/{id | userPrincipalName}/calendars/{id}/events/{id}/attachments/{id}

GET /me/calendargroup/calendars/{id}/events/{id}/attachments/{id}
GET /users/{id | userPrincipalName}/calendargroup/calendars/{id}/events/{id}/attachments/{id}
```
<span data-ttu-id="e690c-124">属于用户的 [calendarGroup](../resources/calendargroup.md) 的 [日历](../resources/calendar.md) 中的 [事件](../resources/event.md) 附件。</span><span class="sxs-lookup"><span data-stu-id="e690c-124">Attachments for an [event](../resources/event.md) in a [calendar](../resources/calendar.md) belonging to a user's [calendarGroup](../resources/calendargroup.md).</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/calendargroups/{id}/calendars/{id}/events/{id}/attachments/{id}
GET /users/{id | userPrincipalName}/calendargroups/{id}/calendars/{id}/events/{id}/attachments/{id}
```
<span data-ttu-id="e690c-125">用户邮箱中的 [邮件](../resources/message.md) 附件。</span><span class="sxs-lookup"><span data-stu-id="e690c-125">Attachments for a [message](../resources/message.md) in a user's mailbox.</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/messages/{id}/attachments/{id}
GET /users/{id | userPrincipalName}/messages/{id}/attachments/{id}
```
<span data-ttu-id="e690c-126">用户邮箱的顶级 [mailFolder](../resources/mailfolder.md) 中包含的 [邮件](../resources/message.md) 附件。</span><span class="sxs-lookup"><span data-stu-id="e690c-126">Attachments for a [message](../resources/message.md) contained in a top level [mailFolder](../resources/mailfolder.md) in a user's mailbox.</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/{id}/messages/{id}/attachments/{id}
GET /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/attachments/{id}
```
<span data-ttu-id="e690c-127">[邮件](../resources/message.md)的用户的邮箱中[mailFolder](../resources/mailfolder.md)子文件夹中包含的附件。</span><span class="sxs-lookup"><span data-stu-id="e690c-127">Attachments for a [message](../resources/message.md) contained in a child folder of a [mailFolder](../resources/mailfolder.md) in a user's mailbox.</span></span>  <span data-ttu-id="e690c-128">下面的示例演示一个级别的嵌套，但一条消息可以位于子级的子级，依此类推。</span><span class="sxs-lookup"><span data-stu-id="e690c-128">The example below shows one level of nesting, but a message can be located in a child of a child and so on.</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/{id}/childFolders/{id}/.../messages/{id}/attachments/{id}
GET /users/{id | userPrincipalName}/mailFolders/{id}/childFolders/{id}/messages/{id}/attachments/{id}
```

<span data-ttu-id="e690c-129">为[Outlook 任务](../resources/outlooktask.md)在用户的邮箱，或指定的任务文件夹或任务组中的附件。</span><span class="sxs-lookup"><span data-stu-id="e690c-129">Attachments for an [Outlook task](../resources/outlooktask.md) in the user's mailbox, or in a specified task folder or task group.</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/outlook/tasks/<id>/attachments/{id}
GET /users/<id>/outlook/tasks/<id>/attachments/{id}

GET /me/outlook/taskFolders/<id>/tasks/<id>/attachments/{id}
GET /users/<id>/outlook/taskFolders/<id>/tasks/<id>/attachments/{id}

GET /me/outlook/taskGroups/<id>/taskFolders/<id>/tasks/<id>/attachments/{id}
GET /users/<id>/outlook/taskGroups/<id>/taskFolders/<id>/tasks/<id>/attachments/{id}
```

<span data-ttu-id="e690c-130">属于组的 [对话](../resources/conversation.md) 的 [线程](../resources/conversationthread.md) 中的 [帖子](../resources/post.md) 附件。</span><span class="sxs-lookup"><span data-stu-id="e690c-130">Attachments for a [post](../resources/post.md) in a [thread](../resources/conversationthread.md) belonging to a [conversation](../resources/conversation.md) of a group.</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/threads/{id}/posts/{id}/attachments/{id}
GET /groups/{id}/conversations/{id}/threads/{id}/posts/{id}/attachments/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="e690c-131">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="e690c-131">Optional query parameters</span></span>
<span data-ttu-id="e690c-132">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="e690c-132">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="e690c-133">请求标头</span><span class="sxs-lookup"><span data-stu-id="e690c-133">Request headers</span></span>
| <span data-ttu-id="e690c-134">名称</span><span class="sxs-lookup"><span data-stu-id="e690c-134">Name</span></span>       | <span data-ttu-id="e690c-135">类型</span><span class="sxs-lookup"><span data-stu-id="e690c-135">Type</span></span> | <span data-ttu-id="e690c-136">说明</span><span class="sxs-lookup"><span data-stu-id="e690c-136">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="e690c-137">Authorization</span><span class="sxs-lookup"><span data-stu-id="e690c-137">Authorization</span></span>  | <span data-ttu-id="e690c-138">string</span><span class="sxs-lookup"><span data-stu-id="e690c-138">string</span></span>  | <span data-ttu-id="e690c-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="e690c-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e690c-141">请求正文</span><span class="sxs-lookup"><span data-stu-id="e690c-141">Request body</span></span>
<span data-ttu-id="e690c-142">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="e690c-142">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e690c-143">响应</span><span class="sxs-lookup"><span data-stu-id="e690c-143">Response</span></span>

<span data-ttu-id="e690c-144">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和 [attachment](../resources/attachment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="e690c-144">If successful, this method returns a `200 OK` response code and [attachment](../resources/attachment.md) object in the response body.</span></span>

## <a name="example-file-attachment"></a><span data-ttu-id="e690c-145">示例（文件附件）</span><span class="sxs-lookup"><span data-stu-id="e690c-145">Example (file attachment)</span></span>

##### <a name="request"></a><span data-ttu-id="e690c-146">请求</span><span class="sxs-lookup"><span data-stu-id="e690c-146">Request</span></span>
<span data-ttu-id="e690c-147">下面的示例展示了用于获取事件的文件附件的请求。</span><span class="sxs-lookup"><span data-stu-id="e690c-147">Here is an example of the request to get a file attachment on an event.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_file_attachment"
}-->
```http
GET https://graph.microsoft.com/beta/me/events/{id}/attachments/{id}
```

##### <a name="response"></a><span data-ttu-id="e690c-148">响应</span><span class="sxs-lookup"><span data-stu-id="e690c-148">Response</span></span>
<span data-ttu-id="e690c-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="e690c-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.fileAttachment"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 199

{
  "@odata.type": "#microsoft.graph.fileAttachment",
  "contentType": "contentType-value",
  "contentLocation": "contentLocation-value",
  "contentBytes": "contentBytes-value",
  "contentId": "null",
  "lastModifiedDateTime": "2016-01-01T12:00:00Z",
  "id": "id-value",
  "isInline": false,
  "name": "name-value",
  "size": 99
}
```
## <a name="example-item-attachment"></a><span data-ttu-id="e690c-152">示例（项目附件）</span><span class="sxs-lookup"><span data-stu-id="e690c-152">Example (item attachment)</span></span>

##### <a name="request-1"></a><span data-ttu-id="e690c-153">请求 1</span><span class="sxs-lookup"><span data-stu-id="e690c-153">Request 1</span></span>
<span data-ttu-id="e690c-p107">第一个示例演示如何在邮件上获取项目附件。返回 **itemAttachment** 的属性。</span><span class="sxs-lookup"><span data-stu-id="e690c-p107">The first example shows how to get an item attachment on a message. The properties of the **itemAttachment** are returned.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_item_attachment"
}-->
```http
GET https://graph.microsoft.com/beta/me/messages('AAMkADA1M-zAAA=')/attachments('AAMkADA1M-CJKtzmnlcqVgqI=')
```

##### <a name="response-1"></a><span data-ttu-id="e690c-156">响应 1</span><span class="sxs-lookup"><span data-stu-id="e690c-156">Response 1</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.itemAttachment"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#users('d1a2fae9-db66-4cc9-8133-2184c77af1b8')/messages('AAMkADA1M-zAAA%3D')/attachments/$entity",
  "@odata.type":"#microsoft.graph.itemAttachment",
  "id":"AAMkADA1MCJKtzmnlcqVgqI=",
  "lastModifiedDateTime":"2017-07-21T00:20:34Z",
  "name":"Reminder - please bring laptop",
  "contentType":null,
  "size":32005,
  "isInline":false
}
```


##### <a name="request-2"></a><span data-ttu-id="e690c-157">请求 2</span><span class="sxs-lookup"><span data-stu-id="e690c-157">Request 2</span></span>
<span data-ttu-id="e690c-p108">下面的示例演示如何使用 `$expand` 来获取附加到该邮件的项目的属性。在此示例中，该项目是一封邮件；还会返回该附加邮件的属性。</span><span class="sxs-lookup"><span data-stu-id="e690c-p108">The next example shows how to use `$expand` to get the properties of the item that is attached to the message. In this example, that item is a message; the properties of that attached message are also returned.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_and_expand_item_attachment"
}-->
```http
GET https://graph.microsoft.com/beta/me/messages('AAMkADA1M-zAAA=')/attachments('AAMkADA1M-CJKtzmnlcqVgqI=')/?$expand=microsoft.graph.itemattachment/item 
```

##### <a name="response-2"></a><span data-ttu-id="e690c-160">响应 2</span><span class="sxs-lookup"><span data-stu-id="e690c-160">Response 2</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.itemAttachment"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#users('d1a2fae9-db66-4cc9-8133-2184c77af1b8')/messages('AAMkADA1M-zAAA%3D')/attachments/$entity",
  "@odata.type":"#microsoft.graph.itemAttachment",
  "id":"AAMkADA1MCJKtzmnlcqVgqI=",
  "lastModifiedDateTime":"2017-07-21T00:20:34Z",
  "name":"Reminder - please bring laptop",
  "contentType":null,
  "size":32005,
  "isInline":false,
  "item@odata.context":"https://graph.microsoft.com/beta/$metadata#users('d1a2fae9-db66-4cc9-8133-2184c77af1b8')/messages('AAMkADA1M-zAAA%3D')/attachments('AAMkADA1M-CJKtzmnlcqVgqI%3D')/microsoft.graph.itemAttachment/item/$entity",
  "item":{
    "@odata.type":"#microsoft.graph.message",
    "id":"",
    "createdDateTime":"2017-07-21T00:20:41Z",
    "lastModifiedDateTime":"2017-07-21T00:20:34Z",
    "receivedDateTime":"2017-07-21T00:19:55Z",
    "sentDateTime":"2017-07-21T00:19:52Z",
    "hasAttachments":false,
    "internetMessageId":"<BY2PR15MB05189A084C01F466709E414F9CA40@BY2PR15MB0518.namprd15.prod.outlook.com>",
    "subject":"Reminder - please bring laptop",
    "importance":"normal",
    "conversationId":"AAQkADA1MzMyOGI4LTlkZDctNDkzYy05M2RiLTdiN2E1NDE3MTRkOQAQAMG_NSCMBqdKrLa2EmR-lO0=",
    "conversationIndex":"AQHTAbcSwb41IIwGp0qstrYSZH+U7Q==",
    "isDeliveryReceiptRequested":false,
    "isReadReceiptRequested":false,
    "isRead":false,
    "isDraft":false,
    "webLink":"https://outlook.office365.com/owa/?ItemID=AAMkADA1M3MTRkOQAAAA%3D%3D&exvsurl=1&viewmodel=ReadMessageItem",
    "body":{
      "contentType":"html",
      "content":"<html><head>\r\n</head>\r\n<body>\r\n</body>\r\n</html>"
    },
    "sender":{
      "emailAddress":{
        "name":"Adele Vance",
        "address":"AdeleV@contoso.onmicrosoft.com"
      }
    },
    "from":{
      "emailAddress":{
        "name":"Adele Vance",
        "address":"AdeleV@contoso.onmicrosoft.com"
      }
    },
    "toRecipients":[
      {
        "emailAddress":{
          "name":"Alex Wilbur",
          "address":"AlexW@contoso.onmicrosoft.com"
        }
      }
    ],
    "ccRecipients":[
      {
        "emailAddress":{
          "name":"Adele Vance",
          "address":"AdeleV@contoso.onmicrosoft.com"
        }
      }
    ],
    "flag":{
      "flagStatus":"notFlagged"
    }
  }
}
```


## <a name="example-reference-attachment"></a><span data-ttu-id="e690c-161">示例（参考附件）</span><span class="sxs-lookup"><span data-stu-id="e690c-161">Example (reference attachment)</span></span>

##### <a name="request"></a><span data-ttu-id="e690c-162">请求</span><span class="sxs-lookup"><span data-stu-id="e690c-162">Request</span></span>
<span data-ttu-id="e690c-163">下面的示例展示了用于获取事件的参考附件的请求。</span><span class="sxs-lookup"><span data-stu-id="e690c-163">Here is an example of the request to get a reference attachment on an event.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_reference_attachment"
}-->
```http
GET https://graph.microsoft.com/beta/me/events/AAMkAGE1M88AADUv0uAAAG=/attachments/AAMkAGE1Mg72tgf7hJp0PICVGCc0g=
```

##### <a name="response"></a><span data-ttu-id="e690c-164">响应</span><span class="sxs-lookup"><span data-stu-id="e690c-164">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.referenceAttachment"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#users/ddfcd489-628b-40d7-b48b-57002df800e5/events/AAMkAGE1M88AADUv0uAAAG%3D/attachments/$entity",
  "@odata.type": "#microsoft.graph.referenceAttachment",
  "id": "AAMkAGE1Mg72tgf7hJp0PCGVCIc0g=",
  "lastModifiedDateTime": "2016-03-12T06:04:38Z",
  "name": "Personal pictures",
  "contentType": null,
  "size": 382,
  "isInline": false,
  "sourceUrl": "https://contoso.com/personal/mario_contoso_net/Documents/Pics",
  "providerType": "oneDriveConsumer",
  "thumbnailUrl": null,
  "previewUrl": null,
  "permission": "edit",
  "isFolder": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get attachment",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
