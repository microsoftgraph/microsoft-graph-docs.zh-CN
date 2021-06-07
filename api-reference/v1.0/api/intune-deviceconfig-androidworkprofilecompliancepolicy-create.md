---
title: 创建 androidWorkProfileCompliancePolicy
description: 创建新的 androidWorkProfileCompliancePolicy 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 38a370dac056a49cc264c28cfe8b22cea3bea60f
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52757211"
---
# <a name="create-androidworkprofilecompliancepolicy"></a><span data-ttu-id="90cb2-103">创建 androidWorkProfileCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="90cb2-103">Create androidWorkProfileCompliancePolicy</span></span>

<span data-ttu-id="90cb2-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="90cb2-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="90cb2-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="90cb2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="90cb2-106">创建新的 [androidWorkProfileCompliancePolicy](../resources/intune-deviceconfig-androidworkprofilecompliancepolicy.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="90cb2-106">Create a new [androidWorkProfileCompliancePolicy](../resources/intune-deviceconfig-androidworkprofilecompliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="90cb2-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="90cb2-107">Prerequisites</span></span>
<span data-ttu-id="90cb2-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="90cb2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="90cb2-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="90cb2-110">Permission type</span></span>|<span data-ttu-id="90cb2-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="90cb2-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="90cb2-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="90cb2-112">Delegated (work or school account)</span></span>|<span data-ttu-id="90cb2-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="90cb2-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="90cb2-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="90cb2-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="90cb2-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="90cb2-115">Not supported.</span></span>|
|<span data-ttu-id="90cb2-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="90cb2-116">Application</span></span>|<span data-ttu-id="90cb2-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="90cb2-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="90cb2-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="90cb2-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="90cb2-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="90cb2-119">Request headers</span></span>
|<span data-ttu-id="90cb2-120">标头</span><span class="sxs-lookup"><span data-stu-id="90cb2-120">Header</span></span>|<span data-ttu-id="90cb2-121">值</span><span class="sxs-lookup"><span data-stu-id="90cb2-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="90cb2-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="90cb2-122">Authorization</span></span>|<span data-ttu-id="90cb2-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="90cb2-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="90cb2-124">接受</span><span class="sxs-lookup"><span data-stu-id="90cb2-124">Accept</span></span>|<span data-ttu-id="90cb2-125">application/json</span><span class="sxs-lookup"><span data-stu-id="90cb2-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="90cb2-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="90cb2-126">Request body</span></span>
<span data-ttu-id="90cb2-127">在请求正文中，提供 androidWorkProfileCompliancePolicy 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="90cb2-127">In the request body, supply a JSON representation for the androidWorkProfileCompliancePolicy object.</span></span>

<span data-ttu-id="90cb2-128">下表显示创建 androidWorkProfileCompliancePolicy 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="90cb2-128">The following table shows the properties that are required when you create the androidWorkProfileCompliancePolicy.</span></span>

|<span data-ttu-id="90cb2-129">属性</span><span class="sxs-lookup"><span data-stu-id="90cb2-129">Property</span></span>|<span data-ttu-id="90cb2-130">类型</span><span class="sxs-lookup"><span data-stu-id="90cb2-130">Type</span></span>|<span data-ttu-id="90cb2-131">说明</span><span class="sxs-lookup"><span data-stu-id="90cb2-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="90cb2-132">id</span><span class="sxs-lookup"><span data-stu-id="90cb2-132">id</span></span>|<span data-ttu-id="90cb2-133">String</span><span class="sxs-lookup"><span data-stu-id="90cb2-133">String</span></span>|<span data-ttu-id="90cb2-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="90cb2-134">Key of the entity.</span></span> <span data-ttu-id="90cb2-135">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="90cb2-135">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="90cb2-136">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="90cb2-136">createdDateTime</span></span>|<span data-ttu-id="90cb2-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="90cb2-137">DateTimeOffset</span></span>|<span data-ttu-id="90cb2-138">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="90cb2-138">DateTime the object was created.</span></span> <span data-ttu-id="90cb2-139">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="90cb2-139">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="90cb2-140">说明</span><span class="sxs-lookup"><span data-stu-id="90cb2-140">description</span></span>|<span data-ttu-id="90cb2-141">String</span><span class="sxs-lookup"><span data-stu-id="90cb2-141">String</span></span>|<span data-ttu-id="90cb2-142">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="90cb2-142">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="90cb2-143">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="90cb2-143">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="90cb2-144">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="90cb2-144">lastModifiedDateTime</span></span>|<span data-ttu-id="90cb2-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="90cb2-145">DateTimeOffset</span></span>|<span data-ttu-id="90cb2-146">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="90cb2-146">DateTime the object was last modified.</span></span> <span data-ttu-id="90cb2-147">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="90cb2-147">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="90cb2-148">displayName</span><span class="sxs-lookup"><span data-stu-id="90cb2-148">displayName</span></span>|<span data-ttu-id="90cb2-149">String</span><span class="sxs-lookup"><span data-stu-id="90cb2-149">String</span></span>|<span data-ttu-id="90cb2-150">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="90cb2-150">Admin provided name of the device configuration.</span></span> <span data-ttu-id="90cb2-151">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="90cb2-151">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="90cb2-152">version</span><span class="sxs-lookup"><span data-stu-id="90cb2-152">version</span></span>|<span data-ttu-id="90cb2-153">Int32</span><span class="sxs-lookup"><span data-stu-id="90cb2-153">Int32</span></span>|<span data-ttu-id="90cb2-154">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="90cb2-154">Version of the device configuration.</span></span> <span data-ttu-id="90cb2-155">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="90cb2-155">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="90cb2-156">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="90cb2-156">passwordRequired</span></span>|<span data-ttu-id="90cb2-157">Boolean</span><span class="sxs-lookup"><span data-stu-id="90cb2-157">Boolean</span></span>|<span data-ttu-id="90cb2-158">需要密码才可解锁设备。</span><span class="sxs-lookup"><span data-stu-id="90cb2-158">Require a password to unlock device.</span></span>|
|<span data-ttu-id="90cb2-159">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="90cb2-159">passwordMinimumLength</span></span>|<span data-ttu-id="90cb2-160">Int32</span><span class="sxs-lookup"><span data-stu-id="90cb2-160">Int32</span></span>|<span data-ttu-id="90cb2-161">最短密码长度。</span><span class="sxs-lookup"><span data-stu-id="90cb2-161">Minimum password length.</span></span> <span data-ttu-id="90cb2-162">有效值为 4 至 16</span><span class="sxs-lookup"><span data-stu-id="90cb2-162">Valid values 4 to 16</span></span>|
|<span data-ttu-id="90cb2-163">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="90cb2-163">passwordRequiredType</span></span>|[<span data-ttu-id="90cb2-164">androidRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="90cb2-164">androidRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androidrequiredpasswordtype.md)|<span data-ttu-id="90cb2-165">密码中的字符类型。</span><span class="sxs-lookup"><span data-stu-id="90cb2-165">Type of characters in password.</span></span> <span data-ttu-id="90cb2-166">可取值为：`deviceDefault`、`alphabetic`、`alphanumeric`、`alphanumericWithSymbols`、`lowSecurityBiometric`、`numeric`、`numericComplex`、`any`。</span><span class="sxs-lookup"><span data-stu-id="90cb2-166">Possible values are: `deviceDefault`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `numeric`, `numericComplex`, `any`.</span></span>|
|<span data-ttu-id="90cb2-167">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="90cb2-167">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="90cb2-168">Int32</span><span class="sxs-lookup"><span data-stu-id="90cb2-168">Int32</span></span>|<span data-ttu-id="90cb2-169">在需要密码之前不活动的分钟数。</span><span class="sxs-lookup"><span data-stu-id="90cb2-169">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="90cb2-170">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="90cb2-170">passwordExpirationDays</span></span>|<span data-ttu-id="90cb2-171">Int32</span><span class="sxs-lookup"><span data-stu-id="90cb2-171">Int32</span></span>|<span data-ttu-id="90cb2-172">密码过期前的天数。</span><span class="sxs-lookup"><span data-stu-id="90cb2-172">Number of days before the password expires.</span></span> <span data-ttu-id="90cb2-173">有效值为 1 至 365</span><span class="sxs-lookup"><span data-stu-id="90cb2-173">Valid values 1 to 365</span></span>|
|<span data-ttu-id="90cb2-174">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="90cb2-174">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="90cb2-175">Int32</span><span class="sxs-lookup"><span data-stu-id="90cb2-175">Int32</span></span>|<span data-ttu-id="90cb2-176">要阻止的以前密码的数量。</span><span class="sxs-lookup"><span data-stu-id="90cb2-176">Number of previous passwords to block.</span></span> <span data-ttu-id="90cb2-177">有效值为 1 至 24</span><span class="sxs-lookup"><span data-stu-id="90cb2-177">Valid values 1 to 24</span></span>|
|<span data-ttu-id="90cb2-178">securityPreventInstallAppsFromUnknownSources</span><span class="sxs-lookup"><span data-stu-id="90cb2-178">securityPreventInstallAppsFromUnknownSources</span></span>|<span data-ttu-id="90cb2-179">Boolean</span><span class="sxs-lookup"><span data-stu-id="90cb2-179">Boolean</span></span>|<span data-ttu-id="90cb2-180">要求设备不允许安装来自未知源的应用。</span><span class="sxs-lookup"><span data-stu-id="90cb2-180">Require that devices disallow installation of apps from unknown sources.</span></span>|
|<span data-ttu-id="90cb2-181">securityDisableUsbDebugging</span><span class="sxs-lookup"><span data-stu-id="90cb2-181">securityDisableUsbDebugging</span></span>|<span data-ttu-id="90cb2-182">Boolean</span><span class="sxs-lookup"><span data-stu-id="90cb2-182">Boolean</span></span>|<span data-ttu-id="90cb2-183">在 Android 设备上禁用 USB 调试。</span><span class="sxs-lookup"><span data-stu-id="90cb2-183">Disable USB debugging on Android devices.</span></span>|
|<span data-ttu-id="90cb2-184">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="90cb2-184">securityRequireVerifyApps</span></span>|<span data-ttu-id="90cb2-185">Boolean</span><span class="sxs-lookup"><span data-stu-id="90cb2-185">Boolean</span></span>|<span data-ttu-id="90cb2-186">要求启用 Android 验证应用功能。</span><span class="sxs-lookup"><span data-stu-id="90cb2-186">Require the Android Verify apps feature is turned on.</span></span>|
|<span data-ttu-id="90cb2-187">deviceThreatProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="90cb2-187">deviceThreatProtectionEnabled</span></span>|<span data-ttu-id="90cb2-188">Boolean</span><span class="sxs-lookup"><span data-stu-id="90cb2-188">Boolean</span></span>|<span data-ttu-id="90cb2-189">要求设备已启用设备威胁防护。</span><span class="sxs-lookup"><span data-stu-id="90cb2-189">Require that devices have enabled device threat protection.</span></span>|
|<span data-ttu-id="90cb2-190">deviceThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="90cb2-190">deviceThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="90cb2-191">deviceThreatProtectionLevel</span><span class="sxs-lookup"><span data-stu-id="90cb2-191">deviceThreatProtectionLevel</span></span>](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|<span data-ttu-id="90cb2-192">要求移动威胁防护最低风险级别来报告不符合情况。</span><span class="sxs-lookup"><span data-stu-id="90cb2-192">Require Mobile Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="90cb2-193">可取值为：`unavailable`、`secured`、`low`、`medium`、`high`、`notSet`。</span><span class="sxs-lookup"><span data-stu-id="90cb2-193">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="90cb2-194">securityBlockJailbrokenDevices</span><span class="sxs-lookup"><span data-stu-id="90cb2-194">securityBlockJailbrokenDevices</span></span>|<span data-ttu-id="90cb2-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="90cb2-195">Boolean</span></span>|<span data-ttu-id="90cb2-196">设备不得越狱或取得 root 权限。</span><span class="sxs-lookup"><span data-stu-id="90cb2-196">Devices must not be jailbroken or rooted.</span></span>|
|<span data-ttu-id="90cb2-197">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="90cb2-197">osMinimumVersion</span></span>|<span data-ttu-id="90cb2-198">String</span><span class="sxs-lookup"><span data-stu-id="90cb2-198">String</span></span>|<span data-ttu-id="90cb2-199">最低 Android 版本。</span><span class="sxs-lookup"><span data-stu-id="90cb2-199">Minimum Android version.</span></span>|
|<span data-ttu-id="90cb2-200">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="90cb2-200">osMaximumVersion</span></span>|<span data-ttu-id="90cb2-201">String</span><span class="sxs-lookup"><span data-stu-id="90cb2-201">String</span></span>|<span data-ttu-id="90cb2-202">最高 Android 版本。</span><span class="sxs-lookup"><span data-stu-id="90cb2-202">Maximum Android version.</span></span>|
|<span data-ttu-id="90cb2-203">minAndroidSecurityPatchLevel</span><span class="sxs-lookup"><span data-stu-id="90cb2-203">minAndroidSecurityPatchLevel</span></span>|<span data-ttu-id="90cb2-204">String</span><span class="sxs-lookup"><span data-stu-id="90cb2-204">String</span></span>|<span data-ttu-id="90cb2-205">最低 Android 安全修补程序级别。</span><span class="sxs-lookup"><span data-stu-id="90cb2-205">Minimum Android security patch level.</span></span>|
|<span data-ttu-id="90cb2-206">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="90cb2-206">storageRequireEncryption</span></span>|<span data-ttu-id="90cb2-207">Boolean</span><span class="sxs-lookup"><span data-stu-id="90cb2-207">Boolean</span></span>|<span data-ttu-id="90cb2-208">要求对 Android 设备加密。</span><span class="sxs-lookup"><span data-stu-id="90cb2-208">Require encryption on Android devices.</span></span>|
|<span data-ttu-id="90cb2-209">securityRequireSafetyNetAttestationBasicIntegrity</span><span class="sxs-lookup"><span data-stu-id="90cb2-209">securityRequireSafetyNetAttestationBasicIntegrity</span></span>|<span data-ttu-id="90cb2-210">Boolean</span><span class="sxs-lookup"><span data-stu-id="90cb2-210">Boolean</span></span>|<span data-ttu-id="90cb2-211">要求设备传递 SafetyNet 基本完整性检查。</span><span class="sxs-lookup"><span data-stu-id="90cb2-211">Require the device to pass the SafetyNet basic integrity check.</span></span>|
|<span data-ttu-id="90cb2-212">securityRequireSafetyNetAttestationCertifiedDevice</span><span class="sxs-lookup"><span data-stu-id="90cb2-212">securityRequireSafetyNetAttestationCertifiedDevice</span></span>|<span data-ttu-id="90cb2-213">Boolean</span><span class="sxs-lookup"><span data-stu-id="90cb2-213">Boolean</span></span>|<span data-ttu-id="90cb2-214">要求设备传递 SafetyNet 认证设备检查。</span><span class="sxs-lookup"><span data-stu-id="90cb2-214">Require the device to pass the SafetyNet certified device check.</span></span>|
|<span data-ttu-id="90cb2-215">securityRequireGooglePlayServices</span><span class="sxs-lookup"><span data-stu-id="90cb2-215">securityRequireGooglePlayServices</span></span>|<span data-ttu-id="90cb2-216">Boolean</span><span class="sxs-lookup"><span data-stu-id="90cb2-216">Boolean</span></span>|<span data-ttu-id="90cb2-217">要求在设备上安装并启用 Google Play Services。</span><span class="sxs-lookup"><span data-stu-id="90cb2-217">Require Google Play Services to be installed and enabled on the device.</span></span>|
|<span data-ttu-id="90cb2-218">securityRequireUpToDateSecurityProviders</span><span class="sxs-lookup"><span data-stu-id="90cb2-218">securityRequireUpToDateSecurityProviders</span></span>|<span data-ttu-id="90cb2-219">Boolean</span><span class="sxs-lookup"><span data-stu-id="90cb2-219">Boolean</span></span>|<span data-ttu-id="90cb2-220">要求设备具有最新的安全提供程序。</span><span class="sxs-lookup"><span data-stu-id="90cb2-220">Require the device to have up to date security providers.</span></span> <span data-ttu-id="90cb2-221">设备将要求启用 Google Play Services 并保持最新状态。</span><span class="sxs-lookup"><span data-stu-id="90cb2-221">The device will require Google Play Services to be enabled and up to date.</span></span>|
|<span data-ttu-id="90cb2-222">securityRequireCompanyPortalAppIntegrity</span><span class="sxs-lookup"><span data-stu-id="90cb2-222">securityRequireCompanyPortalAppIntegrity</span></span>|<span data-ttu-id="90cb2-223">Boolean</span><span class="sxs-lookup"><span data-stu-id="90cb2-223">Boolean</span></span>|<span data-ttu-id="90cb2-224">要求设备传递公司门户客户端应用运行时完整性检查。</span><span class="sxs-lookup"><span data-stu-id="90cb2-224">Require the device to pass the Company Portal client app runtime integrity check.</span></span>|



## <a name="response"></a><span data-ttu-id="90cb2-225">响应</span><span class="sxs-lookup"><span data-stu-id="90cb2-225">Response</span></span>
<span data-ttu-id="90cb2-226">如果成功，此方法在响应 `201 Created` 正文中返回 响应代码和 [androidWorkProfileCompliancePolicy](../resources/intune-deviceconfig-androidworkprofilecompliancepolicy.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="90cb2-226">If successful, this method returns a `201 Created` response code and a [androidWorkProfileCompliancePolicy](../resources/intune-deviceconfig-androidworkprofilecompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="90cb2-227">示例</span><span class="sxs-lookup"><span data-stu-id="90cb2-227">Example</span></span>

### <a name="request"></a><span data-ttu-id="90cb2-228">请求</span><span class="sxs-lookup"><span data-stu-id="90cb2-228">Request</span></span>
<span data-ttu-id="90cb2-229">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="90cb2-229">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="90cb2-230">响应</span><span class="sxs-lookup"><span data-stu-id="90cb2-230">Response</span></span>
<span data-ttu-id="90cb2-p114">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="90cb2-p114">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




