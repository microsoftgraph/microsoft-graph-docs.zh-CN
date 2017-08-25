# <a name="list-devices"></a><span data-ttu-id="c3087-101">列出设备</span><span class="sxs-lookup"><span data-stu-id="c3087-101">List devices</span></span>

<span data-ttu-id="c3087-102">检索组织中注册的 device 对象的列表。</span><span class="sxs-lookup"><span data-stu-id="c3087-102">Retrieve a list of device objects registered in the organization.</span></span>

## <a name="permissions"></a><span data-ttu-id="c3087-103">权限</span><span class="sxs-lookup"><span data-stu-id="c3087-103">Permissions</span></span>
<span data-ttu-id="c3087-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="c3087-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>


|<span data-ttu-id="c3087-106">权限类型</span><span class="sxs-lookup"><span data-stu-id="c3087-106">Permission type</span></span>      | <span data-ttu-id="c3087-107">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c3087-107">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="c3087-108">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c3087-108">Delegated (work or school account)</span></span> | <span data-ttu-id="c3087-109">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="c3087-109">One of the following scopes is required to execute this API: Directory.Read.All; Directory.ReadWrite.All; Directory.AccessAsUser.All</span></span>    | 
|<span data-ttu-id="c3087-110">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c3087-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c3087-111">不支持。</span><span class="sxs-lookup"><span data-stu-id="c3087-111">Not supported.</span></span>    | 
|<span data-ttu-id="c3087-112">应用程序</span><span class="sxs-lookup"><span data-stu-id="c3087-112">Application</span></span> | <span data-ttu-id="c3087-113">Device.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c3087-113">Device.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="c3087-114">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c3087-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /devices
```
## <a name="optional-query-parameters"></a><span data-ttu-id="c3087-115">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="c3087-115">Optional query parameters</span></span>
<span data-ttu-id="c3087-116">此方法支持 [OData 查询参数](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="c3087-116">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="c3087-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="c3087-117">Request headers</span></span>
| <span data-ttu-id="c3087-118">名称</span><span class="sxs-lookup"><span data-stu-id="c3087-118">Name</span></span>       | <span data-ttu-id="c3087-119">类型</span><span class="sxs-lookup"><span data-stu-id="c3087-119">Type</span></span> | <span data-ttu-id="c3087-120">说明</span><span class="sxs-lookup"><span data-stu-id="c3087-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="c3087-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="c3087-121">Authorization</span></span>  | <span data-ttu-id="c3087-122">string</span><span class="sxs-lookup"><span data-stu-id="c3087-122">string</span></span>  | <span data-ttu-id="c3087-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="c3087-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c3087-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="c3087-125">Request body</span></span>
<span data-ttu-id="c3087-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="c3087-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c3087-127">响应</span><span class="sxs-lookup"><span data-stu-id="c3087-127">Response</span></span>

<span data-ttu-id="c3087-128">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [device](../resources/device.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="c3087-128">If successful, this method returns a `200 OK` response code and collection of [device](../resources/device.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="c3087-129">示例</span><span class="sxs-lookup"><span data-stu-id="c3087-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c3087-130">请求</span><span class="sxs-lookup"><span data-stu-id="c3087-130">Request</span></span>
<span data-ttu-id="c3087-131">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="c3087-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_devices"
}-->
```http
GET https://graph.microsoft.com/v1.0/devices
```

##### <a name="response"></a><span data-ttu-id="c3087-132">响应</span><span class="sxs-lookup"><span data-stu-id="c3087-132">Response</span></span>
<span data-ttu-id="c3087-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="c3087-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.device",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "accountEnabled":false,
      "alternativeSecurityIds":
      [
        {
          "type":2,
          "key":"Y3YxN2E1MWFlYw==",
          "identityProvider": null
        }
      ],
      "deviceId":"4c299165-6e8f-4b45-a5ba-c5d250a707ff",
      "displayName":"Test device",
      "id": "id-value",
      "operatingSystem":"linux",
      "operatingSystemVersion":"1"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List devices",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
