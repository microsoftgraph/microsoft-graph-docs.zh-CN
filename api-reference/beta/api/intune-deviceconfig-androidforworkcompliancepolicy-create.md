---
title: 创建 androidForWorkCompliancePolicy
description: 创建新的 androidForWorkCompliancePolicy 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: ac3affaf984f252e51bcdcf8490dd8294217a6d5
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/26/2021
ms.locfileid: "52665502"
---
# <a name="create-androidforworkcompliancepolicy"></a><span data-ttu-id="55eb3-103">创建 androidForWorkCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="55eb3-103">Create androidForWorkCompliancePolicy</span></span>

<span data-ttu-id="55eb3-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="55eb3-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="55eb3-105">**重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="55eb3-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="55eb3-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="55eb3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="55eb3-107">创建新的 [androidForWorkCompliancePolicy](../resources/intune-deviceconfig-androidforworkcompliancepolicy.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="55eb3-107">Create a new [androidForWorkCompliancePolicy](../resources/intune-deviceconfig-androidforworkcompliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="55eb3-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="55eb3-108">Prerequisites</span></span>
<span data-ttu-id="55eb3-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="55eb3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="55eb3-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="55eb3-111">Permission type</span></span>|<span data-ttu-id="55eb3-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="55eb3-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="55eb3-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="55eb3-113">Delegated (work or school account)</span></span>|<span data-ttu-id="55eb3-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="55eb3-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="55eb3-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="55eb3-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="55eb3-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="55eb3-116">Not supported.</span></span>|
|<span data-ttu-id="55eb3-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="55eb3-117">Application</span></span>|<span data-ttu-id="55eb3-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="55eb3-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="55eb3-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="55eb3-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="55eb3-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="55eb3-120">Request headers</span></span>
|<span data-ttu-id="55eb3-121">标头</span><span class="sxs-lookup"><span data-stu-id="55eb3-121">Header</span></span>|<span data-ttu-id="55eb3-122">值</span><span class="sxs-lookup"><span data-stu-id="55eb3-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="55eb3-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="55eb3-123">Authorization</span></span>|<span data-ttu-id="55eb3-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="55eb3-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="55eb3-125">接受</span><span class="sxs-lookup"><span data-stu-id="55eb3-125">Accept</span></span>|<span data-ttu-id="55eb3-126">application/json</span><span class="sxs-lookup"><span data-stu-id="55eb3-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="55eb3-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="55eb3-127">Request body</span></span>
<span data-ttu-id="55eb3-128">在请求正文中，提供 androidForWorkCompliancePolicy 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="55eb3-128">In the request body, supply a JSON representation for the androidForWorkCompliancePolicy object.</span></span>

<span data-ttu-id="55eb3-129">下表显示创建 androidForWorkCompliancePolicy 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="55eb3-129">The following table shows the properties that are required when you create the androidForWorkCompliancePolicy.</span></span>

|<span data-ttu-id="55eb3-130">属性</span><span class="sxs-lookup"><span data-stu-id="55eb3-130">Property</span></span>|<span data-ttu-id="55eb3-131">类型</span><span class="sxs-lookup"><span data-stu-id="55eb3-131">Type</span></span>|<span data-ttu-id="55eb3-132">说明</span><span class="sxs-lookup"><span data-stu-id="55eb3-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="55eb3-133">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="55eb3-133">roleScopeTagIds</span></span>|<span data-ttu-id="55eb3-134">String collection</span><span class="sxs-lookup"><span data-stu-id="55eb3-134">String collection</span></span>|<span data-ttu-id="55eb3-135">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="55eb3-135">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="55eb3-136">继承自 [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="55eb3-136">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="55eb3-137">id</span><span class="sxs-lookup"><span data-stu-id="55eb3-137">id</span></span>|<span data-ttu-id="55eb3-138">String</span><span class="sxs-lookup"><span data-stu-id="55eb3-138">String</span></span>|<span data-ttu-id="55eb3-139">实体的键。</span><span class="sxs-lookup"><span data-stu-id="55eb3-139">Key of the entity.</span></span> <span data-ttu-id="55eb3-140">继承自 [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="55eb3-140">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="55eb3-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="55eb3-141">createdDateTime</span></span>|<span data-ttu-id="55eb3-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="55eb3-142">DateTimeOffset</span></span>|<span data-ttu-id="55eb3-143">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="55eb3-143">DateTime the object was created.</span></span> <span data-ttu-id="55eb3-144">继承自 [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="55eb3-144">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="55eb3-145">说明</span><span class="sxs-lookup"><span data-stu-id="55eb3-145">description</span></span>|<span data-ttu-id="55eb3-146">String</span><span class="sxs-lookup"><span data-stu-id="55eb3-146">String</span></span>|<span data-ttu-id="55eb3-147">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="55eb3-147">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="55eb3-148">继承自 [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="55eb3-148">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="55eb3-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="55eb3-149">lastModifiedDateTime</span></span>|<span data-ttu-id="55eb3-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="55eb3-150">DateTimeOffset</span></span>|<span data-ttu-id="55eb3-151">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="55eb3-151">DateTime the object was last modified.</span></span> <span data-ttu-id="55eb3-152">继承自 [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="55eb3-152">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="55eb3-153">displayName</span><span class="sxs-lookup"><span data-stu-id="55eb3-153">displayName</span></span>|<span data-ttu-id="55eb3-154">String</span><span class="sxs-lookup"><span data-stu-id="55eb3-154">String</span></span>|<span data-ttu-id="55eb3-155">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="55eb3-155">Admin provided name of the device configuration.</span></span> <span data-ttu-id="55eb3-156">继承自 [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="55eb3-156">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="55eb3-157">version</span><span class="sxs-lookup"><span data-stu-id="55eb3-157">version</span></span>|<span data-ttu-id="55eb3-158">Int32</span><span class="sxs-lookup"><span data-stu-id="55eb3-158">Int32</span></span>|<span data-ttu-id="55eb3-159">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="55eb3-159">Version of the device configuration.</span></span> <span data-ttu-id="55eb3-160">继承自 [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="55eb3-160">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="55eb3-161">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="55eb3-161">passwordRequired</span></span>|<span data-ttu-id="55eb3-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="55eb3-162">Boolean</span></span>|<span data-ttu-id="55eb3-163">需要密码才可解锁设备。</span><span class="sxs-lookup"><span data-stu-id="55eb3-163">Require a password to unlock device.</span></span>|
|<span data-ttu-id="55eb3-164">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="55eb3-164">passwordMinimumLength</span></span>|<span data-ttu-id="55eb3-165">Int32</span><span class="sxs-lookup"><span data-stu-id="55eb3-165">Int32</span></span>|<span data-ttu-id="55eb3-166">最短密码长度。</span><span class="sxs-lookup"><span data-stu-id="55eb3-166">Minimum password length.</span></span> <span data-ttu-id="55eb3-167">有效值为 4 至 16</span><span class="sxs-lookup"><span data-stu-id="55eb3-167">Valid values 4 to 16</span></span>|
|<span data-ttu-id="55eb3-168">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="55eb3-168">passwordRequiredType</span></span>|[<span data-ttu-id="55eb3-169">androidRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="55eb3-169">androidRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androidrequiredpasswordtype.md)|<span data-ttu-id="55eb3-170">密码中的字符类型。</span><span class="sxs-lookup"><span data-stu-id="55eb3-170">Type of characters in password.</span></span> <span data-ttu-id="55eb3-171">可取值为：`deviceDefault`、`alphabetic`、`alphanumeric`、`alphanumericWithSymbols`、`lowSecurityBiometric`、`numeric`、`numericComplex`、`any`。</span><span class="sxs-lookup"><span data-stu-id="55eb3-171">Possible values are: `deviceDefault`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `numeric`, `numericComplex`, `any`.</span></span>|
|<span data-ttu-id="55eb3-172">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="55eb3-172">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="55eb3-173">Int32</span><span class="sxs-lookup"><span data-stu-id="55eb3-173">Int32</span></span>|<span data-ttu-id="55eb3-174">在需要密码之前不活动的分钟数。</span><span class="sxs-lookup"><span data-stu-id="55eb3-174">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="55eb3-175">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="55eb3-175">passwordExpirationDays</span></span>|<span data-ttu-id="55eb3-176">Int32</span><span class="sxs-lookup"><span data-stu-id="55eb3-176">Int32</span></span>|<span data-ttu-id="55eb3-177">密码过期前的天数。</span><span class="sxs-lookup"><span data-stu-id="55eb3-177">Number of days before the password expires.</span></span> <span data-ttu-id="55eb3-178">有效值为 1 至 365</span><span class="sxs-lookup"><span data-stu-id="55eb3-178">Valid values 1 to 365</span></span>|
|<span data-ttu-id="55eb3-179">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="55eb3-179">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="55eb3-180">Int32</span><span class="sxs-lookup"><span data-stu-id="55eb3-180">Int32</span></span>|<span data-ttu-id="55eb3-181">要阻止的以前密码的数量。</span><span class="sxs-lookup"><span data-stu-id="55eb3-181">Number of previous passwords to block.</span></span> <span data-ttu-id="55eb3-182">有效值为 1 至 24</span><span class="sxs-lookup"><span data-stu-id="55eb3-182">Valid values 1 to 24</span></span>|
|<span data-ttu-id="55eb3-183">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="55eb3-183">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="55eb3-184">Int32</span><span class="sxs-lookup"><span data-stu-id="55eb3-184">Int32</span></span>|<span data-ttu-id="55eb3-185">恢复出厂设置之前允许的登录失败次数。</span><span class="sxs-lookup"><span data-stu-id="55eb3-185">Number of sign-in failures allowed before factory reset.</span></span> <span data-ttu-id="55eb3-186">有效值为 1 到 16</span><span class="sxs-lookup"><span data-stu-id="55eb3-186">Valid values 1 to 16</span></span>|
|<span data-ttu-id="55eb3-187">securityPreventInstallAppsFromUnknownSources</span><span class="sxs-lookup"><span data-stu-id="55eb3-187">securityPreventInstallAppsFromUnknownSources</span></span>|<span data-ttu-id="55eb3-188">Boolean</span><span class="sxs-lookup"><span data-stu-id="55eb3-188">Boolean</span></span>|<span data-ttu-id="55eb3-189">要求设备不允许安装来自未知源的应用。</span><span class="sxs-lookup"><span data-stu-id="55eb3-189">Require that devices disallow installation of apps from unknown sources.</span></span>|
|<span data-ttu-id="55eb3-190">securityDisableUsbDebugging</span><span class="sxs-lookup"><span data-stu-id="55eb3-190">securityDisableUsbDebugging</span></span>|<span data-ttu-id="55eb3-191">Boolean</span><span class="sxs-lookup"><span data-stu-id="55eb3-191">Boolean</span></span>|<span data-ttu-id="55eb3-192">在 Android 设备上禁用 USB 调试。</span><span class="sxs-lookup"><span data-stu-id="55eb3-192">Disable USB debugging on Android devices.</span></span>|
|<span data-ttu-id="55eb3-193">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="55eb3-193">securityRequireVerifyApps</span></span>|<span data-ttu-id="55eb3-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="55eb3-194">Boolean</span></span>|<span data-ttu-id="55eb3-195">要求启用 Android 验证应用功能。</span><span class="sxs-lookup"><span data-stu-id="55eb3-195">Require the Android Verify apps feature is turned on.</span></span>|
|<span data-ttu-id="55eb3-196">deviceThreatProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="55eb3-196">deviceThreatProtectionEnabled</span></span>|<span data-ttu-id="55eb3-197">Boolean</span><span class="sxs-lookup"><span data-stu-id="55eb3-197">Boolean</span></span>|<span data-ttu-id="55eb3-198">要求设备已启用设备威胁防护。</span><span class="sxs-lookup"><span data-stu-id="55eb3-198">Require that devices have enabled device threat protection.</span></span>|
|<span data-ttu-id="55eb3-199">deviceThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="55eb3-199">deviceThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="55eb3-200">deviceThreatProtectionLevel</span><span class="sxs-lookup"><span data-stu-id="55eb3-200">deviceThreatProtectionLevel</span></span>](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|<span data-ttu-id="55eb3-201">要求移动威胁防护最低风险级别来报告不符合情况。</span><span class="sxs-lookup"><span data-stu-id="55eb3-201">Require Mobile Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="55eb3-202">可取值为：`unavailable`、`secured`、`low`、`medium`、`high`、`notSet`。</span><span class="sxs-lookup"><span data-stu-id="55eb3-202">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="55eb3-203">securityBlockJailbrokenDevices</span><span class="sxs-lookup"><span data-stu-id="55eb3-203">securityBlockJailbrokenDevices</span></span>|<span data-ttu-id="55eb3-204">Boolean</span><span class="sxs-lookup"><span data-stu-id="55eb3-204">Boolean</span></span>|<span data-ttu-id="55eb3-205">设备不得越狱或取得 root 权限。</span><span class="sxs-lookup"><span data-stu-id="55eb3-205">Devices must not be jailbroken or rooted.</span></span>|
|<span data-ttu-id="55eb3-206">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="55eb3-206">osMinimumVersion</span></span>|<span data-ttu-id="55eb3-207">String</span><span class="sxs-lookup"><span data-stu-id="55eb3-207">String</span></span>|<span data-ttu-id="55eb3-208">最低 Android 版本。</span><span class="sxs-lookup"><span data-stu-id="55eb3-208">Minimum Android version.</span></span>|
|<span data-ttu-id="55eb3-209">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="55eb3-209">osMaximumVersion</span></span>|<span data-ttu-id="55eb3-210">String</span><span class="sxs-lookup"><span data-stu-id="55eb3-210">String</span></span>|<span data-ttu-id="55eb3-211">最高 Android 版本。</span><span class="sxs-lookup"><span data-stu-id="55eb3-211">Maximum Android version.</span></span>|
|<span data-ttu-id="55eb3-212">minAndroidSecurityPatchLevel</span><span class="sxs-lookup"><span data-stu-id="55eb3-212">minAndroidSecurityPatchLevel</span></span>|<span data-ttu-id="55eb3-213">String</span><span class="sxs-lookup"><span data-stu-id="55eb3-213">String</span></span>|<span data-ttu-id="55eb3-214">最低 Android 安全修补程序级别。</span><span class="sxs-lookup"><span data-stu-id="55eb3-214">Minimum Android security patch level.</span></span>|
|<span data-ttu-id="55eb3-215">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="55eb3-215">storageRequireEncryption</span></span>|<span data-ttu-id="55eb3-216">Boolean</span><span class="sxs-lookup"><span data-stu-id="55eb3-216">Boolean</span></span>|<span data-ttu-id="55eb3-217">要求对 Android 设备加密。</span><span class="sxs-lookup"><span data-stu-id="55eb3-217">Require encryption on Android devices.</span></span>|
|<span data-ttu-id="55eb3-218">securityRequireSafetyNetAttestationBasicIntegrity</span><span class="sxs-lookup"><span data-stu-id="55eb3-218">securityRequireSafetyNetAttestationBasicIntegrity</span></span>|<span data-ttu-id="55eb3-219">Boolean</span><span class="sxs-lookup"><span data-stu-id="55eb3-219">Boolean</span></span>|<span data-ttu-id="55eb3-220">要求设备传递 SafetyNet 基本完整性检查。</span><span class="sxs-lookup"><span data-stu-id="55eb3-220">Require the device to pass the SafetyNet basic integrity check.</span></span>|
|<span data-ttu-id="55eb3-221">securityRequireSafetyNetAttestationCertifiedDevice</span><span class="sxs-lookup"><span data-stu-id="55eb3-221">securityRequireSafetyNetAttestationCertifiedDevice</span></span>|<span data-ttu-id="55eb3-222">Boolean</span><span class="sxs-lookup"><span data-stu-id="55eb3-222">Boolean</span></span>|<span data-ttu-id="55eb3-223">要求设备传递 SafetyNet 认证设备检查。</span><span class="sxs-lookup"><span data-stu-id="55eb3-223">Require the device to pass the SafetyNet certified device check.</span></span>|
|<span data-ttu-id="55eb3-224">securityRequireGooglePlayServices</span><span class="sxs-lookup"><span data-stu-id="55eb3-224">securityRequireGooglePlayServices</span></span>|<span data-ttu-id="55eb3-225">Boolean</span><span class="sxs-lookup"><span data-stu-id="55eb3-225">Boolean</span></span>|<span data-ttu-id="55eb3-226">要求在设备上安装并启用 Google Play Services。</span><span class="sxs-lookup"><span data-stu-id="55eb3-226">Require Google Play Services to be installed and enabled on the device.</span></span>|
|<span data-ttu-id="55eb3-227">securityRequireUpToDateSecurityProviders</span><span class="sxs-lookup"><span data-stu-id="55eb3-227">securityRequireUpToDateSecurityProviders</span></span>|<span data-ttu-id="55eb3-228">Boolean</span><span class="sxs-lookup"><span data-stu-id="55eb3-228">Boolean</span></span>|<span data-ttu-id="55eb3-229">要求设备具有最新的安全提供程序。</span><span class="sxs-lookup"><span data-stu-id="55eb3-229">Require the device to have up to date security providers.</span></span> <span data-ttu-id="55eb3-230">设备将要求启用 Google Play Services 并保持最新状态。</span><span class="sxs-lookup"><span data-stu-id="55eb3-230">The device will require Google Play Services to be enabled and up to date.</span></span>|
|<span data-ttu-id="55eb3-231">securityRequireCompanyPortalAppIntegrity</span><span class="sxs-lookup"><span data-stu-id="55eb3-231">securityRequireCompanyPortalAppIntegrity</span></span>|<span data-ttu-id="55eb3-232">Boolean</span><span class="sxs-lookup"><span data-stu-id="55eb3-232">Boolean</span></span>|<span data-ttu-id="55eb3-233">要求设备传递公司门户客户端应用运行时完整性检查。</span><span class="sxs-lookup"><span data-stu-id="55eb3-233">Require the device to pass the Company Portal client app runtime integrity check.</span></span>|
|<span data-ttu-id="55eb3-234">securityRequiredAndroidSafetyNetEvaluationType</span><span class="sxs-lookup"><span data-stu-id="55eb3-234">securityRequiredAndroidSafetyNetEvaluationType</span></span>|[<span data-ttu-id="55eb3-235">androidSafetyNetEvaluationType</span><span class="sxs-lookup"><span data-stu-id="55eb3-235">androidSafetyNetEvaluationType</span></span>](../resources/intune-deviceconfig-androidsafetynetevaluationtype.md)|<span data-ttu-id="55eb3-236">要求特定的 SafetyNet 评估类型满足合规性要求。</span><span class="sxs-lookup"><span data-stu-id="55eb3-236">Require a specific SafetyNet evaluation type for compliance.</span></span> <span data-ttu-id="55eb3-237">可取值为：`basic`、`hardwareBacked`。</span><span class="sxs-lookup"><span data-stu-id="55eb3-237">Possible values are: `basic`, `hardwareBacked`.</span></span>|



## <a name="response"></a><span data-ttu-id="55eb3-238">响应</span><span class="sxs-lookup"><span data-stu-id="55eb3-238">Response</span></span>
<span data-ttu-id="55eb3-239">如果成功，此方法在响应 `201 Created` 正文中返回 响应代码和 [androidForWorkCompliancePolicy](../resources/intune-deviceconfig-androidforworkcompliancepolicy.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="55eb3-239">If successful, this method returns a `201 Created` response code and a [androidForWorkCompliancePolicy](../resources/intune-deviceconfig-androidforworkcompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="55eb3-240">示例</span><span class="sxs-lookup"><span data-stu-id="55eb3-240">Example</span></span>

### <a name="request"></a><span data-ttu-id="55eb3-241">请求</span><span class="sxs-lookup"><span data-stu-id="55eb3-241">Request</span></span>
<span data-ttu-id="55eb3-242">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="55eb3-242">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies
Content-type: application/json
Content-length: 1354

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
  "securityRequireCompanyPortalAppIntegrity": true,
  "securityRequiredAndroidSafetyNetEvaluationType": "hardwareBacked"
}
```

### <a name="response"></a><span data-ttu-id="55eb3-243">响应</span><span class="sxs-lookup"><span data-stu-id="55eb3-243">Response</span></span>
<span data-ttu-id="55eb3-p117">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="55eb3-p117">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1526

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
  "securityRequireCompanyPortalAppIntegrity": true,
  "securityRequiredAndroidSafetyNetEvaluationType": "hardwareBacked"
}
```




