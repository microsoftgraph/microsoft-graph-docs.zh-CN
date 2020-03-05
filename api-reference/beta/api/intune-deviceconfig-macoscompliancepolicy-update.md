---
title: 更新 macOSCompliancePolicy
description: 更新 macOSCompliancePolicy 对象的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 5095f6750e347f3d2ff83cb72878c175098a93c3
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42442444"
---
# <a name="update-macoscompliancepolicy"></a><span data-ttu-id="da7af-103">更新 macOSCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="da7af-103">Update macOSCompliancePolicy</span></span>

<span data-ttu-id="da7af-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="da7af-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="da7af-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="da7af-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="da7af-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="da7af-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="da7af-107">更新 [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="da7af-107">Update the properties of a [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="da7af-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="da7af-108">Prerequisites</span></span>
<span data-ttu-id="da7af-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="da7af-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="da7af-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="da7af-111">Permission type</span></span>|<span data-ttu-id="da7af-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="da7af-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="da7af-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="da7af-113">Delegated (work or school account)</span></span>|<span data-ttu-id="da7af-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="da7af-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="da7af-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="da7af-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="da7af-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="da7af-116">Not supported.</span></span>|
|<span data-ttu-id="da7af-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="da7af-117">Application</span></span>|<span data-ttu-id="da7af-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="da7af-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="da7af-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="da7af-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="da7af-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="da7af-120">Request headers</span></span>
|<span data-ttu-id="da7af-121">标头</span><span class="sxs-lookup"><span data-stu-id="da7af-121">Header</span></span>|<span data-ttu-id="da7af-122">值</span><span class="sxs-lookup"><span data-stu-id="da7af-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="da7af-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="da7af-123">Authorization</span></span>|<span data-ttu-id="da7af-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="da7af-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="da7af-125">接受</span><span class="sxs-lookup"><span data-stu-id="da7af-125">Accept</span></span>|<span data-ttu-id="da7af-126">application/json</span><span class="sxs-lookup"><span data-stu-id="da7af-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="da7af-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="da7af-127">Request body</span></span>
<span data-ttu-id="da7af-128">在请求正文中，提供 [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="da7af-128">In the request body, supply a JSON representation for the [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) object.</span></span>

<span data-ttu-id="da7af-129">下表显示创建 [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="da7af-129">The following table shows the properties that are required when you create the [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md).</span></span>

|<span data-ttu-id="da7af-130">属性</span><span class="sxs-lookup"><span data-stu-id="da7af-130">Property</span></span>|<span data-ttu-id="da7af-131">类型</span><span class="sxs-lookup"><span data-stu-id="da7af-131">Type</span></span>|<span data-ttu-id="da7af-132">说明</span><span class="sxs-lookup"><span data-stu-id="da7af-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="da7af-133">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="da7af-133">roleScopeTagIds</span></span>|<span data-ttu-id="da7af-134">String 集合</span><span class="sxs-lookup"><span data-stu-id="da7af-134">String collection</span></span>|<span data-ttu-id="da7af-135">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="da7af-135">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="da7af-136">继承自 [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="da7af-136">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="da7af-137">id</span><span class="sxs-lookup"><span data-stu-id="da7af-137">id</span></span>|<span data-ttu-id="da7af-138">字符串</span><span class="sxs-lookup"><span data-stu-id="da7af-138">String</span></span>|<span data-ttu-id="da7af-139">实体的键。</span><span class="sxs-lookup"><span data-stu-id="da7af-139">Key of the entity.</span></span> <span data-ttu-id="da7af-140">继承自 [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="da7af-140">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="da7af-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="da7af-141">createdDateTime</span></span>|<span data-ttu-id="da7af-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="da7af-142">DateTimeOffset</span></span>|<span data-ttu-id="da7af-143">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="da7af-143">DateTime the object was created.</span></span> <span data-ttu-id="da7af-144">继承自 [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="da7af-144">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="da7af-145">说明</span><span class="sxs-lookup"><span data-stu-id="da7af-145">description</span></span>|<span data-ttu-id="da7af-146">String</span><span class="sxs-lookup"><span data-stu-id="da7af-146">String</span></span>|<span data-ttu-id="da7af-147">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="da7af-147">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="da7af-148">继承自 [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="da7af-148">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="da7af-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="da7af-149">lastModifiedDateTime</span></span>|<span data-ttu-id="da7af-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="da7af-150">DateTimeOffset</span></span>|<span data-ttu-id="da7af-151">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="da7af-151">DateTime the object was last modified.</span></span> <span data-ttu-id="da7af-152">继承自 [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="da7af-152">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="da7af-153">displayName</span><span class="sxs-lookup"><span data-stu-id="da7af-153">displayName</span></span>|<span data-ttu-id="da7af-154">String</span><span class="sxs-lookup"><span data-stu-id="da7af-154">String</span></span>|<span data-ttu-id="da7af-155">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="da7af-155">Admin provided name of the device configuration.</span></span> <span data-ttu-id="da7af-156">继承自 [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="da7af-156">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="da7af-157">version</span><span class="sxs-lookup"><span data-stu-id="da7af-157">version</span></span>|<span data-ttu-id="da7af-158">Int32</span><span class="sxs-lookup"><span data-stu-id="da7af-158">Int32</span></span>|<span data-ttu-id="da7af-159">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="da7af-159">Version of the device configuration.</span></span> <span data-ttu-id="da7af-160">继承自 [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="da7af-160">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="da7af-161">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="da7af-161">passwordRequired</span></span>|<span data-ttu-id="da7af-162">布尔</span><span class="sxs-lookup"><span data-stu-id="da7af-162">Boolean</span></span>|<span data-ttu-id="da7af-163">是否需要密码。</span><span class="sxs-lookup"><span data-stu-id="da7af-163">Whether or not to require a password.</span></span>|
|<span data-ttu-id="da7af-164">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="da7af-164">passwordBlockSimple</span></span>|<span data-ttu-id="da7af-165">布尔</span><span class="sxs-lookup"><span data-stu-id="da7af-165">Boolean</span></span>|<span data-ttu-id="da7af-166">指示是否阻止简单密码。</span><span class="sxs-lookup"><span data-stu-id="da7af-166">Indicates whether or not to block simple passwords.</span></span>|
|<span data-ttu-id="da7af-167">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="da7af-167">passwordExpirationDays</span></span>|<span data-ttu-id="da7af-168">Int32</span><span class="sxs-lookup"><span data-stu-id="da7af-168">Int32</span></span>|<span data-ttu-id="da7af-169">密码过期前的天数。</span><span class="sxs-lookup"><span data-stu-id="da7af-169">Number of days before the password expires.</span></span> <span data-ttu-id="da7af-170">有效值为 1 至 65535</span><span class="sxs-lookup"><span data-stu-id="da7af-170">Valid values 1 to 65535</span></span>|
|<span data-ttu-id="da7af-171">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="da7af-171">passwordMinimumLength</span></span>|<span data-ttu-id="da7af-172">Int32</span><span class="sxs-lookup"><span data-stu-id="da7af-172">Int32</span></span>|<span data-ttu-id="da7af-173">密码的最小长度。</span><span class="sxs-lookup"><span data-stu-id="da7af-173">Minimum length of password.</span></span> <span data-ttu-id="da7af-174">有效值为 4 至 14</span><span class="sxs-lookup"><span data-stu-id="da7af-174">Valid values 4 to 14</span></span>|
|<span data-ttu-id="da7af-175">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="da7af-175">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="da7af-176">Int32</span><span class="sxs-lookup"><span data-stu-id="da7af-176">Int32</span></span>|<span data-ttu-id="da7af-177">在需要密码之前不活动的分钟数。</span><span class="sxs-lookup"><span data-stu-id="da7af-177">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="da7af-178">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="da7af-178">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="da7af-179">Int32</span><span class="sxs-lookup"><span data-stu-id="da7af-179">Int32</span></span>|<span data-ttu-id="da7af-180">要阻止的以前密码的数量。</span><span class="sxs-lookup"><span data-stu-id="da7af-180">Number of previous passwords to block.</span></span> <span data-ttu-id="da7af-181">有效值为 1 至 24</span><span class="sxs-lookup"><span data-stu-id="da7af-181">Valid values 1 to 24</span></span>|
|<span data-ttu-id="da7af-182">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="da7af-182">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="da7af-183">Int32</span><span class="sxs-lookup"><span data-stu-id="da7af-183">Int32</span></span>|<span data-ttu-id="da7af-184">密码中必需的字符集数。</span><span class="sxs-lookup"><span data-stu-id="da7af-184">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="da7af-185">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="da7af-185">passwordRequiredType</span></span>|[<span data-ttu-id="da7af-186">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="da7af-186">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="da7af-187">必需的密码类型。</span><span class="sxs-lookup"><span data-stu-id="da7af-187">The required password type.</span></span> <span data-ttu-id="da7af-188">可取值为：`deviceDefault`、`alphanumeric`、`numeric`。</span><span class="sxs-lookup"><span data-stu-id="da7af-188">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="da7af-189">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="da7af-189">osMinimumVersion</span></span>|<span data-ttu-id="da7af-190">String</span><span class="sxs-lookup"><span data-stu-id="da7af-190">String</span></span>|<span data-ttu-id="da7af-191">最低 MacOS 版本。</span><span class="sxs-lookup"><span data-stu-id="da7af-191">Minimum MacOS version.</span></span>|
|<span data-ttu-id="da7af-192">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="da7af-192">osMaximumVersion</span></span>|<span data-ttu-id="da7af-193">String</span><span class="sxs-lookup"><span data-stu-id="da7af-193">String</span></span>|<span data-ttu-id="da7af-194">最大 MacOS 版本。</span><span class="sxs-lookup"><span data-stu-id="da7af-194">Maximum MacOS version.</span></span>|
|<span data-ttu-id="da7af-195">osMinimumBuildVersion</span><span class="sxs-lookup"><span data-stu-id="da7af-195">osMinimumBuildVersion</span></span>|<span data-ttu-id="da7af-196">String</span><span class="sxs-lookup"><span data-stu-id="da7af-196">String</span></span>|<span data-ttu-id="da7af-197">最低 MacOS 内部版本。</span><span class="sxs-lookup"><span data-stu-id="da7af-197">Minimum MacOS build version.</span></span>|
|<span data-ttu-id="da7af-198">osMaximumBuildVersion</span><span class="sxs-lookup"><span data-stu-id="da7af-198">osMaximumBuildVersion</span></span>|<span data-ttu-id="da7af-199">String</span><span class="sxs-lookup"><span data-stu-id="da7af-199">String</span></span>|<span data-ttu-id="da7af-200">最大 MacOS 内部版本。</span><span class="sxs-lookup"><span data-stu-id="da7af-200">Maximum MacOS build version.</span></span>|
|<span data-ttu-id="da7af-201">systemIntegrityProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="da7af-201">systemIntegrityProtectionEnabled</span></span>|<span data-ttu-id="da7af-202">Boolean</span><span class="sxs-lookup"><span data-stu-id="da7af-202">Boolean</span></span>|<span data-ttu-id="da7af-203">要求设备已启用系统完整性保护。</span><span class="sxs-lookup"><span data-stu-id="da7af-203">Require that devices have enabled system integrity protection.</span></span>|
|<span data-ttu-id="da7af-204">deviceThreatProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="da7af-204">deviceThreatProtectionEnabled</span></span>|<span data-ttu-id="da7af-205">布尔</span><span class="sxs-lookup"><span data-stu-id="da7af-205">Boolean</span></span>|<span data-ttu-id="da7af-206">要求设备已启用设备威胁防护。</span><span class="sxs-lookup"><span data-stu-id="da7af-206">Require that devices have enabled device threat protection.</span></span>|
|<span data-ttu-id="da7af-207">deviceThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="da7af-207">deviceThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="da7af-208">deviceThreatProtectionLevel</span><span class="sxs-lookup"><span data-stu-id="da7af-208">deviceThreatProtectionLevel</span></span>](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|<span data-ttu-id="da7af-209">要求移动威胁防护最低风险级别来报告不符合情况。</span><span class="sxs-lookup"><span data-stu-id="da7af-209">Require Mobile Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="da7af-210">可取值为：`unavailable`、`secured`、`low`、`medium`、`high`、`notSet`。</span><span class="sxs-lookup"><span data-stu-id="da7af-210">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="da7af-211">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="da7af-211">storageRequireEncryption</span></span>|<span data-ttu-id="da7af-212">Boolean</span><span class="sxs-lookup"><span data-stu-id="da7af-212">Boolean</span></span>|<span data-ttu-id="da7af-213">要求对 Mac OS 设备加密。</span><span class="sxs-lookup"><span data-stu-id="da7af-213">Require encryption on Mac OS devices.</span></span>|
|<span data-ttu-id="da7af-214">gatekeeperAllowedAppSource</span><span class="sxs-lookup"><span data-stu-id="da7af-214">gatekeeperAllowedAppSource</span></span>|[<span data-ttu-id="da7af-215">macOSGatekeeperAppSources</span><span class="sxs-lookup"><span data-stu-id="da7af-215">macOSGatekeeperAppSources</span></span>](../resources/intune-deviceconfig-macosgatekeeperappsources.md)|<span data-ttu-id="da7af-216">确定可以从 macOS 设备上运行哪些下载位置应用程序的系统和隐私设置。</span><span class="sxs-lookup"><span data-stu-id="da7af-216">System and Privacy setting that determines which download locations apps can be run from on a macOS device.</span></span> <span data-ttu-id="da7af-217">可取值为：`notConfigured`、`macAppStore`、`macAppStoreAndIdentifiedDevelopers`、`anywhere`。</span><span class="sxs-lookup"><span data-stu-id="da7af-217">Possible values are: `notConfigured`, `macAppStore`, `macAppStoreAndIdentifiedDevelopers`, `anywhere`.</span></span>|
|<span data-ttu-id="da7af-218">firewallEnabled</span><span class="sxs-lookup"><span data-stu-id="da7af-218">firewallEnabled</span></span>|<span data-ttu-id="da7af-219">布尔</span><span class="sxs-lookup"><span data-stu-id="da7af-219">Boolean</span></span>|<span data-ttu-id="da7af-220">是否应启用防火墙。</span><span class="sxs-lookup"><span data-stu-id="da7af-220">Whether the firewall should be enabled or not.</span></span>|
|<span data-ttu-id="da7af-221">firewallBlockAllIncoming</span><span class="sxs-lookup"><span data-stu-id="da7af-221">firewallBlockAllIncoming</span></span>|<span data-ttu-id="da7af-222">布尔</span><span class="sxs-lookup"><span data-stu-id="da7af-222">Boolean</span></span>|<span data-ttu-id="da7af-223">对应于 "阻止所有传入连接" 选项。</span><span class="sxs-lookup"><span data-stu-id="da7af-223">Corresponds to the “Block all incoming connections” option.</span></span>|
|<span data-ttu-id="da7af-224">firewallEnableStealthMode</span><span class="sxs-lookup"><span data-stu-id="da7af-224">firewallEnableStealthMode</span></span>|<span data-ttu-id="da7af-225">布尔</span><span class="sxs-lookup"><span data-stu-id="da7af-225">Boolean</span></span>|<span data-ttu-id="da7af-226">对应于 "启用隐形模式"。</span><span class="sxs-lookup"><span data-stu-id="da7af-226">Corresponds to “Enable stealth mode.”</span></span>|



## <a name="response"></a><span data-ttu-id="da7af-227">响应</span><span class="sxs-lookup"><span data-stu-id="da7af-227">Response</span></span>
<span data-ttu-id="da7af-228">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和更新的 [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="da7af-228">If successful, this method returns a `200 OK` response code and an updated [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="da7af-229">示例</span><span class="sxs-lookup"><span data-stu-id="da7af-229">Example</span></span>

### <a name="request"></a><span data-ttu-id="da7af-230">请求</span><span class="sxs-lookup"><span data-stu-id="da7af-230">Request</span></span>
<span data-ttu-id="da7af-231">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="da7af-231">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
Content-type: application/json
Content-length: 1083

{
  "@odata.type": "#microsoft.graph.macOSCompliancePolicy",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
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
  "osMinimumBuildVersion": "Os Minimum Build Version value",
  "osMaximumBuildVersion": "Os Maximum Build Version value",
  "systemIntegrityProtectionEnabled": true,
  "deviceThreatProtectionEnabled": true,
  "deviceThreatProtectionRequiredSecurityLevel": "secured",
  "storageRequireEncryption": true,
  "gatekeeperAllowedAppSource": "macAppStore",
  "firewallEnabled": true,
  "firewallBlockAllIncoming": true,
  "firewallEnableStealthMode": true
}
```

### <a name="response"></a><span data-ttu-id="da7af-232">响应</span><span class="sxs-lookup"><span data-stu-id="da7af-232">Response</span></span>
<span data-ttu-id="da7af-p115">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="da7af-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1255

{
  "@odata.type": "#microsoft.graph.macOSCompliancePolicy",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
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
  "osMinimumBuildVersion": "Os Minimum Build Version value",
  "osMaximumBuildVersion": "Os Maximum Build Version value",
  "systemIntegrityProtectionEnabled": true,
  "deviceThreatProtectionEnabled": true,
  "deviceThreatProtectionRequiredSecurityLevel": "secured",
  "storageRequireEncryption": true,
  "gatekeeperAllowedAppSource": "macAppStore",
  "firewallEnabled": true,
  "firewallBlockAllIncoming": true,
  "firewallEnableStealthMode": true
}
```





