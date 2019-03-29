---
title: 创建 androidWorkProfileGeneralDeviceConfiguration
description: 创建新的 androidWorkProfileGeneralDeviceConfiguration 对象。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b0e1ae2e8eed358054163295dc8608a1bbaba68f
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/29/2019
ms.locfileid: "30960200"
---
# <a name="create-androidworkprofilegeneraldeviceconfiguration"></a><span data-ttu-id="63a23-103">创建 androidWorkProfileGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="63a23-103">Create androidWorkProfileGeneralDeviceConfiguration</span></span>

> <span data-ttu-id="63a23-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="63a23-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="63a23-105">创建新的[androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="63a23-105">Create a new [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="63a23-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="63a23-106">Prerequisites</span></span>
<span data-ttu-id="63a23-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="63a23-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="63a23-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="63a23-109">Permission type</span></span>|<span data-ttu-id="63a23-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="63a23-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="63a23-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="63a23-111">Delegated (work or school account)</span></span>|<span data-ttu-id="63a23-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="63a23-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="63a23-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="63a23-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="63a23-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="63a23-114">Not supported.</span></span>|
|<span data-ttu-id="63a23-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="63a23-115">Application</span></span>|<span data-ttu-id="63a23-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="63a23-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="63a23-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="63a23-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="63a23-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="63a23-118">Request headers</span></span>
|<span data-ttu-id="63a23-119">标头</span><span class="sxs-lookup"><span data-stu-id="63a23-119">Header</span></span>|<span data-ttu-id="63a23-120">值</span><span class="sxs-lookup"><span data-stu-id="63a23-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="63a23-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="63a23-121">Authorization</span></span>|<span data-ttu-id="63a23-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="63a23-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="63a23-123">接受</span><span class="sxs-lookup"><span data-stu-id="63a23-123">Accept</span></span>|<span data-ttu-id="63a23-124">application/json</span><span class="sxs-lookup"><span data-stu-id="63a23-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="63a23-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="63a23-125">Request body</span></span>
<span data-ttu-id="63a23-126">在请求正文中, 提供 androidWorkProfileGeneralDeviceConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="63a23-126">In the request body, supply a JSON representation for the androidWorkProfileGeneralDeviceConfiguration object.</span></span>

<span data-ttu-id="63a23-127">下表显示创建 androidWorkProfileGeneralDeviceConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="63a23-127">The following table shows the properties that are required when you create the androidWorkProfileGeneralDeviceConfiguration.</span></span>

|<span data-ttu-id="63a23-128">属性</span><span class="sxs-lookup"><span data-stu-id="63a23-128">Property</span></span>|<span data-ttu-id="63a23-129">类型</span><span class="sxs-lookup"><span data-stu-id="63a23-129">Type</span></span>|<span data-ttu-id="63a23-130">说明</span><span class="sxs-lookup"><span data-stu-id="63a23-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="63a23-131">id</span><span class="sxs-lookup"><span data-stu-id="63a23-131">id</span></span>|<span data-ttu-id="63a23-132">String</span><span class="sxs-lookup"><span data-stu-id="63a23-132">String</span></span>|<span data-ttu-id="63a23-133">实体的键。</span><span class="sxs-lookup"><span data-stu-id="63a23-133">Key of the entity.</span></span> <span data-ttu-id="63a23-134">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="63a23-134">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="63a23-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="63a23-135">lastModifiedDateTime</span></span>|<span data-ttu-id="63a23-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="63a23-136">DateTimeOffset</span></span>|<span data-ttu-id="63a23-137">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="63a23-137">DateTime the object was last modified.</span></span> <span data-ttu-id="63a23-138">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="63a23-138">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="63a23-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="63a23-139">createdDateTime</span></span>|<span data-ttu-id="63a23-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="63a23-140">DateTimeOffset</span></span>|<span data-ttu-id="63a23-141">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="63a23-141">DateTime the object was created.</span></span> <span data-ttu-id="63a23-142">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="63a23-142">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="63a23-143">description</span><span class="sxs-lookup"><span data-stu-id="63a23-143">description</span></span>|<span data-ttu-id="63a23-144">String</span><span class="sxs-lookup"><span data-stu-id="63a23-144">String</span></span>|<span data-ttu-id="63a23-145">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="63a23-145">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="63a23-146">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="63a23-146">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="63a23-147">displayName</span><span class="sxs-lookup"><span data-stu-id="63a23-147">displayName</span></span>|<span data-ttu-id="63a23-148">String</span><span class="sxs-lookup"><span data-stu-id="63a23-148">String</span></span>|<span data-ttu-id="63a23-149">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="63a23-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="63a23-150">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="63a23-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="63a23-151">version</span><span class="sxs-lookup"><span data-stu-id="63a23-151">version</span></span>|<span data-ttu-id="63a23-152">Int32</span><span class="sxs-lookup"><span data-stu-id="63a23-152">Int32</span></span>|<span data-ttu-id="63a23-153">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="63a23-153">Version of the device configuration.</span></span> <span data-ttu-id="63a23-154">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="63a23-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="63a23-155">passwordBlockFingerprintUnlock</span><span class="sxs-lookup"><span data-stu-id="63a23-155">passwordBlockFingerprintUnlock</span></span>|<span data-ttu-id="63a23-156">Boolean</span><span class="sxs-lookup"><span data-stu-id="63a23-156">Boolean</span></span>|<span data-ttu-id="63a23-157">指示是否阻止指纹解锁。</span><span class="sxs-lookup"><span data-stu-id="63a23-157">Indicates whether or not to block fingerprint unlock.</span></span>|
|<span data-ttu-id="63a23-158">passwordBlockTrustAgents</span><span class="sxs-lookup"><span data-stu-id="63a23-158">passwordBlockTrustAgents</span></span>|<span data-ttu-id="63a23-159">Boolean</span><span class="sxs-lookup"><span data-stu-id="63a23-159">Boolean</span></span>|<span data-ttu-id="63a23-160">指示是否阻止 Smart Lock 和其他信任代理。</span><span class="sxs-lookup"><span data-stu-id="63a23-160">Indicates whether or not to block Smart Lock and other trust agents.</span></span>|
|<span data-ttu-id="63a23-161">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="63a23-161">passwordExpirationDays</span></span>|<span data-ttu-id="63a23-162">Int32</span><span class="sxs-lookup"><span data-stu-id="63a23-162">Int32</span></span>|<span data-ttu-id="63a23-163">密码过期前的天数。</span><span class="sxs-lookup"><span data-stu-id="63a23-163">Number of days before the password expires.</span></span> <span data-ttu-id="63a23-164">有效值为 1 至 365。</span><span class="sxs-lookup"><span data-stu-id="63a23-164">Valid values 1 to 365</span></span>|
|<span data-ttu-id="63a23-165">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="63a23-165">passwordMinimumLength</span></span>|<span data-ttu-id="63a23-166">Int32</span><span class="sxs-lookup"><span data-stu-id="63a23-166">Int32</span></span>|<span data-ttu-id="63a23-167">密码的最小长度。</span><span class="sxs-lookup"><span data-stu-id="63a23-167">Minimum length of passwords.</span></span> <span data-ttu-id="63a23-168">有效值为 4 至 16</span><span class="sxs-lookup"><span data-stu-id="63a23-168">Valid values 4 to 16</span></span>|
|<span data-ttu-id="63a23-169">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="63a23-169">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="63a23-170">Int32</span><span class="sxs-lookup"><span data-stu-id="63a23-170">Int32</span></span>|<span data-ttu-id="63a23-171">屏幕超时之前的不活动分钟数。</span><span class="sxs-lookup"><span data-stu-id="63a23-171">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="63a23-172">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="63a23-172">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="63a23-173">Int32</span><span class="sxs-lookup"><span data-stu-id="63a23-173">Int32</span></span>|<span data-ttu-id="63a23-174">要阻止的以前密码的数量。</span><span class="sxs-lookup"><span data-stu-id="63a23-174">Number of previous passwords to block.</span></span> <span data-ttu-id="63a23-175">有效值为 0 至 24</span><span class="sxs-lookup"><span data-stu-id="63a23-175">Valid values 0 to 24</span></span>|
|<span data-ttu-id="63a23-176">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="63a23-176">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="63a23-177">Int32</span><span class="sxs-lookup"><span data-stu-id="63a23-177">Int32</span></span>|<span data-ttu-id="63a23-178">恢复出厂设置之前允许登录失败的次数。</span><span class="sxs-lookup"><span data-stu-id="63a23-178">Number of sign in failures allowed before factory reset.</span></span> <span data-ttu-id="63a23-179">有效值为1至16</span><span class="sxs-lookup"><span data-stu-id="63a23-179">Valid values 1 to 16</span></span>|
|<span data-ttu-id="63a23-180">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="63a23-180">passwordRequiredType</span></span>|[<span data-ttu-id="63a23-181">androidWorkProfileRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="63a23-181">androidWorkProfileRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androidworkprofilerequiredpasswordtype.md)|<span data-ttu-id="63a23-182">必需的密码类型。</span><span class="sxs-lookup"><span data-stu-id="63a23-182">Type of password that is required.</span></span> <span data-ttu-id="63a23-183">可取值为：`deviceDefault`、`lowSecurityBiometric`、`required`、`atLeastNumeric`、`numericComplex`、`atLeastAlphabetic`、`atLeastAlphanumeric`、`alphanumericWithSymbols`。</span><span class="sxs-lookup"><span data-stu-id="63a23-183">Possible values are: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric`, `alphanumericWithSymbols`.</span></span>|
|<span data-ttu-id="63a23-184">workProfileDataSharingType</span><span class="sxs-lookup"><span data-stu-id="63a23-184">workProfileDataSharingType</span></span>|[<span data-ttu-id="63a23-185">androidWorkProfileCrossProfileDataSharingType</span><span class="sxs-lookup"><span data-stu-id="63a23-185">androidWorkProfileCrossProfileDataSharingType</span></span>](../resources/intune-deviceconfig-androidworkprofilecrossprofiledatasharingtype.md)|<span data-ttu-id="63a23-186">允许的数据共享类型。</span><span class="sxs-lookup"><span data-stu-id="63a23-186">Type of data sharing that is allowed.</span></span> <span data-ttu-id="63a23-187">可取值为：`deviceDefault`、`preventAny`、`allowPersonalToWork`、`noRestrictions`。</span><span class="sxs-lookup"><span data-stu-id="63a23-187">Possible values are: `deviceDefault`, `preventAny`, `allowPersonalToWork`, `noRestrictions`.</span></span>|
|<span data-ttu-id="63a23-188">workProfileBlockNotificationsWhileDeviceLocked</span><span class="sxs-lookup"><span data-stu-id="63a23-188">workProfileBlockNotificationsWhileDeviceLocked</span></span>|<span data-ttu-id="63a23-189">Boolean</span><span class="sxs-lookup"><span data-stu-id="63a23-189">Boolean</span></span>|<span data-ttu-id="63a23-190">指示在设备锁定时是否阻止通知。</span><span class="sxs-lookup"><span data-stu-id="63a23-190">Indicates whether or not to block notifications while device locked.</span></span>|
|<span data-ttu-id="63a23-191">workProfileBlockAddingAccounts</span><span class="sxs-lookup"><span data-stu-id="63a23-191">workProfileBlockAddingAccounts</span></span>|<span data-ttu-id="63a23-192">Boolean</span><span class="sxs-lookup"><span data-stu-id="63a23-192">Boolean</span></span>|<span data-ttu-id="63a23-193">阻止用户在工作配置文件中添加/删除帐户。</span><span class="sxs-lookup"><span data-stu-id="63a23-193">Block users from adding/removing accounts in work profile.</span></span>|
|<span data-ttu-id="63a23-194">workProfileBluetoothEnableContactSharing</span><span class="sxs-lookup"><span data-stu-id="63a23-194">workProfileBluetoothEnableContactSharing</span></span>|<span data-ttu-id="63a23-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="63a23-195">Boolean</span></span>|<span data-ttu-id="63a23-196">允许蓝牙设备访问企业联系人。</span><span class="sxs-lookup"><span data-stu-id="63a23-196">Allow bluetooth devices to access enterprise contacts.</span></span>|
|<span data-ttu-id="63a23-197">workProfileBlockScreenCapture</span><span class="sxs-lookup"><span data-stu-id="63a23-197">workProfileBlockScreenCapture</span></span>|<span data-ttu-id="63a23-198">Boolean</span><span class="sxs-lookup"><span data-stu-id="63a23-198">Boolean</span></span>|<span data-ttu-id="63a23-199">在工作配置文件中阻止屏幕捕获。</span><span class="sxs-lookup"><span data-stu-id="63a23-199">Block screen capture in work profile.</span></span>|
|<span data-ttu-id="63a23-200">workProfileBlockCrossProfileCallerId</span><span class="sxs-lookup"><span data-stu-id="63a23-200">workProfileBlockCrossProfileCallerId</span></span>|<span data-ttu-id="63a23-201">Boolean</span><span class="sxs-lookup"><span data-stu-id="63a23-201">Boolean</span></span>|<span data-ttu-id="63a23-202">阻止显示个人配置文件中的工作配置文件呼叫者 ID。</span><span class="sxs-lookup"><span data-stu-id="63a23-202">Block display work profile caller ID in personal profile.</span></span>|
|<span data-ttu-id="63a23-203">workProfileBlockCamera</span><span class="sxs-lookup"><span data-stu-id="63a23-203">workProfileBlockCamera</span></span>|<span data-ttu-id="63a23-204">Boolean</span><span class="sxs-lookup"><span data-stu-id="63a23-204">Boolean</span></span>|<span data-ttu-id="63a23-205">阻止工作配置文件相机。</span><span class="sxs-lookup"><span data-stu-id="63a23-205">Block work profile camera.</span></span>|
|<span data-ttu-id="63a23-206">workProfileBlockCrossProfileContactsSearch</span><span class="sxs-lookup"><span data-stu-id="63a23-206">workProfileBlockCrossProfileContactsSearch</span></span>|<span data-ttu-id="63a23-207">Boolean</span><span class="sxs-lookup"><span data-stu-id="63a23-207">Boolean</span></span>|<span data-ttu-id="63a23-208">阻止个人配置文件中的工作配置文件联系人可用性。</span><span class="sxs-lookup"><span data-stu-id="63a23-208">Block work profile contacts availability in personal profile.</span></span>|
|<span data-ttu-id="63a23-209">workProfileBlockCrossProfileCopyPaste</span><span class="sxs-lookup"><span data-stu-id="63a23-209">workProfileBlockCrossProfileCopyPaste</span></span>|<span data-ttu-id="63a23-210">Boolean</span><span class="sxs-lookup"><span data-stu-id="63a23-210">Boolean</span></span>|<span data-ttu-id="63a23-211">指示是否启用 "禁用跨配置文件复制/粘贴" 设置的 Boolean。</span><span class="sxs-lookup"><span data-stu-id="63a23-211">Boolean that indicates if the setting disallow cross profile copy/paste is enabled.</span></span>|
|<span data-ttu-id="63a23-212">workProfileDefaultAppPermissionPolicy</span><span class="sxs-lookup"><span data-stu-id="63a23-212">workProfileDefaultAppPermissionPolicy</span></span>|[<span data-ttu-id="63a23-213">androidWorkProfileDefaultAppPermissionPolicyType</span><span class="sxs-lookup"><span data-stu-id="63a23-213">androidWorkProfileDefaultAppPermissionPolicyType</span></span>](../resources/intune-deviceconfig-androidworkprofiledefaultapppermissionpolicytype.md)|<span data-ttu-id="63a23-214">必需的密码类型。</span><span class="sxs-lookup"><span data-stu-id="63a23-214">Type of password that is required.</span></span> <span data-ttu-id="63a23-215">可取值为：`deviceDefault`、`prompt`、`autoGrant`、`autoDeny`。</span><span class="sxs-lookup"><span data-stu-id="63a23-215">Possible values are: `deviceDefault`, `prompt`, `autoGrant`, `autoDeny`.</span></span>|
|<span data-ttu-id="63a23-216">workProfilePasswordBlockFingerprintUnlock</span><span class="sxs-lookup"><span data-stu-id="63a23-216">workProfilePasswordBlockFingerprintUnlock</span></span>|<span data-ttu-id="63a23-217">Boolean</span><span class="sxs-lookup"><span data-stu-id="63a23-217">Boolean</span></span>|<span data-ttu-id="63a23-218">指示是否阻止工作配置文件的指纹解锁。</span><span class="sxs-lookup"><span data-stu-id="63a23-218">Indicates whether or not to block fingerprint unlock for work profile.</span></span>|
|<span data-ttu-id="63a23-219">workProfilePasswordBlockTrustAgents</span><span class="sxs-lookup"><span data-stu-id="63a23-219">workProfilePasswordBlockTrustAgents</span></span>|<span data-ttu-id="63a23-220">Boolean</span><span class="sxs-lookup"><span data-stu-id="63a23-220">Boolean</span></span>|<span data-ttu-id="63a23-221">指示是否阻止智能锁定和其他信任代理用于工作配置文件。</span><span class="sxs-lookup"><span data-stu-id="63a23-221">Indicates whether or not to block Smart Lock and other trust agents for work profile.</span></span>|
|<span data-ttu-id="63a23-222">workProfilePasswordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="63a23-222">workProfilePasswordExpirationDays</span></span>|<span data-ttu-id="63a23-223">Int32</span><span class="sxs-lookup"><span data-stu-id="63a23-223">Int32</span></span>|<span data-ttu-id="63a23-224">工作配置文件密码到期前的天数。</span><span class="sxs-lookup"><span data-stu-id="63a23-224">Number of days before the work profile password expires.</span></span> <span data-ttu-id="63a23-225">有效值为 1 至 365。</span><span class="sxs-lookup"><span data-stu-id="63a23-225">Valid values 1 to 365</span></span>|
|<span data-ttu-id="63a23-226">workProfilePasswordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="63a23-226">workProfilePasswordMinimumLength</span></span>|<span data-ttu-id="63a23-227">Int32</span><span class="sxs-lookup"><span data-stu-id="63a23-227">Int32</span></span>|<span data-ttu-id="63a23-228">工作配置文件密码的最小长度。</span><span class="sxs-lookup"><span data-stu-id="63a23-228">Minimum length of work profile password.</span></span> <span data-ttu-id="63a23-229">有效值为 4 至 16</span><span class="sxs-lookup"><span data-stu-id="63a23-229">Valid values 4 to 16</span></span>|
|<span data-ttu-id="63a23-230">workProfilePasswordMinNumericCharacters</span><span class="sxs-lookup"><span data-stu-id="63a23-230">workProfilePasswordMinNumericCharacters</span></span>|<span data-ttu-id="63a23-231">Int32</span><span class="sxs-lookup"><span data-stu-id="63a23-231">Int32</span></span>|<span data-ttu-id="63a23-232">工作配置文件密码中所需的最小数字字符数。</span><span class="sxs-lookup"><span data-stu-id="63a23-232">Minimum # of numeric characters required in work profile password.</span></span> <span data-ttu-id="63a23-233">有效值为1至10</span><span class="sxs-lookup"><span data-stu-id="63a23-233">Valid values 1 to 10</span></span>|
|<span data-ttu-id="63a23-234">workProfilePasswordMinNonLetterCharacters</span><span class="sxs-lookup"><span data-stu-id="63a23-234">workProfilePasswordMinNonLetterCharacters</span></span>|<span data-ttu-id="63a23-235">Int32</span><span class="sxs-lookup"><span data-stu-id="63a23-235">Int32</span></span>|<span data-ttu-id="63a23-236">工作配置文件密码中所需的最小非字母字符数。</span><span class="sxs-lookup"><span data-stu-id="63a23-236">Minimum # of non-letter characters required in work profile password.</span></span> <span data-ttu-id="63a23-237">有效值为1至10</span><span class="sxs-lookup"><span data-stu-id="63a23-237">Valid values 1 to 10</span></span>|
|<span data-ttu-id="63a23-238">workProfilePasswordMinLetterCharacters</span><span class="sxs-lookup"><span data-stu-id="63a23-238">workProfilePasswordMinLetterCharacters</span></span>|<span data-ttu-id="63a23-239">Int32</span><span class="sxs-lookup"><span data-stu-id="63a23-239">Int32</span></span>|<span data-ttu-id="63a23-240">工作配置文件密码中所需的字母字符的最小数目。</span><span class="sxs-lookup"><span data-stu-id="63a23-240">Minimum # of letter characters required in work profile password.</span></span> <span data-ttu-id="63a23-241">有效值为1至10</span><span class="sxs-lookup"><span data-stu-id="63a23-241">Valid values 1 to 10</span></span>|
|<span data-ttu-id="63a23-242">workProfilePasswordMinLowerCaseCharacters</span><span class="sxs-lookup"><span data-stu-id="63a23-242">workProfilePasswordMinLowerCaseCharacters</span></span>|<span data-ttu-id="63a23-243">Int32</span><span class="sxs-lookup"><span data-stu-id="63a23-243">Int32</span></span>|<span data-ttu-id="63a23-244">工作配置文件密码中所需的小写字符的最小数量。</span><span class="sxs-lookup"><span data-stu-id="63a23-244">Minimum # of lower-case characters required in work profile password.</span></span> <span data-ttu-id="63a23-245">有效值为1至10</span><span class="sxs-lookup"><span data-stu-id="63a23-245">Valid values 1 to 10</span></span>|
|<span data-ttu-id="63a23-246">workProfilePasswordMinUpperCaseCharacters</span><span class="sxs-lookup"><span data-stu-id="63a23-246">workProfilePasswordMinUpperCaseCharacters</span></span>|<span data-ttu-id="63a23-247">Int32</span><span class="sxs-lookup"><span data-stu-id="63a23-247">Int32</span></span>|<span data-ttu-id="63a23-248">工作配置文件密码中要求的大写字符的最小数量。</span><span class="sxs-lookup"><span data-stu-id="63a23-248">Minimum # of upper-case characters required in work profile password.</span></span> <span data-ttu-id="63a23-249">有效值为1至10</span><span class="sxs-lookup"><span data-stu-id="63a23-249">Valid values 1 to 10</span></span>|
|<span data-ttu-id="63a23-250">workProfilePasswordMinSymbolCharacters</span><span class="sxs-lookup"><span data-stu-id="63a23-250">workProfilePasswordMinSymbolCharacters</span></span>|<span data-ttu-id="63a23-251">Int32</span><span class="sxs-lookup"><span data-stu-id="63a23-251">Int32</span></span>|<span data-ttu-id="63a23-252">工作配置文件密码中所需的最小符号数。</span><span class="sxs-lookup"><span data-stu-id="63a23-252">Minimum # of symbols required in work profile password.</span></span> <span data-ttu-id="63a23-253">有效值为1至10</span><span class="sxs-lookup"><span data-stu-id="63a23-253">Valid values 1 to 10</span></span>|
|<span data-ttu-id="63a23-254">workProfilePasswordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="63a23-254">workProfilePasswordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="63a23-255">Int32</span><span class="sxs-lookup"><span data-stu-id="63a23-255">Int32</span></span>|<span data-ttu-id="63a23-256">屏幕超时之前的不活动分钟数。</span><span class="sxs-lookup"><span data-stu-id="63a23-256">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="63a23-257">workProfilePasswordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="63a23-257">workProfilePasswordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="63a23-258">Int32</span><span class="sxs-lookup"><span data-stu-id="63a23-258">Int32</span></span>|<span data-ttu-id="63a23-259">要阻止的以前的工作配置文件密码的数量。</span><span class="sxs-lookup"><span data-stu-id="63a23-259">Number of previous work profile passwords to block.</span></span> <span data-ttu-id="63a23-260">有效值为 0 至 24</span><span class="sxs-lookup"><span data-stu-id="63a23-260">Valid values 0 to 24</span></span>|
|<span data-ttu-id="63a23-261">workProfilePasswordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="63a23-261">workProfilePasswordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="63a23-262">Int32</span><span class="sxs-lookup"><span data-stu-id="63a23-262">Int32</span></span>|<span data-ttu-id="63a23-263">在删除工作配置文件和删除所有公司数据之前允许的登录失败次数。</span><span class="sxs-lookup"><span data-stu-id="63a23-263">Number of sign in failures allowed before work profile is removed and all corporate data deleted.</span></span> <span data-ttu-id="63a23-264">有效值为1至16</span><span class="sxs-lookup"><span data-stu-id="63a23-264">Valid values 1 to 16</span></span>|
|<span data-ttu-id="63a23-265">workProfilePasswordRequiredType</span><span class="sxs-lookup"><span data-stu-id="63a23-265">workProfilePasswordRequiredType</span></span>|[<span data-ttu-id="63a23-266">androidWorkProfileRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="63a23-266">androidWorkProfileRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androidworkprofilerequiredpasswordtype.md)|<span data-ttu-id="63a23-267">所需的工作配置文件密码类型。</span><span class="sxs-lookup"><span data-stu-id="63a23-267">Type of work profile password that is required.</span></span> <span data-ttu-id="63a23-268">可取值为：`deviceDefault`、`lowSecurityBiometric`、`required`、`atLeastNumeric`、`numericComplex`、`atLeastAlphabetic`、`atLeastAlphanumeric`、`alphanumericWithSymbols`。</span><span class="sxs-lookup"><span data-stu-id="63a23-268">Possible values are: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric`, `alphanumericWithSymbols`.</span></span>|
|<span data-ttu-id="63a23-269">workProfileRequirePassword</span><span class="sxs-lookup"><span data-stu-id="63a23-269">workProfileRequirePassword</span></span>|<span data-ttu-id="63a23-270">Boolean</span><span class="sxs-lookup"><span data-stu-id="63a23-270">Boolean</span></span>|<span data-ttu-id="63a23-271">对于工作配置文件, 密码是必需的</span><span class="sxs-lookup"><span data-stu-id="63a23-271">Password is required or not for work profile</span></span>|
|<span data-ttu-id="63a23-272">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="63a23-272">securityRequireVerifyApps</span></span>|<span data-ttu-id="63a23-273">Boolean</span><span class="sxs-lookup"><span data-stu-id="63a23-273">Boolean</span></span>|<span data-ttu-id="63a23-274">要求启用 Android 验证应用功能。</span><span class="sxs-lookup"><span data-stu-id="63a23-274">Require the Android Verify apps feature is turned on.</span></span>|



## <a name="response"></a><span data-ttu-id="63a23-275">响应</span><span class="sxs-lookup"><span data-stu-id="63a23-275">Response</span></span>
<span data-ttu-id="63a23-276">如果成功, 此方法在响应`201 Created`正文中返回响应代码和[androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="63a23-276">If successful, this method returns a `201 Created` response code and a [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="63a23-277">示例</span><span class="sxs-lookup"><span data-stu-id="63a23-277">Example</span></span>

### <a name="request"></a><span data-ttu-id="63a23-278">请求</span><span class="sxs-lookup"><span data-stu-id="63a23-278">Request</span></span>
<span data-ttu-id="63a23-279">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="63a23-279">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="63a23-280">响应</span><span class="sxs-lookup"><span data-stu-id="63a23-280">Response</span></span>
<span data-ttu-id="63a23-p126">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="63a23-p126">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



