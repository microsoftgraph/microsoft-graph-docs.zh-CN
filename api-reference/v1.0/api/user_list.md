# <a name="list-users"></a><span data-ttu-id="58a29-101">列出用户</span><span class="sxs-lookup"><span data-stu-id="58a29-101">List users</span></span>

<span data-ttu-id="58a29-102">检索 user 对象列表。</span><span class="sxs-lookup"><span data-stu-id="58a29-102">Retrieve a list of user objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="58a29-103">权限</span><span class="sxs-lookup"><span data-stu-id="58a29-103">Permissions</span></span>

<span data-ttu-id="58a29-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="58a29-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="58a29-106">权限类型</span><span class="sxs-lookup"><span data-stu-id="58a29-106">Permission type</span></span>      | <span data-ttu-id="58a29-107">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="58a29-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="58a29-108">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="58a29-108">Delegated (work or school account)</span></span> | <span data-ttu-id="58a29-109">User.ReadBasic.All、User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="58a29-109">User.ReadBasic.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="58a29-110">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="58a29-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="58a29-111">不支持。</span><span class="sxs-lookup"><span data-stu-id="58a29-111">Not supported.</span></span>    |
|<span data-ttu-id="58a29-112">应用程序</span><span class="sxs-lookup"><span data-stu-id="58a29-112">Application</span></span> | <span data-ttu-id="58a29-113">User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="58a29-113">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="58a29-114">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="58a29-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users
```

## <a name="optional-query-parameters"></a><span data-ttu-id="58a29-115">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="58a29-115">Optional query parameters</span></span>

<span data-ttu-id="58a29-116">此方法支持 [OData 查询参数](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="58a29-116">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="58a29-117">默认情况下，仅返回一组有限的属性（_businessPhones、displayName、givenName、id、jobTitle、mail、mobilePhone、officeLocation、preferredLanguage、surname、userPrincipalName_</span><span class="sxs-lookup"><span data-stu-id="58a29-117">By default, only a limited set of properties are returned (_businessPhones, displayName, givenName, id, jobTitle, mail, mobilePhone, officeLocation, preferredLanguage, surname, userPrincipalName_).</span></span> 

<span data-ttu-id="58a29-p102">若要返回其他属性，必须使用 ODATA `$select` 查询参数指定所需的一组 [user](../resources/user.md) 属性。例如，若要返回 _displayName_、_givenName_、_id_ 和 _postalCode_，则需要将以下项添加到查询 `$select=displayName,givenName,postalCode`</span><span class="sxs-lookup"><span data-stu-id="58a29-p102">To return an alternative property set, you must specify the desired set of [user](../resources/user.md) properties using the ODATA `$select` query parameter. For example, to return _displayName_, _givenName_, _id_ and _postalCode_, you would use the add the following to your query `$select=displayName,givenName,postalCode`</span></span>

> <span data-ttu-id="58a29-p103">注意：某些属性无法在用户集合中返回。以下属性仅在[检索单个用户 ](./user_get.md) 时受支持：_aboutMe、birthday、hireDate、interests、mySite、pastProjects、preferredName、responsibilities、schools、skills、mailboxSettings_</span><span class="sxs-lookup"><span data-stu-id="58a29-p103">Note: Certain properties cannot be returned within a user collection. The following properties are only supported when [retrieving an single user](./user_get.md): _aboutMe, birthday, hireDate, interests, mySite, pastProjects, preferredName, responsibilities, schools, skills, mailboxSettings_</span></span>

## <a name="request-headers"></a><span data-ttu-id="58a29-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="58a29-122">Request headers</span></span>

| <span data-ttu-id="58a29-123">标头</span><span class="sxs-lookup"><span data-stu-id="58a29-123">Header</span></span>        | <span data-ttu-id="58a29-124">值</span><span class="sxs-lookup"><span data-stu-id="58a29-124">Value</span></span>                      |
|:--------------|:---------------------------|
| <span data-ttu-id="58a29-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="58a29-125">Authorization</span></span> | <span data-ttu-id="58a29-126">Bearer {token}（必需）</span><span class="sxs-lookup"><span data-stu-id="58a29-126">Bearer {token} (required)</span></span>  |
| <span data-ttu-id="58a29-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="58a29-127">Content-Type</span></span>  | <span data-ttu-id="58a29-128">application/json</span><span class="sxs-lookup"><span data-stu-id="58a29-128">application/json</span></span>           |

## <a name="request-body"></a><span data-ttu-id="58a29-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="58a29-129">Request body</span></span>

<span data-ttu-id="58a29-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="58a29-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="58a29-131">响应</span><span class="sxs-lookup"><span data-stu-id="58a29-131">Response</span></span>

<span data-ttu-id="58a29-132">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [user](../resources/user.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="58a29-132">If successful, this method returns a `200 OK` response code and collection of [user](../resources/user.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="58a29-133">示例</span><span class="sxs-lookup"><span data-stu-id="58a29-133">Example</span></span>

##### <a name="request"></a><span data-ttu-id="58a29-134">请求</span><span class="sxs-lookup"><span data-stu-id="58a29-134">Request</span></span>

<span data-ttu-id="58a29-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="58a29-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_users"
}-->
```http
GET https://graph.microsoft.com/v1.0/users
```

##### <a name="response"></a><span data-ttu-id="58a29-136">响应</span><span class="sxs-lookup"><span data-stu-id="58a29-136">Response</span></span>

<span data-ttu-id="58a29-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="58a29-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 608

{
  "value": [
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
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List users",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
