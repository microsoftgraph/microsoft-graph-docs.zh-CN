# <a name="get-device"></a><span data-ttu-id="2f506-101">获取设备</span><span class="sxs-lookup"><span data-stu-id="2f506-101">Get device</span></span>

<span data-ttu-id="2f506-102">获取 device 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="2f506-102">Get the properties and relationships of a device object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="2f506-103">先决条件</span><span class="sxs-lookup"><span data-stu-id="2f506-103">Prerequisites</span></span>
<span data-ttu-id="2f506-104">要执行此 API，需要以下**范围**之一：*Device.ReadWrite.All* 或 *Directory.Read.All* 或 *Directory.ReadWrite.All* 或 *Directory.AccessAsUser.All*</span><span class="sxs-lookup"><span data-stu-id="2f506-104">One of the following **scopes** is required to execute this API: *Device.ReadWrite.All* or *Directory.Read.All* or *Directory.ReadWrite.All* or *Directory.AccessAsUser.All*</span></span>

## <a name="http-request"></a><span data-ttu-id="2f506-105">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2f506-105">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /devices/{id}
```
> <span data-ttu-id="2f506-106">注意：请求中的“id”是设备的“id”属性，不是“deviceId”属性。</span><span class="sxs-lookup"><span data-stu-id="2f506-106">Note: The "id" in the request is the "id" property of the device, not the "deviceId" property.</span></span>

## <a name="optional-query-parameters"></a><span data-ttu-id="2f506-107">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="2f506-107">Optional query parameters</span></span>
<span data-ttu-id="2f506-108">此方法支持 [OData 查询参数](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="2f506-108">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2f506-109">请求标头</span><span class="sxs-lookup"><span data-stu-id="2f506-109">Request headers</span></span>
| <span data-ttu-id="2f506-110">名称</span><span class="sxs-lookup"><span data-stu-id="2f506-110">Name</span></span>       | <span data-ttu-id="2f506-111">类型</span><span class="sxs-lookup"><span data-stu-id="2f506-111">Type</span></span> | <span data-ttu-id="2f506-112">说明</span><span class="sxs-lookup"><span data-stu-id="2f506-112">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="2f506-113">Authorization</span><span class="sxs-lookup"><span data-stu-id="2f506-113">Authorization</span></span>  | <span data-ttu-id="2f506-114">string</span><span class="sxs-lookup"><span data-stu-id="2f506-114">string</span></span>  | <span data-ttu-id="2f506-p101">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="2f506-p101">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2f506-117">请求正文</span><span class="sxs-lookup"><span data-stu-id="2f506-117">Request body</span></span>
<span data-ttu-id="2f506-118">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="2f506-118">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2f506-119">响应</span><span class="sxs-lookup"><span data-stu-id="2f506-119">Response</span></span>

<span data-ttu-id="2f506-120">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [device](../resources/device.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="2f506-120">If successful, this method returns a `200 OK` response code and [device](../resources/device.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="2f506-121">示例</span><span class="sxs-lookup"><span data-stu-id="2f506-121">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2f506-122">请求</span><span class="sxs-lookup"><span data-stu-id="2f506-122">Request</span></span>
<span data-ttu-id="2f506-123">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="2f506-123">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_device"
}-->
```http
GET https://graph.microsoft.com/v1.0/devices/{id}
```
##### <a name="response"></a><span data-ttu-id="2f506-124">响应</span><span class="sxs-lookup"><span data-stu-id="2f506-124">Response</span></span>
<span data-ttu-id="2f506-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="2f506-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.device"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "accountEnabled":false,
  "alternativeSecurityIds":
  [
    {
      "type": 2,
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
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get device",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
