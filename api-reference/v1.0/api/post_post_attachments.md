# <a name="add-attachment"></a><span data-ttu-id="238ed-101">添加附件</span><span class="sxs-lookup"><span data-stu-id="238ed-101">Add attachment</span></span>

<span data-ttu-id="238ed-p101">使用此 API 将 [附件](../resources/attachment.md) 添加到帖子。由于目前每个 REST 请求的总大小限制为 4 MB，这就要求可添加的附件小于 4 MB。</span><span class="sxs-lookup"><span data-stu-id="238ed-p101">Use this API to add an [attachment](../resources/attachment.md) to a post. Since there is currently a limit of 4MB on the total size of each REST request, this limits the size of the attachment you can add to under 4MB.</span></span>

<span data-ttu-id="238ed-104">附件可以是下列类型之一：</span><span class="sxs-lookup"><span data-stu-id="238ed-104">An attachment can be one of the following types:</span></span>

* <span data-ttu-id="238ed-105">文件（[fileAttachment](../resources/fileattachment.md) 资源）。</span><span class="sxs-lookup"><span data-stu-id="238ed-105">A file ([fileAttachment](../resources/fileattachment.md) resource).</span></span>
* <span data-ttu-id="238ed-106">项（由 [itemAttachment](../resources/itemattachment.md) 资源表示的联系人、事件或邮件）。</span><span class="sxs-lookup"><span data-stu-id="238ed-106">An item (contact, event or message, represented by an [itemAttachment](../resources/itemattachment.md) resource).</span></span>
* <span data-ttu-id="238ed-107">指向文件的链接（[referenceAttachment](../resources/referenceAttachment.md) 资源）。</span><span class="sxs-lookup"><span data-stu-id="238ed-107">A link to a file ([referenceAttachment](../resources/referenceAttachment.md) resource).</span></span>

<span data-ttu-id="238ed-108">所有这些类型的 attachment 资源均派生自 [attachment](../resources/attachment.md) 资源。</span><span class="sxs-lookup"><span data-stu-id="238ed-108">All these types of attachment resources are derived from the [attachment](../resources/attachment.md) resource.</span></span> 

## <a name="permissions"></a><span data-ttu-id="238ed-109">权限</span><span class="sxs-lookup"><span data-stu-id="238ed-109">Permissions</span></span>
<span data-ttu-id="238ed-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="238ed-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="238ed-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="238ed-112">Permission type</span></span>      | <span data-ttu-id="238ed-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="238ed-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="238ed-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="238ed-114">Delegated (work or school account)</span></span> | <span data-ttu-id="238ed-115">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="238ed-115">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="238ed-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="238ed-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="238ed-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="238ed-117">Not supported.</span></span>    |
|<span data-ttu-id="238ed-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="238ed-118">Application</span></span> | <span data-ttu-id="238ed-119">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="238ed-119">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="238ed-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="238ed-120">HTTP request</span></span>
<span data-ttu-id="238ed-121"><!-- { "blockType": "ignored" } --> [线程](../resources/post.md)中 [帖子](../resources/conversationthread.md)的附件属于分组 [对话](../resources/conversation.md) 。</span><span class="sxs-lookup"><span data-stu-id="238ed-121">Attachments for a [post](../resources/post.md) in a [thread](../resources/conversationthread.md) belonging to a [conversation](../resources/conversation.md) of a group.</span></span>
```http
POST /groups/{id}/threads/{id}/posts/{id}/attachments
POST /groups/{id}/conversations/{id}/threads/{id}/posts/{id}/attachments
```
## <a name="request-headers"></a><span data-ttu-id="238ed-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="238ed-122">Request headers</span></span>
| <span data-ttu-id="238ed-123">标头</span><span class="sxs-lookup"><span data-stu-id="238ed-123">Header</span></span>       | <span data-ttu-id="238ed-124">值</span><span class="sxs-lookup"><span data-stu-id="238ed-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="238ed-125">授权</span><span class="sxs-lookup"><span data-stu-id="238ed-125">Authorization</span></span>  | <span data-ttu-id="238ed-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="238ed-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="238ed-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="238ed-128">Request body</span></span>
<span data-ttu-id="238ed-129">在请求正文中，提供 [Attachment](../resources/attachment.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="238ed-129">In the request body, supply a JSON representation of [Attachment](../resources/attachment.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="238ed-130">响应</span><span class="sxs-lookup"><span data-stu-id="238ed-130">Response</span></span>

<span data-ttu-id="238ed-131">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [Attachment](../resources/attachment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="238ed-131">If successful, this method returns `201 Created` response code and [Attachment](../resources/attachment.md) object in the response body.</span></span>

## <a name="example-file-attachment"></a><span data-ttu-id="238ed-132">示例（文件附件）</span><span class="sxs-lookup"><span data-stu-id="238ed-132">Example (file attachment)</span></span>

##### <a name="request"></a><span data-ttu-id="238ed-133">请求</span><span class="sxs-lookup"><span data-stu-id="238ed-133">Request</span></span>
<span data-ttu-id="238ed-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="238ed-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_file_attachment_from_post"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/threads/{id}/posts/{id}/attachments
Content-type: application/json
Content-length: 142

{
  "@odata.type": "#microsoft.graph.fileAttachment",
  "name": "name-value",
  "contentBytes": "base64-contentBytes-value"
}
```

<span data-ttu-id="238ed-135">在请求正文中，提供 [attachment](../resources/attachment.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="238ed-135">In the request body, supply a JSON representation of [attachment](../resources/attachment.md) object.</span></span>

##### <a name="response"></a><span data-ttu-id="238ed-136">响应</span><span class="sxs-lookup"><span data-stu-id="238ed-136">Response</span></span>
<span data-ttu-id="238ed-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="238ed-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.attachment"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 162

{
  "lastModifiedDateTime": "datetime-value",
  "name": "name-value",
  "contentType": "contentType-value",
  "size": 99,
  "isInline": true,
  "id": "id-value"
}
```

## <a name="example-item-attachment"></a><span data-ttu-id="238ed-140">示例（项目附件）</span><span class="sxs-lookup"><span data-stu-id="238ed-140">Example (item attachment)</span></span>

##### <a name="request"></a><span data-ttu-id="238ed-141">请求</span><span class="sxs-lookup"><span data-stu-id="238ed-141">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "create_item_attachment_from_post"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/threads/{id}/posts/{id}/attachments
Content-type: application/json
Content-length: 100

{
  "@odata.type": "#microsoft.graph.itemAttachment",
  "name": "name-value",
  "item": { }
}
```

##### <a name="response"></a><span data-ttu-id="238ed-142">响应</span><span class="sxs-lookup"><span data-stu-id="238ed-142">Response</span></span>
<span data-ttu-id="238ed-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="238ed-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.attachment"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 162

{
  "lastModifiedDateTime": "datetime-value",
  "name": "name-value",
  "contentType": "contentType-value",
  "size": 99,
  "isInline": true,
  "id": "id-value"
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
