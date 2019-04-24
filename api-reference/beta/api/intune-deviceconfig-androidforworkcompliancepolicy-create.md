---
title: 创建 androidForWorkCompliancePolicy
description: 创建新的 androidForWorkCompliancePolicy 对象。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: defd1b3aaf1b015e691ecf7a435270401e8cdf42
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32479363"
---
# <a name="create-androidforworkcompliancepolicy"></a><span data-ttu-id="890e0-103">创建 androidForWorkCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="890e0-103">Create androidForWorkCompliancePolicy</span></span>

> <span data-ttu-id="890e0-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="890e0-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="890e0-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="890e0-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="890e0-106">创建新的[androidForWorkCompliancePolicy](../resources/intune-deviceconfig-androidforworkcompliancepolicy.md)对象。</span><span class="sxs-lookup"><span data-stu-id="890e0-106">Create a new [androidForWorkCompliancePolicy](../resources/intune-deviceconfig-androidforworkcompliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="890e0-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="890e0-107">Prerequisites</span></span>
<span data-ttu-id="890e0-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="890e0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="890e0-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="890e0-110">Permission type</span></span>|<span data-ttu-id="890e0-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="890e0-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="890e0-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="890e0-112">Delegated (work or school account)</span></span>|<span data-ttu-id="890e0-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="890e0-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="890e0-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="890e0-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="890e0-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="890e0-115">Not supported.</span></span>|
|<span data-ttu-id="890e0-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="890e0-116">Application</span></span>|<span data-ttu-id="890e0-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="890e0-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="890e0-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="890e0-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="890e0-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="890e0-119">Request headers</span></span>
|<span data-ttu-id="890e0-120">标头</span><span class="sxs-lookup"><span data-stu-id="890e0-120">Header</span></span>|<span data-ttu-id="890e0-121">值</span><span class="sxs-lookup"><span data-stu-id="890e0-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="890e0-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="890e0-122">Authorization</span></span>|<span data-ttu-id="890e0-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="890e0-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="890e0-124">接受</span><span class="sxs-lookup"><span data-stu-id="890e0-124">Accept</span></span>|<span data-ttu-id="890e0-125">application/json</span><span class="sxs-lookup"><span data-stu-id="890e0-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="890e0-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="890e0-126">Request body</span></span>
<span data-ttu-id="890e0-127">在请求正文中, 提供 androidForWorkCompliancePolicy 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="890e0-127">In the request body, supply a JSON representation for the androidForWorkCompliancePolicy object.</span></span>

<span data-ttu-id="890e0-128">下表显示创建 androidForWorkCompliancePolicy 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="890e0-128">The following table shows the properties that are required when you create the androidForWorkCompliancePolicy.</span></span>

|<span data-ttu-id="890e0-129">属性</span><span class="sxs-lookup"><span data-stu-id="890e0-129">Property</span></span>|<span data-ttu-id="890e0-130">类型</span><span class="sxs-lookup"><span data-stu-id="890e0-130">Type</span></span>|<span data-ttu-id="890e0-131">说明</span><span class="sxs-lookup"><span data-stu-id="890e0-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="890e0-132">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="890e0-132">roleScopeTagIds</span></span>|<span data-ttu-id="890e0-133">String collection</span><span class="sxs-lookup"><span data-stu-id="890e0-133">String collection</span></span>|<span data-ttu-id="890e0-134">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="890e0-134">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="890e0-135">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="890e0-135">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="890e0-136">id</span><span class="sxs-lookup"><span data-stu-id="890e0-136">id</span></span>|<span data-ttu-id="890e0-137">String</span><span class="sxs-lookup"><span data-stu-id="890e0-137">String</span></span>|<span data-ttu-id="890e0-138">实体的键。</span><span class="sxs-lookup"><span data-stu-id="890e0-138">Key of the entity.</span></span> <span data-ttu-id="890e0-139">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="890e0-139">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="890e0-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="890e0-140">createdDateTime</span></span>|<span data-ttu-id="890e0-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="890e0-141">DateTimeOffset</span></span>|<span data-ttu-id="890e0-142">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="890e0-142">DateTime the object was created.</span></span> <span data-ttu-id="890e0-143">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="890e0-143">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="890e0-144">description</span><span class="sxs-lookup"><span data-stu-id="890e0-144">description</span></span>|<span data-ttu-id="890e0-145">字符串</span><span class="sxs-lookup"><span data-stu-id="890e0-145">String</span></span>|<span data-ttu-id="890e0-146">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="890e0-146">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="890e0-147">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="890e0-147">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="890e0-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="890e0-148">lastModifiedDateTime</span></span>|<span data-ttu-id="890e0-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="890e0-149">DateTimeOffset</span></span>|<span data-ttu-id="890e0-150">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="890e0-150">DateTime the object was last modified.</span></span> <span data-ttu-id="890e0-151">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="890e0-151">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="890e0-152">displayName</span><span class="sxs-lookup"><span data-stu-id="890e0-152">displayName</span></span>|<span data-ttu-id="890e0-153">字符串</span><span class="sxs-lookup"><span data-stu-id="890e0-153">String</span></span>|<span data-ttu-id="890e0-154">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="890e0-154">Admin provided name of the device configuration.</span></span> <span data-ttu-id="890e0-155">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="890e0-155">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="890e0-156">version</span><span class="sxs-lookup"><span data-stu-id="890e0-156">version</span></span>|<span data-ttu-id="890e0-157">Int32</span><span class="sxs-lookup"><span data-stu-id="890e0-157">Int32</span></span>|<span data-ttu-id="890e0-158">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="890e0-158">Version of the device configuration.</span></span> <span data-ttu-id="890e0-159">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="890e0-159">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="890e0-160">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="890e0-160">passwordRequired</span></span>|<span data-ttu-id="890e0-161">布尔</span><span class="sxs-lookup"><span data-stu-id="890e0-161">Boolean</span></span>|<span data-ttu-id="890e0-162">需要密码才可解锁设备。</span><span class="sxs-lookup"><span data-stu-id="890e0-162">Require a password to unlock device.</span></span>|
|<span data-ttu-id="890e0-163">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="890e0-163">passwordMinimumLength</span></span>|<span data-ttu-id="890e0-164">Int32</span><span class="sxs-lookup"><span data-stu-id="890e0-164">Int32</span></span>|<span data-ttu-id="890e0-165">最短密码长度。</span><span class="sxs-lookup"><span data-stu-id="890e0-165">Minimum password length.</span></span> <span data-ttu-id="890e0-166">有效值为 4 至 16</span><span class="sxs-lookup"><span data-stu-id="890e0-166">Valid values 4 to 16</span></span>|
|<span data-ttu-id="890e0-167">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="890e0-167">passwordRequiredType</span></span>|[<span data-ttu-id="890e0-168">androidRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="890e0-168">androidRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androidrequiredpasswordtype.md)|<span data-ttu-id="890e0-169">密码中的字符类型。</span><span class="sxs-lookup"><span data-stu-id="890e0-169">Type of characters in password.</span></span> <span data-ttu-id="890e0-170">可取值为：`deviceDefault`、`alphabetic`、`alphanumeric`、`alphanumericWithSymbols`、`lowSecurityBiometric`、`numeric`、`numericComplex`、`any`。</span><span class="sxs-lookup"><span data-stu-id="890e0-170">Possible values are: `deviceDefault`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `numeric`, `numericComplex`, `any`.</span></span>|
|<span data-ttu-id="890e0-171">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="890e0-171">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="890e0-172">Int32</span><span class="sxs-lookup"><span data-stu-id="890e0-172">Int32</span></span>|<span data-ttu-id="890e0-173">在需要密码之前不活动的分钟数。</span><span class="sxs-lookup"><span data-stu-id="890e0-173">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="890e0-174">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="890e0-174">passwordExpirationDays</span></span>|<span data-ttu-id="890e0-175">Int32</span><span class="sxs-lookup"><span data-stu-id="890e0-175">Int32</span></span>|<span data-ttu-id="890e0-176">密码过期前的天数。</span><span class="sxs-lookup"><span data-stu-id="890e0-176">Number of days before the password expires.</span></span> <span data-ttu-id="890e0-177">有效值为 1 至 365</span><span class="sxs-lookup"><span data-stu-id="890e0-177">Valid values 1 to 365</span></span>|
|<span data-ttu-id="890e0-178">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="890e0-178">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="890e0-179">Int32</span><span class="sxs-lookup"><span data-stu-id="890e0-179">Int32</span></span>|<span data-ttu-id="890e0-180">要阻止的以前密码的数量。</span><span class="sxs-lookup"><span data-stu-id="890e0-180">Number of previous passwords to block.</span></span> <span data-ttu-id="890e0-181">有效值为 1 至 24</span><span class="sxs-lookup"><span data-stu-id="890e0-181">Valid values 1 to 24</span></span>|
|<span data-ttu-id="890e0-182">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="890e0-182">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="890e0-183">Int32</span><span class="sxs-lookup"><span data-stu-id="890e0-183">Int32</span></span>|<span data-ttu-id="890e0-184">在恢复出厂设置之前允许的登录失败次数。</span><span class="sxs-lookup"><span data-stu-id="890e0-184">Number of sign-in failures allowed before factory reset.</span></span> <span data-ttu-id="890e0-185">有效值为1至16</span><span class="sxs-lookup"><span data-stu-id="890e0-185">Valid values 1 to 16</span></span>|
|<span data-ttu-id="890e0-186">securityPreventInstallAppsFromUnknownSources</span><span class="sxs-lookup"><span data-stu-id="890e0-186">securityPreventInstallAppsFromUnknownSources</span></span>|<span data-ttu-id="890e0-187">布尔</span><span class="sxs-lookup"><span data-stu-id="890e0-187">Boolean</span></span>|<span data-ttu-id="890e0-188">要求设备不允许安装来自未知源的应用。</span><span class="sxs-lookup"><span data-stu-id="890e0-188">Require that devices disallow installation of apps from unknown sources.</span></span>|
|<span data-ttu-id="890e0-189">securityDisableUsbDebugging</span><span class="sxs-lookup"><span data-stu-id="890e0-189">securityDisableUsbDebugging</span></span>|<span data-ttu-id="890e0-190">布尔</span><span class="sxs-lookup"><span data-stu-id="890e0-190">Boolean</span></span>|<span data-ttu-id="890e0-191">在 Android 设备上禁用 USB 调试。</span><span class="sxs-lookup"><span data-stu-id="890e0-191">Disable USB debugging on Android devices.</span></span>|
|<span data-ttu-id="890e0-192">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="890e0-192">securityRequireVerifyApps</span></span>|<span data-ttu-id="890e0-193">布尔</span><span class="sxs-lookup"><span data-stu-id="890e0-193">Boolean</span></span>|<span data-ttu-id="890e0-194">要求启用 Android 验证应用功能。</span><span class="sxs-lookup"><span data-stu-id="890e0-194">Require the Android Verify apps feature is turned on.</span></span>|
|<span data-ttu-id="890e0-195">deviceThreatProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="890e0-195">deviceThreatProtectionEnabled</span></span>|<span data-ttu-id="890e0-196">布尔</span><span class="sxs-lookup"><span data-stu-id="890e0-196">Boolean</span></span>|<span data-ttu-id="890e0-197">要求设备已启用设备威胁防护。</span><span class="sxs-lookup"><span data-stu-id="890e0-197">Require that devices have enabled device threat protection.</span></span>|
|<span data-ttu-id="890e0-198">deviceThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="890e0-198">deviceThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="890e0-199">deviceThreatProtectionLevel</span><span class="sxs-lookup"><span data-stu-id="890e0-199">deviceThreatProtectionLevel</span></span>](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|<span data-ttu-id="890e0-200">要求移动威胁防护最低风险级别来报告不符合情况。</span><span class="sxs-lookup"><span data-stu-id="890e0-200">Require Mobile Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="890e0-201">可取值为：`unavailable`、`secured`、`low`、`medium`、`high`、`notSet`。</span><span class="sxs-lookup"><span data-stu-id="890e0-201">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="890e0-202">securityBlockJailbrokenDevices</span><span class="sxs-lookup"><span data-stu-id="890e0-202">securityBlockJailbrokenDevices</span></span>|<span data-ttu-id="890e0-203">布尔</span><span class="sxs-lookup"><span data-stu-id="890e0-203">Boolean</span></span>|<span data-ttu-id="890e0-204">设备不得越狱或取得 root 权限。</span><span class="sxs-lookup"><span data-stu-id="890e0-204">Devices must not be jailbroken or rooted.</span></span>|
|<span data-ttu-id="890e0-205">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="890e0-205">osMinimumVersion</span></span>|<span data-ttu-id="890e0-206">字符串</span><span class="sxs-lookup"><span data-stu-id="890e0-206">String</span></span>|<span data-ttu-id="890e0-207">最低 Android 版本。</span><span class="sxs-lookup"><span data-stu-id="890e0-207">Minimum Android version.</span></span>|
|<span data-ttu-id="890e0-208">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="890e0-208">osMaximumVersion</span></span>|<span data-ttu-id="890e0-209">字符串</span><span class="sxs-lookup"><span data-stu-id="890e0-209">String</span></span>|<span data-ttu-id="890e0-210">最高 Android 版本。</span><span class="sxs-lookup"><span data-stu-id="890e0-210">Maximum Android version.</span></span>|
|<span data-ttu-id="890e0-211">minAndroidSecurityPatchLevel</span><span class="sxs-lookup"><span data-stu-id="890e0-211">minAndroidSecurityPatchLevel</span></span>|<span data-ttu-id="890e0-212">String</span><span class="sxs-lookup"><span data-stu-id="890e0-212">String</span></span>|<span data-ttu-id="890e0-213">最低 Android 安全修补程序级别。</span><span class="sxs-lookup"><span data-stu-id="890e0-213">Minimum Android security patch level.</span></span>|
|<span data-ttu-id="890e0-214">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="890e0-214">storageRequireEncryption</span></span>|<span data-ttu-id="890e0-215">布尔</span><span class="sxs-lookup"><span data-stu-id="890e0-215">Boolean</span></span>|<span data-ttu-id="890e0-216">要求对 Android 设备加密。</span><span class="sxs-lookup"><span data-stu-id="890e0-216">Require encryption on Android devices.</span></span>|
|<span data-ttu-id="890e0-217">securityRequireSafetyNetAttestationBasicIntegrity</span><span class="sxs-lookup"><span data-stu-id="890e0-217">securityRequireSafetyNetAttestationBasicIntegrity</span></span>|<span data-ttu-id="890e0-218">布尔</span><span class="sxs-lookup"><span data-stu-id="890e0-218">Boolean</span></span>|<span data-ttu-id="890e0-219">要求设备传递 SafetyNet 基本完整性检查。</span><span class="sxs-lookup"><span data-stu-id="890e0-219">Require the device to pass the SafetyNet basic integrity check.</span></span>|
|<span data-ttu-id="890e0-220">securityRequireSafetyNetAttestationCertifiedDevice</span><span class="sxs-lookup"><span data-stu-id="890e0-220">securityRequireSafetyNetAttestationCertifiedDevice</span></span>|<span data-ttu-id="890e0-221">布尔</span><span class="sxs-lookup"><span data-stu-id="890e0-221">Boolean</span></span>|<span data-ttu-id="890e0-222">要求设备传递 SafetyNet 认证设备检查。</span><span class="sxs-lookup"><span data-stu-id="890e0-222">Require the device to pass the SafetyNet certified device check.</span></span>|
|<span data-ttu-id="890e0-223">securityRequireGooglePlayServices</span><span class="sxs-lookup"><span data-stu-id="890e0-223">securityRequireGooglePlayServices</span></span>|<span data-ttu-id="890e0-224">Boolean</span><span class="sxs-lookup"><span data-stu-id="890e0-224">Boolean</span></span>|<span data-ttu-id="890e0-225">要求在设备上安装并启用 Google Play Services。</span><span class="sxs-lookup"><span data-stu-id="890e0-225">Require Google Play Services to be installed and enabled on the device.</span></span>|
|<span data-ttu-id="890e0-226">securityRequireUpToDateSecurityProviders</span><span class="sxs-lookup"><span data-stu-id="890e0-226">securityRequireUpToDateSecurityProviders</span></span>|<span data-ttu-id="890e0-227">布尔</span><span class="sxs-lookup"><span data-stu-id="890e0-227">Boolean</span></span>|<span data-ttu-id="890e0-228">要求设备具有最新的安全提供程序。</span><span class="sxs-lookup"><span data-stu-id="890e0-228">Require the device to have up to date security providers.</span></span> <span data-ttu-id="890e0-229">设备将要求启用 Google Play Services 并保持最新状态。</span><span class="sxs-lookup"><span data-stu-id="890e0-229">The device will require Google Play Services to be enabled and up to date.</span></span>|
|<span data-ttu-id="890e0-230">securityRequireCompanyPortalAppIntegrity</span><span class="sxs-lookup"><span data-stu-id="890e0-230">securityRequireCompanyPortalAppIntegrity</span></span>|<span data-ttu-id="890e0-231">Boolean</span><span class="sxs-lookup"><span data-stu-id="890e0-231">Boolean</span></span>|<span data-ttu-id="890e0-232">要求设备传递公司门户客户端应用运行时完整性检查。</span><span class="sxs-lookup"><span data-stu-id="890e0-232">Require the device to pass the Company Portal client app runtime integrity check.</span></span>|



## <a name="response"></a><span data-ttu-id="890e0-233">响应</span><span class="sxs-lookup"><span data-stu-id="890e0-233">Response</span></span>
<span data-ttu-id="890e0-234">如果成功, 此方法在响应`201 Created`正文中返回响应代码和[androidForWorkCompliancePolicy](../resources/intune-deviceconfig-androidforworkcompliancepolicy.md)对象。</span><span class="sxs-lookup"><span data-stu-id="890e0-234">If successful, this method returns a `201 Created` response code and a [androidForWorkCompliancePolicy](../resources/intune-deviceconfig-androidforworkcompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="890e0-235">示例</span><span class="sxs-lookup"><span data-stu-id="890e0-235">Example</span></span>

### <a name="request"></a><span data-ttu-id="890e0-236">请求</span><span class="sxs-lookup"><span data-stu-id="890e0-236">Request</span></span>
<span data-ttu-id="890e0-237">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="890e0-237">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies
Content-type: application/json
Content-length: 1283

{
  "@odata.type": "#microsoft.graph.androidForWorkCompliancePolicy",
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
  "securityRequireCompanyPortalAppIntegrity": true
}
```

### <a name="response"></a><span data-ttu-id="890e0-238">响应</span><span class="sxs-lookup"><span data-stu-id="890e0-238">Response</span></span>
<span data-ttu-id="890e0-p116">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="890e0-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1455

{
  "@odata.type": "#microsoft.graph.androidForWorkCompliancePolicy",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "id": "a8d667bd-67bd-a8d6-bd67-d6a8bd67d6a8",
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
  "securityRequireCompanyPortalAppIntegrity": true
}
```





