# <a name="get-permission"></a><span data-ttu-id="8a8a5-101">获取权限</span><span class="sxs-lookup"><span data-stu-id="8a8a5-101">Get permission</span></span>

<span data-ttu-id="8a8a5-102">检索 permission 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="8a8a5-102">Retrieve the properties and relationships of permission object.</span></span>

## <a name="permissions"></a><span data-ttu-id="8a8a5-103">权限</span><span class="sxs-lookup"><span data-stu-id="8a8a5-103">Permissions</span></span>
<span data-ttu-id="8a8a5-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="8a8a5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="8a8a5-106">权限类型</span><span class="sxs-lookup"><span data-stu-id="8a8a5-106">Permission type</span></span>      | <span data-ttu-id="8a8a5-107">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="8a8a5-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8a8a5-108">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8a8a5-108">Delegated (work or school account)</span></span> | <span data-ttu-id="8a8a5-109">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8a8a5-109">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="8a8a5-110">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8a8a5-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8a8a5-111">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8a8a5-111">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="8a8a5-112">应用程序</span><span class="sxs-lookup"><span data-stu-id="8a8a5-112">Application</span></span> | <span data-ttu-id="8a8a5-113">Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8a8a5-113">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="8a8a5-114">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8a8a5-114">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/drive/items/{item-id}/permissions/{perm-id}
GET /me/drive/root:/{path}:/permissions/{perm-id}
GET /drives/{drive-id}/items/{item-id}/permissions/{perm-id}
GET /groups/{group-id}/drive/items/{item-id}/permissions/{perm-id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="8a8a5-115">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="8a8a5-115">Optional query parameters</span></span>
<span data-ttu-id="8a8a5-116">此方法支持 [OData 查询参数](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="8a8a5-116">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>

## <a name="request-body"></a><span data-ttu-id="8a8a5-117">请求正文</span><span class="sxs-lookup"><span data-stu-id="8a8a5-117">Request body</span></span>
<span data-ttu-id="8a8a5-118">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="8a8a5-118">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8a8a5-119">响应</span><span class="sxs-lookup"><span data-stu-id="8a8a5-119">Response</span></span>

<span data-ttu-id="8a8a5-120">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [权限](../resources/permission.md) 资源。</span><span class="sxs-lookup"><span data-stu-id="8a8a5-120">If successful, this method returns a `200 OK` response code and [Permission](../resources/permission.md) resource in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8a8a5-121">示例</span><span class="sxs-lookup"><span data-stu-id="8a8a5-121">Example</span></span>

##### <a name="request"></a><span data-ttu-id="8a8a5-122">请求</span><span class="sxs-lookup"><span data-stu-id="8a8a5-122">Request</span></span>

<span data-ttu-id="8a8a5-123">下面是请求访问根文件夹权限的示例。</span><span class="sxs-lookup"><span data-stu-id="8a8a5-123">Here is an example of the request to access a permission on the root folder.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_permission"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{item-id}/permissions/{perm-id}
```
##### <a name="response"></a><span data-ttu-id="8a8a5-124">响应</span><span class="sxs-lookup"><span data-stu-id="8a8a5-124">Response</span></span>
<span data-ttu-id="8a8a5-125">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="8a8a5-125">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.permission"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 762

{
  "grantedTo": {
    "user": {
      "displayName": "Ryan Gregg",
      "id": "efee1b77-fb3b-4f65-99d6-274c11914d12"
    }
  },
  "id": "1",
  "roles": [ "write" ]
}
```

## <a name="remarks"></a><span data-ttu-id="8a8a5-126">注解</span><span class="sxs-lookup"><span data-stu-id="8a8a5-126">Remarks</span></span>

<span data-ttu-id="8a8a5-127">[权限](../resources/permission.md) 资源使用 _facet_ 提供有关由该资源表示的权限类型的信息。</span><span class="sxs-lookup"><span data-stu-id="8a8a5-127">The [Permission](../resources/permission.md) resource uses _facets_ to provide information about the kind of permission represented by the resource.</span></span>

<span data-ttu-id="8a8a5-p102">具有 [**链接**](../resources/sharinglink.md) facet 的权限表示在该项上创建的共享链接。共享链接包含一个唯一令牌，可以为具有上述链接的任何人提供对项目的访问权限。</span><span class="sxs-lookup"><span data-stu-id="8a8a5-p102">Permissions with a [**link**](../resources/sharinglink.md) facet represent sharing links created on the item. Sharing links contain a unique token that provides access to the item for anyone with the link.</span></span>

<span data-ttu-id="8a8a5-130">具有 [**邀请**](../resources/sharinginvitation.md) facet 的权限表示通过邀请特定用户或组访问该文件添加的权限。</span><span class="sxs-lookup"><span data-stu-id="8a8a5-130">Permissions with a [**invitation**](../resources/sharinginvitation.md) facet represent permissions added by inviting specific users or groups to have access to the file.</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get permission",
  "keywords": "",
  "section": "documentation",
  "tocPath": "OneDrive/Item/Get permission"
}-->
