# <a name="update-devicecategory"></a><span data-ttu-id="d2d93-101">更新 deviceCategory</span><span class="sxs-lookup"><span data-stu-id="d2d93-101">Update deviceCategory</span></span>

> <span data-ttu-id="d2d93-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="d2d93-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d2d93-103">更新 [deviceCategory](../resources/intune_shared_devicecategory.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="d2d93-103">Update the properties of a [deviceCategory](../resources/intune_shared_devicecategory.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="d2d93-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="d2d93-104">Prerequisites</span></span>
<span data-ttu-id="d2d93-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="d2d93-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="d2d93-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="d2d93-107">Permission type</span></span>|<span data-ttu-id="d2d93-108">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="d2d93-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d2d93-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d2d93-109">Delegated (work or school account)</span></span>|<span data-ttu-id="d2d93-110">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d2d93-110">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="d2d93-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d2d93-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d2d93-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="d2d93-112">Not supported.</span></span>|
|<span data-ttu-id="d2d93-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="d2d93-113">Application</span></span>|<span data-ttu-id="d2d93-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="d2d93-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d2d93-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d2d93-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCategories/{deviceCategoryId}
PATCH /deviceManagement/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/deviceCategory
```

## <a name="request-headers"></a><span data-ttu-id="d2d93-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="d2d93-116">Request headers</span></span>
|<span data-ttu-id="d2d93-117">标头</span><span class="sxs-lookup"><span data-stu-id="d2d93-117">Header</span></span>|<span data-ttu-id="d2d93-118">值</span><span class="sxs-lookup"><span data-stu-id="d2d93-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d2d93-119">授权</span><span class="sxs-lookup"><span data-stu-id="d2d93-119">Authorization</span></span>|<span data-ttu-id="d2d93-120">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="d2d93-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d2d93-121">接受</span><span class="sxs-lookup"><span data-stu-id="d2d93-121">Accept</span></span>|<span data-ttu-id="d2d93-122">应用/json</span><span class="sxs-lookup"><span data-stu-id="d2d93-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d2d93-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="d2d93-123">Request body</span></span>
<span data-ttu-id="d2d93-124">在请求正文中，提供 [deviceCategory](../resources/intune_shared_devicecategory.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d2d93-124">In the request body, supply a JSON representation for the [deviceCategory](../resources/intune_shared_devicecategory.md) object.</span></span>

<span data-ttu-id="d2d93-125">下表显示创建 [deviceCategory](../resources/intune_shared_devicecategory.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="d2d93-125">The following table shows the properties that are required when you create the [deviceCategory](../resources/intune_shared_devicecategory.md).</span></span>

|<span data-ttu-id="d2d93-126">属性</span><span class="sxs-lookup"><span data-stu-id="d2d93-126">Property</span></span>|<span data-ttu-id="d2d93-127">类型</span><span class="sxs-lookup"><span data-stu-id="d2d93-127">Type</span></span>|<span data-ttu-id="d2d93-128">说明</span><span class="sxs-lookup"><span data-stu-id="d2d93-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d2d93-129">id</span><span class="sxs-lookup"><span data-stu-id="d2d93-129">id</span></span>|<span data-ttu-id="d2d93-130">字符串</span><span class="sxs-lookup"><span data-stu-id="d2d93-130">String</span></span>|<span data-ttu-id="d2d93-131">设备类别的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="d2d93-131">Unique identifier for the device category.</span></span> <span data-ttu-id="d2d93-132">只读。</span><span class="sxs-lookup"><span data-stu-id="d2d93-132">Read-only.</span></span>|
|<span data-ttu-id="d2d93-133">**起始安排**</span><span class="sxs-lookup"><span data-stu-id="d2d93-133">**On-boarding**</span></span>|
|<span data-ttu-id="d2d93-134">displayName</span><span class="sxs-lookup"><span data-stu-id="d2d93-134">displayName</span></span>|<span data-ttu-id="d2d93-135">字符串</span><span class="sxs-lookup"><span data-stu-id="d2d93-135">String</span></span>|<span data-ttu-id="d2d93-136">设备类别的显示名称。</span><span class="sxs-lookup"><span data-stu-id="d2d93-136">Display name for the device category.</span></span>|
|<span data-ttu-id="d2d93-137">说明</span><span class="sxs-lookup"><span data-stu-id="d2d93-137">description</span></span>|<span data-ttu-id="d2d93-138">字符串</span><span class="sxs-lookup"><span data-stu-id="d2d93-138">String</span></span>|<span data-ttu-id="d2d93-139">设备类别的可选说明。</span><span class="sxs-lookup"><span data-stu-id="d2d93-139">Optional description for the device category.</span></span>|



## <a name="response"></a><span data-ttu-id="d2d93-140">响应</span><span class="sxs-lookup"><span data-stu-id="d2d93-140">Response</span></span>
<span data-ttu-id="d2d93-141">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [deviceCategory](../resources/intune_shared_devicecategory.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="d2d93-141">If successful, this method returns a `200 OK` response code and an updated [deviceCategory](../resources/intune_shared_devicecategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d2d93-142">示例</span><span class="sxs-lookup"><span data-stu-id="d2d93-142">Example</span></span>
### <a name="request"></a><span data-ttu-id="d2d93-143">请求</span><span class="sxs-lookup"><span data-stu-id="d2d93-143">Request</span></span>
<span data-ttu-id="d2d93-144">下面是请求的示例。</span><span class="sxs-lookup"><span data-stu-id="d2d93-144">Here are a couple of examples of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceCategories/{deviceCategoryId}
Content-type: application/json
Content-length: 82

{
  "displayName": "Display Name value",
  "description": "Description value"
}

PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/deviceCategory
```

### <a name="response"></a><span data-ttu-id="d2d93-145">响应</span><span class="sxs-lookup"><span data-stu-id="d2d93-145">Response</span></span>
<span data-ttu-id="d2d93-146">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="d2d93-146">Here is an example of the response.</span></span> <span data-ttu-id="d2d93-147">注意：为简洁起见，可能会截断此处展示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="d2d93-147">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="d2d93-148">响应的属性根据上下文不同而有所不同。</span><span class="sxs-lookup"><span data-stu-id="d2d93-148">Response properties will vary according to context.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 184

{
  "@odata.type": "#microsoft.graph.deviceCategory",
  "id": "f881b841-b841-f881-41b8-81f841b881f8",
  "displayName": "Display Name value",
  "description": "Description value"
}
```



