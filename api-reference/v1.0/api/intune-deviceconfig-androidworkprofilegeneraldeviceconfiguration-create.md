---
title: 创建 androidWorkProfileGeneralDeviceConfiguration
description: 创建新的 androidWorkProfileGeneralDeviceConfiguration 对象。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 62ed82dcfd3892970491296597d414ac7677f9b6
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35997839"
---
# <a name="create-androidworkprofilegeneraldeviceconfiguration"></a><span data-ttu-id="bed00-103">创建 androidWorkProfileGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="bed00-103">Create androidWorkProfileGeneralDeviceConfiguration</span></span>

> <span data-ttu-id="bed00-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="bed00-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bed00-105">创建新的[androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="bed00-105">Create a new [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bed00-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="bed00-106">Prerequisites</span></span>
<span data-ttu-id="bed00-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="bed00-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bed00-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="bed00-109">Permission type</span></span>|<span data-ttu-id="bed00-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="bed00-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bed00-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="bed00-111">Delegated (work or school account)</span></span>|<span data-ttu-id="bed00-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bed00-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="bed00-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="bed00-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bed00-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="bed00-114">Not supported.</span></span>|
|<span data-ttu-id="bed00-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="bed00-115">Application</span></span>|<span data-ttu-id="bed00-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="bed00-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="bed00-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="bed00-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="bed00-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="bed00-118">Request headers</span></span>
|<span data-ttu-id="bed00-119">标头</span><span class="sxs-lookup"><span data-stu-id="bed00-119">Header</span></span>|<span data-ttu-id="bed00-120">值</span><span class="sxs-lookup"><span data-stu-id="bed00-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bed00-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="bed00-121">Authorization</span></span>|<span data-ttu-id="bed00-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="bed00-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bed00-123">接受</span><span class="sxs-lookup"><span data-stu-id="bed00-123">Accept</span></span>|<span data-ttu-id="bed00-124">application/json</span><span class="sxs-lookup"><span data-stu-id="bed00-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bed00-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="bed00-125">Request body</span></span>
<span data-ttu-id="bed00-126">在请求正文中, 提供 androidWorkProfileGeneralDeviceConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="bed00-126">In the request body, supply a JSON representation for the androidWorkProfileGeneralDeviceConfiguration object.</span></span>

<span data-ttu-id="bed00-127">下表显示创建 androidWorkProfileGeneralDeviceConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="bed00-127">The following table shows the properties that are required when you create the androidWorkProfileGeneralDeviceConfiguration.</span></span>

|<span data-ttu-id="bed00-128">属性</span><span class="sxs-lookup"><span data-stu-id="bed00-128">Property</span></span>|<span data-ttu-id="bed00-129">类型</span><span class="sxs-lookup"><span data-stu-id="bed00-129">Type</span></span>|<span data-ttu-id="bed00-130">说明</span><span class="sxs-lookup"><span data-stu-id="bed00-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bed00-131">id</span><span class="sxs-lookup"><span data-stu-id="bed00-131">id</span></span>|<span data-ttu-id="bed00-132">字符串</span><span class="sxs-lookup"><span data-stu-id="bed00-132">String</span></span>|<span data-ttu-id="bed00-133">实体的键。</span><span class="sxs-lookup"><span data-stu-id="bed00-133">Key of the entity.</span></span> <span data-ttu-id="bed00-134">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bed00-134">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bed00-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="bed00-135">lastModifiedDateTime</span></span>|<span data-ttu-id="bed00-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bed00-136">DateTimeOffset</span></span>|<span data-ttu-id="bed00-137">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="bed00-137">DateTime the object was last modified.</span></span> <span data-ttu-id="bed00-138">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bed00-138">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bed00-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="bed00-139">createdDateTime</span></span>|<span data-ttu-id="bed00-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bed00-140">DateTimeOffset</span></span>|<span data-ttu-id="bed00-141">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="bed00-141">DateTime the object was created.</span></span> <span data-ttu-id="bed00-142">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bed00-142">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bed00-143">说明</span><span class="sxs-lookup"><span data-stu-id="bed00-143">description</span></span>|<span data-ttu-id="bed00-144">String</span><span class="sxs-lookup"><span data-stu-id="bed00-144">String</span></span>|<span data-ttu-id="bed00-145">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="bed00-145">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="bed00-146">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bed00-146">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bed00-147">displayName</span><span class="sxs-lookup"><span data-stu-id="bed00-147">displayName</span></span>|<span data-ttu-id="bed00-148">String</span><span class="sxs-lookup"><span data-stu-id="bed00-148">String</span></span>|<span data-ttu-id="bed00-149">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="bed00-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="bed00-150">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bed00-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bed00-151">version</span><span class="sxs-lookup"><span data-stu-id="bed00-151">version</span></span>|<span data-ttu-id="bed00-152">Int32</span><span class="sxs-lookup"><span data-stu-id="bed00-152">Int32</span></span>|<span data-ttu-id="bed00-153">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="bed00-153">Version of the device configuration.</span></span> <span data-ttu-id="bed00-154">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bed00-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bed00-155">passwordBlockFingerprintUnlock</span><span class="sxs-lookup"><span data-stu-id="bed00-155">passwordBlockFingerprintUnlock</span></span>|<span data-ttu-id="bed00-156">Boolean</span><span class="sxs-lookup"><span data-stu-id="bed00-156">Boolean</span></span>|<span data-ttu-id="bed00-157">指示是否阻止指纹解锁。</span><span class="sxs-lookup"><span data-stu-id="bed00-157">Indicates whether or not to block fingerprint unlock.</span></span>|
|<span data-ttu-id="bed00-158">passwordBlockTrustAgents</span><span class="sxs-lookup"><span data-stu-id="bed00-158">passwordBlockTrustAgents</span></span>|<span data-ttu-id="bed00-159">Boolean</span><span class="sxs-lookup"><span data-stu-id="bed00-159">Boolean</span></span>|<span data-ttu-id="bed00-160">指示是否阻止 Smart Lock 和其他信任代理。</span><span class="sxs-lookup"><span data-stu-id="bed00-160">Indicates whether or not to block Smart Lock and other trust agents.</span></span>|
|<span data-ttu-id="bed00-161">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="bed00-161">passwordExpirationDays</span></span>|<span data-ttu-id="bed00-162">Int32</span><span class="sxs-lookup"><span data-stu-id="bed00-162">Int32</span></span>|<span data-ttu-id="bed00-163">密码过期前的天数。</span><span class="sxs-lookup"><span data-stu-id="bed00-163">Number of days before the password expires.</span></span> <span data-ttu-id="bed00-164">有效值为 1 至 365。</span><span class="sxs-lookup"><span data-stu-id="bed00-164">Valid values 1 to 365</span></span>|
|<span data-ttu-id="bed00-165">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="bed00-165">passwordMinimumLength</span></span>|<span data-ttu-id="bed00-166">Int32</span><span class="sxs-lookup"><span data-stu-id="bed00-166">Int32</span></span>|<span data-ttu-id="bed00-167">密码的最小长度。</span><span class="sxs-lookup"><span data-stu-id="bed00-167">Minimum length of passwords.</span></span> <span data-ttu-id="bed00-168">有效值为 4 至 16</span><span class="sxs-lookup"><span data-stu-id="bed00-168">Valid values 4 to 16</span></span>|
|<span data-ttu-id="bed00-169">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="bed00-169">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="bed00-170">Int32</span><span class="sxs-lookup"><span data-stu-id="bed00-170">Int32</span></span>|<span data-ttu-id="bed00-171">屏幕超时之前的不活动分钟数。</span><span class="sxs-lookup"><span data-stu-id="bed00-171">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="bed00-172">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="bed00-172">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="bed00-173">Int32</span><span class="sxs-lookup"><span data-stu-id="bed00-173">Int32</span></span>|<span data-ttu-id="bed00-174">要阻止的以前密码的数量。</span><span class="sxs-lookup"><span data-stu-id="bed00-174">Number of previous passwords to block.</span></span> <span data-ttu-id="bed00-175">有效值为 0 至 24</span><span class="sxs-lookup"><span data-stu-id="bed00-175">Valid values 0 to 24</span></span>|
|<span data-ttu-id="bed00-176">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="bed00-176">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="bed00-177">Int32</span><span class="sxs-lookup"><span data-stu-id="bed00-177">Int32</span></span>|<span data-ttu-id="bed00-178">恢复出厂设置之前允许登录失败的次数。</span><span class="sxs-lookup"><span data-stu-id="bed00-178">Number of sign in failures allowed before factory reset.</span></span> <span data-ttu-id="bed00-179">有效值为1至16</span><span class="sxs-lookup"><span data-stu-id="bed00-179">Valid values 1 to 16</span></span>|
|<span data-ttu-id="bed00-180">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="bed00-180">passwordRequiredType</span></span>|[<span data-ttu-id="bed00-181">androidWorkProfileRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="bed00-181">androidWorkProfileRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androidworkprofilerequiredpasswordtype.md)|<span data-ttu-id="bed00-182">必需的密码类型。</span><span class="sxs-lookup"><span data-stu-id="bed00-182">Type of password that is required.</span></span> <span data-ttu-id="bed00-183">可取值为：`deviceDefault`、`lowSecurityBiometric`、`required`、`atLeastNumeric`、`numericComplex`、`atLeastAlphabetic`、`atLeastAlphanumeric`、`alphanumericWithSymbols`。</span><span class="sxs-lookup"><span data-stu-id="bed00-183">Possible values are: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric`, `alphanumericWithSymbols`.</span></span>|
|<span data-ttu-id="bed00-184">workProfileDataSharingType</span><span class="sxs-lookup"><span data-stu-id="bed00-184">workProfileDataSharingType</span></span>|[<span data-ttu-id="bed00-185">androidWorkProfileCrossProfileDataSharingType</span><span class="sxs-lookup"><span data-stu-id="bed00-185">androidWorkProfileCrossProfileDataSharingType</span></span>](../resources/intune-deviceconfig-androidworkprofilecrossprofiledatasharingtype.md)|<span data-ttu-id="bed00-186">允许的数据共享类型。</span><span class="sxs-lookup"><span data-stu-id="bed00-186">Type of data sharing that is allowed.</span></span> <span data-ttu-id="bed00-187">可取值为：`deviceDefault`、`preventAny`、`allowPersonalToWork`、`noRestrictions`。</span><span class="sxs-lookup"><span data-stu-id="bed00-187">Possible values are: `deviceDefault`, `preventAny`, `allowPersonalToWork`, `noRestrictions`.</span></span>|
|<span data-ttu-id="bed00-188">workProfileBlockNotificationsWhileDeviceLocked</span><span class="sxs-lookup"><span data-stu-id="bed00-188">workProfileBlockNotificationsWhileDeviceLocked</span></span>|<span data-ttu-id="bed00-189">Boolean</span><span class="sxs-lookup"><span data-stu-id="bed00-189">Boolean</span></span>|<span data-ttu-id="bed00-190">指示在设备锁定时是否阻止通知。</span><span class="sxs-lookup"><span data-stu-id="bed00-190">Indicates whether or not to block notifications while device locked.</span></span>|
|<span data-ttu-id="bed00-191">workProfileBlockAddingAccounts</span><span class="sxs-lookup"><span data-stu-id="bed00-191">workProfileBlockAddingAccounts</span></span>|<span data-ttu-id="bed00-192">Boolean</span><span class="sxs-lookup"><span data-stu-id="bed00-192">Boolean</span></span>|<span data-ttu-id="bed00-193">阻止用户在工作配置文件中添加/删除帐户。</span><span class="sxs-lookup"><span data-stu-id="bed00-193">Block users from adding/removing accounts in work profile.</span></span>|
|<span data-ttu-id="bed00-194">workProfileBluetoothEnableContactSharing</span><span class="sxs-lookup"><span data-stu-id="bed00-194">workProfileBluetoothEnableContactSharing</span></span>|<span data-ttu-id="bed00-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="bed00-195">Boolean</span></span>|<span data-ttu-id="bed00-196">允许蓝牙设备访问企业联系人。</span><span class="sxs-lookup"><span data-stu-id="bed00-196">Allow bluetooth devices to access enterprise contacts.</span></span>|
|<span data-ttu-id="bed00-197">workProfileBlockScreenCapture</span><span class="sxs-lookup"><span data-stu-id="bed00-197">workProfileBlockScreenCapture</span></span>|<span data-ttu-id="bed00-198">Boolean</span><span class="sxs-lookup"><span data-stu-id="bed00-198">Boolean</span></span>|<span data-ttu-id="bed00-199">在工作配置文件中阻止屏幕捕获。</span><span class="sxs-lookup"><span data-stu-id="bed00-199">Block screen capture in work profile.</span></span>|
|<span data-ttu-id="bed00-200">workProfileBlockCrossProfileCallerId</span><span class="sxs-lookup"><span data-stu-id="bed00-200">workProfileBlockCrossProfileCallerId</span></span>|<span data-ttu-id="bed00-201">Boolean</span><span class="sxs-lookup"><span data-stu-id="bed00-201">Boolean</span></span>|<span data-ttu-id="bed00-202">阻止显示个人配置文件中的工作配置文件呼叫者 ID。</span><span class="sxs-lookup"><span data-stu-id="bed00-202">Block display work profile caller ID in personal profile.</span></span>|
|<span data-ttu-id="bed00-203">workProfileBlockCamera</span><span class="sxs-lookup"><span data-stu-id="bed00-203">workProfileBlockCamera</span></span>|<span data-ttu-id="bed00-204">Boolean</span><span class="sxs-lookup"><span data-stu-id="bed00-204">Boolean</span></span>|<span data-ttu-id="bed00-205">阻止工作配置文件相机。</span><span class="sxs-lookup"><span data-stu-id="bed00-205">Block work profile camera.</span></span>|
|<span data-ttu-id="bed00-206">workProfileBlockCrossProfileContactsSearch</span><span class="sxs-lookup"><span data-stu-id="bed00-206">workProfileBlockCrossProfileContactsSearch</span></span>|<span data-ttu-id="bed00-207">Boolean</span><span class="sxs-lookup"><span data-stu-id="bed00-207">Boolean</span></span>|<span data-ttu-id="bed00-208">阻止个人配置文件中的工作配置文件联系人可用性。</span><span class="sxs-lookup"><span data-stu-id="bed00-208">Block work profile contacts availability in personal profile.</span></span>|
|<span data-ttu-id="bed00-209">workProfileBlockCrossProfileCopyPaste</span><span class="sxs-lookup"><span data-stu-id="bed00-209">workProfileBlockCrossProfileCopyPaste</span></span>|<span data-ttu-id="bed00-210">Boolean</span><span class="sxs-lookup"><span data-stu-id="bed00-210">Boolean</span></span>|<span data-ttu-id="bed00-211">指示是否启用 "禁用跨配置文件复制/粘贴" 设置的 Boolean。</span><span class="sxs-lookup"><span data-stu-id="bed00-211">Boolean that indicates if the setting disallow cross profile copy/paste is enabled.</span></span>|
|<span data-ttu-id="bed00-212">workProfileDefaultAppPermissionPolicy</span><span class="sxs-lookup"><span data-stu-id="bed00-212">workProfileDefaultAppPermissionPolicy</span></span>|[<span data-ttu-id="bed00-213">androidWorkProfileDefaultAppPermissionPolicyType</span><span class="sxs-lookup"><span data-stu-id="bed00-213">androidWorkProfileDefaultAppPermissionPolicyType</span></span>](../resources/intune-deviceconfig-androidworkprofiledefaultapppermissionpolicytype.md)|<span data-ttu-id="bed00-214">必需的密码类型。</span><span class="sxs-lookup"><span data-stu-id="bed00-214">Type of password that is required.</span></span> <span data-ttu-id="bed00-215">可取值为：`deviceDefault`、`prompt`、`autoGrant`、`autoDeny`。</span><span class="sxs-lookup"><span data-stu-id="bed00-215">Possible values are: `deviceDefault`, `prompt`, `autoGrant`, `autoDeny`.</span></span>|
|<span data-ttu-id="bed00-216">workProfilePasswordBlockFingerprintUnlock</span><span class="sxs-lookup"><span data-stu-id="bed00-216">workProfilePasswordBlockFingerprintUnlock</span></span>|<span data-ttu-id="bed00-217">Boolean</span><span class="sxs-lookup"><span data-stu-id="bed00-217">Boolean</span></span>|<span data-ttu-id="bed00-218">指示是否阻止工作配置文件的指纹解锁。</span><span class="sxs-lookup"><span data-stu-id="bed00-218">Indicates whether or not to block fingerprint unlock for work profile.</span></span>|
|<span data-ttu-id="bed00-219">workProfilePasswordBlockTrustAgents</span><span class="sxs-lookup"><span data-stu-id="bed00-219">workProfilePasswordBlockTrustAgents</span></span>|<span data-ttu-id="bed00-220">Boolean</span><span class="sxs-lookup"><span data-stu-id="bed00-220">Boolean</span></span>|<span data-ttu-id="bed00-221">指示是否阻止智能锁定和其他信任代理用于工作配置文件。</span><span class="sxs-lookup"><span data-stu-id="bed00-221">Indicates whether or not to block Smart Lock and other trust agents for work profile.</span></span>|
|<span data-ttu-id="bed00-222">workProfilePasswordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="bed00-222">workProfilePasswordExpirationDays</span></span>|<span data-ttu-id="bed00-223">Int32</span><span class="sxs-lookup"><span data-stu-id="bed00-223">Int32</span></span>|<span data-ttu-id="bed00-224">工作配置文件密码到期前的天数。</span><span class="sxs-lookup"><span data-stu-id="bed00-224">Number of days before the work profile password expires.</span></span> <span data-ttu-id="bed00-225">有效值为 1 至 365。</span><span class="sxs-lookup"><span data-stu-id="bed00-225">Valid values 1 to 365</span></span>|
|<span data-ttu-id="bed00-226">workProfilePasswordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="bed00-226">workProfilePasswordMinimumLength</span></span>|<span data-ttu-id="bed00-227">Int32</span><span class="sxs-lookup"><span data-stu-id="bed00-227">Int32</span></span>|<span data-ttu-id="bed00-228">工作配置文件密码的最小长度。</span><span class="sxs-lookup"><span data-stu-id="bed00-228">Minimum length of work profile password.</span></span> <span data-ttu-id="bed00-229">有效值为 4 至 16</span><span class="sxs-lookup"><span data-stu-id="bed00-229">Valid values 4 to 16</span></span>|
|<span data-ttu-id="bed00-230">workProfilePasswordMinNumericCharacters</span><span class="sxs-lookup"><span data-stu-id="bed00-230">workProfilePasswordMinNumericCharacters</span></span>|<span data-ttu-id="bed00-231">Int32</span><span class="sxs-lookup"><span data-stu-id="bed00-231">Int32</span></span>|<span data-ttu-id="bed00-232">工作配置文件密码中所需的最小数字字符数。</span><span class="sxs-lookup"><span data-stu-id="bed00-232">Minimum # of numeric characters required in work profile password.</span></span> <span data-ttu-id="bed00-233">有效值为1至10</span><span class="sxs-lookup"><span data-stu-id="bed00-233">Valid values 1 to 10</span></span>|
|<span data-ttu-id="bed00-234">workProfilePasswordMinNonLetterCharacters</span><span class="sxs-lookup"><span data-stu-id="bed00-234">workProfilePasswordMinNonLetterCharacters</span></span>|<span data-ttu-id="bed00-235">Int32</span><span class="sxs-lookup"><span data-stu-id="bed00-235">Int32</span></span>|<span data-ttu-id="bed00-236">工作配置文件密码中所需的最小非字母字符数。</span><span class="sxs-lookup"><span data-stu-id="bed00-236">Minimum # of non-letter characters required in work profile password.</span></span> <span data-ttu-id="bed00-237">有效值为1至10</span><span class="sxs-lookup"><span data-stu-id="bed00-237">Valid values 1 to 10</span></span>|
|<span data-ttu-id="bed00-238">workProfilePasswordMinLetterCharacters</span><span class="sxs-lookup"><span data-stu-id="bed00-238">workProfilePasswordMinLetterCharacters</span></span>|<span data-ttu-id="bed00-239">Int32</span><span class="sxs-lookup"><span data-stu-id="bed00-239">Int32</span></span>|<span data-ttu-id="bed00-240">工作配置文件密码中所需的字母字符的最小数目。</span><span class="sxs-lookup"><span data-stu-id="bed00-240">Minimum # of letter characters required in work profile password.</span></span> <span data-ttu-id="bed00-241">有效值为1至10</span><span class="sxs-lookup"><span data-stu-id="bed00-241">Valid values 1 to 10</span></span>|
|<span data-ttu-id="bed00-242">workProfilePasswordMinLowerCaseCharacters</span><span class="sxs-lookup"><span data-stu-id="bed00-242">workProfilePasswordMinLowerCaseCharacters</span></span>|<span data-ttu-id="bed00-243">Int32</span><span class="sxs-lookup"><span data-stu-id="bed00-243">Int32</span></span>|<span data-ttu-id="bed00-244">工作配置文件密码中所需的小写字符的最小数量。</span><span class="sxs-lookup"><span data-stu-id="bed00-244">Minimum # of lower-case characters required in work profile password.</span></span> <span data-ttu-id="bed00-245">有效值为1至10</span><span class="sxs-lookup"><span data-stu-id="bed00-245">Valid values 1 to 10</span></span>|
|<span data-ttu-id="bed00-246">workProfilePasswordMinUpperCaseCharacters</span><span class="sxs-lookup"><span data-stu-id="bed00-246">workProfilePasswordMinUpperCaseCharacters</span></span>|<span data-ttu-id="bed00-247">Int32</span><span class="sxs-lookup"><span data-stu-id="bed00-247">Int32</span></span>|<span data-ttu-id="bed00-248">工作配置文件密码中要求的大写字符的最小数量。</span><span class="sxs-lookup"><span data-stu-id="bed00-248">Minimum # of upper-case characters required in work profile password.</span></span> <span data-ttu-id="bed00-249">有效值为1至10</span><span class="sxs-lookup"><span data-stu-id="bed00-249">Valid values 1 to 10</span></span>|
|<span data-ttu-id="bed00-250">workProfilePasswordMinSymbolCharacters</span><span class="sxs-lookup"><span data-stu-id="bed00-250">workProfilePasswordMinSymbolCharacters</span></span>|<span data-ttu-id="bed00-251">Int32</span><span class="sxs-lookup"><span data-stu-id="bed00-251">Int32</span></span>|<span data-ttu-id="bed00-252">工作配置文件密码中所需的最小符号数。</span><span class="sxs-lookup"><span data-stu-id="bed00-252">Minimum # of symbols required in work profile password.</span></span> <span data-ttu-id="bed00-253">有效值为1至10</span><span class="sxs-lookup"><span data-stu-id="bed00-253">Valid values 1 to 10</span></span>|
|<span data-ttu-id="bed00-254">workProfilePasswordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="bed00-254">workProfilePasswordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="bed00-255">Int32</span><span class="sxs-lookup"><span data-stu-id="bed00-255">Int32</span></span>|<span data-ttu-id="bed00-256">屏幕超时之前的不活动分钟数。</span><span class="sxs-lookup"><span data-stu-id="bed00-256">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="bed00-257">workProfilePasswordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="bed00-257">workProfilePasswordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="bed00-258">Int32</span><span class="sxs-lookup"><span data-stu-id="bed00-258">Int32</span></span>|<span data-ttu-id="bed00-259">要阻止的以前的工作配置文件密码的数量。</span><span class="sxs-lookup"><span data-stu-id="bed00-259">Number of previous work profile passwords to block.</span></span> <span data-ttu-id="bed00-260">有效值为 0 至 24</span><span class="sxs-lookup"><span data-stu-id="bed00-260">Valid values 0 to 24</span></span>|
|<span data-ttu-id="bed00-261">workProfilePasswordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="bed00-261">workProfilePasswordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="bed00-262">Int32</span><span class="sxs-lookup"><span data-stu-id="bed00-262">Int32</span></span>|<span data-ttu-id="bed00-263">在删除工作配置文件和删除所有公司数据之前允许的登录失败次数。</span><span class="sxs-lookup"><span data-stu-id="bed00-263">Number of sign in failures allowed before work profile is removed and all corporate data deleted.</span></span> <span data-ttu-id="bed00-264">有效值为1至16</span><span class="sxs-lookup"><span data-stu-id="bed00-264">Valid values 1 to 16</span></span>|
|<span data-ttu-id="bed00-265">workProfilePasswordRequiredType</span><span class="sxs-lookup"><span data-stu-id="bed00-265">workProfilePasswordRequiredType</span></span>|[<span data-ttu-id="bed00-266">androidWorkProfileRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="bed00-266">androidWorkProfileRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androidworkprofilerequiredpasswordtype.md)|<span data-ttu-id="bed00-267">所需的工作配置文件密码类型。</span><span class="sxs-lookup"><span data-stu-id="bed00-267">Type of work profile password that is required.</span></span> <span data-ttu-id="bed00-268">可取值为：`deviceDefault`、`lowSecurityBiometric`、`required`、`atLeastNumeric`、`numericComplex`、`atLeastAlphabetic`、`atLeastAlphanumeric`、`alphanumericWithSymbols`。</span><span class="sxs-lookup"><span data-stu-id="bed00-268">Possible values are: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric`, `alphanumericWithSymbols`.</span></span>|
|<span data-ttu-id="bed00-269">workProfileRequirePassword</span><span class="sxs-lookup"><span data-stu-id="bed00-269">workProfileRequirePassword</span></span>|<span data-ttu-id="bed00-270">Boolean</span><span class="sxs-lookup"><span data-stu-id="bed00-270">Boolean</span></span>|<span data-ttu-id="bed00-271">对于工作配置文件, 密码是必需的</span><span class="sxs-lookup"><span data-stu-id="bed00-271">Password is required or not for work profile</span></span>|
|<span data-ttu-id="bed00-272">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="bed00-272">securityRequireVerifyApps</span></span>|<span data-ttu-id="bed00-273">Boolean</span><span class="sxs-lookup"><span data-stu-id="bed00-273">Boolean</span></span>|<span data-ttu-id="bed00-274">要求启用 Android 验证应用功能。</span><span class="sxs-lookup"><span data-stu-id="bed00-274">Require the Android Verify apps feature is turned on.</span></span>|



## <a name="response"></a><span data-ttu-id="bed00-275">响应</span><span class="sxs-lookup"><span data-stu-id="bed00-275">Response</span></span>
<span data-ttu-id="bed00-276">如果成功, 此方法在响应`201 Created`正文中返回响应代码和[androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="bed00-276">If successful, this method returns a `201 Created` response code and a [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bed00-277">示例</span><span class="sxs-lookup"><span data-stu-id="bed00-277">Example</span></span>

### <a name="request"></a><span data-ttu-id="bed00-278">请求</span><span class="sxs-lookup"><span data-stu-id="bed00-278">Request</span></span>
<span data-ttu-id="bed00-279">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="bed00-279">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
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

### <a name="response"></a><span data-ttu-id="bed00-280">响应</span><span class="sxs-lookup"><span data-stu-id="bed00-280">Response</span></span>
<span data-ttu-id="bed00-p126">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="bed00-p126">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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



