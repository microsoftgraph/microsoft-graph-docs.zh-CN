# <a name="get-device"></a><span data-ttu-id="7a61b-101">获取设备</span><span class="sxs-lookup"><span data-stu-id="7a61b-101">Get device</span></span>

<span data-ttu-id="7a61b-102">获取 device 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="7a61b-102">Get the properties and relationships of a device object.</span></span>
## <a name="permissions"></a><span data-ttu-id="7a61b-103">权限</span><span class="sxs-lookup"><span data-stu-id="7a61b-103">Permissions</span></span>
<span data-ttu-id="7a61b-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="7a61b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>


|<span data-ttu-id="7a61b-106">权限类型</span><span class="sxs-lookup"><span data-stu-id="7a61b-106">Permission type</span></span>      | <span data-ttu-id="7a61b-107">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="7a61b-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7a61b-108">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7a61b-108">Delegated (work or school account)</span></span> | <span data-ttu-id="7a61b-109">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="7a61b-109">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="7a61b-110">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7a61b-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7a61b-111">不支持。</span><span class="sxs-lookup"><span data-stu-id="7a61b-111">Not supported.</span></span>    |
|<span data-ttu-id="7a61b-112">应用程序</span><span class="sxs-lookup"><span data-stu-id="7a61b-112">Application</span></span> | <span data-ttu-id="7a61b-113">Device.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7a61b-113">Device.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7a61b-114">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7a61b-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /devices/{id}
```
> <span data-ttu-id="7a61b-115">注意：请求中的“id”是设备的“id”属性，不是“deviceId”属性。</span><span class="sxs-lookup"><span data-stu-id="7a61b-115">Note: The "id" in the request is the "id" property of the device, not the "deviceId" property.</span></span>

## <a name="optional-query-parameters"></a><span data-ttu-id="7a61b-116">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="7a61b-116">Optional query parameters</span></span>
<span data-ttu-id="7a61b-117">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="7a61b-117">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7a61b-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="7a61b-118">Request headers</span></span>
| <span data-ttu-id="7a61b-119">名称</span><span class="sxs-lookup"><span data-stu-id="7a61b-119">Name</span></span>       | <span data-ttu-id="7a61b-120">类型</span><span class="sxs-lookup"><span data-stu-id="7a61b-120">Type</span></span> | <span data-ttu-id="7a61b-121">说明</span><span class="sxs-lookup"><span data-stu-id="7a61b-121">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="7a61b-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="7a61b-122">Authorization</span></span>  | <span data-ttu-id="7a61b-123">string</span><span class="sxs-lookup"><span data-stu-id="7a61b-123">string</span></span>  | <span data-ttu-id="7a61b-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="7a61b-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7a61b-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="7a61b-126">Request body</span></span>
<span data-ttu-id="7a61b-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="7a61b-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7a61b-128">响应</span><span class="sxs-lookup"><span data-stu-id="7a61b-128">Response</span></span>

<span data-ttu-id="7a61b-129">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [device](../resources/device.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="7a61b-129">If successful, this method returns a `200 OK` response code and [device](../resources/device.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="7a61b-130">示例</span><span class="sxs-lookup"><span data-stu-id="7a61b-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7a61b-131">请求</span><span class="sxs-lookup"><span data-stu-id="7a61b-131">Request</span></span>
<span data-ttu-id="7a61b-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="7a61b-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_device"
}-->
```http
GET https://graph.microsoft.com/v1.0/devices/{id}
```
##### <a name="response"></a><span data-ttu-id="7a61b-133">响应</span><span class="sxs-lookup"><span data-stu-id="7a61b-133">Response</span></span>
<span data-ttu-id="7a61b-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="7a61b-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
