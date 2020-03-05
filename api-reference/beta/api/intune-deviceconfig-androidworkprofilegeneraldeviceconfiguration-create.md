---
title: 创建 androidWorkProfileGeneralDeviceConfiguration
description: 创建新的 androidWorkProfileGeneralDeviceConfiguration 对象。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: df3eddba7c3f7729fbd326a2ac5af21a9f884f13
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42443501"
---
# <a name="create-androidworkprofilegeneraldeviceconfiguration"></a><span data-ttu-id="adeae-103">创建 androidWorkProfileGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="adeae-103">Create androidWorkProfileGeneralDeviceConfiguration</span></span>

<span data-ttu-id="adeae-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="adeae-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="adeae-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="adeae-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="adeae-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="adeae-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="adeae-107">创建新的[androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="adeae-107">Create a new [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="adeae-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="adeae-108">Prerequisites</span></span>
<span data-ttu-id="adeae-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="adeae-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="adeae-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="adeae-111">Permission type</span></span>|<span data-ttu-id="adeae-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="adeae-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="adeae-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="adeae-113">Delegated (work or school account)</span></span>|<span data-ttu-id="adeae-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="adeae-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="adeae-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="adeae-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="adeae-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="adeae-116">Not supported.</span></span>|
|<span data-ttu-id="adeae-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="adeae-117">Application</span></span>|<span data-ttu-id="adeae-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="adeae-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="adeae-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="adeae-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="adeae-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="adeae-120">Request headers</span></span>
|<span data-ttu-id="adeae-121">标头</span><span class="sxs-lookup"><span data-stu-id="adeae-121">Header</span></span>|<span data-ttu-id="adeae-122">值</span><span class="sxs-lookup"><span data-stu-id="adeae-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="adeae-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="adeae-123">Authorization</span></span>|<span data-ttu-id="adeae-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="adeae-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="adeae-125">接受</span><span class="sxs-lookup"><span data-stu-id="adeae-125">Accept</span></span>|<span data-ttu-id="adeae-126">application/json</span><span class="sxs-lookup"><span data-stu-id="adeae-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="adeae-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="adeae-127">Request body</span></span>
<span data-ttu-id="adeae-128">在请求正文中，提供 androidWorkProfileGeneralDeviceConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="adeae-128">In the request body, supply a JSON representation for the androidWorkProfileGeneralDeviceConfiguration object.</span></span>

<span data-ttu-id="adeae-129">下表显示创建 androidWorkProfileGeneralDeviceConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="adeae-129">The following table shows the properties that are required when you create the androidWorkProfileGeneralDeviceConfiguration.</span></span>

|<span data-ttu-id="adeae-130">属性</span><span class="sxs-lookup"><span data-stu-id="adeae-130">Property</span></span>|<span data-ttu-id="adeae-131">类型</span><span class="sxs-lookup"><span data-stu-id="adeae-131">Type</span></span>|<span data-ttu-id="adeae-132">说明</span><span class="sxs-lookup"><span data-stu-id="adeae-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="adeae-133">id</span><span class="sxs-lookup"><span data-stu-id="adeae-133">id</span></span>|<span data-ttu-id="adeae-134">字符串</span><span class="sxs-lookup"><span data-stu-id="adeae-134">String</span></span>|<span data-ttu-id="adeae-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="adeae-135">Key of the entity.</span></span> <span data-ttu-id="adeae-136">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="adeae-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="adeae-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="adeae-137">lastModifiedDateTime</span></span>|<span data-ttu-id="adeae-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="adeae-138">DateTimeOffset</span></span>|<span data-ttu-id="adeae-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="adeae-139">DateTime the object was last modified.</span></span> <span data-ttu-id="adeae-140">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="adeae-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="adeae-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="adeae-141">roleScopeTagIds</span></span>|<span data-ttu-id="adeae-142">String 集合</span><span class="sxs-lookup"><span data-stu-id="adeae-142">String collection</span></span>|<span data-ttu-id="adeae-143">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="adeae-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="adeae-144">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="adeae-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="adeae-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="adeae-145">supportsScopeTags</span></span>|<span data-ttu-id="adeae-146">布尔</span><span class="sxs-lookup"><span data-stu-id="adeae-146">Boolean</span></span>|<span data-ttu-id="adeae-147">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="adeae-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="adeae-148">如果此值为 false，则不允许分配给 ScopeTags 属性，并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="adeae-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="adeae-149">这适用于在 Silverlight 中创建的旧版策略，可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="adeae-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="adeae-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="adeae-150">This property is read-only.</span></span> <span data-ttu-id="adeae-151">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="adeae-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="adeae-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="adeae-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="adeae-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="adeae-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="adeae-154">适用于此策略的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="adeae-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="adeae-155">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="adeae-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="adeae-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="adeae-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="adeae-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="adeae-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="adeae-158">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="adeae-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="adeae-159">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="adeae-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="adeae-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="adeae-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="adeae-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="adeae-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="adeae-162">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="adeae-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="adeae-163">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="adeae-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="adeae-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="adeae-164">createdDateTime</span></span>|<span data-ttu-id="adeae-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="adeae-165">DateTimeOffset</span></span>|<span data-ttu-id="adeae-166">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="adeae-166">DateTime the object was created.</span></span> <span data-ttu-id="adeae-167">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="adeae-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="adeae-168">说明</span><span class="sxs-lookup"><span data-stu-id="adeae-168">description</span></span>|<span data-ttu-id="adeae-169">String</span><span class="sxs-lookup"><span data-stu-id="adeae-169">String</span></span>|<span data-ttu-id="adeae-170">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="adeae-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="adeae-171">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="adeae-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="adeae-172">displayName</span><span class="sxs-lookup"><span data-stu-id="adeae-172">displayName</span></span>|<span data-ttu-id="adeae-173">String</span><span class="sxs-lookup"><span data-stu-id="adeae-173">String</span></span>|<span data-ttu-id="adeae-174">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="adeae-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="adeae-175">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="adeae-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="adeae-176">version</span><span class="sxs-lookup"><span data-stu-id="adeae-176">version</span></span>|<span data-ttu-id="adeae-177">Int32</span><span class="sxs-lookup"><span data-stu-id="adeae-177">Int32</span></span>|<span data-ttu-id="adeae-178">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="adeae-178">Version of the device configuration.</span></span> <span data-ttu-id="adeae-179">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="adeae-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="adeae-180">passwordBlockFingerprintUnlock</span><span class="sxs-lookup"><span data-stu-id="adeae-180">passwordBlockFingerprintUnlock</span></span>|<span data-ttu-id="adeae-181">布尔</span><span class="sxs-lookup"><span data-stu-id="adeae-181">Boolean</span></span>|<span data-ttu-id="adeae-182">指示是否阻止指纹解锁。</span><span class="sxs-lookup"><span data-stu-id="adeae-182">Indicates whether or not to block fingerprint unlock.</span></span>|
|<span data-ttu-id="adeae-183">passwordBlockTrustAgents</span><span class="sxs-lookup"><span data-stu-id="adeae-183">passwordBlockTrustAgents</span></span>|<span data-ttu-id="adeae-184">Boolean</span><span class="sxs-lookup"><span data-stu-id="adeae-184">Boolean</span></span>|<span data-ttu-id="adeae-185">指示是否阻止 Smart Lock 和其他信任代理。</span><span class="sxs-lookup"><span data-stu-id="adeae-185">Indicates whether or not to block Smart Lock and other trust agents.</span></span>|
|<span data-ttu-id="adeae-186">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="adeae-186">passwordExpirationDays</span></span>|<span data-ttu-id="adeae-187">Int32</span><span class="sxs-lookup"><span data-stu-id="adeae-187">Int32</span></span>|<span data-ttu-id="adeae-188">密码过期前的天数。</span><span class="sxs-lookup"><span data-stu-id="adeae-188">Number of days before the password expires.</span></span> <span data-ttu-id="adeae-189">有效值为 1 至 365。</span><span class="sxs-lookup"><span data-stu-id="adeae-189">Valid values 1 to 365</span></span>|
|<span data-ttu-id="adeae-190">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="adeae-190">passwordMinimumLength</span></span>|<span data-ttu-id="adeae-191">Int32</span><span class="sxs-lookup"><span data-stu-id="adeae-191">Int32</span></span>|<span data-ttu-id="adeae-192">密码的最小长度。</span><span class="sxs-lookup"><span data-stu-id="adeae-192">Minimum length of passwords.</span></span> <span data-ttu-id="adeae-193">有效值为 4 至 16</span><span class="sxs-lookup"><span data-stu-id="adeae-193">Valid values 4 to 16</span></span>|
|<span data-ttu-id="adeae-194">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="adeae-194">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="adeae-195">Int32</span><span class="sxs-lookup"><span data-stu-id="adeae-195">Int32</span></span>|<span data-ttu-id="adeae-196">屏幕超时之前的不活动分钟数。</span><span class="sxs-lookup"><span data-stu-id="adeae-196">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="adeae-197">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="adeae-197">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="adeae-198">Int32</span><span class="sxs-lookup"><span data-stu-id="adeae-198">Int32</span></span>|<span data-ttu-id="adeae-199">要阻止的以前密码的数量。</span><span class="sxs-lookup"><span data-stu-id="adeae-199">Number of previous passwords to block.</span></span> <span data-ttu-id="adeae-200">有效值为 0 至 24</span><span class="sxs-lookup"><span data-stu-id="adeae-200">Valid values 0 to 24</span></span>|
|<span data-ttu-id="adeae-201">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="adeae-201">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="adeae-202">Int32</span><span class="sxs-lookup"><span data-stu-id="adeae-202">Int32</span></span>|<span data-ttu-id="adeae-203">恢复出厂设置之前允许登录失败的次数。</span><span class="sxs-lookup"><span data-stu-id="adeae-203">Number of sign in failures allowed before factory reset.</span></span> <span data-ttu-id="adeae-204">有效值为1至16</span><span class="sxs-lookup"><span data-stu-id="adeae-204">Valid values 1 to 16</span></span>|
|<span data-ttu-id="adeae-205">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="adeae-205">passwordRequiredType</span></span>|[<span data-ttu-id="adeae-206">androidWorkProfileRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="adeae-206">androidWorkProfileRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androidworkprofilerequiredpasswordtype.md)|<span data-ttu-id="adeae-207">必需的密码类型。</span><span class="sxs-lookup"><span data-stu-id="adeae-207">Type of password that is required.</span></span> <span data-ttu-id="adeae-208">可取值为：`deviceDefault`、`lowSecurityBiometric`、`required`、`atLeastNumeric`、`numericComplex`、`atLeastAlphabetic`、`atLeastAlphanumeric`、`alphanumericWithSymbols`。</span><span class="sxs-lookup"><span data-stu-id="adeae-208">Possible values are: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric`, `alphanumericWithSymbols`.</span></span>|
|<span data-ttu-id="adeae-209">workProfileDataSharingType</span><span class="sxs-lookup"><span data-stu-id="adeae-209">workProfileDataSharingType</span></span>|[<span data-ttu-id="adeae-210">androidWorkProfileCrossProfileDataSharingType</span><span class="sxs-lookup"><span data-stu-id="adeae-210">androidWorkProfileCrossProfileDataSharingType</span></span>](../resources/intune-deviceconfig-androidworkprofilecrossprofiledatasharingtype.md)|<span data-ttu-id="adeae-211">允许的数据共享类型。</span><span class="sxs-lookup"><span data-stu-id="adeae-211">Type of data sharing that is allowed.</span></span> <span data-ttu-id="adeae-212">可取值为：`deviceDefault`、`preventAny`、`allowPersonalToWork`、`noRestrictions`。</span><span class="sxs-lookup"><span data-stu-id="adeae-212">Possible values are: `deviceDefault`, `preventAny`, `allowPersonalToWork`, `noRestrictions`.</span></span>|
|<span data-ttu-id="adeae-213">workProfileBlockNotificationsWhileDeviceLocked</span><span class="sxs-lookup"><span data-stu-id="adeae-213">workProfileBlockNotificationsWhileDeviceLocked</span></span>|<span data-ttu-id="adeae-214">布尔</span><span class="sxs-lookup"><span data-stu-id="adeae-214">Boolean</span></span>|<span data-ttu-id="adeae-215">指示在设备锁定时是否阻止通知。</span><span class="sxs-lookup"><span data-stu-id="adeae-215">Indicates whether or not to block notifications while device locked.</span></span>|
|<span data-ttu-id="adeae-216">workProfileBlockAddingAccounts</span><span class="sxs-lookup"><span data-stu-id="adeae-216">workProfileBlockAddingAccounts</span></span>|<span data-ttu-id="adeae-217">布尔</span><span class="sxs-lookup"><span data-stu-id="adeae-217">Boolean</span></span>|<span data-ttu-id="adeae-218">阻止用户在工作配置文件中添加/删除帐户。</span><span class="sxs-lookup"><span data-stu-id="adeae-218">Block users from adding/removing accounts in work profile.</span></span>|
|<span data-ttu-id="adeae-219">workProfileBluetoothEnableContactSharing</span><span class="sxs-lookup"><span data-stu-id="adeae-219">workProfileBluetoothEnableContactSharing</span></span>|<span data-ttu-id="adeae-220">布尔</span><span class="sxs-lookup"><span data-stu-id="adeae-220">Boolean</span></span>|<span data-ttu-id="adeae-221">允许蓝牙设备访问企业联系人。</span><span class="sxs-lookup"><span data-stu-id="adeae-221">Allow bluetooth devices to access enterprise contacts.</span></span>|
|<span data-ttu-id="adeae-222">workProfileBlockScreenCapture</span><span class="sxs-lookup"><span data-stu-id="adeae-222">workProfileBlockScreenCapture</span></span>|<span data-ttu-id="adeae-223">布尔</span><span class="sxs-lookup"><span data-stu-id="adeae-223">Boolean</span></span>|<span data-ttu-id="adeae-224">在工作配置文件中阻止屏幕捕获。</span><span class="sxs-lookup"><span data-stu-id="adeae-224">Block screen capture in work profile.</span></span>|
|<span data-ttu-id="adeae-225">workProfileBlockCrossProfileCallerId</span><span class="sxs-lookup"><span data-stu-id="adeae-225">workProfileBlockCrossProfileCallerId</span></span>|<span data-ttu-id="adeae-226">布尔</span><span class="sxs-lookup"><span data-stu-id="adeae-226">Boolean</span></span>|<span data-ttu-id="adeae-227">阻止显示个人配置文件中的工作配置文件呼叫者 ID。</span><span class="sxs-lookup"><span data-stu-id="adeae-227">Block display work profile caller ID in personal profile.</span></span>|
|<span data-ttu-id="adeae-228">workProfileBlockCamera</span><span class="sxs-lookup"><span data-stu-id="adeae-228">workProfileBlockCamera</span></span>|<span data-ttu-id="adeae-229">布尔</span><span class="sxs-lookup"><span data-stu-id="adeae-229">Boolean</span></span>|<span data-ttu-id="adeae-230">阻止工作配置文件相机。</span><span class="sxs-lookup"><span data-stu-id="adeae-230">Block work profile camera.</span></span>|
|<span data-ttu-id="adeae-231">workProfileBlockCrossProfileContactsSearch</span><span class="sxs-lookup"><span data-stu-id="adeae-231">workProfileBlockCrossProfileContactsSearch</span></span>|<span data-ttu-id="adeae-232">布尔</span><span class="sxs-lookup"><span data-stu-id="adeae-232">Boolean</span></span>|<span data-ttu-id="adeae-233">阻止个人配置文件中的工作配置文件联系人可用性。</span><span class="sxs-lookup"><span data-stu-id="adeae-233">Block work profile contacts availability in personal profile.</span></span>|
|<span data-ttu-id="adeae-234">workProfileBlockCrossProfileCopyPaste</span><span class="sxs-lookup"><span data-stu-id="adeae-234">workProfileBlockCrossProfileCopyPaste</span></span>|<span data-ttu-id="adeae-235">布尔</span><span class="sxs-lookup"><span data-stu-id="adeae-235">Boolean</span></span>|<span data-ttu-id="adeae-236">指示是否启用 "禁用跨配置文件复制/粘贴" 设置的 Boolean。</span><span class="sxs-lookup"><span data-stu-id="adeae-236">Boolean that indicates if the setting disallow cross profile copy/paste is enabled.</span></span>|
|<span data-ttu-id="adeae-237">workProfileDefaultAppPermissionPolicy</span><span class="sxs-lookup"><span data-stu-id="adeae-237">workProfileDefaultAppPermissionPolicy</span></span>|[<span data-ttu-id="adeae-238">androidWorkProfileDefaultAppPermissionPolicyType</span><span class="sxs-lookup"><span data-stu-id="adeae-238">androidWorkProfileDefaultAppPermissionPolicyType</span></span>](../resources/intune-deviceconfig-androidworkprofiledefaultapppermissionpolicytype.md)|<span data-ttu-id="adeae-239">必需的密码类型。</span><span class="sxs-lookup"><span data-stu-id="adeae-239">Type of password that is required.</span></span> <span data-ttu-id="adeae-240">可取值为：`deviceDefault`、`prompt`、`autoGrant`、`autoDeny`。</span><span class="sxs-lookup"><span data-stu-id="adeae-240">Possible values are: `deviceDefault`, `prompt`, `autoGrant`, `autoDeny`.</span></span>|
|<span data-ttu-id="adeae-241">workProfilePasswordBlockFingerprintUnlock</span><span class="sxs-lookup"><span data-stu-id="adeae-241">workProfilePasswordBlockFingerprintUnlock</span></span>|<span data-ttu-id="adeae-242">布尔</span><span class="sxs-lookup"><span data-stu-id="adeae-242">Boolean</span></span>|<span data-ttu-id="adeae-243">指示是否阻止工作配置文件的指纹解锁。</span><span class="sxs-lookup"><span data-stu-id="adeae-243">Indicates whether or not to block fingerprint unlock for work profile.</span></span>|
|<span data-ttu-id="adeae-244">workProfilePasswordBlockTrustAgents</span><span class="sxs-lookup"><span data-stu-id="adeae-244">workProfilePasswordBlockTrustAgents</span></span>|<span data-ttu-id="adeae-245">布尔</span><span class="sxs-lookup"><span data-stu-id="adeae-245">Boolean</span></span>|<span data-ttu-id="adeae-246">指示是否阻止智能锁定和其他信任代理用于工作配置文件。</span><span class="sxs-lookup"><span data-stu-id="adeae-246">Indicates whether or not to block Smart Lock and other trust agents for work profile.</span></span>|
|<span data-ttu-id="adeae-247">workProfilePasswordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="adeae-247">workProfilePasswordExpirationDays</span></span>|<span data-ttu-id="adeae-248">Int32</span><span class="sxs-lookup"><span data-stu-id="adeae-248">Int32</span></span>|<span data-ttu-id="adeae-249">工作配置文件密码到期前的天数。</span><span class="sxs-lookup"><span data-stu-id="adeae-249">Number of days before the work profile password expires.</span></span> <span data-ttu-id="adeae-250">有效值为 1 至 365。</span><span class="sxs-lookup"><span data-stu-id="adeae-250">Valid values 1 to 365</span></span>|
|<span data-ttu-id="adeae-251">workProfilePasswordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="adeae-251">workProfilePasswordMinimumLength</span></span>|<span data-ttu-id="adeae-252">Int32</span><span class="sxs-lookup"><span data-stu-id="adeae-252">Int32</span></span>|<span data-ttu-id="adeae-253">工作配置文件密码的最小长度。</span><span class="sxs-lookup"><span data-stu-id="adeae-253">Minimum length of work profile password.</span></span> <span data-ttu-id="adeae-254">有效值为 4 至 16</span><span class="sxs-lookup"><span data-stu-id="adeae-254">Valid values 4 to 16</span></span>|
|<span data-ttu-id="adeae-255">workProfilePasswordMinNumericCharacters</span><span class="sxs-lookup"><span data-stu-id="adeae-255">workProfilePasswordMinNumericCharacters</span></span>|<span data-ttu-id="adeae-256">Int32</span><span class="sxs-lookup"><span data-stu-id="adeae-256">Int32</span></span>|<span data-ttu-id="adeae-257">工作配置文件密码中所需的最小数字字符数。</span><span class="sxs-lookup"><span data-stu-id="adeae-257">Minimum # of numeric characters required in work profile password.</span></span> <span data-ttu-id="adeae-258">有效值为1至10</span><span class="sxs-lookup"><span data-stu-id="adeae-258">Valid values 1 to 10</span></span>|
|<span data-ttu-id="adeae-259">workProfilePasswordMinNonLetterCharacters</span><span class="sxs-lookup"><span data-stu-id="adeae-259">workProfilePasswordMinNonLetterCharacters</span></span>|<span data-ttu-id="adeae-260">Int32</span><span class="sxs-lookup"><span data-stu-id="adeae-260">Int32</span></span>|<span data-ttu-id="adeae-261">工作配置文件密码中所需的最小非字母字符数。</span><span class="sxs-lookup"><span data-stu-id="adeae-261">Minimum # of non-letter characters required in work profile password.</span></span> <span data-ttu-id="adeae-262">有效值为1至10</span><span class="sxs-lookup"><span data-stu-id="adeae-262">Valid values 1 to 10</span></span>|
|<span data-ttu-id="adeae-263">workProfilePasswordMinLetterCharacters</span><span class="sxs-lookup"><span data-stu-id="adeae-263">workProfilePasswordMinLetterCharacters</span></span>|<span data-ttu-id="adeae-264">Int32</span><span class="sxs-lookup"><span data-stu-id="adeae-264">Int32</span></span>|<span data-ttu-id="adeae-265">工作配置文件密码中所需的字母字符的最小数目。</span><span class="sxs-lookup"><span data-stu-id="adeae-265">Minimum # of letter characters required in work profile password.</span></span> <span data-ttu-id="adeae-266">有效值为1至10</span><span class="sxs-lookup"><span data-stu-id="adeae-266">Valid values 1 to 10</span></span>|
|<span data-ttu-id="adeae-267">workProfilePasswordMinLowerCaseCharacters</span><span class="sxs-lookup"><span data-stu-id="adeae-267">workProfilePasswordMinLowerCaseCharacters</span></span>|<span data-ttu-id="adeae-268">Int32</span><span class="sxs-lookup"><span data-stu-id="adeae-268">Int32</span></span>|<span data-ttu-id="adeae-269">工作配置文件密码中所需的小写字符的最小数量。</span><span class="sxs-lookup"><span data-stu-id="adeae-269">Minimum # of lower-case characters required in work profile password.</span></span> <span data-ttu-id="adeae-270">有效值为1至10</span><span class="sxs-lookup"><span data-stu-id="adeae-270">Valid values 1 to 10</span></span>|
|<span data-ttu-id="adeae-271">workProfilePasswordMinUpperCaseCharacters</span><span class="sxs-lookup"><span data-stu-id="adeae-271">workProfilePasswordMinUpperCaseCharacters</span></span>|<span data-ttu-id="adeae-272">Int32</span><span class="sxs-lookup"><span data-stu-id="adeae-272">Int32</span></span>|<span data-ttu-id="adeae-273">工作配置文件密码中要求的大写字符的最小数量。</span><span class="sxs-lookup"><span data-stu-id="adeae-273">Minimum # of upper-case characters required in work profile password.</span></span> <span data-ttu-id="adeae-274">有效值为1至10</span><span class="sxs-lookup"><span data-stu-id="adeae-274">Valid values 1 to 10</span></span>|
|<span data-ttu-id="adeae-275">workProfilePasswordMinSymbolCharacters</span><span class="sxs-lookup"><span data-stu-id="adeae-275">workProfilePasswordMinSymbolCharacters</span></span>|<span data-ttu-id="adeae-276">Int32</span><span class="sxs-lookup"><span data-stu-id="adeae-276">Int32</span></span>|<span data-ttu-id="adeae-277">工作配置文件密码中所需的最小符号数。</span><span class="sxs-lookup"><span data-stu-id="adeae-277">Minimum # of symbols required in work profile password.</span></span> <span data-ttu-id="adeae-278">有效值为1至10</span><span class="sxs-lookup"><span data-stu-id="adeae-278">Valid values 1 to 10</span></span>|
|<span data-ttu-id="adeae-279">workProfilePasswordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="adeae-279">workProfilePasswordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="adeae-280">Int32</span><span class="sxs-lookup"><span data-stu-id="adeae-280">Int32</span></span>|<span data-ttu-id="adeae-281">屏幕超时之前的不活动分钟数。</span><span class="sxs-lookup"><span data-stu-id="adeae-281">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="adeae-282">workProfilePasswordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="adeae-282">workProfilePasswordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="adeae-283">Int32</span><span class="sxs-lookup"><span data-stu-id="adeae-283">Int32</span></span>|<span data-ttu-id="adeae-284">要阻止的以前的工作配置文件密码的数量。</span><span class="sxs-lookup"><span data-stu-id="adeae-284">Number of previous work profile passwords to block.</span></span> <span data-ttu-id="adeae-285">有效值为 0 至 24</span><span class="sxs-lookup"><span data-stu-id="adeae-285">Valid values 0 to 24</span></span>|
|<span data-ttu-id="adeae-286">workProfilePasswordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="adeae-286">workProfilePasswordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="adeae-287">Int32</span><span class="sxs-lookup"><span data-stu-id="adeae-287">Int32</span></span>|<span data-ttu-id="adeae-288">在删除工作配置文件和删除所有公司数据之前允许的登录失败次数。</span><span class="sxs-lookup"><span data-stu-id="adeae-288">Number of sign in failures allowed before work profile is removed and all corporate data deleted.</span></span> <span data-ttu-id="adeae-289">有效值为1至16</span><span class="sxs-lookup"><span data-stu-id="adeae-289">Valid values 1 to 16</span></span>|
|<span data-ttu-id="adeae-290">workProfilePasswordRequiredType</span><span class="sxs-lookup"><span data-stu-id="adeae-290">workProfilePasswordRequiredType</span></span>|[<span data-ttu-id="adeae-291">androidWorkProfileRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="adeae-291">androidWorkProfileRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androidworkprofilerequiredpasswordtype.md)|<span data-ttu-id="adeae-292">所需的工作配置文件密码类型。</span><span class="sxs-lookup"><span data-stu-id="adeae-292">Type of work profile password that is required.</span></span> <span data-ttu-id="adeae-293">可取值为：`deviceDefault`、`lowSecurityBiometric`、`required`、`atLeastNumeric`、`numericComplex`、`atLeastAlphabetic`、`atLeastAlphanumeric`、`alphanumericWithSymbols`。</span><span class="sxs-lookup"><span data-stu-id="adeae-293">Possible values are: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric`, `alphanumericWithSymbols`.</span></span>|
|<span data-ttu-id="adeae-294">workProfileRequirePassword</span><span class="sxs-lookup"><span data-stu-id="adeae-294">workProfileRequirePassword</span></span>|<span data-ttu-id="adeae-295">布尔</span><span class="sxs-lookup"><span data-stu-id="adeae-295">Boolean</span></span>|<span data-ttu-id="adeae-296">对于工作配置文件，密码是必需的</span><span class="sxs-lookup"><span data-stu-id="adeae-296">Password is required or not for work profile</span></span>|
|<span data-ttu-id="adeae-297">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="adeae-297">securityRequireVerifyApps</span></span>|<span data-ttu-id="adeae-298">Boolean</span><span class="sxs-lookup"><span data-stu-id="adeae-298">Boolean</span></span>|<span data-ttu-id="adeae-299">要求启用 Android 验证应用功能。</span><span class="sxs-lookup"><span data-stu-id="adeae-299">Require the Android Verify apps feature is turned on.</span></span>|
|<span data-ttu-id="adeae-300">vpnAlwaysOnPackageIdentifier</span><span class="sxs-lookup"><span data-stu-id="adeae-300">vpnAlwaysOnPackageIdentifier</span></span>|<span data-ttu-id="adeae-301">String</span><span class="sxs-lookup"><span data-stu-id="adeae-301">String</span></span>|<span data-ttu-id="adeae-302">为 always on VPN 启用锁定模式。</span><span class="sxs-lookup"><span data-stu-id="adeae-302">Enable lockdown mode for always-on VPN.</span></span>|
|<span data-ttu-id="adeae-303">vpnEnableAlwaysOnLockdownMode</span><span class="sxs-lookup"><span data-stu-id="adeae-303">vpnEnableAlwaysOnLockdownMode</span></span>|<span data-ttu-id="adeae-304">布尔</span><span class="sxs-lookup"><span data-stu-id="adeae-304">Boolean</span></span>|<span data-ttu-id="adeae-305">为 always on VPN 启用锁定模式。</span><span class="sxs-lookup"><span data-stu-id="adeae-305">Enable lockdown mode for always-on VPN.</span></span>|
|<span data-ttu-id="adeae-306">workProfileAllowWidgets</span><span class="sxs-lookup"><span data-stu-id="adeae-306">workProfileAllowWidgets</span></span>|<span data-ttu-id="adeae-307">布尔</span><span class="sxs-lookup"><span data-stu-id="adeae-307">Boolean</span></span>|<span data-ttu-id="adeae-308">允许来自工作配置文件应用程序的小部件。</span><span class="sxs-lookup"><span data-stu-id="adeae-308">Allow widgets from work profile apps.</span></span>|
|<span data-ttu-id="adeae-309">workProfileBlockPersonalAppInstallsFromUnknownSources</span><span class="sxs-lookup"><span data-stu-id="adeae-309">workProfileBlockPersonalAppInstallsFromUnknownSources</span></span>|<span data-ttu-id="adeae-310">布尔</span><span class="sxs-lookup"><span data-stu-id="adeae-310">Boolean</span></span>|<span data-ttu-id="adeae-311">阻止从个人配置文件中的未知源进行应用程序安装。</span><span class="sxs-lookup"><span data-stu-id="adeae-311">Prevent app installations from unknown sources in the personal profile.</span></span>|



## <a name="response"></a><span data-ttu-id="adeae-312">响应</span><span class="sxs-lookup"><span data-stu-id="adeae-312">Response</span></span>
<span data-ttu-id="adeae-313">如果成功，此方法在响应`201 Created`正文中返回响应代码和[androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="adeae-313">If successful, this method returns a `201 Created` response code and a [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="adeae-314">示例</span><span class="sxs-lookup"><span data-stu-id="adeae-314">Example</span></span>

### <a name="request"></a><span data-ttu-id="adeae-315">请求</span><span class="sxs-lookup"><span data-stu-id="adeae-315">Request</span></span>
<span data-ttu-id="adeae-316">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="adeae-316">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 2917

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
  "vpnEnableAlwaysOnLockdownMode": true,
  "workProfileAllowWidgets": true,
  "workProfileBlockPersonalAppInstallsFromUnknownSources": true
}
```

### <a name="response"></a><span data-ttu-id="adeae-317">响应</span><span class="sxs-lookup"><span data-stu-id="adeae-317">Response</span></span>
<span data-ttu-id="adeae-p131">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="adeae-p131">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 3089

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
  "vpnEnableAlwaysOnLockdownMode": true,
  "workProfileAllowWidgets": true,
  "workProfileBlockPersonalAppInstallsFromUnknownSources": true
}
```





