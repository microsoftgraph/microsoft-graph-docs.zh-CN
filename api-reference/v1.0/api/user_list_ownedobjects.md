# <a name="list-ownedobjects"></a><span data-ttu-id="94f04-101">列出 ownedObject</span><span class="sxs-lookup"><span data-stu-id="94f04-101">List ownedObjects</span></span>

<span data-ttu-id="94f04-102">获取用户拥有的 directory 对象列表。</span><span class="sxs-lookup"><span data-stu-id="94f04-102">Get the list of directory objects that are owned by the user.</span></span>
## <a name="permissions"></a><span data-ttu-id="94f04-103">权限</span><span class="sxs-lookup"><span data-stu-id="94f04-103">Permissions</span></span>
<span data-ttu-id="94f04-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="94f04-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="94f04-106">权限类型</span><span class="sxs-lookup"><span data-stu-id="94f04-106">Permission type</span></span>      | <span data-ttu-id="94f04-107">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="94f04-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="94f04-108">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="94f04-108">Delegated (work or school account)</span></span> | <span data-ttu-id="94f04-109">User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="94f04-109">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="94f04-110">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="94f04-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="94f04-111">不支持。</span><span class="sxs-lookup"><span data-stu-id="94f04-111">Not supported.</span></span>    |
|<span data-ttu-id="94f04-112">应用程序</span><span class="sxs-lookup"><span data-stu-id="94f04-112">Application</span></span> | <span data-ttu-id="94f04-113">User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="94f04-113">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="94f04-114">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="94f04-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id | userPrincipalName}/ownedObjects
```
## <a name="optional-query-parameters"></a><span data-ttu-id="94f04-115">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="94f04-115">Optional query parameters</span></span>
<span data-ttu-id="94f04-116">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="94f04-116">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="94f04-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="94f04-117">Request headers</span></span>
| <span data-ttu-id="94f04-118">标头</span><span class="sxs-lookup"><span data-stu-id="94f04-118">Header</span></span>       | <span data-ttu-id="94f04-119">值</span><span class="sxs-lookup"><span data-stu-id="94f04-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="94f04-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="94f04-120">Authorization</span></span>  | <span data-ttu-id="94f04-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="94f04-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="94f04-123">Accept</span><span class="sxs-lookup"><span data-stu-id="94f04-123">Accept</span></span>  | <span data-ttu-id="94f04-124">application/json</span><span class="sxs-lookup"><span data-stu-id="94f04-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="94f04-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="94f04-125">Request body</span></span>
<span data-ttu-id="94f04-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="94f04-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="94f04-127">响应</span><span class="sxs-lookup"><span data-stu-id="94f04-127">Response</span></span>

<span data-ttu-id="94f04-128">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [directoryObject](../resources/directoryobject.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="94f04-128">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="94f04-129">示例</span><span class="sxs-lookup"><span data-stu-id="94f04-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="94f04-130">请求</span><span class="sxs-lookup"><span data-stu-id="94f04-130">Request</span></span>
<span data-ttu-id="94f04-131">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="94f04-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_ownedobjects"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/ownedObjects
```
##### <a name="response"></a><span data-ttu-id="94f04-132">响应</span><span class="sxs-lookup"><span data-stu-id="94f04-132">Response</span></span>
<span data-ttu-id="94f04-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="94f04-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "List ownedObjects",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->