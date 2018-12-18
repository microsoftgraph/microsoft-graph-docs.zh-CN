---
title: 更新 iosCompliancePolicy
description: 更新 iosCompliancePolicy 对象的属性。
author: tfitzmac
ms.openlocfilehash: 3b6589601622015f589c10f2ed839117b4755269
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27305122"
---
# <a name="update-ioscompliancepolicy"></a><span data-ttu-id="2c90d-103">更新 iosCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="2c90d-103">Update iosCompliancePolicy</span></span>

> <span data-ttu-id="2c90d-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="2c90d-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2c90d-105">更新 [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="2c90d-105">Update the properties of a [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="2c90d-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="2c90d-106">Prerequisites</span></span>
<span data-ttu-id="2c90d-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="2c90d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2c90d-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="2c90d-109">Permission type</span></span>|<span data-ttu-id="2c90d-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="2c90d-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2c90d-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2c90d-111">Delegated (work or school account)</span></span>|<span data-ttu-id="2c90d-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2c90d-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="2c90d-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2c90d-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2c90d-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="2c90d-114">Not supported.</span></span>|
|<span data-ttu-id="2c90d-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="2c90d-115">Application</span></span>|<span data-ttu-id="2c90d-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="2c90d-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2c90d-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2c90d-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="2c90d-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="2c90d-118">Request headers</span></span>
|<span data-ttu-id="2c90d-119">标头</span><span class="sxs-lookup"><span data-stu-id="2c90d-119">Header</span></span>|<span data-ttu-id="2c90d-120">值</span><span class="sxs-lookup"><span data-stu-id="2c90d-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2c90d-121">授权</span><span class="sxs-lookup"><span data-stu-id="2c90d-121">Authorization</span></span>|<span data-ttu-id="2c90d-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="2c90d-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2c90d-123">Accept</span><span class="sxs-lookup"><span data-stu-id="2c90d-123">Accept</span></span>|<span data-ttu-id="2c90d-124">application/json</span><span class="sxs-lookup"><span data-stu-id="2c90d-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2c90d-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="2c90d-125">Request body</span></span>
<span data-ttu-id="2c90d-126">在请求正文中，提供 [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2c90d-126">In the request body, supply a JSON representation for the [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) object.</span></span>

<span data-ttu-id="2c90d-127">下表显示了创建 [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="2c90d-127">The following table shows the properties that are required when you create the [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md).</span></span>

|<span data-ttu-id="2c90d-128">属性</span><span class="sxs-lookup"><span data-stu-id="2c90d-128">Property</span></span>|<span data-ttu-id="2c90d-129">类型</span><span class="sxs-lookup"><span data-stu-id="2c90d-129">Type</span></span>|<span data-ttu-id="2c90d-130">说明</span><span class="sxs-lookup"><span data-stu-id="2c90d-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2c90d-131">id</span><span class="sxs-lookup"><span data-stu-id="2c90d-131">id</span></span>|<span data-ttu-id="2c90d-132">String</span><span class="sxs-lookup"><span data-stu-id="2c90d-132">String</span></span>|<span data-ttu-id="2c90d-133">实体的键。</span><span class="sxs-lookup"><span data-stu-id="2c90d-133">Key of the entity.</span></span> <span data-ttu-id="2c90d-134">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="2c90d-134">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="2c90d-135">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="2c90d-135">createdDateTime</span></span>|<span data-ttu-id="2c90d-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2c90d-136">DateTimeOffset</span></span>|<span data-ttu-id="2c90d-137">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="2c90d-137">DateTime the object was created.</span></span> <span data-ttu-id="2c90d-138">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="2c90d-138">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="2c90d-139">description</span><span class="sxs-lookup"><span data-stu-id="2c90d-139">description</span></span>|<span data-ttu-id="2c90d-140">String</span><span class="sxs-lookup"><span data-stu-id="2c90d-140">String</span></span>|<span data-ttu-id="2c90d-141">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="2c90d-141">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="2c90d-142">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="2c90d-142">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="2c90d-143">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2c90d-143">lastModifiedDateTime</span></span>|<span data-ttu-id="2c90d-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2c90d-144">DateTimeOffset</span></span>|<span data-ttu-id="2c90d-145">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="2c90d-145">DateTime the object was last modified.</span></span> <span data-ttu-id="2c90d-146">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="2c90d-146">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="2c90d-147">displayName</span><span class="sxs-lookup"><span data-stu-id="2c90d-147">displayName</span></span>|<span data-ttu-id="2c90d-148">String</span><span class="sxs-lookup"><span data-stu-id="2c90d-148">String</span></span>|<span data-ttu-id="2c90d-149">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="2c90d-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="2c90d-150">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="2c90d-150">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="2c90d-151">version</span><span class="sxs-lookup"><span data-stu-id="2c90d-151">version</span></span>|<span data-ttu-id="2c90d-152">Int32</span><span class="sxs-lookup"><span data-stu-id="2c90d-152">Int32</span></span>|<span data-ttu-id="2c90d-153">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="2c90d-153">Version of the device configuration.</span></span> <span data-ttu-id="2c90d-154">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="2c90d-154">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="2c90d-155">passcodeBlockSimple</span><span class="sxs-lookup"><span data-stu-id="2c90d-155">passcodeBlockSimple</span></span>|<span data-ttu-id="2c90d-156">Boolean</span><span class="sxs-lookup"><span data-stu-id="2c90d-156">Boolean</span></span>|<span data-ttu-id="2c90d-157">指示是否阻止简单密码。</span><span class="sxs-lookup"><span data-stu-id="2c90d-157">Indicates whether or not to block simple passcodes.</span></span>|
|<span data-ttu-id="2c90d-158">passcodeExpirationDays</span><span class="sxs-lookup"><span data-stu-id="2c90d-158">passcodeExpirationDays</span></span>|<span data-ttu-id="2c90d-159">Int32</span><span class="sxs-lookup"><span data-stu-id="2c90d-159">Int32</span></span>|<span data-ttu-id="2c90d-160">密码过期前的天数。</span><span class="sxs-lookup"><span data-stu-id="2c90d-160">Number of days before the passcode expires.</span></span> <span data-ttu-id="2c90d-161">有效值为 1 至 65535</span><span class="sxs-lookup"><span data-stu-id="2c90d-161">Valid values 1 to 65535</span></span>|
|<span data-ttu-id="2c90d-162">passcodeMinimumLength</span><span class="sxs-lookup"><span data-stu-id="2c90d-162">passcodeMinimumLength</span></span>|<span data-ttu-id="2c90d-163">Int32</span><span class="sxs-lookup"><span data-stu-id="2c90d-163">Int32</span></span>|<span data-ttu-id="2c90d-164">密码的最小长度。</span><span class="sxs-lookup"><span data-stu-id="2c90d-164">Minimum length of passcode.</span></span> <span data-ttu-id="2c90d-165">有效值为 4 至 14</span><span class="sxs-lookup"><span data-stu-id="2c90d-165">Valid values 4 to 14</span></span>|
|<span data-ttu-id="2c90d-166">passcodeMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="2c90d-166">passcodeMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="2c90d-167">Int32</span><span class="sxs-lookup"><span data-stu-id="2c90d-167">Int32</span></span>|<span data-ttu-id="2c90d-168">在需要密码之前不活动的分钟数。</span><span class="sxs-lookup"><span data-stu-id="2c90d-168">Minutes of inactivity before a passcode is required.</span></span>|
|<span data-ttu-id="2c90d-169">passcodePreviousPasscodeBlockCount</span><span class="sxs-lookup"><span data-stu-id="2c90d-169">passcodePreviousPasscodeBlockCount</span></span>|<span data-ttu-id="2c90d-170">Int32</span><span class="sxs-lookup"><span data-stu-id="2c90d-170">Int32</span></span>|<span data-ttu-id="2c90d-171">要阻止的以前密码的数量。</span><span class="sxs-lookup"><span data-stu-id="2c90d-171">Number of previous passcodes to block.</span></span> <span data-ttu-id="2c90d-172">有效值为 1 至 24</span><span class="sxs-lookup"><span data-stu-id="2c90d-172">Valid values 1 to 24</span></span>|
|<span data-ttu-id="2c90d-173">passcodeMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="2c90d-173">passcodeMinimumCharacterSetCount</span></span>|<span data-ttu-id="2c90d-174">Int32</span><span class="sxs-lookup"><span data-stu-id="2c90d-174">Int32</span></span>|<span data-ttu-id="2c90d-175">密码中必需的字符集数。</span><span class="sxs-lookup"><span data-stu-id="2c90d-175">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="2c90d-176">passcodeRequiredType</span><span class="sxs-lookup"><span data-stu-id="2c90d-176">passcodeRequiredType</span></span>|[<span data-ttu-id="2c90d-177">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="2c90d-177">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="2c90d-178">必需的密码类型。</span><span class="sxs-lookup"><span data-stu-id="2c90d-178">The required passcode type.</span></span> <span data-ttu-id="2c90d-179">可取值为：`deviceDefault`、`alphanumeric`、`numeric`。</span><span class="sxs-lookup"><span data-stu-id="2c90d-179">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="2c90d-180">passcodeRequired</span><span class="sxs-lookup"><span data-stu-id="2c90d-180">passcodeRequired</span></span>|<span data-ttu-id="2c90d-181">Boolean</span><span class="sxs-lookup"><span data-stu-id="2c90d-181">Boolean</span></span>|<span data-ttu-id="2c90d-182">指示是否需要密码。</span><span class="sxs-lookup"><span data-stu-id="2c90d-182">Indicates whether or not to require a passcode.</span></span>|
|<span data-ttu-id="2c90d-183">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="2c90d-183">osMinimumVersion</span></span>|<span data-ttu-id="2c90d-184">String</span><span class="sxs-lookup"><span data-stu-id="2c90d-184">String</span></span>|<span data-ttu-id="2c90d-185">最低 IOS 版本。</span><span class="sxs-lookup"><span data-stu-id="2c90d-185">Minimum IOS version.</span></span>|
|<span data-ttu-id="2c90d-186">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="2c90d-186">osMaximumVersion</span></span>|<span data-ttu-id="2c90d-187">String</span><span class="sxs-lookup"><span data-stu-id="2c90d-187">String</span></span>|<span data-ttu-id="2c90d-188">最高 IOS 版本。</span><span class="sxs-lookup"><span data-stu-id="2c90d-188">Maximum IOS version.</span></span>|
|<span data-ttu-id="2c90d-189">securityBlockJailbrokenDevices</span><span class="sxs-lookup"><span data-stu-id="2c90d-189">securityBlockJailbrokenDevices</span></span>|<span data-ttu-id="2c90d-190">Boolean</span><span class="sxs-lookup"><span data-stu-id="2c90d-190">Boolean</span></span>|<span data-ttu-id="2c90d-191">设备不得越狱或取得 root 权限。</span><span class="sxs-lookup"><span data-stu-id="2c90d-191">Devices must not be jailbroken or rooted.</span></span>|
|<span data-ttu-id="2c90d-192">deviceThreatProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="2c90d-192">deviceThreatProtectionEnabled</span></span>|<span data-ttu-id="2c90d-193">Boolean</span><span class="sxs-lookup"><span data-stu-id="2c90d-193">Boolean</span></span>|<span data-ttu-id="2c90d-194">要求设备已启用设备威胁防护。</span><span class="sxs-lookup"><span data-stu-id="2c90d-194">Require that devices have enabled device threat protection .</span></span>|
|<span data-ttu-id="2c90d-195">deviceThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="2c90d-195">deviceThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="2c90d-196">deviceThreatProtectionLevel</span><span class="sxs-lookup"><span data-stu-id="2c90d-196">deviceThreatProtectionLevel</span></span>](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|<span data-ttu-id="2c90d-197">要求移动威胁防护最低风险级别来报告不符合情况。</span><span class="sxs-lookup"><span data-stu-id="2c90d-197">Require Mobile Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="2c90d-198">可取值为：`unavailable`、`secured`、`low`、`medium`、`high`、`notSet`。</span><span class="sxs-lookup"><span data-stu-id="2c90d-198">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="2c90d-199">managedEmailProfileRequired</span><span class="sxs-lookup"><span data-stu-id="2c90d-199">managedEmailProfileRequired</span></span>|<span data-ttu-id="2c90d-200">Boolean</span><span class="sxs-lookup"><span data-stu-id="2c90d-200">Boolean</span></span>|<span data-ttu-id="2c90d-201">指示是否需要托管电子邮件配置文件。</span><span class="sxs-lookup"><span data-stu-id="2c90d-201">Indicates whether or not to require a managed email profile.</span></span>|



## <a name="response"></a><span data-ttu-id="2c90d-202">响应</span><span class="sxs-lookup"><span data-stu-id="2c90d-202">Response</span></span>
<span data-ttu-id="2c90d-203">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和更新的 [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="2c90d-203">If successful, this method returns a `200 OK` response code and an updated [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2c90d-204">示例</span><span class="sxs-lookup"><span data-stu-id="2c90d-204">Example</span></span>
### <a name="request"></a><span data-ttu-id="2c90d-205">请求</span><span class="sxs-lookup"><span data-stu-id="2c90d-205">Request</span></span>
<span data-ttu-id="2c90d-206">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="2c90d-206">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="2c90d-207">响应</span><span class="sxs-lookup"><span data-stu-id="2c90d-207">Response</span></span>
<span data-ttu-id="2c90d-p113">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="2c90d-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



