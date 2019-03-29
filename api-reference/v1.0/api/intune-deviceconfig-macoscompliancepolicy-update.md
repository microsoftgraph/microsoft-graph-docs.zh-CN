---
title: 更新 macOSCompliancePolicy
description: 更新 macOSCompliancePolicy 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 922b63ba99ae17505e36a861c6d12a4b6a195c8c
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/29/2019
ms.locfileid: "30978190"
---
# <a name="update-macoscompliancepolicy"></a><span data-ttu-id="9fcfa-103">更新 macOSCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="9fcfa-103">Update macOSCompliancePolicy</span></span>

> <span data-ttu-id="9fcfa-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="9fcfa-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9fcfa-105">更新 [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="9fcfa-105">Update the properties of a [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9fcfa-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="9fcfa-106">Prerequisites</span></span>
<span data-ttu-id="9fcfa-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9fcfa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9fcfa-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="9fcfa-109">Permission type</span></span>|<span data-ttu-id="9fcfa-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="9fcfa-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9fcfa-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9fcfa-111">Delegated (work or school account)</span></span>|<span data-ttu-id="9fcfa-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9fcfa-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="9fcfa-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9fcfa-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9fcfa-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="9fcfa-114">Not supported.</span></span>|
|<span data-ttu-id="9fcfa-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="9fcfa-115">Application</span></span>|<span data-ttu-id="9fcfa-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="9fcfa-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9fcfa-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9fcfa-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="9fcfa-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="9fcfa-118">Request headers</span></span>
|<span data-ttu-id="9fcfa-119">标头</span><span class="sxs-lookup"><span data-stu-id="9fcfa-119">Header</span></span>|<span data-ttu-id="9fcfa-120">值</span><span class="sxs-lookup"><span data-stu-id="9fcfa-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9fcfa-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="9fcfa-121">Authorization</span></span>|<span data-ttu-id="9fcfa-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="9fcfa-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9fcfa-123">接受</span><span class="sxs-lookup"><span data-stu-id="9fcfa-123">Accept</span></span>|<span data-ttu-id="9fcfa-124">application/json</span><span class="sxs-lookup"><span data-stu-id="9fcfa-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9fcfa-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="9fcfa-125">Request body</span></span>
<span data-ttu-id="9fcfa-126">在请求正文中，提供 [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9fcfa-126">In the request body, supply a JSON representation for the [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) object.</span></span>

<span data-ttu-id="9fcfa-127">下表显示创建 [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="9fcfa-127">The following table shows the properties that are required when you create the [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md).</span></span>

|<span data-ttu-id="9fcfa-128">属性</span><span class="sxs-lookup"><span data-stu-id="9fcfa-128">Property</span></span>|<span data-ttu-id="9fcfa-129">类型</span><span class="sxs-lookup"><span data-stu-id="9fcfa-129">Type</span></span>|<span data-ttu-id="9fcfa-130">说明</span><span class="sxs-lookup"><span data-stu-id="9fcfa-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9fcfa-131">id</span><span class="sxs-lookup"><span data-stu-id="9fcfa-131">id</span></span>|<span data-ttu-id="9fcfa-132">String</span><span class="sxs-lookup"><span data-stu-id="9fcfa-132">String</span></span>|<span data-ttu-id="9fcfa-133">实体的键。</span><span class="sxs-lookup"><span data-stu-id="9fcfa-133">Key of the entity.</span></span> <span data-ttu-id="9fcfa-134">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="9fcfa-134">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="9fcfa-135">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="9fcfa-135">createdDateTime</span></span>|<span data-ttu-id="9fcfa-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9fcfa-136">DateTimeOffset</span></span>|<span data-ttu-id="9fcfa-137">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="9fcfa-137">DateTime the object was created.</span></span> <span data-ttu-id="9fcfa-138">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="9fcfa-138">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="9fcfa-139">description</span><span class="sxs-lookup"><span data-stu-id="9fcfa-139">description</span></span>|<span data-ttu-id="9fcfa-140">String</span><span class="sxs-lookup"><span data-stu-id="9fcfa-140">String</span></span>|<span data-ttu-id="9fcfa-141">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="9fcfa-141">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="9fcfa-142">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="9fcfa-142">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="9fcfa-143">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9fcfa-143">lastModifiedDateTime</span></span>|<span data-ttu-id="9fcfa-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9fcfa-144">DateTimeOffset</span></span>|<span data-ttu-id="9fcfa-145">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="9fcfa-145">DateTime the object was last modified.</span></span> <span data-ttu-id="9fcfa-146">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="9fcfa-146">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="9fcfa-147">displayName</span><span class="sxs-lookup"><span data-stu-id="9fcfa-147">displayName</span></span>|<span data-ttu-id="9fcfa-148">String</span><span class="sxs-lookup"><span data-stu-id="9fcfa-148">String</span></span>|<span data-ttu-id="9fcfa-149">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="9fcfa-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="9fcfa-150">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="9fcfa-150">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="9fcfa-151">version</span><span class="sxs-lookup"><span data-stu-id="9fcfa-151">version</span></span>|<span data-ttu-id="9fcfa-152">Int32</span><span class="sxs-lookup"><span data-stu-id="9fcfa-152">Int32</span></span>|<span data-ttu-id="9fcfa-153">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="9fcfa-153">Version of the device configuration.</span></span> <span data-ttu-id="9fcfa-154">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="9fcfa-154">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="9fcfa-155">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="9fcfa-155">passwordRequired</span></span>|<span data-ttu-id="9fcfa-156">Boolean</span><span class="sxs-lookup"><span data-stu-id="9fcfa-156">Boolean</span></span>|<span data-ttu-id="9fcfa-157">是否需要密码。</span><span class="sxs-lookup"><span data-stu-id="9fcfa-157">Whether or not to require a password.</span></span>|
|<span data-ttu-id="9fcfa-158">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="9fcfa-158">passwordBlockSimple</span></span>|<span data-ttu-id="9fcfa-159">Boolean</span><span class="sxs-lookup"><span data-stu-id="9fcfa-159">Boolean</span></span>|<span data-ttu-id="9fcfa-160">指示是否阻止简单密码。</span><span class="sxs-lookup"><span data-stu-id="9fcfa-160">Indicates whether or not to block simple passwords.</span></span>|
|<span data-ttu-id="9fcfa-161">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="9fcfa-161">passwordExpirationDays</span></span>|<span data-ttu-id="9fcfa-162">Int32</span><span class="sxs-lookup"><span data-stu-id="9fcfa-162">Int32</span></span>|<span data-ttu-id="9fcfa-163">密码过期前的天数。</span><span class="sxs-lookup"><span data-stu-id="9fcfa-163">Number of days before the password expires.</span></span> <span data-ttu-id="9fcfa-164">有效值为 1 至 65535</span><span class="sxs-lookup"><span data-stu-id="9fcfa-164">Valid values 1 to 65535</span></span>|
|<span data-ttu-id="9fcfa-165">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="9fcfa-165">passwordMinimumLength</span></span>|<span data-ttu-id="9fcfa-166">Int32</span><span class="sxs-lookup"><span data-stu-id="9fcfa-166">Int32</span></span>|<span data-ttu-id="9fcfa-167">密码的最小长度。</span><span class="sxs-lookup"><span data-stu-id="9fcfa-167">Minimum length of password.</span></span> <span data-ttu-id="9fcfa-168">有效值为 4 至 14</span><span class="sxs-lookup"><span data-stu-id="9fcfa-168">Valid values 4 to 14</span></span>|
|<span data-ttu-id="9fcfa-169">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="9fcfa-169">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="9fcfa-170">Int32</span><span class="sxs-lookup"><span data-stu-id="9fcfa-170">Int32</span></span>|<span data-ttu-id="9fcfa-171">在需要密码之前不活动的分钟数。</span><span class="sxs-lookup"><span data-stu-id="9fcfa-171">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="9fcfa-172">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="9fcfa-172">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="9fcfa-173">Int32</span><span class="sxs-lookup"><span data-stu-id="9fcfa-173">Int32</span></span>|<span data-ttu-id="9fcfa-174">要阻止的以前密码的数量。</span><span class="sxs-lookup"><span data-stu-id="9fcfa-174">Number of previous passwords to block.</span></span> <span data-ttu-id="9fcfa-175">有效值为 1 至 24</span><span class="sxs-lookup"><span data-stu-id="9fcfa-175">Valid values 1 to 24</span></span>|
|<span data-ttu-id="9fcfa-176">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="9fcfa-176">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="9fcfa-177">Int32</span><span class="sxs-lookup"><span data-stu-id="9fcfa-177">Int32</span></span>|<span data-ttu-id="9fcfa-178">密码中必需的字符集数。</span><span class="sxs-lookup"><span data-stu-id="9fcfa-178">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="9fcfa-179">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="9fcfa-179">passwordRequiredType</span></span>|[<span data-ttu-id="9fcfa-180">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="9fcfa-180">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="9fcfa-181">必需的密码类型。</span><span class="sxs-lookup"><span data-stu-id="9fcfa-181">The required password type.</span></span> <span data-ttu-id="9fcfa-182">可取值为：`deviceDefault`、`alphanumeric`、`numeric`。</span><span class="sxs-lookup"><span data-stu-id="9fcfa-182">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="9fcfa-183">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="9fcfa-183">osMinimumVersion</span></span>|<span data-ttu-id="9fcfa-184">String</span><span class="sxs-lookup"><span data-stu-id="9fcfa-184">String</span></span>|<span data-ttu-id="9fcfa-185">最低 MacOS 版本。</span><span class="sxs-lookup"><span data-stu-id="9fcfa-185">Minimum MacOS version.</span></span>|
|<span data-ttu-id="9fcfa-186">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="9fcfa-186">osMaximumVersion</span></span>|<span data-ttu-id="9fcfa-187">String</span><span class="sxs-lookup"><span data-stu-id="9fcfa-187">String</span></span>|<span data-ttu-id="9fcfa-188">最大 MacOS 版本。</span><span class="sxs-lookup"><span data-stu-id="9fcfa-188">Maximum MacOS version.</span></span>|
|<span data-ttu-id="9fcfa-189">systemIntegrityProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="9fcfa-189">systemIntegrityProtectionEnabled</span></span>|<span data-ttu-id="9fcfa-190">Boolean</span><span class="sxs-lookup"><span data-stu-id="9fcfa-190">Boolean</span></span>|<span data-ttu-id="9fcfa-191">要求设备已启用系统完整性保护。</span><span class="sxs-lookup"><span data-stu-id="9fcfa-191">Require that devices have enabled system integrity protection.</span></span>|
|<span data-ttu-id="9fcfa-192">deviceThreatProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="9fcfa-192">deviceThreatProtectionEnabled</span></span>|<span data-ttu-id="9fcfa-193">Boolean</span><span class="sxs-lookup"><span data-stu-id="9fcfa-193">Boolean</span></span>|<span data-ttu-id="9fcfa-194">要求设备已启用设备威胁防护。</span><span class="sxs-lookup"><span data-stu-id="9fcfa-194">Require that devices have enabled device threat protection.</span></span>|
|<span data-ttu-id="9fcfa-195">deviceThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="9fcfa-195">deviceThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="9fcfa-196">deviceThreatProtectionLevel</span><span class="sxs-lookup"><span data-stu-id="9fcfa-196">deviceThreatProtectionLevel</span></span>](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|<span data-ttu-id="9fcfa-197">要求移动威胁防护最低风险级别来报告不符合情况。</span><span class="sxs-lookup"><span data-stu-id="9fcfa-197">Require Mobile Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="9fcfa-198">可取值为：`unavailable`、`secured`、`low`、`medium`、`high`、`notSet`。</span><span class="sxs-lookup"><span data-stu-id="9fcfa-198">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="9fcfa-199">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="9fcfa-199">storageRequireEncryption</span></span>|<span data-ttu-id="9fcfa-200">Boolean</span><span class="sxs-lookup"><span data-stu-id="9fcfa-200">Boolean</span></span>|<span data-ttu-id="9fcfa-201">要求对 Mac OS 设备加密。</span><span class="sxs-lookup"><span data-stu-id="9fcfa-201">Require encryption on Mac OS devices.</span></span>|
|<span data-ttu-id="9fcfa-202">firewallEnabled</span><span class="sxs-lookup"><span data-stu-id="9fcfa-202">firewallEnabled</span></span>|<span data-ttu-id="9fcfa-203">Boolean</span><span class="sxs-lookup"><span data-stu-id="9fcfa-203">Boolean</span></span>|<span data-ttu-id="9fcfa-204">是否应启用防火墙。</span><span class="sxs-lookup"><span data-stu-id="9fcfa-204">Whether the firewall should be enabled or not.</span></span>|
|<span data-ttu-id="9fcfa-205">firewallBlockAllIncoming</span><span class="sxs-lookup"><span data-stu-id="9fcfa-205">firewallBlockAllIncoming</span></span>|<span data-ttu-id="9fcfa-206">Boolean</span><span class="sxs-lookup"><span data-stu-id="9fcfa-206">Boolean</span></span>|<span data-ttu-id="9fcfa-207">对应于 "阻止所有传入连接" 选项。</span><span class="sxs-lookup"><span data-stu-id="9fcfa-207">Corresponds to the “Block all incoming connections” option.</span></span>|
|<span data-ttu-id="9fcfa-208">firewallEnableStealthMode</span><span class="sxs-lookup"><span data-stu-id="9fcfa-208">firewallEnableStealthMode</span></span>|<span data-ttu-id="9fcfa-209">Boolean</span><span class="sxs-lookup"><span data-stu-id="9fcfa-209">Boolean</span></span>|<span data-ttu-id="9fcfa-210">对应于 "启用隐形模式"。</span><span class="sxs-lookup"><span data-stu-id="9fcfa-210">Corresponds to “Enable stealth mode.”</span></span>|



## <a name="response"></a><span data-ttu-id="9fcfa-211">响应</span><span class="sxs-lookup"><span data-stu-id="9fcfa-211">Response</span></span>
<span data-ttu-id="9fcfa-212">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和更新的 [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="9fcfa-212">If successful, this method returns a `200 OK` response code and an updated [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9fcfa-213">示例</span><span class="sxs-lookup"><span data-stu-id="9fcfa-213">Example</span></span>

### <a name="request"></a><span data-ttu-id="9fcfa-214">请求</span><span class="sxs-lookup"><span data-stu-id="9fcfa-214">Request</span></span>
<span data-ttu-id="9fcfa-215">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="9fcfa-215">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="9fcfa-216">响应</span><span class="sxs-lookup"><span data-stu-id="9fcfa-216">Response</span></span>
<span data-ttu-id="9fcfa-p113">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="9fcfa-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



