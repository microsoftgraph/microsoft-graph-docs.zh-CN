---
title: 更新 windowsDefenderAdvancedThreatProtectionConfiguration
description: 更新 windowsDefenderAdvancedThreatProtectionConfiguration 对象的属性。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: fea7f12f3ea6e90aaeea38d828dbe072b2995430
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29396369"
---
# <a name="update-windowsdefenderadvancedthreatprotectionconfiguration"></a><span data-ttu-id="83ef3-103">更新 windowsDefenderAdvancedThreatProtectionConfiguration</span><span class="sxs-lookup"><span data-stu-id="83ef3-103">Update windowsDefenderAdvancedThreatProtectionConfiguration</span></span>

> <span data-ttu-id="83ef3-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="83ef3-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="83ef3-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="83ef3-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="83ef3-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="83ef3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="83ef3-107">更新 [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="83ef3-107">Update the properties of a [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="83ef3-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="83ef3-108">Prerequisites</span></span>
<span data-ttu-id="83ef3-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="83ef3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="83ef3-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="83ef3-111">Permission type</span></span>|<span data-ttu-id="83ef3-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="83ef3-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="83ef3-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="83ef3-113">Delegated (work or school account)</span></span>|<span data-ttu-id="83ef3-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="83ef3-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="83ef3-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="83ef3-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="83ef3-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="83ef3-116">Not supported.</span></span>|
|<span data-ttu-id="83ef3-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="83ef3-117">Application</span></span>|<span data-ttu-id="83ef3-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="83ef3-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="83ef3-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="83ef3-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="83ef3-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="83ef3-120">Request headers</span></span>
|<span data-ttu-id="83ef3-121">标头</span><span class="sxs-lookup"><span data-stu-id="83ef3-121">Header</span></span>|<span data-ttu-id="83ef3-122">值</span><span class="sxs-lookup"><span data-stu-id="83ef3-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="83ef3-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="83ef3-123">Authorization</span></span>|<span data-ttu-id="83ef3-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="83ef3-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="83ef3-125">Accept</span><span class="sxs-lookup"><span data-stu-id="83ef3-125">Accept</span></span>|<span data-ttu-id="83ef3-126">application/json</span><span class="sxs-lookup"><span data-stu-id="83ef3-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="83ef3-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="83ef3-127">Request body</span></span>
<span data-ttu-id="83ef3-128">在请求正文中，提供 [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="83ef3-128">In the request body, supply a JSON representation for the [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md) object.</span></span>

<span data-ttu-id="83ef3-129">下表显示创建 [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="83ef3-129">The following table shows the properties that are required when you create the [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md).</span></span>

|<span data-ttu-id="83ef3-130">属性</span><span class="sxs-lookup"><span data-stu-id="83ef3-130">Property</span></span>|<span data-ttu-id="83ef3-131">类型</span><span class="sxs-lookup"><span data-stu-id="83ef3-131">Type</span></span>|<span data-ttu-id="83ef3-132">说明</span><span class="sxs-lookup"><span data-stu-id="83ef3-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="83ef3-133">id</span><span class="sxs-lookup"><span data-stu-id="83ef3-133">id</span></span>|<span data-ttu-id="83ef3-134">String</span><span class="sxs-lookup"><span data-stu-id="83ef3-134">String</span></span>|<span data-ttu-id="83ef3-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="83ef3-135">Key of the entity.</span></span> <span data-ttu-id="83ef3-136">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="83ef3-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="83ef3-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="83ef3-137">lastModifiedDateTime</span></span>|<span data-ttu-id="83ef3-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="83ef3-138">DateTimeOffset</span></span>|<span data-ttu-id="83ef3-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="83ef3-139">DateTime the object was last modified.</span></span> <span data-ttu-id="83ef3-140">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="83ef3-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="83ef3-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="83ef3-141">roleScopeTagIds</span></span>|<span data-ttu-id="83ef3-142">String 集合</span><span class="sxs-lookup"><span data-stu-id="83ef3-142">String collection</span></span>|<span data-ttu-id="83ef3-143">此实体实例范围标记的列表。</span><span class="sxs-lookup"><span data-stu-id="83ef3-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="83ef3-144">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="83ef3-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="83ef3-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="83ef3-145">supportsScopeTags</span></span>|<span data-ttu-id="83ef3-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="83ef3-146">Boolean</span></span>|<span data-ttu-id="83ef3-147">指示基础的设备配置支持分配的范围标记。</span><span class="sxs-lookup"><span data-stu-id="83ef3-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="83ef3-148">此值为 false，并且实体将不会对作用域的用户可见时，不允许将分配给 ScopeTags 属性。</span><span class="sxs-lookup"><span data-stu-id="83ef3-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="83ef3-149">这将发生在 Silverlight 中创建的旧策略，并可以解析通过删除并重新创建 Azure 门户中的策略。</span><span class="sxs-lookup"><span data-stu-id="83ef3-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="83ef3-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="83ef3-150">This property is read-only.</span></span> <span data-ttu-id="83ef3-151">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="83ef3-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="83ef3-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="83ef3-152">createdDateTime</span></span>|<span data-ttu-id="83ef3-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="83ef3-153">DateTimeOffset</span></span>|<span data-ttu-id="83ef3-154">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="83ef3-154">DateTime the object was created.</span></span> <span data-ttu-id="83ef3-155">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="83ef3-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="83ef3-156">description</span><span class="sxs-lookup"><span data-stu-id="83ef3-156">description</span></span>|<span data-ttu-id="83ef3-157">String</span><span class="sxs-lookup"><span data-stu-id="83ef3-157">String</span></span>|<span data-ttu-id="83ef3-158">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="83ef3-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="83ef3-159">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="83ef3-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="83ef3-160">displayName</span><span class="sxs-lookup"><span data-stu-id="83ef3-160">displayName</span></span>|<span data-ttu-id="83ef3-161">String</span><span class="sxs-lookup"><span data-stu-id="83ef3-161">String</span></span>|<span data-ttu-id="83ef3-162">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="83ef3-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="83ef3-163">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="83ef3-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="83ef3-164">version</span><span class="sxs-lookup"><span data-stu-id="83ef3-164">version</span></span>|<span data-ttu-id="83ef3-165">Int32</span><span class="sxs-lookup"><span data-stu-id="83ef3-165">Int32</span></span>|<span data-ttu-id="83ef3-166">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="83ef3-166">Version of the device configuration.</span></span> <span data-ttu-id="83ef3-167">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="83ef3-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="83ef3-168">advancedThreatProtectionOnboardingBlob</span><span class="sxs-lookup"><span data-stu-id="83ef3-168">advancedThreatProtectionOnboardingBlob</span></span>|<span data-ttu-id="83ef3-169">String</span><span class="sxs-lookup"><span data-stu-id="83ef3-169">String</span></span>|<span data-ttu-id="83ef3-170">Windows Defender AdvancedThreatProtection 入职培训 Blob。</span><span class="sxs-lookup"><span data-stu-id="83ef3-170">Windows Defender AdvancedThreatProtection Onboarding Blob.</span></span>|
|<span data-ttu-id="83ef3-171">advancedThreatProtectionOnboardingFilename</span><span class="sxs-lookup"><span data-stu-id="83ef3-171">advancedThreatProtectionOnboardingFilename</span></span>|<span data-ttu-id="83ef3-172">String</span><span class="sxs-lookup"><span data-stu-id="83ef3-172">String</span></span>|<span data-ttu-id="83ef3-173">从中获取 AdvancedThreatProtectionOnboardingBlob 文件的名称。</span><span class="sxs-lookup"><span data-stu-id="83ef3-173">Name of the file from which AdvancedThreatProtectionOnboardingBlob was obtained.</span></span>|
|<span data-ttu-id="83ef3-174">advancedThreatProtectionAutoPopulateOnboardingBlob</span><span class="sxs-lookup"><span data-stu-id="83ef3-174">advancedThreatProtectionAutoPopulateOnboardingBlob</span></span>|<span data-ttu-id="83ef3-175">Boolean</span><span class="sxs-lookup"><span data-stu-id="83ef3-175">Boolean</span></span>|<span data-ttu-id="83ef3-176">自动填充入职培训 blob 以编程方式从高级威胁保护服务</span><span class="sxs-lookup"><span data-stu-id="83ef3-176">Auto populate onboarding blob programmatically from Advanced Threat protection service</span></span>|
|<span data-ttu-id="83ef3-177">allowSampleSharing</span><span class="sxs-lookup"><span data-stu-id="83ef3-177">allowSampleSharing</span></span>|<span data-ttu-id="83ef3-178">Boolean</span><span class="sxs-lookup"><span data-stu-id="83ef3-178">Boolean</span></span>|<span data-ttu-id="83ef3-179">Windows Defender 高级威胁防护“允许示例共享”规则</span><span class="sxs-lookup"><span data-stu-id="83ef3-179">Windows Defender AdvancedThreatProtection "Allow Sample Sharing" Rule</span></span>|
|<span data-ttu-id="83ef3-180">enableExpeditedTelemetryReporting</span><span class="sxs-lookup"><span data-stu-id="83ef3-180">enableExpeditedTelemetryReporting</span></span>|<span data-ttu-id="83ef3-181">Boolean</span><span class="sxs-lookup"><span data-stu-id="83ef3-181">Boolean</span></span>|<span data-ttu-id="83ef3-182">加速 Windows Defender 高级威胁防护遥测报告的频率。</span><span class="sxs-lookup"><span data-stu-id="83ef3-182">Expedite Windows Defender Advanced Threat Protection telemetry reporting frequency.</span></span>|
|<span data-ttu-id="83ef3-183">advancedThreatProtectionOffboardingBlob</span><span class="sxs-lookup"><span data-stu-id="83ef3-183">advancedThreatProtectionOffboardingBlob</span></span>|<span data-ttu-id="83ef3-184">String</span><span class="sxs-lookup"><span data-stu-id="83ef3-184">String</span></span>|<span data-ttu-id="83ef3-185">Windows Defender AdvancedThreatProtection 分离 Blob。</span><span class="sxs-lookup"><span data-stu-id="83ef3-185">Windows Defender AdvancedThreatProtection Offboarding Blob.</span></span>|
|<span data-ttu-id="83ef3-186">advancedThreatProtectionOffboardingFilename</span><span class="sxs-lookup"><span data-stu-id="83ef3-186">advancedThreatProtectionOffboardingFilename</span></span>|<span data-ttu-id="83ef3-187">String</span><span class="sxs-lookup"><span data-stu-id="83ef3-187">String</span></span>|<span data-ttu-id="83ef3-188">从中获取 AdvancedThreatProtectionOffboardingBlob 文件的名称。</span><span class="sxs-lookup"><span data-stu-id="83ef3-188">Name of the file from which AdvancedThreatProtectionOffboardingBlob was obtained.</span></span>|



## <a name="response"></a><span data-ttu-id="83ef3-189">响应</span><span class="sxs-lookup"><span data-stu-id="83ef3-189">Response</span></span>
<span data-ttu-id="83ef3-190">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="83ef3-190">If successful, this method returns a `200 OK` response code and an updated [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="83ef3-191">示例</span><span class="sxs-lookup"><span data-stu-id="83ef3-191">Example</span></span>

### <a name="request"></a><span data-ttu-id="83ef3-192">请求</span><span class="sxs-lookup"><span data-stu-id="83ef3-192">Request</span></span>
<span data-ttu-id="83ef3-193">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="83ef3-193">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="83ef3-194">响应</span><span class="sxs-lookup"><span data-stu-id="83ef3-194">Response</span></span>
<span data-ttu-id="83ef3-p111">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="83ef3-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




