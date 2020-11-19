---
title: 更新 windowsDefenderAdvancedThreatProtectionConfiguration
description: 更新 windowsDefenderAdvancedThreatProtectionConfiguration 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: a36533ea1a0062ef1bdd9d4faa769a0864e01945
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49230035"
---
# <a name="update-windowsdefenderadvancedthreatprotectionconfiguration"></a><span data-ttu-id="5159e-103">更新 windowsDefenderAdvancedThreatProtectionConfiguration</span><span class="sxs-lookup"><span data-stu-id="5159e-103">Update windowsDefenderAdvancedThreatProtectionConfiguration</span></span>

<span data-ttu-id="5159e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5159e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5159e-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="5159e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5159e-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="5159e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5159e-107">更新 [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="5159e-107">Update the properties of a [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5159e-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="5159e-108">Prerequisites</span></span>
<span data-ttu-id="5159e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="5159e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5159e-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="5159e-111">Permission type</span></span>|<span data-ttu-id="5159e-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="5159e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5159e-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5159e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="5159e-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5159e-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="5159e-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5159e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5159e-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="5159e-116">Not supported.</span></span>|
|<span data-ttu-id="5159e-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="5159e-117">Application</span></span>|<span data-ttu-id="5159e-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5159e-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="5159e-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5159e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="5159e-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="5159e-120">Request headers</span></span>
|<span data-ttu-id="5159e-121">标头</span><span class="sxs-lookup"><span data-stu-id="5159e-121">Header</span></span>|<span data-ttu-id="5159e-122">值</span><span class="sxs-lookup"><span data-stu-id="5159e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5159e-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="5159e-123">Authorization</span></span>|<span data-ttu-id="5159e-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="5159e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5159e-125">接受</span><span class="sxs-lookup"><span data-stu-id="5159e-125">Accept</span></span>|<span data-ttu-id="5159e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="5159e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5159e-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="5159e-127">Request body</span></span>
<span data-ttu-id="5159e-128">在请求正文中，提供 [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5159e-128">In the request body, supply a JSON representation for the [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md) object.</span></span>

<span data-ttu-id="5159e-129">下表显示创建 [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="5159e-129">The following table shows the properties that are required when you create the [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md).</span></span>

|<span data-ttu-id="5159e-130">属性</span><span class="sxs-lookup"><span data-stu-id="5159e-130">Property</span></span>|<span data-ttu-id="5159e-131">类型</span><span class="sxs-lookup"><span data-stu-id="5159e-131">Type</span></span>|<span data-ttu-id="5159e-132">说明</span><span class="sxs-lookup"><span data-stu-id="5159e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5159e-133">id</span><span class="sxs-lookup"><span data-stu-id="5159e-133">id</span></span>|<span data-ttu-id="5159e-134">String</span><span class="sxs-lookup"><span data-stu-id="5159e-134">String</span></span>|<span data-ttu-id="5159e-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="5159e-135">Key of the entity.</span></span> <span data-ttu-id="5159e-136">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5159e-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5159e-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="5159e-137">lastModifiedDateTime</span></span>|<span data-ttu-id="5159e-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5159e-138">DateTimeOffset</span></span>|<span data-ttu-id="5159e-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="5159e-139">DateTime the object was last modified.</span></span> <span data-ttu-id="5159e-140">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5159e-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5159e-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="5159e-141">roleScopeTagIds</span></span>|<span data-ttu-id="5159e-142">String 集合</span><span class="sxs-lookup"><span data-stu-id="5159e-142">String collection</span></span>|<span data-ttu-id="5159e-143">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="5159e-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="5159e-144">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5159e-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5159e-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="5159e-145">supportsScopeTags</span></span>|<span data-ttu-id="5159e-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="5159e-146">Boolean</span></span>|<span data-ttu-id="5159e-147">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="5159e-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="5159e-148">如果此值为 false，则不允许分配给 ScopeTags 属性，并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="5159e-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="5159e-149">这适用于在 Silverlight 中创建的旧版策略，可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="5159e-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="5159e-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="5159e-150">This property is read-only.</span></span> <span data-ttu-id="5159e-151">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5159e-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5159e-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="5159e-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="5159e-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="5159e-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="5159e-154">适用于此策略的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="5159e-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="5159e-155">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5159e-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5159e-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="5159e-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="5159e-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="5159e-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="5159e-158">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="5159e-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="5159e-159">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5159e-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5159e-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="5159e-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="5159e-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="5159e-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="5159e-162">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="5159e-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="5159e-163">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5159e-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5159e-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="5159e-164">createdDateTime</span></span>|<span data-ttu-id="5159e-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5159e-165">DateTimeOffset</span></span>|<span data-ttu-id="5159e-166">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="5159e-166">DateTime the object was created.</span></span> <span data-ttu-id="5159e-167">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5159e-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5159e-168">description</span><span class="sxs-lookup"><span data-stu-id="5159e-168">description</span></span>|<span data-ttu-id="5159e-169">String</span><span class="sxs-lookup"><span data-stu-id="5159e-169">String</span></span>|<span data-ttu-id="5159e-170">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="5159e-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="5159e-171">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5159e-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5159e-172">displayName</span><span class="sxs-lookup"><span data-stu-id="5159e-172">displayName</span></span>|<span data-ttu-id="5159e-173">String</span><span class="sxs-lookup"><span data-stu-id="5159e-173">String</span></span>|<span data-ttu-id="5159e-174">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="5159e-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="5159e-175">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5159e-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5159e-176">version</span><span class="sxs-lookup"><span data-stu-id="5159e-176">version</span></span>|<span data-ttu-id="5159e-177">Int32</span><span class="sxs-lookup"><span data-stu-id="5159e-177">Int32</span></span>|<span data-ttu-id="5159e-178">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="5159e-178">Version of the device configuration.</span></span> <span data-ttu-id="5159e-179">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5159e-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5159e-180">advancedThreatProtectionOnboardingBlob</span><span class="sxs-lookup"><span data-stu-id="5159e-180">advancedThreatProtectionOnboardingBlob</span></span>|<span data-ttu-id="5159e-181">String</span><span class="sxs-lookup"><span data-stu-id="5159e-181">String</span></span>|<span data-ttu-id="5159e-182">Windows Defender 高级威胁防护载入 Blob。</span><span class="sxs-lookup"><span data-stu-id="5159e-182">Windows Defender AdvancedThreatProtection Onboarding Blob.</span></span>|
|<span data-ttu-id="5159e-183">advancedThreatProtectionOnboardingFilename</span><span class="sxs-lookup"><span data-stu-id="5159e-183">advancedThreatProtectionOnboardingFilename</span></span>|<span data-ttu-id="5159e-184">String</span><span class="sxs-lookup"><span data-stu-id="5159e-184">String</span></span>|<span data-ttu-id="5159e-185">从中获取 AdvancedThreatProtectionOnboardingBlob 的文件的名称。</span><span class="sxs-lookup"><span data-stu-id="5159e-185">Name of the file from which AdvancedThreatProtectionOnboardingBlob was obtained.</span></span>|
|<span data-ttu-id="5159e-186">advancedThreatProtectionAutoPopulateOnboardingBlob</span><span class="sxs-lookup"><span data-stu-id="5159e-186">advancedThreatProtectionAutoPopulateOnboardingBlob</span></span>|<span data-ttu-id="5159e-187">Boolean</span><span class="sxs-lookup"><span data-stu-id="5159e-187">Boolean</span></span>|<span data-ttu-id="5159e-188">通过从高级威胁防护服务以编程方式自动填充载入 blob</span><span class="sxs-lookup"><span data-stu-id="5159e-188">Auto populate onboarding blob programmatically from Advanced Threat protection service</span></span>|
|<span data-ttu-id="5159e-189">allowSampleSharing</span><span class="sxs-lookup"><span data-stu-id="5159e-189">allowSampleSharing</span></span>|<span data-ttu-id="5159e-190">Boolean</span><span class="sxs-lookup"><span data-stu-id="5159e-190">Boolean</span></span>|<span data-ttu-id="5159e-191">Windows Defender 高级威胁防护“允许示例共享”规则</span><span class="sxs-lookup"><span data-stu-id="5159e-191">Windows Defender AdvancedThreatProtection "Allow Sample Sharing" Rule</span></span>|
|<span data-ttu-id="5159e-192">enableExpeditedTelemetryReporting</span><span class="sxs-lookup"><span data-stu-id="5159e-192">enableExpeditedTelemetryReporting</span></span>|<span data-ttu-id="5159e-193">Boolean</span><span class="sxs-lookup"><span data-stu-id="5159e-193">Boolean</span></span>|<span data-ttu-id="5159e-194">加速 Windows Defender 高级威胁防护遥测报告的频率。</span><span class="sxs-lookup"><span data-stu-id="5159e-194">Expedite Windows Defender Advanced Threat Protection telemetry reporting frequency.</span></span>|
|<span data-ttu-id="5159e-195">advancedThreatProtectionOffboardingBlob</span><span class="sxs-lookup"><span data-stu-id="5159e-195">advancedThreatProtectionOffboardingBlob</span></span>|<span data-ttu-id="5159e-196">String</span><span class="sxs-lookup"><span data-stu-id="5159e-196">String</span></span>|<span data-ttu-id="5159e-197">Windows Defender 高级威胁防护脱离 Blob。</span><span class="sxs-lookup"><span data-stu-id="5159e-197">Windows Defender AdvancedThreatProtection Offboarding Blob.</span></span>|
|<span data-ttu-id="5159e-198">advancedThreatProtectionOffboardingFilename</span><span class="sxs-lookup"><span data-stu-id="5159e-198">advancedThreatProtectionOffboardingFilename</span></span>|<span data-ttu-id="5159e-199">String</span><span class="sxs-lookup"><span data-stu-id="5159e-199">String</span></span>|<span data-ttu-id="5159e-200">从中获取 AdvancedThreatProtectionOffboardingBlob 的文件的名称。</span><span class="sxs-lookup"><span data-stu-id="5159e-200">Name of the file from which AdvancedThreatProtectionOffboardingBlob was obtained.</span></span>|



## <a name="response"></a><span data-ttu-id="5159e-201">响应</span><span class="sxs-lookup"><span data-stu-id="5159e-201">Response</span></span>
<span data-ttu-id="5159e-202">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="5159e-202">If successful, this method returns a `200 OK` response code and an updated [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5159e-203">示例</span><span class="sxs-lookup"><span data-stu-id="5159e-203">Example</span></span>

### <a name="request"></a><span data-ttu-id="5159e-204">请求</span><span class="sxs-lookup"><span data-stu-id="5159e-204">Request</span></span>
<span data-ttu-id="5159e-205">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="5159e-205">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="5159e-206">响应</span><span class="sxs-lookup"><span data-stu-id="5159e-206">Response</span></span>
<span data-ttu-id="5159e-p113">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="5159e-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




