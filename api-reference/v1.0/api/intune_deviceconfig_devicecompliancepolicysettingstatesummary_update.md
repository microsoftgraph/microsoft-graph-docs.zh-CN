# <a name="update-devicecompliancepolicysettingstatesummary"></a><span data-ttu-id="a1dff-101">更新 deviceCompliancePolicySettingStateSummary</span><span class="sxs-lookup"><span data-stu-id="a1dff-101">Update deviceCompliancePolicySettingStateSummary</span></span>

> <span data-ttu-id="a1dff-102">**注意：**使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="a1dff-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a1dff-103">更新 [deviceCompliancePolicySettingStateSummary](../resources/intune_deviceconfig_devicecompliancepolicysettingstatesummary.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="a1dff-103">Update the properties of a [calendar](../resources/intune_deviceconfig_devicecompliancepolicysettingstatesummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="a1dff-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="a1dff-104">Prerequisites</span></span>
<span data-ttu-id="a1dff-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="a1dff-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="a1dff-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="a1dff-107">Permission type</span></span>|<span data-ttu-id="a1dff-108">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="a1dff-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a1dff-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a1dff-109">Delegated (work or school account)</span></span>|<span data-ttu-id="a1dff-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a1dff-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a1dff-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a1dff-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a1dff-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="a1dff-112">Not supported.</span></span>|
|<span data-ttu-id="a1dff-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="a1dff-113">Application</span></span>|<span data-ttu-id="a1dff-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="a1dff-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a1dff-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a1dff-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicySettingStateSummaries/{deviceCompliancePolicySettingStateSummaryId}
```

## <a name="request-headers"></a><span data-ttu-id="a1dff-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="a1dff-116">Request headers</span></span>
|<span data-ttu-id="a1dff-117">标头</span><span class="sxs-lookup"><span data-stu-id="a1dff-117">Header</span></span>|<span data-ttu-id="a1dff-118">值</span><span class="sxs-lookup"><span data-stu-id="a1dff-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a1dff-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="a1dff-119">Authorization</span></span>|<span data-ttu-id="a1dff-120">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="a1dff-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="a1dff-121">Accept</span><span class="sxs-lookup"><span data-stu-id="a1dff-121">Accept</span></span>|<span data-ttu-id="a1dff-122">application/json</span><span class="sxs-lookup"><span data-stu-id="a1dff-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a1dff-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="a1dff-123">Request body</span></span>
<span data-ttu-id="a1dff-124">在请求正文中，提供 [deviceCompliancePolicySettingStateSummary](../resources/intune_deviceconfig_devicecompliancepolicysettingstatesummary.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a1dff-124">In the request body, supply a JSON representation of the [Contact](../resources/intune_deviceconfig_devicecompliancepolicysettingstatesummary.md) object.</span></span>

<span data-ttu-id="a1dff-125">下表显示创建 [deviceCompliancePolicySettingStateSummary](../resources/intune_deviceconfig_devicecompliancepolicysettingstatesummary.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="a1dff-125">The following table shows the properties that are required when you create a user.</span></span>

|<span data-ttu-id="a1dff-126">属性</span><span class="sxs-lookup"><span data-stu-id="a1dff-126">Property</span></span>|<span data-ttu-id="a1dff-127">类型</span><span class="sxs-lookup"><span data-stu-id="a1dff-127">Type</span></span>|<span data-ttu-id="a1dff-128">说明</span><span class="sxs-lookup"><span data-stu-id="a1dff-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a1dff-129">setting</span><span class="sxs-lookup"><span data-stu-id="a1dff-129">setting</span></span>|<span data-ttu-id="a1dff-130">String</span><span class="sxs-lookup"><span data-stu-id="a1dff-130">String</span></span>|<span data-ttu-id="a1dff-131">设置类名和属性名。</span><span class="sxs-lookup"><span data-stu-id="a1dff-131">The setting class name and property name.</span></span>|
|<span data-ttu-id="a1dff-132">settingName</span><span class="sxs-lookup"><span data-stu-id="a1dff-132">settingName</span></span>|<span data-ttu-id="a1dff-133">String</span><span class="sxs-lookup"><span data-stu-id="a1dff-133">String</span></span>|<span data-ttu-id="a1dff-134">设置的名称。</span><span class="sxs-lookup"><span data-stu-id="a1dff-134">Name of the setting.</span></span>|
|<span data-ttu-id="a1dff-135">platformType</span><span class="sxs-lookup"><span data-stu-id="a1dff-135">PlatformType</span></span>|<span data-ttu-id="a1dff-136">String</span><span class="sxs-lookup"><span data-stu-id="a1dff-136">String</span></span>|<span data-ttu-id="a1dff-137">设置平台。可取值为：`android`、`iOS`、`macOS`、`windowsPhone81`、`windows81AndLater`、`windows10AndLater`、`all`。</span><span class="sxs-lookup"><span data-stu-id="a1dff-137">Setting platform Possible values are: `android`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `all`.</span></span>|
|<span data-ttu-id="a1dff-138">id</span><span class="sxs-lookup"><span data-stu-id="a1dff-138">id</span></span>|<span data-ttu-id="a1dff-139">String</span><span class="sxs-lookup"><span data-stu-id="a1dff-139">String</span></span>|<span data-ttu-id="a1dff-140">实体的键。</span><span class="sxs-lookup"><span data-stu-id="a1dff-140">Key of the setting.</span></span>|
|<span data-ttu-id="a1dff-141">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="a1dff-141">unknownDeviceCount</span></span>|<span data-ttu-id="a1dff-142">Int32</span><span class="sxs-lookup"><span data-stu-id="a1dff-142">Int32</span></span>|<span data-ttu-id="a1dff-143">未知设备的数量</span><span class="sxs-lookup"><span data-stu-id="a1dff-143">Number of unknown devices</span></span>|
|<span data-ttu-id="a1dff-144">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="a1dff-144">notApplicableDeviceCount</span></span>|<span data-ttu-id="a1dff-145">Int32</span><span class="sxs-lookup"><span data-stu-id="a1dff-145">Int32</span></span>|<span data-ttu-id="a1dff-146">不适用设备的数量</span><span class="sxs-lookup"><span data-stu-id="a1dff-146">Number of not applicable devices</span></span>|
|<span data-ttu-id="a1dff-147">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="a1dff-147">compliantDeviceCount</span></span>|<span data-ttu-id="a1dff-148">Int32</span><span class="sxs-lookup"><span data-stu-id="a1dff-148">Int32</span></span>|<span data-ttu-id="a1dff-149">兼容设备的数量</span><span class="sxs-lookup"><span data-stu-id="a1dff-149">Number of compliant devices</span></span>|
|<span data-ttu-id="a1dff-150">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="a1dff-150">remediatedDeviceCount</span></span>|<span data-ttu-id="a1dff-151">Int32</span><span class="sxs-lookup"><span data-stu-id="a1dff-151">Int32</span></span>|<span data-ttu-id="a1dff-152">已修复设备的数量</span><span class="sxs-lookup"><span data-stu-id="a1dff-152">Number of remediated devices</span></span>|
|<span data-ttu-id="a1dff-153">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="a1dff-153">nonCompliantDeviceCount</span></span>|<span data-ttu-id="a1dff-154">Int32</span><span class="sxs-lookup"><span data-stu-id="a1dff-154">Int32</span></span>|<span data-ttu-id="a1dff-155">不兼容设备的数量</span><span class="sxs-lookup"><span data-stu-id="a1dff-155">Number of NonCompliant devices</span></span>|
|<span data-ttu-id="a1dff-156">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="a1dff-156">errorDeviceCount</span></span>|<span data-ttu-id="a1dff-157">Int32</span><span class="sxs-lookup"><span data-stu-id="a1dff-157">Int32</span></span>|<span data-ttu-id="a1dff-158">错误设备的数量</span><span class="sxs-lookup"><span data-stu-id="a1dff-158">Number of error devices</span></span>|
|<span data-ttu-id="a1dff-159">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="a1dff-159">conflictDeviceCount</span></span>|<span data-ttu-id="a1dff-160">Int32</span><span class="sxs-lookup"><span data-stu-id="a1dff-160">Int32</span></span>|<span data-ttu-id="a1dff-161">冲突设备的数量</span><span class="sxs-lookup"><span data-stu-id="a1dff-161">Number of conflict devices</span></span>|



## <a name="response"></a><span data-ttu-id="a1dff-162">响应</span><span class="sxs-lookup"><span data-stu-id="a1dff-162">Response</span></span>
<span data-ttu-id="a1dff-163">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和更新的 [deviceCompliancePolicySettingStateSummary](../resources/intune_deviceconfig_devicecompliancepolicysettingstatesummary.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="a1dff-163">If successful, this method returns a `200 OK` response code and an updated [contact](../resources/intune_deviceconfig_devicecompliancepolicysettingstatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a1dff-164">示例</span><span class="sxs-lookup"><span data-stu-id="a1dff-164">Example</span></span>
### <a name="request"></a><span data-ttu-id="a1dff-165">请求</span><span class="sxs-lookup"><span data-stu-id="a1dff-165">Request</span></span>
<span data-ttu-id="a1dff-166">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="a1dff-166">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicySettingStateSummaries/{deviceCompliancePolicySettingStateSummaryId}
Content-type: application/json
Content-length: 311

{
  "setting": "Setting value",
  "settingName": "Setting Name value",
  "platformType": "iOS",
  "unknownDeviceCount": 2,
  "notApplicableDeviceCount": 8,
  "compliantDeviceCount": 4,
  "remediatedDeviceCount": 5,
  "nonCompliantDeviceCount": 7,
  "errorDeviceCount": 0,
  "conflictDeviceCount": 3
}
```

### <a name="response"></a><span data-ttu-id="a1dff-167">响应</span><span class="sxs-lookup"><span data-stu-id="a1dff-167">Response</span></span>
<span data-ttu-id="a1dff-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="a1dff-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 440

{
  "@odata.type": "#microsoft.graph.deviceCompliancePolicySettingStateSummary",
  "setting": "Setting value",
  "settingName": "Setting Name value",
  "platformType": "iOS",
  "id": "7474d6d5-d6d5-7474-d5d6-7474d5d67474",
  "unknownDeviceCount": 2,
  "notApplicableDeviceCount": 8,
  "compliantDeviceCount": 4,
  "remediatedDeviceCount": 5,
  "nonCompliantDeviceCount": 7,
  "errorDeviceCount": 0,
  "conflictDeviceCount": 3
}
```



