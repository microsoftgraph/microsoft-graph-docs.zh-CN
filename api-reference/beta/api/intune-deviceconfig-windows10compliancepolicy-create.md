---
title: 创建 windows10CompliancePolicy
description: 创建新的 windows10CompliancePolicy 对象。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 64649c1028a0ed7c4beca8ceb41eb683c25c8a27
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32517874"
---
# <a name="create-windows10compliancepolicy"></a><span data-ttu-id="2ad5d-103">创建 windows10CompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="2ad5d-103">Create windows10CompliancePolicy</span></span>

> <span data-ttu-id="2ad5d-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="2ad5d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2ad5d-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="2ad5d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2ad5d-106">创建新的 [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="2ad5d-106">Create a new [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2ad5d-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="2ad5d-107">Prerequisites</span></span>
<span data-ttu-id="2ad5d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2ad5d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2ad5d-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="2ad5d-110">Permission type</span></span>|<span data-ttu-id="2ad5d-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="2ad5d-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2ad5d-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2ad5d-112">Delegated (work or school account)</span></span>|<span data-ttu-id="2ad5d-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2ad5d-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="2ad5d-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2ad5d-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2ad5d-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="2ad5d-115">Not supported.</span></span>|
|<span data-ttu-id="2ad5d-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="2ad5d-116">Application</span></span>|<span data-ttu-id="2ad5d-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="2ad5d-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2ad5d-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2ad5d-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="2ad5d-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="2ad5d-119">Request headers</span></span>
|<span data-ttu-id="2ad5d-120">标头</span><span class="sxs-lookup"><span data-stu-id="2ad5d-120">Header</span></span>|<span data-ttu-id="2ad5d-121">值</span><span class="sxs-lookup"><span data-stu-id="2ad5d-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2ad5d-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="2ad5d-122">Authorization</span></span>|<span data-ttu-id="2ad5d-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="2ad5d-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2ad5d-124">接受</span><span class="sxs-lookup"><span data-stu-id="2ad5d-124">Accept</span></span>|<span data-ttu-id="2ad5d-125">application/json</span><span class="sxs-lookup"><span data-stu-id="2ad5d-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2ad5d-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="2ad5d-126">Request body</span></span>
<span data-ttu-id="2ad5d-127">在请求正文中，提供 windows10CompliancePolicy 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2ad5d-127">In the request body, supply a JSON representation for the windows10CompliancePolicy object.</span></span>

<span data-ttu-id="2ad5d-128">下表显示创建 windows10CompliancePolicy 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="2ad5d-128">The following table shows the properties that are required when you create the windows10CompliancePolicy.</span></span>

|<span data-ttu-id="2ad5d-129">属性</span><span class="sxs-lookup"><span data-stu-id="2ad5d-129">Property</span></span>|<span data-ttu-id="2ad5d-130">类型</span><span class="sxs-lookup"><span data-stu-id="2ad5d-130">Type</span></span>|<span data-ttu-id="2ad5d-131">说明</span><span class="sxs-lookup"><span data-stu-id="2ad5d-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2ad5d-132">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="2ad5d-132">roleScopeTagIds</span></span>|<span data-ttu-id="2ad5d-133">String collection</span><span class="sxs-lookup"><span data-stu-id="2ad5d-133">String collection</span></span>|<span data-ttu-id="2ad5d-134">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="2ad5d-134">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="2ad5d-135">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="2ad5d-135">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="2ad5d-136">id</span><span class="sxs-lookup"><span data-stu-id="2ad5d-136">id</span></span>|<span data-ttu-id="2ad5d-137">String</span><span class="sxs-lookup"><span data-stu-id="2ad5d-137">String</span></span>|<span data-ttu-id="2ad5d-138">实体的键。</span><span class="sxs-lookup"><span data-stu-id="2ad5d-138">Key of the entity.</span></span> <span data-ttu-id="2ad5d-139">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="2ad5d-139">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="2ad5d-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="2ad5d-140">createdDateTime</span></span>|<span data-ttu-id="2ad5d-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2ad5d-141">DateTimeOffset</span></span>|<span data-ttu-id="2ad5d-142">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="2ad5d-142">DateTime the object was created.</span></span> <span data-ttu-id="2ad5d-143">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="2ad5d-143">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="2ad5d-144">description</span><span class="sxs-lookup"><span data-stu-id="2ad5d-144">description</span></span>|<span data-ttu-id="2ad5d-145">字符串</span><span class="sxs-lookup"><span data-stu-id="2ad5d-145">String</span></span>|<span data-ttu-id="2ad5d-146">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="2ad5d-146">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="2ad5d-147">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="2ad5d-147">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="2ad5d-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2ad5d-148">lastModifiedDateTime</span></span>|<span data-ttu-id="2ad5d-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2ad5d-149">DateTimeOffset</span></span>|<span data-ttu-id="2ad5d-150">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="2ad5d-150">DateTime the object was last modified.</span></span> <span data-ttu-id="2ad5d-151">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="2ad5d-151">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="2ad5d-152">displayName</span><span class="sxs-lookup"><span data-stu-id="2ad5d-152">displayName</span></span>|<span data-ttu-id="2ad5d-153">字符串</span><span class="sxs-lookup"><span data-stu-id="2ad5d-153">String</span></span>|<span data-ttu-id="2ad5d-154">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="2ad5d-154">Admin provided name of the device configuration.</span></span> <span data-ttu-id="2ad5d-155">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="2ad5d-155">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="2ad5d-156">version</span><span class="sxs-lookup"><span data-stu-id="2ad5d-156">version</span></span>|<span data-ttu-id="2ad5d-157">Int32</span><span class="sxs-lookup"><span data-stu-id="2ad5d-157">Int32</span></span>|<span data-ttu-id="2ad5d-158">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="2ad5d-158">Version of the device configuration.</span></span> <span data-ttu-id="2ad5d-159">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="2ad5d-159">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="2ad5d-160">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="2ad5d-160">passwordRequired</span></span>|<span data-ttu-id="2ad5d-161">布尔</span><span class="sxs-lookup"><span data-stu-id="2ad5d-161">Boolean</span></span>|<span data-ttu-id="2ad5d-162">需要密码才可解锁 Windows 设备。</span><span class="sxs-lookup"><span data-stu-id="2ad5d-162">Require a password to unlock Windows device.</span></span>|
|<span data-ttu-id="2ad5d-163">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="2ad5d-163">passwordBlockSimple</span></span>|<span data-ttu-id="2ad5d-164">布尔</span><span class="sxs-lookup"><span data-stu-id="2ad5d-164">Boolean</span></span>|<span data-ttu-id="2ad5d-165">指示是否阻止简单密码。</span><span class="sxs-lookup"><span data-stu-id="2ad5d-165">Indicates whether or not to block simple password.</span></span>|
|<span data-ttu-id="2ad5d-166">passwordRequiredToUnlockFromIdle</span><span class="sxs-lookup"><span data-stu-id="2ad5d-166">passwordRequiredToUnlockFromIdle</span></span>|<span data-ttu-id="2ad5d-167">布尔</span><span class="sxs-lookup"><span data-stu-id="2ad5d-167">Boolean</span></span>|<span data-ttu-id="2ad5d-168">需要密码才可解锁空闲设备。</span><span class="sxs-lookup"><span data-stu-id="2ad5d-168">Require a password to unlock an idle device.</span></span>|
|<span data-ttu-id="2ad5d-169">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="2ad5d-169">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="2ad5d-170">Int32</span><span class="sxs-lookup"><span data-stu-id="2ad5d-170">Int32</span></span>|<span data-ttu-id="2ad5d-171">在需要密码之前不活动的分钟数。</span><span class="sxs-lookup"><span data-stu-id="2ad5d-171">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="2ad5d-172">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="2ad5d-172">passwordExpirationDays</span></span>|<span data-ttu-id="2ad5d-173">Int32</span><span class="sxs-lookup"><span data-stu-id="2ad5d-173">Int32</span></span>|<span data-ttu-id="2ad5d-174">密码过期天数。</span><span class="sxs-lookup"><span data-stu-id="2ad5d-174">The password expiration in days.</span></span>|
|<span data-ttu-id="2ad5d-175">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="2ad5d-175">passwordMinimumLength</span></span>|<span data-ttu-id="2ad5d-176">Int32</span><span class="sxs-lookup"><span data-stu-id="2ad5d-176">Int32</span></span>|<span data-ttu-id="2ad5d-177">密码最短长度。</span><span class="sxs-lookup"><span data-stu-id="2ad5d-177">The minimum password length.</span></span>|
|<span data-ttu-id="2ad5d-178">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="2ad5d-178">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="2ad5d-179">Int32</span><span class="sxs-lookup"><span data-stu-id="2ad5d-179">Int32</span></span>|<span data-ttu-id="2ad5d-180">密码中必需的字符集数。</span><span class="sxs-lookup"><span data-stu-id="2ad5d-180">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="2ad5d-181">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="2ad5d-181">passwordRequiredType</span></span>|[<span data-ttu-id="2ad5d-182">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="2ad5d-182">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="2ad5d-183">必需的密码类型。</span><span class="sxs-lookup"><span data-stu-id="2ad5d-183">The required password type.</span></span> <span data-ttu-id="2ad5d-184">可取值为：`deviceDefault`、`alphanumeric`、`numeric`。</span><span class="sxs-lookup"><span data-stu-id="2ad5d-184">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="2ad5d-185">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="2ad5d-185">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="2ad5d-186">Int32</span><span class="sxs-lookup"><span data-stu-id="2ad5d-186">Int32</span></span>|<span data-ttu-id="2ad5d-187">防止重复使用的先前密码的数量。</span><span class="sxs-lookup"><span data-stu-id="2ad5d-187">The number of previous passwords to prevent re-use of.</span></span>|
|<span data-ttu-id="2ad5d-188">requireHealthyDeviceReport</span><span class="sxs-lookup"><span data-stu-id="2ad5d-188">requireHealthyDeviceReport</span></span>|<span data-ttu-id="2ad5d-189">布尔</span><span class="sxs-lookup"><span data-stu-id="2ad5d-189">Boolean</span></span>|<span data-ttu-id="2ad5d-190">要求设备由 Windows 设备运行状况证明报告为正常。</span><span class="sxs-lookup"><span data-stu-id="2ad5d-190">Require devices to be reported as healthy by Windows Device Health Attestation.</span></span>|
|<span data-ttu-id="2ad5d-191">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="2ad5d-191">osMinimumVersion</span></span>|<span data-ttu-id="2ad5d-192">字符串</span><span class="sxs-lookup"><span data-stu-id="2ad5d-192">String</span></span>|<span data-ttu-id="2ad5d-193">最低 Windows 10 版本。</span><span class="sxs-lookup"><span data-stu-id="2ad5d-193">Minimum Windows 10 version.</span></span>|
|<span data-ttu-id="2ad5d-194">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="2ad5d-194">osMaximumVersion</span></span>|<span data-ttu-id="2ad5d-195">字符串</span><span class="sxs-lookup"><span data-stu-id="2ad5d-195">String</span></span>|<span data-ttu-id="2ad5d-196">最高 Windows 10 版本。</span><span class="sxs-lookup"><span data-stu-id="2ad5d-196">Maximum Windows 10 version.</span></span>|
|<span data-ttu-id="2ad5d-197">mobileOsMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="2ad5d-197">mobileOsMinimumVersion</span></span>|<span data-ttu-id="2ad5d-198">字符串</span><span class="sxs-lookup"><span data-stu-id="2ad5d-198">String</span></span>|<span data-ttu-id="2ad5d-199">最低 Windows Phone 版本。</span><span class="sxs-lookup"><span data-stu-id="2ad5d-199">Minimum Windows Phone version.</span></span>|
|<span data-ttu-id="2ad5d-200">mobileOsMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="2ad5d-200">mobileOsMaximumVersion</span></span>|<span data-ttu-id="2ad5d-201">String</span><span class="sxs-lookup"><span data-stu-id="2ad5d-201">String</span></span>|<span data-ttu-id="2ad5d-202">最高 Windows Phone 版本。</span><span class="sxs-lookup"><span data-stu-id="2ad5d-202">Maximum Windows Phone version.</span></span>|
|<span data-ttu-id="2ad5d-203">earlyLaunchAntiMalwareDriverEnabled</span><span class="sxs-lookup"><span data-stu-id="2ad5d-203">earlyLaunchAntiMalwareDriverEnabled</span></span>|<span data-ttu-id="2ad5d-204">布尔</span><span class="sxs-lookup"><span data-stu-id="2ad5d-204">Boolean</span></span>|<span data-ttu-id="2ad5d-205">要求设备由 Windows 设备运行状况证明报告为正常 - 提前启动反恶意驱动程序已启用。</span><span class="sxs-lookup"><span data-stu-id="2ad5d-205">Require devices to be reported as healthy by Windows Device Health Attestation - early launch antimalware driver is enabled.</span></span>|
|<span data-ttu-id="2ad5d-206">bitLockerEnabled</span><span class="sxs-lookup"><span data-stu-id="2ad5d-206">bitLockerEnabled</span></span>|<span data-ttu-id="2ad5d-207">布尔</span><span class="sxs-lookup"><span data-stu-id="2ad5d-207">Boolean</span></span>|<span data-ttu-id="2ad5d-208">要求设备由 Windows 设备运行状况证明报告为正常 - bit locker 已启用。</span><span class="sxs-lookup"><span data-stu-id="2ad5d-208">Require devices to be reported healthy by Windows Device Health Attestation - bit locker is enabled</span></span>|
|<span data-ttu-id="2ad5d-209">secureBootEnabled</span><span class="sxs-lookup"><span data-stu-id="2ad5d-209">secureBootEnabled</span></span>|<span data-ttu-id="2ad5d-210">布尔</span><span class="sxs-lookup"><span data-stu-id="2ad5d-210">Boolean</span></span>|<span data-ttu-id="2ad5d-211">要求设备由 Windows 设备运行状况证明报告为正常 - 安全启动已启用。</span><span class="sxs-lookup"><span data-stu-id="2ad5d-211">Require devices to be reported as healthy by Windows Device Health Attestation - secure boot is enabled.</span></span>|
|<span data-ttu-id="2ad5d-212">codeIntegrityEnabled</span><span class="sxs-lookup"><span data-stu-id="2ad5d-212">codeIntegrityEnabled</span></span>|<span data-ttu-id="2ad5d-213">Boolean</span><span class="sxs-lookup"><span data-stu-id="2ad5d-213">Boolean</span></span>|<span data-ttu-id="2ad5d-214">要求设备由 Windows 设备运行状况证明报告为正常。</span><span class="sxs-lookup"><span data-stu-id="2ad5d-214">Require devices to be reported as healthy by Windows Device Health Attestation.</span></span>|
|<span data-ttu-id="2ad5d-215">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="2ad5d-215">storageRequireEncryption</span></span>|<span data-ttu-id="2ad5d-216">Boolean</span><span class="sxs-lookup"><span data-stu-id="2ad5d-216">Boolean</span></span>|<span data-ttu-id="2ad5d-217">要求对 Windows 设备加密。</span><span class="sxs-lookup"><span data-stu-id="2ad5d-217">Require encryption on windows devices.</span></span>|
|<span data-ttu-id="2ad5d-218">activeFirewallRequired</span><span class="sxs-lookup"><span data-stu-id="2ad5d-218">activeFirewallRequired</span></span>|<span data-ttu-id="2ad5d-219">布尔</span><span class="sxs-lookup"><span data-stu-id="2ad5d-219">Boolean</span></span>|<span data-ttu-id="2ad5d-220">在 Windows 设备上需要活动防火墙。</span><span class="sxs-lookup"><span data-stu-id="2ad5d-220">Require active firewall on Windows devices.</span></span>|
|<span data-ttu-id="2ad5d-221">defenderEnabled</span><span class="sxs-lookup"><span data-stu-id="2ad5d-221">defenderEnabled</span></span>|<span data-ttu-id="2ad5d-222">布尔</span><span class="sxs-lookup"><span data-stu-id="2ad5d-222">Boolean</span></span>|<span data-ttu-id="2ad5d-223">在 windows 设备上需要 windows Defender 反恶意软件。</span><span class="sxs-lookup"><span data-stu-id="2ad5d-223">Require Windows Defender Antimalware on Windows devices.</span></span>|
|<span data-ttu-id="2ad5d-224">defenderVersion</span><span class="sxs-lookup"><span data-stu-id="2ad5d-224">defenderVersion</span></span>|<span data-ttu-id="2ad5d-225">字符串</span><span class="sxs-lookup"><span data-stu-id="2ad5d-225">String</span></span>|<span data-ttu-id="2ad5d-226">在 windows 设备上要求 windows Defender 反恶意软件的最低版本。</span><span class="sxs-lookup"><span data-stu-id="2ad5d-226">Require Windows Defender Antimalware minimum version on Windows devices.</span></span>|
|<span data-ttu-id="2ad5d-227">signatureOutOfDate</span><span class="sxs-lookup"><span data-stu-id="2ad5d-227">signatureOutOfDate</span></span>|<span data-ttu-id="2ad5d-228">布尔</span><span class="sxs-lookup"><span data-stu-id="2ad5d-228">Boolean</span></span>|<span data-ttu-id="2ad5d-229">windows 设备上要求 windows Defender 反恶意软件签名为最新。</span><span class="sxs-lookup"><span data-stu-id="2ad5d-229">Require Windows Defender Antimalware Signature to be up to date on Windows devices.</span></span>|
|<span data-ttu-id="2ad5d-230">rtpEnabled</span><span class="sxs-lookup"><span data-stu-id="2ad5d-230">rtpEnabled</span></span>|<span data-ttu-id="2ad5d-231">布尔</span><span class="sxs-lookup"><span data-stu-id="2ad5d-231">Boolean</span></span>|<span data-ttu-id="2ad5d-232">在 windows 设备上需要 windows Defender 反恶意软件实时保护。</span><span class="sxs-lookup"><span data-stu-id="2ad5d-232">Require Windows Defender Antimalware Real-Time Protection on Windows devices.</span></span>|
|<span data-ttu-id="2ad5d-233">antivirusRequired</span><span class="sxs-lookup"><span data-stu-id="2ad5d-233">antivirusRequired</span></span>|<span data-ttu-id="2ad5d-234">布尔</span><span class="sxs-lookup"><span data-stu-id="2ad5d-234">Boolean</span></span>|<span data-ttu-id="2ad5d-235">要求在 Windows Decurity Center 中注册的任何防病毒解决方案都处于启用和监控 (例如, Symantec、Windows Defender)。</span><span class="sxs-lookup"><span data-stu-id="2ad5d-235">Require any Antivirus solution registered with Windows Decurity Center to be on and monitoring (e.g. Symantec, Windows Defender).</span></span>|
|<span data-ttu-id="2ad5d-236">antiSpywareRequired</span><span class="sxs-lookup"><span data-stu-id="2ad5d-236">antiSpywareRequired</span></span>|<span data-ttu-id="2ad5d-237">布尔</span><span class="sxs-lookup"><span data-stu-id="2ad5d-237">Boolean</span></span>|<span data-ttu-id="2ad5d-238">要求在 Windows Decurity Center 中注册的任何反间谍软件解决方案都处于启用和监控 (例如, Symantec、Windows Defender)。</span><span class="sxs-lookup"><span data-stu-id="2ad5d-238">Require any AntiSpyware solution registered with Windows Decurity Center to be on and monitoring (e.g. Symantec, Windows Defender).</span></span>|
|<span data-ttu-id="2ad5d-239">validOperatingSystemBuildRanges</span><span class="sxs-lookup"><span data-stu-id="2ad5d-239">validOperatingSystemBuildRanges</span></span>|<span data-ttu-id="2ad5d-240">[operatingSystemVersionRange](../resources/intune-deviceconfig-operatingsystemversionrange.md)集合</span><span class="sxs-lookup"><span data-stu-id="2ad5d-240">[operatingSystemVersionRange](../resources/intune-deviceconfig-operatingsystemversionrange.md) collection</span></span>|<span data-ttu-id="2ad5d-241">Windows 设备上的有效操作系统内部版本范围。</span><span class="sxs-lookup"><span data-stu-id="2ad5d-241">The valid operating system build ranges on Windows devices.</span></span> <span data-ttu-id="2ad5d-242">该集合最多可包含 10000 个元素。</span><span class="sxs-lookup"><span data-stu-id="2ad5d-242">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="2ad5d-243">deviceThreatProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="2ad5d-243">deviceThreatProtectionEnabled</span></span>|<span data-ttu-id="2ad5d-244">Boolean</span><span class="sxs-lookup"><span data-stu-id="2ad5d-244">Boolean</span></span>|<span data-ttu-id="2ad5d-245">要求设备已启用设备威胁防护。</span><span class="sxs-lookup"><span data-stu-id="2ad5d-245">Require that devices have enabled device threat protection.</span></span>|
|<span data-ttu-id="2ad5d-246">deviceThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="2ad5d-246">deviceThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="2ad5d-247">deviceThreatProtectionLevel</span><span class="sxs-lookup"><span data-stu-id="2ad5d-247">deviceThreatProtectionLevel</span></span>](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|<span data-ttu-id="2ad5d-248">需要设备威胁防护最低风险级别来报告不合规。</span><span class="sxs-lookup"><span data-stu-id="2ad5d-248">Require Device Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="2ad5d-249">可取值为：`unavailable`、`secured`、`low`、`medium`、`high`、`notSet`。</span><span class="sxs-lookup"><span data-stu-id="2ad5d-249">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="2ad5d-250">configurationManagerComplianceRequired</span><span class="sxs-lookup"><span data-stu-id="2ad5d-250">configurationManagerComplianceRequired</span></span>|<span data-ttu-id="2ad5d-251">布尔</span><span class="sxs-lookup"><span data-stu-id="2ad5d-251">Boolean</span></span>|<span data-ttu-id="2ad5d-252">需要考虑将 SCCM 合规性状态考虑到 Intune 合规性状态。</span><span class="sxs-lookup"><span data-stu-id="2ad5d-252">Require to consider SCCM Compliance state into consideration for Intune Compliance State.</span></span>|



## <a name="response"></a><span data-ttu-id="2ad5d-253">响应</span><span class="sxs-lookup"><span data-stu-id="2ad5d-253">Response</span></span>
<span data-ttu-id="2ad5d-254">如果成功，此方法会在响应正文中返回 `201 Created` 响应代码和 [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="2ad5d-254">If successful, this method returns a `201 Created` response code and a [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2ad5d-255">示例</span><span class="sxs-lookup"><span data-stu-id="2ad5d-255">Example</span></span>

### <a name="request"></a><span data-ttu-id="2ad5d-256">请求</span><span class="sxs-lookup"><span data-stu-id="2ad5d-256">Request</span></span>
<span data-ttu-id="2ad5d-257">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="2ad5d-257">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies
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

### <a name="response"></a><span data-ttu-id="2ad5d-258">响应</span><span class="sxs-lookup"><span data-stu-id="2ad5d-258">Response</span></span>
<span data-ttu-id="2ad5d-p112">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="2ad5d-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





