---
title: 创建 editionUpgradeConfiguration
description: 创建新的 editionUpgradeConfiguration 对象。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: a45feaefd9a8540f8ed29b280d7ce234f9ccf0b0
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/26/2019
ms.locfileid: "37168059"
---
# <a name="create-editionupgradeconfiguration"></a><span data-ttu-id="901c8-103">创建 editionUpgradeConfiguration</span><span class="sxs-lookup"><span data-stu-id="901c8-103">Create editionUpgradeConfiguration</span></span>

> <span data-ttu-id="901c8-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="901c8-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="901c8-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="901c8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="901c8-106">创建新的 [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="901c8-106">Create a new [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="901c8-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="901c8-107">Prerequisites</span></span>
<span data-ttu-id="901c8-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="901c8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="901c8-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="901c8-110">Permission type</span></span>|<span data-ttu-id="901c8-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="901c8-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="901c8-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="901c8-112">Delegated (work or school account)</span></span>|<span data-ttu-id="901c8-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="901c8-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="901c8-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="901c8-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="901c8-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="901c8-115">Not supported.</span></span>|
|<span data-ttu-id="901c8-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="901c8-116">Application</span></span>|<span data-ttu-id="901c8-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="901c8-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="901c8-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="901c8-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="901c8-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="901c8-119">Request headers</span></span>
|<span data-ttu-id="901c8-120">标头</span><span class="sxs-lookup"><span data-stu-id="901c8-120">Header</span></span>|<span data-ttu-id="901c8-121">值</span><span class="sxs-lookup"><span data-stu-id="901c8-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="901c8-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="901c8-122">Authorization</span></span>|<span data-ttu-id="901c8-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="901c8-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="901c8-124">接受</span><span class="sxs-lookup"><span data-stu-id="901c8-124">Accept</span></span>|<span data-ttu-id="901c8-125">application/json</span><span class="sxs-lookup"><span data-stu-id="901c8-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="901c8-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="901c8-126">Request body</span></span>
<span data-ttu-id="901c8-127">在请求正文中，提供 editionUpgradeConfiguration对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="901c8-127">In the request body, supply a JSON representation for the editionUpgradeConfiguration object.</span></span>

<span data-ttu-id="901c8-128">下表显示创建 editionUpgradeConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="901c8-128">The following table shows the properties that are required when you create the editionUpgradeConfiguration.</span></span>

|<span data-ttu-id="901c8-129">属性</span><span class="sxs-lookup"><span data-stu-id="901c8-129">Property</span></span>|<span data-ttu-id="901c8-130">类型</span><span class="sxs-lookup"><span data-stu-id="901c8-130">Type</span></span>|<span data-ttu-id="901c8-131">说明</span><span class="sxs-lookup"><span data-stu-id="901c8-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="901c8-132">id</span><span class="sxs-lookup"><span data-stu-id="901c8-132">id</span></span>|<span data-ttu-id="901c8-133">字符串</span><span class="sxs-lookup"><span data-stu-id="901c8-133">String</span></span>|<span data-ttu-id="901c8-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="901c8-134">Key of the entity.</span></span> <span data-ttu-id="901c8-135">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="901c8-135">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="901c8-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="901c8-136">lastModifiedDateTime</span></span>|<span data-ttu-id="901c8-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="901c8-137">DateTimeOffset</span></span>|<span data-ttu-id="901c8-138">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="901c8-138">DateTime the object was last modified.</span></span> <span data-ttu-id="901c8-139">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="901c8-139">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="901c8-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="901c8-140">roleScopeTagIds</span></span>|<span data-ttu-id="901c8-141">String collection</span><span class="sxs-lookup"><span data-stu-id="901c8-141">String collection</span></span>|<span data-ttu-id="901c8-142">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="901c8-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="901c8-143">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="901c8-143">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="901c8-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="901c8-144">supportsScopeTags</span></span>|<span data-ttu-id="901c8-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="901c8-145">Boolean</span></span>|<span data-ttu-id="901c8-146">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="901c8-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="901c8-147">如果此值为 false，则不允许分配给 ScopeTags 属性，并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="901c8-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="901c8-148">这适用于在 Silverlight 中创建的旧版策略，可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="901c8-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="901c8-149">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="901c8-149">This property is read-only.</span></span> <span data-ttu-id="901c8-150">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="901c8-150">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="901c8-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="901c8-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="901c8-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="901c8-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="901c8-153">适用于此策略的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="901c8-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="901c8-154">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="901c8-154">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="901c8-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="901c8-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="901c8-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="901c8-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="901c8-157">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="901c8-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="901c8-158">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="901c8-158">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="901c8-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="901c8-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="901c8-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="901c8-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="901c8-161">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="901c8-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="901c8-162">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="901c8-162">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="901c8-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="901c8-163">createdDateTime</span></span>|<span data-ttu-id="901c8-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="901c8-164">DateTimeOffset</span></span>|<span data-ttu-id="901c8-165">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="901c8-165">DateTime the object was created.</span></span> <span data-ttu-id="901c8-166">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="901c8-166">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="901c8-167">说明</span><span class="sxs-lookup"><span data-stu-id="901c8-167">description</span></span>|<span data-ttu-id="901c8-168">String</span><span class="sxs-lookup"><span data-stu-id="901c8-168">String</span></span>|<span data-ttu-id="901c8-169">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="901c8-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="901c8-170">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="901c8-170">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="901c8-171">displayName</span><span class="sxs-lookup"><span data-stu-id="901c8-171">displayName</span></span>|<span data-ttu-id="901c8-172">String</span><span class="sxs-lookup"><span data-stu-id="901c8-172">String</span></span>|<span data-ttu-id="901c8-173">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="901c8-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="901c8-174">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="901c8-174">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="901c8-175">version</span><span class="sxs-lookup"><span data-stu-id="901c8-175">version</span></span>|<span data-ttu-id="901c8-176">Int32</span><span class="sxs-lookup"><span data-stu-id="901c8-176">Int32</span></span>|<span data-ttu-id="901c8-177">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="901c8-177">Version of the device configuration.</span></span> <span data-ttu-id="901c8-178">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="901c8-178">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="901c8-179">licenseType</span><span class="sxs-lookup"><span data-stu-id="901c8-179">licenseType</span></span>|[<span data-ttu-id="901c8-180">editionUpgradeLicenseType</span><span class="sxs-lookup"><span data-stu-id="901c8-180">editionUpgradeLicenseType</span></span>](../resources/intune-deviceconfig-editionupgradelicensetype.md)|<span data-ttu-id="901c8-181">版本升级许可证类型。</span><span class="sxs-lookup"><span data-stu-id="901c8-181">Edition Upgrade License Type.</span></span> <span data-ttu-id="901c8-182">可取值为：`productKey`、`licenseFile`、`notConfigured`。</span><span class="sxs-lookup"><span data-stu-id="901c8-182">Possible values are: `productKey`, `licenseFile`, `notConfigured`.</span></span>|
|<span data-ttu-id="901c8-183">targetEdition</span><span class="sxs-lookup"><span data-stu-id="901c8-183">targetEdition</span></span>|[<span data-ttu-id="901c8-184">windows10EditionType</span><span class="sxs-lookup"><span data-stu-id="901c8-184">windows10EditionType</span></span>](../resources/intune-deviceconfig-windows10editiontype.md)|<span data-ttu-id="901c8-185">版本升级目标版本。</span><span class="sxs-lookup"><span data-stu-id="901c8-185">Edition Upgrade Target Edition.</span></span> <span data-ttu-id="901c8-186">可能的值为`windows10Enterprise`： `windows10EnterpriseN`、 `windows10Education`、 `windows10EducationN` `windows10MobileEnterprise` `windows10HolographicEnterprise` `windows10Professional` `windows10ProfessionalN` `windows10ProfessionalEducation` `windows10ProfessionalEducationN` `windows10ProfessionalWorkstation` `windows10ProfessionalWorkstationN` `notConfigured`、、、、、、、、、、、、、、、、 `windows10Home` `windows10HomeChina` `windows10HomeN` `windows10HomeSingleLanguage` `windows10Mobile` `windows10IoTCore`, `windows10IoTCoreCommercial`.</span><span class="sxs-lookup"><span data-stu-id="901c8-186">Possible values are: `windows10Enterprise`, `windows10EnterpriseN`, `windows10Education`, `windows10EducationN`, `windows10MobileEnterprise`, `windows10HolographicEnterprise`, `windows10Professional`, `windows10ProfessionalN`, `windows10ProfessionalEducation`, `windows10ProfessionalEducationN`, `windows10ProfessionalWorkstation`, `windows10ProfessionalWorkstationN`, `notConfigured`, `windows10Home`, `windows10HomeChina`, `windows10HomeN`, `windows10HomeSingleLanguage`, `windows10Mobile`, `windows10IoTCore`, `windows10IoTCoreCommercial`.</span></span>|
|<span data-ttu-id="901c8-187">license</span><span class="sxs-lookup"><span data-stu-id="901c8-187">license</span></span>|<span data-ttu-id="901c8-188">String</span><span class="sxs-lookup"><span data-stu-id="901c8-188">String</span></span>|<span data-ttu-id="901c8-189">版本升级许可证文件内容。</span><span class="sxs-lookup"><span data-stu-id="901c8-189">Edition Upgrade License File Content.</span></span>|
|<span data-ttu-id="901c8-190">productKey</span><span class="sxs-lookup"><span data-stu-id="901c8-190">productKey</span></span>|<span data-ttu-id="901c8-191">String</span><span class="sxs-lookup"><span data-stu-id="901c8-191">String</span></span>|<span data-ttu-id="901c8-192">版本升级产品密钥。</span><span class="sxs-lookup"><span data-stu-id="901c8-192">Edition Upgrade Product Key.</span></span>|
|<span data-ttu-id="901c8-193">windowsSMode</span><span class="sxs-lookup"><span data-stu-id="901c8-193">windowsSMode</span></span>|[<span data-ttu-id="901c8-194">windowsSModeConfiguration</span><span class="sxs-lookup"><span data-stu-id="901c8-194">windowsSModeConfiguration</span></span>](../resources/intune-deviceconfig-windowssmodeconfiguration.md)|<span data-ttu-id="901c8-195">S 模式配置。</span><span class="sxs-lookup"><span data-stu-id="901c8-195">S mode configuration.</span></span> <span data-ttu-id="901c8-196">可取值为：`noRestriction`、`block`、`unlock`。</span><span class="sxs-lookup"><span data-stu-id="901c8-196">Possible values are: `noRestriction`, `block`, `unlock`.</span></span>|



## <a name="response"></a><span data-ttu-id="901c8-197">响应</span><span class="sxs-lookup"><span data-stu-id="901c8-197">Response</span></span>
<span data-ttu-id="901c8-198">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="901c8-198">If successful, this method returns a `201 Created` response code and a [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="901c8-199">示例</span><span class="sxs-lookup"><span data-stu-id="901c8-199">Example</span></span>

### <a name="request"></a><span data-ttu-id="901c8-200">请求</span><span class="sxs-lookup"><span data-stu-id="901c8-200">Request</span></span>
<span data-ttu-id="901c8-201">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="901c8-201">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1204

{
  "@odata.type": "#microsoft.graph.editionUpgradeConfiguration",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "deviceManagementApplicabilityRuleOsEdition": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsEdition",
    "osEditionTypes": [
      "windows10EnterpriseN"
    ],
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleOsVersion": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsVersion",
    "minOSVersion": "Min OSVersion value",
    "maxOSVersion": "Max OSVersion value",
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleDeviceMode": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleDeviceMode",
    "deviceMode": "sModeConfiguration",
    "name": "Name value",
    "ruleType": "exclude"
  },
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "licenseType": "licenseFile",
  "targetEdition": "windows10EnterpriseN",
  "license": "License value",
  "productKey": "Product Key value",
  "windowsSMode": "block"
}
```

### <a name="response"></a><span data-ttu-id="901c8-202">响应</span><span class="sxs-lookup"><span data-stu-id="901c8-202">Response</span></span>
<span data-ttu-id="901c8-p116">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="901c8-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1376

{
  "@odata.type": "#microsoft.graph.editionUpgradeConfiguration",
  "id": "f39fc471-c471-f39f-71c4-9ff371c49ff3",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "deviceManagementApplicabilityRuleOsEdition": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsEdition",
    "osEditionTypes": [
      "windows10EnterpriseN"
    ],
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleOsVersion": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsVersion",
    "minOSVersion": "Min OSVersion value",
    "maxOSVersion": "Max OSVersion value",
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleDeviceMode": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleDeviceMode",
    "deviceMode": "sModeConfiguration",
    "name": "Name value",
    "ruleType": "exclude"
  },
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "licenseType": "licenseFile",
  "targetEdition": "windows10EnterpriseN",
  "license": "License value",
  "productKey": "Product Key value",
  "windowsSMode": "block"
}
```




