---
title: 更新 windows10MobileCompliancePolicy
description: 更新 windows10MobileCompliancePolicy 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0cbfbc758e3457b69a7ae2ef741745531c8a6770
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32541274"
---
# <a name="update-windows10mobilecompliancepolicy"></a><span data-ttu-id="2f784-103">更新 windows10MobileCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="2f784-103">Update windows10MobileCompliancePolicy</span></span>

> <span data-ttu-id="2f784-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="2f784-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2f784-105">更新 [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="2f784-105">Update the properties of a [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2f784-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="2f784-106">Prerequisites</span></span>
<span data-ttu-id="2f784-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2f784-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2f784-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="2f784-109">Permission type</span></span>|<span data-ttu-id="2f784-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="2f784-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2f784-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2f784-111">Delegated (work or school account)</span></span>|<span data-ttu-id="2f784-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2f784-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="2f784-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2f784-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2f784-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="2f784-114">Not supported.</span></span>|
|<span data-ttu-id="2f784-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="2f784-115">Application</span></span>|<span data-ttu-id="2f784-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="2f784-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2f784-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2f784-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="2f784-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="2f784-118">Request headers</span></span>
|<span data-ttu-id="2f784-119">标头</span><span class="sxs-lookup"><span data-stu-id="2f784-119">Header</span></span>|<span data-ttu-id="2f784-120">值</span><span class="sxs-lookup"><span data-stu-id="2f784-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2f784-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="2f784-121">Authorization</span></span>|<span data-ttu-id="2f784-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="2f784-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2f784-123">接受</span><span class="sxs-lookup"><span data-stu-id="2f784-123">Accept</span></span>|<span data-ttu-id="2f784-124">application/json</span><span class="sxs-lookup"><span data-stu-id="2f784-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2f784-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="2f784-125">Request body</span></span>
<span data-ttu-id="2f784-126">在请求正文中，提供 [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2f784-126">In the request body, supply a JSON representation for the [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md) object.</span></span>

<span data-ttu-id="2f784-127">下表显示了创建 [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="2f784-127">The following table shows the properties that are required when you create the [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md).</span></span>

|<span data-ttu-id="2f784-128">属性</span><span class="sxs-lookup"><span data-stu-id="2f784-128">Property</span></span>|<span data-ttu-id="2f784-129">类型</span><span class="sxs-lookup"><span data-stu-id="2f784-129">Type</span></span>|<span data-ttu-id="2f784-130">说明</span><span class="sxs-lookup"><span data-stu-id="2f784-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2f784-131">id</span><span class="sxs-lookup"><span data-stu-id="2f784-131">id</span></span>|<span data-ttu-id="2f784-132">字符串</span><span class="sxs-lookup"><span data-stu-id="2f784-132">String</span></span>|<span data-ttu-id="2f784-133">实体的键。</span><span class="sxs-lookup"><span data-stu-id="2f784-133">Key of the entity.</span></span> <span data-ttu-id="2f784-134">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="2f784-134">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="2f784-135">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="2f784-135">createdDateTime</span></span>|<span data-ttu-id="2f784-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2f784-136">DateTimeOffset</span></span>|<span data-ttu-id="2f784-137">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="2f784-137">DateTime the object was created.</span></span> <span data-ttu-id="2f784-138">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="2f784-138">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="2f784-139">description</span><span class="sxs-lookup"><span data-stu-id="2f784-139">description</span></span>|<span data-ttu-id="2f784-140">String</span><span class="sxs-lookup"><span data-stu-id="2f784-140">String</span></span>|<span data-ttu-id="2f784-141">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="2f784-141">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="2f784-142">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="2f784-142">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="2f784-143">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2f784-143">lastModifiedDateTime</span></span>|<span data-ttu-id="2f784-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2f784-144">DateTimeOffset</span></span>|<span data-ttu-id="2f784-145">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="2f784-145">DateTime the object was last modified.</span></span> <span data-ttu-id="2f784-146">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="2f784-146">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="2f784-147">displayName</span><span class="sxs-lookup"><span data-stu-id="2f784-147">displayName</span></span>|<span data-ttu-id="2f784-148">字符串</span><span class="sxs-lookup"><span data-stu-id="2f784-148">String</span></span>|<span data-ttu-id="2f784-149">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="2f784-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="2f784-150">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="2f784-150">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="2f784-151">version</span><span class="sxs-lookup"><span data-stu-id="2f784-151">version</span></span>|<span data-ttu-id="2f784-152">Int32</span><span class="sxs-lookup"><span data-stu-id="2f784-152">Int32</span></span>|<span data-ttu-id="2f784-153">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="2f784-153">Version of the device configuration.</span></span> <span data-ttu-id="2f784-154">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="2f784-154">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="2f784-155">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="2f784-155">passwordRequired</span></span>|<span data-ttu-id="2f784-156">布尔值</span><span class="sxs-lookup"><span data-stu-id="2f784-156">Boolean</span></span>|<span data-ttu-id="2f784-157">需要密码才可解锁 Windows Phone 设备。</span><span class="sxs-lookup"><span data-stu-id="2f784-157">Require a password to unlock Windows Phone device.</span></span>|
|<span data-ttu-id="2f784-158">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="2f784-158">passwordBlockSimple</span></span>|<span data-ttu-id="2f784-159">Boolean</span><span class="sxs-lookup"><span data-stu-id="2f784-159">Boolean</span></span>|<span data-ttu-id="2f784-160">是否阻止同步日历。</span><span class="sxs-lookup"><span data-stu-id="2f784-160">Whether or not to block syncing the calendar.</span></span>|
|<span data-ttu-id="2f784-161">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="2f784-161">passwordMinimumLength</span></span>|<span data-ttu-id="2f784-162">Int32</span><span class="sxs-lookup"><span data-stu-id="2f784-162">Int32</span></span>|<span data-ttu-id="2f784-163">最短密码长度。</span><span class="sxs-lookup"><span data-stu-id="2f784-163">Minimum password length.</span></span> <span data-ttu-id="2f784-164">有效值为 4 至 16</span><span class="sxs-lookup"><span data-stu-id="2f784-164">Valid values 4 to 16</span></span>|
|<span data-ttu-id="2f784-165">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="2f784-165">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="2f784-166">Int32</span><span class="sxs-lookup"><span data-stu-id="2f784-166">Int32</span></span>|<span data-ttu-id="2f784-167">密码中必需的字符集数。</span><span class="sxs-lookup"><span data-stu-id="2f784-167">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="2f784-168">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="2f784-168">passwordRequiredType</span></span>|[<span data-ttu-id="2f784-169">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="2f784-169">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="2f784-170">必需的密码类型。</span><span class="sxs-lookup"><span data-stu-id="2f784-170">The required password type.</span></span> <span data-ttu-id="2f784-171">可取值为：`deviceDefault`、`alphanumeric`、`numeric`。</span><span class="sxs-lookup"><span data-stu-id="2f784-171">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="2f784-172">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="2f784-172">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="2f784-173">Int32</span><span class="sxs-lookup"><span data-stu-id="2f784-173">Int32</span></span>|<span data-ttu-id="2f784-174">防止重复使用的先前密码的数量。</span><span class="sxs-lookup"><span data-stu-id="2f784-174">The number of previous passwords to prevent re-use of.</span></span>|
|<span data-ttu-id="2f784-175">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="2f784-175">passwordExpirationDays</span></span>|<span data-ttu-id="2f784-176">Int32</span><span class="sxs-lookup"><span data-stu-id="2f784-176">Int32</span></span>|<span data-ttu-id="2f784-177">密码过期前的天数。</span><span class="sxs-lookup"><span data-stu-id="2f784-177">Number of days before password expiration.</span></span> <span data-ttu-id="2f784-178">有效值为 1 至 255</span><span class="sxs-lookup"><span data-stu-id="2f784-178">Valid values 1 to 255</span></span>|
|<span data-ttu-id="2f784-179">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="2f784-179">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="2f784-180">Int32</span><span class="sxs-lookup"><span data-stu-id="2f784-180">Int32</span></span>|<span data-ttu-id="2f784-181">在需要密码之前不活动的分钟数。</span><span class="sxs-lookup"><span data-stu-id="2f784-181">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="2f784-182">passwordRequireToUnlockFromIdle</span><span class="sxs-lookup"><span data-stu-id="2f784-182">passwordRequireToUnlockFromIdle</span></span>|<span data-ttu-id="2f784-183">Boolean</span><span class="sxs-lookup"><span data-stu-id="2f784-183">Boolean</span></span>|<span data-ttu-id="2f784-184">需要密码才可解锁空闲设备。</span><span class="sxs-lookup"><span data-stu-id="2f784-184">Require a password to unlock an idle device.</span></span>|
|<span data-ttu-id="2f784-185">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="2f784-185">osMinimumVersion</span></span>|<span data-ttu-id="2f784-186">String</span><span class="sxs-lookup"><span data-stu-id="2f784-186">String</span></span>|<span data-ttu-id="2f784-187">最低 Windows Phone 版本。</span><span class="sxs-lookup"><span data-stu-id="2f784-187">Minimum Windows Phone version.</span></span>|
|<span data-ttu-id="2f784-188">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="2f784-188">osMaximumVersion</span></span>|<span data-ttu-id="2f784-189">String</span><span class="sxs-lookup"><span data-stu-id="2f784-189">String</span></span>|<span data-ttu-id="2f784-190">最高 Windows Phone 版本。</span><span class="sxs-lookup"><span data-stu-id="2f784-190">Maximum Windows Phone version.</span></span>|
|<span data-ttu-id="2f784-191">earlyLaunchAntiMalwareDriverEnabled</span><span class="sxs-lookup"><span data-stu-id="2f784-191">earlyLaunchAntiMalwareDriverEnabled</span></span>|<span data-ttu-id="2f784-192">布尔值</span><span class="sxs-lookup"><span data-stu-id="2f784-192">Boolean</span></span>|<span data-ttu-id="2f784-193">要求设备由 Windows 设备运行状况证明报告为正常 - 提前启动反恶意驱动程序已启用。</span><span class="sxs-lookup"><span data-stu-id="2f784-193">Require devices to be reported as healthy by Windows Device Health Attestation - early launch antimalware driver is enabled.</span></span>|
|<span data-ttu-id="2f784-194">bitLockerEnabled</span><span class="sxs-lookup"><span data-stu-id="2f784-194">bitLockerEnabled</span></span>|<span data-ttu-id="2f784-195">布尔值</span><span class="sxs-lookup"><span data-stu-id="2f784-195">Boolean</span></span>|<span data-ttu-id="2f784-196">要求设备由 Windows 设备运行状况证明报告为正常 - bit locker 已启用。</span><span class="sxs-lookup"><span data-stu-id="2f784-196">Require devices to be reported healthy by Windows Device Health Attestation - bit locker is enabled</span></span>|
|<span data-ttu-id="2f784-197">secureBootEnabled</span><span class="sxs-lookup"><span data-stu-id="2f784-197">secureBootEnabled</span></span>|<span data-ttu-id="2f784-198">布尔值</span><span class="sxs-lookup"><span data-stu-id="2f784-198">Boolean</span></span>|<span data-ttu-id="2f784-199">要求设备由 Windows 设备运行状况证明报告为正常 - 安全启动已启用。</span><span class="sxs-lookup"><span data-stu-id="2f784-199">Require devices to be reported as healthy by Windows Device Health Attestation - secure boot is enabled.</span></span>|
|<span data-ttu-id="2f784-200">codeIntegrityEnabled</span><span class="sxs-lookup"><span data-stu-id="2f784-200">codeIntegrityEnabled</span></span>|<span data-ttu-id="2f784-201">布尔值</span><span class="sxs-lookup"><span data-stu-id="2f784-201">Boolean</span></span>|<span data-ttu-id="2f784-202">要求设备由 Windows 设备运行状况证明报告为正常。</span><span class="sxs-lookup"><span data-stu-id="2f784-202">Require devices to be reported as healthy by Windows Device Health Attestation.</span></span>|
|<span data-ttu-id="2f784-203">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="2f784-203">storageRequireEncryption</span></span>|<span data-ttu-id="2f784-204">布尔值</span><span class="sxs-lookup"><span data-stu-id="2f784-204">Boolean</span></span>|<span data-ttu-id="2f784-205">要求对 Windows 设备加密。</span><span class="sxs-lookup"><span data-stu-id="2f784-205">Require encryption on windows devices.</span></span>|



## <a name="response"></a><span data-ttu-id="2f784-206">响应</span><span class="sxs-lookup"><span data-stu-id="2f784-206">Response</span></span>
<span data-ttu-id="2f784-207">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和更新的 [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="2f784-207">If successful, this method returns a `200 OK` response code and an updated [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2f784-208">示例</span><span class="sxs-lookup"><span data-stu-id="2f784-208">Example</span></span>

### <a name="request"></a><span data-ttu-id="2f784-209">请求</span><span class="sxs-lookup"><span data-stu-id="2f784-209">Request</span></span>
<span data-ttu-id="2f784-210">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="2f784-210">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="2f784-211">响应</span><span class="sxs-lookup"><span data-stu-id="2f784-211">Response</span></span>
<span data-ttu-id="2f784-p111">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="2f784-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



