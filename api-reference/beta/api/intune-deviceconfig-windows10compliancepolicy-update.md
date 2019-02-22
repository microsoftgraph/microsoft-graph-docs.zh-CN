---
title: 更新 windows10CompliancePolicy
description: 更新 windows10CompliancePolicy 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d4d24c0d964fd43e12c4fcd9a3ff91a0bcd1238b
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30172266"
---
# <a name="update-windows10compliancepolicy"></a><span data-ttu-id="56a86-103">更新 windows10CompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="56a86-103">Update windows10CompliancePolicy</span></span>

> <span data-ttu-id="56a86-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="56a86-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="56a86-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="56a86-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="56a86-106">更新 [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="56a86-106">Update the properties of a [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="56a86-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="56a86-107">Prerequisites</span></span>
<span data-ttu-id="56a86-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="56a86-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="56a86-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="56a86-110">Permission type</span></span>|<span data-ttu-id="56a86-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="56a86-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="56a86-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="56a86-112">Delegated (work or school account)</span></span>|<span data-ttu-id="56a86-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="56a86-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="56a86-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="56a86-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="56a86-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="56a86-115">Not supported.</span></span>|
|<span data-ttu-id="56a86-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="56a86-116">Application</span></span>|<span data-ttu-id="56a86-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="56a86-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="56a86-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="56a86-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="56a86-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="56a86-119">Request headers</span></span>
|<span data-ttu-id="56a86-120">标头</span><span class="sxs-lookup"><span data-stu-id="56a86-120">Header</span></span>|<span data-ttu-id="56a86-121">值</span><span class="sxs-lookup"><span data-stu-id="56a86-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="56a86-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="56a86-122">Authorization</span></span>|<span data-ttu-id="56a86-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="56a86-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="56a86-124">Accept</span><span class="sxs-lookup"><span data-stu-id="56a86-124">Accept</span></span>|<span data-ttu-id="56a86-125">application/json</span><span class="sxs-lookup"><span data-stu-id="56a86-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="56a86-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="56a86-126">Request body</span></span>
<span data-ttu-id="56a86-127">在请求正文中，提供 [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="56a86-127">In the request body, supply a JSON representation for the [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) object.</span></span>

<span data-ttu-id="56a86-128">下表显示创建 [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="56a86-128">The following table shows the properties that are required when you create the [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md).</span></span>

|<span data-ttu-id="56a86-129">属性</span><span class="sxs-lookup"><span data-stu-id="56a86-129">Property</span></span>|<span data-ttu-id="56a86-130">类型</span><span class="sxs-lookup"><span data-stu-id="56a86-130">Type</span></span>|<span data-ttu-id="56a86-131">说明</span><span class="sxs-lookup"><span data-stu-id="56a86-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="56a86-132">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="56a86-132">roleScopeTagIds</span></span>|<span data-ttu-id="56a86-133">String collection</span><span class="sxs-lookup"><span data-stu-id="56a86-133">String collection</span></span>|<span data-ttu-id="56a86-134">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="56a86-134">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="56a86-135">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="56a86-135">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="56a86-136">id</span><span class="sxs-lookup"><span data-stu-id="56a86-136">id</span></span>|<span data-ttu-id="56a86-137">字串符号</span><span class="sxs-lookup"><span data-stu-id="56a86-137">String</span></span>|<span data-ttu-id="56a86-138">实体的键。</span><span class="sxs-lookup"><span data-stu-id="56a86-138">Key of the entity.</span></span> <span data-ttu-id="56a86-139">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="56a86-139">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="56a86-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="56a86-140">createdDateTime</span></span>|<span data-ttu-id="56a86-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="56a86-141">DateTimeOffset</span></span>|<span data-ttu-id="56a86-142">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="56a86-142">DateTime the object was created.</span></span> <span data-ttu-id="56a86-143">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="56a86-143">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="56a86-144">description</span><span class="sxs-lookup"><span data-stu-id="56a86-144">description</span></span>|<span data-ttu-id="56a86-145">字符串</span><span class="sxs-lookup"><span data-stu-id="56a86-145">String</span></span>|<span data-ttu-id="56a86-146">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="56a86-146">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="56a86-147">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="56a86-147">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="56a86-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="56a86-148">lastModifiedDateTime</span></span>|<span data-ttu-id="56a86-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="56a86-149">DateTimeOffset</span></span>|<span data-ttu-id="56a86-150">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="56a86-150">DateTime the object was last modified.</span></span> <span data-ttu-id="56a86-151">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="56a86-151">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="56a86-152">displayName</span><span class="sxs-lookup"><span data-stu-id="56a86-152">displayName</span></span>|<span data-ttu-id="56a86-153">字符串</span><span class="sxs-lookup"><span data-stu-id="56a86-153">String</span></span>|<span data-ttu-id="56a86-154">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="56a86-154">Admin provided name of the device configuration.</span></span> <span data-ttu-id="56a86-155">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="56a86-155">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="56a86-156">version</span><span class="sxs-lookup"><span data-stu-id="56a86-156">version</span></span>|<span data-ttu-id="56a86-157">Int32</span><span class="sxs-lookup"><span data-stu-id="56a86-157">Int32</span></span>|<span data-ttu-id="56a86-158">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="56a86-158">Version of the device configuration.</span></span> <span data-ttu-id="56a86-159">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="56a86-159">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="56a86-160">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="56a86-160">passwordRequired</span></span>|<span data-ttu-id="56a86-161">布尔</span><span class="sxs-lookup"><span data-stu-id="56a86-161">Boolean</span></span>|<span data-ttu-id="56a86-162">需要密码才可解锁 Windows 设备。</span><span class="sxs-lookup"><span data-stu-id="56a86-162">Require a password to unlock Windows device.</span></span>|
|<span data-ttu-id="56a86-163">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="56a86-163">passwordBlockSimple</span></span>|<span data-ttu-id="56a86-164">Boolean</span><span class="sxs-lookup"><span data-stu-id="56a86-164">Boolean</span></span>|<span data-ttu-id="56a86-165">指示是否阻止简单密码。</span><span class="sxs-lookup"><span data-stu-id="56a86-165">Indicates whether or not to block simple password.</span></span>|
|<span data-ttu-id="56a86-166">passwordRequiredToUnlockFromIdle</span><span class="sxs-lookup"><span data-stu-id="56a86-166">passwordRequiredToUnlockFromIdle</span></span>|<span data-ttu-id="56a86-167">布尔</span><span class="sxs-lookup"><span data-stu-id="56a86-167">Boolean</span></span>|<span data-ttu-id="56a86-168">需要密码才可解锁空闲设备。</span><span class="sxs-lookup"><span data-stu-id="56a86-168">Require a password to unlock an idle device.</span></span>|
|<span data-ttu-id="56a86-169">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="56a86-169">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="56a86-170">Int32</span><span class="sxs-lookup"><span data-stu-id="56a86-170">Int32</span></span>|<span data-ttu-id="56a86-171">在需要密码之前不活动的分钟数。</span><span class="sxs-lookup"><span data-stu-id="56a86-171">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="56a86-172">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="56a86-172">passwordExpirationDays</span></span>|<span data-ttu-id="56a86-173">Int32</span><span class="sxs-lookup"><span data-stu-id="56a86-173">Int32</span></span>|<span data-ttu-id="56a86-174">密码过期天数。</span><span class="sxs-lookup"><span data-stu-id="56a86-174">The password expiration in days.</span></span>|
|<span data-ttu-id="56a86-175">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="56a86-175">passwordMinimumLength</span></span>|<span data-ttu-id="56a86-176">Int32</span><span class="sxs-lookup"><span data-stu-id="56a86-176">Int32</span></span>|<span data-ttu-id="56a86-177">密码最短长度。</span><span class="sxs-lookup"><span data-stu-id="56a86-177">The minimum password length.</span></span>|
|<span data-ttu-id="56a86-178">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="56a86-178">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="56a86-179">Int32</span><span class="sxs-lookup"><span data-stu-id="56a86-179">Int32</span></span>|<span data-ttu-id="56a86-180">密码中必需的字符集数。</span><span class="sxs-lookup"><span data-stu-id="56a86-180">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="56a86-181">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="56a86-181">passwordRequiredType</span></span>|[<span data-ttu-id="56a86-182">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="56a86-182">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="56a86-183">必需的密码类型。</span><span class="sxs-lookup"><span data-stu-id="56a86-183">The required password type.</span></span> <span data-ttu-id="56a86-184">可取值为：`deviceDefault`、`alphanumeric`、`numeric`。</span><span class="sxs-lookup"><span data-stu-id="56a86-184">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="56a86-185">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="56a86-185">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="56a86-186">Int32</span><span class="sxs-lookup"><span data-stu-id="56a86-186">Int32</span></span>|<span data-ttu-id="56a86-187">防止重复使用的先前密码的数量。</span><span class="sxs-lookup"><span data-stu-id="56a86-187">The number of previous passwords to prevent re-use of.</span></span>|
|<span data-ttu-id="56a86-188">requireHealthyDeviceReport</span><span class="sxs-lookup"><span data-stu-id="56a86-188">requireHealthyDeviceReport</span></span>|<span data-ttu-id="56a86-189">Boolean</span><span class="sxs-lookup"><span data-stu-id="56a86-189">Boolean</span></span>|<span data-ttu-id="56a86-190">要求设备由 Windows 设备运行状况证明报告为正常。</span><span class="sxs-lookup"><span data-stu-id="56a86-190">Require devices to be reported as healthy by Windows Device Health Attestation.</span></span>|
|<span data-ttu-id="56a86-191">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="56a86-191">osMinimumVersion</span></span>|<span data-ttu-id="56a86-192">String</span><span class="sxs-lookup"><span data-stu-id="56a86-192">String</span></span>|<span data-ttu-id="56a86-193">最低 Windows 10 版本。</span><span class="sxs-lookup"><span data-stu-id="56a86-193">Minimum Windows 10 version.</span></span>|
|<span data-ttu-id="56a86-194">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="56a86-194">osMaximumVersion</span></span>|<span data-ttu-id="56a86-195">String</span><span class="sxs-lookup"><span data-stu-id="56a86-195">String</span></span>|<span data-ttu-id="56a86-196">最高 Windows 10 版本。</span><span class="sxs-lookup"><span data-stu-id="56a86-196">Maximum Windows 10 version.</span></span>|
|<span data-ttu-id="56a86-197">mobileOsMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="56a86-197">mobileOsMinimumVersion</span></span>|<span data-ttu-id="56a86-198">String</span><span class="sxs-lookup"><span data-stu-id="56a86-198">String</span></span>|<span data-ttu-id="56a86-199">最低 Windows Phone 版本。</span><span class="sxs-lookup"><span data-stu-id="56a86-199">Minimum Windows Phone version.</span></span>|
|<span data-ttu-id="56a86-200">mobileOsMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="56a86-200">mobileOsMaximumVersion</span></span>|<span data-ttu-id="56a86-201">String</span><span class="sxs-lookup"><span data-stu-id="56a86-201">String</span></span>|<span data-ttu-id="56a86-202">最高 Windows Phone 版本。</span><span class="sxs-lookup"><span data-stu-id="56a86-202">Maximum Windows Phone version.</span></span>|
|<span data-ttu-id="56a86-203">earlyLaunchAntiMalwareDriverEnabled</span><span class="sxs-lookup"><span data-stu-id="56a86-203">earlyLaunchAntiMalwareDriverEnabled</span></span>|<span data-ttu-id="56a86-204">布尔</span><span class="sxs-lookup"><span data-stu-id="56a86-204">Boolean</span></span>|<span data-ttu-id="56a86-205">要求设备由 Windows 设备运行状况证明报告为正常 - 提前启动反恶意驱动程序已启用。</span><span class="sxs-lookup"><span data-stu-id="56a86-205">Require devices to be reported as healthy by Windows Device Health Attestation - early launch antimalware driver is enabled.</span></span>|
|<span data-ttu-id="56a86-206">bitLockerEnabled</span><span class="sxs-lookup"><span data-stu-id="56a86-206">bitLockerEnabled</span></span>|<span data-ttu-id="56a86-207">布尔</span><span class="sxs-lookup"><span data-stu-id="56a86-207">Boolean</span></span>|<span data-ttu-id="56a86-208">要求设备由 Windows 设备运行状况证明报告为正常 - bit locker 已启用。</span><span class="sxs-lookup"><span data-stu-id="56a86-208">Require devices to be reported healthy by Windows Device Health Attestation - bit locker is enabled</span></span>|
|<span data-ttu-id="56a86-209">secureBootEnabled</span><span class="sxs-lookup"><span data-stu-id="56a86-209">secureBootEnabled</span></span>|<span data-ttu-id="56a86-210">布尔</span><span class="sxs-lookup"><span data-stu-id="56a86-210">Boolean</span></span>|<span data-ttu-id="56a86-211">要求设备由 Windows 设备运行状况证明报告为正常 - 安全启动已启用。</span><span class="sxs-lookup"><span data-stu-id="56a86-211">Require devices to be reported as healthy by Windows Device Health Attestation - secure boot is enabled.</span></span>|
|<span data-ttu-id="56a86-212">codeIntegrityEnabled</span><span class="sxs-lookup"><span data-stu-id="56a86-212">codeIntegrityEnabled</span></span>|<span data-ttu-id="56a86-213">Boolean</span><span class="sxs-lookup"><span data-stu-id="56a86-213">Boolean</span></span>|<span data-ttu-id="56a86-214">要求设备由 Windows 设备运行状况证明报告为正常。</span><span class="sxs-lookup"><span data-stu-id="56a86-214">Require devices to be reported as healthy by Windows Device Health Attestation.</span></span>|
|<span data-ttu-id="56a86-215">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="56a86-215">storageRequireEncryption</span></span>|<span data-ttu-id="56a86-216">布尔</span><span class="sxs-lookup"><span data-stu-id="56a86-216">Boolean</span></span>|<span data-ttu-id="56a86-217">要求对 Windows 设备加密。</span><span class="sxs-lookup"><span data-stu-id="56a86-217">Require encryption on windows devices.</span></span>|
|<span data-ttu-id="56a86-218">activeFirewallRequired</span><span class="sxs-lookup"><span data-stu-id="56a86-218">activeFirewallRequired</span></span>|<span data-ttu-id="56a86-219">布尔</span><span class="sxs-lookup"><span data-stu-id="56a86-219">Boolean</span></span>|<span data-ttu-id="56a86-220">在 Windows 设备上需要活动防火墙。</span><span class="sxs-lookup"><span data-stu-id="56a86-220">Require active firewall on Windows devices.</span></span>|
|<span data-ttu-id="56a86-221">defenderEnabled</span><span class="sxs-lookup"><span data-stu-id="56a86-221">defenderEnabled</span></span>|<span data-ttu-id="56a86-222">布尔</span><span class="sxs-lookup"><span data-stu-id="56a86-222">Boolean</span></span>|<span data-ttu-id="56a86-223">在 windows 设备上需要 windows Defender 反恶意软件。</span><span class="sxs-lookup"><span data-stu-id="56a86-223">Require Windows Defender Antimalware on Windows devices.</span></span>|
|<span data-ttu-id="56a86-224">defenderVersion</span><span class="sxs-lookup"><span data-stu-id="56a86-224">defenderVersion</span></span>|<span data-ttu-id="56a86-225">字符串</span><span class="sxs-lookup"><span data-stu-id="56a86-225">String</span></span>|<span data-ttu-id="56a86-226">在 windows 设备上要求 windows Defender 反恶意软件的最低版本。</span><span class="sxs-lookup"><span data-stu-id="56a86-226">Require Windows Defender Antimalware minimum version on Windows devices.</span></span>|
|<span data-ttu-id="56a86-227">signatureOutOfDate</span><span class="sxs-lookup"><span data-stu-id="56a86-227">signatureOutOfDate</span></span>|<span data-ttu-id="56a86-228">布尔</span><span class="sxs-lookup"><span data-stu-id="56a86-228">Boolean</span></span>|<span data-ttu-id="56a86-229">windows 设备上要求 windows Defender 反恶意软件签名为最新。</span><span class="sxs-lookup"><span data-stu-id="56a86-229">Require Windows Defender Antimalware Signature to be up to date on Windows devices.</span></span>|
|<span data-ttu-id="56a86-230">rtpEnabled</span><span class="sxs-lookup"><span data-stu-id="56a86-230">rtpEnabled</span></span>|<span data-ttu-id="56a86-231">布尔</span><span class="sxs-lookup"><span data-stu-id="56a86-231">Boolean</span></span>|<span data-ttu-id="56a86-232">在 windows 设备上需要 windows Defender 反恶意软件实时保护。</span><span class="sxs-lookup"><span data-stu-id="56a86-232">Require Windows Defender Antimalware Real-Time Protection on Windows devices.</span></span>|
|<span data-ttu-id="56a86-233">antivirusRequired</span><span class="sxs-lookup"><span data-stu-id="56a86-233">antivirusRequired</span></span>|<span data-ttu-id="56a86-234">布尔</span><span class="sxs-lookup"><span data-stu-id="56a86-234">Boolean</span></span>|<span data-ttu-id="56a86-235">要求在 Windows Decurity Center 中注册的任何防病毒解决方案都处于启用和监控 (例如, Symantec、Windows Defender)。</span><span class="sxs-lookup"><span data-stu-id="56a86-235">Require any Antivirus solution registered with Windows Decurity Center to be on and monitoring (e.g. Symantec, Windows Defender).</span></span>|
|<span data-ttu-id="56a86-236">antiSpywareRequired</span><span class="sxs-lookup"><span data-stu-id="56a86-236">antiSpywareRequired</span></span>|<span data-ttu-id="56a86-237">布尔</span><span class="sxs-lookup"><span data-stu-id="56a86-237">Boolean</span></span>|<span data-ttu-id="56a86-238">要求在 Windows Decurity Center 中注册的任何反间谍软件解决方案都处于启用和监控 (例如, Symantec、Windows Defender)。</span><span class="sxs-lookup"><span data-stu-id="56a86-238">Require any AntiSpyware solution registered with Windows Decurity Center to be on and monitoring (e.g. Symantec, Windows Defender).</span></span>|
|<span data-ttu-id="56a86-239">validOperatingSystemBuildRanges</span><span class="sxs-lookup"><span data-stu-id="56a86-239">validOperatingSystemBuildRanges</span></span>|<span data-ttu-id="56a86-240">[operatingSystemVersionRange](../resources/intune-deviceconfig-operatingsystemversionrange.md)集合</span><span class="sxs-lookup"><span data-stu-id="56a86-240">[operatingSystemVersionRange](../resources/intune-deviceconfig-operatingsystemversionrange.md) collection</span></span>|<span data-ttu-id="56a86-241">Windows 设备上的有效操作系统内部版本范围。</span><span class="sxs-lookup"><span data-stu-id="56a86-241">The valid operating system build ranges on Windows devices.</span></span> <span data-ttu-id="56a86-242">该集合最多可包含 10000 个元素。</span><span class="sxs-lookup"><span data-stu-id="56a86-242">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="56a86-243">deviceThreatProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="56a86-243">deviceThreatProtectionEnabled</span></span>|<span data-ttu-id="56a86-244">Boolean</span><span class="sxs-lookup"><span data-stu-id="56a86-244">Boolean</span></span>|<span data-ttu-id="56a86-245">要求设备已启用设备威胁防护。</span><span class="sxs-lookup"><span data-stu-id="56a86-245">Require that devices have enabled device threat protection.</span></span>|
|<span data-ttu-id="56a86-246">deviceThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="56a86-246">deviceThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="56a86-247">deviceThreatProtectionLevel</span><span class="sxs-lookup"><span data-stu-id="56a86-247">deviceThreatProtectionLevel</span></span>](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|<span data-ttu-id="56a86-248">需要设备威胁防护最低风险级别来报告不合规。</span><span class="sxs-lookup"><span data-stu-id="56a86-248">Require Device Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="56a86-249">可取值为：`unavailable`、`secured`、`low`、`medium`、`high`、`notSet`。</span><span class="sxs-lookup"><span data-stu-id="56a86-249">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="56a86-250">configurationManagerComplianceRequired</span><span class="sxs-lookup"><span data-stu-id="56a86-250">configurationManagerComplianceRequired</span></span>|<span data-ttu-id="56a86-251">布尔</span><span class="sxs-lookup"><span data-stu-id="56a86-251">Boolean</span></span>|<span data-ttu-id="56a86-252">需要考虑将 SCCM 合规性状态考虑到 Intune 合规性状态。</span><span class="sxs-lookup"><span data-stu-id="56a86-252">Require to consider SCCM Compliance state into consideration for Intune Compliance State.</span></span>|



## <a name="response"></a><span data-ttu-id="56a86-253">响应</span><span class="sxs-lookup"><span data-stu-id="56a86-253">Response</span></span>
<span data-ttu-id="56a86-254">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和更新的 [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="56a86-254">If successful, this method returns a `200 OK` response code and an updated [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="56a86-255">示例</span><span class="sxs-lookup"><span data-stu-id="56a86-255">Example</span></span>

### <a name="request"></a><span data-ttu-id="56a86-256">请求</span><span class="sxs-lookup"><span data-stu-id="56a86-256">Request</span></span>
<span data-ttu-id="56a86-257">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="56a86-257">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
Content-type: application/json
Content-length: 1666

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
  "configurationManagerComplianceRequired": true
}
```

### <a name="response"></a><span data-ttu-id="56a86-258">响应</span><span class="sxs-lookup"><span data-stu-id="56a86-258">Response</span></span>
<span data-ttu-id="56a86-p112">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="56a86-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1838

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
  "configurationManagerComplianceRequired": true
}
```




