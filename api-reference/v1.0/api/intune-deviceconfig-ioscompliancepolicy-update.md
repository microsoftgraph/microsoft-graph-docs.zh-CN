---
title: 更新 iosCompliancePolicy
description: 更新 iosCompliancePolicy 对象的属性。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: acb29cd24faa95e0874c9ff0aa92f915489f8041
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/02/2019
ms.locfileid: "37368335"
---
# <a name="update-ioscompliancepolicy"></a><span data-ttu-id="9a260-103">更新 iosCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="9a260-103">Update iosCompliancePolicy</span></span>

> <span data-ttu-id="9a260-104">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="9a260-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9a260-105">更新 [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="9a260-105">Update the properties of a [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9a260-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="9a260-106">Prerequisites</span></span>
<span data-ttu-id="9a260-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9a260-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9a260-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="9a260-109">Permission type</span></span>|<span data-ttu-id="9a260-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="9a260-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9a260-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9a260-111">Delegated (work or school account)</span></span>|<span data-ttu-id="9a260-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9a260-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="9a260-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9a260-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9a260-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="9a260-114">Not supported.</span></span>|
|<span data-ttu-id="9a260-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="9a260-115">Application</span></span>|<span data-ttu-id="9a260-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="9a260-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9a260-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9a260-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="9a260-118">请求头</span><span class="sxs-lookup"><span data-stu-id="9a260-118">Request headers</span></span>
|<span data-ttu-id="9a260-119">标头</span><span class="sxs-lookup"><span data-stu-id="9a260-119">Header</span></span>|<span data-ttu-id="9a260-120">值</span><span class="sxs-lookup"><span data-stu-id="9a260-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9a260-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="9a260-121">Authorization</span></span>|<span data-ttu-id="9a260-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="9a260-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9a260-123">接受</span><span class="sxs-lookup"><span data-stu-id="9a260-123">Accept</span></span>|<span data-ttu-id="9a260-124">application/json</span><span class="sxs-lookup"><span data-stu-id="9a260-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9a260-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="9a260-125">Request body</span></span>
<span data-ttu-id="9a260-126">在请求正文中，提供 [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9a260-126">In the request body, supply a JSON representation for the [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) object.</span></span>

<span data-ttu-id="9a260-127">下表显示了创建 [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="9a260-127">The following table shows the properties that are required when you create the [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md).</span></span>

|<span data-ttu-id="9a260-128">属性</span><span class="sxs-lookup"><span data-stu-id="9a260-128">Property</span></span>|<span data-ttu-id="9a260-129">类型</span><span class="sxs-lookup"><span data-stu-id="9a260-129">Type</span></span>|<span data-ttu-id="9a260-130">说明</span><span class="sxs-lookup"><span data-stu-id="9a260-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9a260-131">id</span><span class="sxs-lookup"><span data-stu-id="9a260-131">id</span></span>|<span data-ttu-id="9a260-132">字符串</span><span class="sxs-lookup"><span data-stu-id="9a260-132">String</span></span>|<span data-ttu-id="9a260-133">实体的键。</span><span class="sxs-lookup"><span data-stu-id="9a260-133">Key of the entity.</span></span> <span data-ttu-id="9a260-134">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="9a260-134">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="9a260-135">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="9a260-135">createdDateTime</span></span>|<span data-ttu-id="9a260-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9a260-136">DateTimeOffset</span></span>|<span data-ttu-id="9a260-137">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="9a260-137">DateTime the object was created.</span></span> <span data-ttu-id="9a260-138">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="9a260-138">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="9a260-139">说明</span><span class="sxs-lookup"><span data-stu-id="9a260-139">description</span></span>|<span data-ttu-id="9a260-140">String</span><span class="sxs-lookup"><span data-stu-id="9a260-140">String</span></span>|<span data-ttu-id="9a260-141">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="9a260-141">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="9a260-142">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="9a260-142">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="9a260-143">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9a260-143">lastModifiedDateTime</span></span>|<span data-ttu-id="9a260-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9a260-144">DateTimeOffset</span></span>|<span data-ttu-id="9a260-145">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="9a260-145">DateTime the object was last modified.</span></span> <span data-ttu-id="9a260-146">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="9a260-146">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="9a260-147">displayName</span><span class="sxs-lookup"><span data-stu-id="9a260-147">displayName</span></span>|<span data-ttu-id="9a260-148">字符串</span><span class="sxs-lookup"><span data-stu-id="9a260-148">String</span></span>|<span data-ttu-id="9a260-149">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="9a260-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="9a260-150">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="9a260-150">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="9a260-151">version</span><span class="sxs-lookup"><span data-stu-id="9a260-151">version</span></span>|<span data-ttu-id="9a260-152">Int32</span><span class="sxs-lookup"><span data-stu-id="9a260-152">Int32</span></span>|<span data-ttu-id="9a260-153">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="9a260-153">Version of the device configuration.</span></span> <span data-ttu-id="9a260-154">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="9a260-154">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="9a260-155">passcodeBlockSimple</span><span class="sxs-lookup"><span data-stu-id="9a260-155">passcodeBlockSimple</span></span>|<span data-ttu-id="9a260-156">Boolean</span><span class="sxs-lookup"><span data-stu-id="9a260-156">Boolean</span></span>|<span data-ttu-id="9a260-157">指示是否阻止简单密码。</span><span class="sxs-lookup"><span data-stu-id="9a260-157">Indicates whether or not to block simple passcodes.</span></span>|
|<span data-ttu-id="9a260-158">passcodeExpirationDays</span><span class="sxs-lookup"><span data-stu-id="9a260-158">passcodeExpirationDays</span></span>|<span data-ttu-id="9a260-159">Int32</span><span class="sxs-lookup"><span data-stu-id="9a260-159">Int32</span></span>|<span data-ttu-id="9a260-160">密码过期前的天数。</span><span class="sxs-lookup"><span data-stu-id="9a260-160">Number of days before the passcode expires.</span></span> <span data-ttu-id="9a260-161">有效值为 1 至 65535</span><span class="sxs-lookup"><span data-stu-id="9a260-161">Valid values 1 to 65535</span></span>|
|<span data-ttu-id="9a260-162">passcodeMinimumLength</span><span class="sxs-lookup"><span data-stu-id="9a260-162">passcodeMinimumLength</span></span>|<span data-ttu-id="9a260-163">Int32</span><span class="sxs-lookup"><span data-stu-id="9a260-163">Int32</span></span>|<span data-ttu-id="9a260-164">密码的最小长度。</span><span class="sxs-lookup"><span data-stu-id="9a260-164">Minimum length of passcode.</span></span> <span data-ttu-id="9a260-165">有效值为 4 至 14</span><span class="sxs-lookup"><span data-stu-id="9a260-165">Valid values 4 to 14</span></span>|
|<span data-ttu-id="9a260-166">passcodeMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="9a260-166">passcodeMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="9a260-167">Int32</span><span class="sxs-lookup"><span data-stu-id="9a260-167">Int32</span></span>|<span data-ttu-id="9a260-168">在需要密码之前不活动的分钟数。</span><span class="sxs-lookup"><span data-stu-id="9a260-168">Minutes of inactivity before a passcode is required.</span></span>|
|<span data-ttu-id="9a260-169">passcodePreviousPasscodeBlockCount</span><span class="sxs-lookup"><span data-stu-id="9a260-169">passcodePreviousPasscodeBlockCount</span></span>|<span data-ttu-id="9a260-170">Int32</span><span class="sxs-lookup"><span data-stu-id="9a260-170">Int32</span></span>|<span data-ttu-id="9a260-171">要阻止的以前密码的数量。</span><span class="sxs-lookup"><span data-stu-id="9a260-171">Number of previous passcodes to block.</span></span> <span data-ttu-id="9a260-172">有效值为 1 至 24</span><span class="sxs-lookup"><span data-stu-id="9a260-172">Valid values 1 to 24</span></span>|
|<span data-ttu-id="9a260-173">passcodeMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="9a260-173">passcodeMinimumCharacterSetCount</span></span>|<span data-ttu-id="9a260-174">Int32</span><span class="sxs-lookup"><span data-stu-id="9a260-174">Int32</span></span>|<span data-ttu-id="9a260-175">密码中必需的字符集数。</span><span class="sxs-lookup"><span data-stu-id="9a260-175">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="9a260-176">passcodeRequiredType</span><span class="sxs-lookup"><span data-stu-id="9a260-176">passcodeRequiredType</span></span>|[<span data-ttu-id="9a260-177">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="9a260-177">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="9a260-178">必需的密码类型。</span><span class="sxs-lookup"><span data-stu-id="9a260-178">The required passcode type.</span></span> <span data-ttu-id="9a260-179">可取值为：`deviceDefault`、`alphanumeric`、`numeric`。</span><span class="sxs-lookup"><span data-stu-id="9a260-179">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="9a260-180">passcodeRequired</span><span class="sxs-lookup"><span data-stu-id="9a260-180">passcodeRequired</span></span>|<span data-ttu-id="9a260-181">Boolean</span><span class="sxs-lookup"><span data-stu-id="9a260-181">Boolean</span></span>|<span data-ttu-id="9a260-182">指示是否需要密码。</span><span class="sxs-lookup"><span data-stu-id="9a260-182">Indicates whether or not to require a passcode.</span></span>|
|<span data-ttu-id="9a260-183">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="9a260-183">osMinimumVersion</span></span>|<span data-ttu-id="9a260-184">String</span><span class="sxs-lookup"><span data-stu-id="9a260-184">String</span></span>|<span data-ttu-id="9a260-185">最低 IOS 版本。</span><span class="sxs-lookup"><span data-stu-id="9a260-185">Minimum IOS version.</span></span>|
|<span data-ttu-id="9a260-186">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="9a260-186">osMaximumVersion</span></span>|<span data-ttu-id="9a260-187">String</span><span class="sxs-lookup"><span data-stu-id="9a260-187">String</span></span>|<span data-ttu-id="9a260-188">最高 IOS 版本。</span><span class="sxs-lookup"><span data-stu-id="9a260-188">Maximum IOS version.</span></span>|
|<span data-ttu-id="9a260-189">securityBlockJailbrokenDevices</span><span class="sxs-lookup"><span data-stu-id="9a260-189">securityBlockJailbrokenDevices</span></span>|<span data-ttu-id="9a260-190">Boolean</span><span class="sxs-lookup"><span data-stu-id="9a260-190">Boolean</span></span>|<span data-ttu-id="9a260-191">设备不得越狱或取得 root 权限。</span><span class="sxs-lookup"><span data-stu-id="9a260-191">Devices must not be jailbroken or rooted.</span></span>|
|<span data-ttu-id="9a260-192">deviceThreatProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="9a260-192">deviceThreatProtectionEnabled</span></span>|<span data-ttu-id="9a260-193">Boolean</span><span class="sxs-lookup"><span data-stu-id="9a260-193">Boolean</span></span>|<span data-ttu-id="9a260-194">要求设备已启用设备威胁防护。</span><span class="sxs-lookup"><span data-stu-id="9a260-194">Require that devices have enabled device threat protection .</span></span>|
|<span data-ttu-id="9a260-195">deviceThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="9a260-195">deviceThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="9a260-196">deviceThreatProtectionLevel</span><span class="sxs-lookup"><span data-stu-id="9a260-196">deviceThreatProtectionLevel</span></span>](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|<span data-ttu-id="9a260-197">要求移动威胁防护最低风险级别来报告不符合情况。</span><span class="sxs-lookup"><span data-stu-id="9a260-197">Require Mobile Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="9a260-198">可取值为：`unavailable`、`secured`、`low`、`medium`、`high`、`notSet`。</span><span class="sxs-lookup"><span data-stu-id="9a260-198">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="9a260-199">managedEmailProfileRequired</span><span class="sxs-lookup"><span data-stu-id="9a260-199">managedEmailProfileRequired</span></span>|<span data-ttu-id="9a260-200">Boolean</span><span class="sxs-lookup"><span data-stu-id="9a260-200">Boolean</span></span>|<span data-ttu-id="9a260-201">指示是否需要托管电子邮件配置文件。</span><span class="sxs-lookup"><span data-stu-id="9a260-201">Indicates whether or not to require a managed email profile.</span></span>|



## <a name="response"></a><span data-ttu-id="9a260-202">响应</span><span class="sxs-lookup"><span data-stu-id="9a260-202">Response</span></span>
<span data-ttu-id="9a260-203">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和更新的 [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="9a260-203">If successful, this method returns a `200 OK` response code and an updated [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9a260-204">示例</span><span class="sxs-lookup"><span data-stu-id="9a260-204">Example</span></span>

### <a name="request"></a><span data-ttu-id="9a260-205">请求</span><span class="sxs-lookup"><span data-stu-id="9a260-205">Request</span></span>
<span data-ttu-id="9a260-206">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="9a260-206">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="9a260-207">响应</span><span class="sxs-lookup"><span data-stu-id="9a260-207">Response</span></span>
<span data-ttu-id="9a260-p113">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="9a260-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




