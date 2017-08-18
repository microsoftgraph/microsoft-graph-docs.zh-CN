# <a name="list-manager"></a><span data-ttu-id="b3ac5-101">列出经理</span><span class="sxs-lookup"><span data-stu-id="b3ac5-101">List manager</span></span>

<span data-ttu-id="b3ac5-p101">获取用户的经理。返回指定为用户经理的用户或联系人。</span><span class="sxs-lookup"><span data-stu-id="b3ac5-p101">Get user's manager. Returns the user or contact assigned as the user's manager.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="b3ac5-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="b3ac5-104">Prerequisites</span></span>
<span data-ttu-id="b3ac5-105">要执行此 API，需要以下**范围**之一：*User.Read.All；User.ReadWrite.All；Directory.Read.All；Directory.ReadWrite.All；Directory.AccessAsUser.All*</span><span class="sxs-lookup"><span data-stu-id="b3ac5-105">One of the following **scopes** is required to execute this API: *User.Read.All; User.ReadWrite.All; Directory.Read.All; Directory.ReadWrite.All; Directory.AccessAsUser.All*</span></span>

## <a name="http-request"></a><span data-ttu-id="b3ac5-106">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b3ac5-106">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id | userPrincipalName}/manager
```
## <a name="optional-query-parameters"></a><span data-ttu-id="b3ac5-107">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="b3ac5-107">Optional query parameters</span></span>
<span data-ttu-id="b3ac5-108">此方法支持 [OData 查询参数](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="b3ac5-108">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="b3ac5-109">请求标头</span><span class="sxs-lookup"><span data-stu-id="b3ac5-109">Request headers</span></span>
| <span data-ttu-id="b3ac5-110">标头</span><span class="sxs-lookup"><span data-stu-id="b3ac5-110">Header</span></span>       | <span data-ttu-id="b3ac5-111">值</span><span class="sxs-lookup"><span data-stu-id="b3ac5-111">Value</span></span>|
|:-----------|:------|
| <span data-ttu-id="b3ac5-112">Authorization</span><span class="sxs-lookup"><span data-stu-id="b3ac5-112">Authorization</span></span>  | <span data-ttu-id="b3ac5-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="b3ac5-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="b3ac5-115">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b3ac5-115">Content-Type</span></span>   | <span data-ttu-id="b3ac5-116">application/json</span><span class="sxs-lookup"><span data-stu-id="b3ac5-116">application/json</span></span>  | 

## <a name="request-body"></a><span data-ttu-id="b3ac5-117">请求正文</span><span class="sxs-lookup"><span data-stu-id="b3ac5-117">Request body</span></span>
<span data-ttu-id="b3ac5-118">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="b3ac5-118">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b3ac5-119">响应</span><span class="sxs-lookup"><span data-stu-id="b3ac5-119">Response</span></span>

<span data-ttu-id="b3ac5-120">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [directoryObject](../resources/directoryobject.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="b3ac5-120">If successful, this method returns a `200 OK` response code and a [directoryObject](../resources/directoryobject.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="b3ac5-121">示例</span><span class="sxs-lookup"><span data-stu-id="b3ac5-121">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b3ac5-122">请求</span><span class="sxs-lookup"><span data-stu-id="b3ac5-122">Request</span></span>
<span data-ttu-id="b3ac5-123">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="b3ac5-123">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_manager"
}-->
```http
GET https://graph.microsoft.com/v1.0/users/{id|userPrincipalName}/manager
```
##### <a name="response"></a><span data-ttu-id="b3ac5-124">响应</span><span class="sxs-lookup"><span data-stu-id="b3ac5-124">Response</span></span>
<span data-ttu-id="b3ac5-125">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="b3ac5-125">Here is an example of the response.</span></span>
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
