---
title: 更新 androidForWorkGeneralDeviceConfiguration
description: 更新 androidForWorkGeneralDeviceConfiguration 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 2cd7bd5071c38d3921707259bcfb4a434b4776ec
ms.sourcegitcommit: dc3bade0c096d5ce716d4bc07cd9c7cabb52477b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/18/2020
ms.locfileid: "46790873"
---
# <a name="update-androidforworkgeneraldeviceconfiguration"></a><span data-ttu-id="e01df-103">更新 androidForWorkGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="e01df-103">Update androidForWorkGeneralDeviceConfiguration</span></span>

<span data-ttu-id="e01df-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e01df-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e01df-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="e01df-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e01df-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="e01df-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e01df-107">更新 [androidForWorkGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidforworkgeneraldeviceconfiguration.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="e01df-107">Update the properties of a [androidForWorkGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidforworkgeneraldeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e01df-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="e01df-108">Prerequisites</span></span>
<span data-ttu-id="e01df-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e01df-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e01df-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="e01df-111">Permission type</span></span>|<span data-ttu-id="e01df-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="e01df-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e01df-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e01df-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e01df-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e01df-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="e01df-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e01df-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e01df-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="e01df-116">Not supported.</span></span>|
|<span data-ttu-id="e01df-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="e01df-117">Application</span></span>|<span data-ttu-id="e01df-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e01df-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e01df-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e01df-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="e01df-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="e01df-120">Request headers</span></span>
|<span data-ttu-id="e01df-121">标头</span><span class="sxs-lookup"><span data-stu-id="e01df-121">Header</span></span>|<span data-ttu-id="e01df-122">值</span><span class="sxs-lookup"><span data-stu-id="e01df-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e01df-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e01df-123">Authorization</span></span>|<span data-ttu-id="e01df-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="e01df-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e01df-125">接受</span><span class="sxs-lookup"><span data-stu-id="e01df-125">Accept</span></span>|<span data-ttu-id="e01df-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e01df-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e01df-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="e01df-127">Request body</span></span>
<span data-ttu-id="e01df-128">在请求正文中，提供 [androidForWorkGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidforworkgeneraldeviceconfiguration.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e01df-128">In the request body, supply a JSON representation for the [androidForWorkGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidforworkgeneraldeviceconfiguration.md) object.</span></span>

<span data-ttu-id="e01df-129">下表显示创建 [androidForWorkGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidforworkgeneraldeviceconfiguration.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="e01df-129">The following table shows the properties that are required when you create the [androidForWorkGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidforworkgeneraldeviceconfiguration.md).</span></span>

|<span data-ttu-id="e01df-130">属性</span><span class="sxs-lookup"><span data-stu-id="e01df-130">Property</span></span>|<span data-ttu-id="e01df-131">类型</span><span class="sxs-lookup"><span data-stu-id="e01df-131">Type</span></span>|<span data-ttu-id="e01df-132">说明</span><span class="sxs-lookup"><span data-stu-id="e01df-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e01df-133">id</span><span class="sxs-lookup"><span data-stu-id="e01df-133">id</span></span>|<span data-ttu-id="e01df-134">String</span><span class="sxs-lookup"><span data-stu-id="e01df-134">String</span></span>|<span data-ttu-id="e01df-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="e01df-135">Key of the entity.</span></span> <span data-ttu-id="e01df-136">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e01df-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e01df-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e01df-137">lastModifiedDateTime</span></span>|<span data-ttu-id="e01df-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e01df-138">DateTimeOffset</span></span>|<span data-ttu-id="e01df-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="e01df-139">DateTime the object was last modified.</span></span> <span data-ttu-id="e01df-140">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e01df-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e01df-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="e01df-141">roleScopeTagIds</span></span>|<span data-ttu-id="e01df-142">字符串集合</span><span class="sxs-lookup"><span data-stu-id="e01df-142">String collection</span></span>|<span data-ttu-id="e01df-143">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="e01df-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="e01df-144">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e01df-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e01df-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="e01df-145">supportsScopeTags</span></span>|<span data-ttu-id="e01df-146">布尔值</span><span class="sxs-lookup"><span data-stu-id="e01df-146">Boolean</span></span>|<span data-ttu-id="e01df-147">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="e01df-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="e01df-148">如果此值为 false，则不允许分配给 ScopeTags 属性，并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="e01df-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="e01df-149">这适用于在 Silverlight 中创建的旧版策略，可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="e01df-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="e01df-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="e01df-150">This property is read-only.</span></span> <span data-ttu-id="e01df-151">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e01df-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e01df-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="e01df-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="e01df-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="e01df-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="e01df-154">适用于此策略的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="e01df-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="e01df-155">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e01df-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e01df-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="e01df-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="e01df-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="e01df-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="e01df-158">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="e01df-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="e01df-159">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e01df-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e01df-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="e01df-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="e01df-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="e01df-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="e01df-162">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="e01df-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="e01df-163">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e01df-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e01df-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e01df-164">createdDateTime</span></span>|<span data-ttu-id="e01df-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e01df-165">DateTimeOffset</span></span>|<span data-ttu-id="e01df-166">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="e01df-166">DateTime the object was created.</span></span> <span data-ttu-id="e01df-167">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e01df-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e01df-168">description</span><span class="sxs-lookup"><span data-stu-id="e01df-168">description</span></span>|<span data-ttu-id="e01df-169">String</span><span class="sxs-lookup"><span data-stu-id="e01df-169">String</span></span>|<span data-ttu-id="e01df-170">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="e01df-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="e01df-171">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e01df-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e01df-172">displayName</span><span class="sxs-lookup"><span data-stu-id="e01df-172">displayName</span></span>|<span data-ttu-id="e01df-173">String</span><span class="sxs-lookup"><span data-stu-id="e01df-173">String</span></span>|<span data-ttu-id="e01df-174">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="e01df-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="e01df-175">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e01df-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e01df-176">version</span><span class="sxs-lookup"><span data-stu-id="e01df-176">version</span></span>|<span data-ttu-id="e01df-177">Int32</span><span class="sxs-lookup"><span data-stu-id="e01df-177">Int32</span></span>|<span data-ttu-id="e01df-178">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="e01df-178">Version of the device configuration.</span></span> <span data-ttu-id="e01df-179">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e01df-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e01df-180">passwordBlockFaceUnlock</span><span class="sxs-lookup"><span data-stu-id="e01df-180">passwordBlockFaceUnlock</span></span>|<span data-ttu-id="e01df-181">布尔值</span><span class="sxs-lookup"><span data-stu-id="e01df-181">Boolean</span></span>|<span data-ttu-id="e01df-182">指示是否阻止人脸解锁。</span><span class="sxs-lookup"><span data-stu-id="e01df-182">Indicates whether or not to block face unlock.</span></span>|
|<span data-ttu-id="e01df-183">passwordBlockFingerprintUnlock</span><span class="sxs-lookup"><span data-stu-id="e01df-183">passwordBlockFingerprintUnlock</span></span>|<span data-ttu-id="e01df-184">Boolean</span><span class="sxs-lookup"><span data-stu-id="e01df-184">Boolean</span></span>|<span data-ttu-id="e01df-185">指示是否阻止指纹解锁。</span><span class="sxs-lookup"><span data-stu-id="e01df-185">Indicates whether or not to block fingerprint unlock.</span></span>|
|<span data-ttu-id="e01df-186">passwordBlockIrisUnlock</span><span class="sxs-lookup"><span data-stu-id="e01df-186">passwordBlockIrisUnlock</span></span>|<span data-ttu-id="e01df-187">布尔值</span><span class="sxs-lookup"><span data-stu-id="e01df-187">Boolean</span></span>|<span data-ttu-id="e01df-188">指示是否阻止 iri 解锁。</span><span class="sxs-lookup"><span data-stu-id="e01df-188">Indicates whether or not to block iris unlock.</span></span>|
|<span data-ttu-id="e01df-189">passwordBlockTrustAgents</span><span class="sxs-lookup"><span data-stu-id="e01df-189">passwordBlockTrustAgents</span></span>|<span data-ttu-id="e01df-190">Boolean</span><span class="sxs-lookup"><span data-stu-id="e01df-190">Boolean</span></span>|<span data-ttu-id="e01df-191">指示是否阻止 Smart Lock 和其他信任代理。</span><span class="sxs-lookup"><span data-stu-id="e01df-191">Indicates whether or not to block Smart Lock and other trust agents.</span></span>|
|<span data-ttu-id="e01df-192">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="e01df-192">passwordExpirationDays</span></span>|<span data-ttu-id="e01df-193">Int32</span><span class="sxs-lookup"><span data-stu-id="e01df-193">Int32</span></span>|<span data-ttu-id="e01df-194">密码过期前的天数。</span><span class="sxs-lookup"><span data-stu-id="e01df-194">Number of days before the password expires.</span></span> <span data-ttu-id="e01df-195">有效值为 1 至 365。</span><span class="sxs-lookup"><span data-stu-id="e01df-195">Valid values 1 to 365</span></span>|
|<span data-ttu-id="e01df-196">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="e01df-196">passwordMinimumLength</span></span>|<span data-ttu-id="e01df-197">Int32</span><span class="sxs-lookup"><span data-stu-id="e01df-197">Int32</span></span>|<span data-ttu-id="e01df-198">密码的最小长度。</span><span class="sxs-lookup"><span data-stu-id="e01df-198">Minimum length of passwords.</span></span> <span data-ttu-id="e01df-199">有效值为 4 至 16</span><span class="sxs-lookup"><span data-stu-id="e01df-199">Valid values 4 to 16</span></span>|
|<span data-ttu-id="e01df-200">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="e01df-200">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="e01df-201">Int32</span><span class="sxs-lookup"><span data-stu-id="e01df-201">Int32</span></span>|<span data-ttu-id="e01df-202">屏幕超时之前的不活动分钟数。</span><span class="sxs-lookup"><span data-stu-id="e01df-202">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="e01df-203">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="e01df-203">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="e01df-204">Int32</span><span class="sxs-lookup"><span data-stu-id="e01df-204">Int32</span></span>|<span data-ttu-id="e01df-205">要阻止的以前密码的数量。</span><span class="sxs-lookup"><span data-stu-id="e01df-205">Number of previous passwords to block.</span></span> <span data-ttu-id="e01df-206">有效值为 0 至 24</span><span class="sxs-lookup"><span data-stu-id="e01df-206">Valid values 0 to 24</span></span>|
|<span data-ttu-id="e01df-207">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="e01df-207">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="e01df-208">Int32</span><span class="sxs-lookup"><span data-stu-id="e01df-208">Int32</span></span>|<span data-ttu-id="e01df-209">恢复出厂设置之前允许登录失败的次数。</span><span class="sxs-lookup"><span data-stu-id="e01df-209">Number of sign in failures allowed before factory reset.</span></span> <span data-ttu-id="e01df-210">有效值为1至16</span><span class="sxs-lookup"><span data-stu-id="e01df-210">Valid values 1 to 16</span></span>|
|<span data-ttu-id="e01df-211">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="e01df-211">passwordRequiredType</span></span>|[<span data-ttu-id="e01df-212">androidForWorkRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="e01df-212">androidForWorkRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androidforworkrequiredpasswordtype.md)|<span data-ttu-id="e01df-213">必需的密码类型。</span><span class="sxs-lookup"><span data-stu-id="e01df-213">Type of password that is required.</span></span> <span data-ttu-id="e01df-214">可取值为：`deviceDefault`、`lowSecurityBiometric`、`required`、`atLeastNumeric`、`numericComplex`、`atLeastAlphabetic`、`atLeastAlphanumeric`、`alphanumericWithSymbols`。</span><span class="sxs-lookup"><span data-stu-id="e01df-214">Possible values are: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric`, `alphanumericWithSymbols`.</span></span>|
|<span data-ttu-id="e01df-215">workProfileDataSharingType</span><span class="sxs-lookup"><span data-stu-id="e01df-215">workProfileDataSharingType</span></span>|[<span data-ttu-id="e01df-216">androidForWorkCrossProfileDataSharingType</span><span class="sxs-lookup"><span data-stu-id="e01df-216">androidForWorkCrossProfileDataSharingType</span></span>](../resources/intune-deviceconfig-androidforworkcrossprofiledatasharingtype.md)|<span data-ttu-id="e01df-217">允许的数据共享类型。</span><span class="sxs-lookup"><span data-stu-id="e01df-217">Type of data sharing that is allowed.</span></span> <span data-ttu-id="e01df-218">可取值为：`deviceDefault`、`preventAny`、`allowPersonalToWork`、`noRestrictions`。</span><span class="sxs-lookup"><span data-stu-id="e01df-218">Possible values are: `deviceDefault`, `preventAny`, `allowPersonalToWork`, `noRestrictions`.</span></span>|
|<span data-ttu-id="e01df-219">workProfileBlockNotificationsWhileDeviceLocked</span><span class="sxs-lookup"><span data-stu-id="e01df-219">workProfileBlockNotificationsWhileDeviceLocked</span></span>|<span data-ttu-id="e01df-220">布尔值</span><span class="sxs-lookup"><span data-stu-id="e01df-220">Boolean</span></span>|<span data-ttu-id="e01df-221">指示在设备锁定时是否阻止通知。</span><span class="sxs-lookup"><span data-stu-id="e01df-221">Indicates whether or not to block notifications while device locked.</span></span>|
|<span data-ttu-id="e01df-222">workProfileBlockAddingAccounts</span><span class="sxs-lookup"><span data-stu-id="e01df-222">workProfileBlockAddingAccounts</span></span>|<span data-ttu-id="e01df-223">布尔值</span><span class="sxs-lookup"><span data-stu-id="e01df-223">Boolean</span></span>|<span data-ttu-id="e01df-224">阻止用户在工作配置文件中添加/删除帐户。</span><span class="sxs-lookup"><span data-stu-id="e01df-224">Block users from adding/removing accounts in work profile.</span></span>|
|<span data-ttu-id="e01df-225">workProfileBluetoothEnableContactSharing</span><span class="sxs-lookup"><span data-stu-id="e01df-225">workProfileBluetoothEnableContactSharing</span></span>|<span data-ttu-id="e01df-226">布尔值</span><span class="sxs-lookup"><span data-stu-id="e01df-226">Boolean</span></span>|<span data-ttu-id="e01df-227">允许蓝牙设备访问企业联系人。</span><span class="sxs-lookup"><span data-stu-id="e01df-227">Allow bluetooth devices to access enterprise contacts.</span></span>|
|<span data-ttu-id="e01df-228">workProfileBlockScreenCapture</span><span class="sxs-lookup"><span data-stu-id="e01df-228">workProfileBlockScreenCapture</span></span>|<span data-ttu-id="e01df-229">布尔值</span><span class="sxs-lookup"><span data-stu-id="e01df-229">Boolean</span></span>|<span data-ttu-id="e01df-230">在工作配置文件中阻止屏幕捕获。</span><span class="sxs-lookup"><span data-stu-id="e01df-230">Block screen capture in work profile.</span></span>|
|<span data-ttu-id="e01df-231">workProfileBlockCrossProfileCallerId</span><span class="sxs-lookup"><span data-stu-id="e01df-231">workProfileBlockCrossProfileCallerId</span></span>|<span data-ttu-id="e01df-232">布尔值</span><span class="sxs-lookup"><span data-stu-id="e01df-232">Boolean</span></span>|<span data-ttu-id="e01df-233">阻止显示个人配置文件中的工作配置文件呼叫者 ID。</span><span class="sxs-lookup"><span data-stu-id="e01df-233">Block display work profile caller ID in personal profile.</span></span>|
|<span data-ttu-id="e01df-234">workProfileBlockCamera</span><span class="sxs-lookup"><span data-stu-id="e01df-234">workProfileBlockCamera</span></span>|<span data-ttu-id="e01df-235">布尔值</span><span class="sxs-lookup"><span data-stu-id="e01df-235">Boolean</span></span>|<span data-ttu-id="e01df-236">阻止工作配置文件相机。</span><span class="sxs-lookup"><span data-stu-id="e01df-236">Block work profile camera.</span></span>|
|<span data-ttu-id="e01df-237">workProfileBlockCrossProfileContactsSearch</span><span class="sxs-lookup"><span data-stu-id="e01df-237">workProfileBlockCrossProfileContactsSearch</span></span>|<span data-ttu-id="e01df-238">布尔值</span><span class="sxs-lookup"><span data-stu-id="e01df-238">Boolean</span></span>|<span data-ttu-id="e01df-239">阻止个人配置文件中的工作配置文件联系人可用性。</span><span class="sxs-lookup"><span data-stu-id="e01df-239">Block work profile contacts availability in personal profile.</span></span>|
|<span data-ttu-id="e01df-240">workProfileBlockCrossProfileCopyPaste</span><span class="sxs-lookup"><span data-stu-id="e01df-240">workProfileBlockCrossProfileCopyPaste</span></span>|<span data-ttu-id="e01df-241">布尔值</span><span class="sxs-lookup"><span data-stu-id="e01df-241">Boolean</span></span>|<span data-ttu-id="e01df-242">指示是否启用 "禁用跨配置文件复制/粘贴" 设置的 Boolean。</span><span class="sxs-lookup"><span data-stu-id="e01df-242">Boolean that indicates if the setting disallow cross profile copy/paste is enabled.</span></span>|
|<span data-ttu-id="e01df-243">workProfileDefaultAppPermissionPolicy</span><span class="sxs-lookup"><span data-stu-id="e01df-243">workProfileDefaultAppPermissionPolicy</span></span>|[<span data-ttu-id="e01df-244">androidForWorkDefaultAppPermissionPolicyType</span><span class="sxs-lookup"><span data-stu-id="e01df-244">androidForWorkDefaultAppPermissionPolicyType</span></span>](../resources/intune-deviceconfig-androidforworkdefaultapppermissionpolicytype.md)|<span data-ttu-id="e01df-245">必需的密码类型。</span><span class="sxs-lookup"><span data-stu-id="e01df-245">Type of password that is required.</span></span> <span data-ttu-id="e01df-246">可取值为：`deviceDefault`、`prompt`、`autoGrant`、`autoDeny`。</span><span class="sxs-lookup"><span data-stu-id="e01df-246">Possible values are: `deviceDefault`, `prompt`, `autoGrant`, `autoDeny`.</span></span>|
|<span data-ttu-id="e01df-247">workProfilePasswordBlockFaceUnlock</span><span class="sxs-lookup"><span data-stu-id="e01df-247">workProfilePasswordBlockFaceUnlock</span></span>|<span data-ttu-id="e01df-248">布尔值</span><span class="sxs-lookup"><span data-stu-id="e01df-248">Boolean</span></span>|<span data-ttu-id="e01df-249">指示是否阻止工作配置文件的人脸解锁。</span><span class="sxs-lookup"><span data-stu-id="e01df-249">Indicates whether or not to block face unlock for work profile.</span></span>|
|<span data-ttu-id="e01df-250">workProfilePasswordBlockFingerprintUnlock</span><span class="sxs-lookup"><span data-stu-id="e01df-250">workProfilePasswordBlockFingerprintUnlock</span></span>|<span data-ttu-id="e01df-251">布尔值</span><span class="sxs-lookup"><span data-stu-id="e01df-251">Boolean</span></span>|<span data-ttu-id="e01df-252">指示是否阻止工作配置文件的指纹解锁。</span><span class="sxs-lookup"><span data-stu-id="e01df-252">Indicates whether or not to block fingerprint unlock for work profile.</span></span>|
|<span data-ttu-id="e01df-253">workProfilePasswordBlockIrisUnlock</span><span class="sxs-lookup"><span data-stu-id="e01df-253">workProfilePasswordBlockIrisUnlock</span></span>|<span data-ttu-id="e01df-254">布尔值</span><span class="sxs-lookup"><span data-stu-id="e01df-254">Boolean</span></span>|<span data-ttu-id="e01df-255">指示是否阻止对工作配置文件的 iri 解除锁定。</span><span class="sxs-lookup"><span data-stu-id="e01df-255">Indicates whether or not to block iris unlock for work profile.</span></span>|
|<span data-ttu-id="e01df-256">workProfilePasswordBlockTrustAgents</span><span class="sxs-lookup"><span data-stu-id="e01df-256">workProfilePasswordBlockTrustAgents</span></span>|<span data-ttu-id="e01df-257">布尔值</span><span class="sxs-lookup"><span data-stu-id="e01df-257">Boolean</span></span>|<span data-ttu-id="e01df-258">指示是否阻止智能锁定和其他信任代理用于工作配置文件。</span><span class="sxs-lookup"><span data-stu-id="e01df-258">Indicates whether or not to block Smart Lock and other trust agents for work profile.</span></span>|
|<span data-ttu-id="e01df-259">workProfilePasswordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="e01df-259">workProfilePasswordExpirationDays</span></span>|<span data-ttu-id="e01df-260">Int32</span><span class="sxs-lookup"><span data-stu-id="e01df-260">Int32</span></span>|<span data-ttu-id="e01df-261">工作配置文件密码到期前的天数。</span><span class="sxs-lookup"><span data-stu-id="e01df-261">Number of days before the work profile password expires.</span></span> <span data-ttu-id="e01df-262">有效值为 1 至 365。</span><span class="sxs-lookup"><span data-stu-id="e01df-262">Valid values 1 to 365</span></span>|
|<span data-ttu-id="e01df-263">workProfilePasswordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="e01df-263">workProfilePasswordMinimumLength</span></span>|<span data-ttu-id="e01df-264">Int32</span><span class="sxs-lookup"><span data-stu-id="e01df-264">Int32</span></span>|<span data-ttu-id="e01df-265">工作配置文件密码的最小长度。</span><span class="sxs-lookup"><span data-stu-id="e01df-265">Minimum length of work profile password.</span></span> <span data-ttu-id="e01df-266">有效值为 4 至 16</span><span class="sxs-lookup"><span data-stu-id="e01df-266">Valid values 4 to 16</span></span>|
|<span data-ttu-id="e01df-267">workProfilePasswordMinNumericCharacters</span><span class="sxs-lookup"><span data-stu-id="e01df-267">workProfilePasswordMinNumericCharacters</span></span>|<span data-ttu-id="e01df-268">Int32</span><span class="sxs-lookup"><span data-stu-id="e01df-268">Int32</span></span>|<span data-ttu-id="e01df-269">工作配置文件密码中所需的最小数字字符数。</span><span class="sxs-lookup"><span data-stu-id="e01df-269">Minimum # of numeric characters required in work profile password.</span></span> <span data-ttu-id="e01df-270">有效值为1至10</span><span class="sxs-lookup"><span data-stu-id="e01df-270">Valid values 1 to 10</span></span>|
|<span data-ttu-id="e01df-271">workProfilePasswordMinNonLetterCharacters</span><span class="sxs-lookup"><span data-stu-id="e01df-271">workProfilePasswordMinNonLetterCharacters</span></span>|<span data-ttu-id="e01df-272">Int32</span><span class="sxs-lookup"><span data-stu-id="e01df-272">Int32</span></span>|<span data-ttu-id="e01df-273">工作配置文件密码中所需的最小非字母字符数。</span><span class="sxs-lookup"><span data-stu-id="e01df-273">Minimum # of non-letter characters required in work profile password.</span></span> <span data-ttu-id="e01df-274">有效值为1至10</span><span class="sxs-lookup"><span data-stu-id="e01df-274">Valid values 1 to 10</span></span>|
|<span data-ttu-id="e01df-275">workProfilePasswordMinLetterCharacters</span><span class="sxs-lookup"><span data-stu-id="e01df-275">workProfilePasswordMinLetterCharacters</span></span>|<span data-ttu-id="e01df-276">Int32</span><span class="sxs-lookup"><span data-stu-id="e01df-276">Int32</span></span>|<span data-ttu-id="e01df-277">工作配置文件密码中所需的字母字符的最小数目。</span><span class="sxs-lookup"><span data-stu-id="e01df-277">Minimum # of letter characters required in work profile password.</span></span> <span data-ttu-id="e01df-278">有效值为1至10</span><span class="sxs-lookup"><span data-stu-id="e01df-278">Valid values 1 to 10</span></span>|
|<span data-ttu-id="e01df-279">workProfilePasswordMinLowerCaseCharacters</span><span class="sxs-lookup"><span data-stu-id="e01df-279">workProfilePasswordMinLowerCaseCharacters</span></span>|<span data-ttu-id="e01df-280">Int32</span><span class="sxs-lookup"><span data-stu-id="e01df-280">Int32</span></span>|<span data-ttu-id="e01df-281">工作配置文件密码中所需的小写字符的最小数量。</span><span class="sxs-lookup"><span data-stu-id="e01df-281">Minimum # of lower-case characters required in work profile password.</span></span> <span data-ttu-id="e01df-282">有效值为1至10</span><span class="sxs-lookup"><span data-stu-id="e01df-282">Valid values 1 to 10</span></span>|
|<span data-ttu-id="e01df-283">workProfilePasswordMinUpperCaseCharacters</span><span class="sxs-lookup"><span data-stu-id="e01df-283">workProfilePasswordMinUpperCaseCharacters</span></span>|<span data-ttu-id="e01df-284">Int32</span><span class="sxs-lookup"><span data-stu-id="e01df-284">Int32</span></span>|<span data-ttu-id="e01df-285">工作配置文件密码中要求的大写字符的最小数量。</span><span class="sxs-lookup"><span data-stu-id="e01df-285">Minimum # of upper-case characters required in work profile password.</span></span> <span data-ttu-id="e01df-286">有效值为1至10</span><span class="sxs-lookup"><span data-stu-id="e01df-286">Valid values 1 to 10</span></span>|
|<span data-ttu-id="e01df-287">workProfilePasswordMinSymbolCharacters</span><span class="sxs-lookup"><span data-stu-id="e01df-287">workProfilePasswordMinSymbolCharacters</span></span>|<span data-ttu-id="e01df-288">Int32</span><span class="sxs-lookup"><span data-stu-id="e01df-288">Int32</span></span>|<span data-ttu-id="e01df-289">工作配置文件密码中所需的最小符号数。</span><span class="sxs-lookup"><span data-stu-id="e01df-289">Minimum # of symbols required in work profile password.</span></span> <span data-ttu-id="e01df-290">有效值为1至10</span><span class="sxs-lookup"><span data-stu-id="e01df-290">Valid values 1 to 10</span></span>|
|<span data-ttu-id="e01df-291">workProfilePasswordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="e01df-291">workProfilePasswordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="e01df-292">Int32</span><span class="sxs-lookup"><span data-stu-id="e01df-292">Int32</span></span>|<span data-ttu-id="e01df-293">屏幕超时之前的不活动分钟数。</span><span class="sxs-lookup"><span data-stu-id="e01df-293">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="e01df-294">workProfilePasswordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="e01df-294">workProfilePasswordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="e01df-295">Int32</span><span class="sxs-lookup"><span data-stu-id="e01df-295">Int32</span></span>|<span data-ttu-id="e01df-296">要阻止的以前的工作配置文件密码的数量。</span><span class="sxs-lookup"><span data-stu-id="e01df-296">Number of previous work profile passwords to block.</span></span> <span data-ttu-id="e01df-297">有效值为 0 至 24</span><span class="sxs-lookup"><span data-stu-id="e01df-297">Valid values 0 to 24</span></span>|
|<span data-ttu-id="e01df-298">workProfilePasswordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="e01df-298">workProfilePasswordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="e01df-299">Int32</span><span class="sxs-lookup"><span data-stu-id="e01df-299">Int32</span></span>|<span data-ttu-id="e01df-300">在删除工作配置文件和删除所有公司数据之前允许的登录失败次数。</span><span class="sxs-lookup"><span data-stu-id="e01df-300">Number of sign in failures allowed before work profile is removed and all corporate data deleted.</span></span> <span data-ttu-id="e01df-301">有效值为1至16</span><span class="sxs-lookup"><span data-stu-id="e01df-301">Valid values 1 to 16</span></span>|
|<span data-ttu-id="e01df-302">workProfilePasswordRequiredType</span><span class="sxs-lookup"><span data-stu-id="e01df-302">workProfilePasswordRequiredType</span></span>|[<span data-ttu-id="e01df-303">androidForWorkRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="e01df-303">androidForWorkRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androidforworkrequiredpasswordtype.md)|<span data-ttu-id="e01df-304">所需的工作配置文件密码类型。</span><span class="sxs-lookup"><span data-stu-id="e01df-304">Type of work profile password that is required.</span></span> <span data-ttu-id="e01df-305">可取值为：`deviceDefault`、`lowSecurityBiometric`、`required`、`atLeastNumeric`、`numericComplex`、`atLeastAlphabetic`、`atLeastAlphanumeric`、`alphanumericWithSymbols`。</span><span class="sxs-lookup"><span data-stu-id="e01df-305">Possible values are: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric`, `alphanumericWithSymbols`.</span></span>|
|<span data-ttu-id="e01df-306">workProfileRequirePassword</span><span class="sxs-lookup"><span data-stu-id="e01df-306">workProfileRequirePassword</span></span>|<span data-ttu-id="e01df-307">布尔值</span><span class="sxs-lookup"><span data-stu-id="e01df-307">Boolean</span></span>|<span data-ttu-id="e01df-308">对于工作配置文件，密码是必需的</span><span class="sxs-lookup"><span data-stu-id="e01df-308">Password is required or not for work profile</span></span>|
|<span data-ttu-id="e01df-309">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="e01df-309">securityRequireVerifyApps</span></span>|<span data-ttu-id="e01df-310">Boolean</span><span class="sxs-lookup"><span data-stu-id="e01df-310">Boolean</span></span>|<span data-ttu-id="e01df-311">要求启用 Android 验证应用功能。</span><span class="sxs-lookup"><span data-stu-id="e01df-311">Require the Android Verify apps feature is turned on.</span></span>|
|<span data-ttu-id="e01df-312">vpnAlwaysOnPackageIdentifier</span><span class="sxs-lookup"><span data-stu-id="e01df-312">vpnAlwaysOnPackageIdentifier</span></span>|<span data-ttu-id="e01df-313">String</span><span class="sxs-lookup"><span data-stu-id="e01df-313">String</span></span>|<span data-ttu-id="e01df-314">为 always on VPN 启用锁定模式。</span><span class="sxs-lookup"><span data-stu-id="e01df-314">Enable lockdown mode for always-on VPN.</span></span>|
|<span data-ttu-id="e01df-315">vpnEnableAlwaysOnLockdownMode</span><span class="sxs-lookup"><span data-stu-id="e01df-315">vpnEnableAlwaysOnLockdownMode</span></span>|<span data-ttu-id="e01df-316">布尔值</span><span class="sxs-lookup"><span data-stu-id="e01df-316">Boolean</span></span>|<span data-ttu-id="e01df-317">为 always on VPN 启用锁定模式。</span><span class="sxs-lookup"><span data-stu-id="e01df-317">Enable lockdown mode for always-on VPN.</span></span>|
|<span data-ttu-id="e01df-318">workProfileAllowWidgets</span><span class="sxs-lookup"><span data-stu-id="e01df-318">workProfileAllowWidgets</span></span>|<span data-ttu-id="e01df-319">布尔值</span><span class="sxs-lookup"><span data-stu-id="e01df-319">Boolean</span></span>|<span data-ttu-id="e01df-320">允许来自工作配置文件应用程序的小部件。</span><span class="sxs-lookup"><span data-stu-id="e01df-320">Allow widgets from work profile apps.</span></span>|
|<span data-ttu-id="e01df-321">workProfileBlockPersonalAppInstallsFromUnknownSources</span><span class="sxs-lookup"><span data-stu-id="e01df-321">workProfileBlockPersonalAppInstallsFromUnknownSources</span></span>|<span data-ttu-id="e01df-322">布尔值</span><span class="sxs-lookup"><span data-stu-id="e01df-322">Boolean</span></span>|<span data-ttu-id="e01df-323">阻止从个人配置文件中的未知源进行应用程序安装。</span><span class="sxs-lookup"><span data-stu-id="e01df-323">Prevent app installations from unknown sources in the personal profile.</span></span>|



## <a name="response"></a><span data-ttu-id="e01df-324">响应</span><span class="sxs-lookup"><span data-stu-id="e01df-324">Response</span></span>
<span data-ttu-id="e01df-325">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和更新的 [androidForWorkGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidforworkgeneraldeviceconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="e01df-325">If successful, this method returns a `200 OK` response code and an updated [androidForWorkGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidforworkgeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e01df-326">示例</span><span class="sxs-lookup"><span data-stu-id="e01df-326">Example</span></span>

### <a name="request"></a><span data-ttu-id="e01df-327">请求</span><span class="sxs-lookup"><span data-stu-id="e01df-327">Request</span></span>
<span data-ttu-id="e01df-328">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="e01df-328">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 3079

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
  "passwordBlockFaceUnlock": true,
  "passwordBlockFingerprintUnlock": true,
  "passwordBlockIrisUnlock": true,
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
  "workProfilePasswordBlockFaceUnlock": true,
  "workProfilePasswordBlockFingerprintUnlock": true,
  "workProfilePasswordBlockIrisUnlock": true,
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

### <a name="response"></a><span data-ttu-id="e01df-329">响应</span><span class="sxs-lookup"><span data-stu-id="e01df-329">Response</span></span>
<span data-ttu-id="e01df-p131">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="e01df-p131">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 3251

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
  "passwordBlockFaceUnlock": true,
  "passwordBlockFingerprintUnlock": true,
  "passwordBlockIrisUnlock": true,
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
  "workProfilePasswordBlockFaceUnlock": true,
  "workProfilePasswordBlockFingerprintUnlock": true,
  "workProfilePasswordBlockIrisUnlock": true,
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



