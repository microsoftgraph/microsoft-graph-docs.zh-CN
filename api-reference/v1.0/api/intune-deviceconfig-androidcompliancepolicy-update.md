---
title: 更新 androidCompliancePolicy
description: 更新 androidCompliancePolicy 对象的属性。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 8fc8fcae7881caaff174c3464b02480d0d0e0080
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/02/2019
ms.locfileid: "37357638"
---
# <a name="update-androidcompliancepolicy"></a><span data-ttu-id="b6261-103">更新 androidCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="b6261-103">Update androidCompliancePolicy</span></span>

> <span data-ttu-id="b6261-104">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b6261-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b6261-105">更新 [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="b6261-105">Update the properties of a [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b6261-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="b6261-106">Prerequisites</span></span>
<span data-ttu-id="b6261-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b6261-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b6261-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="b6261-109">Permission type</span></span>|<span data-ttu-id="b6261-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="b6261-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b6261-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b6261-111">Delegated (work or school account)</span></span>|<span data-ttu-id="b6261-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b6261-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b6261-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b6261-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b6261-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="b6261-114">Not supported.</span></span>|
|<span data-ttu-id="b6261-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="b6261-115">Application</span></span>|<span data-ttu-id="b6261-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="b6261-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b6261-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b6261-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="b6261-118">请求头</span><span class="sxs-lookup"><span data-stu-id="b6261-118">Request headers</span></span>
|<span data-ttu-id="b6261-119">标头</span><span class="sxs-lookup"><span data-stu-id="b6261-119">Header</span></span>|<span data-ttu-id="b6261-120">值</span><span class="sxs-lookup"><span data-stu-id="b6261-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b6261-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="b6261-121">Authorization</span></span>|<span data-ttu-id="b6261-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="b6261-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b6261-123">接受</span><span class="sxs-lookup"><span data-stu-id="b6261-123">Accept</span></span>|<span data-ttu-id="b6261-124">application/json</span><span class="sxs-lookup"><span data-stu-id="b6261-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b6261-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="b6261-125">Request body</span></span>
<span data-ttu-id="b6261-126">在请求正文中，提供 [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b6261-126">In the request body, supply a JSON representation for the [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md) object.</span></span>

<span data-ttu-id="b6261-127">下表显示了创建 [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="b6261-127">The following table shows the properties that are required when you create the [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md).</span></span>

|<span data-ttu-id="b6261-128">属性</span><span class="sxs-lookup"><span data-stu-id="b6261-128">Property</span></span>|<span data-ttu-id="b6261-129">类型</span><span class="sxs-lookup"><span data-stu-id="b6261-129">Type</span></span>|<span data-ttu-id="b6261-130">说明</span><span class="sxs-lookup"><span data-stu-id="b6261-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b6261-131">id</span><span class="sxs-lookup"><span data-stu-id="b6261-131">id</span></span>|<span data-ttu-id="b6261-132">字符串</span><span class="sxs-lookup"><span data-stu-id="b6261-132">String</span></span>|<span data-ttu-id="b6261-133">实体的键。</span><span class="sxs-lookup"><span data-stu-id="b6261-133">Key of the entity.</span></span> <span data-ttu-id="b6261-134">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="b6261-134">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="b6261-135">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b6261-135">createdDateTime</span></span>|<span data-ttu-id="b6261-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b6261-136">DateTimeOffset</span></span>|<span data-ttu-id="b6261-137">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="b6261-137">DateTime the object was created.</span></span> <span data-ttu-id="b6261-138">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="b6261-138">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="b6261-139">说明</span><span class="sxs-lookup"><span data-stu-id="b6261-139">description</span></span>|<span data-ttu-id="b6261-140">String</span><span class="sxs-lookup"><span data-stu-id="b6261-140">String</span></span>|<span data-ttu-id="b6261-141">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="b6261-141">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="b6261-142">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="b6261-142">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="b6261-143">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b6261-143">lastModifiedDateTime</span></span>|<span data-ttu-id="b6261-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b6261-144">DateTimeOffset</span></span>|<span data-ttu-id="b6261-145">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="b6261-145">DateTime the object was last modified.</span></span> <span data-ttu-id="b6261-146">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="b6261-146">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="b6261-147">displayName</span><span class="sxs-lookup"><span data-stu-id="b6261-147">displayName</span></span>|<span data-ttu-id="b6261-148">字符串</span><span class="sxs-lookup"><span data-stu-id="b6261-148">String</span></span>|<span data-ttu-id="b6261-149">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="b6261-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="b6261-150">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="b6261-150">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="b6261-151">version</span><span class="sxs-lookup"><span data-stu-id="b6261-151">version</span></span>|<span data-ttu-id="b6261-152">Int32</span><span class="sxs-lookup"><span data-stu-id="b6261-152">Int32</span></span>|<span data-ttu-id="b6261-153">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="b6261-153">Version of the device configuration.</span></span> <span data-ttu-id="b6261-154">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="b6261-154">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="b6261-155">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="b6261-155">passwordRequired</span></span>|<span data-ttu-id="b6261-156">Boolean</span><span class="sxs-lookup"><span data-stu-id="b6261-156">Boolean</span></span>|<span data-ttu-id="b6261-157">需要密码才可解锁设备。</span><span class="sxs-lookup"><span data-stu-id="b6261-157">Require a password to unlock device.</span></span>|
|<span data-ttu-id="b6261-158">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="b6261-158">passwordMinimumLength</span></span>|<span data-ttu-id="b6261-159">Int32</span><span class="sxs-lookup"><span data-stu-id="b6261-159">Int32</span></span>|<span data-ttu-id="b6261-160">最短密码长度。</span><span class="sxs-lookup"><span data-stu-id="b6261-160">Minimum password length.</span></span> <span data-ttu-id="b6261-161">有效值为 4 至 16</span><span class="sxs-lookup"><span data-stu-id="b6261-161">Valid values 4 to 16</span></span>|
|<span data-ttu-id="b6261-162">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="b6261-162">passwordRequiredType</span></span>|[<span data-ttu-id="b6261-163">androidRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="b6261-163">androidRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androidrequiredpasswordtype.md)|<span data-ttu-id="b6261-164">密码中的字符类型。</span><span class="sxs-lookup"><span data-stu-id="b6261-164">Type of characters in password.</span></span> <span data-ttu-id="b6261-165">可取值为：`deviceDefault`、`alphabetic`、`alphanumeric`、`alphanumericWithSymbols`、`lowSecurityBiometric`、`numeric`、`numericComplex`、`any`。</span><span class="sxs-lookup"><span data-stu-id="b6261-165">Possible values are: `deviceDefault`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `numeric`, `numericComplex`, `any`.</span></span>|
|<span data-ttu-id="b6261-166">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="b6261-166">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="b6261-167">Int32</span><span class="sxs-lookup"><span data-stu-id="b6261-167">Int32</span></span>|<span data-ttu-id="b6261-168">在需要密码之前不活动的分钟数。</span><span class="sxs-lookup"><span data-stu-id="b6261-168">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="b6261-169">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="b6261-169">passwordExpirationDays</span></span>|<span data-ttu-id="b6261-170">Int32</span><span class="sxs-lookup"><span data-stu-id="b6261-170">Int32</span></span>|<span data-ttu-id="b6261-171">密码过期前的天数。</span><span class="sxs-lookup"><span data-stu-id="b6261-171">Number of days before the password expires.</span></span> <span data-ttu-id="b6261-172">有效值为 1 至 365</span><span class="sxs-lookup"><span data-stu-id="b6261-172">Valid values 1 to 365</span></span>|
|<span data-ttu-id="b6261-173">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="b6261-173">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="b6261-174">Int32</span><span class="sxs-lookup"><span data-stu-id="b6261-174">Int32</span></span>|<span data-ttu-id="b6261-175">要阻止的以前密码的数量。</span><span class="sxs-lookup"><span data-stu-id="b6261-175">Number of previous passwords to block.</span></span> <span data-ttu-id="b6261-176">有效值为 1 至 24</span><span class="sxs-lookup"><span data-stu-id="b6261-176">Valid values 1 to 24</span></span>|
|<span data-ttu-id="b6261-177">securityPreventInstallAppsFromUnknownSources</span><span class="sxs-lookup"><span data-stu-id="b6261-177">securityPreventInstallAppsFromUnknownSources</span></span>|<span data-ttu-id="b6261-178">Boolean</span><span class="sxs-lookup"><span data-stu-id="b6261-178">Boolean</span></span>|<span data-ttu-id="b6261-179">要求设备不允许安装来自未知源的应用。</span><span class="sxs-lookup"><span data-stu-id="b6261-179">Require that devices disallow installation of apps from unknown sources.</span></span>|
|<span data-ttu-id="b6261-180">securityDisableUsbDebugging</span><span class="sxs-lookup"><span data-stu-id="b6261-180">securityDisableUsbDebugging</span></span>|<span data-ttu-id="b6261-181">Boolean</span><span class="sxs-lookup"><span data-stu-id="b6261-181">Boolean</span></span>|<span data-ttu-id="b6261-182">在 Android 设备上禁用 USB 调试。</span><span class="sxs-lookup"><span data-stu-id="b6261-182">Disable USB debugging on Android devices.</span></span>|
|<span data-ttu-id="b6261-183">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="b6261-183">securityRequireVerifyApps</span></span>|<span data-ttu-id="b6261-184">Boolean</span><span class="sxs-lookup"><span data-stu-id="b6261-184">Boolean</span></span>|<span data-ttu-id="b6261-185">要求启用 Android 验证应用功能。</span><span class="sxs-lookup"><span data-stu-id="b6261-185">Require the Android Verify apps feature is turned on.</span></span>|
|<span data-ttu-id="b6261-186">deviceThreatProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="b6261-186">deviceThreatProtectionEnabled</span></span>|<span data-ttu-id="b6261-187">Boolean</span><span class="sxs-lookup"><span data-stu-id="b6261-187">Boolean</span></span>|<span data-ttu-id="b6261-188">要求设备已启用设备威胁防护。</span><span class="sxs-lookup"><span data-stu-id="b6261-188">Require that devices have enabled device threat protection.</span></span>|
|<span data-ttu-id="b6261-189">deviceThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="b6261-189">deviceThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="b6261-190">deviceThreatProtectionLevel</span><span class="sxs-lookup"><span data-stu-id="b6261-190">deviceThreatProtectionLevel</span></span>](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|<span data-ttu-id="b6261-191">要求移动威胁防护最低风险级别来报告不符合情况。</span><span class="sxs-lookup"><span data-stu-id="b6261-191">Require Mobile Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="b6261-192">可取值为：`unavailable`、`secured`、`low`、`medium`、`high`、`notSet`。</span><span class="sxs-lookup"><span data-stu-id="b6261-192">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="b6261-193">securityBlockJailbrokenDevices</span><span class="sxs-lookup"><span data-stu-id="b6261-193">securityBlockJailbrokenDevices</span></span>|<span data-ttu-id="b6261-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="b6261-194">Boolean</span></span>|<span data-ttu-id="b6261-195">设备不得越狱或取得 root 权限。</span><span class="sxs-lookup"><span data-stu-id="b6261-195">Devices must not be jailbroken or rooted.</span></span>|
|<span data-ttu-id="b6261-196">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="b6261-196">osMinimumVersion</span></span>|<span data-ttu-id="b6261-197">String</span><span class="sxs-lookup"><span data-stu-id="b6261-197">String</span></span>|<span data-ttu-id="b6261-198">最低 Android 版本。</span><span class="sxs-lookup"><span data-stu-id="b6261-198">Minimum Android version.</span></span>|
|<span data-ttu-id="b6261-199">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="b6261-199">osMaximumVersion</span></span>|<span data-ttu-id="b6261-200">String</span><span class="sxs-lookup"><span data-stu-id="b6261-200">String</span></span>|<span data-ttu-id="b6261-201">最高 Android 版本。</span><span class="sxs-lookup"><span data-stu-id="b6261-201">Maximum Android version.</span></span>|
|<span data-ttu-id="b6261-202">minAndroidSecurityPatchLevel</span><span class="sxs-lookup"><span data-stu-id="b6261-202">minAndroidSecurityPatchLevel</span></span>|<span data-ttu-id="b6261-203">String</span><span class="sxs-lookup"><span data-stu-id="b6261-203">String</span></span>|<span data-ttu-id="b6261-204">最低 Android 安全修补程序级别。</span><span class="sxs-lookup"><span data-stu-id="b6261-204">Minimum Android security patch level.</span></span>|
|<span data-ttu-id="b6261-205">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="b6261-205">storageRequireEncryption</span></span>|<span data-ttu-id="b6261-206">Boolean</span><span class="sxs-lookup"><span data-stu-id="b6261-206">Boolean</span></span>|<span data-ttu-id="b6261-207">要求对 Android 设备加密。</span><span class="sxs-lookup"><span data-stu-id="b6261-207">Require encryption on Android devices.</span></span>|
|<span data-ttu-id="b6261-208">securityRequireSafetyNetAttestationBasicIntegrity</span><span class="sxs-lookup"><span data-stu-id="b6261-208">securityRequireSafetyNetAttestationBasicIntegrity</span></span>|<span data-ttu-id="b6261-209">Boolean</span><span class="sxs-lookup"><span data-stu-id="b6261-209">Boolean</span></span>|<span data-ttu-id="b6261-210">要求设备传递 SafetyNet 基本完整性检查。</span><span class="sxs-lookup"><span data-stu-id="b6261-210">Require the device to pass the SafetyNet basic integrity check.</span></span>|
|<span data-ttu-id="b6261-211">securityRequireSafetyNetAttestationCertifiedDevice</span><span class="sxs-lookup"><span data-stu-id="b6261-211">securityRequireSafetyNetAttestationCertifiedDevice</span></span>|<span data-ttu-id="b6261-212">Boolean</span><span class="sxs-lookup"><span data-stu-id="b6261-212">Boolean</span></span>|<span data-ttu-id="b6261-213">要求设备传递 SafetyNet 认证设备检查。</span><span class="sxs-lookup"><span data-stu-id="b6261-213">Require the device to pass the SafetyNet certified device check.</span></span>|
|<span data-ttu-id="b6261-214">securityRequireGooglePlayServices</span><span class="sxs-lookup"><span data-stu-id="b6261-214">securityRequireGooglePlayServices</span></span>|<span data-ttu-id="b6261-215">Boolean</span><span class="sxs-lookup"><span data-stu-id="b6261-215">Boolean</span></span>|<span data-ttu-id="b6261-216">要求在设备上安装并启用 Google Play Services。</span><span class="sxs-lookup"><span data-stu-id="b6261-216">Require Google Play Services to be installed and enabled on the device.</span></span>|
|<span data-ttu-id="b6261-217">securityRequireUpToDateSecurityProviders</span><span class="sxs-lookup"><span data-stu-id="b6261-217">securityRequireUpToDateSecurityProviders</span></span>|<span data-ttu-id="b6261-218">Boolean</span><span class="sxs-lookup"><span data-stu-id="b6261-218">Boolean</span></span>|<span data-ttu-id="b6261-219">要求设备具有最新的安全提供程序。</span><span class="sxs-lookup"><span data-stu-id="b6261-219">Require the device to have up to date security providers.</span></span> <span data-ttu-id="b6261-220">设备将要求启用 Google Play Services 并保持最新状态。</span><span class="sxs-lookup"><span data-stu-id="b6261-220">The device will require Google Play Services to be enabled and up to date.</span></span>|
|<span data-ttu-id="b6261-221">securityRequireCompanyPortalAppIntegrity</span><span class="sxs-lookup"><span data-stu-id="b6261-221">securityRequireCompanyPortalAppIntegrity</span></span>|<span data-ttu-id="b6261-222">Boolean</span><span class="sxs-lookup"><span data-stu-id="b6261-222">Boolean</span></span>|<span data-ttu-id="b6261-223">要求设备传递公司门户客户端应用运行时完整性检查。</span><span class="sxs-lookup"><span data-stu-id="b6261-223">Require the device to pass the Company Portal client app runtime integrity check.</span></span>|



## <a name="response"></a><span data-ttu-id="b6261-224">响应</span><span class="sxs-lookup"><span data-stu-id="b6261-224">Response</span></span>
<span data-ttu-id="b6261-225">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和更新的 [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="b6261-225">If successful, this method returns a `200 OK` response code and an updated [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b6261-226">示例</span><span class="sxs-lookup"><span data-stu-id="b6261-226">Example</span></span>

### <a name="request"></a><span data-ttu-id="b6261-227">请求</span><span class="sxs-lookup"><span data-stu-id="b6261-227">Request</span></span>
<span data-ttu-id="b6261-228">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="b6261-228">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
Content-type: application/json
Content-length: 1159

{
  "@odata.type": "#microsoft.graph.androidCompliancePolicy",
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

### <a name="response"></a><span data-ttu-id="b6261-229">响应</span><span class="sxs-lookup"><span data-stu-id="b6261-229">Response</span></span>
<span data-ttu-id="b6261-p114">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="b6261-p114">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1331

{
  "@odata.type": "#microsoft.graph.androidCompliancePolicy",
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




