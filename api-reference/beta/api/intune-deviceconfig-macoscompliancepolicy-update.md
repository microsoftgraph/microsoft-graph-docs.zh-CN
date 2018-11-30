---
title: 更新 macOSCompliancePolicy
description: 更新 macOSCompliancePolicy 对象的属性。
ms.openlocfilehash: 73e6d4d3fb0d24699e22b87dc3489a17e1287bd7
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27046286"
---
# <a name="update-macoscompliancepolicy"></a><span data-ttu-id="eb64e-103">更新 macOSCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="eb64e-103">Update macOSCompliancePolicy</span></span>

> <span data-ttu-id="eb64e-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="eb64e-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="eb64e-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="eb64e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="eb64e-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="eb64e-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="eb64e-107">更新 [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="eb64e-107">Update the properties of a [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="eb64e-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="eb64e-108">Prerequisites</span></span>
<span data-ttu-id="eb64e-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="eb64e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="eb64e-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="eb64e-111">Permission type</span></span>|<span data-ttu-id="eb64e-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="eb64e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="eb64e-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="eb64e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="eb64e-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eb64e-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="eb64e-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="eb64e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="eb64e-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="eb64e-116">Not supported.</span></span>|
|<span data-ttu-id="eb64e-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="eb64e-117">Application</span></span>|<span data-ttu-id="eb64e-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="eb64e-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="eb64e-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="eb64e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="eb64e-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="eb64e-120">Request headers</span></span>
|<span data-ttu-id="eb64e-121">标头</span><span class="sxs-lookup"><span data-stu-id="eb64e-121">Header</span></span>|<span data-ttu-id="eb64e-122">值</span><span class="sxs-lookup"><span data-stu-id="eb64e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="eb64e-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="eb64e-123">Authorization</span></span>|<span data-ttu-id="eb64e-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="eb64e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="eb64e-125">Accept</span><span class="sxs-lookup"><span data-stu-id="eb64e-125">Accept</span></span>|<span data-ttu-id="eb64e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="eb64e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="eb64e-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="eb64e-127">Request body</span></span>
<span data-ttu-id="eb64e-128">在请求正文中，提供 [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="eb64e-128">In the request body, supply a JSON representation for the [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) object.</span></span>

<span data-ttu-id="eb64e-129">下表显示创建 [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="eb64e-129">The following table shows the properties that are required when you create the [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md).</span></span>

|<span data-ttu-id="eb64e-130">属性</span><span class="sxs-lookup"><span data-stu-id="eb64e-130">Property</span></span>|<span data-ttu-id="eb64e-131">类型</span><span class="sxs-lookup"><span data-stu-id="eb64e-131">Type</span></span>|<span data-ttu-id="eb64e-132">说明</span><span class="sxs-lookup"><span data-stu-id="eb64e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="eb64e-133">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="eb64e-133">roleScopeTagIds</span></span>|<span data-ttu-id="eb64e-134">String 集合</span><span class="sxs-lookup"><span data-stu-id="eb64e-134">String collection</span></span>|<span data-ttu-id="eb64e-135">此实体实例范围标记的列表。</span><span class="sxs-lookup"><span data-stu-id="eb64e-135">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="eb64e-136">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="eb64e-136">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="eb64e-137">id</span><span class="sxs-lookup"><span data-stu-id="eb64e-137">id</span></span>|<span data-ttu-id="eb64e-138">String</span><span class="sxs-lookup"><span data-stu-id="eb64e-138">String</span></span>|<span data-ttu-id="eb64e-139">实体的键。</span><span class="sxs-lookup"><span data-stu-id="eb64e-139">Key of the entity.</span></span> <span data-ttu-id="eb64e-140">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="eb64e-140">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="eb64e-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="eb64e-141">createdDateTime</span></span>|<span data-ttu-id="eb64e-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="eb64e-142">DateTimeOffset</span></span>|<span data-ttu-id="eb64e-143">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="eb64e-143">DateTime the object was created.</span></span> <span data-ttu-id="eb64e-144">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="eb64e-144">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="eb64e-145">description</span><span class="sxs-lookup"><span data-stu-id="eb64e-145">description</span></span>|<span data-ttu-id="eb64e-146">String</span><span class="sxs-lookup"><span data-stu-id="eb64e-146">String</span></span>|<span data-ttu-id="eb64e-147">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="eb64e-147">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="eb64e-148">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="eb64e-148">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="eb64e-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="eb64e-149">lastModifiedDateTime</span></span>|<span data-ttu-id="eb64e-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="eb64e-150">DateTimeOffset</span></span>|<span data-ttu-id="eb64e-151">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="eb64e-151">DateTime the object was last modified.</span></span> <span data-ttu-id="eb64e-152">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="eb64e-152">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="eb64e-153">displayName</span><span class="sxs-lookup"><span data-stu-id="eb64e-153">displayName</span></span>|<span data-ttu-id="eb64e-154">String</span><span class="sxs-lookup"><span data-stu-id="eb64e-154">String</span></span>|<span data-ttu-id="eb64e-155">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="eb64e-155">Admin provided name of the device configuration.</span></span> <span data-ttu-id="eb64e-156">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="eb64e-156">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="eb64e-157">version</span><span class="sxs-lookup"><span data-stu-id="eb64e-157">version</span></span>|<span data-ttu-id="eb64e-158">Int32</span><span class="sxs-lookup"><span data-stu-id="eb64e-158">Int32</span></span>|<span data-ttu-id="eb64e-159">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="eb64e-159">Version of the device configuration.</span></span> <span data-ttu-id="eb64e-160">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="eb64e-160">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="eb64e-161">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="eb64e-161">passwordRequired</span></span>|<span data-ttu-id="eb64e-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="eb64e-162">Boolean</span></span>|<span data-ttu-id="eb64e-163">是否需要密码。</span><span class="sxs-lookup"><span data-stu-id="eb64e-163">Whether or not to require a password.</span></span>|
|<span data-ttu-id="eb64e-164">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="eb64e-164">passwordBlockSimple</span></span>|<span data-ttu-id="eb64e-165">Boolean</span><span class="sxs-lookup"><span data-stu-id="eb64e-165">Boolean</span></span>|<span data-ttu-id="eb64e-166">指示是否阻止简单密码。</span><span class="sxs-lookup"><span data-stu-id="eb64e-166">Indicates whether or not to block simple passwords.</span></span>|
|<span data-ttu-id="eb64e-167">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="eb64e-167">passwordExpirationDays</span></span>|<span data-ttu-id="eb64e-168">Int32</span><span class="sxs-lookup"><span data-stu-id="eb64e-168">Int32</span></span>|<span data-ttu-id="eb64e-169">密码过期前的天数。</span><span class="sxs-lookup"><span data-stu-id="eb64e-169">Number of days before the password expires.</span></span> <span data-ttu-id="eb64e-170">有效值为 1 至 65535</span><span class="sxs-lookup"><span data-stu-id="eb64e-170">Valid values 1 to 65535</span></span>|
|<span data-ttu-id="eb64e-171">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="eb64e-171">passwordMinimumLength</span></span>|<span data-ttu-id="eb64e-172">Int32</span><span class="sxs-lookup"><span data-stu-id="eb64e-172">Int32</span></span>|<span data-ttu-id="eb64e-173">密码的最小长度。</span><span class="sxs-lookup"><span data-stu-id="eb64e-173">Minimum length of password.</span></span> <span data-ttu-id="eb64e-174">有效值为 4 至 14</span><span class="sxs-lookup"><span data-stu-id="eb64e-174">Valid values 4 to 14</span></span>|
|<span data-ttu-id="eb64e-175">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="eb64e-175">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="eb64e-176">Int32</span><span class="sxs-lookup"><span data-stu-id="eb64e-176">Int32</span></span>|<span data-ttu-id="eb64e-177">在需要密码之前不活动的分钟数。</span><span class="sxs-lookup"><span data-stu-id="eb64e-177">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="eb64e-178">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="eb64e-178">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="eb64e-179">Int32</span><span class="sxs-lookup"><span data-stu-id="eb64e-179">Int32</span></span>|<span data-ttu-id="eb64e-180">要阻止的以前密码的数量。</span><span class="sxs-lookup"><span data-stu-id="eb64e-180">Number of previous passwords to block.</span></span> <span data-ttu-id="eb64e-181">有效值为 1 至 24</span><span class="sxs-lookup"><span data-stu-id="eb64e-181">Valid values 1 to 24</span></span>|
|<span data-ttu-id="eb64e-182">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="eb64e-182">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="eb64e-183">Int32</span><span class="sxs-lookup"><span data-stu-id="eb64e-183">Int32</span></span>|<span data-ttu-id="eb64e-184">密码中必需的字符集数。</span><span class="sxs-lookup"><span data-stu-id="eb64e-184">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="eb64e-185">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="eb64e-185">passwordRequiredType</span></span>|[<span data-ttu-id="eb64e-186">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="eb64e-186">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="eb64e-187">必需的密码类型。</span><span class="sxs-lookup"><span data-stu-id="eb64e-187">The required password type.</span></span> <span data-ttu-id="eb64e-188">可取值为：`deviceDefault`、`alphanumeric`、`numeric`。</span><span class="sxs-lookup"><span data-stu-id="eb64e-188">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="eb64e-189">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="eb64e-189">osMinimumVersion</span></span>|<span data-ttu-id="eb64e-190">String</span><span class="sxs-lookup"><span data-stu-id="eb64e-190">String</span></span>|<span data-ttu-id="eb64e-191">最低 IOS 版本。</span><span class="sxs-lookup"><span data-stu-id="eb64e-191">Minimum IOS version.</span></span>|
|<span data-ttu-id="eb64e-192">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="eb64e-192">osMaximumVersion</span></span>|<span data-ttu-id="eb64e-193">String</span><span class="sxs-lookup"><span data-stu-id="eb64e-193">String</span></span>|<span data-ttu-id="eb64e-194">最高 IOS 版本。</span><span class="sxs-lookup"><span data-stu-id="eb64e-194">Maximum IOS version.</span></span>|
|<span data-ttu-id="eb64e-195">systemIntegrityProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="eb64e-195">systemIntegrityProtectionEnabled</span></span>|<span data-ttu-id="eb64e-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="eb64e-196">Boolean</span></span>|<span data-ttu-id="eb64e-197">要求设备已启用系统完整性保护。</span><span class="sxs-lookup"><span data-stu-id="eb64e-197">Require that devices have enabled system integrity protection.</span></span>|
|<span data-ttu-id="eb64e-198">deviceThreatProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="eb64e-198">deviceThreatProtectionEnabled</span></span>|<span data-ttu-id="eb64e-199">Boolean</span><span class="sxs-lookup"><span data-stu-id="eb64e-199">Boolean</span></span>|<span data-ttu-id="eb64e-200">要求设备已启用设备威胁防护。</span><span class="sxs-lookup"><span data-stu-id="eb64e-200">Require that devices have enabled device threat protection .</span></span>|
|<span data-ttu-id="eb64e-201">deviceThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="eb64e-201">deviceThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="eb64e-202">deviceThreatProtectionLevel</span><span class="sxs-lookup"><span data-stu-id="eb64e-202">deviceThreatProtectionLevel</span></span>](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|<span data-ttu-id="eb64e-203">要求移动威胁防护最低风险级别来报告不符合情况。</span><span class="sxs-lookup"><span data-stu-id="eb64e-203">Require Mobile Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="eb64e-204">可取值为：`unavailable`、`secured`、`low`、`medium`、`high`、`notSet`。</span><span class="sxs-lookup"><span data-stu-id="eb64e-204">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="eb64e-205">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="eb64e-205">storageRequireEncryption</span></span>|<span data-ttu-id="eb64e-206">Boolean</span><span class="sxs-lookup"><span data-stu-id="eb64e-206">Boolean</span></span>|<span data-ttu-id="eb64e-207">要求对 Mac OS 设备加密。</span><span class="sxs-lookup"><span data-stu-id="eb64e-207">Require encryption on Mac OS devices.</span></span>|
|<span data-ttu-id="eb64e-208">gatekeeperAllowedAppSource</span><span class="sxs-lookup"><span data-stu-id="eb64e-208">gatekeeperAllowedAppSource</span></span>|[<span data-ttu-id="eb64e-209">macOSGatekeeperAppSources</span><span class="sxs-lookup"><span data-stu-id="eb64e-209">macOSGatekeeperAppSources</span></span>](../resources/intune-deviceconfig-macosgatekeeperappsources.md)|<span data-ttu-id="eb64e-210">系统和确定可以从 macOS 设备上运行的下载位置应用程序的隐私设置。</span><span class="sxs-lookup"><span data-stu-id="eb64e-210">System and Privacy setting that determines which download locations apps can be run from on a macOS device.</span></span> <span data-ttu-id="eb64e-211">可取值为：`notConfigured`、`macAppStore`、`macAppStoreAndIdentifiedDevelopers`、`anywhere`。</span><span class="sxs-lookup"><span data-stu-id="eb64e-211">Possible values are: `notConfigured`, `macAppStore`, `macAppStoreAndIdentifiedDevelopers`, `anywhere`.</span></span>|
|<span data-ttu-id="eb64e-212">firewallEnabled</span><span class="sxs-lookup"><span data-stu-id="eb64e-212">firewallEnabled</span></span>|<span data-ttu-id="eb64e-213">布尔</span><span class="sxs-lookup"><span data-stu-id="eb64e-213">Boolean</span></span>|<span data-ttu-id="eb64e-214">是否应启用防火墙，或不。</span><span class="sxs-lookup"><span data-stu-id="eb64e-214">Whether the firewall should be enabled or not.</span></span>|
|<span data-ttu-id="eb64e-215">firewallBlockAllIncoming</span><span class="sxs-lookup"><span data-stu-id="eb64e-215">firewallBlockAllIncoming</span></span>|<span data-ttu-id="eb64e-216">布尔</span><span class="sxs-lookup"><span data-stu-id="eb64e-216">Boolean</span></span>|<span data-ttu-id="eb64e-217">对应于"阻止所有传入连接"选项。</span><span class="sxs-lookup"><span data-stu-id="eb64e-217">Corresponds to the “Block all incoming connections” option.</span></span>|
|<span data-ttu-id="eb64e-218">firewallEnableStealthMode</span><span class="sxs-lookup"><span data-stu-id="eb64e-218">firewallEnableStealthMode</span></span>|<span data-ttu-id="eb64e-219">布尔</span><span class="sxs-lookup"><span data-stu-id="eb64e-219">Boolean</span></span>|<span data-ttu-id="eb64e-220">对应于"启用隐藏模式"。</span><span class="sxs-lookup"><span data-stu-id="eb64e-220">Corresponds to “Enable stealth mode.”</span></span>|



## <a name="response"></a><span data-ttu-id="eb64e-221">响应</span><span class="sxs-lookup"><span data-stu-id="eb64e-221">Response</span></span>
<span data-ttu-id="eb64e-222">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和更新的 [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="eb64e-222">If successful, this method returns a `200 OK` response code and an updated [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="eb64e-223">示例</span><span class="sxs-lookup"><span data-stu-id="eb64e-223">Example</span></span>
### <a name="request"></a><span data-ttu-id="eb64e-224">请求</span><span class="sxs-lookup"><span data-stu-id="eb64e-224">Request</span></span>
<span data-ttu-id="eb64e-225">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="eb64e-225">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
Content-type: application/json
Content-length: 963

{
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
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

### <a name="response"></a><span data-ttu-id="eb64e-226">响应</span><span class="sxs-lookup"><span data-stu-id="eb64e-226">Response</span></span>
<span data-ttu-id="eb64e-p116">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="eb64e-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1131

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





