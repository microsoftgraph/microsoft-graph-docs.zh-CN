---
title: 创建 macOSCompliancePolicy
description: 创建新的 macOSCompliancePolicy 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 002620d8c0dd3b9538071d557473cf5bf723dbcc
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48073143"
---
# <a name="create-macoscompliancepolicy"></a><span data-ttu-id="60b7f-103">创建 macOSCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="60b7f-103">Create macOSCompliancePolicy</span></span>

<span data-ttu-id="60b7f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="60b7f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="60b7f-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="60b7f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="60b7f-106">创建新的 [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="60b7f-106">Create a new [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="60b7f-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="60b7f-107">Prerequisites</span></span>
<span data-ttu-id="60b7f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="60b7f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="60b7f-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="60b7f-110">Permission type</span></span>|<span data-ttu-id="60b7f-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="60b7f-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="60b7f-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="60b7f-112">Delegated (work or school account)</span></span>|<span data-ttu-id="60b7f-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="60b7f-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="60b7f-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="60b7f-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="60b7f-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="60b7f-115">Not supported.</span></span>|
|<span data-ttu-id="60b7f-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="60b7f-116">Application</span></span>|<span data-ttu-id="60b7f-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="60b7f-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="60b7f-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="60b7f-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="60b7f-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="60b7f-119">Request headers</span></span>
|<span data-ttu-id="60b7f-120">标头</span><span class="sxs-lookup"><span data-stu-id="60b7f-120">Header</span></span>|<span data-ttu-id="60b7f-121">值</span><span class="sxs-lookup"><span data-stu-id="60b7f-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="60b7f-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="60b7f-122">Authorization</span></span>|<span data-ttu-id="60b7f-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="60b7f-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="60b7f-124">接受</span><span class="sxs-lookup"><span data-stu-id="60b7f-124">Accept</span></span>|<span data-ttu-id="60b7f-125">application/json</span><span class="sxs-lookup"><span data-stu-id="60b7f-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="60b7f-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="60b7f-126">Request body</span></span>
<span data-ttu-id="60b7f-127">在请求正文中，提供 macOSCompliancePolicy 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="60b7f-127">In the request body, supply a JSON representation for the macOSCompliancePolicy object.</span></span>

<span data-ttu-id="60b7f-128">下表显示创建 macOSCompliancePolicy 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="60b7f-128">The following table shows the properties that are required when you create the macOSCompliancePolicy.</span></span>

|<span data-ttu-id="60b7f-129">属性</span><span class="sxs-lookup"><span data-stu-id="60b7f-129">Property</span></span>|<span data-ttu-id="60b7f-130">类型</span><span class="sxs-lookup"><span data-stu-id="60b7f-130">Type</span></span>|<span data-ttu-id="60b7f-131">说明</span><span class="sxs-lookup"><span data-stu-id="60b7f-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="60b7f-132">id</span><span class="sxs-lookup"><span data-stu-id="60b7f-132">id</span></span>|<span data-ttu-id="60b7f-133">String</span><span class="sxs-lookup"><span data-stu-id="60b7f-133">String</span></span>|<span data-ttu-id="60b7f-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="60b7f-134">Key of the entity.</span></span> <span data-ttu-id="60b7f-135">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="60b7f-135">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="60b7f-136">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="60b7f-136">createdDateTime</span></span>|<span data-ttu-id="60b7f-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="60b7f-137">DateTimeOffset</span></span>|<span data-ttu-id="60b7f-138">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="60b7f-138">DateTime the object was created.</span></span> <span data-ttu-id="60b7f-139">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="60b7f-139">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="60b7f-140">description</span><span class="sxs-lookup"><span data-stu-id="60b7f-140">description</span></span>|<span data-ttu-id="60b7f-141">String</span><span class="sxs-lookup"><span data-stu-id="60b7f-141">String</span></span>|<span data-ttu-id="60b7f-142">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="60b7f-142">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="60b7f-143">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="60b7f-143">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="60b7f-144">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="60b7f-144">lastModifiedDateTime</span></span>|<span data-ttu-id="60b7f-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="60b7f-145">DateTimeOffset</span></span>|<span data-ttu-id="60b7f-146">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="60b7f-146">DateTime the object was last modified.</span></span> <span data-ttu-id="60b7f-147">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="60b7f-147">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="60b7f-148">displayName</span><span class="sxs-lookup"><span data-stu-id="60b7f-148">displayName</span></span>|<span data-ttu-id="60b7f-149">String</span><span class="sxs-lookup"><span data-stu-id="60b7f-149">String</span></span>|<span data-ttu-id="60b7f-150">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="60b7f-150">Admin provided name of the device configuration.</span></span> <span data-ttu-id="60b7f-151">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="60b7f-151">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="60b7f-152">version</span><span class="sxs-lookup"><span data-stu-id="60b7f-152">version</span></span>|<span data-ttu-id="60b7f-153">Int32</span><span class="sxs-lookup"><span data-stu-id="60b7f-153">Int32</span></span>|<span data-ttu-id="60b7f-154">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="60b7f-154">Version of the device configuration.</span></span> <span data-ttu-id="60b7f-155">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="60b7f-155">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="60b7f-156">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="60b7f-156">passwordRequired</span></span>|<span data-ttu-id="60b7f-157">Boolean</span><span class="sxs-lookup"><span data-stu-id="60b7f-157">Boolean</span></span>|<span data-ttu-id="60b7f-158">是否需要密码。</span><span class="sxs-lookup"><span data-stu-id="60b7f-158">Whether or not to require a password.</span></span>|
|<span data-ttu-id="60b7f-159">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="60b7f-159">passwordBlockSimple</span></span>|<span data-ttu-id="60b7f-160">Boolean</span><span class="sxs-lookup"><span data-stu-id="60b7f-160">Boolean</span></span>|<span data-ttu-id="60b7f-161">指示是否阻止简单密码。</span><span class="sxs-lookup"><span data-stu-id="60b7f-161">Indicates whether or not to block simple passwords.</span></span>|
|<span data-ttu-id="60b7f-162">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="60b7f-162">passwordExpirationDays</span></span>|<span data-ttu-id="60b7f-163">Int32</span><span class="sxs-lookup"><span data-stu-id="60b7f-163">Int32</span></span>|<span data-ttu-id="60b7f-164">密码过期前的天数。</span><span class="sxs-lookup"><span data-stu-id="60b7f-164">Number of days before the password expires.</span></span> <span data-ttu-id="60b7f-165">有效值为 1 至 65535</span><span class="sxs-lookup"><span data-stu-id="60b7f-165">Valid values 1 to 65535</span></span>|
|<span data-ttu-id="60b7f-166">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="60b7f-166">passwordMinimumLength</span></span>|<span data-ttu-id="60b7f-167">Int32</span><span class="sxs-lookup"><span data-stu-id="60b7f-167">Int32</span></span>|<span data-ttu-id="60b7f-168">密码的最小长度。</span><span class="sxs-lookup"><span data-stu-id="60b7f-168">Minimum length of password.</span></span> <span data-ttu-id="60b7f-169">有效值为 4 至 14</span><span class="sxs-lookup"><span data-stu-id="60b7f-169">Valid values 4 to 14</span></span>|
|<span data-ttu-id="60b7f-170">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="60b7f-170">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="60b7f-171">Int32</span><span class="sxs-lookup"><span data-stu-id="60b7f-171">Int32</span></span>|<span data-ttu-id="60b7f-172">在需要密码之前不活动的分钟数。</span><span class="sxs-lookup"><span data-stu-id="60b7f-172">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="60b7f-173">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="60b7f-173">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="60b7f-174">Int32</span><span class="sxs-lookup"><span data-stu-id="60b7f-174">Int32</span></span>|<span data-ttu-id="60b7f-175">要阻止的以前密码的数量。</span><span class="sxs-lookup"><span data-stu-id="60b7f-175">Number of previous passwords to block.</span></span> <span data-ttu-id="60b7f-176">有效值为 1 至 24</span><span class="sxs-lookup"><span data-stu-id="60b7f-176">Valid values 1 to 24</span></span>|
|<span data-ttu-id="60b7f-177">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="60b7f-177">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="60b7f-178">Int32</span><span class="sxs-lookup"><span data-stu-id="60b7f-178">Int32</span></span>|<span data-ttu-id="60b7f-179">密码中必需的字符集数。</span><span class="sxs-lookup"><span data-stu-id="60b7f-179">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="60b7f-180">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="60b7f-180">passwordRequiredType</span></span>|[<span data-ttu-id="60b7f-181">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="60b7f-181">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="60b7f-182">必需的密码类型。</span><span class="sxs-lookup"><span data-stu-id="60b7f-182">The required password type.</span></span> <span data-ttu-id="60b7f-183">可取值为：`deviceDefault`、`alphanumeric`、`numeric`。</span><span class="sxs-lookup"><span data-stu-id="60b7f-183">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="60b7f-184">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="60b7f-184">osMinimumVersion</span></span>|<span data-ttu-id="60b7f-185">String</span><span class="sxs-lookup"><span data-stu-id="60b7f-185">String</span></span>|<span data-ttu-id="60b7f-186">最低 MacOS 版本。</span><span class="sxs-lookup"><span data-stu-id="60b7f-186">Minimum MacOS version.</span></span>|
|<span data-ttu-id="60b7f-187">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="60b7f-187">osMaximumVersion</span></span>|<span data-ttu-id="60b7f-188">String</span><span class="sxs-lookup"><span data-stu-id="60b7f-188">String</span></span>|<span data-ttu-id="60b7f-189">最大 MacOS 版本。</span><span class="sxs-lookup"><span data-stu-id="60b7f-189">Maximum MacOS version.</span></span>|
|<span data-ttu-id="60b7f-190">systemIntegrityProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="60b7f-190">systemIntegrityProtectionEnabled</span></span>|<span data-ttu-id="60b7f-191">Boolean</span><span class="sxs-lookup"><span data-stu-id="60b7f-191">Boolean</span></span>|<span data-ttu-id="60b7f-192">要求设备已启用系统完整性保护。</span><span class="sxs-lookup"><span data-stu-id="60b7f-192">Require that devices have enabled system integrity protection.</span></span>|
|<span data-ttu-id="60b7f-193">deviceThreatProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="60b7f-193">deviceThreatProtectionEnabled</span></span>|<span data-ttu-id="60b7f-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="60b7f-194">Boolean</span></span>|<span data-ttu-id="60b7f-195">要求设备已启用设备威胁防护。</span><span class="sxs-lookup"><span data-stu-id="60b7f-195">Require that devices have enabled device threat protection.</span></span>|
|<span data-ttu-id="60b7f-196">deviceThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="60b7f-196">deviceThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="60b7f-197">deviceThreatProtectionLevel</span><span class="sxs-lookup"><span data-stu-id="60b7f-197">deviceThreatProtectionLevel</span></span>](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|<span data-ttu-id="60b7f-198">要求移动威胁防护最低风险级别来报告不符合情况。</span><span class="sxs-lookup"><span data-stu-id="60b7f-198">Require Mobile Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="60b7f-199">可取值为：`unavailable`、`secured`、`low`、`medium`、`high`、`notSet`。</span><span class="sxs-lookup"><span data-stu-id="60b7f-199">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="60b7f-200">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="60b7f-200">storageRequireEncryption</span></span>|<span data-ttu-id="60b7f-201">Boolean</span><span class="sxs-lookup"><span data-stu-id="60b7f-201">Boolean</span></span>|<span data-ttu-id="60b7f-202">要求对 Mac OS 设备加密。</span><span class="sxs-lookup"><span data-stu-id="60b7f-202">Require encryption on Mac OS devices.</span></span>|
|<span data-ttu-id="60b7f-203">firewallEnabled</span><span class="sxs-lookup"><span data-stu-id="60b7f-203">firewallEnabled</span></span>|<span data-ttu-id="60b7f-204">Boolean</span><span class="sxs-lookup"><span data-stu-id="60b7f-204">Boolean</span></span>|<span data-ttu-id="60b7f-205">是否应启用防火墙。</span><span class="sxs-lookup"><span data-stu-id="60b7f-205">Whether the firewall should be enabled or not.</span></span>|
|<span data-ttu-id="60b7f-206">firewallBlockAllIncoming</span><span class="sxs-lookup"><span data-stu-id="60b7f-206">firewallBlockAllIncoming</span></span>|<span data-ttu-id="60b7f-207">Boolean</span><span class="sxs-lookup"><span data-stu-id="60b7f-207">Boolean</span></span>|<span data-ttu-id="60b7f-208">对应于 "阻止所有传入连接" 选项。</span><span class="sxs-lookup"><span data-stu-id="60b7f-208">Corresponds to the “Block all incoming connections” option.</span></span>|
|<span data-ttu-id="60b7f-209">firewallEnableStealthMode</span><span class="sxs-lookup"><span data-stu-id="60b7f-209">firewallEnableStealthMode</span></span>|<span data-ttu-id="60b7f-210">Boolean</span><span class="sxs-lookup"><span data-stu-id="60b7f-210">Boolean</span></span>|<span data-ttu-id="60b7f-211">对应于 "启用隐形模式"。</span><span class="sxs-lookup"><span data-stu-id="60b7f-211">Corresponds to “Enable stealth mode.”</span></span>|



## <a name="response"></a><span data-ttu-id="60b7f-212">响应</span><span class="sxs-lookup"><span data-stu-id="60b7f-212">Response</span></span>
<span data-ttu-id="60b7f-213">如果成功，此方法会在响应正文中返回 `201 Created` 响应代码和 [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="60b7f-213">If successful, this method returns a `201 Created` response code and a [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="60b7f-214">示例</span><span class="sxs-lookup"><span data-stu-id="60b7f-214">Example</span></span>

### <a name="request"></a><span data-ttu-id="60b7f-215">请求</span><span class="sxs-lookup"><span data-stu-id="60b7f-215">Request</span></span>
<span data-ttu-id="60b7f-216">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="60b7f-216">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="60b7f-217">响应</span><span class="sxs-lookup"><span data-stu-id="60b7f-217">Response</span></span>
<span data-ttu-id="60b7f-p113">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="60b7f-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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









