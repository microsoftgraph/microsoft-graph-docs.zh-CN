---
title: 创建 windows10MobileCompliancePolicy
description: 创建新的 windows10MobileCompliancePolicy 对象。
author: tfitzmac
ms.openlocfilehash: 2d0c7c4a4f27ad723f8d29a24fc20d1fddd2633f
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27324281"
---
# <a name="create-windows10mobilecompliancepolicy"></a><span data-ttu-id="49e02-103">创建 windows10MobileCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="49e02-103">Create windows10MobileCompliancePolicy</span></span>

> <span data-ttu-id="49e02-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="49e02-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="49e02-105">创建新的 [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="49e02-105">Create a new [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="49e02-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="49e02-106">Prerequisites</span></span>
<span data-ttu-id="49e02-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="49e02-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="49e02-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="49e02-109">Permission type</span></span>|<span data-ttu-id="49e02-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="49e02-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="49e02-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="49e02-111">Delegated (work or school account)</span></span>|<span data-ttu-id="49e02-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="49e02-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="49e02-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="49e02-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="49e02-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="49e02-114">Not supported.</span></span>|
|<span data-ttu-id="49e02-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="49e02-115">Application</span></span>|<span data-ttu-id="49e02-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="49e02-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="49e02-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="49e02-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="49e02-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="49e02-118">Request headers</span></span>
|<span data-ttu-id="49e02-119">标头</span><span class="sxs-lookup"><span data-stu-id="49e02-119">Header</span></span>|<span data-ttu-id="49e02-120">值</span><span class="sxs-lookup"><span data-stu-id="49e02-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="49e02-121">授权</span><span class="sxs-lookup"><span data-stu-id="49e02-121">Authorization</span></span>|<span data-ttu-id="49e02-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="49e02-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="49e02-123">Accept</span><span class="sxs-lookup"><span data-stu-id="49e02-123">Accept</span></span>|<span data-ttu-id="49e02-124">application/json</span><span class="sxs-lookup"><span data-stu-id="49e02-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="49e02-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="49e02-125">Request body</span></span>
<span data-ttu-id="49e02-126">在请求正文中，提供 windows10MobileCompliancePolicy 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="49e02-126">In the request body, supply a JSON representation for the windows10MobileCompliancePolicy object.</span></span>

<span data-ttu-id="49e02-127">下表显示了创建 windows10MobileCompliancePolicy 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="49e02-127">The following table shows the properties that are required when you create the windows10MobileCompliancePolicy.</span></span>

|<span data-ttu-id="49e02-128">属性</span><span class="sxs-lookup"><span data-stu-id="49e02-128">Property</span></span>|<span data-ttu-id="49e02-129">类型</span><span class="sxs-lookup"><span data-stu-id="49e02-129">Type</span></span>|<span data-ttu-id="49e02-130">说明</span><span class="sxs-lookup"><span data-stu-id="49e02-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="49e02-131">id</span><span class="sxs-lookup"><span data-stu-id="49e02-131">id</span></span>|<span data-ttu-id="49e02-132">String</span><span class="sxs-lookup"><span data-stu-id="49e02-132">String</span></span>|<span data-ttu-id="49e02-133">实体的键。</span><span class="sxs-lookup"><span data-stu-id="49e02-133">Key of the entity.</span></span> <span data-ttu-id="49e02-134">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="49e02-134">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="49e02-135">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="49e02-135">createdDateTime</span></span>|<span data-ttu-id="49e02-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="49e02-136">DateTimeOffset</span></span>|<span data-ttu-id="49e02-137">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="49e02-137">DateTime the object was created.</span></span> <span data-ttu-id="49e02-138">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="49e02-138">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="49e02-139">description</span><span class="sxs-lookup"><span data-stu-id="49e02-139">description</span></span>|<span data-ttu-id="49e02-140">String</span><span class="sxs-lookup"><span data-stu-id="49e02-140">String</span></span>|<span data-ttu-id="49e02-141">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="49e02-141">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="49e02-142">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="49e02-142">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="49e02-143">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="49e02-143">lastModifiedDateTime</span></span>|<span data-ttu-id="49e02-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="49e02-144">DateTimeOffset</span></span>|<span data-ttu-id="49e02-145">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="49e02-145">DateTime the object was last modified.</span></span> <span data-ttu-id="49e02-146">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="49e02-146">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="49e02-147">displayName</span><span class="sxs-lookup"><span data-stu-id="49e02-147">displayName</span></span>|<span data-ttu-id="49e02-148">String</span><span class="sxs-lookup"><span data-stu-id="49e02-148">String</span></span>|<span data-ttu-id="49e02-149">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="49e02-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="49e02-150">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="49e02-150">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="49e02-151">version</span><span class="sxs-lookup"><span data-stu-id="49e02-151">version</span></span>|<span data-ttu-id="49e02-152">Int32</span><span class="sxs-lookup"><span data-stu-id="49e02-152">Int32</span></span>|<span data-ttu-id="49e02-153">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="49e02-153">Version of the device configuration.</span></span> <span data-ttu-id="49e02-154">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="49e02-154">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="49e02-155">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="49e02-155">passwordRequired</span></span>|<span data-ttu-id="49e02-156">Boolean</span><span class="sxs-lookup"><span data-stu-id="49e02-156">Boolean</span></span>|<span data-ttu-id="49e02-157">需要密码才可解锁 Windows Phone 设备。</span><span class="sxs-lookup"><span data-stu-id="49e02-157">Require a password to unlock Windows Phone device.</span></span>|
|<span data-ttu-id="49e02-158">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="49e02-158">passwordBlockSimple</span></span>|<span data-ttu-id="49e02-159">Boolean</span><span class="sxs-lookup"><span data-stu-id="49e02-159">Boolean</span></span>|<span data-ttu-id="49e02-160">是否阻止同步日历。</span><span class="sxs-lookup"><span data-stu-id="49e02-160">Whether or not to block syncing the calendar.</span></span>|
|<span data-ttu-id="49e02-161">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="49e02-161">passwordMinimumLength</span></span>|<span data-ttu-id="49e02-162">Int32</span><span class="sxs-lookup"><span data-stu-id="49e02-162">Int32</span></span>|<span data-ttu-id="49e02-163">最短密码长度。</span><span class="sxs-lookup"><span data-stu-id="49e02-163">Minimum password length.</span></span> <span data-ttu-id="49e02-164">有效值为 4 至 16</span><span class="sxs-lookup"><span data-stu-id="49e02-164">Valid values 4 to 16</span></span>|
|<span data-ttu-id="49e02-165">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="49e02-165">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="49e02-166">Int32</span><span class="sxs-lookup"><span data-stu-id="49e02-166">Int32</span></span>|<span data-ttu-id="49e02-167">密码中必需的字符集数。</span><span class="sxs-lookup"><span data-stu-id="49e02-167">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="49e02-168">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="49e02-168">passwordRequiredType</span></span>|[<span data-ttu-id="49e02-169">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="49e02-169">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="49e02-170">必需的密码类型。</span><span class="sxs-lookup"><span data-stu-id="49e02-170">The required password type.</span></span> <span data-ttu-id="49e02-171">可取值为：`deviceDefault`、`alphanumeric`、`numeric`。</span><span class="sxs-lookup"><span data-stu-id="49e02-171">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="49e02-172">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="49e02-172">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="49e02-173">Int32</span><span class="sxs-lookup"><span data-stu-id="49e02-173">Int32</span></span>|<span data-ttu-id="49e02-174">防止重复使用的先前密码的数量。</span><span class="sxs-lookup"><span data-stu-id="49e02-174">The number of previous passwords to prevent re-use of.</span></span>|
|<span data-ttu-id="49e02-175">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="49e02-175">passwordExpirationDays</span></span>|<span data-ttu-id="49e02-176">Int32</span><span class="sxs-lookup"><span data-stu-id="49e02-176">Int32</span></span>|<span data-ttu-id="49e02-177">密码过期前的天数。</span><span class="sxs-lookup"><span data-stu-id="49e02-177">Number of days before password expiration.</span></span> <span data-ttu-id="49e02-178">有效值为 1 至 255</span><span class="sxs-lookup"><span data-stu-id="49e02-178">Valid values 1 to 255</span></span>|
|<span data-ttu-id="49e02-179">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="49e02-179">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="49e02-180">Int32</span><span class="sxs-lookup"><span data-stu-id="49e02-180">Int32</span></span>|<span data-ttu-id="49e02-181">在需要密码之前不活动的分钟数。</span><span class="sxs-lookup"><span data-stu-id="49e02-181">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="49e02-182">passwordRequireToUnlockFromIdle</span><span class="sxs-lookup"><span data-stu-id="49e02-182">passwordRequireToUnlockFromIdle</span></span>|<span data-ttu-id="49e02-183">Boolean</span><span class="sxs-lookup"><span data-stu-id="49e02-183">Boolean</span></span>|<span data-ttu-id="49e02-184">需要密码才可解锁空闲设备。</span><span class="sxs-lookup"><span data-stu-id="49e02-184">Require a password to unlock an idle device.</span></span>|
|<span data-ttu-id="49e02-185">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="49e02-185">osMinimumVersion</span></span>|<span data-ttu-id="49e02-186">String</span><span class="sxs-lookup"><span data-stu-id="49e02-186">String</span></span>|<span data-ttu-id="49e02-187">最低 Windows Phone 版本。</span><span class="sxs-lookup"><span data-stu-id="49e02-187">Minimum Windows Phone version.</span></span>|
|<span data-ttu-id="49e02-188">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="49e02-188">osMaximumVersion</span></span>|<span data-ttu-id="49e02-189">String</span><span class="sxs-lookup"><span data-stu-id="49e02-189">String</span></span>|<span data-ttu-id="49e02-190">最高 Windows Phone 版本。</span><span class="sxs-lookup"><span data-stu-id="49e02-190">Maximum Windows Phone version.</span></span>|
|<span data-ttu-id="49e02-191">earlyLaunchAntiMalwareDriverEnabled</span><span class="sxs-lookup"><span data-stu-id="49e02-191">earlyLaunchAntiMalwareDriverEnabled</span></span>|<span data-ttu-id="49e02-192">Boolean</span><span class="sxs-lookup"><span data-stu-id="49e02-192">Boolean</span></span>|<span data-ttu-id="49e02-193">要求设备由 Windows 设备运行状况证明报告为正常 - 提前启动反恶意驱动程序已启用。</span><span class="sxs-lookup"><span data-stu-id="49e02-193">Require devices to be reported as healthy by Windows Device Health Attestation - early launch antimalware driver is enabled.</span></span>|
|<span data-ttu-id="49e02-194">bitLockerEnabled</span><span class="sxs-lookup"><span data-stu-id="49e02-194">bitLockerEnabled</span></span>|<span data-ttu-id="49e02-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="49e02-195">Boolean</span></span>|<span data-ttu-id="49e02-196">要求设备由 Windows 设备运行状况证明报告为正常 - bit locker 已启用。</span><span class="sxs-lookup"><span data-stu-id="49e02-196">Require devices to be reported healthy by Windows Device Health Attestation - bit locker is enabled</span></span>|
|<span data-ttu-id="49e02-197">secureBootEnabled</span><span class="sxs-lookup"><span data-stu-id="49e02-197">secureBootEnabled</span></span>|<span data-ttu-id="49e02-198">Boolean</span><span class="sxs-lookup"><span data-stu-id="49e02-198">Boolean</span></span>|<span data-ttu-id="49e02-199">要求设备由 Windows 设备运行状况证明报告为正常 - 安全启动已启用。</span><span class="sxs-lookup"><span data-stu-id="49e02-199">Require devices to be reported as healthy by Windows Device Health Attestation - secure boot is enabled.</span></span>|
|<span data-ttu-id="49e02-200">codeIntegrityEnabled</span><span class="sxs-lookup"><span data-stu-id="49e02-200">codeIntegrityEnabled</span></span>|<span data-ttu-id="49e02-201">Boolean</span><span class="sxs-lookup"><span data-stu-id="49e02-201">Boolean</span></span>|<span data-ttu-id="49e02-202">要求设备由 Windows 设备运行状况证明报告为正常。</span><span class="sxs-lookup"><span data-stu-id="49e02-202">Require devices to be reported as healthy by Windows Device Health Attestation.</span></span>|
|<span data-ttu-id="49e02-203">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="49e02-203">storageRequireEncryption</span></span>|<span data-ttu-id="49e02-204">Boolean</span><span class="sxs-lookup"><span data-stu-id="49e02-204">Boolean</span></span>|<span data-ttu-id="49e02-205">要求对 Windows 设备加密。</span><span class="sxs-lookup"><span data-stu-id="49e02-205">Require encryption on windows devices.</span></span>|



## <a name="response"></a><span data-ttu-id="49e02-206">响应</span><span class="sxs-lookup"><span data-stu-id="49e02-206">Response</span></span>
<span data-ttu-id="49e02-207">如果成功，此方法将在响应正文中返回 `201 Created` 响应代码和 [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="49e02-207">If successful, this method returns a `201 Created` response code and a [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="49e02-208">示例</span><span class="sxs-lookup"><span data-stu-id="49e02-208">Example</span></span>
### <a name="request"></a><span data-ttu-id="49e02-209">请求</span><span class="sxs-lookup"><span data-stu-id="49e02-209">Request</span></span>
<span data-ttu-id="49e02-210">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="49e02-210">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies
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

### <a name="response"></a><span data-ttu-id="49e02-211">响应</span><span class="sxs-lookup"><span data-stu-id="49e02-211">Response</span></span>
<span data-ttu-id="49e02-p111">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="49e02-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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



