# <a name="list-createdobjects"></a><span data-ttu-id="497fb-101">列出 createdObjects</span><span class="sxs-lookup"><span data-stu-id="497fb-101">List createdObjects</span></span>

<span data-ttu-id="497fb-102">获取由用户创建的 directory 对象列表。</span><span class="sxs-lookup"><span data-stu-id="497fb-102">Get a list of directory objects that were created by the user.</span></span>
## <a name="permissions"></a><span data-ttu-id="497fb-103">权限</span><span class="sxs-lookup"><span data-stu-id="497fb-103">Permissions</span></span>
<span data-ttu-id="497fb-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="497fb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="497fb-106">权限类型</span><span class="sxs-lookup"><span data-stu-id="497fb-106">Permission type</span></span>      | <span data-ttu-id="497fb-107">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="497fb-107">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="497fb-108">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="497fb-108">Delegated (work or school account)</span></span> | <span data-ttu-id="497fb-109">User.Read、User.ReadWrite、User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="497fb-109">One of the following scopes is required to execute this API: User.Read; User.ReadWrite; User.Read.All; User.ReadWrite.All; Directory.Read.All; Directory.ReadWrite.All; Directory.AccessAsUser.All</span></span>    | 
|<span data-ttu-id="497fb-110">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="497fb-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="497fb-111">User.Read、User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="497fb-111">User.Read, User.ReadWrite</span></span>    | 
|<span data-ttu-id="497fb-112">应用程序</span><span class="sxs-lookup"><span data-stu-id="497fb-112">Application</span></span> | <span data-ttu-id="497fb-113">User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="497fb-113">One of the following scopes is required to execute this API: User.Read.All; User.ReadWrite.All; Directory.Read.All; Directory.ReadWrite.All; Directory.AccessAsUser.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="497fb-114">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="497fb-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id | userPrincipalName}/createdObjects
```
## <a name="optional-query-parameters"></a><span data-ttu-id="497fb-115">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="497fb-115">Optional query parameters</span></span>
<span data-ttu-id="497fb-116">此方法支持 [OData 查询参数](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="497fb-116">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="497fb-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="497fb-117">Request headers</span></span>
| <span data-ttu-id="497fb-118">标头</span><span class="sxs-lookup"><span data-stu-id="497fb-118">Header</span></span>       | <span data-ttu-id="497fb-119">值</span><span class="sxs-lookup"><span data-stu-id="497fb-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="497fb-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="497fb-120">Authorization</span></span>  | <span data-ttu-id="497fb-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="497fb-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="497fb-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="497fb-123">Content-Type</span></span>  | <span data-ttu-id="497fb-124">application/json</span><span class="sxs-lookup"><span data-stu-id="497fb-124">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="497fb-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="497fb-125">Request body</span></span>
<span data-ttu-id="497fb-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="497fb-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="497fb-127">响应</span><span class="sxs-lookup"><span data-stu-id="497fb-127">Response</span></span>

<span data-ttu-id="497fb-128">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [directoryObject](../resources/directoryobject.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="497fb-128">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="497fb-129">示例</span><span class="sxs-lookup"><span data-stu-id="497fb-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="497fb-130">请求</span><span class="sxs-lookup"><span data-stu-id="497fb-130">Request</span></span>
<span data-ttu-id="497fb-131">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="497fb-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_createdobjects"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/createdObjects
```
##### <a name="response"></a><span data-ttu-id="497fb-132">响应</span><span class="sxs-lookup"><span data-stu-id="497fb-132">Response</span></span>
<span data-ttu-id="497fb-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="497fb-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "List createdObjects",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->