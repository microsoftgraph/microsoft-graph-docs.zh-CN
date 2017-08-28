# <a name="list-memberof"></a><span data-ttu-id="cf6dd-101">列出 memberOf</span><span class="sxs-lookup"><span data-stu-id="cf6dd-101">List memberOf</span></span>

<span data-ttu-id="cf6dd-102">获取直接成员组构成的组集合。</span><span class="sxs-lookup"><span data-stu-id="cf6dd-102">Get groups that the group is a direct member of.</span></span> 

<span data-ttu-id="cf6dd-p101">此操作不可传递。与获取用户的 Office 365 组不同，该操作将返回所有类型的组，而不仅是 Office 365 组。</span><span class="sxs-lookup"><span data-stu-id="cf6dd-p101">This operation is not transitive. Unlike getting a user's Office 365 Groups, this returns all types of groups, not just Office 365 groups.</span></span> 

## <a name="permissions"></a><span data-ttu-id="cf6dd-105">权限</span><span class="sxs-lookup"><span data-stu-id="cf6dd-105">Permissions</span></span>
<span data-ttu-id="cf6dd-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="cf6dd-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="cf6dd-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="cf6dd-108">Permission type</span></span>      | <span data-ttu-id="cf6dd-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="cf6dd-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cf6dd-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="cf6dd-110">Delegated (work or school account)</span></span> | <span data-ttu-id="cf6dd-111">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="cf6dd-111">Group.Read.All</span></span>    |
|<span data-ttu-id="cf6dd-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="cf6dd-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cf6dd-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="cf6dd-113">Not supported.</span></span>    |
|<span data-ttu-id="cf6dd-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="cf6dd-114">Application</span></span> | <span data-ttu-id="cf6dd-115">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="cf6dd-115">Group.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="cf6dd-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="cf6dd-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/memberOf
```
## <a name="optional-query-parameters"></a><span data-ttu-id="cf6dd-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="cf6dd-117">Optional query parameters</span></span>
<span data-ttu-id="cf6dd-118">此方法支持 [OData 查询参数](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="cf6dd-118">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="cf6dd-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="cf6dd-119">Request headers</span></span>
| <span data-ttu-id="cf6dd-120">名称</span><span class="sxs-lookup"><span data-stu-id="cf6dd-120">Name</span></span>       | <span data-ttu-id="cf6dd-121">类型</span><span class="sxs-lookup"><span data-stu-id="cf6dd-121">Type</span></span> | <span data-ttu-id="cf6dd-122">说明</span><span class="sxs-lookup"><span data-stu-id="cf6dd-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="cf6dd-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="cf6dd-123">Authorization</span></span>  | <span data-ttu-id="cf6dd-124">string</span><span class="sxs-lookup"><span data-stu-id="cf6dd-124">string</span></span>  | <span data-ttu-id="cf6dd-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="cf6dd-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="cf6dd-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="cf6dd-127">Request body</span></span>
<span data-ttu-id="cf6dd-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="cf6dd-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cf6dd-129">响应</span><span class="sxs-lookup"><span data-stu-id="cf6dd-129">Response</span></span>

<span data-ttu-id="cf6dd-130">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [directoryObject](../resources/directoryobject.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="cf6dd-130">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="cf6dd-131">示例</span><span class="sxs-lookup"><span data-stu-id="cf6dd-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="cf6dd-132">请求</span><span class="sxs-lookup"><span data-stu-id="cf6dd-132">Request</span></span>
<span data-ttu-id="cf6dd-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="cf6dd-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_memberof"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/{id}/memberOf
```
##### <a name="response"></a><span data-ttu-id="cf6dd-134">响应</span><span class="sxs-lookup"><span data-stu-id="cf6dd-134">Response</span></span>
<span data-ttu-id="cf6dd-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="cf6dd-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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