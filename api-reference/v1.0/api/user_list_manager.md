<span data-ttu-id="a86a9-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="a86a9-p102">Bearer token. Required.</span></span>  | Bearer {token}。必需。  |
| <span data-ttu-id="a86a9-115">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a86a9-115">Content-Type</span></span>   | <span data-ttu-id="a86a9-116">application/json</span><span class="sxs-lookup"><span data-stu-id="a86a9-116">application/json</span></span>  | 

## <span data-ttu-id="a86a9-117">请求正文</span><span class="sxs-lookup"><span data-stu-id="a86a9-117">Request body</span></span>
<a id="request-body" class="xliff"></a>
<span data-ttu-id="a86a9-118">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="a86a9-118">Do not supply a request body for this method.</span></span>
## <span data-ttu-id="a86a9-119">响应</span><span class="sxs-lookup"><span data-stu-id="a86a9-119">Response</span></span>
<a id="response" class="xliff"></a>
<span data-ttu-id="a86a9-120">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [directoryObject](../resources/directoryobject.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="a86a9-120">If successful, this method returns a `200 OK` response code and a [directoryObject](../resources/directoryobject.md) object in the response body.</span></span>
## <span data-ttu-id="a86a9-121">示例</span><span class="sxs-lookup"><span data-stu-id="a86a9-121">Example</span></span>
<a id="example" class="xliff"></a>
##### <span data-ttu-id="a86a9-122">请求</span><span class="sxs-lookup"><span data-stu-id="a86a9-122">Request</span></span>
<a id="request" class="xliff"></a>
<span data-ttu-id="a86a9-123">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="a86a9-123">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_manager"
}-->
```http
GET https://graph.microsoft.com/v1.0/users/{id|userPrincipalName}/manager
```
##### <span data-ttu-id="a86a9-124">响应</span><span class="sxs-lookup"><span data-stu-id="a86a9-124">Response</span></span>
<a id="response" class="xliff"></a>
<span data-ttu-id="a86a9-125">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="a86a9-125">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": false
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "objectType": "User",
  "id": "111048d2-2761-4347-b978-07354283363b",
  "accountEnabled": true,
  "city": "San Diego",
  "country": "United States",
  "department": "Sales & Marketing",
  "displayName": "Sara Davis",
  "givenName": "Sara",
  "jobTitle": "Finance VP",
  "mail": "SaraD@contoso.onmicrosoft.com",
  "mailNickname": "SaraD",
  "state": "CA",
  "streetAddress": "9256 Towne Center Dr., Suite 400",
  "surname": "Davis",
  "usageLocation": "US",
  "userPrincipalName": "SaraD@contoso.onmicrosoft.com"
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
