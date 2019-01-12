---
title: 创建 androidWorkProfileCompliancePolicy
description: 创建新的 androidWorkProfileCompliancePolicy 对象。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 19dcffbad18221a452ce69503f716dc73fe177c3
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27929051"
---
# <a name="create-androidworkprofilecompliancepolicy"></a><span data-ttu-id="95559-103">创建 androidWorkProfileCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="95559-103">Create androidWorkProfileCompliancePolicy</span></span>

> <span data-ttu-id="95559-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="95559-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="95559-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="95559-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="95559-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="95559-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="95559-107">创建新的[androidWorkProfileCompliancePolicy](../resources/intune-deviceconfig-androidworkprofilecompliancepolicy.md)对象。</span><span class="sxs-lookup"><span data-stu-id="95559-107">Create a new [androidWorkProfileCompliancePolicy](../resources/intune-deviceconfig-androidworkprofilecompliancepolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="95559-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="95559-108">Prerequisites</span></span>
<span data-ttu-id="95559-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="95559-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="95559-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="95559-111">Permission type</span></span>|<span data-ttu-id="95559-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="95559-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="95559-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="95559-113">Delegated (work or school account)</span></span>|<span data-ttu-id="95559-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="95559-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="95559-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="95559-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="95559-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="95559-116">Not supported.</span></span>|
|<span data-ttu-id="95559-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="95559-117">Application</span></span>|<span data-ttu-id="95559-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="95559-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="95559-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="95559-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="95559-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="95559-120">Request headers</span></span>
|<span data-ttu-id="95559-121">标头</span><span class="sxs-lookup"><span data-stu-id="95559-121">Header</span></span>|<span data-ttu-id="95559-122">值</span><span class="sxs-lookup"><span data-stu-id="95559-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="95559-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="95559-123">Authorization</span></span>|<span data-ttu-id="95559-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="95559-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="95559-125">Accept</span><span class="sxs-lookup"><span data-stu-id="95559-125">Accept</span></span>|<span data-ttu-id="95559-126">application/json</span><span class="sxs-lookup"><span data-stu-id="95559-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="95559-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="95559-127">Request body</span></span>
<span data-ttu-id="95559-128">在请求正文中，提供 androidWorkProfileCompliancePolicy 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="95559-128">In the request body, supply a JSON representation for the androidWorkProfileCompliancePolicy object.</span></span>

<span data-ttu-id="95559-129">下表显示时创建 androidWorkProfileCompliancePolicy 所需的属性。</span><span class="sxs-lookup"><span data-stu-id="95559-129">The following table shows the properties that are required when you create the androidWorkProfileCompliancePolicy.</span></span>

|<span data-ttu-id="95559-130">属性</span><span class="sxs-lookup"><span data-stu-id="95559-130">Property</span></span>|<span data-ttu-id="95559-131">类型</span><span class="sxs-lookup"><span data-stu-id="95559-131">Type</span></span>|<span data-ttu-id="95559-132">Description</span><span class="sxs-lookup"><span data-stu-id="95559-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="95559-133">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="95559-133">roleScopeTagIds</span></span>|<span data-ttu-id="95559-134">String 集合</span><span class="sxs-lookup"><span data-stu-id="95559-134">String collection</span></span>|<span data-ttu-id="95559-135">此实体实例范围标记的列表。</span><span class="sxs-lookup"><span data-stu-id="95559-135">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="95559-136">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="95559-136">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="95559-137">id</span><span class="sxs-lookup"><span data-stu-id="95559-137">id</span></span>|<span data-ttu-id="95559-138">String</span><span class="sxs-lookup"><span data-stu-id="95559-138">String</span></span>|<span data-ttu-id="95559-139">实体的键。</span><span class="sxs-lookup"><span data-stu-id="95559-139">Key of the entity.</span></span> <span data-ttu-id="95559-140">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="95559-140">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="95559-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="95559-141">createdDateTime</span></span>|<span data-ttu-id="95559-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="95559-142">DateTimeOffset</span></span>|<span data-ttu-id="95559-143">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="95559-143">DateTime the object was created.</span></span> <span data-ttu-id="95559-144">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="95559-144">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="95559-145">description</span><span class="sxs-lookup"><span data-stu-id="95559-145">description</span></span>|<span data-ttu-id="95559-146">String</span><span class="sxs-lookup"><span data-stu-id="95559-146">String</span></span>|<span data-ttu-id="95559-147">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="95559-147">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="95559-148">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="95559-148">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="95559-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="95559-149">lastModifiedDateTime</span></span>|<span data-ttu-id="95559-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="95559-150">DateTimeOffset</span></span>|<span data-ttu-id="95559-151">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="95559-151">DateTime the object was last modified.</span></span> <span data-ttu-id="95559-152">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="95559-152">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="95559-153">displayName</span><span class="sxs-lookup"><span data-stu-id="95559-153">displayName</span></span>|<span data-ttu-id="95559-154">String</span><span class="sxs-lookup"><span data-stu-id="95559-154">String</span></span>|<span data-ttu-id="95559-155">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="95559-155">Admin provided name of the device configuration.</span></span> <span data-ttu-id="95559-156">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="95559-156">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="95559-157">version</span><span class="sxs-lookup"><span data-stu-id="95559-157">version</span></span>|<span data-ttu-id="95559-158">Int32</span><span class="sxs-lookup"><span data-stu-id="95559-158">Int32</span></span>|<span data-ttu-id="95559-159">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="95559-159">Version of the device configuration.</span></span> <span data-ttu-id="95559-160">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="95559-160">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="95559-161">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="95559-161">passwordRequired</span></span>|<span data-ttu-id="95559-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="95559-162">Boolean</span></span>|<span data-ttu-id="95559-163">需要密码才可解锁设备。</span><span class="sxs-lookup"><span data-stu-id="95559-163">Require a password to unlock device.</span></span>|
|<span data-ttu-id="95559-164">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="95559-164">passwordMinimumLength</span></span>|<span data-ttu-id="95559-165">Int32</span><span class="sxs-lookup"><span data-stu-id="95559-165">Int32</span></span>|<span data-ttu-id="95559-166">最短密码长度。</span><span class="sxs-lookup"><span data-stu-id="95559-166">Minimum password length.</span></span> <span data-ttu-id="95559-167">有效值为 4 至 16</span><span class="sxs-lookup"><span data-stu-id="95559-167">Valid values 4 to 16</span></span>|
|<span data-ttu-id="95559-168">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="95559-168">passwordRequiredType</span></span>|[<span data-ttu-id="95559-169">androidRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="95559-169">androidRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androidrequiredpasswordtype.md)|<span data-ttu-id="95559-170">密码中的字符类型。</span><span class="sxs-lookup"><span data-stu-id="95559-170">Type of characters in password.</span></span> <span data-ttu-id="95559-171">可取值为：`deviceDefault`、`alphabetic`、`alphanumeric`、`alphanumericWithSymbols`、`lowSecurityBiometric`、`numeric`、`numericComplex`、`any`。</span><span class="sxs-lookup"><span data-stu-id="95559-171">Possible values are: `deviceDefault`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `numeric`, `numericComplex`, `any`.</span></span>|
|<span data-ttu-id="95559-172">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="95559-172">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="95559-173">Int32</span><span class="sxs-lookup"><span data-stu-id="95559-173">Int32</span></span>|<span data-ttu-id="95559-174">在需要密码之前不活动的分钟数。</span><span class="sxs-lookup"><span data-stu-id="95559-174">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="95559-175">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="95559-175">passwordExpirationDays</span></span>|<span data-ttu-id="95559-176">Int32</span><span class="sxs-lookup"><span data-stu-id="95559-176">Int32</span></span>|<span data-ttu-id="95559-177">密码过期前的天数。</span><span class="sxs-lookup"><span data-stu-id="95559-177">Number of days before the password expires.</span></span> <span data-ttu-id="95559-178">有效值为 1 至 365</span><span class="sxs-lookup"><span data-stu-id="95559-178">Valid values 1 to 365</span></span>|
|<span data-ttu-id="95559-179">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="95559-179">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="95559-180">Int32</span><span class="sxs-lookup"><span data-stu-id="95559-180">Int32</span></span>|<span data-ttu-id="95559-181">要阻止的以前密码的数量。</span><span class="sxs-lookup"><span data-stu-id="95559-181">Number of previous passwords to block.</span></span>|
|<span data-ttu-id="95559-182">securityPreventInstallAppsFromUnknownSources</span><span class="sxs-lookup"><span data-stu-id="95559-182">securityPreventInstallAppsFromUnknownSources</span></span>|<span data-ttu-id="95559-183">Boolean</span><span class="sxs-lookup"><span data-stu-id="95559-183">Boolean</span></span>|<span data-ttu-id="95559-184">要求设备不允许安装来自未知源的应用。</span><span class="sxs-lookup"><span data-stu-id="95559-184">Require that devices disallow installation of apps from unknown sources.</span></span>|
|<span data-ttu-id="95559-185">securityDisableUsbDebugging</span><span class="sxs-lookup"><span data-stu-id="95559-185">securityDisableUsbDebugging</span></span>|<span data-ttu-id="95559-186">Boolean</span><span class="sxs-lookup"><span data-stu-id="95559-186">Boolean</span></span>|<span data-ttu-id="95559-187">在 Android 设备上禁用 USB 调试。</span><span class="sxs-lookup"><span data-stu-id="95559-187">Disable USB debugging on Android devices.</span></span>|
|<span data-ttu-id="95559-188">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="95559-188">securityRequireVerifyApps</span></span>|<span data-ttu-id="95559-189">Boolean</span><span class="sxs-lookup"><span data-stu-id="95559-189">Boolean</span></span>|<span data-ttu-id="95559-190">要求启用 Android 验证应用功能。</span><span class="sxs-lookup"><span data-stu-id="95559-190">Require the Android Verify apps feature is turned on.</span></span>|
|<span data-ttu-id="95559-191">deviceThreatProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="95559-191">deviceThreatProtectionEnabled</span></span>|<span data-ttu-id="95559-192">Boolean</span><span class="sxs-lookup"><span data-stu-id="95559-192">Boolean</span></span>|<span data-ttu-id="95559-193">要求设备已启用设备威胁防护。</span><span class="sxs-lookup"><span data-stu-id="95559-193">Require that devices have enabled device threat protection.</span></span>|
|<span data-ttu-id="95559-194">deviceThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="95559-194">deviceThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="95559-195">deviceThreatProtectionLevel</span><span class="sxs-lookup"><span data-stu-id="95559-195">deviceThreatProtectionLevel</span></span>](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|<span data-ttu-id="95559-196">要求移动威胁防护最低风险级别来报告不符合情况。</span><span class="sxs-lookup"><span data-stu-id="95559-196">Require Mobile Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="95559-197">可取值为：`unavailable`、`secured`、`low`、`medium`、`high`、`notSet`。</span><span class="sxs-lookup"><span data-stu-id="95559-197">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="95559-198">securityBlockJailbrokenDevices</span><span class="sxs-lookup"><span data-stu-id="95559-198">securityBlockJailbrokenDevices</span></span>|<span data-ttu-id="95559-199">Boolean</span><span class="sxs-lookup"><span data-stu-id="95559-199">Boolean</span></span>|<span data-ttu-id="95559-200">设备不得越狱或取得 root 权限。</span><span class="sxs-lookup"><span data-stu-id="95559-200">Devices must not be jailbroken or rooted.</span></span>|
|<span data-ttu-id="95559-201">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="95559-201">osMinimumVersion</span></span>|<span data-ttu-id="95559-202">String</span><span class="sxs-lookup"><span data-stu-id="95559-202">String</span></span>|<span data-ttu-id="95559-203">最低 Android 版本。</span><span class="sxs-lookup"><span data-stu-id="95559-203">Minimum Android version.</span></span>|
|<span data-ttu-id="95559-204">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="95559-204">osMaximumVersion</span></span>|<span data-ttu-id="95559-205">String</span><span class="sxs-lookup"><span data-stu-id="95559-205">String</span></span>|<span data-ttu-id="95559-206">最高 Android 版本。</span><span class="sxs-lookup"><span data-stu-id="95559-206">Maximum Android version.</span></span>|
|<span data-ttu-id="95559-207">minAndroidSecurityPatchLevel</span><span class="sxs-lookup"><span data-stu-id="95559-207">minAndroidSecurityPatchLevel</span></span>|<span data-ttu-id="95559-208">String</span><span class="sxs-lookup"><span data-stu-id="95559-208">String</span></span>|<span data-ttu-id="95559-209">最低 Android 安全修补程序级别。</span><span class="sxs-lookup"><span data-stu-id="95559-209">Minimum Android security patch level.</span></span>|
|<span data-ttu-id="95559-210">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="95559-210">storageRequireEncryption</span></span>|<span data-ttu-id="95559-211">Boolean</span><span class="sxs-lookup"><span data-stu-id="95559-211">Boolean</span></span>|<span data-ttu-id="95559-212">要求对 Android 设备加密。</span><span class="sxs-lookup"><span data-stu-id="95559-212">Require encryption on Android devices.</span></span>|
|<span data-ttu-id="95559-213">securityRequireSafetyNetAttestationBasicIntegrity</span><span class="sxs-lookup"><span data-stu-id="95559-213">securityRequireSafetyNetAttestationBasicIntegrity</span></span>|<span data-ttu-id="95559-214">Boolean</span><span class="sxs-lookup"><span data-stu-id="95559-214">Boolean</span></span>|<span data-ttu-id="95559-215">要求设备传递 SafetyNet 基本完整性检查。</span><span class="sxs-lookup"><span data-stu-id="95559-215">Require the device to pass the SafetyNet basic integrity check.</span></span>|
|<span data-ttu-id="95559-216">securityRequireSafetyNetAttestationCertifiedDevice</span><span class="sxs-lookup"><span data-stu-id="95559-216">securityRequireSafetyNetAttestationCertifiedDevice</span></span>|<span data-ttu-id="95559-217">Boolean</span><span class="sxs-lookup"><span data-stu-id="95559-217">Boolean</span></span>|<span data-ttu-id="95559-218">要求设备传递 SafetyNet 认证设备检查。</span><span class="sxs-lookup"><span data-stu-id="95559-218">Require the device to pass the SafetyNet certified device check.</span></span>|
|<span data-ttu-id="95559-219">securityRequireGooglePlayServices</span><span class="sxs-lookup"><span data-stu-id="95559-219">securityRequireGooglePlayServices</span></span>|<span data-ttu-id="95559-220">Boolean</span><span class="sxs-lookup"><span data-stu-id="95559-220">Boolean</span></span>|<span data-ttu-id="95559-221">要求在设备上安装并启用 Google Play Services。</span><span class="sxs-lookup"><span data-stu-id="95559-221">Require Google Play Services to be installed and enabled on the device.</span></span>|
|<span data-ttu-id="95559-222">securityRequireUpToDateSecurityProviders</span><span class="sxs-lookup"><span data-stu-id="95559-222">securityRequireUpToDateSecurityProviders</span></span>|<span data-ttu-id="95559-223">Boolean</span><span class="sxs-lookup"><span data-stu-id="95559-223">Boolean</span></span>|<span data-ttu-id="95559-224">要求设备具有最新的安全提供程序。</span><span class="sxs-lookup"><span data-stu-id="95559-224">Require the device to have up to date security providers.</span></span> <span data-ttu-id="95559-225">设备将要求启用 Google Play Services 并保持最新状态。</span><span class="sxs-lookup"><span data-stu-id="95559-225">The device will require Google Play Services to be enabled and up to date.</span></span>|
|<span data-ttu-id="95559-226">securityRequireCompanyPortalAppIntegrity</span><span class="sxs-lookup"><span data-stu-id="95559-226">securityRequireCompanyPortalAppIntegrity</span></span>|<span data-ttu-id="95559-227">Boolean</span><span class="sxs-lookup"><span data-stu-id="95559-227">Boolean</span></span>|<span data-ttu-id="95559-228">要求设备传递公司门户客户端应用运行时完整性检查。</span><span class="sxs-lookup"><span data-stu-id="95559-228">Require the device to pass the Company Portal client app runtime integrity check.</span></span>|



## <a name="response"></a><span data-ttu-id="95559-229">响应</span><span class="sxs-lookup"><span data-stu-id="95559-229">Response</span></span>
<span data-ttu-id="95559-230">如果成功，此方法返回`201 Created`响应代码和响应正文中的[androidWorkProfileCompliancePolicy](../resources/intune-deviceconfig-androidworkprofilecompliancepolicy.md)对象。</span><span class="sxs-lookup"><span data-stu-id="95559-230">If successful, this method returns a `201 Created` response code and a [androidWorkProfileCompliancePolicy](../resources/intune-deviceconfig-androidworkprofilecompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="95559-231">示例</span><span class="sxs-lookup"><span data-stu-id="95559-231">Example</span></span>
### <a name="request"></a><span data-ttu-id="95559-232">请求</span><span class="sxs-lookup"><span data-stu-id="95559-232">Request</span></span>
<span data-ttu-id="95559-233">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="95559-233">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies
Content-type: application/json
Content-length: 1296

{
  "@odata.type": "#microsoft.graph.androidWorkProfileCompliancePolicy",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
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

### <a name="response"></a><span data-ttu-id="95559-234">响应</span><span class="sxs-lookup"><span data-stu-id="95559-234">Response</span></span>
<span data-ttu-id="95559-p115">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="95559-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1404

{
  "@odata.type": "#microsoft.graph.androidWorkProfileCompliancePolicy",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
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





