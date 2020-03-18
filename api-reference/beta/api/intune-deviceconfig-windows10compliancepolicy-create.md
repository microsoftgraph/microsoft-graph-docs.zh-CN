---
title: 创建 windows10CompliancePolicy
description: 创建新的 windows10CompliancePolicy 对象。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: cc2e2058e989bcea72d8289a02f6ac494537964e
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42741320"
---
# <a name="create-windows10compliancepolicy"></a><span data-ttu-id="ca364-103">创建 windows10CompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="ca364-103">Create windows10CompliancePolicy</span></span>

> <span data-ttu-id="ca364-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="ca364-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ca364-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="ca364-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ca364-106">创建新的 [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="ca364-106">Create a new [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ca364-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="ca364-107">Prerequisites</span></span>
<span data-ttu-id="ca364-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ca364-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ca364-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="ca364-110">Permission type</span></span>|<span data-ttu-id="ca364-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="ca364-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ca364-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ca364-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ca364-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ca364-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="ca364-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ca364-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ca364-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="ca364-115">Not supported.</span></span>|
|<span data-ttu-id="ca364-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="ca364-116">Application</span></span>|<span data-ttu-id="ca364-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ca364-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ca364-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ca364-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="ca364-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="ca364-119">Request headers</span></span>
|<span data-ttu-id="ca364-120">标头</span><span class="sxs-lookup"><span data-stu-id="ca364-120">Header</span></span>|<span data-ttu-id="ca364-121">值</span><span class="sxs-lookup"><span data-stu-id="ca364-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ca364-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="ca364-122">Authorization</span></span>|<span data-ttu-id="ca364-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="ca364-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ca364-124">接受</span><span class="sxs-lookup"><span data-stu-id="ca364-124">Accept</span></span>|<span data-ttu-id="ca364-125">application/json</span><span class="sxs-lookup"><span data-stu-id="ca364-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ca364-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="ca364-126">Request body</span></span>
<span data-ttu-id="ca364-127">在请求正文中，提供 windows10CompliancePolicy 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ca364-127">In the request body, supply a JSON representation for the windows10CompliancePolicy object.</span></span>

<span data-ttu-id="ca364-128">下表显示创建 windows10CompliancePolicy 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="ca364-128">The following table shows the properties that are required when you create the windows10CompliancePolicy.</span></span>

|<span data-ttu-id="ca364-129">属性</span><span class="sxs-lookup"><span data-stu-id="ca364-129">Property</span></span>|<span data-ttu-id="ca364-130">类型</span><span class="sxs-lookup"><span data-stu-id="ca364-130">Type</span></span>|<span data-ttu-id="ca364-131">说明</span><span class="sxs-lookup"><span data-stu-id="ca364-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ca364-132">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="ca364-132">roleScopeTagIds</span></span>|<span data-ttu-id="ca364-133">String collection</span><span class="sxs-lookup"><span data-stu-id="ca364-133">String collection</span></span>|<span data-ttu-id="ca364-134">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="ca364-134">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="ca364-135">继承自 [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="ca364-135">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="ca364-136">id</span><span class="sxs-lookup"><span data-stu-id="ca364-136">id</span></span>|<span data-ttu-id="ca364-137">字符串</span><span class="sxs-lookup"><span data-stu-id="ca364-137">String</span></span>|<span data-ttu-id="ca364-138">实体的键。</span><span class="sxs-lookup"><span data-stu-id="ca364-138">Key of the entity.</span></span> <span data-ttu-id="ca364-139">继承自 [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="ca364-139">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="ca364-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ca364-140">createdDateTime</span></span>|<span data-ttu-id="ca364-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ca364-141">DateTimeOffset</span></span>|<span data-ttu-id="ca364-142">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="ca364-142">DateTime the object was created.</span></span> <span data-ttu-id="ca364-143">继承自 [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="ca364-143">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="ca364-144">说明</span><span class="sxs-lookup"><span data-stu-id="ca364-144">description</span></span>|<span data-ttu-id="ca364-145">String</span><span class="sxs-lookup"><span data-stu-id="ca364-145">String</span></span>|<span data-ttu-id="ca364-146">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="ca364-146">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="ca364-147">继承自 [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="ca364-147">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="ca364-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ca364-148">lastModifiedDateTime</span></span>|<span data-ttu-id="ca364-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ca364-149">DateTimeOffset</span></span>|<span data-ttu-id="ca364-150">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="ca364-150">DateTime the object was last modified.</span></span> <span data-ttu-id="ca364-151">继承自 [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="ca364-151">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="ca364-152">displayName</span><span class="sxs-lookup"><span data-stu-id="ca364-152">displayName</span></span>|<span data-ttu-id="ca364-153">字符串</span><span class="sxs-lookup"><span data-stu-id="ca364-153">String</span></span>|<span data-ttu-id="ca364-154">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="ca364-154">Admin provided name of the device configuration.</span></span> <span data-ttu-id="ca364-155">继承自 [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="ca364-155">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="ca364-156">version</span><span class="sxs-lookup"><span data-stu-id="ca364-156">version</span></span>|<span data-ttu-id="ca364-157">Int32</span><span class="sxs-lookup"><span data-stu-id="ca364-157">Int32</span></span>|<span data-ttu-id="ca364-158">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="ca364-158">Version of the device configuration.</span></span> <span data-ttu-id="ca364-159">继承自 [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="ca364-159">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="ca364-160">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="ca364-160">passwordRequired</span></span>|<span data-ttu-id="ca364-161">布尔值</span><span class="sxs-lookup"><span data-stu-id="ca364-161">Boolean</span></span>|<span data-ttu-id="ca364-162">需要密码才可解锁 Windows 设备。</span><span class="sxs-lookup"><span data-stu-id="ca364-162">Require a password to unlock Windows device.</span></span>|
|<span data-ttu-id="ca364-163">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="ca364-163">passwordBlockSimple</span></span>|<span data-ttu-id="ca364-164">布尔值</span><span class="sxs-lookup"><span data-stu-id="ca364-164">Boolean</span></span>|<span data-ttu-id="ca364-165">指示是否阻止简单密码。</span><span class="sxs-lookup"><span data-stu-id="ca364-165">Indicates whether or not to block simple password.</span></span>|
|<span data-ttu-id="ca364-166">passwordRequiredToUnlockFromIdle</span><span class="sxs-lookup"><span data-stu-id="ca364-166">passwordRequiredToUnlockFromIdle</span></span>|<span data-ttu-id="ca364-167">布尔值</span><span class="sxs-lookup"><span data-stu-id="ca364-167">Boolean</span></span>|<span data-ttu-id="ca364-168">需要密码才可解锁空闲设备。</span><span class="sxs-lookup"><span data-stu-id="ca364-168">Require a password to unlock an idle device.</span></span>|
|<span data-ttu-id="ca364-169">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="ca364-169">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="ca364-170">Int32</span><span class="sxs-lookup"><span data-stu-id="ca364-170">Int32</span></span>|<span data-ttu-id="ca364-171">在需要密码之前不活动的分钟数。</span><span class="sxs-lookup"><span data-stu-id="ca364-171">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="ca364-172">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="ca364-172">passwordExpirationDays</span></span>|<span data-ttu-id="ca364-173">Int32</span><span class="sxs-lookup"><span data-stu-id="ca364-173">Int32</span></span>|<span data-ttu-id="ca364-174">密码过期天数。</span><span class="sxs-lookup"><span data-stu-id="ca364-174">The password expiration in days.</span></span>|
|<span data-ttu-id="ca364-175">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="ca364-175">passwordMinimumLength</span></span>|<span data-ttu-id="ca364-176">Int32</span><span class="sxs-lookup"><span data-stu-id="ca364-176">Int32</span></span>|<span data-ttu-id="ca364-177">密码最短长度。</span><span class="sxs-lookup"><span data-stu-id="ca364-177">The minimum password length.</span></span>|
|<span data-ttu-id="ca364-178">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="ca364-178">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="ca364-179">Int32</span><span class="sxs-lookup"><span data-stu-id="ca364-179">Int32</span></span>|<span data-ttu-id="ca364-180">密码中必需的字符集数。</span><span class="sxs-lookup"><span data-stu-id="ca364-180">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="ca364-181">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="ca364-181">passwordRequiredType</span></span>|[<span data-ttu-id="ca364-182">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="ca364-182">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="ca364-183">必需的密码类型。</span><span class="sxs-lookup"><span data-stu-id="ca364-183">The required password type.</span></span> <span data-ttu-id="ca364-184">可取值为：`deviceDefault`、`alphanumeric`、`numeric`。</span><span class="sxs-lookup"><span data-stu-id="ca364-184">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="ca364-185">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="ca364-185">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="ca364-186">Int32</span><span class="sxs-lookup"><span data-stu-id="ca364-186">Int32</span></span>|<span data-ttu-id="ca364-187">防止重复使用的先前密码的数量。</span><span class="sxs-lookup"><span data-stu-id="ca364-187">The number of previous passwords to prevent re-use of.</span></span>|
|<span data-ttu-id="ca364-188">requireHealthyDeviceReport</span><span class="sxs-lookup"><span data-stu-id="ca364-188">requireHealthyDeviceReport</span></span>|<span data-ttu-id="ca364-189">布尔值</span><span class="sxs-lookup"><span data-stu-id="ca364-189">Boolean</span></span>|<span data-ttu-id="ca364-190">要求设备由 Windows 设备运行状况证明报告为正常。</span><span class="sxs-lookup"><span data-stu-id="ca364-190">Require devices to be reported as healthy by Windows Device Health Attestation.</span></span>|
|<span data-ttu-id="ca364-191">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="ca364-191">osMinimumVersion</span></span>|<span data-ttu-id="ca364-192">String</span><span class="sxs-lookup"><span data-stu-id="ca364-192">String</span></span>|<span data-ttu-id="ca364-193">最低 Windows 10 版本。</span><span class="sxs-lookup"><span data-stu-id="ca364-193">Minimum Windows 10 version.</span></span>|
|<span data-ttu-id="ca364-194">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="ca364-194">osMaximumVersion</span></span>|<span data-ttu-id="ca364-195">String</span><span class="sxs-lookup"><span data-stu-id="ca364-195">String</span></span>|<span data-ttu-id="ca364-196">最高 Windows 10 版本。</span><span class="sxs-lookup"><span data-stu-id="ca364-196">Maximum Windows 10 version.</span></span>|
|<span data-ttu-id="ca364-197">mobileOsMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="ca364-197">mobileOsMinimumVersion</span></span>|<span data-ttu-id="ca364-198">String</span><span class="sxs-lookup"><span data-stu-id="ca364-198">String</span></span>|<span data-ttu-id="ca364-199">最低 Windows Phone 版本。</span><span class="sxs-lookup"><span data-stu-id="ca364-199">Minimum Windows Phone version.</span></span>|
|<span data-ttu-id="ca364-200">mobileOsMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="ca364-200">mobileOsMaximumVersion</span></span>|<span data-ttu-id="ca364-201">String</span><span class="sxs-lookup"><span data-stu-id="ca364-201">String</span></span>|<span data-ttu-id="ca364-202">最高 Windows Phone 版本。</span><span class="sxs-lookup"><span data-stu-id="ca364-202">Maximum Windows Phone version.</span></span>|
|<span data-ttu-id="ca364-203">earlyLaunchAntiMalwareDriverEnabled</span><span class="sxs-lookup"><span data-stu-id="ca364-203">earlyLaunchAntiMalwareDriverEnabled</span></span>|<span data-ttu-id="ca364-204">布尔值</span><span class="sxs-lookup"><span data-stu-id="ca364-204">Boolean</span></span>|<span data-ttu-id="ca364-205">要求设备由 Windows 设备运行状况证明报告为正常 - 提前启动反恶意驱动程序已启用。</span><span class="sxs-lookup"><span data-stu-id="ca364-205">Require devices to be reported as healthy by Windows Device Health Attestation - early launch antimalware driver is enabled.</span></span>|
|<span data-ttu-id="ca364-206">bitLockerEnabled</span><span class="sxs-lookup"><span data-stu-id="ca364-206">bitLockerEnabled</span></span>|<span data-ttu-id="ca364-207">布尔值</span><span class="sxs-lookup"><span data-stu-id="ca364-207">Boolean</span></span>|<span data-ttu-id="ca364-208">要求设备由 Windows 设备运行状况证明报告为正常 - bit locker 已启用。</span><span class="sxs-lookup"><span data-stu-id="ca364-208">Require devices to be reported healthy by Windows Device Health Attestation - bit locker is enabled</span></span>|
|<span data-ttu-id="ca364-209">secureBootEnabled</span><span class="sxs-lookup"><span data-stu-id="ca364-209">secureBootEnabled</span></span>|<span data-ttu-id="ca364-210">布尔值</span><span class="sxs-lookup"><span data-stu-id="ca364-210">Boolean</span></span>|<span data-ttu-id="ca364-211">要求设备由 Windows 设备运行状况证明报告为正常 - 安全启动已启用。</span><span class="sxs-lookup"><span data-stu-id="ca364-211">Require devices to be reported as healthy by Windows Device Health Attestation - secure boot is enabled.</span></span>|
|<span data-ttu-id="ca364-212">codeIntegrityEnabled</span><span class="sxs-lookup"><span data-stu-id="ca364-212">codeIntegrityEnabled</span></span>|<span data-ttu-id="ca364-213">Boolean</span><span class="sxs-lookup"><span data-stu-id="ca364-213">Boolean</span></span>|<span data-ttu-id="ca364-214">要求设备由 Windows 设备运行状况证明报告为正常。</span><span class="sxs-lookup"><span data-stu-id="ca364-214">Require devices to be reported as healthy by Windows Device Health Attestation.</span></span>|
|<span data-ttu-id="ca364-215">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="ca364-215">storageRequireEncryption</span></span>|<span data-ttu-id="ca364-216">Boolean</span><span class="sxs-lookup"><span data-stu-id="ca364-216">Boolean</span></span>|<span data-ttu-id="ca364-217">要求对 Windows 设备加密。</span><span class="sxs-lookup"><span data-stu-id="ca364-217">Require encryption on windows devices.</span></span>|
|<span data-ttu-id="ca364-218">activeFirewallRequired</span><span class="sxs-lookup"><span data-stu-id="ca364-218">activeFirewallRequired</span></span>|<span data-ttu-id="ca364-219">布尔值</span><span class="sxs-lookup"><span data-stu-id="ca364-219">Boolean</span></span>|<span data-ttu-id="ca364-220">在 Windows 设备上需要活动防火墙。</span><span class="sxs-lookup"><span data-stu-id="ca364-220">Require active firewall on Windows devices.</span></span>|
|<span data-ttu-id="ca364-221">defenderEnabled</span><span class="sxs-lookup"><span data-stu-id="ca364-221">defenderEnabled</span></span>|<span data-ttu-id="ca364-222">布尔值</span><span class="sxs-lookup"><span data-stu-id="ca364-222">Boolean</span></span>|<span data-ttu-id="ca364-223">在 Windows 设备上需要 Windows Defender 反恶意软件。</span><span class="sxs-lookup"><span data-stu-id="ca364-223">Require Windows Defender Antimalware on Windows devices.</span></span>|
|<span data-ttu-id="ca364-224">defenderVersion</span><span class="sxs-lookup"><span data-stu-id="ca364-224">defenderVersion</span></span>|<span data-ttu-id="ca364-225">String</span><span class="sxs-lookup"><span data-stu-id="ca364-225">String</span></span>|<span data-ttu-id="ca364-226">在 Windows 设备上要求 Windows Defender 反恶意软件的最低版本。</span><span class="sxs-lookup"><span data-stu-id="ca364-226">Require Windows Defender Antimalware minimum version on Windows devices.</span></span>|
|<span data-ttu-id="ca364-227">signatureOutOfDate</span><span class="sxs-lookup"><span data-stu-id="ca364-227">signatureOutOfDate</span></span>|<span data-ttu-id="ca364-228">布尔值</span><span class="sxs-lookup"><span data-stu-id="ca364-228">Boolean</span></span>|<span data-ttu-id="ca364-229">Windows 设备上要求 Windows Defender 反恶意软件签名为最新。</span><span class="sxs-lookup"><span data-stu-id="ca364-229">Require Windows Defender Antimalware Signature to be up to date on Windows devices.</span></span>|
|<span data-ttu-id="ca364-230">rtpEnabled</span><span class="sxs-lookup"><span data-stu-id="ca364-230">rtpEnabled</span></span>|<span data-ttu-id="ca364-231">布尔值</span><span class="sxs-lookup"><span data-stu-id="ca364-231">Boolean</span></span>|<span data-ttu-id="ca364-232">在 Windows 设备上需要 Windows Defender 反恶意软件实时保护。</span><span class="sxs-lookup"><span data-stu-id="ca364-232">Require Windows Defender Antimalware Real-Time Protection on Windows devices.</span></span>|
|<span data-ttu-id="ca364-233">antivirusRequired</span><span class="sxs-lookup"><span data-stu-id="ca364-233">antivirusRequired</span></span>|<span data-ttu-id="ca364-234">布尔值</span><span class="sxs-lookup"><span data-stu-id="ca364-234">Boolean</span></span>|<span data-ttu-id="ca364-235">要求在 Windows Decurity Center 中注册的任何防病毒解决方案都处于启用和监控（例如，Symantec、Windows Defender）。</span><span class="sxs-lookup"><span data-stu-id="ca364-235">Require any Antivirus solution registered with Windows Decurity Center to be on and monitoring (e.g. Symantec, Windows Defender).</span></span>|
|<span data-ttu-id="ca364-236">antiSpywareRequired</span><span class="sxs-lookup"><span data-stu-id="ca364-236">antiSpywareRequired</span></span>|<span data-ttu-id="ca364-237">布尔值</span><span class="sxs-lookup"><span data-stu-id="ca364-237">Boolean</span></span>|<span data-ttu-id="ca364-238">要求在 Windows Decurity Center 中注册的任何反间谍软件解决方案都处于启用和监控（例如，Symantec、Windows Defender）。</span><span class="sxs-lookup"><span data-stu-id="ca364-238">Require any AntiSpyware solution registered with Windows Decurity Center to be on and monitoring (e.g. Symantec, Windows Defender).</span></span>|
|<span data-ttu-id="ca364-239">validOperatingSystemBuildRanges</span><span class="sxs-lookup"><span data-stu-id="ca364-239">validOperatingSystemBuildRanges</span></span>|<span data-ttu-id="ca364-240">[operatingSystemVersionRange](../resources/intune-deviceconfig-operatingsystemversionrange.md)集合</span><span class="sxs-lookup"><span data-stu-id="ca364-240">[operatingSystemVersionRange](../resources/intune-deviceconfig-operatingsystemversionrange.md) collection</span></span>|<span data-ttu-id="ca364-241">Windows 设备上的有效操作系统内部版本范围。</span><span class="sxs-lookup"><span data-stu-id="ca364-241">The valid operating system build ranges on Windows devices.</span></span> <span data-ttu-id="ca364-242">该集合最多可包含 10000 个元素。</span><span class="sxs-lookup"><span data-stu-id="ca364-242">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="ca364-243">deviceThreatProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="ca364-243">deviceThreatProtectionEnabled</span></span>|<span data-ttu-id="ca364-244">Boolean</span><span class="sxs-lookup"><span data-stu-id="ca364-244">Boolean</span></span>|<span data-ttu-id="ca364-245">要求设备已启用设备威胁防护。</span><span class="sxs-lookup"><span data-stu-id="ca364-245">Require that devices have enabled device threat protection.</span></span>|
|<span data-ttu-id="ca364-246">deviceThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="ca364-246">deviceThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="ca364-247">deviceThreatProtectionLevel</span><span class="sxs-lookup"><span data-stu-id="ca364-247">deviceThreatProtectionLevel</span></span>](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|<span data-ttu-id="ca364-248">需要设备威胁防护最低风险级别来报告不合规。</span><span class="sxs-lookup"><span data-stu-id="ca364-248">Require Device Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="ca364-249">可取值为：`unavailable`、`secured`、`low`、`medium`、`high`、`notSet`。</span><span class="sxs-lookup"><span data-stu-id="ca364-249">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="ca364-250">configurationManagerComplianceRequired</span><span class="sxs-lookup"><span data-stu-id="ca364-250">configurationManagerComplianceRequired</span></span>|<span data-ttu-id="ca364-251">布尔值</span><span class="sxs-lookup"><span data-stu-id="ca364-251">Boolean</span></span>|<span data-ttu-id="ca364-252">需要考虑将 SCCM 合规性状态考虑到 Intune 合规性状态。</span><span class="sxs-lookup"><span data-stu-id="ca364-252">Require to consider SCCM Compliance state into consideration for Intune Compliance State.</span></span>|
|<span data-ttu-id="ca364-253">tpmRequired</span><span class="sxs-lookup"><span data-stu-id="ca364-253">tpmRequired</span></span>|<span data-ttu-id="ca364-254">布尔值</span><span class="sxs-lookup"><span data-stu-id="ca364-254">Boolean</span></span>|<span data-ttu-id="ca364-255">要求存在受信任的平台模块（TPM）。</span><span class="sxs-lookup"><span data-stu-id="ca364-255">Require Trusted Platform Module(TPM) to be present.</span></span>|



## <a name="response"></a><span data-ttu-id="ca364-256">响应</span><span class="sxs-lookup"><span data-stu-id="ca364-256">Response</span></span>
<span data-ttu-id="ca364-257">如果成功，此方法会在响应正文中返回 `201 Created` 响应代码和 [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="ca364-257">If successful, this method returns a `201 Created` response code and a [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ca364-258">示例</span><span class="sxs-lookup"><span data-stu-id="ca364-258">Example</span></span>

### <a name="request"></a><span data-ttu-id="ca364-259">请求</span><span class="sxs-lookup"><span data-stu-id="ca364-259">Request</span></span>
<span data-ttu-id="ca364-260">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="ca364-260">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies
Content-type: application/json
Content-length: 1690

{
  "@odata.type": "#microsoft.graph.windows10CompliancePolicy",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "passwordRequired": true,
  "passwordBlockSimple": true,
  "passwordRequiredToUnlockFromIdle": true,
  "passwordMinutesOfInactivityBeforeLock": 5,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinimumCharacterSetCount": 0,
  "passwordRequiredType": "alphanumeric",
  "passwordPreviousPasswordBlockCount": 2,
  "requireHealthyDeviceReport": true,
  "osMinimumVersion": "Os Minimum Version value",
  "osMaximumVersion": "Os Maximum Version value",
  "mobileOsMinimumVersion": "Mobile Os Minimum Version value",
  "mobileOsMaximumVersion": "Mobile Os Maximum Version value",
  "earlyLaunchAntiMalwareDriverEnabled": true,
  "bitLockerEnabled": true,
  "secureBootEnabled": true,
  "codeIntegrityEnabled": true,
  "storageRequireEncryption": true,
  "activeFirewallRequired": true,
  "defenderEnabled": true,
  "defenderVersion": "Defender Version value",
  "signatureOutOfDate": true,
  "rtpEnabled": true,
  "antivirusRequired": true,
  "antiSpywareRequired": true,
  "validOperatingSystemBuildRanges": [
    {
      "@odata.type": "microsoft.graph.operatingSystemVersionRange",
      "description": "Description value",
      "lowestVersion": "Lowest Version value",
      "highestVersion": "Highest Version value"
    }
  ],
  "deviceThreatProtectionEnabled": true,
  "deviceThreatProtectionRequiredSecurityLevel": "secured",
  "configurationManagerComplianceRequired": true,
  "tpmRequired": true
}
```

### <a name="response"></a><span data-ttu-id="ca364-261">响应</span><span class="sxs-lookup"><span data-stu-id="ca364-261">Response</span></span>
<span data-ttu-id="ca364-p112">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="ca364-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1862

{
  "@odata.type": "#microsoft.graph.windows10CompliancePolicy",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "id": "2919ae62-ae62-2919-62ae-192962ae1929",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "version": 7,
  "passwordRequired": true,
  "passwordBlockSimple": true,
  "passwordRequiredToUnlockFromIdle": true,
  "passwordMinutesOfInactivityBeforeLock": 5,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinimumCharacterSetCount": 0,
  "passwordRequiredType": "alphanumeric",
  "passwordPreviousPasswordBlockCount": 2,
  "requireHealthyDeviceReport": true,
  "osMinimumVersion": "Os Minimum Version value",
  "osMaximumVersion": "Os Maximum Version value",
  "mobileOsMinimumVersion": "Mobile Os Minimum Version value",
  "mobileOsMaximumVersion": "Mobile Os Maximum Version value",
  "earlyLaunchAntiMalwareDriverEnabled": true,
  "bitLockerEnabled": true,
  "secureBootEnabled": true,
  "codeIntegrityEnabled": true,
  "storageRequireEncryption": true,
  "activeFirewallRequired": true,
  "defenderEnabled": true,
  "defenderVersion": "Defender Version value",
  "signatureOutOfDate": true,
  "rtpEnabled": true,
  "antivirusRequired": true,
  "antiSpywareRequired": true,
  "validOperatingSystemBuildRanges": [
    {
      "@odata.type": "microsoft.graph.operatingSystemVersionRange",
      "description": "Description value",
      "lowestVersion": "Lowest Version value",
      "highestVersion": "Highest Version value"
    }
  ],
  "deviceThreatProtectionEnabled": true,
  "deviceThreatProtectionRequiredSecurityLevel": "secured",
  "configurationManagerComplianceRequired": true,
  "tpmRequired": true
}
```




