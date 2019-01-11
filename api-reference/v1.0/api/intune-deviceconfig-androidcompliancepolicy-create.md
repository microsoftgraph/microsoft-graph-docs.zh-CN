---
title: 创建 androidCompliancePolicy
description: 创建新的 androidCompliancePolicy 对象。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 49449d01e15769ba3722f17f90085e6b36484aac
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27879238"
---
# <a name="create-androidcompliancepolicy"></a><span data-ttu-id="b3834-103">创建 androidCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="b3834-103">Create androidCompliancePolicy</span></span>

> <span data-ttu-id="b3834-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="b3834-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b3834-105">创建新的 [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="b3834-105">Create a new [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="b3834-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="b3834-106">Prerequisites</span></span>
<span data-ttu-id="b3834-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="b3834-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b3834-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="b3834-109">Permission type</span></span>|<span data-ttu-id="b3834-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="b3834-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b3834-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b3834-111">Delegated (work or school account)</span></span>|<span data-ttu-id="b3834-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b3834-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b3834-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b3834-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b3834-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="b3834-114">Not supported.</span></span>|
|<span data-ttu-id="b3834-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="b3834-115">Application</span></span>|<span data-ttu-id="b3834-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="b3834-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b3834-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b3834-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="b3834-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="b3834-118">Request headers</span></span>
|<span data-ttu-id="b3834-119">标头</span><span class="sxs-lookup"><span data-stu-id="b3834-119">Header</span></span>|<span data-ttu-id="b3834-120">值</span><span class="sxs-lookup"><span data-stu-id="b3834-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b3834-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="b3834-121">Authorization</span></span>|<span data-ttu-id="b3834-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="b3834-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b3834-123">Accept</span><span class="sxs-lookup"><span data-stu-id="b3834-123">Accept</span></span>|<span data-ttu-id="b3834-124">application/json</span><span class="sxs-lookup"><span data-stu-id="b3834-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b3834-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="b3834-125">Request body</span></span>
<span data-ttu-id="b3834-126">在请求正文中，提供 androidCompliancePolicy 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b3834-126">In the request body, supply a JSON representation for the androidCompliancePolicy object.</span></span>

<span data-ttu-id="b3834-127">下表显示了创建 androidCompliancePolicy 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="b3834-127">The following table shows the properties that are required when you create the androidCompliancePolicy.</span></span>

|<span data-ttu-id="b3834-128">属性</span><span class="sxs-lookup"><span data-stu-id="b3834-128">Property</span></span>|<span data-ttu-id="b3834-129">类型</span><span class="sxs-lookup"><span data-stu-id="b3834-129">Type</span></span>|<span data-ttu-id="b3834-130">说明</span><span class="sxs-lookup"><span data-stu-id="b3834-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b3834-131">id</span><span class="sxs-lookup"><span data-stu-id="b3834-131">id</span></span>|<span data-ttu-id="b3834-132">String</span><span class="sxs-lookup"><span data-stu-id="b3834-132">String</span></span>|<span data-ttu-id="b3834-133">实体的键。</span><span class="sxs-lookup"><span data-stu-id="b3834-133">Key of the entity.</span></span> <span data-ttu-id="b3834-134">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="b3834-134">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="b3834-135">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b3834-135">createdDateTime</span></span>|<span data-ttu-id="b3834-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b3834-136">DateTimeOffset</span></span>|<span data-ttu-id="b3834-137">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="b3834-137">DateTime the object was created.</span></span> <span data-ttu-id="b3834-138">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="b3834-138">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="b3834-139">description</span><span class="sxs-lookup"><span data-stu-id="b3834-139">description</span></span>|<span data-ttu-id="b3834-140">String</span><span class="sxs-lookup"><span data-stu-id="b3834-140">String</span></span>|<span data-ttu-id="b3834-141">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="b3834-141">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="b3834-142">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="b3834-142">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="b3834-143">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b3834-143">lastModifiedDateTime</span></span>|<span data-ttu-id="b3834-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b3834-144">DateTimeOffset</span></span>|<span data-ttu-id="b3834-145">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="b3834-145">DateTime the object was last modified.</span></span> <span data-ttu-id="b3834-146">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="b3834-146">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="b3834-147">displayName</span><span class="sxs-lookup"><span data-stu-id="b3834-147">displayName</span></span>|<span data-ttu-id="b3834-148">String</span><span class="sxs-lookup"><span data-stu-id="b3834-148">String</span></span>|<span data-ttu-id="b3834-149">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="b3834-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="b3834-150">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="b3834-150">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="b3834-151">version</span><span class="sxs-lookup"><span data-stu-id="b3834-151">version</span></span>|<span data-ttu-id="b3834-152">Int32</span><span class="sxs-lookup"><span data-stu-id="b3834-152">Int32</span></span>|<span data-ttu-id="b3834-153">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="b3834-153">Version of the device configuration.</span></span> <span data-ttu-id="b3834-154">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="b3834-154">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="b3834-155">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="b3834-155">passwordRequired</span></span>|<span data-ttu-id="b3834-156">Boolean</span><span class="sxs-lookup"><span data-stu-id="b3834-156">Boolean</span></span>|<span data-ttu-id="b3834-157">需要密码才可解锁设备。</span><span class="sxs-lookup"><span data-stu-id="b3834-157">Require a password to unlock device.</span></span>|
|<span data-ttu-id="b3834-158">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="b3834-158">passwordMinimumLength</span></span>|<span data-ttu-id="b3834-159">Int32</span><span class="sxs-lookup"><span data-stu-id="b3834-159">Int32</span></span>|<span data-ttu-id="b3834-160">最短密码长度。</span><span class="sxs-lookup"><span data-stu-id="b3834-160">Minimum password length.</span></span> <span data-ttu-id="b3834-161">有效值为 4 至 16</span><span class="sxs-lookup"><span data-stu-id="b3834-161">Valid values 4 to 16</span></span>|
|<span data-ttu-id="b3834-162">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="b3834-162">passwordRequiredType</span></span>|[<span data-ttu-id="b3834-163">androidRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="b3834-163">androidRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androidrequiredpasswordtype.md)|<span data-ttu-id="b3834-164">密码中的字符类型。</span><span class="sxs-lookup"><span data-stu-id="b3834-164">Type of characters in password.</span></span> <span data-ttu-id="b3834-165">可取值为：`deviceDefault`、`alphabetic`、`alphanumeric`、`alphanumericWithSymbols`、`lowSecurityBiometric`、`numeric`、`numericComplex`、`any`。</span><span class="sxs-lookup"><span data-stu-id="b3834-165">Possible values are: `deviceDefault`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `numeric`, `numericComplex`, `any`.</span></span>|
|<span data-ttu-id="b3834-166">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="b3834-166">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="b3834-167">Int32</span><span class="sxs-lookup"><span data-stu-id="b3834-167">Int32</span></span>|<span data-ttu-id="b3834-168">在需要密码之前不活动的分钟数。</span><span class="sxs-lookup"><span data-stu-id="b3834-168">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="b3834-169">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="b3834-169">passwordExpirationDays</span></span>|<span data-ttu-id="b3834-170">Int32</span><span class="sxs-lookup"><span data-stu-id="b3834-170">Int32</span></span>|<span data-ttu-id="b3834-171">密码过期前的天数。</span><span class="sxs-lookup"><span data-stu-id="b3834-171">Number of days before the password expires.</span></span> <span data-ttu-id="b3834-172">有效值为 1 至 65535</span><span class="sxs-lookup"><span data-stu-id="b3834-172">Valid values 1 to 65535</span></span>|
|<span data-ttu-id="b3834-173">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="b3834-173">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="b3834-174">Int32</span><span class="sxs-lookup"><span data-stu-id="b3834-174">Int32</span></span>|<span data-ttu-id="b3834-175">要阻止的以前密码的数量。</span><span class="sxs-lookup"><span data-stu-id="b3834-175">Number of previous passwords to block.</span></span>|
|<span data-ttu-id="b3834-176">securityPreventInstallAppsFromUnknownSources</span><span class="sxs-lookup"><span data-stu-id="b3834-176">securityPreventInstallAppsFromUnknownSources</span></span>|<span data-ttu-id="b3834-177">Boolean</span><span class="sxs-lookup"><span data-stu-id="b3834-177">Boolean</span></span>|<span data-ttu-id="b3834-178">要求设备不允许安装来自未知源的应用。</span><span class="sxs-lookup"><span data-stu-id="b3834-178">Require that devices disallow installation of apps from unknown sources.</span></span>|
|<span data-ttu-id="b3834-179">securityDisableUsbDebugging</span><span class="sxs-lookup"><span data-stu-id="b3834-179">securityDisableUsbDebugging</span></span>|<span data-ttu-id="b3834-180">Boolean</span><span class="sxs-lookup"><span data-stu-id="b3834-180">Boolean</span></span>|<span data-ttu-id="b3834-181">在 Android 设备上禁用 USB 调试。</span><span class="sxs-lookup"><span data-stu-id="b3834-181">Disable USB debugging on Android devices.</span></span>|
|<span data-ttu-id="b3834-182">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="b3834-182">securityRequireVerifyApps</span></span>|<span data-ttu-id="b3834-183">Boolean</span><span class="sxs-lookup"><span data-stu-id="b3834-183">Boolean</span></span>|<span data-ttu-id="b3834-184">要求启用 Android 验证应用功能。</span><span class="sxs-lookup"><span data-stu-id="b3834-184">Require the Android Verify apps feature is turned on.</span></span>|
|<span data-ttu-id="b3834-185">deviceThreatProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="b3834-185">deviceThreatProtectionEnabled</span></span>|<span data-ttu-id="b3834-186">Boolean</span><span class="sxs-lookup"><span data-stu-id="b3834-186">Boolean</span></span>|<span data-ttu-id="b3834-187">要求设备已启用设备威胁防护。</span><span class="sxs-lookup"><span data-stu-id="b3834-187">Require that devices have enabled device threat protection.</span></span>|
|<span data-ttu-id="b3834-188">deviceThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="b3834-188">deviceThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="b3834-189">deviceThreatProtectionLevel</span><span class="sxs-lookup"><span data-stu-id="b3834-189">deviceThreatProtectionLevel</span></span>](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|<span data-ttu-id="b3834-190">要求移动威胁防护最低风险级别来报告不符合情况。</span><span class="sxs-lookup"><span data-stu-id="b3834-190">Require Mobile Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="b3834-191">可取值为：`unavailable`、`secured`、`low`、`medium`、`high`、`notSet`。</span><span class="sxs-lookup"><span data-stu-id="b3834-191">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="b3834-192">securityBlockJailbrokenDevices</span><span class="sxs-lookup"><span data-stu-id="b3834-192">securityBlockJailbrokenDevices</span></span>|<span data-ttu-id="b3834-193">Boolean</span><span class="sxs-lookup"><span data-stu-id="b3834-193">Boolean</span></span>|<span data-ttu-id="b3834-194">设备不得越狱或取得 root 权限。</span><span class="sxs-lookup"><span data-stu-id="b3834-194">Devices must not be jailbroken or rooted.</span></span>|
|<span data-ttu-id="b3834-195">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="b3834-195">osMinimumVersion</span></span>|<span data-ttu-id="b3834-196">String</span><span class="sxs-lookup"><span data-stu-id="b3834-196">String</span></span>|<span data-ttu-id="b3834-197">最低 Android 版本。</span><span class="sxs-lookup"><span data-stu-id="b3834-197">Minimum Android version.</span></span>|
|<span data-ttu-id="b3834-198">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="b3834-198">osMaximumVersion</span></span>|<span data-ttu-id="b3834-199">String</span><span class="sxs-lookup"><span data-stu-id="b3834-199">String</span></span>|<span data-ttu-id="b3834-200">最高 Android 版本。</span><span class="sxs-lookup"><span data-stu-id="b3834-200">Maximum Android version.</span></span>|
|<span data-ttu-id="b3834-201">minAndroidSecurityPatchLevel</span><span class="sxs-lookup"><span data-stu-id="b3834-201">minAndroidSecurityPatchLevel</span></span>|<span data-ttu-id="b3834-202">String</span><span class="sxs-lookup"><span data-stu-id="b3834-202">String</span></span>|<span data-ttu-id="b3834-203">最低 Android 安全修补程序级别。</span><span class="sxs-lookup"><span data-stu-id="b3834-203">Minimum Android security patch level.</span></span>|
|<span data-ttu-id="b3834-204">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="b3834-204">storageRequireEncryption</span></span>|<span data-ttu-id="b3834-205">Boolean</span><span class="sxs-lookup"><span data-stu-id="b3834-205">Boolean</span></span>|<span data-ttu-id="b3834-206">要求对 Android 设备加密。</span><span class="sxs-lookup"><span data-stu-id="b3834-206">Require encryption on Android devices.</span></span>|
|<span data-ttu-id="b3834-207">securityRequireSafetyNetAttestationBasicIntegrity</span><span class="sxs-lookup"><span data-stu-id="b3834-207">securityRequireSafetyNetAttestationBasicIntegrity</span></span>|<span data-ttu-id="b3834-208">Boolean</span><span class="sxs-lookup"><span data-stu-id="b3834-208">Boolean</span></span>|<span data-ttu-id="b3834-209">要求设备传递 SafetyNet 基本完整性检查。</span><span class="sxs-lookup"><span data-stu-id="b3834-209">Require the device to pass the SafetyNet basic integrity check.</span></span>|
|<span data-ttu-id="b3834-210">securityRequireSafetyNetAttestationCertifiedDevice</span><span class="sxs-lookup"><span data-stu-id="b3834-210">securityRequireSafetyNetAttestationCertifiedDevice</span></span>|<span data-ttu-id="b3834-211">Boolean</span><span class="sxs-lookup"><span data-stu-id="b3834-211">Boolean</span></span>|<span data-ttu-id="b3834-212">要求设备传递 SafetyNet 认证设备检查。</span><span class="sxs-lookup"><span data-stu-id="b3834-212">Require the device to pass the SafetyNet certified device check.</span></span>|
|<span data-ttu-id="b3834-213">securityRequireGooglePlayServices</span><span class="sxs-lookup"><span data-stu-id="b3834-213">securityRequireGooglePlayServices</span></span>|<span data-ttu-id="b3834-214">Boolean</span><span class="sxs-lookup"><span data-stu-id="b3834-214">Boolean</span></span>|<span data-ttu-id="b3834-215">要求在设备上安装并启用 Google Play Services。</span><span class="sxs-lookup"><span data-stu-id="b3834-215">Require Google Play Services to be installed and enabled on the device.</span></span>|
|<span data-ttu-id="b3834-216">securityRequireUpToDateSecurityProviders</span><span class="sxs-lookup"><span data-stu-id="b3834-216">securityRequireUpToDateSecurityProviders</span></span>|<span data-ttu-id="b3834-217">Boolean</span><span class="sxs-lookup"><span data-stu-id="b3834-217">Boolean</span></span>|<span data-ttu-id="b3834-218">要求设备具有最新的安全提供程序。</span><span class="sxs-lookup"><span data-stu-id="b3834-218">Require the device to have up to date security providers.</span></span> <span data-ttu-id="b3834-219">设备将要求启用 Google Play Services 并保持最新状态。</span><span class="sxs-lookup"><span data-stu-id="b3834-219">The device will require Google Play Services to be enabled and up to date.</span></span>|
|<span data-ttu-id="b3834-220">securityRequireCompanyPortalAppIntegrity</span><span class="sxs-lookup"><span data-stu-id="b3834-220">securityRequireCompanyPortalAppIntegrity</span></span>|<span data-ttu-id="b3834-221">Boolean</span><span class="sxs-lookup"><span data-stu-id="b3834-221">Boolean</span></span>|<span data-ttu-id="b3834-222">要求设备传递公司门户客户端应用运行时完整性检查。</span><span class="sxs-lookup"><span data-stu-id="b3834-222">Require the device to pass the Company Portal client app runtime integrity check.</span></span>|



## <a name="response"></a><span data-ttu-id="b3834-223">响应</span><span class="sxs-lookup"><span data-stu-id="b3834-223">Response</span></span>
<span data-ttu-id="b3834-224">如果成功，此方法会在响应正文中返回 `201 Created` 响应代码和 [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="b3834-224">If successful, this method returns a `201 Created` response code and a [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b3834-225">示例</span><span class="sxs-lookup"><span data-stu-id="b3834-225">Example</span></span>
### <a name="request"></a><span data-ttu-id="b3834-226">请求</span><span class="sxs-lookup"><span data-stu-id="b3834-226">Request</span></span>
<span data-ttu-id="b3834-227">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="b3834-227">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies
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

### <a name="response"></a><span data-ttu-id="b3834-228">响应</span><span class="sxs-lookup"><span data-stu-id="b3834-228">Response</span></span>
<span data-ttu-id="b3834-p113">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="b3834-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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



