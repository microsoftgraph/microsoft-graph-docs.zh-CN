# <a name="list-registeredusers"></a><span data-ttu-id="38ff0-101">列出 registeredUser</span><span class="sxs-lookup"><span data-stu-id="38ff0-101">List registeredUsers</span></span>

<span data-ttu-id="38ff0-102">检索已注册为设备用户的用户列表。</span><span class="sxs-lookup"><span data-stu-id="38ff0-102">Retrieve a list of users that are registered users of the device.</span></span>

<span data-ttu-id="38ff0-103">对于云加入设备和已注册的个人设备，已注册用户在设备注册时设置为与已注册所有者相同的值。</span><span class="sxs-lookup"><span data-stu-id="38ff0-103">For cloud joined devices and registered personal devices, registered users are set to the same value as registered owners at the time of registration.</span></span>

## <a name="permissions"></a><span data-ttu-id="38ff0-104">权限</span><span class="sxs-lookup"><span data-stu-id="38ff0-104">Permissions</span></span>
<span data-ttu-id="38ff0-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="38ff0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>


|<span data-ttu-id="38ff0-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="38ff0-107">Permission type</span></span>      | <span data-ttu-id="38ff0-108">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="38ff0-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="38ff0-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="38ff0-109">Delegated (work or school account)</span></span> | <span data-ttu-id="38ff0-110">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="38ff0-110">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="38ff0-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="38ff0-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="38ff0-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="38ff0-112">Not supported.</span></span>    |
|<span data-ttu-id="38ff0-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="38ff0-113">Application</span></span> | <span data-ttu-id="38ff0-114">Directory.Read.All 或 Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="38ff0-114">Directory.Read.All or Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="38ff0-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="38ff0-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /devices/{id}/registeredUsers
```
## <a name="optional-query-parameters"></a><span data-ttu-id="38ff0-116">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="38ff0-116">Optional query parameters</span></span>
<span data-ttu-id="38ff0-117">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="38ff0-117">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="38ff0-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="38ff0-118">Request headers</span></span>
| <span data-ttu-id="38ff0-119">名称</span><span class="sxs-lookup"><span data-stu-id="38ff0-119">Name</span></span>       | <span data-ttu-id="38ff0-120">类型</span><span class="sxs-lookup"><span data-stu-id="38ff0-120">Type</span></span> | <span data-ttu-id="38ff0-121">说明</span><span class="sxs-lookup"><span data-stu-id="38ff0-121">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="38ff0-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="38ff0-122">Authorization</span></span>  | <span data-ttu-id="38ff0-123">string</span><span class="sxs-lookup"><span data-stu-id="38ff0-123">string</span></span>  | <span data-ttu-id="38ff0-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="38ff0-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="38ff0-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="38ff0-126">Request body</span></span>
<span data-ttu-id="38ff0-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="38ff0-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="38ff0-128">响应</span><span class="sxs-lookup"><span data-stu-id="38ff0-128">Response</span></span>

<span data-ttu-id="38ff0-129">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [directoryObject](../resources/directoryobject.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="38ff0-129">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="38ff0-130">示例</span><span class="sxs-lookup"><span data-stu-id="38ff0-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="38ff0-131">请求</span><span class="sxs-lookup"><span data-stu-id="38ff0-131">Request</span></span>
<span data-ttu-id="38ff0-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="38ff0-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_registeredusers"
}-->
```http
GET https://graph.microsoft.com/v1.0/devices/{id}/registeredUsers
```
##### <a name="response"></a><span data-ttu-id="38ff0-133">响应</span><span class="sxs-lookup"><span data-stu-id="38ff0-133">Response</span></span>
<span data-ttu-id="38ff0-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="38ff0-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "List registeredUsers",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->