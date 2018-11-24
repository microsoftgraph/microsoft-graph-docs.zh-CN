# <a name="update-devicecompliancepolicydevicestatesummary"></a><span data-ttu-id="44dcc-101">更新 deviceCompliancePolicyDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="44dcc-101">Update deviceCompliancePolicyDeviceStateSummary</span></span>

> <span data-ttu-id="44dcc-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="44dcc-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="44dcc-103">更新 [deviceCompliancePolicyDeviceStateSummary](../resources/intune_deviceconfig_devicecompliancepolicydevicestatesummary.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="44dcc-103">Update the properties of a [deviceCompliancePolicyDeviceStateSummary](../resources/intune_deviceconfig_devicecompliancepolicydevicestatesummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="44dcc-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="44dcc-104">Prerequisites</span></span>
<span data-ttu-id="44dcc-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="44dcc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="44dcc-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="44dcc-107">Permission type</span></span>|<span data-ttu-id="44dcc-108">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="44dcc-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="44dcc-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="44dcc-109">Delegated (work or school account)</span></span>|<span data-ttu-id="44dcc-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="44dcc-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="44dcc-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="44dcc-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="44dcc-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="44dcc-112">Not supported.</span></span>|
|<span data-ttu-id="44dcc-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="44dcc-113">Application</span></span>|<span data-ttu-id="44dcc-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="44dcc-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="44dcc-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="44dcc-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicyDeviceStateSummary
```

## <a name="request-headers"></a><span data-ttu-id="44dcc-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="44dcc-116">Request headers</span></span>
|<span data-ttu-id="44dcc-117">标头</span><span class="sxs-lookup"><span data-stu-id="44dcc-117">Header</span></span>|<span data-ttu-id="44dcc-118">值</span><span class="sxs-lookup"><span data-stu-id="44dcc-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="44dcc-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="44dcc-119">Authorization</span></span>|<span data-ttu-id="44dcc-120">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="44dcc-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="44dcc-121">Accept</span><span class="sxs-lookup"><span data-stu-id="44dcc-121">Accept</span></span>|<span data-ttu-id="44dcc-122">application/json</span><span class="sxs-lookup"><span data-stu-id="44dcc-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="44dcc-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="44dcc-123">Request body</span></span>
<span data-ttu-id="44dcc-124">在请求正文中，提供 [deviceCompliancePolicyDeviceStateSummary](../resources/intune_deviceconfig_devicecompliancepolicydevicestatesummary.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="44dcc-124">In the request body, supply a JSON representation for the [deviceCompliancePolicyDeviceStateSummary](../resources/intune_deviceconfig_devicecompliancepolicydevicestatesummary.md) object.</span></span>

<span data-ttu-id="44dcc-125">下表显示了创建 [deviceCompliancePolicyDeviceStateSummary](../resources/intune_deviceconfig_devicecompliancepolicydevicestatesummary.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="44dcc-125">The following table shows the properties that are required when you create the [deviceCompliancePolicyDeviceStateSummary](../resources/intune_deviceconfig_devicecompliancepolicydevicestatesummary.md).</span></span>

|<span data-ttu-id="44dcc-126">属性</span><span class="sxs-lookup"><span data-stu-id="44dcc-126">Property</span></span>|<span data-ttu-id="44dcc-127">类型</span><span class="sxs-lookup"><span data-stu-id="44dcc-127">Type</span></span>|<span data-ttu-id="44dcc-128">说明</span><span class="sxs-lookup"><span data-stu-id="44dcc-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="44dcc-129">inGracePeriodCount</span><span class="sxs-lookup"><span data-stu-id="44dcc-129">inGracePeriodCount</span></span>|<span data-ttu-id="44dcc-130">Int32</span><span class="sxs-lookup"><span data-stu-id="44dcc-130">Int32</span></span>|<span data-ttu-id="44dcc-131">宽限期内的设备数</span><span class="sxs-lookup"><span data-stu-id="44dcc-131">Number of devices that are in grace period</span></span>|
|<span data-ttu-id="44dcc-132">configManagerCount</span><span class="sxs-lookup"><span data-stu-id="44dcc-132">configManagerCount</span></span>|<span data-ttu-id="44dcc-133">Int32</span><span class="sxs-lookup"><span data-stu-id="44dcc-133">Int32</span></span>|<span data-ttu-id="44dcc-134">由 System Center Configuration Manager 管理符合性的设备数</span><span class="sxs-lookup"><span data-stu-id="44dcc-134">Number of devices that have compliance managed by System Center Configuration Manager</span></span>|
|<span data-ttu-id="44dcc-135">id</span><span class="sxs-lookup"><span data-stu-id="44dcc-135">id</span></span>|<span data-ttu-id="44dcc-136">String</span><span class="sxs-lookup"><span data-stu-id="44dcc-136">String</span></span>|<span data-ttu-id="44dcc-137">实体的键。</span><span class="sxs-lookup"><span data-stu-id="44dcc-137">Key of the entity.</span></span>|
|<span data-ttu-id="44dcc-138">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="44dcc-138">unknownDeviceCount</span></span>|<span data-ttu-id="44dcc-139">Int32</span><span class="sxs-lookup"><span data-stu-id="44dcc-139">Int32</span></span>|<span data-ttu-id="44dcc-140">未知设备的数量</span><span class="sxs-lookup"><span data-stu-id="44dcc-140">Number of unknown devices</span></span>|
|<span data-ttu-id="44dcc-141">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="44dcc-141">notApplicableDeviceCount</span></span>|<span data-ttu-id="44dcc-142">Int32</span><span class="sxs-lookup"><span data-stu-id="44dcc-142">Int32</span></span>|<span data-ttu-id="44dcc-143">不适用设备的数量</span><span class="sxs-lookup"><span data-stu-id="44dcc-143">Number of not applicable devices</span></span>|
|<span data-ttu-id="44dcc-144">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="44dcc-144">compliantDeviceCount</span></span>|<span data-ttu-id="44dcc-145">Int32</span><span class="sxs-lookup"><span data-stu-id="44dcc-145">Int32</span></span>|<span data-ttu-id="44dcc-146">兼容设备的数量</span><span class="sxs-lookup"><span data-stu-id="44dcc-146">Number of compliant devices</span></span>|
|<span data-ttu-id="44dcc-147">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="44dcc-147">remediatedDeviceCount</span></span>|<span data-ttu-id="44dcc-148">Int32</span><span class="sxs-lookup"><span data-stu-id="44dcc-148">Int32</span></span>|<span data-ttu-id="44dcc-149">已修复设备的数量</span><span class="sxs-lookup"><span data-stu-id="44dcc-149">Number of remediated devices</span></span>|
|<span data-ttu-id="44dcc-150">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="44dcc-150">nonCompliantDeviceCount</span></span>|<span data-ttu-id="44dcc-151">Int32</span><span class="sxs-lookup"><span data-stu-id="44dcc-151">Int32</span></span>|<span data-ttu-id="44dcc-152">不兼容设备的数量</span><span class="sxs-lookup"><span data-stu-id="44dcc-152">Number of NonCompliant devices</span></span>|
|<span data-ttu-id="44dcc-153">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="44dcc-153">errorDeviceCount</span></span>|<span data-ttu-id="44dcc-154">Int32</span><span class="sxs-lookup"><span data-stu-id="44dcc-154">Int32</span></span>|<span data-ttu-id="44dcc-155">错误设备的数量</span><span class="sxs-lookup"><span data-stu-id="44dcc-155">Number of error devices</span></span>|
|<span data-ttu-id="44dcc-156">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="44dcc-156">conflictDeviceCount</span></span>|<span data-ttu-id="44dcc-157">Int32</span><span class="sxs-lookup"><span data-stu-id="44dcc-157">Int32</span></span>|<span data-ttu-id="44dcc-158">冲突设备的数量</span><span class="sxs-lookup"><span data-stu-id="44dcc-158">Number of conflict devices</span></span>|



## <a name="response"></a><span data-ttu-id="44dcc-159">响应</span><span class="sxs-lookup"><span data-stu-id="44dcc-159">Response</span></span>
<span data-ttu-id="44dcc-160">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和更新的 [deviceCompliancePolicyDeviceStateSummary](../resources/intune_deviceconfig_devicecompliancepolicydevicestatesummary.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="44dcc-160">If successful, this method returns a `200 OK` response code and an updated [deviceCompliancePolicyDeviceStateSummary](../resources/intune_deviceconfig_devicecompliancepolicydevicestatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="44dcc-161">示例</span><span class="sxs-lookup"><span data-stu-id="44dcc-161">Example</span></span>
### <a name="request"></a><span data-ttu-id="44dcc-162">请求</span><span class="sxs-lookup"><span data-stu-id="44dcc-162">Request</span></span>
<span data-ttu-id="44dcc-163">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="44dcc-163">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicyDeviceStateSummary
Content-type: application/json
Content-length: 349

{
  "@odata.type": "#microsoft.graph.deviceCompliancePolicyDeviceStateSummary",
  "inGracePeriodCount": 2,
  "configManagerCount": 2,
  "unknownDeviceCount": 2,
  "notApplicableDeviceCount": 8,
  "compliantDeviceCount": 4,
  "remediatedDeviceCount": 5,
  "nonCompliantDeviceCount": 7,
  "errorDeviceCount": 0,
  "conflictDeviceCount": 3
}
```

### <a name="response"></a><span data-ttu-id="44dcc-164">响应</span><span class="sxs-lookup"><span data-stu-id="44dcc-164">Response</span></span>
<span data-ttu-id="44dcc-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="44dcc-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 398

{
  "@odata.type": "#microsoft.graph.deviceCompliancePolicyDeviceStateSummary",
  "inGracePeriodCount": 2,
  "configManagerCount": 2,
  "id": "8c4de8a7-e8a7-8c4d-a7e8-4d8ca7e84d8c",
  "unknownDeviceCount": 2,
  "notApplicableDeviceCount": 8,
  "compliantDeviceCount": 4,
  "remediatedDeviceCount": 5,
  "nonCompliantDeviceCount": 7,
  "errorDeviceCount": 0,
  "conflictDeviceCount": 3
}
```



