---
title: 更新 windows10CompliancePolicy
description: 更新 windows10CompliancePolicy 对象的属性。
ms.openlocfilehash: ab2d9c76f46ed00f5a0ae20620d8562a9439ad23
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27009722"
---
# <a name="update-windows10compliancepolicy"></a><span data-ttu-id="04f46-103">更新 windows10CompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="04f46-103">Update windows10CompliancePolicy</span></span>

> <span data-ttu-id="04f46-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="04f46-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="04f46-105">更新 [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="04f46-105">Update the properties of a [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="04f46-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="04f46-106">Prerequisites</span></span>
<span data-ttu-id="04f46-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="04f46-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="04f46-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="04f46-109">Permission type</span></span>|<span data-ttu-id="04f46-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="04f46-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="04f46-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="04f46-111">Delegated (work or school account)</span></span>|<span data-ttu-id="04f46-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="04f46-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="04f46-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="04f46-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="04f46-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="04f46-114">Not supported.</span></span>|
|<span data-ttu-id="04f46-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="04f46-115">Application</span></span>|<span data-ttu-id="04f46-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="04f46-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="04f46-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="04f46-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="04f46-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="04f46-118">Request headers</span></span>
|<span data-ttu-id="04f46-119">标头</span><span class="sxs-lookup"><span data-stu-id="04f46-119">Header</span></span>|<span data-ttu-id="04f46-120">值</span><span class="sxs-lookup"><span data-stu-id="04f46-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="04f46-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="04f46-121">Authorization</span></span>|<span data-ttu-id="04f46-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="04f46-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="04f46-123">Accept</span><span class="sxs-lookup"><span data-stu-id="04f46-123">Accept</span></span>|<span data-ttu-id="04f46-124">application/json</span><span class="sxs-lookup"><span data-stu-id="04f46-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="04f46-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="04f46-125">Request body</span></span>
<span data-ttu-id="04f46-126">在请求正文中，提供 [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="04f46-126">In the request body, supply a JSON representation for the [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) object.</span></span>

<span data-ttu-id="04f46-127">下表显示创建 [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="04f46-127">The following table shows the properties that are required when you create the [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md).</span></span>

|<span data-ttu-id="04f46-128">属性</span><span class="sxs-lookup"><span data-stu-id="04f46-128">Property</span></span>|<span data-ttu-id="04f46-129">类型</span><span class="sxs-lookup"><span data-stu-id="04f46-129">Type</span></span>|<span data-ttu-id="04f46-130">说明</span><span class="sxs-lookup"><span data-stu-id="04f46-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="04f46-131">id</span><span class="sxs-lookup"><span data-stu-id="04f46-131">id</span></span>|<span data-ttu-id="04f46-132">String</span><span class="sxs-lookup"><span data-stu-id="04f46-132">String</span></span>|<span data-ttu-id="04f46-133">实体的键。</span><span class="sxs-lookup"><span data-stu-id="04f46-133">Key of the entity.</span></span> <span data-ttu-id="04f46-134">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="04f46-134">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="04f46-135">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="04f46-135">createdDateTime</span></span>|<span data-ttu-id="04f46-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="04f46-136">DateTimeOffset</span></span>|<span data-ttu-id="04f46-137">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="04f46-137">DateTime the object was created.</span></span> <span data-ttu-id="04f46-138">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="04f46-138">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="04f46-139">description</span><span class="sxs-lookup"><span data-stu-id="04f46-139">description</span></span>|<span data-ttu-id="04f46-140">String</span><span class="sxs-lookup"><span data-stu-id="04f46-140">String</span></span>|<span data-ttu-id="04f46-141">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="04f46-141">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="04f46-142">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="04f46-142">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="04f46-143">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="04f46-143">lastModifiedDateTime</span></span>|<span data-ttu-id="04f46-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="04f46-144">DateTimeOffset</span></span>|<span data-ttu-id="04f46-145">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="04f46-145">DateTime the object was last modified.</span></span> <span data-ttu-id="04f46-146">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="04f46-146">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="04f46-147">displayName</span><span class="sxs-lookup"><span data-stu-id="04f46-147">displayName</span></span>|<span data-ttu-id="04f46-148">String</span><span class="sxs-lookup"><span data-stu-id="04f46-148">String</span></span>|<span data-ttu-id="04f46-149">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="04f46-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="04f46-150">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="04f46-150">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="04f46-151">version</span><span class="sxs-lookup"><span data-stu-id="04f46-151">version</span></span>|<span data-ttu-id="04f46-152">Int32</span><span class="sxs-lookup"><span data-stu-id="04f46-152">Int32</span></span>|<span data-ttu-id="04f46-153">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="04f46-153">Version of the device configuration.</span></span> <span data-ttu-id="04f46-154">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="04f46-154">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="04f46-155">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="04f46-155">passwordRequired</span></span>|<span data-ttu-id="04f46-156">Boolean</span><span class="sxs-lookup"><span data-stu-id="04f46-156">Boolean</span></span>|<span data-ttu-id="04f46-157">需要密码才可解锁 Windows 设备。</span><span class="sxs-lookup"><span data-stu-id="04f46-157">Require a password to unlock Windows device.</span></span>|
|<span data-ttu-id="04f46-158">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="04f46-158">passwordBlockSimple</span></span>|<span data-ttu-id="04f46-159">Boolean</span><span class="sxs-lookup"><span data-stu-id="04f46-159">Boolean</span></span>|<span data-ttu-id="04f46-160">指示是否阻止简单密码。</span><span class="sxs-lookup"><span data-stu-id="04f46-160">Indicates whether or not to block simple password.</span></span>|
|<span data-ttu-id="04f46-161">passwordRequiredToUnlockFromIdle</span><span class="sxs-lookup"><span data-stu-id="04f46-161">passwordRequiredToUnlockFromIdle</span></span>|<span data-ttu-id="04f46-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="04f46-162">Boolean</span></span>|<span data-ttu-id="04f46-163">需要密码才可解锁空闲设备。</span><span class="sxs-lookup"><span data-stu-id="04f46-163">Require a password to unlock an idle device.</span></span>|
|<span data-ttu-id="04f46-164">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="04f46-164">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="04f46-165">Int32</span><span class="sxs-lookup"><span data-stu-id="04f46-165">Int32</span></span>|<span data-ttu-id="04f46-166">在需要密码之前不活动的分钟数。</span><span class="sxs-lookup"><span data-stu-id="04f46-166">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="04f46-167">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="04f46-167">passwordExpirationDays</span></span>|<span data-ttu-id="04f46-168">Int32</span><span class="sxs-lookup"><span data-stu-id="04f46-168">Int32</span></span>|<span data-ttu-id="04f46-169">密码过期天数。</span><span class="sxs-lookup"><span data-stu-id="04f46-169">The password expiration in days.</span></span>|
|<span data-ttu-id="04f46-170">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="04f46-170">passwordMinimumLength</span></span>|<span data-ttu-id="04f46-171">Int32</span><span class="sxs-lookup"><span data-stu-id="04f46-171">Int32</span></span>|<span data-ttu-id="04f46-172">密码最短长度。</span><span class="sxs-lookup"><span data-stu-id="04f46-172">The minimum password length.</span></span>|
|<span data-ttu-id="04f46-173">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="04f46-173">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="04f46-174">Int32</span><span class="sxs-lookup"><span data-stu-id="04f46-174">Int32</span></span>|<span data-ttu-id="04f46-175">密码中必需的字符集数。</span><span class="sxs-lookup"><span data-stu-id="04f46-175">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="04f46-176">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="04f46-176">passwordRequiredType</span></span>|[<span data-ttu-id="04f46-177">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="04f46-177">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="04f46-178">必需的密码类型。</span><span class="sxs-lookup"><span data-stu-id="04f46-178">The required password type.</span></span> <span data-ttu-id="04f46-179">可取值为：`deviceDefault`、`alphanumeric`、`numeric`。</span><span class="sxs-lookup"><span data-stu-id="04f46-179">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="04f46-180">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="04f46-180">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="04f46-181">Int32</span><span class="sxs-lookup"><span data-stu-id="04f46-181">Int32</span></span>|<span data-ttu-id="04f46-182">防止重复使用的先前密码的数量。</span><span class="sxs-lookup"><span data-stu-id="04f46-182">The number of previous passwords to prevent re-use of.</span></span>|
|<span data-ttu-id="04f46-183">requireHealthyDeviceReport</span><span class="sxs-lookup"><span data-stu-id="04f46-183">requireHealthyDeviceReport</span></span>|<span data-ttu-id="04f46-184">Boolean</span><span class="sxs-lookup"><span data-stu-id="04f46-184">Boolean</span></span>|<span data-ttu-id="04f46-185">要求设备由 Windows 设备运行状况证明报告为正常。</span><span class="sxs-lookup"><span data-stu-id="04f46-185">Require devices to be reported as healthy by Windows Device Health Attestation.</span></span>|
|<span data-ttu-id="04f46-186">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="04f46-186">osMinimumVersion</span></span>|<span data-ttu-id="04f46-187">String</span><span class="sxs-lookup"><span data-stu-id="04f46-187">String</span></span>|<span data-ttu-id="04f46-188">最低 Windows 10 版本。</span><span class="sxs-lookup"><span data-stu-id="04f46-188">Minimum Windows 10 version.</span></span>|
|<span data-ttu-id="04f46-189">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="04f46-189">osMaximumVersion</span></span>|<span data-ttu-id="04f46-190">String</span><span class="sxs-lookup"><span data-stu-id="04f46-190">String</span></span>|<span data-ttu-id="04f46-191">最高 Windows 10 版本。</span><span class="sxs-lookup"><span data-stu-id="04f46-191">Maximum Windows 10 version.</span></span>|
|<span data-ttu-id="04f46-192">mobileOsMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="04f46-192">mobileOsMinimumVersion</span></span>|<span data-ttu-id="04f46-193">String</span><span class="sxs-lookup"><span data-stu-id="04f46-193">String</span></span>|<span data-ttu-id="04f46-194">最低 Windows Phone 版本。</span><span class="sxs-lookup"><span data-stu-id="04f46-194">Minimum Windows Phone version.</span></span>|
|<span data-ttu-id="04f46-195">mobileOsMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="04f46-195">mobileOsMaximumVersion</span></span>|<span data-ttu-id="04f46-196">String</span><span class="sxs-lookup"><span data-stu-id="04f46-196">String</span></span>|<span data-ttu-id="04f46-197">最高 Windows Phone 版本。</span><span class="sxs-lookup"><span data-stu-id="04f46-197">Maximum Windows Phone version.</span></span>|
|<span data-ttu-id="04f46-198">earlyLaunchAntiMalwareDriverEnabled</span><span class="sxs-lookup"><span data-stu-id="04f46-198">earlyLaunchAntiMalwareDriverEnabled</span></span>|<span data-ttu-id="04f46-199">Boolean</span><span class="sxs-lookup"><span data-stu-id="04f46-199">Boolean</span></span>|<span data-ttu-id="04f46-200">要求设备由 Windows 设备运行状况证明报告为正常 - 提前启动反恶意驱动程序已启用。</span><span class="sxs-lookup"><span data-stu-id="04f46-200">Require devices to be reported as healthy by Windows Device Health Attestation - early launch antimalware driver is enabled.</span></span>|
|<span data-ttu-id="04f46-201">bitLockerEnabled</span><span class="sxs-lookup"><span data-stu-id="04f46-201">bitLockerEnabled</span></span>|<span data-ttu-id="04f46-202">Boolean</span><span class="sxs-lookup"><span data-stu-id="04f46-202">Boolean</span></span>|<span data-ttu-id="04f46-203">要求设备由 Windows 设备运行状况证明报告为正常 - bit locker 已启用。</span><span class="sxs-lookup"><span data-stu-id="04f46-203">Require devices to be reported healthy by Windows Device Health Attestation - bit locker is enabled</span></span>|
|<span data-ttu-id="04f46-204">secureBootEnabled</span><span class="sxs-lookup"><span data-stu-id="04f46-204">secureBootEnabled</span></span>|<span data-ttu-id="04f46-205">Boolean</span><span class="sxs-lookup"><span data-stu-id="04f46-205">Boolean</span></span>|<span data-ttu-id="04f46-206">要求设备由 Windows 设备运行状况证明报告为正常 - 安全启动已启用。</span><span class="sxs-lookup"><span data-stu-id="04f46-206">Require devices to be reported as healthy by Windows Device Health Attestation - secure boot is enabled.</span></span>|
|<span data-ttu-id="04f46-207">codeIntegrityEnabled</span><span class="sxs-lookup"><span data-stu-id="04f46-207">codeIntegrityEnabled</span></span>|<span data-ttu-id="04f46-208">Boolean</span><span class="sxs-lookup"><span data-stu-id="04f46-208">Boolean</span></span>|<span data-ttu-id="04f46-209">要求设备由 Windows 设备运行状况证明报告为正常。</span><span class="sxs-lookup"><span data-stu-id="04f46-209">Require devices to be reported as healthy by Windows Device Health Attestation.</span></span>|
|<span data-ttu-id="04f46-210">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="04f46-210">storageRequireEncryption</span></span>|<span data-ttu-id="04f46-211">Boolean</span><span class="sxs-lookup"><span data-stu-id="04f46-211">Boolean</span></span>|<span data-ttu-id="04f46-212">要求对 Windows 设备加密。</span><span class="sxs-lookup"><span data-stu-id="04f46-212">Require encryption on windows devices.</span></span>|



## <a name="response"></a><span data-ttu-id="04f46-213">响应</span><span class="sxs-lookup"><span data-stu-id="04f46-213">Response</span></span>
<span data-ttu-id="04f46-214">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和更新的 [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="04f46-214">If successful, this method returns a `200 OK` response code and an updated [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="04f46-215">示例</span><span class="sxs-lookup"><span data-stu-id="04f46-215">Example</span></span>
### <a name="request"></a><span data-ttu-id="04f46-216">请求</span><span class="sxs-lookup"><span data-stu-id="04f46-216">Request</span></span>
<span data-ttu-id="04f46-217">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="04f46-217">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
Content-type: application/json
Content-length: 954

{
  "@odata.type": "#microsoft.graph.windows10CompliancePolicy",
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
  "storageRequireEncryption": true
}
```

### <a name="response"></a><span data-ttu-id="04f46-218">响应</span><span class="sxs-lookup"><span data-stu-id="04f46-218">Response</span></span>
<span data-ttu-id="04f46-p109">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="04f46-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1126

{
  "@odata.type": "#microsoft.graph.windows10CompliancePolicy",
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
  "storageRequireEncryption": true
}
```



