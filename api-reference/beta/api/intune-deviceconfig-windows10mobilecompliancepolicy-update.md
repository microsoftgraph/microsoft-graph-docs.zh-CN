---
title: 更新 windows10MobileCompliancePolicy
description: 更新 windows10MobileCompliancePolicy 对象的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 1ddd6ce8eb7090ff87d8751383c3c4d3bb137e76
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35977333"
---
# <a name="update-windows10mobilecompliancepolicy"></a><span data-ttu-id="83168-103">更新 windows10MobileCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="83168-103">Update windows10MobileCompliancePolicy</span></span>

> <span data-ttu-id="83168-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="83168-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="83168-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="83168-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="83168-106">更新 [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="83168-106">Update the properties of a [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="83168-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="83168-107">Prerequisites</span></span>
<span data-ttu-id="83168-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="83168-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="83168-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="83168-110">Permission type</span></span>|<span data-ttu-id="83168-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="83168-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="83168-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="83168-112">Delegated (work or school account)</span></span>|<span data-ttu-id="83168-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="83168-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="83168-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="83168-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="83168-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="83168-115">Not supported.</span></span>|
|<span data-ttu-id="83168-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="83168-116">Application</span></span>|<span data-ttu-id="83168-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="83168-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="83168-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="83168-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="83168-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="83168-119">Request headers</span></span>
|<span data-ttu-id="83168-120">标头</span><span class="sxs-lookup"><span data-stu-id="83168-120">Header</span></span>|<span data-ttu-id="83168-121">值</span><span class="sxs-lookup"><span data-stu-id="83168-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="83168-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="83168-122">Authorization</span></span>|<span data-ttu-id="83168-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="83168-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="83168-124">接受</span><span class="sxs-lookup"><span data-stu-id="83168-124">Accept</span></span>|<span data-ttu-id="83168-125">application/json</span><span class="sxs-lookup"><span data-stu-id="83168-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="83168-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="83168-126">Request body</span></span>
<span data-ttu-id="83168-127">在请求正文中，提供 [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="83168-127">In the request body, supply a JSON representation for the [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md) object.</span></span>

<span data-ttu-id="83168-128">下表显示了创建 [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="83168-128">The following table shows the properties that are required when you create the [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md).</span></span>

|<span data-ttu-id="83168-129">属性</span><span class="sxs-lookup"><span data-stu-id="83168-129">Property</span></span>|<span data-ttu-id="83168-130">类型</span><span class="sxs-lookup"><span data-stu-id="83168-130">Type</span></span>|<span data-ttu-id="83168-131">说明</span><span class="sxs-lookup"><span data-stu-id="83168-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="83168-132">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="83168-132">roleScopeTagIds</span></span>|<span data-ttu-id="83168-133">String collection</span><span class="sxs-lookup"><span data-stu-id="83168-133">String collection</span></span>|<span data-ttu-id="83168-134">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="83168-134">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="83168-135">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="83168-135">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="83168-136">id</span><span class="sxs-lookup"><span data-stu-id="83168-136">id</span></span>|<span data-ttu-id="83168-137">字符串</span><span class="sxs-lookup"><span data-stu-id="83168-137">String</span></span>|<span data-ttu-id="83168-138">实体的键。</span><span class="sxs-lookup"><span data-stu-id="83168-138">Key of the entity.</span></span> <span data-ttu-id="83168-139">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="83168-139">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="83168-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="83168-140">createdDateTime</span></span>|<span data-ttu-id="83168-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="83168-141">DateTimeOffset</span></span>|<span data-ttu-id="83168-142">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="83168-142">DateTime the object was created.</span></span> <span data-ttu-id="83168-143">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="83168-143">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="83168-144">说明</span><span class="sxs-lookup"><span data-stu-id="83168-144">description</span></span>|<span data-ttu-id="83168-145">String</span><span class="sxs-lookup"><span data-stu-id="83168-145">String</span></span>|<span data-ttu-id="83168-146">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="83168-146">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="83168-147">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="83168-147">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="83168-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="83168-148">lastModifiedDateTime</span></span>|<span data-ttu-id="83168-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="83168-149">DateTimeOffset</span></span>|<span data-ttu-id="83168-150">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="83168-150">DateTime the object was last modified.</span></span> <span data-ttu-id="83168-151">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="83168-151">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="83168-152">displayName</span><span class="sxs-lookup"><span data-stu-id="83168-152">displayName</span></span>|<span data-ttu-id="83168-153">字符串</span><span class="sxs-lookup"><span data-stu-id="83168-153">String</span></span>|<span data-ttu-id="83168-154">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="83168-154">Admin provided name of the device configuration.</span></span> <span data-ttu-id="83168-155">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="83168-155">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="83168-156">version</span><span class="sxs-lookup"><span data-stu-id="83168-156">version</span></span>|<span data-ttu-id="83168-157">Int32</span><span class="sxs-lookup"><span data-stu-id="83168-157">Int32</span></span>|<span data-ttu-id="83168-158">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="83168-158">Version of the device configuration.</span></span> <span data-ttu-id="83168-159">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="83168-159">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="83168-160">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="83168-160">passwordRequired</span></span>|<span data-ttu-id="83168-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="83168-161">Boolean</span></span>|<span data-ttu-id="83168-162">需要密码才可解锁 Windows Phone 设备。</span><span class="sxs-lookup"><span data-stu-id="83168-162">Require a password to unlock Windows Phone device.</span></span>|
|<span data-ttu-id="83168-163">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="83168-163">passwordBlockSimple</span></span>|<span data-ttu-id="83168-164">Boolean</span><span class="sxs-lookup"><span data-stu-id="83168-164">Boolean</span></span>|<span data-ttu-id="83168-165">是否阻止同步日历。</span><span class="sxs-lookup"><span data-stu-id="83168-165">Whether or not to block syncing the calendar.</span></span>|
|<span data-ttu-id="83168-166">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="83168-166">passwordMinimumLength</span></span>|<span data-ttu-id="83168-167">Int32</span><span class="sxs-lookup"><span data-stu-id="83168-167">Int32</span></span>|<span data-ttu-id="83168-168">最短密码长度。</span><span class="sxs-lookup"><span data-stu-id="83168-168">Minimum password length.</span></span> <span data-ttu-id="83168-169">有效值为 4 至 16</span><span class="sxs-lookup"><span data-stu-id="83168-169">Valid values 4 to 16</span></span>|
|<span data-ttu-id="83168-170">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="83168-170">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="83168-171">Int32</span><span class="sxs-lookup"><span data-stu-id="83168-171">Int32</span></span>|<span data-ttu-id="83168-172">密码中必需的字符集数。</span><span class="sxs-lookup"><span data-stu-id="83168-172">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="83168-173">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="83168-173">passwordRequiredType</span></span>|[<span data-ttu-id="83168-174">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="83168-174">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="83168-175">必需的密码类型。</span><span class="sxs-lookup"><span data-stu-id="83168-175">The required password type.</span></span> <span data-ttu-id="83168-176">可取值为：`deviceDefault`、`alphanumeric`、`numeric`。</span><span class="sxs-lookup"><span data-stu-id="83168-176">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="83168-177">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="83168-177">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="83168-178">Int32</span><span class="sxs-lookup"><span data-stu-id="83168-178">Int32</span></span>|<span data-ttu-id="83168-179">防止重复使用的先前密码的数量。</span><span class="sxs-lookup"><span data-stu-id="83168-179">The number of previous passwords to prevent re-use of.</span></span>|
|<span data-ttu-id="83168-180">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="83168-180">passwordExpirationDays</span></span>|<span data-ttu-id="83168-181">Int32</span><span class="sxs-lookup"><span data-stu-id="83168-181">Int32</span></span>|<span data-ttu-id="83168-182">密码过期前的天数。</span><span class="sxs-lookup"><span data-stu-id="83168-182">Number of days before password expiration.</span></span> <span data-ttu-id="83168-183">有效值为 1 至 255</span><span class="sxs-lookup"><span data-stu-id="83168-183">Valid values 1 to 255</span></span>|
|<span data-ttu-id="83168-184">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="83168-184">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="83168-185">Int32</span><span class="sxs-lookup"><span data-stu-id="83168-185">Int32</span></span>|<span data-ttu-id="83168-186">在需要密码之前不活动的分钟数。</span><span class="sxs-lookup"><span data-stu-id="83168-186">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="83168-187">passwordRequireToUnlockFromIdle</span><span class="sxs-lookup"><span data-stu-id="83168-187">passwordRequireToUnlockFromIdle</span></span>|<span data-ttu-id="83168-188">Boolean</span><span class="sxs-lookup"><span data-stu-id="83168-188">Boolean</span></span>|<span data-ttu-id="83168-189">需要密码才可解锁空闲设备。</span><span class="sxs-lookup"><span data-stu-id="83168-189">Require a password to unlock an idle device.</span></span>|
|<span data-ttu-id="83168-190">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="83168-190">osMinimumVersion</span></span>|<span data-ttu-id="83168-191">String</span><span class="sxs-lookup"><span data-stu-id="83168-191">String</span></span>|<span data-ttu-id="83168-192">最低 Windows Phone 版本。</span><span class="sxs-lookup"><span data-stu-id="83168-192">Minimum Windows Phone version.</span></span>|
|<span data-ttu-id="83168-193">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="83168-193">osMaximumVersion</span></span>|<span data-ttu-id="83168-194">String</span><span class="sxs-lookup"><span data-stu-id="83168-194">String</span></span>|<span data-ttu-id="83168-195">最高 Windows Phone 版本。</span><span class="sxs-lookup"><span data-stu-id="83168-195">Maximum Windows Phone version.</span></span>|
|<span data-ttu-id="83168-196">earlyLaunchAntiMalwareDriverEnabled</span><span class="sxs-lookup"><span data-stu-id="83168-196">earlyLaunchAntiMalwareDriverEnabled</span></span>|<span data-ttu-id="83168-197">Boolean</span><span class="sxs-lookup"><span data-stu-id="83168-197">Boolean</span></span>|<span data-ttu-id="83168-198">要求设备由 Windows 设备运行状况证明报告为正常 - 提前启动反恶意驱动程序已启用。</span><span class="sxs-lookup"><span data-stu-id="83168-198">Require devices to be reported as healthy by Windows Device Health Attestation - early launch antimalware driver is enabled.</span></span>|
|<span data-ttu-id="83168-199">bitLockerEnabled</span><span class="sxs-lookup"><span data-stu-id="83168-199">bitLockerEnabled</span></span>|<span data-ttu-id="83168-200">Boolean</span><span class="sxs-lookup"><span data-stu-id="83168-200">Boolean</span></span>|<span data-ttu-id="83168-201">要求设备由 Windows 设备运行状况证明报告为正常 - bit locker 已启用。</span><span class="sxs-lookup"><span data-stu-id="83168-201">Require devices to be reported healthy by Windows Device Health Attestation - bit locker is enabled</span></span>|
|<span data-ttu-id="83168-202">secureBootEnabled</span><span class="sxs-lookup"><span data-stu-id="83168-202">secureBootEnabled</span></span>|<span data-ttu-id="83168-203">Boolean</span><span class="sxs-lookup"><span data-stu-id="83168-203">Boolean</span></span>|<span data-ttu-id="83168-204">要求设备由 Windows 设备运行状况证明报告为正常 - 安全启动已启用。</span><span class="sxs-lookup"><span data-stu-id="83168-204">Require devices to be reported as healthy by Windows Device Health Attestation - secure boot is enabled.</span></span>|
|<span data-ttu-id="83168-205">codeIntegrityEnabled</span><span class="sxs-lookup"><span data-stu-id="83168-205">codeIntegrityEnabled</span></span>|<span data-ttu-id="83168-206">Boolean</span><span class="sxs-lookup"><span data-stu-id="83168-206">Boolean</span></span>|<span data-ttu-id="83168-207">要求设备由 Windows 设备运行状况证明报告为正常。</span><span class="sxs-lookup"><span data-stu-id="83168-207">Require devices to be reported as healthy by Windows Device Health Attestation.</span></span>|
|<span data-ttu-id="83168-208">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="83168-208">storageRequireEncryption</span></span>|<span data-ttu-id="83168-209">Boolean</span><span class="sxs-lookup"><span data-stu-id="83168-209">Boolean</span></span>|<span data-ttu-id="83168-210">要求对 Windows 设备加密。</span><span class="sxs-lookup"><span data-stu-id="83168-210">Require encryption on windows devices.</span></span>|
|<span data-ttu-id="83168-211">activeFirewallRequired</span><span class="sxs-lookup"><span data-stu-id="83168-211">activeFirewallRequired</span></span>|<span data-ttu-id="83168-212">Boolean</span><span class="sxs-lookup"><span data-stu-id="83168-212">Boolean</span></span>|<span data-ttu-id="83168-213">在 Windows 设备上需要活动防火墙。</span><span class="sxs-lookup"><span data-stu-id="83168-213">Require active firewall on Windows devices.</span></span>|
|<span data-ttu-id="83168-214">validOperatingSystemBuildRanges</span><span class="sxs-lookup"><span data-stu-id="83168-214">validOperatingSystemBuildRanges</span></span>|<span data-ttu-id="83168-215">[operatingSystemVersionRange](../resources/intune-deviceconfig-operatingsystemversionrange.md)集合</span><span class="sxs-lookup"><span data-stu-id="83168-215">[operatingSystemVersionRange](../resources/intune-deviceconfig-operatingsystemversionrange.md) collection</span></span>|<span data-ttu-id="83168-216">Windows 设备上的有效操作系统内部版本范围。</span><span class="sxs-lookup"><span data-stu-id="83168-216">The valid operating system build ranges on Windows devices.</span></span> <span data-ttu-id="83168-217">该集合最多可包含 10000 个元素。</span><span class="sxs-lookup"><span data-stu-id="83168-217">This collection can contain a maximum of 10000 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="83168-218">响应</span><span class="sxs-lookup"><span data-stu-id="83168-218">Response</span></span>
<span data-ttu-id="83168-219">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和更新的 [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="83168-219">If successful, this method returns a `200 OK` response code and an updated [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="83168-220">示例</span><span class="sxs-lookup"><span data-stu-id="83168-220">Example</span></span>

### <a name="request"></a><span data-ttu-id="83168-221">请求</span><span class="sxs-lookup"><span data-stu-id="83168-221">Request</span></span>
<span data-ttu-id="83168-222">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="83168-222">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="83168-223">响应</span><span class="sxs-lookup"><span data-stu-id="83168-223">Response</span></span>
<span data-ttu-id="83168-p113">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="83168-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





