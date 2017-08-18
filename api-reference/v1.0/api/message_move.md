# <a name="message-move"></a><span data-ttu-id="2203e-101">message: move</span><span class="sxs-lookup"><span data-stu-id="2203e-101">message: move</span></span>

<span data-ttu-id="2203e-p101">将邮件移动到文件夹。该操作会在目标文件夹中创建邮件的新副本。</span><span class="sxs-lookup"><span data-stu-id="2203e-p101">Move a message to a folder. This creates a new copy of the message in the destination folder.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2203e-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="2203e-104">Prerequisites</span></span>
<span data-ttu-id="2203e-105">要执行此 API，需要以下**范围**之一：*Mail.ReadWrite*</span><span class="sxs-lookup"><span data-stu-id="2203e-105">One of the following **scopes** is required to execute this API: *Mail.ReadWrite*</span></span>
## <a name="http-request"></a><span data-ttu-id="2203e-106">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2203e-106">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/messages/{id}/move
POST /users/{id | userPrincipalName}/messages/{id}/move
POST /me/mailFolders/{id}/messages/{id}/move
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/move
```
## <a name="request-headers"></a><span data-ttu-id="2203e-107">请求标头</span><span class="sxs-lookup"><span data-stu-id="2203e-107">Request headers</span></span>
| <span data-ttu-id="2203e-108">名称</span><span class="sxs-lookup"><span data-stu-id="2203e-108">Name</span></span>       | <span data-ttu-id="2203e-109">类型</span><span class="sxs-lookup"><span data-stu-id="2203e-109">Type</span></span> | <span data-ttu-id="2203e-110">说明</span><span class="sxs-lookup"><span data-stu-id="2203e-110">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="2203e-111">Authorization</span><span class="sxs-lookup"><span data-stu-id="2203e-111">Authorization</span></span>  | <span data-ttu-id="2203e-112">string</span><span class="sxs-lookup"><span data-stu-id="2203e-112">string</span></span>  | <span data-ttu-id="2203e-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="2203e-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="2203e-115">Content-Type</span><span class="sxs-lookup"><span data-stu-id="2203e-115">Content-Type</span></span> | <span data-ttu-id="2203e-116">string</span><span class="sxs-lookup"><span data-stu-id="2203e-116">string</span></span>  | <span data-ttu-id="2203e-p103">实体正文中的数据性质。必需。</span><span class="sxs-lookup"><span data-stu-id="2203e-p103">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2203e-119">请求正文</span><span class="sxs-lookup"><span data-stu-id="2203e-119">Request body</span></span>
<span data-ttu-id="2203e-120">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="2203e-120">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="2203e-121">参数</span><span class="sxs-lookup"><span data-stu-id="2203e-121">Parameter</span></span>    | <span data-ttu-id="2203e-122">类型</span><span class="sxs-lookup"><span data-stu-id="2203e-122">Type</span></span>   |<span data-ttu-id="2203e-123">说明</span><span class="sxs-lookup"><span data-stu-id="2203e-123">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2203e-124">DestinationId</span><span class="sxs-lookup"><span data-stu-id="2203e-124">DestinationId</span></span>|<span data-ttu-id="2203e-125">String</span><span class="sxs-lookup"><span data-stu-id="2203e-125">String</span></span>|<span data-ttu-id="2203e-126">目标文件夹 ID，或者 `Inbox`、`Drafts`、`SentItems` 或 `DeletedItems` 已知文件夹的名称。</span><span class="sxs-lookup"><span data-stu-id="2203e-126">The destination folder ID, or the `Inbox`, `Drafts`, `SentItems`, or `DeletedItems` well-known folder name.</span></span>|

## <a name="response"></a><span data-ttu-id="2203e-127">响应</span><span class="sxs-lookup"><span data-stu-id="2203e-127">Response</span></span>

<span data-ttu-id="2203e-128">如果成功，此方法在响应正文中返回 `201, Created` 响应代码和 [Message](../resources/message.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="2203e-128">If successful, this method returns `201, Created` response code and [message](../resources/message.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2203e-129">示例</span><span class="sxs-lookup"><span data-stu-id="2203e-129">Example</span></span>
<span data-ttu-id="2203e-130">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="2203e-130">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="2203e-131">请求</span><span class="sxs-lookup"><span data-stu-id="2203e-131">Request</span></span>
<span data-ttu-id="2203e-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="2203e-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "message_move"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/messages/{id}/move
Content-type: application/json
Content-length: 44

{
  "DestinationId": "destinationId-value"
}
```

##### <a name="response"></a><span data-ttu-id="2203e-133">响应</span><span class="sxs-lookup"><span data-stu-id="2203e-133">Response</span></span>
<span data-ttu-id="2203e-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="2203e-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message"
} -->
```http
HTTP/1.1 200 OK
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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "message: move",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
