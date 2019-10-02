---
title: 创建 windows10MobileCompliancePolicy
description: 创建新的 windows10MobileCompliancePolicy 对象。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: c0bad02732400a9efe06035dc7188e2416600455
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/02/2019
ms.locfileid: "37365310"
---
# <a name="create-windows10mobilecompliancepolicy"></a><span data-ttu-id="72cdc-103">创建 windows10MobileCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="72cdc-103">Create windows10MobileCompliancePolicy</span></span>

> <span data-ttu-id="72cdc-104">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="72cdc-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="72cdc-105">创建新的 [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="72cdc-105">Create a new [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="72cdc-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="72cdc-106">Prerequisites</span></span>
<span data-ttu-id="72cdc-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="72cdc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="72cdc-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="72cdc-109">Permission type</span></span>|<span data-ttu-id="72cdc-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="72cdc-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="72cdc-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="72cdc-111">Delegated (work or school account)</span></span>|<span data-ttu-id="72cdc-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="72cdc-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="72cdc-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="72cdc-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="72cdc-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="72cdc-114">Not supported.</span></span>|
|<span data-ttu-id="72cdc-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="72cdc-115">Application</span></span>|<span data-ttu-id="72cdc-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="72cdc-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="72cdc-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="72cdc-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="72cdc-118">请求头</span><span class="sxs-lookup"><span data-stu-id="72cdc-118">Request headers</span></span>
|<span data-ttu-id="72cdc-119">标头</span><span class="sxs-lookup"><span data-stu-id="72cdc-119">Header</span></span>|<span data-ttu-id="72cdc-120">值</span><span class="sxs-lookup"><span data-stu-id="72cdc-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="72cdc-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="72cdc-121">Authorization</span></span>|<span data-ttu-id="72cdc-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="72cdc-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="72cdc-123">接受</span><span class="sxs-lookup"><span data-stu-id="72cdc-123">Accept</span></span>|<span data-ttu-id="72cdc-124">application/json</span><span class="sxs-lookup"><span data-stu-id="72cdc-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="72cdc-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="72cdc-125">Request body</span></span>
<span data-ttu-id="72cdc-126">在请求正文中，提供 windows10MobileCompliancePolicy 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="72cdc-126">In the request body, supply a JSON representation for the windows10MobileCompliancePolicy object.</span></span>

<span data-ttu-id="72cdc-127">下表显示了创建 windows10MobileCompliancePolicy 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="72cdc-127">The following table shows the properties that are required when you create the windows10MobileCompliancePolicy.</span></span>

|<span data-ttu-id="72cdc-128">属性</span><span class="sxs-lookup"><span data-stu-id="72cdc-128">Property</span></span>|<span data-ttu-id="72cdc-129">类型</span><span class="sxs-lookup"><span data-stu-id="72cdc-129">Type</span></span>|<span data-ttu-id="72cdc-130">说明</span><span class="sxs-lookup"><span data-stu-id="72cdc-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="72cdc-131">id</span><span class="sxs-lookup"><span data-stu-id="72cdc-131">id</span></span>|<span data-ttu-id="72cdc-132">字符串</span><span class="sxs-lookup"><span data-stu-id="72cdc-132">String</span></span>|<span data-ttu-id="72cdc-133">实体的键。</span><span class="sxs-lookup"><span data-stu-id="72cdc-133">Key of the entity.</span></span> <span data-ttu-id="72cdc-134">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="72cdc-134">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="72cdc-135">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="72cdc-135">createdDateTime</span></span>|<span data-ttu-id="72cdc-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="72cdc-136">DateTimeOffset</span></span>|<span data-ttu-id="72cdc-137">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="72cdc-137">DateTime the object was created.</span></span> <span data-ttu-id="72cdc-138">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="72cdc-138">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="72cdc-139">说明</span><span class="sxs-lookup"><span data-stu-id="72cdc-139">description</span></span>|<span data-ttu-id="72cdc-140">String</span><span class="sxs-lookup"><span data-stu-id="72cdc-140">String</span></span>|<span data-ttu-id="72cdc-141">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="72cdc-141">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="72cdc-142">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="72cdc-142">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="72cdc-143">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="72cdc-143">lastModifiedDateTime</span></span>|<span data-ttu-id="72cdc-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="72cdc-144">DateTimeOffset</span></span>|<span data-ttu-id="72cdc-145">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="72cdc-145">DateTime the object was last modified.</span></span> <span data-ttu-id="72cdc-146">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="72cdc-146">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="72cdc-147">displayName</span><span class="sxs-lookup"><span data-stu-id="72cdc-147">displayName</span></span>|<span data-ttu-id="72cdc-148">字符串</span><span class="sxs-lookup"><span data-stu-id="72cdc-148">String</span></span>|<span data-ttu-id="72cdc-149">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="72cdc-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="72cdc-150">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="72cdc-150">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="72cdc-151">version</span><span class="sxs-lookup"><span data-stu-id="72cdc-151">version</span></span>|<span data-ttu-id="72cdc-152">Int32</span><span class="sxs-lookup"><span data-stu-id="72cdc-152">Int32</span></span>|<span data-ttu-id="72cdc-153">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="72cdc-153">Version of the device configuration.</span></span> <span data-ttu-id="72cdc-154">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="72cdc-154">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="72cdc-155">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="72cdc-155">passwordRequired</span></span>|<span data-ttu-id="72cdc-156">Boolean</span><span class="sxs-lookup"><span data-stu-id="72cdc-156">Boolean</span></span>|<span data-ttu-id="72cdc-157">需要密码才可解锁 Windows Phone 设备。</span><span class="sxs-lookup"><span data-stu-id="72cdc-157">Require a password to unlock Windows Phone device.</span></span>|
|<span data-ttu-id="72cdc-158">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="72cdc-158">passwordBlockSimple</span></span>|<span data-ttu-id="72cdc-159">Boolean</span><span class="sxs-lookup"><span data-stu-id="72cdc-159">Boolean</span></span>|<span data-ttu-id="72cdc-160">是否阻止同步日历。</span><span class="sxs-lookup"><span data-stu-id="72cdc-160">Whether or not to block syncing the calendar.</span></span>|
|<span data-ttu-id="72cdc-161">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="72cdc-161">passwordMinimumLength</span></span>|<span data-ttu-id="72cdc-162">Int32</span><span class="sxs-lookup"><span data-stu-id="72cdc-162">Int32</span></span>|<span data-ttu-id="72cdc-163">最短密码长度。</span><span class="sxs-lookup"><span data-stu-id="72cdc-163">Minimum password length.</span></span> <span data-ttu-id="72cdc-164">有效值为 4 至 16</span><span class="sxs-lookup"><span data-stu-id="72cdc-164">Valid values 4 to 16</span></span>|
|<span data-ttu-id="72cdc-165">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="72cdc-165">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="72cdc-166">Int32</span><span class="sxs-lookup"><span data-stu-id="72cdc-166">Int32</span></span>|<span data-ttu-id="72cdc-167">密码中必需的字符集数。</span><span class="sxs-lookup"><span data-stu-id="72cdc-167">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="72cdc-168">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="72cdc-168">passwordRequiredType</span></span>|[<span data-ttu-id="72cdc-169">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="72cdc-169">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="72cdc-170">必需的密码类型。</span><span class="sxs-lookup"><span data-stu-id="72cdc-170">The required password type.</span></span> <span data-ttu-id="72cdc-171">可取值为：`deviceDefault`、`alphanumeric`、`numeric`。</span><span class="sxs-lookup"><span data-stu-id="72cdc-171">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="72cdc-172">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="72cdc-172">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="72cdc-173">Int32</span><span class="sxs-lookup"><span data-stu-id="72cdc-173">Int32</span></span>|<span data-ttu-id="72cdc-174">防止重复使用的先前密码的数量。</span><span class="sxs-lookup"><span data-stu-id="72cdc-174">The number of previous passwords to prevent re-use of.</span></span>|
|<span data-ttu-id="72cdc-175">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="72cdc-175">passwordExpirationDays</span></span>|<span data-ttu-id="72cdc-176">Int32</span><span class="sxs-lookup"><span data-stu-id="72cdc-176">Int32</span></span>|<span data-ttu-id="72cdc-177">密码过期前的天数。</span><span class="sxs-lookup"><span data-stu-id="72cdc-177">Number of days before password expiration.</span></span> <span data-ttu-id="72cdc-178">有效值为 1 至 255</span><span class="sxs-lookup"><span data-stu-id="72cdc-178">Valid values 1 to 255</span></span>|
|<span data-ttu-id="72cdc-179">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="72cdc-179">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="72cdc-180">Int32</span><span class="sxs-lookup"><span data-stu-id="72cdc-180">Int32</span></span>|<span data-ttu-id="72cdc-181">在需要密码之前不活动的分钟数。</span><span class="sxs-lookup"><span data-stu-id="72cdc-181">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="72cdc-182">passwordRequireToUnlockFromIdle</span><span class="sxs-lookup"><span data-stu-id="72cdc-182">passwordRequireToUnlockFromIdle</span></span>|<span data-ttu-id="72cdc-183">Boolean</span><span class="sxs-lookup"><span data-stu-id="72cdc-183">Boolean</span></span>|<span data-ttu-id="72cdc-184">需要密码才可解锁空闲设备。</span><span class="sxs-lookup"><span data-stu-id="72cdc-184">Require a password to unlock an idle device.</span></span>|
|<span data-ttu-id="72cdc-185">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="72cdc-185">osMinimumVersion</span></span>|<span data-ttu-id="72cdc-186">String</span><span class="sxs-lookup"><span data-stu-id="72cdc-186">String</span></span>|<span data-ttu-id="72cdc-187">最低 Windows Phone 版本。</span><span class="sxs-lookup"><span data-stu-id="72cdc-187">Minimum Windows Phone version.</span></span>|
|<span data-ttu-id="72cdc-188">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="72cdc-188">osMaximumVersion</span></span>|<span data-ttu-id="72cdc-189">String</span><span class="sxs-lookup"><span data-stu-id="72cdc-189">String</span></span>|<span data-ttu-id="72cdc-190">最高 Windows Phone 版本。</span><span class="sxs-lookup"><span data-stu-id="72cdc-190">Maximum Windows Phone version.</span></span>|
|<span data-ttu-id="72cdc-191">earlyLaunchAntiMalwareDriverEnabled</span><span class="sxs-lookup"><span data-stu-id="72cdc-191">earlyLaunchAntiMalwareDriverEnabled</span></span>|<span data-ttu-id="72cdc-192">Boolean</span><span class="sxs-lookup"><span data-stu-id="72cdc-192">Boolean</span></span>|<span data-ttu-id="72cdc-193">要求设备由 Windows 设备运行状况证明报告为正常 - 提前启动反恶意驱动程序已启用。</span><span class="sxs-lookup"><span data-stu-id="72cdc-193">Require devices to be reported as healthy by Windows Device Health Attestation - early launch antimalware driver is enabled.</span></span>|
|<span data-ttu-id="72cdc-194">bitLockerEnabled</span><span class="sxs-lookup"><span data-stu-id="72cdc-194">bitLockerEnabled</span></span>|<span data-ttu-id="72cdc-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="72cdc-195">Boolean</span></span>|<span data-ttu-id="72cdc-196">要求设备由 Windows 设备运行状况证明报告为正常 - bit locker 已启用。</span><span class="sxs-lookup"><span data-stu-id="72cdc-196">Require devices to be reported healthy by Windows Device Health Attestation - bit locker is enabled</span></span>|
|<span data-ttu-id="72cdc-197">secureBootEnabled</span><span class="sxs-lookup"><span data-stu-id="72cdc-197">secureBootEnabled</span></span>|<span data-ttu-id="72cdc-198">Boolean</span><span class="sxs-lookup"><span data-stu-id="72cdc-198">Boolean</span></span>|<span data-ttu-id="72cdc-199">要求设备由 Windows 设备运行状况证明报告为正常 - 安全启动已启用。</span><span class="sxs-lookup"><span data-stu-id="72cdc-199">Require devices to be reported as healthy by Windows Device Health Attestation - secure boot is enabled.</span></span>|
|<span data-ttu-id="72cdc-200">codeIntegrityEnabled</span><span class="sxs-lookup"><span data-stu-id="72cdc-200">codeIntegrityEnabled</span></span>|<span data-ttu-id="72cdc-201">Boolean</span><span class="sxs-lookup"><span data-stu-id="72cdc-201">Boolean</span></span>|<span data-ttu-id="72cdc-202">要求设备由 Windows 设备运行状况证明报告为正常。</span><span class="sxs-lookup"><span data-stu-id="72cdc-202">Require devices to be reported as healthy by Windows Device Health Attestation.</span></span>|
|<span data-ttu-id="72cdc-203">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="72cdc-203">storageRequireEncryption</span></span>|<span data-ttu-id="72cdc-204">Boolean</span><span class="sxs-lookup"><span data-stu-id="72cdc-204">Boolean</span></span>|<span data-ttu-id="72cdc-205">要求对 Windows 设备加密。</span><span class="sxs-lookup"><span data-stu-id="72cdc-205">Require encryption on windows devices.</span></span>|



## <a name="response"></a><span data-ttu-id="72cdc-206">响应</span><span class="sxs-lookup"><span data-stu-id="72cdc-206">Response</span></span>
<span data-ttu-id="72cdc-207">如果成功，此方法将在响应正文中返回 `201 Created` 响应代码和 [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="72cdc-207">If successful, this method returns a `201 Created` response code and a [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="72cdc-208">示例</span><span class="sxs-lookup"><span data-stu-id="72cdc-208">Example</span></span>

### <a name="request"></a><span data-ttu-id="72cdc-209">请求</span><span class="sxs-lookup"><span data-stu-id="72cdc-209">Request</span></span>
<span data-ttu-id="72cdc-210">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="72cdc-210">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="72cdc-211">响应</span><span class="sxs-lookup"><span data-stu-id="72cdc-211">Response</span></span>
<span data-ttu-id="72cdc-p111">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="72cdc-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




