---
title: 更新 androidWorkProfileGeneralDeviceConfiguration
description: 更新 androidWorkProfileGeneralDeviceConfiguration 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: f9e7a9e4c36823ae1b66eedaf342f6fa6574fab8
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52756692"
---
# <a name="update-androidworkprofilegeneraldeviceconfiguration"></a><span data-ttu-id="dddaa-103">更新 androidWorkProfileGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="dddaa-103">Update androidWorkProfileGeneralDeviceConfiguration</span></span>

<span data-ttu-id="dddaa-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dddaa-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="dddaa-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="dddaa-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dddaa-106">更新 [androidWorkProfileGeneralDeviceConfiguration 对象](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="dddaa-106">Update the properties of a [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="dddaa-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="dddaa-107">Prerequisites</span></span>
<span data-ttu-id="dddaa-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="dddaa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dddaa-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="dddaa-110">Permission type</span></span>|<span data-ttu-id="dddaa-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="dddaa-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="dddaa-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="dddaa-112">Delegated (work or school account)</span></span>|<span data-ttu-id="dddaa-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dddaa-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="dddaa-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="dddaa-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="dddaa-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="dddaa-115">Not supported.</span></span>|
|<span data-ttu-id="dddaa-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="dddaa-116">Application</span></span>|<span data-ttu-id="dddaa-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dddaa-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="dddaa-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="dddaa-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="dddaa-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="dddaa-119">Request headers</span></span>
|<span data-ttu-id="dddaa-120">标头</span><span class="sxs-lookup"><span data-stu-id="dddaa-120">Header</span></span>|<span data-ttu-id="dddaa-121">值</span><span class="sxs-lookup"><span data-stu-id="dddaa-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="dddaa-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="dddaa-122">Authorization</span></span>|<span data-ttu-id="dddaa-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="dddaa-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="dddaa-124">接受</span><span class="sxs-lookup"><span data-stu-id="dddaa-124">Accept</span></span>|<span data-ttu-id="dddaa-125">application/json</span><span class="sxs-lookup"><span data-stu-id="dddaa-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="dddaa-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="dddaa-126">Request body</span></span>
<span data-ttu-id="dddaa-127">在请求正文中，提供 [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="dddaa-127">In the request body, supply a JSON representation for the [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) object.</span></span>

<span data-ttu-id="dddaa-128">下表显示创建 [androidWorkProfileGeneralDeviceConfiguration 时所需的属性](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md)。</span><span class="sxs-lookup"><span data-stu-id="dddaa-128">The following table shows the properties that are required when you create the [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md).</span></span>

|<span data-ttu-id="dddaa-129">属性</span><span class="sxs-lookup"><span data-stu-id="dddaa-129">Property</span></span>|<span data-ttu-id="dddaa-130">类型</span><span class="sxs-lookup"><span data-stu-id="dddaa-130">Type</span></span>|<span data-ttu-id="dddaa-131">说明</span><span class="sxs-lookup"><span data-stu-id="dddaa-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dddaa-132">id</span><span class="sxs-lookup"><span data-stu-id="dddaa-132">id</span></span>|<span data-ttu-id="dddaa-133">String</span><span class="sxs-lookup"><span data-stu-id="dddaa-133">String</span></span>|<span data-ttu-id="dddaa-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="dddaa-134">Key of the entity.</span></span> <span data-ttu-id="dddaa-135">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="dddaa-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="dddaa-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="dddaa-136">lastModifiedDateTime</span></span>|<span data-ttu-id="dddaa-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dddaa-137">DateTimeOffset</span></span>|<span data-ttu-id="dddaa-138">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="dddaa-138">DateTime the object was last modified.</span></span> <span data-ttu-id="dddaa-139">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="dddaa-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="dddaa-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="dddaa-140">createdDateTime</span></span>|<span data-ttu-id="dddaa-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dddaa-141">DateTimeOffset</span></span>|<span data-ttu-id="dddaa-142">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="dddaa-142">DateTime the object was created.</span></span> <span data-ttu-id="dddaa-143">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="dddaa-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="dddaa-144">说明</span><span class="sxs-lookup"><span data-stu-id="dddaa-144">description</span></span>|<span data-ttu-id="dddaa-145">String</span><span class="sxs-lookup"><span data-stu-id="dddaa-145">String</span></span>|<span data-ttu-id="dddaa-146">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="dddaa-146">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="dddaa-147">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="dddaa-147">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="dddaa-148">displayName</span><span class="sxs-lookup"><span data-stu-id="dddaa-148">displayName</span></span>|<span data-ttu-id="dddaa-149">String</span><span class="sxs-lookup"><span data-stu-id="dddaa-149">String</span></span>|<span data-ttu-id="dddaa-150">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="dddaa-150">Admin provided name of the device configuration.</span></span> <span data-ttu-id="dddaa-151">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="dddaa-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="dddaa-152">version</span><span class="sxs-lookup"><span data-stu-id="dddaa-152">version</span></span>|<span data-ttu-id="dddaa-153">Int32</span><span class="sxs-lookup"><span data-stu-id="dddaa-153">Int32</span></span>|<span data-ttu-id="dddaa-154">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="dddaa-154">Version of the device configuration.</span></span> <span data-ttu-id="dddaa-155">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="dddaa-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="dddaa-156">passwordBlockFingerprintUnlock</span><span class="sxs-lookup"><span data-stu-id="dddaa-156">passwordBlockFingerprintUnlock</span></span>|<span data-ttu-id="dddaa-157">Boolean</span><span class="sxs-lookup"><span data-stu-id="dddaa-157">Boolean</span></span>|<span data-ttu-id="dddaa-158">指示是否阻止指纹解锁。</span><span class="sxs-lookup"><span data-stu-id="dddaa-158">Indicates whether or not to block fingerprint unlock.</span></span>|
|<span data-ttu-id="dddaa-159">passwordBlockTrustAgents</span><span class="sxs-lookup"><span data-stu-id="dddaa-159">passwordBlockTrustAgents</span></span>|<span data-ttu-id="dddaa-160">Boolean</span><span class="sxs-lookup"><span data-stu-id="dddaa-160">Boolean</span></span>|<span data-ttu-id="dddaa-161">指示是否阻止 Smart Lock 和其他信任代理。</span><span class="sxs-lookup"><span data-stu-id="dddaa-161">Indicates whether or not to block Smart Lock and other trust agents.</span></span>|
|<span data-ttu-id="dddaa-162">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="dddaa-162">passwordExpirationDays</span></span>|<span data-ttu-id="dddaa-163">Int32</span><span class="sxs-lookup"><span data-stu-id="dddaa-163">Int32</span></span>|<span data-ttu-id="dddaa-164">密码过期前的天数。</span><span class="sxs-lookup"><span data-stu-id="dddaa-164">Number of days before the password expires.</span></span> <span data-ttu-id="dddaa-165">有效值为 1 至 365。</span><span class="sxs-lookup"><span data-stu-id="dddaa-165">Valid values 1 to 365</span></span>|
|<span data-ttu-id="dddaa-166">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="dddaa-166">passwordMinimumLength</span></span>|<span data-ttu-id="dddaa-167">Int32</span><span class="sxs-lookup"><span data-stu-id="dddaa-167">Int32</span></span>|<span data-ttu-id="dddaa-168">密码的最小长度。</span><span class="sxs-lookup"><span data-stu-id="dddaa-168">Minimum length of passwords.</span></span> <span data-ttu-id="dddaa-169">有效值为 4 至 16</span><span class="sxs-lookup"><span data-stu-id="dddaa-169">Valid values 4 to 16</span></span>|
|<span data-ttu-id="dddaa-170">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="dddaa-170">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="dddaa-171">Int32</span><span class="sxs-lookup"><span data-stu-id="dddaa-171">Int32</span></span>|<span data-ttu-id="dddaa-172">屏幕超时之前的不活动分钟数。</span><span class="sxs-lookup"><span data-stu-id="dddaa-172">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="dddaa-173">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="dddaa-173">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="dddaa-174">Int32</span><span class="sxs-lookup"><span data-stu-id="dddaa-174">Int32</span></span>|<span data-ttu-id="dddaa-175">要阻止的以前密码的数量。</span><span class="sxs-lookup"><span data-stu-id="dddaa-175">Number of previous passwords to block.</span></span> <span data-ttu-id="dddaa-176">有效值为 0 至 24</span><span class="sxs-lookup"><span data-stu-id="dddaa-176">Valid values 0 to 24</span></span>|
|<span data-ttu-id="dddaa-177">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="dddaa-177">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="dddaa-178">Int32</span><span class="sxs-lookup"><span data-stu-id="dddaa-178">Int32</span></span>|<span data-ttu-id="dddaa-179">恢复出厂设置之前允许登录失败的次数。</span><span class="sxs-lookup"><span data-stu-id="dddaa-179">Number of sign in failures allowed before factory reset.</span></span> <span data-ttu-id="dddaa-180">有效值为 1 到 16</span><span class="sxs-lookup"><span data-stu-id="dddaa-180">Valid values 1 to 16</span></span>|
|<span data-ttu-id="dddaa-181">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="dddaa-181">passwordRequiredType</span></span>|[<span data-ttu-id="dddaa-182">androidWorkProfileRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="dddaa-182">androidWorkProfileRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androidworkprofilerequiredpasswordtype.md)|<span data-ttu-id="dddaa-183">必需的密码类型。</span><span class="sxs-lookup"><span data-stu-id="dddaa-183">Type of password that is required.</span></span> <span data-ttu-id="dddaa-184">可取值为：`deviceDefault`、`lowSecurityBiometric`、`required`、`atLeastNumeric`、`numericComplex`、`atLeastAlphabetic`、`atLeastAlphanumeric`、`alphanumericWithSymbols`。</span><span class="sxs-lookup"><span data-stu-id="dddaa-184">Possible values are: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric`, `alphanumericWithSymbols`.</span></span>|
|<span data-ttu-id="dddaa-185">workProfileDataSharingType</span><span class="sxs-lookup"><span data-stu-id="dddaa-185">workProfileDataSharingType</span></span>|[<span data-ttu-id="dddaa-186">androidWorkProfileCrossProfileDataSharingType</span><span class="sxs-lookup"><span data-stu-id="dddaa-186">androidWorkProfileCrossProfileDataSharingType</span></span>](../resources/intune-deviceconfig-androidworkprofilecrossprofiledatasharingtype.md)|<span data-ttu-id="dddaa-187">允许的数据共享类型。</span><span class="sxs-lookup"><span data-stu-id="dddaa-187">Type of data sharing that is allowed.</span></span> <span data-ttu-id="dddaa-188">可取值为：`deviceDefault`、`preventAny`、`allowPersonalToWork`、`noRestrictions`。</span><span class="sxs-lookup"><span data-stu-id="dddaa-188">Possible values are: `deviceDefault`, `preventAny`, `allowPersonalToWork`, `noRestrictions`.</span></span>|
|<span data-ttu-id="dddaa-189">workProfileBlockNotificationsWhileDeviceLocked</span><span class="sxs-lookup"><span data-stu-id="dddaa-189">workProfileBlockNotificationsWhileDeviceLocked</span></span>|<span data-ttu-id="dddaa-190">Boolean</span><span class="sxs-lookup"><span data-stu-id="dddaa-190">Boolean</span></span>|<span data-ttu-id="dddaa-191">指示设备锁定时是否阻止通知。</span><span class="sxs-lookup"><span data-stu-id="dddaa-191">Indicates whether or not to block notifications while device locked.</span></span>|
|<span data-ttu-id="dddaa-192">workProfileBlockAddingAccounts</span><span class="sxs-lookup"><span data-stu-id="dddaa-192">workProfileBlockAddingAccounts</span></span>|<span data-ttu-id="dddaa-193">Boolean</span><span class="sxs-lookup"><span data-stu-id="dddaa-193">Boolean</span></span>|<span data-ttu-id="dddaa-194">阻止用户在工作配置文件中添加/删除帐户。</span><span class="sxs-lookup"><span data-stu-id="dddaa-194">Block users from adding/removing accounts in work profile.</span></span>|
|<span data-ttu-id="dddaa-195">workProfileBluetoothEnableContactSharing</span><span class="sxs-lookup"><span data-stu-id="dddaa-195">workProfileBluetoothEnableContactSharing</span></span>|<span data-ttu-id="dddaa-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="dddaa-196">Boolean</span></span>|<span data-ttu-id="dddaa-197">允许蓝牙设备访问企业联系人。</span><span class="sxs-lookup"><span data-stu-id="dddaa-197">Allow bluetooth devices to access enterprise contacts.</span></span>|
|<span data-ttu-id="dddaa-198">workProfileBlockScreenCapture</span><span class="sxs-lookup"><span data-stu-id="dddaa-198">workProfileBlockScreenCapture</span></span>|<span data-ttu-id="dddaa-199">Boolean</span><span class="sxs-lookup"><span data-stu-id="dddaa-199">Boolean</span></span>|<span data-ttu-id="dddaa-200">阻止工作配置文件中的屏幕捕获。</span><span class="sxs-lookup"><span data-stu-id="dddaa-200">Block screen capture in work profile.</span></span>|
|<span data-ttu-id="dddaa-201">workProfileBlockCrossProfileCallerId</span><span class="sxs-lookup"><span data-stu-id="dddaa-201">workProfileBlockCrossProfileCallerId</span></span>|<span data-ttu-id="dddaa-202">Boolean</span><span class="sxs-lookup"><span data-stu-id="dddaa-202">Boolean</span></span>|<span data-ttu-id="dddaa-203">阻止在个人配置文件中显示工作配置文件调用方 ID。</span><span class="sxs-lookup"><span data-stu-id="dddaa-203">Block display work profile caller ID in personal profile.</span></span>|
|<span data-ttu-id="dddaa-204">workProfileBlockCamera</span><span class="sxs-lookup"><span data-stu-id="dddaa-204">workProfileBlockCamera</span></span>|<span data-ttu-id="dddaa-205">Boolean</span><span class="sxs-lookup"><span data-stu-id="dddaa-205">Boolean</span></span>|<span data-ttu-id="dddaa-206">阻止工作配置文件相机。</span><span class="sxs-lookup"><span data-stu-id="dddaa-206">Block work profile camera.</span></span>|
|<span data-ttu-id="dddaa-207">workProfileBlockCrossProfileContactsSearch</span><span class="sxs-lookup"><span data-stu-id="dddaa-207">workProfileBlockCrossProfileContactsSearch</span></span>|<span data-ttu-id="dddaa-208">Boolean</span><span class="sxs-lookup"><span data-stu-id="dddaa-208">Boolean</span></span>|<span data-ttu-id="dddaa-209">阻止工作配置文件联系人在个人配置文件中的可用性。</span><span class="sxs-lookup"><span data-stu-id="dddaa-209">Block work profile contacts availability in personal profile.</span></span>|
|<span data-ttu-id="dddaa-210">workProfileBlockCrossProfileCopyPaste</span><span class="sxs-lookup"><span data-stu-id="dddaa-210">workProfileBlockCrossProfileCopyPaste</span></span>|<span data-ttu-id="dddaa-211">Boolean</span><span class="sxs-lookup"><span data-stu-id="dddaa-211">Boolean</span></span>|<span data-ttu-id="dddaa-212">指示设置是否禁用跨配置文件复制/粘贴的布尔值。</span><span class="sxs-lookup"><span data-stu-id="dddaa-212">Boolean that indicates if the setting disallow cross profile copy/paste is enabled.</span></span>|
|<span data-ttu-id="dddaa-213">workProfileDefaultAppPermissionPolicy</span><span class="sxs-lookup"><span data-stu-id="dddaa-213">workProfileDefaultAppPermissionPolicy</span></span>|[<span data-ttu-id="dddaa-214">androidWorkProfileDefaultAppPermissionPolicyType</span><span class="sxs-lookup"><span data-stu-id="dddaa-214">androidWorkProfileDefaultAppPermissionPolicyType</span></span>](../resources/intune-deviceconfig-androidworkprofiledefaultapppermissionpolicytype.md)|<span data-ttu-id="dddaa-215">必需的密码类型。</span><span class="sxs-lookup"><span data-stu-id="dddaa-215">Type of password that is required.</span></span> <span data-ttu-id="dddaa-216">可取值为：`deviceDefault`、`prompt`、`autoGrant`、`autoDeny`。</span><span class="sxs-lookup"><span data-stu-id="dddaa-216">Possible values are: `deviceDefault`, `prompt`, `autoGrant`, `autoDeny`.</span></span>|
|<span data-ttu-id="dddaa-217">workProfilePasswordBlockFingerprintUnlock</span><span class="sxs-lookup"><span data-stu-id="dddaa-217">workProfilePasswordBlockFingerprintUnlock</span></span>|<span data-ttu-id="dddaa-218">Boolean</span><span class="sxs-lookup"><span data-stu-id="dddaa-218">Boolean</span></span>|<span data-ttu-id="dddaa-219">指示是否阻止工作配置文件的指纹解锁。</span><span class="sxs-lookup"><span data-stu-id="dddaa-219">Indicates whether or not to block fingerprint unlock for work profile.</span></span>|
|<span data-ttu-id="dddaa-220">workProfilePasswordBlockTrustAgents</span><span class="sxs-lookup"><span data-stu-id="dddaa-220">workProfilePasswordBlockTrustAgents</span></span>|<span data-ttu-id="dddaa-221">Boolean</span><span class="sxs-lookup"><span data-stu-id="dddaa-221">Boolean</span></span>|<span data-ttu-id="dddaa-222">指示是否阻止工作配置文件的智能锁定和其他信任代理。</span><span class="sxs-lookup"><span data-stu-id="dddaa-222">Indicates whether or not to block Smart Lock and other trust agents for work profile.</span></span>|
|<span data-ttu-id="dddaa-223">workProfilePasswordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="dddaa-223">workProfilePasswordExpirationDays</span></span>|<span data-ttu-id="dddaa-224">Int32</span><span class="sxs-lookup"><span data-stu-id="dddaa-224">Int32</span></span>|<span data-ttu-id="dddaa-225">工作配置文件密码过期前的天数。</span><span class="sxs-lookup"><span data-stu-id="dddaa-225">Number of days before the work profile password expires.</span></span> <span data-ttu-id="dddaa-226">有效值为 1 至 365。</span><span class="sxs-lookup"><span data-stu-id="dddaa-226">Valid values 1 to 365</span></span>|
|<span data-ttu-id="dddaa-227">workProfilePasswordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="dddaa-227">workProfilePasswordMinimumLength</span></span>|<span data-ttu-id="dddaa-228">Int32</span><span class="sxs-lookup"><span data-stu-id="dddaa-228">Int32</span></span>|<span data-ttu-id="dddaa-229">工作配置文件密码的最小长度。</span><span class="sxs-lookup"><span data-stu-id="dddaa-229">Minimum length of work profile password.</span></span> <span data-ttu-id="dddaa-230">有效值为 4 至 16</span><span class="sxs-lookup"><span data-stu-id="dddaa-230">Valid values 4 to 16</span></span>|
|<span data-ttu-id="dddaa-231">workProfilePasswordMinNumericCharacters</span><span class="sxs-lookup"><span data-stu-id="dddaa-231">workProfilePasswordMinNumericCharacters</span></span>|<span data-ttu-id="dddaa-232">Int32</span><span class="sxs-lookup"><span data-stu-id="dddaa-232">Int32</span></span>|<span data-ttu-id="dddaa-233">工作配置文件密码中所需的数字字符的最小值。</span><span class="sxs-lookup"><span data-stu-id="dddaa-233">Minimum # of numeric characters required in work profile password.</span></span> <span data-ttu-id="dddaa-234">有效值为 1 到 10</span><span class="sxs-lookup"><span data-stu-id="dddaa-234">Valid values 1 to 10</span></span>|
|<span data-ttu-id="dddaa-235">workProfilePasswordMinNonLetterCharacters</span><span class="sxs-lookup"><span data-stu-id="dddaa-235">workProfilePasswordMinNonLetterCharacters</span></span>|<span data-ttu-id="dddaa-236">Int32</span><span class="sxs-lookup"><span data-stu-id="dddaa-236">Int32</span></span>|<span data-ttu-id="dddaa-237">工作配置文件密码中所需的非字母字符的最小值。</span><span class="sxs-lookup"><span data-stu-id="dddaa-237">Minimum # of non-letter characters required in work profile password.</span></span> <span data-ttu-id="dddaa-238">有效值为 1 到 10</span><span class="sxs-lookup"><span data-stu-id="dddaa-238">Valid values 1 to 10</span></span>|
|<span data-ttu-id="dddaa-239">workProfilePasswordMinLetterCharacters</span><span class="sxs-lookup"><span data-stu-id="dddaa-239">workProfilePasswordMinLetterCharacters</span></span>|<span data-ttu-id="dddaa-240">Int32</span><span class="sxs-lookup"><span data-stu-id="dddaa-240">Int32</span></span>|<span data-ttu-id="dddaa-241">工作配置文件密码中所需的最小字母字符数。</span><span class="sxs-lookup"><span data-stu-id="dddaa-241">Minimum # of letter characters required in work profile password.</span></span> <span data-ttu-id="dddaa-242">有效值为 1 到 10</span><span class="sxs-lookup"><span data-stu-id="dddaa-242">Valid values 1 to 10</span></span>|
|<span data-ttu-id="dddaa-243">workProfilePasswordMinLowerCaseCharacters</span><span class="sxs-lookup"><span data-stu-id="dddaa-243">workProfilePasswordMinLowerCaseCharacters</span></span>|<span data-ttu-id="dddaa-244">Int32</span><span class="sxs-lookup"><span data-stu-id="dddaa-244">Int32</span></span>|<span data-ttu-id="dddaa-245">工作配置文件密码中需要的最小小写字符数。</span><span class="sxs-lookup"><span data-stu-id="dddaa-245">Minimum # of lower-case characters required in work profile password.</span></span> <span data-ttu-id="dddaa-246">有效值为 1 到 10</span><span class="sxs-lookup"><span data-stu-id="dddaa-246">Valid values 1 to 10</span></span>|
|<span data-ttu-id="dddaa-247">workProfilePasswordMinUpperCaseCharacters</span><span class="sxs-lookup"><span data-stu-id="dddaa-247">workProfilePasswordMinUpperCaseCharacters</span></span>|<span data-ttu-id="dddaa-248">Int32</span><span class="sxs-lookup"><span data-stu-id="dddaa-248">Int32</span></span>|<span data-ttu-id="dddaa-249">工作配置文件密码中需要的最小大写字符数。</span><span class="sxs-lookup"><span data-stu-id="dddaa-249">Minimum # of upper-case characters required in work profile password.</span></span> <span data-ttu-id="dddaa-250">有效值为 1 到 10</span><span class="sxs-lookup"><span data-stu-id="dddaa-250">Valid values 1 to 10</span></span>|
|<span data-ttu-id="dddaa-251">workProfilePasswordMinSymbolCharacters</span><span class="sxs-lookup"><span data-stu-id="dddaa-251">workProfilePasswordMinSymbolCharacters</span></span>|<span data-ttu-id="dddaa-252">Int32</span><span class="sxs-lookup"><span data-stu-id="dddaa-252">Int32</span></span>|<span data-ttu-id="dddaa-253">工作配置文件密码中所需的符号的最小数。</span><span class="sxs-lookup"><span data-stu-id="dddaa-253">Minimum # of symbols required in work profile password.</span></span> <span data-ttu-id="dddaa-254">有效值为 1 到 10</span><span class="sxs-lookup"><span data-stu-id="dddaa-254">Valid values 1 to 10</span></span>|
|<span data-ttu-id="dddaa-255">workProfilePasswordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="dddaa-255">workProfilePasswordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="dddaa-256">Int32</span><span class="sxs-lookup"><span data-stu-id="dddaa-256">Int32</span></span>|<span data-ttu-id="dddaa-257">屏幕超时之前的不活动分钟数。</span><span class="sxs-lookup"><span data-stu-id="dddaa-257">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="dddaa-258">workProfilePasswordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="dddaa-258">workProfilePasswordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="dddaa-259">Int32</span><span class="sxs-lookup"><span data-stu-id="dddaa-259">Int32</span></span>|<span data-ttu-id="dddaa-260">要阻止的以前工作配置文件密码的数量。</span><span class="sxs-lookup"><span data-stu-id="dddaa-260">Number of previous work profile passwords to block.</span></span> <span data-ttu-id="dddaa-261">有效值为 0 至 24</span><span class="sxs-lookup"><span data-stu-id="dddaa-261">Valid values 0 to 24</span></span>|
|<span data-ttu-id="dddaa-262">workProfilePasswordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="dddaa-262">workProfilePasswordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="dddaa-263">Int32</span><span class="sxs-lookup"><span data-stu-id="dddaa-263">Int32</span></span>|<span data-ttu-id="dddaa-264">在删除工作配置文件和删除所有公司数据之前允许的登录失败次数。</span><span class="sxs-lookup"><span data-stu-id="dddaa-264">Number of sign in failures allowed before work profile is removed and all corporate data deleted.</span></span> <span data-ttu-id="dddaa-265">有效值为 1 到 16</span><span class="sxs-lookup"><span data-stu-id="dddaa-265">Valid values 1 to 16</span></span>|
|<span data-ttu-id="dddaa-266">workProfilePasswordRequiredType</span><span class="sxs-lookup"><span data-stu-id="dddaa-266">workProfilePasswordRequiredType</span></span>|[<span data-ttu-id="dddaa-267">androidWorkProfileRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="dddaa-267">androidWorkProfileRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androidworkprofilerequiredpasswordtype.md)|<span data-ttu-id="dddaa-268">所需的工作配置文件密码类型。</span><span class="sxs-lookup"><span data-stu-id="dddaa-268">Type of work profile password that is required.</span></span> <span data-ttu-id="dddaa-269">可取值为：`deviceDefault`、`lowSecurityBiometric`、`required`、`atLeastNumeric`、`numericComplex`、`atLeastAlphabetic`、`atLeastAlphanumeric`、`alphanumericWithSymbols`。</span><span class="sxs-lookup"><span data-stu-id="dddaa-269">Possible values are: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric`, `alphanumericWithSymbols`.</span></span>|
|<span data-ttu-id="dddaa-270">workProfileRequirePassword</span><span class="sxs-lookup"><span data-stu-id="dddaa-270">workProfileRequirePassword</span></span>|<span data-ttu-id="dddaa-271">Boolean</span><span class="sxs-lookup"><span data-stu-id="dddaa-271">Boolean</span></span>|<span data-ttu-id="dddaa-272">工作配置文件中是否要求密码</span><span class="sxs-lookup"><span data-stu-id="dddaa-272">Password is required or not for work profile</span></span>|
|<span data-ttu-id="dddaa-273">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="dddaa-273">securityRequireVerifyApps</span></span>|<span data-ttu-id="dddaa-274">Boolean</span><span class="sxs-lookup"><span data-stu-id="dddaa-274">Boolean</span></span>|<span data-ttu-id="dddaa-275">要求启用 Android 验证应用功能。</span><span class="sxs-lookup"><span data-stu-id="dddaa-275">Require the Android Verify apps feature is turned on.</span></span>|



## <a name="response"></a><span data-ttu-id="dddaa-276">响应</span><span class="sxs-lookup"><span data-stu-id="dddaa-276">Response</span></span>
<span data-ttu-id="dddaa-277">如果成功，此方法在响应正文中返回 响应代码和更新的 `200 OK` [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="dddaa-277">If successful, this method returns a `200 OK` response code and an updated [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dddaa-278">示例</span><span class="sxs-lookup"><span data-stu-id="dddaa-278">Example</span></span>

### <a name="request"></a><span data-ttu-id="dddaa-279">请求</span><span class="sxs-lookup"><span data-stu-id="dddaa-279">Request</span></span>
<span data-ttu-id="dddaa-280">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="dddaa-280">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="dddaa-281">响应</span><span class="sxs-lookup"><span data-stu-id="dddaa-281">Response</span></span>
<span data-ttu-id="dddaa-p126">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="dddaa-p126">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




