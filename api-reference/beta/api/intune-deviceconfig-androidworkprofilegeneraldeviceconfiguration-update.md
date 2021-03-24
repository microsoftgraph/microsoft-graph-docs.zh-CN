---
title: 更新 androidWorkProfileGeneralDeviceConfiguration
description: 更新 androidWorkProfileGeneralDeviceConfiguration 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: e1a0c563e83051968d970c9b5bdda69f178b9f68
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51148111"
---
# <a name="update-androidworkprofilegeneraldeviceconfiguration"></a><span data-ttu-id="baa55-103">更新 androidWorkProfileGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="baa55-103">Update androidWorkProfileGeneralDeviceConfiguration</span></span>

<span data-ttu-id="baa55-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="baa55-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="baa55-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="baa55-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="baa55-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="baa55-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="baa55-107">更新 [androidWorkProfileGeneralDeviceConfiguration 对象](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="baa55-107">Update the properties of a [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="baa55-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="baa55-108">Prerequisites</span></span>
<span data-ttu-id="baa55-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="baa55-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="baa55-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="baa55-111">Permission type</span></span>|<span data-ttu-id="baa55-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="baa55-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="baa55-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="baa55-113">Delegated (work or school account)</span></span>|<span data-ttu-id="baa55-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="baa55-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="baa55-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="baa55-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="baa55-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="baa55-116">Not supported.</span></span>|
|<span data-ttu-id="baa55-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="baa55-117">Application</span></span>|<span data-ttu-id="baa55-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="baa55-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="baa55-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="baa55-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="baa55-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="baa55-120">Request headers</span></span>
|<span data-ttu-id="baa55-121">标头</span><span class="sxs-lookup"><span data-stu-id="baa55-121">Header</span></span>|<span data-ttu-id="baa55-122">值</span><span class="sxs-lookup"><span data-stu-id="baa55-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="baa55-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="baa55-123">Authorization</span></span>|<span data-ttu-id="baa55-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="baa55-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="baa55-125">接受</span><span class="sxs-lookup"><span data-stu-id="baa55-125">Accept</span></span>|<span data-ttu-id="baa55-126">application/json</span><span class="sxs-lookup"><span data-stu-id="baa55-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="baa55-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="baa55-127">Request body</span></span>
<span data-ttu-id="baa55-128">在请求正文中，提供 [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="baa55-128">In the request body, supply a JSON representation for the [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) object.</span></span>

<span data-ttu-id="baa55-129">下表显示创建 [androidWorkProfileGeneralDeviceConfiguration 时所需的属性](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md)。</span><span class="sxs-lookup"><span data-stu-id="baa55-129">The following table shows the properties that are required when you create the [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md).</span></span>

|<span data-ttu-id="baa55-130">属性</span><span class="sxs-lookup"><span data-stu-id="baa55-130">Property</span></span>|<span data-ttu-id="baa55-131">类型</span><span class="sxs-lookup"><span data-stu-id="baa55-131">Type</span></span>|<span data-ttu-id="baa55-132">说明</span><span class="sxs-lookup"><span data-stu-id="baa55-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="baa55-133">id</span><span class="sxs-lookup"><span data-stu-id="baa55-133">id</span></span>|<span data-ttu-id="baa55-134">String</span><span class="sxs-lookup"><span data-stu-id="baa55-134">String</span></span>|<span data-ttu-id="baa55-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="baa55-135">Key of the entity.</span></span> <span data-ttu-id="baa55-136">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="baa55-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="baa55-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="baa55-137">lastModifiedDateTime</span></span>|<span data-ttu-id="baa55-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="baa55-138">DateTimeOffset</span></span>|<span data-ttu-id="baa55-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="baa55-139">DateTime the object was last modified.</span></span> <span data-ttu-id="baa55-140">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="baa55-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="baa55-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="baa55-141">roleScopeTagIds</span></span>|<span data-ttu-id="baa55-142">String collection</span><span class="sxs-lookup"><span data-stu-id="baa55-142">String collection</span></span>|<span data-ttu-id="baa55-143">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="baa55-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="baa55-144">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="baa55-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="baa55-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="baa55-145">supportsScopeTags</span></span>|<span data-ttu-id="baa55-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="baa55-146">Boolean</span></span>|<span data-ttu-id="baa55-147">指示基础设备配置是否支持分配范围标记。</span><span class="sxs-lookup"><span data-stu-id="baa55-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="baa55-148">当此值为 false 且实体对作用域用户不可见时，不允许分配给 ScopeTags 属性。</span><span class="sxs-lookup"><span data-stu-id="baa55-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="baa55-149">这适用于在 Silverlight 中创建的旧版策略，可通过在 Azure 门户中删除和重新创建策略来解决。</span><span class="sxs-lookup"><span data-stu-id="baa55-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="baa55-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="baa55-150">This property is read-only.</span></span> <span data-ttu-id="baa55-151">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="baa55-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="baa55-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="baa55-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="baa55-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="baa55-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="baa55-154">此策略的操作系统版本适用性。</span><span class="sxs-lookup"><span data-stu-id="baa55-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="baa55-155">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="baa55-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="baa55-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="baa55-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="baa55-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="baa55-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="baa55-158">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="baa55-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="baa55-159">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="baa55-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="baa55-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="baa55-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="baa55-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="baa55-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="baa55-162">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="baa55-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="baa55-163">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="baa55-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="baa55-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="baa55-164">createdDateTime</span></span>|<span data-ttu-id="baa55-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="baa55-165">DateTimeOffset</span></span>|<span data-ttu-id="baa55-166">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="baa55-166">DateTime the object was created.</span></span> <span data-ttu-id="baa55-167">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="baa55-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="baa55-168">说明</span><span class="sxs-lookup"><span data-stu-id="baa55-168">description</span></span>|<span data-ttu-id="baa55-169">String</span><span class="sxs-lookup"><span data-stu-id="baa55-169">String</span></span>|<span data-ttu-id="baa55-170">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="baa55-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="baa55-171">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="baa55-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="baa55-172">displayName</span><span class="sxs-lookup"><span data-stu-id="baa55-172">displayName</span></span>|<span data-ttu-id="baa55-173">String</span><span class="sxs-lookup"><span data-stu-id="baa55-173">String</span></span>|<span data-ttu-id="baa55-174">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="baa55-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="baa55-175">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="baa55-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="baa55-176">version</span><span class="sxs-lookup"><span data-stu-id="baa55-176">version</span></span>|<span data-ttu-id="baa55-177">Int32</span><span class="sxs-lookup"><span data-stu-id="baa55-177">Int32</span></span>|<span data-ttu-id="baa55-178">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="baa55-178">Version of the device configuration.</span></span> <span data-ttu-id="baa55-179">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="baa55-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="baa55-180">passwordBlockFaceUnlock</span><span class="sxs-lookup"><span data-stu-id="baa55-180">passwordBlockFaceUnlock</span></span>|<span data-ttu-id="baa55-181">Boolean</span><span class="sxs-lookup"><span data-stu-id="baa55-181">Boolean</span></span>|<span data-ttu-id="baa55-182">指示是否阻止人脸解锁。</span><span class="sxs-lookup"><span data-stu-id="baa55-182">Indicates whether or not to block face unlock.</span></span>|
|<span data-ttu-id="baa55-183">passwordBlockFingerprintUnlock</span><span class="sxs-lookup"><span data-stu-id="baa55-183">passwordBlockFingerprintUnlock</span></span>|<span data-ttu-id="baa55-184">Boolean</span><span class="sxs-lookup"><span data-stu-id="baa55-184">Boolean</span></span>|<span data-ttu-id="baa55-185">指示是否阻止指纹解锁。</span><span class="sxs-lookup"><span data-stu-id="baa55-185">Indicates whether or not to block fingerprint unlock.</span></span>|
|<span data-ttu-id="baa55-186">passwordBlockIrisUnlock</span><span class="sxs-lookup"><span data-stu-id="baa55-186">passwordBlockIrisUnlock</span></span>|<span data-ttu-id="baa55-187">Boolean</span><span class="sxs-lookup"><span data-stu-id="baa55-187">Boolean</span></span>|<span data-ttu-id="baa55-188">指示是否阻止虹膜解锁。</span><span class="sxs-lookup"><span data-stu-id="baa55-188">Indicates whether or not to block iris unlock.</span></span>|
|<span data-ttu-id="baa55-189">passwordBlockTrustAgents</span><span class="sxs-lookup"><span data-stu-id="baa55-189">passwordBlockTrustAgents</span></span>|<span data-ttu-id="baa55-190">Boolean</span><span class="sxs-lookup"><span data-stu-id="baa55-190">Boolean</span></span>|<span data-ttu-id="baa55-191">指示是否阻止 Smart Lock 和其他信任代理。</span><span class="sxs-lookup"><span data-stu-id="baa55-191">Indicates whether or not to block Smart Lock and other trust agents.</span></span>|
|<span data-ttu-id="baa55-192">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="baa55-192">passwordExpirationDays</span></span>|<span data-ttu-id="baa55-193">Int32</span><span class="sxs-lookup"><span data-stu-id="baa55-193">Int32</span></span>|<span data-ttu-id="baa55-194">密码过期前的天数。</span><span class="sxs-lookup"><span data-stu-id="baa55-194">Number of days before the password expires.</span></span> <span data-ttu-id="baa55-195">有效值为 1 至 365。</span><span class="sxs-lookup"><span data-stu-id="baa55-195">Valid values 1 to 365</span></span>|
|<span data-ttu-id="baa55-196">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="baa55-196">passwordMinimumLength</span></span>|<span data-ttu-id="baa55-197">Int32</span><span class="sxs-lookup"><span data-stu-id="baa55-197">Int32</span></span>|<span data-ttu-id="baa55-198">密码的最小长度。</span><span class="sxs-lookup"><span data-stu-id="baa55-198">Minimum length of passwords.</span></span> <span data-ttu-id="baa55-199">有效值为 4 至 16</span><span class="sxs-lookup"><span data-stu-id="baa55-199">Valid values 4 to 16</span></span>|
|<span data-ttu-id="baa55-200">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="baa55-200">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="baa55-201">Int32</span><span class="sxs-lookup"><span data-stu-id="baa55-201">Int32</span></span>|<span data-ttu-id="baa55-202">屏幕超时之前的不活动分钟数。</span><span class="sxs-lookup"><span data-stu-id="baa55-202">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="baa55-203">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="baa55-203">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="baa55-204">Int32</span><span class="sxs-lookup"><span data-stu-id="baa55-204">Int32</span></span>|<span data-ttu-id="baa55-205">要阻止的以前密码的数量。</span><span class="sxs-lookup"><span data-stu-id="baa55-205">Number of previous passwords to block.</span></span> <span data-ttu-id="baa55-206">有效值为 0 至 24</span><span class="sxs-lookup"><span data-stu-id="baa55-206">Valid values 0 to 24</span></span>|
|<span data-ttu-id="baa55-207">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="baa55-207">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="baa55-208">Int32</span><span class="sxs-lookup"><span data-stu-id="baa55-208">Int32</span></span>|<span data-ttu-id="baa55-209">恢复出厂设置之前允许登录失败的次数。</span><span class="sxs-lookup"><span data-stu-id="baa55-209">Number of sign in failures allowed before factory reset.</span></span> <span data-ttu-id="baa55-210">有效值为 1 到 16</span><span class="sxs-lookup"><span data-stu-id="baa55-210">Valid values 1 to 16</span></span>|
|<span data-ttu-id="baa55-211">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="baa55-211">passwordRequiredType</span></span>|[<span data-ttu-id="baa55-212">androidWorkProfileRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="baa55-212">androidWorkProfileRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androidworkprofilerequiredpasswordtype.md)|<span data-ttu-id="baa55-213">必需的密码类型。</span><span class="sxs-lookup"><span data-stu-id="baa55-213">Type of password that is required.</span></span> <span data-ttu-id="baa55-214">可取值为：`deviceDefault`、`lowSecurityBiometric`、`required`、`atLeastNumeric`、`numericComplex`、`atLeastAlphabetic`、`atLeastAlphanumeric`、`alphanumericWithSymbols`。</span><span class="sxs-lookup"><span data-stu-id="baa55-214">Possible values are: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric`, `alphanumericWithSymbols`.</span></span>|
|<span data-ttu-id="baa55-215">workProfileAllowAppInstallsFromUnknownSources</span><span class="sxs-lookup"><span data-stu-id="baa55-215">workProfileAllowAppInstallsFromUnknownSources</span></span>|<span data-ttu-id="baa55-216">Boolean</span><span class="sxs-lookup"><span data-stu-id="baa55-216">Boolean</span></span>|<span data-ttu-id="baa55-217">指示是否允许安装来自未知源的应用。</span><span class="sxs-lookup"><span data-stu-id="baa55-217">Indicates whether to allow installation of apps from unknown sources.</span></span>|
|<span data-ttu-id="baa55-218">workProfileDataSharingType</span><span class="sxs-lookup"><span data-stu-id="baa55-218">workProfileDataSharingType</span></span>|[<span data-ttu-id="baa55-219">androidWorkProfileCrossProfileDataSharingType</span><span class="sxs-lookup"><span data-stu-id="baa55-219">androidWorkProfileCrossProfileDataSharingType</span></span>](../resources/intune-deviceconfig-androidworkprofilecrossprofiledatasharingtype.md)|<span data-ttu-id="baa55-220">允许的数据共享类型。</span><span class="sxs-lookup"><span data-stu-id="baa55-220">Type of data sharing that is allowed.</span></span> <span data-ttu-id="baa55-221">可取值为：`deviceDefault`、`preventAny`、`allowPersonalToWork`、`noRestrictions`。</span><span class="sxs-lookup"><span data-stu-id="baa55-221">Possible values are: `deviceDefault`, `preventAny`, `allowPersonalToWork`, `noRestrictions`.</span></span>|
|<span data-ttu-id="baa55-222">workProfileBlockNotificationsWhileDeviceLocked</span><span class="sxs-lookup"><span data-stu-id="baa55-222">workProfileBlockNotificationsWhileDeviceLocked</span></span>|<span data-ttu-id="baa55-223">Boolean</span><span class="sxs-lookup"><span data-stu-id="baa55-223">Boolean</span></span>|<span data-ttu-id="baa55-224">指示设备锁定时是否阻止通知。</span><span class="sxs-lookup"><span data-stu-id="baa55-224">Indicates whether or not to block notifications while device locked.</span></span>|
|<span data-ttu-id="baa55-225">workProfileBlockAddingAccounts</span><span class="sxs-lookup"><span data-stu-id="baa55-225">workProfileBlockAddingAccounts</span></span>|<span data-ttu-id="baa55-226">Boolean</span><span class="sxs-lookup"><span data-stu-id="baa55-226">Boolean</span></span>|<span data-ttu-id="baa55-227">阻止用户在工作配置文件中添加/删除帐户。</span><span class="sxs-lookup"><span data-stu-id="baa55-227">Block users from adding/removing accounts in work profile.</span></span>|
|<span data-ttu-id="baa55-228">workProfileBluetoothEnableContactSharing</span><span class="sxs-lookup"><span data-stu-id="baa55-228">workProfileBluetoothEnableContactSharing</span></span>|<span data-ttu-id="baa55-229">Boolean</span><span class="sxs-lookup"><span data-stu-id="baa55-229">Boolean</span></span>|<span data-ttu-id="baa55-230">允许蓝牙设备访问企业联系人。</span><span class="sxs-lookup"><span data-stu-id="baa55-230">Allow bluetooth devices to access enterprise contacts.</span></span>|
|<span data-ttu-id="baa55-231">workProfileBlockScreenCapture</span><span class="sxs-lookup"><span data-stu-id="baa55-231">workProfileBlockScreenCapture</span></span>|<span data-ttu-id="baa55-232">Boolean</span><span class="sxs-lookup"><span data-stu-id="baa55-232">Boolean</span></span>|<span data-ttu-id="baa55-233">阻止工作配置文件中的屏幕捕获。</span><span class="sxs-lookup"><span data-stu-id="baa55-233">Block screen capture in work profile.</span></span>|
|<span data-ttu-id="baa55-234">workProfileBlockCrossProfileCallerId</span><span class="sxs-lookup"><span data-stu-id="baa55-234">workProfileBlockCrossProfileCallerId</span></span>|<span data-ttu-id="baa55-235">Boolean</span><span class="sxs-lookup"><span data-stu-id="baa55-235">Boolean</span></span>|<span data-ttu-id="baa55-236">阻止在个人配置文件中显示工作配置文件调用方 ID。</span><span class="sxs-lookup"><span data-stu-id="baa55-236">Block display work profile caller ID in personal profile.</span></span>|
|<span data-ttu-id="baa55-237">workProfileBlockCamera</span><span class="sxs-lookup"><span data-stu-id="baa55-237">workProfileBlockCamera</span></span>|<span data-ttu-id="baa55-238">Boolean</span><span class="sxs-lookup"><span data-stu-id="baa55-238">Boolean</span></span>|<span data-ttu-id="baa55-239">阻止工作配置文件相机。</span><span class="sxs-lookup"><span data-stu-id="baa55-239">Block work profile camera.</span></span>|
|<span data-ttu-id="baa55-240">workProfileBlockCrossProfileContactsSearch</span><span class="sxs-lookup"><span data-stu-id="baa55-240">workProfileBlockCrossProfileContactsSearch</span></span>|<span data-ttu-id="baa55-241">Boolean</span><span class="sxs-lookup"><span data-stu-id="baa55-241">Boolean</span></span>|<span data-ttu-id="baa55-242">阻止工作配置文件联系人在个人配置文件中的可用性。</span><span class="sxs-lookup"><span data-stu-id="baa55-242">Block work profile contacts availability in personal profile.</span></span>|
|<span data-ttu-id="baa55-243">workProfileBlockCrossProfileCopyPaste</span><span class="sxs-lookup"><span data-stu-id="baa55-243">workProfileBlockCrossProfileCopyPaste</span></span>|<span data-ttu-id="baa55-244">Boolean</span><span class="sxs-lookup"><span data-stu-id="baa55-244">Boolean</span></span>|<span data-ttu-id="baa55-245">指示设置是否禁用跨配置文件复制/粘贴的布尔值。</span><span class="sxs-lookup"><span data-stu-id="baa55-245">Boolean that indicates if the setting disallow cross profile copy/paste is enabled.</span></span>|
|<span data-ttu-id="baa55-246">workProfileDefaultAppPermissionPolicy</span><span class="sxs-lookup"><span data-stu-id="baa55-246">workProfileDefaultAppPermissionPolicy</span></span>|[<span data-ttu-id="baa55-247">androidWorkProfileDefaultAppPermissionPolicyType</span><span class="sxs-lookup"><span data-stu-id="baa55-247">androidWorkProfileDefaultAppPermissionPolicyType</span></span>](../resources/intune-deviceconfig-androidworkprofiledefaultapppermissionpolicytype.md)|<span data-ttu-id="baa55-248">必需的密码类型。</span><span class="sxs-lookup"><span data-stu-id="baa55-248">Type of password that is required.</span></span> <span data-ttu-id="baa55-249">可取值为：`deviceDefault`、`prompt`、`autoGrant`、`autoDeny`。</span><span class="sxs-lookup"><span data-stu-id="baa55-249">Possible values are: `deviceDefault`, `prompt`, `autoGrant`, `autoDeny`.</span></span>|
|<span data-ttu-id="baa55-250">workProfilePasswordBlockFaceUnlock</span><span class="sxs-lookup"><span data-stu-id="baa55-250">workProfilePasswordBlockFaceUnlock</span></span>|<span data-ttu-id="baa55-251">Boolean</span><span class="sxs-lookup"><span data-stu-id="baa55-251">Boolean</span></span>|<span data-ttu-id="baa55-252">指示是否阻止工作配置文件的人脸解锁。</span><span class="sxs-lookup"><span data-stu-id="baa55-252">Indicates whether or not to block face unlock for work profile.</span></span>|
|<span data-ttu-id="baa55-253">workProfilePasswordBlockFingerprintUnlock</span><span class="sxs-lookup"><span data-stu-id="baa55-253">workProfilePasswordBlockFingerprintUnlock</span></span>|<span data-ttu-id="baa55-254">Boolean</span><span class="sxs-lookup"><span data-stu-id="baa55-254">Boolean</span></span>|<span data-ttu-id="baa55-255">指示是否阻止工作配置文件的指纹解锁。</span><span class="sxs-lookup"><span data-stu-id="baa55-255">Indicates whether or not to block fingerprint unlock for work profile.</span></span>|
|<span data-ttu-id="baa55-256">workProfilePasswordBlockIrisUnlock</span><span class="sxs-lookup"><span data-stu-id="baa55-256">workProfilePasswordBlockIrisUnlock</span></span>|<span data-ttu-id="baa55-257">Boolean</span><span class="sxs-lookup"><span data-stu-id="baa55-257">Boolean</span></span>|<span data-ttu-id="baa55-258">指示是否阻止工作配置文件的虹膜解锁。</span><span class="sxs-lookup"><span data-stu-id="baa55-258">Indicates whether or not to block iris unlock for work profile.</span></span>|
|<span data-ttu-id="baa55-259">workProfilePasswordBlockTrustAgents</span><span class="sxs-lookup"><span data-stu-id="baa55-259">workProfilePasswordBlockTrustAgents</span></span>|<span data-ttu-id="baa55-260">Boolean</span><span class="sxs-lookup"><span data-stu-id="baa55-260">Boolean</span></span>|<span data-ttu-id="baa55-261">指示是否阻止工作配置文件的智能锁定和其他信任代理。</span><span class="sxs-lookup"><span data-stu-id="baa55-261">Indicates whether or not to block Smart Lock and other trust agents for work profile.</span></span>|
|<span data-ttu-id="baa55-262">workProfilePasswordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="baa55-262">workProfilePasswordExpirationDays</span></span>|<span data-ttu-id="baa55-263">Int32</span><span class="sxs-lookup"><span data-stu-id="baa55-263">Int32</span></span>|<span data-ttu-id="baa55-264">工作配置文件密码过期前的天数。</span><span class="sxs-lookup"><span data-stu-id="baa55-264">Number of days before the work profile password expires.</span></span> <span data-ttu-id="baa55-265">有效值为 1 至 365。</span><span class="sxs-lookup"><span data-stu-id="baa55-265">Valid values 1 to 365</span></span>|
|<span data-ttu-id="baa55-266">workProfilePasswordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="baa55-266">workProfilePasswordMinimumLength</span></span>|<span data-ttu-id="baa55-267">Int32</span><span class="sxs-lookup"><span data-stu-id="baa55-267">Int32</span></span>|<span data-ttu-id="baa55-268">工作配置文件密码的最小长度。</span><span class="sxs-lookup"><span data-stu-id="baa55-268">Minimum length of work profile password.</span></span> <span data-ttu-id="baa55-269">有效值为 4 至 16</span><span class="sxs-lookup"><span data-stu-id="baa55-269">Valid values 4 to 16</span></span>|
|<span data-ttu-id="baa55-270">workProfilePasswordMinNumericCharacters</span><span class="sxs-lookup"><span data-stu-id="baa55-270">workProfilePasswordMinNumericCharacters</span></span>|<span data-ttu-id="baa55-271">Int32</span><span class="sxs-lookup"><span data-stu-id="baa55-271">Int32</span></span>|<span data-ttu-id="baa55-272">工作配置文件密码中所需的数字字符的最小值。</span><span class="sxs-lookup"><span data-stu-id="baa55-272">Minimum # of numeric characters required in work profile password.</span></span> <span data-ttu-id="baa55-273">有效值为 1 到 10</span><span class="sxs-lookup"><span data-stu-id="baa55-273">Valid values 1 to 10</span></span>|
|<span data-ttu-id="baa55-274">workProfilePasswordMinNonLetterCharacters</span><span class="sxs-lookup"><span data-stu-id="baa55-274">workProfilePasswordMinNonLetterCharacters</span></span>|<span data-ttu-id="baa55-275">Int32</span><span class="sxs-lookup"><span data-stu-id="baa55-275">Int32</span></span>|<span data-ttu-id="baa55-276">工作配置文件密码中所需的非字母字符的最小值。</span><span class="sxs-lookup"><span data-stu-id="baa55-276">Minimum # of non-letter characters required in work profile password.</span></span> <span data-ttu-id="baa55-277">有效值为 1 到 10</span><span class="sxs-lookup"><span data-stu-id="baa55-277">Valid values 1 to 10</span></span>|
|<span data-ttu-id="baa55-278">workProfilePasswordMinLetterCharacters</span><span class="sxs-lookup"><span data-stu-id="baa55-278">workProfilePasswordMinLetterCharacters</span></span>|<span data-ttu-id="baa55-279">Int32</span><span class="sxs-lookup"><span data-stu-id="baa55-279">Int32</span></span>|<span data-ttu-id="baa55-280">工作配置文件密码中所需的最小字母字符数。</span><span class="sxs-lookup"><span data-stu-id="baa55-280">Minimum # of letter characters required in work profile password.</span></span> <span data-ttu-id="baa55-281">有效值为 1 到 10</span><span class="sxs-lookup"><span data-stu-id="baa55-281">Valid values 1 to 10</span></span>|
|<span data-ttu-id="baa55-282">workProfilePasswordMinLowerCaseCharacters</span><span class="sxs-lookup"><span data-stu-id="baa55-282">workProfilePasswordMinLowerCaseCharacters</span></span>|<span data-ttu-id="baa55-283">Int32</span><span class="sxs-lookup"><span data-stu-id="baa55-283">Int32</span></span>|<span data-ttu-id="baa55-284">工作配置文件密码中需要的最小小写字符数。</span><span class="sxs-lookup"><span data-stu-id="baa55-284">Minimum # of lower-case characters required in work profile password.</span></span> <span data-ttu-id="baa55-285">有效值为 1 到 10</span><span class="sxs-lookup"><span data-stu-id="baa55-285">Valid values 1 to 10</span></span>|
|<span data-ttu-id="baa55-286">workProfilePasswordMinUpperCaseCharacters</span><span class="sxs-lookup"><span data-stu-id="baa55-286">workProfilePasswordMinUpperCaseCharacters</span></span>|<span data-ttu-id="baa55-287">Int32</span><span class="sxs-lookup"><span data-stu-id="baa55-287">Int32</span></span>|<span data-ttu-id="baa55-288">工作配置文件密码中需要的最小大写字符数。</span><span class="sxs-lookup"><span data-stu-id="baa55-288">Minimum # of upper-case characters required in work profile password.</span></span> <span data-ttu-id="baa55-289">有效值为 1 到 10</span><span class="sxs-lookup"><span data-stu-id="baa55-289">Valid values 1 to 10</span></span>|
|<span data-ttu-id="baa55-290">workProfilePasswordMinSymbolCharacters</span><span class="sxs-lookup"><span data-stu-id="baa55-290">workProfilePasswordMinSymbolCharacters</span></span>|<span data-ttu-id="baa55-291">Int32</span><span class="sxs-lookup"><span data-stu-id="baa55-291">Int32</span></span>|<span data-ttu-id="baa55-292">工作配置文件密码中所需的符号的最小数。</span><span class="sxs-lookup"><span data-stu-id="baa55-292">Minimum # of symbols required in work profile password.</span></span> <span data-ttu-id="baa55-293">有效值为 1 到 10</span><span class="sxs-lookup"><span data-stu-id="baa55-293">Valid values 1 to 10</span></span>|
|<span data-ttu-id="baa55-294">workProfilePasswordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="baa55-294">workProfilePasswordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="baa55-295">Int32</span><span class="sxs-lookup"><span data-stu-id="baa55-295">Int32</span></span>|<span data-ttu-id="baa55-296">屏幕超时之前的不活动分钟数。</span><span class="sxs-lookup"><span data-stu-id="baa55-296">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="baa55-297">workProfilePasswordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="baa55-297">workProfilePasswordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="baa55-298">Int32</span><span class="sxs-lookup"><span data-stu-id="baa55-298">Int32</span></span>|<span data-ttu-id="baa55-299">要阻止的以前工作配置文件密码的数量。</span><span class="sxs-lookup"><span data-stu-id="baa55-299">Number of previous work profile passwords to block.</span></span> <span data-ttu-id="baa55-300">有效值为 0 至 24</span><span class="sxs-lookup"><span data-stu-id="baa55-300">Valid values 0 to 24</span></span>|
|<span data-ttu-id="baa55-301">workProfilePasswordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="baa55-301">workProfilePasswordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="baa55-302">Int32</span><span class="sxs-lookup"><span data-stu-id="baa55-302">Int32</span></span>|<span data-ttu-id="baa55-303">在删除工作配置文件和删除所有公司数据之前允许的登录失败次数。</span><span class="sxs-lookup"><span data-stu-id="baa55-303">Number of sign in failures allowed before work profile is removed and all corporate data deleted.</span></span> <span data-ttu-id="baa55-304">有效值为 1 到 16</span><span class="sxs-lookup"><span data-stu-id="baa55-304">Valid values 1 to 16</span></span>|
|<span data-ttu-id="baa55-305">workProfilePasswordRequiredType</span><span class="sxs-lookup"><span data-stu-id="baa55-305">workProfilePasswordRequiredType</span></span>|[<span data-ttu-id="baa55-306">androidWorkProfileRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="baa55-306">androidWorkProfileRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androidworkprofilerequiredpasswordtype.md)|<span data-ttu-id="baa55-307">所需的工作配置文件密码类型。</span><span class="sxs-lookup"><span data-stu-id="baa55-307">Type of work profile password that is required.</span></span> <span data-ttu-id="baa55-308">可取值为：`deviceDefault`、`lowSecurityBiometric`、`required`、`atLeastNumeric`、`numericComplex`、`atLeastAlphabetic`、`atLeastAlphanumeric`、`alphanumericWithSymbols`。</span><span class="sxs-lookup"><span data-stu-id="baa55-308">Possible values are: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric`, `alphanumericWithSymbols`.</span></span>|
|<span data-ttu-id="baa55-309">workProfileRequirePassword</span><span class="sxs-lookup"><span data-stu-id="baa55-309">workProfileRequirePassword</span></span>|<span data-ttu-id="baa55-310">Boolean</span><span class="sxs-lookup"><span data-stu-id="baa55-310">Boolean</span></span>|<span data-ttu-id="baa55-311">工作配置文件中是否要求密码</span><span class="sxs-lookup"><span data-stu-id="baa55-311">Password is required or not for work profile</span></span>|
|<span data-ttu-id="baa55-312">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="baa55-312">securityRequireVerifyApps</span></span>|<span data-ttu-id="baa55-313">Boolean</span><span class="sxs-lookup"><span data-stu-id="baa55-313">Boolean</span></span>|<span data-ttu-id="baa55-314">要求启用 Android 验证应用功能。</span><span class="sxs-lookup"><span data-stu-id="baa55-314">Require the Android Verify apps feature is turned on.</span></span>|
|<span data-ttu-id="baa55-315">vpnAlwaysOnPackageIdentifier</span><span class="sxs-lookup"><span data-stu-id="baa55-315">vpnAlwaysOnPackageIdentifier</span></span>|<span data-ttu-id="baa55-316">String</span><span class="sxs-lookup"><span data-stu-id="baa55-316">String</span></span>|<span data-ttu-id="baa55-317">为始终打开的 VPN 启用锁定模式。</span><span class="sxs-lookup"><span data-stu-id="baa55-317">Enable lockdown mode for always-on VPN.</span></span>|
|<span data-ttu-id="baa55-318">vpnEnableAlwaysOnLockdownMode</span><span class="sxs-lookup"><span data-stu-id="baa55-318">vpnEnableAlwaysOnLockdownMode</span></span>|<span data-ttu-id="baa55-319">Boolean</span><span class="sxs-lookup"><span data-stu-id="baa55-319">Boolean</span></span>|<span data-ttu-id="baa55-320">为始终打开的 VPN 启用锁定模式。</span><span class="sxs-lookup"><span data-stu-id="baa55-320">Enable lockdown mode for always-on VPN.</span></span>|
|<span data-ttu-id="baa55-321">workProfileAllowWidgets</span><span class="sxs-lookup"><span data-stu-id="baa55-321">workProfileAllowWidgets</span></span>|<span data-ttu-id="baa55-322">Boolean</span><span class="sxs-lookup"><span data-stu-id="baa55-322">Boolean</span></span>|<span data-ttu-id="baa55-323">允许来自工作配置文件应用的小部件。</span><span class="sxs-lookup"><span data-stu-id="baa55-323">Allow widgets from work profile apps.</span></span>|
|<span data-ttu-id="baa55-324">workProfileBlockPersonalAppInstallsFromUnknownSources</span><span class="sxs-lookup"><span data-stu-id="baa55-324">workProfileBlockPersonalAppInstallsFromUnknownSources</span></span>|<span data-ttu-id="baa55-325">Boolean</span><span class="sxs-lookup"><span data-stu-id="baa55-325">Boolean</span></span>|<span data-ttu-id="baa55-326">阻止从个人配置文件中的未知源安装应用。</span><span class="sxs-lookup"><span data-stu-id="baa55-326">Prevent app installations from unknown sources in the personal profile.</span></span>|



## <a name="response"></a><span data-ttu-id="baa55-327">响应</span><span class="sxs-lookup"><span data-stu-id="baa55-327">Response</span></span>
<span data-ttu-id="baa55-328">如果成功，此方法在响应正文中返回 响应代码和更新的 `200 OK` [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="baa55-328">If successful, this method returns a `200 OK` response code and an updated [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="baa55-329">示例</span><span class="sxs-lookup"><span data-stu-id="baa55-329">Example</span></span>

### <a name="request"></a><span data-ttu-id="baa55-330">请求</span><span class="sxs-lookup"><span data-stu-id="baa55-330">Request</span></span>
<span data-ttu-id="baa55-331">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="baa55-331">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 3141

{
  "@odata.type": "#microsoft.graph.androidWorkProfileGeneralDeviceConfiguration",
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
  "workProfileAllowAppInstallsFromUnknownSources": true,
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

### <a name="response"></a><span data-ttu-id="baa55-332">响应</span><span class="sxs-lookup"><span data-stu-id="baa55-332">Response</span></span>
<span data-ttu-id="baa55-p131">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="baa55-p131">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 3313

{
  "@odata.type": "#microsoft.graph.androidWorkProfileGeneralDeviceConfiguration",
  "id": "6decda7e-da7e-6dec-7eda-ec6d7edaec6d",
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
  "workProfileAllowAppInstallsFromUnknownSources": true,
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




