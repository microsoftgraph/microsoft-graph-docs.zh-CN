---
title: 创建 macOSCompliancePolicy
description: 创建新的 macOSCompliancePolicy 对象。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 42b3ee5cae17b6965f038a6841a5d2ac1330f374
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/02/2019
ms.locfileid: "37366130"
---
# <a name="create-macoscompliancepolicy"></a><span data-ttu-id="bedae-103">创建 macOSCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="bedae-103">Create macOSCompliancePolicy</span></span>

> <span data-ttu-id="bedae-104">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="bedae-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bedae-105">创建新的 [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="bedae-105">Create a new [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bedae-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="bedae-106">Prerequisites</span></span>
<span data-ttu-id="bedae-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="bedae-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bedae-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="bedae-109">Permission type</span></span>|<span data-ttu-id="bedae-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="bedae-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bedae-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="bedae-111">Delegated (work or school account)</span></span>|<span data-ttu-id="bedae-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bedae-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="bedae-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="bedae-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bedae-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="bedae-114">Not supported.</span></span>|
|<span data-ttu-id="bedae-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="bedae-115">Application</span></span>|<span data-ttu-id="bedae-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="bedae-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="bedae-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="bedae-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="bedae-118">请求头</span><span class="sxs-lookup"><span data-stu-id="bedae-118">Request headers</span></span>
|<span data-ttu-id="bedae-119">标头</span><span class="sxs-lookup"><span data-stu-id="bedae-119">Header</span></span>|<span data-ttu-id="bedae-120">值</span><span class="sxs-lookup"><span data-stu-id="bedae-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bedae-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="bedae-121">Authorization</span></span>|<span data-ttu-id="bedae-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="bedae-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bedae-123">接受</span><span class="sxs-lookup"><span data-stu-id="bedae-123">Accept</span></span>|<span data-ttu-id="bedae-124">application/json</span><span class="sxs-lookup"><span data-stu-id="bedae-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bedae-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="bedae-125">Request body</span></span>
<span data-ttu-id="bedae-126">在请求正文中，提供 macOSCompliancePolicy 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="bedae-126">In the request body, supply a JSON representation for the macOSCompliancePolicy object.</span></span>

<span data-ttu-id="bedae-127">下表显示创建 macOSCompliancePolicy 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="bedae-127">The following table shows the properties that are required when you create the macOSCompliancePolicy.</span></span>

|<span data-ttu-id="bedae-128">属性</span><span class="sxs-lookup"><span data-stu-id="bedae-128">Property</span></span>|<span data-ttu-id="bedae-129">类型</span><span class="sxs-lookup"><span data-stu-id="bedae-129">Type</span></span>|<span data-ttu-id="bedae-130">说明</span><span class="sxs-lookup"><span data-stu-id="bedae-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bedae-131">id</span><span class="sxs-lookup"><span data-stu-id="bedae-131">id</span></span>|<span data-ttu-id="bedae-132">字符串</span><span class="sxs-lookup"><span data-stu-id="bedae-132">String</span></span>|<span data-ttu-id="bedae-133">实体的键。</span><span class="sxs-lookup"><span data-stu-id="bedae-133">Key of the entity.</span></span> <span data-ttu-id="bedae-134">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="bedae-134">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="bedae-135">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="bedae-135">createdDateTime</span></span>|<span data-ttu-id="bedae-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bedae-136">DateTimeOffset</span></span>|<span data-ttu-id="bedae-137">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="bedae-137">DateTime the object was created.</span></span> <span data-ttu-id="bedae-138">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="bedae-138">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="bedae-139">说明</span><span class="sxs-lookup"><span data-stu-id="bedae-139">description</span></span>|<span data-ttu-id="bedae-140">String</span><span class="sxs-lookup"><span data-stu-id="bedae-140">String</span></span>|<span data-ttu-id="bedae-141">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="bedae-141">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="bedae-142">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="bedae-142">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="bedae-143">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="bedae-143">lastModifiedDateTime</span></span>|<span data-ttu-id="bedae-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bedae-144">DateTimeOffset</span></span>|<span data-ttu-id="bedae-145">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="bedae-145">DateTime the object was last modified.</span></span> <span data-ttu-id="bedae-146">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="bedae-146">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="bedae-147">displayName</span><span class="sxs-lookup"><span data-stu-id="bedae-147">displayName</span></span>|<span data-ttu-id="bedae-148">String</span><span class="sxs-lookup"><span data-stu-id="bedae-148">String</span></span>|<span data-ttu-id="bedae-149">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="bedae-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="bedae-150">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="bedae-150">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="bedae-151">version</span><span class="sxs-lookup"><span data-stu-id="bedae-151">version</span></span>|<span data-ttu-id="bedae-152">Int32</span><span class="sxs-lookup"><span data-stu-id="bedae-152">Int32</span></span>|<span data-ttu-id="bedae-153">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="bedae-153">Version of the device configuration.</span></span> <span data-ttu-id="bedae-154">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="bedae-154">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="bedae-155">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="bedae-155">passwordRequired</span></span>|<span data-ttu-id="bedae-156">Boolean</span><span class="sxs-lookup"><span data-stu-id="bedae-156">Boolean</span></span>|<span data-ttu-id="bedae-157">是否需要密码。</span><span class="sxs-lookup"><span data-stu-id="bedae-157">Whether or not to require a password.</span></span>|
|<span data-ttu-id="bedae-158">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="bedae-158">passwordBlockSimple</span></span>|<span data-ttu-id="bedae-159">Boolean</span><span class="sxs-lookup"><span data-stu-id="bedae-159">Boolean</span></span>|<span data-ttu-id="bedae-160">指示是否阻止简单密码。</span><span class="sxs-lookup"><span data-stu-id="bedae-160">Indicates whether or not to block simple passwords.</span></span>|
|<span data-ttu-id="bedae-161">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="bedae-161">passwordExpirationDays</span></span>|<span data-ttu-id="bedae-162">Int32</span><span class="sxs-lookup"><span data-stu-id="bedae-162">Int32</span></span>|<span data-ttu-id="bedae-163">密码过期前的天数。</span><span class="sxs-lookup"><span data-stu-id="bedae-163">Number of days before the password expires.</span></span> <span data-ttu-id="bedae-164">有效值为 1 至 65535</span><span class="sxs-lookup"><span data-stu-id="bedae-164">Valid values 1 to 65535</span></span>|
|<span data-ttu-id="bedae-165">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="bedae-165">passwordMinimumLength</span></span>|<span data-ttu-id="bedae-166">Int32</span><span class="sxs-lookup"><span data-stu-id="bedae-166">Int32</span></span>|<span data-ttu-id="bedae-167">密码的最小长度。</span><span class="sxs-lookup"><span data-stu-id="bedae-167">Minimum length of password.</span></span> <span data-ttu-id="bedae-168">有效值为 4 至 14</span><span class="sxs-lookup"><span data-stu-id="bedae-168">Valid values 4 to 14</span></span>|
|<span data-ttu-id="bedae-169">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="bedae-169">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="bedae-170">Int32</span><span class="sxs-lookup"><span data-stu-id="bedae-170">Int32</span></span>|<span data-ttu-id="bedae-171">在需要密码之前不活动的分钟数。</span><span class="sxs-lookup"><span data-stu-id="bedae-171">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="bedae-172">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="bedae-172">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="bedae-173">Int32</span><span class="sxs-lookup"><span data-stu-id="bedae-173">Int32</span></span>|<span data-ttu-id="bedae-174">要阻止的以前密码的数量。</span><span class="sxs-lookup"><span data-stu-id="bedae-174">Number of previous passwords to block.</span></span> <span data-ttu-id="bedae-175">有效值为 1 至 24</span><span class="sxs-lookup"><span data-stu-id="bedae-175">Valid values 1 to 24</span></span>|
|<span data-ttu-id="bedae-176">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="bedae-176">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="bedae-177">Int32</span><span class="sxs-lookup"><span data-stu-id="bedae-177">Int32</span></span>|<span data-ttu-id="bedae-178">密码中必需的字符集数。</span><span class="sxs-lookup"><span data-stu-id="bedae-178">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="bedae-179">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="bedae-179">passwordRequiredType</span></span>|[<span data-ttu-id="bedae-180">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="bedae-180">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="bedae-181">必需的密码类型。</span><span class="sxs-lookup"><span data-stu-id="bedae-181">The required password type.</span></span> <span data-ttu-id="bedae-182">可取值为：`deviceDefault`、`alphanumeric`、`numeric`。</span><span class="sxs-lookup"><span data-stu-id="bedae-182">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="bedae-183">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="bedae-183">osMinimumVersion</span></span>|<span data-ttu-id="bedae-184">String</span><span class="sxs-lookup"><span data-stu-id="bedae-184">String</span></span>|<span data-ttu-id="bedae-185">最低 MacOS 版本。</span><span class="sxs-lookup"><span data-stu-id="bedae-185">Minimum MacOS version.</span></span>|
|<span data-ttu-id="bedae-186">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="bedae-186">osMaximumVersion</span></span>|<span data-ttu-id="bedae-187">String</span><span class="sxs-lookup"><span data-stu-id="bedae-187">String</span></span>|<span data-ttu-id="bedae-188">最大 MacOS 版本。</span><span class="sxs-lookup"><span data-stu-id="bedae-188">Maximum MacOS version.</span></span>|
|<span data-ttu-id="bedae-189">systemIntegrityProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="bedae-189">systemIntegrityProtectionEnabled</span></span>|<span data-ttu-id="bedae-190">Boolean</span><span class="sxs-lookup"><span data-stu-id="bedae-190">Boolean</span></span>|<span data-ttu-id="bedae-191">要求设备已启用系统完整性保护。</span><span class="sxs-lookup"><span data-stu-id="bedae-191">Require that devices have enabled system integrity protection.</span></span>|
|<span data-ttu-id="bedae-192">deviceThreatProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="bedae-192">deviceThreatProtectionEnabled</span></span>|<span data-ttu-id="bedae-193">Boolean</span><span class="sxs-lookup"><span data-stu-id="bedae-193">Boolean</span></span>|<span data-ttu-id="bedae-194">要求设备已启用设备威胁防护。</span><span class="sxs-lookup"><span data-stu-id="bedae-194">Require that devices have enabled device threat protection.</span></span>|
|<span data-ttu-id="bedae-195">deviceThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="bedae-195">deviceThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="bedae-196">deviceThreatProtectionLevel</span><span class="sxs-lookup"><span data-stu-id="bedae-196">deviceThreatProtectionLevel</span></span>](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|<span data-ttu-id="bedae-197">要求移动威胁防护最低风险级别来报告不符合情况。</span><span class="sxs-lookup"><span data-stu-id="bedae-197">Require Mobile Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="bedae-198">可取值为：`unavailable`、`secured`、`low`、`medium`、`high`、`notSet`。</span><span class="sxs-lookup"><span data-stu-id="bedae-198">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="bedae-199">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="bedae-199">storageRequireEncryption</span></span>|<span data-ttu-id="bedae-200">Boolean</span><span class="sxs-lookup"><span data-stu-id="bedae-200">Boolean</span></span>|<span data-ttu-id="bedae-201">要求对 Mac OS 设备加密。</span><span class="sxs-lookup"><span data-stu-id="bedae-201">Require encryption on Mac OS devices.</span></span>|
|<span data-ttu-id="bedae-202">firewallEnabled</span><span class="sxs-lookup"><span data-stu-id="bedae-202">firewallEnabled</span></span>|<span data-ttu-id="bedae-203">Boolean</span><span class="sxs-lookup"><span data-stu-id="bedae-203">Boolean</span></span>|<span data-ttu-id="bedae-204">是否应启用防火墙。</span><span class="sxs-lookup"><span data-stu-id="bedae-204">Whether the firewall should be enabled or not.</span></span>|
|<span data-ttu-id="bedae-205">firewallBlockAllIncoming</span><span class="sxs-lookup"><span data-stu-id="bedae-205">firewallBlockAllIncoming</span></span>|<span data-ttu-id="bedae-206">Boolean</span><span class="sxs-lookup"><span data-stu-id="bedae-206">Boolean</span></span>|<span data-ttu-id="bedae-207">对应于 "阻止所有传入连接" 选项。</span><span class="sxs-lookup"><span data-stu-id="bedae-207">Corresponds to the “Block all incoming connections” option.</span></span>|
|<span data-ttu-id="bedae-208">firewallEnableStealthMode</span><span class="sxs-lookup"><span data-stu-id="bedae-208">firewallEnableStealthMode</span></span>|<span data-ttu-id="bedae-209">Boolean</span><span class="sxs-lookup"><span data-stu-id="bedae-209">Boolean</span></span>|<span data-ttu-id="bedae-210">对应于 "启用隐形模式"。</span><span class="sxs-lookup"><span data-stu-id="bedae-210">Corresponds to “Enable stealth mode.”</span></span>|



## <a name="response"></a><span data-ttu-id="bedae-211">响应</span><span class="sxs-lookup"><span data-stu-id="bedae-211">Response</span></span>
<span data-ttu-id="bedae-212">如果成功，此方法会在响应正文中返回 `201 Created` 响应代码和 [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="bedae-212">If successful, this method returns a `201 Created` response code and a [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bedae-213">示例</span><span class="sxs-lookup"><span data-stu-id="bedae-213">Example</span></span>

### <a name="request"></a><span data-ttu-id="bedae-214">请求</span><span class="sxs-lookup"><span data-stu-id="bedae-214">Request</span></span>
<span data-ttu-id="bedae-215">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="bedae-215">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="bedae-216">响应</span><span class="sxs-lookup"><span data-stu-id="bedae-216">Response</span></span>
<span data-ttu-id="bedae-p113">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="bedae-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




