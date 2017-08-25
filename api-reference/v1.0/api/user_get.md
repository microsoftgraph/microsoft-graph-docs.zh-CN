# <a name="get-a-user"></a><span data-ttu-id="3a6bb-101">获取用户</span><span class="sxs-lookup"><span data-stu-id="3a6bb-101">Get a user</span></span>

<span data-ttu-id="3a6bb-102">检索用户对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="3a6bb-102">Retrieve the properties and relationships of user object.</span></span>

> <span data-ttu-id="3a6bb-p101">注意：获取用户仅返回一组默认属性（*businessPhones、displayName、givenName、id、jobTitle、mail、mobilePhone、officeLocation、preferredLanguage、surname、userPrincipalName*。使用 `$select` 获取 [user](../resources/user.md) 对象的其他属性和关系。</span><span class="sxs-lookup"><span data-stu-id="3a6bb-p101">Note: Getting a user returns a default set of properties only (*businessPhones, displayName, givenName, id, jobTitle, mail, mobilePhone, officeLocation, preferredLanguage, surname, userPrincipalName*). Use `$select` to get the other properties and relationships for the [user](../resources/user.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="3a6bb-105">权限</span><span class="sxs-lookup"><span data-stu-id="3a6bb-105">Permissions</span></span>
<span data-ttu-id="3a6bb-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="3a6bb-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="3a6bb-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="3a6bb-108">Permission type</span></span>      | <span data-ttu-id="3a6bb-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="3a6bb-109">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="3a6bb-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3a6bb-110">Delegated (work or school account)</span></span> | <span data-ttu-id="3a6bb-111">User.Read、User.ReadWrite、User.ReadBasic.All、User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="3a6bb-111">One of the following scopes is required to execute this API: User.Read; User.ReadWrite; User.ReadBasic.All; User.Read.All; User.ReadWrite.All; Directory.Read.All; Directory.ReadWrite.All; Directory.AccessAsUser.All</span></span>    | 
|<span data-ttu-id="3a6bb-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3a6bb-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3a6bb-113">User.Read、User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3a6bb-113">User.Read, User.ReadWrite</span></span>    | 
|<span data-ttu-id="3a6bb-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="3a6bb-114">Application</span></span> | <span data-ttu-id="3a6bb-115">User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3a6bb-115">One of the following scopes is required to execute this API: User.Read.All; User.ReadWrite.All; Directory.Read.All; Directory.ReadWrite.All; Directory.AccessAsUser.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="3a6bb-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3a6bb-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id | userPrincipalName}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="3a6bb-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="3a6bb-117">Optional query parameters</span></span>
<span data-ttu-id="3a6bb-118">此方法支持 [OData 查询参数](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="3a6bb-118">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="3a6bb-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="3a6bb-119">Request headers</span></span>
| <span data-ttu-id="3a6bb-120">标头</span><span class="sxs-lookup"><span data-stu-id="3a6bb-120">Header</span></span>       | <span data-ttu-id="3a6bb-121">值</span><span class="sxs-lookup"><span data-stu-id="3a6bb-121">Value</span></span>|
|:-----------|:------|
| <span data-ttu-id="3a6bb-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="3a6bb-122">Authorization</span></span>  | <span data-ttu-id="3a6bb-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="3a6bb-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="3a6bb-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="3a6bb-125">Content-Type</span></span>   | <span data-ttu-id="3a6bb-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3a6bb-126">application/json</span></span> | 

## <a name="request-body"></a><span data-ttu-id="3a6bb-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="3a6bb-127">Request body</span></span>
<span data-ttu-id="3a6bb-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="3a6bb-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3a6bb-129">响应</span><span class="sxs-lookup"><span data-stu-id="3a6bb-129">Response</span></span>

<span data-ttu-id="3a6bb-130">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [user](../resources/user.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="3a6bb-130">If successful, this method returns a `200 OK` response code and [user](../resources/user.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="3a6bb-131">示例</span><span class="sxs-lookup"><span data-stu-id="3a6bb-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3a6bb-132">请求</span><span class="sxs-lookup"><span data-stu-id="3a6bb-132">Request</span></span>
<span data-ttu-id="3a6bb-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="3a6bb-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_user"
}-->
```http
GET https://graph.microsoft.com/v1.0/me
```
##### <a name="response"></a><span data-ttu-id="3a6bb-134">响应</span><span class="sxs-lookup"><span data-stu-id="3a6bb-134">Response</span></span>
<span data-ttu-id="3a6bb-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="3a6bb-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 491

{
  "businessPhones": [
       "businessPhones-value"
   ],
   "displayName": "displayName-value",
   "givenName": "givenName-value",
   "jobTitle": "jobTitle-value",
   "mail": "mail-value",
   "mobilePhone": "mobilePhone-value",
   "officeLocation": "officeLocation-value",
   "preferredLanguage": "preferredLanguage-value",
   "surname": "surname-value",
   "userPrincipalName": "userPrincipalName-value",
   "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get user",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
