---
title: 创建 windowsIdentityProtectionConfiguration
description: 创建新的 windowsIdentityProtectionConfiguration 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 674e4fccb6777c527b1051fddc0926253966a8cd
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51150953"
---
# <a name="create-windowsidentityprotectionconfiguration"></a><span data-ttu-id="57e63-103">创建 windowsIdentityProtectionConfiguration</span><span class="sxs-lookup"><span data-stu-id="57e63-103">Create windowsIdentityProtectionConfiguration</span></span>

<span data-ttu-id="57e63-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="57e63-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="57e63-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="57e63-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="57e63-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="57e63-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="57e63-107">创建新的 [windowsIdentityProtectionConfiguration](../resources/intune-deviceconfig-windowsidentityprotectionconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="57e63-107">Create a new [windowsIdentityProtectionConfiguration](../resources/intune-deviceconfig-windowsidentityprotectionconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="57e63-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="57e63-108">Prerequisites</span></span>
<span data-ttu-id="57e63-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="57e63-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="57e63-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="57e63-111">Permission type</span></span>|<span data-ttu-id="57e63-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="57e63-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="57e63-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="57e63-113">Delegated (work or school account)</span></span>|<span data-ttu-id="57e63-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="57e63-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="57e63-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="57e63-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="57e63-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="57e63-116">Not supported.</span></span>|
|<span data-ttu-id="57e63-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="57e63-117">Application</span></span>|<span data-ttu-id="57e63-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="57e63-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="57e63-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="57e63-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="57e63-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="57e63-120">Request headers</span></span>
|<span data-ttu-id="57e63-121">标头</span><span class="sxs-lookup"><span data-stu-id="57e63-121">Header</span></span>|<span data-ttu-id="57e63-122">值</span><span class="sxs-lookup"><span data-stu-id="57e63-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="57e63-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="57e63-123">Authorization</span></span>|<span data-ttu-id="57e63-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="57e63-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="57e63-125">接受</span><span class="sxs-lookup"><span data-stu-id="57e63-125">Accept</span></span>|<span data-ttu-id="57e63-126">application/json</span><span class="sxs-lookup"><span data-stu-id="57e63-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="57e63-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="57e63-127">Request body</span></span>
<span data-ttu-id="57e63-128">在请求正文中，提供 windowsIdentityProtectionConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="57e63-128">In the request body, supply a JSON representation for the windowsIdentityProtectionConfiguration object.</span></span>

<span data-ttu-id="57e63-129">下表显示创建 windowsIdentityProtectionConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="57e63-129">The following table shows the properties that are required when you create the windowsIdentityProtectionConfiguration.</span></span>

|<span data-ttu-id="57e63-130">属性</span><span class="sxs-lookup"><span data-stu-id="57e63-130">Property</span></span>|<span data-ttu-id="57e63-131">类型</span><span class="sxs-lookup"><span data-stu-id="57e63-131">Type</span></span>|<span data-ttu-id="57e63-132">说明</span><span class="sxs-lookup"><span data-stu-id="57e63-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="57e63-133">id</span><span class="sxs-lookup"><span data-stu-id="57e63-133">id</span></span>|<span data-ttu-id="57e63-134">String</span><span class="sxs-lookup"><span data-stu-id="57e63-134">String</span></span>|<span data-ttu-id="57e63-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="57e63-135">Key of the entity.</span></span> <span data-ttu-id="57e63-136">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="57e63-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="57e63-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="57e63-137">lastModifiedDateTime</span></span>|<span data-ttu-id="57e63-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="57e63-138">DateTimeOffset</span></span>|<span data-ttu-id="57e63-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="57e63-139">DateTime the object was last modified.</span></span> <span data-ttu-id="57e63-140">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="57e63-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="57e63-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="57e63-141">roleScopeTagIds</span></span>|<span data-ttu-id="57e63-142">String collection</span><span class="sxs-lookup"><span data-stu-id="57e63-142">String collection</span></span>|<span data-ttu-id="57e63-143">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="57e63-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="57e63-144">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="57e63-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="57e63-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="57e63-145">supportsScopeTags</span></span>|<span data-ttu-id="57e63-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="57e63-146">Boolean</span></span>|<span data-ttu-id="57e63-147">指示基础设备配置是否支持分配范围标记。</span><span class="sxs-lookup"><span data-stu-id="57e63-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="57e63-148">当此值为 false 且实体对作用域用户不可见时，不允许分配给 ScopeTags 属性。</span><span class="sxs-lookup"><span data-stu-id="57e63-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="57e63-149">这适用于在 Silverlight 中创建的旧版策略，可通过在 Azure 门户中删除和重新创建策略来解决。</span><span class="sxs-lookup"><span data-stu-id="57e63-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="57e63-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="57e63-150">This property is read-only.</span></span> <span data-ttu-id="57e63-151">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="57e63-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="57e63-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="57e63-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="57e63-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="57e63-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="57e63-154">此策略的操作系统版本适用性。</span><span class="sxs-lookup"><span data-stu-id="57e63-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="57e63-155">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="57e63-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="57e63-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="57e63-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="57e63-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="57e63-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="57e63-158">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="57e63-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="57e63-159">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="57e63-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="57e63-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="57e63-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="57e63-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="57e63-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="57e63-162">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="57e63-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="57e63-163">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="57e63-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="57e63-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="57e63-164">createdDateTime</span></span>|<span data-ttu-id="57e63-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="57e63-165">DateTimeOffset</span></span>|<span data-ttu-id="57e63-166">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="57e63-166">DateTime the object was created.</span></span> <span data-ttu-id="57e63-167">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="57e63-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="57e63-168">说明</span><span class="sxs-lookup"><span data-stu-id="57e63-168">description</span></span>|<span data-ttu-id="57e63-169">String</span><span class="sxs-lookup"><span data-stu-id="57e63-169">String</span></span>|<span data-ttu-id="57e63-170">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="57e63-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="57e63-171">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="57e63-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="57e63-172">displayName</span><span class="sxs-lookup"><span data-stu-id="57e63-172">displayName</span></span>|<span data-ttu-id="57e63-173">String</span><span class="sxs-lookup"><span data-stu-id="57e63-173">String</span></span>|<span data-ttu-id="57e63-174">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="57e63-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="57e63-175">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="57e63-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="57e63-176">version</span><span class="sxs-lookup"><span data-stu-id="57e63-176">version</span></span>|<span data-ttu-id="57e63-177">Int32</span><span class="sxs-lookup"><span data-stu-id="57e63-177">Int32</span></span>|<span data-ttu-id="57e63-178">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="57e63-178">Version of the device configuration.</span></span> <span data-ttu-id="57e63-179">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="57e63-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="57e63-180">useSecurityKeyForSignin</span><span class="sxs-lookup"><span data-stu-id="57e63-180">useSecurityKeyForSignin</span></span>|<span data-ttu-id="57e63-181">Boolean</span><span class="sxs-lookup"><span data-stu-id="57e63-181">Boolean</span></span>|<span data-ttu-id="57e63-182">用于启用 Windows Hello 安全密钥作为登录凭据的布尔值。</span><span class="sxs-lookup"><span data-stu-id="57e63-182">Boolean value used to enable the Windows Hello security key as a logon credential.</span></span>|
|<span data-ttu-id="57e63-183">enhancedAntiSpoofingForFacialFeaturesEnabled</span><span class="sxs-lookup"><span data-stu-id="57e63-183">enhancedAntiSpoofingForFacialFeaturesEnabled</span></span>|<span data-ttu-id="57e63-184">Boolean</span><span class="sxs-lookup"><span data-stu-id="57e63-184">Boolean</span></span>|<span data-ttu-id="57e63-185">用于启用增强的反欺骗的布尔值，用于在 Windows Hello 人脸身份验证上识别面部功能。</span><span class="sxs-lookup"><span data-stu-id="57e63-185">Boolean value used to enable enhanced anti-spoofing for facial feature recognition on Windows Hello face authentication.</span></span>|
|<span data-ttu-id="57e63-186">pinMinimumLength</span><span class="sxs-lookup"><span data-stu-id="57e63-186">pinMinimumLength</span></span>|<span data-ttu-id="57e63-187">Int32</span><span class="sxs-lookup"><span data-stu-id="57e63-187">Int32</span></span>|<span data-ttu-id="57e63-188">用于设置 Windows Hello 企业 PIN 所需的最少字符数的整数值。</span><span class="sxs-lookup"><span data-stu-id="57e63-188">Integer value that sets the minimum number of characters required for the Windows Hello for Business PIN.</span></span> <span data-ttu-id="57e63-189">有效值为 4 到 127（含 4 和 127）以及小于或等于为最大 PIN 设置的值。</span><span class="sxs-lookup"><span data-stu-id="57e63-189">Valid values are 4 to 127 inclusive and less than or equal to the value set for the maximum PIN.</span></span> <span data-ttu-id="57e63-190">有效值为 4 至 127</span><span class="sxs-lookup"><span data-stu-id="57e63-190">Valid values 4 to 127</span></span>|
|<span data-ttu-id="57e63-191">pinMaximumLength</span><span class="sxs-lookup"><span data-stu-id="57e63-191">pinMaximumLength</span></span>|<span data-ttu-id="57e63-192">Int32</span><span class="sxs-lookup"><span data-stu-id="57e63-192">Int32</span></span>|<span data-ttu-id="57e63-193">用于设置工作 PIN 允许的最大字符数的整数值。</span><span class="sxs-lookup"><span data-stu-id="57e63-193">Integer value that sets the maximum number of characters allowed for the work PIN.</span></span> <span data-ttu-id="57e63-194">有效值为 4 到 127（含 4 和 127）并且大于或等于为最小 PIN 设置的值。</span><span class="sxs-lookup"><span data-stu-id="57e63-194">Valid values are 4 to 127 inclusive and greater than or equal to the value set for the minimum PIN.</span></span> <span data-ttu-id="57e63-195">有效值为 4 至 127</span><span class="sxs-lookup"><span data-stu-id="57e63-195">Valid values 4 to 127</span></span>|
|<span data-ttu-id="57e63-196">pinUppercaseCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="57e63-196">pinUppercaseCharactersUsage</span></span>|[<span data-ttu-id="57e63-197">configurationUsage</span><span class="sxs-lookup"><span data-stu-id="57e63-197">configurationUsage</span></span>](../resources/intune-deviceconfig-configurationusage.md)|<span data-ttu-id="57e63-198">此值配置 Windows Hello 企业 PIN 中的大写字符的使用。</span><span class="sxs-lookup"><span data-stu-id="57e63-198">This value configures the use of uppercase characters in the Windows Hello for Business PIN.</span></span> <span data-ttu-id="57e63-199">可取值为：`blocked`、`required`、`allowed`、`notConfigured`。</span><span class="sxs-lookup"><span data-stu-id="57e63-199">Possible values are: `blocked`, `required`, `allowed`, `notConfigured`.</span></span>|
|<span data-ttu-id="57e63-200">pinLowercaseCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="57e63-200">pinLowercaseCharactersUsage</span></span>|[<span data-ttu-id="57e63-201">configurationUsage</span><span class="sxs-lookup"><span data-stu-id="57e63-201">configurationUsage</span></span>](../resources/intune-deviceconfig-configurationusage.md)|<span data-ttu-id="57e63-202">此值配置 Windows Hello 企业 PIN 中的小写字符的使用。</span><span class="sxs-lookup"><span data-stu-id="57e63-202">This value configures the use of lowercase characters in the Windows Hello for Business PIN.</span></span> <span data-ttu-id="57e63-203">可取值为：`blocked`、`required`、`allowed`、`notConfigured`。</span><span class="sxs-lookup"><span data-stu-id="57e63-203">Possible values are: `blocked`, `required`, `allowed`, `notConfigured`.</span></span>|
|<span data-ttu-id="57e63-204">pinSpecialCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="57e63-204">pinSpecialCharactersUsage</span></span>|[<span data-ttu-id="57e63-205">configurationUsage</span><span class="sxs-lookup"><span data-stu-id="57e63-205">configurationUsage</span></span>](../resources/intune-deviceconfig-configurationusage.md)|<span data-ttu-id="57e63-206">控制在 Windows Hello 企业 PIN 中使用特殊字符的能力。</span><span class="sxs-lookup"><span data-stu-id="57e63-206">Controls the ability to use special characters in the Windows Hello for Business PIN.</span></span> <span data-ttu-id="57e63-207">可取值为：`blocked`、`required`、`allowed`、`notConfigured`。</span><span class="sxs-lookup"><span data-stu-id="57e63-207">Possible values are: `blocked`, `required`, `allowed`, `notConfigured`.</span></span>|
|<span data-ttu-id="57e63-208">pinExpirationInDays</span><span class="sxs-lookup"><span data-stu-id="57e63-208">pinExpirationInDays</span></span>|<span data-ttu-id="57e63-209">Int32</span><span class="sxs-lookup"><span data-stu-id="57e63-209">Int32</span></span>|<span data-ttu-id="57e63-210">Integer 值指定在系统 (PIN) 之前可以使用 PIN 的时间段（以天为单位）。</span><span class="sxs-lookup"><span data-stu-id="57e63-210">Integer value specifies the period (in days) that a PIN can be used before the system requires the user to change it.</span></span> <span data-ttu-id="57e63-211">有效值为 0 到 730（含 0 和 730）。</span><span class="sxs-lookup"><span data-stu-id="57e63-211">Valid values are 0 to 730 inclusive.</span></span> <span data-ttu-id="57e63-212">有效值为 0 至 730</span><span class="sxs-lookup"><span data-stu-id="57e63-212">Valid values 0 to 730</span></span>|
|<span data-ttu-id="57e63-213">pinPreviousBlockCount</span><span class="sxs-lookup"><span data-stu-id="57e63-213">pinPreviousBlockCount</span></span>|<span data-ttu-id="57e63-214">Int32</span><span class="sxs-lookup"><span data-stu-id="57e63-214">Int32</span></span>|<span data-ttu-id="57e63-215">控制阻止用户使用过去 PIN 的能力。</span><span class="sxs-lookup"><span data-stu-id="57e63-215">Controls the ability to prevent users from using past PINs.</span></span> <span data-ttu-id="57e63-216">必须将其设置为 0 到 50（含 0 和 50）之间，并且用户的当前 PIN 包含在该计数中。</span><span class="sxs-lookup"><span data-stu-id="57e63-216">This must be set between 0 and 50, inclusive, and the current PIN of the user is included in that count.</span></span> <span data-ttu-id="57e63-217">如果设置为 0，则不存储以前的 PIN。</span><span class="sxs-lookup"><span data-stu-id="57e63-217">If set to 0, previous PINs are not stored.</span></span> <span data-ttu-id="57e63-218">PIN 历史记录不会通过 PIN 重置保留。</span><span class="sxs-lookup"><span data-stu-id="57e63-218">PIN history is not preserved through a PIN reset.</span></span> <span data-ttu-id="57e63-219">有效值为 0 至 50</span><span class="sxs-lookup"><span data-stu-id="57e63-219">Valid values 0 to 50</span></span>|
|<span data-ttu-id="57e63-220">pinRecoveryEnabled</span><span class="sxs-lookup"><span data-stu-id="57e63-220">pinRecoveryEnabled</span></span>|<span data-ttu-id="57e63-221">Boolean</span><span class="sxs-lookup"><span data-stu-id="57e63-221">Boolean</span></span>|<span data-ttu-id="57e63-222">允许用户使用 Windows Hello 企业 PIN 恢复服务更改其 PIN 的布尔值。</span><span class="sxs-lookup"><span data-stu-id="57e63-222">Boolean value that enables a user to change their PIN by using the Windows Hello for Business PIN recovery service.</span></span>|
|<span data-ttu-id="57e63-223">securityDeviceRequired</span><span class="sxs-lookup"><span data-stu-id="57e63-223">securityDeviceRequired</span></span>|<span data-ttu-id="57e63-224">Boolean</span><span class="sxs-lookup"><span data-stu-id="57e63-224">Boolean</span></span>|<span data-ttu-id="57e63-225">控制是否需要受信任的平台模块 (TPM) 预配 Windows Hello 企业版本。</span><span class="sxs-lookup"><span data-stu-id="57e63-225">Controls whether to require a Trusted Platform Module (TPM) for provisioning Windows Hello for Business.</span></span> <span data-ttu-id="57e63-226">TPM 提供了额外的安全优势，因为存储在 TPM 上的数据不能用于其他设备。</span><span class="sxs-lookup"><span data-stu-id="57e63-226">A TPM provides an additional security benefit in that data stored on it cannot be used on other devices.</span></span> <span data-ttu-id="57e63-227">如果设置为 False，则所有设备都可以预配 Windows Hello 企业版本，即使没有可用 TPM。</span><span class="sxs-lookup"><span data-stu-id="57e63-227">If set to False, all devices can provision Windows Hello for Business even if there is not a usable TPM.</span></span>|
|<span data-ttu-id="57e63-228">unlockWithBiometricsEnabled</span><span class="sxs-lookup"><span data-stu-id="57e63-228">unlockWithBiometricsEnabled</span></span>|<span data-ttu-id="57e63-229">Boolean</span><span class="sxs-lookup"><span data-stu-id="57e63-229">Boolean</span></span>|<span data-ttu-id="57e63-230">控制将生物识别手势（如人脸和指纹）用作 Windows Hello 企业 PIN 的替代方法。</span><span class="sxs-lookup"><span data-stu-id="57e63-230">Controls the use of biometric gestures, such as face and fingerprint, as an alternative to the Windows Hello for Business PIN.</span></span>  <span data-ttu-id="57e63-231">如果设置为 False，则不允许生物识别手势。</span><span class="sxs-lookup"><span data-stu-id="57e63-231">If set to False, biometric gestures are not allowed.</span></span> <span data-ttu-id="57e63-232">用户仍必须将 PIN 配置为备份，以防发生故障。</span><span class="sxs-lookup"><span data-stu-id="57e63-232">Users must still configure a PIN as a backup in case of failures.</span></span>|
|<span data-ttu-id="57e63-233">useCertificatesForOnPremisesAuthEnabled</span><span class="sxs-lookup"><span data-stu-id="57e63-233">useCertificatesForOnPremisesAuthEnabled</span></span>|<span data-ttu-id="57e63-234">Boolean</span><span class="sxs-lookup"><span data-stu-id="57e63-234">Boolean</span></span>|<span data-ttu-id="57e63-235">使 Windows Hello 企业版本能够使用证书对本地资源进行身份验证的布尔值。</span><span class="sxs-lookup"><span data-stu-id="57e63-235">Boolean value that enables Windows Hello for Business to use certificates to authenticate on-premise resources.</span></span>|
|<span data-ttu-id="57e63-236">windowsHelloForBusinessBlocked</span><span class="sxs-lookup"><span data-stu-id="57e63-236">windowsHelloForBusinessBlocked</span></span>|<span data-ttu-id="57e63-237">Boolean</span><span class="sxs-lookup"><span data-stu-id="57e63-237">Boolean</span></span>|<span data-ttu-id="57e63-238">阻止将 Windows Hello 企业版本作为登录 Windows 的方法的布尔值。</span><span class="sxs-lookup"><span data-stu-id="57e63-238">Boolean value that blocks Windows Hello for Business as a method for signing into Windows.</span></span>|



## <a name="response"></a><span data-ttu-id="57e63-239">响应</span><span class="sxs-lookup"><span data-stu-id="57e63-239">Response</span></span>
<span data-ttu-id="57e63-240">如果成功，此方法在响应正文中返回 响应代码和 `201 Created` [windowsIdentityProtectionConfiguration](../resources/intune-deviceconfig-windowsidentityprotectionconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="57e63-240">If successful, this method returns a `201 Created` response code and a [windowsIdentityProtectionConfiguration](../resources/intune-deviceconfig-windowsidentityprotectionconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="57e63-241">示例</span><span class="sxs-lookup"><span data-stu-id="57e63-241">Example</span></span>

### <a name="request"></a><span data-ttu-id="57e63-242">请求</span><span class="sxs-lookup"><span data-stu-id="57e63-242">Request</span></span>
<span data-ttu-id="57e63-243">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="57e63-243">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1583

{
  "@odata.type": "#microsoft.graph.windowsIdentityProtectionConfiguration",
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
  "useSecurityKeyForSignin": true,
  "enhancedAntiSpoofingForFacialFeaturesEnabled": true,
  "pinMinimumLength": 0,
  "pinMaximumLength": 0,
  "pinUppercaseCharactersUsage": "required",
  "pinLowercaseCharactersUsage": "required",
  "pinSpecialCharactersUsage": "required",
  "pinExpirationInDays": 3,
  "pinPreviousBlockCount": 5,
  "pinRecoveryEnabled": true,
  "securityDeviceRequired": true,
  "unlockWithBiometricsEnabled": true,
  "useCertificatesForOnPremisesAuthEnabled": true,
  "windowsHelloForBusinessBlocked": true
}
```

### <a name="response"></a><span data-ttu-id="57e63-244">响应</span><span class="sxs-lookup"><span data-stu-id="57e63-244">Response</span></span>
<span data-ttu-id="57e63-p122">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="57e63-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1755

{
  "@odata.type": "#microsoft.graph.windowsIdentityProtectionConfiguration",
  "id": "b2e64303-4303-b2e6-0343-e6b20343e6b2",
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
  "useSecurityKeyForSignin": true,
  "enhancedAntiSpoofingForFacialFeaturesEnabled": true,
  "pinMinimumLength": 0,
  "pinMaximumLength": 0,
  "pinUppercaseCharactersUsage": "required",
  "pinLowercaseCharactersUsage": "required",
  "pinSpecialCharactersUsage": "required",
  "pinExpirationInDays": 3,
  "pinPreviousBlockCount": 5,
  "pinRecoveryEnabled": true,
  "securityDeviceRequired": true,
  "unlockWithBiometricsEnabled": true,
  "useCertificatesForOnPremisesAuthEnabled": true,
  "windowsHelloForBusinessBlocked": true
}
```




