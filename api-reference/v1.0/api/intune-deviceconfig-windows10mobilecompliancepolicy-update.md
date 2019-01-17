---
title: 更新 windows10MobileCompliancePolicy
description: 更新 windows10MobileCompliancePolicy 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 1b036b4c73800e647e6617413fc330f4c6d40dea
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27966823"
---
# <a name="update-windows10mobilecompliancepolicy"></a><span data-ttu-id="af963-103">更新 windows10MobileCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="af963-103">Update windows10MobileCompliancePolicy</span></span>

> <span data-ttu-id="af963-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="af963-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="af963-105">更新 [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="af963-105">Update the properties of a [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="af963-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="af963-106">Prerequisites</span></span>
<span data-ttu-id="af963-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="af963-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="af963-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="af963-109">Permission type</span></span>|<span data-ttu-id="af963-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="af963-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="af963-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="af963-111">Delegated (work or school account)</span></span>|<span data-ttu-id="af963-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="af963-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="af963-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="af963-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="af963-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="af963-114">Not supported.</span></span>|
|<span data-ttu-id="af963-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="af963-115">Application</span></span>|<span data-ttu-id="af963-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="af963-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="af963-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="af963-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="af963-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="af963-118">Request headers</span></span>
|<span data-ttu-id="af963-119">标头</span><span class="sxs-lookup"><span data-stu-id="af963-119">Header</span></span>|<span data-ttu-id="af963-120">值</span><span class="sxs-lookup"><span data-stu-id="af963-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="af963-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="af963-121">Authorization</span></span>|<span data-ttu-id="af963-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="af963-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="af963-123">Accept</span><span class="sxs-lookup"><span data-stu-id="af963-123">Accept</span></span>|<span data-ttu-id="af963-124">application/json</span><span class="sxs-lookup"><span data-stu-id="af963-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="af963-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="af963-125">Request body</span></span>
<span data-ttu-id="af963-126">在请求正文中，提供 [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="af963-126">In the request body, supply a JSON representation for the [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md) object.</span></span>

<span data-ttu-id="af963-127">下表显示了创建 [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="af963-127">The following table shows the properties that are required when you create the [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md).</span></span>

|<span data-ttu-id="af963-128">属性</span><span class="sxs-lookup"><span data-stu-id="af963-128">Property</span></span>|<span data-ttu-id="af963-129">类型</span><span class="sxs-lookup"><span data-stu-id="af963-129">Type</span></span>|<span data-ttu-id="af963-130">说明</span><span class="sxs-lookup"><span data-stu-id="af963-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="af963-131">id</span><span class="sxs-lookup"><span data-stu-id="af963-131">id</span></span>|<span data-ttu-id="af963-132">String</span><span class="sxs-lookup"><span data-stu-id="af963-132">String</span></span>|<span data-ttu-id="af963-133">实体的键。</span><span class="sxs-lookup"><span data-stu-id="af963-133">Key of the entity.</span></span> <span data-ttu-id="af963-134">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="af963-134">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="af963-135">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="af963-135">createdDateTime</span></span>|<span data-ttu-id="af963-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="af963-136">DateTimeOffset</span></span>|<span data-ttu-id="af963-137">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="af963-137">DateTime the object was created.</span></span> <span data-ttu-id="af963-138">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="af963-138">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="af963-139">description</span><span class="sxs-lookup"><span data-stu-id="af963-139">description</span></span>|<span data-ttu-id="af963-140">String</span><span class="sxs-lookup"><span data-stu-id="af963-140">String</span></span>|<span data-ttu-id="af963-141">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="af963-141">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="af963-142">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="af963-142">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="af963-143">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="af963-143">lastModifiedDateTime</span></span>|<span data-ttu-id="af963-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="af963-144">DateTimeOffset</span></span>|<span data-ttu-id="af963-145">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="af963-145">DateTime the object was last modified.</span></span> <span data-ttu-id="af963-146">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="af963-146">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="af963-147">displayName</span><span class="sxs-lookup"><span data-stu-id="af963-147">displayName</span></span>|<span data-ttu-id="af963-148">String</span><span class="sxs-lookup"><span data-stu-id="af963-148">String</span></span>|<span data-ttu-id="af963-149">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="af963-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="af963-150">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="af963-150">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="af963-151">version</span><span class="sxs-lookup"><span data-stu-id="af963-151">version</span></span>|<span data-ttu-id="af963-152">Int32</span><span class="sxs-lookup"><span data-stu-id="af963-152">Int32</span></span>|<span data-ttu-id="af963-153">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="af963-153">Version of the device configuration.</span></span> <span data-ttu-id="af963-154">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="af963-154">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="af963-155">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="af963-155">passwordRequired</span></span>|<span data-ttu-id="af963-156">Boolean</span><span class="sxs-lookup"><span data-stu-id="af963-156">Boolean</span></span>|<span data-ttu-id="af963-157">需要密码才可解锁 Windows Phone 设备。</span><span class="sxs-lookup"><span data-stu-id="af963-157">Require a password to unlock Windows Phone device.</span></span>|
|<span data-ttu-id="af963-158">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="af963-158">passwordBlockSimple</span></span>|<span data-ttu-id="af963-159">Boolean</span><span class="sxs-lookup"><span data-stu-id="af963-159">Boolean</span></span>|<span data-ttu-id="af963-160">是否阻止同步日历。</span><span class="sxs-lookup"><span data-stu-id="af963-160">Whether or not to block syncing the calendar.</span></span>|
|<span data-ttu-id="af963-161">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="af963-161">passwordMinimumLength</span></span>|<span data-ttu-id="af963-162">Int32</span><span class="sxs-lookup"><span data-stu-id="af963-162">Int32</span></span>|<span data-ttu-id="af963-163">最短密码长度。</span><span class="sxs-lookup"><span data-stu-id="af963-163">Minimum password length.</span></span> <span data-ttu-id="af963-164">有效值为 4 至 16</span><span class="sxs-lookup"><span data-stu-id="af963-164">Valid values 4 to 16</span></span>|
|<span data-ttu-id="af963-165">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="af963-165">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="af963-166">Int32</span><span class="sxs-lookup"><span data-stu-id="af963-166">Int32</span></span>|<span data-ttu-id="af963-167">密码中必需的字符集数。</span><span class="sxs-lookup"><span data-stu-id="af963-167">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="af963-168">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="af963-168">passwordRequiredType</span></span>|[<span data-ttu-id="af963-169">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="af963-169">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="af963-170">必需的密码类型。</span><span class="sxs-lookup"><span data-stu-id="af963-170">The required password type.</span></span> <span data-ttu-id="af963-171">可取值为：`deviceDefault`、`alphanumeric`、`numeric`。</span><span class="sxs-lookup"><span data-stu-id="af963-171">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="af963-172">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="af963-172">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="af963-173">Int32</span><span class="sxs-lookup"><span data-stu-id="af963-173">Int32</span></span>|<span data-ttu-id="af963-174">防止重复使用的先前密码的数量。</span><span class="sxs-lookup"><span data-stu-id="af963-174">The number of previous passwords to prevent re-use of.</span></span>|
|<span data-ttu-id="af963-175">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="af963-175">passwordExpirationDays</span></span>|<span data-ttu-id="af963-176">Int32</span><span class="sxs-lookup"><span data-stu-id="af963-176">Int32</span></span>|<span data-ttu-id="af963-177">密码过期前的天数。</span><span class="sxs-lookup"><span data-stu-id="af963-177">Number of days before password expiration.</span></span> <span data-ttu-id="af963-178">有效值为 1 至 255</span><span class="sxs-lookup"><span data-stu-id="af963-178">Valid values 1 to 255</span></span>|
|<span data-ttu-id="af963-179">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="af963-179">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="af963-180">Int32</span><span class="sxs-lookup"><span data-stu-id="af963-180">Int32</span></span>|<span data-ttu-id="af963-181">在需要密码之前不活动的分钟数。</span><span class="sxs-lookup"><span data-stu-id="af963-181">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="af963-182">passwordRequireToUnlockFromIdle</span><span class="sxs-lookup"><span data-stu-id="af963-182">passwordRequireToUnlockFromIdle</span></span>|<span data-ttu-id="af963-183">Boolean</span><span class="sxs-lookup"><span data-stu-id="af963-183">Boolean</span></span>|<span data-ttu-id="af963-184">需要密码才可解锁空闲设备。</span><span class="sxs-lookup"><span data-stu-id="af963-184">Require a password to unlock an idle device.</span></span>|
|<span data-ttu-id="af963-185">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="af963-185">osMinimumVersion</span></span>|<span data-ttu-id="af963-186">String</span><span class="sxs-lookup"><span data-stu-id="af963-186">String</span></span>|<span data-ttu-id="af963-187">最低 Windows Phone 版本。</span><span class="sxs-lookup"><span data-stu-id="af963-187">Minimum Windows Phone version.</span></span>|
|<span data-ttu-id="af963-188">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="af963-188">osMaximumVersion</span></span>|<span data-ttu-id="af963-189">String</span><span class="sxs-lookup"><span data-stu-id="af963-189">String</span></span>|<span data-ttu-id="af963-190">最高 Windows Phone 版本。</span><span class="sxs-lookup"><span data-stu-id="af963-190">Maximum Windows Phone version.</span></span>|
|<span data-ttu-id="af963-191">earlyLaunchAntiMalwareDriverEnabled</span><span class="sxs-lookup"><span data-stu-id="af963-191">earlyLaunchAntiMalwareDriverEnabled</span></span>|<span data-ttu-id="af963-192">Boolean</span><span class="sxs-lookup"><span data-stu-id="af963-192">Boolean</span></span>|<span data-ttu-id="af963-193">要求设备由 Windows 设备运行状况证明报告为正常 - 提前启动反恶意驱动程序已启用。</span><span class="sxs-lookup"><span data-stu-id="af963-193">Require devices to be reported as healthy by Windows Device Health Attestation - early launch antimalware driver is enabled.</span></span>|
|<span data-ttu-id="af963-194">bitLockerEnabled</span><span class="sxs-lookup"><span data-stu-id="af963-194">bitLockerEnabled</span></span>|<span data-ttu-id="af963-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="af963-195">Boolean</span></span>|<span data-ttu-id="af963-196">要求设备由 Windows 设备运行状况证明报告为正常 - bit locker 已启用。</span><span class="sxs-lookup"><span data-stu-id="af963-196">Require devices to be reported healthy by Windows Device Health Attestation - bit locker is enabled</span></span>|
|<span data-ttu-id="af963-197">secureBootEnabled</span><span class="sxs-lookup"><span data-stu-id="af963-197">secureBootEnabled</span></span>|<span data-ttu-id="af963-198">Boolean</span><span class="sxs-lookup"><span data-stu-id="af963-198">Boolean</span></span>|<span data-ttu-id="af963-199">要求设备由 Windows 设备运行状况证明报告为正常 - 安全启动已启用。</span><span class="sxs-lookup"><span data-stu-id="af963-199">Require devices to be reported as healthy by Windows Device Health Attestation - secure boot is enabled.</span></span>|
|<span data-ttu-id="af963-200">codeIntegrityEnabled</span><span class="sxs-lookup"><span data-stu-id="af963-200">codeIntegrityEnabled</span></span>|<span data-ttu-id="af963-201">Boolean</span><span class="sxs-lookup"><span data-stu-id="af963-201">Boolean</span></span>|<span data-ttu-id="af963-202">要求设备由 Windows 设备运行状况证明报告为正常。</span><span class="sxs-lookup"><span data-stu-id="af963-202">Require devices to be reported as healthy by Windows Device Health Attestation.</span></span>|
|<span data-ttu-id="af963-203">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="af963-203">storageRequireEncryption</span></span>|<span data-ttu-id="af963-204">Boolean</span><span class="sxs-lookup"><span data-stu-id="af963-204">Boolean</span></span>|<span data-ttu-id="af963-205">要求对 Windows 设备加密。</span><span class="sxs-lookup"><span data-stu-id="af963-205">Require encryption on windows devices.</span></span>|



## <a name="response"></a><span data-ttu-id="af963-206">响应</span><span class="sxs-lookup"><span data-stu-id="af963-206">Response</span></span>
<span data-ttu-id="af963-207">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和更新的 [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="af963-207">If successful, this method returns a `200 OK` response code and an updated [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="af963-208">示例</span><span class="sxs-lookup"><span data-stu-id="af963-208">Example</span></span>
### <a name="request"></a><span data-ttu-id="af963-209">请求</span><span class="sxs-lookup"><span data-stu-id="af963-209">Request</span></span>
<span data-ttu-id="af963-210">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="af963-210">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
Content-type: application/json
Content-length: 792

{
  "@odata.type": "#microsoft.graph.windows10MobileCompliancePolicy",
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
  "storageRequireEncryption": true
}
```

### <a name="response"></a><span data-ttu-id="af963-211">响应</span><span class="sxs-lookup"><span data-stu-id="af963-211">Response</span></span>
<span data-ttu-id="af963-p111">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="af963-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 964

{
  "@odata.type": "#microsoft.graph.windows10MobileCompliancePolicy",
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
  "storageRequireEncryption": true
}
```



