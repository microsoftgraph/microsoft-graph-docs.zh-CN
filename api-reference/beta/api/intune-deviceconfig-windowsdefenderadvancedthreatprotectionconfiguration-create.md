---
title: 创建 windowsDefenderAdvancedThreatProtectionConfiguration
description: 创建新的 windowsDefenderAdvancedThreatProtectionConfiguration 对象。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: ecbfe82a2a426022ef84182739004b9aecfbab4b
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/16/2019
ms.locfileid: "37532888"
---
# <a name="create-windowsdefenderadvancedthreatprotectionconfiguration"></a><span data-ttu-id="f277e-103">创建 windowsDefenderAdvancedThreatProtectionConfiguration</span><span class="sxs-lookup"><span data-stu-id="f277e-103">Create windowsDefenderAdvancedThreatProtectionConfiguration</span></span>

> <span data-ttu-id="f277e-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="f277e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f277e-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f277e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f277e-106">创建新的 [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="f277e-106">Create a new [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f277e-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="f277e-107">Prerequisites</span></span>
<span data-ttu-id="f277e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f277e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f277e-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="f277e-110">Permission type</span></span>|<span data-ttu-id="f277e-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="f277e-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f277e-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f277e-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f277e-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f277e-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f277e-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f277e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f277e-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="f277e-115">Not supported.</span></span>|
|<span data-ttu-id="f277e-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="f277e-116">Application</span></span>|<span data-ttu-id="f277e-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f277e-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f277e-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f277e-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="f277e-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="f277e-119">Request headers</span></span>
|<span data-ttu-id="f277e-120">标头</span><span class="sxs-lookup"><span data-stu-id="f277e-120">Header</span></span>|<span data-ttu-id="f277e-121">值</span><span class="sxs-lookup"><span data-stu-id="f277e-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f277e-122">授权</span><span class="sxs-lookup"><span data-stu-id="f277e-122">Authorization</span></span>|<span data-ttu-id="f277e-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="f277e-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f277e-124">接受</span><span class="sxs-lookup"><span data-stu-id="f277e-124">Accept</span></span>|<span data-ttu-id="f277e-125">application/json</span><span class="sxs-lookup"><span data-stu-id="f277e-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f277e-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="f277e-126">Request body</span></span>
<span data-ttu-id="f277e-127">在请求正文中，提供 windowsDefenderAdvancedThreatProtectionConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f277e-127">In the request body, supply a JSON representation for the windowsDefenderAdvancedThreatProtectionConfiguration object.</span></span>

<span data-ttu-id="f277e-128">下表显示创建 windowsDefenderAdvancedThreatProtectionConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="f277e-128">The following table shows the properties that are required when you create the windowsDefenderAdvancedThreatProtectionConfiguration.</span></span>

|<span data-ttu-id="f277e-129">属性</span><span class="sxs-lookup"><span data-stu-id="f277e-129">Property</span></span>|<span data-ttu-id="f277e-130">类型</span><span class="sxs-lookup"><span data-stu-id="f277e-130">Type</span></span>|<span data-ttu-id="f277e-131">说明</span><span class="sxs-lookup"><span data-stu-id="f277e-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f277e-132">id</span><span class="sxs-lookup"><span data-stu-id="f277e-132">id</span></span>|<span data-ttu-id="f277e-133">字符串</span><span class="sxs-lookup"><span data-stu-id="f277e-133">String</span></span>|<span data-ttu-id="f277e-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="f277e-134">Key of the entity.</span></span> <span data-ttu-id="f277e-135">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f277e-135">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f277e-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f277e-136">lastModifiedDateTime</span></span>|<span data-ttu-id="f277e-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f277e-137">DateTimeOffset</span></span>|<span data-ttu-id="f277e-138">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="f277e-138">DateTime the object was last modified.</span></span> <span data-ttu-id="f277e-139">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f277e-139">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f277e-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="f277e-140">roleScopeTagIds</span></span>|<span data-ttu-id="f277e-141">String 集合</span><span class="sxs-lookup"><span data-stu-id="f277e-141">String collection</span></span>|<span data-ttu-id="f277e-142">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="f277e-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="f277e-143">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f277e-143">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f277e-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="f277e-144">supportsScopeTags</span></span>|<span data-ttu-id="f277e-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="f277e-145">Boolean</span></span>|<span data-ttu-id="f277e-146">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="f277e-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="f277e-147">如果此值为 false，则不允许分配给 ScopeTags 属性，并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="f277e-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="f277e-148">这适用于在 Silverlight 中创建的旧版策略，可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="f277e-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="f277e-149">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="f277e-149">This property is read-only.</span></span> <span data-ttu-id="f277e-150">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f277e-150">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f277e-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="f277e-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="f277e-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="f277e-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="f277e-153">适用于此策略的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="f277e-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="f277e-154">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f277e-154">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f277e-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="f277e-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="f277e-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="f277e-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="f277e-157">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="f277e-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="f277e-158">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f277e-158">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f277e-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="f277e-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="f277e-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="f277e-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="f277e-161">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="f277e-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="f277e-162">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f277e-162">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f277e-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f277e-163">createdDateTime</span></span>|<span data-ttu-id="f277e-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f277e-164">DateTimeOffset</span></span>|<span data-ttu-id="f277e-165">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="f277e-165">DateTime the object was created.</span></span> <span data-ttu-id="f277e-166">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f277e-166">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f277e-167">说明</span><span class="sxs-lookup"><span data-stu-id="f277e-167">description</span></span>|<span data-ttu-id="f277e-168">String</span><span class="sxs-lookup"><span data-stu-id="f277e-168">String</span></span>|<span data-ttu-id="f277e-169">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="f277e-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="f277e-170">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f277e-170">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f277e-171">displayName</span><span class="sxs-lookup"><span data-stu-id="f277e-171">displayName</span></span>|<span data-ttu-id="f277e-172">String</span><span class="sxs-lookup"><span data-stu-id="f277e-172">String</span></span>|<span data-ttu-id="f277e-173">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="f277e-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="f277e-174">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f277e-174">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f277e-175">version</span><span class="sxs-lookup"><span data-stu-id="f277e-175">version</span></span>|<span data-ttu-id="f277e-176">Int32</span><span class="sxs-lookup"><span data-stu-id="f277e-176">Int32</span></span>|<span data-ttu-id="f277e-177">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="f277e-177">Version of the device configuration.</span></span> <span data-ttu-id="f277e-178">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f277e-178">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f277e-179">advancedThreatProtectionOnboardingBlob</span><span class="sxs-lookup"><span data-stu-id="f277e-179">advancedThreatProtectionOnboardingBlob</span></span>|<span data-ttu-id="f277e-180">字符串</span><span class="sxs-lookup"><span data-stu-id="f277e-180">String</span></span>|<span data-ttu-id="f277e-181">Windows Defender 高级威胁防护载入 Blob。</span><span class="sxs-lookup"><span data-stu-id="f277e-181">Windows Defender AdvancedThreatProtection Onboarding Blob.</span></span>|
|<span data-ttu-id="f277e-182">advancedThreatProtectionOnboardingFilename</span><span class="sxs-lookup"><span data-stu-id="f277e-182">advancedThreatProtectionOnboardingFilename</span></span>|<span data-ttu-id="f277e-183">字符串</span><span class="sxs-lookup"><span data-stu-id="f277e-183">String</span></span>|<span data-ttu-id="f277e-184">从中获取 AdvancedThreatProtectionOnboardingBlob 的文件的名称。</span><span class="sxs-lookup"><span data-stu-id="f277e-184">Name of the file from which AdvancedThreatProtectionOnboardingBlob was obtained.</span></span>|
|<span data-ttu-id="f277e-185">advancedThreatProtectionAutoPopulateOnboardingBlob</span><span class="sxs-lookup"><span data-stu-id="f277e-185">advancedThreatProtectionAutoPopulateOnboardingBlob</span></span>|<span data-ttu-id="f277e-186">Boolean</span><span class="sxs-lookup"><span data-stu-id="f277e-186">Boolean</span></span>|<span data-ttu-id="f277e-187">通过从高级威胁防护服务以编程方式自动填充载入 blob</span><span class="sxs-lookup"><span data-stu-id="f277e-187">Auto populate onboarding blob programmatically from Advanced Threat protection service</span></span>|
|<span data-ttu-id="f277e-188">allowSampleSharing</span><span class="sxs-lookup"><span data-stu-id="f277e-188">allowSampleSharing</span></span>|<span data-ttu-id="f277e-189">Boolean</span><span class="sxs-lookup"><span data-stu-id="f277e-189">Boolean</span></span>|<span data-ttu-id="f277e-190">Windows Defender 高级威胁防护“允许示例共享”规则</span><span class="sxs-lookup"><span data-stu-id="f277e-190">Windows Defender AdvancedThreatProtection "Allow Sample Sharing" Rule</span></span>|
|<span data-ttu-id="f277e-191">enableExpeditedTelemetryReporting</span><span class="sxs-lookup"><span data-stu-id="f277e-191">enableExpeditedTelemetryReporting</span></span>|<span data-ttu-id="f277e-192">Boolean</span><span class="sxs-lookup"><span data-stu-id="f277e-192">Boolean</span></span>|<span data-ttu-id="f277e-193">加速 Windows Defender 高级威胁防护遥测报告的频率。</span><span class="sxs-lookup"><span data-stu-id="f277e-193">Expedite Windows Defender Advanced Threat Protection telemetry reporting frequency.</span></span>|
|<span data-ttu-id="f277e-194">advancedThreatProtectionOffboardingBlob</span><span class="sxs-lookup"><span data-stu-id="f277e-194">advancedThreatProtectionOffboardingBlob</span></span>|<span data-ttu-id="f277e-195">字符串</span><span class="sxs-lookup"><span data-stu-id="f277e-195">String</span></span>|<span data-ttu-id="f277e-196">Windows Defender 高级威胁防护脱离 Blob。</span><span class="sxs-lookup"><span data-stu-id="f277e-196">Windows Defender AdvancedThreatProtection Offboarding Blob.</span></span>|
|<span data-ttu-id="f277e-197">advancedThreatProtectionOffboardingFilename</span><span class="sxs-lookup"><span data-stu-id="f277e-197">advancedThreatProtectionOffboardingFilename</span></span>|<span data-ttu-id="f277e-198">字符串</span><span class="sxs-lookup"><span data-stu-id="f277e-198">String</span></span>|<span data-ttu-id="f277e-199">从中获取 AdvancedThreatProtectionOffboardingBlob 的文件的名称。</span><span class="sxs-lookup"><span data-stu-id="f277e-199">Name of the file from which AdvancedThreatProtectionOffboardingBlob was obtained.</span></span>|



## <a name="response"></a><span data-ttu-id="f277e-200">响应</span><span class="sxs-lookup"><span data-stu-id="f277e-200">Response</span></span>
<span data-ttu-id="f277e-201">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="f277e-201">If successful, this method returns a `201 Created` response code and a [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f277e-202">示例</span><span class="sxs-lookup"><span data-stu-id="f277e-202">Example</span></span>

### <a name="request"></a><span data-ttu-id="f277e-203">请求</span><span class="sxs-lookup"><span data-stu-id="f277e-203">Request</span></span>
<span data-ttu-id="f277e-204">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="f277e-204">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
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

### <a name="response"></a><span data-ttu-id="f277e-205">响应</span><span class="sxs-lookup"><span data-stu-id="f277e-205">Response</span></span>
<span data-ttu-id="f277e-p113">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="f277e-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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






