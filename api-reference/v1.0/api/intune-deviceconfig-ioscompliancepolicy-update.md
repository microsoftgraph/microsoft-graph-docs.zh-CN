---
title: 更新 iosCompliancePolicy
description: 更新 iosCompliancePolicy 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: fb8b8590fd59154fce31912d6275d23929a66f94
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/29/2019
ms.locfileid: "30977476"
---
# <a name="update-ioscompliancepolicy"></a><span data-ttu-id="c3812-103">更新 iosCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="c3812-103">Update iosCompliancePolicy</span></span>

> <span data-ttu-id="c3812-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c3812-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c3812-105">更新 [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="c3812-105">Update the properties of a [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c3812-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="c3812-106">Prerequisites</span></span>
<span data-ttu-id="c3812-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c3812-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c3812-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="c3812-109">Permission type</span></span>|<span data-ttu-id="c3812-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="c3812-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c3812-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c3812-111">Delegated (work or school account)</span></span>|<span data-ttu-id="c3812-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c3812-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c3812-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c3812-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c3812-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="c3812-114">Not supported.</span></span>|
|<span data-ttu-id="c3812-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="c3812-115">Application</span></span>|<span data-ttu-id="c3812-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="c3812-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c3812-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c3812-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="c3812-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="c3812-118">Request headers</span></span>
|<span data-ttu-id="c3812-119">标头</span><span class="sxs-lookup"><span data-stu-id="c3812-119">Header</span></span>|<span data-ttu-id="c3812-120">值</span><span class="sxs-lookup"><span data-stu-id="c3812-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c3812-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="c3812-121">Authorization</span></span>|<span data-ttu-id="c3812-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="c3812-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c3812-123">接受</span><span class="sxs-lookup"><span data-stu-id="c3812-123">Accept</span></span>|<span data-ttu-id="c3812-124">application/json</span><span class="sxs-lookup"><span data-stu-id="c3812-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c3812-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="c3812-125">Request body</span></span>
<span data-ttu-id="c3812-126">在请求正文中，提供 [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c3812-126">In the request body, supply a JSON representation for the [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) object.</span></span>

<span data-ttu-id="c3812-127">下表显示了创建 [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="c3812-127">The following table shows the properties that are required when you create the [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md).</span></span>

|<span data-ttu-id="c3812-128">属性</span><span class="sxs-lookup"><span data-stu-id="c3812-128">Property</span></span>|<span data-ttu-id="c3812-129">类型</span><span class="sxs-lookup"><span data-stu-id="c3812-129">Type</span></span>|<span data-ttu-id="c3812-130">说明</span><span class="sxs-lookup"><span data-stu-id="c3812-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c3812-131">id</span><span class="sxs-lookup"><span data-stu-id="c3812-131">id</span></span>|<span data-ttu-id="c3812-132">String</span><span class="sxs-lookup"><span data-stu-id="c3812-132">String</span></span>|<span data-ttu-id="c3812-133">实体的键。</span><span class="sxs-lookup"><span data-stu-id="c3812-133">Key of the entity.</span></span> <span data-ttu-id="c3812-134">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="c3812-134">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="c3812-135">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c3812-135">createdDateTime</span></span>|<span data-ttu-id="c3812-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c3812-136">DateTimeOffset</span></span>|<span data-ttu-id="c3812-137">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="c3812-137">DateTime the object was created.</span></span> <span data-ttu-id="c3812-138">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="c3812-138">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="c3812-139">description</span><span class="sxs-lookup"><span data-stu-id="c3812-139">description</span></span>|<span data-ttu-id="c3812-140">String</span><span class="sxs-lookup"><span data-stu-id="c3812-140">String</span></span>|<span data-ttu-id="c3812-141">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="c3812-141">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="c3812-142">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="c3812-142">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="c3812-143">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c3812-143">lastModifiedDateTime</span></span>|<span data-ttu-id="c3812-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c3812-144">DateTimeOffset</span></span>|<span data-ttu-id="c3812-145">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="c3812-145">DateTime the object was last modified.</span></span> <span data-ttu-id="c3812-146">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="c3812-146">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="c3812-147">displayName</span><span class="sxs-lookup"><span data-stu-id="c3812-147">displayName</span></span>|<span data-ttu-id="c3812-148">String</span><span class="sxs-lookup"><span data-stu-id="c3812-148">String</span></span>|<span data-ttu-id="c3812-149">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="c3812-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="c3812-150">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="c3812-150">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="c3812-151">version</span><span class="sxs-lookup"><span data-stu-id="c3812-151">version</span></span>|<span data-ttu-id="c3812-152">Int32</span><span class="sxs-lookup"><span data-stu-id="c3812-152">Int32</span></span>|<span data-ttu-id="c3812-153">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="c3812-153">Version of the device configuration.</span></span> <span data-ttu-id="c3812-154">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="c3812-154">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="c3812-155">passcodeBlockSimple</span><span class="sxs-lookup"><span data-stu-id="c3812-155">passcodeBlockSimple</span></span>|<span data-ttu-id="c3812-156">Boolean</span><span class="sxs-lookup"><span data-stu-id="c3812-156">Boolean</span></span>|<span data-ttu-id="c3812-157">指示是否阻止简单密码。</span><span class="sxs-lookup"><span data-stu-id="c3812-157">Indicates whether or not to block simple passcodes.</span></span>|
|<span data-ttu-id="c3812-158">passcodeExpirationDays</span><span class="sxs-lookup"><span data-stu-id="c3812-158">passcodeExpirationDays</span></span>|<span data-ttu-id="c3812-159">Int32</span><span class="sxs-lookup"><span data-stu-id="c3812-159">Int32</span></span>|<span data-ttu-id="c3812-160">密码过期前的天数。</span><span class="sxs-lookup"><span data-stu-id="c3812-160">Number of days before the passcode expires.</span></span> <span data-ttu-id="c3812-161">有效值为 1 至 65535</span><span class="sxs-lookup"><span data-stu-id="c3812-161">Valid values 1 to 65535</span></span>|
|<span data-ttu-id="c3812-162">passcodeMinimumLength</span><span class="sxs-lookup"><span data-stu-id="c3812-162">passcodeMinimumLength</span></span>|<span data-ttu-id="c3812-163">Int32</span><span class="sxs-lookup"><span data-stu-id="c3812-163">Int32</span></span>|<span data-ttu-id="c3812-164">密码的最小长度。</span><span class="sxs-lookup"><span data-stu-id="c3812-164">Minimum length of passcode.</span></span> <span data-ttu-id="c3812-165">有效值为 4 至 14</span><span class="sxs-lookup"><span data-stu-id="c3812-165">Valid values 4 to 14</span></span>|
|<span data-ttu-id="c3812-166">passcodeMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="c3812-166">passcodeMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="c3812-167">Int32</span><span class="sxs-lookup"><span data-stu-id="c3812-167">Int32</span></span>|<span data-ttu-id="c3812-168">在需要密码之前不活动的分钟数。</span><span class="sxs-lookup"><span data-stu-id="c3812-168">Minutes of inactivity before a passcode is required.</span></span>|
|<span data-ttu-id="c3812-169">passcodePreviousPasscodeBlockCount</span><span class="sxs-lookup"><span data-stu-id="c3812-169">passcodePreviousPasscodeBlockCount</span></span>|<span data-ttu-id="c3812-170">Int32</span><span class="sxs-lookup"><span data-stu-id="c3812-170">Int32</span></span>|<span data-ttu-id="c3812-171">要阻止的以前密码的数量。</span><span class="sxs-lookup"><span data-stu-id="c3812-171">Number of previous passcodes to block.</span></span> <span data-ttu-id="c3812-172">有效值为 1 至 24</span><span class="sxs-lookup"><span data-stu-id="c3812-172">Valid values 1 to 24</span></span>|
|<span data-ttu-id="c3812-173">passcodeMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="c3812-173">passcodeMinimumCharacterSetCount</span></span>|<span data-ttu-id="c3812-174">Int32</span><span class="sxs-lookup"><span data-stu-id="c3812-174">Int32</span></span>|<span data-ttu-id="c3812-175">密码中必需的字符集数。</span><span class="sxs-lookup"><span data-stu-id="c3812-175">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="c3812-176">passcodeRequiredType</span><span class="sxs-lookup"><span data-stu-id="c3812-176">passcodeRequiredType</span></span>|[<span data-ttu-id="c3812-177">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="c3812-177">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="c3812-178">必需的密码类型。</span><span class="sxs-lookup"><span data-stu-id="c3812-178">The required passcode type.</span></span> <span data-ttu-id="c3812-179">可取值为：`deviceDefault`、`alphanumeric`、`numeric`。</span><span class="sxs-lookup"><span data-stu-id="c3812-179">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="c3812-180">passcodeRequired</span><span class="sxs-lookup"><span data-stu-id="c3812-180">passcodeRequired</span></span>|<span data-ttu-id="c3812-181">Boolean</span><span class="sxs-lookup"><span data-stu-id="c3812-181">Boolean</span></span>|<span data-ttu-id="c3812-182">指示是否需要密码。</span><span class="sxs-lookup"><span data-stu-id="c3812-182">Indicates whether or not to require a passcode.</span></span>|
|<span data-ttu-id="c3812-183">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="c3812-183">osMinimumVersion</span></span>|<span data-ttu-id="c3812-184">String</span><span class="sxs-lookup"><span data-stu-id="c3812-184">String</span></span>|<span data-ttu-id="c3812-185">最低 IOS 版本。</span><span class="sxs-lookup"><span data-stu-id="c3812-185">Minimum IOS version.</span></span>|
|<span data-ttu-id="c3812-186">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="c3812-186">osMaximumVersion</span></span>|<span data-ttu-id="c3812-187">String</span><span class="sxs-lookup"><span data-stu-id="c3812-187">String</span></span>|<span data-ttu-id="c3812-188">最高 IOS 版本。</span><span class="sxs-lookup"><span data-stu-id="c3812-188">Maximum IOS version.</span></span>|
|<span data-ttu-id="c3812-189">securityBlockJailbrokenDevices</span><span class="sxs-lookup"><span data-stu-id="c3812-189">securityBlockJailbrokenDevices</span></span>|<span data-ttu-id="c3812-190">Boolean</span><span class="sxs-lookup"><span data-stu-id="c3812-190">Boolean</span></span>|<span data-ttu-id="c3812-191">设备不得越狱或取得 root 权限。</span><span class="sxs-lookup"><span data-stu-id="c3812-191">Devices must not be jailbroken or rooted.</span></span>|
|<span data-ttu-id="c3812-192">deviceThreatProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="c3812-192">deviceThreatProtectionEnabled</span></span>|<span data-ttu-id="c3812-193">Boolean</span><span class="sxs-lookup"><span data-stu-id="c3812-193">Boolean</span></span>|<span data-ttu-id="c3812-194">要求设备已启用设备威胁防护。</span><span class="sxs-lookup"><span data-stu-id="c3812-194">Require that devices have enabled device threat protection .</span></span>|
|<span data-ttu-id="c3812-195">deviceThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="c3812-195">deviceThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="c3812-196">deviceThreatProtectionLevel</span><span class="sxs-lookup"><span data-stu-id="c3812-196">deviceThreatProtectionLevel</span></span>](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|<span data-ttu-id="c3812-197">要求移动威胁防护最低风险级别来报告不符合情况。</span><span class="sxs-lookup"><span data-stu-id="c3812-197">Require Mobile Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="c3812-198">可取值为：`unavailable`、`secured`、`low`、`medium`、`high`、`notSet`。</span><span class="sxs-lookup"><span data-stu-id="c3812-198">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="c3812-199">managedEmailProfileRequired</span><span class="sxs-lookup"><span data-stu-id="c3812-199">managedEmailProfileRequired</span></span>|<span data-ttu-id="c3812-200">Boolean</span><span class="sxs-lookup"><span data-stu-id="c3812-200">Boolean</span></span>|<span data-ttu-id="c3812-201">指示是否需要托管电子邮件配置文件。</span><span class="sxs-lookup"><span data-stu-id="c3812-201">Indicates whether or not to require a managed email profile.</span></span>|



## <a name="response"></a><span data-ttu-id="c3812-202">响应</span><span class="sxs-lookup"><span data-stu-id="c3812-202">Response</span></span>
<span data-ttu-id="c3812-203">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和更新的 [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="c3812-203">If successful, this method returns a `200 OK` response code and an updated [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c3812-204">示例</span><span class="sxs-lookup"><span data-stu-id="c3812-204">Example</span></span>

### <a name="request"></a><span data-ttu-id="c3812-205">请求</span><span class="sxs-lookup"><span data-stu-id="c3812-205">Request</span></span>
<span data-ttu-id="c3812-206">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="c3812-206">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="c3812-207">响应</span><span class="sxs-lookup"><span data-stu-id="c3812-207">Response</span></span>
<span data-ttu-id="c3812-p113">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="c3812-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



