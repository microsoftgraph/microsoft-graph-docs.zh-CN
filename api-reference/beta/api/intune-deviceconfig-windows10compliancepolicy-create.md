---
title: 创建 windows10CompliancePolicy
description: 创建新的 windows10CompliancePolicy 对象。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: dce12d5b759acf2e26e193638a196fd9b826d8af
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2019
ms.locfileid: "33921910"
---
# <a name="create-windows10compliancepolicy"></a><span data-ttu-id="9e575-103">创建 windows10CompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="9e575-103">Create windows10CompliancePolicy</span></span>

> <span data-ttu-id="9e575-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="9e575-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9e575-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="9e575-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9e575-106">创建新的 [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="9e575-106">Create a new [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9e575-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="9e575-107">Prerequisites</span></span>
<span data-ttu-id="9e575-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9e575-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9e575-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="9e575-110">Permission type</span></span>|<span data-ttu-id="9e575-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="9e575-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9e575-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9e575-112">Delegated (work or school account)</span></span>|<span data-ttu-id="9e575-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9e575-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="9e575-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9e575-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9e575-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="9e575-115">Not supported.</span></span>|
|<span data-ttu-id="9e575-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="9e575-116">Application</span></span>|<span data-ttu-id="9e575-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="9e575-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9e575-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9e575-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="9e575-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="9e575-119">Request headers</span></span>
|<span data-ttu-id="9e575-120">标头</span><span class="sxs-lookup"><span data-stu-id="9e575-120">Header</span></span>|<span data-ttu-id="9e575-121">值</span><span class="sxs-lookup"><span data-stu-id="9e575-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9e575-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="9e575-122">Authorization</span></span>|<span data-ttu-id="9e575-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="9e575-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9e575-124">接受</span><span class="sxs-lookup"><span data-stu-id="9e575-124">Accept</span></span>|<span data-ttu-id="9e575-125">application/json</span><span class="sxs-lookup"><span data-stu-id="9e575-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9e575-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="9e575-126">Request body</span></span>
<span data-ttu-id="9e575-127">在请求正文中，提供 windows10CompliancePolicy 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9e575-127">In the request body, supply a JSON representation for the windows10CompliancePolicy object.</span></span>

<span data-ttu-id="9e575-128">下表显示创建 windows10CompliancePolicy 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="9e575-128">The following table shows the properties that are required when you create the windows10CompliancePolicy.</span></span>

|<span data-ttu-id="9e575-129">属性</span><span class="sxs-lookup"><span data-stu-id="9e575-129">Property</span></span>|<span data-ttu-id="9e575-130">类型</span><span class="sxs-lookup"><span data-stu-id="9e575-130">Type</span></span>|<span data-ttu-id="9e575-131">说明</span><span class="sxs-lookup"><span data-stu-id="9e575-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9e575-132">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="9e575-132">roleScopeTagIds</span></span>|<span data-ttu-id="9e575-133">String collection</span><span class="sxs-lookup"><span data-stu-id="9e575-133">String collection</span></span>|<span data-ttu-id="9e575-134">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="9e575-134">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="9e575-135">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="9e575-135">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="9e575-136">id</span><span class="sxs-lookup"><span data-stu-id="9e575-136">id</span></span>|<span data-ttu-id="9e575-137">字符串</span><span class="sxs-lookup"><span data-stu-id="9e575-137">String</span></span>|<span data-ttu-id="9e575-138">实体的键。</span><span class="sxs-lookup"><span data-stu-id="9e575-138">Key of the entity.</span></span> <span data-ttu-id="9e575-139">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="9e575-139">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="9e575-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="9e575-140">createdDateTime</span></span>|<span data-ttu-id="9e575-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9e575-141">DateTimeOffset</span></span>|<span data-ttu-id="9e575-142">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="9e575-142">DateTime the object was created.</span></span> <span data-ttu-id="9e575-143">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="9e575-143">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="9e575-144">说明</span><span class="sxs-lookup"><span data-stu-id="9e575-144">description</span></span>|<span data-ttu-id="9e575-145">String</span><span class="sxs-lookup"><span data-stu-id="9e575-145">String</span></span>|<span data-ttu-id="9e575-146">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="9e575-146">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="9e575-147">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="9e575-147">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="9e575-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9e575-148">lastModifiedDateTime</span></span>|<span data-ttu-id="9e575-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9e575-149">DateTimeOffset</span></span>|<span data-ttu-id="9e575-150">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="9e575-150">DateTime the object was last modified.</span></span> <span data-ttu-id="9e575-151">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="9e575-151">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="9e575-152">displayName</span><span class="sxs-lookup"><span data-stu-id="9e575-152">displayName</span></span>|<span data-ttu-id="9e575-153">字符串</span><span class="sxs-lookup"><span data-stu-id="9e575-153">String</span></span>|<span data-ttu-id="9e575-154">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="9e575-154">Admin provided name of the device configuration.</span></span> <span data-ttu-id="9e575-155">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="9e575-155">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="9e575-156">version</span><span class="sxs-lookup"><span data-stu-id="9e575-156">version</span></span>|<span data-ttu-id="9e575-157">Int32</span><span class="sxs-lookup"><span data-stu-id="9e575-157">Int32</span></span>|<span data-ttu-id="9e575-158">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="9e575-158">Version of the device configuration.</span></span> <span data-ttu-id="9e575-159">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="9e575-159">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="9e575-160">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="9e575-160">passwordRequired</span></span>|<span data-ttu-id="9e575-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="9e575-161">Boolean</span></span>|<span data-ttu-id="9e575-162">需要密码才可解锁 Windows 设备。</span><span class="sxs-lookup"><span data-stu-id="9e575-162">Require a password to unlock Windows device.</span></span>|
|<span data-ttu-id="9e575-163">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="9e575-163">passwordBlockSimple</span></span>|<span data-ttu-id="9e575-164">Boolean</span><span class="sxs-lookup"><span data-stu-id="9e575-164">Boolean</span></span>|<span data-ttu-id="9e575-165">指示是否阻止简单密码。</span><span class="sxs-lookup"><span data-stu-id="9e575-165">Indicates whether or not to block simple password.</span></span>|
|<span data-ttu-id="9e575-166">passwordRequiredToUnlockFromIdle</span><span class="sxs-lookup"><span data-stu-id="9e575-166">passwordRequiredToUnlockFromIdle</span></span>|<span data-ttu-id="9e575-167">Boolean</span><span class="sxs-lookup"><span data-stu-id="9e575-167">Boolean</span></span>|<span data-ttu-id="9e575-168">需要密码才可解锁空闲设备。</span><span class="sxs-lookup"><span data-stu-id="9e575-168">Require a password to unlock an idle device.</span></span>|
|<span data-ttu-id="9e575-169">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="9e575-169">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="9e575-170">Int32</span><span class="sxs-lookup"><span data-stu-id="9e575-170">Int32</span></span>|<span data-ttu-id="9e575-171">在需要密码之前不活动的分钟数。</span><span class="sxs-lookup"><span data-stu-id="9e575-171">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="9e575-172">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="9e575-172">passwordExpirationDays</span></span>|<span data-ttu-id="9e575-173">Int32</span><span class="sxs-lookup"><span data-stu-id="9e575-173">Int32</span></span>|<span data-ttu-id="9e575-174">密码过期天数。</span><span class="sxs-lookup"><span data-stu-id="9e575-174">The password expiration in days.</span></span>|
|<span data-ttu-id="9e575-175">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="9e575-175">passwordMinimumLength</span></span>|<span data-ttu-id="9e575-176">Int32</span><span class="sxs-lookup"><span data-stu-id="9e575-176">Int32</span></span>|<span data-ttu-id="9e575-177">密码最短长度。</span><span class="sxs-lookup"><span data-stu-id="9e575-177">The minimum password length.</span></span>|
|<span data-ttu-id="9e575-178">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="9e575-178">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="9e575-179">Int32</span><span class="sxs-lookup"><span data-stu-id="9e575-179">Int32</span></span>|<span data-ttu-id="9e575-180">密码中必需的字符集数。</span><span class="sxs-lookup"><span data-stu-id="9e575-180">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="9e575-181">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="9e575-181">passwordRequiredType</span></span>|[<span data-ttu-id="9e575-182">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="9e575-182">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="9e575-183">必需的密码类型。</span><span class="sxs-lookup"><span data-stu-id="9e575-183">The required password type.</span></span> <span data-ttu-id="9e575-184">可取值为：`deviceDefault`、`alphanumeric`、`numeric`。</span><span class="sxs-lookup"><span data-stu-id="9e575-184">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="9e575-185">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="9e575-185">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="9e575-186">Int32</span><span class="sxs-lookup"><span data-stu-id="9e575-186">Int32</span></span>|<span data-ttu-id="9e575-187">防止重复使用的先前密码的数量。</span><span class="sxs-lookup"><span data-stu-id="9e575-187">The number of previous passwords to prevent re-use of.</span></span>|
|<span data-ttu-id="9e575-188">requireHealthyDeviceReport</span><span class="sxs-lookup"><span data-stu-id="9e575-188">requireHealthyDeviceReport</span></span>|<span data-ttu-id="9e575-189">Boolean</span><span class="sxs-lookup"><span data-stu-id="9e575-189">Boolean</span></span>|<span data-ttu-id="9e575-190">要求设备由 Windows 设备运行状况证明报告为正常。</span><span class="sxs-lookup"><span data-stu-id="9e575-190">Require devices to be reported as healthy by Windows Device Health Attestation.</span></span>|
|<span data-ttu-id="9e575-191">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="9e575-191">osMinimumVersion</span></span>|<span data-ttu-id="9e575-192">String</span><span class="sxs-lookup"><span data-stu-id="9e575-192">String</span></span>|<span data-ttu-id="9e575-193">最低 Windows 10 版本。</span><span class="sxs-lookup"><span data-stu-id="9e575-193">Minimum Windows 10 version.</span></span>|
|<span data-ttu-id="9e575-194">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="9e575-194">osMaximumVersion</span></span>|<span data-ttu-id="9e575-195">String</span><span class="sxs-lookup"><span data-stu-id="9e575-195">String</span></span>|<span data-ttu-id="9e575-196">最高 Windows 10 版本。</span><span class="sxs-lookup"><span data-stu-id="9e575-196">Maximum Windows 10 version.</span></span>|
|<span data-ttu-id="9e575-197">mobileOsMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="9e575-197">mobileOsMinimumVersion</span></span>|<span data-ttu-id="9e575-198">String</span><span class="sxs-lookup"><span data-stu-id="9e575-198">String</span></span>|<span data-ttu-id="9e575-199">最低 Windows Phone 版本。</span><span class="sxs-lookup"><span data-stu-id="9e575-199">Minimum Windows Phone version.</span></span>|
|<span data-ttu-id="9e575-200">mobileOsMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="9e575-200">mobileOsMaximumVersion</span></span>|<span data-ttu-id="9e575-201">String</span><span class="sxs-lookup"><span data-stu-id="9e575-201">String</span></span>|<span data-ttu-id="9e575-202">最高 Windows Phone 版本。</span><span class="sxs-lookup"><span data-stu-id="9e575-202">Maximum Windows Phone version.</span></span>|
|<span data-ttu-id="9e575-203">earlyLaunchAntiMalwareDriverEnabled</span><span class="sxs-lookup"><span data-stu-id="9e575-203">earlyLaunchAntiMalwareDriverEnabled</span></span>|<span data-ttu-id="9e575-204">Boolean</span><span class="sxs-lookup"><span data-stu-id="9e575-204">Boolean</span></span>|<span data-ttu-id="9e575-205">要求设备由 Windows 设备运行状况证明报告为正常 - 提前启动反恶意驱动程序已启用。</span><span class="sxs-lookup"><span data-stu-id="9e575-205">Require devices to be reported as healthy by Windows Device Health Attestation - early launch antimalware driver is enabled.</span></span>|
|<span data-ttu-id="9e575-206">bitLockerEnabled</span><span class="sxs-lookup"><span data-stu-id="9e575-206">bitLockerEnabled</span></span>|<span data-ttu-id="9e575-207">Boolean</span><span class="sxs-lookup"><span data-stu-id="9e575-207">Boolean</span></span>|<span data-ttu-id="9e575-208">要求设备由 Windows 设备运行状况证明报告为正常 - bit locker 已启用。</span><span class="sxs-lookup"><span data-stu-id="9e575-208">Require devices to be reported healthy by Windows Device Health Attestation - bit locker is enabled</span></span>|
|<span data-ttu-id="9e575-209">secureBootEnabled</span><span class="sxs-lookup"><span data-stu-id="9e575-209">secureBootEnabled</span></span>|<span data-ttu-id="9e575-210">Boolean</span><span class="sxs-lookup"><span data-stu-id="9e575-210">Boolean</span></span>|<span data-ttu-id="9e575-211">要求设备由 Windows 设备运行状况证明报告为正常 - 安全启动已启用。</span><span class="sxs-lookup"><span data-stu-id="9e575-211">Require devices to be reported as healthy by Windows Device Health Attestation - secure boot is enabled.</span></span>|
|<span data-ttu-id="9e575-212">codeIntegrityEnabled</span><span class="sxs-lookup"><span data-stu-id="9e575-212">codeIntegrityEnabled</span></span>|<span data-ttu-id="9e575-213">Boolean</span><span class="sxs-lookup"><span data-stu-id="9e575-213">Boolean</span></span>|<span data-ttu-id="9e575-214">要求设备由 Windows 设备运行状况证明报告为正常。</span><span class="sxs-lookup"><span data-stu-id="9e575-214">Require devices to be reported as healthy by Windows Device Health Attestation.</span></span>|
|<span data-ttu-id="9e575-215">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="9e575-215">storageRequireEncryption</span></span>|<span data-ttu-id="9e575-216">Boolean</span><span class="sxs-lookup"><span data-stu-id="9e575-216">Boolean</span></span>|<span data-ttu-id="9e575-217">要求对 Windows 设备加密。</span><span class="sxs-lookup"><span data-stu-id="9e575-217">Require encryption on windows devices.</span></span>|
|<span data-ttu-id="9e575-218">activeFirewallRequired</span><span class="sxs-lookup"><span data-stu-id="9e575-218">activeFirewallRequired</span></span>|<span data-ttu-id="9e575-219">Boolean</span><span class="sxs-lookup"><span data-stu-id="9e575-219">Boolean</span></span>|<span data-ttu-id="9e575-220">在 Windows 设备上需要活动防火墙。</span><span class="sxs-lookup"><span data-stu-id="9e575-220">Require active firewall on Windows devices.</span></span>|
|<span data-ttu-id="9e575-221">defenderEnabled</span><span class="sxs-lookup"><span data-stu-id="9e575-221">defenderEnabled</span></span>|<span data-ttu-id="9e575-222">Boolean</span><span class="sxs-lookup"><span data-stu-id="9e575-222">Boolean</span></span>|<span data-ttu-id="9e575-223">在 Windows 设备上需要 Windows Defender 反恶意软件。</span><span class="sxs-lookup"><span data-stu-id="9e575-223">Require Windows Defender Antimalware on Windows devices.</span></span>|
|<span data-ttu-id="9e575-224">defenderVersion</span><span class="sxs-lookup"><span data-stu-id="9e575-224">defenderVersion</span></span>|<span data-ttu-id="9e575-225">String</span><span class="sxs-lookup"><span data-stu-id="9e575-225">String</span></span>|<span data-ttu-id="9e575-226">在 Windows 设备上要求 Windows Defender 反恶意软件的最低版本。</span><span class="sxs-lookup"><span data-stu-id="9e575-226">Require Windows Defender Antimalware minimum version on Windows devices.</span></span>|
|<span data-ttu-id="9e575-227">signatureOutOfDate</span><span class="sxs-lookup"><span data-stu-id="9e575-227">signatureOutOfDate</span></span>|<span data-ttu-id="9e575-228">Boolean</span><span class="sxs-lookup"><span data-stu-id="9e575-228">Boolean</span></span>|<span data-ttu-id="9e575-229">Windows 设备上要求 Windows Defender 反恶意软件签名为最新。</span><span class="sxs-lookup"><span data-stu-id="9e575-229">Require Windows Defender Antimalware Signature to be up to date on Windows devices.</span></span>|
|<span data-ttu-id="9e575-230">rtpEnabled</span><span class="sxs-lookup"><span data-stu-id="9e575-230">rtpEnabled</span></span>|<span data-ttu-id="9e575-231">Boolean</span><span class="sxs-lookup"><span data-stu-id="9e575-231">Boolean</span></span>|<span data-ttu-id="9e575-232">在 Windows 设备上需要 Windows Defender 反恶意软件实时保护。</span><span class="sxs-lookup"><span data-stu-id="9e575-232">Require Windows Defender Antimalware Real-Time Protection on Windows devices.</span></span>|
|<span data-ttu-id="9e575-233">antivirusRequired</span><span class="sxs-lookup"><span data-stu-id="9e575-233">antivirusRequired</span></span>|<span data-ttu-id="9e575-234">Boolean</span><span class="sxs-lookup"><span data-stu-id="9e575-234">Boolean</span></span>|<span data-ttu-id="9e575-235">要求在 Windows Decurity Center 中注册的任何防病毒解决方案都处于启用和监控 (例如, Symantec、Windows Defender)。</span><span class="sxs-lookup"><span data-stu-id="9e575-235">Require any Antivirus solution registered with Windows Decurity Center to be on and monitoring (e.g. Symantec, Windows Defender).</span></span>|
|<span data-ttu-id="9e575-236">antiSpywareRequired</span><span class="sxs-lookup"><span data-stu-id="9e575-236">antiSpywareRequired</span></span>|<span data-ttu-id="9e575-237">Boolean</span><span class="sxs-lookup"><span data-stu-id="9e575-237">Boolean</span></span>|<span data-ttu-id="9e575-238">要求在 Windows Decurity Center 中注册的任何反间谍软件解决方案都处于启用和监控 (例如, Symantec、Windows Defender)。</span><span class="sxs-lookup"><span data-stu-id="9e575-238">Require any AntiSpyware solution registered with Windows Decurity Center to be on and monitoring (e.g. Symantec, Windows Defender).</span></span>|
|<span data-ttu-id="9e575-239">validOperatingSystemBuildRanges</span><span class="sxs-lookup"><span data-stu-id="9e575-239">validOperatingSystemBuildRanges</span></span>|<span data-ttu-id="9e575-240">[operatingSystemVersionRange](../resources/intune-deviceconfig-operatingsystemversionrange.md)集合</span><span class="sxs-lookup"><span data-stu-id="9e575-240">[operatingSystemVersionRange](../resources/intune-deviceconfig-operatingsystemversionrange.md) collection</span></span>|<span data-ttu-id="9e575-241">Windows 设备上的有效操作系统内部版本范围。</span><span class="sxs-lookup"><span data-stu-id="9e575-241">The valid operating system build ranges on Windows devices.</span></span> <span data-ttu-id="9e575-242">该集合最多可包含 10000 个元素。</span><span class="sxs-lookup"><span data-stu-id="9e575-242">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="9e575-243">deviceThreatProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="9e575-243">deviceThreatProtectionEnabled</span></span>|<span data-ttu-id="9e575-244">Boolean</span><span class="sxs-lookup"><span data-stu-id="9e575-244">Boolean</span></span>|<span data-ttu-id="9e575-245">要求设备已启用设备威胁防护。</span><span class="sxs-lookup"><span data-stu-id="9e575-245">Require that devices have enabled device threat protection.</span></span>|
|<span data-ttu-id="9e575-246">deviceThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="9e575-246">deviceThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="9e575-247">deviceThreatProtectionLevel</span><span class="sxs-lookup"><span data-stu-id="9e575-247">deviceThreatProtectionLevel</span></span>](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|<span data-ttu-id="9e575-248">需要设备威胁防护最低风险级别来报告不合规。</span><span class="sxs-lookup"><span data-stu-id="9e575-248">Require Device Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="9e575-249">可取值为：`unavailable`、`secured`、`low`、`medium`、`high`、`notSet`。</span><span class="sxs-lookup"><span data-stu-id="9e575-249">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="9e575-250">configurationManagerComplianceRequired</span><span class="sxs-lookup"><span data-stu-id="9e575-250">configurationManagerComplianceRequired</span></span>|<span data-ttu-id="9e575-251">Boolean</span><span class="sxs-lookup"><span data-stu-id="9e575-251">Boolean</span></span>|<span data-ttu-id="9e575-252">需要考虑将 SCCM 合规性状态考虑到 Intune 合规性状态。</span><span class="sxs-lookup"><span data-stu-id="9e575-252">Require to consider SCCM Compliance state into consideration for Intune Compliance State.</span></span>|
|<span data-ttu-id="9e575-253">tpmRequired</span><span class="sxs-lookup"><span data-stu-id="9e575-253">tpmRequired</span></span>|<span data-ttu-id="9e575-254">Boolean</span><span class="sxs-lookup"><span data-stu-id="9e575-254">Boolean</span></span>|<span data-ttu-id="9e575-255">要求存在受信任的平台模块 (TPM)。</span><span class="sxs-lookup"><span data-stu-id="9e575-255">Require Trusted Platform Module(TPM) to be present.</span></span>|



## <a name="response"></a><span data-ttu-id="9e575-256">响应</span><span class="sxs-lookup"><span data-stu-id="9e575-256">Response</span></span>
<span data-ttu-id="9e575-257">如果成功，此方法会在响应正文中返回 `201 Created` 响应代码和 [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="9e575-257">If successful, this method returns a `201 Created` response code and a [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9e575-258">示例</span><span class="sxs-lookup"><span data-stu-id="9e575-258">Example</span></span>

### <a name="request"></a><span data-ttu-id="9e575-259">请求</span><span class="sxs-lookup"><span data-stu-id="9e575-259">Request</span></span>
<span data-ttu-id="9e575-260">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="9e575-260">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="9e575-261">响应</span><span class="sxs-lookup"><span data-stu-id="9e575-261">Response</span></span>
<span data-ttu-id="9e575-p112">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="9e575-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




