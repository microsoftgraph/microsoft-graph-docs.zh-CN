# <a name="get-a-user"></a><span data-ttu-id="f4c35-101">获取用户</span><span class="sxs-lookup"><span data-stu-id="f4c35-101">Get a user</span></span>

<span data-ttu-id="f4c35-102">检索用户对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="f4c35-102">Retrieve the properties and relationships of user object.</span></span>

> <span data-ttu-id="f4c35-p101">注意：获取用户仅返回一组默认属性（*businessPhones、displayName、givenName、id、jobTitle、mail、mobilePhone、officeLocation、preferredLanguage、surname、userPrincipalName*。使用 `$select` 获取 [user](../resources/user.md) 对象的其他属性和关系。</span><span class="sxs-lookup"><span data-stu-id="f4c35-p101">Note: Getting a user returns a default set of properties only (*businessPhones, displayName, givenName, id, jobTitle, mail, mobilePhone, officeLocation, preferredLanguage, surname, userPrincipalName*). Use `$select` to get the other properties and relationships for the [user](../resources/user.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="f4c35-105">权限</span><span class="sxs-lookup"><span data-stu-id="f4c35-105">Permissions</span></span>
<span data-ttu-id="f4c35-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="f4c35-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="f4c35-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="f4c35-108">Permission type</span></span>      | <span data-ttu-id="f4c35-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f4c35-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f4c35-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f4c35-110">Delegated (work or school account)</span></span> | <span data-ttu-id="f4c35-111">User.Read、User.ReadWrite、User.ReadBasic.All、User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="f4c35-111">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="f4c35-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f4c35-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f4c35-113">User.Read、User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f4c35-113">User.Read, User.ReadWrite</span></span>    |
|<span data-ttu-id="f4c35-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="f4c35-114">Application</span></span> | <span data-ttu-id="f4c35-115">User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f4c35-115">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f4c35-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f4c35-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id | userPrincipalName}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="f4c35-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="f4c35-117">Optional query parameters</span></span>
<span data-ttu-id="f4c35-118">此方法支持使用 [OData 查询参数](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters)来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="f4c35-118">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="f4c35-119">默认情况下，仅返回一组有限的属性（_businessPhones、displayName、givenName、id、jobTitle、mail、mobilePhone、officeLocation、preferredLanguage、surname、userPrincipalName_）。</span><span class="sxs-lookup"><span data-stu-id="f4c35-119">By default, only a limited set of properties are returned (_businessPhones, displayName, givenName, id, jobTitle, mail, mobilePhone, officeLocation, preferredLanguage, surname, userPrincipalName_).</span></span> 

<span data-ttu-id="f4c35-120">若要返回其他属性，必须使用 OData `$select` 查询参数指定所需的一组 [user](../resources/user.md) 属性。</span><span class="sxs-lookup"><span data-stu-id="f4c35-120">To return an alternative property set, you must specify the desired set of [user](../resources/user.md) properties using the ODATA `$select` query parameter. For example, to return displayName, givenName, id and postalCode, you would use the add the following to your query </span></span> <span data-ttu-id="f4c35-121">例如，若要返回 _displayName_、_givenName_、和 _postalCode_，则需要将以下项添加到查询 `$select=displayName,givenName,postalCode`</span><span class="sxs-lookup"><span data-stu-id="f4c35-121">To return an alternative property set, you must specify the desired set of user properties using the ODATA  query parameter. For example, to return _displayName_, _givenName, id_ and _postalCode_, you would use the add the following to your query `$select=displayName,givenName,postalCode`</span></span>

## <a name="request-headers"></a><span data-ttu-id="f4c35-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="f4c35-122">Request headers</span></span>
| <span data-ttu-id="f4c35-123">标头</span><span class="sxs-lookup"><span data-stu-id="f4c35-123">Header</span></span>       | <span data-ttu-id="f4c35-124">值</span><span class="sxs-lookup"><span data-stu-id="f4c35-124">Value</span></span>|
|:-----------|:------|
| <span data-ttu-id="f4c35-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="f4c35-125">Authorization</span></span>  | <span data-ttu-id="f4c35-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="f4c35-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="f4c35-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f4c35-128">Content-Type</span></span>   | <span data-ttu-id="f4c35-129">application/json</span><span class="sxs-lookup"><span data-stu-id="f4c35-129">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="f4c35-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="f4c35-130">Request body</span></span>
<span data-ttu-id="f4c35-131">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="f4c35-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f4c35-132">响应</span><span class="sxs-lookup"><span data-stu-id="f4c35-132">Response</span></span>

<span data-ttu-id="f4c35-133">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [user](../resources/user.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="f4c35-133">If successful, this method returns a `200 OK` response code and [user](../resources/user.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="f4c35-134">示例</span><span class="sxs-lookup"><span data-stu-id="f4c35-134">Examples</span></span>

### <a name="example-1-standard-users-request"></a><span data-ttu-id="f4c35-135">示例 1：标准用户请求</span><span class="sxs-lookup"><span data-stu-id="f4c35-135">Example 1: Standard users request</span></span>

<span data-ttu-id="f4c35-136">默认情况下，仅返回一组有限的属性（_businessPhones、displayName、givenName、id、jobTitle、mail、mobilePhone、officeLocation、preferredLanguage、surname、userPrincipalName_）。</span><span class="sxs-lookup"><span data-stu-id="f4c35-136">By default, only a limited set of properties are returned (_businessPhones, displayName, givenName, id, jobTitle, mail, mobilePhone, officeLocation, preferredLanguage, surname, userPrincipalName_).</span></span> <span data-ttu-id="f4c35-137">此示例演示了默认请求和响应。</span><span class="sxs-lookup"><span data-stu-id="f4c35-137">This example illustrates the default request and response.</span></span> 

##### <a name="request"></a><span data-ttu-id="f4c35-138">请求</span><span class="sxs-lookup"><span data-stu-id="f4c35-138">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_user"
}-->
```http
GET https://graph.microsoft.com/v1.0/me
```
##### <a name="response"></a><span data-ttu-id="f4c35-139">响应</span><span class="sxs-lookup"><span data-stu-id="f4c35-139">Response</span></span>

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

### <a name="example-2-users-request-using-select"></a><span data-ttu-id="f4c35-140">示例 2：使用 $select 的用户请求</span><span class="sxs-lookup"><span data-stu-id="f4c35-140">Example 2: Users request using $select</span></span>

<span data-ttu-id="f4c35-141">如果需要其他属性集，可以使用 OData `$select` 查询参数。</span><span class="sxs-lookup"><span data-stu-id="f4c35-141">If you need a different property set, you can use the OData `$select` query parameter.</span></span> <span data-ttu-id="f4c35-142">例如，若要返回 _displayName_、_givenName_、和 _postalCode_，则需要将以下项添加到查询 `$select=displayName,givenName,postalCode`</span><span class="sxs-lookup"><span data-stu-id="f4c35-142">To return an alternative property set, you must specify the desired set of user properties using the ODATA  query parameter. For example, to return _displayName_, _givenName, id_ and _postalCode_, you would use the add the following to your query `$select=displayName,givenName,postalCode`</span></span>

##### <a name="request"></a><span data-ttu-id="f4c35-143">请求</span><span class="sxs-lookup"><span data-stu-id="f4c35-143">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_user"
}-->
```http
GET https://graph.microsoft.com/v1.0/me?$select=displayName,givenName,postalCode
```
##### <a name="response"></a><span data-ttu-id="f4c35-144">响应</span><span class="sxs-lookup"><span data-stu-id="f4c35-144">Response</span></span>
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
   "displayName": "displayName-value",
   "givenName": "givenName-value",
   "postalCode": "postalCode-value"
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
