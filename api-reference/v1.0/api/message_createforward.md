# <a name="message-createforward"></a><span data-ttu-id="a8a08-101">message: createForward</span><span class="sxs-lookup"><span data-stu-id="a8a08-101">message: createForward</span></span>

<span data-ttu-id="a8a08-p101">创建转发邮件的草稿。然后，你可以 [更新](../api/message_update.md) 或 [发送](../api/message_send.md) 草稿。</span><span class="sxs-lookup"><span data-stu-id="a8a08-p101">Create a draft of the Forward message. You can then [update](../api/message_update.md) or [send](../api/message_send.md) the draft.</span></span>

## <a name="permissions"></a><span data-ttu-id="a8a08-104">权限</span><span class="sxs-lookup"><span data-stu-id="a8a08-104">Permissions</span></span>
<span data-ttu-id="a8a08-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="a8a08-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="a8a08-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="a8a08-107">Permission type</span></span>      | <span data-ttu-id="a8a08-108">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a8a08-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a8a08-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a8a08-109">Delegated (work or school account)</span></span> | <span data-ttu-id="a8a08-110">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a8a08-110">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="a8a08-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a8a08-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a8a08-112">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a8a08-112">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="a8a08-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="a8a08-113">Application</span></span> | <span data-ttu-id="a8a08-114">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a8a08-114">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="a8a08-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a8a08-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/messages/{id}/createForward
POST /users/{id | userPrincipalName}/messages/{id}/createForward
POST /me/mailFolders/{id}/messages/{id}/createForward
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/createForward
```
## <a name="request-headers"></a><span data-ttu-id="a8a08-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="a8a08-116">Request headers</span></span>
| <span data-ttu-id="a8a08-117">名称</span><span class="sxs-lookup"><span data-stu-id="a8a08-117">Name</span></span>       | <span data-ttu-id="a8a08-118">类型</span><span class="sxs-lookup"><span data-stu-id="a8a08-118">Type</span></span> | <span data-ttu-id="a8a08-119">说明</span><span class="sxs-lookup"><span data-stu-id="a8a08-119">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="a8a08-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="a8a08-120">Authorization</span></span>  | <span data-ttu-id="a8a08-121">string</span><span class="sxs-lookup"><span data-stu-id="a8a08-121">string</span></span>  | <span data-ttu-id="a8a08-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="a8a08-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="a8a08-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a8a08-124">Content-Type</span></span> | <span data-ttu-id="a8a08-125">string</span><span class="sxs-lookup"><span data-stu-id="a8a08-125">string</span></span>  | <span data-ttu-id="a8a08-p104">实体正文中的数据性质。必需。</span><span class="sxs-lookup"><span data-stu-id="a8a08-p104">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a8a08-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="a8a08-128">Request body</span></span>

## <a name="response"></a><span data-ttu-id="a8a08-129">响应</span><span class="sxs-lookup"><span data-stu-id="a8a08-129">Response</span></span>

<span data-ttu-id="a8a08-130">如果成功，此方法在响应正文中返回 `201, Created` 响应代码和 [Message](../resources/message.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="a8a08-130">If successful, this method returns `201, Created` response code and [Message](../resources/message.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a8a08-131">示例</span><span class="sxs-lookup"><span data-stu-id="a8a08-131">Example</span></span>
<span data-ttu-id="a8a08-132">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="a8a08-132">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="a8a08-133">请求</span><span class="sxs-lookup"><span data-stu-id="a8a08-133">Request</span></span>
<span data-ttu-id="a8a08-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="a8a08-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "message_createforward"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/messages/{id}/createForward
Content-type: application/json
Content-length: 248

{
  "comment": "Comment-value",
  "toRecipients": [
    {
      "emailAddress": {
        "address": "address-value"
      }
    },
    {
      "emailAddress": {
        "address": "address-value"
      }
    }
  ]
}
```

##### <a name="response"></a><span data-ttu-id="a8a08-135">响应</span><span class="sxs-lookup"><span data-stu-id="a8a08-135">Response</span></span>
<span data-ttu-id="a8a08-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="a8a08-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "message: createForward",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
