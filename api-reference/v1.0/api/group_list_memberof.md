# <a name="list-memberof"></a><span data-ttu-id="5cae3-101">列出 memberOf</span><span class="sxs-lookup"><span data-stu-id="5cae3-101">List memberOf</span></span>

<span data-ttu-id="5cae3-102">获取直接成员组构成的组集合。</span><span class="sxs-lookup"><span data-stu-id="5cae3-102">Get groups that the group is a direct member of.</span></span> 

<span data-ttu-id="5cae3-p101">此操作不可传递。与获取用户的 Office 365 组不同，该操作将返回所有类型的组，而不仅是 Office 365 组。</span><span class="sxs-lookup"><span data-stu-id="5cae3-p101">This operation is not transitive. Unlike getting a user's Office 365 Groups, this returns all types of groups, not just Office 365 groups.</span></span> 

## <a name="prerequisites"></a><span data-ttu-id="5cae3-105">先决条件</span><span class="sxs-lookup"><span data-stu-id="5cae3-105">Prerequisites</span></span>
<span data-ttu-id="5cae3-106">要执行此 API，需要以下**范围**之一：*Group.Read.All*</span><span class="sxs-lookup"><span data-stu-id="5cae3-106">One of the following **scopes** is required to execute this API: *Group.Read.All*</span></span>
## <a name="http-request"></a><span data-ttu-id="5cae3-107">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5cae3-107">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/memberOf
```
## <a name="optional-query-parameters"></a><span data-ttu-id="5cae3-108">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="5cae3-108">Optional query parameters</span></span>
<span data-ttu-id="5cae3-109">此方法支持 [OData 查询参数](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="5cae3-109">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="5cae3-110">请求标头</span><span class="sxs-lookup"><span data-stu-id="5cae3-110">Request headers</span></span>
| <span data-ttu-id="5cae3-111">名称</span><span class="sxs-lookup"><span data-stu-id="5cae3-111">Name</span></span>       | <span data-ttu-id="5cae3-112">类型</span><span class="sxs-lookup"><span data-stu-id="5cae3-112">Type</span></span> | <span data-ttu-id="5cae3-113">说明</span><span class="sxs-lookup"><span data-stu-id="5cae3-113">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="5cae3-114">Authorization</span><span class="sxs-lookup"><span data-stu-id="5cae3-114">Authorization</span></span>  | <span data-ttu-id="5cae3-115">string</span><span class="sxs-lookup"><span data-stu-id="5cae3-115">string</span></span>  | <span data-ttu-id="5cae3-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="5cae3-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5cae3-118">请求正文</span><span class="sxs-lookup"><span data-stu-id="5cae3-118">Request body</span></span>
<span data-ttu-id="5cae3-119">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="5cae3-119">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5cae3-120">响应</span><span class="sxs-lookup"><span data-stu-id="5cae3-120">Response</span></span>

<span data-ttu-id="5cae3-121">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [directoryObject](../resources/directoryobject.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="5cae3-121">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="5cae3-122">示例</span><span class="sxs-lookup"><span data-stu-id="5cae3-122">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5cae3-123">请求</span><span class="sxs-lookup"><span data-stu-id="5cae3-123">Request</span></span>
<span data-ttu-id="5cae3-124">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="5cae3-124">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_memberof"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/{id}/memberOf
```
##### <a name="response"></a><span data-ttu-id="5cae3-125">响应</span><span class="sxs-lookup"><span data-stu-id="5cae3-125">Response</span></span>
<span data-ttu-id="5cae3-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="5cae3-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 55

{
  "value": [
    {
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List memberOf",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->