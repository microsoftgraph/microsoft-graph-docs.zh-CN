---
title: 创建 iosCompliancePolicy
description: 创建新的 iosCompliancePolicy 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: fccf80d259562c6064a8307c601d477dfc8c3693
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52759259"
---
# <a name="create-ioscompliancepolicy"></a><span data-ttu-id="01735-103">创建 iosCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="01735-103">Create iosCompliancePolicy</span></span>

<span data-ttu-id="01735-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="01735-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="01735-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="01735-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="01735-106">创建新的 [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="01735-106">Create a new [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="01735-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="01735-107">Prerequisites</span></span>
<span data-ttu-id="01735-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="01735-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="01735-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="01735-110">Permission type</span></span>|<span data-ttu-id="01735-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="01735-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="01735-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="01735-112">Delegated (work or school account)</span></span>|<span data-ttu-id="01735-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="01735-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="01735-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="01735-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="01735-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="01735-115">Not supported.</span></span>|
|<span data-ttu-id="01735-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="01735-116">Application</span></span>|<span data-ttu-id="01735-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="01735-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="01735-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="01735-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="01735-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="01735-119">Request headers</span></span>
|<span data-ttu-id="01735-120">标头</span><span class="sxs-lookup"><span data-stu-id="01735-120">Header</span></span>|<span data-ttu-id="01735-121">值</span><span class="sxs-lookup"><span data-stu-id="01735-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="01735-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="01735-122">Authorization</span></span>|<span data-ttu-id="01735-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="01735-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="01735-124">接受</span><span class="sxs-lookup"><span data-stu-id="01735-124">Accept</span></span>|<span data-ttu-id="01735-125">application/json</span><span class="sxs-lookup"><span data-stu-id="01735-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="01735-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="01735-126">Request body</span></span>
<span data-ttu-id="01735-127">在请求正文中，提供 iosCompliancePolicy 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="01735-127">In the request body, supply a JSON representation for the iosCompliancePolicy object.</span></span>

<span data-ttu-id="01735-128">下表显示了创建 iosCompliancePolicy 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="01735-128">The following table shows the properties that are required when you create the iosCompliancePolicy.</span></span>

|<span data-ttu-id="01735-129">属性</span><span class="sxs-lookup"><span data-stu-id="01735-129">Property</span></span>|<span data-ttu-id="01735-130">类型</span><span class="sxs-lookup"><span data-stu-id="01735-130">Type</span></span>|<span data-ttu-id="01735-131">说明</span><span class="sxs-lookup"><span data-stu-id="01735-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="01735-132">id</span><span class="sxs-lookup"><span data-stu-id="01735-132">id</span></span>|<span data-ttu-id="01735-133">String</span><span class="sxs-lookup"><span data-stu-id="01735-133">String</span></span>|<span data-ttu-id="01735-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="01735-134">Key of the entity.</span></span> <span data-ttu-id="01735-135">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="01735-135">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="01735-136">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="01735-136">createdDateTime</span></span>|<span data-ttu-id="01735-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="01735-137">DateTimeOffset</span></span>|<span data-ttu-id="01735-138">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="01735-138">DateTime the object was created.</span></span> <span data-ttu-id="01735-139">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="01735-139">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="01735-140">description</span><span class="sxs-lookup"><span data-stu-id="01735-140">description</span></span>|<span data-ttu-id="01735-141">String</span><span class="sxs-lookup"><span data-stu-id="01735-141">String</span></span>|<span data-ttu-id="01735-142">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="01735-142">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="01735-143">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="01735-143">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="01735-144">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="01735-144">lastModifiedDateTime</span></span>|<span data-ttu-id="01735-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="01735-145">DateTimeOffset</span></span>|<span data-ttu-id="01735-146">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="01735-146">DateTime the object was last modified.</span></span> <span data-ttu-id="01735-147">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="01735-147">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="01735-148">displayName</span><span class="sxs-lookup"><span data-stu-id="01735-148">displayName</span></span>|<span data-ttu-id="01735-149">String</span><span class="sxs-lookup"><span data-stu-id="01735-149">String</span></span>|<span data-ttu-id="01735-150">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="01735-150">Admin provided name of the device configuration.</span></span> <span data-ttu-id="01735-151">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="01735-151">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="01735-152">version</span><span class="sxs-lookup"><span data-stu-id="01735-152">version</span></span>|<span data-ttu-id="01735-153">Int32</span><span class="sxs-lookup"><span data-stu-id="01735-153">Int32</span></span>|<span data-ttu-id="01735-154">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="01735-154">Version of the device configuration.</span></span> <span data-ttu-id="01735-155">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="01735-155">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="01735-156">passcodeBlockSimple</span><span class="sxs-lookup"><span data-stu-id="01735-156">passcodeBlockSimple</span></span>|<span data-ttu-id="01735-157">Boolean</span><span class="sxs-lookup"><span data-stu-id="01735-157">Boolean</span></span>|<span data-ttu-id="01735-158">指示是否阻止简单密码。</span><span class="sxs-lookup"><span data-stu-id="01735-158">Indicates whether or not to block simple passcodes.</span></span>|
|<span data-ttu-id="01735-159">passcodeExpirationDays</span><span class="sxs-lookup"><span data-stu-id="01735-159">passcodeExpirationDays</span></span>|<span data-ttu-id="01735-160">Int32</span><span class="sxs-lookup"><span data-stu-id="01735-160">Int32</span></span>|<span data-ttu-id="01735-161">密码过期前的天数。</span><span class="sxs-lookup"><span data-stu-id="01735-161">Number of days before the passcode expires.</span></span> <span data-ttu-id="01735-162">有效值为 1 至 65535</span><span class="sxs-lookup"><span data-stu-id="01735-162">Valid values 1 to 65535</span></span>|
|<span data-ttu-id="01735-163">passcodeMinimumLength</span><span class="sxs-lookup"><span data-stu-id="01735-163">passcodeMinimumLength</span></span>|<span data-ttu-id="01735-164">Int32</span><span class="sxs-lookup"><span data-stu-id="01735-164">Int32</span></span>|<span data-ttu-id="01735-165">密码的最小长度。</span><span class="sxs-lookup"><span data-stu-id="01735-165">Minimum length of passcode.</span></span> <span data-ttu-id="01735-166">有效值为 4 至 14</span><span class="sxs-lookup"><span data-stu-id="01735-166">Valid values 4 to 14</span></span>|
|<span data-ttu-id="01735-167">passcodeMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="01735-167">passcodeMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="01735-168">Int32</span><span class="sxs-lookup"><span data-stu-id="01735-168">Int32</span></span>|<span data-ttu-id="01735-169">在需要密码之前不活动的分钟数。</span><span class="sxs-lookup"><span data-stu-id="01735-169">Minutes of inactivity before a passcode is required.</span></span>|
|<span data-ttu-id="01735-170">passcodePreviousPasscodeBlockCount</span><span class="sxs-lookup"><span data-stu-id="01735-170">passcodePreviousPasscodeBlockCount</span></span>|<span data-ttu-id="01735-171">Int32</span><span class="sxs-lookup"><span data-stu-id="01735-171">Int32</span></span>|<span data-ttu-id="01735-172">要阻止的以前密码的数量。</span><span class="sxs-lookup"><span data-stu-id="01735-172">Number of previous passcodes to block.</span></span> <span data-ttu-id="01735-173">有效值为 1 至 24</span><span class="sxs-lookup"><span data-stu-id="01735-173">Valid values 1 to 24</span></span>|
|<span data-ttu-id="01735-174">passcodeMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="01735-174">passcodeMinimumCharacterSetCount</span></span>|<span data-ttu-id="01735-175">Int32</span><span class="sxs-lookup"><span data-stu-id="01735-175">Int32</span></span>|<span data-ttu-id="01735-176">密码中必需的字符集数。</span><span class="sxs-lookup"><span data-stu-id="01735-176">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="01735-177">passcodeRequiredType</span><span class="sxs-lookup"><span data-stu-id="01735-177">passcodeRequiredType</span></span>|[<span data-ttu-id="01735-178">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="01735-178">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="01735-179">必需的密码类型。</span><span class="sxs-lookup"><span data-stu-id="01735-179">The required passcode type.</span></span> <span data-ttu-id="01735-180">可取值为：`deviceDefault`、`alphanumeric`、`numeric`。</span><span class="sxs-lookup"><span data-stu-id="01735-180">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="01735-181">passcodeRequired</span><span class="sxs-lookup"><span data-stu-id="01735-181">passcodeRequired</span></span>|<span data-ttu-id="01735-182">Boolean</span><span class="sxs-lookup"><span data-stu-id="01735-182">Boolean</span></span>|<span data-ttu-id="01735-183">指示是否需要密码。</span><span class="sxs-lookup"><span data-stu-id="01735-183">Indicates whether or not to require a passcode.</span></span>|
|<span data-ttu-id="01735-184">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="01735-184">osMinimumVersion</span></span>|<span data-ttu-id="01735-185">String</span><span class="sxs-lookup"><span data-stu-id="01735-185">String</span></span>|<span data-ttu-id="01735-186">最低 IOS 版本。</span><span class="sxs-lookup"><span data-stu-id="01735-186">Minimum IOS version.</span></span>|
|<span data-ttu-id="01735-187">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="01735-187">osMaximumVersion</span></span>|<span data-ttu-id="01735-188">String</span><span class="sxs-lookup"><span data-stu-id="01735-188">String</span></span>|<span data-ttu-id="01735-189">最高 IOS 版本。</span><span class="sxs-lookup"><span data-stu-id="01735-189">Maximum IOS version.</span></span>|
|<span data-ttu-id="01735-190">securityBlockJailbrokenDevices</span><span class="sxs-lookup"><span data-stu-id="01735-190">securityBlockJailbrokenDevices</span></span>|<span data-ttu-id="01735-191">Boolean</span><span class="sxs-lookup"><span data-stu-id="01735-191">Boolean</span></span>|<span data-ttu-id="01735-192">设备不得越狱或取得 root 权限。</span><span class="sxs-lookup"><span data-stu-id="01735-192">Devices must not be jailbroken or rooted.</span></span>|
|<span data-ttu-id="01735-193">deviceThreatProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="01735-193">deviceThreatProtectionEnabled</span></span>|<span data-ttu-id="01735-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="01735-194">Boolean</span></span>|<span data-ttu-id="01735-195">要求设备已启用设备威胁防护。</span><span class="sxs-lookup"><span data-stu-id="01735-195">Require that devices have enabled device threat protection .</span></span>|
|<span data-ttu-id="01735-196">deviceThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="01735-196">deviceThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="01735-197">deviceThreatProtectionLevel</span><span class="sxs-lookup"><span data-stu-id="01735-197">deviceThreatProtectionLevel</span></span>](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|<span data-ttu-id="01735-198">要求移动威胁防护最低风险级别来报告不符合情况。</span><span class="sxs-lookup"><span data-stu-id="01735-198">Require Mobile Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="01735-199">可取值为：`unavailable`、`secured`、`low`、`medium`、`high`、`notSet`。</span><span class="sxs-lookup"><span data-stu-id="01735-199">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="01735-200">managedEmailProfileRequired</span><span class="sxs-lookup"><span data-stu-id="01735-200">managedEmailProfileRequired</span></span>|<span data-ttu-id="01735-201">Boolean</span><span class="sxs-lookup"><span data-stu-id="01735-201">Boolean</span></span>|<span data-ttu-id="01735-202">指示是否需要托管电子邮件配置文件。</span><span class="sxs-lookup"><span data-stu-id="01735-202">Indicates whether or not to require a managed email profile.</span></span>|



## <a name="response"></a><span data-ttu-id="01735-203">响应</span><span class="sxs-lookup"><span data-stu-id="01735-203">Response</span></span>
<span data-ttu-id="01735-204">如果成功，此方法将在响应正文中返回 `201 Created` 响应代码和 [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="01735-204">If successful, this method returns a `201 Created` response code and a [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="01735-205">示例</span><span class="sxs-lookup"><span data-stu-id="01735-205">Example</span></span>

### <a name="request"></a><span data-ttu-id="01735-206">请求</span><span class="sxs-lookup"><span data-stu-id="01735-206">Request</span></span>
<span data-ttu-id="01735-207">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="01735-207">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies
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

### <a name="response"></a><span data-ttu-id="01735-208">响应</span><span class="sxs-lookup"><span data-stu-id="01735-208">Response</span></span>
<span data-ttu-id="01735-p113">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="01735-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




