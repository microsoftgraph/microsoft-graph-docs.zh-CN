---
title: 创建 androidDeviceOwnerCompliancePolicy
description: 创建新的 androidDeviceOwnerCompliancePolicy 对象。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 2c6df95e12c0837cfcb70cbaae1e59731b484a63
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/26/2019
ms.locfileid: "37170054"
---
# <a name="create-androiddeviceownercompliancepolicy"></a><span data-ttu-id="6e0ee-103">创建 androidDeviceOwnerCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="6e0ee-103">Create androidDeviceOwnerCompliancePolicy</span></span>

> <span data-ttu-id="6e0ee-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="6e0ee-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6e0ee-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="6e0ee-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6e0ee-106">创建新的[androidDeviceOwnerCompliancePolicy](../resources/intune-deviceconfig-androiddeviceownercompliancepolicy.md)对象。</span><span class="sxs-lookup"><span data-stu-id="6e0ee-106">Create a new [androidDeviceOwnerCompliancePolicy](../resources/intune-deviceconfig-androiddeviceownercompliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6e0ee-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="6e0ee-107">Prerequisites</span></span>
<span data-ttu-id="6e0ee-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6e0ee-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6e0ee-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="6e0ee-110">Permission type</span></span>|<span data-ttu-id="6e0ee-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="6e0ee-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6e0ee-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6e0ee-112">Delegated (work or school account)</span></span>|<span data-ttu-id="6e0ee-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6e0ee-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="6e0ee-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6e0ee-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6e0ee-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="6e0ee-115">Not supported.</span></span>|
|<span data-ttu-id="6e0ee-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="6e0ee-116">Application</span></span>|<span data-ttu-id="6e0ee-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6e0ee-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6e0ee-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6e0ee-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="6e0ee-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="6e0ee-119">Request headers</span></span>
|<span data-ttu-id="6e0ee-120">标头</span><span class="sxs-lookup"><span data-stu-id="6e0ee-120">Header</span></span>|<span data-ttu-id="6e0ee-121">值</span><span class="sxs-lookup"><span data-stu-id="6e0ee-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6e0ee-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="6e0ee-122">Authorization</span></span>|<span data-ttu-id="6e0ee-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="6e0ee-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6e0ee-124">接受</span><span class="sxs-lookup"><span data-stu-id="6e0ee-124">Accept</span></span>|<span data-ttu-id="6e0ee-125">application/json</span><span class="sxs-lookup"><span data-stu-id="6e0ee-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6e0ee-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="6e0ee-126">Request body</span></span>
<span data-ttu-id="6e0ee-127">在请求正文中，提供 androidDeviceOwnerCompliancePolicy 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6e0ee-127">In the request body, supply a JSON representation for the androidDeviceOwnerCompliancePolicy object.</span></span>

<span data-ttu-id="6e0ee-128">下表显示创建 androidDeviceOwnerCompliancePolicy 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="6e0ee-128">The following table shows the properties that are required when you create the androidDeviceOwnerCompliancePolicy.</span></span>

|<span data-ttu-id="6e0ee-129">属性</span><span class="sxs-lookup"><span data-stu-id="6e0ee-129">Property</span></span>|<span data-ttu-id="6e0ee-130">类型</span><span class="sxs-lookup"><span data-stu-id="6e0ee-130">Type</span></span>|<span data-ttu-id="6e0ee-131">说明</span><span class="sxs-lookup"><span data-stu-id="6e0ee-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6e0ee-132">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="6e0ee-132">roleScopeTagIds</span></span>|<span data-ttu-id="6e0ee-133">String collection</span><span class="sxs-lookup"><span data-stu-id="6e0ee-133">String collection</span></span>|<span data-ttu-id="6e0ee-134">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="6e0ee-134">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="6e0ee-135">继承自 [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="6e0ee-135">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="6e0ee-136">id</span><span class="sxs-lookup"><span data-stu-id="6e0ee-136">id</span></span>|<span data-ttu-id="6e0ee-137">字符串</span><span class="sxs-lookup"><span data-stu-id="6e0ee-137">String</span></span>|<span data-ttu-id="6e0ee-138">实体的键。</span><span class="sxs-lookup"><span data-stu-id="6e0ee-138">Key of the entity.</span></span> <span data-ttu-id="6e0ee-139">继承自 [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="6e0ee-139">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="6e0ee-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6e0ee-140">createdDateTime</span></span>|<span data-ttu-id="6e0ee-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6e0ee-141">DateTimeOffset</span></span>|<span data-ttu-id="6e0ee-142">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="6e0ee-142">DateTime the object was created.</span></span> <span data-ttu-id="6e0ee-143">继承自 [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="6e0ee-143">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="6e0ee-144">说明</span><span class="sxs-lookup"><span data-stu-id="6e0ee-144">description</span></span>|<span data-ttu-id="6e0ee-145">String</span><span class="sxs-lookup"><span data-stu-id="6e0ee-145">String</span></span>|<span data-ttu-id="6e0ee-146">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="6e0ee-146">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="6e0ee-147">继承自 [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="6e0ee-147">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="6e0ee-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6e0ee-148">lastModifiedDateTime</span></span>|<span data-ttu-id="6e0ee-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6e0ee-149">DateTimeOffset</span></span>|<span data-ttu-id="6e0ee-150">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="6e0ee-150">DateTime the object was last modified.</span></span> <span data-ttu-id="6e0ee-151">继承自 [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="6e0ee-151">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="6e0ee-152">displayName</span><span class="sxs-lookup"><span data-stu-id="6e0ee-152">displayName</span></span>|<span data-ttu-id="6e0ee-153">字符串</span><span class="sxs-lookup"><span data-stu-id="6e0ee-153">String</span></span>|<span data-ttu-id="6e0ee-154">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="6e0ee-154">Admin provided name of the device configuration.</span></span> <span data-ttu-id="6e0ee-155">继承自 [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="6e0ee-155">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="6e0ee-156">version</span><span class="sxs-lookup"><span data-stu-id="6e0ee-156">version</span></span>|<span data-ttu-id="6e0ee-157">Int32</span><span class="sxs-lookup"><span data-stu-id="6e0ee-157">Int32</span></span>|<span data-ttu-id="6e0ee-158">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="6e0ee-158">Version of the device configuration.</span></span> <span data-ttu-id="6e0ee-159">继承自 [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="6e0ee-159">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="6e0ee-160">deviceThreatProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="6e0ee-160">deviceThreatProtectionEnabled</span></span>|<span data-ttu-id="6e0ee-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="6e0ee-161">Boolean</span></span>|<span data-ttu-id="6e0ee-162">要求设备已启用设备威胁防护。</span><span class="sxs-lookup"><span data-stu-id="6e0ee-162">Require that devices have enabled device threat protection.</span></span>|
|<span data-ttu-id="6e0ee-163">deviceThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="6e0ee-163">deviceThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="6e0ee-164">deviceThreatProtectionLevel</span><span class="sxs-lookup"><span data-stu-id="6e0ee-164">deviceThreatProtectionLevel</span></span>](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|<span data-ttu-id="6e0ee-165">要求移动威胁防护最低风险级别来报告不符合情况。</span><span class="sxs-lookup"><span data-stu-id="6e0ee-165">Require Mobile Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="6e0ee-166">可取值为：`unavailable`、`secured`、`low`、`medium`、`high`、`notSet`。</span><span class="sxs-lookup"><span data-stu-id="6e0ee-166">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="6e0ee-167">securityRequireSafetyNetAttestationBasicIntegrity</span><span class="sxs-lookup"><span data-stu-id="6e0ee-167">securityRequireSafetyNetAttestationBasicIntegrity</span></span>|<span data-ttu-id="6e0ee-168">Boolean</span><span class="sxs-lookup"><span data-stu-id="6e0ee-168">Boolean</span></span>|<span data-ttu-id="6e0ee-169">要求设备传递 SafetyNet 基本完整性检查。</span><span class="sxs-lookup"><span data-stu-id="6e0ee-169">Require the device to pass the SafetyNet basic integrity check.</span></span>|
|<span data-ttu-id="6e0ee-170">securityRequireSafetyNetAttestationCertifiedDevice</span><span class="sxs-lookup"><span data-stu-id="6e0ee-170">securityRequireSafetyNetAttestationCertifiedDevice</span></span>|<span data-ttu-id="6e0ee-171">Boolean</span><span class="sxs-lookup"><span data-stu-id="6e0ee-171">Boolean</span></span>|<span data-ttu-id="6e0ee-172">要求设备传递 SafetyNet 认证设备检查。</span><span class="sxs-lookup"><span data-stu-id="6e0ee-172">Require the device to pass the SafetyNet certified device check.</span></span>|
|<span data-ttu-id="6e0ee-173">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="6e0ee-173">osMinimumVersion</span></span>|<span data-ttu-id="6e0ee-174">String</span><span class="sxs-lookup"><span data-stu-id="6e0ee-174">String</span></span>|<span data-ttu-id="6e0ee-175">最低 Android 版本。</span><span class="sxs-lookup"><span data-stu-id="6e0ee-175">Minimum Android version.</span></span>|
|<span data-ttu-id="6e0ee-176">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="6e0ee-176">osMaximumVersion</span></span>|<span data-ttu-id="6e0ee-177">String</span><span class="sxs-lookup"><span data-stu-id="6e0ee-177">String</span></span>|<span data-ttu-id="6e0ee-178">最高 Android 版本。</span><span class="sxs-lookup"><span data-stu-id="6e0ee-178">Maximum Android version.</span></span>|
|<span data-ttu-id="6e0ee-179">minAndroidSecurityPatchLevel</span><span class="sxs-lookup"><span data-stu-id="6e0ee-179">minAndroidSecurityPatchLevel</span></span>|<span data-ttu-id="6e0ee-180">String</span><span class="sxs-lookup"><span data-stu-id="6e0ee-180">String</span></span>|<span data-ttu-id="6e0ee-181">最低 Android 安全修补程序级别。</span><span class="sxs-lookup"><span data-stu-id="6e0ee-181">Minimum Android security patch level.</span></span>|
|<span data-ttu-id="6e0ee-182">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="6e0ee-182">passwordRequired</span></span>|<span data-ttu-id="6e0ee-183">Boolean</span><span class="sxs-lookup"><span data-stu-id="6e0ee-183">Boolean</span></span>|<span data-ttu-id="6e0ee-184">需要密码才可解锁设备。</span><span class="sxs-lookup"><span data-stu-id="6e0ee-184">Require a password to unlock device.</span></span>|
|<span data-ttu-id="6e0ee-185">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="6e0ee-185">passwordMinimumLength</span></span>|<span data-ttu-id="6e0ee-186">Int32</span><span class="sxs-lookup"><span data-stu-id="6e0ee-186">Int32</span></span>|<span data-ttu-id="6e0ee-187">最短密码长度。</span><span class="sxs-lookup"><span data-stu-id="6e0ee-187">Minimum password length.</span></span> <span data-ttu-id="6e0ee-188">有效值为 4 至 16</span><span class="sxs-lookup"><span data-stu-id="6e0ee-188">Valid values 4 to 16</span></span>|
|<span data-ttu-id="6e0ee-189">passwordMinimumLetterCharacters</span><span class="sxs-lookup"><span data-stu-id="6e0ee-189">passwordMinimumLetterCharacters</span></span>|<span data-ttu-id="6e0ee-190">Int32</span><span class="sxs-lookup"><span data-stu-id="6e0ee-190">Int32</span></span>|<span data-ttu-id="6e0ee-191">指示设备密码所需的字母字符的最小数量。</span><span class="sxs-lookup"><span data-stu-id="6e0ee-191">Indicates the minimum number of letter characters required for device password.</span></span> <span data-ttu-id="6e0ee-192">有效值为1至16</span><span class="sxs-lookup"><span data-stu-id="6e0ee-192">Valid values 1 to 16</span></span>|
|<span data-ttu-id="6e0ee-193">passwordMinimumLowerCaseCharacters</span><span class="sxs-lookup"><span data-stu-id="6e0ee-193">passwordMinimumLowerCaseCharacters</span></span>|<span data-ttu-id="6e0ee-194">Int32</span><span class="sxs-lookup"><span data-stu-id="6e0ee-194">Int32</span></span>|<span data-ttu-id="6e0ee-195">指示设备密码所需的最小小写字符数。</span><span class="sxs-lookup"><span data-stu-id="6e0ee-195">Indicates the minimum number of lower case characters required for device password.</span></span> <span data-ttu-id="6e0ee-196">有效值为1至16</span><span class="sxs-lookup"><span data-stu-id="6e0ee-196">Valid values 1 to 16</span></span>|
|<span data-ttu-id="6e0ee-197">passwordMinimumNonLetterCharacters</span><span class="sxs-lookup"><span data-stu-id="6e0ee-197">passwordMinimumNonLetterCharacters</span></span>|<span data-ttu-id="6e0ee-198">Int32</span><span class="sxs-lookup"><span data-stu-id="6e0ee-198">Int32</span></span>|<span data-ttu-id="6e0ee-199">指示设备密码所需的最小非字母字符数。</span><span class="sxs-lookup"><span data-stu-id="6e0ee-199">Indicates the minimum number of non-letter characters required for device password.</span></span> <span data-ttu-id="6e0ee-200">有效值为1至16</span><span class="sxs-lookup"><span data-stu-id="6e0ee-200">Valid values 1 to 16</span></span>|
|<span data-ttu-id="6e0ee-201">passwordMinimumNumericCharacters</span><span class="sxs-lookup"><span data-stu-id="6e0ee-201">passwordMinimumNumericCharacters</span></span>|<span data-ttu-id="6e0ee-202">Int32</span><span class="sxs-lookup"><span data-stu-id="6e0ee-202">Int32</span></span>|<span data-ttu-id="6e0ee-203">指示设备密码所需的最小数字字符数。</span><span class="sxs-lookup"><span data-stu-id="6e0ee-203">Indicates the minimum number of numeric characters required for device password.</span></span> <span data-ttu-id="6e0ee-204">有效值为1至16</span><span class="sxs-lookup"><span data-stu-id="6e0ee-204">Valid values 1 to 16</span></span>|
|<span data-ttu-id="6e0ee-205">passwordMinimumSymbolCharacters</span><span class="sxs-lookup"><span data-stu-id="6e0ee-205">passwordMinimumSymbolCharacters</span></span>|<span data-ttu-id="6e0ee-206">Int32</span><span class="sxs-lookup"><span data-stu-id="6e0ee-206">Int32</span></span>|<span data-ttu-id="6e0ee-207">指示设备密码所需的最小符号字符数。</span><span class="sxs-lookup"><span data-stu-id="6e0ee-207">Indicates the minimum number of symbol characters required for device password.</span></span> <span data-ttu-id="6e0ee-208">有效值为1至16</span><span class="sxs-lookup"><span data-stu-id="6e0ee-208">Valid values 1 to 16</span></span>|
|<span data-ttu-id="6e0ee-209">passwordMinimumUpperCaseCharacters</span><span class="sxs-lookup"><span data-stu-id="6e0ee-209">passwordMinimumUpperCaseCharacters</span></span>|<span data-ttu-id="6e0ee-210">Int32</span><span class="sxs-lookup"><span data-stu-id="6e0ee-210">Int32</span></span>|<span data-ttu-id="6e0ee-211">指示设备密码所需的大写字母字符的最小数量。</span><span class="sxs-lookup"><span data-stu-id="6e0ee-211">Indicates the minimum number of upper case letter characters required for device password.</span></span> <span data-ttu-id="6e0ee-212">有效值为1至16</span><span class="sxs-lookup"><span data-stu-id="6e0ee-212">Valid values 1 to 16</span></span>|
|<span data-ttu-id="6e0ee-213">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="6e0ee-213">passwordRequiredType</span></span>|[<span data-ttu-id="6e0ee-214">androidDeviceOwnerRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="6e0ee-214">androidDeviceOwnerRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androiddeviceownerrequiredpasswordtype.md)|<span data-ttu-id="6e0ee-215">密码中的字符类型。</span><span class="sxs-lookup"><span data-stu-id="6e0ee-215">Type of characters in password.</span></span> <span data-ttu-id="6e0ee-216">可取值为：`deviceDefault`、`required`、`numeric`、`numericComplex`、`alphabetic`、`alphanumeric`、`alphanumericWithSymbols`、`lowSecurityBiometric`。</span><span class="sxs-lookup"><span data-stu-id="6e0ee-216">Possible values are: `deviceDefault`, `required`, `numeric`, `numericComplex`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`.</span></span>|
|<span data-ttu-id="6e0ee-217">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="6e0ee-217">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="6e0ee-218">Int32</span><span class="sxs-lookup"><span data-stu-id="6e0ee-218">Int32</span></span>|<span data-ttu-id="6e0ee-219">在需要密码之前不活动的分钟数。</span><span class="sxs-lookup"><span data-stu-id="6e0ee-219">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="6e0ee-220">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="6e0ee-220">passwordExpirationDays</span></span>|<span data-ttu-id="6e0ee-221">Int32</span><span class="sxs-lookup"><span data-stu-id="6e0ee-221">Int32</span></span>|<span data-ttu-id="6e0ee-222">密码过期前的天数。</span><span class="sxs-lookup"><span data-stu-id="6e0ee-222">Number of days before the password expires.</span></span> <span data-ttu-id="6e0ee-223">有效值为 1 至 365。</span><span class="sxs-lookup"><span data-stu-id="6e0ee-223">Valid values 1 to 365</span></span>|
|<span data-ttu-id="6e0ee-224">passwordPreviousPasswordCountToBlock</span><span class="sxs-lookup"><span data-stu-id="6e0ee-224">passwordPreviousPasswordCountToBlock</span></span>|<span data-ttu-id="6e0ee-225">Int32</span><span class="sxs-lookup"><span data-stu-id="6e0ee-225">Int32</span></span>|<span data-ttu-id="6e0ee-226">要阻止的以前密码的数量。</span><span class="sxs-lookup"><span data-stu-id="6e0ee-226">Number of previous passwords to block.</span></span> <span data-ttu-id="6e0ee-227">有效值为 1 至 24</span><span class="sxs-lookup"><span data-stu-id="6e0ee-227">Valid values 1 to 24</span></span>|
|<span data-ttu-id="6e0ee-228">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="6e0ee-228">storageRequireEncryption</span></span>|<span data-ttu-id="6e0ee-229">Boolean</span><span class="sxs-lookup"><span data-stu-id="6e0ee-229">Boolean</span></span>|<span data-ttu-id="6e0ee-230">要求对 Android 设备加密。</span><span class="sxs-lookup"><span data-stu-id="6e0ee-230">Require encryption on Android devices.</span></span>|



## <a name="response"></a><span data-ttu-id="6e0ee-231">响应</span><span class="sxs-lookup"><span data-stu-id="6e0ee-231">Response</span></span>
<span data-ttu-id="6e0ee-232">如果成功，此方法在响应`201 Created`正文中返回响应代码和[androidDeviceOwnerCompliancePolicy](../resources/intune-deviceconfig-androiddeviceownercompliancepolicy.md)对象。</span><span class="sxs-lookup"><span data-stu-id="6e0ee-232">If successful, this method returns a `201 Created` response code and a [androidDeviceOwnerCompliancePolicy](../resources/intune-deviceconfig-androiddeviceownercompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6e0ee-233">示例</span><span class="sxs-lookup"><span data-stu-id="6e0ee-233">Example</span></span>

### <a name="request"></a><span data-ttu-id="6e0ee-234">请求</span><span class="sxs-lookup"><span data-stu-id="6e0ee-234">Request</span></span>
<span data-ttu-id="6e0ee-235">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="6e0ee-235">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies
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

### <a name="response"></a><span data-ttu-id="6e0ee-236">响应</span><span class="sxs-lookup"><span data-stu-id="6e0ee-236">Response</span></span>
<span data-ttu-id="6e0ee-p120">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="6e0ee-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




