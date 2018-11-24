# <a name="update-deviceconfigurationdeviceoverview"></a><span data-ttu-id="d22df-101">更新 deviceConfigurationDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="d22df-101">Update deviceConfigurationDeviceOverview</span></span>

> <span data-ttu-id="d22df-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="d22df-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d22df-103">更新 [deviceConfigurationDeviceOverview](../resources/intune_deviceconfig_deviceconfigurationdeviceoverview.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="d22df-103">Update the properties of a [deviceConfigurationDeviceOverview](../resources/intune_deviceconfig_deviceconfigurationdeviceoverview.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="d22df-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="d22df-104">Prerequisites</span></span>
<span data-ttu-id="d22df-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="d22df-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="d22df-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="d22df-107">Permission type</span></span>|<span data-ttu-id="d22df-108">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="d22df-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d22df-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d22df-109">Delegated (work or school account)</span></span>|<span data-ttu-id="d22df-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d22df-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d22df-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d22df-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d22df-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="d22df-112">Not supported.</span></span>|
|<span data-ttu-id="d22df-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="d22df-113">Application</span></span>|<span data-ttu-id="d22df-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="d22df-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d22df-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d22df-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceStatusOverview
```

## <a name="request-headers"></a><span data-ttu-id="d22df-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="d22df-116">Request headers</span></span>
|<span data-ttu-id="d22df-117">标头</span><span class="sxs-lookup"><span data-stu-id="d22df-117">Header</span></span>|<span data-ttu-id="d22df-118">值</span><span class="sxs-lookup"><span data-stu-id="d22df-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d22df-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="d22df-119">Authorization</span></span>|<span data-ttu-id="d22df-120">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="d22df-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d22df-121">Accept</span><span class="sxs-lookup"><span data-stu-id="d22df-121">Accept</span></span>|<span data-ttu-id="d22df-122">application/json</span><span class="sxs-lookup"><span data-stu-id="d22df-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d22df-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="d22df-123">Request body</span></span>
<span data-ttu-id="d22df-124">在请求正文中，提供 [deviceConfigurationDeviceOverview](../resources/intune_deviceconfig_deviceconfigurationdeviceoverview.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d22df-124">In the request body, supply a JSON representation for the [deviceConfigurationDeviceOverview](../resources/intune_deviceconfig_deviceconfigurationdeviceoverview.md) object.</span></span>

<span data-ttu-id="d22df-125">下表显示创建 [deviceConfigurationDeviceOverview](../resources/intune_deviceconfig_deviceconfigurationdeviceoverview.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="d22df-125">The following table shows the properties that are required when you create the [deviceConfigurationDeviceOverview](../resources/intune_deviceconfig_deviceconfigurationdeviceoverview.md).</span></span>

|<span data-ttu-id="d22df-126">属性</span><span class="sxs-lookup"><span data-stu-id="d22df-126">Property</span></span>|<span data-ttu-id="d22df-127">类型</span><span class="sxs-lookup"><span data-stu-id="d22df-127">Type</span></span>|<span data-ttu-id="d22df-128">说明</span><span class="sxs-lookup"><span data-stu-id="d22df-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d22df-129">id</span><span class="sxs-lookup"><span data-stu-id="d22df-129">id</span></span>|<span data-ttu-id="d22df-130">String</span><span class="sxs-lookup"><span data-stu-id="d22df-130">String</span></span>|<span data-ttu-id="d22df-131">实体的键。</span><span class="sxs-lookup"><span data-stu-id="d22df-131">Key of the entity.</span></span>|
|<span data-ttu-id="d22df-132">pendingCount</span><span class="sxs-lookup"><span data-stu-id="d22df-132">pendingCount</span></span>|<span data-ttu-id="d22df-133">Int32</span><span class="sxs-lookup"><span data-stu-id="d22df-133">Int32</span></span>|<span data-ttu-id="d22df-134">挂起设备的数量</span><span class="sxs-lookup"><span data-stu-id="d22df-134">Number of pending devices</span></span>|
|<span data-ttu-id="d22df-135">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="d22df-135">notApplicableCount</span></span>|<span data-ttu-id="d22df-136">Int32</span><span class="sxs-lookup"><span data-stu-id="d22df-136">Int32</span></span>|<span data-ttu-id="d22df-137">不适用设备的数量</span><span class="sxs-lookup"><span data-stu-id="d22df-137">Number of not applicable devices</span></span>|
|<span data-ttu-id="d22df-138">successCount</span><span class="sxs-lookup"><span data-stu-id="d22df-138">successCount</span></span>|<span data-ttu-id="d22df-139">Int32</span><span class="sxs-lookup"><span data-stu-id="d22df-139">Int32</span></span>|<span data-ttu-id="d22df-140">成功设备的数量</span><span class="sxs-lookup"><span data-stu-id="d22df-140">Number of succeeded devices</span></span>|
|<span data-ttu-id="d22df-141">errorCount</span><span class="sxs-lookup"><span data-stu-id="d22df-141">errorCount</span></span>|<span data-ttu-id="d22df-142">Int32</span><span class="sxs-lookup"><span data-stu-id="d22df-142">Int32</span></span>|<span data-ttu-id="d22df-143">错误设备的数量</span><span class="sxs-lookup"><span data-stu-id="d22df-143">Number of error devices</span></span>|
|<span data-ttu-id="d22df-144">failedCount</span><span class="sxs-lookup"><span data-stu-id="d22df-144">failedCount</span></span>|<span data-ttu-id="d22df-145">Int32</span><span class="sxs-lookup"><span data-stu-id="d22df-145">Int32</span></span>|<span data-ttu-id="d22df-146">失败设备的数量</span><span class="sxs-lookup"><span data-stu-id="d22df-146">Number of failed devices</span></span>|
|<span data-ttu-id="d22df-147">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="d22df-147">lastUpdateDateTime</span></span>|<span data-ttu-id="d22df-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d22df-148">DateTimeOffset</span></span>|<span data-ttu-id="d22df-149">上次更新时间</span><span class="sxs-lookup"><span data-stu-id="d22df-149">Last update time</span></span>|
|<span data-ttu-id="d22df-150">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="d22df-150">configurationVersion</span></span>|<span data-ttu-id="d22df-151">Int32</span><span class="sxs-lookup"><span data-stu-id="d22df-151">Int32</span></span>|<span data-ttu-id="d22df-152">用于此概述的策略版本</span><span class="sxs-lookup"><span data-stu-id="d22df-152">Version of the policy for that overview</span></span>|



## <a name="response"></a><span data-ttu-id="d22df-153">响应</span><span class="sxs-lookup"><span data-stu-id="d22df-153">Response</span></span>
<span data-ttu-id="d22df-154">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和更新的 [deviceConfigurationDeviceOverview](../resources/intune_deviceconfig_deviceconfigurationdeviceoverview.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="d22df-154">If successful, this method returns a `200 OK` response code and an updated [deviceConfigurationDeviceOverview](../resources/intune_deviceconfig_deviceconfigurationdeviceoverview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d22df-155">示例</span><span class="sxs-lookup"><span data-stu-id="d22df-155">Example</span></span>
### <a name="request"></a><span data-ttu-id="d22df-156">请求</span><span class="sxs-lookup"><span data-stu-id="d22df-156">Request</span></span>
<span data-ttu-id="d22df-157">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="d22df-157">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceStatusOverview
Content-type: application/json
Content-length: 284

{
  "@odata.type": "#microsoft.graph.deviceConfigurationDeviceOverview",
  "pendingCount": 12,
  "notApplicableCount": 2,
  "successCount": 12,
  "errorCount": 10,
  "failedCount": 11,
  "lastUpdateDateTime": "2016-12-31T23:58:21.6459442-08:00",
  "configurationVersion": 4
}
```

### <a name="response"></a><span data-ttu-id="d22df-158">响应</span><span class="sxs-lookup"><span data-stu-id="d22df-158">Response</span></span>
<span data-ttu-id="d22df-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="d22df-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 333

{
  "@odata.type": "#microsoft.graph.deviceConfigurationDeviceOverview",
  "id": "62d48e3a-8e3a-62d4-3a8e-d4623a8ed462",
  "pendingCount": 12,
  "notApplicableCount": 2,
  "successCount": 12,
  "errorCount": 10,
  "failedCount": 11,
  "lastUpdateDateTime": "2016-12-31T23:58:21.6459442-08:00",
  "configurationVersion": 4
}
```



