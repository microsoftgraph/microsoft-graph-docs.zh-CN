---
title: 更新 windows10CompliancePolicy
description: 更新 windows10CompliancePolicy 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: b95a86d88d693e34e79f8c59a8d905db9b95ee33
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/18/2020
ms.locfileid: "44792616"
---
# <a name="update-windows10compliancepolicy"></a><span data-ttu-id="42351-103">更新 windows10CompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="42351-103">Update windows10CompliancePolicy</span></span>

<span data-ttu-id="42351-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="42351-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="42351-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="42351-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="42351-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="42351-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="42351-107">更新 [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="42351-107">Update the properties of a [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="42351-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="42351-108">Prerequisites</span></span>
<span data-ttu-id="42351-109">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="42351-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="42351-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="42351-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="42351-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="42351-111">Permission type</span></span>|<span data-ttu-id="42351-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="42351-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="42351-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="42351-113">Delegated (work or school account)</span></span>|<span data-ttu-id="42351-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="42351-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="42351-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="42351-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="42351-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="42351-116">Not supported.</span></span>|
|<span data-ttu-id="42351-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="42351-117">Application</span></span>|<span data-ttu-id="42351-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="42351-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="42351-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="42351-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="42351-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="42351-120">Request headers</span></span>
|<span data-ttu-id="42351-121">标头</span><span class="sxs-lookup"><span data-stu-id="42351-121">Header</span></span>|<span data-ttu-id="42351-122">值</span><span class="sxs-lookup"><span data-stu-id="42351-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="42351-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="42351-123">Authorization</span></span>|<span data-ttu-id="42351-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="42351-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="42351-125">接受</span><span class="sxs-lookup"><span data-stu-id="42351-125">Accept</span></span>|<span data-ttu-id="42351-126">application/json</span><span class="sxs-lookup"><span data-stu-id="42351-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="42351-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="42351-127">Request body</span></span>
<span data-ttu-id="42351-128">在请求正文中，提供 [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="42351-128">In the request body, supply a JSON representation for the [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) object.</span></span>

<span data-ttu-id="42351-129">下表显示创建 [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="42351-129">The following table shows the properties that are required when you create the [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md).</span></span>

|<span data-ttu-id="42351-130">属性</span><span class="sxs-lookup"><span data-stu-id="42351-130">Property</span></span>|<span data-ttu-id="42351-131">类型</span><span class="sxs-lookup"><span data-stu-id="42351-131">Type</span></span>|<span data-ttu-id="42351-132">说明</span><span class="sxs-lookup"><span data-stu-id="42351-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="42351-133">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="42351-133">roleScopeTagIds</span></span>|<span data-ttu-id="42351-134">String collection</span><span class="sxs-lookup"><span data-stu-id="42351-134">String collection</span></span>|<span data-ttu-id="42351-135">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="42351-135">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="42351-136">继承自 [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="42351-136">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="42351-137">id</span><span class="sxs-lookup"><span data-stu-id="42351-137">id</span></span>|<span data-ttu-id="42351-138">字符串</span><span class="sxs-lookup"><span data-stu-id="42351-138">String</span></span>|<span data-ttu-id="42351-139">实体的键。</span><span class="sxs-lookup"><span data-stu-id="42351-139">Key of the entity.</span></span> <span data-ttu-id="42351-140">继承自 [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="42351-140">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="42351-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="42351-141">createdDateTime</span></span>|<span data-ttu-id="42351-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="42351-142">DateTimeOffset</span></span>|<span data-ttu-id="42351-143">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="42351-143">DateTime the object was created.</span></span> <span data-ttu-id="42351-144">继承自 [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="42351-144">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="42351-145">说明</span><span class="sxs-lookup"><span data-stu-id="42351-145">description</span></span>|<span data-ttu-id="42351-146">String</span><span class="sxs-lookup"><span data-stu-id="42351-146">String</span></span>|<span data-ttu-id="42351-147">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="42351-147">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="42351-148">继承自 [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="42351-148">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="42351-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="42351-149">lastModifiedDateTime</span></span>|<span data-ttu-id="42351-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="42351-150">DateTimeOffset</span></span>|<span data-ttu-id="42351-151">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="42351-151">DateTime the object was last modified.</span></span> <span data-ttu-id="42351-152">继承自 [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="42351-152">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="42351-153">displayName</span><span class="sxs-lookup"><span data-stu-id="42351-153">displayName</span></span>|<span data-ttu-id="42351-154">字符串</span><span class="sxs-lookup"><span data-stu-id="42351-154">String</span></span>|<span data-ttu-id="42351-155">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="42351-155">Admin provided name of the device configuration.</span></span> <span data-ttu-id="42351-156">继承自 [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="42351-156">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="42351-157">version</span><span class="sxs-lookup"><span data-stu-id="42351-157">version</span></span>|<span data-ttu-id="42351-158">Int32</span><span class="sxs-lookup"><span data-stu-id="42351-158">Int32</span></span>|<span data-ttu-id="42351-159">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="42351-159">Version of the device configuration.</span></span> <span data-ttu-id="42351-160">继承自 [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="42351-160">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="42351-161">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="42351-161">passwordRequired</span></span>|<span data-ttu-id="42351-162">布尔值</span><span class="sxs-lookup"><span data-stu-id="42351-162">Boolean</span></span>|<span data-ttu-id="42351-163">需要密码才可解锁 Windows 设备。</span><span class="sxs-lookup"><span data-stu-id="42351-163">Require a password to unlock Windows device.</span></span>|
|<span data-ttu-id="42351-164">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="42351-164">passwordBlockSimple</span></span>|<span data-ttu-id="42351-165">布尔值</span><span class="sxs-lookup"><span data-stu-id="42351-165">Boolean</span></span>|<span data-ttu-id="42351-166">指示是否阻止简单密码。</span><span class="sxs-lookup"><span data-stu-id="42351-166">Indicates whether or not to block simple password.</span></span>|
|<span data-ttu-id="42351-167">passwordRequiredToUnlockFromIdle</span><span class="sxs-lookup"><span data-stu-id="42351-167">passwordRequiredToUnlockFromIdle</span></span>|<span data-ttu-id="42351-168">布尔值</span><span class="sxs-lookup"><span data-stu-id="42351-168">Boolean</span></span>|<span data-ttu-id="42351-169">需要密码才可解锁空闲设备。</span><span class="sxs-lookup"><span data-stu-id="42351-169">Require a password to unlock an idle device.</span></span>|
|<span data-ttu-id="42351-170">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="42351-170">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="42351-171">Int32</span><span class="sxs-lookup"><span data-stu-id="42351-171">Int32</span></span>|<span data-ttu-id="42351-172">在需要密码之前不活动的分钟数。</span><span class="sxs-lookup"><span data-stu-id="42351-172">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="42351-173">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="42351-173">passwordExpirationDays</span></span>|<span data-ttu-id="42351-174">Int32</span><span class="sxs-lookup"><span data-stu-id="42351-174">Int32</span></span>|<span data-ttu-id="42351-175">密码过期天数。</span><span class="sxs-lookup"><span data-stu-id="42351-175">The password expiration in days.</span></span>|
|<span data-ttu-id="42351-176">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="42351-176">passwordMinimumLength</span></span>|<span data-ttu-id="42351-177">Int32</span><span class="sxs-lookup"><span data-stu-id="42351-177">Int32</span></span>|<span data-ttu-id="42351-178">密码最短长度。</span><span class="sxs-lookup"><span data-stu-id="42351-178">The minimum password length.</span></span>|
|<span data-ttu-id="42351-179">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="42351-179">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="42351-180">Int32</span><span class="sxs-lookup"><span data-stu-id="42351-180">Int32</span></span>|<span data-ttu-id="42351-181">密码中必需的字符集数。</span><span class="sxs-lookup"><span data-stu-id="42351-181">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="42351-182">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="42351-182">passwordRequiredType</span></span>|[<span data-ttu-id="42351-183">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="42351-183">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="42351-184">必需的密码类型。</span><span class="sxs-lookup"><span data-stu-id="42351-184">The required password type.</span></span> <span data-ttu-id="42351-185">可取值为：`deviceDefault`、`alphanumeric`、`numeric`。</span><span class="sxs-lookup"><span data-stu-id="42351-185">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="42351-186">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="42351-186">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="42351-187">Int32</span><span class="sxs-lookup"><span data-stu-id="42351-187">Int32</span></span>|<span data-ttu-id="42351-188">防止重复使用的先前密码的数量。</span><span class="sxs-lookup"><span data-stu-id="42351-188">The number of previous passwords to prevent re-use of.</span></span>|
|<span data-ttu-id="42351-189">requireHealthyDeviceReport</span><span class="sxs-lookup"><span data-stu-id="42351-189">requireHealthyDeviceReport</span></span>|<span data-ttu-id="42351-190">布尔值</span><span class="sxs-lookup"><span data-stu-id="42351-190">Boolean</span></span>|<span data-ttu-id="42351-191">要求设备由 Windows 设备运行状况证明报告为正常。</span><span class="sxs-lookup"><span data-stu-id="42351-191">Require devices to be reported as healthy by Windows Device Health Attestation.</span></span>|
|<span data-ttu-id="42351-192">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="42351-192">osMinimumVersion</span></span>|<span data-ttu-id="42351-193">String</span><span class="sxs-lookup"><span data-stu-id="42351-193">String</span></span>|<span data-ttu-id="42351-194">最低 Windows 10 版本。</span><span class="sxs-lookup"><span data-stu-id="42351-194">Minimum Windows 10 version.</span></span>|
|<span data-ttu-id="42351-195">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="42351-195">osMaximumVersion</span></span>|<span data-ttu-id="42351-196">String</span><span class="sxs-lookup"><span data-stu-id="42351-196">String</span></span>|<span data-ttu-id="42351-197">最高 Windows 10 版本。</span><span class="sxs-lookup"><span data-stu-id="42351-197">Maximum Windows 10 version.</span></span>|
|<span data-ttu-id="42351-198">mobileOsMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="42351-198">mobileOsMinimumVersion</span></span>|<span data-ttu-id="42351-199">String</span><span class="sxs-lookup"><span data-stu-id="42351-199">String</span></span>|<span data-ttu-id="42351-200">最低 Windows Phone 版本。</span><span class="sxs-lookup"><span data-stu-id="42351-200">Minimum Windows Phone version.</span></span>|
|<span data-ttu-id="42351-201">mobileOsMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="42351-201">mobileOsMaximumVersion</span></span>|<span data-ttu-id="42351-202">String</span><span class="sxs-lookup"><span data-stu-id="42351-202">String</span></span>|<span data-ttu-id="42351-203">最高 Windows Phone 版本。</span><span class="sxs-lookup"><span data-stu-id="42351-203">Maximum Windows Phone version.</span></span>|
|<span data-ttu-id="42351-204">earlyLaunchAntiMalwareDriverEnabled</span><span class="sxs-lookup"><span data-stu-id="42351-204">earlyLaunchAntiMalwareDriverEnabled</span></span>|<span data-ttu-id="42351-205">布尔值</span><span class="sxs-lookup"><span data-stu-id="42351-205">Boolean</span></span>|<span data-ttu-id="42351-206">要求设备由 Windows 设备运行状况证明报告为正常 - 提前启动反恶意驱动程序已启用。</span><span class="sxs-lookup"><span data-stu-id="42351-206">Require devices to be reported as healthy by Windows Device Health Attestation - early launch antimalware driver is enabled.</span></span>|
|<span data-ttu-id="42351-207">bitLockerEnabled</span><span class="sxs-lookup"><span data-stu-id="42351-207">bitLockerEnabled</span></span>|<span data-ttu-id="42351-208">布尔值</span><span class="sxs-lookup"><span data-stu-id="42351-208">Boolean</span></span>|<span data-ttu-id="42351-209">要求设备由 Windows 设备运行状况证明报告为正常 - bit locker 已启用。</span><span class="sxs-lookup"><span data-stu-id="42351-209">Require devices to be reported healthy by Windows Device Health Attestation - bit locker is enabled</span></span>|
|<span data-ttu-id="42351-210">secureBootEnabled</span><span class="sxs-lookup"><span data-stu-id="42351-210">secureBootEnabled</span></span>|<span data-ttu-id="42351-211">布尔值</span><span class="sxs-lookup"><span data-stu-id="42351-211">Boolean</span></span>|<span data-ttu-id="42351-212">要求设备由 Windows 设备运行状况证明报告为正常 - 安全启动已启用。</span><span class="sxs-lookup"><span data-stu-id="42351-212">Require devices to be reported as healthy by Windows Device Health Attestation - secure boot is enabled.</span></span>|
|<span data-ttu-id="42351-213">codeIntegrityEnabled</span><span class="sxs-lookup"><span data-stu-id="42351-213">codeIntegrityEnabled</span></span>|<span data-ttu-id="42351-214">Boolean</span><span class="sxs-lookup"><span data-stu-id="42351-214">Boolean</span></span>|<span data-ttu-id="42351-215">要求设备由 Windows 设备运行状况证明报告为正常。</span><span class="sxs-lookup"><span data-stu-id="42351-215">Require devices to be reported as healthy by Windows Device Health Attestation.</span></span>|
|<span data-ttu-id="42351-216">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="42351-216">storageRequireEncryption</span></span>|<span data-ttu-id="42351-217">Boolean</span><span class="sxs-lookup"><span data-stu-id="42351-217">Boolean</span></span>|<span data-ttu-id="42351-218">要求对 Windows 设备加密。</span><span class="sxs-lookup"><span data-stu-id="42351-218">Require encryption on windows devices.</span></span>|
|<span data-ttu-id="42351-219">activeFirewallRequired</span><span class="sxs-lookup"><span data-stu-id="42351-219">activeFirewallRequired</span></span>|<span data-ttu-id="42351-220">布尔值</span><span class="sxs-lookup"><span data-stu-id="42351-220">Boolean</span></span>|<span data-ttu-id="42351-221">在 Windows 设备上需要活动防火墙。</span><span class="sxs-lookup"><span data-stu-id="42351-221">Require active firewall on Windows devices.</span></span>|
|<span data-ttu-id="42351-222">defenderEnabled</span><span class="sxs-lookup"><span data-stu-id="42351-222">defenderEnabled</span></span>|<span data-ttu-id="42351-223">布尔值</span><span class="sxs-lookup"><span data-stu-id="42351-223">Boolean</span></span>|<span data-ttu-id="42351-224">在 Windows 设备上需要 Windows Defender 反恶意软件。</span><span class="sxs-lookup"><span data-stu-id="42351-224">Require Windows Defender Antimalware on Windows devices.</span></span>|
|<span data-ttu-id="42351-225">defenderVersion</span><span class="sxs-lookup"><span data-stu-id="42351-225">defenderVersion</span></span>|<span data-ttu-id="42351-226">String</span><span class="sxs-lookup"><span data-stu-id="42351-226">String</span></span>|<span data-ttu-id="42351-227">在 Windows 设备上要求 Windows Defender 反恶意软件的最低版本。</span><span class="sxs-lookup"><span data-stu-id="42351-227">Require Windows Defender Antimalware minimum version on Windows devices.</span></span>|
|<span data-ttu-id="42351-228">signatureOutOfDate</span><span class="sxs-lookup"><span data-stu-id="42351-228">signatureOutOfDate</span></span>|<span data-ttu-id="42351-229">布尔值</span><span class="sxs-lookup"><span data-stu-id="42351-229">Boolean</span></span>|<span data-ttu-id="42351-230">Windows 设备上要求 Windows Defender 反恶意软件签名为最新。</span><span class="sxs-lookup"><span data-stu-id="42351-230">Require Windows Defender Antimalware Signature to be up to date on Windows devices.</span></span>|
|<span data-ttu-id="42351-231">rtpEnabled</span><span class="sxs-lookup"><span data-stu-id="42351-231">rtpEnabled</span></span>|<span data-ttu-id="42351-232">布尔值</span><span class="sxs-lookup"><span data-stu-id="42351-232">Boolean</span></span>|<span data-ttu-id="42351-233">在 Windows 设备上需要 Windows Defender 反恶意软件实时保护。</span><span class="sxs-lookup"><span data-stu-id="42351-233">Require Windows Defender Antimalware Real-Time Protection on Windows devices.</span></span>|
|<span data-ttu-id="42351-234">antivirusRequired</span><span class="sxs-lookup"><span data-stu-id="42351-234">antivirusRequired</span></span>|<span data-ttu-id="42351-235">布尔值</span><span class="sxs-lookup"><span data-stu-id="42351-235">Boolean</span></span>|<span data-ttu-id="42351-236">要求在 Windows Decurity Center 中注册的任何防病毒解决方案都处于启用和监控（例如，Symantec、Windows Defender）。</span><span class="sxs-lookup"><span data-stu-id="42351-236">Require any Antivirus solution registered with Windows Decurity Center to be on and monitoring (e.g. Symantec, Windows Defender).</span></span>|
|<span data-ttu-id="42351-237">antiSpywareRequired</span><span class="sxs-lookup"><span data-stu-id="42351-237">antiSpywareRequired</span></span>|<span data-ttu-id="42351-238">布尔值</span><span class="sxs-lookup"><span data-stu-id="42351-238">Boolean</span></span>|<span data-ttu-id="42351-239">要求在 Windows Decurity Center 中注册的任何反间谍软件解决方案都处于启用和监控（例如，Symantec、Windows Defender）。</span><span class="sxs-lookup"><span data-stu-id="42351-239">Require any AntiSpyware solution registered with Windows Decurity Center to be on and monitoring (e.g. Symantec, Windows Defender).</span></span>|
|<span data-ttu-id="42351-240">validOperatingSystemBuildRanges</span><span class="sxs-lookup"><span data-stu-id="42351-240">validOperatingSystemBuildRanges</span></span>|<span data-ttu-id="42351-241">[operatingSystemVersionRange](../resources/intune-deviceconfig-operatingsystemversionrange.md)集合</span><span class="sxs-lookup"><span data-stu-id="42351-241">[operatingSystemVersionRange](../resources/intune-deviceconfig-operatingsystemversionrange.md) collection</span></span>|<span data-ttu-id="42351-242">Windows 设备上的有效操作系统内部版本范围。</span><span class="sxs-lookup"><span data-stu-id="42351-242">The valid operating system build ranges on Windows devices.</span></span> <span data-ttu-id="42351-243">该集合最多可包含 10000 个元素。</span><span class="sxs-lookup"><span data-stu-id="42351-243">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="42351-244">deviceThreatProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="42351-244">deviceThreatProtectionEnabled</span></span>|<span data-ttu-id="42351-245">Boolean</span><span class="sxs-lookup"><span data-stu-id="42351-245">Boolean</span></span>|<span data-ttu-id="42351-246">要求设备已启用设备威胁防护。</span><span class="sxs-lookup"><span data-stu-id="42351-246">Require that devices have enabled device threat protection.</span></span>|
|<span data-ttu-id="42351-247">deviceThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="42351-247">deviceThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="42351-248">deviceThreatProtectionLevel</span><span class="sxs-lookup"><span data-stu-id="42351-248">deviceThreatProtectionLevel</span></span>](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|<span data-ttu-id="42351-249">需要设备威胁防护最低风险级别来报告不合规。</span><span class="sxs-lookup"><span data-stu-id="42351-249">Require Device Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="42351-250">可取值为：`unavailable`、`secured`、`low`、`medium`、`high`、`notSet`。</span><span class="sxs-lookup"><span data-stu-id="42351-250">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="42351-251">configurationManagerComplianceRequired</span><span class="sxs-lookup"><span data-stu-id="42351-251">configurationManagerComplianceRequired</span></span>|<span data-ttu-id="42351-252">布尔值</span><span class="sxs-lookup"><span data-stu-id="42351-252">Boolean</span></span>|<span data-ttu-id="42351-253">需要考虑将 SCCM 合规性状态考虑到 Intune 合规性状态。</span><span class="sxs-lookup"><span data-stu-id="42351-253">Require to consider SCCM Compliance state into consideration for Intune Compliance State.</span></span>|
|<span data-ttu-id="42351-254">tpmRequired</span><span class="sxs-lookup"><span data-stu-id="42351-254">tpmRequired</span></span>|<span data-ttu-id="42351-255">布尔值</span><span class="sxs-lookup"><span data-stu-id="42351-255">Boolean</span></span>|<span data-ttu-id="42351-256">要求存在受信任的平台模块（TPM）。</span><span class="sxs-lookup"><span data-stu-id="42351-256">Require Trusted Platform Module(TPM) to be present.</span></span>|
|<span data-ttu-id="42351-257">deviceCompliancePolicyScript</span><span class="sxs-lookup"><span data-stu-id="42351-257">deviceCompliancePolicyScript</span></span>|[<span data-ttu-id="42351-258">deviceCompliancePolicyScript</span><span class="sxs-lookup"><span data-stu-id="42351-258">deviceCompliancePolicyScript</span></span>](../resources/intune-deviceconfig-devicecompliancepolicyscript.md)|<span data-ttu-id="42351-259">尚未记录</span><span class="sxs-lookup"><span data-stu-id="42351-259">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="42351-260">响应</span><span class="sxs-lookup"><span data-stu-id="42351-260">Response</span></span>
<span data-ttu-id="42351-261">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和更新的 [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="42351-261">If successful, this method returns a `200 OK` response code and an updated [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="42351-262">示例</span><span class="sxs-lookup"><span data-stu-id="42351-262">Example</span></span>

### <a name="request"></a><span data-ttu-id="42351-263">请求</span><span class="sxs-lookup"><span data-stu-id="42351-263">Request</span></span>
<span data-ttu-id="42351-264">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="42351-264">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
Content-type: application/json
Content-length: 1911

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
  "tpmRequired": true,
  "deviceCompliancePolicyScript": {
    "@odata.type": "microsoft.graph.deviceCompliancePolicyScript",
    "deviceComplianceScriptId": "Device Compliance Script Id value",
    "rulesContent": "cnVsZXNDb250ZW50"
  }
}
```

### <a name="response"></a><span data-ttu-id="42351-265">响应</span><span class="sxs-lookup"><span data-stu-id="42351-265">Response</span></span>
<span data-ttu-id="42351-266">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="42351-266">Here is an example of the response.</span></span> <span data-ttu-id="42351-267">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="42351-267">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="42351-268">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="42351-268">All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2083

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
  "tpmRequired": true,
  "deviceCompliancePolicyScript": {
    "@odata.type": "microsoft.graph.deviceCompliancePolicyScript",
    "deviceComplianceScriptId": "Device Compliance Script Id value",
    "rulesContent": "cnVsZXNDb250ZW50"
  }
}
```



