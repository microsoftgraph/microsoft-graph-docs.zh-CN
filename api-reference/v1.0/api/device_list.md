# <a name="list-devices"></a><span data-ttu-id="bb5d8-101">列出设备</span><span class="sxs-lookup"><span data-stu-id="bb5d8-101">List devices</span></span>

<span data-ttu-id="bb5d8-102">检索组织中注册的 device 对象的列表。</span><span class="sxs-lookup"><span data-stu-id="bb5d8-102">Retrieve a list of device objects registered in the organization.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bb5d8-103">先决条件</span><span class="sxs-lookup"><span data-stu-id="bb5d8-103">Prerequisites</span></span>
<span data-ttu-id="bb5d8-104">要执行此 API，需要以下**范围**之一：*Device.ReadWrite.All* 或 *Directory.Read.All* 或 *Directory.ReadWrite.All* 或 *Directory.AccessAsUser.All*</span><span class="sxs-lookup"><span data-stu-id="bb5d8-104">One of the following **scopes** is required to execute this API: *Device.ReadWrite.All* or *Directory.Read.All* or *Directory.ReadWrite.All* or *Directory.AccessAsUser.All*</span></span>

## <a name="http-request"></a><span data-ttu-id="bb5d8-105">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="bb5d8-105">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /devices
```
## <a name="optional-query-parameters"></a><span data-ttu-id="bb5d8-106">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="bb5d8-106">Optional query parameters</span></span>
<span data-ttu-id="bb5d8-107">此方法支持 [OData 查询参数](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="bb5d8-107">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="bb5d8-108">请求标头</span><span class="sxs-lookup"><span data-stu-id="bb5d8-108">Request headers</span></span>
| <span data-ttu-id="bb5d8-109">名称</span><span class="sxs-lookup"><span data-stu-id="bb5d8-109">Name</span></span>       | <span data-ttu-id="bb5d8-110">类型</span><span class="sxs-lookup"><span data-stu-id="bb5d8-110">Type</span></span> | <span data-ttu-id="bb5d8-111">说明</span><span class="sxs-lookup"><span data-stu-id="bb5d8-111">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="bb5d8-112">Authorization</span><span class="sxs-lookup"><span data-stu-id="bb5d8-112">Authorization</span></span>  | <span data-ttu-id="bb5d8-113">string</span><span class="sxs-lookup"><span data-stu-id="bb5d8-113">string</span></span>  | <span data-ttu-id="bb5d8-p101">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="bb5d8-p101">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="bb5d8-116">请求正文</span><span class="sxs-lookup"><span data-stu-id="bb5d8-116">Request body</span></span>
<span data-ttu-id="bb5d8-117">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="bb5d8-117">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bb5d8-118">响应</span><span class="sxs-lookup"><span data-stu-id="bb5d8-118">Response</span></span>

<span data-ttu-id="bb5d8-119">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [device](../resources/device.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="bb5d8-119">If successful, this method returns a `200 OK` response code and collection of [device](../resources/device.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="bb5d8-120">示例</span><span class="sxs-lookup"><span data-stu-id="bb5d8-120">Example</span></span>
##### <a name="request"></a><span data-ttu-id="bb5d8-121">请求</span><span class="sxs-lookup"><span data-stu-id="bb5d8-121">Request</span></span>
<span data-ttu-id="bb5d8-122">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="bb5d8-122">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_devices"
}-->
```http
GET https://graph.microsoft.com/v1.0/devices
```

##### <a name="response"></a><span data-ttu-id="bb5d8-123">响应</span><span class="sxs-lookup"><span data-stu-id="bb5d8-123">Response</span></span>
<span data-ttu-id="bb5d8-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="bb5d8-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
