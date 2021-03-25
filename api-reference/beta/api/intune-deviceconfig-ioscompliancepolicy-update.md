---
title: 更新 iosCompliancePolicy
description: 更新 iosCompliancePolicy 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: a90cc72523685efefb0b203f7d8f73b54c4983cd
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51151485"
---
# <a name="update-ioscompliancepolicy"></a><span data-ttu-id="9ec6b-103">更新 iosCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="9ec6b-103">Update iosCompliancePolicy</span></span>

<span data-ttu-id="9ec6b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9ec6b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9ec6b-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="9ec6b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9ec6b-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="9ec6b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9ec6b-107">更新 [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="9ec6b-107">Update the properties of a [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9ec6b-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="9ec6b-108">Prerequisites</span></span>
<span data-ttu-id="9ec6b-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9ec6b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9ec6b-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="9ec6b-111">Permission type</span></span>|<span data-ttu-id="9ec6b-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="9ec6b-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9ec6b-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9ec6b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9ec6b-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9ec6b-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="9ec6b-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9ec6b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9ec6b-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="9ec6b-116">Not supported.</span></span>|
|<span data-ttu-id="9ec6b-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="9ec6b-117">Application</span></span>|<span data-ttu-id="9ec6b-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9ec6b-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="9ec6b-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9ec6b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="9ec6b-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="9ec6b-120">Request headers</span></span>
|<span data-ttu-id="9ec6b-121">标头</span><span class="sxs-lookup"><span data-stu-id="9ec6b-121">Header</span></span>|<span data-ttu-id="9ec6b-122">值</span><span class="sxs-lookup"><span data-stu-id="9ec6b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9ec6b-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="9ec6b-123">Authorization</span></span>|<span data-ttu-id="9ec6b-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="9ec6b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9ec6b-125">接受</span><span class="sxs-lookup"><span data-stu-id="9ec6b-125">Accept</span></span>|<span data-ttu-id="9ec6b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9ec6b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9ec6b-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="9ec6b-127">Request body</span></span>
<span data-ttu-id="9ec6b-128">在请求正文中，提供 [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9ec6b-128">In the request body, supply a JSON representation for the [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) object.</span></span>

<span data-ttu-id="9ec6b-129">下表显示了创建 [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="9ec6b-129">The following table shows the properties that are required when you create the [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md).</span></span>

|<span data-ttu-id="9ec6b-130">属性</span><span class="sxs-lookup"><span data-stu-id="9ec6b-130">Property</span></span>|<span data-ttu-id="9ec6b-131">类型</span><span class="sxs-lookup"><span data-stu-id="9ec6b-131">Type</span></span>|<span data-ttu-id="9ec6b-132">说明</span><span class="sxs-lookup"><span data-stu-id="9ec6b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9ec6b-133">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="9ec6b-133">roleScopeTagIds</span></span>|<span data-ttu-id="9ec6b-134">String collection</span><span class="sxs-lookup"><span data-stu-id="9ec6b-134">String collection</span></span>|<span data-ttu-id="9ec6b-135">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="9ec6b-135">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="9ec6b-136">继承自 [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="9ec6b-136">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="9ec6b-137">id</span><span class="sxs-lookup"><span data-stu-id="9ec6b-137">id</span></span>|<span data-ttu-id="9ec6b-138">String</span><span class="sxs-lookup"><span data-stu-id="9ec6b-138">String</span></span>|<span data-ttu-id="9ec6b-139">实体的键。</span><span class="sxs-lookup"><span data-stu-id="9ec6b-139">Key of the entity.</span></span> <span data-ttu-id="9ec6b-140">继承自 [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="9ec6b-140">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="9ec6b-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="9ec6b-141">createdDateTime</span></span>|<span data-ttu-id="9ec6b-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9ec6b-142">DateTimeOffset</span></span>|<span data-ttu-id="9ec6b-143">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="9ec6b-143">DateTime the object was created.</span></span> <span data-ttu-id="9ec6b-144">继承自 [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="9ec6b-144">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="9ec6b-145">说明</span><span class="sxs-lookup"><span data-stu-id="9ec6b-145">description</span></span>|<span data-ttu-id="9ec6b-146">String</span><span class="sxs-lookup"><span data-stu-id="9ec6b-146">String</span></span>|<span data-ttu-id="9ec6b-147">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="9ec6b-147">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="9ec6b-148">继承自 [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="9ec6b-148">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="9ec6b-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9ec6b-149">lastModifiedDateTime</span></span>|<span data-ttu-id="9ec6b-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9ec6b-150">DateTimeOffset</span></span>|<span data-ttu-id="9ec6b-151">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="9ec6b-151">DateTime the object was last modified.</span></span> <span data-ttu-id="9ec6b-152">继承自 [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="9ec6b-152">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="9ec6b-153">displayName</span><span class="sxs-lookup"><span data-stu-id="9ec6b-153">displayName</span></span>|<span data-ttu-id="9ec6b-154">String</span><span class="sxs-lookup"><span data-stu-id="9ec6b-154">String</span></span>|<span data-ttu-id="9ec6b-155">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="9ec6b-155">Admin provided name of the device configuration.</span></span> <span data-ttu-id="9ec6b-156">继承自 [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="9ec6b-156">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="9ec6b-157">version</span><span class="sxs-lookup"><span data-stu-id="9ec6b-157">version</span></span>|<span data-ttu-id="9ec6b-158">Int32</span><span class="sxs-lookup"><span data-stu-id="9ec6b-158">Int32</span></span>|<span data-ttu-id="9ec6b-159">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="9ec6b-159">Version of the device configuration.</span></span> <span data-ttu-id="9ec6b-160">继承自 [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="9ec6b-160">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="9ec6b-161">passcodeBlockSimple</span><span class="sxs-lookup"><span data-stu-id="9ec6b-161">passcodeBlockSimple</span></span>|<span data-ttu-id="9ec6b-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="9ec6b-162">Boolean</span></span>|<span data-ttu-id="9ec6b-163">指示是否阻止简单密码。</span><span class="sxs-lookup"><span data-stu-id="9ec6b-163">Indicates whether or not to block simple passcodes.</span></span>|
|<span data-ttu-id="9ec6b-164">passcodeExpirationDays</span><span class="sxs-lookup"><span data-stu-id="9ec6b-164">passcodeExpirationDays</span></span>|<span data-ttu-id="9ec6b-165">Int32</span><span class="sxs-lookup"><span data-stu-id="9ec6b-165">Int32</span></span>|<span data-ttu-id="9ec6b-166">密码过期前的天数。</span><span class="sxs-lookup"><span data-stu-id="9ec6b-166">Number of days before the passcode expires.</span></span> <span data-ttu-id="9ec6b-167">有效值为 1 至 65535</span><span class="sxs-lookup"><span data-stu-id="9ec6b-167">Valid values 1 to 65535</span></span>|
|<span data-ttu-id="9ec6b-168">passcodeMinimumLength</span><span class="sxs-lookup"><span data-stu-id="9ec6b-168">passcodeMinimumLength</span></span>|<span data-ttu-id="9ec6b-169">Int32</span><span class="sxs-lookup"><span data-stu-id="9ec6b-169">Int32</span></span>|<span data-ttu-id="9ec6b-170">密码的最小长度。</span><span class="sxs-lookup"><span data-stu-id="9ec6b-170">Minimum length of passcode.</span></span> <span data-ttu-id="9ec6b-171">有效值为 4 至 14</span><span class="sxs-lookup"><span data-stu-id="9ec6b-171">Valid values 4 to 14</span></span>|
|<span data-ttu-id="9ec6b-172">passcodeMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="9ec6b-172">passcodeMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="9ec6b-173">Int32</span><span class="sxs-lookup"><span data-stu-id="9ec6b-173">Int32</span></span>|<span data-ttu-id="9ec6b-174">需要密码之前的不活动分钟数。</span><span class="sxs-lookup"><span data-stu-id="9ec6b-174">Minutes of inactivity before a passcode is required.</span></span>|
|<span data-ttu-id="9ec6b-175">passcodeMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="9ec6b-175">passcodeMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="9ec6b-176">Int32</span><span class="sxs-lookup"><span data-stu-id="9ec6b-176">Int32</span></span>|<span data-ttu-id="9ec6b-177">屏幕超时之前的不活动分钟数。</span><span class="sxs-lookup"><span data-stu-id="9ec6b-177">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="9ec6b-178">passcodePreviousPasscodeBlockCount</span><span class="sxs-lookup"><span data-stu-id="9ec6b-178">passcodePreviousPasscodeBlockCount</span></span>|<span data-ttu-id="9ec6b-179">Int32</span><span class="sxs-lookup"><span data-stu-id="9ec6b-179">Int32</span></span>|<span data-ttu-id="9ec6b-180">要阻止的以前密码的数量。</span><span class="sxs-lookup"><span data-stu-id="9ec6b-180">Number of previous passcodes to block.</span></span> <span data-ttu-id="9ec6b-181">有效值为 1 至 24</span><span class="sxs-lookup"><span data-stu-id="9ec6b-181">Valid values 1 to 24</span></span>|
|<span data-ttu-id="9ec6b-182">passcodeMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="9ec6b-182">passcodeMinimumCharacterSetCount</span></span>|<span data-ttu-id="9ec6b-183">Int32</span><span class="sxs-lookup"><span data-stu-id="9ec6b-183">Int32</span></span>|<span data-ttu-id="9ec6b-184">密码中必需的字符集数。</span><span class="sxs-lookup"><span data-stu-id="9ec6b-184">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="9ec6b-185">passcodeRequiredType</span><span class="sxs-lookup"><span data-stu-id="9ec6b-185">passcodeRequiredType</span></span>|[<span data-ttu-id="9ec6b-186">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="9ec6b-186">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="9ec6b-187">必需的密码类型。</span><span class="sxs-lookup"><span data-stu-id="9ec6b-187">The required passcode type.</span></span> <span data-ttu-id="9ec6b-188">可取值为：`deviceDefault`、`alphanumeric`、`numeric`。</span><span class="sxs-lookup"><span data-stu-id="9ec6b-188">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="9ec6b-189">passcodeRequired</span><span class="sxs-lookup"><span data-stu-id="9ec6b-189">passcodeRequired</span></span>|<span data-ttu-id="9ec6b-190">Boolean</span><span class="sxs-lookup"><span data-stu-id="9ec6b-190">Boolean</span></span>|<span data-ttu-id="9ec6b-191">指示是否需要密码。</span><span class="sxs-lookup"><span data-stu-id="9ec6b-191">Indicates whether or not to require a passcode.</span></span>|
|<span data-ttu-id="9ec6b-192">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="9ec6b-192">osMinimumVersion</span></span>|<span data-ttu-id="9ec6b-193">String</span><span class="sxs-lookup"><span data-stu-id="9ec6b-193">String</span></span>|<span data-ttu-id="9ec6b-194">最低 IOS 版本。</span><span class="sxs-lookup"><span data-stu-id="9ec6b-194">Minimum IOS version.</span></span>|
|<span data-ttu-id="9ec6b-195">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="9ec6b-195">osMaximumVersion</span></span>|<span data-ttu-id="9ec6b-196">String</span><span class="sxs-lookup"><span data-stu-id="9ec6b-196">String</span></span>|<span data-ttu-id="9ec6b-197">最高 IOS 版本。</span><span class="sxs-lookup"><span data-stu-id="9ec6b-197">Maximum IOS version.</span></span>|
|<span data-ttu-id="9ec6b-198">osMinimumBuildVersion</span><span class="sxs-lookup"><span data-stu-id="9ec6b-198">osMinimumBuildVersion</span></span>|<span data-ttu-id="9ec6b-199">String</span><span class="sxs-lookup"><span data-stu-id="9ec6b-199">String</span></span>|<span data-ttu-id="9ec6b-200">最低 IOS 内部版本。</span><span class="sxs-lookup"><span data-stu-id="9ec6b-200">Minimum IOS build version.</span></span>|
|<span data-ttu-id="9ec6b-201">osMaximumBuildVersion</span><span class="sxs-lookup"><span data-stu-id="9ec6b-201">osMaximumBuildVersion</span></span>|<span data-ttu-id="9ec6b-202">String</span><span class="sxs-lookup"><span data-stu-id="9ec6b-202">String</span></span>|<span data-ttu-id="9ec6b-203">最大 IOS 内部版本。</span><span class="sxs-lookup"><span data-stu-id="9ec6b-203">Maximum IOS build version.</span></span>|
|<span data-ttu-id="9ec6b-204">securityBlockJailbrokenDevices</span><span class="sxs-lookup"><span data-stu-id="9ec6b-204">securityBlockJailbrokenDevices</span></span>|<span data-ttu-id="9ec6b-205">Boolean</span><span class="sxs-lookup"><span data-stu-id="9ec6b-205">Boolean</span></span>|<span data-ttu-id="9ec6b-206">设备不得越狱或取得 root 权限。</span><span class="sxs-lookup"><span data-stu-id="9ec6b-206">Devices must not be jailbroken or rooted.</span></span>|
|<span data-ttu-id="9ec6b-207">deviceThreatProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="9ec6b-207">deviceThreatProtectionEnabled</span></span>|<span data-ttu-id="9ec6b-208">Boolean</span><span class="sxs-lookup"><span data-stu-id="9ec6b-208">Boolean</span></span>|<span data-ttu-id="9ec6b-209">要求设备已启用设备威胁防护。</span><span class="sxs-lookup"><span data-stu-id="9ec6b-209">Require that devices have enabled device threat protection .</span></span>|
|<span data-ttu-id="9ec6b-210">deviceThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="9ec6b-210">deviceThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="9ec6b-211">deviceThreatProtectionLevel</span><span class="sxs-lookup"><span data-stu-id="9ec6b-211">deviceThreatProtectionLevel</span></span>](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|<span data-ttu-id="9ec6b-212">要求移动威胁防护最低风险级别来报告不符合情况。</span><span class="sxs-lookup"><span data-stu-id="9ec6b-212">Require Mobile Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="9ec6b-213">可取值为：`unavailable`、`secured`、`low`、`medium`、`high`、`notSet`。</span><span class="sxs-lookup"><span data-stu-id="9ec6b-213">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="9ec6b-214">advancedThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="9ec6b-214">advancedThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="9ec6b-215">deviceThreatProtectionLevel</span><span class="sxs-lookup"><span data-stu-id="9ec6b-215">deviceThreatProtectionLevel</span></span>](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|<span data-ttu-id="9ec6b-216">MDATP 要求移动威胁防护最低风险级别来报告不相容情况。</span><span class="sxs-lookup"><span data-stu-id="9ec6b-216">MDATP Require Mobile Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="9ec6b-217">可取值为：`unavailable`、`secured`、`low`、`medium`、`high`、`notSet`。</span><span class="sxs-lookup"><span data-stu-id="9ec6b-217">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="9ec6b-218">managedEmailProfileRequired</span><span class="sxs-lookup"><span data-stu-id="9ec6b-218">managedEmailProfileRequired</span></span>|<span data-ttu-id="9ec6b-219">Boolean</span><span class="sxs-lookup"><span data-stu-id="9ec6b-219">Boolean</span></span>|<span data-ttu-id="9ec6b-220">指示是否需要托管电子邮件配置文件。</span><span class="sxs-lookup"><span data-stu-id="9ec6b-220">Indicates whether or not to require a managed email profile.</span></span>|
|<span data-ttu-id="9ec6b-221">restrictedApps</span><span class="sxs-lookup"><span data-stu-id="9ec6b-221">restrictedApps</span></span>|<span data-ttu-id="9ec6b-222">[appListItem](../resources/intune-deviceconfig-applistitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="9ec6b-222">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="9ec6b-223">要求设备未安装指定的应用。</span><span class="sxs-lookup"><span data-stu-id="9ec6b-223">Require the device to not have the specified apps installed.</span></span> <span data-ttu-id="9ec6b-224">此集合最多可包含 100 个元素。</span><span class="sxs-lookup"><span data-stu-id="9ec6b-224">This collection can contain a maximum of 100 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="9ec6b-225">响应</span><span class="sxs-lookup"><span data-stu-id="9ec6b-225">Response</span></span>
<span data-ttu-id="9ec6b-226">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和更新的 [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="9ec6b-226">If successful, this method returns a `200 OK` response code and an updated [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9ec6b-227">示例</span><span class="sxs-lookup"><span data-stu-id="9ec6b-227">Example</span></span>

### <a name="request"></a><span data-ttu-id="9ec6b-228">请求</span><span class="sxs-lookup"><span data-stu-id="9ec6b-228">Request</span></span>
<span data-ttu-id="9ec6b-229">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="9ec6b-229">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
Content-type: application/json
Content-length: 1304

{
  "@odata.type": "#microsoft.graph.iosCompliancePolicy",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "passcodeBlockSimple": true,
  "passcodeExpirationDays": 6,
  "passcodeMinimumLength": 5,
  "passcodeMinutesOfInactivityBeforeLock": 5,
  "passcodeMinutesOfInactivityBeforeScreenTimeout": 14,
  "passcodePreviousPasscodeBlockCount": 2,
  "passcodeMinimumCharacterSetCount": 0,
  "passcodeRequiredType": "alphanumeric",
  "passcodeRequired": true,
  "osMinimumVersion": "Os Minimum Version value",
  "osMaximumVersion": "Os Maximum Version value",
  "osMinimumBuildVersion": "Os Minimum Build Version value",
  "osMaximumBuildVersion": "Os Maximum Build Version value",
  "securityBlockJailbrokenDevices": true,
  "deviceThreatProtectionEnabled": true,
  "deviceThreatProtectionRequiredSecurityLevel": "secured",
  "advancedThreatProtectionRequiredSecurityLevel": "secured",
  "managedEmailProfileRequired": true,
  "restrictedApps": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="9ec6b-230">响应</span><span class="sxs-lookup"><span data-stu-id="9ec6b-230">Response</span></span>
<span data-ttu-id="9ec6b-p116">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="9ec6b-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1476

{
  "@odata.type": "#microsoft.graph.iosCompliancePolicy",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "id": "4f501351-1351-4f50-5113-504f5113504f",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "version": 7,
  "passcodeBlockSimple": true,
  "passcodeExpirationDays": 6,
  "passcodeMinimumLength": 5,
  "passcodeMinutesOfInactivityBeforeLock": 5,
  "passcodeMinutesOfInactivityBeforeScreenTimeout": 14,
  "passcodePreviousPasscodeBlockCount": 2,
  "passcodeMinimumCharacterSetCount": 0,
  "passcodeRequiredType": "alphanumeric",
  "passcodeRequired": true,
  "osMinimumVersion": "Os Minimum Version value",
  "osMaximumVersion": "Os Maximum Version value",
  "osMinimumBuildVersion": "Os Minimum Build Version value",
  "osMaximumBuildVersion": "Os Maximum Build Version value",
  "securityBlockJailbrokenDevices": true,
  "deviceThreatProtectionEnabled": true,
  "deviceThreatProtectionRequiredSecurityLevel": "secured",
  "advancedThreatProtectionRequiredSecurityLevel": "secured",
  "managedEmailProfileRequired": true,
  "restrictedApps": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ]
}
```




