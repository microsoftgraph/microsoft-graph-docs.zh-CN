---
title: 创建 macOSCompliancePolicy
description: 创建新的 macOSCompliancePolicy 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: efbec3d5d89524900ab9c5b597a1fc82a41c9f46
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48704397"
---
# <a name="create-macoscompliancepolicy"></a><span data-ttu-id="f9976-103">创建 macOSCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="f9976-103">Create macOSCompliancePolicy</span></span>

<span data-ttu-id="f9976-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f9976-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f9976-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="f9976-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f9976-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f9976-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f9976-107">创建新的 [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="f9976-107">Create a new [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f9976-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="f9976-108">Prerequisites</span></span>
<span data-ttu-id="f9976-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f9976-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f9976-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="f9976-111">Permission type</span></span>|<span data-ttu-id="f9976-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="f9976-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f9976-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f9976-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f9976-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f9976-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f9976-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f9976-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f9976-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="f9976-116">Not supported.</span></span>|
|<span data-ttu-id="f9976-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="f9976-117">Application</span></span>|<span data-ttu-id="f9976-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f9976-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f9976-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f9976-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="f9976-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="f9976-120">Request headers</span></span>
|<span data-ttu-id="f9976-121">标头</span><span class="sxs-lookup"><span data-stu-id="f9976-121">Header</span></span>|<span data-ttu-id="f9976-122">值</span><span class="sxs-lookup"><span data-stu-id="f9976-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f9976-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f9976-123">Authorization</span></span>|<span data-ttu-id="f9976-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="f9976-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f9976-125">接受</span><span class="sxs-lookup"><span data-stu-id="f9976-125">Accept</span></span>|<span data-ttu-id="f9976-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f9976-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f9976-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="f9976-127">Request body</span></span>
<span data-ttu-id="f9976-128">在请求正文中，提供 macOSCompliancePolicy 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f9976-128">In the request body, supply a JSON representation for the macOSCompliancePolicy object.</span></span>

<span data-ttu-id="f9976-129">下表显示创建 macOSCompliancePolicy 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="f9976-129">The following table shows the properties that are required when you create the macOSCompliancePolicy.</span></span>

|<span data-ttu-id="f9976-130">属性</span><span class="sxs-lookup"><span data-stu-id="f9976-130">Property</span></span>|<span data-ttu-id="f9976-131">类型</span><span class="sxs-lookup"><span data-stu-id="f9976-131">Type</span></span>|<span data-ttu-id="f9976-132">说明</span><span class="sxs-lookup"><span data-stu-id="f9976-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f9976-133">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="f9976-133">roleScopeTagIds</span></span>|<span data-ttu-id="f9976-134">String collection</span><span class="sxs-lookup"><span data-stu-id="f9976-134">String collection</span></span>|<span data-ttu-id="f9976-135">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="f9976-135">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="f9976-136">继承自 [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="f9976-136">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="f9976-137">id</span><span class="sxs-lookup"><span data-stu-id="f9976-137">id</span></span>|<span data-ttu-id="f9976-138">String</span><span class="sxs-lookup"><span data-stu-id="f9976-138">String</span></span>|<span data-ttu-id="f9976-139">实体的键。</span><span class="sxs-lookup"><span data-stu-id="f9976-139">Key of the entity.</span></span> <span data-ttu-id="f9976-140">继承自 [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="f9976-140">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="f9976-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f9976-141">createdDateTime</span></span>|<span data-ttu-id="f9976-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f9976-142">DateTimeOffset</span></span>|<span data-ttu-id="f9976-143">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="f9976-143">DateTime the object was created.</span></span> <span data-ttu-id="f9976-144">继承自 [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="f9976-144">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="f9976-145">说明</span><span class="sxs-lookup"><span data-stu-id="f9976-145">description</span></span>|<span data-ttu-id="f9976-146">String</span><span class="sxs-lookup"><span data-stu-id="f9976-146">String</span></span>|<span data-ttu-id="f9976-147">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="f9976-147">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="f9976-148">继承自 [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="f9976-148">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="f9976-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f9976-149">lastModifiedDateTime</span></span>|<span data-ttu-id="f9976-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f9976-150">DateTimeOffset</span></span>|<span data-ttu-id="f9976-151">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="f9976-151">DateTime the object was last modified.</span></span> <span data-ttu-id="f9976-152">继承自 [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="f9976-152">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="f9976-153">displayName</span><span class="sxs-lookup"><span data-stu-id="f9976-153">displayName</span></span>|<span data-ttu-id="f9976-154">String</span><span class="sxs-lookup"><span data-stu-id="f9976-154">String</span></span>|<span data-ttu-id="f9976-155">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="f9976-155">Admin provided name of the device configuration.</span></span> <span data-ttu-id="f9976-156">继承自 [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="f9976-156">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="f9976-157">version</span><span class="sxs-lookup"><span data-stu-id="f9976-157">version</span></span>|<span data-ttu-id="f9976-158">Int32</span><span class="sxs-lookup"><span data-stu-id="f9976-158">Int32</span></span>|<span data-ttu-id="f9976-159">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="f9976-159">Version of the device configuration.</span></span> <span data-ttu-id="f9976-160">继承自 [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="f9976-160">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="f9976-161">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="f9976-161">passwordRequired</span></span>|<span data-ttu-id="f9976-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="f9976-162">Boolean</span></span>|<span data-ttu-id="f9976-163">是否需要密码。</span><span class="sxs-lookup"><span data-stu-id="f9976-163">Whether or not to require a password.</span></span>|
|<span data-ttu-id="f9976-164">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="f9976-164">passwordBlockSimple</span></span>|<span data-ttu-id="f9976-165">Boolean</span><span class="sxs-lookup"><span data-stu-id="f9976-165">Boolean</span></span>|<span data-ttu-id="f9976-166">指示是否阻止简单密码。</span><span class="sxs-lookup"><span data-stu-id="f9976-166">Indicates whether or not to block simple passwords.</span></span>|
|<span data-ttu-id="f9976-167">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="f9976-167">passwordExpirationDays</span></span>|<span data-ttu-id="f9976-168">Int32</span><span class="sxs-lookup"><span data-stu-id="f9976-168">Int32</span></span>|<span data-ttu-id="f9976-169">密码过期前的天数。</span><span class="sxs-lookup"><span data-stu-id="f9976-169">Number of days before the password expires.</span></span> <span data-ttu-id="f9976-170">有效值为 1 至 65535</span><span class="sxs-lookup"><span data-stu-id="f9976-170">Valid values 1 to 65535</span></span>|
|<span data-ttu-id="f9976-171">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="f9976-171">passwordMinimumLength</span></span>|<span data-ttu-id="f9976-172">Int32</span><span class="sxs-lookup"><span data-stu-id="f9976-172">Int32</span></span>|<span data-ttu-id="f9976-173">密码的最小长度。</span><span class="sxs-lookup"><span data-stu-id="f9976-173">Minimum length of password.</span></span> <span data-ttu-id="f9976-174">有效值为 4 至 14</span><span class="sxs-lookup"><span data-stu-id="f9976-174">Valid values 4 to 14</span></span>|
|<span data-ttu-id="f9976-175">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="f9976-175">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="f9976-176">Int32</span><span class="sxs-lookup"><span data-stu-id="f9976-176">Int32</span></span>|<span data-ttu-id="f9976-177">在需要密码之前不活动的分钟数。</span><span class="sxs-lookup"><span data-stu-id="f9976-177">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="f9976-178">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="f9976-178">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="f9976-179">Int32</span><span class="sxs-lookup"><span data-stu-id="f9976-179">Int32</span></span>|<span data-ttu-id="f9976-180">要阻止的以前密码的数量。</span><span class="sxs-lookup"><span data-stu-id="f9976-180">Number of previous passwords to block.</span></span> <span data-ttu-id="f9976-181">有效值为 1 至 24</span><span class="sxs-lookup"><span data-stu-id="f9976-181">Valid values 1 to 24</span></span>|
|<span data-ttu-id="f9976-182">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="f9976-182">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="f9976-183">Int32</span><span class="sxs-lookup"><span data-stu-id="f9976-183">Int32</span></span>|<span data-ttu-id="f9976-184">密码中必需的字符集数。</span><span class="sxs-lookup"><span data-stu-id="f9976-184">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="f9976-185">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="f9976-185">passwordRequiredType</span></span>|[<span data-ttu-id="f9976-186">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="f9976-186">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="f9976-187">必需的密码类型。</span><span class="sxs-lookup"><span data-stu-id="f9976-187">The required password type.</span></span> <span data-ttu-id="f9976-188">可取值为：`deviceDefault`、`alphanumeric`、`numeric`。</span><span class="sxs-lookup"><span data-stu-id="f9976-188">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="f9976-189">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="f9976-189">osMinimumVersion</span></span>|<span data-ttu-id="f9976-190">String</span><span class="sxs-lookup"><span data-stu-id="f9976-190">String</span></span>|<span data-ttu-id="f9976-191">最低 MacOS 版本。</span><span class="sxs-lookup"><span data-stu-id="f9976-191">Minimum MacOS version.</span></span>|
|<span data-ttu-id="f9976-192">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="f9976-192">osMaximumVersion</span></span>|<span data-ttu-id="f9976-193">String</span><span class="sxs-lookup"><span data-stu-id="f9976-193">String</span></span>|<span data-ttu-id="f9976-194">最大 MacOS 版本。</span><span class="sxs-lookup"><span data-stu-id="f9976-194">Maximum MacOS version.</span></span>|
|<span data-ttu-id="f9976-195">osMinimumBuildVersion</span><span class="sxs-lookup"><span data-stu-id="f9976-195">osMinimumBuildVersion</span></span>|<span data-ttu-id="f9976-196">String</span><span class="sxs-lookup"><span data-stu-id="f9976-196">String</span></span>|<span data-ttu-id="f9976-197">最低 MacOS 内部版本。</span><span class="sxs-lookup"><span data-stu-id="f9976-197">Minimum MacOS build version.</span></span>|
|<span data-ttu-id="f9976-198">osMaximumBuildVersion</span><span class="sxs-lookup"><span data-stu-id="f9976-198">osMaximumBuildVersion</span></span>|<span data-ttu-id="f9976-199">String</span><span class="sxs-lookup"><span data-stu-id="f9976-199">String</span></span>|<span data-ttu-id="f9976-200">最大 MacOS 内部版本。</span><span class="sxs-lookup"><span data-stu-id="f9976-200">Maximum MacOS build version.</span></span>|
|<span data-ttu-id="f9976-201">systemIntegrityProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="f9976-201">systemIntegrityProtectionEnabled</span></span>|<span data-ttu-id="f9976-202">Boolean</span><span class="sxs-lookup"><span data-stu-id="f9976-202">Boolean</span></span>|<span data-ttu-id="f9976-203">要求设备已启用系统完整性保护。</span><span class="sxs-lookup"><span data-stu-id="f9976-203">Require that devices have enabled system integrity protection.</span></span>|
|<span data-ttu-id="f9976-204">deviceThreatProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="f9976-204">deviceThreatProtectionEnabled</span></span>|<span data-ttu-id="f9976-205">Boolean</span><span class="sxs-lookup"><span data-stu-id="f9976-205">Boolean</span></span>|<span data-ttu-id="f9976-206">要求设备已启用设备威胁防护。</span><span class="sxs-lookup"><span data-stu-id="f9976-206">Require that devices have enabled device threat protection.</span></span>|
|<span data-ttu-id="f9976-207">deviceThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="f9976-207">deviceThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="f9976-208">deviceThreatProtectionLevel</span><span class="sxs-lookup"><span data-stu-id="f9976-208">deviceThreatProtectionLevel</span></span>](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|<span data-ttu-id="f9976-209">要求移动威胁防护最低风险级别来报告不符合情况。</span><span class="sxs-lookup"><span data-stu-id="f9976-209">Require Mobile Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="f9976-210">可取值为：`unavailable`、`secured`、`low`、`medium`、`high`、`notSet`。</span><span class="sxs-lookup"><span data-stu-id="f9976-210">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="f9976-211">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="f9976-211">storageRequireEncryption</span></span>|<span data-ttu-id="f9976-212">Boolean</span><span class="sxs-lookup"><span data-stu-id="f9976-212">Boolean</span></span>|<span data-ttu-id="f9976-213">要求对 Mac OS 设备加密。</span><span class="sxs-lookup"><span data-stu-id="f9976-213">Require encryption on Mac OS devices.</span></span>|
|<span data-ttu-id="f9976-214">gatekeeperAllowedAppSource</span><span class="sxs-lookup"><span data-stu-id="f9976-214">gatekeeperAllowedAppSource</span></span>|[<span data-ttu-id="f9976-215">macOSGatekeeperAppSources</span><span class="sxs-lookup"><span data-stu-id="f9976-215">macOSGatekeeperAppSources</span></span>](../resources/intune-deviceconfig-macosgatekeeperappsources.md)|<span data-ttu-id="f9976-216">确定可以从 macOS 设备上运行哪些下载位置应用程序的系统和隐私设置。</span><span class="sxs-lookup"><span data-stu-id="f9976-216">System and Privacy setting that determines which download locations apps can be run from on a macOS device.</span></span> <span data-ttu-id="f9976-217">可取值为：`notConfigured`、`macAppStore`、`macAppStoreAndIdentifiedDevelopers`、`anywhere`。</span><span class="sxs-lookup"><span data-stu-id="f9976-217">Possible values are: `notConfigured`, `macAppStore`, `macAppStoreAndIdentifiedDevelopers`, `anywhere`.</span></span>|
|<span data-ttu-id="f9976-218">firewallEnabled</span><span class="sxs-lookup"><span data-stu-id="f9976-218">firewallEnabled</span></span>|<span data-ttu-id="f9976-219">布尔</span><span class="sxs-lookup"><span data-stu-id="f9976-219">Boolean</span></span>|<span data-ttu-id="f9976-220">是否应启用防火墙。</span><span class="sxs-lookup"><span data-stu-id="f9976-220">Whether the firewall should be enabled or not.</span></span>|
|<span data-ttu-id="f9976-221">firewallBlockAllIncoming</span><span class="sxs-lookup"><span data-stu-id="f9976-221">firewallBlockAllIncoming</span></span>|<span data-ttu-id="f9976-222">布尔</span><span class="sxs-lookup"><span data-stu-id="f9976-222">Boolean</span></span>|<span data-ttu-id="f9976-223">对应于 "阻止所有传入连接" 选项。</span><span class="sxs-lookup"><span data-stu-id="f9976-223">Corresponds to the “Block all incoming connections” option.</span></span>|
|<span data-ttu-id="f9976-224">firewallEnableStealthMode</span><span class="sxs-lookup"><span data-stu-id="f9976-224">firewallEnableStealthMode</span></span>|<span data-ttu-id="f9976-225">布尔</span><span class="sxs-lookup"><span data-stu-id="f9976-225">Boolean</span></span>|<span data-ttu-id="f9976-226">对应于 "启用隐形模式"。</span><span class="sxs-lookup"><span data-stu-id="f9976-226">Corresponds to “Enable stealth mode.”</span></span>|



## <a name="response"></a><span data-ttu-id="f9976-227">响应</span><span class="sxs-lookup"><span data-stu-id="f9976-227">Response</span></span>
<span data-ttu-id="f9976-228">如果成功，此方法会在响应正文中返回 `201 Created` 响应代码和 [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="f9976-228">If successful, this method returns a `201 Created` response code and a [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f9976-229">示例</span><span class="sxs-lookup"><span data-stu-id="f9976-229">Example</span></span>

### <a name="request"></a><span data-ttu-id="f9976-230">请求</span><span class="sxs-lookup"><span data-stu-id="f9976-230">Request</span></span>
<span data-ttu-id="f9976-231">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="f9976-231">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="f9976-232">响应</span><span class="sxs-lookup"><span data-stu-id="f9976-232">Response</span></span>
<span data-ttu-id="f9976-p115">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="f9976-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





