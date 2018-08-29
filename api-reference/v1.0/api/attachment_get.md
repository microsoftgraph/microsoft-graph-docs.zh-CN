# <a name="get-attachment"></a><span data-ttu-id="7be31-101">获取附件</span><span class="sxs-lookup"><span data-stu-id="7be31-101">Get attachment</span></span>

<span data-ttu-id="7be31-102">读取附加到[事件](../resources/event.md)、[邮件](../resources/message.md)或[帖子](../resources/post.md)的附件的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="7be31-102">Read the properties and relationships of an attachment, attached to an [event](../resources/event.md), [message](../resources/message.md), or [post](../resources/post.md).</span></span> 

<span data-ttu-id="7be31-103">附件可以是下列类型之一：</span><span class="sxs-lookup"><span data-stu-id="7be31-103">An attachment can be one of the following types:</span></span>

* <span data-ttu-id="7be31-104">文件（[fileAttachment](../resources/fileattachment.md) 资源）。</span><span class="sxs-lookup"><span data-stu-id="7be31-104">A file ([fileAttachment](../resources/fileattachment.md) resource).</span></span>
* <span data-ttu-id="7be31-p101">项（由 [itemAttachment](../resources/itemattachment.md) 资源表示的联系人、事件或邮件）。可以使用 `$expand` 来进一步获取该项的属性。请参阅以下[示例](#request-2)。</span><span class="sxs-lookup"><span data-stu-id="7be31-p101">An item (contact, event or message, represented by an [itemAttachment](../resources/itemattachment.md) resource). You can use `$expand` to further get the properties of that item. See an [example](#request-2) below.</span></span>
* <span data-ttu-id="7be31-108">文件链接（[referenceAttachment](../resources/referenceAttachment.md) 资源）。</span><span class="sxs-lookup"><span data-stu-id="7be31-108">A link to a file ([referenceAttachment](../resources/referenceAttachment.md) resource).</span></span>

<span data-ttu-id="7be31-109">所有这些类型的 attachment 资源均派生自 [attachment](../resources/attachment.md) 资源。</span><span class="sxs-lookup"><span data-stu-id="7be31-109">All these types of attachment resources are derived from the [attachment](../resources/attachment.md) resource.</span></span> 


## <a name="permissions"></a><span data-ttu-id="7be31-110">权限</span><span class="sxs-lookup"><span data-stu-id="7be31-110">Permissions</span></span>
<span data-ttu-id="7be31-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="7be31-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

* <span data-ttu-id="7be31-113">如果访问邮件中的附件：Mail.Read。</span><span class="sxs-lookup"><span data-stu-id="7be31-113">If accessing attachments in messages: Mail.Read.</span></span>
* <span data-ttu-id="7be31-114">如果访问事件中的附件：Calendars.Read。</span><span class="sxs-lookup"><span data-stu-id="7be31-114">If accessing attachments in events: Calendars.Read.</span></span>
* <span data-ttu-id="7be31-115">如果访问组帖子中的附件：Group.Read.All。</span><span class="sxs-lookup"><span data-stu-id="7be31-115">If accessing attachments in group events or posts: Group.Read.All.</span></span>

<!--
* If accessing attachments in group events or posts: Group.Read.All.
-->

## <a name="http-request"></a><span data-ttu-id="7be31-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7be31-116">HTTP request</span></span>
<span data-ttu-id="7be31-117">用户的默认[日历](../resources/calendar.md)中的 [事件](../resources/event.md)附件。</span><span class="sxs-lookup"><span data-stu-id="7be31-117">Attachments for an [event](../resources/event.md) in the user's or group's default [calendar](../resources/calendar.md).</span></span>

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

<span data-ttu-id="7be31-118">属于用户的默认 [calendarGroup](../resources/calendargroup.md) 的 [日历](../resources/calendar.md)中的 [事件](../resources/event.md)附件。</span><span class="sxs-lookup"><span data-stu-id="7be31-118">Attachments for an [event](../resources/event.md) in a [calendar](../resources/calendar.md) belonging to the user's default [calendarGroup](../resources/calendargroup.md).</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/calendars/{id}/events/{id}/attachments/{id}
GET /users/{id | userPrincipalName}/calendars/{id}/events/{id}/attachments/{id}

GET /me/calendargroup/calendars/{id}/events/{id}/attachments/{id}
GET /users/{id | userPrincipalName}/calendargroup/calendars/{id}/events/{id}/attachments/{id}
```
<span data-ttu-id="7be31-119">属于用户的 [calendarGroup](../resources/calendargroup.md) 的 [日历](../resources/calendar.md) 中的 [事件](../resources/event.md) 附件。</span><span class="sxs-lookup"><span data-stu-id="7be31-119">Attachments for an [event](../resources/event.md) in a [calendar](../resources/calendar.md) belonging to a user's [calendarGroup](../resources/calendargroup.md).</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/calendargroups/{id}/calendars/{id}/events/{id}/attachments/{id}
GET /users/{id | userPrincipalName}/calendargroups/{id}/calendars/{id}/events/{id}/attachments/{id}
```
<span data-ttu-id="7be31-120">用户邮箱中的 [邮件](../resources/message.md) 附件。</span><span class="sxs-lookup"><span data-stu-id="7be31-120">Attachments for a [message](../resources/message.md) in a user's mailbox.</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/messages/{id}/attachments/{id}
GET /users/{id | userPrincipalName}/messages/{id}/attachments/{id}
```
<span data-ttu-id="7be31-121">用户邮箱的顶级 [mailFolder](../resources/mailfolder.md) 中包含的[邮件](../resources/message.md)附件。</span><span class="sxs-lookup"><span data-stu-id="7be31-121">Attachments for a [message](../resources/message.md) contained in a top level [mailFolder](../resources/mailfolder.md) in a user's mailbox.</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/{id}/messages/{id}/attachments/{id}
GET /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/attachments/{id}
```
<span data-ttu-id="7be31-122">用户邮箱的子文件夹 [mailFolder](../resources/mailfolder.md) 中包含的 [邮件](../resources/message.md)附件。</span><span class="sxs-lookup"><span data-stu-id="7be31-122">Attachments for a [message](../resources/message.md) contained in a top level [mailFolder](../resources/mailfolder.md) in a user's mailbox.</span></span>  <span data-ttu-id="7be31-123">下面的示例显示了一个嵌套级别，但联系人可能位于子级的子级中，诸如此类。</span><span class="sxs-lookup"><span data-stu-id="7be31-123">A contact contained in a child folder of a contactFolder. The example below shows one level of nesting, but a contact can be located in a child of a child and so on.</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/{id}/childFolders/{id}/.../messages/{id}/attachments/{id}
GET /users/{id | userPrincipalName}/mailFolders/{id}/childFolders/{id}/messages/{id}/attachments/{id}
```
<span data-ttu-id="7be31-124">属于组的 [对话](../resources/conversation.md)的 [线程](../resources/conversationthread.md)中的 [帖子](../resources/post.md)附件。</span><span class="sxs-lookup"><span data-stu-id="7be31-124">Attachments for a [post](../resources/post.md) in a [thread](../resources/conversationthread.md) belonging to a [conversation](../resources/conversation.md) of a group.</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/threads/{id}/posts/{id}/attachments/{id}
GET /groups/{id}/conversations/{id}/threads/{id}/posts/{id}/attachments/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="7be31-125">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="7be31-125">Optional query parameters</span></span>
<span data-ttu-id="7be31-126">此方法支持 [OData 查询参数](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="7be31-126">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="7be31-127">请求标头</span><span class="sxs-lookup"><span data-stu-id="7be31-127">Request headers</span></span>
| <span data-ttu-id="7be31-128">名称</span><span class="sxs-lookup"><span data-stu-id="7be31-128">Name</span></span>       | <span data-ttu-id="7be31-129">类型</span><span class="sxs-lookup"><span data-stu-id="7be31-129">Type</span></span> | <span data-ttu-id="7be31-130">说明</span><span class="sxs-lookup"><span data-stu-id="7be31-130">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="7be31-131">授权</span><span class="sxs-lookup"><span data-stu-id="7be31-131">Authorization</span></span>  | <span data-ttu-id="7be31-132">字符串</span><span class="sxs-lookup"><span data-stu-id="7be31-132">string</span></span>  | <span data-ttu-id="7be31-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="7be31-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7be31-135">请求正文</span><span class="sxs-lookup"><span data-stu-id="7be31-135">Request body</span></span>
<span data-ttu-id="7be31-136">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="7be31-136">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7be31-137">响应</span><span class="sxs-lookup"><span data-stu-id="7be31-137">Response</span></span>

<span data-ttu-id="7be31-p105">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和 **attachment** 对象。返回附件类型的属性：[fileAttachment](../resources/fileattachment.md)、[itemAttachment](../resources/itemattachment.md) 或 [referenceAttachment](../resources/referenceAttachment.md)。</span><span class="sxs-lookup"><span data-stu-id="7be31-p105">If successful, this method returns a `200 OK` response code and an **attachment** object in the response body. The properties of that type of attachment are returned: [fileAttachment](../resources/fileattachment.md), [itemAttachment](../resources/itemattachment.md), or [referenceAttachment](../resources/referenceAttachment.md).</span></span>

## <a name="example-file-attachment"></a><span data-ttu-id="7be31-140">示例（文件附件）</span><span class="sxs-lookup"><span data-stu-id="7be31-140">Example (file attachment)</span></span>

##### <a name="request"></a><span data-ttu-id="7be31-141">请求</span><span class="sxs-lookup"><span data-stu-id="7be31-141">Request</span></span>
<span data-ttu-id="7be31-142">下面的示例展示了用于获取事件的文件附件的请求。</span><span class="sxs-lookup"><span data-stu-id="7be31-142">Here is an example of the request to get a file attachment on an event.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_file_attachment"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/events/{id}/attachments/{id}
```

##### <a name="response"></a><span data-ttu-id="7be31-143">响应</span><span class="sxs-lookup"><span data-stu-id="7be31-143">Response</span></span>
<span data-ttu-id="7be31-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="7be31-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "contentBytes": "binary",
  "contentId": "null",
  "lastModifiedDateTime": "2016-01-01T12:00:00Z",
  "id": "id-value",
  "isInline": false,
  "name": "name-value",
  "size": 99
}
```
## <a name="example-item-attachment"></a><span data-ttu-id="7be31-147">示例（项目附件）</span><span class="sxs-lookup"><span data-stu-id="7be31-147">Example (item attachment)</span></span>

##### <a name="request-1"></a><span data-ttu-id="7be31-148">请求 1</span><span class="sxs-lookup"><span data-stu-id="7be31-148">Request 1</span></span>
<span data-ttu-id="7be31-p107">第一个示例演示如何在邮件上获取项目附件。返回 **itemAttachment** 的属性。</span><span class="sxs-lookup"><span data-stu-id="7be31-p107">The first example shows how to get an item attachment on a message. The properties of the **itemAttachment** are returned.</span></span>
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkADA1M-zAAA=", "AAMkADA1M-CJKtzmnlcqVgqI="],
  "name": "get_item_attachment"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/messages/AAMkADA1M-zAAA=/attachments/AAMkADA1M-CJKtzmnlcqVgqI=
```

##### <a name="response-1"></a><span data-ttu-id="7be31-151">响应 1</span><span class="sxs-lookup"><span data-stu-id="7be31-151">Response 1</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.itemAttachment"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users('d1a2fae9-db66-4cc9-8133-2184c77af1b8')/messages('AAMkADA1M-zAAA%3D')/attachments/$entity",
  "@odata.type":"#microsoft.graph.itemAttachment",
  "id":"AAMkADA1MCJKtzmnlcqVgqI=",
  "lastModifiedDateTime":"2017-07-21T00:20:34Z",
  "name":"Reminder - please bring laptop",
  "contentType":null,
  "size":32005,
  "isInline":false
}
```

##### <a name="request-2"></a><span data-ttu-id="7be31-152">请求 2</span><span class="sxs-lookup"><span data-stu-id="7be31-152">Request 2</span></span>
<span data-ttu-id="7be31-p108">下面的示例演示如何使用 `$expand` 来获取附加到该邮件的项目的属性。在此示例中，该项目是一封邮件；还会返回该附加邮件的属性。</span><span class="sxs-lookup"><span data-stu-id="7be31-p108">The next example shows how to use `$expand` to get the properties of the item that is attached to the message. In this example, that item is a message; the properties of that attached message are also returned.</span></span>
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkADA1M-zAAA=", "AAMkADA1M-CJKtzmnlcqVgqI="],
  "name": "get_and_expand_item_attachment"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/messages/AAMkADA1M-zAAA=/attachments/AAMkADA1M-CJKtzmnlcqVgqI=/?$expand=microsoft.graph.itemattachment/item 
```

##### <a name="response-2"></a><span data-ttu-id="7be31-155">响应 2</span><span class="sxs-lookup"><span data-stu-id="7be31-155">Response 2</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.itemAttachment"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users('d1a2fae9-db66-4cc9-8133-2184c77af1b8')/messages('AAMkADA1M-zAAA%3D')/attachments/$entity",
  "@odata.type":"#microsoft.graph.itemAttachment",
  "id":"AAMkADA1MCJKtzmnlcqVgqI=",
  "lastModifiedDateTime":"2017-07-21T00:20:34Z",
  "name":"Reminder - please bring laptop",
  "contentType":null,
  "size":32005,
  "isInline":false,
  "item@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users('d1a2fae9-db66-4cc9-8133-2184c77af1b8')/messages('AAMkADA1M-zAAA%3D')/attachments('AAMkADA1M-CJKtzmnlcqVgqI%3D')/microsoft.graph.itemAttachment/item/$entity",
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
    ]
  }
}
```



## <a name="example-reference-attachment"></a><span data-ttu-id="7be31-156">示例（参考附件）</span><span class="sxs-lookup"><span data-stu-id="7be31-156">Example (reference attachment)</span></span>
##### <a name="request"></a><span data-ttu-id="7be31-157">请求</span><span class="sxs-lookup"><span data-stu-id="7be31-157">Request</span></span>
<span data-ttu-id="7be31-158">下面的示例展示了用于获取事件的参考附件的请求。</span><span class="sxs-lookup"><span data-stu-id="7be31-158">Here is an example of the request to get a reference attachment on an event.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_reference_attachment"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/events/{id}/attachments/{id}
```
##### <a name="response"></a><span data-ttu-id="7be31-159">响应</span><span class="sxs-lookup"><span data-stu-id="7be31-159">Response</span></span>
<span data-ttu-id="7be31-p109">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="7be31-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.referenceAttachment"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 215

{
  "@odata.type": "#microsoft.graph.referenceAttachment",
  "contentType": "contentType-value",
  "lastModifiedDateTime": "datetime-value",
  "id": "id-value",
  "isInline": false,
  "name": "name-value",
  "size": 99,
}
```



<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get attachment",
  "keywords": "",
  "section": "documentation",
  "suppressions": [
    "Error: get_and_expand_item_attachment/item:
      Property 'item' is of type Custom but has no custom members."
  ],
  "tocPath": ""
}-->
