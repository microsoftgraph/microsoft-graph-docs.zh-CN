# <a name="create-devicecompliancepolicysettingstatesummary"></a><span data-ttu-id="801a1-101">创建 deviceCompliancePolicySettingStateSummary</span><span class="sxs-lookup"><span data-stu-id="801a1-101">Create deviceCompliancePolicySettingStateSummary</span></span>

> <span data-ttu-id="801a1-102">**注意：**使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="801a1-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="801a1-103">创建新的 [deviceCompliancePolicySettingStateSummary](../resources/intune_deviceconfig_devicecompliancepolicysettingstatesummary.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="801a1-103">Create a new [plannerBucket](../resources/intune_deviceconfig_devicecompliancepolicysettingstatesummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="801a1-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="801a1-104">Prerequisites</span></span>
<span data-ttu-id="801a1-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="801a1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="801a1-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="801a1-107">Permission type</span></span>|<span data-ttu-id="801a1-108">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="801a1-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="801a1-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="801a1-109">Delegated (work or school account)</span></span>|<span data-ttu-id="801a1-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="801a1-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="801a1-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="801a1-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="801a1-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="801a1-112">Not supported.</span></span>|
|<span data-ttu-id="801a1-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="801a1-113">Application</span></span>|<span data-ttu-id="801a1-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="801a1-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="801a1-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="801a1-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicySettingStateSummaries
```

## <a name="request-headers"></a><span data-ttu-id="801a1-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="801a1-116">Request headers</span></span>
|<span data-ttu-id="801a1-117">标头</span><span class="sxs-lookup"><span data-stu-id="801a1-117">Header</span></span>|<span data-ttu-id="801a1-118">值</span><span class="sxs-lookup"><span data-stu-id="801a1-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="801a1-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="801a1-119">Authorization</span></span>|<span data-ttu-id="801a1-120">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="801a1-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="801a1-121">Accept</span><span class="sxs-lookup"><span data-stu-id="801a1-121">Accept</span></span>|<span data-ttu-id="801a1-122">application/json</span><span class="sxs-lookup"><span data-stu-id="801a1-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="801a1-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="801a1-123">Request body</span></span>
<span data-ttu-id="801a1-124">在请求正文中，提供 deviceCompliancePolicySettingStateSummary 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="801a1-124">In the request body, supply a JSON representation of the schemaExtension object.</span></span>

<span data-ttu-id="801a1-125">下表显示了创建 deviceCompliancePolicySettingStateSummary 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="801a1-125">The following table shows the properties that are required when you create a user.</span></span>

|<span data-ttu-id="801a1-126">属性</span><span class="sxs-lookup"><span data-stu-id="801a1-126">Property</span></span>|<span data-ttu-id="801a1-127">类型</span><span class="sxs-lookup"><span data-stu-id="801a1-127">Type</span></span>|<span data-ttu-id="801a1-128">说明</span><span class="sxs-lookup"><span data-stu-id="801a1-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="801a1-129">setting</span><span class="sxs-lookup"><span data-stu-id="801a1-129">setting</span></span>|<span data-ttu-id="801a1-130">String</span><span class="sxs-lookup"><span data-stu-id="801a1-130">String</span></span>|<span data-ttu-id="801a1-131">设置类名和属性名。</span><span class="sxs-lookup"><span data-stu-id="801a1-131">The setting class name and property name.</span></span>|
|<span data-ttu-id="801a1-132">settingName</span><span class="sxs-lookup"><span data-stu-id="801a1-132">settingName</span></span>|<span data-ttu-id="801a1-133">String</span><span class="sxs-lookup"><span data-stu-id="801a1-133">String</span></span>|<span data-ttu-id="801a1-134">设置的名称。</span><span class="sxs-lookup"><span data-stu-id="801a1-134">Name of the setting.</span></span>|
|<span data-ttu-id="801a1-135">platformType</span><span class="sxs-lookup"><span data-stu-id="801a1-135">PlatformType</span></span>|<span data-ttu-id="801a1-136">String</span><span class="sxs-lookup"><span data-stu-id="801a1-136">String</span></span>|<span data-ttu-id="801a1-137">设置平台。可取值为：`android`、`iOS`、`macOS`、`windowsPhone81`、`windows81AndLater`、`windows10AndLater`、`all`。</span><span class="sxs-lookup"><span data-stu-id="801a1-137">Setting platform Possible values are: `android`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `all`.</span></span>|
|<span data-ttu-id="801a1-138">id</span><span class="sxs-lookup"><span data-stu-id="801a1-138">id</span></span>|<span data-ttu-id="801a1-139">String</span><span class="sxs-lookup"><span data-stu-id="801a1-139">String</span></span>|<span data-ttu-id="801a1-140">实体的键。</span><span class="sxs-lookup"><span data-stu-id="801a1-140">Key of the setting.</span></span>|
|<span data-ttu-id="801a1-141">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="801a1-141">unknownDeviceCount</span></span>|<span data-ttu-id="801a1-142">Int32</span><span class="sxs-lookup"><span data-stu-id="801a1-142">Int32</span></span>|<span data-ttu-id="801a1-143">未知设备的数量</span><span class="sxs-lookup"><span data-stu-id="801a1-143">Number of unknown devices</span></span>|
|<span data-ttu-id="801a1-144">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="801a1-144">notApplicableDeviceCount</span></span>|<span data-ttu-id="801a1-145">Int32</span><span class="sxs-lookup"><span data-stu-id="801a1-145">Int32</span></span>|<span data-ttu-id="801a1-146">不适用设备的数量</span><span class="sxs-lookup"><span data-stu-id="801a1-146">Number of not applicable devices</span></span>|
|<span data-ttu-id="801a1-147">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="801a1-147">compliantDeviceCount</span></span>|<span data-ttu-id="801a1-148">Int32</span><span class="sxs-lookup"><span data-stu-id="801a1-148">Int32</span></span>|<span data-ttu-id="801a1-149">兼容设备的数量</span><span class="sxs-lookup"><span data-stu-id="801a1-149">Number of compliant devices</span></span>|
|<span data-ttu-id="801a1-150">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="801a1-150">remediatedDeviceCount</span></span>|<span data-ttu-id="801a1-151">Int32</span><span class="sxs-lookup"><span data-stu-id="801a1-151">Int32</span></span>|<span data-ttu-id="801a1-152">已修复设备数</span><span class="sxs-lookup"><span data-stu-id="801a1-152">Number of remediated devices</span></span>|
|<span data-ttu-id="801a1-153">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="801a1-153">nonCompliantDeviceCount</span></span>|<span data-ttu-id="801a1-154">Int32</span><span class="sxs-lookup"><span data-stu-id="801a1-154">Int32</span></span>|<span data-ttu-id="801a1-155">不兼容设备的数量</span><span class="sxs-lookup"><span data-stu-id="801a1-155">Number of NonCompliant devices</span></span>|
|<span data-ttu-id="801a1-156">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="801a1-156">errorDeviceCount</span></span>|<span data-ttu-id="801a1-157">Int32</span><span class="sxs-lookup"><span data-stu-id="801a1-157">Int32</span></span>|<span data-ttu-id="801a1-158">错误设备的数量</span><span class="sxs-lookup"><span data-stu-id="801a1-158">Number of error devices</span></span>|
|<span data-ttu-id="801a1-159">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="801a1-159">conflictDeviceCount</span></span>|<span data-ttu-id="801a1-160">Int32</span><span class="sxs-lookup"><span data-stu-id="801a1-160">Int32</span></span>|<span data-ttu-id="801a1-161">冲突设备的数量</span><span class="sxs-lookup"><span data-stu-id="801a1-161">Number of conflict devices</span></span>|



## <a name="response"></a><span data-ttu-id="801a1-162">响应</span><span class="sxs-lookup"><span data-stu-id="801a1-162">Response</span></span>
<span data-ttu-id="801a1-163">如果成功，此方法将在响应正文中返回 `201 Created` 响应代码和 [deviceCompliancePolicySettingStateSummary](../resources/intune_deviceconfig_devicecompliancepolicysettingstatesummary.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="801a1-163">If successful, this method returns a `201 Created` response code and a [directoryObject](../resources/intune_deviceconfig_devicecompliancepolicysettingstatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="801a1-164">示例</span><span class="sxs-lookup"><span data-stu-id="801a1-164">Example</span></span>
### <a name="request"></a><span data-ttu-id="801a1-165">请求</span><span class="sxs-lookup"><span data-stu-id="801a1-165">Request</span></span>
<span data-ttu-id="801a1-166">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="801a1-166">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="801a1-167">响应</span><span class="sxs-lookup"><span data-stu-id="801a1-167">Response</span></span>
<span data-ttu-id="801a1-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="801a1-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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



