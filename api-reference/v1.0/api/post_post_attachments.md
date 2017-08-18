# <a name="add-attachment"></a><span data-ttu-id="a2564-101">Add attachment</span><span class="sxs-lookup"><span data-stu-id="a2564-101">Add attachment</span></span>

<span data-ttu-id="a2564-p101">使用此 API 将 [附件](../resources/attachment.md) 添加到帖子。由于目前每个 REST 请求的总大小限制为 4 MB，这就要求可添加的附件小于 4 MB。</span><span class="sxs-lookup"><span data-stu-id="a2564-p101">Use this API to add an [attachment](../resources/attachment.md) to a post. Since there is currently a limit of 4MB on the total size of each REST request, this limits the size of the attachment you can add to under 4MB.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="a2564-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="a2564-104">Prerequisites</span></span>
<span data-ttu-id="a2564-105">要执行此 API，需要以下**范围**之一：</span><span class="sxs-lookup"><span data-stu-id="a2564-105">One of the following **scopes** is required to execute this API:</span></span>

* <span data-ttu-id="a2564-106">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a2564-106">Group.ReadWrite.All</span></span>

## <a name="http-request"></a><span data-ttu-id="a2564-107">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a2564-107">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="a2564-108">属于组的 [对话](../resources/conversation.md) 的 [线程](../resources/conversationthread.md) 中的 [帖子](../resources/post.md) 附件。</span><span class="sxs-lookup"><span data-stu-id="a2564-108">Attachments for a [post](../resources/post.md) in a [thread](../resources/conversationthread.md) belonging to a [conversation](../resources/conversation.md) of a group.</span></span>
```http
POST /groups/{id}/threads/{id}/posts/{id}/attachments
POST /groups/{id}/conversations/{id}/threads/{id}/posts/{id}/attachments
```
## <a name="request-headers"></a><span data-ttu-id="a2564-109">请求标头</span><span class="sxs-lookup"><span data-stu-id="a2564-109">Request headers</span></span>
| <span data-ttu-id="a2564-110">标头</span><span class="sxs-lookup"><span data-stu-id="a2564-110">Header</span></span>       | <span data-ttu-id="a2564-111">值</span><span class="sxs-lookup"><span data-stu-id="a2564-111">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="a2564-112">Authorization</span><span class="sxs-lookup"><span data-stu-id="a2564-112">Authorization</span></span>  | <span data-ttu-id="a2564-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="a2564-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="a2564-115">请求正文</span><span class="sxs-lookup"><span data-stu-id="a2564-115">Request body</span></span>
<span data-ttu-id="a2564-116">在请求正文中，提供 [Attachment](../resources/attachment.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a2564-116">In the request body, supply a JSON representation of [attachment](../resources/attachment.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="a2564-117">响应</span><span class="sxs-lookup"><span data-stu-id="a2564-117">Response</span></span>

<span data-ttu-id="a2564-118">如果成功，此方法在响应正文中返回 `201, Created` 响应代码和 [Attachment](../resources/attachment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="a2564-118">If successful, this method returns `201, Created` response code and [Attachment](../resources/attachment.md) object in the response body.</span></span>

## <a name="example-file-attachment"></a><span data-ttu-id="a2564-119">示例（文件附件）</span><span class="sxs-lookup"><span data-stu-id="a2564-119">Example (file attachment)</span></span>

##### <a name="request"></a><span data-ttu-id="a2564-120">请求</span><span class="sxs-lookup"><span data-stu-id="a2564-120">Request</span></span>
<span data-ttu-id="a2564-121">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="a2564-121">Here is an example of the request.</span></span>
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
  "contentBytes": "contentBytes-value"
}
```

<span data-ttu-id="a2564-122">在请求正文中，提供 [attachment](../resources/attachment.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a2564-122">In the request body, supply a JSON representation of [attachment](../resources/attachment.md) object.</span></span>

##### <a name="response"></a><span data-ttu-id="a2564-123">响应</span><span class="sxs-lookup"><span data-stu-id="a2564-123">Response</span></span>
<span data-ttu-id="a2564-p103">下面是一个响应示例。注意：为简洁起见，可能会截断此处展示的响应对象。实际调用会返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="a2564-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

## <a name="example-item-attachment"></a><span data-ttu-id="a2564-127">示例（项目附件）</span><span class="sxs-lookup"><span data-stu-id="a2564-127">Example (item attachment)</span></span>

##### <a name="request"></a><span data-ttu-id="a2564-128">请求</span><span class="sxs-lookup"><span data-stu-id="a2564-128">Request</span></span>
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

##### <a name="response"></a><span data-ttu-id="a2564-129">响应</span><span class="sxs-lookup"><span data-stu-id="a2564-129">Response</span></span>
<span data-ttu-id="a2564-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="a2564-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
