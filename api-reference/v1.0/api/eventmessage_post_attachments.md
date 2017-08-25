# <a name="add-attachment"></a><span data-ttu-id="d36ea-101">Add attachment</span><span class="sxs-lookup"><span data-stu-id="d36ea-101">Add attachment</span></span>

<span data-ttu-id="d36ea-102">使用此 API 新建附件。</span><span class="sxs-lookup"><span data-stu-id="d36ea-102">Use this API to create a new Attachment.</span></span>
## <a name="permissions"></a><span data-ttu-id="d36ea-103">权限</span><span class="sxs-lookup"><span data-stu-id="d36ea-103">Permissions</span></span>
<span data-ttu-id="d36ea-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="d36ea-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="d36ea-106">权限类型</span><span class="sxs-lookup"><span data-stu-id="d36ea-106">Permission type</span></span>      | <span data-ttu-id="d36ea-107">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d36ea-107">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="d36ea-108">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d36ea-108">Delegated (work or school account)</span></span> | <span data-ttu-id="d36ea-109">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d36ea-109">Mail.ReadWrite</span></span>    | 
|<span data-ttu-id="d36ea-110">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d36ea-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d36ea-111">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d36ea-111">Mail.ReadWrite</span></span>    | 
|<span data-ttu-id="d36ea-112">应用程序</span><span class="sxs-lookup"><span data-stu-id="d36ea-112">Application</span></span> | <span data-ttu-id="d36ea-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d36ea-113">Mail.ReadWrite</span></span> | 

## <a name="http-request"></a><span data-ttu-id="d36ea-114">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d36ea-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/messages/{id}/attachments
POST /users/{id | userPrincipalName}/messages/{id}/attachments
```
## <a name="request-headers"></a><span data-ttu-id="d36ea-115">请求标头</span><span class="sxs-lookup"><span data-stu-id="d36ea-115">Request headers</span></span>
| <span data-ttu-id="d36ea-116">名称</span><span class="sxs-lookup"><span data-stu-id="d36ea-116">Name</span></span>       | <span data-ttu-id="d36ea-117">类型</span><span class="sxs-lookup"><span data-stu-id="d36ea-117">Type</span></span> | <span data-ttu-id="d36ea-118">说明</span><span class="sxs-lookup"><span data-stu-id="d36ea-118">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="d36ea-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="d36ea-119">Authorization</span></span>  | <span data-ttu-id="d36ea-120">string</span><span class="sxs-lookup"><span data-stu-id="d36ea-120">string</span></span>  | <span data-ttu-id="d36ea-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="d36ea-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="d36ea-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d36ea-123">Content-Type</span></span> | <span data-ttu-id="d36ea-124">string</span><span class="sxs-lookup"><span data-stu-id="d36ea-124">string</span></span>  | <span data-ttu-id="d36ea-p103">实体正文中的数据性质。必需。</span><span class="sxs-lookup"><span data-stu-id="d36ea-p103">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d36ea-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="d36ea-127">Request body</span></span>
<span data-ttu-id="d36ea-128">在请求正文中，提供 [Attachment](../resources/attachment.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d36ea-128">In the request body, supply a JSON representation of [Attachment](../resources/attachment.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="d36ea-129">响应</span><span class="sxs-lookup"><span data-stu-id="d36ea-129">Response</span></span>

<span data-ttu-id="d36ea-130">如果成功，此方法在响应正文中返回 `201, Created` 响应代码和 [Attachment](../resources/attachment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="d36ea-130">If successful, this method returns `201, Created` response code and [Attachment](../resources/attachment.md) object in the response body.</span></span>

## <a name="example-file-attachment"></a><span data-ttu-id="d36ea-131">示例（文件附件）</span><span class="sxs-lookup"><span data-stu-id="d36ea-131">Example (File attachment)</span></span>
##### <a name="request"></a><span data-ttu-id="d36ea-132">请求</span><span class="sxs-lookup"><span data-stu-id="d36ea-132">Request</span></span>
<span data-ttu-id="d36ea-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="d36ea-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_file_attachment_from_eventmessage"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/messages/{id}/attachments
Content-type: application/json
Content-length: 142

{
  "@odata.type": "#Microsoft.OutlookServices.FileAttachment",
  "name": "name-value",
  "contentType": "contentType-value",
  "isInline": false,
  "contentLocation": "contentLocation-value",
  "contentBytes": "contentBytes-value"
}
```

<span data-ttu-id="d36ea-134">在请求正文中，提供 [attachment](../resources/attachment.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d36ea-134">In the request body, supply a JSON representation of [attachment](../resources/attachment.md) object.</span></span>

##### <a name="response"></a><span data-ttu-id="d36ea-135">响应</span><span class="sxs-lookup"><span data-stu-id="d36ea-135">Response</span></span>
<span data-ttu-id="d36ea-p104">下面是一个响应示例。注意：为简洁起见，可能会截断此处展示的响应对象。实际调用会返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="d36ea-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.attachment"
} -->
```http
HTTP/1.1 201 Created
```

## <a name="example-item-attachment"></a><span data-ttu-id="d36ea-139">示例（项目附件）</span><span class="sxs-lookup"><span data-stu-id="d36ea-139">Example (item attachment)</span></span>

##### <a name="request"></a><span data-ttu-id="d36ea-140">请求</span><span class="sxs-lookup"><span data-stu-id="d36ea-140">Request</span></span>
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

##### <a name="response"></a><span data-ttu-id="d36ea-141">响应</span><span class="sxs-lookup"><span data-stu-id="d36ea-141">Response</span></span>
<span data-ttu-id="d36ea-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="d36ea-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
