---
title: 更新 androidDeviceOwnerCompliancePolicy
description: 更新 androidDeviceOwnerCompliancePolicy 对象的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 7ce02b9ab27b3382da6ddad0be802d3be46f653f
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42450088"
---
# <a name="update-androiddeviceownercompliancepolicy"></a><span data-ttu-id="2b2aa-103">更新 androidDeviceOwnerCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="2b2aa-103">Update androidDeviceOwnerCompliancePolicy</span></span>

<span data-ttu-id="2b2aa-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="2b2aa-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2b2aa-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="2b2aa-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2b2aa-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="2b2aa-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2b2aa-107">更新[androidDeviceOwnerCompliancePolicy](../resources/intune-deviceconfig-androiddeviceownercompliancepolicy.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="2b2aa-107">Update the properties of a [androidDeviceOwnerCompliancePolicy](../resources/intune-deviceconfig-androiddeviceownercompliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2b2aa-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="2b2aa-108">Prerequisites</span></span>
<span data-ttu-id="2b2aa-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2b2aa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2b2aa-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="2b2aa-111">Permission type</span></span>|<span data-ttu-id="2b2aa-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="2b2aa-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2b2aa-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2b2aa-113">Delegated (work or school account)</span></span>|<span data-ttu-id="2b2aa-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2b2aa-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="2b2aa-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2b2aa-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2b2aa-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="2b2aa-116">Not supported.</span></span>|
|<span data-ttu-id="2b2aa-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="2b2aa-117">Application</span></span>|<span data-ttu-id="2b2aa-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2b2aa-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2b2aa-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2b2aa-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="2b2aa-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="2b2aa-120">Request headers</span></span>
|<span data-ttu-id="2b2aa-121">标头</span><span class="sxs-lookup"><span data-stu-id="2b2aa-121">Header</span></span>|<span data-ttu-id="2b2aa-122">值</span><span class="sxs-lookup"><span data-stu-id="2b2aa-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2b2aa-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="2b2aa-123">Authorization</span></span>|<span data-ttu-id="2b2aa-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="2b2aa-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2b2aa-125">接受</span><span class="sxs-lookup"><span data-stu-id="2b2aa-125">Accept</span></span>|<span data-ttu-id="2b2aa-126">application/json</span><span class="sxs-lookup"><span data-stu-id="2b2aa-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2b2aa-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="2b2aa-127">Request body</span></span>
<span data-ttu-id="2b2aa-128">在请求正文中，提供[androidDeviceOwnerCompliancePolicy](../resources/intune-deviceconfig-androiddeviceownercompliancepolicy.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2b2aa-128">In the request body, supply a JSON representation for the [androidDeviceOwnerCompliancePolicy](../resources/intune-deviceconfig-androiddeviceownercompliancepolicy.md) object.</span></span>

<span data-ttu-id="2b2aa-129">下表显示创建[androidDeviceOwnerCompliancePolicy](../resources/intune-deviceconfig-androiddeviceownercompliancepolicy.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="2b2aa-129">The following table shows the properties that are required when you create the [androidDeviceOwnerCompliancePolicy](../resources/intune-deviceconfig-androiddeviceownercompliancepolicy.md).</span></span>

|<span data-ttu-id="2b2aa-130">属性</span><span class="sxs-lookup"><span data-stu-id="2b2aa-130">Property</span></span>|<span data-ttu-id="2b2aa-131">类型</span><span class="sxs-lookup"><span data-stu-id="2b2aa-131">Type</span></span>|<span data-ttu-id="2b2aa-132">说明</span><span class="sxs-lookup"><span data-stu-id="2b2aa-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2b2aa-133">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="2b2aa-133">roleScopeTagIds</span></span>|<span data-ttu-id="2b2aa-134">String 集合</span><span class="sxs-lookup"><span data-stu-id="2b2aa-134">String collection</span></span>|<span data-ttu-id="2b2aa-135">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="2b2aa-135">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="2b2aa-136">继承自 [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="2b2aa-136">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="2b2aa-137">id</span><span class="sxs-lookup"><span data-stu-id="2b2aa-137">id</span></span>|<span data-ttu-id="2b2aa-138">字符串</span><span class="sxs-lookup"><span data-stu-id="2b2aa-138">String</span></span>|<span data-ttu-id="2b2aa-139">实体的键。</span><span class="sxs-lookup"><span data-stu-id="2b2aa-139">Key of the entity.</span></span> <span data-ttu-id="2b2aa-140">继承自 [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="2b2aa-140">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="2b2aa-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="2b2aa-141">createdDateTime</span></span>|<span data-ttu-id="2b2aa-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2b2aa-142">DateTimeOffset</span></span>|<span data-ttu-id="2b2aa-143">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="2b2aa-143">DateTime the object was created.</span></span> <span data-ttu-id="2b2aa-144">继承自 [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="2b2aa-144">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="2b2aa-145">说明</span><span class="sxs-lookup"><span data-stu-id="2b2aa-145">description</span></span>|<span data-ttu-id="2b2aa-146">String</span><span class="sxs-lookup"><span data-stu-id="2b2aa-146">String</span></span>|<span data-ttu-id="2b2aa-147">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="2b2aa-147">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="2b2aa-148">继承自 [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="2b2aa-148">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="2b2aa-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2b2aa-149">lastModifiedDateTime</span></span>|<span data-ttu-id="2b2aa-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2b2aa-150">DateTimeOffset</span></span>|<span data-ttu-id="2b2aa-151">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="2b2aa-151">DateTime the object was last modified.</span></span> <span data-ttu-id="2b2aa-152">继承自 [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="2b2aa-152">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="2b2aa-153">displayName</span><span class="sxs-lookup"><span data-stu-id="2b2aa-153">displayName</span></span>|<span data-ttu-id="2b2aa-154">字符串</span><span class="sxs-lookup"><span data-stu-id="2b2aa-154">String</span></span>|<span data-ttu-id="2b2aa-155">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="2b2aa-155">Admin provided name of the device configuration.</span></span> <span data-ttu-id="2b2aa-156">继承自 [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="2b2aa-156">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="2b2aa-157">version</span><span class="sxs-lookup"><span data-stu-id="2b2aa-157">version</span></span>|<span data-ttu-id="2b2aa-158">Int32</span><span class="sxs-lookup"><span data-stu-id="2b2aa-158">Int32</span></span>|<span data-ttu-id="2b2aa-159">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="2b2aa-159">Version of the device configuration.</span></span> <span data-ttu-id="2b2aa-160">继承自 [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="2b2aa-160">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="2b2aa-161">deviceThreatProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="2b2aa-161">deviceThreatProtectionEnabled</span></span>|<span data-ttu-id="2b2aa-162">布尔</span><span class="sxs-lookup"><span data-stu-id="2b2aa-162">Boolean</span></span>|<span data-ttu-id="2b2aa-163">要求设备已启用设备威胁防护。</span><span class="sxs-lookup"><span data-stu-id="2b2aa-163">Require that devices have enabled device threat protection.</span></span>|
|<span data-ttu-id="2b2aa-164">deviceThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="2b2aa-164">deviceThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="2b2aa-165">deviceThreatProtectionLevel</span><span class="sxs-lookup"><span data-stu-id="2b2aa-165">deviceThreatProtectionLevel</span></span>](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|<span data-ttu-id="2b2aa-166">要求移动威胁防护最低风险级别来报告不符合情况。</span><span class="sxs-lookup"><span data-stu-id="2b2aa-166">Require Mobile Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="2b2aa-167">可取值为：`unavailable`、`secured`、`low`、`medium`、`high`、`notSet`。</span><span class="sxs-lookup"><span data-stu-id="2b2aa-167">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="2b2aa-168">advancedThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="2b2aa-168">advancedThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="2b2aa-169">deviceThreatProtectionLevel</span><span class="sxs-lookup"><span data-stu-id="2b2aa-169">deviceThreatProtectionLevel</span></span>](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|<span data-ttu-id="2b2aa-170">MDATP 要求移动威胁防护最低风险级别来报告不合规。</span><span class="sxs-lookup"><span data-stu-id="2b2aa-170">MDATP Require Mobile Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="2b2aa-171">可取值为：`unavailable`、`secured`、`low`、`medium`、`high`、`notSet`。</span><span class="sxs-lookup"><span data-stu-id="2b2aa-171">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="2b2aa-172">securityRequireSafetyNetAttestationBasicIntegrity</span><span class="sxs-lookup"><span data-stu-id="2b2aa-172">securityRequireSafetyNetAttestationBasicIntegrity</span></span>|<span data-ttu-id="2b2aa-173">布尔</span><span class="sxs-lookup"><span data-stu-id="2b2aa-173">Boolean</span></span>|<span data-ttu-id="2b2aa-174">要求设备传递 SafetyNet 基本完整性检查。</span><span class="sxs-lookup"><span data-stu-id="2b2aa-174">Require the device to pass the SafetyNet basic integrity check.</span></span>|
|<span data-ttu-id="2b2aa-175">securityRequireSafetyNetAttestationCertifiedDevice</span><span class="sxs-lookup"><span data-stu-id="2b2aa-175">securityRequireSafetyNetAttestationCertifiedDevice</span></span>|<span data-ttu-id="2b2aa-176">Boolean</span><span class="sxs-lookup"><span data-stu-id="2b2aa-176">Boolean</span></span>|<span data-ttu-id="2b2aa-177">要求设备传递 SafetyNet 认证设备检查。</span><span class="sxs-lookup"><span data-stu-id="2b2aa-177">Require the device to pass the SafetyNet certified device check.</span></span>|
|<span data-ttu-id="2b2aa-178">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="2b2aa-178">osMinimumVersion</span></span>|<span data-ttu-id="2b2aa-179">String</span><span class="sxs-lookup"><span data-stu-id="2b2aa-179">String</span></span>|<span data-ttu-id="2b2aa-180">最低 Android 版本。</span><span class="sxs-lookup"><span data-stu-id="2b2aa-180">Minimum Android version.</span></span>|
|<span data-ttu-id="2b2aa-181">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="2b2aa-181">osMaximumVersion</span></span>|<span data-ttu-id="2b2aa-182">String</span><span class="sxs-lookup"><span data-stu-id="2b2aa-182">String</span></span>|<span data-ttu-id="2b2aa-183">最高 Android 版本。</span><span class="sxs-lookup"><span data-stu-id="2b2aa-183">Maximum Android version.</span></span>|
|<span data-ttu-id="2b2aa-184">minAndroidSecurityPatchLevel</span><span class="sxs-lookup"><span data-stu-id="2b2aa-184">minAndroidSecurityPatchLevel</span></span>|<span data-ttu-id="2b2aa-185">String</span><span class="sxs-lookup"><span data-stu-id="2b2aa-185">String</span></span>|<span data-ttu-id="2b2aa-186">最低 Android 安全修补程序级别。</span><span class="sxs-lookup"><span data-stu-id="2b2aa-186">Minimum Android security patch level.</span></span>|
|<span data-ttu-id="2b2aa-187">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="2b2aa-187">passwordRequired</span></span>|<span data-ttu-id="2b2aa-188">布尔</span><span class="sxs-lookup"><span data-stu-id="2b2aa-188">Boolean</span></span>|<span data-ttu-id="2b2aa-189">需要密码才可解锁设备。</span><span class="sxs-lookup"><span data-stu-id="2b2aa-189">Require a password to unlock device.</span></span>|
|<span data-ttu-id="2b2aa-190">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="2b2aa-190">passwordMinimumLength</span></span>|<span data-ttu-id="2b2aa-191">Int32</span><span class="sxs-lookup"><span data-stu-id="2b2aa-191">Int32</span></span>|<span data-ttu-id="2b2aa-192">最短密码长度。</span><span class="sxs-lookup"><span data-stu-id="2b2aa-192">Minimum password length.</span></span> <span data-ttu-id="2b2aa-193">有效值为 4 至 16</span><span class="sxs-lookup"><span data-stu-id="2b2aa-193">Valid values 4 to 16</span></span>|
|<span data-ttu-id="2b2aa-194">passwordMinimumLetterCharacters</span><span class="sxs-lookup"><span data-stu-id="2b2aa-194">passwordMinimumLetterCharacters</span></span>|<span data-ttu-id="2b2aa-195">Int32</span><span class="sxs-lookup"><span data-stu-id="2b2aa-195">Int32</span></span>|<span data-ttu-id="2b2aa-196">指示设备密码所需的字母字符的最小数量。</span><span class="sxs-lookup"><span data-stu-id="2b2aa-196">Indicates the minimum number of letter characters required for device password.</span></span> <span data-ttu-id="2b2aa-197">有效值为1至16</span><span class="sxs-lookup"><span data-stu-id="2b2aa-197">Valid values 1 to 16</span></span>|
|<span data-ttu-id="2b2aa-198">passwordMinimumLowerCaseCharacters</span><span class="sxs-lookup"><span data-stu-id="2b2aa-198">passwordMinimumLowerCaseCharacters</span></span>|<span data-ttu-id="2b2aa-199">Int32</span><span class="sxs-lookup"><span data-stu-id="2b2aa-199">Int32</span></span>|<span data-ttu-id="2b2aa-200">指示设备密码所需的最小小写字符数。</span><span class="sxs-lookup"><span data-stu-id="2b2aa-200">Indicates the minimum number of lower case characters required for device password.</span></span> <span data-ttu-id="2b2aa-201">有效值为1至16</span><span class="sxs-lookup"><span data-stu-id="2b2aa-201">Valid values 1 to 16</span></span>|
|<span data-ttu-id="2b2aa-202">passwordMinimumNonLetterCharacters</span><span class="sxs-lookup"><span data-stu-id="2b2aa-202">passwordMinimumNonLetterCharacters</span></span>|<span data-ttu-id="2b2aa-203">Int32</span><span class="sxs-lookup"><span data-stu-id="2b2aa-203">Int32</span></span>|<span data-ttu-id="2b2aa-204">指示设备密码所需的最小非字母字符数。</span><span class="sxs-lookup"><span data-stu-id="2b2aa-204">Indicates the minimum number of non-letter characters required for device password.</span></span> <span data-ttu-id="2b2aa-205">有效值为1至16</span><span class="sxs-lookup"><span data-stu-id="2b2aa-205">Valid values 1 to 16</span></span>|
|<span data-ttu-id="2b2aa-206">passwordMinimumNumericCharacters</span><span class="sxs-lookup"><span data-stu-id="2b2aa-206">passwordMinimumNumericCharacters</span></span>|<span data-ttu-id="2b2aa-207">Int32</span><span class="sxs-lookup"><span data-stu-id="2b2aa-207">Int32</span></span>|<span data-ttu-id="2b2aa-208">指示设备密码所需的最小数字字符数。</span><span class="sxs-lookup"><span data-stu-id="2b2aa-208">Indicates the minimum number of numeric characters required for device password.</span></span> <span data-ttu-id="2b2aa-209">有效值为1至16</span><span class="sxs-lookup"><span data-stu-id="2b2aa-209">Valid values 1 to 16</span></span>|
|<span data-ttu-id="2b2aa-210">passwordMinimumSymbolCharacters</span><span class="sxs-lookup"><span data-stu-id="2b2aa-210">passwordMinimumSymbolCharacters</span></span>|<span data-ttu-id="2b2aa-211">Int32</span><span class="sxs-lookup"><span data-stu-id="2b2aa-211">Int32</span></span>|<span data-ttu-id="2b2aa-212">指示设备密码所需的最小符号字符数。</span><span class="sxs-lookup"><span data-stu-id="2b2aa-212">Indicates the minimum number of symbol characters required for device password.</span></span> <span data-ttu-id="2b2aa-213">有效值为1至16</span><span class="sxs-lookup"><span data-stu-id="2b2aa-213">Valid values 1 to 16</span></span>|
|<span data-ttu-id="2b2aa-214">passwordMinimumUpperCaseCharacters</span><span class="sxs-lookup"><span data-stu-id="2b2aa-214">passwordMinimumUpperCaseCharacters</span></span>|<span data-ttu-id="2b2aa-215">Int32</span><span class="sxs-lookup"><span data-stu-id="2b2aa-215">Int32</span></span>|<span data-ttu-id="2b2aa-216">指示设备密码所需的大写字母字符的最小数量。</span><span class="sxs-lookup"><span data-stu-id="2b2aa-216">Indicates the minimum number of upper case letter characters required for device password.</span></span> <span data-ttu-id="2b2aa-217">有效值为1至16</span><span class="sxs-lookup"><span data-stu-id="2b2aa-217">Valid values 1 to 16</span></span>|
|<span data-ttu-id="2b2aa-218">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="2b2aa-218">passwordRequiredType</span></span>|[<span data-ttu-id="2b2aa-219">androidDeviceOwnerRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="2b2aa-219">androidDeviceOwnerRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androiddeviceownerrequiredpasswordtype.md)|<span data-ttu-id="2b2aa-220">密码中的字符类型。</span><span class="sxs-lookup"><span data-stu-id="2b2aa-220">Type of characters in password.</span></span> <span data-ttu-id="2b2aa-221">可取值为：`deviceDefault`、`required`、`numeric`、`numericComplex`、`alphabetic`、`alphanumeric`、`alphanumericWithSymbols`、`lowSecurityBiometric`、`customPassword`。</span><span class="sxs-lookup"><span data-stu-id="2b2aa-221">Possible values are: `deviceDefault`, `required`, `numeric`, `numericComplex`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `customPassword`.</span></span>|
|<span data-ttu-id="2b2aa-222">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="2b2aa-222">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="2b2aa-223">Int32</span><span class="sxs-lookup"><span data-stu-id="2b2aa-223">Int32</span></span>|<span data-ttu-id="2b2aa-224">在需要密码之前不活动的分钟数。</span><span class="sxs-lookup"><span data-stu-id="2b2aa-224">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="2b2aa-225">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="2b2aa-225">passwordExpirationDays</span></span>|<span data-ttu-id="2b2aa-226">Int32</span><span class="sxs-lookup"><span data-stu-id="2b2aa-226">Int32</span></span>|<span data-ttu-id="2b2aa-227">密码过期前的天数。</span><span class="sxs-lookup"><span data-stu-id="2b2aa-227">Number of days before the password expires.</span></span> <span data-ttu-id="2b2aa-228">有效值为 1 至 365。</span><span class="sxs-lookup"><span data-stu-id="2b2aa-228">Valid values 1 to 365</span></span>|
|<span data-ttu-id="2b2aa-229">passwordPreviousPasswordCountToBlock</span><span class="sxs-lookup"><span data-stu-id="2b2aa-229">passwordPreviousPasswordCountToBlock</span></span>|<span data-ttu-id="2b2aa-230">Int32</span><span class="sxs-lookup"><span data-stu-id="2b2aa-230">Int32</span></span>|<span data-ttu-id="2b2aa-231">要阻止的以前密码的数量。</span><span class="sxs-lookup"><span data-stu-id="2b2aa-231">Number of previous passwords to block.</span></span> <span data-ttu-id="2b2aa-232">有效值为 1 至 24</span><span class="sxs-lookup"><span data-stu-id="2b2aa-232">Valid values 1 to 24</span></span>|
|<span data-ttu-id="2b2aa-233">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="2b2aa-233">storageRequireEncryption</span></span>|<span data-ttu-id="2b2aa-234">Boolean</span><span class="sxs-lookup"><span data-stu-id="2b2aa-234">Boolean</span></span>|<span data-ttu-id="2b2aa-235">要求对 Android 设备加密。</span><span class="sxs-lookup"><span data-stu-id="2b2aa-235">Require encryption on Android devices.</span></span>|



## <a name="response"></a><span data-ttu-id="2b2aa-236">响应</span><span class="sxs-lookup"><span data-stu-id="2b2aa-236">Response</span></span>
<span data-ttu-id="2b2aa-237">如果成功，此方法在响应`200 OK`正文中返回响应代码和更新的[androidDeviceOwnerCompliancePolicy](../resources/intune-deviceconfig-androiddeviceownercompliancepolicy.md)对象。</span><span class="sxs-lookup"><span data-stu-id="2b2aa-237">If successful, this method returns a `200 OK` response code and an updated [androidDeviceOwnerCompliancePolicy](../resources/intune-deviceconfig-androiddeviceownercompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2b2aa-238">示例</span><span class="sxs-lookup"><span data-stu-id="2b2aa-238">Example</span></span>

### <a name="request"></a><span data-ttu-id="2b2aa-239">请求</span><span class="sxs-lookup"><span data-stu-id="2b2aa-239">Request</span></span>
<span data-ttu-id="2b2aa-240">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="2b2aa-240">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="2b2aa-241">响应</span><span class="sxs-lookup"><span data-stu-id="2b2aa-241">Response</span></span>
<span data-ttu-id="2b2aa-p121">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="2b2aa-p121">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





