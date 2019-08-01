---
title: 更新 windows10CompliancePolicy
description: 更新 windows10CompliancePolicy 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: d894e85cbd1821f9223b3951c8c88756b90509b7
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36016921"
---
# <a name="update-windows10compliancepolicy"></a><span data-ttu-id="900a6-103">更新 windows10CompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="900a6-103">Update windows10CompliancePolicy</span></span>

> <span data-ttu-id="900a6-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="900a6-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="900a6-105">更新 [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="900a6-105">Update the properties of a [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="900a6-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="900a6-106">Prerequisites</span></span>
<span data-ttu-id="900a6-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="900a6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="900a6-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="900a6-109">Permission type</span></span>|<span data-ttu-id="900a6-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="900a6-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="900a6-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="900a6-111">Delegated (work or school account)</span></span>|<span data-ttu-id="900a6-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="900a6-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="900a6-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="900a6-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="900a6-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="900a6-114">Not supported.</span></span>|
|<span data-ttu-id="900a6-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="900a6-115">Application</span></span>|<span data-ttu-id="900a6-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="900a6-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="900a6-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="900a6-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="900a6-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="900a6-118">Request headers</span></span>
|<span data-ttu-id="900a6-119">标头</span><span class="sxs-lookup"><span data-stu-id="900a6-119">Header</span></span>|<span data-ttu-id="900a6-120">值</span><span class="sxs-lookup"><span data-stu-id="900a6-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="900a6-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="900a6-121">Authorization</span></span>|<span data-ttu-id="900a6-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="900a6-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="900a6-123">接受</span><span class="sxs-lookup"><span data-stu-id="900a6-123">Accept</span></span>|<span data-ttu-id="900a6-124">application/json</span><span class="sxs-lookup"><span data-stu-id="900a6-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="900a6-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="900a6-125">Request body</span></span>
<span data-ttu-id="900a6-126">在请求正文中，提供 [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="900a6-126">In the request body, supply a JSON representation for the [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) object.</span></span>

<span data-ttu-id="900a6-127">下表显示创建 [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="900a6-127">The following table shows the properties that are required when you create the [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md).</span></span>

|<span data-ttu-id="900a6-128">属性</span><span class="sxs-lookup"><span data-stu-id="900a6-128">Property</span></span>|<span data-ttu-id="900a6-129">类型</span><span class="sxs-lookup"><span data-stu-id="900a6-129">Type</span></span>|<span data-ttu-id="900a6-130">说明</span><span class="sxs-lookup"><span data-stu-id="900a6-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="900a6-131">id</span><span class="sxs-lookup"><span data-stu-id="900a6-131">id</span></span>|<span data-ttu-id="900a6-132">字符串</span><span class="sxs-lookup"><span data-stu-id="900a6-132">String</span></span>|<span data-ttu-id="900a6-133">实体的键。</span><span class="sxs-lookup"><span data-stu-id="900a6-133">Key of the entity.</span></span> <span data-ttu-id="900a6-134">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="900a6-134">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="900a6-135">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="900a6-135">createdDateTime</span></span>|<span data-ttu-id="900a6-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="900a6-136">DateTimeOffset</span></span>|<span data-ttu-id="900a6-137">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="900a6-137">DateTime the object was created.</span></span> <span data-ttu-id="900a6-138">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="900a6-138">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="900a6-139">说明</span><span class="sxs-lookup"><span data-stu-id="900a6-139">description</span></span>|<span data-ttu-id="900a6-140">String</span><span class="sxs-lookup"><span data-stu-id="900a6-140">String</span></span>|<span data-ttu-id="900a6-141">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="900a6-141">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="900a6-142">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="900a6-142">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="900a6-143">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="900a6-143">lastModifiedDateTime</span></span>|<span data-ttu-id="900a6-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="900a6-144">DateTimeOffset</span></span>|<span data-ttu-id="900a6-145">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="900a6-145">DateTime the object was last modified.</span></span> <span data-ttu-id="900a6-146">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="900a6-146">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="900a6-147">displayName</span><span class="sxs-lookup"><span data-stu-id="900a6-147">displayName</span></span>|<span data-ttu-id="900a6-148">字符串</span><span class="sxs-lookup"><span data-stu-id="900a6-148">String</span></span>|<span data-ttu-id="900a6-149">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="900a6-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="900a6-150">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="900a6-150">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="900a6-151">version</span><span class="sxs-lookup"><span data-stu-id="900a6-151">version</span></span>|<span data-ttu-id="900a6-152">Int32</span><span class="sxs-lookup"><span data-stu-id="900a6-152">Int32</span></span>|<span data-ttu-id="900a6-153">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="900a6-153">Version of the device configuration.</span></span> <span data-ttu-id="900a6-154">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="900a6-154">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="900a6-155">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="900a6-155">passwordRequired</span></span>|<span data-ttu-id="900a6-156">Boolean</span><span class="sxs-lookup"><span data-stu-id="900a6-156">Boolean</span></span>|<span data-ttu-id="900a6-157">需要密码才可解锁 Windows 设备。</span><span class="sxs-lookup"><span data-stu-id="900a6-157">Require a password to unlock Windows device.</span></span>|
|<span data-ttu-id="900a6-158">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="900a6-158">passwordBlockSimple</span></span>|<span data-ttu-id="900a6-159">Boolean</span><span class="sxs-lookup"><span data-stu-id="900a6-159">Boolean</span></span>|<span data-ttu-id="900a6-160">指示是否阻止简单密码。</span><span class="sxs-lookup"><span data-stu-id="900a6-160">Indicates whether or not to block simple password.</span></span>|
|<span data-ttu-id="900a6-161">passwordRequiredToUnlockFromIdle</span><span class="sxs-lookup"><span data-stu-id="900a6-161">passwordRequiredToUnlockFromIdle</span></span>|<span data-ttu-id="900a6-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="900a6-162">Boolean</span></span>|<span data-ttu-id="900a6-163">需要密码才可解锁空闲设备。</span><span class="sxs-lookup"><span data-stu-id="900a6-163">Require a password to unlock an idle device.</span></span>|
|<span data-ttu-id="900a6-164">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="900a6-164">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="900a6-165">Int32</span><span class="sxs-lookup"><span data-stu-id="900a6-165">Int32</span></span>|<span data-ttu-id="900a6-166">在需要密码之前不活动的分钟数。</span><span class="sxs-lookup"><span data-stu-id="900a6-166">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="900a6-167">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="900a6-167">passwordExpirationDays</span></span>|<span data-ttu-id="900a6-168">Int32</span><span class="sxs-lookup"><span data-stu-id="900a6-168">Int32</span></span>|<span data-ttu-id="900a6-169">密码过期天数。</span><span class="sxs-lookup"><span data-stu-id="900a6-169">The password expiration in days.</span></span>|
|<span data-ttu-id="900a6-170">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="900a6-170">passwordMinimumLength</span></span>|<span data-ttu-id="900a6-171">Int32</span><span class="sxs-lookup"><span data-stu-id="900a6-171">Int32</span></span>|<span data-ttu-id="900a6-172">密码最短长度。</span><span class="sxs-lookup"><span data-stu-id="900a6-172">The minimum password length.</span></span>|
|<span data-ttu-id="900a6-173">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="900a6-173">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="900a6-174">Int32</span><span class="sxs-lookup"><span data-stu-id="900a6-174">Int32</span></span>|<span data-ttu-id="900a6-175">密码中必需的字符集数。</span><span class="sxs-lookup"><span data-stu-id="900a6-175">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="900a6-176">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="900a6-176">passwordRequiredType</span></span>|[<span data-ttu-id="900a6-177">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="900a6-177">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="900a6-178">必需的密码类型。</span><span class="sxs-lookup"><span data-stu-id="900a6-178">The required password type.</span></span> <span data-ttu-id="900a6-179">可取值为：`deviceDefault`、`alphanumeric`、`numeric`。</span><span class="sxs-lookup"><span data-stu-id="900a6-179">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="900a6-180">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="900a6-180">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="900a6-181">Int32</span><span class="sxs-lookup"><span data-stu-id="900a6-181">Int32</span></span>|<span data-ttu-id="900a6-182">防止重复使用的先前密码的数量。</span><span class="sxs-lookup"><span data-stu-id="900a6-182">The number of previous passwords to prevent re-use of.</span></span>|
|<span data-ttu-id="900a6-183">requireHealthyDeviceReport</span><span class="sxs-lookup"><span data-stu-id="900a6-183">requireHealthyDeviceReport</span></span>|<span data-ttu-id="900a6-184">Boolean</span><span class="sxs-lookup"><span data-stu-id="900a6-184">Boolean</span></span>|<span data-ttu-id="900a6-185">要求设备由 Windows 设备运行状况证明报告为正常。</span><span class="sxs-lookup"><span data-stu-id="900a6-185">Require devices to be reported as healthy by Windows Device Health Attestation.</span></span>|
|<span data-ttu-id="900a6-186">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="900a6-186">osMinimumVersion</span></span>|<span data-ttu-id="900a6-187">String</span><span class="sxs-lookup"><span data-stu-id="900a6-187">String</span></span>|<span data-ttu-id="900a6-188">最低 Windows 10 版本。</span><span class="sxs-lookup"><span data-stu-id="900a6-188">Minimum Windows 10 version.</span></span>|
|<span data-ttu-id="900a6-189">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="900a6-189">osMaximumVersion</span></span>|<span data-ttu-id="900a6-190">String</span><span class="sxs-lookup"><span data-stu-id="900a6-190">String</span></span>|<span data-ttu-id="900a6-191">最高 Windows 10 版本。</span><span class="sxs-lookup"><span data-stu-id="900a6-191">Maximum Windows 10 version.</span></span>|
|<span data-ttu-id="900a6-192">mobileOsMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="900a6-192">mobileOsMinimumVersion</span></span>|<span data-ttu-id="900a6-193">String</span><span class="sxs-lookup"><span data-stu-id="900a6-193">String</span></span>|<span data-ttu-id="900a6-194">最低 Windows Phone 版本。</span><span class="sxs-lookup"><span data-stu-id="900a6-194">Minimum Windows Phone version.</span></span>|
|<span data-ttu-id="900a6-195">mobileOsMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="900a6-195">mobileOsMaximumVersion</span></span>|<span data-ttu-id="900a6-196">String</span><span class="sxs-lookup"><span data-stu-id="900a6-196">String</span></span>|<span data-ttu-id="900a6-197">最高 Windows Phone 版本。</span><span class="sxs-lookup"><span data-stu-id="900a6-197">Maximum Windows Phone version.</span></span>|
|<span data-ttu-id="900a6-198">earlyLaunchAntiMalwareDriverEnabled</span><span class="sxs-lookup"><span data-stu-id="900a6-198">earlyLaunchAntiMalwareDriverEnabled</span></span>|<span data-ttu-id="900a6-199">Boolean</span><span class="sxs-lookup"><span data-stu-id="900a6-199">Boolean</span></span>|<span data-ttu-id="900a6-200">要求设备由 Windows 设备运行状况证明报告为正常 - 提前启动反恶意驱动程序已启用。</span><span class="sxs-lookup"><span data-stu-id="900a6-200">Require devices to be reported as healthy by Windows Device Health Attestation - early launch antimalware driver is enabled.</span></span>|
|<span data-ttu-id="900a6-201">bitLockerEnabled</span><span class="sxs-lookup"><span data-stu-id="900a6-201">bitLockerEnabled</span></span>|<span data-ttu-id="900a6-202">Boolean</span><span class="sxs-lookup"><span data-stu-id="900a6-202">Boolean</span></span>|<span data-ttu-id="900a6-203">要求设备由 Windows 设备运行状况证明报告为正常 - bit locker 已启用。</span><span class="sxs-lookup"><span data-stu-id="900a6-203">Require devices to be reported healthy by Windows Device Health Attestation - bit locker is enabled</span></span>|
|<span data-ttu-id="900a6-204">secureBootEnabled</span><span class="sxs-lookup"><span data-stu-id="900a6-204">secureBootEnabled</span></span>|<span data-ttu-id="900a6-205">Boolean</span><span class="sxs-lookup"><span data-stu-id="900a6-205">Boolean</span></span>|<span data-ttu-id="900a6-206">要求设备由 Windows 设备运行状况证明报告为正常 - 安全启动已启用。</span><span class="sxs-lookup"><span data-stu-id="900a6-206">Require devices to be reported as healthy by Windows Device Health Attestation - secure boot is enabled.</span></span>|
|<span data-ttu-id="900a6-207">codeIntegrityEnabled</span><span class="sxs-lookup"><span data-stu-id="900a6-207">codeIntegrityEnabled</span></span>|<span data-ttu-id="900a6-208">Boolean</span><span class="sxs-lookup"><span data-stu-id="900a6-208">Boolean</span></span>|<span data-ttu-id="900a6-209">要求设备由 Windows 设备运行状况证明报告为正常。</span><span class="sxs-lookup"><span data-stu-id="900a6-209">Require devices to be reported as healthy by Windows Device Health Attestation.</span></span>|
|<span data-ttu-id="900a6-210">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="900a6-210">storageRequireEncryption</span></span>|<span data-ttu-id="900a6-211">Boolean</span><span class="sxs-lookup"><span data-stu-id="900a6-211">Boolean</span></span>|<span data-ttu-id="900a6-212">要求对 Windows 设备加密。</span><span class="sxs-lookup"><span data-stu-id="900a6-212">Require encryption on windows devices.</span></span>|



## <a name="response"></a><span data-ttu-id="900a6-213">响应</span><span class="sxs-lookup"><span data-stu-id="900a6-213">Response</span></span>
<span data-ttu-id="900a6-214">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和更新的 [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="900a6-214">If successful, this method returns a `200 OK` response code and an updated [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="900a6-215">示例</span><span class="sxs-lookup"><span data-stu-id="900a6-215">Example</span></span>

### <a name="request"></a><span data-ttu-id="900a6-216">请求</span><span class="sxs-lookup"><span data-stu-id="900a6-216">Request</span></span>
<span data-ttu-id="900a6-217">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="900a6-217">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="900a6-218">响应</span><span class="sxs-lookup"><span data-stu-id="900a6-218">Response</span></span>
<span data-ttu-id="900a6-p109">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="900a6-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



