---
title: 创建 macOSCompliancePolicy
description: 创建新的 macOSCompliancePolicy 对象。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 113642efee7673c0d211a2f9cc5fe7c05d37607b
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27987879"
---
# <a name="create-macoscompliancepolicy"></a><span data-ttu-id="73839-103">创建 macOSCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="73839-103">Create macOSCompliancePolicy</span></span>

> <span data-ttu-id="73839-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="73839-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="73839-105">创建新的 [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="73839-105">Create a new [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="73839-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="73839-106">Prerequisites</span></span>
<span data-ttu-id="73839-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="73839-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="73839-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="73839-109">Permission type</span></span>|<span data-ttu-id="73839-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="73839-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="73839-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="73839-111">Delegated (work or school account)</span></span>|<span data-ttu-id="73839-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="73839-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="73839-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="73839-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="73839-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="73839-114">Not supported.</span></span>|
|<span data-ttu-id="73839-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="73839-115">Application</span></span>|<span data-ttu-id="73839-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="73839-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="73839-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="73839-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="73839-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="73839-118">Request headers</span></span>
|<span data-ttu-id="73839-119">标头</span><span class="sxs-lookup"><span data-stu-id="73839-119">Header</span></span>|<span data-ttu-id="73839-120">值</span><span class="sxs-lookup"><span data-stu-id="73839-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="73839-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="73839-121">Authorization</span></span>|<span data-ttu-id="73839-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="73839-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="73839-123">Accept</span><span class="sxs-lookup"><span data-stu-id="73839-123">Accept</span></span>|<span data-ttu-id="73839-124">application/json</span><span class="sxs-lookup"><span data-stu-id="73839-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="73839-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="73839-125">Request body</span></span>
<span data-ttu-id="73839-126">在请求正文中，提供 macOSCompliancePolicy 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="73839-126">In the request body, supply a JSON representation for the macOSCompliancePolicy object.</span></span>

<span data-ttu-id="73839-127">下表显示创建 macOSCompliancePolicy 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="73839-127">The following table shows the properties that are required when you create the macOSCompliancePolicy.</span></span>

|<span data-ttu-id="73839-128">属性</span><span class="sxs-lookup"><span data-stu-id="73839-128">Property</span></span>|<span data-ttu-id="73839-129">类型</span><span class="sxs-lookup"><span data-stu-id="73839-129">Type</span></span>|<span data-ttu-id="73839-130">说明</span><span class="sxs-lookup"><span data-stu-id="73839-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="73839-131">id</span><span class="sxs-lookup"><span data-stu-id="73839-131">id</span></span>|<span data-ttu-id="73839-132">String</span><span class="sxs-lookup"><span data-stu-id="73839-132">String</span></span>|<span data-ttu-id="73839-133">实体的键。</span><span class="sxs-lookup"><span data-stu-id="73839-133">Key of the entity.</span></span> <span data-ttu-id="73839-134">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="73839-134">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="73839-135">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="73839-135">createdDateTime</span></span>|<span data-ttu-id="73839-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="73839-136">DateTimeOffset</span></span>|<span data-ttu-id="73839-137">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="73839-137">DateTime the object was created.</span></span> <span data-ttu-id="73839-138">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="73839-138">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="73839-139">description</span><span class="sxs-lookup"><span data-stu-id="73839-139">description</span></span>|<span data-ttu-id="73839-140">String</span><span class="sxs-lookup"><span data-stu-id="73839-140">String</span></span>|<span data-ttu-id="73839-141">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="73839-141">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="73839-142">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="73839-142">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="73839-143">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="73839-143">lastModifiedDateTime</span></span>|<span data-ttu-id="73839-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="73839-144">DateTimeOffset</span></span>|<span data-ttu-id="73839-145">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="73839-145">DateTime the object was last modified.</span></span> <span data-ttu-id="73839-146">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="73839-146">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="73839-147">displayName</span><span class="sxs-lookup"><span data-stu-id="73839-147">displayName</span></span>|<span data-ttu-id="73839-148">String</span><span class="sxs-lookup"><span data-stu-id="73839-148">String</span></span>|<span data-ttu-id="73839-149">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="73839-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="73839-150">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="73839-150">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="73839-151">version</span><span class="sxs-lookup"><span data-stu-id="73839-151">version</span></span>|<span data-ttu-id="73839-152">Int32</span><span class="sxs-lookup"><span data-stu-id="73839-152">Int32</span></span>|<span data-ttu-id="73839-153">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="73839-153">Version of the device configuration.</span></span> <span data-ttu-id="73839-154">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="73839-154">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="73839-155">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="73839-155">passwordRequired</span></span>|<span data-ttu-id="73839-156">Boolean</span><span class="sxs-lookup"><span data-stu-id="73839-156">Boolean</span></span>|<span data-ttu-id="73839-157">是否需要密码。</span><span class="sxs-lookup"><span data-stu-id="73839-157">Whether or not to require a password.</span></span>|
|<span data-ttu-id="73839-158">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="73839-158">passwordBlockSimple</span></span>|<span data-ttu-id="73839-159">Boolean</span><span class="sxs-lookup"><span data-stu-id="73839-159">Boolean</span></span>|<span data-ttu-id="73839-160">指示是否阻止简单密码。</span><span class="sxs-lookup"><span data-stu-id="73839-160">Indicates whether or not to block simple passwords.</span></span>|
|<span data-ttu-id="73839-161">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="73839-161">passwordExpirationDays</span></span>|<span data-ttu-id="73839-162">Int32</span><span class="sxs-lookup"><span data-stu-id="73839-162">Int32</span></span>|<span data-ttu-id="73839-163">密码过期前的天数。</span><span class="sxs-lookup"><span data-stu-id="73839-163">Number of days before the password expires.</span></span> <span data-ttu-id="73839-164">有效值为 1 至 65535</span><span class="sxs-lookup"><span data-stu-id="73839-164">Valid values 1 to 65535</span></span>|
|<span data-ttu-id="73839-165">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="73839-165">passwordMinimumLength</span></span>|<span data-ttu-id="73839-166">Int32</span><span class="sxs-lookup"><span data-stu-id="73839-166">Int32</span></span>|<span data-ttu-id="73839-167">密码的最小长度。</span><span class="sxs-lookup"><span data-stu-id="73839-167">Minimum length of password.</span></span> <span data-ttu-id="73839-168">有效值为 4 至 14</span><span class="sxs-lookup"><span data-stu-id="73839-168">Valid values 4 to 14</span></span>|
|<span data-ttu-id="73839-169">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="73839-169">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="73839-170">Int32</span><span class="sxs-lookup"><span data-stu-id="73839-170">Int32</span></span>|<span data-ttu-id="73839-171">在需要密码之前不活动的分钟数。</span><span class="sxs-lookup"><span data-stu-id="73839-171">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="73839-172">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="73839-172">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="73839-173">Int32</span><span class="sxs-lookup"><span data-stu-id="73839-173">Int32</span></span>|<span data-ttu-id="73839-174">要阻止的以前密码的数量。</span><span class="sxs-lookup"><span data-stu-id="73839-174">Number of previous passwords to block.</span></span> <span data-ttu-id="73839-175">有效值为 1 至 24</span><span class="sxs-lookup"><span data-stu-id="73839-175">Valid values 1 to 24</span></span>|
|<span data-ttu-id="73839-176">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="73839-176">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="73839-177">Int32</span><span class="sxs-lookup"><span data-stu-id="73839-177">Int32</span></span>|<span data-ttu-id="73839-178">密码中必需的字符集数。</span><span class="sxs-lookup"><span data-stu-id="73839-178">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="73839-179">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="73839-179">passwordRequiredType</span></span>|[<span data-ttu-id="73839-180">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="73839-180">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="73839-181">必需的密码类型。</span><span class="sxs-lookup"><span data-stu-id="73839-181">The required password type.</span></span> <span data-ttu-id="73839-182">可取值为：`deviceDefault`、`alphanumeric`、`numeric`。</span><span class="sxs-lookup"><span data-stu-id="73839-182">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="73839-183">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="73839-183">osMinimumVersion</span></span>|<span data-ttu-id="73839-184">String</span><span class="sxs-lookup"><span data-stu-id="73839-184">String</span></span>|<span data-ttu-id="73839-185">最低 IOS 版本。</span><span class="sxs-lookup"><span data-stu-id="73839-185">Minimum IOS version.</span></span>|
|<span data-ttu-id="73839-186">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="73839-186">osMaximumVersion</span></span>|<span data-ttu-id="73839-187">String</span><span class="sxs-lookup"><span data-stu-id="73839-187">String</span></span>|<span data-ttu-id="73839-188">最高 IOS 版本。</span><span class="sxs-lookup"><span data-stu-id="73839-188">Maximum IOS version.</span></span>|
|<span data-ttu-id="73839-189">systemIntegrityProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="73839-189">systemIntegrityProtectionEnabled</span></span>|<span data-ttu-id="73839-190">Boolean</span><span class="sxs-lookup"><span data-stu-id="73839-190">Boolean</span></span>|<span data-ttu-id="73839-191">要求设备已启用系统完整性保护。</span><span class="sxs-lookup"><span data-stu-id="73839-191">Require that devices have enabled system integrity protection.</span></span>|
|<span data-ttu-id="73839-192">deviceThreatProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="73839-192">deviceThreatProtectionEnabled</span></span>|<span data-ttu-id="73839-193">Boolean</span><span class="sxs-lookup"><span data-stu-id="73839-193">Boolean</span></span>|<span data-ttu-id="73839-194">要求设备已启用设备威胁防护。</span><span class="sxs-lookup"><span data-stu-id="73839-194">Require that devices have enabled device threat protection .</span></span>|
|<span data-ttu-id="73839-195">deviceThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="73839-195">deviceThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="73839-196">deviceThreatProtectionLevel</span><span class="sxs-lookup"><span data-stu-id="73839-196">deviceThreatProtectionLevel</span></span>](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|<span data-ttu-id="73839-197">要求移动威胁防护最低风险级别来报告不符合情况。</span><span class="sxs-lookup"><span data-stu-id="73839-197">Require Mobile Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="73839-198">可取值为：`unavailable`、`secured`、`low`、`medium`、`high`、`notSet`。</span><span class="sxs-lookup"><span data-stu-id="73839-198">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="73839-199">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="73839-199">storageRequireEncryption</span></span>|<span data-ttu-id="73839-200">Boolean</span><span class="sxs-lookup"><span data-stu-id="73839-200">Boolean</span></span>|<span data-ttu-id="73839-201">要求对 Mac OS 设备加密。</span><span class="sxs-lookup"><span data-stu-id="73839-201">Require encryption on Mac OS devices.</span></span>|
|<span data-ttu-id="73839-202">firewallEnabled</span><span class="sxs-lookup"><span data-stu-id="73839-202">firewallEnabled</span></span>|<span data-ttu-id="73839-203">Boolean</span><span class="sxs-lookup"><span data-stu-id="73839-203">Boolean</span></span>|<span data-ttu-id="73839-204">是否应启用防火墙，或不。</span><span class="sxs-lookup"><span data-stu-id="73839-204">Whether the firewall should be enabled or not.</span></span>|
|<span data-ttu-id="73839-205">firewallBlockAllIncoming</span><span class="sxs-lookup"><span data-stu-id="73839-205">firewallBlockAllIncoming</span></span>|<span data-ttu-id="73839-206">Boolean</span><span class="sxs-lookup"><span data-stu-id="73839-206">Boolean</span></span>|<span data-ttu-id="73839-207">对应于"阻止所有传入连接"选项。</span><span class="sxs-lookup"><span data-stu-id="73839-207">Corresponds to the “Block all incoming connections” option.</span></span>|
|<span data-ttu-id="73839-208">firewallEnableStealthMode</span><span class="sxs-lookup"><span data-stu-id="73839-208">firewallEnableStealthMode</span></span>|<span data-ttu-id="73839-209">Boolean</span><span class="sxs-lookup"><span data-stu-id="73839-209">Boolean</span></span>|<span data-ttu-id="73839-210">对应于"启用隐藏模式"。</span><span class="sxs-lookup"><span data-stu-id="73839-210">Corresponds to “Enable stealth mode.”</span></span>|



## <a name="response"></a><span data-ttu-id="73839-211">响应</span><span class="sxs-lookup"><span data-stu-id="73839-211">Response</span></span>
<span data-ttu-id="73839-212">如果成功，此方法会在响应正文中返回 `201 Created` 响应代码和 [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="73839-212">If successful, this method returns a `201 Created` response code and a [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="73839-213">示例</span><span class="sxs-lookup"><span data-stu-id="73839-213">Example</span></span>
### <a name="request"></a><span data-ttu-id="73839-214">请求</span><span class="sxs-lookup"><span data-stu-id="73839-214">Request</span></span>
<span data-ttu-id="73839-215">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="73839-215">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies
Content-type: application/json
Content-length: 849

{
  "@odata.type": "#microsoft.graph.macOSCompliancePolicy",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "passwordRequired": true,
  "passwordBlockSimple": true,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeLock": 5,
  "passwordPreviousPasswordBlockCount": 2,
  "passwordMinimumCharacterSetCount": 0,
  "passwordRequiredType": "alphanumeric",
  "osMinimumVersion": "Os Minimum Version value",
  "osMaximumVersion": "Os Maximum Version value",
  "systemIntegrityProtectionEnabled": true,
  "deviceThreatProtectionEnabled": true,
  "deviceThreatProtectionRequiredSecurityLevel": "secured",
  "storageRequireEncryption": true,
  "firewallEnabled": true,
  "firewallBlockAllIncoming": true,
  "firewallEnableStealthMode": true
}
```

### <a name="response"></a><span data-ttu-id="73839-216">响应</span><span class="sxs-lookup"><span data-stu-id="73839-216">Response</span></span>
<span data-ttu-id="73839-p113">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="73839-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1021

{
  "@odata.type": "#microsoft.graph.macOSCompliancePolicy",
  "id": "ddbadff3-dff3-ddba-f3df-baddf3dfbadd",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "version": 7,
  "passwordRequired": true,
  "passwordBlockSimple": true,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeLock": 5,
  "passwordPreviousPasswordBlockCount": 2,
  "passwordMinimumCharacterSetCount": 0,
  "passwordRequiredType": "alphanumeric",
  "osMinimumVersion": "Os Minimum Version value",
  "osMaximumVersion": "Os Maximum Version value",
  "systemIntegrityProtectionEnabled": true,
  "deviceThreatProtectionEnabled": true,
  "deviceThreatProtectionRequiredSecurityLevel": "secured",
  "storageRequireEncryption": true,
  "firewallEnabled": true,
  "firewallBlockAllIncoming": true,
  "firewallEnableStealthMode": true
}
```



