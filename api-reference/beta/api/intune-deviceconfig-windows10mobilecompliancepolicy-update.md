---
title: 更新 windows10MobileCompliancePolicy
description: 更新 windows10MobileCompliancePolicy 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: c1858040856180b2940b5ae5c74f2fbee224cb80
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51127674"
---
# <a name="update-windows10mobilecompliancepolicy"></a><span data-ttu-id="c50c0-103">更新 windows10MobileCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="c50c0-103">Update windows10MobileCompliancePolicy</span></span>

<span data-ttu-id="c50c0-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c50c0-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c50c0-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="c50c0-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c50c0-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c50c0-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c50c0-107">更新 [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="c50c0-107">Update the properties of a [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c50c0-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="c50c0-108">Prerequisites</span></span>
<span data-ttu-id="c50c0-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c50c0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c50c0-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="c50c0-111">Permission type</span></span>|<span data-ttu-id="c50c0-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c50c0-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c50c0-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c50c0-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c50c0-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c50c0-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c50c0-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c50c0-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c50c0-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="c50c0-116">Not supported.</span></span>|
|<span data-ttu-id="c50c0-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="c50c0-117">Application</span></span>|<span data-ttu-id="c50c0-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c50c0-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c50c0-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c50c0-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="c50c0-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="c50c0-120">Request headers</span></span>
|<span data-ttu-id="c50c0-121">标头</span><span class="sxs-lookup"><span data-stu-id="c50c0-121">Header</span></span>|<span data-ttu-id="c50c0-122">值</span><span class="sxs-lookup"><span data-stu-id="c50c0-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c50c0-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c50c0-123">Authorization</span></span>|<span data-ttu-id="c50c0-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="c50c0-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c50c0-125">接受</span><span class="sxs-lookup"><span data-stu-id="c50c0-125">Accept</span></span>|<span data-ttu-id="c50c0-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c50c0-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c50c0-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="c50c0-127">Request body</span></span>
<span data-ttu-id="c50c0-128">在请求正文中，提供 [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c50c0-128">In the request body, supply a JSON representation for the [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md) object.</span></span>

<span data-ttu-id="c50c0-129">下表显示了创建 [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="c50c0-129">The following table shows the properties that are required when you create the [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md).</span></span>

|<span data-ttu-id="c50c0-130">属性</span><span class="sxs-lookup"><span data-stu-id="c50c0-130">Property</span></span>|<span data-ttu-id="c50c0-131">类型</span><span class="sxs-lookup"><span data-stu-id="c50c0-131">Type</span></span>|<span data-ttu-id="c50c0-132">说明</span><span class="sxs-lookup"><span data-stu-id="c50c0-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c50c0-133">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="c50c0-133">roleScopeTagIds</span></span>|<span data-ttu-id="c50c0-134">String collection</span><span class="sxs-lookup"><span data-stu-id="c50c0-134">String collection</span></span>|<span data-ttu-id="c50c0-135">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="c50c0-135">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="c50c0-136">继承自 [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="c50c0-136">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="c50c0-137">id</span><span class="sxs-lookup"><span data-stu-id="c50c0-137">id</span></span>|<span data-ttu-id="c50c0-138">String</span><span class="sxs-lookup"><span data-stu-id="c50c0-138">String</span></span>|<span data-ttu-id="c50c0-139">实体的键。</span><span class="sxs-lookup"><span data-stu-id="c50c0-139">Key of the entity.</span></span> <span data-ttu-id="c50c0-140">继承自 [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="c50c0-140">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="c50c0-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c50c0-141">createdDateTime</span></span>|<span data-ttu-id="c50c0-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c50c0-142">DateTimeOffset</span></span>|<span data-ttu-id="c50c0-143">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="c50c0-143">DateTime the object was created.</span></span> <span data-ttu-id="c50c0-144">继承自 [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="c50c0-144">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="c50c0-145">说明</span><span class="sxs-lookup"><span data-stu-id="c50c0-145">description</span></span>|<span data-ttu-id="c50c0-146">String</span><span class="sxs-lookup"><span data-stu-id="c50c0-146">String</span></span>|<span data-ttu-id="c50c0-147">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="c50c0-147">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="c50c0-148">继承自 [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="c50c0-148">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="c50c0-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c50c0-149">lastModifiedDateTime</span></span>|<span data-ttu-id="c50c0-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c50c0-150">DateTimeOffset</span></span>|<span data-ttu-id="c50c0-151">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="c50c0-151">DateTime the object was last modified.</span></span> <span data-ttu-id="c50c0-152">继承自 [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="c50c0-152">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="c50c0-153">displayName</span><span class="sxs-lookup"><span data-stu-id="c50c0-153">displayName</span></span>|<span data-ttu-id="c50c0-154">String</span><span class="sxs-lookup"><span data-stu-id="c50c0-154">String</span></span>|<span data-ttu-id="c50c0-155">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="c50c0-155">Admin provided name of the device configuration.</span></span> <span data-ttu-id="c50c0-156">继承自 [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="c50c0-156">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="c50c0-157">version</span><span class="sxs-lookup"><span data-stu-id="c50c0-157">version</span></span>|<span data-ttu-id="c50c0-158">Int32</span><span class="sxs-lookup"><span data-stu-id="c50c0-158">Int32</span></span>|<span data-ttu-id="c50c0-159">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="c50c0-159">Version of the device configuration.</span></span> <span data-ttu-id="c50c0-160">继承自 [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="c50c0-160">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="c50c0-161">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="c50c0-161">passwordRequired</span></span>|<span data-ttu-id="c50c0-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="c50c0-162">Boolean</span></span>|<span data-ttu-id="c50c0-163">需要密码才可解锁 Windows Phone 设备。</span><span class="sxs-lookup"><span data-stu-id="c50c0-163">Require a password to unlock Windows Phone device.</span></span>|
|<span data-ttu-id="c50c0-164">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="c50c0-164">passwordBlockSimple</span></span>|<span data-ttu-id="c50c0-165">Boolean</span><span class="sxs-lookup"><span data-stu-id="c50c0-165">Boolean</span></span>|<span data-ttu-id="c50c0-166">是否阻止同步日历。</span><span class="sxs-lookup"><span data-stu-id="c50c0-166">Whether or not to block syncing the calendar.</span></span>|
|<span data-ttu-id="c50c0-167">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="c50c0-167">passwordMinimumLength</span></span>|<span data-ttu-id="c50c0-168">Int32</span><span class="sxs-lookup"><span data-stu-id="c50c0-168">Int32</span></span>|<span data-ttu-id="c50c0-169">最短密码长度。</span><span class="sxs-lookup"><span data-stu-id="c50c0-169">Minimum password length.</span></span> <span data-ttu-id="c50c0-170">有效值为 4 至 16</span><span class="sxs-lookup"><span data-stu-id="c50c0-170">Valid values 4 to 16</span></span>|
|<span data-ttu-id="c50c0-171">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="c50c0-171">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="c50c0-172">Int32</span><span class="sxs-lookup"><span data-stu-id="c50c0-172">Int32</span></span>|<span data-ttu-id="c50c0-173">密码中必需的字符集数。</span><span class="sxs-lookup"><span data-stu-id="c50c0-173">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="c50c0-174">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="c50c0-174">passwordRequiredType</span></span>|[<span data-ttu-id="c50c0-175">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="c50c0-175">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="c50c0-176">必需的密码类型。</span><span class="sxs-lookup"><span data-stu-id="c50c0-176">The required password type.</span></span> <span data-ttu-id="c50c0-177">可取值为：`deviceDefault`、`alphanumeric`、`numeric`。</span><span class="sxs-lookup"><span data-stu-id="c50c0-177">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="c50c0-178">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="c50c0-178">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="c50c0-179">Int32</span><span class="sxs-lookup"><span data-stu-id="c50c0-179">Int32</span></span>|<span data-ttu-id="c50c0-180">防止重复使用的先前密码的数量。</span><span class="sxs-lookup"><span data-stu-id="c50c0-180">The number of previous passwords to prevent re-use of.</span></span>|
|<span data-ttu-id="c50c0-181">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="c50c0-181">passwordExpirationDays</span></span>|<span data-ttu-id="c50c0-182">Int32</span><span class="sxs-lookup"><span data-stu-id="c50c0-182">Int32</span></span>|<span data-ttu-id="c50c0-183">密码过期前的天数。</span><span class="sxs-lookup"><span data-stu-id="c50c0-183">Number of days before password expiration.</span></span> <span data-ttu-id="c50c0-184">有效值为 1 至 255</span><span class="sxs-lookup"><span data-stu-id="c50c0-184">Valid values 1 to 255</span></span>|
|<span data-ttu-id="c50c0-185">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="c50c0-185">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="c50c0-186">Int32</span><span class="sxs-lookup"><span data-stu-id="c50c0-186">Int32</span></span>|<span data-ttu-id="c50c0-187">在需要密码之前不活动的分钟数。</span><span class="sxs-lookup"><span data-stu-id="c50c0-187">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="c50c0-188">passwordRequireToUnlockFromIdle</span><span class="sxs-lookup"><span data-stu-id="c50c0-188">passwordRequireToUnlockFromIdle</span></span>|<span data-ttu-id="c50c0-189">Boolean</span><span class="sxs-lookup"><span data-stu-id="c50c0-189">Boolean</span></span>|<span data-ttu-id="c50c0-190">需要密码才可解锁空闲设备。</span><span class="sxs-lookup"><span data-stu-id="c50c0-190">Require a password to unlock an idle device.</span></span>|
|<span data-ttu-id="c50c0-191">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="c50c0-191">osMinimumVersion</span></span>|<span data-ttu-id="c50c0-192">String</span><span class="sxs-lookup"><span data-stu-id="c50c0-192">String</span></span>|<span data-ttu-id="c50c0-193">最低 Windows Phone 版本。</span><span class="sxs-lookup"><span data-stu-id="c50c0-193">Minimum Windows Phone version.</span></span>|
|<span data-ttu-id="c50c0-194">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="c50c0-194">osMaximumVersion</span></span>|<span data-ttu-id="c50c0-195">String</span><span class="sxs-lookup"><span data-stu-id="c50c0-195">String</span></span>|<span data-ttu-id="c50c0-196">最高 Windows Phone 版本。</span><span class="sxs-lookup"><span data-stu-id="c50c0-196">Maximum Windows Phone version.</span></span>|
|<span data-ttu-id="c50c0-197">earlyLaunchAntiMalwareDriverEnabled</span><span class="sxs-lookup"><span data-stu-id="c50c0-197">earlyLaunchAntiMalwareDriverEnabled</span></span>|<span data-ttu-id="c50c0-198">Boolean</span><span class="sxs-lookup"><span data-stu-id="c50c0-198">Boolean</span></span>|<span data-ttu-id="c50c0-199">要求设备由 Windows 设备运行状况证明报告为正常 - 提前启动反恶意驱动程序已启用。</span><span class="sxs-lookup"><span data-stu-id="c50c0-199">Require devices to be reported as healthy by Windows Device Health Attestation - early launch antimalware driver is enabled.</span></span>|
|<span data-ttu-id="c50c0-200">bitLockerEnabled</span><span class="sxs-lookup"><span data-stu-id="c50c0-200">bitLockerEnabled</span></span>|<span data-ttu-id="c50c0-201">Boolean</span><span class="sxs-lookup"><span data-stu-id="c50c0-201">Boolean</span></span>|<span data-ttu-id="c50c0-202">要求设备由 Windows 设备运行状况证明报告为正常 - bit locker 已启用。</span><span class="sxs-lookup"><span data-stu-id="c50c0-202">Require devices to be reported healthy by Windows Device Health Attestation - bit locker is enabled</span></span>|
|<span data-ttu-id="c50c0-203">secureBootEnabled</span><span class="sxs-lookup"><span data-stu-id="c50c0-203">secureBootEnabled</span></span>|<span data-ttu-id="c50c0-204">Boolean</span><span class="sxs-lookup"><span data-stu-id="c50c0-204">Boolean</span></span>|<span data-ttu-id="c50c0-205">要求设备由 Windows 设备运行状况证明报告为正常 - 安全启动已启用。</span><span class="sxs-lookup"><span data-stu-id="c50c0-205">Require devices to be reported as healthy by Windows Device Health Attestation - secure boot is enabled.</span></span>|
|<span data-ttu-id="c50c0-206">codeIntegrityEnabled</span><span class="sxs-lookup"><span data-stu-id="c50c0-206">codeIntegrityEnabled</span></span>|<span data-ttu-id="c50c0-207">Boolean</span><span class="sxs-lookup"><span data-stu-id="c50c0-207">Boolean</span></span>|<span data-ttu-id="c50c0-208">要求设备由 Windows 设备运行状况证明报告为正常。</span><span class="sxs-lookup"><span data-stu-id="c50c0-208">Require devices to be reported as healthy by Windows Device Health Attestation.</span></span>|
|<span data-ttu-id="c50c0-209">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="c50c0-209">storageRequireEncryption</span></span>|<span data-ttu-id="c50c0-210">Boolean</span><span class="sxs-lookup"><span data-stu-id="c50c0-210">Boolean</span></span>|<span data-ttu-id="c50c0-211">要求对 Windows 设备加密。</span><span class="sxs-lookup"><span data-stu-id="c50c0-211">Require encryption on windows devices.</span></span>|
|<span data-ttu-id="c50c0-212">activeFirewallRequired</span><span class="sxs-lookup"><span data-stu-id="c50c0-212">activeFirewallRequired</span></span>|<span data-ttu-id="c50c0-213">Boolean</span><span class="sxs-lookup"><span data-stu-id="c50c0-213">Boolean</span></span>|<span data-ttu-id="c50c0-214">在 Windows 设备上需要活动防火墙。</span><span class="sxs-lookup"><span data-stu-id="c50c0-214">Require active firewall on Windows devices.</span></span>|
|<span data-ttu-id="c50c0-215">validOperatingSystemBuildRanges</span><span class="sxs-lookup"><span data-stu-id="c50c0-215">validOperatingSystemBuildRanges</span></span>|<span data-ttu-id="c50c0-216">[operatingSystemVersionRange](../resources/intune-deviceconfig-operatingsystemversionrange.md) 集合</span><span class="sxs-lookup"><span data-stu-id="c50c0-216">[operatingSystemVersionRange](../resources/intune-deviceconfig-operatingsystemversionrange.md) collection</span></span>|<span data-ttu-id="c50c0-217">Windows 设备上有效的操作系统生成范围。</span><span class="sxs-lookup"><span data-stu-id="c50c0-217">The valid operating system build ranges on Windows devices.</span></span> <span data-ttu-id="c50c0-218">该集合最多可包含 10000 个元素。</span><span class="sxs-lookup"><span data-stu-id="c50c0-218">This collection can contain a maximum of 10000 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="c50c0-219">响应</span><span class="sxs-lookup"><span data-stu-id="c50c0-219">Response</span></span>
<span data-ttu-id="c50c0-220">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和更新的 [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="c50c0-220">If successful, this method returns a `200 OK` response code and an updated [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c50c0-221">示例</span><span class="sxs-lookup"><span data-stu-id="c50c0-221">Example</span></span>

### <a name="request"></a><span data-ttu-id="c50c0-222">请求</span><span class="sxs-lookup"><span data-stu-id="c50c0-222">Request</span></span>
<span data-ttu-id="c50c0-223">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="c50c0-223">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
Content-type: application/json
Content-length: 1158

{
  "@odata.type": "#microsoft.graph.windows10MobileCompliancePolicy",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "description": "Description value",
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

### <a name="response"></a><span data-ttu-id="c50c0-224">响应</span><span class="sxs-lookup"><span data-stu-id="c50c0-224">Response</span></span>
<span data-ttu-id="c50c0-p113">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="c50c0-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




