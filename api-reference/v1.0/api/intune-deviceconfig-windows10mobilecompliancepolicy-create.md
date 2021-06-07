---
title: 创建 windows10MobileCompliancePolicy
description: 创建新的 windows10MobileCompliancePolicy 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 1b8ba7f0ef1b78abe538442d3b0efc6b4caf8012
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52760515"
---
# <a name="create-windows10mobilecompliancepolicy"></a><span data-ttu-id="5fbc3-103">创建 windows10MobileCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="5fbc3-103">Create windows10MobileCompliancePolicy</span></span>

<span data-ttu-id="5fbc3-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5fbc3-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5fbc3-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="5fbc3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5fbc3-106">创建新的 [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="5fbc3-106">Create a new [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5fbc3-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="5fbc3-107">Prerequisites</span></span>
<span data-ttu-id="5fbc3-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="5fbc3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5fbc3-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="5fbc3-110">Permission type</span></span>|<span data-ttu-id="5fbc3-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="5fbc3-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5fbc3-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5fbc3-112">Delegated (work or school account)</span></span>|<span data-ttu-id="5fbc3-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5fbc3-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="5fbc3-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5fbc3-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5fbc3-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="5fbc3-115">Not supported.</span></span>|
|<span data-ttu-id="5fbc3-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="5fbc3-116">Application</span></span>|<span data-ttu-id="5fbc3-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5fbc3-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="5fbc3-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5fbc3-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="5fbc3-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="5fbc3-119">Request headers</span></span>
|<span data-ttu-id="5fbc3-120">标头</span><span class="sxs-lookup"><span data-stu-id="5fbc3-120">Header</span></span>|<span data-ttu-id="5fbc3-121">值</span><span class="sxs-lookup"><span data-stu-id="5fbc3-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5fbc3-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="5fbc3-122">Authorization</span></span>|<span data-ttu-id="5fbc3-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="5fbc3-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5fbc3-124">接受</span><span class="sxs-lookup"><span data-stu-id="5fbc3-124">Accept</span></span>|<span data-ttu-id="5fbc3-125">application/json</span><span class="sxs-lookup"><span data-stu-id="5fbc3-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5fbc3-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="5fbc3-126">Request body</span></span>
<span data-ttu-id="5fbc3-127">在请求正文中，提供 windows10MobileCompliancePolicy 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5fbc3-127">In the request body, supply a JSON representation for the windows10MobileCompliancePolicy object.</span></span>

<span data-ttu-id="5fbc3-128">下表显示了创建 windows10MobileCompliancePolicy 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="5fbc3-128">The following table shows the properties that are required when you create the windows10MobileCompliancePolicy.</span></span>

|<span data-ttu-id="5fbc3-129">属性</span><span class="sxs-lookup"><span data-stu-id="5fbc3-129">Property</span></span>|<span data-ttu-id="5fbc3-130">类型</span><span class="sxs-lookup"><span data-stu-id="5fbc3-130">Type</span></span>|<span data-ttu-id="5fbc3-131">说明</span><span class="sxs-lookup"><span data-stu-id="5fbc3-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5fbc3-132">id</span><span class="sxs-lookup"><span data-stu-id="5fbc3-132">id</span></span>|<span data-ttu-id="5fbc3-133">String</span><span class="sxs-lookup"><span data-stu-id="5fbc3-133">String</span></span>|<span data-ttu-id="5fbc3-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="5fbc3-134">Key of the entity.</span></span> <span data-ttu-id="5fbc3-135">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="5fbc3-135">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="5fbc3-136">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="5fbc3-136">createdDateTime</span></span>|<span data-ttu-id="5fbc3-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5fbc3-137">DateTimeOffset</span></span>|<span data-ttu-id="5fbc3-138">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="5fbc3-138">DateTime the object was created.</span></span> <span data-ttu-id="5fbc3-139">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="5fbc3-139">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="5fbc3-140">description</span><span class="sxs-lookup"><span data-stu-id="5fbc3-140">description</span></span>|<span data-ttu-id="5fbc3-141">String</span><span class="sxs-lookup"><span data-stu-id="5fbc3-141">String</span></span>|<span data-ttu-id="5fbc3-142">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="5fbc3-142">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="5fbc3-143">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="5fbc3-143">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="5fbc3-144">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="5fbc3-144">lastModifiedDateTime</span></span>|<span data-ttu-id="5fbc3-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5fbc3-145">DateTimeOffset</span></span>|<span data-ttu-id="5fbc3-146">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="5fbc3-146">DateTime the object was last modified.</span></span> <span data-ttu-id="5fbc3-147">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="5fbc3-147">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="5fbc3-148">displayName</span><span class="sxs-lookup"><span data-stu-id="5fbc3-148">displayName</span></span>|<span data-ttu-id="5fbc3-149">String</span><span class="sxs-lookup"><span data-stu-id="5fbc3-149">String</span></span>|<span data-ttu-id="5fbc3-150">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="5fbc3-150">Admin provided name of the device configuration.</span></span> <span data-ttu-id="5fbc3-151">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="5fbc3-151">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="5fbc3-152">version</span><span class="sxs-lookup"><span data-stu-id="5fbc3-152">version</span></span>|<span data-ttu-id="5fbc3-153">Int32</span><span class="sxs-lookup"><span data-stu-id="5fbc3-153">Int32</span></span>|<span data-ttu-id="5fbc3-154">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="5fbc3-154">Version of the device configuration.</span></span> <span data-ttu-id="5fbc3-155">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="5fbc3-155">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="5fbc3-156">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="5fbc3-156">passwordRequired</span></span>|<span data-ttu-id="5fbc3-157">Boolean</span><span class="sxs-lookup"><span data-stu-id="5fbc3-157">Boolean</span></span>|<span data-ttu-id="5fbc3-158">需要密码才可解锁 Windows Phone 设备。</span><span class="sxs-lookup"><span data-stu-id="5fbc3-158">Require a password to unlock Windows Phone device.</span></span>|
|<span data-ttu-id="5fbc3-159">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="5fbc3-159">passwordBlockSimple</span></span>|<span data-ttu-id="5fbc3-160">Boolean</span><span class="sxs-lookup"><span data-stu-id="5fbc3-160">Boolean</span></span>|<span data-ttu-id="5fbc3-161">是否阻止同步日历。</span><span class="sxs-lookup"><span data-stu-id="5fbc3-161">Whether or not to block syncing the calendar.</span></span>|
|<span data-ttu-id="5fbc3-162">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="5fbc3-162">passwordMinimumLength</span></span>|<span data-ttu-id="5fbc3-163">Int32</span><span class="sxs-lookup"><span data-stu-id="5fbc3-163">Int32</span></span>|<span data-ttu-id="5fbc3-164">最短密码长度。</span><span class="sxs-lookup"><span data-stu-id="5fbc3-164">Minimum password length.</span></span> <span data-ttu-id="5fbc3-165">有效值为 4 至 16</span><span class="sxs-lookup"><span data-stu-id="5fbc3-165">Valid values 4 to 16</span></span>|
|<span data-ttu-id="5fbc3-166">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="5fbc3-166">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="5fbc3-167">Int32</span><span class="sxs-lookup"><span data-stu-id="5fbc3-167">Int32</span></span>|<span data-ttu-id="5fbc3-168">密码中必需的字符集数。</span><span class="sxs-lookup"><span data-stu-id="5fbc3-168">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="5fbc3-169">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="5fbc3-169">passwordRequiredType</span></span>|[<span data-ttu-id="5fbc3-170">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="5fbc3-170">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="5fbc3-171">必需的密码类型。</span><span class="sxs-lookup"><span data-stu-id="5fbc3-171">The required password type.</span></span> <span data-ttu-id="5fbc3-172">可取值为：`deviceDefault`、`alphanumeric`、`numeric`。</span><span class="sxs-lookup"><span data-stu-id="5fbc3-172">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="5fbc3-173">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="5fbc3-173">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="5fbc3-174">Int32</span><span class="sxs-lookup"><span data-stu-id="5fbc3-174">Int32</span></span>|<span data-ttu-id="5fbc3-175">防止重复使用的先前密码的数量。</span><span class="sxs-lookup"><span data-stu-id="5fbc3-175">The number of previous passwords to prevent re-use of.</span></span>|
|<span data-ttu-id="5fbc3-176">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="5fbc3-176">passwordExpirationDays</span></span>|<span data-ttu-id="5fbc3-177">Int32</span><span class="sxs-lookup"><span data-stu-id="5fbc3-177">Int32</span></span>|<span data-ttu-id="5fbc3-178">密码过期前的天数。</span><span class="sxs-lookup"><span data-stu-id="5fbc3-178">Number of days before password expiration.</span></span> <span data-ttu-id="5fbc3-179">有效值为 1 至 255</span><span class="sxs-lookup"><span data-stu-id="5fbc3-179">Valid values 1 to 255</span></span>|
|<span data-ttu-id="5fbc3-180">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="5fbc3-180">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="5fbc3-181">Int32</span><span class="sxs-lookup"><span data-stu-id="5fbc3-181">Int32</span></span>|<span data-ttu-id="5fbc3-182">在需要密码之前不活动的分钟数。</span><span class="sxs-lookup"><span data-stu-id="5fbc3-182">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="5fbc3-183">passwordRequireToUnlockFromIdle</span><span class="sxs-lookup"><span data-stu-id="5fbc3-183">passwordRequireToUnlockFromIdle</span></span>|<span data-ttu-id="5fbc3-184">Boolean</span><span class="sxs-lookup"><span data-stu-id="5fbc3-184">Boolean</span></span>|<span data-ttu-id="5fbc3-185">需要密码才可解锁空闲设备。</span><span class="sxs-lookup"><span data-stu-id="5fbc3-185">Require a password to unlock an idle device.</span></span>|
|<span data-ttu-id="5fbc3-186">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="5fbc3-186">osMinimumVersion</span></span>|<span data-ttu-id="5fbc3-187">String</span><span class="sxs-lookup"><span data-stu-id="5fbc3-187">String</span></span>|<span data-ttu-id="5fbc3-188">最低 Windows Phone 版本。</span><span class="sxs-lookup"><span data-stu-id="5fbc3-188">Minimum Windows Phone version.</span></span>|
|<span data-ttu-id="5fbc3-189">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="5fbc3-189">osMaximumVersion</span></span>|<span data-ttu-id="5fbc3-190">String</span><span class="sxs-lookup"><span data-stu-id="5fbc3-190">String</span></span>|<span data-ttu-id="5fbc3-191">最高 Windows Phone 版本。</span><span class="sxs-lookup"><span data-stu-id="5fbc3-191">Maximum Windows Phone version.</span></span>|
|<span data-ttu-id="5fbc3-192">earlyLaunchAntiMalwareDriverEnabled</span><span class="sxs-lookup"><span data-stu-id="5fbc3-192">earlyLaunchAntiMalwareDriverEnabled</span></span>|<span data-ttu-id="5fbc3-193">Boolean</span><span class="sxs-lookup"><span data-stu-id="5fbc3-193">Boolean</span></span>|<span data-ttu-id="5fbc3-194">要求设备由 Windows 设备运行状况证明报告为正常 - 提前启动反恶意驱动程序已启用。</span><span class="sxs-lookup"><span data-stu-id="5fbc3-194">Require devices to be reported as healthy by Windows Device Health Attestation - early launch antimalware driver is enabled.</span></span>|
|<span data-ttu-id="5fbc3-195">bitLockerEnabled</span><span class="sxs-lookup"><span data-stu-id="5fbc3-195">bitLockerEnabled</span></span>|<span data-ttu-id="5fbc3-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="5fbc3-196">Boolean</span></span>|<span data-ttu-id="5fbc3-197">要求设备由 Windows 设备运行状况证明报告为正常 - bit locker 已启用。</span><span class="sxs-lookup"><span data-stu-id="5fbc3-197">Require devices to be reported healthy by Windows Device Health Attestation - bit locker is enabled</span></span>|
|<span data-ttu-id="5fbc3-198">secureBootEnabled</span><span class="sxs-lookup"><span data-stu-id="5fbc3-198">secureBootEnabled</span></span>|<span data-ttu-id="5fbc3-199">Boolean</span><span class="sxs-lookup"><span data-stu-id="5fbc3-199">Boolean</span></span>|<span data-ttu-id="5fbc3-200">要求设备由 Windows 设备运行状况证明报告为正常 - 安全启动已启用。</span><span class="sxs-lookup"><span data-stu-id="5fbc3-200">Require devices to be reported as healthy by Windows Device Health Attestation - secure boot is enabled.</span></span>|
|<span data-ttu-id="5fbc3-201">codeIntegrityEnabled</span><span class="sxs-lookup"><span data-stu-id="5fbc3-201">codeIntegrityEnabled</span></span>|<span data-ttu-id="5fbc3-202">Boolean</span><span class="sxs-lookup"><span data-stu-id="5fbc3-202">Boolean</span></span>|<span data-ttu-id="5fbc3-203">要求设备由 Windows 设备运行状况证明报告为正常。</span><span class="sxs-lookup"><span data-stu-id="5fbc3-203">Require devices to be reported as healthy by Windows Device Health Attestation.</span></span>|
|<span data-ttu-id="5fbc3-204">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="5fbc3-204">storageRequireEncryption</span></span>|<span data-ttu-id="5fbc3-205">Boolean</span><span class="sxs-lookup"><span data-stu-id="5fbc3-205">Boolean</span></span>|<span data-ttu-id="5fbc3-206">要求对 Windows 设备加密。</span><span class="sxs-lookup"><span data-stu-id="5fbc3-206">Require encryption on windows devices.</span></span>|



## <a name="response"></a><span data-ttu-id="5fbc3-207">响应</span><span class="sxs-lookup"><span data-stu-id="5fbc3-207">Response</span></span>
<span data-ttu-id="5fbc3-208">如果成功，此方法将在响应正文中返回 `201 Created` 响应代码和 [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="5fbc3-208">If successful, this method returns a `201 Created` response code and a [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5fbc3-209">示例</span><span class="sxs-lookup"><span data-stu-id="5fbc3-209">Example</span></span>

### <a name="request"></a><span data-ttu-id="5fbc3-210">请求</span><span class="sxs-lookup"><span data-stu-id="5fbc3-210">Request</span></span>
<span data-ttu-id="5fbc3-211">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="5fbc3-211">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="5fbc3-212">响应</span><span class="sxs-lookup"><span data-stu-id="5fbc3-212">Response</span></span>
<span data-ttu-id="5fbc3-p111">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="5fbc3-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




