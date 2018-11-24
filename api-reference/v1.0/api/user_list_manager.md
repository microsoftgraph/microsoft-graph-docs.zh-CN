# <a name="list-manager"></a><span data-ttu-id="221b5-101">列出经理</span><span class="sxs-lookup"><span data-stu-id="221b5-101">List manager</span></span>

<span data-ttu-id="221b5-p101">获取用户的经理。返回指定为用户经理的用户或联系人。</span><span class="sxs-lookup"><span data-stu-id="221b5-p101">Get user's manager. Returns the user or contact assigned as the user's manager.</span></span>
## <a name="permissions"></a><span data-ttu-id="221b5-104">权限</span><span class="sxs-lookup"><span data-stu-id="221b5-104">Permissions</span></span>
<span data-ttu-id="221b5-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="221b5-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="221b5-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="221b5-107">Permission type</span></span>      | <span data-ttu-id="221b5-108">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="221b5-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="221b5-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="221b5-109">Delegated (work or school account)</span></span> | <span data-ttu-id="221b5-110">User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="221b5-110">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="221b5-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="221b5-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="221b5-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="221b5-112">Not supported.</span></span>    |
|<span data-ttu-id="221b5-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="221b5-113">Application</span></span> | <span data-ttu-id="221b5-114">User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="221b5-114">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="221b5-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="221b5-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id | userPrincipalName}/manager
```
## <a name="optional-query-parameters"></a><span data-ttu-id="221b5-116">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="221b5-116">Optional query parameters</span></span>
<span data-ttu-id="221b5-117">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="221b5-117">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="221b5-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="221b5-118">Request headers</span></span>
| <span data-ttu-id="221b5-119">标头</span><span class="sxs-lookup"><span data-stu-id="221b5-119">Header</span></span>       | <span data-ttu-id="221b5-120">值</span><span class="sxs-lookup"><span data-stu-id="221b5-120">Value</span></span>|
|:-----------|:------|
| <span data-ttu-id="221b5-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="221b5-121">Authorization</span></span>  | <span data-ttu-id="221b5-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="221b5-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="221b5-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="221b5-124">Content-Type</span></span>   | <span data-ttu-id="221b5-125">application/json</span><span class="sxs-lookup"><span data-stu-id="221b5-125">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="221b5-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="221b5-126">Request body</span></span>
<span data-ttu-id="221b5-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="221b5-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="221b5-128">响应</span><span class="sxs-lookup"><span data-stu-id="221b5-128">Response</span></span>

<span data-ttu-id="221b5-129">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [directoryObject](../resources/directoryobject.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="221b5-129">If successful, this method returns a `200 OK` response code and a [directoryObject](../resources/directoryobject.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="221b5-130">示例</span><span class="sxs-lookup"><span data-stu-id="221b5-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="221b5-131">请求</span><span class="sxs-lookup"><span data-stu-id="221b5-131">Request</span></span>
<span data-ttu-id="221b5-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="221b5-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_manager"
}-->
```http
GET https://graph.microsoft.com/v1.0/users/{id|userPrincipalName}/manager
```
##### <a name="response"></a><span data-ttu-id="221b5-133">响应</span><span class="sxs-lookup"><span data-stu-id="221b5-133">Response</span></span>
<span data-ttu-id="221b5-134">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="221b5-134">Here is an example of the response.</span></span>
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
