# <a name="create-message"></a><span data-ttu-id="c1ea8-101">创建邮件</span><span class="sxs-lookup"><span data-stu-id="c1ea8-101">Create Message</span></span>

<span data-ttu-id="c1ea8-p101">使用此 API 创建新邮件的草稿。可以在任意文件夹中创建草稿，也可以在发送前更新草稿。若要将邮件保存到“草稿”文件夹，请使用 /messages 快捷方式。</span><span class="sxs-lookup"><span data-stu-id="c1ea8-p101">Use this API to create a draft of a new message. Drafts can be created in any folder and optionally updated before sending. To save to the Drafts folder, use the /messages shortcut.</span></span>

<span data-ttu-id="c1ea8-105">在同一个 **POST** 调用中创建草稿时，可以添加[附件](../resources/attachment.md)。</span><span class="sxs-lookup"><span data-stu-id="c1ea8-105">While creating the draft in the same **POST** call, you can include an [attachment](../resources/attachment.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="c1ea8-106">权限</span><span class="sxs-lookup"><span data-stu-id="c1ea8-106">Permissions</span></span>
<span data-ttu-id="c1ea8-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="c1ea8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="c1ea8-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="c1ea8-109">Permission type</span></span>      | <span data-ttu-id="c1ea8-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c1ea8-110">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="c1ea8-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c1ea8-111">Delegated (work or school account)</span></span> | <span data-ttu-id="c1ea8-112">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c1ea8-112">Mail.ReadWrite</span></span>    | 
|<span data-ttu-id="c1ea8-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c1ea8-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c1ea8-114">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c1ea8-114">Mail.ReadWrite</span></span>    | 
|<span data-ttu-id="c1ea8-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="c1ea8-115">Application</span></span> | <span data-ttu-id="c1ea8-116">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c1ea8-116">Mail.ReadWrite</span></span> | 

## <a name="http-request"></a><span data-ttu-id="c1ea8-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c1ea8-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/messages
POST /users/{id|userPrincipalName}/messages
POST /me/mailFolders/{id}/messages
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages
```
## <a name="request-headers"></a><span data-ttu-id="c1ea8-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="c1ea8-118">Request headers</span></span>
| <span data-ttu-id="c1ea8-119">标头</span><span class="sxs-lookup"><span data-stu-id="c1ea8-119">Header</span></span>       | <span data-ttu-id="c1ea8-120">值</span><span class="sxs-lookup"><span data-stu-id="c1ea8-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="c1ea8-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="c1ea8-121">Authorization</span></span>  | <span data-ttu-id="c1ea8-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="c1ea8-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="c1ea8-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c1ea8-124">Content-Type</span></span>  | <span data-ttu-id="c1ea8-125">application/json</span><span class="sxs-lookup"><span data-stu-id="c1ea8-125">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="c1ea8-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="c1ea8-126">Request body</span></span>
<span data-ttu-id="c1ea8-127">在请求正文中，提供 [Message](../resources/message.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c1ea8-127">In the request body, supply a JSON representation of [message](../resources/message.md) object.</span></span>

<span data-ttu-id="c1ea8-128">由于**邮件**资源支持[扩展](../../../concepts/extensibility_overview.md)因此可以使用 `POST` 操作，并在创建邮件时向其添加含有自己的数据的自定义属性。</span><span class="sxs-lookup"><span data-stu-id="c1ea8-128">Since the **message** resource supports [extensions](../../../concepts/extensibility_overview.md), you can use the `POST` operation and add custom properties with your own data to the message while creating it.</span></span>

## <a name="response"></a><span data-ttu-id="c1ea8-129">响应</span><span class="sxs-lookup"><span data-stu-id="c1ea8-129">Response</span></span>

<span data-ttu-id="c1ea8-130">如果成功，此方法在响应正文中返回 `201, Created` 响应代码和 [message](../resources/message.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="c1ea8-130">If successful, this method returns `201, Created` response code and [message](../resources/message.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c1ea8-131">示例</span><span class="sxs-lookup"><span data-stu-id="c1ea8-131">Example</span></span>
##### <a name="request-1"></a><span data-ttu-id="c1ea8-132">请求 1</span><span class="sxs-lookup"><span data-stu-id="c1ea8-132">Request 1</span></span>
<span data-ttu-id="c1ea8-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="c1ea8-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_message_from_user"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/messages
Content-type: application/json
Content-length: 248

{
  "receivedDateTime": "datetime-value",
  "sentDateTime": "datetime-value",
  "hasAttachments": true,
  "subject": "subject-value",
  "body": {
    "contentType": "",
    "content": "content-value"
  },
  "bodyPreview": "bodyPreview-value"
}
```
<span data-ttu-id="c1ea8-134">在请求正文中，提供 [Message](../resources/message.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c1ea8-134">In the request body, supply a JSON representation of [message](../resources/message.md) object.</span></span>
##### <a name="response-1"></a><span data-ttu-id="c1ea8-135">响应 1</span><span class="sxs-lookup"><span data-stu-id="c1ea8-135">Response 1</span></span>
<span data-ttu-id="c1ea8-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="c1ea8-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 248

{
  "receivedDateTime": "datetime-value",
  "sentDateTime": "datetime-value",
  "hasAttachments": true,
  "subject": "subject-value",
  "body": {
    "contentType": "",
    "content": "content-value"
  },
  "bodyPreview": "bodyPreview-value"
}
```

## <a name="see-also"></a><span data-ttu-id="c1ea8-139">另请参阅</span><span class="sxs-lookup"><span data-stu-id="c1ea8-139">See also</span></span>

- [<span data-ttu-id="c1ea8-140">使用扩展向资源添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="c1ea8-140">Add custom data to resources using extensions</span></span>](../../../concepts/extensibility_overview.md)
- [<span data-ttu-id="c1ea8-141">使用开放扩展向用户添加自定义数据（预览）</span><span class="sxs-lookup"><span data-stu-id="c1ea8-141">Add custom data to users using open extensions (preview)</span></span>](../../../concepts/extensibility_open_users.md)
<!--
- [Add custom data to groups using schema extensions (preview)](../../../concepts/extensibility_schema_groups.md)
-->


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create Message",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
