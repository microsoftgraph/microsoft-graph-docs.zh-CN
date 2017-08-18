# <a name="list-messages"></a><span data-ttu-id="e5a3a-101">List messages</span><span class="sxs-lookup"><span data-stu-id="e5a3a-101">List messages</span></span>

<span data-ttu-id="e5a3a-102">获取登录用户的邮箱（包括“已删除邮件”和“待筛选邮件”文件夹）中的邮件。</span><span class="sxs-lookup"><span data-stu-id="e5a3a-102">Get the messages in the signed-in user's mailbox (including the Deleted Items and Clutter folders).</span></span>

<span data-ttu-id="e5a3a-103">目前，此操作返回纯 HTML 格式的邮件正文。</span><span class="sxs-lookup"><span data-stu-id="e5a3a-103">Currently, this operation returns message bodies in only HTML format.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e5a3a-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="e5a3a-104">Prerequisites</span></span>
<span data-ttu-id="e5a3a-105">要执行此 API，需要以下**范围**之一：*Mail.Read；Mail.ReadWrite*</span><span class="sxs-lookup"><span data-stu-id="e5a3a-105">One of the following scopes is required to execute this API: Mail.Read; Mail.ReadWrite</span></span>
## <a name="http-request"></a><span data-ttu-id="e5a3a-106">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e5a3a-106">HTTP request</span></span>

<span data-ttu-id="e5a3a-107">若要获取用户邮箱中的所有邮件，请执行以下操作：</span><span class="sxs-lookup"><span data-stu-id="e5a3a-107">To get all the messages in a user's mailbox:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/messages
GET /users/{id | userPrincipalName}/messages
```

<span data-ttu-id="e5a3a-108">若要获取用户邮箱中特定文件夹中的邮件，请执行以下操作：</span><span class="sxs-lookup"><span data-stu-id="e5a3a-108">To get messages in a specific folder in the user's mailbox:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/{id}/messages
GET /users/{id | userPrincipalName}/mailFolders/{id}/messages
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e5a3a-109">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="e5a3a-109">Optional query parameters</span></span>
<span data-ttu-id="e5a3a-110">此方法支持 [OData 查询参数](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="e5a3a-110">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="e5a3a-111">请求标头</span><span class="sxs-lookup"><span data-stu-id="e5a3a-111">Request headers</span></span>
| <span data-ttu-id="e5a3a-112">标头</span><span class="sxs-lookup"><span data-stu-id="e5a3a-112">Header</span></span>       | <span data-ttu-id="e5a3a-113">值</span><span class="sxs-lookup"><span data-stu-id="e5a3a-113">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="e5a3a-114">Authorization</span><span class="sxs-lookup"><span data-stu-id="e5a3a-114">Authorization</span></span>  | <span data-ttu-id="e5a3a-p101">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="e5a3a-p101">Bearer {token}. Required.</span></span>  |
 

## <a name="request-body"></a><span data-ttu-id="e5a3a-117">请求正文</span><span class="sxs-lookup"><span data-stu-id="e5a3a-117">Request body</span></span>
<span data-ttu-id="e5a3a-118">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="e5a3a-118">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e5a3a-119">响应</span><span class="sxs-lookup"><span data-stu-id="e5a3a-119">Response</span></span>

<span data-ttu-id="e5a3a-120">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和一组 [Message](../resources/message.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="e5a3a-120">If successful, this method returns a `200 OK` response code and collection of [Message](../resources/message.md) objects in the response body.</span></span>

<span data-ttu-id="e5a3a-121">此请求的默认页面大小为 10 封邮件。</span><span class="sxs-lookup"><span data-stu-id="e5a3a-121">The default page size for this request is 10 messages.</span></span>

## <a name="example"></a><span data-ttu-id="e5a3a-122">示例</span><span class="sxs-lookup"><span data-stu-id="e5a3a-122">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e5a3a-123">请求</span><span class="sxs-lookup"><span data-stu-id="e5a3a-123">Request</span></span>
<span data-ttu-id="e5a3a-124">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="e5a3a-124">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_messages"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/messages
```
##### <a name="response"></a><span data-ttu-id="e5a3a-125">响应</span><span class="sxs-lookup"><span data-stu-id="e5a3a-125">Response</span></span>
<span data-ttu-id="e5a3a-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="e5a3a-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
