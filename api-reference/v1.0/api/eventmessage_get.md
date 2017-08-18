# <a name="get-eventmessage"></a><span data-ttu-id="d85f0-101">获取 eventMessage</span><span class="sxs-lookup"><span data-stu-id="d85f0-101">Get eventMessage</span></span>

<span data-ttu-id="d85f0-102">检索 [eventMessage](../resources/eventmessage.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="d85f0-102">Retrieve the properties and relationships of [eventMessage](../resources/eventmessage.md) object.</span></span>

<span data-ttu-id="d85f0-103">目前，此操作返回纯 HTML 格式的事件消息正文。</span><span class="sxs-lookup"><span data-stu-id="d85f0-103">Currently, this operation returns event message bodies in only HTML format.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d85f0-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="d85f0-104">Prerequisites</span></span>
<span data-ttu-id="d85f0-105">要执行此 API，需要以下**范围**之一：*Mail.Read*</span><span class="sxs-lookup"><span data-stu-id="d85f0-105">One of the following **scopes** is required to execute this API: *Mail.Read*</span></span>
## <a name="http-request"></a><span data-ttu-id="d85f0-106">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d85f0-106">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/messages/{id}
GET /users/{id | userPrincipalName}/messages/{id}

GET /me/mailFolders/{id}/messages/{id}
GET /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="d85f0-107">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="d85f0-107">Optional query parameters</span></span>
<span data-ttu-id="d85f0-108">此方法支持 [OData 查询参数](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="d85f0-108">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="d85f0-109">请求标头</span><span class="sxs-lookup"><span data-stu-id="d85f0-109">Request headers</span></span>
| <span data-ttu-id="d85f0-110">名称</span><span class="sxs-lookup"><span data-stu-id="d85f0-110">Name</span></span>       | <span data-ttu-id="d85f0-111">类型</span><span class="sxs-lookup"><span data-stu-id="d85f0-111">Type</span></span> | <span data-ttu-id="d85f0-112">说明</span><span class="sxs-lookup"><span data-stu-id="d85f0-112">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="d85f0-113">Authorization</span><span class="sxs-lookup"><span data-stu-id="d85f0-113">Authorization</span></span>  | <span data-ttu-id="d85f0-114">string</span><span class="sxs-lookup"><span data-stu-id="d85f0-114">string</span></span>  | <span data-ttu-id="d85f0-p101">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="d85f0-p101">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d85f0-117">请求正文</span><span class="sxs-lookup"><span data-stu-id="d85f0-117">Request body</span></span>
<span data-ttu-id="d85f0-118">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="d85f0-118">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d85f0-119">响应</span><span class="sxs-lookup"><span data-stu-id="d85f0-119">Response</span></span>

<span data-ttu-id="d85f0-120">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [eventMessage](../resources/eventmessage.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="d85f0-120">If successful, this method returns a `200 OK` response code and [eventMessage](../resources/eventmessage.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="d85f0-121">示例</span><span class="sxs-lookup"><span data-stu-id="d85f0-121">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d85f0-122">请求</span><span class="sxs-lookup"><span data-stu-id="d85f0-122">Request</span></span>
<span data-ttu-id="d85f0-123">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="d85f0-123">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_eventmessage"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/messages/{id}
```
##### <a name="response"></a><span data-ttu-id="d85f0-124">响应</span><span class="sxs-lookup"><span data-stu-id="d85f0-124">Response</span></span>
<span data-ttu-id="d85f0-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="d85f0-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.eventmessage"
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
  "bodyPreview": "bodyPreview-value",
  "meetingMessageType": "meetingMessageType-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get eventMessage",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
