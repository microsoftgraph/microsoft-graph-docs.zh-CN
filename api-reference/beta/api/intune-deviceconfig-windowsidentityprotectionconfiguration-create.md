---
title: 创建 windowsIdentityProtectionConfiguration
description: 创建新的 windowsIdentityProtectionConfiguration 对象。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 5c84107eeefef0d0233052f4bc5d5b10459581a3
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/10/2019
ms.locfileid: "39946782"
---
# <a name="create-windowsidentityprotectionconfiguration"></a><span data-ttu-id="1b240-103">创建 windowsIdentityProtectionConfiguration</span><span class="sxs-lookup"><span data-stu-id="1b240-103">Create windowsIdentityProtectionConfiguration</span></span>

> <span data-ttu-id="1b240-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="1b240-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1b240-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="1b240-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1b240-106">创建新的[windowsIdentityProtectionConfiguration](../resources/intune-deviceconfig-windowsidentityprotectionconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="1b240-106">Create a new [windowsIdentityProtectionConfiguration](../resources/intune-deviceconfig-windowsidentityprotectionconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1b240-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="1b240-107">Prerequisites</span></span>
<span data-ttu-id="1b240-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="1b240-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1b240-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="1b240-110">Permission type</span></span>|<span data-ttu-id="1b240-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="1b240-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1b240-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1b240-112">Delegated (work or school account)</span></span>|<span data-ttu-id="1b240-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1b240-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="1b240-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1b240-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1b240-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="1b240-115">Not supported.</span></span>|
|<span data-ttu-id="1b240-116">Application</span><span class="sxs-lookup"><span data-stu-id="1b240-116">Application</span></span>|<span data-ttu-id="1b240-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1b240-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1b240-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1b240-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="1b240-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="1b240-119">Request headers</span></span>
|<span data-ttu-id="1b240-120">标头</span><span class="sxs-lookup"><span data-stu-id="1b240-120">Header</span></span>|<span data-ttu-id="1b240-121">值</span><span class="sxs-lookup"><span data-stu-id="1b240-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1b240-122">授权</span><span class="sxs-lookup"><span data-stu-id="1b240-122">Authorization</span></span>|<span data-ttu-id="1b240-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="1b240-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1b240-124">接受</span><span class="sxs-lookup"><span data-stu-id="1b240-124">Accept</span></span>|<span data-ttu-id="1b240-125">application/json</span><span class="sxs-lookup"><span data-stu-id="1b240-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1b240-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="1b240-126">Request body</span></span>
<span data-ttu-id="1b240-127">在请求正文中，提供 windowsIdentityProtectionConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1b240-127">In the request body, supply a JSON representation for the windowsIdentityProtectionConfiguration object.</span></span>

<span data-ttu-id="1b240-128">下表显示创建 windowsIdentityProtectionConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="1b240-128">The following table shows the properties that are required when you create the windowsIdentityProtectionConfiguration.</span></span>

|<span data-ttu-id="1b240-129">属性</span><span class="sxs-lookup"><span data-stu-id="1b240-129">Property</span></span>|<span data-ttu-id="1b240-130">类型</span><span class="sxs-lookup"><span data-stu-id="1b240-130">Type</span></span>|<span data-ttu-id="1b240-131">说明</span><span class="sxs-lookup"><span data-stu-id="1b240-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1b240-132">id</span><span class="sxs-lookup"><span data-stu-id="1b240-132">id</span></span>|<span data-ttu-id="1b240-133">字符串</span><span class="sxs-lookup"><span data-stu-id="1b240-133">String</span></span>|<span data-ttu-id="1b240-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="1b240-134">Key of the entity.</span></span> <span data-ttu-id="1b240-135">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1b240-135">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1b240-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1b240-136">lastModifiedDateTime</span></span>|<span data-ttu-id="1b240-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1b240-137">DateTimeOffset</span></span>|<span data-ttu-id="1b240-138">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="1b240-138">DateTime the object was last modified.</span></span> <span data-ttu-id="1b240-139">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1b240-139">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1b240-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="1b240-140">roleScopeTagIds</span></span>|<span data-ttu-id="1b240-141">String collection</span><span class="sxs-lookup"><span data-stu-id="1b240-141">String collection</span></span>|<span data-ttu-id="1b240-142">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="1b240-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="1b240-143">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1b240-143">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1b240-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="1b240-144">supportsScopeTags</span></span>|<span data-ttu-id="1b240-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="1b240-145">Boolean</span></span>|<span data-ttu-id="1b240-146">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="1b240-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="1b240-147">如果此值为 false，则不允许分配给 ScopeTags 属性，并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="1b240-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="1b240-148">这适用于在 Silverlight 中创建的旧版策略，可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="1b240-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="1b240-149">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="1b240-149">This property is read-only.</span></span> <span data-ttu-id="1b240-150">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1b240-150">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1b240-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="1b240-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="1b240-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="1b240-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="1b240-153">适用于此策略的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="1b240-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="1b240-154">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1b240-154">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1b240-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="1b240-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="1b240-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="1b240-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="1b240-157">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="1b240-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="1b240-158">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1b240-158">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1b240-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="1b240-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="1b240-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="1b240-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="1b240-161">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="1b240-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="1b240-162">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1b240-162">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1b240-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1b240-163">createdDateTime</span></span>|<span data-ttu-id="1b240-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1b240-164">DateTimeOffset</span></span>|<span data-ttu-id="1b240-165">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="1b240-165">DateTime the object was created.</span></span> <span data-ttu-id="1b240-166">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1b240-166">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1b240-167">说明</span><span class="sxs-lookup"><span data-stu-id="1b240-167">description</span></span>|<span data-ttu-id="1b240-168">String</span><span class="sxs-lookup"><span data-stu-id="1b240-168">String</span></span>|<span data-ttu-id="1b240-169">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="1b240-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="1b240-170">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1b240-170">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1b240-171">displayName</span><span class="sxs-lookup"><span data-stu-id="1b240-171">displayName</span></span>|<span data-ttu-id="1b240-172">String</span><span class="sxs-lookup"><span data-stu-id="1b240-172">String</span></span>|<span data-ttu-id="1b240-173">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="1b240-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="1b240-174">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1b240-174">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1b240-175">version</span><span class="sxs-lookup"><span data-stu-id="1b240-175">version</span></span>|<span data-ttu-id="1b240-176">Int32</span><span class="sxs-lookup"><span data-stu-id="1b240-176">Int32</span></span>|<span data-ttu-id="1b240-177">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="1b240-177">Version of the device configuration.</span></span> <span data-ttu-id="1b240-178">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1b240-178">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1b240-179">useSecurityKeyForSignin</span><span class="sxs-lookup"><span data-stu-id="1b240-179">useSecurityKeyForSignin</span></span>|<span data-ttu-id="1b240-180">Boolean</span><span class="sxs-lookup"><span data-stu-id="1b240-180">Boolean</span></span>|<span data-ttu-id="1b240-181">用于将 Windows Hello 安全密钥启用为登录凭据的布尔值。</span><span class="sxs-lookup"><span data-stu-id="1b240-181">Boolean value used to enable the Windows Hello security key as a logon credential.</span></span>|
|<span data-ttu-id="1b240-182">enhancedAntiSpoofingForFacialFeaturesEnabled</span><span class="sxs-lookup"><span data-stu-id="1b240-182">enhancedAntiSpoofingForFacialFeaturesEnabled</span></span>|<span data-ttu-id="1b240-183">Boolean</span><span class="sxs-lookup"><span data-stu-id="1b240-183">Boolean</span></span>|<span data-ttu-id="1b240-184">用于在 Windows Hello 人脸身份验证中为面部功能识别启用增强型反欺骗的布尔值。</span><span class="sxs-lookup"><span data-stu-id="1b240-184">Boolean value used to enable enhanced anti-spoofing for facial feature recognition on Windows Hello face authentication.</span></span>|
|<span data-ttu-id="1b240-185">pinMinimumLength</span><span class="sxs-lookup"><span data-stu-id="1b240-185">pinMinimumLength</span></span>|<span data-ttu-id="1b240-186">Int32</span><span class="sxs-lookup"><span data-stu-id="1b240-186">Int32</span></span>|<span data-ttu-id="1b240-187">整数值，用于设置 Windows Hello 企业版 PIN 所需的最小字符数。</span><span class="sxs-lookup"><span data-stu-id="1b240-187">Integer value that sets the minimum number of characters required for the Windows Hello for Business PIN.</span></span> <span data-ttu-id="1b240-188">有效值为4到127，且小于或等于最大 PIN 的值集。</span><span class="sxs-lookup"><span data-stu-id="1b240-188">Valid values are 4 to 127 inclusive and less than or equal to the value set for the maximum PIN.</span></span> <span data-ttu-id="1b240-189">有效值为4至127</span><span class="sxs-lookup"><span data-stu-id="1b240-189">Valid values 4 to 127</span></span>|
|<span data-ttu-id="1b240-190">pinMaximumLength</span><span class="sxs-lookup"><span data-stu-id="1b240-190">pinMaximumLength</span></span>|<span data-ttu-id="1b240-191">Int32</span><span class="sxs-lookup"><span data-stu-id="1b240-191">Int32</span></span>|<span data-ttu-id="1b240-192">整数值，用于设置允许的工作 PIN 的最大字符数。</span><span class="sxs-lookup"><span data-stu-id="1b240-192">Integer value that sets the maximum number of characters allowed for the work PIN.</span></span> <span data-ttu-id="1b240-193">有效值为4到127，并大于或等于最小 PIN 的值集。</span><span class="sxs-lookup"><span data-stu-id="1b240-193">Valid values are 4 to 127 inclusive and greater than or equal to the value set for the minimum PIN.</span></span> <span data-ttu-id="1b240-194">有效值为4至127</span><span class="sxs-lookup"><span data-stu-id="1b240-194">Valid values 4 to 127</span></span>|
|<span data-ttu-id="1b240-195">pinUppercaseCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="1b240-195">pinUppercaseCharactersUsage</span></span>|[<span data-ttu-id="1b240-196">configurationUsage</span><span class="sxs-lookup"><span data-stu-id="1b240-196">configurationUsage</span></span>](../resources/intune-deviceconfig-configurationusage.md)|<span data-ttu-id="1b240-197">此值配置 Windows Hello 企业版 PIN 中的大写字符的使用。</span><span class="sxs-lookup"><span data-stu-id="1b240-197">This value configures the use of uppercase characters in the Windows Hello for Business PIN.</span></span> <span data-ttu-id="1b240-198">可取值为：`blocked`、`required`、`allowed`。</span><span class="sxs-lookup"><span data-stu-id="1b240-198">Possible values are: `blocked`, `required`, `allowed`.</span></span>|
|<span data-ttu-id="1b240-199">pinLowercaseCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="1b240-199">pinLowercaseCharactersUsage</span></span>|[<span data-ttu-id="1b240-200">configurationUsage</span><span class="sxs-lookup"><span data-stu-id="1b240-200">configurationUsage</span></span>](../resources/intune-deviceconfig-configurationusage.md)|<span data-ttu-id="1b240-201">此值配置 Windows Hello 企业版 PIN 中的小写字符的使用。</span><span class="sxs-lookup"><span data-stu-id="1b240-201">This value configures the use of lowercase characters in the Windows Hello for Business PIN.</span></span> <span data-ttu-id="1b240-202">可取值为：`blocked`、`required`、`allowed`。</span><span class="sxs-lookup"><span data-stu-id="1b240-202">Possible values are: `blocked`, `required`, `allowed`.</span></span>|
|<span data-ttu-id="1b240-203">pinSpecialCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="1b240-203">pinSpecialCharactersUsage</span></span>|[<span data-ttu-id="1b240-204">configurationUsage</span><span class="sxs-lookup"><span data-stu-id="1b240-204">configurationUsage</span></span>](../resources/intune-deviceconfig-configurationusage.md)|<span data-ttu-id="1b240-205">控制在 Windows Hello 企业版 PIN 中使用特殊字符的功能。</span><span class="sxs-lookup"><span data-stu-id="1b240-205">Controls the ability to use special characters in the Windows Hello for Business PIN.</span></span> <span data-ttu-id="1b240-206">可取值为：`blocked`、`required`、`allowed`。</span><span class="sxs-lookup"><span data-stu-id="1b240-206">Possible values are: `blocked`, `required`, `allowed`.</span></span>|
|<span data-ttu-id="1b240-207">pinExpirationInDays</span><span class="sxs-lookup"><span data-stu-id="1b240-207">pinExpirationInDays</span></span>|<span data-ttu-id="1b240-208">Int32</span><span class="sxs-lookup"><span data-stu-id="1b240-208">Int32</span></span>|<span data-ttu-id="1b240-209">Integer 值指定在系统要求用户更改 PIN 之前可以使用 PIN 的时间段（以天为单位）。</span><span class="sxs-lookup"><span data-stu-id="1b240-209">Integer value specifies the period (in days) that a PIN can be used before the system requires the user to change it.</span></span> <span data-ttu-id="1b240-210">有效值为0至730，含0到。</span><span class="sxs-lookup"><span data-stu-id="1b240-210">Valid values are 0 to 730 inclusive.</span></span> <span data-ttu-id="1b240-211">有效值为 0 至 730</span><span class="sxs-lookup"><span data-stu-id="1b240-211">Valid values 0 to 730</span></span>|
|<span data-ttu-id="1b240-212">pinPreviousBlockCount</span><span class="sxs-lookup"><span data-stu-id="1b240-212">pinPreviousBlockCount</span></span>|<span data-ttu-id="1b240-213">Int32</span><span class="sxs-lookup"><span data-stu-id="1b240-213">Int32</span></span>|<span data-ttu-id="1b240-214">控制阻止用户使用过去的 Pin 的功能。</span><span class="sxs-lookup"><span data-stu-id="1b240-214">Controls the ability to prevent users from using past PINs.</span></span> <span data-ttu-id="1b240-215">必须在0和50之间设置此值（包括这两个值），并且用户的当前 PIN 包含在该计数中。</span><span class="sxs-lookup"><span data-stu-id="1b240-215">This must be set between 0 and 50, inclusive, and the current PIN of the user is included in that count.</span></span> <span data-ttu-id="1b240-216">如果设置为0，则不存储以前的 Pin。</span><span class="sxs-lookup"><span data-stu-id="1b240-216">If set to 0, previous PINs are not stored.</span></span> <span data-ttu-id="1b240-217">PIN 历史记录不会通过 PIN 重置来保留。</span><span class="sxs-lookup"><span data-stu-id="1b240-217">PIN history is not preserved through a PIN reset.</span></span> <span data-ttu-id="1b240-218">有效值为 0 至 50</span><span class="sxs-lookup"><span data-stu-id="1b240-218">Valid values 0 to 50</span></span>|
|<span data-ttu-id="1b240-219">pinRecoveryEnabled</span><span class="sxs-lookup"><span data-stu-id="1b240-219">pinRecoveryEnabled</span></span>|<span data-ttu-id="1b240-220">Boolean</span><span class="sxs-lookup"><span data-stu-id="1b240-220">Boolean</span></span>|<span data-ttu-id="1b240-221">允许用户使用 Windows Hello 企业版 PIN 恢复服务更改其 PIN 的布尔值。</span><span class="sxs-lookup"><span data-stu-id="1b240-221">Boolean value that enables a user to change their PIN by using the Windows Hello for Business PIN recovery service.</span></span>|
|<span data-ttu-id="1b240-222">securityDeviceRequired</span><span class="sxs-lookup"><span data-stu-id="1b240-222">securityDeviceRequired</span></span>|<span data-ttu-id="1b240-223">Boolean</span><span class="sxs-lookup"><span data-stu-id="1b240-223">Boolean</span></span>|<span data-ttu-id="1b240-224">控制是否需要用于设置 Windows Hello 企业版的受信任的平台模块（TPM）。</span><span class="sxs-lookup"><span data-stu-id="1b240-224">Controls whether to require a Trusted Platform Module (TPM) for provisioning Windows Hello for Business.</span></span> <span data-ttu-id="1b240-225">TPM 在其他设备上不能使用存储在其上的数据带来额外的安全性优势。</span><span class="sxs-lookup"><span data-stu-id="1b240-225">A TPM provides an additional security benefit in that data stored on it cannot be used on other devices.</span></span> <span data-ttu-id="1b240-226">如果设置为 False，即使没有可用的 TPM，所有设备也可以预配 Windows Hello 企业版。</span><span class="sxs-lookup"><span data-stu-id="1b240-226">If set to False, all devices can provision Windows Hello for Business even if there is not a usable TPM.</span></span>|
|<span data-ttu-id="1b240-227">unlockWithBiometricsEnabled</span><span class="sxs-lookup"><span data-stu-id="1b240-227">unlockWithBiometricsEnabled</span></span>|<span data-ttu-id="1b240-228">Boolean</span><span class="sxs-lookup"><span data-stu-id="1b240-228">Boolean</span></span>|<span data-ttu-id="1b240-229">控制使用生物特征手势（如面孔和指纹）作为 Windows Hello 企业版 PIN 的替代方法。</span><span class="sxs-lookup"><span data-stu-id="1b240-229">Controls the use of biometric gestures, such as face and fingerprint, as an alternative to the Windows Hello for Business PIN.</span></span>  <span data-ttu-id="1b240-230">如果设置为 False，则不允许使用生物特征手势。</span><span class="sxs-lookup"><span data-stu-id="1b240-230">If set to False, biometric gestures are not allowed.</span></span> <span data-ttu-id="1b240-231">用户仍必须在发生故障时将 PIN 配置为备份。</span><span class="sxs-lookup"><span data-stu-id="1b240-231">Users must still configure a PIN as a backup in case of failures.</span></span>|
|<span data-ttu-id="1b240-232">useCertificatesForOnPremisesAuthEnabled</span><span class="sxs-lookup"><span data-stu-id="1b240-232">useCertificatesForOnPremisesAuthEnabled</span></span>|<span data-ttu-id="1b240-233">Boolean</span><span class="sxs-lookup"><span data-stu-id="1b240-233">Boolean</span></span>|<span data-ttu-id="1b240-234">使 Windows Hello 企业版能够使用证书对本地资源进行身份验证的布尔值。</span><span class="sxs-lookup"><span data-stu-id="1b240-234">Boolean value that enables Windows Hello for Business to use certificates to authenticate on-premise resources.</span></span>|
|<span data-ttu-id="1b240-235">windowsHelloForBusinessBlocked</span><span class="sxs-lookup"><span data-stu-id="1b240-235">windowsHelloForBusinessBlocked</span></span>|<span data-ttu-id="1b240-236">Boolean</span><span class="sxs-lookup"><span data-stu-id="1b240-236">Boolean</span></span>|<span data-ttu-id="1b240-237">一个布尔值，它将 Windows Hello 企业版作为登录 Windows 的方法来阻止。</span><span class="sxs-lookup"><span data-stu-id="1b240-237">Boolean value that blocks Windows Hello for Business as a method for signing into Windows.</span></span>|



## <a name="response"></a><span data-ttu-id="1b240-238">响应</span><span class="sxs-lookup"><span data-stu-id="1b240-238">Response</span></span>
<span data-ttu-id="1b240-239">如果成功，此方法在响应`201 Created`正文中返回响应代码和[windowsIdentityProtectionConfiguration](../resources/intune-deviceconfig-windowsidentityprotectionconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="1b240-239">If successful, this method returns a `201 Created` response code and a [windowsIdentityProtectionConfiguration](../resources/intune-deviceconfig-windowsidentityprotectionconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1b240-240">示例</span><span class="sxs-lookup"><span data-stu-id="1b240-240">Example</span></span>

### <a name="request"></a><span data-ttu-id="1b240-241">请求</span><span class="sxs-lookup"><span data-stu-id="1b240-241">Request</span></span>
<span data-ttu-id="1b240-242">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="1b240-242">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="1b240-243">响应</span><span class="sxs-lookup"><span data-stu-id="1b240-243">Response</span></span>
<span data-ttu-id="1b240-p122">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="1b240-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





