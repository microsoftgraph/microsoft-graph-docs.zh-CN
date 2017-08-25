# <a name="list-members"></a><span data-ttu-id="10b16-101">列出成员</span><span class="sxs-lookup"><span data-stu-id="10b16-101">List members</span></span>

<span data-ttu-id="10b16-p101">获取组的直接成员列表。组可将用户、联系人和其他组作为成员。此操作不可传递。</span><span class="sxs-lookup"><span data-stu-id="10b16-p101">Get a list of the group's direct members. A group can have users, contacts, and other groups as members. This operation is not transitive.</span></span>
## <a name="permissions"></a><span data-ttu-id="10b16-105">权限</span><span class="sxs-lookup"><span data-stu-id="10b16-105">Permissions</span></span>
<span data-ttu-id="10b16-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="10b16-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="10b16-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="10b16-108">Permission type</span></span>      | <span data-ttu-id="10b16-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="10b16-109">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="10b16-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="10b16-110">Delegated (work or school account)</span></span> | <span data-ttu-id="10b16-111">User.ReadBasic.All、User.Read.All、Directory.Read.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="10b16-111">User.ReadBasic.All, User.Read.All, Directory.Read.All, Directory.AccessAsUser.All</span></span>   | 
|<span data-ttu-id="10b16-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="10b16-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="10b16-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="10b16-113">Not supported.</span></span>    | 
|<span data-ttu-id="10b16-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="10b16-114">Application</span></span> | <span data-ttu-id="10b16-115">User.Read.All、Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="10b16-115">User.Read.All, Directory.Read.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="10b16-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="10b16-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/members
```
## <a name="optional-query-parameters"></a><span data-ttu-id="10b16-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="10b16-117">Optional query parameters</span></span>
<span data-ttu-id="10b16-118">此方法支持 [OData 查询参数](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="10b16-118">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="10b16-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="10b16-119">Request headers</span></span>
| <span data-ttu-id="10b16-120">名称</span><span class="sxs-lookup"><span data-stu-id="10b16-120">Name</span></span>       | <span data-ttu-id="10b16-121">类型</span><span class="sxs-lookup"><span data-stu-id="10b16-121">Type</span></span> | <span data-ttu-id="10b16-122">说明</span><span class="sxs-lookup"><span data-stu-id="10b16-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="10b16-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="10b16-123">Authorization</span></span>  | <span data-ttu-id="10b16-124">string</span><span class="sxs-lookup"><span data-stu-id="10b16-124">string</span></span>  | <span data-ttu-id="10b16-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="10b16-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="10b16-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="10b16-127">Request body</span></span>
<span data-ttu-id="10b16-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="10b16-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="10b16-129">响应</span><span class="sxs-lookup"><span data-stu-id="10b16-129">Response</span></span>

<span data-ttu-id="10b16-130">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [directoryObject](../resources/directoryobject.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="10b16-130">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="10b16-131">示例</span><span class="sxs-lookup"><span data-stu-id="10b16-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="10b16-132">请求</span><span class="sxs-lookup"><span data-stu-id="10b16-132">Request</span></span>
<span data-ttu-id="10b16-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="10b16-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_members"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/{id}/members
```
##### <a name="response"></a><span data-ttu-id="10b16-134">响应</span><span class="sxs-lookup"><span data-stu-id="10b16-134">Response</span></span>
<span data-ttu-id="10b16-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="10b16-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "List members",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->