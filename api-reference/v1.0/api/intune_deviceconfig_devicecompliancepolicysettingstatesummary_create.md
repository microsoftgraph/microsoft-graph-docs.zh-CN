# <a name="create-devicecompliancepolicysettingstatesummary"></a><span data-ttu-id="3e09b-101">创建 deviceCompliancePolicySettingStateSummary</span><span class="sxs-lookup"><span data-stu-id="3e09b-101">Create deviceCompliancePolicySettingStateSummary</span></span>

> <span data-ttu-id="3e09b-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="3e09b-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3e09b-103">创建新的 [deviceCompliancePolicySettingStateSummary](../resources/intune_deviceconfig_devicecompliancepolicysettingstatesummary.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="3e09b-103">Create a new [deviceCompliancePolicySettingStateSummary](../resources/intune_deviceconfig_devicecompliancepolicysettingstatesummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="3e09b-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="3e09b-104">Prerequisites</span></span>
<span data-ttu-id="3e09b-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="3e09b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="3e09b-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="3e09b-107">Permission type</span></span>|<span data-ttu-id="3e09b-108">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="3e09b-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3e09b-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3e09b-109">Delegated (work or school account)</span></span>|<span data-ttu-id="3e09b-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3e09b-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="3e09b-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3e09b-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3e09b-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="3e09b-112">Not supported.</span></span>|
|<span data-ttu-id="3e09b-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="3e09b-113">Application</span></span>|<span data-ttu-id="3e09b-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="3e09b-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3e09b-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3e09b-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicySettingStateSummaries
```

## <a name="request-headers"></a><span data-ttu-id="3e09b-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="3e09b-116">Request headers</span></span>
|<span data-ttu-id="3e09b-117">标头</span><span class="sxs-lookup"><span data-stu-id="3e09b-117">Header</span></span>|<span data-ttu-id="3e09b-118">值</span><span class="sxs-lookup"><span data-stu-id="3e09b-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3e09b-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="3e09b-119">Authorization</span></span>|<span data-ttu-id="3e09b-120">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="3e09b-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3e09b-121">Accept</span><span class="sxs-lookup"><span data-stu-id="3e09b-121">Accept</span></span>|<span data-ttu-id="3e09b-122">application/json</span><span class="sxs-lookup"><span data-stu-id="3e09b-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3e09b-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="3e09b-123">Request body</span></span>
<span data-ttu-id="3e09b-124">在请求正文中，提供 deviceCompliancePolicySettingStateSummary 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3e09b-124">In the request body, supply a JSON representation for the deviceCompliancePolicySettingStateSummary object.</span></span>

<span data-ttu-id="3e09b-125">下表显示了创建 deviceCompliancePolicySettingStateSummary 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="3e09b-125">The following table shows the properties that are required when you create the deviceCompliancePolicySettingStateSummary.</span></span>

|<span data-ttu-id="3e09b-126">属性</span><span class="sxs-lookup"><span data-stu-id="3e09b-126">Property</span></span>|<span data-ttu-id="3e09b-127">类型</span><span class="sxs-lookup"><span data-stu-id="3e09b-127">Type</span></span>|<span data-ttu-id="3e09b-128">说明</span><span class="sxs-lookup"><span data-stu-id="3e09b-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3e09b-129">id</span><span class="sxs-lookup"><span data-stu-id="3e09b-129">id</span></span>|<span data-ttu-id="3e09b-130">String</span><span class="sxs-lookup"><span data-stu-id="3e09b-130">String</span></span>|<span data-ttu-id="3e09b-131">实体的键。</span><span class="sxs-lookup"><span data-stu-id="3e09b-131">Key of the entity.</span></span>|
|<span data-ttu-id="3e09b-132">setting</span><span class="sxs-lookup"><span data-stu-id="3e09b-132">setting</span></span>|<span data-ttu-id="3e09b-133">String</span><span class="sxs-lookup"><span data-stu-id="3e09b-133">String</span></span>|<span data-ttu-id="3e09b-134">设置类名和属性名。</span><span class="sxs-lookup"><span data-stu-id="3e09b-134">The setting class name and property name.</span></span>|
|<span data-ttu-id="3e09b-135">settingName</span><span class="sxs-lookup"><span data-stu-id="3e09b-135">settingName</span></span>|<span data-ttu-id="3e09b-136">String</span><span class="sxs-lookup"><span data-stu-id="3e09b-136">String</span></span>|<span data-ttu-id="3e09b-137">设置的名称。</span><span class="sxs-lookup"><span data-stu-id="3e09b-137">Name of the setting.</span></span>|
|<span data-ttu-id="3e09b-138">platformType</span><span class="sxs-lookup"><span data-stu-id="3e09b-138">platformType</span></span>|[<span data-ttu-id="3e09b-139">policyPlatformType</span><span class="sxs-lookup"><span data-stu-id="3e09b-139">policyPlatformType</span></span>](../resources/intune_deviceconfig_policyplatformtype.md)|<span data-ttu-id="3e09b-140">设置平台。</span><span class="sxs-lookup"><span data-stu-id="3e09b-140">Setting platform.</span></span> <span data-ttu-id="3e09b-141">可取值为：`android`、`iOS`、`macOS`、`windowsPhone81`、`windows81AndLater`、`windows10AndLater`、`androidWorkProfile`、`all`。</span><span class="sxs-lookup"><span data-stu-id="3e09b-141">Possible values are: `android`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `all`.</span></span>|
|<span data-ttu-id="3e09b-142">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="3e09b-142">unknownDeviceCount</span></span>|<span data-ttu-id="3e09b-143">Int32</span><span class="sxs-lookup"><span data-stu-id="3e09b-143">Int32</span></span>|<span data-ttu-id="3e09b-144">未知设备的数量</span><span class="sxs-lookup"><span data-stu-id="3e09b-144">Number of unknown devices</span></span>|
|<span data-ttu-id="3e09b-145">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="3e09b-145">notApplicableDeviceCount</span></span>|<span data-ttu-id="3e09b-146">Int32</span><span class="sxs-lookup"><span data-stu-id="3e09b-146">Int32</span></span>|<span data-ttu-id="3e09b-147">不适用设备的数量</span><span class="sxs-lookup"><span data-stu-id="3e09b-147">Number of not applicable devices</span></span>|
|<span data-ttu-id="3e09b-148">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="3e09b-148">compliantDeviceCount</span></span>|<span data-ttu-id="3e09b-149">Int32</span><span class="sxs-lookup"><span data-stu-id="3e09b-149">Int32</span></span>|<span data-ttu-id="3e09b-150">兼容设备的数量</span><span class="sxs-lookup"><span data-stu-id="3e09b-150">Number of compliant devices</span></span>|
|<span data-ttu-id="3e09b-151">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="3e09b-151">remediatedDeviceCount</span></span>|<span data-ttu-id="3e09b-152">Int32</span><span class="sxs-lookup"><span data-stu-id="3e09b-152">Int32</span></span>|<span data-ttu-id="3e09b-153">已修复设备的数量</span><span class="sxs-lookup"><span data-stu-id="3e09b-153">Number of remediated devices</span></span>|
|<span data-ttu-id="3e09b-154">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="3e09b-154">nonCompliantDeviceCount</span></span>|<span data-ttu-id="3e09b-155">Int32</span><span class="sxs-lookup"><span data-stu-id="3e09b-155">Int32</span></span>|<span data-ttu-id="3e09b-156">不兼容设备的数量</span><span class="sxs-lookup"><span data-stu-id="3e09b-156">Number of NonCompliant devices</span></span>|
|<span data-ttu-id="3e09b-157">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="3e09b-157">errorDeviceCount</span></span>|<span data-ttu-id="3e09b-158">Int32</span><span class="sxs-lookup"><span data-stu-id="3e09b-158">Int32</span></span>|<span data-ttu-id="3e09b-159">错误设备的数量</span><span class="sxs-lookup"><span data-stu-id="3e09b-159">Number of error devices</span></span>|
|<span data-ttu-id="3e09b-160">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="3e09b-160">conflictDeviceCount</span></span>|<span data-ttu-id="3e09b-161">Int32</span><span class="sxs-lookup"><span data-stu-id="3e09b-161">Int32</span></span>|<span data-ttu-id="3e09b-162">冲突设备的数量</span><span class="sxs-lookup"><span data-stu-id="3e09b-162">Number of conflict devices</span></span>|



## <a name="response"></a><span data-ttu-id="3e09b-163">响应</span><span class="sxs-lookup"><span data-stu-id="3e09b-163">Response</span></span>
<span data-ttu-id="3e09b-164">如果成功，此方法将在响应正文中返回 `201 Created` 响应代码和 [deviceCompliancePolicySettingStateSummary](../resources/intune_deviceconfig_devicecompliancepolicysettingstatesummary.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="3e09b-164">If successful, this method returns a `201 Created` response code and a [deviceCompliancePolicySettingStateSummary](../resources/intune_deviceconfig_devicecompliancepolicysettingstatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3e09b-165">示例</span><span class="sxs-lookup"><span data-stu-id="3e09b-165">Example</span></span>
### <a name="request"></a><span data-ttu-id="3e09b-166">请求</span><span class="sxs-lookup"><span data-stu-id="3e09b-166">Request</span></span>
<span data-ttu-id="3e09b-167">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="3e09b-167">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicySettingStateSummaries
Content-type: application/json
Content-length: 391

{
  "@odata.type": "#microsoft.graph.deviceCompliancePolicySettingStateSummary",
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

### <a name="response"></a><span data-ttu-id="3e09b-168">响应</span><span class="sxs-lookup"><span data-stu-id="3e09b-168">Response</span></span>
<span data-ttu-id="3e09b-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="3e09b-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 440

{
  "@odata.type": "#microsoft.graph.deviceCompliancePolicySettingStateSummary",
  "id": "7474d6d5-d6d5-7474-d5d6-7474d5d67474",
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



