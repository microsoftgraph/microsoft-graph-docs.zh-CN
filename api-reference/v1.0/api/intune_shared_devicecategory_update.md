# <a name="update-devicecategory"></a><span data-ttu-id="e4918-101">更新 deviceCategory</span><span class="sxs-lookup"><span data-stu-id="e4918-101">Update deviceCategory</span></span>

> <span data-ttu-id="e4918-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="e4918-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e4918-103">更新 [deviceCategory](../resources/intune_shared_devicecategory.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="e4918-103">Update the properties of a [deviceCategory](../resources/intune_shared_devicecategory.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="e4918-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="e4918-104">Prerequisites</span></span>
<span data-ttu-id="e4918-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](../../../concepts/permissions_reference.md)。
</span><span class="sxs-lookup"><span data-stu-id="e4918-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="e4918-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="e4918-107">Permission type</span></span>|<span data-ttu-id="e4918-108">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="e4918-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e4918-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e4918-109">Delegated (work or school account)</span></span>||
| <span data-ttu-id="e4918-110">&nbsp;&nbsp; **入职培训**和</span><span class="sxs-lookup"><span data-stu-id="e4918-110">&nbsp; &nbsp; **Onboarding** and</span></span> <br> <span data-ttu-id="e4918-111">&nbsp;&nbsp; **设备管理**</span><span class="sxs-lookup"><span data-stu-id="e4918-111">&nbsp; &nbsp; **Device Management**</span></span>| <span data-ttu-id="e4918-112">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e4918-112">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="e4918-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e4918-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e4918-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="e4918-114">Not supported.</span></span>|
|<span data-ttu-id="e4918-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="e4918-115">Application</span></span>|<span data-ttu-id="e4918-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="e4918-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e4918-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e4918-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCategories/{deviceCategoryId}
PATCH /deviceManagement/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/deviceCategory
```

## <a name="request-headers"></a><span data-ttu-id="e4918-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="e4918-118">Request headers</span></span>
|<span data-ttu-id="e4918-119">标头</span><span class="sxs-lookup"><span data-stu-id="e4918-119">Header</span></span>|<span data-ttu-id="e4918-120">值</span><span class="sxs-lookup"><span data-stu-id="e4918-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e4918-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="e4918-121">Authorization</span></span>|<span data-ttu-id="e4918-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="e4918-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e4918-123">Accept</span><span class="sxs-lookup"><span data-stu-id="e4918-123">Accept</span></span>|<span data-ttu-id="e4918-124">application/json</span><span class="sxs-lookup"><span data-stu-id="e4918-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e4918-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="e4918-125">Request body</span></span>
<span data-ttu-id="e4918-126">在请求正文中，提供 [deviceCategory](../resources/intune_shared_devicecategory.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e4918-126">In the request body, supply a JSON representation for the [deviceCategory](../resources/intune_shared_devicecategory.md) object.</span></span>

<span data-ttu-id="e4918-127">下表显示创建 [deviceCategory](../resources/intune_shared_devicecategory.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="e4918-127">The following table shows the properties that are required when you create the [deviceCategory](../resources/intune_shared_devicecategory.md).</span></span>

|<span data-ttu-id="e4918-128">属性</span><span class="sxs-lookup"><span data-stu-id="e4918-128">Property</span></span>|<span data-ttu-id="e4918-129">类型</span><span class="sxs-lookup"><span data-stu-id="e4918-129">Type</span></span>|<span data-ttu-id="e4918-130">说明</span><span class="sxs-lookup"><span data-stu-id="e4918-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e4918-131">id</span><span class="sxs-lookup"><span data-stu-id="e4918-131">id</span></span>|<span data-ttu-id="e4918-132">String</span><span class="sxs-lookup"><span data-stu-id="e4918-132">String</span></span>|<span data-ttu-id="e4918-133">设备类别的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="e4918-133">Unique identifier for the device category.</span></span> <span data-ttu-id="e4918-134">只读。</span><span class="sxs-lookup"><span data-stu-id="e4918-134">Read-only.</span></span>|
|<span data-ttu-id="e4918-135">**入职培训**</span><span class="sxs-lookup"><span data-stu-id="e4918-135">**Onboarding**</span></span>|
|<span data-ttu-id="e4918-136">displayName</span><span class="sxs-lookup"><span data-stu-id="e4918-136">displayName</span></span>|<span data-ttu-id="e4918-137">String</span><span class="sxs-lookup"><span data-stu-id="e4918-137">String</span></span>|<span data-ttu-id="e4918-138">设备类别的显示名称。</span><span class="sxs-lookup"><span data-stu-id="e4918-138">Display name for the device category.</span></span>|
|<span data-ttu-id="e4918-139">description</span><span class="sxs-lookup"><span data-stu-id="e4918-139">description</span></span>|<span data-ttu-id="e4918-140">String</span><span class="sxs-lookup"><span data-stu-id="e4918-140">String</span></span>|<span data-ttu-id="e4918-141">设备类别的可选说明。</span><span class="sxs-lookup"><span data-stu-id="e4918-141">Optional description for the device category.</span></span>|



## <a name="response"></a><span data-ttu-id="e4918-142">响应</span><span class="sxs-lookup"><span data-stu-id="e4918-142">Response</span></span>
<span data-ttu-id="e4918-143">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [deviceCategory](../resources/intune_shared_devicecategory.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="e4918-143">If successful, this method returns a `200 OK` response code and an updated [deviceCategory](../resources/intune_shared_devicecategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e4918-144">示例</span><span class="sxs-lookup"><span data-stu-id="e4918-144">Example</span></span>
### <a name="request"></a><span data-ttu-id="e4918-145">请求</span><span class="sxs-lookup"><span data-stu-id="e4918-145">Request</span></span>
<span data-ttu-id="e4918-146">下面是请求的示例。</span><span class="sxs-lookup"><span data-stu-id="e4918-146">Here are examples of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="e4918-147">响应</span><span class="sxs-lookup"><span data-stu-id="e4918-147">Response</span></span>
<span data-ttu-id="e4918-148">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="e4918-148">Here is an example of the response.</span></span> <span data-ttu-id="e4918-149">注意：为简洁起见，可能会截断此处展示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="e4918-149">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="e4918-150">响应属性根据上下文不同而有所不同。</span><span class="sxs-lookup"><span data-stu-id="e4918-150">Response properties will vary according to context.</span></span>
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



