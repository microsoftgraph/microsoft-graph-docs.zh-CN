---
title: 获取附件
description: '读取附加到事件的附件的属性和关系 '
localization_priority: Priority
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 411191bd9a67452e46209f31d193fb148585cb34
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35443852"
---
# <a name="get-attachment"></a><span data-ttu-id="d8feb-103">获取附件</span><span class="sxs-lookup"><span data-stu-id="d8feb-103">Get attachment</span></span>

<span data-ttu-id="d8feb-104">读取附加到[事件](../resources/event.md)、[邮件](../resources/message.md)或[帖子](../resources/post.md)的附件的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="d8feb-104">Read the properties and relationships of an attachment, attached to an [event](../resources/event.md), [message](../resources/message.md), or [post](../resources/post.md).</span></span> 

<span data-ttu-id="d8feb-105">附件可以是下列类型之一：</span><span class="sxs-lookup"><span data-stu-id="d8feb-105">An attachment can be one of the following types:</span></span>

* <span data-ttu-id="d8feb-106">文件（[fileAttachment](../resources/fileattachment.md) 资源）。</span><span class="sxs-lookup"><span data-stu-id="d8feb-106">A file ([fileAttachment](../resources/fileattachment.md) resource).</span></span>
* <span data-ttu-id="d8feb-107">项（由 [itemAttachment](../resources/itemattachment.md) 资源表示的联系人、事件或邮件）。</span><span class="sxs-lookup"><span data-stu-id="d8feb-107">An item (contact, event or message, represented by an [itemAttachment](../resources/itemattachment.md) resource).</span></span> <span data-ttu-id="d8feb-108">可使用 `$expand` 来进一步获取该项的属性。</span><span class="sxs-lookup"><span data-stu-id="d8feb-108">You can use `$expand` to further get the properties of that item.</span></span> <span data-ttu-id="d8feb-109">请参阅以下[示例](#request-2)。</span><span class="sxs-lookup"><span data-stu-id="d8feb-109">See an [example](#request-2) below.</span></span>
* <span data-ttu-id="d8feb-110">指向文件的链接（[referenceAttachment](../resources/referenceattachment.md) 资源）。</span><span class="sxs-lookup"><span data-stu-id="d8feb-110">A link to a file ([referenceAttachment](../resources/referenceattachment.md) resource).</span></span>

<span data-ttu-id="d8feb-111">所有这些类型的 attachment 资源均派生自 [attachment](../resources/attachment.md) 资源。</span><span class="sxs-lookup"><span data-stu-id="d8feb-111">All these types of attachment resources are derived from the [attachment](../resources/attachment.md) resource.</span></span> 


## <a name="permissions"></a><span data-ttu-id="d8feb-112">权限</span><span class="sxs-lookup"><span data-stu-id="d8feb-112">Permissions</span></span>
<span data-ttu-id="d8feb-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d8feb-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

* <span data-ttu-id="d8feb-115">如果访问邮件中的附件：Mail.Read。</span><span class="sxs-lookup"><span data-stu-id="d8feb-115">If accessing attachments in Messages: Mail.Read</span></span>
* <span data-ttu-id="d8feb-116">如果访问事件中的附件：Calendars.Read。</span><span class="sxs-lookup"><span data-stu-id="d8feb-116">If accessing attachments in Events: Calendars.Read</span></span>
* <span data-ttu-id="d8feb-117">如果访问组帖子中的附件：Group.Read.All。</span><span class="sxs-lookup"><span data-stu-id="d8feb-117">If accessing attachments in group events or posts: Group.Read.All</span></span>

<!--
* If accessing attachments in group events or posts: Group.Read.All.
-->

## <a name="http-request"></a><span data-ttu-id="d8feb-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d8feb-118">HTTP request</span></span>
<span data-ttu-id="d8feb-119">用户的默认[日历](../resources/calendar.md)中的[事件](../resources/event.md)附件。</span><span class="sxs-lookup"><span data-stu-id="d8feb-119">Attachments for an [event](../resources/event.md) in the user's or group's default [calendar](../resources/calendar.md).</span></span>

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

<span data-ttu-id="d8feb-120">属于用户的默认 [calendarGroup](../resources/calendargroup.md) 的 [日历](../resources/calendar.md) 中的 [事件](../resources/event.md) 附件。</span><span class="sxs-lookup"><span data-stu-id="d8feb-120">Attachments for an [event](../resources/event.md) in a [calendar](../resources/calendar.md) belonging to the user's default [calendarGroup](../resources/calendargroup.md).</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/calendars/{id}/events/{id}/attachments/{id}
GET /users/{id | userPrincipalName}/calendars/{id}/events/{id}/attachments/{id}

GET /me/calendargroup/calendars/{id}/events/{id}/attachments/{id}
GET /users/{id | userPrincipalName}/calendargroup/calendars/{id}/events/{id}/attachments/{id}
```
<span data-ttu-id="d8feb-121">属于用户的 [calendarGroup](../resources/calendargroup.md) 的 [日历](../resources/calendar.md) 中的 [事件](../resources/event.md) 附件。</span><span class="sxs-lookup"><span data-stu-id="d8feb-121">Attachments for an [event](../resources/event.md) in a [calendar](../resources/calendar.md) belonging to a user's [calendarGroup](../resources/calendargroup.md).</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/calendargroups/{id}/calendars/{id}/events/{id}/attachments/{id}
GET /users/{id | userPrincipalName}/calendargroups/{id}/calendars/{id}/events/{id}/attachments/{id}
```
<span data-ttu-id="d8feb-122">用户邮箱中的 [邮件](../resources/message.md) 附件。</span><span class="sxs-lookup"><span data-stu-id="d8feb-122">Attachments for a [message](../resources/message.md) in a user's mailbox.</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/messages/{id}/attachments/{id}
GET /users/{id | userPrincipalName}/messages/{id}/attachments/{id}
```
<span data-ttu-id="d8feb-123">用户邮箱的顶级 [mailFolder](../resources/mailfolder.md) 中包含的 [邮件](../resources/message.md) 附件。</span><span class="sxs-lookup"><span data-stu-id="d8feb-123">Attachments for a [message](../resources/message.md) contained in a top level [mailFolder](../resources/mailfolder.md) in a user's mailbox.</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/{id}/messages/{id}/attachments/{id}
GET /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/attachments/{id}
```
<span data-ttu-id="d8feb-p103">用户邮箱的 [mailFolder](../resources/mailfolder.md) 的子文件夹中包含的 [邮件](../resources/message.md) 附件。下面的示例显示了一个嵌套级别，但邮件可能位于子级的子级中，诸如此类。 </span><span class="sxs-lookup"><span data-stu-id="d8feb-p103">Attachments for a [message](../resources/message.md) contained in a child folder of a [mailFolder](../resources/mailfolder.md) in a user's mailbox.  The example below shows one level of nesting, but a message can be located in a child of a child and so on. </span></span><!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/{id}/childFolders/{id}/.../messages/{id}/attachments/{id}
GET /users/{id | userPrincipalName}/mailFolders/{id}/childFolders/{id}/messages/{id}/attachments/{id}
```
<span data-ttu-id="d8feb-126">属于组的 [对话](../resources/conversation.md) 的 [线程](../resources/conversationthread.md) 中的 [帖子](../resources/post.md) 附件。</span><span class="sxs-lookup"><span data-stu-id="d8feb-126">Attachments for a [post](../resources/post.md) in a [thread](../resources/conversationthread.md) belonging to a [conversation](../resources/conversation.md) of a group.</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/threads/{id}/posts/{id}/attachments/{id}
GET /groups/{id}/conversations/{id}/threads/{id}/posts/{id}/attachments/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="d8feb-127">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="d8feb-127">Optional query parameters</span></span>
<span data-ttu-id="d8feb-128">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="d8feb-128">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="d8feb-129">请求标头</span><span class="sxs-lookup"><span data-stu-id="d8feb-129">Request headers</span></span>
| <span data-ttu-id="d8feb-130">名称</span><span class="sxs-lookup"><span data-stu-id="d8feb-130">Name</span></span>       | <span data-ttu-id="d8feb-131">类型</span><span class="sxs-lookup"><span data-stu-id="d8feb-131">Type</span></span> | <span data-ttu-id="d8feb-132">说明</span><span class="sxs-lookup"><span data-stu-id="d8feb-132">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="d8feb-133">Authorization</span><span class="sxs-lookup"><span data-stu-id="d8feb-133">Authorization</span></span>  | <span data-ttu-id="d8feb-134">string</span><span class="sxs-lookup"><span data-stu-id="d8feb-134">string</span></span>  | <span data-ttu-id="d8feb-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="d8feb-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d8feb-137">请求正文</span><span class="sxs-lookup"><span data-stu-id="d8feb-137">Request body</span></span>
<span data-ttu-id="d8feb-138">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="d8feb-138">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d8feb-139">响应</span><span class="sxs-lookup"><span data-stu-id="d8feb-139">Response</span></span>

<span data-ttu-id="d8feb-140">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和 **attachment** 对象。</span><span class="sxs-lookup"><span data-stu-id="d8feb-140">If successful, this method returns a `200 OK` response code and **attachment** object in the response body.</span></span> <span data-ttu-id="d8feb-141">返回附件类型的属性：[fileAttachment](../resources/fileattachment.md)、[itemAttachment](../resources/itemattachment.md) 或 [referenceAttachment](../resources/referenceattachment.md)。</span><span class="sxs-lookup"><span data-stu-id="d8feb-141">The properties of that type of attachment are returned: [fileAttachment](../resources/fileattachment.md), [itemAttachment](../resources/itemattachment.md), or [referenceAttachment](../resources/referenceattachment.md).</span></span>

## <a name="example-file-attachment"></a><span data-ttu-id="d8feb-142">示例（文件附件）</span><span class="sxs-lookup"><span data-stu-id="d8feb-142">Example (file attachment)</span></span>

##### <a name="request"></a><span data-ttu-id="d8feb-143">请求</span><span class="sxs-lookup"><span data-stu-id="d8feb-143">Request</span></span>
<span data-ttu-id="d8feb-144">下面的示例展示了用于获取事件的文件附件的请求。</span><span class="sxs-lookup"><span data-stu-id="d8feb-144">Here is an example of the request to get a file attachment on an event.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="d8feb-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="d8feb-145">--Http</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_file_attachment"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/events/{id}/attachments/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="d8feb-146">C#</span><span class="sxs-lookup"><span data-stu-id="d8feb-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-file-attachment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d8feb-147">Javascript</span><span class="sxs-lookup"><span data-stu-id="d8feb-147">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-file-attachment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="d8feb-148">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d8feb-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-file-attachment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="d8feb-149">响应</span><span class="sxs-lookup"><span data-stu-id="d8feb-149">Response</span></span>
<span data-ttu-id="d8feb-p106">下面是一个响应示例。注意：为简洁起见，可能会截断此处展示的响应对象。实际调用会返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="d8feb-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
## <a name="example-item-attachment"></a><span data-ttu-id="d8feb-153">示例（项目附件）</span><span class="sxs-lookup"><span data-stu-id="d8feb-153">Example (item attachment)</span></span>

##### <a name="request-1"></a><span data-ttu-id="d8feb-154">请求 1</span><span class="sxs-lookup"><span data-stu-id="d8feb-154">Request 1</span></span>
<span data-ttu-id="d8feb-155">第一个示例演示如何在邮件上获取项目附件。</span><span class="sxs-lookup"><span data-stu-id="d8feb-155">The first example shows how to get an item attachment on a message.</span></span> <span data-ttu-id="d8feb-156">返回 **itemAttachment** 的属性。</span><span class="sxs-lookup"><span data-stu-id="d8feb-156">The properties of the **itemAttachment** are returned.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="d8feb-157">HTTP</span><span class="sxs-lookup"><span data-stu-id="d8feb-157">--Http</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkADA1M-zAAA=", "AAMkADA1M-CJKtzmnlcqVgqI="],
  "name": "get_item_attachment"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/messages/AAMkADA1M-zAAA=/attachments/AAMkADA1M-CJKtzmnlcqVgqI=
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="d8feb-158">C#</span><span class="sxs-lookup"><span data-stu-id="d8feb-158">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-item-attachment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d8feb-159">Javascript</span><span class="sxs-lookup"><span data-stu-id="d8feb-159">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-item-attachment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="d8feb-160">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d8feb-160">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-item-attachment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response-1"></a><span data-ttu-id="d8feb-161">响应 1</span><span class="sxs-lookup"><span data-stu-id="d8feb-161">Response 1</span></span>
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

##### <a name="request-2"></a><span data-ttu-id="d8feb-162">请求 2</span><span class="sxs-lookup"><span data-stu-id="d8feb-162">Request 2</span></span>
<span data-ttu-id="d8feb-163">下面的示例演示如何使用 `$expand` 来获取附加到该邮件的项目的属性。</span><span class="sxs-lookup"><span data-stu-id="d8feb-163">The next example shows how to use `$expand` to get the properties of the item that is attached to the message.</span></span> <span data-ttu-id="d8feb-164">在此示例中，该项目是一封邮件；还会返回该附加邮件的属性。</span><span class="sxs-lookup"><span data-stu-id="d8feb-164">In this example, that item is a message; the properties of that attached message are also returned.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="d8feb-165">HTTP</span><span class="sxs-lookup"><span data-stu-id="d8feb-165">--Http</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkADA1M-zAAA=", "AAMkADA1M-CJKtzmnlcqVgqI="],
  "name": "get_and_expand_item_attachment"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/messages/AAMkADA1M-zAAA=/attachments/AAMkADA1M-CJKtzmnlcqVgqI=/?$expand=microsoft.graph.itemattachment/item 
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="d8feb-166">C#</span><span class="sxs-lookup"><span data-stu-id="d8feb-166">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-and-expand-item-attachment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d8feb-167">Javascript</span><span class="sxs-lookup"><span data-stu-id="d8feb-167">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-and-expand-item-attachment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="d8feb-168">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d8feb-168">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-and-expand-item-attachment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response-2"></a><span data-ttu-id="d8feb-169">响应 2</span><span class="sxs-lookup"><span data-stu-id="d8feb-169">Response 2</span></span>
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



## <a name="example-reference-attachment"></a><span data-ttu-id="d8feb-170">示例（参考附件）</span><span class="sxs-lookup"><span data-stu-id="d8feb-170">Example (reference attachment)</span></span>
##### <a name="request"></a><span data-ttu-id="d8feb-171">请求</span><span class="sxs-lookup"><span data-stu-id="d8feb-171">Request</span></span>
<span data-ttu-id="d8feb-172">下面的示例展示了用于获取消息的参考附件的请求。</span><span class="sxs-lookup"><span data-stu-id="d8feb-172">Here is an example of the request to get a reference attachment on an event.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="d8feb-173">HTTP</span><span class="sxs-lookup"><span data-stu-id="d8feb-173">--Http</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_reference_attachment",
  "sampleKeys": ["AAMkAGUzY5QKgAAA=","AAMkAGUzY5QKgAAABEgAQAISJOe1FEqdNsMEQmpZjRW8="]
}-->
```http
GET https://graph.microsoft.com/v1.0/me/messages/AAMkAGUzY5QKgAAA=/attachments/AAMkAGUzY5QKgAAABEgAQAISJOe1FEqdNsMEQmpZjRW8=
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="d8feb-174">C#</span><span class="sxs-lookup"><span data-stu-id="d8feb-174">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-reference-attachment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d8feb-175">Javascript</span><span class="sxs-lookup"><span data-stu-id="d8feb-175">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-reference-attachment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="d8feb-176">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d8feb-176">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-reference-attachment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="d8feb-177">响应</span><span class="sxs-lookup"><span data-stu-id="d8feb-177">Response</span></span>
<span data-ttu-id="d8feb-p109">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="d8feb-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "name": "get_reference_attachment",
  "truncated": true,
  "@odata.type": "microsoft.graph.referenceAttachment"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users('bb8775a4-4d8c-42cf-a1d4-4d58c2bb668f')/messages('AAMkAGUzY5QKgAAA%3D')/attachments/$entity",
    "@odata.type": "#microsoft.graph.referenceAttachment",
    "id": "AAMkAGUzY5QKgAAABEgAQAISJOe1FEqdNsMEQmpZjRW8=",
    "lastModifiedDateTime": "2019-04-02T02:58:11Z",
    "name": "Sales Invoice Template.docx",
    "contentType": "application/vnd.openxmlformats-officedocument.wordprocessingml.document",
    "size": 1060,
    "isInline": true
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
