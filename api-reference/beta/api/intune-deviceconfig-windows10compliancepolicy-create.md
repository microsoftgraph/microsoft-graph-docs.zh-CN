---
title: 创建 windows10CompliancePolicy
description: 创建新的 windows10CompliancePolicy 对象。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 2eba67635ea4e596dd9bf1881b5b5c0d7b9743df
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29422738"
---
# <a name="create-windows10compliancepolicy"></a><span data-ttu-id="c84b3-103">创建 windows10CompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="c84b3-103">Create windows10CompliancePolicy</span></span>

> <span data-ttu-id="c84b3-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="c84b3-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="c84b3-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="c84b3-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c84b3-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c84b3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c84b3-107">创建新的 [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="c84b3-107">Create a new [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c84b3-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="c84b3-108">Prerequisites</span></span>
<span data-ttu-id="c84b3-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="c84b3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="c84b3-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="c84b3-111">Permission type</span></span>|<span data-ttu-id="c84b3-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="c84b3-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c84b3-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c84b3-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c84b3-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c84b3-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c84b3-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c84b3-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c84b3-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="c84b3-116">Not supported.</span></span>|
|<span data-ttu-id="c84b3-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="c84b3-117">Application</span></span>|<span data-ttu-id="c84b3-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="c84b3-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c84b3-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c84b3-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="c84b3-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="c84b3-120">Request headers</span></span>
|<span data-ttu-id="c84b3-121">标头</span><span class="sxs-lookup"><span data-stu-id="c84b3-121">Header</span></span>|<span data-ttu-id="c84b3-122">值</span><span class="sxs-lookup"><span data-stu-id="c84b3-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c84b3-123">授权</span><span class="sxs-lookup"><span data-stu-id="c84b3-123">Authorization</span></span>|<span data-ttu-id="c84b3-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="c84b3-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c84b3-125">Accept</span><span class="sxs-lookup"><span data-stu-id="c84b3-125">Accept</span></span>|<span data-ttu-id="c84b3-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c84b3-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c84b3-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="c84b3-127">Request body</span></span>
<span data-ttu-id="c84b3-128">在请求正文中，提供 windows10CompliancePolicy 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c84b3-128">In the request body, supply a JSON representation for the windows10CompliancePolicy object.</span></span>

<span data-ttu-id="c84b3-129">下表显示创建 windows10CompliancePolicy 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="c84b3-129">The following table shows the properties that are required when you create the windows10CompliancePolicy.</span></span>

|<span data-ttu-id="c84b3-130">属性</span><span class="sxs-lookup"><span data-stu-id="c84b3-130">Property</span></span>|<span data-ttu-id="c84b3-131">类型</span><span class="sxs-lookup"><span data-stu-id="c84b3-131">Type</span></span>|<span data-ttu-id="c84b3-132">说明</span><span class="sxs-lookup"><span data-stu-id="c84b3-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c84b3-133">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="c84b3-133">roleScopeTagIds</span></span>|<span data-ttu-id="c84b3-134">String 集合</span><span class="sxs-lookup"><span data-stu-id="c84b3-134">String collection</span></span>|<span data-ttu-id="c84b3-135">此实体实例范围标记的列表。</span><span class="sxs-lookup"><span data-stu-id="c84b3-135">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="c84b3-136">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="c84b3-136">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="c84b3-137">id</span><span class="sxs-lookup"><span data-stu-id="c84b3-137">id</span></span>|<span data-ttu-id="c84b3-138">String</span><span class="sxs-lookup"><span data-stu-id="c84b3-138">String</span></span>|<span data-ttu-id="c84b3-139">实体的键。</span><span class="sxs-lookup"><span data-stu-id="c84b3-139">Key of the entity.</span></span> <span data-ttu-id="c84b3-140">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="c84b3-140">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="c84b3-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c84b3-141">createdDateTime</span></span>|<span data-ttu-id="c84b3-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c84b3-142">DateTimeOffset</span></span>|<span data-ttu-id="c84b3-143">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="c84b3-143">DateTime the object was created.</span></span> <span data-ttu-id="c84b3-144">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="c84b3-144">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="c84b3-145">description</span><span class="sxs-lookup"><span data-stu-id="c84b3-145">description</span></span>|<span data-ttu-id="c84b3-146">String</span><span class="sxs-lookup"><span data-stu-id="c84b3-146">String</span></span>|<span data-ttu-id="c84b3-147">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="c84b3-147">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="c84b3-148">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="c84b3-148">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="c84b3-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c84b3-149">lastModifiedDateTime</span></span>|<span data-ttu-id="c84b3-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c84b3-150">DateTimeOffset</span></span>|<span data-ttu-id="c84b3-151">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="c84b3-151">DateTime the object was last modified.</span></span> <span data-ttu-id="c84b3-152">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="c84b3-152">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="c84b3-153">displayName</span><span class="sxs-lookup"><span data-stu-id="c84b3-153">displayName</span></span>|<span data-ttu-id="c84b3-154">String</span><span class="sxs-lookup"><span data-stu-id="c84b3-154">String</span></span>|<span data-ttu-id="c84b3-155">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="c84b3-155">Admin provided name of the device configuration.</span></span> <span data-ttu-id="c84b3-156">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="c84b3-156">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="c84b3-157">version</span><span class="sxs-lookup"><span data-stu-id="c84b3-157">version</span></span>|<span data-ttu-id="c84b3-158">Int32</span><span class="sxs-lookup"><span data-stu-id="c84b3-158">Int32</span></span>|<span data-ttu-id="c84b3-159">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="c84b3-159">Version of the device configuration.</span></span> <span data-ttu-id="c84b3-160">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="c84b3-160">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="c84b3-161">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="c84b3-161">passwordRequired</span></span>|<span data-ttu-id="c84b3-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="c84b3-162">Boolean</span></span>|<span data-ttu-id="c84b3-163">需要密码才可解锁 Windows 设备。</span><span class="sxs-lookup"><span data-stu-id="c84b3-163">Require a password to unlock Windows device.</span></span>|
|<span data-ttu-id="c84b3-164">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="c84b3-164">passwordBlockSimple</span></span>|<span data-ttu-id="c84b3-165">Boolean</span><span class="sxs-lookup"><span data-stu-id="c84b3-165">Boolean</span></span>|<span data-ttu-id="c84b3-166">指示是否阻止简单密码。</span><span class="sxs-lookup"><span data-stu-id="c84b3-166">Indicates whether or not to block simple password.</span></span>|
|<span data-ttu-id="c84b3-167">passwordRequiredToUnlockFromIdle</span><span class="sxs-lookup"><span data-stu-id="c84b3-167">passwordRequiredToUnlockFromIdle</span></span>|<span data-ttu-id="c84b3-168">Boolean</span><span class="sxs-lookup"><span data-stu-id="c84b3-168">Boolean</span></span>|<span data-ttu-id="c84b3-169">需要密码才可解锁空闲设备。</span><span class="sxs-lookup"><span data-stu-id="c84b3-169">Require a password to unlock an idle device.</span></span>|
|<span data-ttu-id="c84b3-170">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="c84b3-170">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="c84b3-171">Int32</span><span class="sxs-lookup"><span data-stu-id="c84b3-171">Int32</span></span>|<span data-ttu-id="c84b3-172">在需要密码之前不活动的分钟数。</span><span class="sxs-lookup"><span data-stu-id="c84b3-172">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="c84b3-173">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="c84b3-173">passwordExpirationDays</span></span>|<span data-ttu-id="c84b3-174">Int32</span><span class="sxs-lookup"><span data-stu-id="c84b3-174">Int32</span></span>|<span data-ttu-id="c84b3-175">密码过期天数。</span><span class="sxs-lookup"><span data-stu-id="c84b3-175">The password expiration in days.</span></span>|
|<span data-ttu-id="c84b3-176">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="c84b3-176">passwordMinimumLength</span></span>|<span data-ttu-id="c84b3-177">Int32</span><span class="sxs-lookup"><span data-stu-id="c84b3-177">Int32</span></span>|<span data-ttu-id="c84b3-178">密码最短长度。</span><span class="sxs-lookup"><span data-stu-id="c84b3-178">The minimum password length.</span></span>|
|<span data-ttu-id="c84b3-179">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="c84b3-179">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="c84b3-180">Int32</span><span class="sxs-lookup"><span data-stu-id="c84b3-180">Int32</span></span>|<span data-ttu-id="c84b3-181">密码中必需的字符集数。</span><span class="sxs-lookup"><span data-stu-id="c84b3-181">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="c84b3-182">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="c84b3-182">passwordRequiredType</span></span>|[<span data-ttu-id="c84b3-183">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="c84b3-183">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="c84b3-184">必需的密码类型。</span><span class="sxs-lookup"><span data-stu-id="c84b3-184">The required password type.</span></span> <span data-ttu-id="c84b3-185">可取值为：`deviceDefault`、`alphanumeric`、`numeric`。</span><span class="sxs-lookup"><span data-stu-id="c84b3-185">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="c84b3-186">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="c84b3-186">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="c84b3-187">Int32</span><span class="sxs-lookup"><span data-stu-id="c84b3-187">Int32</span></span>|<span data-ttu-id="c84b3-188">防止重复使用的先前密码的数量。</span><span class="sxs-lookup"><span data-stu-id="c84b3-188">The number of previous passwords to prevent re-use of.</span></span>|
|<span data-ttu-id="c84b3-189">requireHealthyDeviceReport</span><span class="sxs-lookup"><span data-stu-id="c84b3-189">requireHealthyDeviceReport</span></span>|<span data-ttu-id="c84b3-190">Boolean</span><span class="sxs-lookup"><span data-stu-id="c84b3-190">Boolean</span></span>|<span data-ttu-id="c84b3-191">要求设备由 Windows 设备运行状况证明报告为正常。</span><span class="sxs-lookup"><span data-stu-id="c84b3-191">Require devices to be reported as healthy by Windows Device Health Attestation.</span></span>|
|<span data-ttu-id="c84b3-192">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="c84b3-192">osMinimumVersion</span></span>|<span data-ttu-id="c84b3-193">String</span><span class="sxs-lookup"><span data-stu-id="c84b3-193">String</span></span>|<span data-ttu-id="c84b3-194">最低 Windows 10 版本。</span><span class="sxs-lookup"><span data-stu-id="c84b3-194">Minimum Windows 10 version.</span></span>|
|<span data-ttu-id="c84b3-195">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="c84b3-195">osMaximumVersion</span></span>|<span data-ttu-id="c84b3-196">String</span><span class="sxs-lookup"><span data-stu-id="c84b3-196">String</span></span>|<span data-ttu-id="c84b3-197">最高 Windows 10 版本。</span><span class="sxs-lookup"><span data-stu-id="c84b3-197">Maximum Windows 10 version.</span></span>|
|<span data-ttu-id="c84b3-198">mobileOsMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="c84b3-198">mobileOsMinimumVersion</span></span>|<span data-ttu-id="c84b3-199">String</span><span class="sxs-lookup"><span data-stu-id="c84b3-199">String</span></span>|<span data-ttu-id="c84b3-200">最低 Windows Phone 版本。</span><span class="sxs-lookup"><span data-stu-id="c84b3-200">Minimum Windows Phone version.</span></span>|
|<span data-ttu-id="c84b3-201">mobileOsMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="c84b3-201">mobileOsMaximumVersion</span></span>|<span data-ttu-id="c84b3-202">String</span><span class="sxs-lookup"><span data-stu-id="c84b3-202">String</span></span>|<span data-ttu-id="c84b3-203">最高 Windows Phone 版本。</span><span class="sxs-lookup"><span data-stu-id="c84b3-203">Maximum Windows Phone version.</span></span>|
|<span data-ttu-id="c84b3-204">earlyLaunchAntiMalwareDriverEnabled</span><span class="sxs-lookup"><span data-stu-id="c84b3-204">earlyLaunchAntiMalwareDriverEnabled</span></span>|<span data-ttu-id="c84b3-205">Boolean</span><span class="sxs-lookup"><span data-stu-id="c84b3-205">Boolean</span></span>|<span data-ttu-id="c84b3-206">要求设备由 Windows 设备运行状况证明报告为正常 - 提前启动反恶意驱动程序已启用。</span><span class="sxs-lookup"><span data-stu-id="c84b3-206">Require devices to be reported as healthy by Windows Device Health Attestation - early launch antimalware driver is enabled.</span></span>|
|<span data-ttu-id="c84b3-207">bitLockerEnabled</span><span class="sxs-lookup"><span data-stu-id="c84b3-207">bitLockerEnabled</span></span>|<span data-ttu-id="c84b3-208">Boolean</span><span class="sxs-lookup"><span data-stu-id="c84b3-208">Boolean</span></span>|<span data-ttu-id="c84b3-209">要求设备由 Windows 设备运行状况证明报告为正常 - bit locker 已启用。</span><span class="sxs-lookup"><span data-stu-id="c84b3-209">Require devices to be reported healthy by Windows Device Health Attestation - bit locker is enabled</span></span>|
|<span data-ttu-id="c84b3-210">secureBootEnabled</span><span class="sxs-lookup"><span data-stu-id="c84b3-210">secureBootEnabled</span></span>|<span data-ttu-id="c84b3-211">Boolean</span><span class="sxs-lookup"><span data-stu-id="c84b3-211">Boolean</span></span>|<span data-ttu-id="c84b3-212">要求设备由 Windows 设备运行状况证明报告为正常 - 安全启动已启用。</span><span class="sxs-lookup"><span data-stu-id="c84b3-212">Require devices to be reported as healthy by Windows Device Health Attestation - secure boot is enabled.</span></span>|
|<span data-ttu-id="c84b3-213">codeIntegrityEnabled</span><span class="sxs-lookup"><span data-stu-id="c84b3-213">codeIntegrityEnabled</span></span>|<span data-ttu-id="c84b3-214">Boolean</span><span class="sxs-lookup"><span data-stu-id="c84b3-214">Boolean</span></span>|<span data-ttu-id="c84b3-215">要求设备由 Windows 设备运行状况证明报告为正常。</span><span class="sxs-lookup"><span data-stu-id="c84b3-215">Require devices to be reported as healthy by Windows Device Health Attestation.</span></span>|
|<span data-ttu-id="c84b3-216">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="c84b3-216">storageRequireEncryption</span></span>|<span data-ttu-id="c84b3-217">Boolean</span><span class="sxs-lookup"><span data-stu-id="c84b3-217">Boolean</span></span>|<span data-ttu-id="c84b3-218">要求对 Windows 设备加密。</span><span class="sxs-lookup"><span data-stu-id="c84b3-218">Require encryption on windows devices.</span></span>|
|<span data-ttu-id="c84b3-219">activeFirewallRequired</span><span class="sxs-lookup"><span data-stu-id="c84b3-219">activeFirewallRequired</span></span>|<span data-ttu-id="c84b3-220">Boolean</span><span class="sxs-lookup"><span data-stu-id="c84b3-220">Boolean</span></span>|<span data-ttu-id="c84b3-221">要求在 Windows 设备上的活动防火墙。</span><span class="sxs-lookup"><span data-stu-id="c84b3-221">Require active firewall on Windows devices.</span></span>|
|<span data-ttu-id="c84b3-222">defenderEnabled</span><span class="sxs-lookup"><span data-stu-id="c84b3-222">defenderEnabled</span></span>|<span data-ttu-id="c84b3-223">Boolean</span><span class="sxs-lookup"><span data-stu-id="c84b3-223">Boolean</span></span>|<span data-ttu-id="c84b3-224">在 Windows 设备上需要 Windows Defender 反恶意软件。</span><span class="sxs-lookup"><span data-stu-id="c84b3-224">Require Windows Defender Antimalware on Windows devices.</span></span>|
|<span data-ttu-id="c84b3-225">defenderVersion</span><span class="sxs-lookup"><span data-stu-id="c84b3-225">defenderVersion</span></span>|<span data-ttu-id="c84b3-226">String</span><span class="sxs-lookup"><span data-stu-id="c84b3-226">String</span></span>|<span data-ttu-id="c84b3-227">需要 Windows Defender 反恶意软件在 Windows 设备上的最低版本。</span><span class="sxs-lookup"><span data-stu-id="c84b3-227">Require Windows Defender Antimalware minimum version on Windows devices.</span></span>|
|<span data-ttu-id="c84b3-228">signatureOutOfDate</span><span class="sxs-lookup"><span data-stu-id="c84b3-228">signatureOutOfDate</span></span>|<span data-ttu-id="c84b3-229">Boolean</span><span class="sxs-lookup"><span data-stu-id="c84b3-229">Boolean</span></span>|<span data-ttu-id="c84b3-230">需要 Windows Defender 反恶意软件签名是最新 Windows 设备上。</span><span class="sxs-lookup"><span data-stu-id="c84b3-230">Require Windows Defender Antimalware Signature to be up to date on Windows devices.</span></span>|
|<span data-ttu-id="c84b3-231">rtpEnabled</span><span class="sxs-lookup"><span data-stu-id="c84b3-231">rtpEnabled</span></span>|<span data-ttu-id="c84b3-232">Boolean</span><span class="sxs-lookup"><span data-stu-id="c84b3-232">Boolean</span></span>|<span data-ttu-id="c84b3-233">在 Windows 设备上需要 Windows Defender 反恶意软件实时保护。</span><span class="sxs-lookup"><span data-stu-id="c84b3-233">Require Windows Defender Antimalware Real-Time Protection on Windows devices.</span></span>|
|<span data-ttu-id="c84b3-234">antivirusRequired</span><span class="sxs-lookup"><span data-stu-id="c84b3-234">antivirusRequired</span></span>|<span data-ttu-id="c84b3-235">Boolean</span><span class="sxs-lookup"><span data-stu-id="c84b3-235">Boolean</span></span>|<span data-ttu-id="c84b3-236">需要与 Windows Decurity 中心上注册和监视 (例如 Symantec，Windows Defender) 的任何防病毒解决方案。</span><span class="sxs-lookup"><span data-stu-id="c84b3-236">Require any Antivirus solution registered with Windows Decurity Center to be on and monitoring (e.g. Symantec, Windows Defender).</span></span>|
|<span data-ttu-id="c84b3-237">antiSpywareRequired</span><span class="sxs-lookup"><span data-stu-id="c84b3-237">antiSpywareRequired</span></span>|<span data-ttu-id="c84b3-238">Boolean</span><span class="sxs-lookup"><span data-stu-id="c84b3-238">Boolean</span></span>|<span data-ttu-id="c84b3-239">需要的任何反间谍软件解决方案注册 Windows Decurity 中心上为和监视 （例如 Symantec、 Windows Defender）。</span><span class="sxs-lookup"><span data-stu-id="c84b3-239">Require any AntiSpyware solution registered with Windows Decurity Center to be on and monitoring (e.g. Symantec, Windows Defender).</span></span>|
|<span data-ttu-id="c84b3-240">validOperatingSystemBuildRanges</span><span class="sxs-lookup"><span data-stu-id="c84b3-240">validOperatingSystemBuildRanges</span></span>|<span data-ttu-id="c84b3-241">[operatingSystemVersionRange](../resources/intune-deviceconfig-operatingsystemversionrange.md)集合</span><span class="sxs-lookup"><span data-stu-id="c84b3-241">[operatingSystemVersionRange](../resources/intune-deviceconfig-operatingsystemversionrange.md) collection</span></span>|<span data-ttu-id="c84b3-242">有效的操作系统构建 Windows 设备上的区域。</span><span class="sxs-lookup"><span data-stu-id="c84b3-242">The valid operating system build ranges on Windows devices.</span></span> <span data-ttu-id="c84b3-243">该集合最多可包含 10000 个元素。</span><span class="sxs-lookup"><span data-stu-id="c84b3-243">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="c84b3-244">deviceThreatProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="c84b3-244">deviceThreatProtectionEnabled</span></span>|<span data-ttu-id="c84b3-245">Boolean</span><span class="sxs-lookup"><span data-stu-id="c84b3-245">Boolean</span></span>|<span data-ttu-id="c84b3-246">要求设备已启用设备威胁防护。</span><span class="sxs-lookup"><span data-stu-id="c84b3-246">Require that devices have enabled device threat protection.</span></span>|
|<span data-ttu-id="c84b3-247">deviceThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="c84b3-247">deviceThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="c84b3-248">deviceThreatProtectionLevel</span><span class="sxs-lookup"><span data-stu-id="c84b3-248">deviceThreatProtectionLevel</span></span>](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|<span data-ttu-id="c84b3-249">要求设备威胁保护最低风险级别报告如此。</span><span class="sxs-lookup"><span data-stu-id="c84b3-249">Require Device Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="c84b3-250">可取值为：`unavailable`、`secured`、`low`、`medium`、`high`、`notSet`。</span><span class="sxs-lookup"><span data-stu-id="c84b3-250">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="c84b3-251">configurationManagerComplianceRequired</span><span class="sxs-lookup"><span data-stu-id="c84b3-251">configurationManagerComplianceRequired</span></span>|<span data-ttu-id="c84b3-252">Boolean</span><span class="sxs-lookup"><span data-stu-id="c84b3-252">Boolean</span></span>|<span data-ttu-id="c84b3-253">需要考虑 Intune 合规性状态考虑 SCCM 合规性状态。</span><span class="sxs-lookup"><span data-stu-id="c84b3-253">Require to consider SCCM Compliance state into consideration for Intune Compliance State.</span></span>|



## <a name="response"></a><span data-ttu-id="c84b3-254">响应</span><span class="sxs-lookup"><span data-stu-id="c84b3-254">Response</span></span>
<span data-ttu-id="c84b3-255">如果成功，此方法会在响应正文中返回 `201 Created` 响应代码和 [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="c84b3-255">If successful, this method returns a `201 Created` response code and a [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c84b3-256">示例</span><span class="sxs-lookup"><span data-stu-id="c84b3-256">Example</span></span>

### <a name="request"></a><span data-ttu-id="c84b3-257">请求</span><span class="sxs-lookup"><span data-stu-id="c84b3-257">Request</span></span>
<span data-ttu-id="c84b3-258">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="c84b3-258">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="c84b3-259">响应</span><span class="sxs-lookup"><span data-stu-id="c84b3-259">Response</span></span>
<span data-ttu-id="c84b3-p113">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="c84b3-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




