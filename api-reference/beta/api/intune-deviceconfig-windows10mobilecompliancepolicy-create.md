---
title: 创建 windows10MobileCompliancePolicy
description: 创建新的 windows10MobileCompliancePolicy 对象。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 37e8ae87869e6cd76e80a589c80b3f63e849dda1
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36345153"
---
# <a name="create-windows10mobilecompliancepolicy"></a><span data-ttu-id="f6f65-103">创建 windows10MobileCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="f6f65-103">Create windows10MobileCompliancePolicy</span></span>

> <span data-ttu-id="f6f65-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="f6f65-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f6f65-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f6f65-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f6f65-106">创建新的 [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="f6f65-106">Create a new [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f6f65-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="f6f65-107">Prerequisites</span></span>
<span data-ttu-id="f6f65-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f6f65-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f6f65-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="f6f65-110">Permission type</span></span>|<span data-ttu-id="f6f65-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="f6f65-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f6f65-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f6f65-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f6f65-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f6f65-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f6f65-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f6f65-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f6f65-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="f6f65-115">Not supported.</span></span>|
|<span data-ttu-id="f6f65-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="f6f65-116">Application</span></span>|<span data-ttu-id="f6f65-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f6f65-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f6f65-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f6f65-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="f6f65-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="f6f65-119">Request headers</span></span>
|<span data-ttu-id="f6f65-120">标头</span><span class="sxs-lookup"><span data-stu-id="f6f65-120">Header</span></span>|<span data-ttu-id="f6f65-121">值</span><span class="sxs-lookup"><span data-stu-id="f6f65-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f6f65-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="f6f65-122">Authorization</span></span>|<span data-ttu-id="f6f65-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="f6f65-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f6f65-124">接受</span><span class="sxs-lookup"><span data-stu-id="f6f65-124">Accept</span></span>|<span data-ttu-id="f6f65-125">application/json</span><span class="sxs-lookup"><span data-stu-id="f6f65-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f6f65-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="f6f65-126">Request body</span></span>
<span data-ttu-id="f6f65-127">在请求正文中，提供 windows10MobileCompliancePolicy 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f6f65-127">In the request body, supply a JSON representation for the windows10MobileCompliancePolicy object.</span></span>

<span data-ttu-id="f6f65-128">下表显示了创建 windows10MobileCompliancePolicy 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="f6f65-128">The following table shows the properties that are required when you create the windows10MobileCompliancePolicy.</span></span>

|<span data-ttu-id="f6f65-129">属性</span><span class="sxs-lookup"><span data-stu-id="f6f65-129">Property</span></span>|<span data-ttu-id="f6f65-130">类型</span><span class="sxs-lookup"><span data-stu-id="f6f65-130">Type</span></span>|<span data-ttu-id="f6f65-131">说明</span><span class="sxs-lookup"><span data-stu-id="f6f65-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f6f65-132">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="f6f65-132">roleScopeTagIds</span></span>|<span data-ttu-id="f6f65-133">String collection</span><span class="sxs-lookup"><span data-stu-id="f6f65-133">String collection</span></span>|<span data-ttu-id="f6f65-134">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="f6f65-134">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="f6f65-135">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="f6f65-135">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="f6f65-136">id</span><span class="sxs-lookup"><span data-stu-id="f6f65-136">id</span></span>|<span data-ttu-id="f6f65-137">字符串</span><span class="sxs-lookup"><span data-stu-id="f6f65-137">String</span></span>|<span data-ttu-id="f6f65-138">实体的键。</span><span class="sxs-lookup"><span data-stu-id="f6f65-138">Key of the entity.</span></span> <span data-ttu-id="f6f65-139">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="f6f65-139">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="f6f65-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f6f65-140">createdDateTime</span></span>|<span data-ttu-id="f6f65-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f6f65-141">DateTimeOffset</span></span>|<span data-ttu-id="f6f65-142">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="f6f65-142">DateTime the object was created.</span></span> <span data-ttu-id="f6f65-143">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="f6f65-143">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="f6f65-144">说明</span><span class="sxs-lookup"><span data-stu-id="f6f65-144">description</span></span>|<span data-ttu-id="f6f65-145">String</span><span class="sxs-lookup"><span data-stu-id="f6f65-145">String</span></span>|<span data-ttu-id="f6f65-146">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="f6f65-146">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="f6f65-147">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="f6f65-147">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="f6f65-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f6f65-148">lastModifiedDateTime</span></span>|<span data-ttu-id="f6f65-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f6f65-149">DateTimeOffset</span></span>|<span data-ttu-id="f6f65-150">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="f6f65-150">DateTime the object was last modified.</span></span> <span data-ttu-id="f6f65-151">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="f6f65-151">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="f6f65-152">displayName</span><span class="sxs-lookup"><span data-stu-id="f6f65-152">displayName</span></span>|<span data-ttu-id="f6f65-153">字符串</span><span class="sxs-lookup"><span data-stu-id="f6f65-153">String</span></span>|<span data-ttu-id="f6f65-154">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="f6f65-154">Admin provided name of the device configuration.</span></span> <span data-ttu-id="f6f65-155">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="f6f65-155">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="f6f65-156">version</span><span class="sxs-lookup"><span data-stu-id="f6f65-156">version</span></span>|<span data-ttu-id="f6f65-157">Int32</span><span class="sxs-lookup"><span data-stu-id="f6f65-157">Int32</span></span>|<span data-ttu-id="f6f65-158">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="f6f65-158">Version of the device configuration.</span></span> <span data-ttu-id="f6f65-159">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="f6f65-159">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="f6f65-160">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="f6f65-160">passwordRequired</span></span>|<span data-ttu-id="f6f65-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="f6f65-161">Boolean</span></span>|<span data-ttu-id="f6f65-162">需要密码才可解锁 Windows Phone 设备。</span><span class="sxs-lookup"><span data-stu-id="f6f65-162">Require a password to unlock Windows Phone device.</span></span>|
|<span data-ttu-id="f6f65-163">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="f6f65-163">passwordBlockSimple</span></span>|<span data-ttu-id="f6f65-164">Boolean</span><span class="sxs-lookup"><span data-stu-id="f6f65-164">Boolean</span></span>|<span data-ttu-id="f6f65-165">是否阻止同步日历。</span><span class="sxs-lookup"><span data-stu-id="f6f65-165">Whether or not to block syncing the calendar.</span></span>|
|<span data-ttu-id="f6f65-166">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="f6f65-166">passwordMinimumLength</span></span>|<span data-ttu-id="f6f65-167">Int32</span><span class="sxs-lookup"><span data-stu-id="f6f65-167">Int32</span></span>|<span data-ttu-id="f6f65-168">最短密码长度。</span><span class="sxs-lookup"><span data-stu-id="f6f65-168">Minimum password length.</span></span> <span data-ttu-id="f6f65-169">有效值为 4 至 16</span><span class="sxs-lookup"><span data-stu-id="f6f65-169">Valid values 4 to 16</span></span>|
|<span data-ttu-id="f6f65-170">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="f6f65-170">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="f6f65-171">Int32</span><span class="sxs-lookup"><span data-stu-id="f6f65-171">Int32</span></span>|<span data-ttu-id="f6f65-172">密码中必需的字符集数。</span><span class="sxs-lookup"><span data-stu-id="f6f65-172">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="f6f65-173">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="f6f65-173">passwordRequiredType</span></span>|[<span data-ttu-id="f6f65-174">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="f6f65-174">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="f6f65-175">必需的密码类型。</span><span class="sxs-lookup"><span data-stu-id="f6f65-175">The required password type.</span></span> <span data-ttu-id="f6f65-176">可取值为：`deviceDefault`、`alphanumeric`、`numeric`。</span><span class="sxs-lookup"><span data-stu-id="f6f65-176">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="f6f65-177">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="f6f65-177">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="f6f65-178">Int32</span><span class="sxs-lookup"><span data-stu-id="f6f65-178">Int32</span></span>|<span data-ttu-id="f6f65-179">防止重复使用的先前密码的数量。</span><span class="sxs-lookup"><span data-stu-id="f6f65-179">The number of previous passwords to prevent re-use of.</span></span>|
|<span data-ttu-id="f6f65-180">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="f6f65-180">passwordExpirationDays</span></span>|<span data-ttu-id="f6f65-181">Int32</span><span class="sxs-lookup"><span data-stu-id="f6f65-181">Int32</span></span>|<span data-ttu-id="f6f65-182">密码过期前的天数。</span><span class="sxs-lookup"><span data-stu-id="f6f65-182">Number of days before password expiration.</span></span> <span data-ttu-id="f6f65-183">有效值为 1 至 255</span><span class="sxs-lookup"><span data-stu-id="f6f65-183">Valid values 1 to 255</span></span>|
|<span data-ttu-id="f6f65-184">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="f6f65-184">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="f6f65-185">Int32</span><span class="sxs-lookup"><span data-stu-id="f6f65-185">Int32</span></span>|<span data-ttu-id="f6f65-186">在需要密码之前不活动的分钟数。</span><span class="sxs-lookup"><span data-stu-id="f6f65-186">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="f6f65-187">passwordRequireToUnlockFromIdle</span><span class="sxs-lookup"><span data-stu-id="f6f65-187">passwordRequireToUnlockFromIdle</span></span>|<span data-ttu-id="f6f65-188">Boolean</span><span class="sxs-lookup"><span data-stu-id="f6f65-188">Boolean</span></span>|<span data-ttu-id="f6f65-189">需要密码才可解锁空闲设备。</span><span class="sxs-lookup"><span data-stu-id="f6f65-189">Require a password to unlock an idle device.</span></span>|
|<span data-ttu-id="f6f65-190">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="f6f65-190">osMinimumVersion</span></span>|<span data-ttu-id="f6f65-191">String</span><span class="sxs-lookup"><span data-stu-id="f6f65-191">String</span></span>|<span data-ttu-id="f6f65-192">最低 Windows Phone 版本。</span><span class="sxs-lookup"><span data-stu-id="f6f65-192">Minimum Windows Phone version.</span></span>|
|<span data-ttu-id="f6f65-193">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="f6f65-193">osMaximumVersion</span></span>|<span data-ttu-id="f6f65-194">String</span><span class="sxs-lookup"><span data-stu-id="f6f65-194">String</span></span>|<span data-ttu-id="f6f65-195">最高 Windows Phone 版本。</span><span class="sxs-lookup"><span data-stu-id="f6f65-195">Maximum Windows Phone version.</span></span>|
|<span data-ttu-id="f6f65-196">earlyLaunchAntiMalwareDriverEnabled</span><span class="sxs-lookup"><span data-stu-id="f6f65-196">earlyLaunchAntiMalwareDriverEnabled</span></span>|<span data-ttu-id="f6f65-197">Boolean</span><span class="sxs-lookup"><span data-stu-id="f6f65-197">Boolean</span></span>|<span data-ttu-id="f6f65-198">要求设备由 Windows 设备运行状况证明报告为正常 - 提前启动反恶意驱动程序已启用。</span><span class="sxs-lookup"><span data-stu-id="f6f65-198">Require devices to be reported as healthy by Windows Device Health Attestation - early launch antimalware driver is enabled.</span></span>|
|<span data-ttu-id="f6f65-199">bitLockerEnabled</span><span class="sxs-lookup"><span data-stu-id="f6f65-199">bitLockerEnabled</span></span>|<span data-ttu-id="f6f65-200">Boolean</span><span class="sxs-lookup"><span data-stu-id="f6f65-200">Boolean</span></span>|<span data-ttu-id="f6f65-201">要求设备由 Windows 设备运行状况证明报告为正常 - bit locker 已启用。</span><span class="sxs-lookup"><span data-stu-id="f6f65-201">Require devices to be reported healthy by Windows Device Health Attestation - bit locker is enabled</span></span>|
|<span data-ttu-id="f6f65-202">secureBootEnabled</span><span class="sxs-lookup"><span data-stu-id="f6f65-202">secureBootEnabled</span></span>|<span data-ttu-id="f6f65-203">Boolean</span><span class="sxs-lookup"><span data-stu-id="f6f65-203">Boolean</span></span>|<span data-ttu-id="f6f65-204">要求设备由 Windows 设备运行状况证明报告为正常 - 安全启动已启用。</span><span class="sxs-lookup"><span data-stu-id="f6f65-204">Require devices to be reported as healthy by Windows Device Health Attestation - secure boot is enabled.</span></span>|
|<span data-ttu-id="f6f65-205">codeIntegrityEnabled</span><span class="sxs-lookup"><span data-stu-id="f6f65-205">codeIntegrityEnabled</span></span>|<span data-ttu-id="f6f65-206">Boolean</span><span class="sxs-lookup"><span data-stu-id="f6f65-206">Boolean</span></span>|<span data-ttu-id="f6f65-207">要求设备由 Windows 设备运行状况证明报告为正常。</span><span class="sxs-lookup"><span data-stu-id="f6f65-207">Require devices to be reported as healthy by Windows Device Health Attestation.</span></span>|
|<span data-ttu-id="f6f65-208">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="f6f65-208">storageRequireEncryption</span></span>|<span data-ttu-id="f6f65-209">Boolean</span><span class="sxs-lookup"><span data-stu-id="f6f65-209">Boolean</span></span>|<span data-ttu-id="f6f65-210">要求对 Windows 设备加密。</span><span class="sxs-lookup"><span data-stu-id="f6f65-210">Require encryption on windows devices.</span></span>|
|<span data-ttu-id="f6f65-211">activeFirewallRequired</span><span class="sxs-lookup"><span data-stu-id="f6f65-211">activeFirewallRequired</span></span>|<span data-ttu-id="f6f65-212">Boolean</span><span class="sxs-lookup"><span data-stu-id="f6f65-212">Boolean</span></span>|<span data-ttu-id="f6f65-213">在 Windows 设备上需要活动防火墙。</span><span class="sxs-lookup"><span data-stu-id="f6f65-213">Require active firewall on Windows devices.</span></span>|
|<span data-ttu-id="f6f65-214">validOperatingSystemBuildRanges</span><span class="sxs-lookup"><span data-stu-id="f6f65-214">validOperatingSystemBuildRanges</span></span>|<span data-ttu-id="f6f65-215">[operatingSystemVersionRange](../resources/intune-deviceconfig-operatingsystemversionrange.md)集合</span><span class="sxs-lookup"><span data-stu-id="f6f65-215">[operatingSystemVersionRange](../resources/intune-deviceconfig-operatingsystemversionrange.md) collection</span></span>|<span data-ttu-id="f6f65-216">Windows 设备上的有效操作系统内部版本范围。</span><span class="sxs-lookup"><span data-stu-id="f6f65-216">The valid operating system build ranges on Windows devices.</span></span> <span data-ttu-id="f6f65-217">该集合最多可包含 10000 个元素。</span><span class="sxs-lookup"><span data-stu-id="f6f65-217">This collection can contain a maximum of 10000 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="f6f65-218">响应</span><span class="sxs-lookup"><span data-stu-id="f6f65-218">Response</span></span>
<span data-ttu-id="f6f65-219">如果成功，此方法将在响应正文中返回 `201 Created` 响应代码和 [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="f6f65-219">If successful, this method returns a `201 Created` response code and a [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f6f65-220">示例</span><span class="sxs-lookup"><span data-stu-id="f6f65-220">Example</span></span>

### <a name="request"></a><span data-ttu-id="f6f65-221">请求</span><span class="sxs-lookup"><span data-stu-id="f6f65-221">Request</span></span>
<span data-ttu-id="f6f65-222">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="f6f65-222">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies
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

### <a name="response"></a><span data-ttu-id="f6f65-223">响应</span><span class="sxs-lookup"><span data-stu-id="f6f65-223">Response</span></span>
<span data-ttu-id="f6f65-p113">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="f6f65-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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






