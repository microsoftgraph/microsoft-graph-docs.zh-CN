# <a name="list-registeredowners"></a><span data-ttu-id="fde54-101">列出 registeredOwner</span><span class="sxs-lookup"><span data-stu-id="fde54-101">List registeredOwners</span></span>

<span data-ttu-id="fde54-102">检索身份为已注册设备的所有者的用户列表。</span><span class="sxs-lookup"><span data-stu-id="fde54-102">Retrieve a list of users that are registered owners of the device.</span></span> <span data-ttu-id="fde54-103">已注册的所有者是云加入设备或已注册个人设备的用户。</span><span class="sxs-lookup"><span data-stu-id="fde54-103">A registered owner is the user that cloud joined the device or registered their personal device.</span></span> <span data-ttu-id="fde54-104">已注册的所有者是在注册时设置。</span><span class="sxs-lookup"><span data-stu-id="fde54-104">The registered owner is set at the time of registration.</span></span> <span data-ttu-id="fde54-105">目前，只能有一个所有者。</span><span class="sxs-lookup"><span data-stu-id="fde54-105">Currently, there can be only one owner.</span></span>

## <a name="permissions"></a><span data-ttu-id="fde54-106">权限</span><span class="sxs-lookup"><span data-stu-id="fde54-106">Permissions</span></span>
<span data-ttu-id="fde54-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="fde54-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>


|<span data-ttu-id="fde54-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="fde54-109">Permission type</span></span>      | <span data-ttu-id="fde54-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="fde54-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fde54-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="fde54-111">Delegated (work or school account)</span></span> | <span data-ttu-id="fde54-112">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="fde54-112">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="fde54-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="fde54-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fde54-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="fde54-114">Not supported.</span></span>    |
|<span data-ttu-id="fde54-115">应用</span><span class="sxs-lookup"><span data-stu-id="fde54-115">Application</span></span> | <span data-ttu-id="fde54-116">Device.ReadWrite.All 和 User.ReadBasic.All 或 Directory.Read.All 或 Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fde54-116">Device.ReadWrite.All and User.ReadBasic.All or Directory.Read.All or Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="fde54-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="fde54-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /devices/{id}/registeredOwners
```
## <a name="optional-query-parameters"></a><span data-ttu-id="fde54-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="fde54-118">Optional query parameters</span></span>
<span data-ttu-id="fde54-119">此方法支持 [OData 查询参数](http://developer.microsoft.com/zh-CN/graph/docs/overview/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="fde54-119">This method supports the [OData Query Parameters](http://developer.microsoft.com/zh-CN/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="fde54-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="fde54-120">Request headers</span></span>
| <span data-ttu-id="fde54-121">名称</span><span class="sxs-lookup"><span data-stu-id="fde54-121">Name</span></span>       | <span data-ttu-id="fde54-122">类型</span><span class="sxs-lookup"><span data-stu-id="fde54-122">Type</span></span> | <span data-ttu-id="fde54-123">说明</span><span class="sxs-lookup"><span data-stu-id="fde54-123">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="fde54-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="fde54-124">Authorization</span></span>  | <span data-ttu-id="fde54-125">string</span><span class="sxs-lookup"><span data-stu-id="fde54-125">string</span></span>  | <span data-ttu-id="fde54-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="fde54-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="fde54-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="fde54-128">Request body</span></span>
<span data-ttu-id="fde54-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="fde54-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fde54-130">响应</span><span class="sxs-lookup"><span data-stu-id="fde54-130">Response</span></span>

<span data-ttu-id="fde54-131">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [directoryObject](../resources/directoryobject.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="fde54-131">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="fde54-132">示例</span><span class="sxs-lookup"><span data-stu-id="fde54-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="fde54-133">请求</span><span class="sxs-lookup"><span data-stu-id="fde54-133">Request</span></span>
<span data-ttu-id="fde54-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="fde54-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_registeredowners"
}-->
```http
GET https://graph.microsoft.com/v1.0/devices/{id}/registeredOwners
```
##### <a name="response"></a><span data-ttu-id="fde54-135">响应</span><span class="sxs-lookup"><span data-stu-id="fde54-135">Response</span></span>
<span data-ttu-id="fde54-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="fde54-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 55

{
  "value": [
    {
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List registeredOwners",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->