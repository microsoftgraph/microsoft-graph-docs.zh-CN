---
title: 更新 windows10CompliancePolicy
description: 更新 windows10CompliancePolicy 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: b63f2665a081263deae42cd6b66e370a90ee61d9
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52760564"
---
# <a name="update-windows10compliancepolicy"></a><span data-ttu-id="8ab95-103">更新 windows10CompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="8ab95-103">Update windows10CompliancePolicy</span></span>

<span data-ttu-id="8ab95-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8ab95-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8ab95-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="8ab95-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8ab95-106">更新 [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="8ab95-106">Update the properties of a [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8ab95-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="8ab95-107">Prerequisites</span></span>
<span data-ttu-id="8ab95-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8ab95-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8ab95-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="8ab95-110">Permission type</span></span>|<span data-ttu-id="8ab95-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="8ab95-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8ab95-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8ab95-112">Delegated (work or school account)</span></span>|<span data-ttu-id="8ab95-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8ab95-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="8ab95-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8ab95-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8ab95-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="8ab95-115">Not supported.</span></span>|
|<span data-ttu-id="8ab95-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="8ab95-116">Application</span></span>|<span data-ttu-id="8ab95-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8ab95-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8ab95-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8ab95-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="8ab95-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="8ab95-119">Request headers</span></span>
|<span data-ttu-id="8ab95-120">标头</span><span class="sxs-lookup"><span data-stu-id="8ab95-120">Header</span></span>|<span data-ttu-id="8ab95-121">值</span><span class="sxs-lookup"><span data-stu-id="8ab95-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8ab95-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="8ab95-122">Authorization</span></span>|<span data-ttu-id="8ab95-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="8ab95-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8ab95-124">接受</span><span class="sxs-lookup"><span data-stu-id="8ab95-124">Accept</span></span>|<span data-ttu-id="8ab95-125">application/json</span><span class="sxs-lookup"><span data-stu-id="8ab95-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8ab95-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="8ab95-126">Request body</span></span>
<span data-ttu-id="8ab95-127">在请求正文中，提供 [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8ab95-127">In the request body, supply a JSON representation for the [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) object.</span></span>

<span data-ttu-id="8ab95-128">下表显示创建 [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="8ab95-128">The following table shows the properties that are required when you create the [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md).</span></span>

|<span data-ttu-id="8ab95-129">属性</span><span class="sxs-lookup"><span data-stu-id="8ab95-129">Property</span></span>|<span data-ttu-id="8ab95-130">类型</span><span class="sxs-lookup"><span data-stu-id="8ab95-130">Type</span></span>|<span data-ttu-id="8ab95-131">说明</span><span class="sxs-lookup"><span data-stu-id="8ab95-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8ab95-132">id</span><span class="sxs-lookup"><span data-stu-id="8ab95-132">id</span></span>|<span data-ttu-id="8ab95-133">String</span><span class="sxs-lookup"><span data-stu-id="8ab95-133">String</span></span>|<span data-ttu-id="8ab95-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="8ab95-134">Key of the entity.</span></span> <span data-ttu-id="8ab95-135">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="8ab95-135">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="8ab95-136">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8ab95-136">createdDateTime</span></span>|<span data-ttu-id="8ab95-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8ab95-137">DateTimeOffset</span></span>|<span data-ttu-id="8ab95-138">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="8ab95-138">DateTime the object was created.</span></span> <span data-ttu-id="8ab95-139">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="8ab95-139">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="8ab95-140">description</span><span class="sxs-lookup"><span data-stu-id="8ab95-140">description</span></span>|<span data-ttu-id="8ab95-141">String</span><span class="sxs-lookup"><span data-stu-id="8ab95-141">String</span></span>|<span data-ttu-id="8ab95-142">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="8ab95-142">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="8ab95-143">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="8ab95-143">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="8ab95-144">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8ab95-144">lastModifiedDateTime</span></span>|<span data-ttu-id="8ab95-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8ab95-145">DateTimeOffset</span></span>|<span data-ttu-id="8ab95-146">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="8ab95-146">DateTime the object was last modified.</span></span> <span data-ttu-id="8ab95-147">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="8ab95-147">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="8ab95-148">displayName</span><span class="sxs-lookup"><span data-stu-id="8ab95-148">displayName</span></span>|<span data-ttu-id="8ab95-149">String</span><span class="sxs-lookup"><span data-stu-id="8ab95-149">String</span></span>|<span data-ttu-id="8ab95-150">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="8ab95-150">Admin provided name of the device configuration.</span></span> <span data-ttu-id="8ab95-151">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="8ab95-151">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="8ab95-152">version</span><span class="sxs-lookup"><span data-stu-id="8ab95-152">version</span></span>|<span data-ttu-id="8ab95-153">Int32</span><span class="sxs-lookup"><span data-stu-id="8ab95-153">Int32</span></span>|<span data-ttu-id="8ab95-154">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="8ab95-154">Version of the device configuration.</span></span> <span data-ttu-id="8ab95-155">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="8ab95-155">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="8ab95-156">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="8ab95-156">passwordRequired</span></span>|<span data-ttu-id="8ab95-157">Boolean</span><span class="sxs-lookup"><span data-stu-id="8ab95-157">Boolean</span></span>|<span data-ttu-id="8ab95-158">需要密码才可解锁 Windows 设备。</span><span class="sxs-lookup"><span data-stu-id="8ab95-158">Require a password to unlock Windows device.</span></span>|
|<span data-ttu-id="8ab95-159">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="8ab95-159">passwordBlockSimple</span></span>|<span data-ttu-id="8ab95-160">Boolean</span><span class="sxs-lookup"><span data-stu-id="8ab95-160">Boolean</span></span>|<span data-ttu-id="8ab95-161">指示是否阻止简单密码。</span><span class="sxs-lookup"><span data-stu-id="8ab95-161">Indicates whether or not to block simple password.</span></span>|
|<span data-ttu-id="8ab95-162">passwordRequiredToUnlockFromIdle</span><span class="sxs-lookup"><span data-stu-id="8ab95-162">passwordRequiredToUnlockFromIdle</span></span>|<span data-ttu-id="8ab95-163">Boolean</span><span class="sxs-lookup"><span data-stu-id="8ab95-163">Boolean</span></span>|<span data-ttu-id="8ab95-164">需要密码才可解锁空闲设备。</span><span class="sxs-lookup"><span data-stu-id="8ab95-164">Require a password to unlock an idle device.</span></span>|
|<span data-ttu-id="8ab95-165">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="8ab95-165">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="8ab95-166">Int32</span><span class="sxs-lookup"><span data-stu-id="8ab95-166">Int32</span></span>|<span data-ttu-id="8ab95-167">在需要密码之前不活动的分钟数。</span><span class="sxs-lookup"><span data-stu-id="8ab95-167">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="8ab95-168">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="8ab95-168">passwordExpirationDays</span></span>|<span data-ttu-id="8ab95-169">Int32</span><span class="sxs-lookup"><span data-stu-id="8ab95-169">Int32</span></span>|<span data-ttu-id="8ab95-170">密码过期天数。</span><span class="sxs-lookup"><span data-stu-id="8ab95-170">The password expiration in days.</span></span>|
|<span data-ttu-id="8ab95-171">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="8ab95-171">passwordMinimumLength</span></span>|<span data-ttu-id="8ab95-172">Int32</span><span class="sxs-lookup"><span data-stu-id="8ab95-172">Int32</span></span>|<span data-ttu-id="8ab95-173">密码最短长度。</span><span class="sxs-lookup"><span data-stu-id="8ab95-173">The minimum password length.</span></span>|
|<span data-ttu-id="8ab95-174">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="8ab95-174">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="8ab95-175">Int32</span><span class="sxs-lookup"><span data-stu-id="8ab95-175">Int32</span></span>|<span data-ttu-id="8ab95-176">密码中必需的字符集数。</span><span class="sxs-lookup"><span data-stu-id="8ab95-176">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="8ab95-177">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="8ab95-177">passwordRequiredType</span></span>|[<span data-ttu-id="8ab95-178">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="8ab95-178">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="8ab95-179">必需的密码类型。</span><span class="sxs-lookup"><span data-stu-id="8ab95-179">The required password type.</span></span> <span data-ttu-id="8ab95-180">可取值为：`deviceDefault`、`alphanumeric`、`numeric`。</span><span class="sxs-lookup"><span data-stu-id="8ab95-180">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="8ab95-181">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="8ab95-181">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="8ab95-182">Int32</span><span class="sxs-lookup"><span data-stu-id="8ab95-182">Int32</span></span>|<span data-ttu-id="8ab95-183">防止重复使用的先前密码的数量。</span><span class="sxs-lookup"><span data-stu-id="8ab95-183">The number of previous passwords to prevent re-use of.</span></span>|
|<span data-ttu-id="8ab95-184">requireHealthyDeviceReport</span><span class="sxs-lookup"><span data-stu-id="8ab95-184">requireHealthyDeviceReport</span></span>|<span data-ttu-id="8ab95-185">Boolean</span><span class="sxs-lookup"><span data-stu-id="8ab95-185">Boolean</span></span>|<span data-ttu-id="8ab95-186">要求设备由 Windows 设备运行状况证明报告为正常。</span><span class="sxs-lookup"><span data-stu-id="8ab95-186">Require devices to be reported as healthy by Windows Device Health Attestation.</span></span>|
|<span data-ttu-id="8ab95-187">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="8ab95-187">osMinimumVersion</span></span>|<span data-ttu-id="8ab95-188">String</span><span class="sxs-lookup"><span data-stu-id="8ab95-188">String</span></span>|<span data-ttu-id="8ab95-189">最低 Windows 10 版本。</span><span class="sxs-lookup"><span data-stu-id="8ab95-189">Minimum Windows 10 version.</span></span>|
|<span data-ttu-id="8ab95-190">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="8ab95-190">osMaximumVersion</span></span>|<span data-ttu-id="8ab95-191">String</span><span class="sxs-lookup"><span data-stu-id="8ab95-191">String</span></span>|<span data-ttu-id="8ab95-192">最高 Windows 10 版本。</span><span class="sxs-lookup"><span data-stu-id="8ab95-192">Maximum Windows 10 version.</span></span>|
|<span data-ttu-id="8ab95-193">mobileOsMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="8ab95-193">mobileOsMinimumVersion</span></span>|<span data-ttu-id="8ab95-194">String</span><span class="sxs-lookup"><span data-stu-id="8ab95-194">String</span></span>|<span data-ttu-id="8ab95-195">最低 Windows Phone 版本。</span><span class="sxs-lookup"><span data-stu-id="8ab95-195">Minimum Windows Phone version.</span></span>|
|<span data-ttu-id="8ab95-196">mobileOsMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="8ab95-196">mobileOsMaximumVersion</span></span>|<span data-ttu-id="8ab95-197">String</span><span class="sxs-lookup"><span data-stu-id="8ab95-197">String</span></span>|<span data-ttu-id="8ab95-198">最高 Windows Phone 版本。</span><span class="sxs-lookup"><span data-stu-id="8ab95-198">Maximum Windows Phone version.</span></span>|
|<span data-ttu-id="8ab95-199">earlyLaunchAntiMalwareDriverEnabled</span><span class="sxs-lookup"><span data-stu-id="8ab95-199">earlyLaunchAntiMalwareDriverEnabled</span></span>|<span data-ttu-id="8ab95-200">Boolean</span><span class="sxs-lookup"><span data-stu-id="8ab95-200">Boolean</span></span>|<span data-ttu-id="8ab95-201">要求设备由 Windows 设备运行状况证明报告为正常 - 提前启动反恶意驱动程序已启用。</span><span class="sxs-lookup"><span data-stu-id="8ab95-201">Require devices to be reported as healthy by Windows Device Health Attestation - early launch antimalware driver is enabled.</span></span>|
|<span data-ttu-id="8ab95-202">bitLockerEnabled</span><span class="sxs-lookup"><span data-stu-id="8ab95-202">bitLockerEnabled</span></span>|<span data-ttu-id="8ab95-203">Boolean</span><span class="sxs-lookup"><span data-stu-id="8ab95-203">Boolean</span></span>|<span data-ttu-id="8ab95-204">要求设备由 Windows 设备运行状况证明报告为正常 - bit locker 已启用。</span><span class="sxs-lookup"><span data-stu-id="8ab95-204">Require devices to be reported healthy by Windows Device Health Attestation - bit locker is enabled</span></span>|
|<span data-ttu-id="8ab95-205">secureBootEnabled</span><span class="sxs-lookup"><span data-stu-id="8ab95-205">secureBootEnabled</span></span>|<span data-ttu-id="8ab95-206">Boolean</span><span class="sxs-lookup"><span data-stu-id="8ab95-206">Boolean</span></span>|<span data-ttu-id="8ab95-207">要求设备由 Windows 设备运行状况证明报告为正常 - 安全启动已启用。</span><span class="sxs-lookup"><span data-stu-id="8ab95-207">Require devices to be reported as healthy by Windows Device Health Attestation - secure boot is enabled.</span></span>|
|<span data-ttu-id="8ab95-208">codeIntegrityEnabled</span><span class="sxs-lookup"><span data-stu-id="8ab95-208">codeIntegrityEnabled</span></span>|<span data-ttu-id="8ab95-209">Boolean</span><span class="sxs-lookup"><span data-stu-id="8ab95-209">Boolean</span></span>|<span data-ttu-id="8ab95-210">要求设备由 Windows 设备运行状况证明报告为正常。</span><span class="sxs-lookup"><span data-stu-id="8ab95-210">Require devices to be reported as healthy by Windows Device Health Attestation.</span></span>|
|<span data-ttu-id="8ab95-211">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="8ab95-211">storageRequireEncryption</span></span>|<span data-ttu-id="8ab95-212">Boolean</span><span class="sxs-lookup"><span data-stu-id="8ab95-212">Boolean</span></span>|<span data-ttu-id="8ab95-213">要求对 Windows 设备加密。</span><span class="sxs-lookup"><span data-stu-id="8ab95-213">Require encryption on windows devices.</span></span>|



## <a name="response"></a><span data-ttu-id="8ab95-214">响应</span><span class="sxs-lookup"><span data-stu-id="8ab95-214">Response</span></span>
<span data-ttu-id="8ab95-215">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和更新的 [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="8ab95-215">If successful, this method returns a `200 OK` response code and an updated [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8ab95-216">示例</span><span class="sxs-lookup"><span data-stu-id="8ab95-216">Example</span></span>

### <a name="request"></a><span data-ttu-id="8ab95-217">请求</span><span class="sxs-lookup"><span data-stu-id="8ab95-217">Request</span></span>
<span data-ttu-id="8ab95-218">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="8ab95-218">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="8ab95-219">响应</span><span class="sxs-lookup"><span data-stu-id="8ab95-219">Response</span></span>
<span data-ttu-id="8ab95-p109">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="8ab95-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




