---
title: 更新 iosCompliancePolicy
description: 更新 iosCompliancePolicy 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: f292e991cdfb32a26538eb703eae9fd710ef95d4
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48066738"
---
# <a name="update-ioscompliancepolicy"></a><span data-ttu-id="5536f-103">更新 iosCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="5536f-103">Update iosCompliancePolicy</span></span>

<span data-ttu-id="5536f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5536f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5536f-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="5536f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5536f-106">更新 [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="5536f-106">Update the properties of a [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5536f-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="5536f-107">Prerequisites</span></span>
<span data-ttu-id="5536f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="5536f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5536f-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="5536f-110">Permission type</span></span>|<span data-ttu-id="5536f-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="5536f-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5536f-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5536f-112">Delegated (work or school account)</span></span>|<span data-ttu-id="5536f-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5536f-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="5536f-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5536f-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5536f-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="5536f-115">Not supported.</span></span>|
|<span data-ttu-id="5536f-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="5536f-116">Application</span></span>|<span data-ttu-id="5536f-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="5536f-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5536f-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5536f-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="5536f-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="5536f-119">Request headers</span></span>
|<span data-ttu-id="5536f-120">标头</span><span class="sxs-lookup"><span data-stu-id="5536f-120">Header</span></span>|<span data-ttu-id="5536f-121">值</span><span class="sxs-lookup"><span data-stu-id="5536f-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5536f-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="5536f-122">Authorization</span></span>|<span data-ttu-id="5536f-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="5536f-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5536f-124">接受</span><span class="sxs-lookup"><span data-stu-id="5536f-124">Accept</span></span>|<span data-ttu-id="5536f-125">application/json</span><span class="sxs-lookup"><span data-stu-id="5536f-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5536f-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="5536f-126">Request body</span></span>
<span data-ttu-id="5536f-127">在请求正文中，提供 [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5536f-127">In the request body, supply a JSON representation for the [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) object.</span></span>

<span data-ttu-id="5536f-128">下表显示了创建 [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="5536f-128">The following table shows the properties that are required when you create the [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md).</span></span>

|<span data-ttu-id="5536f-129">属性</span><span class="sxs-lookup"><span data-stu-id="5536f-129">Property</span></span>|<span data-ttu-id="5536f-130">类型</span><span class="sxs-lookup"><span data-stu-id="5536f-130">Type</span></span>|<span data-ttu-id="5536f-131">说明</span><span class="sxs-lookup"><span data-stu-id="5536f-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5536f-132">id</span><span class="sxs-lookup"><span data-stu-id="5536f-132">id</span></span>|<span data-ttu-id="5536f-133">String</span><span class="sxs-lookup"><span data-stu-id="5536f-133">String</span></span>|<span data-ttu-id="5536f-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="5536f-134">Key of the entity.</span></span> <span data-ttu-id="5536f-135">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="5536f-135">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="5536f-136">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="5536f-136">createdDateTime</span></span>|<span data-ttu-id="5536f-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5536f-137">DateTimeOffset</span></span>|<span data-ttu-id="5536f-138">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="5536f-138">DateTime the object was created.</span></span> <span data-ttu-id="5536f-139">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="5536f-139">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="5536f-140">description</span><span class="sxs-lookup"><span data-stu-id="5536f-140">description</span></span>|<span data-ttu-id="5536f-141">String</span><span class="sxs-lookup"><span data-stu-id="5536f-141">String</span></span>|<span data-ttu-id="5536f-142">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="5536f-142">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="5536f-143">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="5536f-143">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="5536f-144">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="5536f-144">lastModifiedDateTime</span></span>|<span data-ttu-id="5536f-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5536f-145">DateTimeOffset</span></span>|<span data-ttu-id="5536f-146">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="5536f-146">DateTime the object was last modified.</span></span> <span data-ttu-id="5536f-147">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="5536f-147">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="5536f-148">displayName</span><span class="sxs-lookup"><span data-stu-id="5536f-148">displayName</span></span>|<span data-ttu-id="5536f-149">String</span><span class="sxs-lookup"><span data-stu-id="5536f-149">String</span></span>|<span data-ttu-id="5536f-150">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="5536f-150">Admin provided name of the device configuration.</span></span> <span data-ttu-id="5536f-151">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="5536f-151">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="5536f-152">version</span><span class="sxs-lookup"><span data-stu-id="5536f-152">version</span></span>|<span data-ttu-id="5536f-153">Int32</span><span class="sxs-lookup"><span data-stu-id="5536f-153">Int32</span></span>|<span data-ttu-id="5536f-154">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="5536f-154">Version of the device configuration.</span></span> <span data-ttu-id="5536f-155">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="5536f-155">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="5536f-156">passcodeBlockSimple</span><span class="sxs-lookup"><span data-stu-id="5536f-156">passcodeBlockSimple</span></span>|<span data-ttu-id="5536f-157">Boolean</span><span class="sxs-lookup"><span data-stu-id="5536f-157">Boolean</span></span>|<span data-ttu-id="5536f-158">指示是否阻止简单密码。</span><span class="sxs-lookup"><span data-stu-id="5536f-158">Indicates whether or not to block simple passcodes.</span></span>|
|<span data-ttu-id="5536f-159">passcodeExpirationDays</span><span class="sxs-lookup"><span data-stu-id="5536f-159">passcodeExpirationDays</span></span>|<span data-ttu-id="5536f-160">Int32</span><span class="sxs-lookup"><span data-stu-id="5536f-160">Int32</span></span>|<span data-ttu-id="5536f-161">密码过期前的天数。</span><span class="sxs-lookup"><span data-stu-id="5536f-161">Number of days before the passcode expires.</span></span> <span data-ttu-id="5536f-162">有效值为 1 至 65535</span><span class="sxs-lookup"><span data-stu-id="5536f-162">Valid values 1 to 65535</span></span>|
|<span data-ttu-id="5536f-163">passcodeMinimumLength</span><span class="sxs-lookup"><span data-stu-id="5536f-163">passcodeMinimumLength</span></span>|<span data-ttu-id="5536f-164">Int32</span><span class="sxs-lookup"><span data-stu-id="5536f-164">Int32</span></span>|<span data-ttu-id="5536f-165">密码的最小长度。</span><span class="sxs-lookup"><span data-stu-id="5536f-165">Minimum length of passcode.</span></span> <span data-ttu-id="5536f-166">有效值为 4 至 14</span><span class="sxs-lookup"><span data-stu-id="5536f-166">Valid values 4 to 14</span></span>|
|<span data-ttu-id="5536f-167">passcodeMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="5536f-167">passcodeMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="5536f-168">Int32</span><span class="sxs-lookup"><span data-stu-id="5536f-168">Int32</span></span>|<span data-ttu-id="5536f-169">在需要密码之前不活动的分钟数。</span><span class="sxs-lookup"><span data-stu-id="5536f-169">Minutes of inactivity before a passcode is required.</span></span>|
|<span data-ttu-id="5536f-170">passcodePreviousPasscodeBlockCount</span><span class="sxs-lookup"><span data-stu-id="5536f-170">passcodePreviousPasscodeBlockCount</span></span>|<span data-ttu-id="5536f-171">Int32</span><span class="sxs-lookup"><span data-stu-id="5536f-171">Int32</span></span>|<span data-ttu-id="5536f-172">要阻止的以前密码的数量。</span><span class="sxs-lookup"><span data-stu-id="5536f-172">Number of previous passcodes to block.</span></span> <span data-ttu-id="5536f-173">有效值为 1 至 24</span><span class="sxs-lookup"><span data-stu-id="5536f-173">Valid values 1 to 24</span></span>|
|<span data-ttu-id="5536f-174">passcodeMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="5536f-174">passcodeMinimumCharacterSetCount</span></span>|<span data-ttu-id="5536f-175">Int32</span><span class="sxs-lookup"><span data-stu-id="5536f-175">Int32</span></span>|<span data-ttu-id="5536f-176">密码中必需的字符集数。</span><span class="sxs-lookup"><span data-stu-id="5536f-176">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="5536f-177">passcodeRequiredType</span><span class="sxs-lookup"><span data-stu-id="5536f-177">passcodeRequiredType</span></span>|[<span data-ttu-id="5536f-178">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="5536f-178">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="5536f-179">必需的密码类型。</span><span class="sxs-lookup"><span data-stu-id="5536f-179">The required passcode type.</span></span> <span data-ttu-id="5536f-180">可取值为：`deviceDefault`、`alphanumeric`、`numeric`。</span><span class="sxs-lookup"><span data-stu-id="5536f-180">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="5536f-181">passcodeRequired</span><span class="sxs-lookup"><span data-stu-id="5536f-181">passcodeRequired</span></span>|<span data-ttu-id="5536f-182">Boolean</span><span class="sxs-lookup"><span data-stu-id="5536f-182">Boolean</span></span>|<span data-ttu-id="5536f-183">指示是否需要密码。</span><span class="sxs-lookup"><span data-stu-id="5536f-183">Indicates whether or not to require a passcode.</span></span>|
|<span data-ttu-id="5536f-184">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="5536f-184">osMinimumVersion</span></span>|<span data-ttu-id="5536f-185">String</span><span class="sxs-lookup"><span data-stu-id="5536f-185">String</span></span>|<span data-ttu-id="5536f-186">最低 IOS 版本。</span><span class="sxs-lookup"><span data-stu-id="5536f-186">Minimum IOS version.</span></span>|
|<span data-ttu-id="5536f-187">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="5536f-187">osMaximumVersion</span></span>|<span data-ttu-id="5536f-188">String</span><span class="sxs-lookup"><span data-stu-id="5536f-188">String</span></span>|<span data-ttu-id="5536f-189">最高 IOS 版本。</span><span class="sxs-lookup"><span data-stu-id="5536f-189">Maximum IOS version.</span></span>|
|<span data-ttu-id="5536f-190">securityBlockJailbrokenDevices</span><span class="sxs-lookup"><span data-stu-id="5536f-190">securityBlockJailbrokenDevices</span></span>|<span data-ttu-id="5536f-191">Boolean</span><span class="sxs-lookup"><span data-stu-id="5536f-191">Boolean</span></span>|<span data-ttu-id="5536f-192">设备不得越狱或取得 root 权限。</span><span class="sxs-lookup"><span data-stu-id="5536f-192">Devices must not be jailbroken or rooted.</span></span>|
|<span data-ttu-id="5536f-193">deviceThreatProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="5536f-193">deviceThreatProtectionEnabled</span></span>|<span data-ttu-id="5536f-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="5536f-194">Boolean</span></span>|<span data-ttu-id="5536f-195">要求设备已启用设备威胁防护。</span><span class="sxs-lookup"><span data-stu-id="5536f-195">Require that devices have enabled device threat protection .</span></span>|
|<span data-ttu-id="5536f-196">deviceThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="5536f-196">deviceThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="5536f-197">deviceThreatProtectionLevel</span><span class="sxs-lookup"><span data-stu-id="5536f-197">deviceThreatProtectionLevel</span></span>](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|<span data-ttu-id="5536f-198">要求移动威胁防护最低风险级别来报告不符合情况。</span><span class="sxs-lookup"><span data-stu-id="5536f-198">Require Mobile Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="5536f-199">可取值为：`unavailable`、`secured`、`low`、`medium`、`high`、`notSet`。</span><span class="sxs-lookup"><span data-stu-id="5536f-199">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="5536f-200">managedEmailProfileRequired</span><span class="sxs-lookup"><span data-stu-id="5536f-200">managedEmailProfileRequired</span></span>|<span data-ttu-id="5536f-201">Boolean</span><span class="sxs-lookup"><span data-stu-id="5536f-201">Boolean</span></span>|<span data-ttu-id="5536f-202">指示是否需要托管电子邮件配置文件。</span><span class="sxs-lookup"><span data-stu-id="5536f-202">Indicates whether or not to require a managed email profile.</span></span>|



## <a name="response"></a><span data-ttu-id="5536f-203">响应</span><span class="sxs-lookup"><span data-stu-id="5536f-203">Response</span></span>
<span data-ttu-id="5536f-204">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和更新的 [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="5536f-204">If successful, this method returns a `200 OK` response code and an updated [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5536f-205">示例</span><span class="sxs-lookup"><span data-stu-id="5536f-205">Example</span></span>

### <a name="request"></a><span data-ttu-id="5536f-206">请求</span><span class="sxs-lookup"><span data-stu-id="5536f-206">Request</span></span>
<span data-ttu-id="5536f-207">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="5536f-207">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="5536f-208">响应</span><span class="sxs-lookup"><span data-stu-id="5536f-208">Response</span></span>
<span data-ttu-id="5536f-p113">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="5536f-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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









