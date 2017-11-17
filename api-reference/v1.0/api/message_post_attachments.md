# <a name="add-attachment"></a><span data-ttu-id="48708-101">Add attachment</span><span class="sxs-lookup"><span data-stu-id="48708-101">Add attachment</span></span>

<span data-ttu-id="48708-102">使用此 API 可将[附件](../resources/attachment.md)添加到邮件中。</span><span class="sxs-lookup"><span data-stu-id="48708-102">Use this API to add an [attachment](../resources/attachment.md) to a message.</span></span> 

<span data-ttu-id="48708-103">附件可以是下列类型之一：</span><span class="sxs-lookup"><span data-stu-id="48708-103">An attachment can be one of the following types:</span></span>

* <span data-ttu-id="48708-104">文件（[fileAttachment](../resources/fileattachment.md) 资源）。</span><span class="sxs-lookup"><span data-stu-id="48708-104">A file ([fileAttachment](../resources/fileattachment.md) resource).</span></span>
* <span data-ttu-id="48708-105">项（由 [itemAttachment](../resources/itemattachment.md) 资源表示的联系人、事件或邮件）。</span><span class="sxs-lookup"><span data-stu-id="48708-105">An item (contact, event or message, represented by an [itemAttachment](../resources/itemattachment.md) resource).</span></span>
* <span data-ttu-id="48708-106">指向文件的链接（[referenceAttachment](../resources/referenceAttachment.md) 资源）。</span><span class="sxs-lookup"><span data-stu-id="48708-106">A link to a file ([referenceAttachment](../resources/referenceAttachment.md) resource).</span></span>

<span data-ttu-id="48708-107">所有这些类型的 attachment 资源均派生自 [attachment](../resources/attachment.md) 资源。</span><span class="sxs-lookup"><span data-stu-id="48708-107">All these types of attachment resources are derived from the [attachment](../resources/attachment.md) resource.</span></span> 

<span data-ttu-id="48708-108">通过发布到邮件附件集合，你可以把附件添加到现有邮件，也可以把附件添加到 [正在创建和发送的邮件](../api/user_sendmail.md)。</span><span class="sxs-lookup"><span data-stu-id="48708-108">You can add an attachment to an existing message by posting to its attachments collection, or you can add an attachment to a message that is being [created and sent on the fly](../api/user_sendmail.md).</span></span>

<span data-ttu-id="48708-109">由于目前每个 REST 请求的总大小限制为 4 MB，这就要求可添加的附件小于 4 MB。</span><span class="sxs-lookup"><span data-stu-id="48708-109">Since there is currently a limit of 4MB on the total size of each REST request, this limits the size of the attachment you can add to under 4MB.</span></span>
## <a name="permissions"></a><span data-ttu-id="48708-110">权限</span><span class="sxs-lookup"><span data-stu-id="48708-110">Permissions</span></span>
<span data-ttu-id="48708-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="48708-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="48708-113">权限类型</span><span class="sxs-lookup"><span data-stu-id="48708-113">Permission type</span></span>      | <span data-ttu-id="48708-114">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="48708-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="48708-115">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="48708-115">Delegated (work or school account)</span></span> | <span data-ttu-id="48708-116">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="48708-116">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="48708-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="48708-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="48708-118">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="48708-118">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="48708-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="48708-119">Application</span></span> | <span data-ttu-id="48708-120">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="48708-120">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="48708-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="48708-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="48708-122">用户邮箱中的 [邮件](../resources/message.md) 附件。</span><span class="sxs-lookup"><span data-stu-id="48708-122">Attachments for a [message](../resources/message.md) in a user's mailbox.</span></span>
```http
POST /me/messages/{id}/attachments
POST /users/{id | userPrincipalName}/messages/{id}/attachments
```
<span data-ttu-id="48708-123">用户邮箱的顶级 [mailFolder](../resources/mailfolder.md) 中包含的 [邮件](../resources/message.md) 附件。</span><span class="sxs-lookup"><span data-stu-id="48708-123">Attachments for a [message](../resources/message.md) contained in a top level [mailFolder](../resources/mailfolder.md) in a user's mailbox.</span></span>
```http
POST /me/mailFolders/{id}/messages/{id}/attachments
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/attachments
```
<span data-ttu-id="48708-p102">用户邮箱的 [mailFolder](../resources/mailfolder.md) 的子文件夹中包含的 [邮件](../resources/message.md) 附件。下面的示例显示了一个嵌套级别，但邮件可能位于子级的子级中，诸如此类。</span><span class="sxs-lookup"><span data-stu-id="48708-p102">Attachments for a [message](../resources/message.md) contained in a child folder of a [mailFolder](../resources/mailfolder.md) in a user's mailbox.  The example below shows one level of nesting, but a message can be located in a child of a child and so on.</span></span>
```http
POST /me/mailFolders/{id}/childFolders/{id}/.../messages/{id}/attachments/{id}
POST /users/{id | userPrincipalName}/mailFolders/{id}/childFolders/{id}/messages/{id}/attachments/{id}
```
## <a name="request-headers"></a><span data-ttu-id="48708-126">请求标头</span><span class="sxs-lookup"><span data-stu-id="48708-126">Request headers</span></span>
| <span data-ttu-id="48708-127">名称</span><span class="sxs-lookup"><span data-stu-id="48708-127">Name</span></span>       | <span data-ttu-id="48708-128">类型</span><span class="sxs-lookup"><span data-stu-id="48708-128">Type</span></span> | <span data-ttu-id="48708-129">说明</span><span class="sxs-lookup"><span data-stu-id="48708-129">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="48708-130">Authorization</span><span class="sxs-lookup"><span data-stu-id="48708-130">Authorization</span></span>  | <span data-ttu-id="48708-131">string</span><span class="sxs-lookup"><span data-stu-id="48708-131">string</span></span>  | <span data-ttu-id="48708-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="48708-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="48708-134">Content-Type</span><span class="sxs-lookup"><span data-stu-id="48708-134">Content-Type</span></span> | <span data-ttu-id="48708-135">string</span><span class="sxs-lookup"><span data-stu-id="48708-135">string</span></span>  | <span data-ttu-id="48708-p104">实体正文中的数据性质。必需。</span><span class="sxs-lookup"><span data-stu-id="48708-p104">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="48708-138">请求正文</span><span class="sxs-lookup"><span data-stu-id="48708-138">Request body</span></span>
<span data-ttu-id="48708-139">在请求正文中，提供 [Attachment](../resources/attachment.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="48708-139">In the request body, supply a JSON representation of [Attachment](../resources/attachment.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="48708-140">响应</span><span class="sxs-lookup"><span data-stu-id="48708-140">Response</span></span>

<span data-ttu-id="48708-141">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [Attachment](../resources/attachment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="48708-141">If successful, this method returns `201 Created` response code and [Attachment](../resources/attachment.md) object in the response body.</span></span>

## <a name="example-file-attachment"></a><span data-ttu-id="48708-142">示例（文件附件）</span><span class="sxs-lookup"><span data-stu-id="48708-142">Example (file attachment)</span></span>

##### <a name="request"></a><span data-ttu-id="48708-143">请求</span><span class="sxs-lookup"><span data-stu-id="48708-143">Request</span></span>
<span data-ttu-id="48708-144">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="48708-144">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_file_attachment_from_message"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/messages/AAMkpsDRVK/attachments
Content-type: application/json
Content-length: 142

{
  "@odata.type": "#microsoft.graph.fileAttachment",
  "name": "smile",
  "contentBytes": "R0lGODdhEAYEAA7"
}
```

<span data-ttu-id="48708-145">在请求正文中，提供 [attachment](../resources/attachment.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="48708-145">In the request body, supply a JSON representation of [attachment](../resources/attachment.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="48708-146">响应</span><span class="sxs-lookup"><span data-stu-id="48708-146">Response</span></span>
<span data-ttu-id="48708-147">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="48708-147">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.fileAttachment"
} -->
```http
HTTP 201 Created
Content-type: application/json
Content-length: 202

{
    "id": "AAMkADNkN2R",
    "lastModifiedDateTime": "2017-01-26T08:48:28Z",
    "name": "smile",
    "contentType": "image/gif",
    "size": 1008,
    "isInline": false,
    "contentId": null,
    "contentLocation": null,
    "contentBytes": "R0lGODdhEAYEAA7"
}

```

## <a name="example-item-attachment"></a><span data-ttu-id="48708-148">示例（项目附件）</span><span class="sxs-lookup"><span data-stu-id="48708-148">Example (item attachment)</span></span>

##### <a name="request"></a><span data-ttu-id="48708-149">请求</span><span class="sxs-lookup"><span data-stu-id="48708-149">Request</span></span>
<span data-ttu-id="48708-150">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="48708-150">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_item_attachment_from_message"
}-->

```
POST https://graph.microsoft.com/v1.0/me/messages/AAMkpsDRVK/attachments
Content-type: application/json
Content-length: 200

{
  "@odata.type": "#microsoft.graph.itemAttachment",
  "name": "Holiday event", 
  "item": {
    "@odata.type": "microsoft.graph.event",
    "subject": "Discuss gifts for children",
    "body": {
      "contentType": "HTML",
      "content": "Let's look for funding!"
    },
    "start": {
      "dateTime": "2016-12-02T18:00:00",
      "timeZone": "Pacific Standard Time"
    },
    "end": {
      "dateTime": "2016-12-02T19:00:00",
      "timeZone": "Pacific Standard Time"
    }
  }
}
```

##### <a name="response"></a><span data-ttu-id="48708-151">响应</span><span class="sxs-lookup"><span data-stu-id="48708-151">Response</span></span>
<span data-ttu-id="48708-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="48708-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.itemAttachment"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 162

{
  "id":"AAMkADNkNJp5JVnQIe9r0=",
  "lastModifiedDateTime":"2016-12-01T22:27:13Z",
  "name":"Holiday event",
  "contentType":null,
  "size":2473,
  "isInline":false
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create Attachment",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
