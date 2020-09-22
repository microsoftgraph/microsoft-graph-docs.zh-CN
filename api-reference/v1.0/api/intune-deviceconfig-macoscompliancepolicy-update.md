---
title: 更新 macOSCompliancePolicy
description: 更新 macOSCompliancePolicy 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 56913d9acd753399e963d606f3994734b9afcae0
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48073150"
---
# <a name="update-macoscompliancepolicy"></a><span data-ttu-id="d851d-103">更新 macOSCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="d851d-103">Update macOSCompliancePolicy</span></span>

<span data-ttu-id="d851d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d851d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d851d-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d851d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d851d-106">更新 [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="d851d-106">Update the properties of a [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d851d-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="d851d-107">Prerequisites</span></span>
<span data-ttu-id="d851d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d851d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d851d-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="d851d-110">Permission type</span></span>|<span data-ttu-id="d851d-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="d851d-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d851d-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d851d-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d851d-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d851d-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d851d-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d851d-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d851d-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="d851d-115">Not supported.</span></span>|
|<span data-ttu-id="d851d-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="d851d-116">Application</span></span>|<span data-ttu-id="d851d-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="d851d-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d851d-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d851d-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="d851d-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="d851d-119">Request headers</span></span>
|<span data-ttu-id="d851d-120">标头</span><span class="sxs-lookup"><span data-stu-id="d851d-120">Header</span></span>|<span data-ttu-id="d851d-121">值</span><span class="sxs-lookup"><span data-stu-id="d851d-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d851d-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="d851d-122">Authorization</span></span>|<span data-ttu-id="d851d-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="d851d-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d851d-124">接受</span><span class="sxs-lookup"><span data-stu-id="d851d-124">Accept</span></span>|<span data-ttu-id="d851d-125">application/json</span><span class="sxs-lookup"><span data-stu-id="d851d-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d851d-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="d851d-126">Request body</span></span>
<span data-ttu-id="d851d-127">在请求正文中，提供 [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d851d-127">In the request body, supply a JSON representation for the [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) object.</span></span>

<span data-ttu-id="d851d-128">下表显示创建 [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="d851d-128">The following table shows the properties that are required when you create the [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md).</span></span>

|<span data-ttu-id="d851d-129">属性</span><span class="sxs-lookup"><span data-stu-id="d851d-129">Property</span></span>|<span data-ttu-id="d851d-130">类型</span><span class="sxs-lookup"><span data-stu-id="d851d-130">Type</span></span>|<span data-ttu-id="d851d-131">说明</span><span class="sxs-lookup"><span data-stu-id="d851d-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d851d-132">id</span><span class="sxs-lookup"><span data-stu-id="d851d-132">id</span></span>|<span data-ttu-id="d851d-133">String</span><span class="sxs-lookup"><span data-stu-id="d851d-133">String</span></span>|<span data-ttu-id="d851d-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="d851d-134">Key of the entity.</span></span> <span data-ttu-id="d851d-135">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="d851d-135">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="d851d-136">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d851d-136">createdDateTime</span></span>|<span data-ttu-id="d851d-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d851d-137">DateTimeOffset</span></span>|<span data-ttu-id="d851d-138">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="d851d-138">DateTime the object was created.</span></span> <span data-ttu-id="d851d-139">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="d851d-139">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="d851d-140">description</span><span class="sxs-lookup"><span data-stu-id="d851d-140">description</span></span>|<span data-ttu-id="d851d-141">String</span><span class="sxs-lookup"><span data-stu-id="d851d-141">String</span></span>|<span data-ttu-id="d851d-142">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="d851d-142">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="d851d-143">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="d851d-143">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="d851d-144">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d851d-144">lastModifiedDateTime</span></span>|<span data-ttu-id="d851d-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d851d-145">DateTimeOffset</span></span>|<span data-ttu-id="d851d-146">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="d851d-146">DateTime the object was last modified.</span></span> <span data-ttu-id="d851d-147">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="d851d-147">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="d851d-148">displayName</span><span class="sxs-lookup"><span data-stu-id="d851d-148">displayName</span></span>|<span data-ttu-id="d851d-149">String</span><span class="sxs-lookup"><span data-stu-id="d851d-149">String</span></span>|<span data-ttu-id="d851d-150">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="d851d-150">Admin provided name of the device configuration.</span></span> <span data-ttu-id="d851d-151">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="d851d-151">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="d851d-152">version</span><span class="sxs-lookup"><span data-stu-id="d851d-152">version</span></span>|<span data-ttu-id="d851d-153">Int32</span><span class="sxs-lookup"><span data-stu-id="d851d-153">Int32</span></span>|<span data-ttu-id="d851d-154">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="d851d-154">Version of the device configuration.</span></span> <span data-ttu-id="d851d-155">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="d851d-155">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="d851d-156">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="d851d-156">passwordRequired</span></span>|<span data-ttu-id="d851d-157">Boolean</span><span class="sxs-lookup"><span data-stu-id="d851d-157">Boolean</span></span>|<span data-ttu-id="d851d-158">是否需要密码。</span><span class="sxs-lookup"><span data-stu-id="d851d-158">Whether or not to require a password.</span></span>|
|<span data-ttu-id="d851d-159">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="d851d-159">passwordBlockSimple</span></span>|<span data-ttu-id="d851d-160">Boolean</span><span class="sxs-lookup"><span data-stu-id="d851d-160">Boolean</span></span>|<span data-ttu-id="d851d-161">指示是否阻止简单密码。</span><span class="sxs-lookup"><span data-stu-id="d851d-161">Indicates whether or not to block simple passwords.</span></span>|
|<span data-ttu-id="d851d-162">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="d851d-162">passwordExpirationDays</span></span>|<span data-ttu-id="d851d-163">Int32</span><span class="sxs-lookup"><span data-stu-id="d851d-163">Int32</span></span>|<span data-ttu-id="d851d-164">密码过期前的天数。</span><span class="sxs-lookup"><span data-stu-id="d851d-164">Number of days before the password expires.</span></span> <span data-ttu-id="d851d-165">有效值为 1 至 65535</span><span class="sxs-lookup"><span data-stu-id="d851d-165">Valid values 1 to 65535</span></span>|
|<span data-ttu-id="d851d-166">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="d851d-166">passwordMinimumLength</span></span>|<span data-ttu-id="d851d-167">Int32</span><span class="sxs-lookup"><span data-stu-id="d851d-167">Int32</span></span>|<span data-ttu-id="d851d-168">密码的最小长度。</span><span class="sxs-lookup"><span data-stu-id="d851d-168">Minimum length of password.</span></span> <span data-ttu-id="d851d-169">有效值为 4 至 14</span><span class="sxs-lookup"><span data-stu-id="d851d-169">Valid values 4 to 14</span></span>|
|<span data-ttu-id="d851d-170">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="d851d-170">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="d851d-171">Int32</span><span class="sxs-lookup"><span data-stu-id="d851d-171">Int32</span></span>|<span data-ttu-id="d851d-172">在需要密码之前不活动的分钟数。</span><span class="sxs-lookup"><span data-stu-id="d851d-172">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="d851d-173">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="d851d-173">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="d851d-174">Int32</span><span class="sxs-lookup"><span data-stu-id="d851d-174">Int32</span></span>|<span data-ttu-id="d851d-175">要阻止的以前密码的数量。</span><span class="sxs-lookup"><span data-stu-id="d851d-175">Number of previous passwords to block.</span></span> <span data-ttu-id="d851d-176">有效值为 1 至 24</span><span class="sxs-lookup"><span data-stu-id="d851d-176">Valid values 1 to 24</span></span>|
|<span data-ttu-id="d851d-177">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="d851d-177">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="d851d-178">Int32</span><span class="sxs-lookup"><span data-stu-id="d851d-178">Int32</span></span>|<span data-ttu-id="d851d-179">密码中必需的字符集数。</span><span class="sxs-lookup"><span data-stu-id="d851d-179">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="d851d-180">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="d851d-180">passwordRequiredType</span></span>|[<span data-ttu-id="d851d-181">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="d851d-181">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="d851d-182">必需的密码类型。</span><span class="sxs-lookup"><span data-stu-id="d851d-182">The required password type.</span></span> <span data-ttu-id="d851d-183">可取值为：`deviceDefault`、`alphanumeric`、`numeric`。</span><span class="sxs-lookup"><span data-stu-id="d851d-183">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="d851d-184">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="d851d-184">osMinimumVersion</span></span>|<span data-ttu-id="d851d-185">String</span><span class="sxs-lookup"><span data-stu-id="d851d-185">String</span></span>|<span data-ttu-id="d851d-186">最低 MacOS 版本。</span><span class="sxs-lookup"><span data-stu-id="d851d-186">Minimum MacOS version.</span></span>|
|<span data-ttu-id="d851d-187">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="d851d-187">osMaximumVersion</span></span>|<span data-ttu-id="d851d-188">String</span><span class="sxs-lookup"><span data-stu-id="d851d-188">String</span></span>|<span data-ttu-id="d851d-189">最大 MacOS 版本。</span><span class="sxs-lookup"><span data-stu-id="d851d-189">Maximum MacOS version.</span></span>|
|<span data-ttu-id="d851d-190">systemIntegrityProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="d851d-190">systemIntegrityProtectionEnabled</span></span>|<span data-ttu-id="d851d-191">Boolean</span><span class="sxs-lookup"><span data-stu-id="d851d-191">Boolean</span></span>|<span data-ttu-id="d851d-192">要求设备已启用系统完整性保护。</span><span class="sxs-lookup"><span data-stu-id="d851d-192">Require that devices have enabled system integrity protection.</span></span>|
|<span data-ttu-id="d851d-193">deviceThreatProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="d851d-193">deviceThreatProtectionEnabled</span></span>|<span data-ttu-id="d851d-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="d851d-194">Boolean</span></span>|<span data-ttu-id="d851d-195">要求设备已启用设备威胁防护。</span><span class="sxs-lookup"><span data-stu-id="d851d-195">Require that devices have enabled device threat protection.</span></span>|
|<span data-ttu-id="d851d-196">deviceThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="d851d-196">deviceThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="d851d-197">deviceThreatProtectionLevel</span><span class="sxs-lookup"><span data-stu-id="d851d-197">deviceThreatProtectionLevel</span></span>](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|<span data-ttu-id="d851d-198">要求移动威胁防护最低风险级别来报告不符合情况。</span><span class="sxs-lookup"><span data-stu-id="d851d-198">Require Mobile Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="d851d-199">可取值为：`unavailable`、`secured`、`low`、`medium`、`high`、`notSet`。</span><span class="sxs-lookup"><span data-stu-id="d851d-199">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="d851d-200">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="d851d-200">storageRequireEncryption</span></span>|<span data-ttu-id="d851d-201">Boolean</span><span class="sxs-lookup"><span data-stu-id="d851d-201">Boolean</span></span>|<span data-ttu-id="d851d-202">要求对 Mac OS 设备加密。</span><span class="sxs-lookup"><span data-stu-id="d851d-202">Require encryption on Mac OS devices.</span></span>|
|<span data-ttu-id="d851d-203">firewallEnabled</span><span class="sxs-lookup"><span data-stu-id="d851d-203">firewallEnabled</span></span>|<span data-ttu-id="d851d-204">Boolean</span><span class="sxs-lookup"><span data-stu-id="d851d-204">Boolean</span></span>|<span data-ttu-id="d851d-205">是否应启用防火墙。</span><span class="sxs-lookup"><span data-stu-id="d851d-205">Whether the firewall should be enabled or not.</span></span>|
|<span data-ttu-id="d851d-206">firewallBlockAllIncoming</span><span class="sxs-lookup"><span data-stu-id="d851d-206">firewallBlockAllIncoming</span></span>|<span data-ttu-id="d851d-207">Boolean</span><span class="sxs-lookup"><span data-stu-id="d851d-207">Boolean</span></span>|<span data-ttu-id="d851d-208">对应于 "阻止所有传入连接" 选项。</span><span class="sxs-lookup"><span data-stu-id="d851d-208">Corresponds to the “Block all incoming connections” option.</span></span>|
|<span data-ttu-id="d851d-209">firewallEnableStealthMode</span><span class="sxs-lookup"><span data-stu-id="d851d-209">firewallEnableStealthMode</span></span>|<span data-ttu-id="d851d-210">Boolean</span><span class="sxs-lookup"><span data-stu-id="d851d-210">Boolean</span></span>|<span data-ttu-id="d851d-211">对应于 "启用隐形模式"。</span><span class="sxs-lookup"><span data-stu-id="d851d-211">Corresponds to “Enable stealth mode.”</span></span>|



## <a name="response"></a><span data-ttu-id="d851d-212">响应</span><span class="sxs-lookup"><span data-stu-id="d851d-212">Response</span></span>
<span data-ttu-id="d851d-213">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和更新的 [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="d851d-213">If successful, this method returns a `200 OK` response code and an updated [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d851d-214">示例</span><span class="sxs-lookup"><span data-stu-id="d851d-214">Example</span></span>

### <a name="request"></a><span data-ttu-id="d851d-215">请求</span><span class="sxs-lookup"><span data-stu-id="d851d-215">Request</span></span>
<span data-ttu-id="d851d-216">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="d851d-216">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
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

### <a name="response"></a><span data-ttu-id="d851d-217">响应</span><span class="sxs-lookup"><span data-stu-id="d851d-217">Response</span></span>
<span data-ttu-id="d851d-p113">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="d851d-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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









