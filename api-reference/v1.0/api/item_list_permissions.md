# <a name="list-permissions-on-a-driveitem"></a><span data-ttu-id="63a0d-101">列出 DriveItem 中的权限</span><span class="sxs-lookup"><span data-stu-id="63a0d-101">List permissions on a DriveItem</span></span>

<span data-ttu-id="63a0d-102">列出 [DriveItem](../resources/driveitem.md) 中的有效权限。</span><span class="sxs-lookup"><span data-stu-id="63a0d-102">List the effective permissions of on a [DriveItem](../resources/driveitem.md).</span></span>

<span data-ttu-id="63a0d-p101">不能在 [获取 DriveItem](item_get.md) 的调用过程中或 DriveItem 集合中扩展 DriveItem 的**权限**关系。必须直接访问权限属性。</span><span class="sxs-lookup"><span data-stu-id="63a0d-p101">The **permissions** relationship of DriveItem cannot be expanded as part of a call to [get DriveItem](item_get.md) or a collection of DriveItems. You must access the permissions property directly.</span></span>

## <a name="access-to-permissions"></a><span data-ttu-id="63a0d-105">访问权限</span><span class="sxs-lookup"><span data-stu-id="63a0d-105">Access to Permissions</span></span>

<span data-ttu-id="63a0d-106">权限集合包括潜在的敏感信息，不可能适用于每个调用方。</span><span class="sxs-lookup"><span data-stu-id="63a0d-106">The permissions collection includes potentially sensitive information and may not be available for every caller.</span></span>

* <span data-ttu-id="63a0d-p102">对于该项目的所有者，将返回所有权限。这包括共有者。</span><span class="sxs-lookup"><span data-stu-id="63a0d-p102">For the owner of the item, all permissions will be returned. This includes co-owners.</span></span>
* <span data-ttu-id="63a0d-109">对于非所有者的调用方，仅返回应用于调用方的权限。</span><span class="sxs-lookup"><span data-stu-id="63a0d-109">For a non-owner caller, only the permissions that apply to the caller are returned.</span></span>
* <span data-ttu-id="63a0d-110">对于能够创建 Permission 的调用方，仅返回包含机密信息（例如 `shareId` 和 `webUrl`）的 Permission 属性。</span><span class="sxs-lookup"><span data-stu-id="63a0d-110">Permission properties that contain secrets (e.g. `shareId` and `webUrl`) are only returned for callers that are able to create the Permission.</span></span>

## <a name="permissions"></a><span data-ttu-id="63a0d-111">权限</span><span class="sxs-lookup"><span data-stu-id="63a0d-111">Permissions</span></span>
<span data-ttu-id="63a0d-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="63a0d-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="63a0d-114">权限类型</span><span class="sxs-lookup"><span data-stu-id="63a0d-114">Permission type</span></span>      | <span data-ttu-id="63a0d-115">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="63a0d-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="63a0d-116">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="63a0d-116">Delegated (work or school account)</span></span> | <span data-ttu-id="63a0d-117">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="63a0d-117">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="63a0d-118">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="63a0d-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="63a0d-119">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="63a0d-119">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="63a0d-120">应用程序</span><span class="sxs-lookup"><span data-stu-id="63a0d-120">Application</span></span> | <span data-ttu-id="63a0d-121">Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="63a0d-121">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="63a0d-122">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="63a0d-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/drive/items/{item-id}/permissions
GET /me/drive/root:/{path}:/permissions
GET /drives/{drive-id}/items/{item-id}/permissions
GET /groups/{group-id}/drive/items/{item-id}/permissions
```

## <a name="request-headers"></a><span data-ttu-id="63a0d-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="63a0d-123">Request headers</span></span>

| <span data-ttu-id="63a0d-124">名称</span><span class="sxs-lookup"><span data-stu-id="63a0d-124">Name</span></span>          | <span data-ttu-id="63a0d-125">类型</span><span class="sxs-lookup"><span data-stu-id="63a0d-125">Type</span></span>   | <span data-ttu-id="63a0d-126">说明</span><span class="sxs-lookup"><span data-stu-id="63a0d-126">Description</span></span>                                                                                                                                     |
|:--------------|:-------|:------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="63a0d-127">if-none-match</span><span class="sxs-lookup"><span data-stu-id="63a0d-127">if-none-match</span></span> | <span data-ttu-id="63a0d-128">string</span><span class="sxs-lookup"><span data-stu-id="63a0d-128">string</span></span> | <span data-ttu-id="63a0d-129">如果包含此请求头，且提供的 eTag 与项中的当前 etag 不匹配，则返回 `HTTP 304 Not Modified` 响应。</span><span class="sxs-lookup"><span data-stu-id="63a0d-129">If this request header is included and the etag provided matches the current etag on the item, an `HTTP 304 Not Modified` response is returned.</span></span> |

## <a name="optional-query-parameters"></a><span data-ttu-id="63a0d-130">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="63a0d-130">Optional query parameters</span></span>
<span data-ttu-id="63a0d-131">此方法支持 [OData 查询参数](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="63a0d-131">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>

## <a name="request-body"></a><span data-ttu-id="63a0d-132">请求正文</span><span class="sxs-lookup"><span data-stu-id="63a0d-132">Request body</span></span>
<span data-ttu-id="63a0d-133">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="63a0d-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="63a0d-134">响应</span><span class="sxs-lookup"><span data-stu-id="63a0d-134">Response</span></span>

<span data-ttu-id="63a0d-135">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [权限](../resources/permission.md) 资源集合。</span><span class="sxs-lookup"><span data-stu-id="63a0d-135">If successful, this method returns a `200 OK` response code and collection of [Permission](../resources/permission.md) resources in the response body.</span></span>

<span data-ttu-id="63a0d-136">项目的有效权限可能来自两个源：</span><span class="sxs-lookup"><span data-stu-id="63a0d-136">Effective permissions of an item can come from two sources:</span></span>

* <span data-ttu-id="63a0d-137">直接对项目本身应用的权限</span><span class="sxs-lookup"><span data-stu-id="63a0d-137">Permissions applied directly on the item itself</span></span>
* <span data-ttu-id="63a0d-138">从项目的上级继承的权限</span><span class="sxs-lookup"><span data-stu-id="63a0d-138">Permissions inherited from the item's ancestors</span></span>

<span data-ttu-id="63a0d-p104">调用方可以通过检查 **inheritedFrom** 属性来区分是否为继承权限。此属性是引用从中继承该权限的上级的 [**itemReference**](../resources/itemreference.md) 资源。</span><span class="sxs-lookup"><span data-stu-id="63a0d-p104">Callers can differentiate if the permission is inherited or not by checking the **inheritedFrom** property. This property is an [**itemReference**](../resources/itemreference.md) resource referencing the ancestor that the permission is inherited from.</span></span>

## <a name="example"></a><span data-ttu-id="63a0d-141">示例</span><span class="sxs-lookup"><span data-stu-id="63a0d-141">Example</span></span>
##### <a name="request"></a><span data-ttu-id="63a0d-142">请求</span><span class="sxs-lookup"><span data-stu-id="63a0d-142">Request</span></span>
<span data-ttu-id="63a0d-143">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="63a0d-143">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_permissions"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{item-id}/permissions
```


##### <a name="response"></a><span data-ttu-id="63a0d-144">响应</span><span class="sxs-lookup"><span data-stu-id="63a0d-144">Response</span></span>
<span data-ttu-id="63a0d-145">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="63a0d-145">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.permission",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "id": "1",
      "roles": ["write"],
      "link": {
        "webUrl": "https://onedrive.live.com/redir?resid=5D33DD65C6932946!70859&authkey=!AL7N1QAfSWcjNU8&ithint=folder%2cgif",
        "type": "edit"
      }
    },
    {
      "id": "2",
      "roles": ["write"],
      "grantedTo": {
        "user": {
          "id": "5D33DD65C6932946",
          "displayName": "John Doe"
        }
      },
      "inheritedFrom": {
        "driveId": "1234567890ABD",
        "id": "1234567890ABC!123",
        "path": "/drive/root:/Documents" }
    },
    {
      "id": "3",
      "roles": ["write"],
      "link": {
        "webUrl": "https://onedrive.live.com/redir?resid=5D33DD65C6932946!70859&authkey=!AL7N1QAfSWcjNU8&ithint=folder%2cgif",
        "type": "edit",
        "application": {
          "id": "12345",
          "displayName": "TimeTravelPlus"
        }
      }
    }
  ]
}
```

<span data-ttu-id="63a0d-146">有关检索单个权限资源的详细信息，请参阅 [获取权限](permission_get.md)。</span><span class="sxs-lookup"><span data-stu-id="63a0d-146">See [Get permission](permission_get.md) for more details on retrieving a single permission resource.</span></span>


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List permissions",
  "keywords": "",
  "section": "documentation",
  "tocPath": "OneDrive/Item/List permissions"
}-->
