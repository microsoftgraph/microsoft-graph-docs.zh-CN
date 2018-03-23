# <a name="update-devicecategory"></a><span data-ttu-id="4ace7-101">更新 deviceCategory</span><span class="sxs-lookup"><span data-stu-id="4ace7-101">Update deviceCategory</span></span>

> <span data-ttu-id="4ace7-102">**注意：**使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="4ace7-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4ace7-103">更新 [deviceCategory](../resources/intune_devices_devicecategory.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="4ace7-103">Update the properties of a [calendar](../resources/intune_devices_devicecategory.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="4ace7-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="4ace7-104">Prerequisites</span></span>
<span data-ttu-id="4ace7-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="4ace7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="4ace7-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="4ace7-107">Permission type</span></span>|<span data-ttu-id="4ace7-108">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="4ace7-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4ace7-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4ace7-109">Delegated (work or school account)</span></span>|<span data-ttu-id="4ace7-110">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4ace7-110">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="4ace7-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4ace7-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4ace7-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="4ace7-112">Not supported.</span></span>|
|<span data-ttu-id="4ace7-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="4ace7-113">Application</span></span>|<span data-ttu-id="4ace7-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="4ace7-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4ace7-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4ace7-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/deviceCategory
```

## <a name="request-headers"></a><span data-ttu-id="4ace7-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="4ace7-116">Request headers</span></span>
|<span data-ttu-id="4ace7-117">标头</span><span class="sxs-lookup"><span data-stu-id="4ace7-117">Header</span></span>|<span data-ttu-id="4ace7-118">值</span><span class="sxs-lookup"><span data-stu-id="4ace7-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4ace7-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="4ace7-119">Authorization</span></span>|<span data-ttu-id="4ace7-120">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="4ace7-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="4ace7-121">Accept</span><span class="sxs-lookup"><span data-stu-id="4ace7-121">Accept</span></span>|<span data-ttu-id="4ace7-122">application/json</span><span class="sxs-lookup"><span data-stu-id="4ace7-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4ace7-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="4ace7-123">Request body</span></span>
<span data-ttu-id="4ace7-124">在请求正文中，提供 [deviceCategory](../resources/intune_devices_devicecategory.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4ace7-124">In the request body, supply a JSON representation of [Attachment](../resources/intune_devices_devicecategory.md) object.</span></span>

<span data-ttu-id="4ace7-125">下表显示创建 [deviceCategory](../resources/intune_devices_devicecategory.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="4ace7-125">The following table shows the properties that are required when you create a user.</span></span>

|<span data-ttu-id="4ace7-126">属性</span><span class="sxs-lookup"><span data-stu-id="4ace7-126">Property</span></span>|<span data-ttu-id="4ace7-127">类型</span><span class="sxs-lookup"><span data-stu-id="4ace7-127">Type</span></span>|<span data-ttu-id="4ace7-128">说明</span><span class="sxs-lookup"><span data-stu-id="4ace7-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4ace7-129">id</span><span class="sxs-lookup"><span data-stu-id="4ace7-129">id</span></span>|<span data-ttu-id="4ace7-130">String</span><span class="sxs-lookup"><span data-stu-id="4ace7-130">String</span></span>|<span data-ttu-id="4ace7-131">设备类别的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="4ace7-131">Unique identifier for the device category.</span></span> <span data-ttu-id="4ace7-132">只读。</span><span class="sxs-lookup"><span data-stu-id="4ace7-132">Read-only.</span></span>|



## <a name="response"></a><span data-ttu-id="4ace7-133">响应</span><span class="sxs-lookup"><span data-stu-id="4ace7-133">Response</span></span>
<span data-ttu-id="4ace7-134">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [deviceCategory](../resources/intune_devices_devicecategory.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="4ace7-134">If successful, this method returns a `200 OK` response code and an updated [contact](../resources/intune_devices_devicecategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4ace7-135">示例</span><span class="sxs-lookup"><span data-stu-id="4ace7-135">Example</span></span>
### <a name="request"></a><span data-ttu-id="4ace7-136">请求</span><span class="sxs-lookup"><span data-stu-id="4ace7-136">Request</span></span>
<span data-ttu-id="4ace7-137">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="4ace7-137">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/deviceCategory
Content-type: application/json
Content-length: 2

{}
```

### <a name="response"></a><span data-ttu-id="4ace7-138">响应</span><span class="sxs-lookup"><span data-stu-id="4ace7-138">Response</span></span>
<span data-ttu-id="4ace7-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="4ace7-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 105

{
  "@odata.type": "#microsoft.graph.deviceCategory",
  "id": "f881b841-b841-f881-41b8-81f841b881f8"
}
```



