# <a name="get-post"></a><span data-ttu-id="6c2a9-101">获取帖子</span><span class="sxs-lookup"><span data-stu-id="6c2a9-101">Get post</span></span>

<span data-ttu-id="6c2a9-p101">获取指定线程中的帖子的属性和关系。可以指定父对话和线程，也可以指定线程，而不引用父对话。</span><span class="sxs-lookup"><span data-stu-id="6c2a9-p101">Get the properties and relationships of a post in a specified thread. You can specify both the parent conversation and the thread, or, you can specify the thread without referencing the parent conversation.</span></span>

<span data-ttu-id="6c2a9-104">由于**帖子**资源支持[扩展](../../../concepts/extensibility_overview.md)，因此也可使用 `GET` 操作获取**帖子**实例中的自定义属性和扩展数据。</span><span class="sxs-lookup"><span data-stu-id="6c2a9-104">Since the **post** resource supports [extensions](../../../concepts/extensibility_overview.md), you can also use the `GET` operation to get custom properties and extension data in a **post** instance.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6c2a9-105">先决条件</span><span class="sxs-lookup"><span data-stu-id="6c2a9-105">Prerequisites</span></span>
<span data-ttu-id="6c2a9-106">要执行此 API，需要以下**范围**之一：</span><span class="sxs-lookup"><span data-stu-id="6c2a9-106">One of the following **scopes** is required to execute this API:</span></span>

<span data-ttu-id="6c2a9-107">*Group.Read.All*、*Group.ReadWrite.All*</span><span class="sxs-lookup"><span data-stu-id="6c2a9-107">*Group.Read.All*, *Group.Readwrite.All*</span></span>

## <a name="http-request"></a><span data-ttu-id="6c2a9-108">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6c2a9-108">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/threads/{id}/posts/{id}
GET /groups/{id}/conversations/{id}/threads/{id}/posts/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="6c2a9-109">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="6c2a9-109">Optional query parameters</span></span>
<span data-ttu-id="6c2a9-110">此方法支持 [OData 查询参数](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="6c2a9-110">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="6c2a9-111">请求标头</span><span class="sxs-lookup"><span data-stu-id="6c2a9-111">Request headers</span></span>
| <span data-ttu-id="6c2a9-112">标头</span><span class="sxs-lookup"><span data-stu-id="6c2a9-112">Header</span></span>       | <span data-ttu-id="6c2a9-113">值</span><span class="sxs-lookup"><span data-stu-id="6c2a9-113">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="6c2a9-114">Authorization</span><span class="sxs-lookup"><span data-stu-id="6c2a9-114">Authorization</span></span>  | <span data-ttu-id="6c2a9-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="6c2a9-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="6c2a9-117">请求正文</span><span class="sxs-lookup"><span data-stu-id="6c2a9-117">Request body</span></span>
<span data-ttu-id="6c2a9-118">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="6c2a9-118">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6c2a9-119">响应</span><span class="sxs-lookup"><span data-stu-id="6c2a9-119">Response</span></span>

<span data-ttu-id="6c2a9-120">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [post](../resources/post.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="6c2a9-120">If successful, this method returns a `200 OK` response code and [post](../resources/post.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="6c2a9-121">示例</span><span class="sxs-lookup"><span data-stu-id="6c2a9-121">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6c2a9-122">请求</span><span class="sxs-lookup"><span data-stu-id="6c2a9-122">Request</span></span>
<span data-ttu-id="6c2a9-123">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="6c2a9-123">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_post"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/{id}/threads/{id}/posts/{id}
```
##### <a name="response"></a><span data-ttu-id="6c2a9-124">响应</span><span class="sxs-lookup"><span data-stu-id="6c2a9-124">Response</span></span>
<span data-ttu-id="6c2a9-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="6c2a9-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.post"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 414

{
  "body": {
    "contentType": "",
    "content": "content-value"
  },
  "receivedDateTime": "datetime-value",
  "hasAttachments": true,
  "from": {
    "emailAddress": {
      "name": "name-value",
      "address": "address-value"
    }
  },
  "sender": {
    "emailAddress": {
      "name": "name-value",
      "address": "address-value"
    }
  }
}
```

## <a name="see-also"></a><span data-ttu-id="6c2a9-128">另请参阅</span><span class="sxs-lookup"><span data-stu-id="6c2a9-128">See also</span></span>

- [<span data-ttu-id="6c2a9-129">使用扩展向资源添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="6c2a9-129">Add custom data to resources using extensions</span></span>](../../../concepts/extensibility_overview.md)
- [<span data-ttu-id="6c2a9-130">使用开放扩展向用户添加自定义数据（预览）</span><span class="sxs-lookup"><span data-stu-id="6c2a9-130">Add custom data to users using open extensions (preview)</span></span>](../../../concepts/extensibility_open_users.md)
<!--
- [Add custom data to groups using schema extensions (preview)](../../../concepts/extensibility_schema_groups.md)
-->


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get post",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
