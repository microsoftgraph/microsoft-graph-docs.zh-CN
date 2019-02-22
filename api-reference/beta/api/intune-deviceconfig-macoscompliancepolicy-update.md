---
title: 更新 macOSCompliancePolicy
description: 更新 macOSCompliancePolicy 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 44d6f0e4aaddbed4ab1b4820916949397d271fee
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30141893"
---
# <a name="update-macoscompliancepolicy"></a><span data-ttu-id="4933a-103">更新 macOSCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="4933a-103">Update macOSCompliancePolicy</span></span>

> <span data-ttu-id="4933a-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="4933a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4933a-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="4933a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4933a-106">更新 [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="4933a-106">Update the properties of a [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4933a-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="4933a-107">Prerequisites</span></span>
<span data-ttu-id="4933a-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="4933a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="4933a-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="4933a-110">Permission type</span></span>|<span data-ttu-id="4933a-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="4933a-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4933a-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4933a-112">Delegated (work or school account)</span></span>|<span data-ttu-id="4933a-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4933a-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="4933a-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4933a-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4933a-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="4933a-115">Not supported.</span></span>|
|<span data-ttu-id="4933a-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="4933a-116">Application</span></span>|<span data-ttu-id="4933a-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="4933a-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4933a-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4933a-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="4933a-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="4933a-119">Request headers</span></span>
|<span data-ttu-id="4933a-120">标头</span><span class="sxs-lookup"><span data-stu-id="4933a-120">Header</span></span>|<span data-ttu-id="4933a-121">值</span><span class="sxs-lookup"><span data-stu-id="4933a-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4933a-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="4933a-122">Authorization</span></span>|<span data-ttu-id="4933a-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="4933a-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4933a-124">Accept</span><span class="sxs-lookup"><span data-stu-id="4933a-124">Accept</span></span>|<span data-ttu-id="4933a-125">application/json</span><span class="sxs-lookup"><span data-stu-id="4933a-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4933a-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="4933a-126">Request body</span></span>
<span data-ttu-id="4933a-127">在请求正文中，提供 [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4933a-127">In the request body, supply a JSON representation for the [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) object.</span></span>

<span data-ttu-id="4933a-128">下表显示创建 [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="4933a-128">The following table shows the properties that are required when you create the [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md).</span></span>

|<span data-ttu-id="4933a-129">属性</span><span class="sxs-lookup"><span data-stu-id="4933a-129">Property</span></span>|<span data-ttu-id="4933a-130">类型</span><span class="sxs-lookup"><span data-stu-id="4933a-130">Type</span></span>|<span data-ttu-id="4933a-131">说明</span><span class="sxs-lookup"><span data-stu-id="4933a-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4933a-132">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="4933a-132">roleScopeTagIds</span></span>|<span data-ttu-id="4933a-133">String collection</span><span class="sxs-lookup"><span data-stu-id="4933a-133">String collection</span></span>|<span data-ttu-id="4933a-134">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="4933a-134">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="4933a-135">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="4933a-135">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="4933a-136">id</span><span class="sxs-lookup"><span data-stu-id="4933a-136">id</span></span>|<span data-ttu-id="4933a-137">字串符号</span><span class="sxs-lookup"><span data-stu-id="4933a-137">String</span></span>|<span data-ttu-id="4933a-138">实体的键。</span><span class="sxs-lookup"><span data-stu-id="4933a-138">Key of the entity.</span></span> <span data-ttu-id="4933a-139">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="4933a-139">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="4933a-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="4933a-140">createdDateTime</span></span>|<span data-ttu-id="4933a-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4933a-141">DateTimeOffset</span></span>|<span data-ttu-id="4933a-142">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="4933a-142">DateTime the object was created.</span></span> <span data-ttu-id="4933a-143">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="4933a-143">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="4933a-144">description</span><span class="sxs-lookup"><span data-stu-id="4933a-144">description</span></span>|<span data-ttu-id="4933a-145">字符串</span><span class="sxs-lookup"><span data-stu-id="4933a-145">String</span></span>|<span data-ttu-id="4933a-146">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="4933a-146">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="4933a-147">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="4933a-147">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="4933a-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4933a-148">lastModifiedDateTime</span></span>|<span data-ttu-id="4933a-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4933a-149">DateTimeOffset</span></span>|<span data-ttu-id="4933a-150">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="4933a-150">DateTime the object was last modified.</span></span> <span data-ttu-id="4933a-151">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="4933a-151">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="4933a-152">displayName</span><span class="sxs-lookup"><span data-stu-id="4933a-152">displayName</span></span>|<span data-ttu-id="4933a-153">String</span><span class="sxs-lookup"><span data-stu-id="4933a-153">String</span></span>|<span data-ttu-id="4933a-154">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="4933a-154">Admin provided name of the device configuration.</span></span> <span data-ttu-id="4933a-155">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="4933a-155">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="4933a-156">version</span><span class="sxs-lookup"><span data-stu-id="4933a-156">version</span></span>|<span data-ttu-id="4933a-157">Int32</span><span class="sxs-lookup"><span data-stu-id="4933a-157">Int32</span></span>|<span data-ttu-id="4933a-158">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="4933a-158">Version of the device configuration.</span></span> <span data-ttu-id="4933a-159">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="4933a-159">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="4933a-160">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="4933a-160">passwordRequired</span></span>|<span data-ttu-id="4933a-161">布尔</span><span class="sxs-lookup"><span data-stu-id="4933a-161">Boolean</span></span>|<span data-ttu-id="4933a-162">是否需要密码。</span><span class="sxs-lookup"><span data-stu-id="4933a-162">Whether or not to require a password.</span></span>|
|<span data-ttu-id="4933a-163">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="4933a-163">passwordBlockSimple</span></span>|<span data-ttu-id="4933a-164">布尔</span><span class="sxs-lookup"><span data-stu-id="4933a-164">Boolean</span></span>|<span data-ttu-id="4933a-165">指示是否阻止简单密码。</span><span class="sxs-lookup"><span data-stu-id="4933a-165">Indicates whether or not to block simple passwords.</span></span>|
|<span data-ttu-id="4933a-166">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="4933a-166">passwordExpirationDays</span></span>|<span data-ttu-id="4933a-167">Int32</span><span class="sxs-lookup"><span data-stu-id="4933a-167">Int32</span></span>|<span data-ttu-id="4933a-168">密码过期前的天数。</span><span class="sxs-lookup"><span data-stu-id="4933a-168">Number of days before the password expires.</span></span> <span data-ttu-id="4933a-169">有效值为 1 至 65535</span><span class="sxs-lookup"><span data-stu-id="4933a-169">Valid values 1 to 65535</span></span>|
|<span data-ttu-id="4933a-170">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="4933a-170">passwordMinimumLength</span></span>|<span data-ttu-id="4933a-171">Int32</span><span class="sxs-lookup"><span data-stu-id="4933a-171">Int32</span></span>|<span data-ttu-id="4933a-172">密码的最小长度。</span><span class="sxs-lookup"><span data-stu-id="4933a-172">Minimum length of password.</span></span> <span data-ttu-id="4933a-173">有效值为 4 至 14</span><span class="sxs-lookup"><span data-stu-id="4933a-173">Valid values 4 to 14</span></span>|
|<span data-ttu-id="4933a-174">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="4933a-174">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="4933a-175">Int32</span><span class="sxs-lookup"><span data-stu-id="4933a-175">Int32</span></span>|<span data-ttu-id="4933a-176">在需要密码之前不活动的分钟数。</span><span class="sxs-lookup"><span data-stu-id="4933a-176">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="4933a-177">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="4933a-177">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="4933a-178">Int32</span><span class="sxs-lookup"><span data-stu-id="4933a-178">Int32</span></span>|<span data-ttu-id="4933a-179">要阻止的以前密码的数量。</span><span class="sxs-lookup"><span data-stu-id="4933a-179">Number of previous passwords to block.</span></span> <span data-ttu-id="4933a-180">有效值为 1 至 24</span><span class="sxs-lookup"><span data-stu-id="4933a-180">Valid values 1 to 24</span></span>|
|<span data-ttu-id="4933a-181">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="4933a-181">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="4933a-182">Int32</span><span class="sxs-lookup"><span data-stu-id="4933a-182">Int32</span></span>|<span data-ttu-id="4933a-183">密码中必需的字符集数。</span><span class="sxs-lookup"><span data-stu-id="4933a-183">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="4933a-184">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="4933a-184">passwordRequiredType</span></span>|[<span data-ttu-id="4933a-185">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="4933a-185">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="4933a-186">必需的密码类型。</span><span class="sxs-lookup"><span data-stu-id="4933a-186">The required password type.</span></span> <span data-ttu-id="4933a-187">可取值为：`deviceDefault`、`alphanumeric`、`numeric`。</span><span class="sxs-lookup"><span data-stu-id="4933a-187">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="4933a-188">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="4933a-188">osMinimumVersion</span></span>|<span data-ttu-id="4933a-189">String</span><span class="sxs-lookup"><span data-stu-id="4933a-189">String</span></span>|<span data-ttu-id="4933a-190">最低 MacOS 版本。</span><span class="sxs-lookup"><span data-stu-id="4933a-190">Minimum MacOS version.</span></span>|
|<span data-ttu-id="4933a-191">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="4933a-191">osMaximumVersion</span></span>|<span data-ttu-id="4933a-192">String</span><span class="sxs-lookup"><span data-stu-id="4933a-192">String</span></span>|<span data-ttu-id="4933a-193">最大 MacOS 版本。</span><span class="sxs-lookup"><span data-stu-id="4933a-193">Maximum MacOS version.</span></span>|
|<span data-ttu-id="4933a-194">osMinimumBuildVersion</span><span class="sxs-lookup"><span data-stu-id="4933a-194">osMinimumBuildVersion</span></span>|<span data-ttu-id="4933a-195">字符串</span><span class="sxs-lookup"><span data-stu-id="4933a-195">String</span></span>|<span data-ttu-id="4933a-196">最低 MacOS 内部版本。</span><span class="sxs-lookup"><span data-stu-id="4933a-196">Minimum MacOS build version.</span></span>|
|<span data-ttu-id="4933a-197">osMaximumBuildVersion</span><span class="sxs-lookup"><span data-stu-id="4933a-197">osMaximumBuildVersion</span></span>|<span data-ttu-id="4933a-198">字符串</span><span class="sxs-lookup"><span data-stu-id="4933a-198">String</span></span>|<span data-ttu-id="4933a-199">最大 MacOS 内部版本。</span><span class="sxs-lookup"><span data-stu-id="4933a-199">Maximum MacOS build version.</span></span>|
|<span data-ttu-id="4933a-200">systemIntegrityProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="4933a-200">systemIntegrityProtectionEnabled</span></span>|<span data-ttu-id="4933a-201">Boolean</span><span class="sxs-lookup"><span data-stu-id="4933a-201">Boolean</span></span>|<span data-ttu-id="4933a-202">要求设备已启用系统完整性保护。</span><span class="sxs-lookup"><span data-stu-id="4933a-202">Require that devices have enabled system integrity protection.</span></span>|
|<span data-ttu-id="4933a-203">deviceThreatProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="4933a-203">deviceThreatProtectionEnabled</span></span>|<span data-ttu-id="4933a-204">Boolean</span><span class="sxs-lookup"><span data-stu-id="4933a-204">Boolean</span></span>|<span data-ttu-id="4933a-205">要求设备已启用设备威胁防护。</span><span class="sxs-lookup"><span data-stu-id="4933a-205">Require that devices have enabled device threat protection.</span></span>|
|<span data-ttu-id="4933a-206">deviceThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="4933a-206">deviceThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="4933a-207">deviceThreatProtectionLevel</span><span class="sxs-lookup"><span data-stu-id="4933a-207">deviceThreatProtectionLevel</span></span>](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|<span data-ttu-id="4933a-208">要求移动威胁防护最低风险级别来报告不符合情况。</span><span class="sxs-lookup"><span data-stu-id="4933a-208">Require Mobile Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="4933a-209">可取值为：`unavailable`、`secured`、`low`、`medium`、`high`、`notSet`。</span><span class="sxs-lookup"><span data-stu-id="4933a-209">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="4933a-210">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="4933a-210">storageRequireEncryption</span></span>|<span data-ttu-id="4933a-211">布尔</span><span class="sxs-lookup"><span data-stu-id="4933a-211">Boolean</span></span>|<span data-ttu-id="4933a-212">要求对 Mac OS 设备加密。</span><span class="sxs-lookup"><span data-stu-id="4933a-212">Require encryption on Mac OS devices.</span></span>|
|<span data-ttu-id="4933a-213">gatekeeperAllowedAppSource</span><span class="sxs-lookup"><span data-stu-id="4933a-213">gatekeeperAllowedAppSource</span></span>|[<span data-ttu-id="4933a-214">macOSGatekeeperAppSources</span><span class="sxs-lookup"><span data-stu-id="4933a-214">macOSGatekeeperAppSources</span></span>](../resources/intune-deviceconfig-macosgatekeeperappsources.md)|<span data-ttu-id="4933a-215">确定可以从 macOS 设备上运行哪些下载位置应用程序的系统和隐私设置。</span><span class="sxs-lookup"><span data-stu-id="4933a-215">System and Privacy setting that determines which download locations apps can be run from on a macOS device.</span></span> <span data-ttu-id="4933a-216">可取值为：`notConfigured`、`macAppStore`、`macAppStoreAndIdentifiedDevelopers`、`anywhere`。</span><span class="sxs-lookup"><span data-stu-id="4933a-216">Possible values are: `notConfigured`, `macAppStore`, `macAppStoreAndIdentifiedDevelopers`, `anywhere`.</span></span>|
|<span data-ttu-id="4933a-217">firewallEnabled</span><span class="sxs-lookup"><span data-stu-id="4933a-217">firewallEnabled</span></span>|<span data-ttu-id="4933a-218">布尔</span><span class="sxs-lookup"><span data-stu-id="4933a-218">Boolean</span></span>|<span data-ttu-id="4933a-219">是否应启用防火墙。</span><span class="sxs-lookup"><span data-stu-id="4933a-219">Whether the firewall should be enabled or not.</span></span>|
|<span data-ttu-id="4933a-220">firewallBlockAllIncoming</span><span class="sxs-lookup"><span data-stu-id="4933a-220">firewallBlockAllIncoming</span></span>|<span data-ttu-id="4933a-221">布尔</span><span class="sxs-lookup"><span data-stu-id="4933a-221">Boolean</span></span>|<span data-ttu-id="4933a-222">对应于 "阻止所有传入连接" 选项。</span><span class="sxs-lookup"><span data-stu-id="4933a-222">Corresponds to the “Block all incoming connections” option.</span></span>|
|<span data-ttu-id="4933a-223">firewallEnableStealthMode</span><span class="sxs-lookup"><span data-stu-id="4933a-223">firewallEnableStealthMode</span></span>|<span data-ttu-id="4933a-224">布尔</span><span class="sxs-lookup"><span data-stu-id="4933a-224">Boolean</span></span>|<span data-ttu-id="4933a-225">对应于 "启用隐形模式"。</span><span class="sxs-lookup"><span data-stu-id="4933a-225">Corresponds to “Enable stealth mode.”</span></span>|



## <a name="response"></a><span data-ttu-id="4933a-226">响应</span><span class="sxs-lookup"><span data-stu-id="4933a-226">Response</span></span>
<span data-ttu-id="4933a-227">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和更新的 [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="4933a-227">If successful, this method returns a `200 OK` response code and an updated [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4933a-228">示例</span><span class="sxs-lookup"><span data-stu-id="4933a-228">Example</span></span>

### <a name="request"></a><span data-ttu-id="4933a-229">请求</span><span class="sxs-lookup"><span data-stu-id="4933a-229">Request</span></span>
<span data-ttu-id="4933a-230">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="4933a-230">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="4933a-231">响应</span><span class="sxs-lookup"><span data-stu-id="4933a-231">Response</span></span>
<span data-ttu-id="4933a-p115">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="4933a-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




