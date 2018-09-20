# <a name="list-contacts"></a><span data-ttu-id="a365d-101">列出联系人</span><span class="sxs-lookup"><span data-stu-id="a365d-101">List contacts</span></span>

<span data-ttu-id="a365d-102">从已登录用户的默认联系人文件夹中获取联系人集合。</span><span class="sxs-lookup"><span data-stu-id="a365d-102">Get a contact collection from the default Contacts folder of the signed-in user.</span></span>

<span data-ttu-id="a365d-103">有两种应用可以在另一个用户的联系人文件夹中获取联系人的情景：</span><span class="sxs-lookup"><span data-stu-id="a365d-103">There are two scenarios where an app can get contacts in another user's contact folder:</span></span>

* <span data-ttu-id="a365d-104">如果应用拥有应用程序权限，或者，</span><span class="sxs-lookup"><span data-stu-id="a365d-104">If the app has application permissions, or,</span></span>
* <span data-ttu-id="a365d-105">如果应用拥有来自一个用户的适当的委派[权限](#permissions)，而另一个用户与该用户共享了联系人文件夹，或者已授予该用户委派访问权限。</span><span class="sxs-lookup"><span data-stu-id="a365d-105">If the app has the appropriate delegated [permissions](#permissions) from one user, and another user has shared a contact folder with that user, or, has given delegated access to that user.</span></span> <span data-ttu-id="a365d-106">请参阅[详细信息和示例](../../../concepts/outlook-get-shared-contacts-folders.md)。</span><span class="sxs-lookup"><span data-stu-id="a365d-106">See [details and an example](../../../concepts/outlook-get-shared-contacts-folders.md).</span></span>


## <a name="permissions"></a><span data-ttu-id="a365d-107">权限</span><span class="sxs-lookup"><span data-stu-id="a365d-107">Permissions</span></span>
<span data-ttu-id="a365d-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="a365d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="a365d-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="a365d-110">Permission type</span></span>      | <span data-ttu-id="a365d-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a365d-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a365d-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a365d-112">Delegated (work or school account)</span></span> | <span data-ttu-id="a365d-113">Contacts.Read、Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a365d-113">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="a365d-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a365d-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a365d-115">Contacts.Read、Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a365d-115">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="a365d-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="a365d-116">Application</span></span> | <span data-ttu-id="a365d-117">Contacts.Read、Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a365d-117">Contacts.Read, Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="a365d-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a365d-118">HTTP request</span></span>

<span data-ttu-id="a365d-119">若要获取用户邮箱中的所有联系人，请执行以下操作：</span><span class="sxs-lookup"><span data-stu-id="a365d-119">To get all the contacts in a user's mailbox:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/contacts
GET /users/{id | userPrincipalName}/contacts
```

<span data-ttu-id="a365d-120">若要获取用户邮箱中特定文件夹中的联系人，请执行以下操作：</span><span class="sxs-lookup"><span data-stu-id="a365d-120">To get contacts in a specific folder in the user's mailbox:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/contactfolders/{Id}/contacts
GET /users/{id | userPrincipalName}/contactfolders/{id}/contacts

GET /me/contactFolder/{id}/childFolders/{id}/.../contacts
GET /users/{id | userPrincipalName}/contactFolders/{id}/childFolders/{id}/contacts
```
## <a name="optional-query-parameters"></a><span data-ttu-id="a365d-121">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="a365d-121">Optional query parameters</span></span>
<span data-ttu-id="a365d-122">此方法支持 [OData 查询参数](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="a365d-122">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="a365d-123">例如，你可以使用 `$filter` 查询参数根据联系人的电子邮件地址的域来过滤联系人：</span><span class="sxs-lookup"><span data-stu-id="a365d-123">For example, you can use the `$filter` query parameter to filter contacts based on the domain of their email addresses:</span></span>

`https://graph.microsoft.com/v1.0/me/contacts?$filter=emailAddresses/any(a:a/address eq '@domain.com')`



## <a name="request-headers"></a><span data-ttu-id="a365d-124">请求标头</span><span class="sxs-lookup"><span data-stu-id="a365d-124">Request headers</span></span>
| <span data-ttu-id="a365d-125">标头</span><span class="sxs-lookup"><span data-stu-id="a365d-125">Header</span></span>       | <span data-ttu-id="a365d-126">值</span><span class="sxs-lookup"><span data-stu-id="a365d-126">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="a365d-127">授权</span><span class="sxs-lookup"><span data-stu-id="a365d-127">Authorization</span></span>  | <span data-ttu-id="a365d-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="a365d-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="a365d-130">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a365d-130">Content-Type</span></span>   | <span data-ttu-id="a365d-131">application/json</span><span class="sxs-lookup"><span data-stu-id="a365d-131">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="a365d-132">请求正文</span><span class="sxs-lookup"><span data-stu-id="a365d-132">Request body</span></span>
<span data-ttu-id="a365d-133">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="a365d-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a365d-134">响应</span><span class="sxs-lookup"><span data-stu-id="a365d-134">Response</span></span>

<span data-ttu-id="a365d-135">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [Contact](../resources/contact.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="a365d-135">If successful, this method returns a `200 OK` response code and collection of [Contact](../resources/contact.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="a365d-136">示例</span><span class="sxs-lookup"><span data-stu-id="a365d-136">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a365d-137">请求</span><span class="sxs-lookup"><span data-stu-id="a365d-137">Request</span></span>
<span data-ttu-id="a365d-138">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="a365d-138">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_contacts"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/contacts
```


##### <a name="response"></a><span data-ttu-id="a365d-139">响应</span><span class="sxs-lookup"><span data-stu-id="a365d-139">Response</span></span>
<span data-ttu-id="a365d-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="a365d-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.contact",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 263

{
  "value": [
    {
      "parentFolderId": "parentFolderId-value",
      "birthday": "datetime-value",
      "fileAs": "fileAs-value",
      "displayName": "displayName-value",
      "givenName": "givenName-value",
      "initials": "initials-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List contacts",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
