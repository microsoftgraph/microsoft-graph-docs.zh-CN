---
title: 更新 macOSEndpointProtectionConfiguration
description: 更新 macOSEndpointProtectionConfiguration 对象的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: fb6176da0a02e16e68c793e4ea7252f63820fd8e
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36315440"
---
# <a name="update-macosendpointprotectionconfiguration"></a><span data-ttu-id="38a75-103">更新 macOSEndpointProtectionConfiguration</span><span class="sxs-lookup"><span data-stu-id="38a75-103">Update macOSEndpointProtectionConfiguration</span></span>

> <span data-ttu-id="38a75-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="38a75-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="38a75-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="38a75-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="38a75-106">更新[macOSEndpointProtectionConfiguration](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="38a75-106">Update the properties of a [macOSEndpointProtectionConfiguration](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="38a75-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="38a75-107">Prerequisites</span></span>
<span data-ttu-id="38a75-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="38a75-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="38a75-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="38a75-110">Permission type</span></span>|<span data-ttu-id="38a75-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="38a75-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="38a75-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="38a75-112">Delegated (work or school account)</span></span>|<span data-ttu-id="38a75-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="38a75-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="38a75-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="38a75-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="38a75-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="38a75-115">Not supported.</span></span>|
|<span data-ttu-id="38a75-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="38a75-116">Application</span></span>|<span data-ttu-id="38a75-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="38a75-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="38a75-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="38a75-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="38a75-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="38a75-119">Request headers</span></span>
|<span data-ttu-id="38a75-120">标头</span><span class="sxs-lookup"><span data-stu-id="38a75-120">Header</span></span>|<span data-ttu-id="38a75-121">值</span><span class="sxs-lookup"><span data-stu-id="38a75-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="38a75-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="38a75-122">Authorization</span></span>|<span data-ttu-id="38a75-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="38a75-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="38a75-124">接受</span><span class="sxs-lookup"><span data-stu-id="38a75-124">Accept</span></span>|<span data-ttu-id="38a75-125">application/json</span><span class="sxs-lookup"><span data-stu-id="38a75-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="38a75-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="38a75-126">Request body</span></span>
<span data-ttu-id="38a75-127">在请求正文中, 提供[macOSEndpointProtectionConfiguration](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="38a75-127">In the request body, supply a JSON representation for the [macOSEndpointProtectionConfiguration](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md) object.</span></span>

<span data-ttu-id="38a75-128">下表显示创建[macOSEndpointProtectionConfiguration](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="38a75-128">The following table shows the properties that are required when you create the [macOSEndpointProtectionConfiguration](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md).</span></span>

|<span data-ttu-id="38a75-129">属性</span><span class="sxs-lookup"><span data-stu-id="38a75-129">Property</span></span>|<span data-ttu-id="38a75-130">类型</span><span class="sxs-lookup"><span data-stu-id="38a75-130">Type</span></span>|<span data-ttu-id="38a75-131">说明</span><span class="sxs-lookup"><span data-stu-id="38a75-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="38a75-132">id</span><span class="sxs-lookup"><span data-stu-id="38a75-132">id</span></span>|<span data-ttu-id="38a75-133">字符串</span><span class="sxs-lookup"><span data-stu-id="38a75-133">String</span></span>|<span data-ttu-id="38a75-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="38a75-134">Key of the entity.</span></span> <span data-ttu-id="38a75-135">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="38a75-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="38a75-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="38a75-136">lastModifiedDateTime</span></span>|<span data-ttu-id="38a75-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="38a75-137">DateTimeOffset</span></span>|<span data-ttu-id="38a75-138">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="38a75-138">DateTime the object was last modified.</span></span> <span data-ttu-id="38a75-139">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="38a75-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="38a75-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="38a75-140">roleScopeTagIds</span></span>|<span data-ttu-id="38a75-141">String collection</span><span class="sxs-lookup"><span data-stu-id="38a75-141">String collection</span></span>|<span data-ttu-id="38a75-142">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="38a75-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="38a75-143">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="38a75-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="38a75-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="38a75-144">supportsScopeTags</span></span>|<span data-ttu-id="38a75-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="38a75-145">Boolean</span></span>|<span data-ttu-id="38a75-146">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="38a75-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="38a75-147">如果此值为 false, 则不允许分配给 ScopeTags 属性, 并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="38a75-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="38a75-148">这适用于在 Silverlight 中创建的旧版策略, 可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="38a75-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="38a75-149">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="38a75-149">This property is read-only.</span></span> <span data-ttu-id="38a75-150">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="38a75-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="38a75-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="38a75-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="38a75-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="38a75-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="38a75-153">适用于此策略的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="38a75-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="38a75-154">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="38a75-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="38a75-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="38a75-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="38a75-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="38a75-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="38a75-157">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="38a75-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="38a75-158">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="38a75-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="38a75-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="38a75-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="38a75-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="38a75-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="38a75-161">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="38a75-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="38a75-162">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="38a75-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="38a75-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="38a75-163">createdDateTime</span></span>|<span data-ttu-id="38a75-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="38a75-164">DateTimeOffset</span></span>|<span data-ttu-id="38a75-165">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="38a75-165">DateTime the object was created.</span></span> <span data-ttu-id="38a75-166">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="38a75-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="38a75-167">说明</span><span class="sxs-lookup"><span data-stu-id="38a75-167">description</span></span>|<span data-ttu-id="38a75-168">String</span><span class="sxs-lookup"><span data-stu-id="38a75-168">String</span></span>|<span data-ttu-id="38a75-169">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="38a75-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="38a75-170">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="38a75-170">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="38a75-171">displayName</span><span class="sxs-lookup"><span data-stu-id="38a75-171">displayName</span></span>|<span data-ttu-id="38a75-172">String</span><span class="sxs-lookup"><span data-stu-id="38a75-172">String</span></span>|<span data-ttu-id="38a75-173">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="38a75-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="38a75-174">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="38a75-174">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="38a75-175">version</span><span class="sxs-lookup"><span data-stu-id="38a75-175">version</span></span>|<span data-ttu-id="38a75-176">Int32</span><span class="sxs-lookup"><span data-stu-id="38a75-176">Int32</span></span>|<span data-ttu-id="38a75-177">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="38a75-177">Version of the device configuration.</span></span> <span data-ttu-id="38a75-178">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="38a75-178">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="38a75-179">gatekeeperAllowedAppSource</span><span class="sxs-lookup"><span data-stu-id="38a75-179">gatekeeperAllowedAppSource</span></span>|[<span data-ttu-id="38a75-180">macOSGatekeeperAppSources</span><span class="sxs-lookup"><span data-stu-id="38a75-180">macOSGatekeeperAppSources</span></span>](../resources/intune-deviceconfig-macosgatekeeperappsources.md)|<span data-ttu-id="38a75-181">确定可以从 macOS 设备上运行哪些下载位置应用程序的系统和隐私设置。</span><span class="sxs-lookup"><span data-stu-id="38a75-181">System and Privacy setting that determines which download locations apps can be run from on a macOS device.</span></span> <span data-ttu-id="38a75-182">可取值为：`notConfigured`、`macAppStore`、`macAppStoreAndIdentifiedDevelopers`、`anywhere`。</span><span class="sxs-lookup"><span data-stu-id="38a75-182">Possible values are: `notConfigured`, `macAppStore`, `macAppStoreAndIdentifiedDevelopers`, `anywhere`.</span></span>|
|<span data-ttu-id="38a75-183">gatekeeperBlockOverride</span><span class="sxs-lookup"><span data-stu-id="38a75-183">gatekeeperBlockOverride</span></span>|<span data-ttu-id="38a75-184">Boolean</span><span class="sxs-lookup"><span data-stu-id="38a75-184">Boolean</span></span>|<span data-ttu-id="38a75-185">如果设置为 true, 将禁用网关的用户替代。</span><span class="sxs-lookup"><span data-stu-id="38a75-185">If set to true, the user override for Gatekeeper will be disabled.</span></span>|
|<span data-ttu-id="38a75-186">firewallEnabled</span><span class="sxs-lookup"><span data-stu-id="38a75-186">firewallEnabled</span></span>|<span data-ttu-id="38a75-187">Boolean</span><span class="sxs-lookup"><span data-stu-id="38a75-187">Boolean</span></span>|<span data-ttu-id="38a75-188">是否应启用防火墙。</span><span class="sxs-lookup"><span data-stu-id="38a75-188">Whether the firewall should be enabled or not.</span></span>|
|<span data-ttu-id="38a75-189">firewallBlockAllIncoming</span><span class="sxs-lookup"><span data-stu-id="38a75-189">firewallBlockAllIncoming</span></span>|<span data-ttu-id="38a75-190">Boolean</span><span class="sxs-lookup"><span data-stu-id="38a75-190">Boolean</span></span>|<span data-ttu-id="38a75-191">对应于 "阻止所有传入连接" 选项。</span><span class="sxs-lookup"><span data-stu-id="38a75-191">Corresponds to the “Block all incoming connections” option.</span></span>|
|<span data-ttu-id="38a75-192">firewallEnableStealthMode</span><span class="sxs-lookup"><span data-stu-id="38a75-192">firewallEnableStealthMode</span></span>|<span data-ttu-id="38a75-193">Boolean</span><span class="sxs-lookup"><span data-stu-id="38a75-193">Boolean</span></span>|<span data-ttu-id="38a75-194">对应于 "启用隐形模式"。</span><span class="sxs-lookup"><span data-stu-id="38a75-194">Corresponds to “Enable stealth mode.”</span></span>|
|<span data-ttu-id="38a75-195">firewallApplications</span><span class="sxs-lookup"><span data-stu-id="38a75-195">firewallApplications</span></span>|<span data-ttu-id="38a75-196">[macOSFirewallApplication](../resources/intune-deviceconfig-macosfirewallapplication.md)集合</span><span class="sxs-lookup"><span data-stu-id="38a75-196">[macOSFirewallApplication](../resources/intune-deviceconfig-macosfirewallapplication.md) collection</span></span>|<span data-ttu-id="38a75-197">具有防火墙设置的应用程序列表。</span><span class="sxs-lookup"><span data-stu-id="38a75-197">List of applications with firewall settings.</span></span> <span data-ttu-id="38a75-198">不在此列表中的应用程序的防火墙设置由用户决定。</span><span class="sxs-lookup"><span data-stu-id="38a75-198">Firewall settings for applications not on this list are determined by the user.</span></span> <span data-ttu-id="38a75-199">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="38a75-199">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="38a75-200">fileVaultEnabled</span><span class="sxs-lookup"><span data-stu-id="38a75-200">fileVaultEnabled</span></span>|<span data-ttu-id="38a75-201">Boolean</span><span class="sxs-lookup"><span data-stu-id="38a75-201">Boolean</span></span>|<span data-ttu-id="38a75-202">是否应启用 FileVault。</span><span class="sxs-lookup"><span data-stu-id="38a75-202">Whether FileVault should be enabled or not.</span></span>|
|<span data-ttu-id="38a75-203">fileVaultSelectedRecoveryKeyTypes</span><span class="sxs-lookup"><span data-stu-id="38a75-203">fileVaultSelectedRecoveryKeyTypes</span></span>|[<span data-ttu-id="38a75-204">macOSFileVaultRecoveryKeyTypes</span><span class="sxs-lookup"><span data-stu-id="38a75-204">macOSFileVaultRecoveryKeyTypes</span></span>](../resources/intune-deviceconfig-macosfilevaultrecoverykeytypes.md)|<span data-ttu-id="38a75-205">如果启用了 FileVault, 则需要确定要使用的恢复密钥的类型。</span><span class="sxs-lookup"><span data-stu-id="38a75-205">Required if FileVault is enabled, determines the type(s) of recovery key to use.</span></span> <span data-ttu-id="38a75-206">.</span><span class="sxs-lookup"><span data-stu-id="38a75-206"></span></span> <span data-ttu-id="38a75-207">可取值为：`notConfigured`、`institutionalRecoveryKey`、`personalRecoveryKey`。</span><span class="sxs-lookup"><span data-stu-id="38a75-207">Possible values are: `notConfigured`, `institutionalRecoveryKey`, `personalRecoveryKey`.</span></span>|
|<span data-ttu-id="38a75-208">fileVaultInstitutionalRecoveryKeyCertificate</span><span class="sxs-lookup"><span data-stu-id="38a75-208">fileVaultInstitutionalRecoveryKeyCertificate</span></span>|<span data-ttu-id="38a75-209">Binary</span><span class="sxs-lookup"><span data-stu-id="38a75-209">Binary</span></span>|<span data-ttu-id="38a75-210">如果所选恢复密钥类型包括 InstitutionalRecoveryKey, 则为必需。</span><span class="sxs-lookup"><span data-stu-id="38a75-210">Required if selected recovery key type(s) include InstitutionalRecoveryKey.</span></span> <span data-ttu-id="38a75-211">用于设置机构恢复密钥的 DER 编码证书文件。</span><span class="sxs-lookup"><span data-stu-id="38a75-211">The DER Encoded certificate file used to set an institutional recovery key.</span></span>|
|<span data-ttu-id="38a75-212">fileVaultInstitutionalRecoveryKeyCertificateFileName</span><span class="sxs-lookup"><span data-stu-id="38a75-212">fileVaultInstitutionalRecoveryKeyCertificateFileName</span></span>|<span data-ttu-id="38a75-213">String</span><span class="sxs-lookup"><span data-stu-id="38a75-213">String</span></span>|<span data-ttu-id="38a75-214">要在 UI 中显示的机构恢复密钥证书的文件名。</span><span class="sxs-lookup"><span data-stu-id="38a75-214">File name of the institutional recovery key certificate to display in UI.</span></span> <span data-ttu-id="38a75-215">(\* der)。</span><span class="sxs-lookup"><span data-stu-id="38a75-215">(\*.der).</span></span>|
|<span data-ttu-id="38a75-216">fileVaultPersonalRecoveryKeyHelpMessage</span><span class="sxs-lookup"><span data-stu-id="38a75-216">fileVaultPersonalRecoveryKeyHelpMessage</span></span>|<span data-ttu-id="38a75-217">String</span><span class="sxs-lookup"><span data-stu-id="38a75-217">String</span></span>|<span data-ttu-id="38a75-218">如果所选恢复密钥类型包括 PersonalRecoveryKey, 则为必需。</span><span class="sxs-lookup"><span data-stu-id="38a75-218">Required if selected recovery key type(s) include PersonalRecoveryKey.</span></span> <span data-ttu-id="38a75-219">向用户显示一条简短消息, 说明他们如何检索其个人恢复密钥。</span><span class="sxs-lookup"><span data-stu-id="38a75-219">A short message displayed to the user that explains how they can retrieve their personal recovery key.</span></span>|
|<span data-ttu-id="38a75-220">fileVaultAllowDeferralUntilSignOut</span><span class="sxs-lookup"><span data-stu-id="38a75-220">fileVaultAllowDeferralUntilSignOut</span></span>|<span data-ttu-id="38a75-221">Boolean</span><span class="sxs-lookup"><span data-stu-id="38a75-221">Boolean</span></span>|<span data-ttu-id="38a75-222">可选。</span><span class="sxs-lookup"><span data-stu-id="38a75-222">Optional.</span></span> <span data-ttu-id="38a75-223">如果设置为 true, 则用户可以推迟启用 FileVault, 直到他们注销。</span><span class="sxs-lookup"><span data-stu-id="38a75-223">If set to true, the user can defer the enabling of FileVault until they sign out.</span></span>|
|<span data-ttu-id="38a75-224">fileVaultNumberOfTimesUserCanIgnore</span><span class="sxs-lookup"><span data-stu-id="38a75-224">fileVaultNumberOfTimesUserCanIgnore</span></span>|<span data-ttu-id="38a75-225">Int32</span><span class="sxs-lookup"><span data-stu-id="38a75-225">Int32</span></span>|<span data-ttu-id="38a75-226">可选。</span><span class="sxs-lookup"><span data-stu-id="38a75-226">Optional.</span></span> <span data-ttu-id="38a75-227">使用 Defer 选项时, 此值是用户可以在 FileVault 之前忽略启用 FileVault 的提示的最大次数, 用户将需要这些用户才能登录。</span><span class="sxs-lookup"><span data-stu-id="38a75-227">When using the Defer option, this is the maximum number of times the user can ignore prompts to enable FileVault before FileVault will be required for the user to sign in.</span></span> <span data-ttu-id="38a75-228">如果设置为-1, 则在启用 FileVault 之前, 它将始终提示启用 FileVault, 但它将允许用户绕过启用 FileVault。</span><span class="sxs-lookup"><span data-stu-id="38a75-228">If set to -1, it will always prompt to enable FileVault until FileVault is enabled, though it will allow the user to bypass enabling FileVault.</span></span> <span data-ttu-id="38a75-229">将此设置为0将禁用该功能。</span><span class="sxs-lookup"><span data-stu-id="38a75-229">Setting this to 0 will disable the feature.</span></span>|
|<span data-ttu-id="38a75-230">fileVaultDisablePromptAtSignOut</span><span class="sxs-lookup"><span data-stu-id="38a75-230">fileVaultDisablePromptAtSignOut</span></span>|<span data-ttu-id="38a75-231">Boolean</span><span class="sxs-lookup"><span data-stu-id="38a75-231">Boolean</span></span>|<span data-ttu-id="38a75-232">可选。</span><span class="sxs-lookup"><span data-stu-id="38a75-232">Optional.</span></span> <span data-ttu-id="38a75-233">使用 Defer 选项时, 如果设置为 true, 则不提示用户在注销时启用 FileVault。</span><span class="sxs-lookup"><span data-stu-id="38a75-233">When using the Defer option, if set to true, the user is not prompted to enable FileVault at sign-out.</span></span>|
|<span data-ttu-id="38a75-234">fileVaultPersonalRecoveryKeyRotationInMonths</span><span class="sxs-lookup"><span data-stu-id="38a75-234">fileVaultPersonalRecoveryKeyRotationInMonths</span></span>|<span data-ttu-id="38a75-235">Int32</span><span class="sxs-lookup"><span data-stu-id="38a75-235">Int32</span></span>|<span data-ttu-id="38a75-236">可选。</span><span class="sxs-lookup"><span data-stu-id="38a75-236">Optional.</span></span> <span data-ttu-id="38a75-237">如果所选恢复密钥类型包括 PersonalRecoveryKey, 则以月为单位旋转该密钥的频率。</span><span class="sxs-lookup"><span data-stu-id="38a75-237">If selected recovery key type(s) include PersonalRecoveryKey, the frequency to rotate that key, in months.</span></span>|



## <a name="response"></a><span data-ttu-id="38a75-238">响应</span><span class="sxs-lookup"><span data-stu-id="38a75-238">Response</span></span>
<span data-ttu-id="38a75-239">如果成功, 此方法在响应`200 OK`正文中返回响应代码和更新的[macOSEndpointProtectionConfiguration](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="38a75-239">If successful, this method returns a `200 OK` response code and an updated [macOSEndpointProtectionConfiguration](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="38a75-240">示例</span><span class="sxs-lookup"><span data-stu-id="38a75-240">Example</span></span>

### <a name="request"></a><span data-ttu-id="38a75-241">请求</span><span class="sxs-lookup"><span data-stu-id="38a75-241">Request</span></span>
<span data-ttu-id="38a75-242">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="38a75-242">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 2052

{
  "@odata.type": "#microsoft.graph.macOSEndpointProtectionConfiguration",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "deviceManagementApplicabilityRuleOsEdition": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsEdition",
    "osEditionTypes": [
      "windows10EnterpriseN"
    ],
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleOsVersion": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsVersion",
    "minOSVersion": "Min OSVersion value",
    "maxOSVersion": "Max OSVersion value",
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleDeviceMode": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleDeviceMode",
    "deviceMode": "sModeConfiguration",
    "name": "Name value",
    "ruleType": "exclude"
  },
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "gatekeeperAllowedAppSource": "macAppStore",
  "gatekeeperBlockOverride": true,
  "firewallEnabled": true,
  "firewallBlockAllIncoming": true,
  "firewallEnableStealthMode": true,
  "firewallApplications": [
    {
      "@odata.type": "microsoft.graph.macOSFirewallApplication",
      "bundleId": "Bundle Id value",
      "allowsIncomingConnections": true
    }
  ],
  "fileVaultEnabled": true,
  "fileVaultSelectedRecoveryKeyTypes": "institutionalRecoveryKey",
  "fileVaultInstitutionalRecoveryKeyCertificate": "ZmlsZVZhdWx0SW5zdGl0dXRpb25hbFJlY292ZXJ5S2V5Q2VydGlmaWNhdGU=",
  "fileVaultInstitutionalRecoveryKeyCertificateFileName": "File Vault Institutional Recovery Key Certificate File Name value",
  "fileVaultPersonalRecoveryKeyHelpMessage": "File Vault Personal Recovery Key Help Message value",
  "fileVaultAllowDeferralUntilSignOut": true,
  "fileVaultNumberOfTimesUserCanIgnore": 3,
  "fileVaultDisablePromptAtSignOut": true,
  "fileVaultPersonalRecoveryKeyRotationInMonths": 12
}
```

### <a name="response"></a><span data-ttu-id="38a75-243">响应</span><span class="sxs-lookup"><span data-stu-id="38a75-243">Response</span></span>
<span data-ttu-id="38a75-p123">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="38a75-p123">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2224

{
  "@odata.type": "#microsoft.graph.macOSEndpointProtectionConfiguration",
  "id": "7bf7f3ca-f3ca-7bf7-caf3-f77bcaf3f77b",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "deviceManagementApplicabilityRuleOsEdition": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsEdition",
    "osEditionTypes": [
      "windows10EnterpriseN"
    ],
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleOsVersion": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsVersion",
    "minOSVersion": "Min OSVersion value",
    "maxOSVersion": "Max OSVersion value",
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleDeviceMode": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleDeviceMode",
    "deviceMode": "sModeConfiguration",
    "name": "Name value",
    "ruleType": "exclude"
  },
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "gatekeeperAllowedAppSource": "macAppStore",
  "gatekeeperBlockOverride": true,
  "firewallEnabled": true,
  "firewallBlockAllIncoming": true,
  "firewallEnableStealthMode": true,
  "firewallApplications": [
    {
      "@odata.type": "microsoft.graph.macOSFirewallApplication",
      "bundleId": "Bundle Id value",
      "allowsIncomingConnections": true
    }
  ],
  "fileVaultEnabled": true,
  "fileVaultSelectedRecoveryKeyTypes": "institutionalRecoveryKey",
  "fileVaultInstitutionalRecoveryKeyCertificate": "ZmlsZVZhdWx0SW5zdGl0dXRpb25hbFJlY292ZXJ5S2V5Q2VydGlmaWNhdGU=",
  "fileVaultInstitutionalRecoveryKeyCertificateFileName": "File Vault Institutional Recovery Key Certificate File Name value",
  "fileVaultPersonalRecoveryKeyHelpMessage": "File Vault Personal Recovery Key Help Message value",
  "fileVaultAllowDeferralUntilSignOut": true,
  "fileVaultNumberOfTimesUserCanIgnore": 3,
  "fileVaultDisablePromptAtSignOut": true,
  "fileVaultPersonalRecoveryKeyRotationInMonths": 12
}
```






