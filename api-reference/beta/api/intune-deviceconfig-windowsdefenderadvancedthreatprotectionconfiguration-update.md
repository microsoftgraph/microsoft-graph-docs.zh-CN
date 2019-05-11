---
title: 更新 windowsDefenderAdvancedThreatProtectionConfiguration
description: 更新 windowsDefenderAdvancedThreatProtectionConfiguration 对象的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: db84b3145005a7314c3b6d07b119af860b69b8c4
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2019
ms.locfileid: "33917994"
---
# <a name="update-windowsdefenderadvancedthreatprotectionconfiguration"></a><span data-ttu-id="f03c6-103">更新 windowsDefenderAdvancedThreatProtectionConfiguration</span><span class="sxs-lookup"><span data-stu-id="f03c6-103">Update windowsDefenderAdvancedThreatProtectionConfiguration</span></span>

> <span data-ttu-id="f03c6-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="f03c6-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f03c6-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f03c6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f03c6-106">更新 [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="f03c6-106">Update the properties of a [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f03c6-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="f03c6-107">Prerequisites</span></span>
<span data-ttu-id="f03c6-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f03c6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f03c6-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="f03c6-110">Permission type</span></span>|<span data-ttu-id="f03c6-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="f03c6-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f03c6-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f03c6-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f03c6-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f03c6-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f03c6-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f03c6-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f03c6-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="f03c6-115">Not supported.</span></span>|
|<span data-ttu-id="f03c6-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="f03c6-116">Application</span></span>|<span data-ttu-id="f03c6-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="f03c6-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f03c6-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f03c6-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="f03c6-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="f03c6-119">Request headers</span></span>
|<span data-ttu-id="f03c6-120">标头</span><span class="sxs-lookup"><span data-stu-id="f03c6-120">Header</span></span>|<span data-ttu-id="f03c6-121">值</span><span class="sxs-lookup"><span data-stu-id="f03c6-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f03c6-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="f03c6-122">Authorization</span></span>|<span data-ttu-id="f03c6-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="f03c6-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f03c6-124">接受</span><span class="sxs-lookup"><span data-stu-id="f03c6-124">Accept</span></span>|<span data-ttu-id="f03c6-125">application/json</span><span class="sxs-lookup"><span data-stu-id="f03c6-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f03c6-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="f03c6-126">Request body</span></span>
<span data-ttu-id="f03c6-127">在请求正文中，提供 [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f03c6-127">In the request body, supply a JSON representation for the [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md) object.</span></span>

<span data-ttu-id="f03c6-128">下表显示创建 [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="f03c6-128">The following table shows the properties that are required when you create the [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md).</span></span>

|<span data-ttu-id="f03c6-129">属性</span><span class="sxs-lookup"><span data-stu-id="f03c6-129">Property</span></span>|<span data-ttu-id="f03c6-130">类型</span><span class="sxs-lookup"><span data-stu-id="f03c6-130">Type</span></span>|<span data-ttu-id="f03c6-131">说明</span><span class="sxs-lookup"><span data-stu-id="f03c6-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f03c6-132">id</span><span class="sxs-lookup"><span data-stu-id="f03c6-132">id</span></span>|<span data-ttu-id="f03c6-133">字符串</span><span class="sxs-lookup"><span data-stu-id="f03c6-133">String</span></span>|<span data-ttu-id="f03c6-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="f03c6-134">Key of the entity.</span></span> <span data-ttu-id="f03c6-135">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f03c6-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f03c6-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f03c6-136">lastModifiedDateTime</span></span>|<span data-ttu-id="f03c6-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f03c6-137">DateTimeOffset</span></span>|<span data-ttu-id="f03c6-138">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="f03c6-138">DateTime the object was last modified.</span></span> <span data-ttu-id="f03c6-139">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f03c6-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f03c6-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="f03c6-140">roleScopeTagIds</span></span>|<span data-ttu-id="f03c6-141">String collection</span><span class="sxs-lookup"><span data-stu-id="f03c6-141">String collection</span></span>|<span data-ttu-id="f03c6-142">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="f03c6-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="f03c6-143">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f03c6-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f03c6-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="f03c6-144">supportsScopeTags</span></span>|<span data-ttu-id="f03c6-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="f03c6-145">Boolean</span></span>|<span data-ttu-id="f03c6-146">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="f03c6-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="f03c6-147">如果此值为 false, 则不允许分配给 ScopeTags 属性, 并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="f03c6-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="f03c6-148">这适用于在 Silverlight 中创建的旧版策略, 可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="f03c6-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="f03c6-149">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="f03c6-149">This property is read-only.</span></span> <span data-ttu-id="f03c6-150">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f03c6-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f03c6-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f03c6-151">createdDateTime</span></span>|<span data-ttu-id="f03c6-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f03c6-152">DateTimeOffset</span></span>|<span data-ttu-id="f03c6-153">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="f03c6-153">DateTime the object was created.</span></span> <span data-ttu-id="f03c6-154">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f03c6-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f03c6-155">说明</span><span class="sxs-lookup"><span data-stu-id="f03c6-155">description</span></span>|<span data-ttu-id="f03c6-156">String</span><span class="sxs-lookup"><span data-stu-id="f03c6-156">String</span></span>|<span data-ttu-id="f03c6-157">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="f03c6-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="f03c6-158">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f03c6-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f03c6-159">displayName</span><span class="sxs-lookup"><span data-stu-id="f03c6-159">displayName</span></span>|<span data-ttu-id="f03c6-160">String</span><span class="sxs-lookup"><span data-stu-id="f03c6-160">String</span></span>|<span data-ttu-id="f03c6-161">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="f03c6-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="f03c6-162">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f03c6-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f03c6-163">version</span><span class="sxs-lookup"><span data-stu-id="f03c6-163">version</span></span>|<span data-ttu-id="f03c6-164">Int32</span><span class="sxs-lookup"><span data-stu-id="f03c6-164">Int32</span></span>|<span data-ttu-id="f03c6-165">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="f03c6-165">Version of the device configuration.</span></span> <span data-ttu-id="f03c6-166">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f03c6-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f03c6-167">advancedThreatProtectionOnboardingBlob</span><span class="sxs-lookup"><span data-stu-id="f03c6-167">advancedThreatProtectionOnboardingBlob</span></span>|<span data-ttu-id="f03c6-168">String</span><span class="sxs-lookup"><span data-stu-id="f03c6-168">String</span></span>|<span data-ttu-id="f03c6-169">Windows Defender 高级威胁防护载入 Blob。</span><span class="sxs-lookup"><span data-stu-id="f03c6-169">Windows Defender AdvancedThreatProtection Onboarding Blob.</span></span>|
|<span data-ttu-id="f03c6-170">advancedThreatProtectionOnboardingFilename</span><span class="sxs-lookup"><span data-stu-id="f03c6-170">advancedThreatProtectionOnboardingFilename</span></span>|<span data-ttu-id="f03c6-171">String</span><span class="sxs-lookup"><span data-stu-id="f03c6-171">String</span></span>|<span data-ttu-id="f03c6-172">从中获取 AdvancedThreatProtectionOnboardingBlob 的文件的名称。</span><span class="sxs-lookup"><span data-stu-id="f03c6-172">Name of the file from which AdvancedThreatProtectionOnboardingBlob was obtained.</span></span>|
|<span data-ttu-id="f03c6-173">advancedThreatProtectionAutoPopulateOnboardingBlob</span><span class="sxs-lookup"><span data-stu-id="f03c6-173">advancedThreatProtectionAutoPopulateOnboardingBlob</span></span>|<span data-ttu-id="f03c6-174">Boolean</span><span class="sxs-lookup"><span data-stu-id="f03c6-174">Boolean</span></span>|<span data-ttu-id="f03c6-175">通过从高级威胁防护服务以编程方式自动填充载入 blob</span><span class="sxs-lookup"><span data-stu-id="f03c6-175">Auto populate onboarding blob programmatically from Advanced Threat protection service</span></span>|
|<span data-ttu-id="f03c6-176">allowSampleSharing</span><span class="sxs-lookup"><span data-stu-id="f03c6-176">allowSampleSharing</span></span>|<span data-ttu-id="f03c6-177">Boolean</span><span class="sxs-lookup"><span data-stu-id="f03c6-177">Boolean</span></span>|<span data-ttu-id="f03c6-178">Windows Defender 高级威胁防护“允许示例共享”规则</span><span class="sxs-lookup"><span data-stu-id="f03c6-178">Windows Defender AdvancedThreatProtection "Allow Sample Sharing" Rule</span></span>|
|<span data-ttu-id="f03c6-179">enableExpeditedTelemetryReporting</span><span class="sxs-lookup"><span data-stu-id="f03c6-179">enableExpeditedTelemetryReporting</span></span>|<span data-ttu-id="f03c6-180">Boolean</span><span class="sxs-lookup"><span data-stu-id="f03c6-180">Boolean</span></span>|<span data-ttu-id="f03c6-181">加速 Windows Defender 高级威胁防护遥测报告的频率。</span><span class="sxs-lookup"><span data-stu-id="f03c6-181">Expedite Windows Defender Advanced Threat Protection telemetry reporting frequency.</span></span>|
|<span data-ttu-id="f03c6-182">advancedThreatProtectionOffboardingBlob</span><span class="sxs-lookup"><span data-stu-id="f03c6-182">advancedThreatProtectionOffboardingBlob</span></span>|<span data-ttu-id="f03c6-183">String</span><span class="sxs-lookup"><span data-stu-id="f03c6-183">String</span></span>|<span data-ttu-id="f03c6-184">Windows Defender 高级威胁防护脱离 Blob。</span><span class="sxs-lookup"><span data-stu-id="f03c6-184">Windows Defender AdvancedThreatProtection Offboarding Blob.</span></span>|
|<span data-ttu-id="f03c6-185">advancedThreatProtectionOffboardingFilename</span><span class="sxs-lookup"><span data-stu-id="f03c6-185">advancedThreatProtectionOffboardingFilename</span></span>|<span data-ttu-id="f03c6-186">String</span><span class="sxs-lookup"><span data-stu-id="f03c6-186">String</span></span>|<span data-ttu-id="f03c6-187">从中获取 AdvancedThreatProtectionOffboardingBlob 的文件的名称。</span><span class="sxs-lookup"><span data-stu-id="f03c6-187">Name of the file from which AdvancedThreatProtectionOffboardingBlob was obtained.</span></span>|



## <a name="response"></a><span data-ttu-id="f03c6-188">响应</span><span class="sxs-lookup"><span data-stu-id="f03c6-188">Response</span></span>
<span data-ttu-id="f03c6-189">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="f03c6-189">If successful, this method returns a `200 OK` response code and an updated [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f03c6-190">示例</span><span class="sxs-lookup"><span data-stu-id="f03c6-190">Example</span></span>

### <a name="request"></a><span data-ttu-id="f03c6-191">请求</span><span class="sxs-lookup"><span data-stu-id="f03c6-191">Request</span></span>
<span data-ttu-id="f03c6-192">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="f03c6-192">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 830

{
  "@odata.type": "#microsoft.graph.windowsDefenderAdvancedThreatProtectionConfiguration",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
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

### <a name="response"></a><span data-ttu-id="f03c6-193">响应</span><span class="sxs-lookup"><span data-stu-id="f03c6-193">Response</span></span>
<span data-ttu-id="f03c6-p110">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="f03c6-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1002

{
  "@odata.type": "#microsoft.graph.windowsDefenderAdvancedThreatProtectionConfiguration",
  "id": "294373aa-73aa-2943-aa73-4329aa734329",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
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




