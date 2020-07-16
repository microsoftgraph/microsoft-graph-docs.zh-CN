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
# <a name="update-windows10compliancepolicy"></a><span data-ttu-id="fad71-103">更新 windows10CompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="fad71-103">Update windows10CompliancePolicy</span></span>

<span data-ttu-id="fad71-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fad71-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="fad71-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="fad71-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fad71-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="fad71-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fad71-107">更新 [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="fad71-107">Update the properties of a [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fad71-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="fad71-108">Prerequisites</span></span>
<span data-ttu-id="fad71-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="fad71-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fad71-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="fad71-111">Permission type</span></span>|<span data-ttu-id="fad71-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="fad71-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fad71-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="fad71-113">Delegated (work or school account)</span></span>|<span data-ttu-id="fad71-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fad71-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="fad71-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="fad71-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fad71-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="fad71-116">Not supported.</span></span>|
|<span data-ttu-id="fad71-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="fad71-117">Application</span></span>|<span data-ttu-id="fad71-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fad71-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="fad71-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="fad71-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="fad71-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="fad71-120">Request headers</span></span>
|<span data-ttu-id="fad71-121">标头</span><span class="sxs-lookup"><span data-stu-id="fad71-121">Header</span></span>|<span data-ttu-id="fad71-122">值</span><span class="sxs-lookup"><span data-stu-id="fad71-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fad71-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="fad71-123">Authorization</span></span>|<span data-ttu-id="fad71-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="fad71-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fad71-125">接受</span><span class="sxs-lookup"><span data-stu-id="fad71-125">Accept</span></span>|<span data-ttu-id="fad71-126">application/json</span><span class="sxs-lookup"><span data-stu-id="fad71-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fad71-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="fad71-127">Request body</span></span>
<span data-ttu-id="fad71-128">在请求正文中，提供 [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="fad71-128">In the request body, supply a JSON representation for the [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) object.</span></span>

<span data-ttu-id="fad71-129">下表显示创建 [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="fad71-129">The following table shows the properties that are required when you create the [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md).</span></span>

|<span data-ttu-id="fad71-130">属性</span><span class="sxs-lookup"><span data-stu-id="fad71-130">Property</span></span>|<span data-ttu-id="fad71-131">类型</span><span class="sxs-lookup"><span data-stu-id="fad71-131">Type</span></span>|<span data-ttu-id="fad71-132">说明</span><span class="sxs-lookup"><span data-stu-id="fad71-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fad71-133">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="fad71-133">roleScopeTagIds</span></span>|<span data-ttu-id="fad71-134">String collection</span><span class="sxs-lookup"><span data-stu-id="fad71-134">String collection</span></span>|<span data-ttu-id="fad71-135">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="fad71-135">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="fad71-136">继承自 [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="fad71-136">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="fad71-137">id</span><span class="sxs-lookup"><span data-stu-id="fad71-137">id</span></span>|<span data-ttu-id="fad71-138">字符串</span><span class="sxs-lookup"><span data-stu-id="fad71-138">String</span></span>|<span data-ttu-id="fad71-139">实体的键。</span><span class="sxs-lookup"><span data-stu-id="fad71-139">Key of the entity.</span></span> <span data-ttu-id="fad71-140">继承自 [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="fad71-140">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="fad71-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="fad71-141">createdDateTime</span></span>|<span data-ttu-id="fad71-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fad71-142">DateTimeOffset</span></span>|<span data-ttu-id="fad71-143">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="fad71-143">DateTime the object was created.</span></span> <span data-ttu-id="fad71-144">继承自 [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="fad71-144">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="fad71-145">说明</span><span class="sxs-lookup"><span data-stu-id="fad71-145">description</span></span>|<span data-ttu-id="fad71-146">String</span><span class="sxs-lookup"><span data-stu-id="fad71-146">String</span></span>|<span data-ttu-id="fad71-147">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="fad71-147">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="fad71-148">继承自 [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="fad71-148">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="fad71-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="fad71-149">lastModifiedDateTime</span></span>|<span data-ttu-id="fad71-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fad71-150">DateTimeOffset</span></span>|<span data-ttu-id="fad71-151">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="fad71-151">DateTime the object was last modified.</span></span> <span data-ttu-id="fad71-152">继承自 [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="fad71-152">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="fad71-153">displayName</span><span class="sxs-lookup"><span data-stu-id="fad71-153">displayName</span></span>|<span data-ttu-id="fad71-154">字符串</span><span class="sxs-lookup"><span data-stu-id="fad71-154">String</span></span>|<span data-ttu-id="fad71-155">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="fad71-155">Admin provided name of the device configuration.</span></span> <span data-ttu-id="fad71-156">继承自 [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="fad71-156">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="fad71-157">version</span><span class="sxs-lookup"><span data-stu-id="fad71-157">version</span></span>|<span data-ttu-id="fad71-158">Int32</span><span class="sxs-lookup"><span data-stu-id="fad71-158">Int32</span></span>|<span data-ttu-id="fad71-159">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="fad71-159">Version of the device configuration.</span></span> <span data-ttu-id="fad71-160">继承自 [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="fad71-160">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="fad71-161">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="fad71-161">passwordRequired</span></span>|<span data-ttu-id="fad71-162">布尔值</span><span class="sxs-lookup"><span data-stu-id="fad71-162">Boolean</span></span>|<span data-ttu-id="fad71-163">需要密码才可解锁 Windows 设备。</span><span class="sxs-lookup"><span data-stu-id="fad71-163">Require a password to unlock Windows device.</span></span>|
|<span data-ttu-id="fad71-164">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="fad71-164">passwordBlockSimple</span></span>|<span data-ttu-id="fad71-165">布尔值</span><span class="sxs-lookup"><span data-stu-id="fad71-165">Boolean</span></span>|<span data-ttu-id="fad71-166">指示是否阻止简单密码。</span><span class="sxs-lookup"><span data-stu-id="fad71-166">Indicates whether or not to block simple password.</span></span>|
|<span data-ttu-id="fad71-167">passwordRequiredToUnlockFromIdle</span><span class="sxs-lookup"><span data-stu-id="fad71-167">passwordRequiredToUnlockFromIdle</span></span>|<span data-ttu-id="fad71-168">布尔值</span><span class="sxs-lookup"><span data-stu-id="fad71-168">Boolean</span></span>|<span data-ttu-id="fad71-169">需要密码才可解锁空闲设备。</span><span class="sxs-lookup"><span data-stu-id="fad71-169">Require a password to unlock an idle device.</span></span>|
|<span data-ttu-id="fad71-170">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="fad71-170">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="fad71-171">Int32</span><span class="sxs-lookup"><span data-stu-id="fad71-171">Int32</span></span>|<span data-ttu-id="fad71-172">在需要密码之前不活动的分钟数。</span><span class="sxs-lookup"><span data-stu-id="fad71-172">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="fad71-173">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="fad71-173">passwordExpirationDays</span></span>|<span data-ttu-id="fad71-174">Int32</span><span class="sxs-lookup"><span data-stu-id="fad71-174">Int32</span></span>|<span data-ttu-id="fad71-175">密码过期天数。</span><span class="sxs-lookup"><span data-stu-id="fad71-175">The password expiration in days.</span></span>|
|<span data-ttu-id="fad71-176">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="fad71-176">passwordMinimumLength</span></span>|<span data-ttu-id="fad71-177">Int32</span><span class="sxs-lookup"><span data-stu-id="fad71-177">Int32</span></span>|<span data-ttu-id="fad71-178">密码最短长度。</span><span class="sxs-lookup"><span data-stu-id="fad71-178">The minimum password length.</span></span>|
|<span data-ttu-id="fad71-179">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="fad71-179">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="fad71-180">Int32</span><span class="sxs-lookup"><span data-stu-id="fad71-180">Int32</span></span>|<span data-ttu-id="fad71-181">密码中必需的字符集数。</span><span class="sxs-lookup"><span data-stu-id="fad71-181">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="fad71-182">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="fad71-182">passwordRequiredType</span></span>|[<span data-ttu-id="fad71-183">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="fad71-183">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="fad71-184">必需的密码类型。</span><span class="sxs-lookup"><span data-stu-id="fad71-184">The required password type.</span></span> <span data-ttu-id="fad71-185">可取值为：`deviceDefault`、`alphanumeric`、`numeric`。</span><span class="sxs-lookup"><span data-stu-id="fad71-185">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="fad71-186">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="fad71-186">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="fad71-187">Int32</span><span class="sxs-lookup"><span data-stu-id="fad71-187">Int32</span></span>|<span data-ttu-id="fad71-188">防止重复使用的先前密码的数量。</span><span class="sxs-lookup"><span data-stu-id="fad71-188">The number of previous passwords to prevent re-use of.</span></span>|
|<span data-ttu-id="fad71-189">requireHealthyDeviceReport</span><span class="sxs-lookup"><span data-stu-id="fad71-189">requireHealthyDeviceReport</span></span>|<span data-ttu-id="fad71-190">布尔值</span><span class="sxs-lookup"><span data-stu-id="fad71-190">Boolean</span></span>|<span data-ttu-id="fad71-191">要求设备由 Windows 设备运行状况证明报告为正常。</span><span class="sxs-lookup"><span data-stu-id="fad71-191">Require devices to be reported as healthy by Windows Device Health Attestation.</span></span>|
|<span data-ttu-id="fad71-192">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="fad71-192">osMinimumVersion</span></span>|<span data-ttu-id="fad71-193">String</span><span class="sxs-lookup"><span data-stu-id="fad71-193">String</span></span>|<span data-ttu-id="fad71-194">最低 Windows 10 版本。</span><span class="sxs-lookup"><span data-stu-id="fad71-194">Minimum Windows 10 version.</span></span>|
|<span data-ttu-id="fad71-195">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="fad71-195">osMaximumVersion</span></span>|<span data-ttu-id="fad71-196">String</span><span class="sxs-lookup"><span data-stu-id="fad71-196">String</span></span>|<span data-ttu-id="fad71-197">最高 Windows 10 版本。</span><span class="sxs-lookup"><span data-stu-id="fad71-197">Maximum Windows 10 version.</span></span>|
|<span data-ttu-id="fad71-198">mobileOsMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="fad71-198">mobileOsMinimumVersion</span></span>|<span data-ttu-id="fad71-199">String</span><span class="sxs-lookup"><span data-stu-id="fad71-199">String</span></span>|<span data-ttu-id="fad71-200">最低 Windows Phone 版本。</span><span class="sxs-lookup"><span data-stu-id="fad71-200">Minimum Windows Phone version.</span></span>|
|<span data-ttu-id="fad71-201">mobileOsMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="fad71-201">mobileOsMaximumVersion</span></span>|<span data-ttu-id="fad71-202">String</span><span class="sxs-lookup"><span data-stu-id="fad71-202">String</span></span>|<span data-ttu-id="fad71-203">最高 Windows Phone 版本。</span><span class="sxs-lookup"><span data-stu-id="fad71-203">Maximum Windows Phone version.</span></span>|
|<span data-ttu-id="fad71-204">earlyLaunchAntiMalwareDriverEnabled</span><span class="sxs-lookup"><span data-stu-id="fad71-204">earlyLaunchAntiMalwareDriverEnabled</span></span>|<span data-ttu-id="fad71-205">布尔值</span><span class="sxs-lookup"><span data-stu-id="fad71-205">Boolean</span></span>|<span data-ttu-id="fad71-206">要求设备由 Windows 设备运行状况证明报告为正常 - 提前启动反恶意驱动程序已启用。</span><span class="sxs-lookup"><span data-stu-id="fad71-206">Require devices to be reported as healthy by Windows Device Health Attestation - early launch antimalware driver is enabled.</span></span>|
|<span data-ttu-id="fad71-207">bitLockerEnabled</span><span class="sxs-lookup"><span data-stu-id="fad71-207">bitLockerEnabled</span></span>|<span data-ttu-id="fad71-208">布尔值</span><span class="sxs-lookup"><span data-stu-id="fad71-208">Boolean</span></span>|<span data-ttu-id="fad71-209">要求设备由 Windows 设备运行状况证明报告为正常 - bit locker 已启用。</span><span class="sxs-lookup"><span data-stu-id="fad71-209">Require devices to be reported healthy by Windows Device Health Attestation - bit locker is enabled</span></span>|
|<span data-ttu-id="fad71-210">secureBootEnabled</span><span class="sxs-lookup"><span data-stu-id="fad71-210">secureBootEnabled</span></span>|<span data-ttu-id="fad71-211">布尔值</span><span class="sxs-lookup"><span data-stu-id="fad71-211">Boolean</span></span>|<span data-ttu-id="fad71-212">要求设备由 Windows 设备运行状况证明报告为正常 - 安全启动已启用。</span><span class="sxs-lookup"><span data-stu-id="fad71-212">Require devices to be reported as healthy by Windows Device Health Attestation - secure boot is enabled.</span></span>|
|<span data-ttu-id="fad71-213">codeIntegrityEnabled</span><span class="sxs-lookup"><span data-stu-id="fad71-213">codeIntegrityEnabled</span></span>|<span data-ttu-id="fad71-214">Boolean</span><span class="sxs-lookup"><span data-stu-id="fad71-214">Boolean</span></span>|<span data-ttu-id="fad71-215">要求设备由 Windows 设备运行状况证明报告为正常。</span><span class="sxs-lookup"><span data-stu-id="fad71-215">Require devices to be reported as healthy by Windows Device Health Attestation.</span></span>|
|<span data-ttu-id="fad71-216">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="fad71-216">storageRequireEncryption</span></span>|<span data-ttu-id="fad71-217">Boolean</span><span class="sxs-lookup"><span data-stu-id="fad71-217">Boolean</span></span>|<span data-ttu-id="fad71-218">要求对 Windows 设备加密。</span><span class="sxs-lookup"><span data-stu-id="fad71-218">Require encryption on windows devices.</span></span>|
|<span data-ttu-id="fad71-219">activeFirewallRequired</span><span class="sxs-lookup"><span data-stu-id="fad71-219">activeFirewallRequired</span></span>|<span data-ttu-id="fad71-220">布尔值</span><span class="sxs-lookup"><span data-stu-id="fad71-220">Boolean</span></span>|<span data-ttu-id="fad71-221">在 Windows 设备上需要活动防火墙。</span><span class="sxs-lookup"><span data-stu-id="fad71-221">Require active firewall on Windows devices.</span></span>|
|<span data-ttu-id="fad71-222">defenderEnabled</span><span class="sxs-lookup"><span data-stu-id="fad71-222">defenderEnabled</span></span>|<span data-ttu-id="fad71-223">布尔值</span><span class="sxs-lookup"><span data-stu-id="fad71-223">Boolean</span></span>|<span data-ttu-id="fad71-224">在 Windows 设备上需要 Windows Defender 反恶意软件。</span><span class="sxs-lookup"><span data-stu-id="fad71-224">Require Windows Defender Antimalware on Windows devices.</span></span>|
|<span data-ttu-id="fad71-225">defenderVersion</span><span class="sxs-lookup"><span data-stu-id="fad71-225">defenderVersion</span></span>|<span data-ttu-id="fad71-226">String</span><span class="sxs-lookup"><span data-stu-id="fad71-226">String</span></span>|<span data-ttu-id="fad71-227">在 Windows 设备上要求 Windows Defender 反恶意软件的最低版本。</span><span class="sxs-lookup"><span data-stu-id="fad71-227">Require Windows Defender Antimalware minimum version on Windows devices.</span></span>|
|<span data-ttu-id="fad71-228">signatureOutOfDate</span><span class="sxs-lookup"><span data-stu-id="fad71-228">signatureOutOfDate</span></span>|<span data-ttu-id="fad71-229">布尔值</span><span class="sxs-lookup"><span data-stu-id="fad71-229">Boolean</span></span>|<span data-ttu-id="fad71-230">Windows 设备上要求 Windows Defender 反恶意软件签名为最新。</span><span class="sxs-lookup"><span data-stu-id="fad71-230">Require Windows Defender Antimalware Signature to be up to date on Windows devices.</span></span>|
|<span data-ttu-id="fad71-231">rtpEnabled</span><span class="sxs-lookup"><span data-stu-id="fad71-231">rtpEnabled</span></span>|<span data-ttu-id="fad71-232">布尔值</span><span class="sxs-lookup"><span data-stu-id="fad71-232">Boolean</span></span>|<span data-ttu-id="fad71-233">在 Windows 设备上需要 Windows Defender 反恶意软件实时保护。</span><span class="sxs-lookup"><span data-stu-id="fad71-233">Require Windows Defender Antimalware Real-Time Protection on Windows devices.</span></span>|
|<span data-ttu-id="fad71-234">antivirusRequired</span><span class="sxs-lookup"><span data-stu-id="fad71-234">antivirusRequired</span></span>|<span data-ttu-id="fad71-235">布尔值</span><span class="sxs-lookup"><span data-stu-id="fad71-235">Boolean</span></span>|<span data-ttu-id="fad71-236">要求在 Windows Decurity Center 中注册的任何防病毒解决方案都处于启用和监控（例如，Symantec、Windows Defender）。</span><span class="sxs-lookup"><span data-stu-id="fad71-236">Require any Antivirus solution registered with Windows Decurity Center to be on and monitoring (e.g. Symantec, Windows Defender).</span></span>|
|<span data-ttu-id="fad71-237">antiSpywareRequired</span><span class="sxs-lookup"><span data-stu-id="fad71-237">antiSpywareRequired</span></span>|<span data-ttu-id="fad71-238">布尔值</span><span class="sxs-lookup"><span data-stu-id="fad71-238">Boolean</span></span>|<span data-ttu-id="fad71-239">要求在 Windows Decurity Center 中注册的任何反间谍软件解决方案都处于启用和监控（例如，Symantec、Windows Defender）。</span><span class="sxs-lookup"><span data-stu-id="fad71-239">Require any AntiSpyware solution registered with Windows Decurity Center to be on and monitoring (e.g. Symantec, Windows Defender).</span></span>|
|<span data-ttu-id="fad71-240">validOperatingSystemBuildRanges</span><span class="sxs-lookup"><span data-stu-id="fad71-240">validOperatingSystemBuildRanges</span></span>|<span data-ttu-id="fad71-241">[operatingSystemVersionRange](../resources/intune-deviceconfig-operatingsystemversionrange.md)集合</span><span class="sxs-lookup"><span data-stu-id="fad71-241">[operatingSystemVersionRange](../resources/intune-deviceconfig-operatingsystemversionrange.md) collection</span></span>|<span data-ttu-id="fad71-242">Windows 设备上的有效操作系统内部版本范围。</span><span class="sxs-lookup"><span data-stu-id="fad71-242">The valid operating system build ranges on Windows devices.</span></span> <span data-ttu-id="fad71-243">该集合最多可包含 10000 个元素。</span><span class="sxs-lookup"><span data-stu-id="fad71-243">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="fad71-244">deviceThreatProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="fad71-244">deviceThreatProtectionEnabled</span></span>|<span data-ttu-id="fad71-245">Boolean</span><span class="sxs-lookup"><span data-stu-id="fad71-245">Boolean</span></span>|<span data-ttu-id="fad71-246">要求设备已启用设备威胁防护。</span><span class="sxs-lookup"><span data-stu-id="fad71-246">Require that devices have enabled device threat protection.</span></span>|
|<span data-ttu-id="fad71-247">deviceThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="fad71-247">deviceThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="fad71-248">deviceThreatProtectionLevel</span><span class="sxs-lookup"><span data-stu-id="fad71-248">deviceThreatProtectionLevel</span></span>](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|<span data-ttu-id="fad71-249">需要设备威胁防护最低风险级别来报告不合规。</span><span class="sxs-lookup"><span data-stu-id="fad71-249">Require Device Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="fad71-250">可取值为：`unavailable`、`secured`、`low`、`medium`、`high`、`notSet`。</span><span class="sxs-lookup"><span data-stu-id="fad71-250">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="fad71-251">configurationManagerComplianceRequired</span><span class="sxs-lookup"><span data-stu-id="fad71-251">configurationManagerComplianceRequired</span></span>|<span data-ttu-id="fad71-252">布尔值</span><span class="sxs-lookup"><span data-stu-id="fad71-252">Boolean</span></span>|<span data-ttu-id="fad71-253">需要考虑将 SCCM 合规性状态考虑到 Intune 合规性状态。</span><span class="sxs-lookup"><span data-stu-id="fad71-253">Require to consider SCCM Compliance state into consideration for Intune Compliance State.</span></span>|
|<span data-ttu-id="fad71-254">tpmRequired</span><span class="sxs-lookup"><span data-stu-id="fad71-254">tpmRequired</span></span>|<span data-ttu-id="fad71-255">布尔值</span><span class="sxs-lookup"><span data-stu-id="fad71-255">Boolean</span></span>|<span data-ttu-id="fad71-256">要求存在受信任的平台模块（TPM）。</span><span class="sxs-lookup"><span data-stu-id="fad71-256">Require Trusted Platform Module(TPM) to be present.</span></span>|
|<span data-ttu-id="fad71-257">deviceCompliancePolicyScript</span><span class="sxs-lookup"><span data-stu-id="fad71-257">deviceCompliancePolicyScript</span></span>|[<span data-ttu-id="fad71-258">deviceCompliancePolicyScript</span><span class="sxs-lookup"><span data-stu-id="fad71-258">deviceCompliancePolicyScript</span></span>](../resources/intune-deviceconfig-devicecompliancepolicyscript.md)|<span data-ttu-id="fad71-259">尚未记录</span><span class="sxs-lookup"><span data-stu-id="fad71-259">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="fad71-260">响应</span><span class="sxs-lookup"><span data-stu-id="fad71-260">Response</span></span>
<span data-ttu-id="fad71-261">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和更新的 [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="fad71-261">If successful, this method returns a `200 OK` response code and an updated [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fad71-262">示例</span><span class="sxs-lookup"><span data-stu-id="fad71-262">Example</span></span>

### <a name="request"></a><span data-ttu-id="fad71-263">请求</span><span class="sxs-lookup"><span data-stu-id="fad71-263">Request</span></span>
<span data-ttu-id="fad71-264">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="fad71-264">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="fad71-265">响应</span><span class="sxs-lookup"><span data-stu-id="fad71-265">Response</span></span>
<span data-ttu-id="fad71-p112">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="fad71-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



