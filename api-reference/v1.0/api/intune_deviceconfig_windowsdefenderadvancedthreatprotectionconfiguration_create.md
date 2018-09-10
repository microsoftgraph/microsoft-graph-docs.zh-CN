# <a name="create-windowsdefenderadvancedthreatprotectionconfiguration"></a><span data-ttu-id="8a34e-101">创建 windowsDefenderAdvancedThreatProtectionConfiguration</span><span class="sxs-lookup"><span data-stu-id="8a34e-101">Create windowsDefenderAdvancedThreatProtectionConfiguration</span></span>

> <span data-ttu-id="8a34e-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="8a34e-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8a34e-103">创建新的 [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune_deviceconfig_windowsdefenderadvancedthreatprotectionconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="8a34e-103">Create a new [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune_deviceconfig_windowsdefenderadvancedthreatprotectionconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="8a34e-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="8a34e-104">Prerequisites</span></span>
<span data-ttu-id="8a34e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="8a34e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="8a34e-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="8a34e-107">Permission type</span></span>|<span data-ttu-id="8a34e-108">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="8a34e-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8a34e-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8a34e-109">Delegated (work or school account)</span></span>|<span data-ttu-id="8a34e-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8a34e-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="8a34e-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8a34e-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8a34e-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="8a34e-112">Not supported.</span></span>|
|<span data-ttu-id="8a34e-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="8a34e-113">Application</span></span>|<span data-ttu-id="8a34e-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="8a34e-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8a34e-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8a34e-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="8a34e-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="8a34e-116">Request headers</span></span>
|<span data-ttu-id="8a34e-117">标头</span><span class="sxs-lookup"><span data-stu-id="8a34e-117">Header</span></span>|<span data-ttu-id="8a34e-118">值</span><span class="sxs-lookup"><span data-stu-id="8a34e-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8a34e-119">授权</span><span class="sxs-lookup"><span data-stu-id="8a34e-119">Authorization</span></span>|<span data-ttu-id="8a34e-120">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="8a34e-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8a34e-121">Accept</span><span class="sxs-lookup"><span data-stu-id="8a34e-121">Accept</span></span>|<span data-ttu-id="8a34e-122">application/json</span><span class="sxs-lookup"><span data-stu-id="8a34e-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8a34e-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="8a34e-123">Request body</span></span>
<span data-ttu-id="8a34e-124">在请求正文中，提供 windowsDefenderAdvancedThreatProtectionConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8a34e-124">In the request body, supply a JSON representation for the windowsDefenderAdvancedThreatProtectionConfiguration object.</span></span>

<span data-ttu-id="8a34e-125">下表显示创建 windowsDefenderAdvancedThreatProtectionConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="8a34e-125">The following table shows the properties that are required when you create the windowsDefenderAdvancedThreatProtectionConfiguration.</span></span>

|<span data-ttu-id="8a34e-126">属性</span><span class="sxs-lookup"><span data-stu-id="8a34e-126">Property</span></span>|<span data-ttu-id="8a34e-127">类型</span><span class="sxs-lookup"><span data-stu-id="8a34e-127">Type</span></span>|<span data-ttu-id="8a34e-128">说明</span><span class="sxs-lookup"><span data-stu-id="8a34e-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8a34e-129">ID</span><span class="sxs-lookup"><span data-stu-id="8a34e-129">id</span></span>|<span data-ttu-id="8a34e-130">字符串</span><span class="sxs-lookup"><span data-stu-id="8a34e-130">String</span></span>|<span data-ttu-id="8a34e-131">实体的键。</span><span class="sxs-lookup"><span data-stu-id="8a34e-131">Key of the entity.</span></span> <span data-ttu-id="8a34e-132">继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8a34e-132">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8a34e-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8a34e-133">lastModifiedDateTime</span></span>|<span data-ttu-id="8a34e-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8a34e-134">DateTimeOffset</span></span>|<span data-ttu-id="8a34e-135">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="8a34e-135">DateTime the object was last modified.</span></span> <span data-ttu-id="8a34e-136">继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8a34e-136">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8a34e-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8a34e-137">createdDateTime</span></span>|<span data-ttu-id="8a34e-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8a34e-138">DateTimeOffset</span></span>|<span data-ttu-id="8a34e-139">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="8a34e-139">DateTime the object was created.</span></span> <span data-ttu-id="8a34e-140">继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8a34e-140">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8a34e-141">说明</span><span class="sxs-lookup"><span data-stu-id="8a34e-141">description</span></span>|<span data-ttu-id="8a34e-142">字符串</span><span class="sxs-lookup"><span data-stu-id="8a34e-142">String</span></span>|<span data-ttu-id="8a34e-143">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="8a34e-143">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="8a34e-144">继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8a34e-144">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8a34e-145">displayName</span><span class="sxs-lookup"><span data-stu-id="8a34e-145">displayName</span></span>|<span data-ttu-id="8a34e-146">字符串</span><span class="sxs-lookup"><span data-stu-id="8a34e-146">String</span></span>|<span data-ttu-id="8a34e-147">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="8a34e-147">Admin provided name of the device configuration.</span></span> <span data-ttu-id="8a34e-148">继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8a34e-148">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8a34e-149">version</span><span class="sxs-lookup"><span data-stu-id="8a34e-149">version</span></span>|<span data-ttu-id="8a34e-150">Int32</span><span class="sxs-lookup"><span data-stu-id="8a34e-150">Int32</span></span>|<span data-ttu-id="8a34e-151">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="8a34e-151">Version of the device configuration.</span></span> <span data-ttu-id="8a34e-152">继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8a34e-152">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8a34e-153">allowSampleSharing</span><span class="sxs-lookup"><span data-stu-id="8a34e-153">allowSampleSharing</span></span>|<span data-ttu-id="8a34e-154">布尔</span><span class="sxs-lookup"><span data-stu-id="8a34e-154">Boolean</span></span>|<span data-ttu-id="8a34e-155">Windows Defender 高级威胁防护“允许示例共享”规则</span><span class="sxs-lookup"><span data-stu-id="8a34e-155">Windows Defender AdvancedThreatProtection "Allow Sample Sharing" Rule</span></span>|
|<span data-ttu-id="8a34e-156">enableExpeditedTelemetryReporting</span><span class="sxs-lookup"><span data-stu-id="8a34e-156">enableExpeditedTelemetryReporting</span></span>|<span data-ttu-id="8a34e-157">布尔</span><span class="sxs-lookup"><span data-stu-id="8a34e-157">Boolean</span></span>|<span data-ttu-id="8a34e-158">加速 Windows Defender 高级威胁防护遥测报告的频率。</span><span class="sxs-lookup"><span data-stu-id="8a34e-158">Expedite Windows Defender Advanced Threat Protection telemetry reporting frequency.</span></span>|



## <a name="response"></a><span data-ttu-id="8a34e-159">响应</span><span class="sxs-lookup"><span data-stu-id="8a34e-159">Response</span></span>
<span data-ttu-id="8a34e-160">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune_deviceconfig_windowsdefenderadvancedthreatprotectionconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="8a34e-160">If successful, this method returns a `201 Created` response code and a [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune_deviceconfig_windowsdefenderadvancedthreatprotectionconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8a34e-161">示例</span><span class="sxs-lookup"><span data-stu-id="8a34e-161">Example</span></span>
### <a name="request"></a><span data-ttu-id="8a34e-162">请求</span><span class="sxs-lookup"><span data-stu-id="8a34e-162">Request</span></span>
<span data-ttu-id="8a34e-163">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="8a34e-163">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 331

{
  "@odata.type": "#microsoft.graph.windowsDefenderAdvancedThreatProtectionConfiguration",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "allowSampleSharing": true,
  "enableExpeditedTelemetryReporting": true
}
```

### <a name="response"></a><span data-ttu-id="8a34e-164">响应</span><span class="sxs-lookup"><span data-stu-id="8a34e-164">Response</span></span>
<span data-ttu-id="8a34e-p108">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="8a34e-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 439

{
  "@odata.type": "#microsoft.graph.windowsDefenderAdvancedThreatProtectionConfiguration",
  "id": "294373aa-73aa-2943-aa73-4329aa734329",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "allowSampleSharing": true,
  "enableExpeditedTelemetryReporting": true
}
```








