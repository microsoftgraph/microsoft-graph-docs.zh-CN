---
title: 更新 macOSCompliancePolicy
description: 更新 macOSCompliancePolicy 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c2eb1e7835d0febcd608f8019557d6955065fab1
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/11/2019
ms.locfileid: "31797394"
---
# <a name="update-macoscompliancepolicy"></a><span data-ttu-id="4d615-103">更新 macOSCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="4d615-103">Update macOSCompliancePolicy</span></span>

> <span data-ttu-id="4d615-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="4d615-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4d615-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="4d615-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4d615-106">更新 [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="4d615-106">Update the properties of a [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4d615-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="4d615-107">Prerequisites</span></span>
<span data-ttu-id="4d615-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4d615-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4d615-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="4d615-110">Permission type</span></span>|<span data-ttu-id="4d615-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="4d615-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4d615-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4d615-112">Delegated (work or school account)</span></span>|<span data-ttu-id="4d615-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4d615-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="4d615-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4d615-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4d615-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="4d615-115">Not supported.</span></span>|
|<span data-ttu-id="4d615-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="4d615-116">Application</span></span>|<span data-ttu-id="4d615-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="4d615-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4d615-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4d615-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="4d615-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="4d615-119">Request headers</span></span>
|<span data-ttu-id="4d615-120">标头</span><span class="sxs-lookup"><span data-stu-id="4d615-120">Header</span></span>|<span data-ttu-id="4d615-121">值</span><span class="sxs-lookup"><span data-stu-id="4d615-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4d615-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="4d615-122">Authorization</span></span>|<span data-ttu-id="4d615-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="4d615-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4d615-124">接受</span><span class="sxs-lookup"><span data-stu-id="4d615-124">Accept</span></span>|<span data-ttu-id="4d615-125">application/json</span><span class="sxs-lookup"><span data-stu-id="4d615-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4d615-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="4d615-126">Request body</span></span>
<span data-ttu-id="4d615-127">在请求正文中，提供 [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4d615-127">In the request body, supply a JSON representation for the [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) object.</span></span>

<span data-ttu-id="4d615-128">下表显示创建 [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="4d615-128">The following table shows the properties that are required when you create the [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md).</span></span>

|<span data-ttu-id="4d615-129">属性</span><span class="sxs-lookup"><span data-stu-id="4d615-129">Property</span></span>|<span data-ttu-id="4d615-130">类型</span><span class="sxs-lookup"><span data-stu-id="4d615-130">Type</span></span>|<span data-ttu-id="4d615-131">说明</span><span class="sxs-lookup"><span data-stu-id="4d615-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4d615-132">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="4d615-132">roleScopeTagIds</span></span>|<span data-ttu-id="4d615-133">String 集合</span><span class="sxs-lookup"><span data-stu-id="4d615-133">String collection</span></span>|<span data-ttu-id="4d615-134">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="4d615-134">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="4d615-135">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="4d615-135">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="4d615-136">id</span><span class="sxs-lookup"><span data-stu-id="4d615-136">id</span></span>|<span data-ttu-id="4d615-137">String</span><span class="sxs-lookup"><span data-stu-id="4d615-137">String</span></span>|<span data-ttu-id="4d615-138">实体的键。</span><span class="sxs-lookup"><span data-stu-id="4d615-138">Key of the entity.</span></span> <span data-ttu-id="4d615-139">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="4d615-139">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="4d615-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="4d615-140">createdDateTime</span></span>|<span data-ttu-id="4d615-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4d615-141">DateTimeOffset</span></span>|<span data-ttu-id="4d615-142">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="4d615-142">DateTime the object was created.</span></span> <span data-ttu-id="4d615-143">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="4d615-143">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="4d615-144">description</span><span class="sxs-lookup"><span data-stu-id="4d615-144">description</span></span>|<span data-ttu-id="4d615-145">String</span><span class="sxs-lookup"><span data-stu-id="4d615-145">String</span></span>|<span data-ttu-id="4d615-146">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="4d615-146">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="4d615-147">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="4d615-147">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="4d615-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4d615-148">lastModifiedDateTime</span></span>|<span data-ttu-id="4d615-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4d615-149">DateTimeOffset</span></span>|<span data-ttu-id="4d615-150">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="4d615-150">DateTime the object was last modified.</span></span> <span data-ttu-id="4d615-151">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="4d615-151">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="4d615-152">displayName</span><span class="sxs-lookup"><span data-stu-id="4d615-152">displayName</span></span>|<span data-ttu-id="4d615-153">String</span><span class="sxs-lookup"><span data-stu-id="4d615-153">String</span></span>|<span data-ttu-id="4d615-154">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="4d615-154">Admin provided name of the device configuration.</span></span> <span data-ttu-id="4d615-155">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="4d615-155">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="4d615-156">version</span><span class="sxs-lookup"><span data-stu-id="4d615-156">version</span></span>|<span data-ttu-id="4d615-157">Int32</span><span class="sxs-lookup"><span data-stu-id="4d615-157">Int32</span></span>|<span data-ttu-id="4d615-158">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="4d615-158">Version of the device configuration.</span></span> <span data-ttu-id="4d615-159">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="4d615-159">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="4d615-160">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="4d615-160">passwordRequired</span></span>|<span data-ttu-id="4d615-161">布尔值</span><span class="sxs-lookup"><span data-stu-id="4d615-161">Boolean</span></span>|<span data-ttu-id="4d615-162">是否需要密码。</span><span class="sxs-lookup"><span data-stu-id="4d615-162">Whether or not to require a password.</span></span>|
|<span data-ttu-id="4d615-163">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="4d615-163">passwordBlockSimple</span></span>|<span data-ttu-id="4d615-164">布尔值</span><span class="sxs-lookup"><span data-stu-id="4d615-164">Boolean</span></span>|<span data-ttu-id="4d615-165">指示是否阻止简单密码。</span><span class="sxs-lookup"><span data-stu-id="4d615-165">Indicates whether or not to block simple passwords.</span></span>|
|<span data-ttu-id="4d615-166">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="4d615-166">passwordExpirationDays</span></span>|<span data-ttu-id="4d615-167">Int32</span><span class="sxs-lookup"><span data-stu-id="4d615-167">Int32</span></span>|<span data-ttu-id="4d615-168">密码过期前的天数。</span><span class="sxs-lookup"><span data-stu-id="4d615-168">Number of days before the password expires.</span></span> <span data-ttu-id="4d615-169">有效值为 1 至 65535</span><span class="sxs-lookup"><span data-stu-id="4d615-169">Valid values 1 to 65535</span></span>|
|<span data-ttu-id="4d615-170">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="4d615-170">passwordMinimumLength</span></span>|<span data-ttu-id="4d615-171">Int32</span><span class="sxs-lookup"><span data-stu-id="4d615-171">Int32</span></span>|<span data-ttu-id="4d615-172">密码的最小长度。</span><span class="sxs-lookup"><span data-stu-id="4d615-172">Minimum length of password.</span></span> <span data-ttu-id="4d615-173">有效值为 4 至 14</span><span class="sxs-lookup"><span data-stu-id="4d615-173">Valid values 4 to 14</span></span>|
|<span data-ttu-id="4d615-174">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="4d615-174">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="4d615-175">Int32</span><span class="sxs-lookup"><span data-stu-id="4d615-175">Int32</span></span>|<span data-ttu-id="4d615-176">在需要密码之前不活动的分钟数。</span><span class="sxs-lookup"><span data-stu-id="4d615-176">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="4d615-177">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="4d615-177">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="4d615-178">Int32</span><span class="sxs-lookup"><span data-stu-id="4d615-178">Int32</span></span>|<span data-ttu-id="4d615-179">要阻止的以前密码的数量。</span><span class="sxs-lookup"><span data-stu-id="4d615-179">Number of previous passwords to block.</span></span> <span data-ttu-id="4d615-180">有效值为 1 至 24</span><span class="sxs-lookup"><span data-stu-id="4d615-180">Valid values 1 to 24</span></span>|
|<span data-ttu-id="4d615-181">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="4d615-181">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="4d615-182">Int32</span><span class="sxs-lookup"><span data-stu-id="4d615-182">Int32</span></span>|<span data-ttu-id="4d615-183">密码中必需的字符集数。</span><span class="sxs-lookup"><span data-stu-id="4d615-183">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="4d615-184">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="4d615-184">passwordRequiredType</span></span>|[<span data-ttu-id="4d615-185">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="4d615-185">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="4d615-186">必需的密码类型。</span><span class="sxs-lookup"><span data-stu-id="4d615-186">The required password type.</span></span> <span data-ttu-id="4d615-187">可取值为：`deviceDefault`、`alphanumeric`、`numeric`。</span><span class="sxs-lookup"><span data-stu-id="4d615-187">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="4d615-188">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="4d615-188">osMinimumVersion</span></span>|<span data-ttu-id="4d615-189">String</span><span class="sxs-lookup"><span data-stu-id="4d615-189">String</span></span>|<span data-ttu-id="4d615-190">最低 MacOS 版本。</span><span class="sxs-lookup"><span data-stu-id="4d615-190">Minimum MacOS version.</span></span>|
|<span data-ttu-id="4d615-191">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="4d615-191">osMaximumVersion</span></span>|<span data-ttu-id="4d615-192">String</span><span class="sxs-lookup"><span data-stu-id="4d615-192">String</span></span>|<span data-ttu-id="4d615-193">最大 MacOS 版本。</span><span class="sxs-lookup"><span data-stu-id="4d615-193">Maximum MacOS version.</span></span>|
|<span data-ttu-id="4d615-194">osMinimumBuildVersion</span><span class="sxs-lookup"><span data-stu-id="4d615-194">osMinimumBuildVersion</span></span>|<span data-ttu-id="4d615-195">String</span><span class="sxs-lookup"><span data-stu-id="4d615-195">String</span></span>|<span data-ttu-id="4d615-196">最低 MacOS 内部版本。</span><span class="sxs-lookup"><span data-stu-id="4d615-196">Minimum MacOS build version.</span></span>|
|<span data-ttu-id="4d615-197">osMaximumBuildVersion</span><span class="sxs-lookup"><span data-stu-id="4d615-197">osMaximumBuildVersion</span></span>|<span data-ttu-id="4d615-198">String</span><span class="sxs-lookup"><span data-stu-id="4d615-198">String</span></span>|<span data-ttu-id="4d615-199">最大 MacOS 内部版本。</span><span class="sxs-lookup"><span data-stu-id="4d615-199">Maximum MacOS build version.</span></span>|
|<span data-ttu-id="4d615-200">systemIntegrityProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="4d615-200">systemIntegrityProtectionEnabled</span></span>|<span data-ttu-id="4d615-201">Boolean</span><span class="sxs-lookup"><span data-stu-id="4d615-201">Boolean</span></span>|<span data-ttu-id="4d615-202">要求设备已启用系统完整性保护。</span><span class="sxs-lookup"><span data-stu-id="4d615-202">Require that devices have enabled system integrity protection.</span></span>|
|<span data-ttu-id="4d615-203">deviceThreatProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="4d615-203">deviceThreatProtectionEnabled</span></span>|<span data-ttu-id="4d615-204">布尔值</span><span class="sxs-lookup"><span data-stu-id="4d615-204">Boolean</span></span>|<span data-ttu-id="4d615-205">要求设备已启用设备威胁防护。</span><span class="sxs-lookup"><span data-stu-id="4d615-205">Require that devices have enabled device threat protection.</span></span>|
|<span data-ttu-id="4d615-206">deviceThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="4d615-206">deviceThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="4d615-207">deviceThreatProtectionLevel</span><span class="sxs-lookup"><span data-stu-id="4d615-207">deviceThreatProtectionLevel</span></span>](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|<span data-ttu-id="4d615-208">要求移动威胁防护最低风险级别来报告不符合情况。</span><span class="sxs-lookup"><span data-stu-id="4d615-208">Require Mobile Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="4d615-209">可取值为：`unavailable`、`secured`、`low`、`medium`、`high`、`notSet`。</span><span class="sxs-lookup"><span data-stu-id="4d615-209">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="4d615-210">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="4d615-210">storageRequireEncryption</span></span>|<span data-ttu-id="4d615-211">Boolean</span><span class="sxs-lookup"><span data-stu-id="4d615-211">Boolean</span></span>|<span data-ttu-id="4d615-212">要求对 Mac OS 设备加密。</span><span class="sxs-lookup"><span data-stu-id="4d615-212">Require encryption on Mac OS devices.</span></span>|
|<span data-ttu-id="4d615-213">gatekeeperAllowedAppSource</span><span class="sxs-lookup"><span data-stu-id="4d615-213">gatekeeperAllowedAppSource</span></span>|[<span data-ttu-id="4d615-214">macOSGatekeeperAppSources</span><span class="sxs-lookup"><span data-stu-id="4d615-214">macOSGatekeeperAppSources</span></span>](../resources/intune-deviceconfig-macosgatekeeperappsources.md)|<span data-ttu-id="4d615-215">确定可以从 macOS 设备上运行哪些下载位置应用程序的系统和隐私设置。</span><span class="sxs-lookup"><span data-stu-id="4d615-215">System and Privacy setting that determines which download locations apps can be run from on a macOS device.</span></span> <span data-ttu-id="4d615-216">可取值为：`notConfigured`、`macAppStore`、`macAppStoreAndIdentifiedDevelopers`、`anywhere`。</span><span class="sxs-lookup"><span data-stu-id="4d615-216">Possible values are: `notConfigured`, `macAppStore`, `macAppStoreAndIdentifiedDevelopers`, `anywhere`.</span></span>|
|<span data-ttu-id="4d615-217">firewallEnabled</span><span class="sxs-lookup"><span data-stu-id="4d615-217">firewallEnabled</span></span>|<span data-ttu-id="4d615-218">布尔值</span><span class="sxs-lookup"><span data-stu-id="4d615-218">Boolean</span></span>|<span data-ttu-id="4d615-219">是否应启用防火墙。</span><span class="sxs-lookup"><span data-stu-id="4d615-219">Whether the firewall should be enabled or not.</span></span>|
|<span data-ttu-id="4d615-220">firewallBlockAllIncoming</span><span class="sxs-lookup"><span data-stu-id="4d615-220">firewallBlockAllIncoming</span></span>|<span data-ttu-id="4d615-221">布尔值</span><span class="sxs-lookup"><span data-stu-id="4d615-221">Boolean</span></span>|<span data-ttu-id="4d615-222">对应于 "阻止所有传入连接" 选项。</span><span class="sxs-lookup"><span data-stu-id="4d615-222">Corresponds to the “Block all incoming connections” option.</span></span>|
|<span data-ttu-id="4d615-223">firewallEnableStealthMode</span><span class="sxs-lookup"><span data-stu-id="4d615-223">firewallEnableStealthMode</span></span>|<span data-ttu-id="4d615-224">布尔值</span><span class="sxs-lookup"><span data-stu-id="4d615-224">Boolean</span></span>|<span data-ttu-id="4d615-225">对应于 "启用隐形模式"。</span><span class="sxs-lookup"><span data-stu-id="4d615-225">Corresponds to “Enable stealth mode.”</span></span>|



## <a name="response"></a><span data-ttu-id="4d615-226">响应</span><span class="sxs-lookup"><span data-stu-id="4d615-226">Response</span></span>
<span data-ttu-id="4d615-227">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和更新的 [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="4d615-227">If successful, this method returns a `200 OK` response code and an updated [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4d615-228">示例</span><span class="sxs-lookup"><span data-stu-id="4d615-228">Example</span></span>

### <a name="request"></a><span data-ttu-id="4d615-229">请求</span><span class="sxs-lookup"><span data-stu-id="4d615-229">Request</span></span>
<span data-ttu-id="4d615-230">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="4d615-230">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="4d615-231">响应</span><span class="sxs-lookup"><span data-stu-id="4d615-231">Response</span></span>
<span data-ttu-id="4d615-p115">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="4d615-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





