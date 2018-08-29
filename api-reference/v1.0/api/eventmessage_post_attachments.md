# <a name="add-attachment"></a><span data-ttu-id="94b4c-101">Add attachment</span><span class="sxs-lookup"><span data-stu-id="94b4c-101">Add attachment</span></span>

<span data-ttu-id="94b4c-102">使用此 API 新建附件。</span><span class="sxs-lookup"><span data-stu-id="94b4c-102">Use this API to create a new Attachment.</span></span>

<span data-ttu-id="94b4c-103">附件可以是下列类型之一：</span><span class="sxs-lookup"><span data-stu-id="94b4c-103">An attachment can be one of the following types:</span></span>

* <span data-ttu-id="94b4c-104">文件（[fileAttachment](../resources/fileattachment.md) 资源）。</span><span class="sxs-lookup"><span data-stu-id="94b4c-104">A file ([fileAttachment](../resources/fileattachment.md) resource).</span></span>
* <span data-ttu-id="94b4c-105">项（由 [itemAttachment](../resources/itemattachment.md) 资源表示的联系人、事件或邮件）。</span><span class="sxs-lookup"><span data-stu-id="94b4c-105">An item (contact, event or message, represented by an [itemAttachment](../resources/itemattachment.md) resource).</span></span>
* <span data-ttu-id="94b4c-106">指向文件的链接（[referenceAttachment](../resources/referenceAttachment.md) 资源）。</span><span class="sxs-lookup"><span data-stu-id="94b4c-106">A link to a file ([referenceAttachment](../resources/referenceAttachment.md) resource).</span></span>

<span data-ttu-id="94b4c-107">所有这些类型的 attachment 资源均派生自 [attachment](../resources/attachment.md) 资源。</span><span class="sxs-lookup"><span data-stu-id="94b4c-107">All these types of attachment resources are derived from the [attachment](../resources/attachment.md) resource.</span></span> 

## <a name="permissions"></a><span data-ttu-id="94b4c-108">权限</span><span class="sxs-lookup"><span data-stu-id="94b4c-108">Permissions</span></span>
<span data-ttu-id="94b4c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="94b4c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="94b4c-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="94b4c-111">Permission type</span></span>      | <span data-ttu-id="94b4c-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="94b4c-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="94b4c-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="94b4c-113">Delegated (work or school account)</span></span> | <span data-ttu-id="94b4c-114">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="94b4c-114">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="94b4c-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="94b4c-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="94b4c-116">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="94b4c-116">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="94b4c-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="94b4c-117">Application</span></span> | <span data-ttu-id="94b4c-118">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="94b4c-118">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="94b4c-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="94b4c-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/messages/{id}/attachments
POST /users/{id | userPrincipalName}/messages/{id}/attachments
```
## <a name="request-headers"></a><span data-ttu-id="94b4c-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="94b4c-120">Request headers</span></span>
| <span data-ttu-id="94b4c-121">名称</span><span class="sxs-lookup"><span data-stu-id="94b4c-121">Name</span></span>       | <span data-ttu-id="94b4c-122">类型</span><span class="sxs-lookup"><span data-stu-id="94b4c-122">Type</span></span> | <span data-ttu-id="94b4c-123">说明</span><span class="sxs-lookup"><span data-stu-id="94b4c-123">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="94b4c-124">授权</span><span class="sxs-lookup"><span data-stu-id="94b4c-124">Authorization</span></span>  | <span data-ttu-id="94b4c-125">字符串</span><span class="sxs-lookup"><span data-stu-id="94b4c-125">string</span></span>  | <span data-ttu-id="94b4c-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="94b4c-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="94b4c-128">内容类型</span><span class="sxs-lookup"><span data-stu-id="94b4c-128">Content-Type</span></span> | <span data-ttu-id="94b4c-129">字符串</span><span class="sxs-lookup"><span data-stu-id="94b4c-129">string</span></span>  | <span data-ttu-id="94b4c-p103">实体正文中的数据性质。必需。</span><span class="sxs-lookup"><span data-stu-id="94b4c-p103">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="94b4c-132">请求正文</span><span class="sxs-lookup"><span data-stu-id="94b4c-132">Request body</span></span>
<span data-ttu-id="94b4c-133">在请求正文中，提供 [Attachment](../resources/attachment.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="94b4c-133">In the request body, supply a JSON representation of [Attachment](../resources/attachment.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="94b4c-134">响应</span><span class="sxs-lookup"><span data-stu-id="94b4c-134">Response</span></span>

<span data-ttu-id="94b4c-135">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [Attachment](../resources/attachment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="94b4c-135">If successful, this method returns `201 Created` response code and [Attachment](../resources/attachment.md) object in the response body.</span></span>

## <a name="example-file-attachment"></a><span data-ttu-id="94b4c-136">示例（文件附件）</span><span class="sxs-lookup"><span data-stu-id="94b4c-136">Example (File attachment)</span></span>
##### <a name="request"></a><span data-ttu-id="94b4c-137">请求</span><span class="sxs-lookup"><span data-stu-id="94b4c-137">Request</span></span>
<span data-ttu-id="94b4c-138">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="94b4c-138">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_file_attachment_from_eventmessage"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/messages/{id}/attachments
Content-type: application/json
Content-length: 142

{
  "@odata.type": "microsoft.graph.fileAttachment",
  "name": "name-value",
  "contentType": "contentType-value",
  "isInline": false,
  "contentLocation": "contentLocation-value",
  "contentBytes": "base64-contentBytes-value"
}
```

<span data-ttu-id="94b4c-139">在请求正文中，提供 [attachment](../resources/attachment.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="94b4c-139">In the request body, supply a JSON representation of [attachment](../resources/attachment.md) object.</span></span>

##### <a name="response"></a><span data-ttu-id="94b4c-140">响应</span><span class="sxs-lookup"><span data-stu-id="94b4c-140">Response</span></span>
<span data-ttu-id="94b4c-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="94b4c-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.attachment"
} -->
```http
HTTP/1.1 201 Created
```

## <a name="example-item-attachment"></a><span data-ttu-id="94b4c-144">示例（项目附件）</span><span class="sxs-lookup"><span data-stu-id="94b4c-144">Example (item attachment)</span></span>

##### <a name="request"></a><span data-ttu-id="94b4c-145">请求</span><span class="sxs-lookup"><span data-stu-id="94b4c-145">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "create_item_attachment_from_eventmessage"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/events/{id}/attachments
Content-type: application/json
Content-length: 100

{
  "@odata.type": "#Microsoft.OutlookServices.ItemAttachment",
  "name": "name-value",
  "item": "message or event entity"
}
```

##### <a name="response"></a><span data-ttu-id="94b4c-146">响应</span><span class="sxs-lookup"><span data-stu-id="94b4c-146">Response</span></span>
<span data-ttu-id="94b4c-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="94b4c-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.attachment"
} -->
```http
HTTP/1.1 201 Created
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
