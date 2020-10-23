---
title: 创建 windows10CompliancePolicy
description: 创建新的 windows10CompliancePolicy 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: e6d479193fdb9e54e11dc26950aa17bcb30973b0
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48736581"
---
# <a name="create-windows10compliancepolicy"></a><span data-ttu-id="59d57-103">创建 windows10CompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="59d57-103">Create windows10CompliancePolicy</span></span>

<span data-ttu-id="59d57-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="59d57-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="59d57-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="59d57-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="59d57-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="59d57-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="59d57-107">创建新的 [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="59d57-107">Create a new [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="59d57-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="59d57-108">Prerequisites</span></span>
<span data-ttu-id="59d57-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="59d57-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="59d57-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="59d57-111">Permission type</span></span>|<span data-ttu-id="59d57-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="59d57-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="59d57-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="59d57-113">Delegated (work or school account)</span></span>|<span data-ttu-id="59d57-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="59d57-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="59d57-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="59d57-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="59d57-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="59d57-116">Not supported.</span></span>|
|<span data-ttu-id="59d57-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="59d57-117">Application</span></span>|<span data-ttu-id="59d57-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="59d57-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="59d57-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="59d57-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="59d57-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="59d57-120">Request headers</span></span>
|<span data-ttu-id="59d57-121">标头</span><span class="sxs-lookup"><span data-stu-id="59d57-121">Header</span></span>|<span data-ttu-id="59d57-122">值</span><span class="sxs-lookup"><span data-stu-id="59d57-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="59d57-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="59d57-123">Authorization</span></span>|<span data-ttu-id="59d57-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="59d57-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="59d57-125">接受</span><span class="sxs-lookup"><span data-stu-id="59d57-125">Accept</span></span>|<span data-ttu-id="59d57-126">application/json</span><span class="sxs-lookup"><span data-stu-id="59d57-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="59d57-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="59d57-127">Request body</span></span>
<span data-ttu-id="59d57-128">在请求正文中，提供 windows10CompliancePolicy 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="59d57-128">In the request body, supply a JSON representation for the windows10CompliancePolicy object.</span></span>

<span data-ttu-id="59d57-129">下表显示创建 windows10CompliancePolicy 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="59d57-129">The following table shows the properties that are required when you create the windows10CompliancePolicy.</span></span>

|<span data-ttu-id="59d57-130">属性</span><span class="sxs-lookup"><span data-stu-id="59d57-130">Property</span></span>|<span data-ttu-id="59d57-131">类型</span><span class="sxs-lookup"><span data-stu-id="59d57-131">Type</span></span>|<span data-ttu-id="59d57-132">说明</span><span class="sxs-lookup"><span data-stu-id="59d57-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="59d57-133">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="59d57-133">roleScopeTagIds</span></span>|<span data-ttu-id="59d57-134">String collection</span><span class="sxs-lookup"><span data-stu-id="59d57-134">String collection</span></span>|<span data-ttu-id="59d57-135">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="59d57-135">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="59d57-136">继承自 [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="59d57-136">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="59d57-137">id</span><span class="sxs-lookup"><span data-stu-id="59d57-137">id</span></span>|<span data-ttu-id="59d57-138">String</span><span class="sxs-lookup"><span data-stu-id="59d57-138">String</span></span>|<span data-ttu-id="59d57-139">实体的键。</span><span class="sxs-lookup"><span data-stu-id="59d57-139">Key of the entity.</span></span> <span data-ttu-id="59d57-140">继承自 [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="59d57-140">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="59d57-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="59d57-141">createdDateTime</span></span>|<span data-ttu-id="59d57-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="59d57-142">DateTimeOffset</span></span>|<span data-ttu-id="59d57-143">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="59d57-143">DateTime the object was created.</span></span> <span data-ttu-id="59d57-144">继承自 [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="59d57-144">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="59d57-145">说明</span><span class="sxs-lookup"><span data-stu-id="59d57-145">description</span></span>|<span data-ttu-id="59d57-146">String</span><span class="sxs-lookup"><span data-stu-id="59d57-146">String</span></span>|<span data-ttu-id="59d57-147">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="59d57-147">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="59d57-148">继承自 [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="59d57-148">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="59d57-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="59d57-149">lastModifiedDateTime</span></span>|<span data-ttu-id="59d57-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="59d57-150">DateTimeOffset</span></span>|<span data-ttu-id="59d57-151">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="59d57-151">DateTime the object was last modified.</span></span> <span data-ttu-id="59d57-152">继承自 [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="59d57-152">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="59d57-153">displayName</span><span class="sxs-lookup"><span data-stu-id="59d57-153">displayName</span></span>|<span data-ttu-id="59d57-154">String</span><span class="sxs-lookup"><span data-stu-id="59d57-154">String</span></span>|<span data-ttu-id="59d57-155">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="59d57-155">Admin provided name of the device configuration.</span></span> <span data-ttu-id="59d57-156">继承自 [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="59d57-156">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="59d57-157">version</span><span class="sxs-lookup"><span data-stu-id="59d57-157">version</span></span>|<span data-ttu-id="59d57-158">Int32</span><span class="sxs-lookup"><span data-stu-id="59d57-158">Int32</span></span>|<span data-ttu-id="59d57-159">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="59d57-159">Version of the device configuration.</span></span> <span data-ttu-id="59d57-160">继承自 [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="59d57-160">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="59d57-161">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="59d57-161">passwordRequired</span></span>|<span data-ttu-id="59d57-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="59d57-162">Boolean</span></span>|<span data-ttu-id="59d57-163">需要密码才可解锁 Windows 设备。</span><span class="sxs-lookup"><span data-stu-id="59d57-163">Require a password to unlock Windows device.</span></span>|
|<span data-ttu-id="59d57-164">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="59d57-164">passwordBlockSimple</span></span>|<span data-ttu-id="59d57-165">Boolean</span><span class="sxs-lookup"><span data-stu-id="59d57-165">Boolean</span></span>|<span data-ttu-id="59d57-166">指示是否阻止简单密码。</span><span class="sxs-lookup"><span data-stu-id="59d57-166">Indicates whether or not to block simple password.</span></span>|
|<span data-ttu-id="59d57-167">passwordRequiredToUnlockFromIdle</span><span class="sxs-lookup"><span data-stu-id="59d57-167">passwordRequiredToUnlockFromIdle</span></span>|<span data-ttu-id="59d57-168">Boolean</span><span class="sxs-lookup"><span data-stu-id="59d57-168">Boolean</span></span>|<span data-ttu-id="59d57-169">需要密码才可解锁空闲设备。</span><span class="sxs-lookup"><span data-stu-id="59d57-169">Require a password to unlock an idle device.</span></span>|
|<span data-ttu-id="59d57-170">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="59d57-170">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="59d57-171">Int32</span><span class="sxs-lookup"><span data-stu-id="59d57-171">Int32</span></span>|<span data-ttu-id="59d57-172">在需要密码之前不活动的分钟数。</span><span class="sxs-lookup"><span data-stu-id="59d57-172">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="59d57-173">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="59d57-173">passwordExpirationDays</span></span>|<span data-ttu-id="59d57-174">Int32</span><span class="sxs-lookup"><span data-stu-id="59d57-174">Int32</span></span>|<span data-ttu-id="59d57-175">密码过期天数。</span><span class="sxs-lookup"><span data-stu-id="59d57-175">The password expiration in days.</span></span>|
|<span data-ttu-id="59d57-176">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="59d57-176">passwordMinimumLength</span></span>|<span data-ttu-id="59d57-177">Int32</span><span class="sxs-lookup"><span data-stu-id="59d57-177">Int32</span></span>|<span data-ttu-id="59d57-178">密码最短长度。</span><span class="sxs-lookup"><span data-stu-id="59d57-178">The minimum password length.</span></span>|
|<span data-ttu-id="59d57-179">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="59d57-179">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="59d57-180">Int32</span><span class="sxs-lookup"><span data-stu-id="59d57-180">Int32</span></span>|<span data-ttu-id="59d57-181">密码中必需的字符集数。</span><span class="sxs-lookup"><span data-stu-id="59d57-181">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="59d57-182">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="59d57-182">passwordRequiredType</span></span>|[<span data-ttu-id="59d57-183">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="59d57-183">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="59d57-184">必需的密码类型。</span><span class="sxs-lookup"><span data-stu-id="59d57-184">The required password type.</span></span> <span data-ttu-id="59d57-185">可取值为：`deviceDefault`、`alphanumeric`、`numeric`。</span><span class="sxs-lookup"><span data-stu-id="59d57-185">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="59d57-186">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="59d57-186">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="59d57-187">Int32</span><span class="sxs-lookup"><span data-stu-id="59d57-187">Int32</span></span>|<span data-ttu-id="59d57-188">防止重复使用的先前密码的数量。</span><span class="sxs-lookup"><span data-stu-id="59d57-188">The number of previous passwords to prevent re-use of.</span></span>|
|<span data-ttu-id="59d57-189">requireHealthyDeviceReport</span><span class="sxs-lookup"><span data-stu-id="59d57-189">requireHealthyDeviceReport</span></span>|<span data-ttu-id="59d57-190">Boolean</span><span class="sxs-lookup"><span data-stu-id="59d57-190">Boolean</span></span>|<span data-ttu-id="59d57-191">要求设备由 Windows 设备运行状况证明报告为正常。</span><span class="sxs-lookup"><span data-stu-id="59d57-191">Require devices to be reported as healthy by Windows Device Health Attestation.</span></span>|
|<span data-ttu-id="59d57-192">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="59d57-192">osMinimumVersion</span></span>|<span data-ttu-id="59d57-193">String</span><span class="sxs-lookup"><span data-stu-id="59d57-193">String</span></span>|<span data-ttu-id="59d57-194">最低 Windows 10 版本。</span><span class="sxs-lookup"><span data-stu-id="59d57-194">Minimum Windows 10 version.</span></span>|
|<span data-ttu-id="59d57-195">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="59d57-195">osMaximumVersion</span></span>|<span data-ttu-id="59d57-196">String</span><span class="sxs-lookup"><span data-stu-id="59d57-196">String</span></span>|<span data-ttu-id="59d57-197">最高 Windows 10 版本。</span><span class="sxs-lookup"><span data-stu-id="59d57-197">Maximum Windows 10 version.</span></span>|
|<span data-ttu-id="59d57-198">mobileOsMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="59d57-198">mobileOsMinimumVersion</span></span>|<span data-ttu-id="59d57-199">String</span><span class="sxs-lookup"><span data-stu-id="59d57-199">String</span></span>|<span data-ttu-id="59d57-200">最低 Windows Phone 版本。</span><span class="sxs-lookup"><span data-stu-id="59d57-200">Minimum Windows Phone version.</span></span>|
|<span data-ttu-id="59d57-201">mobileOsMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="59d57-201">mobileOsMaximumVersion</span></span>|<span data-ttu-id="59d57-202">String</span><span class="sxs-lookup"><span data-stu-id="59d57-202">String</span></span>|<span data-ttu-id="59d57-203">最高 Windows Phone 版本。</span><span class="sxs-lookup"><span data-stu-id="59d57-203">Maximum Windows Phone version.</span></span>|
|<span data-ttu-id="59d57-204">earlyLaunchAntiMalwareDriverEnabled</span><span class="sxs-lookup"><span data-stu-id="59d57-204">earlyLaunchAntiMalwareDriverEnabled</span></span>|<span data-ttu-id="59d57-205">Boolean</span><span class="sxs-lookup"><span data-stu-id="59d57-205">Boolean</span></span>|<span data-ttu-id="59d57-206">要求设备由 Windows 设备运行状况证明报告为正常 - 提前启动反恶意驱动程序已启用。</span><span class="sxs-lookup"><span data-stu-id="59d57-206">Require devices to be reported as healthy by Windows Device Health Attestation - early launch antimalware driver is enabled.</span></span>|
|<span data-ttu-id="59d57-207">bitLockerEnabled</span><span class="sxs-lookup"><span data-stu-id="59d57-207">bitLockerEnabled</span></span>|<span data-ttu-id="59d57-208">Boolean</span><span class="sxs-lookup"><span data-stu-id="59d57-208">Boolean</span></span>|<span data-ttu-id="59d57-209">要求设备由 Windows 设备运行状况证明报告为正常 - bit locker 已启用。</span><span class="sxs-lookup"><span data-stu-id="59d57-209">Require devices to be reported healthy by Windows Device Health Attestation - bit locker is enabled</span></span>|
|<span data-ttu-id="59d57-210">secureBootEnabled</span><span class="sxs-lookup"><span data-stu-id="59d57-210">secureBootEnabled</span></span>|<span data-ttu-id="59d57-211">Boolean</span><span class="sxs-lookup"><span data-stu-id="59d57-211">Boolean</span></span>|<span data-ttu-id="59d57-212">要求设备由 Windows 设备运行状况证明报告为正常 - 安全启动已启用。</span><span class="sxs-lookup"><span data-stu-id="59d57-212">Require devices to be reported as healthy by Windows Device Health Attestation - secure boot is enabled.</span></span>|
|<span data-ttu-id="59d57-213">codeIntegrityEnabled</span><span class="sxs-lookup"><span data-stu-id="59d57-213">codeIntegrityEnabled</span></span>|<span data-ttu-id="59d57-214">Boolean</span><span class="sxs-lookup"><span data-stu-id="59d57-214">Boolean</span></span>|<span data-ttu-id="59d57-215">要求设备由 Windows 设备运行状况证明报告为正常。</span><span class="sxs-lookup"><span data-stu-id="59d57-215">Require devices to be reported as healthy by Windows Device Health Attestation.</span></span>|
|<span data-ttu-id="59d57-216">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="59d57-216">storageRequireEncryption</span></span>|<span data-ttu-id="59d57-217">Boolean</span><span class="sxs-lookup"><span data-stu-id="59d57-217">Boolean</span></span>|<span data-ttu-id="59d57-218">要求对 Windows 设备加密。</span><span class="sxs-lookup"><span data-stu-id="59d57-218">Require encryption on windows devices.</span></span>|
|<span data-ttu-id="59d57-219">activeFirewallRequired</span><span class="sxs-lookup"><span data-stu-id="59d57-219">activeFirewallRequired</span></span>|<span data-ttu-id="59d57-220">布尔</span><span class="sxs-lookup"><span data-stu-id="59d57-220">Boolean</span></span>|<span data-ttu-id="59d57-221">在 Windows 设备上需要活动防火墙。</span><span class="sxs-lookup"><span data-stu-id="59d57-221">Require active firewall on Windows devices.</span></span>|
|<span data-ttu-id="59d57-222">defenderEnabled</span><span class="sxs-lookup"><span data-stu-id="59d57-222">defenderEnabled</span></span>|<span data-ttu-id="59d57-223">布尔</span><span class="sxs-lookup"><span data-stu-id="59d57-223">Boolean</span></span>|<span data-ttu-id="59d57-224">在 Windows 设备上需要 Windows Defender 反恶意软件。</span><span class="sxs-lookup"><span data-stu-id="59d57-224">Require Windows Defender Antimalware on Windows devices.</span></span>|
|<span data-ttu-id="59d57-225">defenderVersion</span><span class="sxs-lookup"><span data-stu-id="59d57-225">defenderVersion</span></span>|<span data-ttu-id="59d57-226">String</span><span class="sxs-lookup"><span data-stu-id="59d57-226">String</span></span>|<span data-ttu-id="59d57-227">在 Windows 设备上要求 Windows Defender 反恶意软件的最低版本。</span><span class="sxs-lookup"><span data-stu-id="59d57-227">Require Windows Defender Antimalware minimum version on Windows devices.</span></span>|
|<span data-ttu-id="59d57-228">signatureOutOfDate</span><span class="sxs-lookup"><span data-stu-id="59d57-228">signatureOutOfDate</span></span>|<span data-ttu-id="59d57-229">布尔</span><span class="sxs-lookup"><span data-stu-id="59d57-229">Boolean</span></span>|<span data-ttu-id="59d57-230">Windows 设备上要求 Windows Defender 反恶意软件签名为最新。</span><span class="sxs-lookup"><span data-stu-id="59d57-230">Require Windows Defender Antimalware Signature to be up to date on Windows devices.</span></span>|
|<span data-ttu-id="59d57-231">rtpEnabled</span><span class="sxs-lookup"><span data-stu-id="59d57-231">rtpEnabled</span></span>|<span data-ttu-id="59d57-232">布尔</span><span class="sxs-lookup"><span data-stu-id="59d57-232">Boolean</span></span>|<span data-ttu-id="59d57-233">在 Windows 设备上需要 Windows Defender 反恶意软件 Real-Time 保护。</span><span class="sxs-lookup"><span data-stu-id="59d57-233">Require Windows Defender Antimalware Real-Time Protection on Windows devices.</span></span>|
|<span data-ttu-id="59d57-234">antivirusRequired</span><span class="sxs-lookup"><span data-stu-id="59d57-234">antivirusRequired</span></span>|<span data-ttu-id="59d57-235">布尔</span><span class="sxs-lookup"><span data-stu-id="59d57-235">Boolean</span></span>|<span data-ttu-id="59d57-236">要求在 Windows Decurity 中心注册的任何防病毒解决方案都处于启用和监控 (例如，Symantec、Windows Defender) 。</span><span class="sxs-lookup"><span data-stu-id="59d57-236">Require any Antivirus solution registered with Windows Decurity Center to be on and monitoring (e.g. Symantec, Windows Defender).</span></span>|
|<span data-ttu-id="59d57-237">antiSpywareRequired</span><span class="sxs-lookup"><span data-stu-id="59d57-237">antiSpywareRequired</span></span>|<span data-ttu-id="59d57-238">布尔</span><span class="sxs-lookup"><span data-stu-id="59d57-238">Boolean</span></span>|<span data-ttu-id="59d57-239">需要在 Windows Decurity Center 中注册的任何反间谍软件解决方案在 (（例如 Symantec、Windows Defender) ）上进行监视。</span><span class="sxs-lookup"><span data-stu-id="59d57-239">Require any AntiSpyware solution registered with Windows Decurity Center to be on and monitoring (e.g. Symantec, Windows Defender).</span></span>|
|<span data-ttu-id="59d57-240">validOperatingSystemBuildRanges</span><span class="sxs-lookup"><span data-stu-id="59d57-240">validOperatingSystemBuildRanges</span></span>|<span data-ttu-id="59d57-241">[operatingSystemVersionRange](../resources/intune-deviceconfig-operatingsystemversionrange.md) 集合</span><span class="sxs-lookup"><span data-stu-id="59d57-241">[operatingSystemVersionRange](../resources/intune-deviceconfig-operatingsystemversionrange.md) collection</span></span>|<span data-ttu-id="59d57-242">Windows 设备上的有效操作系统内部版本范围。</span><span class="sxs-lookup"><span data-stu-id="59d57-242">The valid operating system build ranges on Windows devices.</span></span> <span data-ttu-id="59d57-243">该集合最多可包含 10000 个元素。</span><span class="sxs-lookup"><span data-stu-id="59d57-243">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="59d57-244">deviceThreatProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="59d57-244">deviceThreatProtectionEnabled</span></span>|<span data-ttu-id="59d57-245">Boolean</span><span class="sxs-lookup"><span data-stu-id="59d57-245">Boolean</span></span>|<span data-ttu-id="59d57-246">要求设备已启用设备威胁防护。</span><span class="sxs-lookup"><span data-stu-id="59d57-246">Require that devices have enabled device threat protection.</span></span>|
|<span data-ttu-id="59d57-247">deviceThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="59d57-247">deviceThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="59d57-248">deviceThreatProtectionLevel</span><span class="sxs-lookup"><span data-stu-id="59d57-248">deviceThreatProtectionLevel</span></span>](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|<span data-ttu-id="59d57-249">需要设备威胁防护最低风险级别来报告不合规。</span><span class="sxs-lookup"><span data-stu-id="59d57-249">Require Device Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="59d57-250">可取值为：`unavailable`、`secured`、`low`、`medium`、`high`、`notSet`。</span><span class="sxs-lookup"><span data-stu-id="59d57-250">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="59d57-251">configurationManagerComplianceRequired</span><span class="sxs-lookup"><span data-stu-id="59d57-251">configurationManagerComplianceRequired</span></span>|<span data-ttu-id="59d57-252">布尔</span><span class="sxs-lookup"><span data-stu-id="59d57-252">Boolean</span></span>|<span data-ttu-id="59d57-253">需要考虑将 SCCM 合规性状态考虑到 Intune 合规性状态。</span><span class="sxs-lookup"><span data-stu-id="59d57-253">Require to consider SCCM Compliance state into consideration for Intune Compliance State.</span></span>|
|<span data-ttu-id="59d57-254">tpmRequired</span><span class="sxs-lookup"><span data-stu-id="59d57-254">tpmRequired</span></span>|<span data-ttu-id="59d57-255">布尔</span><span class="sxs-lookup"><span data-stu-id="59d57-255">Boolean</span></span>|<span data-ttu-id="59d57-256">需要受信任的平台模块 (TPM) 存在。</span><span class="sxs-lookup"><span data-stu-id="59d57-256">Require Trusted Platform Module(TPM) to be present.</span></span>|
|<span data-ttu-id="59d57-257">deviceCompliancePolicyScript</span><span class="sxs-lookup"><span data-stu-id="59d57-257">deviceCompliancePolicyScript</span></span>|[<span data-ttu-id="59d57-258">deviceCompliancePolicyScript</span><span class="sxs-lookup"><span data-stu-id="59d57-258">deviceCompliancePolicyScript</span></span>](../resources/intune-deviceconfig-devicecompliancepolicyscript.md)|<span data-ttu-id="59d57-259">尚未记录</span><span class="sxs-lookup"><span data-stu-id="59d57-259">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="59d57-260">响应</span><span class="sxs-lookup"><span data-stu-id="59d57-260">Response</span></span>
<span data-ttu-id="59d57-261">如果成功，此方法会在响应正文中返回 `201 Created` 响应代码和 [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="59d57-261">If successful, this method returns a `201 Created` response code and a [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="59d57-262">示例</span><span class="sxs-lookup"><span data-stu-id="59d57-262">Example</span></span>

### <a name="request"></a><span data-ttu-id="59d57-263">请求</span><span class="sxs-lookup"><span data-stu-id="59d57-263">Request</span></span>
<span data-ttu-id="59d57-264">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="59d57-264">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies
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

### <a name="response"></a><span data-ttu-id="59d57-265">响应</span><span class="sxs-lookup"><span data-stu-id="59d57-265">Response</span></span>
<span data-ttu-id="59d57-p112">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="59d57-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





