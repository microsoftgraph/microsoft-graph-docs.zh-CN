# <a name="get-message"></a><span data-ttu-id="014b4-101">获取邮件</span><span class="sxs-lookup"><span data-stu-id="014b4-101">Get message</span></span>

<span data-ttu-id="014b4-102">检索[邮件](../resources/message.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="014b4-102">Retrieve the properties and relationships of a [message](../resources/message.md) object.</span></span>

<span data-ttu-id="014b4-103">由于**邮件**资源支持[扩展](../../../concepts/extensibility_overview.md)，因此也可使用 `GET` 操作获取**邮件**实例中的自定义属性和扩展数据。</span><span class="sxs-lookup"><span data-stu-id="014b4-103">Since the **message** resource supports [extensions](../../../concepts/extensibility_overview.md), you can also use the `GET` operation to get custom properties and extension data in a **message** instance.</span></span>

<span data-ttu-id="014b4-104">目前，此操作返回纯 HTML 格式的邮件正文。</span><span class="sxs-lookup"><span data-stu-id="014b4-104">Currently, this operation returns message bodies in only HTML format.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="014b4-105">先决条件</span><span class="sxs-lookup"><span data-stu-id="014b4-105">Prerequisites</span></span>
<span data-ttu-id="014b4-106">要执行此 API，需要以下**范围**之一：*Mail.Read*</span><span class="sxs-lookup"><span data-stu-id="014b4-106">One of the following **scopes** is required to execute this API: *Mail.Read*</span></span>  
## <a name="http-request"></a><span data-ttu-id="014b4-107">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="014b4-107">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/messages/{id}
GET /users/{id | userPrincipalName}/messages/{id}
GET /me/mailFolders/{id}/messages/{id}
GET /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="014b4-108">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="014b4-108">Optional query parameters</span></span>
<span data-ttu-id="014b4-109">此方法支持 [OData 查询参数](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="014b4-109">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="014b4-110">请求标头</span><span class="sxs-lookup"><span data-stu-id="014b4-110">Request headers</span></span>
| <span data-ttu-id="014b4-111">名称</span><span class="sxs-lookup"><span data-stu-id="014b4-111">Name</span></span>       | <span data-ttu-id="014b4-112">类型</span><span class="sxs-lookup"><span data-stu-id="014b4-112">Type</span></span> | <span data-ttu-id="014b4-113">说明</span><span class="sxs-lookup"><span data-stu-id="014b4-113">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="014b4-114">Authorization</span><span class="sxs-lookup"><span data-stu-id="014b4-114">Authorization</span></span>  | <span data-ttu-id="014b4-115">string</span><span class="sxs-lookup"><span data-stu-id="014b4-115">string</span></span>  | <span data-ttu-id="014b4-p101">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="014b4-p101">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="014b4-118">请求正文</span><span class="sxs-lookup"><span data-stu-id="014b4-118">Request body</span></span>
<span data-ttu-id="014b4-119">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="014b4-119">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="014b4-120">响应</span><span class="sxs-lookup"><span data-stu-id="014b4-120">Response</span></span>

<span data-ttu-id="014b4-121">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [message](../resources/message.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="014b4-121">If successful, this method returns a `200 OK` response code and [message](../resources/message.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="014b4-122">示例</span><span class="sxs-lookup"><span data-stu-id="014b4-122">Example</span></span>
##### <a name="request"></a><span data-ttu-id="014b4-123">请求</span><span class="sxs-lookup"><span data-stu-id="014b4-123">Request</span></span>
<span data-ttu-id="014b4-124">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="014b4-124">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_message"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/messages/{id}
```
##### <a name="response"></a><span data-ttu-id="014b4-125">响应</span><span class="sxs-lookup"><span data-stu-id="014b4-125">Response</span></span>
<span data-ttu-id="014b4-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="014b4-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
    "contentType": "html",
    "content": "content-value"
  },
  "bodyPreview": "bodyPreview-value"
}
```

## <a name="see-also"></a><span data-ttu-id="014b4-129">另请参阅</span><span class="sxs-lookup"><span data-stu-id="014b4-129">See also</span></span>

- [<span data-ttu-id="014b4-130">使用扩展向资源添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="014b4-130">Add custom data to resources using extensions</span></span>](../../../concepts/extensibility_overview.md)
- [<span data-ttu-id="014b4-131">使用开放扩展向用户添加自定义数据（预览）</span><span class="sxs-lookup"><span data-stu-id="014b4-131">Add custom data to users using open extensions (preview)</span></span>](../../../concepts/extensibility_open_users.md)
<!--
- [Add custom data to groups using schema extensions (preview)](../../../concepts/extensibility_schema_groups.md)
-->


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get message",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
