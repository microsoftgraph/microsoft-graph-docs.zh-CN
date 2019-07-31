---
title: 更新 windowsDefenderAdvancedThreatProtectionConfiguration
description: 更新 windowsDefenderAdvancedThreatProtectionConfiguration 对象的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 14c5486e20e8c97414e904c91c78b4b04ea42216
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35982296"
---
# <a name="update-windowsdefenderadvancedthreatprotectionconfiguration"></a><span data-ttu-id="590f5-103">更新 windowsDefenderAdvancedThreatProtectionConfiguration</span><span class="sxs-lookup"><span data-stu-id="590f5-103">Update windowsDefenderAdvancedThreatProtectionConfiguration</span></span>

> <span data-ttu-id="590f5-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="590f5-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="590f5-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="590f5-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="590f5-106">更新 [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="590f5-106">Update the properties of a [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="590f5-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="590f5-107">Prerequisites</span></span>
<span data-ttu-id="590f5-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="590f5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="590f5-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="590f5-110">Permission type</span></span>|<span data-ttu-id="590f5-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="590f5-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="590f5-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="590f5-112">Delegated (work or school account)</span></span>|<span data-ttu-id="590f5-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="590f5-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="590f5-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="590f5-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="590f5-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="590f5-115">Not supported.</span></span>|
|<span data-ttu-id="590f5-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="590f5-116">Application</span></span>|<span data-ttu-id="590f5-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="590f5-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="590f5-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="590f5-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="590f5-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="590f5-119">Request headers</span></span>
|<span data-ttu-id="590f5-120">标头</span><span class="sxs-lookup"><span data-stu-id="590f5-120">Header</span></span>|<span data-ttu-id="590f5-121">值</span><span class="sxs-lookup"><span data-stu-id="590f5-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="590f5-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="590f5-122">Authorization</span></span>|<span data-ttu-id="590f5-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="590f5-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="590f5-124">接受</span><span class="sxs-lookup"><span data-stu-id="590f5-124">Accept</span></span>|<span data-ttu-id="590f5-125">application/json</span><span class="sxs-lookup"><span data-stu-id="590f5-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="590f5-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="590f5-126">Request body</span></span>
<span data-ttu-id="590f5-127">在请求正文中，提供 [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="590f5-127">In the request body, supply a JSON representation for the [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md) object.</span></span>

<span data-ttu-id="590f5-128">下表显示创建 [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="590f5-128">The following table shows the properties that are required when you create the [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md).</span></span>

|<span data-ttu-id="590f5-129">属性</span><span class="sxs-lookup"><span data-stu-id="590f5-129">Property</span></span>|<span data-ttu-id="590f5-130">类型</span><span class="sxs-lookup"><span data-stu-id="590f5-130">Type</span></span>|<span data-ttu-id="590f5-131">说明</span><span class="sxs-lookup"><span data-stu-id="590f5-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="590f5-132">id</span><span class="sxs-lookup"><span data-stu-id="590f5-132">id</span></span>|<span data-ttu-id="590f5-133">字符串</span><span class="sxs-lookup"><span data-stu-id="590f5-133">String</span></span>|<span data-ttu-id="590f5-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="590f5-134">Key of the entity.</span></span> <span data-ttu-id="590f5-135">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="590f5-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="590f5-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="590f5-136">lastModifiedDateTime</span></span>|<span data-ttu-id="590f5-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="590f5-137">DateTimeOffset</span></span>|<span data-ttu-id="590f5-138">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="590f5-138">DateTime the object was last modified.</span></span> <span data-ttu-id="590f5-139">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="590f5-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="590f5-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="590f5-140">roleScopeTagIds</span></span>|<span data-ttu-id="590f5-141">String collection</span><span class="sxs-lookup"><span data-stu-id="590f5-141">String collection</span></span>|<span data-ttu-id="590f5-142">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="590f5-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="590f5-143">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="590f5-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="590f5-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="590f5-144">supportsScopeTags</span></span>|<span data-ttu-id="590f5-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="590f5-145">Boolean</span></span>|<span data-ttu-id="590f5-146">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="590f5-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="590f5-147">如果此值为 false, 则不允许分配给 ScopeTags 属性, 并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="590f5-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="590f5-148">这适用于在 Silverlight 中创建的旧版策略, 可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="590f5-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="590f5-149">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="590f5-149">This property is read-only.</span></span> <span data-ttu-id="590f5-150">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="590f5-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="590f5-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="590f5-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="590f5-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="590f5-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="590f5-153">适用于此策略的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="590f5-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="590f5-154">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="590f5-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="590f5-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="590f5-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="590f5-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="590f5-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="590f5-157">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="590f5-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="590f5-158">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="590f5-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="590f5-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="590f5-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="590f5-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="590f5-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="590f5-161">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="590f5-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="590f5-162">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="590f5-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="590f5-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="590f5-163">createdDateTime</span></span>|<span data-ttu-id="590f5-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="590f5-164">DateTimeOffset</span></span>|<span data-ttu-id="590f5-165">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="590f5-165">DateTime the object was created.</span></span> <span data-ttu-id="590f5-166">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="590f5-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="590f5-167">说明</span><span class="sxs-lookup"><span data-stu-id="590f5-167">description</span></span>|<span data-ttu-id="590f5-168">String</span><span class="sxs-lookup"><span data-stu-id="590f5-168">String</span></span>|<span data-ttu-id="590f5-169">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="590f5-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="590f5-170">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="590f5-170">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="590f5-171">displayName</span><span class="sxs-lookup"><span data-stu-id="590f5-171">displayName</span></span>|<span data-ttu-id="590f5-172">String</span><span class="sxs-lookup"><span data-stu-id="590f5-172">String</span></span>|<span data-ttu-id="590f5-173">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="590f5-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="590f5-174">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="590f5-174">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="590f5-175">version</span><span class="sxs-lookup"><span data-stu-id="590f5-175">version</span></span>|<span data-ttu-id="590f5-176">Int32</span><span class="sxs-lookup"><span data-stu-id="590f5-176">Int32</span></span>|<span data-ttu-id="590f5-177">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="590f5-177">Version of the device configuration.</span></span> <span data-ttu-id="590f5-178">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="590f5-178">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="590f5-179">advancedThreatProtectionOnboardingBlob</span><span class="sxs-lookup"><span data-stu-id="590f5-179">advancedThreatProtectionOnboardingBlob</span></span>|<span data-ttu-id="590f5-180">String</span><span class="sxs-lookup"><span data-stu-id="590f5-180">String</span></span>|<span data-ttu-id="590f5-181">Windows Defender 高级威胁防护载入 Blob。</span><span class="sxs-lookup"><span data-stu-id="590f5-181">Windows Defender AdvancedThreatProtection Onboarding Blob.</span></span>|
|<span data-ttu-id="590f5-182">advancedThreatProtectionOnboardingFilename</span><span class="sxs-lookup"><span data-stu-id="590f5-182">advancedThreatProtectionOnboardingFilename</span></span>|<span data-ttu-id="590f5-183">String</span><span class="sxs-lookup"><span data-stu-id="590f5-183">String</span></span>|<span data-ttu-id="590f5-184">从中获取 AdvancedThreatProtectionOnboardingBlob 的文件的名称。</span><span class="sxs-lookup"><span data-stu-id="590f5-184">Name of the file from which AdvancedThreatProtectionOnboardingBlob was obtained.</span></span>|
|<span data-ttu-id="590f5-185">advancedThreatProtectionAutoPopulateOnboardingBlob</span><span class="sxs-lookup"><span data-stu-id="590f5-185">advancedThreatProtectionAutoPopulateOnboardingBlob</span></span>|<span data-ttu-id="590f5-186">Boolean</span><span class="sxs-lookup"><span data-stu-id="590f5-186">Boolean</span></span>|<span data-ttu-id="590f5-187">通过从高级威胁防护服务以编程方式自动填充载入 blob</span><span class="sxs-lookup"><span data-stu-id="590f5-187">Auto populate onboarding blob programmatically from Advanced Threat protection service</span></span>|
|<span data-ttu-id="590f5-188">allowSampleSharing</span><span class="sxs-lookup"><span data-stu-id="590f5-188">allowSampleSharing</span></span>|<span data-ttu-id="590f5-189">Boolean</span><span class="sxs-lookup"><span data-stu-id="590f5-189">Boolean</span></span>|<span data-ttu-id="590f5-190">Windows Defender 高级威胁防护“允许示例共享”规则</span><span class="sxs-lookup"><span data-stu-id="590f5-190">Windows Defender AdvancedThreatProtection "Allow Sample Sharing" Rule</span></span>|
|<span data-ttu-id="590f5-191">enableExpeditedTelemetryReporting</span><span class="sxs-lookup"><span data-stu-id="590f5-191">enableExpeditedTelemetryReporting</span></span>|<span data-ttu-id="590f5-192">Boolean</span><span class="sxs-lookup"><span data-stu-id="590f5-192">Boolean</span></span>|<span data-ttu-id="590f5-193">加速 Windows Defender 高级威胁防护遥测报告的频率。</span><span class="sxs-lookup"><span data-stu-id="590f5-193">Expedite Windows Defender Advanced Threat Protection telemetry reporting frequency.</span></span>|
|<span data-ttu-id="590f5-194">advancedThreatProtectionOffboardingBlob</span><span class="sxs-lookup"><span data-stu-id="590f5-194">advancedThreatProtectionOffboardingBlob</span></span>|<span data-ttu-id="590f5-195">String</span><span class="sxs-lookup"><span data-stu-id="590f5-195">String</span></span>|<span data-ttu-id="590f5-196">Windows Defender 高级威胁防护脱离 Blob。</span><span class="sxs-lookup"><span data-stu-id="590f5-196">Windows Defender AdvancedThreatProtection Offboarding Blob.</span></span>|
|<span data-ttu-id="590f5-197">advancedThreatProtectionOffboardingFilename</span><span class="sxs-lookup"><span data-stu-id="590f5-197">advancedThreatProtectionOffboardingFilename</span></span>|<span data-ttu-id="590f5-198">String</span><span class="sxs-lookup"><span data-stu-id="590f5-198">String</span></span>|<span data-ttu-id="590f5-199">从中获取 AdvancedThreatProtectionOffboardingBlob 的文件的名称。</span><span class="sxs-lookup"><span data-stu-id="590f5-199">Name of the file from which AdvancedThreatProtectionOffboardingBlob was obtained.</span></span>|



## <a name="response"></a><span data-ttu-id="590f5-200">响应</span><span class="sxs-lookup"><span data-stu-id="590f5-200">Response</span></span>
<span data-ttu-id="590f5-201">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="590f5-201">If successful, this method returns a `200 OK` response code and an updated [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="590f5-202">示例</span><span class="sxs-lookup"><span data-stu-id="590f5-202">Example</span></span>

### <a name="request"></a><span data-ttu-id="590f5-203">请求</span><span class="sxs-lookup"><span data-stu-id="590f5-203">Request</span></span>
<span data-ttu-id="590f5-204">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="590f5-204">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1603

{
  "@odata.type": "#microsoft.graph.windowsDefenderAdvancedThreatProtectionConfiguration",
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
  "advancedThreatProtectionOnboardingBlob": "Advanced Threat Protection Onboarding Blob value",
  "advancedThreatProtectionOnboardingFilename": "Advanced Threat Protection Onboarding Filename value",
  "advancedThreatProtectionAutoPopulateOnboardingBlob": true,
  "allowSampleSharing": true,
  "enableExpeditedTelemetryReporting": true,
  "advancedThreatProtectionOffboardingBlob": "Advanced Threat Protection Offboarding Blob value",
  "advancedThreatProtectionOffboardingFilename": "Advanced Threat Protection Offboarding Filename value"
}
```

### <a name="response"></a><span data-ttu-id="590f5-205">响应</span><span class="sxs-lookup"><span data-stu-id="590f5-205">Response</span></span>
<span data-ttu-id="590f5-p113">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="590f5-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1775

{
  "@odata.type": "#microsoft.graph.windowsDefenderAdvancedThreatProtectionConfiguration",
  "id": "294373aa-73aa-2943-aa73-4329aa734329",
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
  "advancedThreatProtectionOnboardingBlob": "Advanced Threat Protection Onboarding Blob value",
  "advancedThreatProtectionOnboardingFilename": "Advanced Threat Protection Onboarding Filename value",
  "advancedThreatProtectionAutoPopulateOnboardingBlob": true,
  "allowSampleSharing": true,
  "enableExpeditedTelemetryReporting": true,
  "advancedThreatProtectionOffboardingBlob": "Advanced Threat Protection Offboarding Blob value",
  "advancedThreatProtectionOffboardingFilename": "Advanced Threat Protection Offboarding Filename value"
}
```





