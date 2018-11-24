# <a name="create-settingstatedevicesummary"></a><span data-ttu-id="2ba2a-101">创建 settingStateDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="2ba2a-101">Create settingStateDeviceSummary</span></span>

> <span data-ttu-id="2ba2a-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="2ba2a-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2ba2a-103">创建新的 [settingStateDeviceSummary](../resources/intune_deviceconfig_settingstatedevicesummary.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="2ba2a-103">Create a new [settingStateDeviceSummary](../resources/intune_deviceconfig_settingstatedevicesummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="2ba2a-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="2ba2a-104">Prerequisites</span></span>
<span data-ttu-id="2ba2a-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="2ba2a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="2ba2a-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="2ba2a-107">Permission type</span></span>|<span data-ttu-id="2ba2a-108">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="2ba2a-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2ba2a-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2ba2a-109">Delegated (work or school account)</span></span>|<span data-ttu-id="2ba2a-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2ba2a-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="2ba2a-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2ba2a-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2ba2a-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="2ba2a-112">Not supported.</span></span>|
|<span data-ttu-id="2ba2a-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="2ba2a-113">Application</span></span>|<span data-ttu-id="2ba2a-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="2ba2a-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2ba2a-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2ba2a-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceSettingStateSummaries
POST /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/deviceSettingStateSummaries
```

## <a name="request-headers"></a><span data-ttu-id="2ba2a-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="2ba2a-116">Request headers</span></span>
|<span data-ttu-id="2ba2a-117">标头</span><span class="sxs-lookup"><span data-stu-id="2ba2a-117">Header</span></span>|<span data-ttu-id="2ba2a-118">值</span><span class="sxs-lookup"><span data-stu-id="2ba2a-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2ba2a-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="2ba2a-119">Authorization</span></span>|<span data-ttu-id="2ba2a-120">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="2ba2a-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2ba2a-121">Accept</span><span class="sxs-lookup"><span data-stu-id="2ba2a-121">Accept</span></span>|<span data-ttu-id="2ba2a-122">application/json</span><span class="sxs-lookup"><span data-stu-id="2ba2a-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2ba2a-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="2ba2a-123">Request body</span></span>
<span data-ttu-id="2ba2a-124">在请求正文中，提供 settingStateDeviceSummary 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2ba2a-124">In the request body, supply a JSON representation for the settingStateDeviceSummary object.</span></span>

<span data-ttu-id="2ba2a-125">下表显示了创建 settingStateDeviceSummary 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="2ba2a-125">The following table shows the properties that are required when you create the settingStateDeviceSummary.</span></span>

|<span data-ttu-id="2ba2a-126">属性</span><span class="sxs-lookup"><span data-stu-id="2ba2a-126">Property</span></span>|<span data-ttu-id="2ba2a-127">类型</span><span class="sxs-lookup"><span data-stu-id="2ba2a-127">Type</span></span>|<span data-ttu-id="2ba2a-128">说明</span><span class="sxs-lookup"><span data-stu-id="2ba2a-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2ba2a-129">id</span><span class="sxs-lookup"><span data-stu-id="2ba2a-129">id</span></span>|<span data-ttu-id="2ba2a-130">String</span><span class="sxs-lookup"><span data-stu-id="2ba2a-130">String</span></span>|<span data-ttu-id="2ba2a-131">实体的键。</span><span class="sxs-lookup"><span data-stu-id="2ba2a-131">Key of the entity.</span></span>|
|<span data-ttu-id="2ba2a-132">settingName</span><span class="sxs-lookup"><span data-stu-id="2ba2a-132">settingName</span></span>|<span data-ttu-id="2ba2a-133">String</span><span class="sxs-lookup"><span data-stu-id="2ba2a-133">String</span></span>|<span data-ttu-id="2ba2a-134">设置的名称</span><span class="sxs-lookup"><span data-stu-id="2ba2a-134">Name of the setting</span></span>|
|<span data-ttu-id="2ba2a-135">instancePath</span><span class="sxs-lookup"><span data-stu-id="2ba2a-135">instancePath</span></span>|<span data-ttu-id="2ba2a-136">String</span><span class="sxs-lookup"><span data-stu-id="2ba2a-136">String</span></span>|<span data-ttu-id="2ba2a-137">设置的 InstancePath 的名称</span><span class="sxs-lookup"><span data-stu-id="2ba2a-137">Name of the InstancePath for the setting</span></span>|
|<span data-ttu-id="2ba2a-138">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="2ba2a-138">unknownDeviceCount</span></span>|<span data-ttu-id="2ba2a-139">Int32</span><span class="sxs-lookup"><span data-stu-id="2ba2a-139">Int32</span></span>|<span data-ttu-id="2ba2a-140">设置的设备未知计数</span><span class="sxs-lookup"><span data-stu-id="2ba2a-140">Device Unkown count for the setting</span></span>|
|<span data-ttu-id="2ba2a-141">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="2ba2a-141">notApplicableDeviceCount</span></span>|<span data-ttu-id="2ba2a-142">Int32</span><span class="sxs-lookup"><span data-stu-id="2ba2a-142">Int32</span></span>|<span data-ttu-id="2ba2a-143">设置的设备不适用计数</span><span class="sxs-lookup"><span data-stu-id="2ba2a-143">Device Not Applicable count for the setting</span></span>|
|<span data-ttu-id="2ba2a-144">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="2ba2a-144">compliantDeviceCount</span></span>|<span data-ttu-id="2ba2a-145">Int32</span><span class="sxs-lookup"><span data-stu-id="2ba2a-145">Int32</span></span>|<span data-ttu-id="2ba2a-146">设置的设备符合性计数</span><span class="sxs-lookup"><span data-stu-id="2ba2a-146">Device Compliant count for the setting</span></span>|
|<span data-ttu-id="2ba2a-147">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="2ba2a-147">remediatedDeviceCount</span></span>|<span data-ttu-id="2ba2a-148">Int32</span><span class="sxs-lookup"><span data-stu-id="2ba2a-148">Int32</span></span>|<span data-ttu-id="2ba2a-149">设置的设备符合性计数</span><span class="sxs-lookup"><span data-stu-id="2ba2a-149">Device Compliant count for the setting</span></span>|
|<span data-ttu-id="2ba2a-150">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="2ba2a-150">nonCompliantDeviceCount</span></span>|<span data-ttu-id="2ba2a-151">Int32</span><span class="sxs-lookup"><span data-stu-id="2ba2a-151">Int32</span></span>|<span data-ttu-id="2ba2a-152">设置的设备不符合计数</span><span class="sxs-lookup"><span data-stu-id="2ba2a-152">Device NonCompliant count for the setting</span></span>|
|<span data-ttu-id="2ba2a-153">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="2ba2a-153">errorDeviceCount</span></span>|<span data-ttu-id="2ba2a-154">Int32</span><span class="sxs-lookup"><span data-stu-id="2ba2a-154">Int32</span></span>|<span data-ttu-id="2ba2a-155">设置的设备错误计数</span><span class="sxs-lookup"><span data-stu-id="2ba2a-155">Device error count for the setting</span></span>|
|<span data-ttu-id="2ba2a-156">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="2ba2a-156">conflictDeviceCount</span></span>|<span data-ttu-id="2ba2a-157">Int32</span><span class="sxs-lookup"><span data-stu-id="2ba2a-157">Int32</span></span>|<span data-ttu-id="2ba2a-158">设置的设备冲突错误计数</span><span class="sxs-lookup"><span data-stu-id="2ba2a-158">Device conflict error count for the setting</span></span>|



## <a name="response"></a><span data-ttu-id="2ba2a-159">响应</span><span class="sxs-lookup"><span data-stu-id="2ba2a-159">Response</span></span>
<span data-ttu-id="2ba2a-160">如果成功，此方法将在响应正文中返回 `201 Created` 响应代码和 [settingStateDeviceSummary](../resources/intune_deviceconfig_settingstatedevicesummary.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="2ba2a-160">If successful, this method returns a `201 Created` response code and a [settingStateDeviceSummary](../resources/intune_deviceconfig_settingstatedevicesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2ba2a-161">示例</span><span class="sxs-lookup"><span data-stu-id="2ba2a-161">Example</span></span>
### <a name="request"></a><span data-ttu-id="2ba2a-162">请求</span><span class="sxs-lookup"><span data-stu-id="2ba2a-162">Request</span></span>
<span data-ttu-id="2ba2a-163">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="2ba2a-163">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceSettingStateSummaries
Content-type: application/json
Content-length: 360

{
  "@odata.type": "#microsoft.graph.settingStateDeviceSummary",
  "settingName": "Setting Name value",
  "instancePath": "Instance Path value",
  "unknownDeviceCount": 2,
  "notApplicableDeviceCount": 8,
  "compliantDeviceCount": 4,
  "remediatedDeviceCount": 5,
  "nonCompliantDeviceCount": 7,
  "errorDeviceCount": 0,
  "conflictDeviceCount": 3
}
```

### <a name="response"></a><span data-ttu-id="2ba2a-164">响应</span><span class="sxs-lookup"><span data-stu-id="2ba2a-164">Response</span></span>
<span data-ttu-id="2ba2a-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="2ba2a-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 409

{
  "@odata.type": "#microsoft.graph.settingStateDeviceSummary",
  "id": "3e2d4526-4526-3e2d-2645-2d3e26452d3e",
  "settingName": "Setting Name value",
  "instancePath": "Instance Path value",
  "unknownDeviceCount": 2,
  "notApplicableDeviceCount": 8,
  "compliantDeviceCount": 4,
  "remediatedDeviceCount": 5,
  "nonCompliantDeviceCount": 7,
  "errorDeviceCount": 0,
  "conflictDeviceCount": 3
}
```



