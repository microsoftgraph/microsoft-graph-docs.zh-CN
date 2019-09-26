---
title: 更新 androidDeviceOwnerCompliancePolicy
description: 更新 androidDeviceOwnerCompliancePolicy 对象的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: fc10c99329c7efd38f95d9cd41d94cae4e47ab30
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/26/2019
ms.locfileid: "37169998"
---
# <a name="update-androiddeviceownercompliancepolicy"></a><span data-ttu-id="ee07c-103">更新 androidDeviceOwnerCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="ee07c-103">Update androidDeviceOwnerCompliancePolicy</span></span>

> <span data-ttu-id="ee07c-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="ee07c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ee07c-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="ee07c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ee07c-106">更新[androidDeviceOwnerCompliancePolicy](../resources/intune-deviceconfig-androiddeviceownercompliancepolicy.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="ee07c-106">Update the properties of a [androidDeviceOwnerCompliancePolicy](../resources/intune-deviceconfig-androiddeviceownercompliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ee07c-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="ee07c-107">Prerequisites</span></span>
<span data-ttu-id="ee07c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ee07c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ee07c-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="ee07c-110">Permission type</span></span>|<span data-ttu-id="ee07c-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="ee07c-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ee07c-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ee07c-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ee07c-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ee07c-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="ee07c-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ee07c-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ee07c-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="ee07c-115">Not supported.</span></span>|
|<span data-ttu-id="ee07c-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="ee07c-116">Application</span></span>|<span data-ttu-id="ee07c-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ee07c-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ee07c-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ee07c-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="ee07c-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="ee07c-119">Request headers</span></span>
|<span data-ttu-id="ee07c-120">标头</span><span class="sxs-lookup"><span data-stu-id="ee07c-120">Header</span></span>|<span data-ttu-id="ee07c-121">值</span><span class="sxs-lookup"><span data-stu-id="ee07c-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ee07c-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="ee07c-122">Authorization</span></span>|<span data-ttu-id="ee07c-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="ee07c-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ee07c-124">接受</span><span class="sxs-lookup"><span data-stu-id="ee07c-124">Accept</span></span>|<span data-ttu-id="ee07c-125">application/json</span><span class="sxs-lookup"><span data-stu-id="ee07c-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ee07c-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="ee07c-126">Request body</span></span>
<span data-ttu-id="ee07c-127">在请求正文中，提供[androidDeviceOwnerCompliancePolicy](../resources/intune-deviceconfig-androiddeviceownercompliancepolicy.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ee07c-127">In the request body, supply a JSON representation for the [androidDeviceOwnerCompliancePolicy](../resources/intune-deviceconfig-androiddeviceownercompliancepolicy.md) object.</span></span>

<span data-ttu-id="ee07c-128">下表显示创建[androidDeviceOwnerCompliancePolicy](../resources/intune-deviceconfig-androiddeviceownercompliancepolicy.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="ee07c-128">The following table shows the properties that are required when you create the [androidDeviceOwnerCompliancePolicy](../resources/intune-deviceconfig-androiddeviceownercompliancepolicy.md).</span></span>

|<span data-ttu-id="ee07c-129">属性</span><span class="sxs-lookup"><span data-stu-id="ee07c-129">Property</span></span>|<span data-ttu-id="ee07c-130">类型</span><span class="sxs-lookup"><span data-stu-id="ee07c-130">Type</span></span>|<span data-ttu-id="ee07c-131">说明</span><span class="sxs-lookup"><span data-stu-id="ee07c-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ee07c-132">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="ee07c-132">roleScopeTagIds</span></span>|<span data-ttu-id="ee07c-133">String collection</span><span class="sxs-lookup"><span data-stu-id="ee07c-133">String collection</span></span>|<span data-ttu-id="ee07c-134">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="ee07c-134">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="ee07c-135">继承自 [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="ee07c-135">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="ee07c-136">id</span><span class="sxs-lookup"><span data-stu-id="ee07c-136">id</span></span>|<span data-ttu-id="ee07c-137">字符串</span><span class="sxs-lookup"><span data-stu-id="ee07c-137">String</span></span>|<span data-ttu-id="ee07c-138">实体的键。</span><span class="sxs-lookup"><span data-stu-id="ee07c-138">Key of the entity.</span></span> <span data-ttu-id="ee07c-139">继承自 [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="ee07c-139">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="ee07c-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ee07c-140">createdDateTime</span></span>|<span data-ttu-id="ee07c-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ee07c-141">DateTimeOffset</span></span>|<span data-ttu-id="ee07c-142">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="ee07c-142">DateTime the object was created.</span></span> <span data-ttu-id="ee07c-143">继承自 [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="ee07c-143">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="ee07c-144">说明</span><span class="sxs-lookup"><span data-stu-id="ee07c-144">description</span></span>|<span data-ttu-id="ee07c-145">String</span><span class="sxs-lookup"><span data-stu-id="ee07c-145">String</span></span>|<span data-ttu-id="ee07c-146">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="ee07c-146">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="ee07c-147">继承自 [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="ee07c-147">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="ee07c-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ee07c-148">lastModifiedDateTime</span></span>|<span data-ttu-id="ee07c-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ee07c-149">DateTimeOffset</span></span>|<span data-ttu-id="ee07c-150">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="ee07c-150">DateTime the object was last modified.</span></span> <span data-ttu-id="ee07c-151">继承自 [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="ee07c-151">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="ee07c-152">displayName</span><span class="sxs-lookup"><span data-stu-id="ee07c-152">displayName</span></span>|<span data-ttu-id="ee07c-153">字符串</span><span class="sxs-lookup"><span data-stu-id="ee07c-153">String</span></span>|<span data-ttu-id="ee07c-154">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="ee07c-154">Admin provided name of the device configuration.</span></span> <span data-ttu-id="ee07c-155">继承自 [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="ee07c-155">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="ee07c-156">version</span><span class="sxs-lookup"><span data-stu-id="ee07c-156">version</span></span>|<span data-ttu-id="ee07c-157">Int32</span><span class="sxs-lookup"><span data-stu-id="ee07c-157">Int32</span></span>|<span data-ttu-id="ee07c-158">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="ee07c-158">Version of the device configuration.</span></span> <span data-ttu-id="ee07c-159">继承自 [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="ee07c-159">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="ee07c-160">deviceThreatProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="ee07c-160">deviceThreatProtectionEnabled</span></span>|<span data-ttu-id="ee07c-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="ee07c-161">Boolean</span></span>|<span data-ttu-id="ee07c-162">要求设备已启用设备威胁防护。</span><span class="sxs-lookup"><span data-stu-id="ee07c-162">Require that devices have enabled device threat protection.</span></span>|
|<span data-ttu-id="ee07c-163">deviceThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="ee07c-163">deviceThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="ee07c-164">deviceThreatProtectionLevel</span><span class="sxs-lookup"><span data-stu-id="ee07c-164">deviceThreatProtectionLevel</span></span>](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|<span data-ttu-id="ee07c-165">要求移动威胁防护最低风险级别来报告不符合情况。</span><span class="sxs-lookup"><span data-stu-id="ee07c-165">Require Mobile Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="ee07c-166">可取值为：`unavailable`、`secured`、`low`、`medium`、`high`、`notSet`。</span><span class="sxs-lookup"><span data-stu-id="ee07c-166">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="ee07c-167">securityRequireSafetyNetAttestationBasicIntegrity</span><span class="sxs-lookup"><span data-stu-id="ee07c-167">securityRequireSafetyNetAttestationBasicIntegrity</span></span>|<span data-ttu-id="ee07c-168">Boolean</span><span class="sxs-lookup"><span data-stu-id="ee07c-168">Boolean</span></span>|<span data-ttu-id="ee07c-169">要求设备传递 SafetyNet 基本完整性检查。</span><span class="sxs-lookup"><span data-stu-id="ee07c-169">Require the device to pass the SafetyNet basic integrity check.</span></span>|
|<span data-ttu-id="ee07c-170">securityRequireSafetyNetAttestationCertifiedDevice</span><span class="sxs-lookup"><span data-stu-id="ee07c-170">securityRequireSafetyNetAttestationCertifiedDevice</span></span>|<span data-ttu-id="ee07c-171">Boolean</span><span class="sxs-lookup"><span data-stu-id="ee07c-171">Boolean</span></span>|<span data-ttu-id="ee07c-172">要求设备传递 SafetyNet 认证设备检查。</span><span class="sxs-lookup"><span data-stu-id="ee07c-172">Require the device to pass the SafetyNet certified device check.</span></span>|
|<span data-ttu-id="ee07c-173">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="ee07c-173">osMinimumVersion</span></span>|<span data-ttu-id="ee07c-174">String</span><span class="sxs-lookup"><span data-stu-id="ee07c-174">String</span></span>|<span data-ttu-id="ee07c-175">最低 Android 版本。</span><span class="sxs-lookup"><span data-stu-id="ee07c-175">Minimum Android version.</span></span>|
|<span data-ttu-id="ee07c-176">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="ee07c-176">osMaximumVersion</span></span>|<span data-ttu-id="ee07c-177">String</span><span class="sxs-lookup"><span data-stu-id="ee07c-177">String</span></span>|<span data-ttu-id="ee07c-178">最高 Android 版本。</span><span class="sxs-lookup"><span data-stu-id="ee07c-178">Maximum Android version.</span></span>|
|<span data-ttu-id="ee07c-179">minAndroidSecurityPatchLevel</span><span class="sxs-lookup"><span data-stu-id="ee07c-179">minAndroidSecurityPatchLevel</span></span>|<span data-ttu-id="ee07c-180">String</span><span class="sxs-lookup"><span data-stu-id="ee07c-180">String</span></span>|<span data-ttu-id="ee07c-181">最低 Android 安全修补程序级别。</span><span class="sxs-lookup"><span data-stu-id="ee07c-181">Minimum Android security patch level.</span></span>|
|<span data-ttu-id="ee07c-182">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="ee07c-182">passwordRequired</span></span>|<span data-ttu-id="ee07c-183">Boolean</span><span class="sxs-lookup"><span data-stu-id="ee07c-183">Boolean</span></span>|<span data-ttu-id="ee07c-184">需要密码才可解锁设备。</span><span class="sxs-lookup"><span data-stu-id="ee07c-184">Require a password to unlock device.</span></span>|
|<span data-ttu-id="ee07c-185">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="ee07c-185">passwordMinimumLength</span></span>|<span data-ttu-id="ee07c-186">Int32</span><span class="sxs-lookup"><span data-stu-id="ee07c-186">Int32</span></span>|<span data-ttu-id="ee07c-187">最短密码长度。</span><span class="sxs-lookup"><span data-stu-id="ee07c-187">Minimum password length.</span></span> <span data-ttu-id="ee07c-188">有效值为 4 至 16</span><span class="sxs-lookup"><span data-stu-id="ee07c-188">Valid values 4 to 16</span></span>|
|<span data-ttu-id="ee07c-189">passwordMinimumLetterCharacters</span><span class="sxs-lookup"><span data-stu-id="ee07c-189">passwordMinimumLetterCharacters</span></span>|<span data-ttu-id="ee07c-190">Int32</span><span class="sxs-lookup"><span data-stu-id="ee07c-190">Int32</span></span>|<span data-ttu-id="ee07c-191">指示设备密码所需的字母字符的最小数量。</span><span class="sxs-lookup"><span data-stu-id="ee07c-191">Indicates the minimum number of letter characters required for device password.</span></span> <span data-ttu-id="ee07c-192">有效值为1至16</span><span class="sxs-lookup"><span data-stu-id="ee07c-192">Valid values 1 to 16</span></span>|
|<span data-ttu-id="ee07c-193">passwordMinimumLowerCaseCharacters</span><span class="sxs-lookup"><span data-stu-id="ee07c-193">passwordMinimumLowerCaseCharacters</span></span>|<span data-ttu-id="ee07c-194">Int32</span><span class="sxs-lookup"><span data-stu-id="ee07c-194">Int32</span></span>|<span data-ttu-id="ee07c-195">指示设备密码所需的最小小写字符数。</span><span class="sxs-lookup"><span data-stu-id="ee07c-195">Indicates the minimum number of lower case characters required for device password.</span></span> <span data-ttu-id="ee07c-196">有效值为1至16</span><span class="sxs-lookup"><span data-stu-id="ee07c-196">Valid values 1 to 16</span></span>|
|<span data-ttu-id="ee07c-197">passwordMinimumNonLetterCharacters</span><span class="sxs-lookup"><span data-stu-id="ee07c-197">passwordMinimumNonLetterCharacters</span></span>|<span data-ttu-id="ee07c-198">Int32</span><span class="sxs-lookup"><span data-stu-id="ee07c-198">Int32</span></span>|<span data-ttu-id="ee07c-199">指示设备密码所需的最小非字母字符数。</span><span class="sxs-lookup"><span data-stu-id="ee07c-199">Indicates the minimum number of non-letter characters required for device password.</span></span> <span data-ttu-id="ee07c-200">有效值为1至16</span><span class="sxs-lookup"><span data-stu-id="ee07c-200">Valid values 1 to 16</span></span>|
|<span data-ttu-id="ee07c-201">passwordMinimumNumericCharacters</span><span class="sxs-lookup"><span data-stu-id="ee07c-201">passwordMinimumNumericCharacters</span></span>|<span data-ttu-id="ee07c-202">Int32</span><span class="sxs-lookup"><span data-stu-id="ee07c-202">Int32</span></span>|<span data-ttu-id="ee07c-203">指示设备密码所需的最小数字字符数。</span><span class="sxs-lookup"><span data-stu-id="ee07c-203">Indicates the minimum number of numeric characters required for device password.</span></span> <span data-ttu-id="ee07c-204">有效值为1至16</span><span class="sxs-lookup"><span data-stu-id="ee07c-204">Valid values 1 to 16</span></span>|
|<span data-ttu-id="ee07c-205">passwordMinimumSymbolCharacters</span><span class="sxs-lookup"><span data-stu-id="ee07c-205">passwordMinimumSymbolCharacters</span></span>|<span data-ttu-id="ee07c-206">Int32</span><span class="sxs-lookup"><span data-stu-id="ee07c-206">Int32</span></span>|<span data-ttu-id="ee07c-207">指示设备密码所需的最小符号字符数。</span><span class="sxs-lookup"><span data-stu-id="ee07c-207">Indicates the minimum number of symbol characters required for device password.</span></span> <span data-ttu-id="ee07c-208">有效值为1至16</span><span class="sxs-lookup"><span data-stu-id="ee07c-208">Valid values 1 to 16</span></span>|
|<span data-ttu-id="ee07c-209">passwordMinimumUpperCaseCharacters</span><span class="sxs-lookup"><span data-stu-id="ee07c-209">passwordMinimumUpperCaseCharacters</span></span>|<span data-ttu-id="ee07c-210">Int32</span><span class="sxs-lookup"><span data-stu-id="ee07c-210">Int32</span></span>|<span data-ttu-id="ee07c-211">指示设备密码所需的大写字母字符的最小数量。</span><span class="sxs-lookup"><span data-stu-id="ee07c-211">Indicates the minimum number of upper case letter characters required for device password.</span></span> <span data-ttu-id="ee07c-212">有效值为1至16</span><span class="sxs-lookup"><span data-stu-id="ee07c-212">Valid values 1 to 16</span></span>|
|<span data-ttu-id="ee07c-213">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="ee07c-213">passwordRequiredType</span></span>|[<span data-ttu-id="ee07c-214">androidDeviceOwnerRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="ee07c-214">androidDeviceOwnerRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androiddeviceownerrequiredpasswordtype.md)|<span data-ttu-id="ee07c-215">密码中的字符类型。</span><span class="sxs-lookup"><span data-stu-id="ee07c-215">Type of characters in password.</span></span> <span data-ttu-id="ee07c-216">可取值为：`deviceDefault`、`required`、`numeric`、`numericComplex`、`alphabetic`、`alphanumeric`、`alphanumericWithSymbols`、`lowSecurityBiometric`。</span><span class="sxs-lookup"><span data-stu-id="ee07c-216">Possible values are: `deviceDefault`, `required`, `numeric`, `numericComplex`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`.</span></span>|
|<span data-ttu-id="ee07c-217">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="ee07c-217">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="ee07c-218">Int32</span><span class="sxs-lookup"><span data-stu-id="ee07c-218">Int32</span></span>|<span data-ttu-id="ee07c-219">在需要密码之前不活动的分钟数。</span><span class="sxs-lookup"><span data-stu-id="ee07c-219">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="ee07c-220">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="ee07c-220">passwordExpirationDays</span></span>|<span data-ttu-id="ee07c-221">Int32</span><span class="sxs-lookup"><span data-stu-id="ee07c-221">Int32</span></span>|<span data-ttu-id="ee07c-222">密码过期前的天数。</span><span class="sxs-lookup"><span data-stu-id="ee07c-222">Number of days before the password expires.</span></span> <span data-ttu-id="ee07c-223">有效值为 1 至 365。</span><span class="sxs-lookup"><span data-stu-id="ee07c-223">Valid values 1 to 365</span></span>|
|<span data-ttu-id="ee07c-224">passwordPreviousPasswordCountToBlock</span><span class="sxs-lookup"><span data-stu-id="ee07c-224">passwordPreviousPasswordCountToBlock</span></span>|<span data-ttu-id="ee07c-225">Int32</span><span class="sxs-lookup"><span data-stu-id="ee07c-225">Int32</span></span>|<span data-ttu-id="ee07c-226">要阻止的以前密码的数量。</span><span class="sxs-lookup"><span data-stu-id="ee07c-226">Number of previous passwords to block.</span></span> <span data-ttu-id="ee07c-227">有效值为 1 至 24</span><span class="sxs-lookup"><span data-stu-id="ee07c-227">Valid values 1 to 24</span></span>|
|<span data-ttu-id="ee07c-228">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="ee07c-228">storageRequireEncryption</span></span>|<span data-ttu-id="ee07c-229">Boolean</span><span class="sxs-lookup"><span data-stu-id="ee07c-229">Boolean</span></span>|<span data-ttu-id="ee07c-230">要求对 Android 设备加密。</span><span class="sxs-lookup"><span data-stu-id="ee07c-230">Require encryption on Android devices.</span></span>|



## <a name="response"></a><span data-ttu-id="ee07c-231">响应</span><span class="sxs-lookup"><span data-stu-id="ee07c-231">Response</span></span>
<span data-ttu-id="ee07c-232">如果成功，此方法在响应`200 OK`正文中返回响应代码和更新的[androidDeviceOwnerCompliancePolicy](../resources/intune-deviceconfig-androiddeviceownercompliancepolicy.md)对象。</span><span class="sxs-lookup"><span data-stu-id="ee07c-232">If successful, this method returns a `200 OK` response code and an updated [androidDeviceOwnerCompliancePolicy](../resources/intune-deviceconfig-androiddeviceownercompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ee07c-233">示例</span><span class="sxs-lookup"><span data-stu-id="ee07c-233">Example</span></span>

### <a name="request"></a><span data-ttu-id="ee07c-234">请求</span><span class="sxs-lookup"><span data-stu-id="ee07c-234">Request</span></span>
<span data-ttu-id="ee07c-235">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="ee07c-235">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
Content-type: application/json
Content-length: 1160

{
  "@odata.type": "#microsoft.graph.androidDeviceOwnerCompliancePolicy",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "deviceThreatProtectionEnabled": true,
  "deviceThreatProtectionRequiredSecurityLevel": "secured",
  "securityRequireSafetyNetAttestationBasicIntegrity": true,
  "securityRequireSafetyNetAttestationCertifiedDevice": true,
  "osMinimumVersion": "Os Minimum Version value",
  "osMaximumVersion": "Os Maximum Version value",
  "minAndroidSecurityPatchLevel": "Min Android Security Patch Level value",
  "passwordRequired": true,
  "passwordMinimumLength": 5,
  "passwordMinimumLetterCharacters": 15,
  "passwordMinimumLowerCaseCharacters": 2,
  "passwordMinimumNonLetterCharacters": 2,
  "passwordMinimumNumericCharacters": 0,
  "passwordMinimumSymbolCharacters": 15,
  "passwordMinimumUpperCaseCharacters": 2,
  "passwordRequiredType": "required",
  "passwordMinutesOfInactivityBeforeLock": 5,
  "passwordExpirationDays": 6,
  "passwordPreviousPasswordCountToBlock": 4,
  "storageRequireEncryption": true
}
```

### <a name="response"></a><span data-ttu-id="ee07c-236">响应</span><span class="sxs-lookup"><span data-stu-id="ee07c-236">Response</span></span>
<span data-ttu-id="ee07c-p120">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="ee07c-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1332

{
  "@odata.type": "#microsoft.graph.androidDeviceOwnerCompliancePolicy",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "id": "be2464b4-64b4-be24-b464-24beb46424be",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "version": 7,
  "deviceThreatProtectionEnabled": true,
  "deviceThreatProtectionRequiredSecurityLevel": "secured",
  "securityRequireSafetyNetAttestationBasicIntegrity": true,
  "securityRequireSafetyNetAttestationCertifiedDevice": true,
  "osMinimumVersion": "Os Minimum Version value",
  "osMaximumVersion": "Os Maximum Version value",
  "minAndroidSecurityPatchLevel": "Min Android Security Patch Level value",
  "passwordRequired": true,
  "passwordMinimumLength": 5,
  "passwordMinimumLetterCharacters": 15,
  "passwordMinimumLowerCaseCharacters": 2,
  "passwordMinimumNonLetterCharacters": 2,
  "passwordMinimumNumericCharacters": 0,
  "passwordMinimumSymbolCharacters": 15,
  "passwordMinimumUpperCaseCharacters": 2,
  "passwordRequiredType": "required",
  "passwordMinutesOfInactivityBeforeLock": 5,
  "passwordExpirationDays": 6,
  "passwordPreviousPasswordCountToBlock": 4,
  "storageRequireEncryption": true
}
```




