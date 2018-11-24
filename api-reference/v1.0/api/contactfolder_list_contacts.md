# <a name="list-contacts"></a><span data-ttu-id="30aea-101">列出联系人</span><span class="sxs-lookup"><span data-stu-id="30aea-101">List contacts</span></span>

<span data-ttu-id="30aea-102">从已登录用户的默认联系人文件夹 (`.../me/contacts`) 或从指定的联系人文件夹中获取联系人集合。</span><span class="sxs-lookup"><span data-stu-id="30aea-102">Get a contact collection from the default Contacts folder of the signed-in user (`.../me/contacts`), or from the specified contact folder.</span></span>
## <a name="permissions"></a><span data-ttu-id="30aea-103">权限</span><span class="sxs-lookup"><span data-stu-id="30aea-103">Permissions</span></span>
<span data-ttu-id="30aea-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="30aea-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="30aea-106">权限类型</span><span class="sxs-lookup"><span data-stu-id="30aea-106">Permission type</span></span>      | <span data-ttu-id="30aea-107">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="30aea-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="30aea-108">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="30aea-108">Delegated (work or school account)</span></span> | <span data-ttu-id="30aea-109">Contacts.Read、Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="30aea-109">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="30aea-110">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="30aea-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="30aea-111">Contacts.Read、Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="30aea-111">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="30aea-112">应用程序</span><span class="sxs-lookup"><span data-stu-id="30aea-112">Application</span></span> | <span data-ttu-id="30aea-113">Contacts.Read、Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="30aea-113">Contacts.Read, Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="30aea-114">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="30aea-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/contacts
GET /users/{id | userPrincipalName}/contacts

GET /me/contactFolders/{id}/contacts
GET /users/{id | userPrincipalName}/contactFolders/{id}/contacts
```
## <a name="optional-query-parameters"></a><span data-ttu-id="30aea-115">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="30aea-115">Optional query parameters</span></span>
<span data-ttu-id="30aea-116">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="30aea-116">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="30aea-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="30aea-117">Request headers</span></span>
| <span data-ttu-id="30aea-118">名称</span><span class="sxs-lookup"><span data-stu-id="30aea-118">Name</span></span>       | <span data-ttu-id="30aea-119">类型</span><span class="sxs-lookup"><span data-stu-id="30aea-119">Type</span></span> | <span data-ttu-id="30aea-120">说明</span><span class="sxs-lookup"><span data-stu-id="30aea-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="30aea-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="30aea-121">Authorization</span></span>  | <span data-ttu-id="30aea-122">string</span><span class="sxs-lookup"><span data-stu-id="30aea-122">string</span></span>  | <span data-ttu-id="30aea-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="30aea-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="30aea-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="30aea-125">Request body</span></span>
<span data-ttu-id="30aea-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="30aea-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="30aea-127">响应</span><span class="sxs-lookup"><span data-stu-id="30aea-127">Response</span></span>

<span data-ttu-id="30aea-128">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [Contact](../resources/contact.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="30aea-128">If successful, this method returns a `200 OK` response code and collection of [Contact](../resources/contact.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="30aea-129">示例</span><span class="sxs-lookup"><span data-stu-id="30aea-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="30aea-130">请求</span><span class="sxs-lookup"><span data-stu-id="30aea-130">Request</span></span>
<span data-ttu-id="30aea-131">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="30aea-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_contacts"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/contactFolders/{id}/contacts
```
##### <a name="response"></a><span data-ttu-id="30aea-132">响应</span><span class="sxs-lookup"><span data-stu-id="30aea-132">Response</span></span>
<span data-ttu-id="30aea-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="30aea-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
