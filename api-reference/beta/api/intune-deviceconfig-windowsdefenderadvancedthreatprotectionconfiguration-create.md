---
title: 创建 windowsDefenderAdvancedThreatProtectionConfiguration
description: 创建新的 windowsDefenderAdvancedThreatProtectionConfiguration 对象。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 1f6147a054d2addd5159c46f66d0d2133ce9e7bb
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29400499"
---
# <a name="create-windowsdefenderadvancedthreatprotectionconfiguration"></a><span data-ttu-id="111bd-103">创建 windowsDefenderAdvancedThreatProtectionConfiguration</span><span class="sxs-lookup"><span data-stu-id="111bd-103">Create windowsDefenderAdvancedThreatProtectionConfiguration</span></span>

> <span data-ttu-id="111bd-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="111bd-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="111bd-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="111bd-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="111bd-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="111bd-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="111bd-107">创建新的 [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="111bd-107">Create a new [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="111bd-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="111bd-108">Prerequisites</span></span>
<span data-ttu-id="111bd-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="111bd-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="111bd-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="111bd-111">Permission type</span></span>|<span data-ttu-id="111bd-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="111bd-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="111bd-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="111bd-113">Delegated (work or school account)</span></span>|<span data-ttu-id="111bd-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="111bd-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="111bd-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="111bd-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="111bd-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="111bd-116">Not supported.</span></span>|
|<span data-ttu-id="111bd-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="111bd-117">Application</span></span>|<span data-ttu-id="111bd-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="111bd-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="111bd-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="111bd-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="111bd-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="111bd-120">Request headers</span></span>
|<span data-ttu-id="111bd-121">标头</span><span class="sxs-lookup"><span data-stu-id="111bd-121">Header</span></span>|<span data-ttu-id="111bd-122">值</span><span class="sxs-lookup"><span data-stu-id="111bd-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="111bd-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="111bd-123">Authorization</span></span>|<span data-ttu-id="111bd-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="111bd-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="111bd-125">Accept</span><span class="sxs-lookup"><span data-stu-id="111bd-125">Accept</span></span>|<span data-ttu-id="111bd-126">application/json</span><span class="sxs-lookup"><span data-stu-id="111bd-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="111bd-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="111bd-127">Request body</span></span>
<span data-ttu-id="111bd-128">在请求正文中，提供 windowsDefenderAdvancedThreatProtectionConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="111bd-128">In the request body, supply a JSON representation for the windowsDefenderAdvancedThreatProtectionConfiguration object.</span></span>

<span data-ttu-id="111bd-129">下表显示创建 windowsDefenderAdvancedThreatProtectionConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="111bd-129">The following table shows the properties that are required when you create the windowsDefenderAdvancedThreatProtectionConfiguration.</span></span>

|<span data-ttu-id="111bd-130">属性</span><span class="sxs-lookup"><span data-stu-id="111bd-130">Property</span></span>|<span data-ttu-id="111bd-131">类型</span><span class="sxs-lookup"><span data-stu-id="111bd-131">Type</span></span>|<span data-ttu-id="111bd-132">说明</span><span class="sxs-lookup"><span data-stu-id="111bd-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="111bd-133">id</span><span class="sxs-lookup"><span data-stu-id="111bd-133">id</span></span>|<span data-ttu-id="111bd-134">String</span><span class="sxs-lookup"><span data-stu-id="111bd-134">String</span></span>|<span data-ttu-id="111bd-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="111bd-135">Key of the entity.</span></span> <span data-ttu-id="111bd-136">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="111bd-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="111bd-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="111bd-137">lastModifiedDateTime</span></span>|<span data-ttu-id="111bd-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="111bd-138">DateTimeOffset</span></span>|<span data-ttu-id="111bd-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="111bd-139">DateTime the object was last modified.</span></span> <span data-ttu-id="111bd-140">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="111bd-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="111bd-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="111bd-141">roleScopeTagIds</span></span>|<span data-ttu-id="111bd-142">String 集合</span><span class="sxs-lookup"><span data-stu-id="111bd-142">String collection</span></span>|<span data-ttu-id="111bd-143">此实体实例范围标记的列表。</span><span class="sxs-lookup"><span data-stu-id="111bd-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="111bd-144">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="111bd-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="111bd-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="111bd-145">supportsScopeTags</span></span>|<span data-ttu-id="111bd-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="111bd-146">Boolean</span></span>|<span data-ttu-id="111bd-147">指示基础的设备配置支持分配的范围标记。</span><span class="sxs-lookup"><span data-stu-id="111bd-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="111bd-148">此值为 false，并且实体将不会对作用域的用户可见时，不允许将分配给 ScopeTags 属性。</span><span class="sxs-lookup"><span data-stu-id="111bd-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="111bd-149">这将发生在 Silverlight 中创建的旧策略，并可以解析通过删除并重新创建 Azure 门户中的策略。</span><span class="sxs-lookup"><span data-stu-id="111bd-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="111bd-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="111bd-150">This property is read-only.</span></span> <span data-ttu-id="111bd-151">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="111bd-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="111bd-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="111bd-152">createdDateTime</span></span>|<span data-ttu-id="111bd-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="111bd-153">DateTimeOffset</span></span>|<span data-ttu-id="111bd-154">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="111bd-154">DateTime the object was created.</span></span> <span data-ttu-id="111bd-155">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="111bd-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="111bd-156">description</span><span class="sxs-lookup"><span data-stu-id="111bd-156">description</span></span>|<span data-ttu-id="111bd-157">String</span><span class="sxs-lookup"><span data-stu-id="111bd-157">String</span></span>|<span data-ttu-id="111bd-158">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="111bd-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="111bd-159">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="111bd-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="111bd-160">displayName</span><span class="sxs-lookup"><span data-stu-id="111bd-160">displayName</span></span>|<span data-ttu-id="111bd-161">String</span><span class="sxs-lookup"><span data-stu-id="111bd-161">String</span></span>|<span data-ttu-id="111bd-162">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="111bd-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="111bd-163">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="111bd-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="111bd-164">version</span><span class="sxs-lookup"><span data-stu-id="111bd-164">version</span></span>|<span data-ttu-id="111bd-165">Int32</span><span class="sxs-lookup"><span data-stu-id="111bd-165">Int32</span></span>|<span data-ttu-id="111bd-166">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="111bd-166">Version of the device configuration.</span></span> <span data-ttu-id="111bd-167">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="111bd-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="111bd-168">advancedThreatProtectionOnboardingBlob</span><span class="sxs-lookup"><span data-stu-id="111bd-168">advancedThreatProtectionOnboardingBlob</span></span>|<span data-ttu-id="111bd-169">String</span><span class="sxs-lookup"><span data-stu-id="111bd-169">String</span></span>|<span data-ttu-id="111bd-170">Windows Defender AdvancedThreatProtection 入职培训 Blob。</span><span class="sxs-lookup"><span data-stu-id="111bd-170">Windows Defender AdvancedThreatProtection Onboarding Blob.</span></span>|
|<span data-ttu-id="111bd-171">advancedThreatProtectionOnboardingFilename</span><span class="sxs-lookup"><span data-stu-id="111bd-171">advancedThreatProtectionOnboardingFilename</span></span>|<span data-ttu-id="111bd-172">String</span><span class="sxs-lookup"><span data-stu-id="111bd-172">String</span></span>|<span data-ttu-id="111bd-173">从中获取 AdvancedThreatProtectionOnboardingBlob 文件的名称。</span><span class="sxs-lookup"><span data-stu-id="111bd-173">Name of the file from which AdvancedThreatProtectionOnboardingBlob was obtained.</span></span>|
|<span data-ttu-id="111bd-174">advancedThreatProtectionAutoPopulateOnboardingBlob</span><span class="sxs-lookup"><span data-stu-id="111bd-174">advancedThreatProtectionAutoPopulateOnboardingBlob</span></span>|<span data-ttu-id="111bd-175">Boolean</span><span class="sxs-lookup"><span data-stu-id="111bd-175">Boolean</span></span>|<span data-ttu-id="111bd-176">自动填充入职培训 blob 以编程方式从高级威胁保护服务</span><span class="sxs-lookup"><span data-stu-id="111bd-176">Auto populate onboarding blob programmatically from Advanced Threat protection service</span></span>|
|<span data-ttu-id="111bd-177">allowSampleSharing</span><span class="sxs-lookup"><span data-stu-id="111bd-177">allowSampleSharing</span></span>|<span data-ttu-id="111bd-178">Boolean</span><span class="sxs-lookup"><span data-stu-id="111bd-178">Boolean</span></span>|<span data-ttu-id="111bd-179">Windows Defender 高级威胁防护“允许示例共享”规则</span><span class="sxs-lookup"><span data-stu-id="111bd-179">Windows Defender AdvancedThreatProtection "Allow Sample Sharing" Rule</span></span>|
|<span data-ttu-id="111bd-180">enableExpeditedTelemetryReporting</span><span class="sxs-lookup"><span data-stu-id="111bd-180">enableExpeditedTelemetryReporting</span></span>|<span data-ttu-id="111bd-181">Boolean</span><span class="sxs-lookup"><span data-stu-id="111bd-181">Boolean</span></span>|<span data-ttu-id="111bd-182">加速 Windows Defender 高级威胁防护遥测报告的频率。</span><span class="sxs-lookup"><span data-stu-id="111bd-182">Expedite Windows Defender Advanced Threat Protection telemetry reporting frequency.</span></span>|
|<span data-ttu-id="111bd-183">advancedThreatProtectionOffboardingBlob</span><span class="sxs-lookup"><span data-stu-id="111bd-183">advancedThreatProtectionOffboardingBlob</span></span>|<span data-ttu-id="111bd-184">String</span><span class="sxs-lookup"><span data-stu-id="111bd-184">String</span></span>|<span data-ttu-id="111bd-185">Windows Defender AdvancedThreatProtection 分离 Blob。</span><span class="sxs-lookup"><span data-stu-id="111bd-185">Windows Defender AdvancedThreatProtection Offboarding Blob.</span></span>|
|<span data-ttu-id="111bd-186">advancedThreatProtectionOffboardingFilename</span><span class="sxs-lookup"><span data-stu-id="111bd-186">advancedThreatProtectionOffboardingFilename</span></span>|<span data-ttu-id="111bd-187">String</span><span class="sxs-lookup"><span data-stu-id="111bd-187">String</span></span>|<span data-ttu-id="111bd-188">从中获取 AdvancedThreatProtectionOffboardingBlob 文件的名称。</span><span class="sxs-lookup"><span data-stu-id="111bd-188">Name of the file from which AdvancedThreatProtectionOffboardingBlob was obtained.</span></span>|



## <a name="response"></a><span data-ttu-id="111bd-189">响应</span><span class="sxs-lookup"><span data-stu-id="111bd-189">Response</span></span>
<span data-ttu-id="111bd-190">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="111bd-190">If successful, this method returns a `201 Created` response code and a [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="111bd-191">示例</span><span class="sxs-lookup"><span data-stu-id="111bd-191">Example</span></span>

### <a name="request"></a><span data-ttu-id="111bd-192">请求</span><span class="sxs-lookup"><span data-stu-id="111bd-192">Request</span></span>
<span data-ttu-id="111bd-193">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="111bd-193">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
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

### <a name="response"></a><span data-ttu-id="111bd-194">响应</span><span class="sxs-lookup"><span data-stu-id="111bd-194">Response</span></span>
<span data-ttu-id="111bd-p111">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="111bd-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




