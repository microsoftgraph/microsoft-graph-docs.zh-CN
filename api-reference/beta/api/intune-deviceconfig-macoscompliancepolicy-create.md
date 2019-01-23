---
title: 创建 macOSCompliancePolicy
description: 创建新的 macOSCompliancePolicy 对象。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: c08c62af9bc702472ea57801e4bd8e6ef5a4decf
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29397832"
---
# <a name="create-macoscompliancepolicy"></a><span data-ttu-id="6fb84-103">创建 macOSCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="6fb84-103">Create macOSCompliancePolicy</span></span>

> <span data-ttu-id="6fb84-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="6fb84-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="6fb84-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="6fb84-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="6fb84-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="6fb84-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6fb84-107">创建新的 [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="6fb84-107">Create a new [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6fb84-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="6fb84-108">Prerequisites</span></span>
<span data-ttu-id="6fb84-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="6fb84-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="6fb84-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="6fb84-111">Permission type</span></span>|<span data-ttu-id="6fb84-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="6fb84-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6fb84-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6fb84-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6fb84-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6fb84-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="6fb84-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6fb84-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6fb84-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="6fb84-116">Not supported.</span></span>|
|<span data-ttu-id="6fb84-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="6fb84-117">Application</span></span>|<span data-ttu-id="6fb84-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="6fb84-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6fb84-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6fb84-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="6fb84-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="6fb84-120">Request headers</span></span>
|<span data-ttu-id="6fb84-121">标头</span><span class="sxs-lookup"><span data-stu-id="6fb84-121">Header</span></span>|<span data-ttu-id="6fb84-122">值</span><span class="sxs-lookup"><span data-stu-id="6fb84-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6fb84-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="6fb84-123">Authorization</span></span>|<span data-ttu-id="6fb84-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="6fb84-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6fb84-125">Accept</span><span class="sxs-lookup"><span data-stu-id="6fb84-125">Accept</span></span>|<span data-ttu-id="6fb84-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6fb84-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6fb84-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="6fb84-127">Request body</span></span>
<span data-ttu-id="6fb84-128">在请求正文中，提供 macOSCompliancePolicy 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6fb84-128">In the request body, supply a JSON representation for the macOSCompliancePolicy object.</span></span>

<span data-ttu-id="6fb84-129">下表显示创建 macOSCompliancePolicy 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="6fb84-129">The following table shows the properties that are required when you create the macOSCompliancePolicy.</span></span>

|<span data-ttu-id="6fb84-130">属性</span><span class="sxs-lookup"><span data-stu-id="6fb84-130">Property</span></span>|<span data-ttu-id="6fb84-131">类型</span><span class="sxs-lookup"><span data-stu-id="6fb84-131">Type</span></span>|<span data-ttu-id="6fb84-132">说明</span><span class="sxs-lookup"><span data-stu-id="6fb84-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6fb84-133">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="6fb84-133">roleScopeTagIds</span></span>|<span data-ttu-id="6fb84-134">String 集合</span><span class="sxs-lookup"><span data-stu-id="6fb84-134">String collection</span></span>|<span data-ttu-id="6fb84-135">此实体实例范围标记的列表。</span><span class="sxs-lookup"><span data-stu-id="6fb84-135">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="6fb84-136">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="6fb84-136">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="6fb84-137">id</span><span class="sxs-lookup"><span data-stu-id="6fb84-137">id</span></span>|<span data-ttu-id="6fb84-138">String</span><span class="sxs-lookup"><span data-stu-id="6fb84-138">String</span></span>|<span data-ttu-id="6fb84-139">实体的键。</span><span class="sxs-lookup"><span data-stu-id="6fb84-139">Key of the entity.</span></span> <span data-ttu-id="6fb84-140">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="6fb84-140">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="6fb84-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6fb84-141">createdDateTime</span></span>|<span data-ttu-id="6fb84-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6fb84-142">DateTimeOffset</span></span>|<span data-ttu-id="6fb84-143">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="6fb84-143">DateTime the object was created.</span></span> <span data-ttu-id="6fb84-144">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="6fb84-144">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="6fb84-145">description</span><span class="sxs-lookup"><span data-stu-id="6fb84-145">description</span></span>|<span data-ttu-id="6fb84-146">String</span><span class="sxs-lookup"><span data-stu-id="6fb84-146">String</span></span>|<span data-ttu-id="6fb84-147">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="6fb84-147">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="6fb84-148">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="6fb84-148">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="6fb84-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6fb84-149">lastModifiedDateTime</span></span>|<span data-ttu-id="6fb84-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6fb84-150">DateTimeOffset</span></span>|<span data-ttu-id="6fb84-151">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="6fb84-151">DateTime the object was last modified.</span></span> <span data-ttu-id="6fb84-152">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="6fb84-152">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="6fb84-153">displayName</span><span class="sxs-lookup"><span data-stu-id="6fb84-153">displayName</span></span>|<span data-ttu-id="6fb84-154">String</span><span class="sxs-lookup"><span data-stu-id="6fb84-154">String</span></span>|<span data-ttu-id="6fb84-155">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="6fb84-155">Admin provided name of the device configuration.</span></span> <span data-ttu-id="6fb84-156">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="6fb84-156">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="6fb84-157">version</span><span class="sxs-lookup"><span data-stu-id="6fb84-157">version</span></span>|<span data-ttu-id="6fb84-158">Int32</span><span class="sxs-lookup"><span data-stu-id="6fb84-158">Int32</span></span>|<span data-ttu-id="6fb84-159">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="6fb84-159">Version of the device configuration.</span></span> <span data-ttu-id="6fb84-160">继承自 [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="6fb84-160">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="6fb84-161">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="6fb84-161">passwordRequired</span></span>|<span data-ttu-id="6fb84-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="6fb84-162">Boolean</span></span>|<span data-ttu-id="6fb84-163">是否需要密码。</span><span class="sxs-lookup"><span data-stu-id="6fb84-163">Whether or not to require a password.</span></span>|
|<span data-ttu-id="6fb84-164">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="6fb84-164">passwordBlockSimple</span></span>|<span data-ttu-id="6fb84-165">Boolean</span><span class="sxs-lookup"><span data-stu-id="6fb84-165">Boolean</span></span>|<span data-ttu-id="6fb84-166">指示是否阻止简单密码。</span><span class="sxs-lookup"><span data-stu-id="6fb84-166">Indicates whether or not to block simple passwords.</span></span>|
|<span data-ttu-id="6fb84-167">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="6fb84-167">passwordExpirationDays</span></span>|<span data-ttu-id="6fb84-168">Int32</span><span class="sxs-lookup"><span data-stu-id="6fb84-168">Int32</span></span>|<span data-ttu-id="6fb84-169">密码过期前的天数。</span><span class="sxs-lookup"><span data-stu-id="6fb84-169">Number of days before the password expires.</span></span> <span data-ttu-id="6fb84-170">有效值为 1 至 65535</span><span class="sxs-lookup"><span data-stu-id="6fb84-170">Valid values 1 to 65535</span></span>|
|<span data-ttu-id="6fb84-171">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="6fb84-171">passwordMinimumLength</span></span>|<span data-ttu-id="6fb84-172">Int32</span><span class="sxs-lookup"><span data-stu-id="6fb84-172">Int32</span></span>|<span data-ttu-id="6fb84-173">密码的最小长度。</span><span class="sxs-lookup"><span data-stu-id="6fb84-173">Minimum length of password.</span></span> <span data-ttu-id="6fb84-174">有效值为 4 至 14</span><span class="sxs-lookup"><span data-stu-id="6fb84-174">Valid values 4 to 14</span></span>|
|<span data-ttu-id="6fb84-175">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="6fb84-175">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="6fb84-176">Int32</span><span class="sxs-lookup"><span data-stu-id="6fb84-176">Int32</span></span>|<span data-ttu-id="6fb84-177">在需要密码之前不活动的分钟数。</span><span class="sxs-lookup"><span data-stu-id="6fb84-177">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="6fb84-178">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="6fb84-178">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="6fb84-179">Int32</span><span class="sxs-lookup"><span data-stu-id="6fb84-179">Int32</span></span>|<span data-ttu-id="6fb84-180">要阻止的以前密码的数量。</span><span class="sxs-lookup"><span data-stu-id="6fb84-180">Number of previous passwords to block.</span></span> <span data-ttu-id="6fb84-181">有效值为 1 至 24</span><span class="sxs-lookup"><span data-stu-id="6fb84-181">Valid values 1 to 24</span></span>|
|<span data-ttu-id="6fb84-182">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="6fb84-182">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="6fb84-183">Int32</span><span class="sxs-lookup"><span data-stu-id="6fb84-183">Int32</span></span>|<span data-ttu-id="6fb84-184">密码中必需的字符集数。</span><span class="sxs-lookup"><span data-stu-id="6fb84-184">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="6fb84-185">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="6fb84-185">passwordRequiredType</span></span>|[<span data-ttu-id="6fb84-186">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="6fb84-186">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="6fb84-187">必需的密码类型。</span><span class="sxs-lookup"><span data-stu-id="6fb84-187">The required password type.</span></span> <span data-ttu-id="6fb84-188">可取值为：`deviceDefault`、`alphanumeric`、`numeric`。</span><span class="sxs-lookup"><span data-stu-id="6fb84-188">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="6fb84-189">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="6fb84-189">osMinimumVersion</span></span>|<span data-ttu-id="6fb84-190">String</span><span class="sxs-lookup"><span data-stu-id="6fb84-190">String</span></span>|<span data-ttu-id="6fb84-191">最低 MacOS 版本。</span><span class="sxs-lookup"><span data-stu-id="6fb84-191">Minimum MacOS version.</span></span>|
|<span data-ttu-id="6fb84-192">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="6fb84-192">osMaximumVersion</span></span>|<span data-ttu-id="6fb84-193">String</span><span class="sxs-lookup"><span data-stu-id="6fb84-193">String</span></span>|<span data-ttu-id="6fb84-194">最大 MacOS 版本。</span><span class="sxs-lookup"><span data-stu-id="6fb84-194">Maximum MacOS version.</span></span>|
|<span data-ttu-id="6fb84-195">osMinimumBuildVersion</span><span class="sxs-lookup"><span data-stu-id="6fb84-195">osMinimumBuildVersion</span></span>|<span data-ttu-id="6fb84-196">String</span><span class="sxs-lookup"><span data-stu-id="6fb84-196">String</span></span>|<span data-ttu-id="6fb84-197">最小 MacOS 生成版本。</span><span class="sxs-lookup"><span data-stu-id="6fb84-197">Minimum MacOS build version.</span></span>|
|<span data-ttu-id="6fb84-198">osMaximumBuildVersion</span><span class="sxs-lookup"><span data-stu-id="6fb84-198">osMaximumBuildVersion</span></span>|<span data-ttu-id="6fb84-199">String</span><span class="sxs-lookup"><span data-stu-id="6fb84-199">String</span></span>|<span data-ttu-id="6fb84-200">最大 MacOS 生成版本。</span><span class="sxs-lookup"><span data-stu-id="6fb84-200">Maximum MacOS build version.</span></span>|
|<span data-ttu-id="6fb84-201">systemIntegrityProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="6fb84-201">systemIntegrityProtectionEnabled</span></span>|<span data-ttu-id="6fb84-202">Boolean</span><span class="sxs-lookup"><span data-stu-id="6fb84-202">Boolean</span></span>|<span data-ttu-id="6fb84-203">要求设备已启用系统完整性保护。</span><span class="sxs-lookup"><span data-stu-id="6fb84-203">Require that devices have enabled system integrity protection.</span></span>|
|<span data-ttu-id="6fb84-204">deviceThreatProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="6fb84-204">deviceThreatProtectionEnabled</span></span>|<span data-ttu-id="6fb84-205">Boolean</span><span class="sxs-lookup"><span data-stu-id="6fb84-205">Boolean</span></span>|<span data-ttu-id="6fb84-206">要求设备已启用设备威胁防护。</span><span class="sxs-lookup"><span data-stu-id="6fb84-206">Require that devices have enabled device threat protection.</span></span>|
|<span data-ttu-id="6fb84-207">deviceThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="6fb84-207">deviceThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="6fb84-208">deviceThreatProtectionLevel</span><span class="sxs-lookup"><span data-stu-id="6fb84-208">deviceThreatProtectionLevel</span></span>](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|<span data-ttu-id="6fb84-209">要求移动威胁防护最低风险级别来报告不符合情况。</span><span class="sxs-lookup"><span data-stu-id="6fb84-209">Require Mobile Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="6fb84-210">可取值为：`unavailable`、`secured`、`low`、`medium`、`high`、`notSet`。</span><span class="sxs-lookup"><span data-stu-id="6fb84-210">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="6fb84-211">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="6fb84-211">storageRequireEncryption</span></span>|<span data-ttu-id="6fb84-212">Boolean</span><span class="sxs-lookup"><span data-stu-id="6fb84-212">Boolean</span></span>|<span data-ttu-id="6fb84-213">要求对 Mac OS 设备加密。</span><span class="sxs-lookup"><span data-stu-id="6fb84-213">Require encryption on Mac OS devices.</span></span>|
|<span data-ttu-id="6fb84-214">gatekeeperAllowedAppSource</span><span class="sxs-lookup"><span data-stu-id="6fb84-214">gatekeeperAllowedAppSource</span></span>|[<span data-ttu-id="6fb84-215">macOSGatekeeperAppSources</span><span class="sxs-lookup"><span data-stu-id="6fb84-215">macOSGatekeeperAppSources</span></span>](../resources/intune-deviceconfig-macosgatekeeperappsources.md)|<span data-ttu-id="6fb84-216">系统和确定可以从 macOS 设备上运行的下载位置应用程序的隐私设置。</span><span class="sxs-lookup"><span data-stu-id="6fb84-216">System and Privacy setting that determines which download locations apps can be run from on a macOS device.</span></span> <span data-ttu-id="6fb84-217">可取值为：`notConfigured`、`macAppStore`、`macAppStoreAndIdentifiedDevelopers`、`anywhere`。</span><span class="sxs-lookup"><span data-stu-id="6fb84-217">Possible values are: `notConfigured`, `macAppStore`, `macAppStoreAndIdentifiedDevelopers`, `anywhere`.</span></span>|
|<span data-ttu-id="6fb84-218">firewallEnabled</span><span class="sxs-lookup"><span data-stu-id="6fb84-218">firewallEnabled</span></span>|<span data-ttu-id="6fb84-219">Boolean</span><span class="sxs-lookup"><span data-stu-id="6fb84-219">Boolean</span></span>|<span data-ttu-id="6fb84-220">是否应启用防火墙，或不。</span><span class="sxs-lookup"><span data-stu-id="6fb84-220">Whether the firewall should be enabled or not.</span></span>|
|<span data-ttu-id="6fb84-221">firewallBlockAllIncoming</span><span class="sxs-lookup"><span data-stu-id="6fb84-221">firewallBlockAllIncoming</span></span>|<span data-ttu-id="6fb84-222">Boolean</span><span class="sxs-lookup"><span data-stu-id="6fb84-222">Boolean</span></span>|<span data-ttu-id="6fb84-223">对应于"阻止所有传入连接"选项。</span><span class="sxs-lookup"><span data-stu-id="6fb84-223">Corresponds to the “Block all incoming connections” option.</span></span>|
|<span data-ttu-id="6fb84-224">firewallEnableStealthMode</span><span class="sxs-lookup"><span data-stu-id="6fb84-224">firewallEnableStealthMode</span></span>|<span data-ttu-id="6fb84-225">Boolean</span><span class="sxs-lookup"><span data-stu-id="6fb84-225">Boolean</span></span>|<span data-ttu-id="6fb84-226">对应于"启用隐藏模式"。</span><span class="sxs-lookup"><span data-stu-id="6fb84-226">Corresponds to “Enable stealth mode.”</span></span>|



## <a name="response"></a><span data-ttu-id="6fb84-227">响应</span><span class="sxs-lookup"><span data-stu-id="6fb84-227">Response</span></span>
<span data-ttu-id="6fb84-228">如果成功，此方法会在响应正文中返回 `201 Created` 响应代码和 [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="6fb84-228">If successful, this method returns a `201 Created` response code and a [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6fb84-229">示例</span><span class="sxs-lookup"><span data-stu-id="6fb84-229">Example</span></span>

### <a name="request"></a><span data-ttu-id="6fb84-230">请求</span><span class="sxs-lookup"><span data-stu-id="6fb84-230">Request</span></span>
<span data-ttu-id="6fb84-231">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="6fb84-231">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="6fb84-232">响应</span><span class="sxs-lookup"><span data-stu-id="6fb84-232">Response</span></span>
<span data-ttu-id="6fb84-p116">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="6fb84-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




