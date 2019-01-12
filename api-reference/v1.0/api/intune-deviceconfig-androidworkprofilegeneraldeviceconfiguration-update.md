---
title: 更新 androidWorkProfileGeneralDeviceConfiguration
description: 更新 androidWorkProfileGeneralDeviceConfiguration 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 9c9e150fc722842c3d904f2cb06a4127e96fc61c
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27943954"
---
# <a name="update-androidworkprofilegeneraldeviceconfiguration"></a><span data-ttu-id="df237-103">更新 androidWorkProfileGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="df237-103">Update androidWorkProfileGeneralDeviceConfiguration</span></span>

> <span data-ttu-id="df237-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="df237-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="df237-105">更新[androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="df237-105">Update the properties of a [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="df237-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="df237-106">Prerequisites</span></span>
<span data-ttu-id="df237-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="df237-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="df237-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="df237-109">Permission type</span></span>|<span data-ttu-id="df237-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="df237-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="df237-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="df237-111">Delegated (work or school account)</span></span>|<span data-ttu-id="df237-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="df237-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="df237-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="df237-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="df237-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="df237-114">Not supported.</span></span>|
|<span data-ttu-id="df237-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="df237-115">Application</span></span>|<span data-ttu-id="df237-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="df237-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="df237-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="df237-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="df237-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="df237-118">Request headers</span></span>
|<span data-ttu-id="df237-119">标头</span><span class="sxs-lookup"><span data-stu-id="df237-119">Header</span></span>|<span data-ttu-id="df237-120">值</span><span class="sxs-lookup"><span data-stu-id="df237-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="df237-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="df237-121">Authorization</span></span>|<span data-ttu-id="df237-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="df237-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="df237-123">Accept</span><span class="sxs-lookup"><span data-stu-id="df237-123">Accept</span></span>|<span data-ttu-id="df237-124">application/json</span><span class="sxs-lookup"><span data-stu-id="df237-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="df237-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="df237-125">Request body</span></span>
<span data-ttu-id="df237-126">在请求正文中，提供[androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="df237-126">In the request body, supply a JSON representation for the [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) object.</span></span>

<span data-ttu-id="df237-127">下表显示时创建[androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md)所需的属性。</span><span class="sxs-lookup"><span data-stu-id="df237-127">The following table shows the properties that are required when you create the [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md).</span></span>

|<span data-ttu-id="df237-128">属性</span><span class="sxs-lookup"><span data-stu-id="df237-128">Property</span></span>|<span data-ttu-id="df237-129">类型</span><span class="sxs-lookup"><span data-stu-id="df237-129">Type</span></span>|<span data-ttu-id="df237-130">说明</span><span class="sxs-lookup"><span data-stu-id="df237-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="df237-131">id</span><span class="sxs-lookup"><span data-stu-id="df237-131">id</span></span>|<span data-ttu-id="df237-132">String</span><span class="sxs-lookup"><span data-stu-id="df237-132">String</span></span>|<span data-ttu-id="df237-133">实体的键。</span><span class="sxs-lookup"><span data-stu-id="df237-133">Key of the entity.</span></span> <span data-ttu-id="df237-134">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="df237-134">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="df237-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="df237-135">lastModifiedDateTime</span></span>|<span data-ttu-id="df237-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="df237-136">DateTimeOffset</span></span>|<span data-ttu-id="df237-137">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="df237-137">DateTime the object was last modified.</span></span> <span data-ttu-id="df237-138">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="df237-138">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="df237-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="df237-139">createdDateTime</span></span>|<span data-ttu-id="df237-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="df237-140">DateTimeOffset</span></span>|<span data-ttu-id="df237-141">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="df237-141">DateTime the object was created.</span></span> <span data-ttu-id="df237-142">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="df237-142">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="df237-143">description</span><span class="sxs-lookup"><span data-stu-id="df237-143">description</span></span>|<span data-ttu-id="df237-144">String</span><span class="sxs-lookup"><span data-stu-id="df237-144">String</span></span>|<span data-ttu-id="df237-145">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="df237-145">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="df237-146">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="df237-146">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="df237-147">displayName</span><span class="sxs-lookup"><span data-stu-id="df237-147">displayName</span></span>|<span data-ttu-id="df237-148">String</span><span class="sxs-lookup"><span data-stu-id="df237-148">String</span></span>|<span data-ttu-id="df237-149">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="df237-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="df237-150">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="df237-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="df237-151">version</span><span class="sxs-lookup"><span data-stu-id="df237-151">version</span></span>|<span data-ttu-id="df237-152">Int32</span><span class="sxs-lookup"><span data-stu-id="df237-152">Int32</span></span>|<span data-ttu-id="df237-153">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="df237-153">Version of the device configuration.</span></span> <span data-ttu-id="df237-154">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="df237-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="df237-155">passwordBlockFingerprintUnlock</span><span class="sxs-lookup"><span data-stu-id="df237-155">passwordBlockFingerprintUnlock</span></span>|<span data-ttu-id="df237-156">Boolean</span><span class="sxs-lookup"><span data-stu-id="df237-156">Boolean</span></span>|<span data-ttu-id="df237-157">指示是否阻止指纹解锁。</span><span class="sxs-lookup"><span data-stu-id="df237-157">Indicates whether or not to block fingerprint unlock.</span></span>|
|<span data-ttu-id="df237-158">passwordBlockTrustAgents</span><span class="sxs-lookup"><span data-stu-id="df237-158">passwordBlockTrustAgents</span></span>|<span data-ttu-id="df237-159">Boolean</span><span class="sxs-lookup"><span data-stu-id="df237-159">Boolean</span></span>|<span data-ttu-id="df237-160">指示是否阻止 Smart Lock 和其他信任代理。</span><span class="sxs-lookup"><span data-stu-id="df237-160">Indicates whether or not to block Smart Lock and other trust agents.</span></span>|
|<span data-ttu-id="df237-161">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="df237-161">passwordExpirationDays</span></span>|<span data-ttu-id="df237-162">Int32</span><span class="sxs-lookup"><span data-stu-id="df237-162">Int32</span></span>|<span data-ttu-id="df237-163">密码过期前的天数。</span><span class="sxs-lookup"><span data-stu-id="df237-163">Number of days before the password expires.</span></span> <span data-ttu-id="df237-164">有效值为 1 至 365。</span><span class="sxs-lookup"><span data-stu-id="df237-164">Valid values 1 to 365</span></span>|
|<span data-ttu-id="df237-165">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="df237-165">passwordMinimumLength</span></span>|<span data-ttu-id="df237-166">Int32</span><span class="sxs-lookup"><span data-stu-id="df237-166">Int32</span></span>|<span data-ttu-id="df237-167">密码的最小长度。</span><span class="sxs-lookup"><span data-stu-id="df237-167">Minimum length of passwords.</span></span> <span data-ttu-id="df237-168">有效值为 4 至 16</span><span class="sxs-lookup"><span data-stu-id="df237-168">Valid values 4 to 16</span></span>|
|<span data-ttu-id="df237-169">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="df237-169">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="df237-170">Int32</span><span class="sxs-lookup"><span data-stu-id="df237-170">Int32</span></span>|<span data-ttu-id="df237-171">屏幕超时之前的不活动分钟数。</span><span class="sxs-lookup"><span data-stu-id="df237-171">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="df237-172">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="df237-172">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="df237-173">Int32</span><span class="sxs-lookup"><span data-stu-id="df237-173">Int32</span></span>|<span data-ttu-id="df237-174">要阻止的以前密码的数量。</span><span class="sxs-lookup"><span data-stu-id="df237-174">Number of previous passwords to block.</span></span> <span data-ttu-id="df237-175">有效值为 0 至 24</span><span class="sxs-lookup"><span data-stu-id="df237-175">Valid values 0 to 24</span></span>|
|<span data-ttu-id="df237-176">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="df237-176">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="df237-177">Int32</span><span class="sxs-lookup"><span data-stu-id="df237-177">Int32</span></span>|<span data-ttu-id="df237-178">恢复出厂设置之前允许登录失败的次数。</span><span class="sxs-lookup"><span data-stu-id="df237-178">Number of sign in failures allowed before factory reset.</span></span> <span data-ttu-id="df237-179">有效值为 4 至 11</span><span class="sxs-lookup"><span data-stu-id="df237-179">Valid values 4 to 11</span></span>|
|<span data-ttu-id="df237-180">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="df237-180">passwordRequiredType</span></span>|[<span data-ttu-id="df237-181">androidWorkProfileRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="df237-181">androidWorkProfileRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androidworkprofilerequiredpasswordtype.md)|<span data-ttu-id="df237-182">必需的密码类型。</span><span class="sxs-lookup"><span data-stu-id="df237-182">Type of password that is required.</span></span> <span data-ttu-id="df237-183">可取值为：`deviceDefault`、`lowSecurityBiometric`、`required`、`atLeastNumeric`、`numericComplex`、`atLeastAlphabetic`、`atLeastAlphanumeric`、`alphanumericWithSymbols`。</span><span class="sxs-lookup"><span data-stu-id="df237-183">Possible values are: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric`, `alphanumericWithSymbols`.</span></span>|
|<span data-ttu-id="df237-184">workProfileDataSharingType</span><span class="sxs-lookup"><span data-stu-id="df237-184">workProfileDataSharingType</span></span>|[<span data-ttu-id="df237-185">androidWorkProfileCrossProfileDataSharingType</span><span class="sxs-lookup"><span data-stu-id="df237-185">androidWorkProfileCrossProfileDataSharingType</span></span>](../resources/intune-deviceconfig-androidworkprofilecrossprofiledatasharingtype.md)|<span data-ttu-id="df237-186">允许共享的数据的类型。</span><span class="sxs-lookup"><span data-stu-id="df237-186">Type of data sharing that is allowed.</span></span> <span data-ttu-id="df237-187">可取值为：`deviceDefault`、`preventAny`、`allowPersonalToWork`、`noRestrictions`。</span><span class="sxs-lookup"><span data-stu-id="df237-187">Possible values are: `deviceDefault`, `preventAny`, `allowPersonalToWork`, `noRestrictions`.</span></span>|
|<span data-ttu-id="df237-188">workProfileBlockNotificationsWhileDeviceLocked</span><span class="sxs-lookup"><span data-stu-id="df237-188">workProfileBlockNotificationsWhileDeviceLocked</span></span>|<span data-ttu-id="df237-189">布尔</span><span class="sxs-lookup"><span data-stu-id="df237-189">Boolean</span></span>|<span data-ttu-id="df237-190">指示阻止通知时设备锁定。</span><span class="sxs-lookup"><span data-stu-id="df237-190">Indicates whether or not to block notifications while device locked.</span></span>|
|<span data-ttu-id="df237-191">workProfileBlockAddingAccounts</span><span class="sxs-lookup"><span data-stu-id="df237-191">workProfileBlockAddingAccounts</span></span>|<span data-ttu-id="df237-192">布尔</span><span class="sxs-lookup"><span data-stu-id="df237-192">Boolean</span></span>|<span data-ttu-id="df237-193">阻止用户添加/移除工作配置文件中的帐户。</span><span class="sxs-lookup"><span data-stu-id="df237-193">Block users from adding/removing accounts in work profile.</span></span>|
|<span data-ttu-id="df237-194">workProfileBluetoothEnableContactSharing</span><span class="sxs-lookup"><span data-stu-id="df237-194">workProfileBluetoothEnableContactSharing</span></span>|<span data-ttu-id="df237-195">布尔</span><span class="sxs-lookup"><span data-stu-id="df237-195">Boolean</span></span>|<span data-ttu-id="df237-196">允许蓝牙设备访问企业联系人。</span><span class="sxs-lookup"><span data-stu-id="df237-196">Allow bluetooth devices to access enterprise contacts.</span></span>|
|<span data-ttu-id="df237-197">workProfileBlockScreenCapture</span><span class="sxs-lookup"><span data-stu-id="df237-197">workProfileBlockScreenCapture</span></span>|<span data-ttu-id="df237-198">布尔</span><span class="sxs-lookup"><span data-stu-id="df237-198">Boolean</span></span>|<span data-ttu-id="df237-199">阻止工作配置文件中的屏幕截图。</span><span class="sxs-lookup"><span data-stu-id="df237-199">Block screen capture in work profile.</span></span>|
|<span data-ttu-id="df237-200">workProfileBlockCrossProfileCallerId</span><span class="sxs-lookup"><span data-stu-id="df237-200">workProfileBlockCrossProfileCallerId</span></span>|<span data-ttu-id="df237-201">布尔</span><span class="sxs-lookup"><span data-stu-id="df237-201">Boolean</span></span>|<span data-ttu-id="df237-202">阻止显示工作 profile 呼叫者 ID 个人配置文件中。</span><span class="sxs-lookup"><span data-stu-id="df237-202">Block display work profile caller ID in personal profile.</span></span>|
|<span data-ttu-id="df237-203">workProfileBlockCamera</span><span class="sxs-lookup"><span data-stu-id="df237-203">workProfileBlockCamera</span></span>|<span data-ttu-id="df237-204">布尔</span><span class="sxs-lookup"><span data-stu-id="df237-204">Boolean</span></span>|<span data-ttu-id="df237-205">阻止工作 profile 摄像头。</span><span class="sxs-lookup"><span data-stu-id="df237-205">Block work profile camera.</span></span>|
|<span data-ttu-id="df237-206">workProfileBlockCrossProfileContactsSearch</span><span class="sxs-lookup"><span data-stu-id="df237-206">workProfileBlockCrossProfileContactsSearch</span></span>|<span data-ttu-id="df237-207">布尔</span><span class="sxs-lookup"><span data-stu-id="df237-207">Boolean</span></span>|<span data-ttu-id="df237-208">个人配置文件中，阻止工作 profile 联系人可用性。</span><span class="sxs-lookup"><span data-stu-id="df237-208">Block work profile contacts availability in personal profile.</span></span>|
|<span data-ttu-id="df237-209">workProfileBlockCrossProfileCopyPaste</span><span class="sxs-lookup"><span data-stu-id="df237-209">workProfileBlockCrossProfileCopyPaste</span></span>|<span data-ttu-id="df237-210">布尔</span><span class="sxs-lookup"><span data-stu-id="df237-210">Boolean</span></span>|<span data-ttu-id="df237-211">布尔值，指示设置不允许跨是否启用配置文件复制/粘贴。</span><span class="sxs-lookup"><span data-stu-id="df237-211">Boolean that indicates if the setting disallow cross profile copy/paste is enabled.</span></span>|
|<span data-ttu-id="df237-212">workProfileDefaultAppPermissionPolicy</span><span class="sxs-lookup"><span data-stu-id="df237-212">workProfileDefaultAppPermissionPolicy</span></span>|[<span data-ttu-id="df237-213">androidWorkProfileDefaultAppPermissionPolicyType</span><span class="sxs-lookup"><span data-stu-id="df237-213">androidWorkProfileDefaultAppPermissionPolicyType</span></span>](../resources/intune-deviceconfig-androidworkprofiledefaultapppermissionpolicytype.md)|<span data-ttu-id="df237-214">必需的密码类型。</span><span class="sxs-lookup"><span data-stu-id="df237-214">Type of password that is required.</span></span> <span data-ttu-id="df237-215">可取值为：`deviceDefault`、`prompt`、`autoGrant`、`autoDeny`。</span><span class="sxs-lookup"><span data-stu-id="df237-215">Possible values are: `deviceDefault`, `prompt`, `autoGrant`, `autoDeny`.</span></span>|
|<span data-ttu-id="df237-216">workProfilePasswordBlockFingerprintUnlock</span><span class="sxs-lookup"><span data-stu-id="df237-216">workProfilePasswordBlockFingerprintUnlock</span></span>|<span data-ttu-id="df237-217">布尔</span><span class="sxs-lookup"><span data-stu-id="df237-217">Boolean</span></span>|<span data-ttu-id="df237-218">指示是否阻止指纹解锁工作配置文件。</span><span class="sxs-lookup"><span data-stu-id="df237-218">Indicates whether or not to block fingerprint unlock for work profile.</span></span>|
|<span data-ttu-id="df237-219">workProfilePasswordBlockTrustAgents</span><span class="sxs-lookup"><span data-stu-id="df237-219">workProfilePasswordBlockTrustAgents</span></span>|<span data-ttu-id="df237-220">布尔</span><span class="sxs-lookup"><span data-stu-id="df237-220">Boolean</span></span>|<span data-ttu-id="df237-221">指示阻止智能锁定和其他信任代理工作配置文件。</span><span class="sxs-lookup"><span data-stu-id="df237-221">Indicates whether or not to block Smart Lock and other trust agents for work profile.</span></span>|
|<span data-ttu-id="df237-222">workProfilePasswordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="df237-222">workProfilePasswordExpirationDays</span></span>|<span data-ttu-id="df237-223">Int32</span><span class="sxs-lookup"><span data-stu-id="df237-223">Int32</span></span>|<span data-ttu-id="df237-224">过期工作配置文件密码之前的天数。</span><span class="sxs-lookup"><span data-stu-id="df237-224">Number of days before the work profile password expires.</span></span> <span data-ttu-id="df237-225">有效值为 1 至 365。</span><span class="sxs-lookup"><span data-stu-id="df237-225">Valid values 1 to 365</span></span>|
|<span data-ttu-id="df237-226">workProfilePasswordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="df237-226">workProfilePasswordMinimumLength</span></span>|<span data-ttu-id="df237-227">Int32</span><span class="sxs-lookup"><span data-stu-id="df237-227">Int32</span></span>|<span data-ttu-id="df237-228">工作配置文件密码最小长度。</span><span class="sxs-lookup"><span data-stu-id="df237-228">Minimum length of work profile password.</span></span> <span data-ttu-id="df237-229">有效值为 4 至 16</span><span class="sxs-lookup"><span data-stu-id="df237-229">Valid values 4 to 16</span></span>|
|<span data-ttu-id="df237-230">workProfilePasswordMinNumericCharacters</span><span class="sxs-lookup"><span data-stu-id="df237-230">workProfilePasswordMinNumericCharacters</span></span>|<span data-ttu-id="df237-231">Int32</span><span class="sxs-lookup"><span data-stu-id="df237-231">Int32</span></span>|<span data-ttu-id="df237-232">最小 ハ  工作配置文件密码中所需的数字字符。</span><span class="sxs-lookup"><span data-stu-id="df237-232">Minimum # of numeric characters required in work profile password.</span></span> <span data-ttu-id="df237-233">有效的值 1 到 10</span><span class="sxs-lookup"><span data-stu-id="df237-233">Valid values 1 to 10</span></span>|
|<span data-ttu-id="df237-234">workProfilePasswordMinNonLetterCharacters</span><span class="sxs-lookup"><span data-stu-id="df237-234">workProfilePasswordMinNonLetterCharacters</span></span>|<span data-ttu-id="df237-235">Int32</span><span class="sxs-lookup"><span data-stu-id="df237-235">Int32</span></span>|<span data-ttu-id="df237-236">最小 ハ  中工作配置文件密码必须包含非字母字符。</span><span class="sxs-lookup"><span data-stu-id="df237-236">Minimum # of non-letter characters required in work profile password.</span></span> <span data-ttu-id="df237-237">有效的值 1 到 10</span><span class="sxs-lookup"><span data-stu-id="df237-237">Valid values 1 to 10</span></span>|
|<span data-ttu-id="df237-238">workProfilePasswordMinLetterCharacters</span><span class="sxs-lookup"><span data-stu-id="df237-238">workProfilePasswordMinLetterCharacters</span></span>|<span data-ttu-id="df237-239">Int32</span><span class="sxs-lookup"><span data-stu-id="df237-239">Int32</span></span>|<span data-ttu-id="df237-240">最小 ハ  中工作配置文件密码必须包含字母字符。</span><span class="sxs-lookup"><span data-stu-id="df237-240">Minimum # of letter characters required in work profile password.</span></span> <span data-ttu-id="df237-241">有效的值 1 到 10</span><span class="sxs-lookup"><span data-stu-id="df237-241">Valid values 1 to 10</span></span>|
|<span data-ttu-id="df237-242">workProfilePasswordMinLowerCaseCharacters</span><span class="sxs-lookup"><span data-stu-id="df237-242">workProfilePasswordMinLowerCaseCharacters</span></span>|<span data-ttu-id="df237-243">Int32</span><span class="sxs-lookup"><span data-stu-id="df237-243">Int32</span></span>|<span data-ttu-id="df237-244">最小 ハ  工作配置文件密码中需要的小写字符。</span><span class="sxs-lookup"><span data-stu-id="df237-244">Minimum # of lower-case characters required in work profile password.</span></span> <span data-ttu-id="df237-245">有效的值 1 到 10</span><span class="sxs-lookup"><span data-stu-id="df237-245">Valid values 1 to 10</span></span>|
|<span data-ttu-id="df237-246">workProfilePasswordMinUpperCaseCharacters</span><span class="sxs-lookup"><span data-stu-id="df237-246">workProfilePasswordMinUpperCaseCharacters</span></span>|<span data-ttu-id="df237-247">Int32</span><span class="sxs-lookup"><span data-stu-id="df237-247">Int32</span></span>|<span data-ttu-id="df237-248">最小 ハ  中工作配置文件密码必须大写字符。</span><span class="sxs-lookup"><span data-stu-id="df237-248">Minimum # of upper-case characters required in work profile password.</span></span> <span data-ttu-id="df237-249">有效的值 1 到 10</span><span class="sxs-lookup"><span data-stu-id="df237-249">Valid values 1 to 10</span></span>|
|<span data-ttu-id="df237-250">workProfilePasswordMinSymbolCharacters</span><span class="sxs-lookup"><span data-stu-id="df237-250">workProfilePasswordMinSymbolCharacters</span></span>|<span data-ttu-id="df237-251">Int32</span><span class="sxs-lookup"><span data-stu-id="df237-251">Int32</span></span>|<span data-ttu-id="df237-252">最小 ハ  工作配置文件密码中需要的符号。</span><span class="sxs-lookup"><span data-stu-id="df237-252">Minimum # of symbols required in work profile password.</span></span> <span data-ttu-id="df237-253">有效的值 1 到 10</span><span class="sxs-lookup"><span data-stu-id="df237-253">Valid values 1 to 10</span></span>|
|<span data-ttu-id="df237-254">workProfilePasswordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="df237-254">workProfilePasswordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="df237-255">Int32</span><span class="sxs-lookup"><span data-stu-id="df237-255">Int32</span></span>|<span data-ttu-id="df237-256">屏幕超时之前的不活动分钟数。</span><span class="sxs-lookup"><span data-stu-id="df237-256">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="df237-257">workProfilePasswordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="df237-257">workProfilePasswordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="df237-258">Int32</span><span class="sxs-lookup"><span data-stu-id="df237-258">Int32</span></span>|<span data-ttu-id="df237-259">以前的工作配置文件密码，以阻止数。</span><span class="sxs-lookup"><span data-stu-id="df237-259">Number of previous work profile passwords to block.</span></span> <span data-ttu-id="df237-260">有效值为 0 至 24</span><span class="sxs-lookup"><span data-stu-id="df237-260">Valid values 0 to 24</span></span>|
|<span data-ttu-id="df237-261">workProfilePasswordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="df237-261">workProfilePasswordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="df237-262">Int32</span><span class="sxs-lookup"><span data-stu-id="df237-262">Int32</span></span>|<span data-ttu-id="df237-263">登录失败之前删除工作配置文件允许和已删除的所有企业数据的数量。</span><span class="sxs-lookup"><span data-stu-id="df237-263">Number of sign in failures allowed before work profile is removed and all corporate data deleted.</span></span> <span data-ttu-id="df237-264">有效值为 4 至 11</span><span class="sxs-lookup"><span data-stu-id="df237-264">Valid values 4 to 11</span></span>|
|<span data-ttu-id="df237-265">workProfilePasswordRequiredType</span><span class="sxs-lookup"><span data-stu-id="df237-265">workProfilePasswordRequiredType</span></span>|[<span data-ttu-id="df237-266">androidWorkProfileRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="df237-266">androidWorkProfileRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androidworkprofilerequiredpasswordtype.md)|<span data-ttu-id="df237-267">工作所需的配置文件密码的类型。</span><span class="sxs-lookup"><span data-stu-id="df237-267">Type of work profile password that is required.</span></span> <span data-ttu-id="df237-268">可取值为：`deviceDefault`、`lowSecurityBiometric`、`required`、`atLeastNumeric`、`numericComplex`、`atLeastAlphabetic`、`atLeastAlphanumeric`、`alphanumericWithSymbols`。</span><span class="sxs-lookup"><span data-stu-id="df237-268">Possible values are: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric`, `alphanumericWithSymbols`.</span></span>|
|<span data-ttu-id="df237-269">workProfileRequirePassword</span><span class="sxs-lookup"><span data-stu-id="df237-269">workProfileRequirePassword</span></span>|<span data-ttu-id="df237-270">布尔</span><span class="sxs-lookup"><span data-stu-id="df237-270">Boolean</span></span>|<span data-ttu-id="df237-271">密码，则需要或不工作配置文件</span><span class="sxs-lookup"><span data-stu-id="df237-271">Password is required or not for work profile</span></span>|
|<span data-ttu-id="df237-272">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="df237-272">securityRequireVerifyApps</span></span>|<span data-ttu-id="df237-273">Boolean</span><span class="sxs-lookup"><span data-stu-id="df237-273">Boolean</span></span>|<span data-ttu-id="df237-274">要求启用 Android 验证应用功能。</span><span class="sxs-lookup"><span data-stu-id="df237-274">Require the Android Verify apps feature is turned on.</span></span>|



## <a name="response"></a><span data-ttu-id="df237-275">响应</span><span class="sxs-lookup"><span data-stu-id="df237-275">Response</span></span>
<span data-ttu-id="df237-276">如果成功，此方法返回`200 OK`响应代码和响应正文中的更新的[androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="df237-276">If successful, this method returns a `200 OK` response code and an updated [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="df237-277">示例</span><span class="sxs-lookup"><span data-stu-id="df237-277">Example</span></span>
### <a name="request"></a><span data-ttu-id="df237-278">请求</span><span class="sxs-lookup"><span data-stu-id="df237-278">Request</span></span>
<span data-ttu-id="df237-279">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="df237-279">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1831

{
  "@odata.type": "#microsoft.graph.androidWorkProfileGeneralDeviceConfiguration",
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
  "securityRequireVerifyApps": true
}
```

### <a name="response"></a><span data-ttu-id="df237-280">响应</span><span class="sxs-lookup"><span data-stu-id="df237-280">Response</span></span>
<span data-ttu-id="df237-p126">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="df237-p126">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2003

{
  "@odata.type": "#microsoft.graph.androidWorkProfileGeneralDeviceConfiguration",
  "id": "6decda7e-da7e-6dec-7eda-ec6d7edaec6d",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
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
  "securityRequireVerifyApps": true
}
```



