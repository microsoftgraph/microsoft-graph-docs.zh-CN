# <a name="get-post"></a><span data-ttu-id="d4951-101">获取帖子</span><span class="sxs-lookup"><span data-stu-id="d4951-101">Get post</span></span>

<span data-ttu-id="d4951-p101">获取指定线程中的帖子的属性和关系。可以指定父对话和线程，也可以指定线程，而不引用父对话。</span><span class="sxs-lookup"><span data-stu-id="d4951-p101">Get the properties and relationships of a post in a specified thread. You can specify both the parent conversation and the thread, or, you can specify the thread without referencing the parent conversation.</span></span>

<span data-ttu-id="d4951-104">由于**帖子**资源支持[扩展](../../../concepts/extensibility_overview.md)，因此也可使用 `GET` 操作获取**帖子**实例中的自定义属性和扩展数据。</span><span class="sxs-lookup"><span data-stu-id="d4951-104">Since the **post** resource supports [extensions](../../../concepts/extensibility_overview.md), you can also use the `GET` operation to get custom properties and extension data in a **post** instance.</span></span>

## <a name="permissions"></a><span data-ttu-id="d4951-105">权限</span><span class="sxs-lookup"><span data-stu-id="d4951-105">Permissions</span></span>
<span data-ttu-id="d4951-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="d4951-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="d4951-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="d4951-108">Permission type</span></span>      | <span data-ttu-id="d4951-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d4951-109">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="d4951-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d4951-110">Delegated (work or school account)</span></span> | <span data-ttu-id="d4951-111">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d4951-111">Group.Read.All, Group.ReadWrite.All</span></span>    | 
|<span data-ttu-id="d4951-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d4951-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d4951-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="d4951-113">Not supported.</span></span>    | 
|<span data-ttu-id="d4951-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="d4951-114">Application</span></span> | <span data-ttu-id="d4951-115">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d4951-115">Group.Read.All, Group.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="d4951-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d4951-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/threads/{id}/posts/{id}
GET /groups/{id}/conversations/{id}/threads/{id}/posts/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="d4951-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="d4951-117">Optional query parameters</span></span>
<span data-ttu-id="d4951-118">此方法支持 [OData 查询参数](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="d4951-118">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="d4951-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="d4951-119">Request headers</span></span>
| <span data-ttu-id="d4951-120">标头</span><span class="sxs-lookup"><span data-stu-id="d4951-120">Header</span></span>       | <span data-ttu-id="d4951-121">值</span><span class="sxs-lookup"><span data-stu-id="d4951-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="d4951-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="d4951-122">Authorization</span></span>  | <span data-ttu-id="d4951-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="d4951-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="d4951-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="d4951-125">Request body</span></span>
<span data-ttu-id="d4951-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="d4951-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d4951-127">响应</span><span class="sxs-lookup"><span data-stu-id="d4951-127">Response</span></span>

<span data-ttu-id="d4951-128">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [post](../resources/post.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="d4951-128">If successful, this method returns a `200 OK` response code and [post](../resources/post.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="d4951-129">示例</span><span class="sxs-lookup"><span data-stu-id="d4951-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d4951-130">请求</span><span class="sxs-lookup"><span data-stu-id="d4951-130">Request</span></span>
<span data-ttu-id="d4951-131">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="d4951-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_post"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/{id}/threads/{id}/posts/{id}
```
##### <a name="response"></a><span data-ttu-id="d4951-132">响应</span><span class="sxs-lookup"><span data-stu-id="d4951-132">Response</span></span>
<span data-ttu-id="d4951-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="d4951-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="d4951-136">另请参阅</span><span class="sxs-lookup"><span data-stu-id="d4951-136">See also</span></span>

- [<span data-ttu-id="d4951-137">使用扩展向资源添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="d4951-137">Add custom data to resources using extensions</span></span>](../../../concepts/extensibility_overview.md)
- [<span data-ttu-id="d4951-138">使用开放扩展向用户添加自定义数据（预览）</span><span class="sxs-lookup"><span data-stu-id="d4951-138">Add custom data to users using open extensions (preview)</span></span>](../../../concepts/extensibility_open_users.md)
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
