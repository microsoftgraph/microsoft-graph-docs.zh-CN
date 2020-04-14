---
title: 创建 editionUpgradeConfiguration
description: 创建新的 editionUpgradeConfiguration 对象。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 73e2d29f6f045b666b13d2cf6ae8f1f3dd2634ab
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43433143"
---
# <a name="create-editionupgradeconfiguration"></a><span data-ttu-id="7bf87-103">创建 editionUpgradeConfiguration</span><span class="sxs-lookup"><span data-stu-id="7bf87-103">Create editionUpgradeConfiguration</span></span>

<span data-ttu-id="7bf87-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7bf87-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7bf87-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="7bf87-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7bf87-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="7bf87-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7bf87-107">创建新的 [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="7bf87-107">Create a new [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7bf87-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="7bf87-108">Prerequisites</span></span>
<span data-ttu-id="7bf87-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="7bf87-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7bf87-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="7bf87-111">Permission type</span></span>|<span data-ttu-id="7bf87-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="7bf87-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7bf87-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7bf87-113">Delegated (work or school account)</span></span>|<span data-ttu-id="7bf87-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7bf87-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="7bf87-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7bf87-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7bf87-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="7bf87-116">Not supported.</span></span>|
|<span data-ttu-id="7bf87-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="7bf87-117">Application</span></span>|<span data-ttu-id="7bf87-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7bf87-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="7bf87-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7bf87-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="7bf87-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="7bf87-120">Request headers</span></span>
|<span data-ttu-id="7bf87-121">标头</span><span class="sxs-lookup"><span data-stu-id="7bf87-121">Header</span></span>|<span data-ttu-id="7bf87-122">值</span><span class="sxs-lookup"><span data-stu-id="7bf87-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7bf87-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="7bf87-123">Authorization</span></span>|<span data-ttu-id="7bf87-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="7bf87-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7bf87-125">接受</span><span class="sxs-lookup"><span data-stu-id="7bf87-125">Accept</span></span>|<span data-ttu-id="7bf87-126">application/json</span><span class="sxs-lookup"><span data-stu-id="7bf87-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7bf87-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="7bf87-127">Request body</span></span>
<span data-ttu-id="7bf87-128">在请求正文中，提供 editionUpgradeConfiguration对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7bf87-128">In the request body, supply a JSON representation for the editionUpgradeConfiguration object.</span></span>

<span data-ttu-id="7bf87-129">下表显示创建 editionUpgradeConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="7bf87-129">The following table shows the properties that are required when you create the editionUpgradeConfiguration.</span></span>

|<span data-ttu-id="7bf87-130">属性</span><span class="sxs-lookup"><span data-stu-id="7bf87-130">Property</span></span>|<span data-ttu-id="7bf87-131">类型</span><span class="sxs-lookup"><span data-stu-id="7bf87-131">Type</span></span>|<span data-ttu-id="7bf87-132">说明</span><span class="sxs-lookup"><span data-stu-id="7bf87-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7bf87-133">id</span><span class="sxs-lookup"><span data-stu-id="7bf87-133">id</span></span>|<span data-ttu-id="7bf87-134">字符串</span><span class="sxs-lookup"><span data-stu-id="7bf87-134">String</span></span>|<span data-ttu-id="7bf87-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="7bf87-135">Key of the entity.</span></span> <span data-ttu-id="7bf87-136">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7bf87-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7bf87-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="7bf87-137">lastModifiedDateTime</span></span>|<span data-ttu-id="7bf87-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7bf87-138">DateTimeOffset</span></span>|<span data-ttu-id="7bf87-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="7bf87-139">DateTime the object was last modified.</span></span> <span data-ttu-id="7bf87-140">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7bf87-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7bf87-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="7bf87-141">roleScopeTagIds</span></span>|<span data-ttu-id="7bf87-142">String 集合</span><span class="sxs-lookup"><span data-stu-id="7bf87-142">String collection</span></span>|<span data-ttu-id="7bf87-143">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="7bf87-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="7bf87-144">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7bf87-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7bf87-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="7bf87-145">supportsScopeTags</span></span>|<span data-ttu-id="7bf87-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="7bf87-146">Boolean</span></span>|<span data-ttu-id="7bf87-147">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="7bf87-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="7bf87-148">如果此值为 false，则不允许分配给 ScopeTags 属性，并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="7bf87-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="7bf87-149">这适用于在 Silverlight 中创建的旧版策略，可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="7bf87-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="7bf87-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="7bf87-150">This property is read-only.</span></span> <span data-ttu-id="7bf87-151">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7bf87-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7bf87-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="7bf87-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="7bf87-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="7bf87-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="7bf87-154">适用于此策略的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="7bf87-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="7bf87-155">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7bf87-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7bf87-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="7bf87-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="7bf87-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="7bf87-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="7bf87-158">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="7bf87-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="7bf87-159">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7bf87-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7bf87-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="7bf87-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="7bf87-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="7bf87-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="7bf87-162">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="7bf87-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="7bf87-163">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7bf87-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7bf87-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="7bf87-164">createdDateTime</span></span>|<span data-ttu-id="7bf87-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7bf87-165">DateTimeOffset</span></span>|<span data-ttu-id="7bf87-166">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="7bf87-166">DateTime the object was created.</span></span> <span data-ttu-id="7bf87-167">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7bf87-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7bf87-168">description</span><span class="sxs-lookup"><span data-stu-id="7bf87-168">description</span></span>|<span data-ttu-id="7bf87-169">String</span><span class="sxs-lookup"><span data-stu-id="7bf87-169">String</span></span>|<span data-ttu-id="7bf87-170">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="7bf87-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="7bf87-171">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7bf87-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7bf87-172">displayName</span><span class="sxs-lookup"><span data-stu-id="7bf87-172">displayName</span></span>|<span data-ttu-id="7bf87-173">String</span><span class="sxs-lookup"><span data-stu-id="7bf87-173">String</span></span>|<span data-ttu-id="7bf87-174">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="7bf87-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="7bf87-175">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7bf87-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7bf87-176">version</span><span class="sxs-lookup"><span data-stu-id="7bf87-176">version</span></span>|<span data-ttu-id="7bf87-177">Int32</span><span class="sxs-lookup"><span data-stu-id="7bf87-177">Int32</span></span>|<span data-ttu-id="7bf87-178">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="7bf87-178">Version of the device configuration.</span></span> <span data-ttu-id="7bf87-179">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7bf87-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7bf87-180">licenseType</span><span class="sxs-lookup"><span data-stu-id="7bf87-180">licenseType</span></span>|[<span data-ttu-id="7bf87-181">editionUpgradeLicenseType</span><span class="sxs-lookup"><span data-stu-id="7bf87-181">editionUpgradeLicenseType</span></span>](../resources/intune-deviceconfig-editionupgradelicensetype.md)|<span data-ttu-id="7bf87-182">版本升级许可证类型。</span><span class="sxs-lookup"><span data-stu-id="7bf87-182">Edition Upgrade License Type.</span></span> <span data-ttu-id="7bf87-183">可取值为：`productKey`、`licenseFile`、`notConfigured`。</span><span class="sxs-lookup"><span data-stu-id="7bf87-183">Possible values are: `productKey`, `licenseFile`, `notConfigured`.</span></span>|
|<span data-ttu-id="7bf87-184">targetEdition</span><span class="sxs-lookup"><span data-stu-id="7bf87-184">targetEdition</span></span>|[<span data-ttu-id="7bf87-185">windows10EditionType</span><span class="sxs-lookup"><span data-stu-id="7bf87-185">windows10EditionType</span></span>](../resources/intune-deviceconfig-windows10editiontype.md)|<span data-ttu-id="7bf87-186">版本升级目标版本。</span><span class="sxs-lookup"><span data-stu-id="7bf87-186">Edition Upgrade Target Edition.</span></span> <span data-ttu-id="7bf87-187">可能的值为`windows10Enterprise`： `windows10EnterpriseN`、 `windows10Education`、 `windows10EducationN` `windows10MobileEnterprise` `windows10HolographicEnterprise` `windows10Professional` `windows10ProfessionalN` `windows10ProfessionalEducation` `windows10ProfessionalEducationN` `windows10ProfessionalWorkstation` `windows10IoTCoreCommercial`、、 `windows10ProfessionalWorkstationN`、、、、、、、、、、、、、、、。 `notConfigured` `windows10Home` `windows10HomeChina` `windows10HomeN` `windows10HomeSingleLanguage` `windows10Mobile` `windows10IoTCore`</span><span class="sxs-lookup"><span data-stu-id="7bf87-187">Possible values are: `windows10Enterprise`, `windows10EnterpriseN`, `windows10Education`, `windows10EducationN`, `windows10MobileEnterprise`, `windows10HolographicEnterprise`, `windows10Professional`, `windows10ProfessionalN`, `windows10ProfessionalEducation`, `windows10ProfessionalEducationN`, `windows10ProfessionalWorkstation`, `windows10ProfessionalWorkstationN`, `notConfigured`, `windows10Home`, `windows10HomeChina`, `windows10HomeN`, `windows10HomeSingleLanguage`, `windows10Mobile`, `windows10IoTCore`, `windows10IoTCoreCommercial`.</span></span>|
|<span data-ttu-id="7bf87-188">license</span><span class="sxs-lookup"><span data-stu-id="7bf87-188">license</span></span>|<span data-ttu-id="7bf87-189">String</span><span class="sxs-lookup"><span data-stu-id="7bf87-189">String</span></span>|<span data-ttu-id="7bf87-190">版本升级许可证文件内容。</span><span class="sxs-lookup"><span data-stu-id="7bf87-190">Edition Upgrade License File Content.</span></span>|
|<span data-ttu-id="7bf87-191">productKey</span><span class="sxs-lookup"><span data-stu-id="7bf87-191">productKey</span></span>|<span data-ttu-id="7bf87-192">String</span><span class="sxs-lookup"><span data-stu-id="7bf87-192">String</span></span>|<span data-ttu-id="7bf87-193">版本升级产品密钥。</span><span class="sxs-lookup"><span data-stu-id="7bf87-193">Edition Upgrade Product Key.</span></span>|
|<span data-ttu-id="7bf87-194">windowsSMode</span><span class="sxs-lookup"><span data-stu-id="7bf87-194">windowsSMode</span></span>|[<span data-ttu-id="7bf87-195">windowsSModeConfiguration</span><span class="sxs-lookup"><span data-stu-id="7bf87-195">windowsSModeConfiguration</span></span>](../resources/intune-deviceconfig-windowssmodeconfiguration.md)|<span data-ttu-id="7bf87-196">S 模式配置。</span><span class="sxs-lookup"><span data-stu-id="7bf87-196">S mode configuration.</span></span> <span data-ttu-id="7bf87-197">可取值为：`noRestriction`、`block`、`unlock`。</span><span class="sxs-lookup"><span data-stu-id="7bf87-197">Possible values are: `noRestriction`, `block`, `unlock`.</span></span>|



## <a name="response"></a><span data-ttu-id="7bf87-198">响应</span><span class="sxs-lookup"><span data-stu-id="7bf87-198">Response</span></span>
<span data-ttu-id="7bf87-199">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="7bf87-199">If successful, this method returns a `201 Created` response code and a [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7bf87-200">示例</span><span class="sxs-lookup"><span data-stu-id="7bf87-200">Example</span></span>

### <a name="request"></a><span data-ttu-id="7bf87-201">请求</span><span class="sxs-lookup"><span data-stu-id="7bf87-201">Request</span></span>
<span data-ttu-id="7bf87-202">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="7bf87-202">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="7bf87-203">响应</span><span class="sxs-lookup"><span data-stu-id="7bf87-203">Response</span></span>
<span data-ttu-id="7bf87-p116">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="7bf87-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



