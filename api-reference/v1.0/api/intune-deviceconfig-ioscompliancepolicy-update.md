---
title: 更新 iosCompliancePolicy
description: 更新 iosCompliancePolicy 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 27751a2726594029b6b856331ec2f5e9e46d529f
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52753879"
---
# <a name="update-ioscompliancepolicy"></a><span data-ttu-id="3d471-103">更新 iosCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="3d471-103">Update iosCompliancePolicy</span></span>

<span data-ttu-id="3d471-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3d471-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3d471-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="3d471-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3d471-106">更新 [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="3d471-106">Update the properties of a [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3d471-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="3d471-107">Prerequisites</span></span>
<span data-ttu-id="3d471-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="3d471-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3d471-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="3d471-110">Permission type</span></span>|<span data-ttu-id="3d471-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="3d471-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3d471-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3d471-112">Delegated (work or school account)</span></span>|<span data-ttu-id="3d471-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3d471-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="3d471-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3d471-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3d471-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="3d471-115">Not supported.</span></span>|
|<span data-ttu-id="3d471-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="3d471-116">Application</span></span>|<span data-ttu-id="3d471-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3d471-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3d471-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3d471-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="3d471-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="3d471-119">Request headers</span></span>
|<span data-ttu-id="3d471-120">标头</span><span class="sxs-lookup"><span data-stu-id="3d471-120">Header</span></span>|<span data-ttu-id="3d471-121">值</span><span class="sxs-lookup"><span data-stu-id="3d471-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3d471-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="3d471-122">Authorization</span></span>|<span data-ttu-id="3d471-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="3d471-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3d471-124">接受</span><span class="sxs-lookup"><span data-stu-id="3d471-124">Accept</span></span>|<span data-ttu-id="3d471-125">application/json</span><span class="sxs-lookup"><span data-stu-id="3d471-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3d471-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="3d471-126">Request body</span></span>
<span data-ttu-id="3d471-127">在请求正文中，提供 [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3d471-127">In the request body, supply a JSON representation for the [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) object.</span></span>

<span data-ttu-id="3d471-128">下表显示了创建 [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="3d471-128">The following table shows the properties that are required when you create the [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md).</span></span>

|<span data-ttu-id="3d471-129">属性</span><span class="sxs-lookup"><span data-stu-id="3d471-129">Property</span></span>|<span data-ttu-id="3d471-130">类型</span><span class="sxs-lookup"><span data-stu-id="3d471-130">Type</span></span>|<span data-ttu-id="3d471-131">说明</span><span class="sxs-lookup"><span data-stu-id="3d471-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3d471-132">id</span><span class="sxs-lookup"><span data-stu-id="3d471-132">id</span></span>|<span data-ttu-id="3d471-133">String</span><span class="sxs-lookup"><span data-stu-id="3d471-133">String</span></span>|<span data-ttu-id="3d471-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="3d471-134">Key of the entity.</span></span> <span data-ttu-id="3d471-135">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="3d471-135">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="3d471-136">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3d471-136">createdDateTime</span></span>|<span data-ttu-id="3d471-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3d471-137">DateTimeOffset</span></span>|<span data-ttu-id="3d471-138">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="3d471-138">DateTime the object was created.</span></span> <span data-ttu-id="3d471-139">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="3d471-139">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="3d471-140">说明</span><span class="sxs-lookup"><span data-stu-id="3d471-140">description</span></span>|<span data-ttu-id="3d471-141">String</span><span class="sxs-lookup"><span data-stu-id="3d471-141">String</span></span>|<span data-ttu-id="3d471-142">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="3d471-142">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="3d471-143">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="3d471-143">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="3d471-144">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3d471-144">lastModifiedDateTime</span></span>|<span data-ttu-id="3d471-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3d471-145">DateTimeOffset</span></span>|<span data-ttu-id="3d471-146">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="3d471-146">DateTime the object was last modified.</span></span> <span data-ttu-id="3d471-147">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="3d471-147">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="3d471-148">displayName</span><span class="sxs-lookup"><span data-stu-id="3d471-148">displayName</span></span>|<span data-ttu-id="3d471-149">String</span><span class="sxs-lookup"><span data-stu-id="3d471-149">String</span></span>|<span data-ttu-id="3d471-150">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="3d471-150">Admin provided name of the device configuration.</span></span> <span data-ttu-id="3d471-151">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="3d471-151">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="3d471-152">version</span><span class="sxs-lookup"><span data-stu-id="3d471-152">version</span></span>|<span data-ttu-id="3d471-153">Int32</span><span class="sxs-lookup"><span data-stu-id="3d471-153">Int32</span></span>|<span data-ttu-id="3d471-154">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="3d471-154">Version of the device configuration.</span></span> <span data-ttu-id="3d471-155">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="3d471-155">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="3d471-156">passcodeBlockSimple</span><span class="sxs-lookup"><span data-stu-id="3d471-156">passcodeBlockSimple</span></span>|<span data-ttu-id="3d471-157">Boolean</span><span class="sxs-lookup"><span data-stu-id="3d471-157">Boolean</span></span>|<span data-ttu-id="3d471-158">指示是否阻止简单密码。</span><span class="sxs-lookup"><span data-stu-id="3d471-158">Indicates whether or not to block simple passcodes.</span></span>|
|<span data-ttu-id="3d471-159">passcodeExpirationDays</span><span class="sxs-lookup"><span data-stu-id="3d471-159">passcodeExpirationDays</span></span>|<span data-ttu-id="3d471-160">Int32</span><span class="sxs-lookup"><span data-stu-id="3d471-160">Int32</span></span>|<span data-ttu-id="3d471-161">密码过期前的天数。</span><span class="sxs-lookup"><span data-stu-id="3d471-161">Number of days before the passcode expires.</span></span> <span data-ttu-id="3d471-162">有效值为 1 至 65535</span><span class="sxs-lookup"><span data-stu-id="3d471-162">Valid values 1 to 65535</span></span>|
|<span data-ttu-id="3d471-163">passcodeMinimumLength</span><span class="sxs-lookup"><span data-stu-id="3d471-163">passcodeMinimumLength</span></span>|<span data-ttu-id="3d471-164">Int32</span><span class="sxs-lookup"><span data-stu-id="3d471-164">Int32</span></span>|<span data-ttu-id="3d471-165">密码的最小长度。</span><span class="sxs-lookup"><span data-stu-id="3d471-165">Minimum length of passcode.</span></span> <span data-ttu-id="3d471-166">有效值为 4 至 14</span><span class="sxs-lookup"><span data-stu-id="3d471-166">Valid values 4 to 14</span></span>|
|<span data-ttu-id="3d471-167">passcodeMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="3d471-167">passcodeMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="3d471-168">Int32</span><span class="sxs-lookup"><span data-stu-id="3d471-168">Int32</span></span>|<span data-ttu-id="3d471-169">在需要密码之前不活动的分钟数。</span><span class="sxs-lookup"><span data-stu-id="3d471-169">Minutes of inactivity before a passcode is required.</span></span>|
|<span data-ttu-id="3d471-170">passcodePreviousPasscodeBlockCount</span><span class="sxs-lookup"><span data-stu-id="3d471-170">passcodePreviousPasscodeBlockCount</span></span>|<span data-ttu-id="3d471-171">Int32</span><span class="sxs-lookup"><span data-stu-id="3d471-171">Int32</span></span>|<span data-ttu-id="3d471-172">要阻止的以前密码的数量。</span><span class="sxs-lookup"><span data-stu-id="3d471-172">Number of previous passcodes to block.</span></span> <span data-ttu-id="3d471-173">有效值为 1 至 24</span><span class="sxs-lookup"><span data-stu-id="3d471-173">Valid values 1 to 24</span></span>|
|<span data-ttu-id="3d471-174">passcodeMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="3d471-174">passcodeMinimumCharacterSetCount</span></span>|<span data-ttu-id="3d471-175">Int32</span><span class="sxs-lookup"><span data-stu-id="3d471-175">Int32</span></span>|<span data-ttu-id="3d471-176">密码中必需的字符集数。</span><span class="sxs-lookup"><span data-stu-id="3d471-176">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="3d471-177">passcodeRequiredType</span><span class="sxs-lookup"><span data-stu-id="3d471-177">passcodeRequiredType</span></span>|[<span data-ttu-id="3d471-178">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="3d471-178">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="3d471-179">必需的密码类型。</span><span class="sxs-lookup"><span data-stu-id="3d471-179">The required passcode type.</span></span> <span data-ttu-id="3d471-180">可取值为：`deviceDefault`、`alphanumeric`、`numeric`。</span><span class="sxs-lookup"><span data-stu-id="3d471-180">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="3d471-181">passcodeRequired</span><span class="sxs-lookup"><span data-stu-id="3d471-181">passcodeRequired</span></span>|<span data-ttu-id="3d471-182">Boolean</span><span class="sxs-lookup"><span data-stu-id="3d471-182">Boolean</span></span>|<span data-ttu-id="3d471-183">指示是否需要密码。</span><span class="sxs-lookup"><span data-stu-id="3d471-183">Indicates whether or not to require a passcode.</span></span>|
|<span data-ttu-id="3d471-184">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="3d471-184">osMinimumVersion</span></span>|<span data-ttu-id="3d471-185">String</span><span class="sxs-lookup"><span data-stu-id="3d471-185">String</span></span>|<span data-ttu-id="3d471-186">最低 IOS 版本。</span><span class="sxs-lookup"><span data-stu-id="3d471-186">Minimum IOS version.</span></span>|
|<span data-ttu-id="3d471-187">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="3d471-187">osMaximumVersion</span></span>|<span data-ttu-id="3d471-188">String</span><span class="sxs-lookup"><span data-stu-id="3d471-188">String</span></span>|<span data-ttu-id="3d471-189">最高 IOS 版本。</span><span class="sxs-lookup"><span data-stu-id="3d471-189">Maximum IOS version.</span></span>|
|<span data-ttu-id="3d471-190">securityBlockJailbrokenDevices</span><span class="sxs-lookup"><span data-stu-id="3d471-190">securityBlockJailbrokenDevices</span></span>|<span data-ttu-id="3d471-191">Boolean</span><span class="sxs-lookup"><span data-stu-id="3d471-191">Boolean</span></span>|<span data-ttu-id="3d471-192">设备不得越狱或取得 root 权限。</span><span class="sxs-lookup"><span data-stu-id="3d471-192">Devices must not be jailbroken or rooted.</span></span>|
|<span data-ttu-id="3d471-193">deviceThreatProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="3d471-193">deviceThreatProtectionEnabled</span></span>|<span data-ttu-id="3d471-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="3d471-194">Boolean</span></span>|<span data-ttu-id="3d471-195">要求设备已启用设备威胁防护。</span><span class="sxs-lookup"><span data-stu-id="3d471-195">Require that devices have enabled device threat protection .</span></span>|
|<span data-ttu-id="3d471-196">deviceThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="3d471-196">deviceThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="3d471-197">deviceThreatProtectionLevel</span><span class="sxs-lookup"><span data-stu-id="3d471-197">deviceThreatProtectionLevel</span></span>](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|<span data-ttu-id="3d471-198">要求移动威胁防护最低风险级别来报告不符合情况。</span><span class="sxs-lookup"><span data-stu-id="3d471-198">Require Mobile Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="3d471-199">可取值为：`unavailable`、`secured`、`low`、`medium`、`high`、`notSet`。</span><span class="sxs-lookup"><span data-stu-id="3d471-199">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="3d471-200">managedEmailProfileRequired</span><span class="sxs-lookup"><span data-stu-id="3d471-200">managedEmailProfileRequired</span></span>|<span data-ttu-id="3d471-201">Boolean</span><span class="sxs-lookup"><span data-stu-id="3d471-201">Boolean</span></span>|<span data-ttu-id="3d471-202">指示是否需要托管电子邮件配置文件。</span><span class="sxs-lookup"><span data-stu-id="3d471-202">Indicates whether or not to require a managed email profile.</span></span>|



## <a name="response"></a><span data-ttu-id="3d471-203">响应</span><span class="sxs-lookup"><span data-stu-id="3d471-203">Response</span></span>
<span data-ttu-id="3d471-204">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和更新的 [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="3d471-204">If successful, this method returns a `200 OK` response code and an updated [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3d471-205">示例</span><span class="sxs-lookup"><span data-stu-id="3d471-205">Example</span></span>

### <a name="request"></a><span data-ttu-id="3d471-206">请求</span><span class="sxs-lookup"><span data-stu-id="3d471-206">Request</span></span>
<span data-ttu-id="3d471-207">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="3d471-207">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
Content-type: application/json
Content-length: 745

{
  "@odata.type": "#microsoft.graph.iosCompliancePolicy",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "passcodeBlockSimple": true,
  "passcodeExpirationDays": 6,
  "passcodeMinimumLength": 5,
  "passcodeMinutesOfInactivityBeforeLock": 5,
  "passcodePreviousPasscodeBlockCount": 2,
  "passcodeMinimumCharacterSetCount": 0,
  "passcodeRequiredType": "alphanumeric",
  "passcodeRequired": true,
  "osMinimumVersion": "Os Minimum Version value",
  "osMaximumVersion": "Os Maximum Version value",
  "securityBlockJailbrokenDevices": true,
  "deviceThreatProtectionEnabled": true,
  "deviceThreatProtectionRequiredSecurityLevel": "secured",
  "managedEmailProfileRequired": true
}
```

### <a name="response"></a><span data-ttu-id="3d471-208">响应</span><span class="sxs-lookup"><span data-stu-id="3d471-208">Response</span></span>
<span data-ttu-id="3d471-p113">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="3d471-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 917

{
  "@odata.type": "#microsoft.graph.iosCompliancePolicy",
  "id": "4f501351-1351-4f50-5113-504f5113504f",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "version": 7,
  "passcodeBlockSimple": true,
  "passcodeExpirationDays": 6,
  "passcodeMinimumLength": 5,
  "passcodeMinutesOfInactivityBeforeLock": 5,
  "passcodePreviousPasscodeBlockCount": 2,
  "passcodeMinimumCharacterSetCount": 0,
  "passcodeRequiredType": "alphanumeric",
  "passcodeRequired": true,
  "osMinimumVersion": "Os Minimum Version value",
  "osMaximumVersion": "Os Maximum Version value",
  "securityBlockJailbrokenDevices": true,
  "deviceThreatProtectionEnabled": true,
  "deviceThreatProtectionRequiredSecurityLevel": "secured",
  "managedEmailProfileRequired": true
}
```




