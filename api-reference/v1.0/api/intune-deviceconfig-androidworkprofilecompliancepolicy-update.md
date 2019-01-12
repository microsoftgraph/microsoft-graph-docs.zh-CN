---
title: 更新 androidWorkProfileCompliancePolicy
description: 更新 androidWorkProfileCompliancePolicy 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 383eb0ed9ce5ddcd30110567d2f334b1819278e4
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27981936"
---
# <a name="update-androidworkprofilecompliancepolicy"></a><span data-ttu-id="cdbbc-103">更新 androidWorkProfileCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="cdbbc-103">Update androidWorkProfileCompliancePolicy</span></span>

> <span data-ttu-id="cdbbc-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="cdbbc-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="cdbbc-105">更新[androidWorkProfileCompliancePolicy](../resources/intune-deviceconfig-androidworkprofilecompliancepolicy.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="cdbbc-105">Update the properties of a [androidWorkProfileCompliancePolicy](../resources/intune-deviceconfig-androidworkprofilecompliancepolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="cdbbc-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="cdbbc-106">Prerequisites</span></span>
<span data-ttu-id="cdbbc-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="cdbbc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cdbbc-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="cdbbc-109">Permission type</span></span>|<span data-ttu-id="cdbbc-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="cdbbc-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cdbbc-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="cdbbc-111">Delegated (work or school account)</span></span>|<span data-ttu-id="cdbbc-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cdbbc-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="cdbbc-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="cdbbc-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cdbbc-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="cdbbc-114">Not supported.</span></span>|
|<span data-ttu-id="cdbbc-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="cdbbc-115">Application</span></span>|<span data-ttu-id="cdbbc-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="cdbbc-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="cdbbc-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="cdbbc-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="cdbbc-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="cdbbc-118">Request headers</span></span>
|<span data-ttu-id="cdbbc-119">标头</span><span class="sxs-lookup"><span data-stu-id="cdbbc-119">Header</span></span>|<span data-ttu-id="cdbbc-120">值</span><span class="sxs-lookup"><span data-stu-id="cdbbc-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cdbbc-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="cdbbc-121">Authorization</span></span>|<span data-ttu-id="cdbbc-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="cdbbc-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cdbbc-123">Accept</span><span class="sxs-lookup"><span data-stu-id="cdbbc-123">Accept</span></span>|<span data-ttu-id="cdbbc-124">application/json</span><span class="sxs-lookup"><span data-stu-id="cdbbc-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cdbbc-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="cdbbc-125">Request body</span></span>
<span data-ttu-id="cdbbc-126">在请求正文中，提供[androidWorkProfileCompliancePolicy](../resources/intune-deviceconfig-androidworkprofilecompliancepolicy.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="cdbbc-126">In the request body, supply a JSON representation for the [androidWorkProfileCompliancePolicy](../resources/intune-deviceconfig-androidworkprofilecompliancepolicy.md) object.</span></span>

<span data-ttu-id="cdbbc-127">下表显示时创建[androidWorkProfileCompliancePolicy](../resources/intune-deviceconfig-androidworkprofilecompliancepolicy.md)所需的属性。</span><span class="sxs-lookup"><span data-stu-id="cdbbc-127">The following table shows the properties that are required when you create the [androidWorkProfileCompliancePolicy](../resources/intune-deviceconfig-androidworkprofilecompliancepolicy.md).</span></span>

|<span data-ttu-id="cdbbc-128">属性</span><span class="sxs-lookup"><span data-stu-id="cdbbc-128">Property</span></span>|<span data-ttu-id="cdbbc-129">类型</span><span class="sxs-lookup"><span data-stu-id="cdbbc-129">Type</span></span>|<span data-ttu-id="cdbbc-130">说明</span><span class="sxs-lookup"><span data-stu-id="cdbbc-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cdbbc-131">id</span><span class="sxs-lookup"><span data-stu-id="cdbbc-131">id</span></span>|<span data-ttu-id="cdbbc-132">String</span><span class="sxs-lookup"><span data-stu-id="cdbbc-132">String</span></span>|<span data-ttu-id="cdbbc-133">实体的键。</span><span class="sxs-lookup"><span data-stu-id="cdbbc-133">Key of the entity.</span></span> <span data-ttu-id="cdbbc-134">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="cdbbc-134">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="cdbbc-135">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="cdbbc-135">createdDateTime</span></span>|<span data-ttu-id="cdbbc-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cdbbc-136">DateTimeOffset</span></span>|<span data-ttu-id="cdbbc-137">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="cdbbc-137">DateTime the object was created.</span></span> <span data-ttu-id="cdbbc-138">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="cdbbc-138">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="cdbbc-139">description</span><span class="sxs-lookup"><span data-stu-id="cdbbc-139">description</span></span>|<span data-ttu-id="cdbbc-140">String</span><span class="sxs-lookup"><span data-stu-id="cdbbc-140">String</span></span>|<span data-ttu-id="cdbbc-141">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="cdbbc-141">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="cdbbc-142">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="cdbbc-142">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="cdbbc-143">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="cdbbc-143">lastModifiedDateTime</span></span>|<span data-ttu-id="cdbbc-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cdbbc-144">DateTimeOffset</span></span>|<span data-ttu-id="cdbbc-145">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="cdbbc-145">DateTime the object was last modified.</span></span> <span data-ttu-id="cdbbc-146">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="cdbbc-146">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="cdbbc-147">displayName</span><span class="sxs-lookup"><span data-stu-id="cdbbc-147">displayName</span></span>|<span data-ttu-id="cdbbc-148">String</span><span class="sxs-lookup"><span data-stu-id="cdbbc-148">String</span></span>|<span data-ttu-id="cdbbc-149">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="cdbbc-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="cdbbc-150">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="cdbbc-150">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="cdbbc-151">version</span><span class="sxs-lookup"><span data-stu-id="cdbbc-151">version</span></span>|<span data-ttu-id="cdbbc-152">Int32</span><span class="sxs-lookup"><span data-stu-id="cdbbc-152">Int32</span></span>|<span data-ttu-id="cdbbc-153">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="cdbbc-153">Version of the device configuration.</span></span> <span data-ttu-id="cdbbc-154">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="cdbbc-154">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="cdbbc-155">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="cdbbc-155">passwordRequired</span></span>|<span data-ttu-id="cdbbc-156">Boolean</span><span class="sxs-lookup"><span data-stu-id="cdbbc-156">Boolean</span></span>|<span data-ttu-id="cdbbc-157">需要密码才可解锁设备。</span><span class="sxs-lookup"><span data-stu-id="cdbbc-157">Require a password to unlock device.</span></span>|
|<span data-ttu-id="cdbbc-158">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="cdbbc-158">passwordMinimumLength</span></span>|<span data-ttu-id="cdbbc-159">Int32</span><span class="sxs-lookup"><span data-stu-id="cdbbc-159">Int32</span></span>|<span data-ttu-id="cdbbc-160">最短密码长度。</span><span class="sxs-lookup"><span data-stu-id="cdbbc-160">Minimum password length.</span></span> <span data-ttu-id="cdbbc-161">有效值为 4 至 16</span><span class="sxs-lookup"><span data-stu-id="cdbbc-161">Valid values 4 to 16</span></span>|
|<span data-ttu-id="cdbbc-162">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="cdbbc-162">passwordRequiredType</span></span>|[<span data-ttu-id="cdbbc-163">androidRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="cdbbc-163">androidRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androidrequiredpasswordtype.md)|<span data-ttu-id="cdbbc-164">密码中的字符类型。</span><span class="sxs-lookup"><span data-stu-id="cdbbc-164">Type of characters in password.</span></span> <span data-ttu-id="cdbbc-165">可取值为：`deviceDefault`、`alphabetic`、`alphanumeric`、`alphanumericWithSymbols`、`lowSecurityBiometric`、`numeric`、`numericComplex`、`any`。</span><span class="sxs-lookup"><span data-stu-id="cdbbc-165">Possible values are: `deviceDefault`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `numeric`, `numericComplex`, `any`.</span></span>|
|<span data-ttu-id="cdbbc-166">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="cdbbc-166">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="cdbbc-167">Int32</span><span class="sxs-lookup"><span data-stu-id="cdbbc-167">Int32</span></span>|<span data-ttu-id="cdbbc-168">在需要密码之前不活动的分钟数。</span><span class="sxs-lookup"><span data-stu-id="cdbbc-168">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="cdbbc-169">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="cdbbc-169">passwordExpirationDays</span></span>|<span data-ttu-id="cdbbc-170">Int32</span><span class="sxs-lookup"><span data-stu-id="cdbbc-170">Int32</span></span>|<span data-ttu-id="cdbbc-171">密码过期前的天数。</span><span class="sxs-lookup"><span data-stu-id="cdbbc-171">Number of days before the password expires.</span></span> <span data-ttu-id="cdbbc-172">有效值为 1 至 365</span><span class="sxs-lookup"><span data-stu-id="cdbbc-172">Valid values 1 to 365</span></span>|
|<span data-ttu-id="cdbbc-173">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="cdbbc-173">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="cdbbc-174">Int32</span><span class="sxs-lookup"><span data-stu-id="cdbbc-174">Int32</span></span>|<span data-ttu-id="cdbbc-175">要阻止的以前密码的数量。</span><span class="sxs-lookup"><span data-stu-id="cdbbc-175">Number of previous passwords to block.</span></span>|
|<span data-ttu-id="cdbbc-176">securityPreventInstallAppsFromUnknownSources</span><span class="sxs-lookup"><span data-stu-id="cdbbc-176">securityPreventInstallAppsFromUnknownSources</span></span>|<span data-ttu-id="cdbbc-177">Boolean</span><span class="sxs-lookup"><span data-stu-id="cdbbc-177">Boolean</span></span>|<span data-ttu-id="cdbbc-178">要求设备不允许安装来自未知源的应用。</span><span class="sxs-lookup"><span data-stu-id="cdbbc-178">Require that devices disallow installation of apps from unknown sources.</span></span>|
|<span data-ttu-id="cdbbc-179">securityDisableUsbDebugging</span><span class="sxs-lookup"><span data-stu-id="cdbbc-179">securityDisableUsbDebugging</span></span>|<span data-ttu-id="cdbbc-180">Boolean</span><span class="sxs-lookup"><span data-stu-id="cdbbc-180">Boolean</span></span>|<span data-ttu-id="cdbbc-181">在 Android 设备上禁用 USB 调试。</span><span class="sxs-lookup"><span data-stu-id="cdbbc-181">Disable USB debugging on Android devices.</span></span>|
|<span data-ttu-id="cdbbc-182">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="cdbbc-182">securityRequireVerifyApps</span></span>|<span data-ttu-id="cdbbc-183">Boolean</span><span class="sxs-lookup"><span data-stu-id="cdbbc-183">Boolean</span></span>|<span data-ttu-id="cdbbc-184">要求启用 Android 验证应用功能。</span><span class="sxs-lookup"><span data-stu-id="cdbbc-184">Require the Android Verify apps feature is turned on.</span></span>|
|<span data-ttu-id="cdbbc-185">deviceThreatProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="cdbbc-185">deviceThreatProtectionEnabled</span></span>|<span data-ttu-id="cdbbc-186">Boolean</span><span class="sxs-lookup"><span data-stu-id="cdbbc-186">Boolean</span></span>|<span data-ttu-id="cdbbc-187">要求设备已启用设备威胁防护。</span><span class="sxs-lookup"><span data-stu-id="cdbbc-187">Require that devices have enabled device threat protection.</span></span>|
|<span data-ttu-id="cdbbc-188">deviceThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="cdbbc-188">deviceThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="cdbbc-189">deviceThreatProtectionLevel</span><span class="sxs-lookup"><span data-stu-id="cdbbc-189">deviceThreatProtectionLevel</span></span>](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|<span data-ttu-id="cdbbc-190">要求移动威胁防护最低风险级别来报告不符合情况。</span><span class="sxs-lookup"><span data-stu-id="cdbbc-190">Require Mobile Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="cdbbc-191">可取值为：`unavailable`、`secured`、`low`、`medium`、`high`、`notSet`。</span><span class="sxs-lookup"><span data-stu-id="cdbbc-191">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="cdbbc-192">securityBlockJailbrokenDevices</span><span class="sxs-lookup"><span data-stu-id="cdbbc-192">securityBlockJailbrokenDevices</span></span>|<span data-ttu-id="cdbbc-193">Boolean</span><span class="sxs-lookup"><span data-stu-id="cdbbc-193">Boolean</span></span>|<span data-ttu-id="cdbbc-194">设备不得越狱或取得 root 权限。</span><span class="sxs-lookup"><span data-stu-id="cdbbc-194">Devices must not be jailbroken or rooted.</span></span>|
|<span data-ttu-id="cdbbc-195">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="cdbbc-195">osMinimumVersion</span></span>|<span data-ttu-id="cdbbc-196">String</span><span class="sxs-lookup"><span data-stu-id="cdbbc-196">String</span></span>|<span data-ttu-id="cdbbc-197">最低 Android 版本。</span><span class="sxs-lookup"><span data-stu-id="cdbbc-197">Minimum Android version.</span></span>|
|<span data-ttu-id="cdbbc-198">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="cdbbc-198">osMaximumVersion</span></span>|<span data-ttu-id="cdbbc-199">String</span><span class="sxs-lookup"><span data-stu-id="cdbbc-199">String</span></span>|<span data-ttu-id="cdbbc-200">最高 Android 版本。</span><span class="sxs-lookup"><span data-stu-id="cdbbc-200">Maximum Android version.</span></span>|
|<span data-ttu-id="cdbbc-201">minAndroidSecurityPatchLevel</span><span class="sxs-lookup"><span data-stu-id="cdbbc-201">minAndroidSecurityPatchLevel</span></span>|<span data-ttu-id="cdbbc-202">String</span><span class="sxs-lookup"><span data-stu-id="cdbbc-202">String</span></span>|<span data-ttu-id="cdbbc-203">最低 Android 安全修补程序级别。</span><span class="sxs-lookup"><span data-stu-id="cdbbc-203">Minimum Android security patch level.</span></span>|
|<span data-ttu-id="cdbbc-204">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="cdbbc-204">storageRequireEncryption</span></span>|<span data-ttu-id="cdbbc-205">Boolean</span><span class="sxs-lookup"><span data-stu-id="cdbbc-205">Boolean</span></span>|<span data-ttu-id="cdbbc-206">要求对 Android 设备加密。</span><span class="sxs-lookup"><span data-stu-id="cdbbc-206">Require encryption on Android devices.</span></span>|
|<span data-ttu-id="cdbbc-207">securityRequireSafetyNetAttestationBasicIntegrity</span><span class="sxs-lookup"><span data-stu-id="cdbbc-207">securityRequireSafetyNetAttestationBasicIntegrity</span></span>|<span data-ttu-id="cdbbc-208">Boolean</span><span class="sxs-lookup"><span data-stu-id="cdbbc-208">Boolean</span></span>|<span data-ttu-id="cdbbc-209">要求设备传递 SafetyNet 基本完整性检查。</span><span class="sxs-lookup"><span data-stu-id="cdbbc-209">Require the device to pass the SafetyNet basic integrity check.</span></span>|
|<span data-ttu-id="cdbbc-210">securityRequireSafetyNetAttestationCertifiedDevice</span><span class="sxs-lookup"><span data-stu-id="cdbbc-210">securityRequireSafetyNetAttestationCertifiedDevice</span></span>|<span data-ttu-id="cdbbc-211">Boolean</span><span class="sxs-lookup"><span data-stu-id="cdbbc-211">Boolean</span></span>|<span data-ttu-id="cdbbc-212">要求设备传递 SafetyNet 认证设备检查。</span><span class="sxs-lookup"><span data-stu-id="cdbbc-212">Require the device to pass the SafetyNet certified device check.</span></span>|
|<span data-ttu-id="cdbbc-213">securityRequireGooglePlayServices</span><span class="sxs-lookup"><span data-stu-id="cdbbc-213">securityRequireGooglePlayServices</span></span>|<span data-ttu-id="cdbbc-214">Boolean</span><span class="sxs-lookup"><span data-stu-id="cdbbc-214">Boolean</span></span>|<span data-ttu-id="cdbbc-215">要求在设备上安装并启用 Google Play Services。</span><span class="sxs-lookup"><span data-stu-id="cdbbc-215">Require Google Play Services to be installed and enabled on the device.</span></span>|
|<span data-ttu-id="cdbbc-216">securityRequireUpToDateSecurityProviders</span><span class="sxs-lookup"><span data-stu-id="cdbbc-216">securityRequireUpToDateSecurityProviders</span></span>|<span data-ttu-id="cdbbc-217">Boolean</span><span class="sxs-lookup"><span data-stu-id="cdbbc-217">Boolean</span></span>|<span data-ttu-id="cdbbc-218">要求设备具有最新的安全提供程序。</span><span class="sxs-lookup"><span data-stu-id="cdbbc-218">Require the device to have up to date security providers.</span></span> <span data-ttu-id="cdbbc-219">设备将要求启用 Google Play Services 并保持最新状态。</span><span class="sxs-lookup"><span data-stu-id="cdbbc-219">The device will require Google Play Services to be enabled and up to date.</span></span>|
|<span data-ttu-id="cdbbc-220">securityRequireCompanyPortalAppIntegrity</span><span class="sxs-lookup"><span data-stu-id="cdbbc-220">securityRequireCompanyPortalAppIntegrity</span></span>|<span data-ttu-id="cdbbc-221">Boolean</span><span class="sxs-lookup"><span data-stu-id="cdbbc-221">Boolean</span></span>|<span data-ttu-id="cdbbc-222">要求设备传递公司门户客户端应用运行时完整性检查。</span><span class="sxs-lookup"><span data-stu-id="cdbbc-222">Require the device to pass the Company Portal client app runtime integrity check.</span></span>|



## <a name="response"></a><span data-ttu-id="cdbbc-223">响应</span><span class="sxs-lookup"><span data-stu-id="cdbbc-223">Response</span></span>
<span data-ttu-id="cdbbc-224">如果成功，此方法返回`200 OK`响应代码和响应正文中的更新的[androidWorkProfileCompliancePolicy](../resources/intune-deviceconfig-androidworkprofilecompliancepolicy.md)对象。</span><span class="sxs-lookup"><span data-stu-id="cdbbc-224">If successful, this method returns a `200 OK` response code and an updated [androidWorkProfileCompliancePolicy](../resources/intune-deviceconfig-androidworkprofilecompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cdbbc-225">示例</span><span class="sxs-lookup"><span data-stu-id="cdbbc-225">Example</span></span>
### <a name="request"></a><span data-ttu-id="cdbbc-226">请求</span><span class="sxs-lookup"><span data-stu-id="cdbbc-226">Request</span></span>
<span data-ttu-id="cdbbc-227">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="cdbbc-227">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
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

### <a name="response"></a><span data-ttu-id="cdbbc-228">响应</span><span class="sxs-lookup"><span data-stu-id="cdbbc-228">Response</span></span>
<span data-ttu-id="cdbbc-p113">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="cdbbc-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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



