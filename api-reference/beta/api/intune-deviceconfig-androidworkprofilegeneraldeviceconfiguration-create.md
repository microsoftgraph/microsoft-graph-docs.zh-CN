---
title: 创建 androidWorkProfileGeneralDeviceConfiguration
description: 创建新的 androidWorkProfileGeneralDeviceConfiguration 对象。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 50ddaf160919e8f28bdd3db77cdae1873430febb
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/14/2019
ms.locfileid: "34969398"
---
# <a name="create-androidworkprofilegeneraldeviceconfiguration"></a><span data-ttu-id="4a94c-103">创建 androidWorkProfileGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="4a94c-103">Create androidWorkProfileGeneralDeviceConfiguration</span></span>

> <span data-ttu-id="4a94c-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="4a94c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4a94c-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="4a94c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4a94c-106">创建新的[androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="4a94c-106">Create a new [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4a94c-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="4a94c-107">Prerequisites</span></span>
<span data-ttu-id="4a94c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4a94c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4a94c-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="4a94c-110">Permission type</span></span>|<span data-ttu-id="4a94c-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="4a94c-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4a94c-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4a94c-112">Delegated (work or school account)</span></span>|<span data-ttu-id="4a94c-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4a94c-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="4a94c-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4a94c-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4a94c-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="4a94c-115">Not supported.</span></span>|
|<span data-ttu-id="4a94c-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="4a94c-116">Application</span></span>|<span data-ttu-id="4a94c-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="4a94c-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4a94c-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4a94c-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="4a94c-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="4a94c-119">Request headers</span></span>
|<span data-ttu-id="4a94c-120">标头</span><span class="sxs-lookup"><span data-stu-id="4a94c-120">Header</span></span>|<span data-ttu-id="4a94c-121">值</span><span class="sxs-lookup"><span data-stu-id="4a94c-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4a94c-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="4a94c-122">Authorization</span></span>|<span data-ttu-id="4a94c-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="4a94c-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4a94c-124">接受</span><span class="sxs-lookup"><span data-stu-id="4a94c-124">Accept</span></span>|<span data-ttu-id="4a94c-125">application/json</span><span class="sxs-lookup"><span data-stu-id="4a94c-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4a94c-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="4a94c-126">Request body</span></span>
<span data-ttu-id="4a94c-127">在请求正文中, 提供 androidWorkProfileGeneralDeviceConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4a94c-127">In the request body, supply a JSON representation for the androidWorkProfileGeneralDeviceConfiguration object.</span></span>

<span data-ttu-id="4a94c-128">下表显示创建 androidWorkProfileGeneralDeviceConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="4a94c-128">The following table shows the properties that are required when you create the androidWorkProfileGeneralDeviceConfiguration.</span></span>

|<span data-ttu-id="4a94c-129">属性</span><span class="sxs-lookup"><span data-stu-id="4a94c-129">Property</span></span>|<span data-ttu-id="4a94c-130">类型</span><span class="sxs-lookup"><span data-stu-id="4a94c-130">Type</span></span>|<span data-ttu-id="4a94c-131">说明</span><span class="sxs-lookup"><span data-stu-id="4a94c-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4a94c-132">id</span><span class="sxs-lookup"><span data-stu-id="4a94c-132">id</span></span>|<span data-ttu-id="4a94c-133">字符串</span><span class="sxs-lookup"><span data-stu-id="4a94c-133">String</span></span>|<span data-ttu-id="4a94c-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="4a94c-134">Key of the entity.</span></span> <span data-ttu-id="4a94c-135">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4a94c-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4a94c-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4a94c-136">lastModifiedDateTime</span></span>|<span data-ttu-id="4a94c-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4a94c-137">DateTimeOffset</span></span>|<span data-ttu-id="4a94c-138">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="4a94c-138">DateTime the object was last modified.</span></span> <span data-ttu-id="4a94c-139">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4a94c-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4a94c-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="4a94c-140">roleScopeTagIds</span></span>|<span data-ttu-id="4a94c-141">String collection</span><span class="sxs-lookup"><span data-stu-id="4a94c-141">String collection</span></span>|<span data-ttu-id="4a94c-142">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="4a94c-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="4a94c-143">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4a94c-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4a94c-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="4a94c-144">supportsScopeTags</span></span>|<span data-ttu-id="4a94c-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="4a94c-145">Boolean</span></span>|<span data-ttu-id="4a94c-146">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="4a94c-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="4a94c-147">如果此值为 false, 则不允许分配给 ScopeTags 属性, 并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="4a94c-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="4a94c-148">这适用于在 Silverlight 中创建的旧版策略, 可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="4a94c-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="4a94c-149">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="4a94c-149">This property is read-only.</span></span> <span data-ttu-id="4a94c-150">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4a94c-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4a94c-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="4a94c-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="4a94c-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="4a94c-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="4a94c-153">适用于此策略的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="4a94c-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="4a94c-154">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4a94c-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4a94c-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="4a94c-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="4a94c-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="4a94c-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="4a94c-157">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="4a94c-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="4a94c-158">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4a94c-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4a94c-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="4a94c-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="4a94c-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="4a94c-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="4a94c-161">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="4a94c-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="4a94c-162">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4a94c-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4a94c-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="4a94c-163">createdDateTime</span></span>|<span data-ttu-id="4a94c-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4a94c-164">DateTimeOffset</span></span>|<span data-ttu-id="4a94c-165">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="4a94c-165">DateTime the object was created.</span></span> <span data-ttu-id="4a94c-166">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4a94c-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4a94c-167">说明</span><span class="sxs-lookup"><span data-stu-id="4a94c-167">description</span></span>|<span data-ttu-id="4a94c-168">String</span><span class="sxs-lookup"><span data-stu-id="4a94c-168">String</span></span>|<span data-ttu-id="4a94c-169">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="4a94c-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="4a94c-170">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4a94c-170">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4a94c-171">displayName</span><span class="sxs-lookup"><span data-stu-id="4a94c-171">displayName</span></span>|<span data-ttu-id="4a94c-172">String</span><span class="sxs-lookup"><span data-stu-id="4a94c-172">String</span></span>|<span data-ttu-id="4a94c-173">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="4a94c-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="4a94c-174">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4a94c-174">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4a94c-175">version</span><span class="sxs-lookup"><span data-stu-id="4a94c-175">version</span></span>|<span data-ttu-id="4a94c-176">Int32</span><span class="sxs-lookup"><span data-stu-id="4a94c-176">Int32</span></span>|<span data-ttu-id="4a94c-177">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="4a94c-177">Version of the device configuration.</span></span> <span data-ttu-id="4a94c-178">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4a94c-178">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4a94c-179">passwordBlockFingerprintUnlock</span><span class="sxs-lookup"><span data-stu-id="4a94c-179">passwordBlockFingerprintUnlock</span></span>|<span data-ttu-id="4a94c-180">Boolean</span><span class="sxs-lookup"><span data-stu-id="4a94c-180">Boolean</span></span>|<span data-ttu-id="4a94c-181">指示是否阻止指纹解锁。</span><span class="sxs-lookup"><span data-stu-id="4a94c-181">Indicates whether or not to block fingerprint unlock.</span></span>|
|<span data-ttu-id="4a94c-182">passwordBlockTrustAgents</span><span class="sxs-lookup"><span data-stu-id="4a94c-182">passwordBlockTrustAgents</span></span>|<span data-ttu-id="4a94c-183">Boolean</span><span class="sxs-lookup"><span data-stu-id="4a94c-183">Boolean</span></span>|<span data-ttu-id="4a94c-184">指示是否阻止 Smart Lock 和其他信任代理。</span><span class="sxs-lookup"><span data-stu-id="4a94c-184">Indicates whether or not to block Smart Lock and other trust agents.</span></span>|
|<span data-ttu-id="4a94c-185">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="4a94c-185">passwordExpirationDays</span></span>|<span data-ttu-id="4a94c-186">Int32</span><span class="sxs-lookup"><span data-stu-id="4a94c-186">Int32</span></span>|<span data-ttu-id="4a94c-187">密码过期前的天数。</span><span class="sxs-lookup"><span data-stu-id="4a94c-187">Number of days before the password expires.</span></span> <span data-ttu-id="4a94c-188">有效值为 1 至 365。</span><span class="sxs-lookup"><span data-stu-id="4a94c-188">Valid values 1 to 365</span></span>|
|<span data-ttu-id="4a94c-189">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="4a94c-189">passwordMinimumLength</span></span>|<span data-ttu-id="4a94c-190">Int32</span><span class="sxs-lookup"><span data-stu-id="4a94c-190">Int32</span></span>|<span data-ttu-id="4a94c-191">密码的最小长度。</span><span class="sxs-lookup"><span data-stu-id="4a94c-191">Minimum length of passwords.</span></span> <span data-ttu-id="4a94c-192">有效值为 4 至 16</span><span class="sxs-lookup"><span data-stu-id="4a94c-192">Valid values 4 to 16</span></span>|
|<span data-ttu-id="4a94c-193">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="4a94c-193">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="4a94c-194">Int32</span><span class="sxs-lookup"><span data-stu-id="4a94c-194">Int32</span></span>|<span data-ttu-id="4a94c-195">屏幕超时之前的不活动分钟数。</span><span class="sxs-lookup"><span data-stu-id="4a94c-195">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="4a94c-196">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="4a94c-196">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="4a94c-197">Int32</span><span class="sxs-lookup"><span data-stu-id="4a94c-197">Int32</span></span>|<span data-ttu-id="4a94c-198">要阻止的以前密码的数量。</span><span class="sxs-lookup"><span data-stu-id="4a94c-198">Number of previous passwords to block.</span></span> <span data-ttu-id="4a94c-199">有效值为 0 至 24</span><span class="sxs-lookup"><span data-stu-id="4a94c-199">Valid values 0 to 24</span></span>|
|<span data-ttu-id="4a94c-200">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="4a94c-200">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="4a94c-201">Int32</span><span class="sxs-lookup"><span data-stu-id="4a94c-201">Int32</span></span>|<span data-ttu-id="4a94c-202">恢复出厂设置之前允许登录失败的次数。</span><span class="sxs-lookup"><span data-stu-id="4a94c-202">Number of sign in failures allowed before factory reset.</span></span> <span data-ttu-id="4a94c-203">有效值为1至16</span><span class="sxs-lookup"><span data-stu-id="4a94c-203">Valid values 1 to 16</span></span>|
|<span data-ttu-id="4a94c-204">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="4a94c-204">passwordRequiredType</span></span>|[<span data-ttu-id="4a94c-205">androidWorkProfileRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="4a94c-205">androidWorkProfileRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androidworkprofilerequiredpasswordtype.md)|<span data-ttu-id="4a94c-206">必需的密码类型。</span><span class="sxs-lookup"><span data-stu-id="4a94c-206">Type of password that is required.</span></span> <span data-ttu-id="4a94c-207">可取值为：`deviceDefault`、`lowSecurityBiometric`、`required`、`atLeastNumeric`、`numericComplex`、`atLeastAlphabetic`、`atLeastAlphanumeric`、`alphanumericWithSymbols`。</span><span class="sxs-lookup"><span data-stu-id="4a94c-207">Possible values are: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric`, `alphanumericWithSymbols`.</span></span>|
|<span data-ttu-id="4a94c-208">workProfileDataSharingType</span><span class="sxs-lookup"><span data-stu-id="4a94c-208">workProfileDataSharingType</span></span>|[<span data-ttu-id="4a94c-209">androidWorkProfileCrossProfileDataSharingType</span><span class="sxs-lookup"><span data-stu-id="4a94c-209">androidWorkProfileCrossProfileDataSharingType</span></span>](../resources/intune-deviceconfig-androidworkprofilecrossprofiledatasharingtype.md)|<span data-ttu-id="4a94c-210">允许的数据共享类型。</span><span class="sxs-lookup"><span data-stu-id="4a94c-210">Type of data sharing that is allowed.</span></span> <span data-ttu-id="4a94c-211">可取值为：`deviceDefault`、`preventAny`、`allowPersonalToWork`、`noRestrictions`。</span><span class="sxs-lookup"><span data-stu-id="4a94c-211">Possible values are: `deviceDefault`, `preventAny`, `allowPersonalToWork`, `noRestrictions`.</span></span>|
|<span data-ttu-id="4a94c-212">workProfileBlockNotificationsWhileDeviceLocked</span><span class="sxs-lookup"><span data-stu-id="4a94c-212">workProfileBlockNotificationsWhileDeviceLocked</span></span>|<span data-ttu-id="4a94c-213">Boolean</span><span class="sxs-lookup"><span data-stu-id="4a94c-213">Boolean</span></span>|<span data-ttu-id="4a94c-214">指示在设备锁定时是否阻止通知。</span><span class="sxs-lookup"><span data-stu-id="4a94c-214">Indicates whether or not to block notifications while device locked.</span></span>|
|<span data-ttu-id="4a94c-215">workProfileBlockAddingAccounts</span><span class="sxs-lookup"><span data-stu-id="4a94c-215">workProfileBlockAddingAccounts</span></span>|<span data-ttu-id="4a94c-216">Boolean</span><span class="sxs-lookup"><span data-stu-id="4a94c-216">Boolean</span></span>|<span data-ttu-id="4a94c-217">阻止用户在工作配置文件中添加/删除帐户。</span><span class="sxs-lookup"><span data-stu-id="4a94c-217">Block users from adding/removing accounts in work profile.</span></span>|
|<span data-ttu-id="4a94c-218">workProfileBluetoothEnableContactSharing</span><span class="sxs-lookup"><span data-stu-id="4a94c-218">workProfileBluetoothEnableContactSharing</span></span>|<span data-ttu-id="4a94c-219">Boolean</span><span class="sxs-lookup"><span data-stu-id="4a94c-219">Boolean</span></span>|<span data-ttu-id="4a94c-220">允许蓝牙设备访问企业联系人。</span><span class="sxs-lookup"><span data-stu-id="4a94c-220">Allow bluetooth devices to access enterprise contacts.</span></span>|
|<span data-ttu-id="4a94c-221">workProfileBlockScreenCapture</span><span class="sxs-lookup"><span data-stu-id="4a94c-221">workProfileBlockScreenCapture</span></span>|<span data-ttu-id="4a94c-222">Boolean</span><span class="sxs-lookup"><span data-stu-id="4a94c-222">Boolean</span></span>|<span data-ttu-id="4a94c-223">在工作配置文件中阻止屏幕捕获。</span><span class="sxs-lookup"><span data-stu-id="4a94c-223">Block screen capture in work profile.</span></span>|
|<span data-ttu-id="4a94c-224">workProfileBlockCrossProfileCallerId</span><span class="sxs-lookup"><span data-stu-id="4a94c-224">workProfileBlockCrossProfileCallerId</span></span>|<span data-ttu-id="4a94c-225">Boolean</span><span class="sxs-lookup"><span data-stu-id="4a94c-225">Boolean</span></span>|<span data-ttu-id="4a94c-226">阻止显示个人配置文件中的工作配置文件呼叫者 ID。</span><span class="sxs-lookup"><span data-stu-id="4a94c-226">Block display work profile caller ID in personal profile.</span></span>|
|<span data-ttu-id="4a94c-227">workProfileBlockCamera</span><span class="sxs-lookup"><span data-stu-id="4a94c-227">workProfileBlockCamera</span></span>|<span data-ttu-id="4a94c-228">Boolean</span><span class="sxs-lookup"><span data-stu-id="4a94c-228">Boolean</span></span>|<span data-ttu-id="4a94c-229">阻止工作配置文件相机。</span><span class="sxs-lookup"><span data-stu-id="4a94c-229">Block work profile camera.</span></span>|
|<span data-ttu-id="4a94c-230">workProfileBlockCrossProfileContactsSearch</span><span class="sxs-lookup"><span data-stu-id="4a94c-230">workProfileBlockCrossProfileContactsSearch</span></span>|<span data-ttu-id="4a94c-231">Boolean</span><span class="sxs-lookup"><span data-stu-id="4a94c-231">Boolean</span></span>|<span data-ttu-id="4a94c-232">阻止个人配置文件中的工作配置文件联系人可用性。</span><span class="sxs-lookup"><span data-stu-id="4a94c-232">Block work profile contacts availability in personal profile.</span></span>|
|<span data-ttu-id="4a94c-233">workProfileBlockCrossProfileCopyPaste</span><span class="sxs-lookup"><span data-stu-id="4a94c-233">workProfileBlockCrossProfileCopyPaste</span></span>|<span data-ttu-id="4a94c-234">Boolean</span><span class="sxs-lookup"><span data-stu-id="4a94c-234">Boolean</span></span>|<span data-ttu-id="4a94c-235">指示是否启用 "禁用跨配置文件复制/粘贴" 设置的 Boolean。</span><span class="sxs-lookup"><span data-stu-id="4a94c-235">Boolean that indicates if the setting disallow cross profile copy/paste is enabled.</span></span>|
|<span data-ttu-id="4a94c-236">workProfileDefaultAppPermissionPolicy</span><span class="sxs-lookup"><span data-stu-id="4a94c-236">workProfileDefaultAppPermissionPolicy</span></span>|[<span data-ttu-id="4a94c-237">androidWorkProfileDefaultAppPermissionPolicyType</span><span class="sxs-lookup"><span data-stu-id="4a94c-237">androidWorkProfileDefaultAppPermissionPolicyType</span></span>](../resources/intune-deviceconfig-androidworkprofiledefaultapppermissionpolicytype.md)|<span data-ttu-id="4a94c-238">必需的密码类型。</span><span class="sxs-lookup"><span data-stu-id="4a94c-238">Type of password that is required.</span></span> <span data-ttu-id="4a94c-239">可取值为：`deviceDefault`、`prompt`、`autoGrant`、`autoDeny`。</span><span class="sxs-lookup"><span data-stu-id="4a94c-239">Possible values are: `deviceDefault`, `prompt`, `autoGrant`, `autoDeny`.</span></span>|
|<span data-ttu-id="4a94c-240">workProfilePasswordBlockFingerprintUnlock</span><span class="sxs-lookup"><span data-stu-id="4a94c-240">workProfilePasswordBlockFingerprintUnlock</span></span>|<span data-ttu-id="4a94c-241">Boolean</span><span class="sxs-lookup"><span data-stu-id="4a94c-241">Boolean</span></span>|<span data-ttu-id="4a94c-242">指示是否阻止工作配置文件的指纹解锁。</span><span class="sxs-lookup"><span data-stu-id="4a94c-242">Indicates whether or not to block fingerprint unlock for work profile.</span></span>|
|<span data-ttu-id="4a94c-243">workProfilePasswordBlockTrustAgents</span><span class="sxs-lookup"><span data-stu-id="4a94c-243">workProfilePasswordBlockTrustAgents</span></span>|<span data-ttu-id="4a94c-244">Boolean</span><span class="sxs-lookup"><span data-stu-id="4a94c-244">Boolean</span></span>|<span data-ttu-id="4a94c-245">指示是否阻止智能锁定和其他信任代理用于工作配置文件。</span><span class="sxs-lookup"><span data-stu-id="4a94c-245">Indicates whether or not to block Smart Lock and other trust agents for work profile.</span></span>|
|<span data-ttu-id="4a94c-246">workProfilePasswordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="4a94c-246">workProfilePasswordExpirationDays</span></span>|<span data-ttu-id="4a94c-247">Int32</span><span class="sxs-lookup"><span data-stu-id="4a94c-247">Int32</span></span>|<span data-ttu-id="4a94c-248">工作配置文件密码到期前的天数。</span><span class="sxs-lookup"><span data-stu-id="4a94c-248">Number of days before the work profile password expires.</span></span> <span data-ttu-id="4a94c-249">有效值为 1 至 365。</span><span class="sxs-lookup"><span data-stu-id="4a94c-249">Valid values 1 to 365</span></span>|
|<span data-ttu-id="4a94c-250">workProfilePasswordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="4a94c-250">workProfilePasswordMinimumLength</span></span>|<span data-ttu-id="4a94c-251">Int32</span><span class="sxs-lookup"><span data-stu-id="4a94c-251">Int32</span></span>|<span data-ttu-id="4a94c-252">工作配置文件密码的最小长度。</span><span class="sxs-lookup"><span data-stu-id="4a94c-252">Minimum length of work profile password.</span></span> <span data-ttu-id="4a94c-253">有效值为 4 至 16</span><span class="sxs-lookup"><span data-stu-id="4a94c-253">Valid values 4 to 16</span></span>|
|<span data-ttu-id="4a94c-254">workProfilePasswordMinNumericCharacters</span><span class="sxs-lookup"><span data-stu-id="4a94c-254">workProfilePasswordMinNumericCharacters</span></span>|<span data-ttu-id="4a94c-255">Int32</span><span class="sxs-lookup"><span data-stu-id="4a94c-255">Int32</span></span>|<span data-ttu-id="4a94c-256">工作配置文件密码中所需的最小数字字符数。</span><span class="sxs-lookup"><span data-stu-id="4a94c-256">Minimum # of numeric characters required in work profile password.</span></span> <span data-ttu-id="4a94c-257">有效值为1至10</span><span class="sxs-lookup"><span data-stu-id="4a94c-257">Valid values 1 to 10</span></span>|
|<span data-ttu-id="4a94c-258">workProfilePasswordMinNonLetterCharacters</span><span class="sxs-lookup"><span data-stu-id="4a94c-258">workProfilePasswordMinNonLetterCharacters</span></span>|<span data-ttu-id="4a94c-259">Int32</span><span class="sxs-lookup"><span data-stu-id="4a94c-259">Int32</span></span>|<span data-ttu-id="4a94c-260">工作配置文件密码中所需的最小非字母字符数。</span><span class="sxs-lookup"><span data-stu-id="4a94c-260">Minimum # of non-letter characters required in work profile password.</span></span> <span data-ttu-id="4a94c-261">有效值为1至10</span><span class="sxs-lookup"><span data-stu-id="4a94c-261">Valid values 1 to 10</span></span>|
|<span data-ttu-id="4a94c-262">workProfilePasswordMinLetterCharacters</span><span class="sxs-lookup"><span data-stu-id="4a94c-262">workProfilePasswordMinLetterCharacters</span></span>|<span data-ttu-id="4a94c-263">Int32</span><span class="sxs-lookup"><span data-stu-id="4a94c-263">Int32</span></span>|<span data-ttu-id="4a94c-264">工作配置文件密码中所需的字母字符的最小数目。</span><span class="sxs-lookup"><span data-stu-id="4a94c-264">Minimum # of letter characters required in work profile password.</span></span> <span data-ttu-id="4a94c-265">有效值为1至10</span><span class="sxs-lookup"><span data-stu-id="4a94c-265">Valid values 1 to 10</span></span>|
|<span data-ttu-id="4a94c-266">workProfilePasswordMinLowerCaseCharacters</span><span class="sxs-lookup"><span data-stu-id="4a94c-266">workProfilePasswordMinLowerCaseCharacters</span></span>|<span data-ttu-id="4a94c-267">Int32</span><span class="sxs-lookup"><span data-stu-id="4a94c-267">Int32</span></span>|<span data-ttu-id="4a94c-268">工作配置文件密码中所需的小写字符的最小数量。</span><span class="sxs-lookup"><span data-stu-id="4a94c-268">Minimum # of lower-case characters required in work profile password.</span></span> <span data-ttu-id="4a94c-269">有效值为1至10</span><span class="sxs-lookup"><span data-stu-id="4a94c-269">Valid values 1 to 10</span></span>|
|<span data-ttu-id="4a94c-270">workProfilePasswordMinUpperCaseCharacters</span><span class="sxs-lookup"><span data-stu-id="4a94c-270">workProfilePasswordMinUpperCaseCharacters</span></span>|<span data-ttu-id="4a94c-271">Int32</span><span class="sxs-lookup"><span data-stu-id="4a94c-271">Int32</span></span>|<span data-ttu-id="4a94c-272">工作配置文件密码中要求的大写字符的最小数量。</span><span class="sxs-lookup"><span data-stu-id="4a94c-272">Minimum # of upper-case characters required in work profile password.</span></span> <span data-ttu-id="4a94c-273">有效值为1至10</span><span class="sxs-lookup"><span data-stu-id="4a94c-273">Valid values 1 to 10</span></span>|
|<span data-ttu-id="4a94c-274">workProfilePasswordMinSymbolCharacters</span><span class="sxs-lookup"><span data-stu-id="4a94c-274">workProfilePasswordMinSymbolCharacters</span></span>|<span data-ttu-id="4a94c-275">Int32</span><span class="sxs-lookup"><span data-stu-id="4a94c-275">Int32</span></span>|<span data-ttu-id="4a94c-276">工作配置文件密码中所需的最小符号数。</span><span class="sxs-lookup"><span data-stu-id="4a94c-276">Minimum # of symbols required in work profile password.</span></span> <span data-ttu-id="4a94c-277">有效值为1至10</span><span class="sxs-lookup"><span data-stu-id="4a94c-277">Valid values 1 to 10</span></span>|
|<span data-ttu-id="4a94c-278">workProfilePasswordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="4a94c-278">workProfilePasswordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="4a94c-279">Int32</span><span class="sxs-lookup"><span data-stu-id="4a94c-279">Int32</span></span>|<span data-ttu-id="4a94c-280">屏幕超时之前的不活动分钟数。</span><span class="sxs-lookup"><span data-stu-id="4a94c-280">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="4a94c-281">workProfilePasswordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="4a94c-281">workProfilePasswordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="4a94c-282">Int32</span><span class="sxs-lookup"><span data-stu-id="4a94c-282">Int32</span></span>|<span data-ttu-id="4a94c-283">要阻止的以前的工作配置文件密码的数量。</span><span class="sxs-lookup"><span data-stu-id="4a94c-283">Number of previous work profile passwords to block.</span></span> <span data-ttu-id="4a94c-284">有效值为 0 至 24</span><span class="sxs-lookup"><span data-stu-id="4a94c-284">Valid values 0 to 24</span></span>|
|<span data-ttu-id="4a94c-285">workProfilePasswordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="4a94c-285">workProfilePasswordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="4a94c-286">Int32</span><span class="sxs-lookup"><span data-stu-id="4a94c-286">Int32</span></span>|<span data-ttu-id="4a94c-287">在删除工作配置文件和删除所有公司数据之前允许的登录失败次数。</span><span class="sxs-lookup"><span data-stu-id="4a94c-287">Number of sign in failures allowed before work profile is removed and all corporate data deleted.</span></span> <span data-ttu-id="4a94c-288">有效值为1至16</span><span class="sxs-lookup"><span data-stu-id="4a94c-288">Valid values 1 to 16</span></span>|
|<span data-ttu-id="4a94c-289">workProfilePasswordRequiredType</span><span class="sxs-lookup"><span data-stu-id="4a94c-289">workProfilePasswordRequiredType</span></span>|[<span data-ttu-id="4a94c-290">androidWorkProfileRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="4a94c-290">androidWorkProfileRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androidworkprofilerequiredpasswordtype.md)|<span data-ttu-id="4a94c-291">所需的工作配置文件密码类型。</span><span class="sxs-lookup"><span data-stu-id="4a94c-291">Type of work profile password that is required.</span></span> <span data-ttu-id="4a94c-292">可取值为：`deviceDefault`、`lowSecurityBiometric`、`required`、`atLeastNumeric`、`numericComplex`、`atLeastAlphabetic`、`atLeastAlphanumeric`、`alphanumericWithSymbols`。</span><span class="sxs-lookup"><span data-stu-id="4a94c-292">Possible values are: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric`, `alphanumericWithSymbols`.</span></span>|
|<span data-ttu-id="4a94c-293">workProfileRequirePassword</span><span class="sxs-lookup"><span data-stu-id="4a94c-293">workProfileRequirePassword</span></span>|<span data-ttu-id="4a94c-294">Boolean</span><span class="sxs-lookup"><span data-stu-id="4a94c-294">Boolean</span></span>|<span data-ttu-id="4a94c-295">对于工作配置文件, 密码是必需的</span><span class="sxs-lookup"><span data-stu-id="4a94c-295">Password is required or not for work profile</span></span>|
|<span data-ttu-id="4a94c-296">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="4a94c-296">securityRequireVerifyApps</span></span>|<span data-ttu-id="4a94c-297">Boolean</span><span class="sxs-lookup"><span data-stu-id="4a94c-297">Boolean</span></span>|<span data-ttu-id="4a94c-298">要求启用 Android 验证应用功能。</span><span class="sxs-lookup"><span data-stu-id="4a94c-298">Require the Android Verify apps feature is turned on.</span></span>|
|<span data-ttu-id="4a94c-299">vpnAlwaysOnPackageIdentifier</span><span class="sxs-lookup"><span data-stu-id="4a94c-299">vpnAlwaysOnPackageIdentifier</span></span>|<span data-ttu-id="4a94c-300">String</span><span class="sxs-lookup"><span data-stu-id="4a94c-300">String</span></span>|<span data-ttu-id="4a94c-301">为 always on VPN 启用锁定模式。</span><span class="sxs-lookup"><span data-stu-id="4a94c-301">Enable lockdown mode for always-on VPN.</span></span>|
|<span data-ttu-id="4a94c-302">vpnEnableAlwaysOnLockdownMode</span><span class="sxs-lookup"><span data-stu-id="4a94c-302">vpnEnableAlwaysOnLockdownMode</span></span>|<span data-ttu-id="4a94c-303">Boolean</span><span class="sxs-lookup"><span data-stu-id="4a94c-303">Boolean</span></span>|<span data-ttu-id="4a94c-304">为 always on VPN 启用锁定模式。</span><span class="sxs-lookup"><span data-stu-id="4a94c-304">Enable lockdown mode for always-on VPN.</span></span>|



## <a name="response"></a><span data-ttu-id="4a94c-305">响应</span><span class="sxs-lookup"><span data-stu-id="4a94c-305">Response</span></span>
<span data-ttu-id="4a94c-306">如果成功, 此方法在响应`201 Created`正文中返回响应代码和[androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="4a94c-306">If successful, this method returns a `201 Created` response code and a [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4a94c-307">示例</span><span class="sxs-lookup"><span data-stu-id="4a94c-307">Example</span></span>

### <a name="request"></a><span data-ttu-id="4a94c-308">请求</span><span class="sxs-lookup"><span data-stu-id="4a94c-308">Request</span></span>
<span data-ttu-id="4a94c-309">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="4a94c-309">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 2815

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
  "vpnEnableAlwaysOnLockdownMode": true
}
```

### <a name="response"></a><span data-ttu-id="4a94c-310">响应</span><span class="sxs-lookup"><span data-stu-id="4a94c-310">Response</span></span>
<span data-ttu-id="4a94c-p131">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="4a94c-p131">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 2987

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
  "vpnEnableAlwaysOnLockdownMode": true
}
```





