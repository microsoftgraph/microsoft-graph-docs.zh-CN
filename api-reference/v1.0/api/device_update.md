# <a name="update-device"></a><span data-ttu-id="afd53-101">更新设备</span><span class="sxs-lookup"><span data-stu-id="afd53-101">Update device</span></span>

<span data-ttu-id="afd53-102">更新已注册设备的属性。</span><span class="sxs-lookup"><span data-stu-id="afd53-102">Update the properties of a registered device.</span></span>

## <a name="permissions"></a><span data-ttu-id="afd53-103">权限</span><span class="sxs-lookup"><span data-stu-id="afd53-103">Permissions</span></span>
<span data-ttu-id="afd53-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="afd53-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>


|<span data-ttu-id="afd53-106">权限类型</span><span class="sxs-lookup"><span data-stu-id="afd53-106">Permission type</span></span>      | <span data-ttu-id="afd53-107">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="afd53-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="afd53-108">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="afd53-108">Delegated (work or school account)</span></span> | <span data-ttu-id="afd53-109">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="afd53-109">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="afd53-110">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="afd53-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="afd53-111">不支持。</span><span class="sxs-lookup"><span data-stu-id="afd53-111">Not supported.</span></span>    |
|<span data-ttu-id="afd53-112">应用程序</span><span class="sxs-lookup"><span data-stu-id="afd53-112">Application</span></span> | <span data-ttu-id="afd53-113">Device.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="afd53-113">Device.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="afd53-114">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="afd53-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /devices/{id}
```
> <span data-ttu-id="afd53-115">注意：请求中的“id”是设备的“id”属性，不是“deviceId”属性。</span><span class="sxs-lookup"><span data-stu-id="afd53-115">Note: The "id" in the request is the "id" property of the device, not the "deviceId" property.</span></span>

## <a name="request-headers"></a><span data-ttu-id="afd53-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="afd53-116">Request headers</span></span>
| <span data-ttu-id="afd53-117">名称</span><span class="sxs-lookup"><span data-stu-id="afd53-117">Name</span></span>       | <span data-ttu-id="afd53-118">类型</span><span class="sxs-lookup"><span data-stu-id="afd53-118">Type</span></span> | <span data-ttu-id="afd53-119">说明</span><span class="sxs-lookup"><span data-stu-id="afd53-119">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="afd53-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="afd53-120">Authorization</span></span>  | <span data-ttu-id="afd53-121">string</span><span class="sxs-lookup"><span data-stu-id="afd53-121">string</span></span>  | <span data-ttu-id="afd53-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="afd53-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="afd53-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="afd53-124">Request body</span></span>
<span data-ttu-id="afd53-125">在请求正文中，提供应更新的 [device](../resources/device.md) 属性的值。</span><span class="sxs-lookup"><span data-stu-id="afd53-125">In the request body, supply the values for the [device](../resources/device.md) properties that should be updated.</span></span>

## <a name="response"></a><span data-ttu-id="afd53-126">响应</span><span class="sxs-lookup"><span data-stu-id="afd53-126">Response</span></span>

<span data-ttu-id="afd53-127">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="afd53-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="afd53-128">示例</span><span class="sxs-lookup"><span data-stu-id="afd53-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="afd53-129">请求</span><span class="sxs-lookup"><span data-stu-id="afd53-129">Request</span></span>
<span data-ttu-id="afd53-130">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="afd53-130">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_device"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/devices/{id}
Content-type: application/json

{
  "accountEnabled": true
}
```
##### <a name="response"></a><span data-ttu-id="afd53-131">响应</span><span class="sxs-lookup"><span data-stu-id="afd53-131">Response</span></span>
<span data-ttu-id="afd53-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="afd53-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.device"
} -->
```http
HTTP/1.1 204 No Content
```
