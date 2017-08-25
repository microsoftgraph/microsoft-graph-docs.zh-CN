# <a name="message-move"></a><span data-ttu-id="19a2f-101">message: move</span><span class="sxs-lookup"><span data-stu-id="19a2f-101">message: move</span></span>

<span data-ttu-id="19a2f-p101">将邮件移动到文件夹。该操作会在目标文件夹中创建邮件的新副本。</span><span class="sxs-lookup"><span data-stu-id="19a2f-p101">Move a message to a folder. This creates a new copy of the message in the destination folder.</span></span>

## <a name="permissions"></a><span data-ttu-id="19a2f-104">权限</span><span class="sxs-lookup"><span data-stu-id="19a2f-104">Permissions</span></span>
<span data-ttu-id="19a2f-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="19a2f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="19a2f-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="19a2f-107">Permission type</span></span>      | <span data-ttu-id="19a2f-108">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="19a2f-108">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="19a2f-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="19a2f-109">Delegated (work or school account)</span></span> | <span data-ttu-id="19a2f-110">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="19a2f-110">Mail.ReadWrite</span></span>    | 
|<span data-ttu-id="19a2f-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="19a2f-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="19a2f-112">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="19a2f-112">Mail.ReadWrite</span></span>    | 
|<span data-ttu-id="19a2f-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="19a2f-113">Application</span></span> | <span data-ttu-id="19a2f-114">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="19a2f-114">Mail.ReadWrite</span></span> | 

## <a name="http-request"></a><span data-ttu-id="19a2f-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="19a2f-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/messages/{id}/move
POST /users/{id | userPrincipalName}/messages/{id}/move
POST /me/mailFolders/{id}/messages/{id}/move
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/move
```
## <a name="request-headers"></a><span data-ttu-id="19a2f-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="19a2f-116">Request headers</span></span>
| <span data-ttu-id="19a2f-117">名称</span><span class="sxs-lookup"><span data-stu-id="19a2f-117">Name</span></span>       | <span data-ttu-id="19a2f-118">类型</span><span class="sxs-lookup"><span data-stu-id="19a2f-118">Type</span></span> | <span data-ttu-id="19a2f-119">说明</span><span class="sxs-lookup"><span data-stu-id="19a2f-119">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="19a2f-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="19a2f-120">Authorization</span></span>  | <span data-ttu-id="19a2f-121">string</span><span class="sxs-lookup"><span data-stu-id="19a2f-121">string</span></span>  | <span data-ttu-id="19a2f-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="19a2f-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="19a2f-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="19a2f-124">Content-Type</span></span> | <span data-ttu-id="19a2f-125">string</span><span class="sxs-lookup"><span data-stu-id="19a2f-125">string</span></span>  | <span data-ttu-id="19a2f-p104">实体正文中的数据性质。必需。</span><span class="sxs-lookup"><span data-stu-id="19a2f-p104">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="19a2f-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="19a2f-128">Request body</span></span>
<span data-ttu-id="19a2f-129">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="19a2f-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="19a2f-130">参数</span><span class="sxs-lookup"><span data-stu-id="19a2f-130">Parameter</span></span>    | <span data-ttu-id="19a2f-131">类型</span><span class="sxs-lookup"><span data-stu-id="19a2f-131">Type</span></span>   |<span data-ttu-id="19a2f-132">说明</span><span class="sxs-lookup"><span data-stu-id="19a2f-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="19a2f-133">DestinationId</span><span class="sxs-lookup"><span data-stu-id="19a2f-133">DestinationId</span></span>|<span data-ttu-id="19a2f-134">String</span><span class="sxs-lookup"><span data-stu-id="19a2f-134">String</span></span>|<span data-ttu-id="19a2f-135">目标文件夹 ID，或者 `Inbox`、`Drafts`、`SentItems` 或 `DeletedItems` 已知文件夹的名称。</span><span class="sxs-lookup"><span data-stu-id="19a2f-135">The destination folder ID, or the `Inbox`, `Drafts`, `SentItems`, or `DeletedItems` well-known folder name.</span></span>|

## <a name="response"></a><span data-ttu-id="19a2f-136">响应</span><span class="sxs-lookup"><span data-stu-id="19a2f-136">Response</span></span>

<span data-ttu-id="19a2f-137">如果成功，此方法在响应正文中返回 `201, Created` 响应代码和 [Message](../resources/message.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="19a2f-137">If successful, this method returns `201, Created` response code and [Message](../resources/message.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="19a2f-138">示例</span><span class="sxs-lookup"><span data-stu-id="19a2f-138">Example</span></span>
<span data-ttu-id="19a2f-139">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="19a2f-139">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="19a2f-140">请求</span><span class="sxs-lookup"><span data-stu-id="19a2f-140">Request</span></span>
<span data-ttu-id="19a2f-141">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="19a2f-141">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="19a2f-142">响应</span><span class="sxs-lookup"><span data-stu-id="19a2f-142">Response</span></span>
<span data-ttu-id="19a2f-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="19a2f-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
