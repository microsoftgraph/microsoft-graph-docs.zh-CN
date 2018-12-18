---
title: 更新 windows10CompliancePolicy
description: 更新 windows10CompliancePolicy 对象的属性。
author: tfitzmac
ms.openlocfilehash: d80bcd8852a21a1aac216fdee283fb6ba61b461e
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27333395"
---
# <a name="update-windows10compliancepolicy"></a><span data-ttu-id="460e9-103">更新 windows10CompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="460e9-103">Update windows10CompliancePolicy</span></span>

> <span data-ttu-id="460e9-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="460e9-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="460e9-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="460e9-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="460e9-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="460e9-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="460e9-107">更新 [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="460e9-107">Update the properties of a [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="460e9-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="460e9-108">Prerequisites</span></span>
<span data-ttu-id="460e9-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="460e9-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="460e9-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="460e9-111">Permission type</span></span>|<span data-ttu-id="460e9-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="460e9-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="460e9-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="460e9-113">Delegated (work or school account)</span></span>|<span data-ttu-id="460e9-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="460e9-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="460e9-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="460e9-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="460e9-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="460e9-116">Not supported.</span></span>|
|<span data-ttu-id="460e9-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="460e9-117">Application</span></span>|<span data-ttu-id="460e9-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="460e9-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="460e9-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="460e9-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="460e9-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="460e9-120">Request headers</span></span>
|<span data-ttu-id="460e9-121">标头</span><span class="sxs-lookup"><span data-stu-id="460e9-121">Header</span></span>|<span data-ttu-id="460e9-122">值</span><span class="sxs-lookup"><span data-stu-id="460e9-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="460e9-123">授权</span><span class="sxs-lookup"><span data-stu-id="460e9-123">Authorization</span></span>|<span data-ttu-id="460e9-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="460e9-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="460e9-125">Accept</span><span class="sxs-lookup"><span data-stu-id="460e9-125">Accept</span></span>|<span data-ttu-id="460e9-126">application/json</span><span class="sxs-lookup"><span data-stu-id="460e9-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="460e9-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="460e9-127">Request body</span></span>
<span data-ttu-id="460e9-128">在请求正文中，提供 [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="460e9-128">In the request body, supply a JSON representation for the [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) object.</span></span>

<span data-ttu-id="460e9-129">下表显示创建 [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="460e9-129">The following table shows the properties that are required when you create the [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md).</span></span>

|<span data-ttu-id="460e9-130">属性</span><span class="sxs-lookup"><span data-stu-id="460e9-130">Property</span></span>|<span data-ttu-id="460e9-131">类型</span><span class="sxs-lookup"><span data-stu-id="460e9-131">Type</span></span>|<span data-ttu-id="460e9-132">说明</span><span class="sxs-lookup"><span data-stu-id="460e9-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="460e9-133">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="460e9-133">roleScopeTagIds</span></span>|<span data-ttu-id="460e9-134">String 集合</span><span class="sxs-lookup"><span data-stu-id="460e9-134">String collection</span></span>|<span data-ttu-id="460e9-135">此实体实例范围标记的列表。</span><span class="sxs-lookup"><span data-stu-id="460e9-135">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="460e9-136">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="460e9-136">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="460e9-137">id</span><span class="sxs-lookup"><span data-stu-id="460e9-137">id</span></span>|<span data-ttu-id="460e9-138">String</span><span class="sxs-lookup"><span data-stu-id="460e9-138">String</span></span>|<span data-ttu-id="460e9-139">实体的键。</span><span class="sxs-lookup"><span data-stu-id="460e9-139">Key of the entity.</span></span> <span data-ttu-id="460e9-140">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="460e9-140">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="460e9-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="460e9-141">createdDateTime</span></span>|<span data-ttu-id="460e9-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="460e9-142">DateTimeOffset</span></span>|<span data-ttu-id="460e9-143">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="460e9-143">DateTime the object was created.</span></span> <span data-ttu-id="460e9-144">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="460e9-144">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="460e9-145">description</span><span class="sxs-lookup"><span data-stu-id="460e9-145">description</span></span>|<span data-ttu-id="460e9-146">String</span><span class="sxs-lookup"><span data-stu-id="460e9-146">String</span></span>|<span data-ttu-id="460e9-147">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="460e9-147">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="460e9-148">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="460e9-148">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="460e9-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="460e9-149">lastModifiedDateTime</span></span>|<span data-ttu-id="460e9-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="460e9-150">DateTimeOffset</span></span>|<span data-ttu-id="460e9-151">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="460e9-151">DateTime the object was last modified.</span></span> <span data-ttu-id="460e9-152">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="460e9-152">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="460e9-153">displayName</span><span class="sxs-lookup"><span data-stu-id="460e9-153">displayName</span></span>|<span data-ttu-id="460e9-154">String</span><span class="sxs-lookup"><span data-stu-id="460e9-154">String</span></span>|<span data-ttu-id="460e9-155">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="460e9-155">Admin provided name of the device configuration.</span></span> <span data-ttu-id="460e9-156">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="460e9-156">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="460e9-157">version</span><span class="sxs-lookup"><span data-stu-id="460e9-157">version</span></span>|<span data-ttu-id="460e9-158">Int32</span><span class="sxs-lookup"><span data-stu-id="460e9-158">Int32</span></span>|<span data-ttu-id="460e9-159">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="460e9-159">Version of the device configuration.</span></span> <span data-ttu-id="460e9-160">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="460e9-160">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="460e9-161">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="460e9-161">passwordRequired</span></span>|<span data-ttu-id="460e9-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="460e9-162">Boolean</span></span>|<span data-ttu-id="460e9-163">需要密码才可解锁 Windows 设备。</span><span class="sxs-lookup"><span data-stu-id="460e9-163">Require a password to unlock Windows device.</span></span>|
|<span data-ttu-id="460e9-164">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="460e9-164">passwordBlockSimple</span></span>|<span data-ttu-id="460e9-165">Boolean</span><span class="sxs-lookup"><span data-stu-id="460e9-165">Boolean</span></span>|<span data-ttu-id="460e9-166">指示是否阻止简单密码。</span><span class="sxs-lookup"><span data-stu-id="460e9-166">Indicates whether or not to block simple password.</span></span>|
|<span data-ttu-id="460e9-167">passwordRequiredToUnlockFromIdle</span><span class="sxs-lookup"><span data-stu-id="460e9-167">passwordRequiredToUnlockFromIdle</span></span>|<span data-ttu-id="460e9-168">Boolean</span><span class="sxs-lookup"><span data-stu-id="460e9-168">Boolean</span></span>|<span data-ttu-id="460e9-169">需要密码才可解锁空闲设备。</span><span class="sxs-lookup"><span data-stu-id="460e9-169">Require a password to unlock an idle device.</span></span>|
|<span data-ttu-id="460e9-170">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="460e9-170">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="460e9-171">Int32</span><span class="sxs-lookup"><span data-stu-id="460e9-171">Int32</span></span>|<span data-ttu-id="460e9-172">在需要密码之前不活动的分钟数。</span><span class="sxs-lookup"><span data-stu-id="460e9-172">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="460e9-173">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="460e9-173">passwordExpirationDays</span></span>|<span data-ttu-id="460e9-174">Int32</span><span class="sxs-lookup"><span data-stu-id="460e9-174">Int32</span></span>|<span data-ttu-id="460e9-175">密码过期天数。</span><span class="sxs-lookup"><span data-stu-id="460e9-175">The password expiration in days.</span></span>|
|<span data-ttu-id="460e9-176">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="460e9-176">passwordMinimumLength</span></span>|<span data-ttu-id="460e9-177">Int32</span><span class="sxs-lookup"><span data-stu-id="460e9-177">Int32</span></span>|<span data-ttu-id="460e9-178">密码最短长度。</span><span class="sxs-lookup"><span data-stu-id="460e9-178">The minimum password length.</span></span>|
|<span data-ttu-id="460e9-179">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="460e9-179">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="460e9-180">Int32</span><span class="sxs-lookup"><span data-stu-id="460e9-180">Int32</span></span>|<span data-ttu-id="460e9-181">密码中必需的字符集数。</span><span class="sxs-lookup"><span data-stu-id="460e9-181">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="460e9-182">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="460e9-182">passwordRequiredType</span></span>|[<span data-ttu-id="460e9-183">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="460e9-183">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="460e9-184">必需的密码类型。</span><span class="sxs-lookup"><span data-stu-id="460e9-184">The required password type.</span></span> <span data-ttu-id="460e9-185">可取值为：`deviceDefault`、`alphanumeric`、`numeric`。</span><span class="sxs-lookup"><span data-stu-id="460e9-185">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="460e9-186">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="460e9-186">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="460e9-187">Int32</span><span class="sxs-lookup"><span data-stu-id="460e9-187">Int32</span></span>|<span data-ttu-id="460e9-188">防止重复使用的先前密码的数量。</span><span class="sxs-lookup"><span data-stu-id="460e9-188">The number of previous passwords to prevent re-use of.</span></span>|
|<span data-ttu-id="460e9-189">requireHealthyDeviceReport</span><span class="sxs-lookup"><span data-stu-id="460e9-189">requireHealthyDeviceReport</span></span>|<span data-ttu-id="460e9-190">Boolean</span><span class="sxs-lookup"><span data-stu-id="460e9-190">Boolean</span></span>|<span data-ttu-id="460e9-191">要求设备由 Windows 设备运行状况证明报告为正常。</span><span class="sxs-lookup"><span data-stu-id="460e9-191">Require devices to be reported as healthy by Windows Device Health Attestation.</span></span>|
|<span data-ttu-id="460e9-192">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="460e9-192">osMinimumVersion</span></span>|<span data-ttu-id="460e9-193">String</span><span class="sxs-lookup"><span data-stu-id="460e9-193">String</span></span>|<span data-ttu-id="460e9-194">最低 Windows 10 版本。</span><span class="sxs-lookup"><span data-stu-id="460e9-194">Minimum Windows 10 version.</span></span>|
|<span data-ttu-id="460e9-195">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="460e9-195">osMaximumVersion</span></span>|<span data-ttu-id="460e9-196">String</span><span class="sxs-lookup"><span data-stu-id="460e9-196">String</span></span>|<span data-ttu-id="460e9-197">最高 Windows 10 版本。</span><span class="sxs-lookup"><span data-stu-id="460e9-197">Maximum Windows 10 version.</span></span>|
|<span data-ttu-id="460e9-198">mobileOsMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="460e9-198">mobileOsMinimumVersion</span></span>|<span data-ttu-id="460e9-199">String</span><span class="sxs-lookup"><span data-stu-id="460e9-199">String</span></span>|<span data-ttu-id="460e9-200">最低 Windows Phone 版本。</span><span class="sxs-lookup"><span data-stu-id="460e9-200">Minimum Windows Phone version.</span></span>|
|<span data-ttu-id="460e9-201">mobileOsMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="460e9-201">mobileOsMaximumVersion</span></span>|<span data-ttu-id="460e9-202">String</span><span class="sxs-lookup"><span data-stu-id="460e9-202">String</span></span>|<span data-ttu-id="460e9-203">最高 Windows Phone 版本。</span><span class="sxs-lookup"><span data-stu-id="460e9-203">Maximum Windows Phone version.</span></span>|
|<span data-ttu-id="460e9-204">earlyLaunchAntiMalwareDriverEnabled</span><span class="sxs-lookup"><span data-stu-id="460e9-204">earlyLaunchAntiMalwareDriverEnabled</span></span>|<span data-ttu-id="460e9-205">Boolean</span><span class="sxs-lookup"><span data-stu-id="460e9-205">Boolean</span></span>|<span data-ttu-id="460e9-206">要求设备由 Windows 设备运行状况证明报告为正常 - 提前启动反恶意驱动程序已启用。</span><span class="sxs-lookup"><span data-stu-id="460e9-206">Require devices to be reported as healthy by Windows Device Health Attestation - early launch antimalware driver is enabled.</span></span>|
|<span data-ttu-id="460e9-207">bitLockerEnabled</span><span class="sxs-lookup"><span data-stu-id="460e9-207">bitLockerEnabled</span></span>|<span data-ttu-id="460e9-208">Boolean</span><span class="sxs-lookup"><span data-stu-id="460e9-208">Boolean</span></span>|<span data-ttu-id="460e9-209">要求设备由 Windows 设备运行状况证明报告为正常 - bit locker 已启用。</span><span class="sxs-lookup"><span data-stu-id="460e9-209">Require devices to be reported healthy by Windows Device Health Attestation - bit locker is enabled</span></span>|
|<span data-ttu-id="460e9-210">secureBootEnabled</span><span class="sxs-lookup"><span data-stu-id="460e9-210">secureBootEnabled</span></span>|<span data-ttu-id="460e9-211">Boolean</span><span class="sxs-lookup"><span data-stu-id="460e9-211">Boolean</span></span>|<span data-ttu-id="460e9-212">要求设备由 Windows 设备运行状况证明报告为正常 - 安全启动已启用。</span><span class="sxs-lookup"><span data-stu-id="460e9-212">Require devices to be reported as healthy by Windows Device Health Attestation - secure boot is enabled.</span></span>|
|<span data-ttu-id="460e9-213">codeIntegrityEnabled</span><span class="sxs-lookup"><span data-stu-id="460e9-213">codeIntegrityEnabled</span></span>|<span data-ttu-id="460e9-214">Boolean</span><span class="sxs-lookup"><span data-stu-id="460e9-214">Boolean</span></span>|<span data-ttu-id="460e9-215">要求设备由 Windows 设备运行状况证明报告为正常。</span><span class="sxs-lookup"><span data-stu-id="460e9-215">Require devices to be reported as healthy by Windows Device Health Attestation.</span></span>|
|<span data-ttu-id="460e9-216">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="460e9-216">storageRequireEncryption</span></span>|<span data-ttu-id="460e9-217">Boolean</span><span class="sxs-lookup"><span data-stu-id="460e9-217">Boolean</span></span>|<span data-ttu-id="460e9-218">要求对 Windows 设备加密。</span><span class="sxs-lookup"><span data-stu-id="460e9-218">Require encryption on windows devices.</span></span>|
|<span data-ttu-id="460e9-219">activeFirewallRequired</span><span class="sxs-lookup"><span data-stu-id="460e9-219">activeFirewallRequired</span></span>|<span data-ttu-id="460e9-220">Boolean</span><span class="sxs-lookup"><span data-stu-id="460e9-220">Boolean</span></span>|<span data-ttu-id="460e9-221">要求在 Windows 设备上的活动防火墙。</span><span class="sxs-lookup"><span data-stu-id="460e9-221">Require active firewall on Windows devices.</span></span>|
|<span data-ttu-id="460e9-222">defenderEnabled</span><span class="sxs-lookup"><span data-stu-id="460e9-222">defenderEnabled</span></span>|<span data-ttu-id="460e9-223">Boolean</span><span class="sxs-lookup"><span data-stu-id="460e9-223">Boolean</span></span>|<span data-ttu-id="460e9-224">在 Windows 设备上需要 Windows Defender 反恶意软件。</span><span class="sxs-lookup"><span data-stu-id="460e9-224">Require Windows Defender Antimalware on Windows devices.</span></span>|
|<span data-ttu-id="460e9-225">defenderVersion</span><span class="sxs-lookup"><span data-stu-id="460e9-225">defenderVersion</span></span>|<span data-ttu-id="460e9-226">字符串</span><span class="sxs-lookup"><span data-stu-id="460e9-226">String</span></span>|<span data-ttu-id="460e9-227">需要 Windows Defender 反恶意软件在 Windows 设备上的最低版本。</span><span class="sxs-lookup"><span data-stu-id="460e9-227">Require Windows Defender Antimalware minimum version on Windows devices.</span></span>|
|<span data-ttu-id="460e9-228">signatureOutOfDate</span><span class="sxs-lookup"><span data-stu-id="460e9-228">signatureOutOfDate</span></span>|<span data-ttu-id="460e9-229">Boolean</span><span class="sxs-lookup"><span data-stu-id="460e9-229">Boolean</span></span>|<span data-ttu-id="460e9-230">需要 Windows Defender 反恶意软件签名是最新 Windows 设备上。</span><span class="sxs-lookup"><span data-stu-id="460e9-230">Require Windows Defender Antimalware Signature to be up to date on Windows devices.</span></span>|
|<span data-ttu-id="460e9-231">rtpEnabled</span><span class="sxs-lookup"><span data-stu-id="460e9-231">rtpEnabled</span></span>|<span data-ttu-id="460e9-232">Boolean</span><span class="sxs-lookup"><span data-stu-id="460e9-232">Boolean</span></span>|<span data-ttu-id="460e9-233">在 Windows 设备上需要 Windows Defender 反恶意软件实时保护。</span><span class="sxs-lookup"><span data-stu-id="460e9-233">Require Windows Defender Antimalware Real-Time Protection on Windows devices.</span></span>|
|<span data-ttu-id="460e9-234">antivirusRequired</span><span class="sxs-lookup"><span data-stu-id="460e9-234">antivirusRequired</span></span>|<span data-ttu-id="460e9-235">Boolean</span><span class="sxs-lookup"><span data-stu-id="460e9-235">Boolean</span></span>|<span data-ttu-id="460e9-236">需要与 Windows Decurity 中心上注册和监视 (例如 Symantec，Windows Defender) 的任何防病毒解决方案。</span><span class="sxs-lookup"><span data-stu-id="460e9-236">Require any Antivirus solution registered with Windows Decurity Center to be on and monitoring (e.g. Symantec, Windows Defender).</span></span>|
|<span data-ttu-id="460e9-237">antiSpywareRequired</span><span class="sxs-lookup"><span data-stu-id="460e9-237">antiSpywareRequired</span></span>|<span data-ttu-id="460e9-238">Boolean</span><span class="sxs-lookup"><span data-stu-id="460e9-238">Boolean</span></span>|<span data-ttu-id="460e9-239">需要的任何反间谍软件解决方案注册 Windows Decurity 中心上为和监视 （例如 Symantec、 Windows Defender）。</span><span class="sxs-lookup"><span data-stu-id="460e9-239">Require any AntiSpyware solution registered with Windows Decurity Center to be on and monitoring (e.g. Symantec, Windows Defender).</span></span>|
|<span data-ttu-id="460e9-240">validOperatingSystemBuildRanges</span><span class="sxs-lookup"><span data-stu-id="460e9-240">validOperatingSystemBuildRanges</span></span>|<span data-ttu-id="460e9-241">[operatingSystemVersionRange](../resources/intune-deviceconfig-operatingsystemversionrange.md)集合</span><span class="sxs-lookup"><span data-stu-id="460e9-241">[operatingSystemVersionRange](../resources/intune-deviceconfig-operatingsystemversionrange.md) collection</span></span>|<span data-ttu-id="460e9-242">有效的操作系统构建 Windows 设备上的区域。</span><span class="sxs-lookup"><span data-stu-id="460e9-242">The valid operating system build ranges on Windows devices.</span></span> <span data-ttu-id="460e9-243">该集合最多可包含 10000 个元素。</span><span class="sxs-lookup"><span data-stu-id="460e9-243">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="460e9-244">deviceThreatProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="460e9-244">deviceThreatProtectionEnabled</span></span>|<span data-ttu-id="460e9-245">Boolean</span><span class="sxs-lookup"><span data-stu-id="460e9-245">Boolean</span></span>|<span data-ttu-id="460e9-246">要求设备已启用设备威胁防护。</span><span class="sxs-lookup"><span data-stu-id="460e9-246">Require that devices have enabled device threat protection.</span></span>|
|<span data-ttu-id="460e9-247">deviceThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="460e9-247">deviceThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="460e9-248">deviceThreatProtectionLevel</span><span class="sxs-lookup"><span data-stu-id="460e9-248">deviceThreatProtectionLevel</span></span>](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|<span data-ttu-id="460e9-249">要求设备威胁保护最低风险级别报告如此。</span><span class="sxs-lookup"><span data-stu-id="460e9-249">Require Device Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="460e9-250">可取值为：`unavailable`、`secured`、`low`、`medium`、`high`、`notSet`。</span><span class="sxs-lookup"><span data-stu-id="460e9-250">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="460e9-251">configurationManagerComplianceRequired</span><span class="sxs-lookup"><span data-stu-id="460e9-251">configurationManagerComplianceRequired</span></span>|<span data-ttu-id="460e9-252">Boolean</span><span class="sxs-lookup"><span data-stu-id="460e9-252">Boolean</span></span>|<span data-ttu-id="460e9-253">需要考虑 Intune 合规性状态考虑 SCCM 合规性状态。</span><span class="sxs-lookup"><span data-stu-id="460e9-253">Require to consider SCCM Compliance state into consideration for Intune Compliance State.</span></span>|



## <a name="response"></a><span data-ttu-id="460e9-254">响应</span><span class="sxs-lookup"><span data-stu-id="460e9-254">Response</span></span>
<span data-ttu-id="460e9-255">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和更新的 [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="460e9-255">If successful, this method returns a `200 OK` response code and an updated [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="460e9-256">示例</span><span class="sxs-lookup"><span data-stu-id="460e9-256">Example</span></span>
### <a name="request"></a><span data-ttu-id="460e9-257">请求</span><span class="sxs-lookup"><span data-stu-id="460e9-257">Request</span></span>
<span data-ttu-id="460e9-258">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="460e9-258">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
Content-type: application/json
Content-length: 1666

{
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
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

### <a name="response"></a><span data-ttu-id="460e9-259">响应</span><span class="sxs-lookup"><span data-stu-id="460e9-259">Response</span></span>
<span data-ttu-id="460e9-p113">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="460e9-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





