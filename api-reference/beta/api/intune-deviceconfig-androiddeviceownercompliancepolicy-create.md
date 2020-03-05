---
title: 创建 androidDeviceOwnerCompliancePolicy
description: 创建新的 androidDeviceOwnerCompliancePolicy 对象。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 5b6eee3fc662a22335c6860fa5cffee31ec4adbe
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42450102"
---
# <a name="create-androiddeviceownercompliancepolicy"></a><span data-ttu-id="64288-103">创建 androidDeviceOwnerCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="64288-103">Create androidDeviceOwnerCompliancePolicy</span></span>

<span data-ttu-id="64288-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="64288-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="64288-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="64288-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="64288-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="64288-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="64288-107">创建新的[androidDeviceOwnerCompliancePolicy](../resources/intune-deviceconfig-androiddeviceownercompliancepolicy.md)对象。</span><span class="sxs-lookup"><span data-stu-id="64288-107">Create a new [androidDeviceOwnerCompliancePolicy](../resources/intune-deviceconfig-androiddeviceownercompliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="64288-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="64288-108">Prerequisites</span></span>
<span data-ttu-id="64288-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="64288-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="64288-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="64288-111">Permission type</span></span>|<span data-ttu-id="64288-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="64288-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="64288-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="64288-113">Delegated (work or school account)</span></span>|<span data-ttu-id="64288-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="64288-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="64288-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="64288-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="64288-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="64288-116">Not supported.</span></span>|
|<span data-ttu-id="64288-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="64288-117">Application</span></span>|<span data-ttu-id="64288-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="64288-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="64288-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="64288-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="64288-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="64288-120">Request headers</span></span>
|<span data-ttu-id="64288-121">标头</span><span class="sxs-lookup"><span data-stu-id="64288-121">Header</span></span>|<span data-ttu-id="64288-122">值</span><span class="sxs-lookup"><span data-stu-id="64288-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="64288-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="64288-123">Authorization</span></span>|<span data-ttu-id="64288-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="64288-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="64288-125">接受</span><span class="sxs-lookup"><span data-stu-id="64288-125">Accept</span></span>|<span data-ttu-id="64288-126">application/json</span><span class="sxs-lookup"><span data-stu-id="64288-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="64288-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="64288-127">Request body</span></span>
<span data-ttu-id="64288-128">在请求正文中，提供 androidDeviceOwnerCompliancePolicy 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="64288-128">In the request body, supply a JSON representation for the androidDeviceOwnerCompliancePolicy object.</span></span>

<span data-ttu-id="64288-129">下表显示创建 androidDeviceOwnerCompliancePolicy 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="64288-129">The following table shows the properties that are required when you create the androidDeviceOwnerCompliancePolicy.</span></span>

|<span data-ttu-id="64288-130">属性</span><span class="sxs-lookup"><span data-stu-id="64288-130">Property</span></span>|<span data-ttu-id="64288-131">类型</span><span class="sxs-lookup"><span data-stu-id="64288-131">Type</span></span>|<span data-ttu-id="64288-132">说明</span><span class="sxs-lookup"><span data-stu-id="64288-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="64288-133">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="64288-133">roleScopeTagIds</span></span>|<span data-ttu-id="64288-134">String 集合</span><span class="sxs-lookup"><span data-stu-id="64288-134">String collection</span></span>|<span data-ttu-id="64288-135">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="64288-135">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="64288-136">继承自 [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="64288-136">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="64288-137">id</span><span class="sxs-lookup"><span data-stu-id="64288-137">id</span></span>|<span data-ttu-id="64288-138">字符串</span><span class="sxs-lookup"><span data-stu-id="64288-138">String</span></span>|<span data-ttu-id="64288-139">实体的键。</span><span class="sxs-lookup"><span data-stu-id="64288-139">Key of the entity.</span></span> <span data-ttu-id="64288-140">继承自 [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="64288-140">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="64288-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="64288-141">createdDateTime</span></span>|<span data-ttu-id="64288-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="64288-142">DateTimeOffset</span></span>|<span data-ttu-id="64288-143">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="64288-143">DateTime the object was created.</span></span> <span data-ttu-id="64288-144">继承自 [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="64288-144">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="64288-145">说明</span><span class="sxs-lookup"><span data-stu-id="64288-145">description</span></span>|<span data-ttu-id="64288-146">String</span><span class="sxs-lookup"><span data-stu-id="64288-146">String</span></span>|<span data-ttu-id="64288-147">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="64288-147">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="64288-148">继承自 [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="64288-148">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="64288-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="64288-149">lastModifiedDateTime</span></span>|<span data-ttu-id="64288-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="64288-150">DateTimeOffset</span></span>|<span data-ttu-id="64288-151">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="64288-151">DateTime the object was last modified.</span></span> <span data-ttu-id="64288-152">继承自 [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="64288-152">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="64288-153">displayName</span><span class="sxs-lookup"><span data-stu-id="64288-153">displayName</span></span>|<span data-ttu-id="64288-154">字符串</span><span class="sxs-lookup"><span data-stu-id="64288-154">String</span></span>|<span data-ttu-id="64288-155">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="64288-155">Admin provided name of the device configuration.</span></span> <span data-ttu-id="64288-156">继承自 [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="64288-156">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="64288-157">version</span><span class="sxs-lookup"><span data-stu-id="64288-157">version</span></span>|<span data-ttu-id="64288-158">Int32</span><span class="sxs-lookup"><span data-stu-id="64288-158">Int32</span></span>|<span data-ttu-id="64288-159">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="64288-159">Version of the device configuration.</span></span> <span data-ttu-id="64288-160">继承自 [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="64288-160">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="64288-161">deviceThreatProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="64288-161">deviceThreatProtectionEnabled</span></span>|<span data-ttu-id="64288-162">布尔</span><span class="sxs-lookup"><span data-stu-id="64288-162">Boolean</span></span>|<span data-ttu-id="64288-163">要求设备已启用设备威胁防护。</span><span class="sxs-lookup"><span data-stu-id="64288-163">Require that devices have enabled device threat protection.</span></span>|
|<span data-ttu-id="64288-164">deviceThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="64288-164">deviceThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="64288-165">deviceThreatProtectionLevel</span><span class="sxs-lookup"><span data-stu-id="64288-165">deviceThreatProtectionLevel</span></span>](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|<span data-ttu-id="64288-166">要求移动威胁防护最低风险级别来报告不符合情况。</span><span class="sxs-lookup"><span data-stu-id="64288-166">Require Mobile Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="64288-167">可取值为：`unavailable`、`secured`、`low`、`medium`、`high`、`notSet`。</span><span class="sxs-lookup"><span data-stu-id="64288-167">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="64288-168">advancedThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="64288-168">advancedThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="64288-169">deviceThreatProtectionLevel</span><span class="sxs-lookup"><span data-stu-id="64288-169">deviceThreatProtectionLevel</span></span>](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|<span data-ttu-id="64288-170">MDATP 要求移动威胁防护最低风险级别来报告不合规。</span><span class="sxs-lookup"><span data-stu-id="64288-170">MDATP Require Mobile Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="64288-171">可取值为：`unavailable`、`secured`、`low`、`medium`、`high`、`notSet`。</span><span class="sxs-lookup"><span data-stu-id="64288-171">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="64288-172">securityRequireSafetyNetAttestationBasicIntegrity</span><span class="sxs-lookup"><span data-stu-id="64288-172">securityRequireSafetyNetAttestationBasicIntegrity</span></span>|<span data-ttu-id="64288-173">布尔</span><span class="sxs-lookup"><span data-stu-id="64288-173">Boolean</span></span>|<span data-ttu-id="64288-174">要求设备传递 SafetyNet 基本完整性检查。</span><span class="sxs-lookup"><span data-stu-id="64288-174">Require the device to pass the SafetyNet basic integrity check.</span></span>|
|<span data-ttu-id="64288-175">securityRequireSafetyNetAttestationCertifiedDevice</span><span class="sxs-lookup"><span data-stu-id="64288-175">securityRequireSafetyNetAttestationCertifiedDevice</span></span>|<span data-ttu-id="64288-176">Boolean</span><span class="sxs-lookup"><span data-stu-id="64288-176">Boolean</span></span>|<span data-ttu-id="64288-177">要求设备传递 SafetyNet 认证设备检查。</span><span class="sxs-lookup"><span data-stu-id="64288-177">Require the device to pass the SafetyNet certified device check.</span></span>|
|<span data-ttu-id="64288-178">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="64288-178">osMinimumVersion</span></span>|<span data-ttu-id="64288-179">String</span><span class="sxs-lookup"><span data-stu-id="64288-179">String</span></span>|<span data-ttu-id="64288-180">最低 Android 版本。</span><span class="sxs-lookup"><span data-stu-id="64288-180">Minimum Android version.</span></span>|
|<span data-ttu-id="64288-181">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="64288-181">osMaximumVersion</span></span>|<span data-ttu-id="64288-182">String</span><span class="sxs-lookup"><span data-stu-id="64288-182">String</span></span>|<span data-ttu-id="64288-183">最高 Android 版本。</span><span class="sxs-lookup"><span data-stu-id="64288-183">Maximum Android version.</span></span>|
|<span data-ttu-id="64288-184">minAndroidSecurityPatchLevel</span><span class="sxs-lookup"><span data-stu-id="64288-184">minAndroidSecurityPatchLevel</span></span>|<span data-ttu-id="64288-185">String</span><span class="sxs-lookup"><span data-stu-id="64288-185">String</span></span>|<span data-ttu-id="64288-186">最低 Android 安全修补程序级别。</span><span class="sxs-lookup"><span data-stu-id="64288-186">Minimum Android security patch level.</span></span>|
|<span data-ttu-id="64288-187">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="64288-187">passwordRequired</span></span>|<span data-ttu-id="64288-188">布尔</span><span class="sxs-lookup"><span data-stu-id="64288-188">Boolean</span></span>|<span data-ttu-id="64288-189">需要密码才可解锁设备。</span><span class="sxs-lookup"><span data-stu-id="64288-189">Require a password to unlock device.</span></span>|
|<span data-ttu-id="64288-190">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="64288-190">passwordMinimumLength</span></span>|<span data-ttu-id="64288-191">Int32</span><span class="sxs-lookup"><span data-stu-id="64288-191">Int32</span></span>|<span data-ttu-id="64288-192">最短密码长度。</span><span class="sxs-lookup"><span data-stu-id="64288-192">Minimum password length.</span></span> <span data-ttu-id="64288-193">有效值为 4 至 16</span><span class="sxs-lookup"><span data-stu-id="64288-193">Valid values 4 to 16</span></span>|
|<span data-ttu-id="64288-194">passwordMinimumLetterCharacters</span><span class="sxs-lookup"><span data-stu-id="64288-194">passwordMinimumLetterCharacters</span></span>|<span data-ttu-id="64288-195">Int32</span><span class="sxs-lookup"><span data-stu-id="64288-195">Int32</span></span>|<span data-ttu-id="64288-196">指示设备密码所需的字母字符的最小数量。</span><span class="sxs-lookup"><span data-stu-id="64288-196">Indicates the minimum number of letter characters required for device password.</span></span> <span data-ttu-id="64288-197">有效值为1至16</span><span class="sxs-lookup"><span data-stu-id="64288-197">Valid values 1 to 16</span></span>|
|<span data-ttu-id="64288-198">passwordMinimumLowerCaseCharacters</span><span class="sxs-lookup"><span data-stu-id="64288-198">passwordMinimumLowerCaseCharacters</span></span>|<span data-ttu-id="64288-199">Int32</span><span class="sxs-lookup"><span data-stu-id="64288-199">Int32</span></span>|<span data-ttu-id="64288-200">指示设备密码所需的最小小写字符数。</span><span class="sxs-lookup"><span data-stu-id="64288-200">Indicates the minimum number of lower case characters required for device password.</span></span> <span data-ttu-id="64288-201">有效值为1至16</span><span class="sxs-lookup"><span data-stu-id="64288-201">Valid values 1 to 16</span></span>|
|<span data-ttu-id="64288-202">passwordMinimumNonLetterCharacters</span><span class="sxs-lookup"><span data-stu-id="64288-202">passwordMinimumNonLetterCharacters</span></span>|<span data-ttu-id="64288-203">Int32</span><span class="sxs-lookup"><span data-stu-id="64288-203">Int32</span></span>|<span data-ttu-id="64288-204">指示设备密码所需的最小非字母字符数。</span><span class="sxs-lookup"><span data-stu-id="64288-204">Indicates the minimum number of non-letter characters required for device password.</span></span> <span data-ttu-id="64288-205">有效值为1至16</span><span class="sxs-lookup"><span data-stu-id="64288-205">Valid values 1 to 16</span></span>|
|<span data-ttu-id="64288-206">passwordMinimumNumericCharacters</span><span class="sxs-lookup"><span data-stu-id="64288-206">passwordMinimumNumericCharacters</span></span>|<span data-ttu-id="64288-207">Int32</span><span class="sxs-lookup"><span data-stu-id="64288-207">Int32</span></span>|<span data-ttu-id="64288-208">指示设备密码所需的最小数字字符数。</span><span class="sxs-lookup"><span data-stu-id="64288-208">Indicates the minimum number of numeric characters required for device password.</span></span> <span data-ttu-id="64288-209">有效值为1至16</span><span class="sxs-lookup"><span data-stu-id="64288-209">Valid values 1 to 16</span></span>|
|<span data-ttu-id="64288-210">passwordMinimumSymbolCharacters</span><span class="sxs-lookup"><span data-stu-id="64288-210">passwordMinimumSymbolCharacters</span></span>|<span data-ttu-id="64288-211">Int32</span><span class="sxs-lookup"><span data-stu-id="64288-211">Int32</span></span>|<span data-ttu-id="64288-212">指示设备密码所需的最小符号字符数。</span><span class="sxs-lookup"><span data-stu-id="64288-212">Indicates the minimum number of symbol characters required for device password.</span></span> <span data-ttu-id="64288-213">有效值为1至16</span><span class="sxs-lookup"><span data-stu-id="64288-213">Valid values 1 to 16</span></span>|
|<span data-ttu-id="64288-214">passwordMinimumUpperCaseCharacters</span><span class="sxs-lookup"><span data-stu-id="64288-214">passwordMinimumUpperCaseCharacters</span></span>|<span data-ttu-id="64288-215">Int32</span><span class="sxs-lookup"><span data-stu-id="64288-215">Int32</span></span>|<span data-ttu-id="64288-216">指示设备密码所需的大写字母字符的最小数量。</span><span class="sxs-lookup"><span data-stu-id="64288-216">Indicates the minimum number of upper case letter characters required for device password.</span></span> <span data-ttu-id="64288-217">有效值为1至16</span><span class="sxs-lookup"><span data-stu-id="64288-217">Valid values 1 to 16</span></span>|
|<span data-ttu-id="64288-218">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="64288-218">passwordRequiredType</span></span>|[<span data-ttu-id="64288-219">androidDeviceOwnerRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="64288-219">androidDeviceOwnerRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androiddeviceownerrequiredpasswordtype.md)|<span data-ttu-id="64288-220">密码中的字符类型。</span><span class="sxs-lookup"><span data-stu-id="64288-220">Type of characters in password.</span></span> <span data-ttu-id="64288-221">可取值为：`deviceDefault`、`required`、`numeric`、`numericComplex`、`alphabetic`、`alphanumeric`、`alphanumericWithSymbols`、`lowSecurityBiometric`、`customPassword`。</span><span class="sxs-lookup"><span data-stu-id="64288-221">Possible values are: `deviceDefault`, `required`, `numeric`, `numericComplex`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `customPassword`.</span></span>|
|<span data-ttu-id="64288-222">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="64288-222">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="64288-223">Int32</span><span class="sxs-lookup"><span data-stu-id="64288-223">Int32</span></span>|<span data-ttu-id="64288-224">在需要密码之前不活动的分钟数。</span><span class="sxs-lookup"><span data-stu-id="64288-224">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="64288-225">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="64288-225">passwordExpirationDays</span></span>|<span data-ttu-id="64288-226">Int32</span><span class="sxs-lookup"><span data-stu-id="64288-226">Int32</span></span>|<span data-ttu-id="64288-227">密码过期前的天数。</span><span class="sxs-lookup"><span data-stu-id="64288-227">Number of days before the password expires.</span></span> <span data-ttu-id="64288-228">有效值为 1 至 365。</span><span class="sxs-lookup"><span data-stu-id="64288-228">Valid values 1 to 365</span></span>|
|<span data-ttu-id="64288-229">passwordPreviousPasswordCountToBlock</span><span class="sxs-lookup"><span data-stu-id="64288-229">passwordPreviousPasswordCountToBlock</span></span>|<span data-ttu-id="64288-230">Int32</span><span class="sxs-lookup"><span data-stu-id="64288-230">Int32</span></span>|<span data-ttu-id="64288-231">要阻止的以前密码的数量。</span><span class="sxs-lookup"><span data-stu-id="64288-231">Number of previous passwords to block.</span></span> <span data-ttu-id="64288-232">有效值为 1 至 24</span><span class="sxs-lookup"><span data-stu-id="64288-232">Valid values 1 to 24</span></span>|
|<span data-ttu-id="64288-233">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="64288-233">storageRequireEncryption</span></span>|<span data-ttu-id="64288-234">Boolean</span><span class="sxs-lookup"><span data-stu-id="64288-234">Boolean</span></span>|<span data-ttu-id="64288-235">要求对 Android 设备加密。</span><span class="sxs-lookup"><span data-stu-id="64288-235">Require encryption on Android devices.</span></span>|



## <a name="response"></a><span data-ttu-id="64288-236">响应</span><span class="sxs-lookup"><span data-stu-id="64288-236">Response</span></span>
<span data-ttu-id="64288-237">如果成功，此方法在响应`201 Created`正文中返回响应代码和[androidDeviceOwnerCompliancePolicy](../resources/intune-deviceconfig-androiddeviceownercompliancepolicy.md)对象。</span><span class="sxs-lookup"><span data-stu-id="64288-237">If successful, this method returns a `201 Created` response code and a [androidDeviceOwnerCompliancePolicy](../resources/intune-deviceconfig-androiddeviceownercompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="64288-238">示例</span><span class="sxs-lookup"><span data-stu-id="64288-238">Example</span></span>

### <a name="request"></a><span data-ttu-id="64288-239">请求</span><span class="sxs-lookup"><span data-stu-id="64288-239">Request</span></span>
<span data-ttu-id="64288-240">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="64288-240">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies
Content-type: application/json
Content-length: 1223

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
  "advancedThreatProtectionRequiredSecurityLevel": "secured",
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

### <a name="response"></a><span data-ttu-id="64288-241">响应</span><span class="sxs-lookup"><span data-stu-id="64288-241">Response</span></span>
<span data-ttu-id="64288-p121">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="64288-p121">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1395

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
  "advancedThreatProtectionRequiredSecurityLevel": "secured",
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





