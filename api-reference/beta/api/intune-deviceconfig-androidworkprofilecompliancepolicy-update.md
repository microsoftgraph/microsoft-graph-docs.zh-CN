---
title: 更新 androidWorkProfileCompliancePolicy
description: 更新 androidWorkProfileCompliancePolicy 对象的属性。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: ead60a0683738de51947e1186e8821f55651ca15
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29402802"
---
# <a name="update-androidworkprofilecompliancepolicy"></a><span data-ttu-id="805f8-103">更新 androidWorkProfileCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="805f8-103">Update androidWorkProfileCompliancePolicy</span></span>

> <span data-ttu-id="805f8-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="805f8-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="805f8-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="805f8-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="805f8-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="805f8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="805f8-107">更新[androidWorkProfileCompliancePolicy](../resources/intune-deviceconfig-androidworkprofilecompliancepolicy.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="805f8-107">Update the properties of a [androidWorkProfileCompliancePolicy](../resources/intune-deviceconfig-androidworkprofilecompliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="805f8-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="805f8-108">Prerequisites</span></span>
<span data-ttu-id="805f8-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="805f8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="805f8-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="805f8-111">Permission type</span></span>|<span data-ttu-id="805f8-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="805f8-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="805f8-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="805f8-113">Delegated (work or school account)</span></span>|<span data-ttu-id="805f8-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="805f8-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="805f8-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="805f8-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="805f8-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="805f8-116">Not supported.</span></span>|
|<span data-ttu-id="805f8-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="805f8-117">Application</span></span>|<span data-ttu-id="805f8-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="805f8-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="805f8-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="805f8-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="805f8-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="805f8-120">Request headers</span></span>
|<span data-ttu-id="805f8-121">标头</span><span class="sxs-lookup"><span data-stu-id="805f8-121">Header</span></span>|<span data-ttu-id="805f8-122">值</span><span class="sxs-lookup"><span data-stu-id="805f8-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="805f8-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="805f8-123">Authorization</span></span>|<span data-ttu-id="805f8-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="805f8-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="805f8-125">Accept</span><span class="sxs-lookup"><span data-stu-id="805f8-125">Accept</span></span>|<span data-ttu-id="805f8-126">application/json</span><span class="sxs-lookup"><span data-stu-id="805f8-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="805f8-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="805f8-127">Request body</span></span>
<span data-ttu-id="805f8-128">在请求正文中，提供[androidWorkProfileCompliancePolicy](../resources/intune-deviceconfig-androidworkprofilecompliancepolicy.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="805f8-128">In the request body, supply a JSON representation for the [androidWorkProfileCompliancePolicy](../resources/intune-deviceconfig-androidworkprofilecompliancepolicy.md) object.</span></span>

<span data-ttu-id="805f8-129">下表显示时创建[androidWorkProfileCompliancePolicy](../resources/intune-deviceconfig-androidworkprofilecompliancepolicy.md)所需的属性。</span><span class="sxs-lookup"><span data-stu-id="805f8-129">The following table shows the properties that are required when you create the [androidWorkProfileCompliancePolicy](../resources/intune-deviceconfig-androidworkprofilecompliancepolicy.md).</span></span>

|<span data-ttu-id="805f8-130">属性</span><span class="sxs-lookup"><span data-stu-id="805f8-130">Property</span></span>|<span data-ttu-id="805f8-131">类型</span><span class="sxs-lookup"><span data-stu-id="805f8-131">Type</span></span>|<span data-ttu-id="805f8-132">说明</span><span class="sxs-lookup"><span data-stu-id="805f8-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="805f8-133">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="805f8-133">roleScopeTagIds</span></span>|<span data-ttu-id="805f8-134">String 集合</span><span class="sxs-lookup"><span data-stu-id="805f8-134">String collection</span></span>|<span data-ttu-id="805f8-135">此实体实例范围标记的列表。</span><span class="sxs-lookup"><span data-stu-id="805f8-135">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="805f8-136">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="805f8-136">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="805f8-137">id</span><span class="sxs-lookup"><span data-stu-id="805f8-137">id</span></span>|<span data-ttu-id="805f8-138">String</span><span class="sxs-lookup"><span data-stu-id="805f8-138">String</span></span>|<span data-ttu-id="805f8-139">实体的键。</span><span class="sxs-lookup"><span data-stu-id="805f8-139">Key of the entity.</span></span> <span data-ttu-id="805f8-140">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="805f8-140">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="805f8-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="805f8-141">createdDateTime</span></span>|<span data-ttu-id="805f8-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="805f8-142">DateTimeOffset</span></span>|<span data-ttu-id="805f8-143">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="805f8-143">DateTime the object was created.</span></span> <span data-ttu-id="805f8-144">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="805f8-144">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="805f8-145">description</span><span class="sxs-lookup"><span data-stu-id="805f8-145">description</span></span>|<span data-ttu-id="805f8-146">String</span><span class="sxs-lookup"><span data-stu-id="805f8-146">String</span></span>|<span data-ttu-id="805f8-147">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="805f8-147">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="805f8-148">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="805f8-148">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="805f8-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="805f8-149">lastModifiedDateTime</span></span>|<span data-ttu-id="805f8-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="805f8-150">DateTimeOffset</span></span>|<span data-ttu-id="805f8-151">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="805f8-151">DateTime the object was last modified.</span></span> <span data-ttu-id="805f8-152">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="805f8-152">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="805f8-153">displayName</span><span class="sxs-lookup"><span data-stu-id="805f8-153">displayName</span></span>|<span data-ttu-id="805f8-154">String</span><span class="sxs-lookup"><span data-stu-id="805f8-154">String</span></span>|<span data-ttu-id="805f8-155">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="805f8-155">Admin provided name of the device configuration.</span></span> <span data-ttu-id="805f8-156">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="805f8-156">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="805f8-157">version</span><span class="sxs-lookup"><span data-stu-id="805f8-157">version</span></span>|<span data-ttu-id="805f8-158">Int32</span><span class="sxs-lookup"><span data-stu-id="805f8-158">Int32</span></span>|<span data-ttu-id="805f8-159">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="805f8-159">Version of the device configuration.</span></span> <span data-ttu-id="805f8-160">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="805f8-160">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="805f8-161">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="805f8-161">passwordRequired</span></span>|<span data-ttu-id="805f8-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="805f8-162">Boolean</span></span>|<span data-ttu-id="805f8-163">需要密码才可解锁设备。</span><span class="sxs-lookup"><span data-stu-id="805f8-163">Require a password to unlock device.</span></span>|
|<span data-ttu-id="805f8-164">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="805f8-164">passwordMinimumLength</span></span>|<span data-ttu-id="805f8-165">Int32</span><span class="sxs-lookup"><span data-stu-id="805f8-165">Int32</span></span>|<span data-ttu-id="805f8-166">最短密码长度。</span><span class="sxs-lookup"><span data-stu-id="805f8-166">Minimum password length.</span></span> <span data-ttu-id="805f8-167">有效值为 4 至 16</span><span class="sxs-lookup"><span data-stu-id="805f8-167">Valid values 4 to 16</span></span>|
|<span data-ttu-id="805f8-168">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="805f8-168">passwordRequiredType</span></span>|[<span data-ttu-id="805f8-169">androidRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="805f8-169">androidRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androidrequiredpasswordtype.md)|<span data-ttu-id="805f8-170">密码中的字符类型。</span><span class="sxs-lookup"><span data-stu-id="805f8-170">Type of characters in password.</span></span> <span data-ttu-id="805f8-171">可取值为：`deviceDefault`、`alphabetic`、`alphanumeric`、`alphanumericWithSymbols`、`lowSecurityBiometric`、`numeric`、`numericComplex`、`any`。</span><span class="sxs-lookup"><span data-stu-id="805f8-171">Possible values are: `deviceDefault`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `numeric`, `numericComplex`, `any`.</span></span>|
|<span data-ttu-id="805f8-172">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="805f8-172">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="805f8-173">Int32</span><span class="sxs-lookup"><span data-stu-id="805f8-173">Int32</span></span>|<span data-ttu-id="805f8-174">在需要密码之前不活动的分钟数。</span><span class="sxs-lookup"><span data-stu-id="805f8-174">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="805f8-175">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="805f8-175">passwordExpirationDays</span></span>|<span data-ttu-id="805f8-176">Int32</span><span class="sxs-lookup"><span data-stu-id="805f8-176">Int32</span></span>|<span data-ttu-id="805f8-177">密码过期前的天数。</span><span class="sxs-lookup"><span data-stu-id="805f8-177">Number of days before the password expires.</span></span> <span data-ttu-id="805f8-178">有效值为 1 至 365</span><span class="sxs-lookup"><span data-stu-id="805f8-178">Valid values 1 to 365</span></span>|
|<span data-ttu-id="805f8-179">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="805f8-179">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="805f8-180">Int32</span><span class="sxs-lookup"><span data-stu-id="805f8-180">Int32</span></span>|<span data-ttu-id="805f8-181">要阻止的以前密码的数量。</span><span class="sxs-lookup"><span data-stu-id="805f8-181">Number of previous passwords to block.</span></span> <span data-ttu-id="805f8-182">有效值为 1 至 24</span><span class="sxs-lookup"><span data-stu-id="805f8-182">Valid values 1 to 24</span></span>|
|<span data-ttu-id="805f8-183">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="805f8-183">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="805f8-184">Int32</span><span class="sxs-lookup"><span data-stu-id="805f8-184">Int32</span></span>|<span data-ttu-id="805f8-185">出厂重置之前允许的登录失败的次数。</span><span class="sxs-lookup"><span data-stu-id="805f8-185">Number of sign-in failures allowed before factory reset.</span></span> <span data-ttu-id="805f8-186">有效的值 1 到 16</span><span class="sxs-lookup"><span data-stu-id="805f8-186">Valid values 1 to 16</span></span>|
|<span data-ttu-id="805f8-187">securityPreventInstallAppsFromUnknownSources</span><span class="sxs-lookup"><span data-stu-id="805f8-187">securityPreventInstallAppsFromUnknownSources</span></span>|<span data-ttu-id="805f8-188">Boolean</span><span class="sxs-lookup"><span data-stu-id="805f8-188">Boolean</span></span>|<span data-ttu-id="805f8-189">要求设备不允许安装来自未知源的应用。</span><span class="sxs-lookup"><span data-stu-id="805f8-189">Require that devices disallow installation of apps from unknown sources.</span></span>|
|<span data-ttu-id="805f8-190">securityDisableUsbDebugging</span><span class="sxs-lookup"><span data-stu-id="805f8-190">securityDisableUsbDebugging</span></span>|<span data-ttu-id="805f8-191">Boolean</span><span class="sxs-lookup"><span data-stu-id="805f8-191">Boolean</span></span>|<span data-ttu-id="805f8-192">在 Android 设备上禁用 USB 调试。</span><span class="sxs-lookup"><span data-stu-id="805f8-192">Disable USB debugging on Android devices.</span></span>|
|<span data-ttu-id="805f8-193">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="805f8-193">securityRequireVerifyApps</span></span>|<span data-ttu-id="805f8-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="805f8-194">Boolean</span></span>|<span data-ttu-id="805f8-195">要求启用 Android 验证应用功能。</span><span class="sxs-lookup"><span data-stu-id="805f8-195">Require the Android Verify apps feature is turned on.</span></span>|
|<span data-ttu-id="805f8-196">deviceThreatProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="805f8-196">deviceThreatProtectionEnabled</span></span>|<span data-ttu-id="805f8-197">Boolean</span><span class="sxs-lookup"><span data-stu-id="805f8-197">Boolean</span></span>|<span data-ttu-id="805f8-198">要求设备已启用设备威胁防护。</span><span class="sxs-lookup"><span data-stu-id="805f8-198">Require that devices have enabled device threat protection.</span></span>|
|<span data-ttu-id="805f8-199">deviceThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="805f8-199">deviceThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="805f8-200">deviceThreatProtectionLevel</span><span class="sxs-lookup"><span data-stu-id="805f8-200">deviceThreatProtectionLevel</span></span>](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|<span data-ttu-id="805f8-201">要求移动威胁防护最低风险级别来报告不符合情况。</span><span class="sxs-lookup"><span data-stu-id="805f8-201">Require Mobile Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="805f8-202">可取值为：`unavailable`、`secured`、`low`、`medium`、`high`、`notSet`。</span><span class="sxs-lookup"><span data-stu-id="805f8-202">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="805f8-203">securityBlockJailbrokenDevices</span><span class="sxs-lookup"><span data-stu-id="805f8-203">securityBlockJailbrokenDevices</span></span>|<span data-ttu-id="805f8-204">Boolean</span><span class="sxs-lookup"><span data-stu-id="805f8-204">Boolean</span></span>|<span data-ttu-id="805f8-205">设备不得越狱或取得 root 权限。</span><span class="sxs-lookup"><span data-stu-id="805f8-205">Devices must not be jailbroken or rooted.</span></span>|
|<span data-ttu-id="805f8-206">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="805f8-206">osMinimumVersion</span></span>|<span data-ttu-id="805f8-207">String</span><span class="sxs-lookup"><span data-stu-id="805f8-207">String</span></span>|<span data-ttu-id="805f8-208">最低 Android 版本。</span><span class="sxs-lookup"><span data-stu-id="805f8-208">Minimum Android version.</span></span>|
|<span data-ttu-id="805f8-209">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="805f8-209">osMaximumVersion</span></span>|<span data-ttu-id="805f8-210">String</span><span class="sxs-lookup"><span data-stu-id="805f8-210">String</span></span>|<span data-ttu-id="805f8-211">最高 Android 版本。</span><span class="sxs-lookup"><span data-stu-id="805f8-211">Maximum Android version.</span></span>|
|<span data-ttu-id="805f8-212">minAndroidSecurityPatchLevel</span><span class="sxs-lookup"><span data-stu-id="805f8-212">minAndroidSecurityPatchLevel</span></span>|<span data-ttu-id="805f8-213">String</span><span class="sxs-lookup"><span data-stu-id="805f8-213">String</span></span>|<span data-ttu-id="805f8-214">最低 Android 安全修补程序级别。</span><span class="sxs-lookup"><span data-stu-id="805f8-214">Minimum Android security patch level.</span></span>|
|<span data-ttu-id="805f8-215">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="805f8-215">storageRequireEncryption</span></span>|<span data-ttu-id="805f8-216">Boolean</span><span class="sxs-lookup"><span data-stu-id="805f8-216">Boolean</span></span>|<span data-ttu-id="805f8-217">要求对 Android 设备加密。</span><span class="sxs-lookup"><span data-stu-id="805f8-217">Require encryption on Android devices.</span></span>|
|<span data-ttu-id="805f8-218">securityRequireSafetyNetAttestationBasicIntegrity</span><span class="sxs-lookup"><span data-stu-id="805f8-218">securityRequireSafetyNetAttestationBasicIntegrity</span></span>|<span data-ttu-id="805f8-219">Boolean</span><span class="sxs-lookup"><span data-stu-id="805f8-219">Boolean</span></span>|<span data-ttu-id="805f8-220">要求设备传递 SafetyNet 基本完整性检查。</span><span class="sxs-lookup"><span data-stu-id="805f8-220">Require the device to pass the SafetyNet basic integrity check.</span></span>|
|<span data-ttu-id="805f8-221">securityRequireSafetyNetAttestationCertifiedDevice</span><span class="sxs-lookup"><span data-stu-id="805f8-221">securityRequireSafetyNetAttestationCertifiedDevice</span></span>|<span data-ttu-id="805f8-222">Boolean</span><span class="sxs-lookup"><span data-stu-id="805f8-222">Boolean</span></span>|<span data-ttu-id="805f8-223">要求设备传递 SafetyNet 认证设备检查。</span><span class="sxs-lookup"><span data-stu-id="805f8-223">Require the device to pass the SafetyNet certified device check.</span></span>|
|<span data-ttu-id="805f8-224">securityRequireGooglePlayServices</span><span class="sxs-lookup"><span data-stu-id="805f8-224">securityRequireGooglePlayServices</span></span>|<span data-ttu-id="805f8-225">Boolean</span><span class="sxs-lookup"><span data-stu-id="805f8-225">Boolean</span></span>|<span data-ttu-id="805f8-226">要求在设备上安装并启用 Google Play Services。</span><span class="sxs-lookup"><span data-stu-id="805f8-226">Require Google Play Services to be installed and enabled on the device.</span></span>|
|<span data-ttu-id="805f8-227">securityRequireUpToDateSecurityProviders</span><span class="sxs-lookup"><span data-stu-id="805f8-227">securityRequireUpToDateSecurityProviders</span></span>|<span data-ttu-id="805f8-228">Boolean</span><span class="sxs-lookup"><span data-stu-id="805f8-228">Boolean</span></span>|<span data-ttu-id="805f8-229">要求设备具有最新的安全提供程序。</span><span class="sxs-lookup"><span data-stu-id="805f8-229">Require the device to have up to date security providers.</span></span> <span data-ttu-id="805f8-230">设备将要求启用 Google Play Services 并保持最新状态。</span><span class="sxs-lookup"><span data-stu-id="805f8-230">The device will require Google Play Services to be enabled and up to date.</span></span>|
|<span data-ttu-id="805f8-231">securityRequireCompanyPortalAppIntegrity</span><span class="sxs-lookup"><span data-stu-id="805f8-231">securityRequireCompanyPortalAppIntegrity</span></span>|<span data-ttu-id="805f8-232">Boolean</span><span class="sxs-lookup"><span data-stu-id="805f8-232">Boolean</span></span>|<span data-ttu-id="805f8-233">要求设备传递公司门户客户端应用运行时完整性检查。</span><span class="sxs-lookup"><span data-stu-id="805f8-233">Require the device to pass the Company Portal client app runtime integrity check.</span></span>|



## <a name="response"></a><span data-ttu-id="805f8-234">响应</span><span class="sxs-lookup"><span data-stu-id="805f8-234">Response</span></span>
<span data-ttu-id="805f8-235">如果成功，此方法返回`200 OK`响应代码和响应正文中的更新的[androidWorkProfileCompliancePolicy](../resources/intune-deviceconfig-androidworkprofilecompliancepolicy.md)对象。</span><span class="sxs-lookup"><span data-stu-id="805f8-235">If successful, this method returns a `200 OK` response code and an updated [androidWorkProfileCompliancePolicy](../resources/intune-deviceconfig-androidworkprofilecompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="805f8-236">示例</span><span class="sxs-lookup"><span data-stu-id="805f8-236">Example</span></span>

### <a name="request"></a><span data-ttu-id="805f8-237">请求</span><span class="sxs-lookup"><span data-stu-id="805f8-237">Request</span></span>
<span data-ttu-id="805f8-238">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="805f8-238">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
Content-type: application/json
Content-length: 1287

{
  "@odata.type": "#microsoft.graph.androidWorkProfileCompliancePolicy",
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

### <a name="response"></a><span data-ttu-id="805f8-239">响应</span><span class="sxs-lookup"><span data-stu-id="805f8-239">Response</span></span>
<span data-ttu-id="805f8-p117">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="805f8-p117">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1459

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




