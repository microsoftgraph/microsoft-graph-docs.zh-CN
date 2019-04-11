---
title: 更新 androidForWorkCompliancePolicy
description: 更新 androidForWorkCompliancePolicy 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3ee4ad9af831d033aee1ac6e54469e5b591e88a5
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/11/2019
ms.locfileid: "31781328"
---
# <a name="update-androidforworkcompliancepolicy"></a><span data-ttu-id="b9c11-103">更新 androidForWorkCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="b9c11-103">Update androidForWorkCompliancePolicy</span></span>

> <span data-ttu-id="b9c11-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="b9c11-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b9c11-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b9c11-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b9c11-106">更新[androidForWorkCompliancePolicy](../resources/intune-deviceconfig-androidforworkcompliancepolicy.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="b9c11-106">Update the properties of a [androidForWorkCompliancePolicy](../resources/intune-deviceconfig-androidforworkcompliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b9c11-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="b9c11-107">Prerequisites</span></span>
<span data-ttu-id="b9c11-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b9c11-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b9c11-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="b9c11-110">Permission type</span></span>|<span data-ttu-id="b9c11-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="b9c11-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b9c11-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b9c11-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b9c11-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b9c11-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b9c11-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b9c11-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b9c11-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="b9c11-115">Not supported.</span></span>|
|<span data-ttu-id="b9c11-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="b9c11-116">Application</span></span>|<span data-ttu-id="b9c11-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="b9c11-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b9c11-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b9c11-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="b9c11-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="b9c11-119">Request headers</span></span>
|<span data-ttu-id="b9c11-120">标头</span><span class="sxs-lookup"><span data-stu-id="b9c11-120">Header</span></span>|<span data-ttu-id="b9c11-121">值</span><span class="sxs-lookup"><span data-stu-id="b9c11-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b9c11-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="b9c11-122">Authorization</span></span>|<span data-ttu-id="b9c11-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="b9c11-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b9c11-124">接受</span><span class="sxs-lookup"><span data-stu-id="b9c11-124">Accept</span></span>|<span data-ttu-id="b9c11-125">application/json</span><span class="sxs-lookup"><span data-stu-id="b9c11-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b9c11-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="b9c11-126">Request body</span></span>
<span data-ttu-id="b9c11-127">在请求正文中, 提供[androidForWorkCompliancePolicy](../resources/intune-deviceconfig-androidforworkcompliancepolicy.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b9c11-127">In the request body, supply a JSON representation for the [androidForWorkCompliancePolicy](../resources/intune-deviceconfig-androidforworkcompliancepolicy.md) object.</span></span>

<span data-ttu-id="b9c11-128">下表显示创建[androidForWorkCompliancePolicy](../resources/intune-deviceconfig-androidforworkcompliancepolicy.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="b9c11-128">The following table shows the properties that are required when you create the [androidForWorkCompliancePolicy](../resources/intune-deviceconfig-androidforworkcompliancepolicy.md).</span></span>

|<span data-ttu-id="b9c11-129">属性</span><span class="sxs-lookup"><span data-stu-id="b9c11-129">Property</span></span>|<span data-ttu-id="b9c11-130">类型</span><span class="sxs-lookup"><span data-stu-id="b9c11-130">Type</span></span>|<span data-ttu-id="b9c11-131">说明</span><span class="sxs-lookup"><span data-stu-id="b9c11-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b9c11-132">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="b9c11-132">roleScopeTagIds</span></span>|<span data-ttu-id="b9c11-133">String 集合</span><span class="sxs-lookup"><span data-stu-id="b9c11-133">String collection</span></span>|<span data-ttu-id="b9c11-134">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="b9c11-134">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="b9c11-135">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="b9c11-135">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="b9c11-136">id</span><span class="sxs-lookup"><span data-stu-id="b9c11-136">id</span></span>|<span data-ttu-id="b9c11-137">String</span><span class="sxs-lookup"><span data-stu-id="b9c11-137">String</span></span>|<span data-ttu-id="b9c11-138">实体的键。</span><span class="sxs-lookup"><span data-stu-id="b9c11-138">Key of the entity.</span></span> <span data-ttu-id="b9c11-139">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="b9c11-139">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="b9c11-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b9c11-140">createdDateTime</span></span>|<span data-ttu-id="b9c11-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b9c11-141">DateTimeOffset</span></span>|<span data-ttu-id="b9c11-142">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="b9c11-142">DateTime the object was created.</span></span> <span data-ttu-id="b9c11-143">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="b9c11-143">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="b9c11-144">description</span><span class="sxs-lookup"><span data-stu-id="b9c11-144">description</span></span>|<span data-ttu-id="b9c11-145">String</span><span class="sxs-lookup"><span data-stu-id="b9c11-145">String</span></span>|<span data-ttu-id="b9c11-146">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="b9c11-146">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="b9c11-147">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="b9c11-147">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="b9c11-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b9c11-148">lastModifiedDateTime</span></span>|<span data-ttu-id="b9c11-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b9c11-149">DateTimeOffset</span></span>|<span data-ttu-id="b9c11-150">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="b9c11-150">DateTime the object was last modified.</span></span> <span data-ttu-id="b9c11-151">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="b9c11-151">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="b9c11-152">displayName</span><span class="sxs-lookup"><span data-stu-id="b9c11-152">displayName</span></span>|<span data-ttu-id="b9c11-153">String</span><span class="sxs-lookup"><span data-stu-id="b9c11-153">String</span></span>|<span data-ttu-id="b9c11-154">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="b9c11-154">Admin provided name of the device configuration.</span></span> <span data-ttu-id="b9c11-155">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="b9c11-155">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="b9c11-156">version</span><span class="sxs-lookup"><span data-stu-id="b9c11-156">version</span></span>|<span data-ttu-id="b9c11-157">Int32</span><span class="sxs-lookup"><span data-stu-id="b9c11-157">Int32</span></span>|<span data-ttu-id="b9c11-158">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="b9c11-158">Version of the device configuration.</span></span> <span data-ttu-id="b9c11-159">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="b9c11-159">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="b9c11-160">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="b9c11-160">passwordRequired</span></span>|<span data-ttu-id="b9c11-161">布尔值</span><span class="sxs-lookup"><span data-stu-id="b9c11-161">Boolean</span></span>|<span data-ttu-id="b9c11-162">需要密码才可解锁设备。</span><span class="sxs-lookup"><span data-stu-id="b9c11-162">Require a password to unlock device.</span></span>|
|<span data-ttu-id="b9c11-163">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="b9c11-163">passwordMinimumLength</span></span>|<span data-ttu-id="b9c11-164">Int32</span><span class="sxs-lookup"><span data-stu-id="b9c11-164">Int32</span></span>|<span data-ttu-id="b9c11-165">最短密码长度。</span><span class="sxs-lookup"><span data-stu-id="b9c11-165">Minimum password length.</span></span> <span data-ttu-id="b9c11-166">有效值为 4 至 16</span><span class="sxs-lookup"><span data-stu-id="b9c11-166">Valid values 4 to 16</span></span>|
|<span data-ttu-id="b9c11-167">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="b9c11-167">passwordRequiredType</span></span>|[<span data-ttu-id="b9c11-168">androidRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="b9c11-168">androidRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androidrequiredpasswordtype.md)|<span data-ttu-id="b9c11-169">密码中的字符类型。</span><span class="sxs-lookup"><span data-stu-id="b9c11-169">Type of characters in password.</span></span> <span data-ttu-id="b9c11-170">可取值为：`deviceDefault`、`alphabetic`、`alphanumeric`、`alphanumericWithSymbols`、`lowSecurityBiometric`、`numeric`、`numericComplex`、`any`。</span><span class="sxs-lookup"><span data-stu-id="b9c11-170">Possible values are: `deviceDefault`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `numeric`, `numericComplex`, `any`.</span></span>|
|<span data-ttu-id="b9c11-171">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="b9c11-171">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="b9c11-172">Int32</span><span class="sxs-lookup"><span data-stu-id="b9c11-172">Int32</span></span>|<span data-ttu-id="b9c11-173">在需要密码之前不活动的分钟数。</span><span class="sxs-lookup"><span data-stu-id="b9c11-173">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="b9c11-174">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="b9c11-174">passwordExpirationDays</span></span>|<span data-ttu-id="b9c11-175">Int32</span><span class="sxs-lookup"><span data-stu-id="b9c11-175">Int32</span></span>|<span data-ttu-id="b9c11-176">密码过期前的天数。</span><span class="sxs-lookup"><span data-stu-id="b9c11-176">Number of days before the password expires.</span></span> <span data-ttu-id="b9c11-177">有效值为 1 至 365</span><span class="sxs-lookup"><span data-stu-id="b9c11-177">Valid values 1 to 365</span></span>|
|<span data-ttu-id="b9c11-178">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="b9c11-178">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="b9c11-179">Int32</span><span class="sxs-lookup"><span data-stu-id="b9c11-179">Int32</span></span>|<span data-ttu-id="b9c11-180">要阻止的以前密码的数量。</span><span class="sxs-lookup"><span data-stu-id="b9c11-180">Number of previous passwords to block.</span></span> <span data-ttu-id="b9c11-181">有效值为 1 至 24</span><span class="sxs-lookup"><span data-stu-id="b9c11-181">Valid values 1 to 24</span></span>|
|<span data-ttu-id="b9c11-182">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="b9c11-182">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="b9c11-183">Int32</span><span class="sxs-lookup"><span data-stu-id="b9c11-183">Int32</span></span>|<span data-ttu-id="b9c11-184">在恢复出厂设置之前允许的登录失败次数。</span><span class="sxs-lookup"><span data-stu-id="b9c11-184">Number of sign-in failures allowed before factory reset.</span></span> <span data-ttu-id="b9c11-185">有效值为1至16</span><span class="sxs-lookup"><span data-stu-id="b9c11-185">Valid values 1 to 16</span></span>|
|<span data-ttu-id="b9c11-186">securityPreventInstallAppsFromUnknownSources</span><span class="sxs-lookup"><span data-stu-id="b9c11-186">securityPreventInstallAppsFromUnknownSources</span></span>|<span data-ttu-id="b9c11-187">布尔值</span><span class="sxs-lookup"><span data-stu-id="b9c11-187">Boolean</span></span>|<span data-ttu-id="b9c11-188">要求设备不允许安装来自未知源的应用。</span><span class="sxs-lookup"><span data-stu-id="b9c11-188">Require that devices disallow installation of apps from unknown sources.</span></span>|
|<span data-ttu-id="b9c11-189">securityDisableUsbDebugging</span><span class="sxs-lookup"><span data-stu-id="b9c11-189">securityDisableUsbDebugging</span></span>|<span data-ttu-id="b9c11-190">布尔值</span><span class="sxs-lookup"><span data-stu-id="b9c11-190">Boolean</span></span>|<span data-ttu-id="b9c11-191">在 Android 设备上禁用 USB 调试。</span><span class="sxs-lookup"><span data-stu-id="b9c11-191">Disable USB debugging on Android devices.</span></span>|
|<span data-ttu-id="b9c11-192">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="b9c11-192">securityRequireVerifyApps</span></span>|<span data-ttu-id="b9c11-193">布尔值</span><span class="sxs-lookup"><span data-stu-id="b9c11-193">Boolean</span></span>|<span data-ttu-id="b9c11-194">要求启用 Android 验证应用功能。</span><span class="sxs-lookup"><span data-stu-id="b9c11-194">Require the Android Verify apps feature is turned on.</span></span>|
|<span data-ttu-id="b9c11-195">deviceThreatProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="b9c11-195">deviceThreatProtectionEnabled</span></span>|<span data-ttu-id="b9c11-196">布尔值</span><span class="sxs-lookup"><span data-stu-id="b9c11-196">Boolean</span></span>|<span data-ttu-id="b9c11-197">要求设备已启用设备威胁防护。</span><span class="sxs-lookup"><span data-stu-id="b9c11-197">Require that devices have enabled device threat protection.</span></span>|
|<span data-ttu-id="b9c11-198">deviceThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="b9c11-198">deviceThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="b9c11-199">deviceThreatProtectionLevel</span><span class="sxs-lookup"><span data-stu-id="b9c11-199">deviceThreatProtectionLevel</span></span>](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|<span data-ttu-id="b9c11-200">要求移动威胁防护最低风险级别来报告不符合情况。</span><span class="sxs-lookup"><span data-stu-id="b9c11-200">Require Mobile Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="b9c11-201">可取值为：`unavailable`、`secured`、`low`、`medium`、`high`、`notSet`。</span><span class="sxs-lookup"><span data-stu-id="b9c11-201">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="b9c11-202">securityBlockJailbrokenDevices</span><span class="sxs-lookup"><span data-stu-id="b9c11-202">securityBlockJailbrokenDevices</span></span>|<span data-ttu-id="b9c11-203">布尔值</span><span class="sxs-lookup"><span data-stu-id="b9c11-203">Boolean</span></span>|<span data-ttu-id="b9c11-204">设备不得越狱或取得 root 权限。</span><span class="sxs-lookup"><span data-stu-id="b9c11-204">Devices must not be jailbroken or rooted.</span></span>|
|<span data-ttu-id="b9c11-205">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="b9c11-205">osMinimumVersion</span></span>|<span data-ttu-id="b9c11-206">String</span><span class="sxs-lookup"><span data-stu-id="b9c11-206">String</span></span>|<span data-ttu-id="b9c11-207">最低 Android 版本。</span><span class="sxs-lookup"><span data-stu-id="b9c11-207">Minimum Android version.</span></span>|
|<span data-ttu-id="b9c11-208">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="b9c11-208">osMaximumVersion</span></span>|<span data-ttu-id="b9c11-209">String</span><span class="sxs-lookup"><span data-stu-id="b9c11-209">String</span></span>|<span data-ttu-id="b9c11-210">最高 Android 版本。</span><span class="sxs-lookup"><span data-stu-id="b9c11-210">Maximum Android version.</span></span>|
|<span data-ttu-id="b9c11-211">minAndroidSecurityPatchLevel</span><span class="sxs-lookup"><span data-stu-id="b9c11-211">minAndroidSecurityPatchLevel</span></span>|<span data-ttu-id="b9c11-212">String</span><span class="sxs-lookup"><span data-stu-id="b9c11-212">String</span></span>|<span data-ttu-id="b9c11-213">最低 Android 安全修补程序级别。</span><span class="sxs-lookup"><span data-stu-id="b9c11-213">Minimum Android security patch level.</span></span>|
|<span data-ttu-id="b9c11-214">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="b9c11-214">storageRequireEncryption</span></span>|<span data-ttu-id="b9c11-215">布尔值</span><span class="sxs-lookup"><span data-stu-id="b9c11-215">Boolean</span></span>|<span data-ttu-id="b9c11-216">要求对 Android 设备加密。</span><span class="sxs-lookup"><span data-stu-id="b9c11-216">Require encryption on Android devices.</span></span>|
|<span data-ttu-id="b9c11-217">securityRequireSafetyNetAttestationBasicIntegrity</span><span class="sxs-lookup"><span data-stu-id="b9c11-217">securityRequireSafetyNetAttestationBasicIntegrity</span></span>|<span data-ttu-id="b9c11-218">布尔值</span><span class="sxs-lookup"><span data-stu-id="b9c11-218">Boolean</span></span>|<span data-ttu-id="b9c11-219">要求设备传递 SafetyNet 基本完整性检查。</span><span class="sxs-lookup"><span data-stu-id="b9c11-219">Require the device to pass the SafetyNet basic integrity check.</span></span>|
|<span data-ttu-id="b9c11-220">securityRequireSafetyNetAttestationCertifiedDevice</span><span class="sxs-lookup"><span data-stu-id="b9c11-220">securityRequireSafetyNetAttestationCertifiedDevice</span></span>|<span data-ttu-id="b9c11-221">Boolean</span><span class="sxs-lookup"><span data-stu-id="b9c11-221">Boolean</span></span>|<span data-ttu-id="b9c11-222">要求设备传递 SafetyNet 认证设备检查。</span><span class="sxs-lookup"><span data-stu-id="b9c11-222">Require the device to pass the SafetyNet certified device check.</span></span>|
|<span data-ttu-id="b9c11-223">securityRequireGooglePlayServices</span><span class="sxs-lookup"><span data-stu-id="b9c11-223">securityRequireGooglePlayServices</span></span>|<span data-ttu-id="b9c11-224">布尔值</span><span class="sxs-lookup"><span data-stu-id="b9c11-224">Boolean</span></span>|<span data-ttu-id="b9c11-225">要求在设备上安装并启用 Google Play Services。</span><span class="sxs-lookup"><span data-stu-id="b9c11-225">Require Google Play Services to be installed and enabled on the device.</span></span>|
|<span data-ttu-id="b9c11-226">securityRequireUpToDateSecurityProviders</span><span class="sxs-lookup"><span data-stu-id="b9c11-226">securityRequireUpToDateSecurityProviders</span></span>|<span data-ttu-id="b9c11-227">布尔值</span><span class="sxs-lookup"><span data-stu-id="b9c11-227">Boolean</span></span>|<span data-ttu-id="b9c11-228">要求设备具有最新的安全提供程序。</span><span class="sxs-lookup"><span data-stu-id="b9c11-228">Require the device to have up to date security providers.</span></span> <span data-ttu-id="b9c11-229">设备将要求启用 Google Play Services 并保持最新状态。</span><span class="sxs-lookup"><span data-stu-id="b9c11-229">The device will require Google Play Services to be enabled and up to date.</span></span>|
|<span data-ttu-id="b9c11-230">securityRequireCompanyPortalAppIntegrity</span><span class="sxs-lookup"><span data-stu-id="b9c11-230">securityRequireCompanyPortalAppIntegrity</span></span>|<span data-ttu-id="b9c11-231">Boolean</span><span class="sxs-lookup"><span data-stu-id="b9c11-231">Boolean</span></span>|<span data-ttu-id="b9c11-232">要求设备传递公司门户客户端应用运行时完整性检查。</span><span class="sxs-lookup"><span data-stu-id="b9c11-232">Require the device to pass the Company Portal client app runtime integrity check.</span></span>|



## <a name="response"></a><span data-ttu-id="b9c11-233">响应</span><span class="sxs-lookup"><span data-stu-id="b9c11-233">Response</span></span>
<span data-ttu-id="b9c11-234">如果成功, 此方法在响应`200 OK`正文中返回响应代码和更新的[androidForWorkCompliancePolicy](../resources/intune-deviceconfig-androidforworkcompliancepolicy.md)对象。</span><span class="sxs-lookup"><span data-stu-id="b9c11-234">If successful, this method returns a `200 OK` response code and an updated [androidForWorkCompliancePolicy](../resources/intune-deviceconfig-androidforworkcompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b9c11-235">示例</span><span class="sxs-lookup"><span data-stu-id="b9c11-235">Example</span></span>

### <a name="request"></a><span data-ttu-id="b9c11-236">请求</span><span class="sxs-lookup"><span data-stu-id="b9c11-236">Request</span></span>
<span data-ttu-id="b9c11-237">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="b9c11-237">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
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

### <a name="response"></a><span data-ttu-id="b9c11-238">响应</span><span class="sxs-lookup"><span data-stu-id="b9c11-238">Response</span></span>
<span data-ttu-id="b9c11-p116">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="b9c11-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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





