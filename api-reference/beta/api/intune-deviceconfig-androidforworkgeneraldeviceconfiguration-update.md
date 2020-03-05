---
title: 更新 androidForWorkGeneralDeviceConfiguration
description: 更新 androidForWorkGeneralDeviceConfiguration 对象的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 284bd66619d6706923e6a141a64f31f4108abd0d
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42449892"
---
# <a name="update-androidforworkgeneraldeviceconfiguration"></a><span data-ttu-id="6dfa8-103">更新 androidForWorkGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="6dfa8-103">Update androidForWorkGeneralDeviceConfiguration</span></span>

<span data-ttu-id="6dfa8-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="6dfa8-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6dfa8-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="6dfa8-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6dfa8-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="6dfa8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6dfa8-107">更新[androidForWorkGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidforworkgeneraldeviceconfiguration.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="6dfa8-107">Update the properties of a [androidForWorkGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidforworkgeneraldeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6dfa8-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="6dfa8-108">Prerequisites</span></span>
<span data-ttu-id="6dfa8-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6dfa8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6dfa8-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="6dfa8-111">Permission type</span></span>|<span data-ttu-id="6dfa8-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="6dfa8-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6dfa8-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6dfa8-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6dfa8-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6dfa8-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="6dfa8-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6dfa8-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6dfa8-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="6dfa8-116">Not supported.</span></span>|
|<span data-ttu-id="6dfa8-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="6dfa8-117">Application</span></span>|<span data-ttu-id="6dfa8-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6dfa8-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6dfa8-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6dfa8-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="6dfa8-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="6dfa8-120">Request headers</span></span>
|<span data-ttu-id="6dfa8-121">标头</span><span class="sxs-lookup"><span data-stu-id="6dfa8-121">Header</span></span>|<span data-ttu-id="6dfa8-122">值</span><span class="sxs-lookup"><span data-stu-id="6dfa8-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6dfa8-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="6dfa8-123">Authorization</span></span>|<span data-ttu-id="6dfa8-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="6dfa8-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6dfa8-125">接受</span><span class="sxs-lookup"><span data-stu-id="6dfa8-125">Accept</span></span>|<span data-ttu-id="6dfa8-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6dfa8-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6dfa8-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="6dfa8-127">Request body</span></span>
<span data-ttu-id="6dfa8-128">在请求正文中，提供[androidForWorkGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidforworkgeneraldeviceconfiguration.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6dfa8-128">In the request body, supply a JSON representation for the [androidForWorkGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidforworkgeneraldeviceconfiguration.md) object.</span></span>

<span data-ttu-id="6dfa8-129">下表显示创建[androidForWorkGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidforworkgeneraldeviceconfiguration.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="6dfa8-129">The following table shows the properties that are required when you create the [androidForWorkGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidforworkgeneraldeviceconfiguration.md).</span></span>

|<span data-ttu-id="6dfa8-130">属性</span><span class="sxs-lookup"><span data-stu-id="6dfa8-130">Property</span></span>|<span data-ttu-id="6dfa8-131">类型</span><span class="sxs-lookup"><span data-stu-id="6dfa8-131">Type</span></span>|<span data-ttu-id="6dfa8-132">说明</span><span class="sxs-lookup"><span data-stu-id="6dfa8-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6dfa8-133">id</span><span class="sxs-lookup"><span data-stu-id="6dfa8-133">id</span></span>|<span data-ttu-id="6dfa8-134">字符串</span><span class="sxs-lookup"><span data-stu-id="6dfa8-134">String</span></span>|<span data-ttu-id="6dfa8-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="6dfa8-135">Key of the entity.</span></span> <span data-ttu-id="6dfa8-136">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6dfa8-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6dfa8-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6dfa8-137">lastModifiedDateTime</span></span>|<span data-ttu-id="6dfa8-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6dfa8-138">DateTimeOffset</span></span>|<span data-ttu-id="6dfa8-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="6dfa8-139">DateTime the object was last modified.</span></span> <span data-ttu-id="6dfa8-140">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6dfa8-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6dfa8-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="6dfa8-141">roleScopeTagIds</span></span>|<span data-ttu-id="6dfa8-142">String 集合</span><span class="sxs-lookup"><span data-stu-id="6dfa8-142">String collection</span></span>|<span data-ttu-id="6dfa8-143">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="6dfa8-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="6dfa8-144">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6dfa8-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6dfa8-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="6dfa8-145">supportsScopeTags</span></span>|<span data-ttu-id="6dfa8-146">布尔</span><span class="sxs-lookup"><span data-stu-id="6dfa8-146">Boolean</span></span>|<span data-ttu-id="6dfa8-147">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="6dfa8-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="6dfa8-148">如果此值为 false，则不允许分配给 ScopeTags 属性，并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="6dfa8-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="6dfa8-149">这适用于在 Silverlight 中创建的旧版策略，可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="6dfa8-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="6dfa8-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="6dfa8-150">This property is read-only.</span></span> <span data-ttu-id="6dfa8-151">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6dfa8-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6dfa8-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="6dfa8-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="6dfa8-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="6dfa8-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="6dfa8-154">适用于此策略的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="6dfa8-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="6dfa8-155">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6dfa8-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6dfa8-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="6dfa8-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="6dfa8-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="6dfa8-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="6dfa8-158">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="6dfa8-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="6dfa8-159">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6dfa8-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6dfa8-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="6dfa8-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="6dfa8-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="6dfa8-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="6dfa8-162">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="6dfa8-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="6dfa8-163">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6dfa8-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6dfa8-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6dfa8-164">createdDateTime</span></span>|<span data-ttu-id="6dfa8-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6dfa8-165">DateTimeOffset</span></span>|<span data-ttu-id="6dfa8-166">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="6dfa8-166">DateTime the object was created.</span></span> <span data-ttu-id="6dfa8-167">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6dfa8-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6dfa8-168">说明</span><span class="sxs-lookup"><span data-stu-id="6dfa8-168">description</span></span>|<span data-ttu-id="6dfa8-169">String</span><span class="sxs-lookup"><span data-stu-id="6dfa8-169">String</span></span>|<span data-ttu-id="6dfa8-170">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="6dfa8-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="6dfa8-171">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6dfa8-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6dfa8-172">displayName</span><span class="sxs-lookup"><span data-stu-id="6dfa8-172">displayName</span></span>|<span data-ttu-id="6dfa8-173">String</span><span class="sxs-lookup"><span data-stu-id="6dfa8-173">String</span></span>|<span data-ttu-id="6dfa8-174">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="6dfa8-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="6dfa8-175">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6dfa8-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6dfa8-176">version</span><span class="sxs-lookup"><span data-stu-id="6dfa8-176">version</span></span>|<span data-ttu-id="6dfa8-177">Int32</span><span class="sxs-lookup"><span data-stu-id="6dfa8-177">Int32</span></span>|<span data-ttu-id="6dfa8-178">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="6dfa8-178">Version of the device configuration.</span></span> <span data-ttu-id="6dfa8-179">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6dfa8-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6dfa8-180">passwordBlockFingerprintUnlock</span><span class="sxs-lookup"><span data-stu-id="6dfa8-180">passwordBlockFingerprintUnlock</span></span>|<span data-ttu-id="6dfa8-181">布尔</span><span class="sxs-lookup"><span data-stu-id="6dfa8-181">Boolean</span></span>|<span data-ttu-id="6dfa8-182">指示是否阻止指纹解锁。</span><span class="sxs-lookup"><span data-stu-id="6dfa8-182">Indicates whether or not to block fingerprint unlock.</span></span>|
|<span data-ttu-id="6dfa8-183">passwordBlockTrustAgents</span><span class="sxs-lookup"><span data-stu-id="6dfa8-183">passwordBlockTrustAgents</span></span>|<span data-ttu-id="6dfa8-184">Boolean</span><span class="sxs-lookup"><span data-stu-id="6dfa8-184">Boolean</span></span>|<span data-ttu-id="6dfa8-185">指示是否阻止 Smart Lock 和其他信任代理。</span><span class="sxs-lookup"><span data-stu-id="6dfa8-185">Indicates whether or not to block Smart Lock and other trust agents.</span></span>|
|<span data-ttu-id="6dfa8-186">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="6dfa8-186">passwordExpirationDays</span></span>|<span data-ttu-id="6dfa8-187">Int32</span><span class="sxs-lookup"><span data-stu-id="6dfa8-187">Int32</span></span>|<span data-ttu-id="6dfa8-188">密码过期前的天数。</span><span class="sxs-lookup"><span data-stu-id="6dfa8-188">Number of days before the password expires.</span></span> <span data-ttu-id="6dfa8-189">有效值为 1 至 365。</span><span class="sxs-lookup"><span data-stu-id="6dfa8-189">Valid values 1 to 365</span></span>|
|<span data-ttu-id="6dfa8-190">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="6dfa8-190">passwordMinimumLength</span></span>|<span data-ttu-id="6dfa8-191">Int32</span><span class="sxs-lookup"><span data-stu-id="6dfa8-191">Int32</span></span>|<span data-ttu-id="6dfa8-192">密码的最小长度。</span><span class="sxs-lookup"><span data-stu-id="6dfa8-192">Minimum length of passwords.</span></span> <span data-ttu-id="6dfa8-193">有效值为 4 至 16</span><span class="sxs-lookup"><span data-stu-id="6dfa8-193">Valid values 4 to 16</span></span>|
|<span data-ttu-id="6dfa8-194">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="6dfa8-194">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="6dfa8-195">Int32</span><span class="sxs-lookup"><span data-stu-id="6dfa8-195">Int32</span></span>|<span data-ttu-id="6dfa8-196">屏幕超时之前的不活动分钟数。</span><span class="sxs-lookup"><span data-stu-id="6dfa8-196">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="6dfa8-197">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="6dfa8-197">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="6dfa8-198">Int32</span><span class="sxs-lookup"><span data-stu-id="6dfa8-198">Int32</span></span>|<span data-ttu-id="6dfa8-199">要阻止的以前密码的数量。</span><span class="sxs-lookup"><span data-stu-id="6dfa8-199">Number of previous passwords to block.</span></span> <span data-ttu-id="6dfa8-200">有效值为 0 至 24</span><span class="sxs-lookup"><span data-stu-id="6dfa8-200">Valid values 0 to 24</span></span>|
|<span data-ttu-id="6dfa8-201">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="6dfa8-201">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="6dfa8-202">Int32</span><span class="sxs-lookup"><span data-stu-id="6dfa8-202">Int32</span></span>|<span data-ttu-id="6dfa8-203">恢复出厂设置之前允许登录失败的次数。</span><span class="sxs-lookup"><span data-stu-id="6dfa8-203">Number of sign in failures allowed before factory reset.</span></span> <span data-ttu-id="6dfa8-204">有效值为1至16</span><span class="sxs-lookup"><span data-stu-id="6dfa8-204">Valid values 1 to 16</span></span>|
|<span data-ttu-id="6dfa8-205">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="6dfa8-205">passwordRequiredType</span></span>|[<span data-ttu-id="6dfa8-206">androidForWorkRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="6dfa8-206">androidForWorkRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androidforworkrequiredpasswordtype.md)|<span data-ttu-id="6dfa8-207">必需的密码类型。</span><span class="sxs-lookup"><span data-stu-id="6dfa8-207">Type of password that is required.</span></span> <span data-ttu-id="6dfa8-208">可取值为：`deviceDefault`、`lowSecurityBiometric`、`required`、`atLeastNumeric`、`numericComplex`、`atLeastAlphabetic`、`atLeastAlphanumeric`、`alphanumericWithSymbols`。</span><span class="sxs-lookup"><span data-stu-id="6dfa8-208">Possible values are: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric`, `alphanumericWithSymbols`.</span></span>|
|<span data-ttu-id="6dfa8-209">workProfileDataSharingType</span><span class="sxs-lookup"><span data-stu-id="6dfa8-209">workProfileDataSharingType</span></span>|[<span data-ttu-id="6dfa8-210">androidForWorkCrossProfileDataSharingType</span><span class="sxs-lookup"><span data-stu-id="6dfa8-210">androidForWorkCrossProfileDataSharingType</span></span>](../resources/intune-deviceconfig-androidforworkcrossprofiledatasharingtype.md)|<span data-ttu-id="6dfa8-211">允许的数据共享类型。</span><span class="sxs-lookup"><span data-stu-id="6dfa8-211">Type of data sharing that is allowed.</span></span> <span data-ttu-id="6dfa8-212">可取值为：`deviceDefault`、`preventAny`、`allowPersonalToWork`、`noRestrictions`。</span><span class="sxs-lookup"><span data-stu-id="6dfa8-212">Possible values are: `deviceDefault`, `preventAny`, `allowPersonalToWork`, `noRestrictions`.</span></span>|
|<span data-ttu-id="6dfa8-213">workProfileBlockNotificationsWhileDeviceLocked</span><span class="sxs-lookup"><span data-stu-id="6dfa8-213">workProfileBlockNotificationsWhileDeviceLocked</span></span>|<span data-ttu-id="6dfa8-214">布尔</span><span class="sxs-lookup"><span data-stu-id="6dfa8-214">Boolean</span></span>|<span data-ttu-id="6dfa8-215">指示在设备锁定时是否阻止通知。</span><span class="sxs-lookup"><span data-stu-id="6dfa8-215">Indicates whether or not to block notifications while device locked.</span></span>|
|<span data-ttu-id="6dfa8-216">workProfileBlockAddingAccounts</span><span class="sxs-lookup"><span data-stu-id="6dfa8-216">workProfileBlockAddingAccounts</span></span>|<span data-ttu-id="6dfa8-217">布尔</span><span class="sxs-lookup"><span data-stu-id="6dfa8-217">Boolean</span></span>|<span data-ttu-id="6dfa8-218">阻止用户在工作配置文件中添加/删除帐户。</span><span class="sxs-lookup"><span data-stu-id="6dfa8-218">Block users from adding/removing accounts in work profile.</span></span>|
|<span data-ttu-id="6dfa8-219">workProfileBluetoothEnableContactSharing</span><span class="sxs-lookup"><span data-stu-id="6dfa8-219">workProfileBluetoothEnableContactSharing</span></span>|<span data-ttu-id="6dfa8-220">布尔</span><span class="sxs-lookup"><span data-stu-id="6dfa8-220">Boolean</span></span>|<span data-ttu-id="6dfa8-221">允许蓝牙设备访问企业联系人。</span><span class="sxs-lookup"><span data-stu-id="6dfa8-221">Allow bluetooth devices to access enterprise contacts.</span></span>|
|<span data-ttu-id="6dfa8-222">workProfileBlockScreenCapture</span><span class="sxs-lookup"><span data-stu-id="6dfa8-222">workProfileBlockScreenCapture</span></span>|<span data-ttu-id="6dfa8-223">布尔</span><span class="sxs-lookup"><span data-stu-id="6dfa8-223">Boolean</span></span>|<span data-ttu-id="6dfa8-224">在工作配置文件中阻止屏幕捕获。</span><span class="sxs-lookup"><span data-stu-id="6dfa8-224">Block screen capture in work profile.</span></span>|
|<span data-ttu-id="6dfa8-225">workProfileBlockCrossProfileCallerId</span><span class="sxs-lookup"><span data-stu-id="6dfa8-225">workProfileBlockCrossProfileCallerId</span></span>|<span data-ttu-id="6dfa8-226">布尔</span><span class="sxs-lookup"><span data-stu-id="6dfa8-226">Boolean</span></span>|<span data-ttu-id="6dfa8-227">阻止显示个人配置文件中的工作配置文件呼叫者 ID。</span><span class="sxs-lookup"><span data-stu-id="6dfa8-227">Block display work profile caller ID in personal profile.</span></span>|
|<span data-ttu-id="6dfa8-228">workProfileBlockCamera</span><span class="sxs-lookup"><span data-stu-id="6dfa8-228">workProfileBlockCamera</span></span>|<span data-ttu-id="6dfa8-229">布尔</span><span class="sxs-lookup"><span data-stu-id="6dfa8-229">Boolean</span></span>|<span data-ttu-id="6dfa8-230">阻止工作配置文件相机。</span><span class="sxs-lookup"><span data-stu-id="6dfa8-230">Block work profile camera.</span></span>|
|<span data-ttu-id="6dfa8-231">workProfileBlockCrossProfileContactsSearch</span><span class="sxs-lookup"><span data-stu-id="6dfa8-231">workProfileBlockCrossProfileContactsSearch</span></span>|<span data-ttu-id="6dfa8-232">布尔</span><span class="sxs-lookup"><span data-stu-id="6dfa8-232">Boolean</span></span>|<span data-ttu-id="6dfa8-233">阻止个人配置文件中的工作配置文件联系人可用性。</span><span class="sxs-lookup"><span data-stu-id="6dfa8-233">Block work profile contacts availability in personal profile.</span></span>|
|<span data-ttu-id="6dfa8-234">workProfileBlockCrossProfileCopyPaste</span><span class="sxs-lookup"><span data-stu-id="6dfa8-234">workProfileBlockCrossProfileCopyPaste</span></span>|<span data-ttu-id="6dfa8-235">布尔</span><span class="sxs-lookup"><span data-stu-id="6dfa8-235">Boolean</span></span>|<span data-ttu-id="6dfa8-236">指示是否启用 "禁用跨配置文件复制/粘贴" 设置的 Boolean。</span><span class="sxs-lookup"><span data-stu-id="6dfa8-236">Boolean that indicates if the setting disallow cross profile copy/paste is enabled.</span></span>|
|<span data-ttu-id="6dfa8-237">workProfileDefaultAppPermissionPolicy</span><span class="sxs-lookup"><span data-stu-id="6dfa8-237">workProfileDefaultAppPermissionPolicy</span></span>|[<span data-ttu-id="6dfa8-238">androidForWorkDefaultAppPermissionPolicyType</span><span class="sxs-lookup"><span data-stu-id="6dfa8-238">androidForWorkDefaultAppPermissionPolicyType</span></span>](../resources/intune-deviceconfig-androidforworkdefaultapppermissionpolicytype.md)|<span data-ttu-id="6dfa8-239">必需的密码类型。</span><span class="sxs-lookup"><span data-stu-id="6dfa8-239">Type of password that is required.</span></span> <span data-ttu-id="6dfa8-240">可取值为：`deviceDefault`、`prompt`、`autoGrant`、`autoDeny`。</span><span class="sxs-lookup"><span data-stu-id="6dfa8-240">Possible values are: `deviceDefault`, `prompt`, `autoGrant`, `autoDeny`.</span></span>|
|<span data-ttu-id="6dfa8-241">workProfilePasswordBlockFingerprintUnlock</span><span class="sxs-lookup"><span data-stu-id="6dfa8-241">workProfilePasswordBlockFingerprintUnlock</span></span>|<span data-ttu-id="6dfa8-242">布尔</span><span class="sxs-lookup"><span data-stu-id="6dfa8-242">Boolean</span></span>|<span data-ttu-id="6dfa8-243">指示是否阻止工作配置文件的指纹解锁。</span><span class="sxs-lookup"><span data-stu-id="6dfa8-243">Indicates whether or not to block fingerprint unlock for work profile.</span></span>|
|<span data-ttu-id="6dfa8-244">workProfilePasswordBlockTrustAgents</span><span class="sxs-lookup"><span data-stu-id="6dfa8-244">workProfilePasswordBlockTrustAgents</span></span>|<span data-ttu-id="6dfa8-245">布尔</span><span class="sxs-lookup"><span data-stu-id="6dfa8-245">Boolean</span></span>|<span data-ttu-id="6dfa8-246">指示是否阻止智能锁定和其他信任代理用于工作配置文件。</span><span class="sxs-lookup"><span data-stu-id="6dfa8-246">Indicates whether or not to block Smart Lock and other trust agents for work profile.</span></span>|
|<span data-ttu-id="6dfa8-247">workProfilePasswordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="6dfa8-247">workProfilePasswordExpirationDays</span></span>|<span data-ttu-id="6dfa8-248">Int32</span><span class="sxs-lookup"><span data-stu-id="6dfa8-248">Int32</span></span>|<span data-ttu-id="6dfa8-249">工作配置文件密码到期前的天数。</span><span class="sxs-lookup"><span data-stu-id="6dfa8-249">Number of days before the work profile password expires.</span></span> <span data-ttu-id="6dfa8-250">有效值为 1 至 365。</span><span class="sxs-lookup"><span data-stu-id="6dfa8-250">Valid values 1 to 365</span></span>|
|<span data-ttu-id="6dfa8-251">workProfilePasswordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="6dfa8-251">workProfilePasswordMinimumLength</span></span>|<span data-ttu-id="6dfa8-252">Int32</span><span class="sxs-lookup"><span data-stu-id="6dfa8-252">Int32</span></span>|<span data-ttu-id="6dfa8-253">工作配置文件密码的最小长度。</span><span class="sxs-lookup"><span data-stu-id="6dfa8-253">Minimum length of work profile password.</span></span> <span data-ttu-id="6dfa8-254">有效值为 4 至 16</span><span class="sxs-lookup"><span data-stu-id="6dfa8-254">Valid values 4 to 16</span></span>|
|<span data-ttu-id="6dfa8-255">workProfilePasswordMinNumericCharacters</span><span class="sxs-lookup"><span data-stu-id="6dfa8-255">workProfilePasswordMinNumericCharacters</span></span>|<span data-ttu-id="6dfa8-256">Int32</span><span class="sxs-lookup"><span data-stu-id="6dfa8-256">Int32</span></span>|<span data-ttu-id="6dfa8-257">工作配置文件密码中所需的最小数字字符数。</span><span class="sxs-lookup"><span data-stu-id="6dfa8-257">Minimum # of numeric characters required in work profile password.</span></span> <span data-ttu-id="6dfa8-258">有效值为1至10</span><span class="sxs-lookup"><span data-stu-id="6dfa8-258">Valid values 1 to 10</span></span>|
|<span data-ttu-id="6dfa8-259">workProfilePasswordMinNonLetterCharacters</span><span class="sxs-lookup"><span data-stu-id="6dfa8-259">workProfilePasswordMinNonLetterCharacters</span></span>|<span data-ttu-id="6dfa8-260">Int32</span><span class="sxs-lookup"><span data-stu-id="6dfa8-260">Int32</span></span>|<span data-ttu-id="6dfa8-261">工作配置文件密码中所需的最小非字母字符数。</span><span class="sxs-lookup"><span data-stu-id="6dfa8-261">Minimum # of non-letter characters required in work profile password.</span></span> <span data-ttu-id="6dfa8-262">有效值为1至10</span><span class="sxs-lookup"><span data-stu-id="6dfa8-262">Valid values 1 to 10</span></span>|
|<span data-ttu-id="6dfa8-263">workProfilePasswordMinLetterCharacters</span><span class="sxs-lookup"><span data-stu-id="6dfa8-263">workProfilePasswordMinLetterCharacters</span></span>|<span data-ttu-id="6dfa8-264">Int32</span><span class="sxs-lookup"><span data-stu-id="6dfa8-264">Int32</span></span>|<span data-ttu-id="6dfa8-265">工作配置文件密码中所需的字母字符的最小数目。</span><span class="sxs-lookup"><span data-stu-id="6dfa8-265">Minimum # of letter characters required in work profile password.</span></span> <span data-ttu-id="6dfa8-266">有效值为1至10</span><span class="sxs-lookup"><span data-stu-id="6dfa8-266">Valid values 1 to 10</span></span>|
|<span data-ttu-id="6dfa8-267">workProfilePasswordMinLowerCaseCharacters</span><span class="sxs-lookup"><span data-stu-id="6dfa8-267">workProfilePasswordMinLowerCaseCharacters</span></span>|<span data-ttu-id="6dfa8-268">Int32</span><span class="sxs-lookup"><span data-stu-id="6dfa8-268">Int32</span></span>|<span data-ttu-id="6dfa8-269">工作配置文件密码中所需的小写字符的最小数量。</span><span class="sxs-lookup"><span data-stu-id="6dfa8-269">Minimum # of lower-case characters required in work profile password.</span></span> <span data-ttu-id="6dfa8-270">有效值为1至10</span><span class="sxs-lookup"><span data-stu-id="6dfa8-270">Valid values 1 to 10</span></span>|
|<span data-ttu-id="6dfa8-271">workProfilePasswordMinUpperCaseCharacters</span><span class="sxs-lookup"><span data-stu-id="6dfa8-271">workProfilePasswordMinUpperCaseCharacters</span></span>|<span data-ttu-id="6dfa8-272">Int32</span><span class="sxs-lookup"><span data-stu-id="6dfa8-272">Int32</span></span>|<span data-ttu-id="6dfa8-273">工作配置文件密码中要求的大写字符的最小数量。</span><span class="sxs-lookup"><span data-stu-id="6dfa8-273">Minimum # of upper-case characters required in work profile password.</span></span> <span data-ttu-id="6dfa8-274">有效值为1至10</span><span class="sxs-lookup"><span data-stu-id="6dfa8-274">Valid values 1 to 10</span></span>|
|<span data-ttu-id="6dfa8-275">workProfilePasswordMinSymbolCharacters</span><span class="sxs-lookup"><span data-stu-id="6dfa8-275">workProfilePasswordMinSymbolCharacters</span></span>|<span data-ttu-id="6dfa8-276">Int32</span><span class="sxs-lookup"><span data-stu-id="6dfa8-276">Int32</span></span>|<span data-ttu-id="6dfa8-277">工作配置文件密码中所需的最小符号数。</span><span class="sxs-lookup"><span data-stu-id="6dfa8-277">Minimum # of symbols required in work profile password.</span></span> <span data-ttu-id="6dfa8-278">有效值为1至10</span><span class="sxs-lookup"><span data-stu-id="6dfa8-278">Valid values 1 to 10</span></span>|
|<span data-ttu-id="6dfa8-279">workProfilePasswordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="6dfa8-279">workProfilePasswordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="6dfa8-280">Int32</span><span class="sxs-lookup"><span data-stu-id="6dfa8-280">Int32</span></span>|<span data-ttu-id="6dfa8-281">屏幕超时之前的不活动分钟数。</span><span class="sxs-lookup"><span data-stu-id="6dfa8-281">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="6dfa8-282">workProfilePasswordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="6dfa8-282">workProfilePasswordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="6dfa8-283">Int32</span><span class="sxs-lookup"><span data-stu-id="6dfa8-283">Int32</span></span>|<span data-ttu-id="6dfa8-284">要阻止的以前的工作配置文件密码的数量。</span><span class="sxs-lookup"><span data-stu-id="6dfa8-284">Number of previous work profile passwords to block.</span></span> <span data-ttu-id="6dfa8-285">有效值为 0 至 24</span><span class="sxs-lookup"><span data-stu-id="6dfa8-285">Valid values 0 to 24</span></span>|
|<span data-ttu-id="6dfa8-286">workProfilePasswordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="6dfa8-286">workProfilePasswordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="6dfa8-287">Int32</span><span class="sxs-lookup"><span data-stu-id="6dfa8-287">Int32</span></span>|<span data-ttu-id="6dfa8-288">在删除工作配置文件和删除所有公司数据之前允许的登录失败次数。</span><span class="sxs-lookup"><span data-stu-id="6dfa8-288">Number of sign in failures allowed before work profile is removed and all corporate data deleted.</span></span> <span data-ttu-id="6dfa8-289">有效值为1至16</span><span class="sxs-lookup"><span data-stu-id="6dfa8-289">Valid values 1 to 16</span></span>|
|<span data-ttu-id="6dfa8-290">workProfilePasswordRequiredType</span><span class="sxs-lookup"><span data-stu-id="6dfa8-290">workProfilePasswordRequiredType</span></span>|[<span data-ttu-id="6dfa8-291">androidForWorkRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="6dfa8-291">androidForWorkRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androidforworkrequiredpasswordtype.md)|<span data-ttu-id="6dfa8-292">所需的工作配置文件密码类型。</span><span class="sxs-lookup"><span data-stu-id="6dfa8-292">Type of work profile password that is required.</span></span> <span data-ttu-id="6dfa8-293">可取值为：`deviceDefault`、`lowSecurityBiometric`、`required`、`atLeastNumeric`、`numericComplex`、`atLeastAlphabetic`、`atLeastAlphanumeric`、`alphanumericWithSymbols`。</span><span class="sxs-lookup"><span data-stu-id="6dfa8-293">Possible values are: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric`, `alphanumericWithSymbols`.</span></span>|
|<span data-ttu-id="6dfa8-294">workProfileRequirePassword</span><span class="sxs-lookup"><span data-stu-id="6dfa8-294">workProfileRequirePassword</span></span>|<span data-ttu-id="6dfa8-295">布尔</span><span class="sxs-lookup"><span data-stu-id="6dfa8-295">Boolean</span></span>|<span data-ttu-id="6dfa8-296">对于工作配置文件，密码是必需的</span><span class="sxs-lookup"><span data-stu-id="6dfa8-296">Password is required or not for work profile</span></span>|
|<span data-ttu-id="6dfa8-297">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="6dfa8-297">securityRequireVerifyApps</span></span>|<span data-ttu-id="6dfa8-298">Boolean</span><span class="sxs-lookup"><span data-stu-id="6dfa8-298">Boolean</span></span>|<span data-ttu-id="6dfa8-299">要求启用 Android 验证应用功能。</span><span class="sxs-lookup"><span data-stu-id="6dfa8-299">Require the Android Verify apps feature is turned on.</span></span>|
|<span data-ttu-id="6dfa8-300">vpnAlwaysOnPackageIdentifier</span><span class="sxs-lookup"><span data-stu-id="6dfa8-300">vpnAlwaysOnPackageIdentifier</span></span>|<span data-ttu-id="6dfa8-301">String</span><span class="sxs-lookup"><span data-stu-id="6dfa8-301">String</span></span>|<span data-ttu-id="6dfa8-302">为 always on VPN 启用锁定模式。</span><span class="sxs-lookup"><span data-stu-id="6dfa8-302">Enable lockdown mode for always-on VPN.</span></span>|
|<span data-ttu-id="6dfa8-303">vpnEnableAlwaysOnLockdownMode</span><span class="sxs-lookup"><span data-stu-id="6dfa8-303">vpnEnableAlwaysOnLockdownMode</span></span>|<span data-ttu-id="6dfa8-304">布尔</span><span class="sxs-lookup"><span data-stu-id="6dfa8-304">Boolean</span></span>|<span data-ttu-id="6dfa8-305">为 always on VPN 启用锁定模式。</span><span class="sxs-lookup"><span data-stu-id="6dfa8-305">Enable lockdown mode for always-on VPN.</span></span>|
|<span data-ttu-id="6dfa8-306">workProfileAllowWidgets</span><span class="sxs-lookup"><span data-stu-id="6dfa8-306">workProfileAllowWidgets</span></span>|<span data-ttu-id="6dfa8-307">布尔</span><span class="sxs-lookup"><span data-stu-id="6dfa8-307">Boolean</span></span>|<span data-ttu-id="6dfa8-308">允许来自工作配置文件应用程序的小部件。</span><span class="sxs-lookup"><span data-stu-id="6dfa8-308">Allow widgets from work profile apps.</span></span>|
|<span data-ttu-id="6dfa8-309">workProfileBlockPersonalAppInstallsFromUnknownSources</span><span class="sxs-lookup"><span data-stu-id="6dfa8-309">workProfileBlockPersonalAppInstallsFromUnknownSources</span></span>|<span data-ttu-id="6dfa8-310">布尔</span><span class="sxs-lookup"><span data-stu-id="6dfa8-310">Boolean</span></span>|<span data-ttu-id="6dfa8-311">阻止从个人配置文件中的未知源进行应用程序安装。</span><span class="sxs-lookup"><span data-stu-id="6dfa8-311">Prevent app installations from unknown sources in the personal profile.</span></span>|



## <a name="response"></a><span data-ttu-id="6dfa8-312">响应</span><span class="sxs-lookup"><span data-stu-id="6dfa8-312">Response</span></span>
<span data-ttu-id="6dfa8-313">如果成功，此方法在响应`200 OK`正文中返回响应代码和更新的[androidForWorkGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidforworkgeneraldeviceconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="6dfa8-313">If successful, this method returns a `200 OK` response code and an updated [androidForWorkGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidforworkgeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6dfa8-314">示例</span><span class="sxs-lookup"><span data-stu-id="6dfa8-314">Example</span></span>

### <a name="request"></a><span data-ttu-id="6dfa8-315">请求</span><span class="sxs-lookup"><span data-stu-id="6dfa8-315">Request</span></span>
<span data-ttu-id="6dfa8-316">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="6dfa8-316">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 2913

{
  "@odata.type": "#microsoft.graph.androidForWorkGeneralDeviceConfiguration",
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
  "passwordBlockFingerprintUnlock": true,
  "passwordBlockTrustAgents": true,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
  "passwordPreviousPasswordBlockCount": 2,
  "passwordSignInFailureCountBeforeFactoryReset": 12,
  "passwordRequiredType": "lowSecurityBiometric",
  "workProfileDataSharingType": "preventAny",
  "workProfileBlockNotificationsWhileDeviceLocked": true,
  "workProfileBlockAddingAccounts": true,
  "workProfileBluetoothEnableContactSharing": true,
  "workProfileBlockScreenCapture": true,
  "workProfileBlockCrossProfileCallerId": true,
  "workProfileBlockCamera": true,
  "workProfileBlockCrossProfileContactsSearch": true,
  "workProfileBlockCrossProfileCopyPaste": true,
  "workProfileDefaultAppPermissionPolicy": "prompt",
  "workProfilePasswordBlockFingerprintUnlock": true,
  "workProfilePasswordBlockTrustAgents": true,
  "workProfilePasswordExpirationDays": 1,
  "workProfilePasswordMinimumLength": 0,
  "workProfilePasswordMinNumericCharacters": 7,
  "workProfilePasswordMinNonLetterCharacters": 9,
  "workProfilePasswordMinLetterCharacters": 6,
  "workProfilePasswordMinLowerCaseCharacters": 9,
  "workProfilePasswordMinUpperCaseCharacters": 9,
  "workProfilePasswordMinSymbolCharacters": 6,
  "workProfilePasswordMinutesOfInactivityBeforeScreenTimeout": 9,
  "workProfilePasswordPreviousPasswordBlockCount": 13,
  "workProfilePasswordSignInFailureCountBeforeFactoryReset": 7,
  "workProfilePasswordRequiredType": "lowSecurityBiometric",
  "workProfileRequirePassword": true,
  "securityRequireVerifyApps": true,
  "vpnAlwaysOnPackageIdentifier": "Vpn Always On Package Identifier value",
  "vpnEnableAlwaysOnLockdownMode": true,
  "workProfileAllowWidgets": true,
  "workProfileBlockPersonalAppInstallsFromUnknownSources": true
}
```

### <a name="response"></a><span data-ttu-id="6dfa8-317">响应</span><span class="sxs-lookup"><span data-stu-id="6dfa8-317">Response</span></span>
<span data-ttu-id="6dfa8-p131">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="6dfa8-p131">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 3085

{
  "@odata.type": "#microsoft.graph.androidForWorkGeneralDeviceConfiguration",
  "id": "a931a366-a366-a931-66a3-31a966a331a9",
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
  "passwordBlockFingerprintUnlock": true,
  "passwordBlockTrustAgents": true,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
  "passwordPreviousPasswordBlockCount": 2,
  "passwordSignInFailureCountBeforeFactoryReset": 12,
  "passwordRequiredType": "lowSecurityBiometric",
  "workProfileDataSharingType": "preventAny",
  "workProfileBlockNotificationsWhileDeviceLocked": true,
  "workProfileBlockAddingAccounts": true,
  "workProfileBluetoothEnableContactSharing": true,
  "workProfileBlockScreenCapture": true,
  "workProfileBlockCrossProfileCallerId": true,
  "workProfileBlockCamera": true,
  "workProfileBlockCrossProfileContactsSearch": true,
  "workProfileBlockCrossProfileCopyPaste": true,
  "workProfileDefaultAppPermissionPolicy": "prompt",
  "workProfilePasswordBlockFingerprintUnlock": true,
  "workProfilePasswordBlockTrustAgents": true,
  "workProfilePasswordExpirationDays": 1,
  "workProfilePasswordMinimumLength": 0,
  "workProfilePasswordMinNumericCharacters": 7,
  "workProfilePasswordMinNonLetterCharacters": 9,
  "workProfilePasswordMinLetterCharacters": 6,
  "workProfilePasswordMinLowerCaseCharacters": 9,
  "workProfilePasswordMinUpperCaseCharacters": 9,
  "workProfilePasswordMinSymbolCharacters": 6,
  "workProfilePasswordMinutesOfInactivityBeforeScreenTimeout": 9,
  "workProfilePasswordPreviousPasswordBlockCount": 13,
  "workProfilePasswordSignInFailureCountBeforeFactoryReset": 7,
  "workProfilePasswordRequiredType": "lowSecurityBiometric",
  "workProfileRequirePassword": true,
  "securityRequireVerifyApps": true,
  "vpnAlwaysOnPackageIdentifier": "Vpn Always On Package Identifier value",
  "vpnEnableAlwaysOnLockdownMode": true,
  "workProfileAllowWidgets": true,
  "workProfileBlockPersonalAppInstallsFromUnknownSources": true
}
```





