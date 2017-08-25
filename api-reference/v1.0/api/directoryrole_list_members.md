# <a name="list-members"></a><span data-ttu-id="e17dd-101">列出成员</span><span class="sxs-lookup"><span data-stu-id="e17dd-101">List members</span></span>

<span data-ttu-id="e17dd-p101">检索分配给目录角色的用户列表。只能将用户分配给目录角色。</span><span class="sxs-lookup"><span data-stu-id="e17dd-p101">Retrieve a list of the users that are assigned to the directory role.  Only users can be assigned to a directory role.</span></span>
## <a name="permissions"></a><span data-ttu-id="e17dd-104">权限</span><span class="sxs-lookup"><span data-stu-id="e17dd-104">Permissions</span></span>
<span data-ttu-id="e17dd-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="e17dd-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>


|<span data-ttu-id="e17dd-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="e17dd-107">Permission type</span></span>      | <span data-ttu-id="e17dd-108">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e17dd-108">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="e17dd-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e17dd-109">Delegated (work or school account)</span></span> | <span data-ttu-id="e17dd-110">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="e17dd-110">One of the following scopes is required to execute this API: Directory.Read.All; Directory.ReadWrite.All; Directory.AccessAsUser.All</span></span>    | 
|<span data-ttu-id="e17dd-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e17dd-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e17dd-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="e17dd-112">Not supported.</span></span>    | 
|<span data-ttu-id="e17dd-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="e17dd-113">Application</span></span> | <span data-ttu-id="e17dd-114">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e17dd-114">Directory.Read.All, Directory.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="e17dd-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e17dd-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /directoryRoles/{id}/members
```
## <a name="optional-query-parameters"></a><span data-ttu-id="e17dd-116">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="e17dd-116">Optional query parameters</span></span>
<span data-ttu-id="e17dd-117">此方法支持 [OData 查询参数](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="e17dd-117">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="e17dd-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="e17dd-118">Request headers</span></span>
| <span data-ttu-id="e17dd-119">名称</span><span class="sxs-lookup"><span data-stu-id="e17dd-119">Name</span></span>       | <span data-ttu-id="e17dd-120">类型</span><span class="sxs-lookup"><span data-stu-id="e17dd-120">Type</span></span> | <span data-ttu-id="e17dd-121">说明</span><span class="sxs-lookup"><span data-stu-id="e17dd-121">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="e17dd-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="e17dd-122">Authorization</span></span>  | <span data-ttu-id="e17dd-123">string</span><span class="sxs-lookup"><span data-stu-id="e17dd-123">string</span></span>  | <span data-ttu-id="e17dd-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="e17dd-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e17dd-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="e17dd-126">Request body</span></span>
<span data-ttu-id="e17dd-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="e17dd-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e17dd-128">响应</span><span class="sxs-lookup"><span data-stu-id="e17dd-128">Response</span></span>

<span data-ttu-id="e17dd-129">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [directoryObject](../resources/directoryobject.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="e17dd-129">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="e17dd-130">示例</span><span class="sxs-lookup"><span data-stu-id="e17dd-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e17dd-131">请求</span><span class="sxs-lookup"><span data-stu-id="e17dd-131">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_members"
}-->
```http
GET https://graph.microsoft.com/v1.0/directoryRoles/{id}/members
```
##### <a name="response"></a><span data-ttu-id="e17dd-132">响应</span><span class="sxs-lookup"><span data-stu-id="e17dd-132">Response</span></span>
<span data-ttu-id="e17dd-p104">注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="e17dd-p104">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "businessPhones":["000-000-0000"],
      "displayName":"First Last",
      "givenName":"First",
      "jobTitle":null,
      "mail":"first@example.com",
      "officeLocation":null,
      "preferredLanguage":"en-US",
      "surname":"Last",
      "userPrincipalName":"first@example.com"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List members",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->