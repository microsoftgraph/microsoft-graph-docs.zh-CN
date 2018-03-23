# <a name="create-editionupgradeconfiguration"></a><span data-ttu-id="b8ed3-101">创建 editionUpgradeConfiguration</span><span class="sxs-lookup"><span data-stu-id="b8ed3-101">Create editionUpgradeConfiguration</span></span>

> <span data-ttu-id="b8ed3-102">**注意：**使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="b8ed3-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b8ed3-103">创建新的 [editionUpgradeConfiguration](../resources/intune_deviceconfig_editionupgradeconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="b8ed3-103">Create a new [plannerBucket](../resources/intune_deviceconfig_editionupgradeconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="b8ed3-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="b8ed3-104">Prerequisites</span></span>
<span data-ttu-id="b8ed3-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="b8ed3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="b8ed3-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="b8ed3-107">Permission type</span></span>|<span data-ttu-id="b8ed3-108">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="b8ed3-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b8ed3-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b8ed3-109">Delegated (work or school account)</span></span>|<span data-ttu-id="b8ed3-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b8ed3-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b8ed3-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b8ed3-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b8ed3-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="b8ed3-112">Not supported.</span></span>|
|<span data-ttu-id="b8ed3-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="b8ed3-113">Application</span></span>|<span data-ttu-id="b8ed3-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="b8ed3-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b8ed3-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b8ed3-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="b8ed3-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="b8ed3-116">Request headers</span></span>
|<span data-ttu-id="b8ed3-117">标头</span><span class="sxs-lookup"><span data-stu-id="b8ed3-117">Header</span></span>|<span data-ttu-id="b8ed3-118">值</span><span class="sxs-lookup"><span data-stu-id="b8ed3-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b8ed3-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="b8ed3-119">Authorization</span></span>|<span data-ttu-id="b8ed3-120">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="b8ed3-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="b8ed3-121">Accept</span><span class="sxs-lookup"><span data-stu-id="b8ed3-121">Accept</span></span>|<span data-ttu-id="b8ed3-122">application/json</span><span class="sxs-lookup"><span data-stu-id="b8ed3-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b8ed3-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="b8ed3-123">Request body</span></span>
<span data-ttu-id="b8ed3-124">在请求正文中，提供 editionUpgradeConfiguration对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b8ed3-124">In the request body, supply a JSON representation of the schemaExtension object.</span></span>

<span data-ttu-id="b8ed3-125">下表显示创建 editionUpgradeConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="b8ed3-125">The following table shows the properties that are required when you create a user.</span></span>

|<span data-ttu-id="b8ed3-126">属性</span><span class="sxs-lookup"><span data-stu-id="b8ed3-126">Property</span></span>|<span data-ttu-id="b8ed3-127">类型</span><span class="sxs-lookup"><span data-stu-id="b8ed3-127">Type</span></span>|<span data-ttu-id="b8ed3-128">说明</span><span class="sxs-lookup"><span data-stu-id="b8ed3-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b8ed3-129">id</span><span class="sxs-lookup"><span data-stu-id="b8ed3-129">id</span></span>|<span data-ttu-id="b8ed3-130">String</span><span class="sxs-lookup"><span data-stu-id="b8ed3-130">String</span></span>|<span data-ttu-id="b8ed3-131">实体的键。</span><span class="sxs-lookup"><span data-stu-id="b8ed3-131">Key of the setting.</span></span> <span data-ttu-id="b8ed3-132">继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b8ed3-132">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b8ed3-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b8ed3-133">lastModifiedDateTime</span></span>|<span data-ttu-id="b8ed3-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b8ed3-134">DateTimeOffset</span></span>|<span data-ttu-id="b8ed3-135">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="b8ed3-135">Indicates the date the object was last modified.</span></span> <span data-ttu-id="b8ed3-136">继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b8ed3-136">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b8ed3-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b8ed3-137">createdDateTime</span></span>|<span data-ttu-id="b8ed3-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b8ed3-138">DateTimeOffset</span></span>|<span data-ttu-id="b8ed3-139">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="b8ed3-139">DateTime the object was created.</span></span> <span data-ttu-id="b8ed3-140">继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b8ed3-140">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b8ed3-141">description</span><span class="sxs-lookup"><span data-stu-id="b8ed3-141">description</span></span>|<span data-ttu-id="b8ed3-142">String</span><span class="sxs-lookup"><span data-stu-id="b8ed3-142">String</span></span>|<span data-ttu-id="b8ed3-143">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="b8ed3-143">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="b8ed3-144">继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b8ed3-144">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b8ed3-145">displayName</span><span class="sxs-lookup"><span data-stu-id="b8ed3-145">displayName</span></span>|<span data-ttu-id="b8ed3-146">String</span><span class="sxs-lookup"><span data-stu-id="b8ed3-146">String</span></span>|<span data-ttu-id="b8ed3-147">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="b8ed3-147">Admin provided name of the device configuration.</span></span> <span data-ttu-id="b8ed3-148">继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b8ed3-148">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b8ed3-149">version</span><span class="sxs-lookup"><span data-stu-id="b8ed3-149">version</span></span>|<span data-ttu-id="b8ed3-150">Int32</span><span class="sxs-lookup"><span data-stu-id="b8ed3-150">Int32</span></span>|<span data-ttu-id="b8ed3-151">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="b8ed3-151">Version of the device configuration.</span></span> <span data-ttu-id="b8ed3-152">继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b8ed3-152">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b8ed3-153">licenseType</span><span class="sxs-lookup"><span data-stu-id="b8ed3-153">licenseType</span></span>|<span data-ttu-id="b8ed3-154">String</span><span class="sxs-lookup"><span data-stu-id="b8ed3-154">String</span></span>|<span data-ttu-id="b8ed3-155">版本升级许可证类型。</span><span class="sxs-lookup"><span data-stu-id="b8ed3-155">Edition Upgrade License Type.</span></span> <span data-ttu-id="b8ed3-156">可取值为：`productKey`、`licenseFile`。</span><span class="sxs-lookup"><span data-stu-id="b8ed3-156">Possible values are: `productKey`, `licenseFile`.</span></span>|
|<span data-ttu-id="b8ed3-157">targetEdition</span><span class="sxs-lookup"><span data-stu-id="b8ed3-157">targetEdition</span></span>|<span data-ttu-id="b8ed3-158">String</span><span class="sxs-lookup"><span data-stu-id="b8ed3-158">String</span></span>|<span data-ttu-id="b8ed3-159">版本升级目标版本。</span><span class="sxs-lookup"><span data-stu-id="b8ed3-159">Edition Upgrade Target Edition.</span></span> <span data-ttu-id="b8ed3-160">可取值为：`windows10Enterprise`、`windows10EnterpriseN`、`windows10Education`、`windows10EducationN`、`windows10MobileEnterprise`、`windows10HolographicEnterprise`、`windows10Professional`、`windows10ProfessionalN`、`windows10ProfessionalEducation`、`windows10ProfessionalEducationN`、`windows10ProfessionalWorkstation`、`windows10ProfessionalWorkstationN`。</span><span class="sxs-lookup"><span data-stu-id="b8ed3-160">Possible values are: `windows10Enterprise`, `windows10EnterpriseN`, `windows10Education`, `windows10EducationN`, `windows10MobileEnterprise`, `windows10HolographicEnterprise`, `windows10Professional`, `windows10ProfessionalN`, `windows10ProfessionalEducation`, `windows10ProfessionalEducationN`, `windows10ProfessionalWorkstation`, `windows10ProfessionalWorkstationN`.</span></span>|
|<span data-ttu-id="b8ed3-161">license</span><span class="sxs-lookup"><span data-stu-id="b8ed3-161">License</span></span>|<span data-ttu-id="b8ed3-162">String</span><span class="sxs-lookup"><span data-stu-id="b8ed3-162">String</span></span>|<span data-ttu-id="b8ed3-163">版本升级许可证文件内容。</span><span class="sxs-lookup"><span data-stu-id="b8ed3-163">Edition Upgrade License File Content.</span></span>|
|<span data-ttu-id="b8ed3-164">productKey</span><span class="sxs-lookup"><span data-stu-id="b8ed3-164">productKey</span></span>|<span data-ttu-id="b8ed3-165">String</span><span class="sxs-lookup"><span data-stu-id="b8ed3-165">String</span></span>|<span data-ttu-id="b8ed3-166">版本升级产品密钥。</span><span class="sxs-lookup"><span data-stu-id="b8ed3-166">Edition Upgrade Product Key.</span></span>|



## <a name="response"></a><span data-ttu-id="b8ed3-167">响应</span><span class="sxs-lookup"><span data-stu-id="b8ed3-167">Response</span></span>
<span data-ttu-id="b8ed3-168">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [editionUpgradeConfiguration](../resources/intune_deviceconfig_editionupgradeconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="b8ed3-168">If successful, this method returns a `201 Created` response code and a [directoryObject](../resources/intune_deviceconfig_editionupgradeconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b8ed3-169">示例</span><span class="sxs-lookup"><span data-stu-id="b8ed3-169">Example</span></span>
### <a name="request"></a><span data-ttu-id="b8ed3-170">请求</span><span class="sxs-lookup"><span data-stu-id="b8ed3-170">Request</span></span>
<span data-ttu-id="b8ed3-171">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="b8ed3-171">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 375

{
  "@odata.type": "#microsoft.graph.editionUpgradeConfiguration",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "licenseType": "licenseFile",
  "targetEdition": "windows10EnterpriseN",
  "license": "License value",
  "productKey": "Product Key value"
}
```

### <a name="response"></a><span data-ttu-id="b8ed3-172">响应</span><span class="sxs-lookup"><span data-stu-id="b8ed3-172">Response</span></span>
<span data-ttu-id="b8ed3-p110">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="b8ed3-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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



