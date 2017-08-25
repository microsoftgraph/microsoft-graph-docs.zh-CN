# <a name="list-messages"></a><span data-ttu-id="b9e23-101">List messages</span><span class="sxs-lookup"><span data-stu-id="b9e23-101">List messages</span></span>

<span data-ttu-id="b9e23-102">获取登录用户的邮箱（包括“已删除邮件”和“待筛选邮件”文件夹）中的邮件。</span><span class="sxs-lookup"><span data-stu-id="b9e23-102">Get the messages in the signed-in user's mailbox (including the Deleted Items and Clutter folders).</span></span>

<span data-ttu-id="b9e23-103">目前，此操作返回纯 HTML 格式的邮件正文。</span><span class="sxs-lookup"><span data-stu-id="b9e23-103">Currently, this operation returns message bodies in only HTML format.</span></span>

## <a name="permissions"></a><span data-ttu-id="b9e23-104">权限</span><span class="sxs-lookup"><span data-stu-id="b9e23-104">Permissions</span></span>
<span data-ttu-id="b9e23-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="b9e23-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="b9e23-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="b9e23-107">Permission type</span></span>      | <span data-ttu-id="b9e23-108">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b9e23-108">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="b9e23-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b9e23-109">Delegated (work or school account)</span></span> | <span data-ttu-id="b9e23-110">Mail.Read、Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b9e23-110">Mail.Read, Mail.ReadWrite</span></span>    | 
|<span data-ttu-id="b9e23-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b9e23-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b9e23-112">Mail.Read、Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b9e23-112">Mail.Read, Mail.ReadWrite</span></span>    | 
|<span data-ttu-id="b9e23-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="b9e23-113">Application</span></span> | <span data-ttu-id="b9e23-114">Mail.Read、Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b9e23-114">Mail.Read, Mail.ReadWrite</span></span> | 

## <a name="http-request"></a><span data-ttu-id="b9e23-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b9e23-115">HTTP request</span></span>

<span data-ttu-id="b9e23-116">若要获取用户邮箱中的所有邮件，请执行以下操作：</span><span class="sxs-lookup"><span data-stu-id="b9e23-116">To get all the messages in a user's mailbox:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/messages
GET /users/{id | userPrincipalName}/messages
```

<span data-ttu-id="b9e23-117">若要获取用户邮箱中特定文件夹中的邮件，请执行以下操作：</span><span class="sxs-lookup"><span data-stu-id="b9e23-117">To get messages in a specific folder in the user's mailbox:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/{id}/messages
GET /users/{id | userPrincipalName}/mailFolders/{id}/messages
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b9e23-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="b9e23-118">Optional query parameters</span></span>
<span data-ttu-id="b9e23-119">此方法支持 [OData 查询参数](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="b9e23-119">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="b9e23-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="b9e23-120">Request headers</span></span>
| <span data-ttu-id="b9e23-121">标头</span><span class="sxs-lookup"><span data-stu-id="b9e23-121">Header</span></span>       | <span data-ttu-id="b9e23-122">值</span><span class="sxs-lookup"><span data-stu-id="b9e23-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="b9e23-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="b9e23-123">Authorization</span></span>  | <span data-ttu-id="b9e23-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="b9e23-p102">Bearer {token}. Required.</span></span>  |
 

## <a name="request-body"></a><span data-ttu-id="b9e23-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="b9e23-126">Request body</span></span>
<span data-ttu-id="b9e23-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="b9e23-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b9e23-128">响应</span><span class="sxs-lookup"><span data-stu-id="b9e23-128">Response</span></span>

<span data-ttu-id="b9e23-129">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和一组 [Message](../resources/message.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="b9e23-129">If successful, this method returns a `200 OK` response code and collection of [Message](../resources/message.md) objects in the response body.</span></span>

<span data-ttu-id="b9e23-130">此请求的默认页面大小为 10 封邮件。</span><span class="sxs-lookup"><span data-stu-id="b9e23-130">The default page size for this request is 10 messages.</span></span>

## <a name="example"></a><span data-ttu-id="b9e23-131">示例</span><span class="sxs-lookup"><span data-stu-id="b9e23-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b9e23-132">请求</span><span class="sxs-lookup"><span data-stu-id="b9e23-132">Request</span></span>
<span data-ttu-id="b9e23-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="b9e23-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_messages"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/messages
```
##### <a name="response"></a><span data-ttu-id="b9e23-134">响应</span><span class="sxs-lookup"><span data-stu-id="b9e23-134">Response</span></span>
<span data-ttu-id="b9e23-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="b9e23-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 317

{
  "value": [
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
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List messages",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
