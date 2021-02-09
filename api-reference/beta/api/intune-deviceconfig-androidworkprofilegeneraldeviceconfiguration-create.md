---
title: 创建 androidWorkProfileGeneralDeviceConfiguration
description: 创建新的 androidWorkProfileGeneralDeviceConfiguration 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 914f95106f8962304bf180a22edcae26300ad093
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/09/2021
ms.locfileid: "50155214"
---
# <a name="create-androidworkprofilegeneraldeviceconfiguration"></a><span data-ttu-id="41e74-103">创建 androidWorkProfileGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="41e74-103">Create androidWorkProfileGeneralDeviceConfiguration</span></span>

<span data-ttu-id="41e74-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="41e74-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="41e74-105">**重要提示：** /beta 版本的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="41e74-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="41e74-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="41e74-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="41e74-107">创建新的 [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="41e74-107">Create a new [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="41e74-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="41e74-108">Prerequisites</span></span>
<span data-ttu-id="41e74-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="41e74-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="41e74-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="41e74-111">Permission type</span></span>|<span data-ttu-id="41e74-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="41e74-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="41e74-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="41e74-113">Delegated (work or school account)</span></span>|<span data-ttu-id="41e74-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="41e74-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="41e74-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="41e74-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="41e74-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="41e74-116">Not supported.</span></span>|
|<span data-ttu-id="41e74-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="41e74-117">Application</span></span>|<span data-ttu-id="41e74-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="41e74-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="41e74-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="41e74-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="41e74-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="41e74-120">Request headers</span></span>
|<span data-ttu-id="41e74-121">标头</span><span class="sxs-lookup"><span data-stu-id="41e74-121">Header</span></span>|<span data-ttu-id="41e74-122">值</span><span class="sxs-lookup"><span data-stu-id="41e74-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="41e74-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="41e74-123">Authorization</span></span>|<span data-ttu-id="41e74-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="41e74-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="41e74-125">接受</span><span class="sxs-lookup"><span data-stu-id="41e74-125">Accept</span></span>|<span data-ttu-id="41e74-126">application/json</span><span class="sxs-lookup"><span data-stu-id="41e74-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="41e74-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="41e74-127">Request body</span></span>
<span data-ttu-id="41e74-128">在请求正文中，提供 androidWorkProfileGeneralDeviceConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="41e74-128">In the request body, supply a JSON representation for the androidWorkProfileGeneralDeviceConfiguration object.</span></span>

<span data-ttu-id="41e74-129">下表显示创建 androidWorkProfileGeneralDeviceConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="41e74-129">The following table shows the properties that are required when you create the androidWorkProfileGeneralDeviceConfiguration.</span></span>

|<span data-ttu-id="41e74-130">属性</span><span class="sxs-lookup"><span data-stu-id="41e74-130">Property</span></span>|<span data-ttu-id="41e74-131">类型</span><span class="sxs-lookup"><span data-stu-id="41e74-131">Type</span></span>|<span data-ttu-id="41e74-132">说明</span><span class="sxs-lookup"><span data-stu-id="41e74-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="41e74-133">id</span><span class="sxs-lookup"><span data-stu-id="41e74-133">id</span></span>|<span data-ttu-id="41e74-134">String</span><span class="sxs-lookup"><span data-stu-id="41e74-134">String</span></span>|<span data-ttu-id="41e74-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="41e74-135">Key of the entity.</span></span> <span data-ttu-id="41e74-136">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="41e74-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="41e74-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="41e74-137">lastModifiedDateTime</span></span>|<span data-ttu-id="41e74-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="41e74-138">DateTimeOffset</span></span>|<span data-ttu-id="41e74-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="41e74-139">DateTime the object was last modified.</span></span> <span data-ttu-id="41e74-140">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="41e74-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="41e74-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="41e74-141">roleScopeTagIds</span></span>|<span data-ttu-id="41e74-142">字符串集合</span><span class="sxs-lookup"><span data-stu-id="41e74-142">String collection</span></span>|<span data-ttu-id="41e74-143">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="41e74-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="41e74-144">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="41e74-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="41e74-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="41e74-145">supportsScopeTags</span></span>|<span data-ttu-id="41e74-146">布尔</span><span class="sxs-lookup"><span data-stu-id="41e74-146">Boolean</span></span>|<span data-ttu-id="41e74-147">指示基础设备配置是否支持分配范围标记。</span><span class="sxs-lookup"><span data-stu-id="41e74-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="41e74-148">如果此值为 false 且实体对范围用户不可见，则不允许分配给 ScopeTags 属性。</span><span class="sxs-lookup"><span data-stu-id="41e74-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="41e74-149">这适用于在 Silverlight 中创建的旧策略，可通过在 Azure 门户中删除和重新创建策略来解决。</span><span class="sxs-lookup"><span data-stu-id="41e74-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="41e74-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="41e74-150">This property is read-only.</span></span> <span data-ttu-id="41e74-151">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="41e74-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="41e74-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="41e74-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="41e74-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="41e74-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="41e74-154">此策略的操作系统版本适用性。</span><span class="sxs-lookup"><span data-stu-id="41e74-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="41e74-155">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="41e74-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="41e74-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="41e74-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="41e74-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="41e74-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="41e74-158">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="41e74-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="41e74-159">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="41e74-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="41e74-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="41e74-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="41e74-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="41e74-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="41e74-162">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="41e74-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="41e74-163">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="41e74-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="41e74-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="41e74-164">createdDateTime</span></span>|<span data-ttu-id="41e74-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="41e74-165">DateTimeOffset</span></span>|<span data-ttu-id="41e74-166">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="41e74-166">DateTime the object was created.</span></span> <span data-ttu-id="41e74-167">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="41e74-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="41e74-168">说明</span><span class="sxs-lookup"><span data-stu-id="41e74-168">description</span></span>|<span data-ttu-id="41e74-169">String</span><span class="sxs-lookup"><span data-stu-id="41e74-169">String</span></span>|<span data-ttu-id="41e74-170">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="41e74-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="41e74-171">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="41e74-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="41e74-172">displayName</span><span class="sxs-lookup"><span data-stu-id="41e74-172">displayName</span></span>|<span data-ttu-id="41e74-173">String</span><span class="sxs-lookup"><span data-stu-id="41e74-173">String</span></span>|<span data-ttu-id="41e74-174">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="41e74-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="41e74-175">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="41e74-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="41e74-176">version</span><span class="sxs-lookup"><span data-stu-id="41e74-176">version</span></span>|<span data-ttu-id="41e74-177">Int32</span><span class="sxs-lookup"><span data-stu-id="41e74-177">Int32</span></span>|<span data-ttu-id="41e74-178">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="41e74-178">Version of the device configuration.</span></span> <span data-ttu-id="41e74-179">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="41e74-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="41e74-180">passwordBlockFaceUnlock</span><span class="sxs-lookup"><span data-stu-id="41e74-180">passwordBlockFaceUnlock</span></span>|<span data-ttu-id="41e74-181">布尔</span><span class="sxs-lookup"><span data-stu-id="41e74-181">Boolean</span></span>|<span data-ttu-id="41e74-182">指示是否阻止人脸解锁。</span><span class="sxs-lookup"><span data-stu-id="41e74-182">Indicates whether or not to block face unlock.</span></span>|
|<span data-ttu-id="41e74-183">passwordBlockFingerprintUnlock</span><span class="sxs-lookup"><span data-stu-id="41e74-183">passwordBlockFingerprintUnlock</span></span>|<span data-ttu-id="41e74-184">Boolean</span><span class="sxs-lookup"><span data-stu-id="41e74-184">Boolean</span></span>|<span data-ttu-id="41e74-185">指示是否阻止指纹解锁。</span><span class="sxs-lookup"><span data-stu-id="41e74-185">Indicates whether or not to block fingerprint unlock.</span></span>|
|<span data-ttu-id="41e74-186">passwordBlockIrisUnlock</span><span class="sxs-lookup"><span data-stu-id="41e74-186">passwordBlockIrisUnlock</span></span>|<span data-ttu-id="41e74-187">布尔</span><span class="sxs-lookup"><span data-stu-id="41e74-187">Boolean</span></span>|<span data-ttu-id="41e74-188">指示是否阻止虹膜解锁。</span><span class="sxs-lookup"><span data-stu-id="41e74-188">Indicates whether or not to block iris unlock.</span></span>|
|<span data-ttu-id="41e74-189">passwordBlockTrustAgents</span><span class="sxs-lookup"><span data-stu-id="41e74-189">passwordBlockTrustAgents</span></span>|<span data-ttu-id="41e74-190">Boolean</span><span class="sxs-lookup"><span data-stu-id="41e74-190">Boolean</span></span>|<span data-ttu-id="41e74-191">指示是否阻止 Smart Lock 和其他信任代理。</span><span class="sxs-lookup"><span data-stu-id="41e74-191">Indicates whether or not to block Smart Lock and other trust agents.</span></span>|
|<span data-ttu-id="41e74-192">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="41e74-192">passwordExpirationDays</span></span>|<span data-ttu-id="41e74-193">Int32</span><span class="sxs-lookup"><span data-stu-id="41e74-193">Int32</span></span>|<span data-ttu-id="41e74-194">密码过期前的天数。</span><span class="sxs-lookup"><span data-stu-id="41e74-194">Number of days before the password expires.</span></span> <span data-ttu-id="41e74-195">有效值为 1 至 365。</span><span class="sxs-lookup"><span data-stu-id="41e74-195">Valid values 1 to 365</span></span>|
|<span data-ttu-id="41e74-196">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="41e74-196">passwordMinimumLength</span></span>|<span data-ttu-id="41e74-197">Int32</span><span class="sxs-lookup"><span data-stu-id="41e74-197">Int32</span></span>|<span data-ttu-id="41e74-198">密码的最小长度。</span><span class="sxs-lookup"><span data-stu-id="41e74-198">Minimum length of passwords.</span></span> <span data-ttu-id="41e74-199">有效值为 4 至 16</span><span class="sxs-lookup"><span data-stu-id="41e74-199">Valid values 4 to 16</span></span>|
|<span data-ttu-id="41e74-200">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="41e74-200">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="41e74-201">Int32</span><span class="sxs-lookup"><span data-stu-id="41e74-201">Int32</span></span>|<span data-ttu-id="41e74-202">屏幕超时之前的不活动分钟数。</span><span class="sxs-lookup"><span data-stu-id="41e74-202">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="41e74-203">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="41e74-203">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="41e74-204">Int32</span><span class="sxs-lookup"><span data-stu-id="41e74-204">Int32</span></span>|<span data-ttu-id="41e74-205">要阻止的以前密码的数量。</span><span class="sxs-lookup"><span data-stu-id="41e74-205">Number of previous passwords to block.</span></span> <span data-ttu-id="41e74-206">有效值为 0 至 24</span><span class="sxs-lookup"><span data-stu-id="41e74-206">Valid values 0 to 24</span></span>|
|<span data-ttu-id="41e74-207">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="41e74-207">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="41e74-208">Int32</span><span class="sxs-lookup"><span data-stu-id="41e74-208">Int32</span></span>|<span data-ttu-id="41e74-209">恢复出厂设置之前允许登录失败的次数。</span><span class="sxs-lookup"><span data-stu-id="41e74-209">Number of sign in failures allowed before factory reset.</span></span> <span data-ttu-id="41e74-210">有效值 1 到 16</span><span class="sxs-lookup"><span data-stu-id="41e74-210">Valid values 1 to 16</span></span>|
|<span data-ttu-id="41e74-211">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="41e74-211">passwordRequiredType</span></span>|[<span data-ttu-id="41e74-212">androidWorkProfileRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="41e74-212">androidWorkProfileRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androidworkprofilerequiredpasswordtype.md)|<span data-ttu-id="41e74-213">必需的密码类型。</span><span class="sxs-lookup"><span data-stu-id="41e74-213">Type of password that is required.</span></span> <span data-ttu-id="41e74-214">可取值为：`deviceDefault`、`lowSecurityBiometric`、`required`、`atLeastNumeric`、`numericComplex`、`atLeastAlphabetic`、`atLeastAlphanumeric`、`alphanumericWithSymbols`。</span><span class="sxs-lookup"><span data-stu-id="41e74-214">Possible values are: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric`, `alphanumericWithSymbols`.</span></span>|
|<span data-ttu-id="41e74-215">workProfileAllowAppInstallsFromUnknownSources</span><span class="sxs-lookup"><span data-stu-id="41e74-215">workProfileAllowAppInstallsFromUnknownSources</span></span>|<span data-ttu-id="41e74-216">布尔</span><span class="sxs-lookup"><span data-stu-id="41e74-216">Boolean</span></span>|<span data-ttu-id="41e74-217">指示是否允许安装来自未知源的应用。</span><span class="sxs-lookup"><span data-stu-id="41e74-217">Indicates whether to allow installation of apps from unknown sources.</span></span>|
|<span data-ttu-id="41e74-218">workProfileDataSharingType</span><span class="sxs-lookup"><span data-stu-id="41e74-218">workProfileDataSharingType</span></span>|[<span data-ttu-id="41e74-219">androidWorkProfileCrossProfileDataSharingType</span><span class="sxs-lookup"><span data-stu-id="41e74-219">androidWorkProfileCrossProfileDataSharingType</span></span>](../resources/intune-deviceconfig-androidworkprofilecrossprofiledatasharingtype.md)|<span data-ttu-id="41e74-220">允许的数据共享类型。</span><span class="sxs-lookup"><span data-stu-id="41e74-220">Type of data sharing that is allowed.</span></span> <span data-ttu-id="41e74-221">可取值为：`deviceDefault`、`preventAny`、`allowPersonalToWork`、`noRestrictions`。</span><span class="sxs-lookup"><span data-stu-id="41e74-221">Possible values are: `deviceDefault`, `preventAny`, `allowPersonalToWork`, `noRestrictions`.</span></span>|
|<span data-ttu-id="41e74-222">workProfileBlockNotificationsWhileDeviceLocked</span><span class="sxs-lookup"><span data-stu-id="41e74-222">workProfileBlockNotificationsWhileDeviceLocked</span></span>|<span data-ttu-id="41e74-223">布尔</span><span class="sxs-lookup"><span data-stu-id="41e74-223">Boolean</span></span>|<span data-ttu-id="41e74-224">指示设备锁定时是否阻止通知。</span><span class="sxs-lookup"><span data-stu-id="41e74-224">Indicates whether or not to block notifications while device locked.</span></span>|
|<span data-ttu-id="41e74-225">workProfileBlockAddingAccounts</span><span class="sxs-lookup"><span data-stu-id="41e74-225">workProfileBlockAddingAccounts</span></span>|<span data-ttu-id="41e74-226">布尔</span><span class="sxs-lookup"><span data-stu-id="41e74-226">Boolean</span></span>|<span data-ttu-id="41e74-227">阻止用户在工作配置文件中添加/删除帐户。</span><span class="sxs-lookup"><span data-stu-id="41e74-227">Block users from adding/removing accounts in work profile.</span></span>|
|<span data-ttu-id="41e74-228">workProfileBluetoothEnableContactSharing</span><span class="sxs-lookup"><span data-stu-id="41e74-228">workProfileBluetoothEnableContactSharing</span></span>|<span data-ttu-id="41e74-229">布尔</span><span class="sxs-lookup"><span data-stu-id="41e74-229">Boolean</span></span>|<span data-ttu-id="41e74-230">允许蓝牙设备访问企业联系人。</span><span class="sxs-lookup"><span data-stu-id="41e74-230">Allow bluetooth devices to access enterprise contacts.</span></span>|
|<span data-ttu-id="41e74-231">workProfileBlockScreenCapture</span><span class="sxs-lookup"><span data-stu-id="41e74-231">workProfileBlockScreenCapture</span></span>|<span data-ttu-id="41e74-232">布尔</span><span class="sxs-lookup"><span data-stu-id="41e74-232">Boolean</span></span>|<span data-ttu-id="41e74-233">阻止工作配置文件中的屏幕捕获。</span><span class="sxs-lookup"><span data-stu-id="41e74-233">Block screen capture in work profile.</span></span>|
|<span data-ttu-id="41e74-234">workProfileBlockCrossProfileCallerId</span><span class="sxs-lookup"><span data-stu-id="41e74-234">workProfileBlockCrossProfileCallerId</span></span>|<span data-ttu-id="41e74-235">布尔</span><span class="sxs-lookup"><span data-stu-id="41e74-235">Boolean</span></span>|<span data-ttu-id="41e74-236">阻止在个人配置文件中显示工作配置文件调用方 ID。</span><span class="sxs-lookup"><span data-stu-id="41e74-236">Block display work profile caller ID in personal profile.</span></span>|
|<span data-ttu-id="41e74-237">workProfileBlockCamera</span><span class="sxs-lookup"><span data-stu-id="41e74-237">workProfileBlockCamera</span></span>|<span data-ttu-id="41e74-238">布尔</span><span class="sxs-lookup"><span data-stu-id="41e74-238">Boolean</span></span>|<span data-ttu-id="41e74-239">阻止工作配置文件相机。</span><span class="sxs-lookup"><span data-stu-id="41e74-239">Block work profile camera.</span></span>|
|<span data-ttu-id="41e74-240">workProfileBlockCrossProfileContactsSearch</span><span class="sxs-lookup"><span data-stu-id="41e74-240">workProfileBlockCrossProfileContactsSearch</span></span>|<span data-ttu-id="41e74-241">布尔</span><span class="sxs-lookup"><span data-stu-id="41e74-241">Boolean</span></span>|<span data-ttu-id="41e74-242">阻止工作配置文件联系人在个人配置文件中的可用性。</span><span class="sxs-lookup"><span data-stu-id="41e74-242">Block work profile contacts availability in personal profile.</span></span>|
|<span data-ttu-id="41e74-243">workProfileBlockCrossProfileCopyPaste</span><span class="sxs-lookup"><span data-stu-id="41e74-243">workProfileBlockCrossProfileCopyPaste</span></span>|<span data-ttu-id="41e74-244">布尔</span><span class="sxs-lookup"><span data-stu-id="41e74-244">Boolean</span></span>|<span data-ttu-id="41e74-245">指示是否启用设置禁止跨配置文件复制/粘贴的布尔值。</span><span class="sxs-lookup"><span data-stu-id="41e74-245">Boolean that indicates if the setting disallow cross profile copy/paste is enabled.</span></span>|
|<span data-ttu-id="41e74-246">workProfileDefaultAppPermissionPolicy</span><span class="sxs-lookup"><span data-stu-id="41e74-246">workProfileDefaultAppPermissionPolicy</span></span>|[<span data-ttu-id="41e74-247">androidWorkProfileDefaultAppPermissionPolicyType</span><span class="sxs-lookup"><span data-stu-id="41e74-247">androidWorkProfileDefaultAppPermissionPolicyType</span></span>](../resources/intune-deviceconfig-androidworkprofiledefaultapppermissionpolicytype.md)|<span data-ttu-id="41e74-248">必需的密码类型。</span><span class="sxs-lookup"><span data-stu-id="41e74-248">Type of password that is required.</span></span> <span data-ttu-id="41e74-249">可取值为：`deviceDefault`、`prompt`、`autoGrant`、`autoDeny`。</span><span class="sxs-lookup"><span data-stu-id="41e74-249">Possible values are: `deviceDefault`, `prompt`, `autoGrant`, `autoDeny`.</span></span>|
|<span data-ttu-id="41e74-250">workProfilePasswordBlockFaceUnlock</span><span class="sxs-lookup"><span data-stu-id="41e74-250">workProfilePasswordBlockFaceUnlock</span></span>|<span data-ttu-id="41e74-251">布尔</span><span class="sxs-lookup"><span data-stu-id="41e74-251">Boolean</span></span>|<span data-ttu-id="41e74-252">指示是否阻止工作配置文件的人脸解锁。</span><span class="sxs-lookup"><span data-stu-id="41e74-252">Indicates whether or not to block face unlock for work profile.</span></span>|
|<span data-ttu-id="41e74-253">workProfilePasswordBlockFingerprintUnlock</span><span class="sxs-lookup"><span data-stu-id="41e74-253">workProfilePasswordBlockFingerprintUnlock</span></span>|<span data-ttu-id="41e74-254">布尔</span><span class="sxs-lookup"><span data-stu-id="41e74-254">Boolean</span></span>|<span data-ttu-id="41e74-255">指示是否阻止工作配置文件的指纹解锁。</span><span class="sxs-lookup"><span data-stu-id="41e74-255">Indicates whether or not to block fingerprint unlock for work profile.</span></span>|
|<span data-ttu-id="41e74-256">workProfilePasswordBlockIrisUnlock</span><span class="sxs-lookup"><span data-stu-id="41e74-256">workProfilePasswordBlockIrisUnlock</span></span>|<span data-ttu-id="41e74-257">布尔</span><span class="sxs-lookup"><span data-stu-id="41e74-257">Boolean</span></span>|<span data-ttu-id="41e74-258">指示是否阻止工作配置文件的虹膜解锁。</span><span class="sxs-lookup"><span data-stu-id="41e74-258">Indicates whether or not to block iris unlock for work profile.</span></span>|
|<span data-ttu-id="41e74-259">workProfilePasswordBlockTrustAgents</span><span class="sxs-lookup"><span data-stu-id="41e74-259">workProfilePasswordBlockTrustAgents</span></span>|<span data-ttu-id="41e74-260">布尔</span><span class="sxs-lookup"><span data-stu-id="41e74-260">Boolean</span></span>|<span data-ttu-id="41e74-261">指示是否阻止工作配置文件的智能锁定和其他信任代理。</span><span class="sxs-lookup"><span data-stu-id="41e74-261">Indicates whether or not to block Smart Lock and other trust agents for work profile.</span></span>|
|<span data-ttu-id="41e74-262">workProfilePasswordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="41e74-262">workProfilePasswordExpirationDays</span></span>|<span data-ttu-id="41e74-263">Int32</span><span class="sxs-lookup"><span data-stu-id="41e74-263">Int32</span></span>|<span data-ttu-id="41e74-264">工作配置文件密码过期前的天数。</span><span class="sxs-lookup"><span data-stu-id="41e74-264">Number of days before the work profile password expires.</span></span> <span data-ttu-id="41e74-265">有效值为 1 至 365。</span><span class="sxs-lookup"><span data-stu-id="41e74-265">Valid values 1 to 365</span></span>|
|<span data-ttu-id="41e74-266">workProfilePasswordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="41e74-266">workProfilePasswordMinimumLength</span></span>|<span data-ttu-id="41e74-267">Int32</span><span class="sxs-lookup"><span data-stu-id="41e74-267">Int32</span></span>|<span data-ttu-id="41e74-268">工作配置文件密码的最小长度。</span><span class="sxs-lookup"><span data-stu-id="41e74-268">Minimum length of work profile password.</span></span> <span data-ttu-id="41e74-269">有效值为 4 至 16</span><span class="sxs-lookup"><span data-stu-id="41e74-269">Valid values 4 to 16</span></span>|
|<span data-ttu-id="41e74-270">workProfilePasswordMinNumericCharacters</span><span class="sxs-lookup"><span data-stu-id="41e74-270">workProfilePasswordMinNumericCharacters</span></span>|<span data-ttu-id="41e74-271">Int32</span><span class="sxs-lookup"><span data-stu-id="41e74-271">Int32</span></span>|<span data-ttu-id="41e74-272">工作配置文件密码中所需的数字字符的最小值。</span><span class="sxs-lookup"><span data-stu-id="41e74-272">Minimum # of numeric characters required in work profile password.</span></span> <span data-ttu-id="41e74-273">有效值 1 到 10</span><span class="sxs-lookup"><span data-stu-id="41e74-273">Valid values 1 to 10</span></span>|
|<span data-ttu-id="41e74-274">workProfilePasswordMinNonLetterCharacters</span><span class="sxs-lookup"><span data-stu-id="41e74-274">workProfilePasswordMinNonLetterCharacters</span></span>|<span data-ttu-id="41e74-275">Int32</span><span class="sxs-lookup"><span data-stu-id="41e74-275">Int32</span></span>|<span data-ttu-id="41e74-276">工作配置文件密码中所需的非字母字符的最小值。</span><span class="sxs-lookup"><span data-stu-id="41e74-276">Minimum # of non-letter characters required in work profile password.</span></span> <span data-ttu-id="41e74-277">有效值 1 到 10</span><span class="sxs-lookup"><span data-stu-id="41e74-277">Valid values 1 to 10</span></span>|
|<span data-ttu-id="41e74-278">workProfilePasswordMinLetterCharacters</span><span class="sxs-lookup"><span data-stu-id="41e74-278">workProfilePasswordMinLetterCharacters</span></span>|<span data-ttu-id="41e74-279">Int32</span><span class="sxs-lookup"><span data-stu-id="41e74-279">Int32</span></span>|<span data-ttu-id="41e74-280">工作配置文件密码中要求的最小字母字符数。</span><span class="sxs-lookup"><span data-stu-id="41e74-280">Minimum # of letter characters required in work profile password.</span></span> <span data-ttu-id="41e74-281">有效值 1 到 10</span><span class="sxs-lookup"><span data-stu-id="41e74-281">Valid values 1 to 10</span></span>|
|<span data-ttu-id="41e74-282">workProfilePasswordMinLowerCaseCharacters</span><span class="sxs-lookup"><span data-stu-id="41e74-282">workProfilePasswordMinLowerCaseCharacters</span></span>|<span data-ttu-id="41e74-283">Int32</span><span class="sxs-lookup"><span data-stu-id="41e74-283">Int32</span></span>|<span data-ttu-id="41e74-284">工作配置文件密码中所需的小写字符的最小 # 。</span><span class="sxs-lookup"><span data-stu-id="41e74-284">Minimum # of lower-case characters required in work profile password.</span></span> <span data-ttu-id="41e74-285">有效值 1 到 10</span><span class="sxs-lookup"><span data-stu-id="41e74-285">Valid values 1 to 10</span></span>|
|<span data-ttu-id="41e74-286">workProfilePasswordMinUpperCaseCharacters</span><span class="sxs-lookup"><span data-stu-id="41e74-286">workProfilePasswordMinUpperCaseCharacters</span></span>|<span data-ttu-id="41e74-287">Int32</span><span class="sxs-lookup"><span data-stu-id="41e74-287">Int32</span></span>|<span data-ttu-id="41e74-288">工作配置文件密码中所需的大写字符的最小值。</span><span class="sxs-lookup"><span data-stu-id="41e74-288">Minimum # of upper-case characters required in work profile password.</span></span> <span data-ttu-id="41e74-289">有效值 1 到 10</span><span class="sxs-lookup"><span data-stu-id="41e74-289">Valid values 1 to 10</span></span>|
|<span data-ttu-id="41e74-290">workProfilePasswordMinSymbolCharacters</span><span class="sxs-lookup"><span data-stu-id="41e74-290">workProfilePasswordMinSymbolCharacters</span></span>|<span data-ttu-id="41e74-291">Int32</span><span class="sxs-lookup"><span data-stu-id="41e74-291">Int32</span></span>|<span data-ttu-id="41e74-292">工作配置文件密码中所需的符号的最小数量。</span><span class="sxs-lookup"><span data-stu-id="41e74-292">Minimum # of symbols required in work profile password.</span></span> <span data-ttu-id="41e74-293">有效值 1 到 10</span><span class="sxs-lookup"><span data-stu-id="41e74-293">Valid values 1 to 10</span></span>|
|<span data-ttu-id="41e74-294">workProfilePasswordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="41e74-294">workProfilePasswordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="41e74-295">Int32</span><span class="sxs-lookup"><span data-stu-id="41e74-295">Int32</span></span>|<span data-ttu-id="41e74-296">屏幕超时之前的不活动分钟数。</span><span class="sxs-lookup"><span data-stu-id="41e74-296">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="41e74-297">workProfilePasswordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="41e74-297">workProfilePasswordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="41e74-298">Int32</span><span class="sxs-lookup"><span data-stu-id="41e74-298">Int32</span></span>|<span data-ttu-id="41e74-299">要阻止的以前工作配置文件密码的数量。</span><span class="sxs-lookup"><span data-stu-id="41e74-299">Number of previous work profile passwords to block.</span></span> <span data-ttu-id="41e74-300">有效值为 0 至 24</span><span class="sxs-lookup"><span data-stu-id="41e74-300">Valid values 0 to 24</span></span>|
|<span data-ttu-id="41e74-301">workProfilePasswordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="41e74-301">workProfilePasswordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="41e74-302">Int32</span><span class="sxs-lookup"><span data-stu-id="41e74-302">Int32</span></span>|<span data-ttu-id="41e74-303">在删除工作配置文件和删除所有公司数据之前允许的登录失败次数。</span><span class="sxs-lookup"><span data-stu-id="41e74-303">Number of sign in failures allowed before work profile is removed and all corporate data deleted.</span></span> <span data-ttu-id="41e74-304">有效值 1 到 16</span><span class="sxs-lookup"><span data-stu-id="41e74-304">Valid values 1 to 16</span></span>|
|<span data-ttu-id="41e74-305">workProfilePasswordRequiredType</span><span class="sxs-lookup"><span data-stu-id="41e74-305">workProfilePasswordRequiredType</span></span>|[<span data-ttu-id="41e74-306">androidWorkProfileRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="41e74-306">androidWorkProfileRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androidworkprofilerequiredpasswordtype.md)|<span data-ttu-id="41e74-307">所需的工作配置文件密码类型。</span><span class="sxs-lookup"><span data-stu-id="41e74-307">Type of work profile password that is required.</span></span> <span data-ttu-id="41e74-308">可取值为：`deviceDefault`、`lowSecurityBiometric`、`required`、`atLeastNumeric`、`numericComplex`、`atLeastAlphabetic`、`atLeastAlphanumeric`、`alphanumericWithSymbols`。</span><span class="sxs-lookup"><span data-stu-id="41e74-308">Possible values are: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric`, `alphanumericWithSymbols`.</span></span>|
|<span data-ttu-id="41e74-309">workProfileRequirePassword</span><span class="sxs-lookup"><span data-stu-id="41e74-309">workProfileRequirePassword</span></span>|<span data-ttu-id="41e74-310">布尔</span><span class="sxs-lookup"><span data-stu-id="41e74-310">Boolean</span></span>|<span data-ttu-id="41e74-311">工作配置文件需要密码或不需要密码</span><span class="sxs-lookup"><span data-stu-id="41e74-311">Password is required or not for work profile</span></span>|
|<span data-ttu-id="41e74-312">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="41e74-312">securityRequireVerifyApps</span></span>|<span data-ttu-id="41e74-313">Boolean</span><span class="sxs-lookup"><span data-stu-id="41e74-313">Boolean</span></span>|<span data-ttu-id="41e74-314">要求启用 Android 验证应用功能。</span><span class="sxs-lookup"><span data-stu-id="41e74-314">Require the Android Verify apps feature is turned on.</span></span>|
|<span data-ttu-id="41e74-315">vpnAlwaysOnPackageIdentifier</span><span class="sxs-lookup"><span data-stu-id="41e74-315">vpnAlwaysOnPackageIdentifier</span></span>|<span data-ttu-id="41e74-316">String</span><span class="sxs-lookup"><span data-stu-id="41e74-316">String</span></span>|<span data-ttu-id="41e74-317">为始终打开的 VPN 启用锁定模式。</span><span class="sxs-lookup"><span data-stu-id="41e74-317">Enable lockdown mode for always-on VPN.</span></span>|
|<span data-ttu-id="41e74-318">vpnEnableAlwaysOnLockdownMode</span><span class="sxs-lookup"><span data-stu-id="41e74-318">vpnEnableAlwaysOnLockdownMode</span></span>|<span data-ttu-id="41e74-319">布尔</span><span class="sxs-lookup"><span data-stu-id="41e74-319">Boolean</span></span>|<span data-ttu-id="41e74-320">为始终打开的 VPN 启用锁定模式。</span><span class="sxs-lookup"><span data-stu-id="41e74-320">Enable lockdown mode for always-on VPN.</span></span>|
|<span data-ttu-id="41e74-321">workProfileAllowWidgets</span><span class="sxs-lookup"><span data-stu-id="41e74-321">workProfileAllowWidgets</span></span>|<span data-ttu-id="41e74-322">布尔</span><span class="sxs-lookup"><span data-stu-id="41e74-322">Boolean</span></span>|<span data-ttu-id="41e74-323">允许工作配置文件应用中的小部件。</span><span class="sxs-lookup"><span data-stu-id="41e74-323">Allow widgets from work profile apps.</span></span>|
|<span data-ttu-id="41e74-324">workProfileBlockPersonalAppInstallsFromUnknownSources</span><span class="sxs-lookup"><span data-stu-id="41e74-324">workProfileBlockPersonalAppInstallsFromUnknownSources</span></span>|<span data-ttu-id="41e74-325">布尔</span><span class="sxs-lookup"><span data-stu-id="41e74-325">Boolean</span></span>|<span data-ttu-id="41e74-326">阻止从个人配置文件中的未知源安装应用。</span><span class="sxs-lookup"><span data-stu-id="41e74-326">Prevent app installations from unknown sources in the personal profile.</span></span>|



## <a name="response"></a><span data-ttu-id="41e74-327">响应</span><span class="sxs-lookup"><span data-stu-id="41e74-327">Response</span></span>
<span data-ttu-id="41e74-328">如果成功，此方法在响应正文中返回响应代码和 `201 Created` [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="41e74-328">If successful, this method returns a `201 Created` response code and a [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="41e74-329">示例</span><span class="sxs-lookup"><span data-stu-id="41e74-329">Example</span></span>

### <a name="request"></a><span data-ttu-id="41e74-330">请求</span><span class="sxs-lookup"><span data-stu-id="41e74-330">Request</span></span>
<span data-ttu-id="41e74-331">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="41e74-331">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
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

### <a name="response"></a><span data-ttu-id="41e74-332">响应</span><span class="sxs-lookup"><span data-stu-id="41e74-332">Response</span></span>
<span data-ttu-id="41e74-p131">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="41e74-p131">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




