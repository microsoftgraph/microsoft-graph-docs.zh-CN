---
title: 创建 iosCompliancePolicy
description: 创建新的 iosCompliancePolicy 对象。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 51f0658ab4e1da860048b70ca1c168d8798c173b
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42514639"
---
# <a name="create-ioscompliancepolicy"></a><span data-ttu-id="496f0-103">创建 iosCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="496f0-103">Create iosCompliancePolicy</span></span>

<span data-ttu-id="496f0-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="496f0-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="496f0-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="496f0-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="496f0-106">创建新的 [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="496f0-106">Create a new [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="496f0-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="496f0-107">Prerequisites</span></span>
<span data-ttu-id="496f0-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="496f0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="496f0-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="496f0-110">Permission type</span></span>|<span data-ttu-id="496f0-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="496f0-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="496f0-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="496f0-112">Delegated (work or school account)</span></span>|<span data-ttu-id="496f0-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="496f0-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="496f0-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="496f0-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="496f0-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="496f0-115">Not supported.</span></span>|
|<span data-ttu-id="496f0-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="496f0-116">Application</span></span>|<span data-ttu-id="496f0-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="496f0-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="496f0-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="496f0-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="496f0-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="496f0-119">Request headers</span></span>
|<span data-ttu-id="496f0-120">标头</span><span class="sxs-lookup"><span data-stu-id="496f0-120">Header</span></span>|<span data-ttu-id="496f0-121">值</span><span class="sxs-lookup"><span data-stu-id="496f0-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="496f0-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="496f0-122">Authorization</span></span>|<span data-ttu-id="496f0-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="496f0-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="496f0-124">接受</span><span class="sxs-lookup"><span data-stu-id="496f0-124">Accept</span></span>|<span data-ttu-id="496f0-125">application/json</span><span class="sxs-lookup"><span data-stu-id="496f0-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="496f0-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="496f0-126">Request body</span></span>
<span data-ttu-id="496f0-127">在请求正文中，提供 iosCompliancePolicy 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="496f0-127">In the request body, supply a JSON representation for the iosCompliancePolicy object.</span></span>

<span data-ttu-id="496f0-128">下表显示了创建 iosCompliancePolicy 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="496f0-128">The following table shows the properties that are required when you create the iosCompliancePolicy.</span></span>

|<span data-ttu-id="496f0-129">属性</span><span class="sxs-lookup"><span data-stu-id="496f0-129">Property</span></span>|<span data-ttu-id="496f0-130">类型</span><span class="sxs-lookup"><span data-stu-id="496f0-130">Type</span></span>|<span data-ttu-id="496f0-131">说明</span><span class="sxs-lookup"><span data-stu-id="496f0-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="496f0-132">说明</span><span class="sxs-lookup"><span data-stu-id="496f0-132">description</span></span>|<span data-ttu-id="496f0-133">字符串</span><span class="sxs-lookup"><span data-stu-id="496f0-133">String</span></span>|<span data-ttu-id="496f0-134">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="496f0-134">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="496f0-135">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="496f0-135">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="496f0-136">displayName</span><span class="sxs-lookup"><span data-stu-id="496f0-136">displayName</span></span>|<span data-ttu-id="496f0-137">字符串</span><span class="sxs-lookup"><span data-stu-id="496f0-137">String</span></span>|<span data-ttu-id="496f0-138">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="496f0-138">Admin provided name of the device configuration.</span></span> <span data-ttu-id="496f0-139">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="496f0-139">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="496f0-140">version</span><span class="sxs-lookup"><span data-stu-id="496f0-140">version</span></span>|<span data-ttu-id="496f0-141">Int32</span><span class="sxs-lookup"><span data-stu-id="496f0-141">Int32</span></span>|<span data-ttu-id="496f0-142">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="496f0-142">Version of the device configuration.</span></span> <span data-ttu-id="496f0-143">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="496f0-143">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="496f0-144">passcodeBlockSimple</span><span class="sxs-lookup"><span data-stu-id="496f0-144">passcodeBlockSimple</span></span>|<span data-ttu-id="496f0-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="496f0-145">Boolean</span></span>|<span data-ttu-id="496f0-146">指示是否阻止简单密码。</span><span class="sxs-lookup"><span data-stu-id="496f0-146">Indicates whether or not to block simple passcodes.</span></span>|
|<span data-ttu-id="496f0-147">passcodeExpirationDays</span><span class="sxs-lookup"><span data-stu-id="496f0-147">passcodeExpirationDays</span></span>|<span data-ttu-id="496f0-148">Int32</span><span class="sxs-lookup"><span data-stu-id="496f0-148">Int32</span></span>|<span data-ttu-id="496f0-149">密码过期前的天数。</span><span class="sxs-lookup"><span data-stu-id="496f0-149">Number of days before the passcode expires.</span></span> <span data-ttu-id="496f0-150">有效值为 1 至 65535</span><span class="sxs-lookup"><span data-stu-id="496f0-150">Valid values 1 to 65535</span></span>|
|<span data-ttu-id="496f0-151">passcodeMinimumLength</span><span class="sxs-lookup"><span data-stu-id="496f0-151">passcodeMinimumLength</span></span>|<span data-ttu-id="496f0-152">Int32</span><span class="sxs-lookup"><span data-stu-id="496f0-152">Int32</span></span>|<span data-ttu-id="496f0-153">密码的最小长度。</span><span class="sxs-lookup"><span data-stu-id="496f0-153">Minimum length of passcode.</span></span> <span data-ttu-id="496f0-154">有效值为 4 至 14</span><span class="sxs-lookup"><span data-stu-id="496f0-154">Valid values 4 to 14</span></span>|
|<span data-ttu-id="496f0-155">passcodeMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="496f0-155">passcodeMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="496f0-156">Int32</span><span class="sxs-lookup"><span data-stu-id="496f0-156">Int32</span></span>|<span data-ttu-id="496f0-157">在需要密码之前不活动的分钟数。</span><span class="sxs-lookup"><span data-stu-id="496f0-157">Minutes of inactivity before a passcode is required.</span></span>|
|<span data-ttu-id="496f0-158">passcodePreviousPasscodeBlockCount</span><span class="sxs-lookup"><span data-stu-id="496f0-158">passcodePreviousPasscodeBlockCount</span></span>|<span data-ttu-id="496f0-159">Int32</span><span class="sxs-lookup"><span data-stu-id="496f0-159">Int32</span></span>|<span data-ttu-id="496f0-160">要阻止的以前密码的数量。</span><span class="sxs-lookup"><span data-stu-id="496f0-160">Number of previous passcodes to block.</span></span> <span data-ttu-id="496f0-161">有效值为 1 至 24</span><span class="sxs-lookup"><span data-stu-id="496f0-161">Valid values 1 to 24</span></span>|
|<span data-ttu-id="496f0-162">passcodeMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="496f0-162">passcodeMinimumCharacterSetCount</span></span>|<span data-ttu-id="496f0-163">Int32</span><span class="sxs-lookup"><span data-stu-id="496f0-163">Int32</span></span>|<span data-ttu-id="496f0-164">密码中必需的字符集数。</span><span class="sxs-lookup"><span data-stu-id="496f0-164">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="496f0-165">passcodeRequiredType</span><span class="sxs-lookup"><span data-stu-id="496f0-165">passcodeRequiredType</span></span>|[<span data-ttu-id="496f0-166">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="496f0-166">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="496f0-167">必需的密码类型。</span><span class="sxs-lookup"><span data-stu-id="496f0-167">The required passcode type.</span></span> <span data-ttu-id="496f0-168">可取值为：`deviceDefault`、`alphanumeric`、`numeric`。</span><span class="sxs-lookup"><span data-stu-id="496f0-168">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="496f0-169">passcodeRequired</span><span class="sxs-lookup"><span data-stu-id="496f0-169">passcodeRequired</span></span>|<span data-ttu-id="496f0-170">Boolean</span><span class="sxs-lookup"><span data-stu-id="496f0-170">Boolean</span></span>|<span data-ttu-id="496f0-171">指示是否需要密码。</span><span class="sxs-lookup"><span data-stu-id="496f0-171">Indicates whether or not to require a passcode.</span></span>|
|<span data-ttu-id="496f0-172">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="496f0-172">osMinimumVersion</span></span>|<span data-ttu-id="496f0-173">字符串</span><span class="sxs-lookup"><span data-stu-id="496f0-173">String</span></span>|<span data-ttu-id="496f0-174">最低 IOS 版本。</span><span class="sxs-lookup"><span data-stu-id="496f0-174">Minimum IOS version.</span></span>|
|<span data-ttu-id="496f0-175">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="496f0-175">osMaximumVersion</span></span>|<span data-ttu-id="496f0-176">String</span><span class="sxs-lookup"><span data-stu-id="496f0-176">String</span></span>|<span data-ttu-id="496f0-177">最高 IOS 版本。</span><span class="sxs-lookup"><span data-stu-id="496f0-177">Maximum IOS version.</span></span>|
|<span data-ttu-id="496f0-178">securityBlockJailbrokenDevices</span><span class="sxs-lookup"><span data-stu-id="496f0-178">securityBlockJailbrokenDevices</span></span>|<span data-ttu-id="496f0-179">Boolean</span><span class="sxs-lookup"><span data-stu-id="496f0-179">Boolean</span></span>|<span data-ttu-id="496f0-180">设备不得越狱或取得 root 权限。</span><span class="sxs-lookup"><span data-stu-id="496f0-180">Devices must not be jailbroken or rooted.</span></span>|
|<span data-ttu-id="496f0-181">deviceThreatProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="496f0-181">deviceThreatProtectionEnabled</span></span>|<span data-ttu-id="496f0-182">Boolean</span><span class="sxs-lookup"><span data-stu-id="496f0-182">Boolean</span></span>|<span data-ttu-id="496f0-183">要求设备已启用设备威胁防护。</span><span class="sxs-lookup"><span data-stu-id="496f0-183">Require that devices have enabled device threat protection .</span></span>|
|<span data-ttu-id="496f0-184">deviceThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="496f0-184">deviceThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="496f0-185">deviceThreatProtectionLevel</span><span class="sxs-lookup"><span data-stu-id="496f0-185">deviceThreatProtectionLevel</span></span>](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|<span data-ttu-id="496f0-186">要求移动威胁防护最低风险级别来报告不符合情况。</span><span class="sxs-lookup"><span data-stu-id="496f0-186">Require Mobile Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="496f0-187">可取值为：`unavailable`、`secured`、`low`、`medium`、`high`、`notSet`。</span><span class="sxs-lookup"><span data-stu-id="496f0-187">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="496f0-188">managedEmailProfileRequired</span><span class="sxs-lookup"><span data-stu-id="496f0-188">managedEmailProfileRequired</span></span>|<span data-ttu-id="496f0-189">Boolean</span><span class="sxs-lookup"><span data-stu-id="496f0-189">Boolean</span></span>|<span data-ttu-id="496f0-190">指示是否需要托管电子邮件配置文件。</span><span class="sxs-lookup"><span data-stu-id="496f0-190">Indicates whether or not to require a managed email profile.</span></span>|



## <a name="response"></a><span data-ttu-id="496f0-191">响应</span><span class="sxs-lookup"><span data-stu-id="496f0-191">Response</span></span>
<span data-ttu-id="496f0-192">如果成功，此方法将在响应正文中返回 `201 Created` 响应代码和 [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="496f0-192">If successful, this method returns a `201 Created` response code and a [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="496f0-193">示例</span><span class="sxs-lookup"><span data-stu-id="496f0-193">Example</span></span>

### <a name="request"></a><span data-ttu-id="496f0-194">请求</span><span class="sxs-lookup"><span data-stu-id="496f0-194">Request</span></span>
<span data-ttu-id="496f0-195">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="496f0-195">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="496f0-196">响应</span><span class="sxs-lookup"><span data-stu-id="496f0-196">Response</span></span>
<span data-ttu-id="496f0-p110">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="496f0-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




