---
title: 创建 androidCompliancePolicy
description: 创建新的 androidCompliancePolicy 对象。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 833dc65c4eba3bd4e1fa3876d26540cdf0cac40d
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/29/2019
ms.locfileid: "30964666"
---
# <a name="create-androidcompliancepolicy"></a><span data-ttu-id="41563-103">创建 androidCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="41563-103">Create androidCompliancePolicy</span></span>

> <span data-ttu-id="41563-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="41563-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="41563-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="41563-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="41563-106">创建新的 [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="41563-106">Create a new [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="41563-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="41563-107">Prerequisites</span></span>
<span data-ttu-id="41563-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="41563-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="41563-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="41563-110">Permission type</span></span>|<span data-ttu-id="41563-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="41563-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="41563-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="41563-112">Delegated (work or school account)</span></span>|<span data-ttu-id="41563-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="41563-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="41563-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="41563-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="41563-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="41563-115">Not supported.</span></span>|
|<span data-ttu-id="41563-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="41563-116">Application</span></span>|<span data-ttu-id="41563-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="41563-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="41563-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="41563-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="41563-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="41563-119">Request headers</span></span>
|<span data-ttu-id="41563-120">标头</span><span class="sxs-lookup"><span data-stu-id="41563-120">Header</span></span>|<span data-ttu-id="41563-121">值</span><span class="sxs-lookup"><span data-stu-id="41563-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="41563-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="41563-122">Authorization</span></span>|<span data-ttu-id="41563-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="41563-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="41563-124">接受</span><span class="sxs-lookup"><span data-stu-id="41563-124">Accept</span></span>|<span data-ttu-id="41563-125">application/json</span><span class="sxs-lookup"><span data-stu-id="41563-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="41563-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="41563-126">Request body</span></span>
<span data-ttu-id="41563-127">在请求正文中，提供 androidCompliancePolicy 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="41563-127">In the request body, supply a JSON representation for the androidCompliancePolicy object.</span></span>

<span data-ttu-id="41563-128">下表显示了创建 androidCompliancePolicy 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="41563-128">The following table shows the properties that are required when you create the androidCompliancePolicy.</span></span>

|<span data-ttu-id="41563-129">属性</span><span class="sxs-lookup"><span data-stu-id="41563-129">Property</span></span>|<span data-ttu-id="41563-130">类型</span><span class="sxs-lookup"><span data-stu-id="41563-130">Type</span></span>|<span data-ttu-id="41563-131">说明</span><span class="sxs-lookup"><span data-stu-id="41563-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="41563-132">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="41563-132">roleScopeTagIds</span></span>|<span data-ttu-id="41563-133">String 集合</span><span class="sxs-lookup"><span data-stu-id="41563-133">String collection</span></span>|<span data-ttu-id="41563-134">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="41563-134">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="41563-135">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="41563-135">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="41563-136">id</span><span class="sxs-lookup"><span data-stu-id="41563-136">id</span></span>|<span data-ttu-id="41563-137">String</span><span class="sxs-lookup"><span data-stu-id="41563-137">String</span></span>|<span data-ttu-id="41563-138">实体的键。</span><span class="sxs-lookup"><span data-stu-id="41563-138">Key of the entity.</span></span> <span data-ttu-id="41563-139">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="41563-139">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="41563-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="41563-140">createdDateTime</span></span>|<span data-ttu-id="41563-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="41563-141">DateTimeOffset</span></span>|<span data-ttu-id="41563-142">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="41563-142">DateTime the object was created.</span></span> <span data-ttu-id="41563-143">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="41563-143">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="41563-144">description</span><span class="sxs-lookup"><span data-stu-id="41563-144">description</span></span>|<span data-ttu-id="41563-145">String</span><span class="sxs-lookup"><span data-stu-id="41563-145">String</span></span>|<span data-ttu-id="41563-146">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="41563-146">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="41563-147">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="41563-147">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="41563-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="41563-148">lastModifiedDateTime</span></span>|<span data-ttu-id="41563-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="41563-149">DateTimeOffset</span></span>|<span data-ttu-id="41563-150">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="41563-150">DateTime the object was last modified.</span></span> <span data-ttu-id="41563-151">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="41563-151">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="41563-152">displayName</span><span class="sxs-lookup"><span data-stu-id="41563-152">displayName</span></span>|<span data-ttu-id="41563-153">String</span><span class="sxs-lookup"><span data-stu-id="41563-153">String</span></span>|<span data-ttu-id="41563-154">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="41563-154">Admin provided name of the device configuration.</span></span> <span data-ttu-id="41563-155">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="41563-155">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="41563-156">version</span><span class="sxs-lookup"><span data-stu-id="41563-156">version</span></span>|<span data-ttu-id="41563-157">Int32</span><span class="sxs-lookup"><span data-stu-id="41563-157">Int32</span></span>|<span data-ttu-id="41563-158">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="41563-158">Version of the device configuration.</span></span> <span data-ttu-id="41563-159">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="41563-159">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="41563-160">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="41563-160">passwordRequired</span></span>|<span data-ttu-id="41563-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="41563-161">Boolean</span></span>|<span data-ttu-id="41563-162">需要密码才可解锁设备。</span><span class="sxs-lookup"><span data-stu-id="41563-162">Require a password to unlock device.</span></span>|
|<span data-ttu-id="41563-163">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="41563-163">passwordMinimumLength</span></span>|<span data-ttu-id="41563-164">Int32</span><span class="sxs-lookup"><span data-stu-id="41563-164">Int32</span></span>|<span data-ttu-id="41563-165">最短密码长度。</span><span class="sxs-lookup"><span data-stu-id="41563-165">Minimum password length.</span></span> <span data-ttu-id="41563-166">有效值为 4 至 16</span><span class="sxs-lookup"><span data-stu-id="41563-166">Valid values 4 to 16</span></span>|
|<span data-ttu-id="41563-167">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="41563-167">passwordRequiredType</span></span>|[<span data-ttu-id="41563-168">androidRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="41563-168">androidRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androidrequiredpasswordtype.md)|<span data-ttu-id="41563-169">密码中的字符类型。</span><span class="sxs-lookup"><span data-stu-id="41563-169">Type of characters in password.</span></span> <span data-ttu-id="41563-170">可取值为：`deviceDefault`、`alphabetic`、`alphanumeric`、`alphanumericWithSymbols`、`lowSecurityBiometric`、`numeric`、`numericComplex`、`any`。</span><span class="sxs-lookup"><span data-stu-id="41563-170">Possible values are: `deviceDefault`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `numeric`, `numericComplex`, `any`.</span></span>|
|<span data-ttu-id="41563-171">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="41563-171">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="41563-172">Int32</span><span class="sxs-lookup"><span data-stu-id="41563-172">Int32</span></span>|<span data-ttu-id="41563-173">在需要密码之前不活动的分钟数。</span><span class="sxs-lookup"><span data-stu-id="41563-173">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="41563-174">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="41563-174">passwordExpirationDays</span></span>|<span data-ttu-id="41563-175">Int32</span><span class="sxs-lookup"><span data-stu-id="41563-175">Int32</span></span>|<span data-ttu-id="41563-176">密码过期前的天数。</span><span class="sxs-lookup"><span data-stu-id="41563-176">Number of days before the password expires.</span></span> <span data-ttu-id="41563-177">有效值为 1 至 365</span><span class="sxs-lookup"><span data-stu-id="41563-177">Valid values 1 to 365</span></span>|
|<span data-ttu-id="41563-178">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="41563-178">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="41563-179">Int32</span><span class="sxs-lookup"><span data-stu-id="41563-179">Int32</span></span>|<span data-ttu-id="41563-180">要阻止的以前密码的数量。</span><span class="sxs-lookup"><span data-stu-id="41563-180">Number of previous passwords to block.</span></span> <span data-ttu-id="41563-181">有效值为 1 至 24</span><span class="sxs-lookup"><span data-stu-id="41563-181">Valid values 1 to 24</span></span>|
|<span data-ttu-id="41563-182">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="41563-182">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="41563-183">Int32</span><span class="sxs-lookup"><span data-stu-id="41563-183">Int32</span></span>|<span data-ttu-id="41563-184">在恢复出厂设置之前允许的登录失败次数。</span><span class="sxs-lookup"><span data-stu-id="41563-184">Number of sign-in failures allowed before factory reset.</span></span> <span data-ttu-id="41563-185">有效值为1至16</span><span class="sxs-lookup"><span data-stu-id="41563-185">Valid values 1 to 16</span></span>|
|<span data-ttu-id="41563-186">securityPreventInstallAppsFromUnknownSources</span><span class="sxs-lookup"><span data-stu-id="41563-186">securityPreventInstallAppsFromUnknownSources</span></span>|<span data-ttu-id="41563-187">Boolean</span><span class="sxs-lookup"><span data-stu-id="41563-187">Boolean</span></span>|<span data-ttu-id="41563-188">要求设备不允许安装来自未知源的应用。</span><span class="sxs-lookup"><span data-stu-id="41563-188">Require that devices disallow installation of apps from unknown sources.</span></span>|
|<span data-ttu-id="41563-189">securityDisableUsbDebugging</span><span class="sxs-lookup"><span data-stu-id="41563-189">securityDisableUsbDebugging</span></span>|<span data-ttu-id="41563-190">Boolean</span><span class="sxs-lookup"><span data-stu-id="41563-190">Boolean</span></span>|<span data-ttu-id="41563-191">在 Android 设备上禁用 USB 调试。</span><span class="sxs-lookup"><span data-stu-id="41563-191">Disable USB debugging on Android devices.</span></span>|
|<span data-ttu-id="41563-192">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="41563-192">securityRequireVerifyApps</span></span>|<span data-ttu-id="41563-193">Boolean</span><span class="sxs-lookup"><span data-stu-id="41563-193">Boolean</span></span>|<span data-ttu-id="41563-194">要求启用 Android 验证应用功能。</span><span class="sxs-lookup"><span data-stu-id="41563-194">Require the Android Verify apps feature is turned on.</span></span>|
|<span data-ttu-id="41563-195">deviceThreatProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="41563-195">deviceThreatProtectionEnabled</span></span>|<span data-ttu-id="41563-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="41563-196">Boolean</span></span>|<span data-ttu-id="41563-197">要求设备已启用设备威胁防护。</span><span class="sxs-lookup"><span data-stu-id="41563-197">Require that devices have enabled device threat protection.</span></span>|
|<span data-ttu-id="41563-198">deviceThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="41563-198">deviceThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="41563-199">deviceThreatProtectionLevel</span><span class="sxs-lookup"><span data-stu-id="41563-199">deviceThreatProtectionLevel</span></span>](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|<span data-ttu-id="41563-200">要求移动威胁防护最低风险级别来报告不符合情况。</span><span class="sxs-lookup"><span data-stu-id="41563-200">Require Mobile Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="41563-201">可取值为：`unavailable`、`secured`、`low`、`medium`、`high`、`notSet`。</span><span class="sxs-lookup"><span data-stu-id="41563-201">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="41563-202">securityBlockJailbrokenDevices</span><span class="sxs-lookup"><span data-stu-id="41563-202">securityBlockJailbrokenDevices</span></span>|<span data-ttu-id="41563-203">Boolean</span><span class="sxs-lookup"><span data-stu-id="41563-203">Boolean</span></span>|<span data-ttu-id="41563-204">设备不得越狱或取得 root 权限。</span><span class="sxs-lookup"><span data-stu-id="41563-204">Devices must not be jailbroken or rooted.</span></span>|
|<span data-ttu-id="41563-205">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="41563-205">osMinimumVersion</span></span>|<span data-ttu-id="41563-206">String</span><span class="sxs-lookup"><span data-stu-id="41563-206">String</span></span>|<span data-ttu-id="41563-207">最低 Android 版本。</span><span class="sxs-lookup"><span data-stu-id="41563-207">Minimum Android version.</span></span>|
|<span data-ttu-id="41563-208">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="41563-208">osMaximumVersion</span></span>|<span data-ttu-id="41563-209">String</span><span class="sxs-lookup"><span data-stu-id="41563-209">String</span></span>|<span data-ttu-id="41563-210">最高 Android 版本。</span><span class="sxs-lookup"><span data-stu-id="41563-210">Maximum Android version.</span></span>|
|<span data-ttu-id="41563-211">minAndroidSecurityPatchLevel</span><span class="sxs-lookup"><span data-stu-id="41563-211">minAndroidSecurityPatchLevel</span></span>|<span data-ttu-id="41563-212">String</span><span class="sxs-lookup"><span data-stu-id="41563-212">String</span></span>|<span data-ttu-id="41563-213">最低 Android 安全修补程序级别。</span><span class="sxs-lookup"><span data-stu-id="41563-213">Minimum Android security patch level.</span></span>|
|<span data-ttu-id="41563-214">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="41563-214">storageRequireEncryption</span></span>|<span data-ttu-id="41563-215">Boolean</span><span class="sxs-lookup"><span data-stu-id="41563-215">Boolean</span></span>|<span data-ttu-id="41563-216">要求对 Android 设备加密。</span><span class="sxs-lookup"><span data-stu-id="41563-216">Require encryption on Android devices.</span></span>|
|<span data-ttu-id="41563-217">securityRequireSafetyNetAttestationBasicIntegrity</span><span class="sxs-lookup"><span data-stu-id="41563-217">securityRequireSafetyNetAttestationBasicIntegrity</span></span>|<span data-ttu-id="41563-218">Boolean</span><span class="sxs-lookup"><span data-stu-id="41563-218">Boolean</span></span>|<span data-ttu-id="41563-219">要求设备传递 SafetyNet 基本完整性检查。</span><span class="sxs-lookup"><span data-stu-id="41563-219">Require the device to pass the SafetyNet basic integrity check.</span></span>|
|<span data-ttu-id="41563-220">securityRequireSafetyNetAttestationCertifiedDevice</span><span class="sxs-lookup"><span data-stu-id="41563-220">securityRequireSafetyNetAttestationCertifiedDevice</span></span>|<span data-ttu-id="41563-221">Boolean</span><span class="sxs-lookup"><span data-stu-id="41563-221">Boolean</span></span>|<span data-ttu-id="41563-222">要求设备传递 SafetyNet 认证设备检查。</span><span class="sxs-lookup"><span data-stu-id="41563-222">Require the device to pass the SafetyNet certified device check.</span></span>|
|<span data-ttu-id="41563-223">securityRequireGooglePlayServices</span><span class="sxs-lookup"><span data-stu-id="41563-223">securityRequireGooglePlayServices</span></span>|<span data-ttu-id="41563-224">Boolean</span><span class="sxs-lookup"><span data-stu-id="41563-224">Boolean</span></span>|<span data-ttu-id="41563-225">要求在设备上安装并启用 Google Play Services。</span><span class="sxs-lookup"><span data-stu-id="41563-225">Require Google Play Services to be installed and enabled on the device.</span></span>|
|<span data-ttu-id="41563-226">securityRequireUpToDateSecurityProviders</span><span class="sxs-lookup"><span data-stu-id="41563-226">securityRequireUpToDateSecurityProviders</span></span>|<span data-ttu-id="41563-227">Boolean</span><span class="sxs-lookup"><span data-stu-id="41563-227">Boolean</span></span>|<span data-ttu-id="41563-228">要求设备具有最新的安全提供程序。</span><span class="sxs-lookup"><span data-stu-id="41563-228">Require the device to have up to date security providers.</span></span> <span data-ttu-id="41563-229">设备将要求启用 Google Play Services 并保持最新状态。</span><span class="sxs-lookup"><span data-stu-id="41563-229">The device will require Google Play Services to be enabled and up to date.</span></span>|
|<span data-ttu-id="41563-230">securityRequireCompanyPortalAppIntegrity</span><span class="sxs-lookup"><span data-stu-id="41563-230">securityRequireCompanyPortalAppIntegrity</span></span>|<span data-ttu-id="41563-231">Boolean</span><span class="sxs-lookup"><span data-stu-id="41563-231">Boolean</span></span>|<span data-ttu-id="41563-232">要求设备传递公司门户客户端应用运行时完整性检查。</span><span class="sxs-lookup"><span data-stu-id="41563-232">Require the device to pass the Company Portal client app runtime integrity check.</span></span>|
|<span data-ttu-id="41563-233">conditionStatementId</span><span class="sxs-lookup"><span data-stu-id="41563-233">conditionStatementId</span></span>|<span data-ttu-id="41563-234">String</span><span class="sxs-lookup"><span data-stu-id="41563-234">String</span></span>|<span data-ttu-id="41563-235">条件语句 id。</span><span class="sxs-lookup"><span data-stu-id="41563-235">Condition statement id.</span></span>|
|<span data-ttu-id="41563-236">restrictedApps</span><span class="sxs-lookup"><span data-stu-id="41563-236">restrictedApps</span></span>|<span data-ttu-id="41563-237">[appListItem](../resources/intune-deviceconfig-applistitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="41563-237">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="41563-238">要求设备未安装指定的应用程序。</span><span class="sxs-lookup"><span data-stu-id="41563-238">Require the device to not have the specified apps installed.</span></span> <span data-ttu-id="41563-239">此集合最多可包含100个元素。</span><span class="sxs-lookup"><span data-stu-id="41563-239">This collection can contain a maximum of 100 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="41563-240">响应</span><span class="sxs-lookup"><span data-stu-id="41563-240">Response</span></span>
<span data-ttu-id="41563-241">如果成功，此方法会在响应正文中返回 `201 Created` 响应代码和 [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="41563-241">If successful, this method returns a `201 Created` response code and a [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="41563-242">示例</span><span class="sxs-lookup"><span data-stu-id="41563-242">Example</span></span>

### <a name="request"></a><span data-ttu-id="41563-243">请求</span><span class="sxs-lookup"><span data-stu-id="41563-243">Request</span></span>
<span data-ttu-id="41563-244">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="41563-244">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies
Content-type: application/json
Content-length: 1588

{
  "@odata.type": "#microsoft.graph.androidCompliancePolicy",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "passwordRequired": true,
  "passwordMinimumLength": 5,
  "passwordRequiredType": "alphabetic",
  "passwordMinutesOfInactivityBeforeLock": 5,
  "passwordExpirationDays": 6,
  "passwordPreviousPasswordBlockCount": 2,
  "passwordSignInFailureCountBeforeFactoryReset": 12,
  "securityPreventInstallAppsFromUnknownSources": true,
  "securityDisableUsbDebugging": true,
  "securityRequireVerifyApps": true,
  "deviceThreatProtectionEnabled": true,
  "deviceThreatProtectionRequiredSecurityLevel": "secured",
  "securityBlockJailbrokenDevices": true,
  "osMinimumVersion": "Os Minimum Version value",
  "osMaximumVersion": "Os Maximum Version value",
  "minAndroidSecurityPatchLevel": "Min Android Security Patch Level value",
  "storageRequireEncryption": true,
  "securityRequireSafetyNetAttestationBasicIntegrity": true,
  "securityRequireSafetyNetAttestationCertifiedDevice": true,
  "securityRequireGooglePlayServices": true,
  "securityRequireUpToDateSecurityProviders": true,
  "securityRequireCompanyPortalAppIntegrity": true,
  "conditionStatementId": "Condition Statement Id value",
  "restrictedApps": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="41563-245">响应</span><span class="sxs-lookup"><span data-stu-id="41563-245">Response</span></span>
<span data-ttu-id="41563-p117">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="41563-p117">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1760

{
  "@odata.type": "#microsoft.graph.androidCompliancePolicy",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "id": "752c820f-820f-752c-0f82-2c750f822c75",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "version": 7,
  "passwordRequired": true,
  "passwordMinimumLength": 5,
  "passwordRequiredType": "alphabetic",
  "passwordMinutesOfInactivityBeforeLock": 5,
  "passwordExpirationDays": 6,
  "passwordPreviousPasswordBlockCount": 2,
  "passwordSignInFailureCountBeforeFactoryReset": 12,
  "securityPreventInstallAppsFromUnknownSources": true,
  "securityDisableUsbDebugging": true,
  "securityRequireVerifyApps": true,
  "deviceThreatProtectionEnabled": true,
  "deviceThreatProtectionRequiredSecurityLevel": "secured",
  "securityBlockJailbrokenDevices": true,
  "osMinimumVersion": "Os Minimum Version value",
  "osMaximumVersion": "Os Maximum Version value",
  "minAndroidSecurityPatchLevel": "Min Android Security Patch Level value",
  "storageRequireEncryption": true,
  "securityRequireSafetyNetAttestationBasicIntegrity": true,
  "securityRequireSafetyNetAttestationCertifiedDevice": true,
  "securityRequireGooglePlayServices": true,
  "securityRequireUpToDateSecurityProviders": true,
  "securityRequireCompanyPortalAppIntegrity": true,
  "conditionStatementId": "Condition Statement Id value",
  "restrictedApps": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ]
}
```




