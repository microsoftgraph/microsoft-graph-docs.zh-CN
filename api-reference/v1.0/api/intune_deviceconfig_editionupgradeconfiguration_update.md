# <a name="update-editionupgradeconfiguration"></a><span data-ttu-id="18b82-101">更新 editionUpgradeConfiguration</span><span class="sxs-lookup"><span data-stu-id="18b82-101">Update editionUpgradeConfiguration</span></span>

> <span data-ttu-id="18b82-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="18b82-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="18b82-103">更新 [editionUpgradeConfiguration](../resources/intune_deviceconfig_editionupgradeconfiguration.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="18b82-103">Update the properties of a [editionUpgradeConfiguration](../resources/intune_deviceconfig_editionupgradeconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="18b82-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="18b82-104">Prerequisites</span></span>
<span data-ttu-id="18b82-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="18b82-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="18b82-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="18b82-107">Permission type</span></span>|<span data-ttu-id="18b82-108">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="18b82-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="18b82-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="18b82-109">Delegated (work or school account)</span></span>|<span data-ttu-id="18b82-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="18b82-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="18b82-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="18b82-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="18b82-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="18b82-112">Not supported.</span></span>|
|<span data-ttu-id="18b82-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="18b82-113">Application</span></span>|<span data-ttu-id="18b82-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="18b82-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="18b82-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="18b82-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="18b82-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="18b82-116">Request headers</span></span>
|<span data-ttu-id="18b82-117">标头</span><span class="sxs-lookup"><span data-stu-id="18b82-117">Header</span></span>|<span data-ttu-id="18b82-118">值</span><span class="sxs-lookup"><span data-stu-id="18b82-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="18b82-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="18b82-119">Authorization</span></span>|<span data-ttu-id="18b82-120">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="18b82-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="18b82-121">Accept</span><span class="sxs-lookup"><span data-stu-id="18b82-121">Accept</span></span>|<span data-ttu-id="18b82-122">application/json</span><span class="sxs-lookup"><span data-stu-id="18b82-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="18b82-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="18b82-123">Request body</span></span>
<span data-ttu-id="18b82-124">在请求正文中，提供 [editionUpgradeConfiguration](../resources/intune_deviceconfig_editionupgradeconfiguration.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="18b82-124">In the request body, supply a JSON representation for the [editionUpgradeConfiguration](../resources/intune_deviceconfig_editionupgradeconfiguration.md) object.</span></span>

<span data-ttu-id="18b82-125">下表显示创建 [editionUpgradeConfiguration](../resources/intune_deviceconfig_editionupgradeconfiguration.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="18b82-125">The following table shows the properties that are required when you create the [editionUpgradeConfiguration](../resources/intune_deviceconfig_editionupgradeconfiguration.md).</span></span>

|<span data-ttu-id="18b82-126">属性</span><span class="sxs-lookup"><span data-stu-id="18b82-126">Property</span></span>|<span data-ttu-id="18b82-127">类型</span><span class="sxs-lookup"><span data-stu-id="18b82-127">Type</span></span>|<span data-ttu-id="18b82-128">说明</span><span class="sxs-lookup"><span data-stu-id="18b82-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="18b82-129">id</span><span class="sxs-lookup"><span data-stu-id="18b82-129">id</span></span>|<span data-ttu-id="18b82-130">String</span><span class="sxs-lookup"><span data-stu-id="18b82-130">String</span></span>|<span data-ttu-id="18b82-131">实体的键。</span><span class="sxs-lookup"><span data-stu-id="18b82-131">Key of the entity.</span></span> <span data-ttu-id="18b82-132">继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="18b82-132">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="18b82-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="18b82-133">lastModifiedDateTime</span></span>|<span data-ttu-id="18b82-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="18b82-134">DateTimeOffset</span></span>|<span data-ttu-id="18b82-135">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="18b82-135">DateTime the object was last modified.</span></span> <span data-ttu-id="18b82-136">继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="18b82-136">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="18b82-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="18b82-137">createdDateTime</span></span>|<span data-ttu-id="18b82-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="18b82-138">DateTimeOffset</span></span>|<span data-ttu-id="18b82-139">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="18b82-139">DateTime the object was created.</span></span> <span data-ttu-id="18b82-140">继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="18b82-140">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="18b82-141">description</span><span class="sxs-lookup"><span data-stu-id="18b82-141">description</span></span>|<span data-ttu-id="18b82-142">String</span><span class="sxs-lookup"><span data-stu-id="18b82-142">String</span></span>|<span data-ttu-id="18b82-143">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="18b82-143">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="18b82-144">继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="18b82-144">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="18b82-145">displayName</span><span class="sxs-lookup"><span data-stu-id="18b82-145">displayName</span></span>|<span data-ttu-id="18b82-146">String</span><span class="sxs-lookup"><span data-stu-id="18b82-146">String</span></span>|<span data-ttu-id="18b82-147">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="18b82-147">Admin provided name of the device configuration.</span></span> <span data-ttu-id="18b82-148">继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="18b82-148">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="18b82-149">version</span><span class="sxs-lookup"><span data-stu-id="18b82-149">version</span></span>|<span data-ttu-id="18b82-150">Int32</span><span class="sxs-lookup"><span data-stu-id="18b82-150">Int32</span></span>|<span data-ttu-id="18b82-151">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="18b82-151">Version of the device configuration.</span></span> <span data-ttu-id="18b82-152">继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="18b82-152">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="18b82-153">licenseType</span><span class="sxs-lookup"><span data-stu-id="18b82-153">licenseType</span></span>|[<span data-ttu-id="18b82-154">editionUpgradeLicenseType</span><span class="sxs-lookup"><span data-stu-id="18b82-154">editionUpgradeLicenseType</span></span>](../resources/intune_deviceconfig_editionupgradelicensetype.md)|<span data-ttu-id="18b82-155">版本升级许可证类型。</span><span class="sxs-lookup"><span data-stu-id="18b82-155">Edition Upgrade License Type.</span></span> <span data-ttu-id="18b82-156">可取值为：`productKey`、`licenseFile`。</span><span class="sxs-lookup"><span data-stu-id="18b82-156">Possible values are: `productKey`, `licenseFile`.</span></span>|
|<span data-ttu-id="18b82-157">targetEdition</span><span class="sxs-lookup"><span data-stu-id="18b82-157">targetEdition</span></span>|[<span data-ttu-id="18b82-158">windows10EditionType</span><span class="sxs-lookup"><span data-stu-id="18b82-158">windows10EditionType</span></span>](../resources/intune_deviceconfig_windows10editiontype.md)|<span data-ttu-id="18b82-159">版本升级目标版本。</span><span class="sxs-lookup"><span data-stu-id="18b82-159">Edition Upgrade Target Edition.</span></span> <span data-ttu-id="18b82-160">可取值为：`windows10Enterprise`、`windows10EnterpriseN`、`windows10Education`、`windows10EducationN`、`windows10MobileEnterprise`、`windows10HolographicEnterprise`、`windows10Professional`、`windows10ProfessionalN`、`windows10ProfessionalEducation`、`windows10ProfessionalEducationN`、`windows10ProfessionalWorkstation`、`windows10ProfessionalWorkstationN`。</span><span class="sxs-lookup"><span data-stu-id="18b82-160">Possible values are: `windows10Enterprise`, `windows10EnterpriseN`, `windows10Education`, `windows10EducationN`, `windows10MobileEnterprise`, `windows10HolographicEnterprise`, `windows10Professional`, `windows10ProfessionalN`, `windows10ProfessionalEducation`, `windows10ProfessionalEducationN`, `windows10ProfessionalWorkstation`, `windows10ProfessionalWorkstationN`.</span></span>|
|<span data-ttu-id="18b82-161">license</span><span class="sxs-lookup"><span data-stu-id="18b82-161">license</span></span>|<span data-ttu-id="18b82-162">String</span><span class="sxs-lookup"><span data-stu-id="18b82-162">String</span></span>|<span data-ttu-id="18b82-163">版本升级许可证文件内容。</span><span class="sxs-lookup"><span data-stu-id="18b82-163">Edition Upgrade License File Content.</span></span>|
|<span data-ttu-id="18b82-164">productKey</span><span class="sxs-lookup"><span data-stu-id="18b82-164">productKey</span></span>|<span data-ttu-id="18b82-165">String</span><span class="sxs-lookup"><span data-stu-id="18b82-165">String</span></span>|<span data-ttu-id="18b82-166">版本升级产品密钥。</span><span class="sxs-lookup"><span data-stu-id="18b82-166">Edition Upgrade Product Key.</span></span>|



## <a name="response"></a><span data-ttu-id="18b82-167">响应</span><span class="sxs-lookup"><span data-stu-id="18b82-167">Response</span></span>
<span data-ttu-id="18b82-168">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [editionUpgradeConfiguration](../resources/intune_deviceconfig_editionupgradeconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="18b82-168">If successful, this method returns a `200 OK` response code and an updated [editionUpgradeConfiguration](../resources/intune_deviceconfig_editionupgradeconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="18b82-169">示例</span><span class="sxs-lookup"><span data-stu-id="18b82-169">Example</span></span>
### <a name="request"></a><span data-ttu-id="18b82-170">请求</span><span class="sxs-lookup"><span data-stu-id="18b82-170">Request</span></span>
<span data-ttu-id="18b82-171">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="18b82-171">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 311

{
  "@odata.type": "#microsoft.graph.editionUpgradeConfiguration",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "licenseType": "licenseFile",
  "targetEdition": "windows10EnterpriseN",
  "license": "License value",
  "productKey": "Product Key value"
}
```

### <a name="response"></a><span data-ttu-id="18b82-172">响应</span><span class="sxs-lookup"><span data-stu-id="18b82-172">Response</span></span>
<span data-ttu-id="18b82-p110">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="18b82-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 483

{
  "@odata.type": "#microsoft.graph.editionUpgradeConfiguration",
  "id": "f39fc471-c471-f39f-71c4-9ff371c49ff3",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "licenseType": "licenseFile",
  "targetEdition": "windows10EnterpriseN",
  "license": "License value",
  "productKey": "Product Key value"
}
```



