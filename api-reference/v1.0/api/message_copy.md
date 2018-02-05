# <a name="message-copy"></a><span data-ttu-id="f9dd2-101">message: copy</span><span class="sxs-lookup"><span data-stu-id="f9dd2-101">message: copy</span></span>

<span data-ttu-id="f9dd2-102">将邮件复制到文件夹。</span><span class="sxs-lookup"><span data-stu-id="f9dd2-102">Copy a message to a folder.</span></span>

## <a name="permissions"></a><span data-ttu-id="f9dd2-103">权限</span><span class="sxs-lookup"><span data-stu-id="f9dd2-103">Permissions</span></span>
<span data-ttu-id="f9dd2-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="f9dd2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="f9dd2-106">权限类型</span><span class="sxs-lookup"><span data-stu-id="f9dd2-106">Permission type</span></span>      | <span data-ttu-id="f9dd2-107">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f9dd2-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f9dd2-108">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f9dd2-108">Delegated (work or school account)</span></span> | <span data-ttu-id="f9dd2-109">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f9dd2-109">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="f9dd2-110">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f9dd2-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f9dd2-111">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f9dd2-111">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="f9dd2-112">应用程序</span><span class="sxs-lookup"><span data-stu-id="f9dd2-112">Application</span></span> | <span data-ttu-id="f9dd2-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f9dd2-113">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="f9dd2-114">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f9dd2-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/messages/{id}/copy
POST /users/{id | userPrincipalName}/messages/{id}/copy
POST /me/mailFolders/{id}/messages/{id}/copy
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/copy
```
## <a name="request-headers"></a><span data-ttu-id="f9dd2-115">请求标头</span><span class="sxs-lookup"><span data-stu-id="f9dd2-115">Request headers</span></span>
| <span data-ttu-id="f9dd2-116">名称</span><span class="sxs-lookup"><span data-stu-id="f9dd2-116">Name</span></span>       | <span data-ttu-id="f9dd2-117">类型</span><span class="sxs-lookup"><span data-stu-id="f9dd2-117">Type</span></span> | <span data-ttu-id="f9dd2-118">说明</span><span class="sxs-lookup"><span data-stu-id="f9dd2-118">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="f9dd2-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="f9dd2-119">Authorization</span></span>  | <span data-ttu-id="f9dd2-120">string</span><span class="sxs-lookup"><span data-stu-id="f9dd2-120">string</span></span>  | <span data-ttu-id="f9dd2-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="f9dd2-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="f9dd2-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f9dd2-123">Content-Type</span></span> | <span data-ttu-id="f9dd2-124">string</span><span class="sxs-lookup"><span data-stu-id="f9dd2-124">string</span></span>  | <span data-ttu-id="f9dd2-p103">实体正文中的数据性质。必需。</span><span class="sxs-lookup"><span data-stu-id="f9dd2-p103">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f9dd2-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="f9dd2-127">Request body</span></span>
<span data-ttu-id="f9dd2-128">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="f9dd2-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="f9dd2-129">参数</span><span class="sxs-lookup"><span data-stu-id="f9dd2-129">Parameter</span></span>    | <span data-ttu-id="f9dd2-130">类型</span><span class="sxs-lookup"><span data-stu-id="f9dd2-130">Type</span></span>   |<span data-ttu-id="f9dd2-131">说明</span><span class="sxs-lookup"><span data-stu-id="f9dd2-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f9dd2-132">destinationId</span><span class="sxs-lookup"><span data-stu-id="f9dd2-132">destinationId</span></span>|<span data-ttu-id="f9dd2-133">String</span><span class="sxs-lookup"><span data-stu-id="f9dd2-133">String</span></span>|<span data-ttu-id="f9dd2-134">目标文件夹 ID，或*收件箱*、*草稿箱*、*已发送邮件*或*已删除邮件*等已知文件夹名称。</span><span class="sxs-lookup"><span data-stu-id="f9dd2-134">The destination folder ID, or a well-known folder name such as *Inbox*, *Drafts*, *SentItems*, or *DeletedItems*.</span></span> <span data-ttu-id="f9dd2-135">有关受支持的已知文件夹名称的列表，请参阅 [mailFolder 资源类型](../resources/mailfolder.md)。</span><span class="sxs-lookup"><span data-stu-id="f9dd2-135">For a list of supported well-known folder names, see [mailFolder resource type](../resources/mailfolder.md).</span></span>|

## <a name="response"></a><span data-ttu-id="f9dd2-136">响应</span><span class="sxs-lookup"><span data-stu-id="f9dd2-136">Response</span></span>

<span data-ttu-id="f9dd2-137">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [Message](../resources/message.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="f9dd2-137">If successful, this method returns `201 Created` response code and [Message](../resources/message.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f9dd2-138">示例</span><span class="sxs-lookup"><span data-stu-id="f9dd2-138">Example</span></span>
<span data-ttu-id="f9dd2-139">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="f9dd2-139">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="f9dd2-140">请求</span><span class="sxs-lookup"><span data-stu-id="f9dd2-140">Request</span></span>
<span data-ttu-id="f9dd2-141">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="f9dd2-141">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "message_copy"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/messages/{id}/copy
Content-type: application/json
Content-length: 44

{
  "destinationId": "destinationId-value"
}
```

##### <a name="response"></a><span data-ttu-id="f9dd2-142">响应</span><span class="sxs-lookup"><span data-stu-id="f9dd2-142">Response</span></span>
<span data-ttu-id="f9dd2-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="f9dd2-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "message: copy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
