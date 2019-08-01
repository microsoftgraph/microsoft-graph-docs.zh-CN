---
title: 创建 androidWorkProfileCompliancePolicy
description: 创建新的 androidWorkProfileCompliancePolicy 对象。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 23709a2b9949afeaf0872db32a59f1304a37bc1a
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36019588"
---
# <a name="create-androidworkprofilecompliancepolicy"></a><span data-ttu-id="cf7c0-103">创建 androidWorkProfileCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="cf7c0-103">Create androidWorkProfileCompliancePolicy</span></span>

> <span data-ttu-id="cf7c0-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="cf7c0-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cf7c0-105">创建新的[androidWorkProfileCompliancePolicy](../resources/intune-deviceconfig-androidworkprofilecompliancepolicy.md)对象。</span><span class="sxs-lookup"><span data-stu-id="cf7c0-105">Create a new [androidWorkProfileCompliancePolicy](../resources/intune-deviceconfig-androidworkprofilecompliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="cf7c0-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="cf7c0-106">Prerequisites</span></span>
<span data-ttu-id="cf7c0-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="cf7c0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cf7c0-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="cf7c0-109">Permission type</span></span>|<span data-ttu-id="cf7c0-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="cf7c0-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cf7c0-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="cf7c0-111">Delegated (work or school account)</span></span>|<span data-ttu-id="cf7c0-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cf7c0-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="cf7c0-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="cf7c0-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cf7c0-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="cf7c0-114">Not supported.</span></span>|
|<span data-ttu-id="cf7c0-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="cf7c0-115">Application</span></span>|<span data-ttu-id="cf7c0-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="cf7c0-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="cf7c0-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="cf7c0-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="cf7c0-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="cf7c0-118">Request headers</span></span>
|<span data-ttu-id="cf7c0-119">标头</span><span class="sxs-lookup"><span data-stu-id="cf7c0-119">Header</span></span>|<span data-ttu-id="cf7c0-120">值</span><span class="sxs-lookup"><span data-stu-id="cf7c0-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cf7c0-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="cf7c0-121">Authorization</span></span>|<span data-ttu-id="cf7c0-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="cf7c0-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cf7c0-123">接受</span><span class="sxs-lookup"><span data-stu-id="cf7c0-123">Accept</span></span>|<span data-ttu-id="cf7c0-124">application/json</span><span class="sxs-lookup"><span data-stu-id="cf7c0-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cf7c0-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="cf7c0-125">Request body</span></span>
<span data-ttu-id="cf7c0-126">在请求正文中, 提供 androidWorkProfileCompliancePolicy 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="cf7c0-126">In the request body, supply a JSON representation for the androidWorkProfileCompliancePolicy object.</span></span>

<span data-ttu-id="cf7c0-127">下表显示创建 androidWorkProfileCompliancePolicy 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="cf7c0-127">The following table shows the properties that are required when you create the androidWorkProfileCompliancePolicy.</span></span>

|<span data-ttu-id="cf7c0-128">属性</span><span class="sxs-lookup"><span data-stu-id="cf7c0-128">Property</span></span>|<span data-ttu-id="cf7c0-129">类型</span><span class="sxs-lookup"><span data-stu-id="cf7c0-129">Type</span></span>|<span data-ttu-id="cf7c0-130">说明</span><span class="sxs-lookup"><span data-stu-id="cf7c0-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cf7c0-131">id</span><span class="sxs-lookup"><span data-stu-id="cf7c0-131">id</span></span>|<span data-ttu-id="cf7c0-132">字符串</span><span class="sxs-lookup"><span data-stu-id="cf7c0-132">String</span></span>|<span data-ttu-id="cf7c0-133">实体的键。</span><span class="sxs-lookup"><span data-stu-id="cf7c0-133">Key of the entity.</span></span> <span data-ttu-id="cf7c0-134">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="cf7c0-134">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="cf7c0-135">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="cf7c0-135">createdDateTime</span></span>|<span data-ttu-id="cf7c0-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cf7c0-136">DateTimeOffset</span></span>|<span data-ttu-id="cf7c0-137">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="cf7c0-137">DateTime the object was created.</span></span> <span data-ttu-id="cf7c0-138">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="cf7c0-138">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="cf7c0-139">说明</span><span class="sxs-lookup"><span data-stu-id="cf7c0-139">description</span></span>|<span data-ttu-id="cf7c0-140">String</span><span class="sxs-lookup"><span data-stu-id="cf7c0-140">String</span></span>|<span data-ttu-id="cf7c0-141">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="cf7c0-141">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="cf7c0-142">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="cf7c0-142">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="cf7c0-143">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="cf7c0-143">lastModifiedDateTime</span></span>|<span data-ttu-id="cf7c0-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cf7c0-144">DateTimeOffset</span></span>|<span data-ttu-id="cf7c0-145">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="cf7c0-145">DateTime the object was last modified.</span></span> <span data-ttu-id="cf7c0-146">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="cf7c0-146">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="cf7c0-147">displayName</span><span class="sxs-lookup"><span data-stu-id="cf7c0-147">displayName</span></span>|<span data-ttu-id="cf7c0-148">字符串</span><span class="sxs-lookup"><span data-stu-id="cf7c0-148">String</span></span>|<span data-ttu-id="cf7c0-149">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="cf7c0-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="cf7c0-150">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="cf7c0-150">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="cf7c0-151">version</span><span class="sxs-lookup"><span data-stu-id="cf7c0-151">version</span></span>|<span data-ttu-id="cf7c0-152">Int32</span><span class="sxs-lookup"><span data-stu-id="cf7c0-152">Int32</span></span>|<span data-ttu-id="cf7c0-153">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="cf7c0-153">Version of the device configuration.</span></span> <span data-ttu-id="cf7c0-154">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="cf7c0-154">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="cf7c0-155">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="cf7c0-155">passwordRequired</span></span>|<span data-ttu-id="cf7c0-156">Boolean</span><span class="sxs-lookup"><span data-stu-id="cf7c0-156">Boolean</span></span>|<span data-ttu-id="cf7c0-157">需要密码才可解锁设备。</span><span class="sxs-lookup"><span data-stu-id="cf7c0-157">Require a password to unlock device.</span></span>|
|<span data-ttu-id="cf7c0-158">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="cf7c0-158">passwordMinimumLength</span></span>|<span data-ttu-id="cf7c0-159">Int32</span><span class="sxs-lookup"><span data-stu-id="cf7c0-159">Int32</span></span>|<span data-ttu-id="cf7c0-160">最短密码长度。</span><span class="sxs-lookup"><span data-stu-id="cf7c0-160">Minimum password length.</span></span> <span data-ttu-id="cf7c0-161">有效值为 4 至 16</span><span class="sxs-lookup"><span data-stu-id="cf7c0-161">Valid values 4 to 16</span></span>|
|<span data-ttu-id="cf7c0-162">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="cf7c0-162">passwordRequiredType</span></span>|[<span data-ttu-id="cf7c0-163">androidRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="cf7c0-163">androidRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androidrequiredpasswordtype.md)|<span data-ttu-id="cf7c0-164">密码中的字符类型。</span><span class="sxs-lookup"><span data-stu-id="cf7c0-164">Type of characters in password.</span></span> <span data-ttu-id="cf7c0-165">可取值为：`deviceDefault`、`alphabetic`、`alphanumeric`、`alphanumericWithSymbols`、`lowSecurityBiometric`、`numeric`、`numericComplex`、`any`。</span><span class="sxs-lookup"><span data-stu-id="cf7c0-165">Possible values are: `deviceDefault`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `numeric`, `numericComplex`, `any`.</span></span>|
|<span data-ttu-id="cf7c0-166">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="cf7c0-166">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="cf7c0-167">Int32</span><span class="sxs-lookup"><span data-stu-id="cf7c0-167">Int32</span></span>|<span data-ttu-id="cf7c0-168">在需要密码之前不活动的分钟数。</span><span class="sxs-lookup"><span data-stu-id="cf7c0-168">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="cf7c0-169">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="cf7c0-169">passwordExpirationDays</span></span>|<span data-ttu-id="cf7c0-170">Int32</span><span class="sxs-lookup"><span data-stu-id="cf7c0-170">Int32</span></span>|<span data-ttu-id="cf7c0-171">密码过期前的天数。</span><span class="sxs-lookup"><span data-stu-id="cf7c0-171">Number of days before the password expires.</span></span> <span data-ttu-id="cf7c0-172">有效值为 1 至 365</span><span class="sxs-lookup"><span data-stu-id="cf7c0-172">Valid values 1 to 365</span></span>|
|<span data-ttu-id="cf7c0-173">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="cf7c0-173">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="cf7c0-174">Int32</span><span class="sxs-lookup"><span data-stu-id="cf7c0-174">Int32</span></span>|<span data-ttu-id="cf7c0-175">要阻止的以前密码的数量。</span><span class="sxs-lookup"><span data-stu-id="cf7c0-175">Number of previous passwords to block.</span></span> <span data-ttu-id="cf7c0-176">有效值为 1 至 24</span><span class="sxs-lookup"><span data-stu-id="cf7c0-176">Valid values 1 to 24</span></span>|
|<span data-ttu-id="cf7c0-177">securityPreventInstallAppsFromUnknownSources</span><span class="sxs-lookup"><span data-stu-id="cf7c0-177">securityPreventInstallAppsFromUnknownSources</span></span>|<span data-ttu-id="cf7c0-178">Boolean</span><span class="sxs-lookup"><span data-stu-id="cf7c0-178">Boolean</span></span>|<span data-ttu-id="cf7c0-179">要求设备不允许安装来自未知源的应用。</span><span class="sxs-lookup"><span data-stu-id="cf7c0-179">Require that devices disallow installation of apps from unknown sources.</span></span>|
|<span data-ttu-id="cf7c0-180">securityDisableUsbDebugging</span><span class="sxs-lookup"><span data-stu-id="cf7c0-180">securityDisableUsbDebugging</span></span>|<span data-ttu-id="cf7c0-181">Boolean</span><span class="sxs-lookup"><span data-stu-id="cf7c0-181">Boolean</span></span>|<span data-ttu-id="cf7c0-182">在 Android 设备上禁用 USB 调试。</span><span class="sxs-lookup"><span data-stu-id="cf7c0-182">Disable USB debugging on Android devices.</span></span>|
|<span data-ttu-id="cf7c0-183">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="cf7c0-183">securityRequireVerifyApps</span></span>|<span data-ttu-id="cf7c0-184">Boolean</span><span class="sxs-lookup"><span data-stu-id="cf7c0-184">Boolean</span></span>|<span data-ttu-id="cf7c0-185">要求启用 Android 验证应用功能。</span><span class="sxs-lookup"><span data-stu-id="cf7c0-185">Require the Android Verify apps feature is turned on.</span></span>|
|<span data-ttu-id="cf7c0-186">deviceThreatProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="cf7c0-186">deviceThreatProtectionEnabled</span></span>|<span data-ttu-id="cf7c0-187">Boolean</span><span class="sxs-lookup"><span data-stu-id="cf7c0-187">Boolean</span></span>|<span data-ttu-id="cf7c0-188">要求设备已启用设备威胁防护。</span><span class="sxs-lookup"><span data-stu-id="cf7c0-188">Require that devices have enabled device threat protection.</span></span>|
|<span data-ttu-id="cf7c0-189">deviceThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="cf7c0-189">deviceThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="cf7c0-190">deviceThreatProtectionLevel</span><span class="sxs-lookup"><span data-stu-id="cf7c0-190">deviceThreatProtectionLevel</span></span>](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|<span data-ttu-id="cf7c0-191">要求移动威胁防护最低风险级别来报告不符合情况。</span><span class="sxs-lookup"><span data-stu-id="cf7c0-191">Require Mobile Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="cf7c0-192">可取值为：`unavailable`、`secured`、`low`、`medium`、`high`、`notSet`。</span><span class="sxs-lookup"><span data-stu-id="cf7c0-192">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="cf7c0-193">securityBlockJailbrokenDevices</span><span class="sxs-lookup"><span data-stu-id="cf7c0-193">securityBlockJailbrokenDevices</span></span>|<span data-ttu-id="cf7c0-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="cf7c0-194">Boolean</span></span>|<span data-ttu-id="cf7c0-195">设备不得越狱或取得 root 权限。</span><span class="sxs-lookup"><span data-stu-id="cf7c0-195">Devices must not be jailbroken or rooted.</span></span>|
|<span data-ttu-id="cf7c0-196">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="cf7c0-196">osMinimumVersion</span></span>|<span data-ttu-id="cf7c0-197">String</span><span class="sxs-lookup"><span data-stu-id="cf7c0-197">String</span></span>|<span data-ttu-id="cf7c0-198">最低 Android 版本。</span><span class="sxs-lookup"><span data-stu-id="cf7c0-198">Minimum Android version.</span></span>|
|<span data-ttu-id="cf7c0-199">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="cf7c0-199">osMaximumVersion</span></span>|<span data-ttu-id="cf7c0-200">String</span><span class="sxs-lookup"><span data-stu-id="cf7c0-200">String</span></span>|<span data-ttu-id="cf7c0-201">最高 Android 版本。</span><span class="sxs-lookup"><span data-stu-id="cf7c0-201">Maximum Android version.</span></span>|
|<span data-ttu-id="cf7c0-202">minAndroidSecurityPatchLevel</span><span class="sxs-lookup"><span data-stu-id="cf7c0-202">minAndroidSecurityPatchLevel</span></span>|<span data-ttu-id="cf7c0-203">String</span><span class="sxs-lookup"><span data-stu-id="cf7c0-203">String</span></span>|<span data-ttu-id="cf7c0-204">最低 Android 安全修补程序级别。</span><span class="sxs-lookup"><span data-stu-id="cf7c0-204">Minimum Android security patch level.</span></span>|
|<span data-ttu-id="cf7c0-205">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="cf7c0-205">storageRequireEncryption</span></span>|<span data-ttu-id="cf7c0-206">Boolean</span><span class="sxs-lookup"><span data-stu-id="cf7c0-206">Boolean</span></span>|<span data-ttu-id="cf7c0-207">要求对 Android 设备加密。</span><span class="sxs-lookup"><span data-stu-id="cf7c0-207">Require encryption on Android devices.</span></span>|
|<span data-ttu-id="cf7c0-208">securityRequireSafetyNetAttestationBasicIntegrity</span><span class="sxs-lookup"><span data-stu-id="cf7c0-208">securityRequireSafetyNetAttestationBasicIntegrity</span></span>|<span data-ttu-id="cf7c0-209">Boolean</span><span class="sxs-lookup"><span data-stu-id="cf7c0-209">Boolean</span></span>|<span data-ttu-id="cf7c0-210">要求设备传递 SafetyNet 基本完整性检查。</span><span class="sxs-lookup"><span data-stu-id="cf7c0-210">Require the device to pass the SafetyNet basic integrity check.</span></span>|
|<span data-ttu-id="cf7c0-211">securityRequireSafetyNetAttestationCertifiedDevice</span><span class="sxs-lookup"><span data-stu-id="cf7c0-211">securityRequireSafetyNetAttestationCertifiedDevice</span></span>|<span data-ttu-id="cf7c0-212">Boolean</span><span class="sxs-lookup"><span data-stu-id="cf7c0-212">Boolean</span></span>|<span data-ttu-id="cf7c0-213">要求设备传递 SafetyNet 认证设备检查。</span><span class="sxs-lookup"><span data-stu-id="cf7c0-213">Require the device to pass the SafetyNet certified device check.</span></span>|
|<span data-ttu-id="cf7c0-214">securityRequireGooglePlayServices</span><span class="sxs-lookup"><span data-stu-id="cf7c0-214">securityRequireGooglePlayServices</span></span>|<span data-ttu-id="cf7c0-215">Boolean</span><span class="sxs-lookup"><span data-stu-id="cf7c0-215">Boolean</span></span>|<span data-ttu-id="cf7c0-216">要求在设备上安装并启用 Google Play Services。</span><span class="sxs-lookup"><span data-stu-id="cf7c0-216">Require Google Play Services to be installed and enabled on the device.</span></span>|
|<span data-ttu-id="cf7c0-217">securityRequireUpToDateSecurityProviders</span><span class="sxs-lookup"><span data-stu-id="cf7c0-217">securityRequireUpToDateSecurityProviders</span></span>|<span data-ttu-id="cf7c0-218">Boolean</span><span class="sxs-lookup"><span data-stu-id="cf7c0-218">Boolean</span></span>|<span data-ttu-id="cf7c0-219">要求设备具有最新的安全提供程序。</span><span class="sxs-lookup"><span data-stu-id="cf7c0-219">Require the device to have up to date security providers.</span></span> <span data-ttu-id="cf7c0-220">设备将要求启用 Google Play Services 并保持最新状态。</span><span class="sxs-lookup"><span data-stu-id="cf7c0-220">The device will require Google Play Services to be enabled and up to date.</span></span>|
|<span data-ttu-id="cf7c0-221">securityRequireCompanyPortalAppIntegrity</span><span class="sxs-lookup"><span data-stu-id="cf7c0-221">securityRequireCompanyPortalAppIntegrity</span></span>|<span data-ttu-id="cf7c0-222">Boolean</span><span class="sxs-lookup"><span data-stu-id="cf7c0-222">Boolean</span></span>|<span data-ttu-id="cf7c0-223">要求设备传递公司门户客户端应用运行时完整性检查。</span><span class="sxs-lookup"><span data-stu-id="cf7c0-223">Require the device to pass the Company Portal client app runtime integrity check.</span></span>|



## <a name="response"></a><span data-ttu-id="cf7c0-224">响应</span><span class="sxs-lookup"><span data-stu-id="cf7c0-224">Response</span></span>
<span data-ttu-id="cf7c0-225">如果成功, 此方法在响应`201 Created`正文中返回响应代码和[androidWorkProfileCompliancePolicy](../resources/intune-deviceconfig-androidworkprofilecompliancepolicy.md)对象。</span><span class="sxs-lookup"><span data-stu-id="cf7c0-225">If successful, this method returns a `201 Created` response code and a [androidWorkProfileCompliancePolicy](../resources/intune-deviceconfig-androidworkprofilecompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cf7c0-226">示例</span><span class="sxs-lookup"><span data-stu-id="cf7c0-226">Example</span></span>

### <a name="request"></a><span data-ttu-id="cf7c0-227">请求</span><span class="sxs-lookup"><span data-stu-id="cf7c0-227">Request</span></span>
<span data-ttu-id="cf7c0-228">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="cf7c0-228">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies
Content-type: application/json
Content-length: 1170

{
  "@odata.type": "#microsoft.graph.androidWorkProfileCompliancePolicy",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "passwordRequired": true,
  "passwordMinimumLength": 5,
  "passwordRequiredType": "alphabetic",
  "passwordMinutesOfInactivityBeforeLock": 5,
  "passwordExpirationDays": 6,
  "passwordPreviousPasswordBlockCount": 2,
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
  "securityRequireCompanyPortalAppIntegrity": true
}
```

### <a name="response"></a><span data-ttu-id="cf7c0-229">响应</span><span class="sxs-lookup"><span data-stu-id="cf7c0-229">Response</span></span>
<span data-ttu-id="cf7c0-p114">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="cf7c0-p114">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1342

{
  "@odata.type": "#microsoft.graph.androidWorkProfileCompliancePolicy",
  "id": "4e385271-5271-4e38-7152-384e7152384e",
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
  "securityRequireCompanyPortalAppIntegrity": true
}
```



