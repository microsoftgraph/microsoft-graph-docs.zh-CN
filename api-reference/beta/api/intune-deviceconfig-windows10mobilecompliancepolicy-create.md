---
title: 创建 windows10MobileCompliancePolicy
description: 创建新的 windows10MobileCompliancePolicy 对象。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 0264cfc06961a485e02b07e02b3c71fd79874457
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27930423"
---
# <a name="create-windows10mobilecompliancepolicy"></a><span data-ttu-id="75470-103">创建 windows10MobileCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="75470-103">Create windows10MobileCompliancePolicy</span></span>

> <span data-ttu-id="75470-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="75470-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="75470-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="75470-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="75470-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="75470-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="75470-107">创建新的 [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="75470-107">Create a new [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="75470-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="75470-108">Prerequisites</span></span>
<span data-ttu-id="75470-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="75470-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="75470-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="75470-111">Permission type</span></span>|<span data-ttu-id="75470-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="75470-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="75470-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="75470-113">Delegated (work or school account)</span></span>|<span data-ttu-id="75470-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="75470-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="75470-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="75470-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="75470-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="75470-116">Not supported.</span></span>|
|<span data-ttu-id="75470-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="75470-117">Application</span></span>|<span data-ttu-id="75470-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="75470-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="75470-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="75470-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="75470-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="75470-120">Request headers</span></span>
|<span data-ttu-id="75470-121">标头</span><span class="sxs-lookup"><span data-stu-id="75470-121">Header</span></span>|<span data-ttu-id="75470-122">值</span><span class="sxs-lookup"><span data-stu-id="75470-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="75470-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="75470-123">Authorization</span></span>|<span data-ttu-id="75470-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="75470-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="75470-125">Accept</span><span class="sxs-lookup"><span data-stu-id="75470-125">Accept</span></span>|<span data-ttu-id="75470-126">application/json</span><span class="sxs-lookup"><span data-stu-id="75470-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="75470-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="75470-127">Request body</span></span>
<span data-ttu-id="75470-128">在请求正文中，提供 windows10MobileCompliancePolicy 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="75470-128">In the request body, supply a JSON representation for the windows10MobileCompliancePolicy object.</span></span>

<span data-ttu-id="75470-129">下表显示了创建 windows10MobileCompliancePolicy 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="75470-129">The following table shows the properties that are required when you create the windows10MobileCompliancePolicy.</span></span>

|<span data-ttu-id="75470-130">属性</span><span class="sxs-lookup"><span data-stu-id="75470-130">Property</span></span>|<span data-ttu-id="75470-131">类型</span><span class="sxs-lookup"><span data-stu-id="75470-131">Type</span></span>|<span data-ttu-id="75470-132">Description</span><span class="sxs-lookup"><span data-stu-id="75470-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="75470-133">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="75470-133">roleScopeTagIds</span></span>|<span data-ttu-id="75470-134">String 集合</span><span class="sxs-lookup"><span data-stu-id="75470-134">String collection</span></span>|<span data-ttu-id="75470-135">此实体实例范围标记的列表。</span><span class="sxs-lookup"><span data-stu-id="75470-135">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="75470-136">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="75470-136">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="75470-137">id</span><span class="sxs-lookup"><span data-stu-id="75470-137">id</span></span>|<span data-ttu-id="75470-138">String</span><span class="sxs-lookup"><span data-stu-id="75470-138">String</span></span>|<span data-ttu-id="75470-139">实体的键。</span><span class="sxs-lookup"><span data-stu-id="75470-139">Key of the entity.</span></span> <span data-ttu-id="75470-140">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="75470-140">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="75470-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="75470-141">createdDateTime</span></span>|<span data-ttu-id="75470-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="75470-142">DateTimeOffset</span></span>|<span data-ttu-id="75470-143">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="75470-143">DateTime the object was created.</span></span> <span data-ttu-id="75470-144">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="75470-144">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="75470-145">description</span><span class="sxs-lookup"><span data-stu-id="75470-145">description</span></span>|<span data-ttu-id="75470-146">String</span><span class="sxs-lookup"><span data-stu-id="75470-146">String</span></span>|<span data-ttu-id="75470-147">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="75470-147">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="75470-148">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="75470-148">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="75470-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="75470-149">lastModifiedDateTime</span></span>|<span data-ttu-id="75470-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="75470-150">DateTimeOffset</span></span>|<span data-ttu-id="75470-151">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="75470-151">DateTime the object was last modified.</span></span> <span data-ttu-id="75470-152">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="75470-152">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="75470-153">displayName</span><span class="sxs-lookup"><span data-stu-id="75470-153">displayName</span></span>|<span data-ttu-id="75470-154">String</span><span class="sxs-lookup"><span data-stu-id="75470-154">String</span></span>|<span data-ttu-id="75470-155">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="75470-155">Admin provided name of the device configuration.</span></span> <span data-ttu-id="75470-156">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="75470-156">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="75470-157">version</span><span class="sxs-lookup"><span data-stu-id="75470-157">version</span></span>|<span data-ttu-id="75470-158">Int32</span><span class="sxs-lookup"><span data-stu-id="75470-158">Int32</span></span>|<span data-ttu-id="75470-159">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="75470-159">Version of the device configuration.</span></span> <span data-ttu-id="75470-160">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="75470-160">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="75470-161">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="75470-161">passwordRequired</span></span>|<span data-ttu-id="75470-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="75470-162">Boolean</span></span>|<span data-ttu-id="75470-163">需要密码才可解锁 Windows Phone 设备。</span><span class="sxs-lookup"><span data-stu-id="75470-163">Require a password to unlock Windows Phone device.</span></span>|
|<span data-ttu-id="75470-164">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="75470-164">passwordBlockSimple</span></span>|<span data-ttu-id="75470-165">Boolean</span><span class="sxs-lookup"><span data-stu-id="75470-165">Boolean</span></span>|<span data-ttu-id="75470-166">是否阻止同步日历。</span><span class="sxs-lookup"><span data-stu-id="75470-166">Whether or not to block syncing the calendar.</span></span>|
|<span data-ttu-id="75470-167">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="75470-167">passwordMinimumLength</span></span>|<span data-ttu-id="75470-168">Int32</span><span class="sxs-lookup"><span data-stu-id="75470-168">Int32</span></span>|<span data-ttu-id="75470-169">最短密码长度。</span><span class="sxs-lookup"><span data-stu-id="75470-169">Minimum password length.</span></span> <span data-ttu-id="75470-170">有效值为 4 至 16</span><span class="sxs-lookup"><span data-stu-id="75470-170">Valid values 4 to 16</span></span>|
|<span data-ttu-id="75470-171">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="75470-171">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="75470-172">Int32</span><span class="sxs-lookup"><span data-stu-id="75470-172">Int32</span></span>|<span data-ttu-id="75470-173">密码中必需的字符集数。</span><span class="sxs-lookup"><span data-stu-id="75470-173">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="75470-174">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="75470-174">passwordRequiredType</span></span>|[<span data-ttu-id="75470-175">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="75470-175">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="75470-176">必需的密码类型。</span><span class="sxs-lookup"><span data-stu-id="75470-176">The required password type.</span></span> <span data-ttu-id="75470-177">可取值为：`deviceDefault`、`alphanumeric`、`numeric`。</span><span class="sxs-lookup"><span data-stu-id="75470-177">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="75470-178">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="75470-178">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="75470-179">Int32</span><span class="sxs-lookup"><span data-stu-id="75470-179">Int32</span></span>|<span data-ttu-id="75470-180">防止重复使用的先前密码的数量。</span><span class="sxs-lookup"><span data-stu-id="75470-180">The number of previous passwords to prevent re-use of.</span></span>|
|<span data-ttu-id="75470-181">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="75470-181">passwordExpirationDays</span></span>|<span data-ttu-id="75470-182">Int32</span><span class="sxs-lookup"><span data-stu-id="75470-182">Int32</span></span>|<span data-ttu-id="75470-183">密码过期前的天数。</span><span class="sxs-lookup"><span data-stu-id="75470-183">Number of days before password expiration.</span></span> <span data-ttu-id="75470-184">有效值为 1 至 255</span><span class="sxs-lookup"><span data-stu-id="75470-184">Valid values 1 to 255</span></span>|
|<span data-ttu-id="75470-185">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="75470-185">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="75470-186">Int32</span><span class="sxs-lookup"><span data-stu-id="75470-186">Int32</span></span>|<span data-ttu-id="75470-187">在需要密码之前不活动的分钟数。</span><span class="sxs-lookup"><span data-stu-id="75470-187">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="75470-188">passwordRequireToUnlockFromIdle</span><span class="sxs-lookup"><span data-stu-id="75470-188">passwordRequireToUnlockFromIdle</span></span>|<span data-ttu-id="75470-189">Boolean</span><span class="sxs-lookup"><span data-stu-id="75470-189">Boolean</span></span>|<span data-ttu-id="75470-190">需要密码才可解锁空闲设备。</span><span class="sxs-lookup"><span data-stu-id="75470-190">Require a password to unlock an idle device.</span></span>|
|<span data-ttu-id="75470-191">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="75470-191">osMinimumVersion</span></span>|<span data-ttu-id="75470-192">String</span><span class="sxs-lookup"><span data-stu-id="75470-192">String</span></span>|<span data-ttu-id="75470-193">最低 Windows Phone 版本。</span><span class="sxs-lookup"><span data-stu-id="75470-193">Minimum Windows Phone version.</span></span>|
|<span data-ttu-id="75470-194">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="75470-194">osMaximumVersion</span></span>|<span data-ttu-id="75470-195">String</span><span class="sxs-lookup"><span data-stu-id="75470-195">String</span></span>|<span data-ttu-id="75470-196">最高 Windows Phone 版本。</span><span class="sxs-lookup"><span data-stu-id="75470-196">Maximum Windows Phone version.</span></span>|
|<span data-ttu-id="75470-197">earlyLaunchAntiMalwareDriverEnabled</span><span class="sxs-lookup"><span data-stu-id="75470-197">earlyLaunchAntiMalwareDriverEnabled</span></span>|<span data-ttu-id="75470-198">Boolean</span><span class="sxs-lookup"><span data-stu-id="75470-198">Boolean</span></span>|<span data-ttu-id="75470-199">要求设备由 Windows 设备运行状况证明报告为正常 - 提前启动反恶意驱动程序已启用。</span><span class="sxs-lookup"><span data-stu-id="75470-199">Require devices to be reported as healthy by Windows Device Health Attestation - early launch antimalware driver is enabled.</span></span>|
|<span data-ttu-id="75470-200">bitLockerEnabled</span><span class="sxs-lookup"><span data-stu-id="75470-200">bitLockerEnabled</span></span>|<span data-ttu-id="75470-201">Boolean</span><span class="sxs-lookup"><span data-stu-id="75470-201">Boolean</span></span>|<span data-ttu-id="75470-202">要求设备由 Windows 设备运行状况证明报告为正常 - bit locker 已启用。</span><span class="sxs-lookup"><span data-stu-id="75470-202">Require devices to be reported healthy by Windows Device Health Attestation - bit locker is enabled</span></span>|
|<span data-ttu-id="75470-203">secureBootEnabled</span><span class="sxs-lookup"><span data-stu-id="75470-203">secureBootEnabled</span></span>|<span data-ttu-id="75470-204">Boolean</span><span class="sxs-lookup"><span data-stu-id="75470-204">Boolean</span></span>|<span data-ttu-id="75470-205">要求设备由 Windows 设备运行状况证明报告为正常 - 安全启动已启用。</span><span class="sxs-lookup"><span data-stu-id="75470-205">Require devices to be reported as healthy by Windows Device Health Attestation - secure boot is enabled.</span></span>|
|<span data-ttu-id="75470-206">codeIntegrityEnabled</span><span class="sxs-lookup"><span data-stu-id="75470-206">codeIntegrityEnabled</span></span>|<span data-ttu-id="75470-207">Boolean</span><span class="sxs-lookup"><span data-stu-id="75470-207">Boolean</span></span>|<span data-ttu-id="75470-208">要求设备由 Windows 设备运行状况证明报告为正常。</span><span class="sxs-lookup"><span data-stu-id="75470-208">Require devices to be reported as healthy by Windows Device Health Attestation.</span></span>|
|<span data-ttu-id="75470-209">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="75470-209">storageRequireEncryption</span></span>|<span data-ttu-id="75470-210">Boolean</span><span class="sxs-lookup"><span data-stu-id="75470-210">Boolean</span></span>|<span data-ttu-id="75470-211">要求对 Windows 设备加密。</span><span class="sxs-lookup"><span data-stu-id="75470-211">Require encryption on windows devices.</span></span>|
|<span data-ttu-id="75470-212">activeFirewallRequired</span><span class="sxs-lookup"><span data-stu-id="75470-212">activeFirewallRequired</span></span>|<span data-ttu-id="75470-213">布尔</span><span class="sxs-lookup"><span data-stu-id="75470-213">Boolean</span></span>|<span data-ttu-id="75470-214">要求在 Windows 设备上的活动防火墙。</span><span class="sxs-lookup"><span data-stu-id="75470-214">Require active firewall on Windows devices.</span></span>|
|<span data-ttu-id="75470-215">validOperatingSystemBuildRanges</span><span class="sxs-lookup"><span data-stu-id="75470-215">validOperatingSystemBuildRanges</span></span>|<span data-ttu-id="75470-216">[operatingSystemVersionRange](../resources/intune-deviceconfig-operatingsystemversionrange.md)集合</span><span class="sxs-lookup"><span data-stu-id="75470-216">[operatingSystemVersionRange](../resources/intune-deviceconfig-operatingsystemversionrange.md) collection</span></span>|<span data-ttu-id="75470-217">有效的操作系统构建 Windows 设备上的区域。</span><span class="sxs-lookup"><span data-stu-id="75470-217">The valid operating system build ranges on Windows devices.</span></span> <span data-ttu-id="75470-218">该集合最多可包含 10000 个元素。</span><span class="sxs-lookup"><span data-stu-id="75470-218">This collection can contain a maximum of 10000 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="75470-219">响应</span><span class="sxs-lookup"><span data-stu-id="75470-219">Response</span></span>
<span data-ttu-id="75470-220">如果成功，此方法将在响应正文中返回 `201 Created` 响应代码和 [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="75470-220">If successful, this method returns a `201 Created` response code and a [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="75470-221">示例</span><span class="sxs-lookup"><span data-stu-id="75470-221">Example</span></span>
### <a name="request"></a><span data-ttu-id="75470-222">请求</span><span class="sxs-lookup"><span data-stu-id="75470-222">Request</span></span>
<span data-ttu-id="75470-223">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="75470-223">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies
Content-type: application/json
Content-length: 1222

{
  "@odata.type": "#microsoft.graph.windows10MobileCompliancePolicy",
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

### <a name="response"></a><span data-ttu-id="75470-224">响应</span><span class="sxs-lookup"><span data-stu-id="75470-224">Response</span></span>
<span data-ttu-id="75470-p114">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="75470-p114">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





