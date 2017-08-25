# <a name="list-contacts"></a><span data-ttu-id="d53d3-101">列出联系人</span><span class="sxs-lookup"><span data-stu-id="d53d3-101">List contacts</span></span>

<span data-ttu-id="d53d3-102">从已登录用户的默认联系人文件夹中获取联系人集合。</span><span class="sxs-lookup"><span data-stu-id="d53d3-102">Get a contact collection from the default Contacts folder of the signed-in user.</span></span>
## <a name="permissions"></a><span data-ttu-id="d53d3-103">权限</span><span class="sxs-lookup"><span data-stu-id="d53d3-103">Permissions</span></span>
<span data-ttu-id="d53d3-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="d53d3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="d53d3-106">权限类型</span><span class="sxs-lookup"><span data-stu-id="d53d3-106">Permission type</span></span>      | <span data-ttu-id="d53d3-107">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d53d3-107">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="d53d3-108">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d53d3-108">Delegated (work or school account)</span></span> | <span data-ttu-id="d53d3-109">Contacts.Read、Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d53d3-109">Contacts.Read, Contacts.ReadWrite</span></span>    | 
|<span data-ttu-id="d53d3-110">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d53d3-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d53d3-111">Contacts.Read、Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d53d3-111">Contacts.Read, Contacts.ReadWrite</span></span>    | 
|<span data-ttu-id="d53d3-112">应用程序</span><span class="sxs-lookup"><span data-stu-id="d53d3-112">Application</span></span> | <span data-ttu-id="d53d3-113">Contacts.Read、Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d53d3-113">Contacts.Read, Contacts.ReadWrite</span></span> | 

## <a name="http-request"></a><span data-ttu-id="d53d3-114">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d53d3-114">HTTP request</span></span>

<span data-ttu-id="d53d3-115">若要获取用户邮箱中的所有联系人，请执行以下操作：</span><span class="sxs-lookup"><span data-stu-id="d53d3-115">To get all the contacts in a user's mailbox:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/contacts
GET /users/{id | userPrincipalName}/contacts
```

<span data-ttu-id="d53d3-116">若要获取用户邮箱中特定文件夹中的联系人，请执行以下操作：</span><span class="sxs-lookup"><span data-stu-id="d53d3-116">To get contacts in a specific folder in the user's mailbox:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/contactfolders/{Id}/contacts
GET /users/{id | userPrincipalName}/contactfolders/{id}/contacts

GET /me/contactFolder/{id}/childFolders/{id}/.../contacts
GET /users/{id | userPrincipalName}/contactFolders/{id}/childFolders/{id}/contacts
```
## <a name="optional-query-parameters"></a><span data-ttu-id="d53d3-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="d53d3-117">Optional query parameters</span></span>
<span data-ttu-id="d53d3-118">此方法支持 [OData 查询参数](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="d53d3-118">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="d53d3-119">例如，你可以使用 `$filter` 查询参数根据联系人的电子邮件地址的域来过滤联系人：</span><span class="sxs-lookup"><span data-stu-id="d53d3-119">For example, you can use the `$filter` query parameter to filter contacts based on the domain of their email addresses:</span></span>

`https://graph.microsoft.com/v1.0/me/contacts?$filter=emailAddresses/any(a:a/address eq '@domain.com')`



## <a name="request-headers"></a><span data-ttu-id="d53d3-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="d53d3-120">Request headers</span></span>
| <span data-ttu-id="d53d3-121">标头</span><span class="sxs-lookup"><span data-stu-id="d53d3-121">Header</span></span>       | <span data-ttu-id="d53d3-122">值</span><span class="sxs-lookup"><span data-stu-id="d53d3-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="d53d3-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="d53d3-123">Authorization</span></span>  | <span data-ttu-id="d53d3-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="d53d3-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="d53d3-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d53d3-126">Content-Type</span></span>   | <span data-ttu-id="d53d3-127">application/json</span><span class="sxs-lookup"><span data-stu-id="d53d3-127">application/json</span></span>  | 

## <a name="request-body"></a><span data-ttu-id="d53d3-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="d53d3-128">Request body</span></span>
<span data-ttu-id="d53d3-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="d53d3-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d53d3-130">响应</span><span class="sxs-lookup"><span data-stu-id="d53d3-130">Response</span></span>

<span data-ttu-id="d53d3-131">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [Contact](../resources/contact.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="d53d3-131">If successful, this method returns a `200 OK` response code and collection of [Contact](../resources/contact.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="d53d3-132">示例</span><span class="sxs-lookup"><span data-stu-id="d53d3-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d53d3-133">请求</span><span class="sxs-lookup"><span data-stu-id="d53d3-133">Request</span></span>
<span data-ttu-id="d53d3-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="d53d3-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_contacts"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/contacts
```


##### <a name="response"></a><span data-ttu-id="d53d3-135">响应</span><span class="sxs-lookup"><span data-stu-id="d53d3-135">Response</span></span>
<span data-ttu-id="d53d3-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="d53d3-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
