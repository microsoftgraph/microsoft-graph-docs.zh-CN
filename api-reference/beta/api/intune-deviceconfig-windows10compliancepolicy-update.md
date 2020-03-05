---
title: 更新 windows10CompliancePolicy
description: 更新 windows10CompliancePolicy 对象的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: a333bfe10ded7168b873cd226fe3aa9d7111cc15
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42481836"
---
# <a name="update-windows10compliancepolicy"></a><span data-ttu-id="93647-103">更新 windows10CompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="93647-103">Update windows10CompliancePolicy</span></span>

<span data-ttu-id="93647-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="93647-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="93647-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="93647-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="93647-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="93647-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="93647-107">更新 [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="93647-107">Update the properties of a [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="93647-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="93647-108">Prerequisites</span></span>
<span data-ttu-id="93647-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="93647-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="93647-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="93647-111">Permission type</span></span>|<span data-ttu-id="93647-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="93647-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="93647-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="93647-113">Delegated (work or school account)</span></span>|<span data-ttu-id="93647-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="93647-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="93647-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="93647-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="93647-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="93647-116">Not supported.</span></span>|
|<span data-ttu-id="93647-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="93647-117">Application</span></span>|<span data-ttu-id="93647-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="93647-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="93647-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="93647-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="93647-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="93647-120">Request headers</span></span>
|<span data-ttu-id="93647-121">标头</span><span class="sxs-lookup"><span data-stu-id="93647-121">Header</span></span>|<span data-ttu-id="93647-122">值</span><span class="sxs-lookup"><span data-stu-id="93647-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="93647-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="93647-123">Authorization</span></span>|<span data-ttu-id="93647-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="93647-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="93647-125">接受</span><span class="sxs-lookup"><span data-stu-id="93647-125">Accept</span></span>|<span data-ttu-id="93647-126">application/json</span><span class="sxs-lookup"><span data-stu-id="93647-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="93647-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="93647-127">Request body</span></span>
<span data-ttu-id="93647-128">在请求正文中，提供 [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="93647-128">In the request body, supply a JSON representation for the [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) object.</span></span>

<span data-ttu-id="93647-129">下表显示创建 [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="93647-129">The following table shows the properties that are required when you create the [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md).</span></span>

|<span data-ttu-id="93647-130">属性</span><span class="sxs-lookup"><span data-stu-id="93647-130">Property</span></span>|<span data-ttu-id="93647-131">类型</span><span class="sxs-lookup"><span data-stu-id="93647-131">Type</span></span>|<span data-ttu-id="93647-132">说明</span><span class="sxs-lookup"><span data-stu-id="93647-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="93647-133">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="93647-133">roleScopeTagIds</span></span>|<span data-ttu-id="93647-134">String 集合</span><span class="sxs-lookup"><span data-stu-id="93647-134">String collection</span></span>|<span data-ttu-id="93647-135">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="93647-135">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="93647-136">继承自 [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="93647-136">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="93647-137">id</span><span class="sxs-lookup"><span data-stu-id="93647-137">id</span></span>|<span data-ttu-id="93647-138">字符串</span><span class="sxs-lookup"><span data-stu-id="93647-138">String</span></span>|<span data-ttu-id="93647-139">实体的键。</span><span class="sxs-lookup"><span data-stu-id="93647-139">Key of the entity.</span></span> <span data-ttu-id="93647-140">继承自 [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="93647-140">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="93647-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="93647-141">createdDateTime</span></span>|<span data-ttu-id="93647-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="93647-142">DateTimeOffset</span></span>|<span data-ttu-id="93647-143">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="93647-143">DateTime the object was created.</span></span> <span data-ttu-id="93647-144">继承自 [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="93647-144">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="93647-145">说明</span><span class="sxs-lookup"><span data-stu-id="93647-145">description</span></span>|<span data-ttu-id="93647-146">String</span><span class="sxs-lookup"><span data-stu-id="93647-146">String</span></span>|<span data-ttu-id="93647-147">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="93647-147">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="93647-148">继承自 [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="93647-148">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="93647-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="93647-149">lastModifiedDateTime</span></span>|<span data-ttu-id="93647-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="93647-150">DateTimeOffset</span></span>|<span data-ttu-id="93647-151">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="93647-151">DateTime the object was last modified.</span></span> <span data-ttu-id="93647-152">继承自 [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="93647-152">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="93647-153">displayName</span><span class="sxs-lookup"><span data-stu-id="93647-153">displayName</span></span>|<span data-ttu-id="93647-154">字符串</span><span class="sxs-lookup"><span data-stu-id="93647-154">String</span></span>|<span data-ttu-id="93647-155">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="93647-155">Admin provided name of the device configuration.</span></span> <span data-ttu-id="93647-156">继承自 [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="93647-156">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="93647-157">version</span><span class="sxs-lookup"><span data-stu-id="93647-157">version</span></span>|<span data-ttu-id="93647-158">Int32</span><span class="sxs-lookup"><span data-stu-id="93647-158">Int32</span></span>|<span data-ttu-id="93647-159">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="93647-159">Version of the device configuration.</span></span> <span data-ttu-id="93647-160">继承自 [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="93647-160">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="93647-161">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="93647-161">passwordRequired</span></span>|<span data-ttu-id="93647-162">布尔</span><span class="sxs-lookup"><span data-stu-id="93647-162">Boolean</span></span>|<span data-ttu-id="93647-163">需要密码才可解锁 Windows 设备。</span><span class="sxs-lookup"><span data-stu-id="93647-163">Require a password to unlock Windows device.</span></span>|
|<span data-ttu-id="93647-164">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="93647-164">passwordBlockSimple</span></span>|<span data-ttu-id="93647-165">布尔</span><span class="sxs-lookup"><span data-stu-id="93647-165">Boolean</span></span>|<span data-ttu-id="93647-166">指示是否阻止简单密码。</span><span class="sxs-lookup"><span data-stu-id="93647-166">Indicates whether or not to block simple password.</span></span>|
|<span data-ttu-id="93647-167">passwordRequiredToUnlockFromIdle</span><span class="sxs-lookup"><span data-stu-id="93647-167">passwordRequiredToUnlockFromIdle</span></span>|<span data-ttu-id="93647-168">布尔</span><span class="sxs-lookup"><span data-stu-id="93647-168">Boolean</span></span>|<span data-ttu-id="93647-169">需要密码才可解锁空闲设备。</span><span class="sxs-lookup"><span data-stu-id="93647-169">Require a password to unlock an idle device.</span></span>|
|<span data-ttu-id="93647-170">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="93647-170">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="93647-171">Int32</span><span class="sxs-lookup"><span data-stu-id="93647-171">Int32</span></span>|<span data-ttu-id="93647-172">在需要密码之前不活动的分钟数。</span><span class="sxs-lookup"><span data-stu-id="93647-172">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="93647-173">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="93647-173">passwordExpirationDays</span></span>|<span data-ttu-id="93647-174">Int32</span><span class="sxs-lookup"><span data-stu-id="93647-174">Int32</span></span>|<span data-ttu-id="93647-175">密码过期天数。</span><span class="sxs-lookup"><span data-stu-id="93647-175">The password expiration in days.</span></span>|
|<span data-ttu-id="93647-176">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="93647-176">passwordMinimumLength</span></span>|<span data-ttu-id="93647-177">Int32</span><span class="sxs-lookup"><span data-stu-id="93647-177">Int32</span></span>|<span data-ttu-id="93647-178">密码最短长度。</span><span class="sxs-lookup"><span data-stu-id="93647-178">The minimum password length.</span></span>|
|<span data-ttu-id="93647-179">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="93647-179">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="93647-180">Int32</span><span class="sxs-lookup"><span data-stu-id="93647-180">Int32</span></span>|<span data-ttu-id="93647-181">密码中必需的字符集数。</span><span class="sxs-lookup"><span data-stu-id="93647-181">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="93647-182">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="93647-182">passwordRequiredType</span></span>|[<span data-ttu-id="93647-183">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="93647-183">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="93647-184">必需的密码类型。</span><span class="sxs-lookup"><span data-stu-id="93647-184">The required password type.</span></span> <span data-ttu-id="93647-185">可取值为：`deviceDefault`、`alphanumeric`、`numeric`。</span><span class="sxs-lookup"><span data-stu-id="93647-185">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="93647-186">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="93647-186">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="93647-187">Int32</span><span class="sxs-lookup"><span data-stu-id="93647-187">Int32</span></span>|<span data-ttu-id="93647-188">防止重复使用的先前密码的数量。</span><span class="sxs-lookup"><span data-stu-id="93647-188">The number of previous passwords to prevent re-use of.</span></span>|
|<span data-ttu-id="93647-189">requireHealthyDeviceReport</span><span class="sxs-lookup"><span data-stu-id="93647-189">requireHealthyDeviceReport</span></span>|<span data-ttu-id="93647-190">布尔</span><span class="sxs-lookup"><span data-stu-id="93647-190">Boolean</span></span>|<span data-ttu-id="93647-191">要求设备由 Windows 设备运行状况证明报告为正常。</span><span class="sxs-lookup"><span data-stu-id="93647-191">Require devices to be reported as healthy by Windows Device Health Attestation.</span></span>|
|<span data-ttu-id="93647-192">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="93647-192">osMinimumVersion</span></span>|<span data-ttu-id="93647-193">String</span><span class="sxs-lookup"><span data-stu-id="93647-193">String</span></span>|<span data-ttu-id="93647-194">最低 Windows 10 版本。</span><span class="sxs-lookup"><span data-stu-id="93647-194">Minimum Windows 10 version.</span></span>|
|<span data-ttu-id="93647-195">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="93647-195">osMaximumVersion</span></span>|<span data-ttu-id="93647-196">String</span><span class="sxs-lookup"><span data-stu-id="93647-196">String</span></span>|<span data-ttu-id="93647-197">最高 Windows 10 版本。</span><span class="sxs-lookup"><span data-stu-id="93647-197">Maximum Windows 10 version.</span></span>|
|<span data-ttu-id="93647-198">mobileOsMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="93647-198">mobileOsMinimumVersion</span></span>|<span data-ttu-id="93647-199">String</span><span class="sxs-lookup"><span data-stu-id="93647-199">String</span></span>|<span data-ttu-id="93647-200">最低 Windows Phone 版本。</span><span class="sxs-lookup"><span data-stu-id="93647-200">Minimum Windows Phone version.</span></span>|
|<span data-ttu-id="93647-201">mobileOsMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="93647-201">mobileOsMaximumVersion</span></span>|<span data-ttu-id="93647-202">String</span><span class="sxs-lookup"><span data-stu-id="93647-202">String</span></span>|<span data-ttu-id="93647-203">最高 Windows Phone 版本。</span><span class="sxs-lookup"><span data-stu-id="93647-203">Maximum Windows Phone version.</span></span>|
|<span data-ttu-id="93647-204">earlyLaunchAntiMalwareDriverEnabled</span><span class="sxs-lookup"><span data-stu-id="93647-204">earlyLaunchAntiMalwareDriverEnabled</span></span>|<span data-ttu-id="93647-205">布尔</span><span class="sxs-lookup"><span data-stu-id="93647-205">Boolean</span></span>|<span data-ttu-id="93647-206">要求设备由 Windows 设备运行状况证明报告为正常 - 提前启动反恶意驱动程序已启用。</span><span class="sxs-lookup"><span data-stu-id="93647-206">Require devices to be reported as healthy by Windows Device Health Attestation - early launch antimalware driver is enabled.</span></span>|
|<span data-ttu-id="93647-207">bitLockerEnabled</span><span class="sxs-lookup"><span data-stu-id="93647-207">bitLockerEnabled</span></span>|<span data-ttu-id="93647-208">布尔</span><span class="sxs-lookup"><span data-stu-id="93647-208">Boolean</span></span>|<span data-ttu-id="93647-209">要求设备由 Windows 设备运行状况证明报告为正常 - bit locker 已启用。</span><span class="sxs-lookup"><span data-stu-id="93647-209">Require devices to be reported healthy by Windows Device Health Attestation - bit locker is enabled</span></span>|
|<span data-ttu-id="93647-210">secureBootEnabled</span><span class="sxs-lookup"><span data-stu-id="93647-210">secureBootEnabled</span></span>|<span data-ttu-id="93647-211">布尔</span><span class="sxs-lookup"><span data-stu-id="93647-211">Boolean</span></span>|<span data-ttu-id="93647-212">要求设备由 Windows 设备运行状况证明报告为正常 - 安全启动已启用。</span><span class="sxs-lookup"><span data-stu-id="93647-212">Require devices to be reported as healthy by Windows Device Health Attestation - secure boot is enabled.</span></span>|
|<span data-ttu-id="93647-213">codeIntegrityEnabled</span><span class="sxs-lookup"><span data-stu-id="93647-213">codeIntegrityEnabled</span></span>|<span data-ttu-id="93647-214">Boolean</span><span class="sxs-lookup"><span data-stu-id="93647-214">Boolean</span></span>|<span data-ttu-id="93647-215">要求设备由 Windows 设备运行状况证明报告为正常。</span><span class="sxs-lookup"><span data-stu-id="93647-215">Require devices to be reported as healthy by Windows Device Health Attestation.</span></span>|
|<span data-ttu-id="93647-216">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="93647-216">storageRequireEncryption</span></span>|<span data-ttu-id="93647-217">Boolean</span><span class="sxs-lookup"><span data-stu-id="93647-217">Boolean</span></span>|<span data-ttu-id="93647-218">要求对 Windows 设备加密。</span><span class="sxs-lookup"><span data-stu-id="93647-218">Require encryption on windows devices.</span></span>|
|<span data-ttu-id="93647-219">activeFirewallRequired</span><span class="sxs-lookup"><span data-stu-id="93647-219">activeFirewallRequired</span></span>|<span data-ttu-id="93647-220">布尔</span><span class="sxs-lookup"><span data-stu-id="93647-220">Boolean</span></span>|<span data-ttu-id="93647-221">在 Windows 设备上需要活动防火墙。</span><span class="sxs-lookup"><span data-stu-id="93647-221">Require active firewall on Windows devices.</span></span>|
|<span data-ttu-id="93647-222">defenderEnabled</span><span class="sxs-lookup"><span data-stu-id="93647-222">defenderEnabled</span></span>|<span data-ttu-id="93647-223">布尔</span><span class="sxs-lookup"><span data-stu-id="93647-223">Boolean</span></span>|<span data-ttu-id="93647-224">在 Windows 设备上需要 Windows Defender 反恶意软件。</span><span class="sxs-lookup"><span data-stu-id="93647-224">Require Windows Defender Antimalware on Windows devices.</span></span>|
|<span data-ttu-id="93647-225">defenderVersion</span><span class="sxs-lookup"><span data-stu-id="93647-225">defenderVersion</span></span>|<span data-ttu-id="93647-226">String</span><span class="sxs-lookup"><span data-stu-id="93647-226">String</span></span>|<span data-ttu-id="93647-227">在 Windows 设备上要求 Windows Defender 反恶意软件的最低版本。</span><span class="sxs-lookup"><span data-stu-id="93647-227">Require Windows Defender Antimalware minimum version on Windows devices.</span></span>|
|<span data-ttu-id="93647-228">signatureOutOfDate</span><span class="sxs-lookup"><span data-stu-id="93647-228">signatureOutOfDate</span></span>|<span data-ttu-id="93647-229">布尔</span><span class="sxs-lookup"><span data-stu-id="93647-229">Boolean</span></span>|<span data-ttu-id="93647-230">Windows 设备上要求 Windows Defender 反恶意软件签名为最新。</span><span class="sxs-lookup"><span data-stu-id="93647-230">Require Windows Defender Antimalware Signature to be up to date on Windows devices.</span></span>|
|<span data-ttu-id="93647-231">rtpEnabled</span><span class="sxs-lookup"><span data-stu-id="93647-231">rtpEnabled</span></span>|<span data-ttu-id="93647-232">布尔</span><span class="sxs-lookup"><span data-stu-id="93647-232">Boolean</span></span>|<span data-ttu-id="93647-233">在 Windows 设备上需要 Windows Defender 反恶意软件实时保护。</span><span class="sxs-lookup"><span data-stu-id="93647-233">Require Windows Defender Antimalware Real-Time Protection on Windows devices.</span></span>|
|<span data-ttu-id="93647-234">antivirusRequired</span><span class="sxs-lookup"><span data-stu-id="93647-234">antivirusRequired</span></span>|<span data-ttu-id="93647-235">布尔</span><span class="sxs-lookup"><span data-stu-id="93647-235">Boolean</span></span>|<span data-ttu-id="93647-236">要求在 Windows Decurity Center 中注册的任何防病毒解决方案都处于启用和监控（例如，Symantec、Windows Defender）。</span><span class="sxs-lookup"><span data-stu-id="93647-236">Require any Antivirus solution registered with Windows Decurity Center to be on and monitoring (e.g. Symantec, Windows Defender).</span></span>|
|<span data-ttu-id="93647-237">antiSpywareRequired</span><span class="sxs-lookup"><span data-stu-id="93647-237">antiSpywareRequired</span></span>|<span data-ttu-id="93647-238">布尔</span><span class="sxs-lookup"><span data-stu-id="93647-238">Boolean</span></span>|<span data-ttu-id="93647-239">要求在 Windows Decurity Center 中注册的任何反间谍软件解决方案都处于启用和监控（例如，Symantec、Windows Defender）。</span><span class="sxs-lookup"><span data-stu-id="93647-239">Require any AntiSpyware solution registered with Windows Decurity Center to be on and monitoring (e.g. Symantec, Windows Defender).</span></span>|
|<span data-ttu-id="93647-240">validOperatingSystemBuildRanges</span><span class="sxs-lookup"><span data-stu-id="93647-240">validOperatingSystemBuildRanges</span></span>|<span data-ttu-id="93647-241">[operatingSystemVersionRange](../resources/intune-deviceconfig-operatingsystemversionrange.md)集合</span><span class="sxs-lookup"><span data-stu-id="93647-241">[operatingSystemVersionRange](../resources/intune-deviceconfig-operatingsystemversionrange.md) collection</span></span>|<span data-ttu-id="93647-242">Windows 设备上的有效操作系统内部版本范围。</span><span class="sxs-lookup"><span data-stu-id="93647-242">The valid operating system build ranges on Windows devices.</span></span> <span data-ttu-id="93647-243">该集合最多可包含 10000 个元素。</span><span class="sxs-lookup"><span data-stu-id="93647-243">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="93647-244">deviceThreatProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="93647-244">deviceThreatProtectionEnabled</span></span>|<span data-ttu-id="93647-245">Boolean</span><span class="sxs-lookup"><span data-stu-id="93647-245">Boolean</span></span>|<span data-ttu-id="93647-246">要求设备已启用设备威胁防护。</span><span class="sxs-lookup"><span data-stu-id="93647-246">Require that devices have enabled device threat protection.</span></span>|
|<span data-ttu-id="93647-247">deviceThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="93647-247">deviceThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="93647-248">deviceThreatProtectionLevel</span><span class="sxs-lookup"><span data-stu-id="93647-248">deviceThreatProtectionLevel</span></span>](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|<span data-ttu-id="93647-249">需要设备威胁防护最低风险级别来报告不合规。</span><span class="sxs-lookup"><span data-stu-id="93647-249">Require Device Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="93647-250">可取值为：`unavailable`、`secured`、`low`、`medium`、`high`、`notSet`。</span><span class="sxs-lookup"><span data-stu-id="93647-250">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="93647-251">configurationManagerComplianceRequired</span><span class="sxs-lookup"><span data-stu-id="93647-251">configurationManagerComplianceRequired</span></span>|<span data-ttu-id="93647-252">布尔</span><span class="sxs-lookup"><span data-stu-id="93647-252">Boolean</span></span>|<span data-ttu-id="93647-253">需要考虑将 SCCM 合规性状态考虑到 Intune 合规性状态。</span><span class="sxs-lookup"><span data-stu-id="93647-253">Require to consider SCCM Compliance state into consideration for Intune Compliance State.</span></span>|
|<span data-ttu-id="93647-254">tpmRequired</span><span class="sxs-lookup"><span data-stu-id="93647-254">tpmRequired</span></span>|<span data-ttu-id="93647-255">布尔</span><span class="sxs-lookup"><span data-stu-id="93647-255">Boolean</span></span>|<span data-ttu-id="93647-256">要求存在受信任的平台模块（TPM）。</span><span class="sxs-lookup"><span data-stu-id="93647-256">Require Trusted Platform Module(TPM) to be present.</span></span>|



## <a name="response"></a><span data-ttu-id="93647-257">响应</span><span class="sxs-lookup"><span data-stu-id="93647-257">Response</span></span>
<span data-ttu-id="93647-258">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和更新的 [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="93647-258">If successful, this method returns a `200 OK` response code and an updated [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="93647-259">示例</span><span class="sxs-lookup"><span data-stu-id="93647-259">Example</span></span>

### <a name="request"></a><span data-ttu-id="93647-260">请求</span><span class="sxs-lookup"><span data-stu-id="93647-260">Request</span></span>
<span data-ttu-id="93647-261">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="93647-261">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
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

### <a name="response"></a><span data-ttu-id="93647-262">响应</span><span class="sxs-lookup"><span data-stu-id="93647-262">Response</span></span>
<span data-ttu-id="93647-p112">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="93647-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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





