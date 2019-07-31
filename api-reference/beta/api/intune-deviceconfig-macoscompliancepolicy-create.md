---
title: 创建 macOSCompliancePolicy
description: 创建新的 macOSCompliancePolicy 对象。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 25255686deaa8a9758fb3e70ad82c19c329aa80b
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35947555"
---
# <a name="create-macoscompliancepolicy"></a><span data-ttu-id="af88c-103">创建 macOSCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="af88c-103">Create macOSCompliancePolicy</span></span>

> <span data-ttu-id="af88c-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="af88c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="af88c-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="af88c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="af88c-106">创建新的 [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="af88c-106">Create a new [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="af88c-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="af88c-107">Prerequisites</span></span>
<span data-ttu-id="af88c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="af88c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="af88c-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="af88c-110">Permission type</span></span>|<span data-ttu-id="af88c-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="af88c-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="af88c-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="af88c-112">Delegated (work or school account)</span></span>|<span data-ttu-id="af88c-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="af88c-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="af88c-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="af88c-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="af88c-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="af88c-115">Not supported.</span></span>|
|<span data-ttu-id="af88c-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="af88c-116">Application</span></span>|<span data-ttu-id="af88c-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="af88c-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="af88c-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="af88c-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="af88c-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="af88c-119">Request headers</span></span>
|<span data-ttu-id="af88c-120">标头</span><span class="sxs-lookup"><span data-stu-id="af88c-120">Header</span></span>|<span data-ttu-id="af88c-121">值</span><span class="sxs-lookup"><span data-stu-id="af88c-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="af88c-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="af88c-122">Authorization</span></span>|<span data-ttu-id="af88c-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="af88c-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="af88c-124">接受</span><span class="sxs-lookup"><span data-stu-id="af88c-124">Accept</span></span>|<span data-ttu-id="af88c-125">application/json</span><span class="sxs-lookup"><span data-stu-id="af88c-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="af88c-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="af88c-126">Request body</span></span>
<span data-ttu-id="af88c-127">在请求正文中，提供 macOSCompliancePolicy 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="af88c-127">In the request body, supply a JSON representation for the macOSCompliancePolicy object.</span></span>

<span data-ttu-id="af88c-128">下表显示创建 macOSCompliancePolicy 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="af88c-128">The following table shows the properties that are required when you create the macOSCompliancePolicy.</span></span>

|<span data-ttu-id="af88c-129">属性</span><span class="sxs-lookup"><span data-stu-id="af88c-129">Property</span></span>|<span data-ttu-id="af88c-130">类型</span><span class="sxs-lookup"><span data-stu-id="af88c-130">Type</span></span>|<span data-ttu-id="af88c-131">说明</span><span class="sxs-lookup"><span data-stu-id="af88c-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="af88c-132">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="af88c-132">roleScopeTagIds</span></span>|<span data-ttu-id="af88c-133">String collection</span><span class="sxs-lookup"><span data-stu-id="af88c-133">String collection</span></span>|<span data-ttu-id="af88c-134">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="af88c-134">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="af88c-135">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="af88c-135">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="af88c-136">id</span><span class="sxs-lookup"><span data-stu-id="af88c-136">id</span></span>|<span data-ttu-id="af88c-137">字符串</span><span class="sxs-lookup"><span data-stu-id="af88c-137">String</span></span>|<span data-ttu-id="af88c-138">实体的键。</span><span class="sxs-lookup"><span data-stu-id="af88c-138">Key of the entity.</span></span> <span data-ttu-id="af88c-139">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="af88c-139">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="af88c-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="af88c-140">createdDateTime</span></span>|<span data-ttu-id="af88c-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="af88c-141">DateTimeOffset</span></span>|<span data-ttu-id="af88c-142">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="af88c-142">DateTime the object was created.</span></span> <span data-ttu-id="af88c-143">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="af88c-143">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="af88c-144">说明</span><span class="sxs-lookup"><span data-stu-id="af88c-144">description</span></span>|<span data-ttu-id="af88c-145">String</span><span class="sxs-lookup"><span data-stu-id="af88c-145">String</span></span>|<span data-ttu-id="af88c-146">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="af88c-146">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="af88c-147">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="af88c-147">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="af88c-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="af88c-148">lastModifiedDateTime</span></span>|<span data-ttu-id="af88c-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="af88c-149">DateTimeOffset</span></span>|<span data-ttu-id="af88c-150">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="af88c-150">DateTime the object was last modified.</span></span> <span data-ttu-id="af88c-151">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="af88c-151">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="af88c-152">displayName</span><span class="sxs-lookup"><span data-stu-id="af88c-152">displayName</span></span>|<span data-ttu-id="af88c-153">String</span><span class="sxs-lookup"><span data-stu-id="af88c-153">String</span></span>|<span data-ttu-id="af88c-154">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="af88c-154">Admin provided name of the device configuration.</span></span> <span data-ttu-id="af88c-155">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="af88c-155">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="af88c-156">version</span><span class="sxs-lookup"><span data-stu-id="af88c-156">version</span></span>|<span data-ttu-id="af88c-157">Int32</span><span class="sxs-lookup"><span data-stu-id="af88c-157">Int32</span></span>|<span data-ttu-id="af88c-158">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="af88c-158">Version of the device configuration.</span></span> <span data-ttu-id="af88c-159">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="af88c-159">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="af88c-160">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="af88c-160">passwordRequired</span></span>|<span data-ttu-id="af88c-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="af88c-161">Boolean</span></span>|<span data-ttu-id="af88c-162">是否需要密码。</span><span class="sxs-lookup"><span data-stu-id="af88c-162">Whether or not to require a password.</span></span>|
|<span data-ttu-id="af88c-163">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="af88c-163">passwordBlockSimple</span></span>|<span data-ttu-id="af88c-164">Boolean</span><span class="sxs-lookup"><span data-stu-id="af88c-164">Boolean</span></span>|<span data-ttu-id="af88c-165">指示是否阻止简单密码。</span><span class="sxs-lookup"><span data-stu-id="af88c-165">Indicates whether or not to block simple passwords.</span></span>|
|<span data-ttu-id="af88c-166">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="af88c-166">passwordExpirationDays</span></span>|<span data-ttu-id="af88c-167">Int32</span><span class="sxs-lookup"><span data-stu-id="af88c-167">Int32</span></span>|<span data-ttu-id="af88c-168">密码过期前的天数。</span><span class="sxs-lookup"><span data-stu-id="af88c-168">Number of days before the password expires.</span></span> <span data-ttu-id="af88c-169">有效值为 1 至 65535</span><span class="sxs-lookup"><span data-stu-id="af88c-169">Valid values 1 to 65535</span></span>|
|<span data-ttu-id="af88c-170">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="af88c-170">passwordMinimumLength</span></span>|<span data-ttu-id="af88c-171">Int32</span><span class="sxs-lookup"><span data-stu-id="af88c-171">Int32</span></span>|<span data-ttu-id="af88c-172">密码的最小长度。</span><span class="sxs-lookup"><span data-stu-id="af88c-172">Minimum length of password.</span></span> <span data-ttu-id="af88c-173">有效值为 4 至 14</span><span class="sxs-lookup"><span data-stu-id="af88c-173">Valid values 4 to 14</span></span>|
|<span data-ttu-id="af88c-174">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="af88c-174">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="af88c-175">Int32</span><span class="sxs-lookup"><span data-stu-id="af88c-175">Int32</span></span>|<span data-ttu-id="af88c-176">在需要密码之前不活动的分钟数。</span><span class="sxs-lookup"><span data-stu-id="af88c-176">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="af88c-177">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="af88c-177">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="af88c-178">Int32</span><span class="sxs-lookup"><span data-stu-id="af88c-178">Int32</span></span>|<span data-ttu-id="af88c-179">要阻止的以前密码的数量。</span><span class="sxs-lookup"><span data-stu-id="af88c-179">Number of previous passwords to block.</span></span> <span data-ttu-id="af88c-180">有效值为 1 至 24</span><span class="sxs-lookup"><span data-stu-id="af88c-180">Valid values 1 to 24</span></span>|
|<span data-ttu-id="af88c-181">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="af88c-181">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="af88c-182">Int32</span><span class="sxs-lookup"><span data-stu-id="af88c-182">Int32</span></span>|<span data-ttu-id="af88c-183">密码中必需的字符集数。</span><span class="sxs-lookup"><span data-stu-id="af88c-183">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="af88c-184">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="af88c-184">passwordRequiredType</span></span>|[<span data-ttu-id="af88c-185">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="af88c-185">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="af88c-186">必需的密码类型。</span><span class="sxs-lookup"><span data-stu-id="af88c-186">The required password type.</span></span> <span data-ttu-id="af88c-187">可取值为：`deviceDefault`、`alphanumeric`、`numeric`。</span><span class="sxs-lookup"><span data-stu-id="af88c-187">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="af88c-188">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="af88c-188">osMinimumVersion</span></span>|<span data-ttu-id="af88c-189">String</span><span class="sxs-lookup"><span data-stu-id="af88c-189">String</span></span>|<span data-ttu-id="af88c-190">最低 MacOS 版本。</span><span class="sxs-lookup"><span data-stu-id="af88c-190">Minimum MacOS version.</span></span>|
|<span data-ttu-id="af88c-191">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="af88c-191">osMaximumVersion</span></span>|<span data-ttu-id="af88c-192">String</span><span class="sxs-lookup"><span data-stu-id="af88c-192">String</span></span>|<span data-ttu-id="af88c-193">最大 MacOS 版本。</span><span class="sxs-lookup"><span data-stu-id="af88c-193">Maximum MacOS version.</span></span>|
|<span data-ttu-id="af88c-194">osMinimumBuildVersion</span><span class="sxs-lookup"><span data-stu-id="af88c-194">osMinimumBuildVersion</span></span>|<span data-ttu-id="af88c-195">String</span><span class="sxs-lookup"><span data-stu-id="af88c-195">String</span></span>|<span data-ttu-id="af88c-196">最低 MacOS 内部版本。</span><span class="sxs-lookup"><span data-stu-id="af88c-196">Minimum MacOS build version.</span></span>|
|<span data-ttu-id="af88c-197">osMaximumBuildVersion</span><span class="sxs-lookup"><span data-stu-id="af88c-197">osMaximumBuildVersion</span></span>|<span data-ttu-id="af88c-198">String</span><span class="sxs-lookup"><span data-stu-id="af88c-198">String</span></span>|<span data-ttu-id="af88c-199">最大 MacOS 内部版本。</span><span class="sxs-lookup"><span data-stu-id="af88c-199">Maximum MacOS build version.</span></span>|
|<span data-ttu-id="af88c-200">systemIntegrityProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="af88c-200">systemIntegrityProtectionEnabled</span></span>|<span data-ttu-id="af88c-201">Boolean</span><span class="sxs-lookup"><span data-stu-id="af88c-201">Boolean</span></span>|<span data-ttu-id="af88c-202">要求设备已启用系统完整性保护。</span><span class="sxs-lookup"><span data-stu-id="af88c-202">Require that devices have enabled system integrity protection.</span></span>|
|<span data-ttu-id="af88c-203">deviceThreatProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="af88c-203">deviceThreatProtectionEnabled</span></span>|<span data-ttu-id="af88c-204">Boolean</span><span class="sxs-lookup"><span data-stu-id="af88c-204">Boolean</span></span>|<span data-ttu-id="af88c-205">要求设备已启用设备威胁防护。</span><span class="sxs-lookup"><span data-stu-id="af88c-205">Require that devices have enabled device threat protection.</span></span>|
|<span data-ttu-id="af88c-206">deviceThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="af88c-206">deviceThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="af88c-207">deviceThreatProtectionLevel</span><span class="sxs-lookup"><span data-stu-id="af88c-207">deviceThreatProtectionLevel</span></span>](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|<span data-ttu-id="af88c-208">要求移动威胁防护最低风险级别来报告不符合情况。</span><span class="sxs-lookup"><span data-stu-id="af88c-208">Require Mobile Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="af88c-209">可取值为：`unavailable`、`secured`、`low`、`medium`、`high`、`notSet`。</span><span class="sxs-lookup"><span data-stu-id="af88c-209">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="af88c-210">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="af88c-210">storageRequireEncryption</span></span>|<span data-ttu-id="af88c-211">Boolean</span><span class="sxs-lookup"><span data-stu-id="af88c-211">Boolean</span></span>|<span data-ttu-id="af88c-212">要求对 Mac OS 设备加密。</span><span class="sxs-lookup"><span data-stu-id="af88c-212">Require encryption on Mac OS devices.</span></span>|
|<span data-ttu-id="af88c-213">gatekeeperAllowedAppSource</span><span class="sxs-lookup"><span data-stu-id="af88c-213">gatekeeperAllowedAppSource</span></span>|[<span data-ttu-id="af88c-214">macOSGatekeeperAppSources</span><span class="sxs-lookup"><span data-stu-id="af88c-214">macOSGatekeeperAppSources</span></span>](../resources/intune-deviceconfig-macosgatekeeperappsources.md)|<span data-ttu-id="af88c-215">确定可以从 macOS 设备上运行哪些下载位置应用程序的系统和隐私设置。</span><span class="sxs-lookup"><span data-stu-id="af88c-215">System and Privacy setting that determines which download locations apps can be run from on a macOS device.</span></span> <span data-ttu-id="af88c-216">可取值为：`notConfigured`、`macAppStore`、`macAppStoreAndIdentifiedDevelopers`、`anywhere`。</span><span class="sxs-lookup"><span data-stu-id="af88c-216">Possible values are: `notConfigured`, `macAppStore`, `macAppStoreAndIdentifiedDevelopers`, `anywhere`.</span></span>|
|<span data-ttu-id="af88c-217">firewallEnabled</span><span class="sxs-lookup"><span data-stu-id="af88c-217">firewallEnabled</span></span>|<span data-ttu-id="af88c-218">Boolean</span><span class="sxs-lookup"><span data-stu-id="af88c-218">Boolean</span></span>|<span data-ttu-id="af88c-219">是否应启用防火墙。</span><span class="sxs-lookup"><span data-stu-id="af88c-219">Whether the firewall should be enabled or not.</span></span>|
|<span data-ttu-id="af88c-220">firewallBlockAllIncoming</span><span class="sxs-lookup"><span data-stu-id="af88c-220">firewallBlockAllIncoming</span></span>|<span data-ttu-id="af88c-221">Boolean</span><span class="sxs-lookup"><span data-stu-id="af88c-221">Boolean</span></span>|<span data-ttu-id="af88c-222">对应于 "阻止所有传入连接" 选项。</span><span class="sxs-lookup"><span data-stu-id="af88c-222">Corresponds to the “Block all incoming connections” option.</span></span>|
|<span data-ttu-id="af88c-223">firewallEnableStealthMode</span><span class="sxs-lookup"><span data-stu-id="af88c-223">firewallEnableStealthMode</span></span>|<span data-ttu-id="af88c-224">Boolean</span><span class="sxs-lookup"><span data-stu-id="af88c-224">Boolean</span></span>|<span data-ttu-id="af88c-225">对应于 "启用隐形模式"。</span><span class="sxs-lookup"><span data-stu-id="af88c-225">Corresponds to “Enable stealth mode.”</span></span>|



## <a name="response"></a><span data-ttu-id="af88c-226">响应</span><span class="sxs-lookup"><span data-stu-id="af88c-226">Response</span></span>
<span data-ttu-id="af88c-227">如果成功，此方法会在响应正文中返回 `201 Created` 响应代码和 [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="af88c-227">If successful, this method returns a `201 Created` response code and a [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="af88c-228">示例</span><span class="sxs-lookup"><span data-stu-id="af88c-228">Example</span></span>

### <a name="request"></a><span data-ttu-id="af88c-229">请求</span><span class="sxs-lookup"><span data-stu-id="af88c-229">Request</span></span>
<span data-ttu-id="af88c-230">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="af88c-230">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies
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

### <a name="response"></a><span data-ttu-id="af88c-231">响应</span><span class="sxs-lookup"><span data-stu-id="af88c-231">Response</span></span>
<span data-ttu-id="af88c-p115">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="af88c-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





