---
title: 更新 androidDeviceOwnerCompliancePolicy
description: 更新 androidDeviceOwnerCompliancePolicy 对象的属性。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 818e7a1717c079c1dbc0f45da898d2494098d83a
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42759862"
---
# <a name="update-androiddeviceownercompliancepolicy"></a><span data-ttu-id="bff4d-103">更新 androidDeviceOwnerCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="bff4d-103">Update androidDeviceOwnerCompliancePolicy</span></span>

> <span data-ttu-id="bff4d-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="bff4d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bff4d-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="bff4d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bff4d-106">更新[androidDeviceOwnerCompliancePolicy](../resources/intune-deviceconfig-androiddeviceownercompliancepolicy.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="bff4d-106">Update the properties of a [androidDeviceOwnerCompliancePolicy](../resources/intune-deviceconfig-androiddeviceownercompliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bff4d-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="bff4d-107">Prerequisites</span></span>
<span data-ttu-id="bff4d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="bff4d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bff4d-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="bff4d-110">Permission type</span></span>|<span data-ttu-id="bff4d-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="bff4d-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bff4d-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="bff4d-112">Delegated (work or school account)</span></span>|<span data-ttu-id="bff4d-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bff4d-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="bff4d-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="bff4d-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bff4d-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="bff4d-115">Not supported.</span></span>|
|<span data-ttu-id="bff4d-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="bff4d-116">Application</span></span>|<span data-ttu-id="bff4d-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bff4d-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="bff4d-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="bff4d-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="bff4d-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="bff4d-119">Request headers</span></span>
|<span data-ttu-id="bff4d-120">标头</span><span class="sxs-lookup"><span data-stu-id="bff4d-120">Header</span></span>|<span data-ttu-id="bff4d-121">值</span><span class="sxs-lookup"><span data-stu-id="bff4d-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bff4d-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="bff4d-122">Authorization</span></span>|<span data-ttu-id="bff4d-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="bff4d-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bff4d-124">接受</span><span class="sxs-lookup"><span data-stu-id="bff4d-124">Accept</span></span>|<span data-ttu-id="bff4d-125">application/json</span><span class="sxs-lookup"><span data-stu-id="bff4d-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bff4d-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="bff4d-126">Request body</span></span>
<span data-ttu-id="bff4d-127">在请求正文中，提供[androidDeviceOwnerCompliancePolicy](../resources/intune-deviceconfig-androiddeviceownercompliancepolicy.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="bff4d-127">In the request body, supply a JSON representation for the [androidDeviceOwnerCompliancePolicy](../resources/intune-deviceconfig-androiddeviceownercompliancepolicy.md) object.</span></span>

<span data-ttu-id="bff4d-128">下表显示创建[androidDeviceOwnerCompliancePolicy](../resources/intune-deviceconfig-androiddeviceownercompliancepolicy.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="bff4d-128">The following table shows the properties that are required when you create the [androidDeviceOwnerCompliancePolicy](../resources/intune-deviceconfig-androiddeviceownercompliancepolicy.md).</span></span>

|<span data-ttu-id="bff4d-129">属性</span><span class="sxs-lookup"><span data-stu-id="bff4d-129">Property</span></span>|<span data-ttu-id="bff4d-130">类型</span><span class="sxs-lookup"><span data-stu-id="bff4d-130">Type</span></span>|<span data-ttu-id="bff4d-131">说明</span><span class="sxs-lookup"><span data-stu-id="bff4d-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bff4d-132">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="bff4d-132">roleScopeTagIds</span></span>|<span data-ttu-id="bff4d-133">String collection</span><span class="sxs-lookup"><span data-stu-id="bff4d-133">String collection</span></span>|<span data-ttu-id="bff4d-134">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="bff4d-134">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="bff4d-135">继承自 [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="bff4d-135">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="bff4d-136">id</span><span class="sxs-lookup"><span data-stu-id="bff4d-136">id</span></span>|<span data-ttu-id="bff4d-137">字符串</span><span class="sxs-lookup"><span data-stu-id="bff4d-137">String</span></span>|<span data-ttu-id="bff4d-138">实体的键。</span><span class="sxs-lookup"><span data-stu-id="bff4d-138">Key of the entity.</span></span> <span data-ttu-id="bff4d-139">继承自 [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="bff4d-139">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="bff4d-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="bff4d-140">createdDateTime</span></span>|<span data-ttu-id="bff4d-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bff4d-141">DateTimeOffset</span></span>|<span data-ttu-id="bff4d-142">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="bff4d-142">DateTime the object was created.</span></span> <span data-ttu-id="bff4d-143">继承自 [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="bff4d-143">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="bff4d-144">说明</span><span class="sxs-lookup"><span data-stu-id="bff4d-144">description</span></span>|<span data-ttu-id="bff4d-145">String</span><span class="sxs-lookup"><span data-stu-id="bff4d-145">String</span></span>|<span data-ttu-id="bff4d-146">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="bff4d-146">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="bff4d-147">继承自 [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="bff4d-147">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="bff4d-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="bff4d-148">lastModifiedDateTime</span></span>|<span data-ttu-id="bff4d-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bff4d-149">DateTimeOffset</span></span>|<span data-ttu-id="bff4d-150">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="bff4d-150">DateTime the object was last modified.</span></span> <span data-ttu-id="bff4d-151">继承自 [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="bff4d-151">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="bff4d-152">displayName</span><span class="sxs-lookup"><span data-stu-id="bff4d-152">displayName</span></span>|<span data-ttu-id="bff4d-153">字符串</span><span class="sxs-lookup"><span data-stu-id="bff4d-153">String</span></span>|<span data-ttu-id="bff4d-154">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="bff4d-154">Admin provided name of the device configuration.</span></span> <span data-ttu-id="bff4d-155">继承自 [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="bff4d-155">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="bff4d-156">version</span><span class="sxs-lookup"><span data-stu-id="bff4d-156">version</span></span>|<span data-ttu-id="bff4d-157">Int32</span><span class="sxs-lookup"><span data-stu-id="bff4d-157">Int32</span></span>|<span data-ttu-id="bff4d-158">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="bff4d-158">Version of the device configuration.</span></span> <span data-ttu-id="bff4d-159">继承自 [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="bff4d-159">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="bff4d-160">deviceThreatProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="bff4d-160">deviceThreatProtectionEnabled</span></span>|<span data-ttu-id="bff4d-161">布尔值</span><span class="sxs-lookup"><span data-stu-id="bff4d-161">Boolean</span></span>|<span data-ttu-id="bff4d-162">要求设备已启用设备威胁防护。</span><span class="sxs-lookup"><span data-stu-id="bff4d-162">Require that devices have enabled device threat protection.</span></span>|
|<span data-ttu-id="bff4d-163">deviceThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="bff4d-163">deviceThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="bff4d-164">deviceThreatProtectionLevel</span><span class="sxs-lookup"><span data-stu-id="bff4d-164">deviceThreatProtectionLevel</span></span>](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|<span data-ttu-id="bff4d-165">要求移动威胁防护最低风险级别来报告不符合情况。</span><span class="sxs-lookup"><span data-stu-id="bff4d-165">Require Mobile Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="bff4d-166">可取值为：`unavailable`、`secured`、`low`、`medium`、`high`、`notSet`。</span><span class="sxs-lookup"><span data-stu-id="bff4d-166">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="bff4d-167">advancedThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="bff4d-167">advancedThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="bff4d-168">deviceThreatProtectionLevel</span><span class="sxs-lookup"><span data-stu-id="bff4d-168">deviceThreatProtectionLevel</span></span>](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|<span data-ttu-id="bff4d-169">MDATP 要求移动威胁防护最低风险级别来报告不合规。</span><span class="sxs-lookup"><span data-stu-id="bff4d-169">MDATP Require Mobile Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="bff4d-170">可取值为：`unavailable`、`secured`、`low`、`medium`、`high`、`notSet`。</span><span class="sxs-lookup"><span data-stu-id="bff4d-170">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="bff4d-171">securityRequireSafetyNetAttestationBasicIntegrity</span><span class="sxs-lookup"><span data-stu-id="bff4d-171">securityRequireSafetyNetAttestationBasicIntegrity</span></span>|<span data-ttu-id="bff4d-172">布尔值</span><span class="sxs-lookup"><span data-stu-id="bff4d-172">Boolean</span></span>|<span data-ttu-id="bff4d-173">要求设备传递 SafetyNet 基本完整性检查。</span><span class="sxs-lookup"><span data-stu-id="bff4d-173">Require the device to pass the SafetyNet basic integrity check.</span></span>|
|<span data-ttu-id="bff4d-174">securityRequireSafetyNetAttestationCertifiedDevice</span><span class="sxs-lookup"><span data-stu-id="bff4d-174">securityRequireSafetyNetAttestationCertifiedDevice</span></span>|<span data-ttu-id="bff4d-175">Boolean</span><span class="sxs-lookup"><span data-stu-id="bff4d-175">Boolean</span></span>|<span data-ttu-id="bff4d-176">要求设备传递 SafetyNet 认证设备检查。</span><span class="sxs-lookup"><span data-stu-id="bff4d-176">Require the device to pass the SafetyNet certified device check.</span></span>|
|<span data-ttu-id="bff4d-177">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="bff4d-177">osMinimumVersion</span></span>|<span data-ttu-id="bff4d-178">String</span><span class="sxs-lookup"><span data-stu-id="bff4d-178">String</span></span>|<span data-ttu-id="bff4d-179">最低 Android 版本。</span><span class="sxs-lookup"><span data-stu-id="bff4d-179">Minimum Android version.</span></span>|
|<span data-ttu-id="bff4d-180">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="bff4d-180">osMaximumVersion</span></span>|<span data-ttu-id="bff4d-181">String</span><span class="sxs-lookup"><span data-stu-id="bff4d-181">String</span></span>|<span data-ttu-id="bff4d-182">最高 Android 版本。</span><span class="sxs-lookup"><span data-stu-id="bff4d-182">Maximum Android version.</span></span>|
|<span data-ttu-id="bff4d-183">minAndroidSecurityPatchLevel</span><span class="sxs-lookup"><span data-stu-id="bff4d-183">minAndroidSecurityPatchLevel</span></span>|<span data-ttu-id="bff4d-184">String</span><span class="sxs-lookup"><span data-stu-id="bff4d-184">String</span></span>|<span data-ttu-id="bff4d-185">最低 Android 安全修补程序级别。</span><span class="sxs-lookup"><span data-stu-id="bff4d-185">Minimum Android security patch level.</span></span>|
|<span data-ttu-id="bff4d-186">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="bff4d-186">passwordRequired</span></span>|<span data-ttu-id="bff4d-187">布尔值</span><span class="sxs-lookup"><span data-stu-id="bff4d-187">Boolean</span></span>|<span data-ttu-id="bff4d-188">需要密码才可解锁设备。</span><span class="sxs-lookup"><span data-stu-id="bff4d-188">Require a password to unlock device.</span></span>|
|<span data-ttu-id="bff4d-189">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="bff4d-189">passwordMinimumLength</span></span>|<span data-ttu-id="bff4d-190">Int32</span><span class="sxs-lookup"><span data-stu-id="bff4d-190">Int32</span></span>|<span data-ttu-id="bff4d-191">最短密码长度。</span><span class="sxs-lookup"><span data-stu-id="bff4d-191">Minimum password length.</span></span> <span data-ttu-id="bff4d-192">有效值为 4 至 16</span><span class="sxs-lookup"><span data-stu-id="bff4d-192">Valid values 4 to 16</span></span>|
|<span data-ttu-id="bff4d-193">passwordMinimumLetterCharacters</span><span class="sxs-lookup"><span data-stu-id="bff4d-193">passwordMinimumLetterCharacters</span></span>|<span data-ttu-id="bff4d-194">Int32</span><span class="sxs-lookup"><span data-stu-id="bff4d-194">Int32</span></span>|<span data-ttu-id="bff4d-195">指示设备密码所需的字母字符的最小数量。</span><span class="sxs-lookup"><span data-stu-id="bff4d-195">Indicates the minimum number of letter characters required for device password.</span></span> <span data-ttu-id="bff4d-196">有效值为1至16</span><span class="sxs-lookup"><span data-stu-id="bff4d-196">Valid values 1 to 16</span></span>|
|<span data-ttu-id="bff4d-197">passwordMinimumLowerCaseCharacters</span><span class="sxs-lookup"><span data-stu-id="bff4d-197">passwordMinimumLowerCaseCharacters</span></span>|<span data-ttu-id="bff4d-198">Int32</span><span class="sxs-lookup"><span data-stu-id="bff4d-198">Int32</span></span>|<span data-ttu-id="bff4d-199">指示设备密码所需的最小小写字符数。</span><span class="sxs-lookup"><span data-stu-id="bff4d-199">Indicates the minimum number of lower case characters required for device password.</span></span> <span data-ttu-id="bff4d-200">有效值为1至16</span><span class="sxs-lookup"><span data-stu-id="bff4d-200">Valid values 1 to 16</span></span>|
|<span data-ttu-id="bff4d-201">passwordMinimumNonLetterCharacters</span><span class="sxs-lookup"><span data-stu-id="bff4d-201">passwordMinimumNonLetterCharacters</span></span>|<span data-ttu-id="bff4d-202">Int32</span><span class="sxs-lookup"><span data-stu-id="bff4d-202">Int32</span></span>|<span data-ttu-id="bff4d-203">指示设备密码所需的最小非字母字符数。</span><span class="sxs-lookup"><span data-stu-id="bff4d-203">Indicates the minimum number of non-letter characters required for device password.</span></span> <span data-ttu-id="bff4d-204">有效值为1至16</span><span class="sxs-lookup"><span data-stu-id="bff4d-204">Valid values 1 to 16</span></span>|
|<span data-ttu-id="bff4d-205">passwordMinimumNumericCharacters</span><span class="sxs-lookup"><span data-stu-id="bff4d-205">passwordMinimumNumericCharacters</span></span>|<span data-ttu-id="bff4d-206">Int32</span><span class="sxs-lookup"><span data-stu-id="bff4d-206">Int32</span></span>|<span data-ttu-id="bff4d-207">指示设备密码所需的最小数字字符数。</span><span class="sxs-lookup"><span data-stu-id="bff4d-207">Indicates the minimum number of numeric characters required for device password.</span></span> <span data-ttu-id="bff4d-208">有效值为1至16</span><span class="sxs-lookup"><span data-stu-id="bff4d-208">Valid values 1 to 16</span></span>|
|<span data-ttu-id="bff4d-209">passwordMinimumSymbolCharacters</span><span class="sxs-lookup"><span data-stu-id="bff4d-209">passwordMinimumSymbolCharacters</span></span>|<span data-ttu-id="bff4d-210">Int32</span><span class="sxs-lookup"><span data-stu-id="bff4d-210">Int32</span></span>|<span data-ttu-id="bff4d-211">指示设备密码所需的最小符号字符数。</span><span class="sxs-lookup"><span data-stu-id="bff4d-211">Indicates the minimum number of symbol characters required for device password.</span></span> <span data-ttu-id="bff4d-212">有效值为1至16</span><span class="sxs-lookup"><span data-stu-id="bff4d-212">Valid values 1 to 16</span></span>|
|<span data-ttu-id="bff4d-213">passwordMinimumUpperCaseCharacters</span><span class="sxs-lookup"><span data-stu-id="bff4d-213">passwordMinimumUpperCaseCharacters</span></span>|<span data-ttu-id="bff4d-214">Int32</span><span class="sxs-lookup"><span data-stu-id="bff4d-214">Int32</span></span>|<span data-ttu-id="bff4d-215">指示设备密码所需的大写字母字符的最小数量。</span><span class="sxs-lookup"><span data-stu-id="bff4d-215">Indicates the minimum number of upper case letter characters required for device password.</span></span> <span data-ttu-id="bff4d-216">有效值为1至16</span><span class="sxs-lookup"><span data-stu-id="bff4d-216">Valid values 1 to 16</span></span>|
|<span data-ttu-id="bff4d-217">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="bff4d-217">passwordRequiredType</span></span>|[<span data-ttu-id="bff4d-218">androidDeviceOwnerRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="bff4d-218">androidDeviceOwnerRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androiddeviceownerrequiredpasswordtype.md)|<span data-ttu-id="bff4d-219">密码中的字符类型。</span><span class="sxs-lookup"><span data-stu-id="bff4d-219">Type of characters in password.</span></span> <span data-ttu-id="bff4d-220">可取值为：`deviceDefault`、`required`、`numeric`、`numericComplex`、`alphabetic`、`alphanumeric`、`alphanumericWithSymbols`、`lowSecurityBiometric`、`customPassword`。</span><span class="sxs-lookup"><span data-stu-id="bff4d-220">Possible values are: `deviceDefault`, `required`, `numeric`, `numericComplex`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `customPassword`.</span></span>|
|<span data-ttu-id="bff4d-221">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="bff4d-221">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="bff4d-222">Int32</span><span class="sxs-lookup"><span data-stu-id="bff4d-222">Int32</span></span>|<span data-ttu-id="bff4d-223">在需要密码之前不活动的分钟数。</span><span class="sxs-lookup"><span data-stu-id="bff4d-223">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="bff4d-224">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="bff4d-224">passwordExpirationDays</span></span>|<span data-ttu-id="bff4d-225">Int32</span><span class="sxs-lookup"><span data-stu-id="bff4d-225">Int32</span></span>|<span data-ttu-id="bff4d-226">密码过期前的天数。</span><span class="sxs-lookup"><span data-stu-id="bff4d-226">Number of days before the password expires.</span></span> <span data-ttu-id="bff4d-227">有效值为 1 至 365。</span><span class="sxs-lookup"><span data-stu-id="bff4d-227">Valid values 1 to 365</span></span>|
|<span data-ttu-id="bff4d-228">passwordPreviousPasswordCountToBlock</span><span class="sxs-lookup"><span data-stu-id="bff4d-228">passwordPreviousPasswordCountToBlock</span></span>|<span data-ttu-id="bff4d-229">Int32</span><span class="sxs-lookup"><span data-stu-id="bff4d-229">Int32</span></span>|<span data-ttu-id="bff4d-230">要阻止的以前密码的数量。</span><span class="sxs-lookup"><span data-stu-id="bff4d-230">Number of previous passwords to block.</span></span> <span data-ttu-id="bff4d-231">有效值为 1 至 24</span><span class="sxs-lookup"><span data-stu-id="bff4d-231">Valid values 1 to 24</span></span>|
|<span data-ttu-id="bff4d-232">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="bff4d-232">storageRequireEncryption</span></span>|<span data-ttu-id="bff4d-233">Boolean</span><span class="sxs-lookup"><span data-stu-id="bff4d-233">Boolean</span></span>|<span data-ttu-id="bff4d-234">要求对 Android 设备加密。</span><span class="sxs-lookup"><span data-stu-id="bff4d-234">Require encryption on Android devices.</span></span>|



## <a name="response"></a><span data-ttu-id="bff4d-235">响应</span><span class="sxs-lookup"><span data-stu-id="bff4d-235">Response</span></span>
<span data-ttu-id="bff4d-236">如果成功，此方法在响应`200 OK`正文中返回响应代码和更新的[androidDeviceOwnerCompliancePolicy](../resources/intune-deviceconfig-androiddeviceownercompliancepolicy.md)对象。</span><span class="sxs-lookup"><span data-stu-id="bff4d-236">If successful, this method returns a `200 OK` response code and an updated [androidDeviceOwnerCompliancePolicy](../resources/intune-deviceconfig-androiddeviceownercompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bff4d-237">示例</span><span class="sxs-lookup"><span data-stu-id="bff4d-237">Example</span></span>

### <a name="request"></a><span data-ttu-id="bff4d-238">请求</span><span class="sxs-lookup"><span data-stu-id="bff4d-238">Request</span></span>
<span data-ttu-id="bff4d-239">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="bff4d-239">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
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

### <a name="response"></a><span data-ttu-id="bff4d-240">响应</span><span class="sxs-lookup"><span data-stu-id="bff4d-240">Response</span></span>
<span data-ttu-id="bff4d-p121">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="bff4d-p121">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




