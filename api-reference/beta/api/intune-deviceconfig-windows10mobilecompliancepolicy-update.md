---
title: 更新 windows10MobileCompliancePolicy
description: 更新 windows10MobileCompliancePolicy 对象的属性。
author: tfitzmac
ms.openlocfilehash: f9a040ab544d112cbe98e579eebc918c52b6f46b
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27341963"
---
# <a name="update-windows10mobilecompliancepolicy"></a><span data-ttu-id="9dad3-103">更新 windows10MobileCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="9dad3-103">Update windows10MobileCompliancePolicy</span></span>

> <span data-ttu-id="9dad3-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="9dad3-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9dad3-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="9dad3-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9dad3-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="9dad3-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9dad3-107">更新 [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="9dad3-107">Update the properties of a [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="9dad3-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="9dad3-108">Prerequisites</span></span>
<span data-ttu-id="9dad3-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="9dad3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9dad3-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="9dad3-111">Permission type</span></span>|<span data-ttu-id="9dad3-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="9dad3-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9dad3-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9dad3-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9dad3-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9dad3-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="9dad3-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9dad3-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9dad3-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="9dad3-116">Not supported.</span></span>|
|<span data-ttu-id="9dad3-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="9dad3-117">Application</span></span>|<span data-ttu-id="9dad3-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="9dad3-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9dad3-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9dad3-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="9dad3-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="9dad3-120">Request headers</span></span>
|<span data-ttu-id="9dad3-121">标头</span><span class="sxs-lookup"><span data-stu-id="9dad3-121">Header</span></span>|<span data-ttu-id="9dad3-122">值</span><span class="sxs-lookup"><span data-stu-id="9dad3-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9dad3-123">授权</span><span class="sxs-lookup"><span data-stu-id="9dad3-123">Authorization</span></span>|<span data-ttu-id="9dad3-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="9dad3-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9dad3-125">Accept</span><span class="sxs-lookup"><span data-stu-id="9dad3-125">Accept</span></span>|<span data-ttu-id="9dad3-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9dad3-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9dad3-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="9dad3-127">Request body</span></span>
<span data-ttu-id="9dad3-128">在请求正文中，提供 [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9dad3-128">In the request body, supply a JSON representation for the [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md) object.</span></span>

<span data-ttu-id="9dad3-129">下表显示了创建 [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="9dad3-129">The following table shows the properties that are required when you create the [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md).</span></span>

|<span data-ttu-id="9dad3-130">属性</span><span class="sxs-lookup"><span data-stu-id="9dad3-130">Property</span></span>|<span data-ttu-id="9dad3-131">类型</span><span class="sxs-lookup"><span data-stu-id="9dad3-131">Type</span></span>|<span data-ttu-id="9dad3-132">说明</span><span class="sxs-lookup"><span data-stu-id="9dad3-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9dad3-133">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="9dad3-133">roleScopeTagIds</span></span>|<span data-ttu-id="9dad3-134">String 集合</span><span class="sxs-lookup"><span data-stu-id="9dad3-134">String collection</span></span>|<span data-ttu-id="9dad3-135">此实体实例范围标记的列表。</span><span class="sxs-lookup"><span data-stu-id="9dad3-135">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="9dad3-136">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="9dad3-136">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="9dad3-137">id</span><span class="sxs-lookup"><span data-stu-id="9dad3-137">id</span></span>|<span data-ttu-id="9dad3-138">String</span><span class="sxs-lookup"><span data-stu-id="9dad3-138">String</span></span>|<span data-ttu-id="9dad3-139">实体的键。</span><span class="sxs-lookup"><span data-stu-id="9dad3-139">Key of the entity.</span></span> <span data-ttu-id="9dad3-140">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="9dad3-140">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="9dad3-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="9dad3-141">createdDateTime</span></span>|<span data-ttu-id="9dad3-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9dad3-142">DateTimeOffset</span></span>|<span data-ttu-id="9dad3-143">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="9dad3-143">DateTime the object was created.</span></span> <span data-ttu-id="9dad3-144">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="9dad3-144">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="9dad3-145">description</span><span class="sxs-lookup"><span data-stu-id="9dad3-145">description</span></span>|<span data-ttu-id="9dad3-146">String</span><span class="sxs-lookup"><span data-stu-id="9dad3-146">String</span></span>|<span data-ttu-id="9dad3-147">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="9dad3-147">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="9dad3-148">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="9dad3-148">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="9dad3-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9dad3-149">lastModifiedDateTime</span></span>|<span data-ttu-id="9dad3-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9dad3-150">DateTimeOffset</span></span>|<span data-ttu-id="9dad3-151">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="9dad3-151">DateTime the object was last modified.</span></span> <span data-ttu-id="9dad3-152">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="9dad3-152">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="9dad3-153">displayName</span><span class="sxs-lookup"><span data-stu-id="9dad3-153">displayName</span></span>|<span data-ttu-id="9dad3-154">String</span><span class="sxs-lookup"><span data-stu-id="9dad3-154">String</span></span>|<span data-ttu-id="9dad3-155">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="9dad3-155">Admin provided name of the device configuration.</span></span> <span data-ttu-id="9dad3-156">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="9dad3-156">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="9dad3-157">version</span><span class="sxs-lookup"><span data-stu-id="9dad3-157">version</span></span>|<span data-ttu-id="9dad3-158">Int32</span><span class="sxs-lookup"><span data-stu-id="9dad3-158">Int32</span></span>|<span data-ttu-id="9dad3-159">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="9dad3-159">Version of the device configuration.</span></span> <span data-ttu-id="9dad3-160">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="9dad3-160">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="9dad3-161">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="9dad3-161">passwordRequired</span></span>|<span data-ttu-id="9dad3-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="9dad3-162">Boolean</span></span>|<span data-ttu-id="9dad3-163">需要密码才可解锁 Windows Phone 设备。</span><span class="sxs-lookup"><span data-stu-id="9dad3-163">Require a password to unlock Windows Phone device.</span></span>|
|<span data-ttu-id="9dad3-164">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="9dad3-164">passwordBlockSimple</span></span>|<span data-ttu-id="9dad3-165">Boolean</span><span class="sxs-lookup"><span data-stu-id="9dad3-165">Boolean</span></span>|<span data-ttu-id="9dad3-166">是否阻止同步日历。</span><span class="sxs-lookup"><span data-stu-id="9dad3-166">Whether or not to block syncing the calendar.</span></span>|
|<span data-ttu-id="9dad3-167">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="9dad3-167">passwordMinimumLength</span></span>|<span data-ttu-id="9dad3-168">Int32</span><span class="sxs-lookup"><span data-stu-id="9dad3-168">Int32</span></span>|<span data-ttu-id="9dad3-169">最短密码长度。</span><span class="sxs-lookup"><span data-stu-id="9dad3-169">Minimum password length.</span></span> <span data-ttu-id="9dad3-170">有效值为 4 至 16</span><span class="sxs-lookup"><span data-stu-id="9dad3-170">Valid values 4 to 16</span></span>|
|<span data-ttu-id="9dad3-171">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="9dad3-171">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="9dad3-172">Int32</span><span class="sxs-lookup"><span data-stu-id="9dad3-172">Int32</span></span>|<span data-ttu-id="9dad3-173">密码中必需的字符集数。</span><span class="sxs-lookup"><span data-stu-id="9dad3-173">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="9dad3-174">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="9dad3-174">passwordRequiredType</span></span>|[<span data-ttu-id="9dad3-175">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="9dad3-175">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="9dad3-176">必需的密码类型。</span><span class="sxs-lookup"><span data-stu-id="9dad3-176">The required password type.</span></span> <span data-ttu-id="9dad3-177">可取值为：`deviceDefault`、`alphanumeric`、`numeric`。</span><span class="sxs-lookup"><span data-stu-id="9dad3-177">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="9dad3-178">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="9dad3-178">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="9dad3-179">Int32</span><span class="sxs-lookup"><span data-stu-id="9dad3-179">Int32</span></span>|<span data-ttu-id="9dad3-180">防止重复使用的先前密码的数量。</span><span class="sxs-lookup"><span data-stu-id="9dad3-180">The number of previous passwords to prevent re-use of.</span></span>|
|<span data-ttu-id="9dad3-181">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="9dad3-181">passwordExpirationDays</span></span>|<span data-ttu-id="9dad3-182">Int32</span><span class="sxs-lookup"><span data-stu-id="9dad3-182">Int32</span></span>|<span data-ttu-id="9dad3-183">密码过期前的天数。</span><span class="sxs-lookup"><span data-stu-id="9dad3-183">Number of days before password expiration.</span></span> <span data-ttu-id="9dad3-184">有效值为 1 至 255</span><span class="sxs-lookup"><span data-stu-id="9dad3-184">Valid values 1 to 255</span></span>|
|<span data-ttu-id="9dad3-185">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="9dad3-185">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="9dad3-186">Int32</span><span class="sxs-lookup"><span data-stu-id="9dad3-186">Int32</span></span>|<span data-ttu-id="9dad3-187">在需要密码之前不活动的分钟数。</span><span class="sxs-lookup"><span data-stu-id="9dad3-187">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="9dad3-188">passwordRequireToUnlockFromIdle</span><span class="sxs-lookup"><span data-stu-id="9dad3-188">passwordRequireToUnlockFromIdle</span></span>|<span data-ttu-id="9dad3-189">Boolean</span><span class="sxs-lookup"><span data-stu-id="9dad3-189">Boolean</span></span>|<span data-ttu-id="9dad3-190">需要密码才可解锁空闲设备。</span><span class="sxs-lookup"><span data-stu-id="9dad3-190">Require a password to unlock an idle device.</span></span>|
|<span data-ttu-id="9dad3-191">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="9dad3-191">osMinimumVersion</span></span>|<span data-ttu-id="9dad3-192">String</span><span class="sxs-lookup"><span data-stu-id="9dad3-192">String</span></span>|<span data-ttu-id="9dad3-193">最低 Windows Phone 版本。</span><span class="sxs-lookup"><span data-stu-id="9dad3-193">Minimum Windows Phone version.</span></span>|
|<span data-ttu-id="9dad3-194">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="9dad3-194">osMaximumVersion</span></span>|<span data-ttu-id="9dad3-195">String</span><span class="sxs-lookup"><span data-stu-id="9dad3-195">String</span></span>|<span data-ttu-id="9dad3-196">最高 Windows Phone 版本。</span><span class="sxs-lookup"><span data-stu-id="9dad3-196">Maximum Windows Phone version.</span></span>|
|<span data-ttu-id="9dad3-197">earlyLaunchAntiMalwareDriverEnabled</span><span class="sxs-lookup"><span data-stu-id="9dad3-197">earlyLaunchAntiMalwareDriverEnabled</span></span>|<span data-ttu-id="9dad3-198">Boolean</span><span class="sxs-lookup"><span data-stu-id="9dad3-198">Boolean</span></span>|<span data-ttu-id="9dad3-199">要求设备由 Windows 设备运行状况证明报告为正常 - 提前启动反恶意驱动程序已启用。</span><span class="sxs-lookup"><span data-stu-id="9dad3-199">Require devices to be reported as healthy by Windows Device Health Attestation - early launch antimalware driver is enabled.</span></span>|
|<span data-ttu-id="9dad3-200">bitLockerEnabled</span><span class="sxs-lookup"><span data-stu-id="9dad3-200">bitLockerEnabled</span></span>|<span data-ttu-id="9dad3-201">Boolean</span><span class="sxs-lookup"><span data-stu-id="9dad3-201">Boolean</span></span>|<span data-ttu-id="9dad3-202">要求设备由 Windows 设备运行状况证明报告为正常 - bit locker 已启用。</span><span class="sxs-lookup"><span data-stu-id="9dad3-202">Require devices to be reported healthy by Windows Device Health Attestation - bit locker is enabled</span></span>|
|<span data-ttu-id="9dad3-203">secureBootEnabled</span><span class="sxs-lookup"><span data-stu-id="9dad3-203">secureBootEnabled</span></span>|<span data-ttu-id="9dad3-204">Boolean</span><span class="sxs-lookup"><span data-stu-id="9dad3-204">Boolean</span></span>|<span data-ttu-id="9dad3-205">要求设备由 Windows 设备运行状况证明报告为正常 - 安全启动已启用。</span><span class="sxs-lookup"><span data-stu-id="9dad3-205">Require devices to be reported as healthy by Windows Device Health Attestation - secure boot is enabled.</span></span>|
|<span data-ttu-id="9dad3-206">codeIntegrityEnabled</span><span class="sxs-lookup"><span data-stu-id="9dad3-206">codeIntegrityEnabled</span></span>|<span data-ttu-id="9dad3-207">Boolean</span><span class="sxs-lookup"><span data-stu-id="9dad3-207">Boolean</span></span>|<span data-ttu-id="9dad3-208">要求设备由 Windows 设备运行状况证明报告为正常。</span><span class="sxs-lookup"><span data-stu-id="9dad3-208">Require devices to be reported as healthy by Windows Device Health Attestation.</span></span>|
|<span data-ttu-id="9dad3-209">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="9dad3-209">storageRequireEncryption</span></span>|<span data-ttu-id="9dad3-210">Boolean</span><span class="sxs-lookup"><span data-stu-id="9dad3-210">Boolean</span></span>|<span data-ttu-id="9dad3-211">要求对 Windows 设备加密。</span><span class="sxs-lookup"><span data-stu-id="9dad3-211">Require encryption on windows devices.</span></span>|
|<span data-ttu-id="9dad3-212">activeFirewallRequired</span><span class="sxs-lookup"><span data-stu-id="9dad3-212">activeFirewallRequired</span></span>|<span data-ttu-id="9dad3-213">Boolean</span><span class="sxs-lookup"><span data-stu-id="9dad3-213">Boolean</span></span>|<span data-ttu-id="9dad3-214">要求在 Windows 设备上的活动防火墙。</span><span class="sxs-lookup"><span data-stu-id="9dad3-214">Require active firewall on Windows devices.</span></span>|
|<span data-ttu-id="9dad3-215">validOperatingSystemBuildRanges</span><span class="sxs-lookup"><span data-stu-id="9dad3-215">validOperatingSystemBuildRanges</span></span>|<span data-ttu-id="9dad3-216">[operatingSystemVersionRange](../resources/intune-deviceconfig-operatingsystemversionrange.md)集合</span><span class="sxs-lookup"><span data-stu-id="9dad3-216">[operatingSystemVersionRange](../resources/intune-deviceconfig-operatingsystemversionrange.md) collection</span></span>|<span data-ttu-id="9dad3-217">有效的操作系统构建 Windows 设备上的区域。</span><span class="sxs-lookup"><span data-stu-id="9dad3-217">The valid operating system build ranges on Windows devices.</span></span> <span data-ttu-id="9dad3-218">该集合最多可包含 10000 个元素。</span><span class="sxs-lookup"><span data-stu-id="9dad3-218">This collection can contain a maximum of 10000 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="9dad3-219">响应</span><span class="sxs-lookup"><span data-stu-id="9dad3-219">Response</span></span>
<span data-ttu-id="9dad3-220">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和更新的 [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="9dad3-220">If successful, this method returns a `200 OK` response code and an updated [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9dad3-221">示例</span><span class="sxs-lookup"><span data-stu-id="9dad3-221">Example</span></span>
### <a name="request"></a><span data-ttu-id="9dad3-222">请求</span><span class="sxs-lookup"><span data-stu-id="9dad3-222">Request</span></span>
<span data-ttu-id="9dad3-223">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="9dad3-223">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
Content-type: application/json
Content-length: 1152

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
  "passwordMinimumLength": 5,
  "passwordMinimumCharacterSetCount": 0,
  "passwordRequiredType": "alphanumeric",
  "passwordPreviousPasswordBlockCount": 2,
  "passwordExpirationDays": 6,
  "passwordMinutesOfInactivityBeforeLock": 5,
  "passwordRequireToUnlockFromIdle": true,
  "osMinimumVersion": "Os Minimum Version value",
  "osMaximumVersion": "Os Maximum Version value",
  "earlyLaunchAntiMalwareDriverEnabled": true,
  "bitLockerEnabled": true,
  "secureBootEnabled": true,
  "codeIntegrityEnabled": true,
  "storageRequireEncryption": true,
  "activeFirewallRequired": true,
  "validOperatingSystemBuildRanges": [
    {
      "@odata.type": "microsoft.graph.operatingSystemVersionRange",
      "description": "Description value",
      "lowestVersion": "Lowest Version value",
      "highestVersion": "Highest Version value"
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="9dad3-224">响应</span><span class="sxs-lookup"><span data-stu-id="9dad3-224">Response</span></span>
<span data-ttu-id="9dad3-p114">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="9dad3-p114">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1330

{
  "@odata.type": "#microsoft.graph.windows10MobileCompliancePolicy",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "id": "3d4237b0-37b0-3d42-b037-423db037423d",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "version": 7,
  "passwordRequired": true,
  "passwordBlockSimple": true,
  "passwordMinimumLength": 5,
  "passwordMinimumCharacterSetCount": 0,
  "passwordRequiredType": "alphanumeric",
  "passwordPreviousPasswordBlockCount": 2,
  "passwordExpirationDays": 6,
  "passwordMinutesOfInactivityBeforeLock": 5,
  "passwordRequireToUnlockFromIdle": true,
  "osMinimumVersion": "Os Minimum Version value",
  "osMaximumVersion": "Os Maximum Version value",
  "earlyLaunchAntiMalwareDriverEnabled": true,
  "bitLockerEnabled": true,
  "secureBootEnabled": true,
  "codeIntegrityEnabled": true,
  "storageRequireEncryption": true,
  "activeFirewallRequired": true,
  "validOperatingSystemBuildRanges": [
    {
      "@odata.type": "microsoft.graph.operatingSystemVersionRange",
      "description": "Description value",
      "lowestVersion": "Lowest Version value",
      "highestVersion": "Highest Version value"
    }
  ]
}
```





