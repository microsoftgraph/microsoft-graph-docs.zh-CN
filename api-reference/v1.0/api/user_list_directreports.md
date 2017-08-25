# <a name="list-directreports"></a><span data-ttu-id="af79b-101">列出 directReports</span><span class="sxs-lookup"><span data-stu-id="af79b-101">List directReports</span></span>

<span data-ttu-id="af79b-p101">获取用户的直接下属。返回指定此用户作为经理的用户和联系人。</span><span class="sxs-lookup"><span data-stu-id="af79b-p101">Get user's direct reports. Returns the users and contacts for whom this user is assigned as manager.</span></span>
## <a name="permissions"></a><span data-ttu-id="af79b-104">权限</span><span class="sxs-lookup"><span data-stu-id="af79b-104">Permissions</span></span>
<span data-ttu-id="af79b-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="af79b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="af79b-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="af79b-107">Permission type</span></span>      | <span data-ttu-id="af79b-108">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="af79b-108">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="af79b-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="af79b-109">Delegated (work or school account)</span></span> | <span data-ttu-id="af79b-110">User.Read、User.ReadWrite、User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="af79b-110">One of the following scopes is required to execute this API: User.Read; User.ReadWrite; User.Read.All; User.ReadWrite.All; Directory.Read.All; Directory.ReadWrite.All; Directory.AccessAsUser.All</span></span>    | 
|<span data-ttu-id="af79b-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="af79b-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="af79b-112">User.Read、User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="af79b-112">User.Read, User.ReadWrite</span></span>    | 
|<span data-ttu-id="af79b-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="af79b-113">Application</span></span> | <span data-ttu-id="af79b-114">User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="af79b-114">One of the following scopes is required to execute this API: User.Read.All; User.ReadWrite.All; Directory.Read.All; Directory.ReadWrite.All; Directory.AccessAsUser.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="af79b-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="af79b-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id | userPrincipalName}/directReports
```
## <a name="optional-query-parameters"></a><span data-ttu-id="af79b-116">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="af79b-116">Optional query parameters</span></span>
<span data-ttu-id="af79b-117">此方法支持 [OData 查询参数](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="af79b-117">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="af79b-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="af79b-118">Request headers</span></span>
| <span data-ttu-id="af79b-119">标头</span><span class="sxs-lookup"><span data-stu-id="af79b-119">Header</span></span>       | <span data-ttu-id="af79b-120">值</span><span class="sxs-lookup"><span data-stu-id="af79b-120">Value</span></span>|
|:-----------|:------|
| <span data-ttu-id="af79b-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="af79b-121">Authorization</span></span>  | <span data-ttu-id="af79b-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="af79b-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="af79b-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="af79b-124">Content-Type</span></span>   | <span data-ttu-id="af79b-125">application/json</span><span class="sxs-lookup"><span data-stu-id="af79b-125">application/json</span></span>  | 

## <a name="request-body"></a><span data-ttu-id="af79b-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="af79b-126">Request body</span></span>
<span data-ttu-id="af79b-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="af79b-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="af79b-128">响应</span><span class="sxs-lookup"><span data-stu-id="af79b-128">Response</span></span>

<span data-ttu-id="af79b-129">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [directoryObject](../resources/directoryobject.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="af79b-129">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="af79b-130">示例</span><span class="sxs-lookup"><span data-stu-id="af79b-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="af79b-131">请求</span><span class="sxs-lookup"><span data-stu-id="af79b-131">Request</span></span>
<span data-ttu-id="af79b-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="af79b-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_directreports"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/directReports
```
##### <a name="response"></a><span data-ttu-id="af79b-133">响应</span><span class="sxs-lookup"><span data-stu-id="af79b-133">Response</span></span>
<span data-ttu-id="af79b-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="af79b-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "List directReports",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->