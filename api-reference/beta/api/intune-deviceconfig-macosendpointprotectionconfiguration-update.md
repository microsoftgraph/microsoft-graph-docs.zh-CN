---
title: 更新 macOSEndpointProtectionConfiguration
description: 更新 macOSEndpointProtectionConfiguration 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 501fe61b0a3b1edb355ae008991b8c4c6e8fef86
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49258302"
---
# <a name="update-macosendpointprotectionconfiguration"></a><span data-ttu-id="615fa-103">更新 macOSEndpointProtectionConfiguration</span><span class="sxs-lookup"><span data-stu-id="615fa-103">Update macOSEndpointProtectionConfiguration</span></span>

<span data-ttu-id="615fa-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="615fa-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="615fa-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="615fa-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="615fa-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="615fa-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="615fa-107">更新 [macOSEndpointProtectionConfiguration](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="615fa-107">Update the properties of a [macOSEndpointProtectionConfiguration](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="615fa-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="615fa-108">Prerequisites</span></span>
<span data-ttu-id="615fa-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="615fa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="615fa-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="615fa-111">Permission type</span></span>|<span data-ttu-id="615fa-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="615fa-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="615fa-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="615fa-113">Delegated (work or school account)</span></span>|<span data-ttu-id="615fa-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="615fa-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="615fa-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="615fa-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="615fa-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="615fa-116">Not supported.</span></span>|
|<span data-ttu-id="615fa-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="615fa-117">Application</span></span>|<span data-ttu-id="615fa-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="615fa-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="615fa-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="615fa-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="615fa-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="615fa-120">Request headers</span></span>
|<span data-ttu-id="615fa-121">标头</span><span class="sxs-lookup"><span data-stu-id="615fa-121">Header</span></span>|<span data-ttu-id="615fa-122">值</span><span class="sxs-lookup"><span data-stu-id="615fa-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="615fa-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="615fa-123">Authorization</span></span>|<span data-ttu-id="615fa-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="615fa-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="615fa-125">接受</span><span class="sxs-lookup"><span data-stu-id="615fa-125">Accept</span></span>|<span data-ttu-id="615fa-126">application/json</span><span class="sxs-lookup"><span data-stu-id="615fa-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="615fa-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="615fa-127">Request body</span></span>
<span data-ttu-id="615fa-128">在请求正文中，提供 [macOSEndpointProtectionConfiguration](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="615fa-128">In the request body, supply a JSON representation for the [macOSEndpointProtectionConfiguration](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md) object.</span></span>

<span data-ttu-id="615fa-129">下表显示创建 [macOSEndpointProtectionConfiguration](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="615fa-129">The following table shows the properties that are required when you create the [macOSEndpointProtectionConfiguration](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md).</span></span>

|<span data-ttu-id="615fa-130">属性</span><span class="sxs-lookup"><span data-stu-id="615fa-130">Property</span></span>|<span data-ttu-id="615fa-131">类型</span><span class="sxs-lookup"><span data-stu-id="615fa-131">Type</span></span>|<span data-ttu-id="615fa-132">说明</span><span class="sxs-lookup"><span data-stu-id="615fa-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="615fa-133">id</span><span class="sxs-lookup"><span data-stu-id="615fa-133">id</span></span>|<span data-ttu-id="615fa-134">String</span><span class="sxs-lookup"><span data-stu-id="615fa-134">String</span></span>|<span data-ttu-id="615fa-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="615fa-135">Key of the entity.</span></span> <span data-ttu-id="615fa-136">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="615fa-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="615fa-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="615fa-137">lastModifiedDateTime</span></span>|<span data-ttu-id="615fa-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="615fa-138">DateTimeOffset</span></span>|<span data-ttu-id="615fa-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="615fa-139">DateTime the object was last modified.</span></span> <span data-ttu-id="615fa-140">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="615fa-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="615fa-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="615fa-141">roleScopeTagIds</span></span>|<span data-ttu-id="615fa-142">String 集合</span><span class="sxs-lookup"><span data-stu-id="615fa-142">String collection</span></span>|<span data-ttu-id="615fa-143">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="615fa-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="615fa-144">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="615fa-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="615fa-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="615fa-145">supportsScopeTags</span></span>|<span data-ttu-id="615fa-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="615fa-146">Boolean</span></span>|<span data-ttu-id="615fa-147">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="615fa-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="615fa-148">如果此值为 false，则不允许分配给 ScopeTags 属性，并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="615fa-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="615fa-149">这适用于在 Silverlight 中创建的旧版策略，可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="615fa-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="615fa-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="615fa-150">This property is read-only.</span></span> <span data-ttu-id="615fa-151">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="615fa-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="615fa-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="615fa-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="615fa-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="615fa-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="615fa-154">适用于此策略的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="615fa-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="615fa-155">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="615fa-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="615fa-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="615fa-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="615fa-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="615fa-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="615fa-158">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="615fa-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="615fa-159">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="615fa-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="615fa-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="615fa-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="615fa-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="615fa-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="615fa-162">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="615fa-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="615fa-163">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="615fa-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="615fa-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="615fa-164">createdDateTime</span></span>|<span data-ttu-id="615fa-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="615fa-165">DateTimeOffset</span></span>|<span data-ttu-id="615fa-166">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="615fa-166">DateTime the object was created.</span></span> <span data-ttu-id="615fa-167">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="615fa-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="615fa-168">description</span><span class="sxs-lookup"><span data-stu-id="615fa-168">description</span></span>|<span data-ttu-id="615fa-169">String</span><span class="sxs-lookup"><span data-stu-id="615fa-169">String</span></span>|<span data-ttu-id="615fa-170">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="615fa-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="615fa-171">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="615fa-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="615fa-172">displayName</span><span class="sxs-lookup"><span data-stu-id="615fa-172">displayName</span></span>|<span data-ttu-id="615fa-173">String</span><span class="sxs-lookup"><span data-stu-id="615fa-173">String</span></span>|<span data-ttu-id="615fa-174">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="615fa-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="615fa-175">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="615fa-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="615fa-176">version</span><span class="sxs-lookup"><span data-stu-id="615fa-176">version</span></span>|<span data-ttu-id="615fa-177">Int32</span><span class="sxs-lookup"><span data-stu-id="615fa-177">Int32</span></span>|<span data-ttu-id="615fa-178">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="615fa-178">Version of the device configuration.</span></span> <span data-ttu-id="615fa-179">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="615fa-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="615fa-180">gatekeeperAllowedAppSource</span><span class="sxs-lookup"><span data-stu-id="615fa-180">gatekeeperAllowedAppSource</span></span>|[<span data-ttu-id="615fa-181">macOSGatekeeperAppSources</span><span class="sxs-lookup"><span data-stu-id="615fa-181">macOSGatekeeperAppSources</span></span>](../resources/intune-deviceconfig-macosgatekeeperappsources.md)|<span data-ttu-id="615fa-182">确定可以从 macOS 设备上运行哪些下载位置应用程序的系统和隐私设置。</span><span class="sxs-lookup"><span data-stu-id="615fa-182">System and Privacy setting that determines which download locations apps can be run from on a macOS device.</span></span> <span data-ttu-id="615fa-183">可取值为：`notConfigured`、`macAppStore`、`macAppStoreAndIdentifiedDevelopers`、`anywhere`。</span><span class="sxs-lookup"><span data-stu-id="615fa-183">Possible values are: `notConfigured`, `macAppStore`, `macAppStoreAndIdentifiedDevelopers`, `anywhere`.</span></span>|
|<span data-ttu-id="615fa-184">gatekeeperBlockOverride</span><span class="sxs-lookup"><span data-stu-id="615fa-184">gatekeeperBlockOverride</span></span>|<span data-ttu-id="615fa-185">Boolean</span><span class="sxs-lookup"><span data-stu-id="615fa-185">Boolean</span></span>|<span data-ttu-id="615fa-186">如果设置为 true，将禁用网关的用户替代。</span><span class="sxs-lookup"><span data-stu-id="615fa-186">If set to true, the user override for Gatekeeper will be disabled.</span></span>|
|<span data-ttu-id="615fa-187">firewallEnabled</span><span class="sxs-lookup"><span data-stu-id="615fa-187">firewallEnabled</span></span>|<span data-ttu-id="615fa-188">Boolean</span><span class="sxs-lookup"><span data-stu-id="615fa-188">Boolean</span></span>|<span data-ttu-id="615fa-189">是否应启用防火墙。</span><span class="sxs-lookup"><span data-stu-id="615fa-189">Whether the firewall should be enabled or not.</span></span>|
|<span data-ttu-id="615fa-190">firewallBlockAllIncoming</span><span class="sxs-lookup"><span data-stu-id="615fa-190">firewallBlockAllIncoming</span></span>|<span data-ttu-id="615fa-191">Boolean</span><span class="sxs-lookup"><span data-stu-id="615fa-191">Boolean</span></span>|<span data-ttu-id="615fa-192">对应于 "阻止所有传入连接" 选项。</span><span class="sxs-lookup"><span data-stu-id="615fa-192">Corresponds to the “Block all incoming connections” option.</span></span>|
|<span data-ttu-id="615fa-193">firewallEnableStealthMode</span><span class="sxs-lookup"><span data-stu-id="615fa-193">firewallEnableStealthMode</span></span>|<span data-ttu-id="615fa-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="615fa-194">Boolean</span></span>|<span data-ttu-id="615fa-195">对应于 "启用隐形模式"。</span><span class="sxs-lookup"><span data-stu-id="615fa-195">Corresponds to “Enable stealth mode.”</span></span>|
|<span data-ttu-id="615fa-196">firewallApplications</span><span class="sxs-lookup"><span data-stu-id="615fa-196">firewallApplications</span></span>|<span data-ttu-id="615fa-197">[macOSFirewallApplication](../resources/intune-deviceconfig-macosfirewallapplication.md) 集合</span><span class="sxs-lookup"><span data-stu-id="615fa-197">[macOSFirewallApplication](../resources/intune-deviceconfig-macosfirewallapplication.md) collection</span></span>|<span data-ttu-id="615fa-198">具有防火墙设置的应用程序列表。</span><span class="sxs-lookup"><span data-stu-id="615fa-198">List of applications with firewall settings.</span></span> <span data-ttu-id="615fa-199">不在此列表中的应用程序的防火墙设置由用户决定。</span><span class="sxs-lookup"><span data-stu-id="615fa-199">Firewall settings for applications not on this list are determined by the user.</span></span> <span data-ttu-id="615fa-200">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="615fa-200">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="615fa-201">fileVaultEnabled</span><span class="sxs-lookup"><span data-stu-id="615fa-201">fileVaultEnabled</span></span>|<span data-ttu-id="615fa-202">Boolean</span><span class="sxs-lookup"><span data-stu-id="615fa-202">Boolean</span></span>|<span data-ttu-id="615fa-203">是否应启用 FileVault。</span><span class="sxs-lookup"><span data-stu-id="615fa-203">Whether FileVault should be enabled or not.</span></span>|
|<span data-ttu-id="615fa-204">fileVaultSelectedRecoveryKeyTypes</span><span class="sxs-lookup"><span data-stu-id="615fa-204">fileVaultSelectedRecoveryKeyTypes</span></span>|[<span data-ttu-id="615fa-205">macOSFileVaultRecoveryKeyTypes</span><span class="sxs-lookup"><span data-stu-id="615fa-205">macOSFileVaultRecoveryKeyTypes</span></span>](../resources/intune-deviceconfig-macosfilevaultrecoverykeytypes.md)|<span data-ttu-id="615fa-206">必需如果启用了 FileVault，则确定要使用的恢复密钥) 类型 (s。</span><span class="sxs-lookup"><span data-stu-id="615fa-206">Required if FileVault is enabled, determines the type(s) of recovery key to use.</span></span> <span data-ttu-id="615fa-207">.</span><span class="sxs-lookup"><span data-stu-id="615fa-207">.</span></span> <span data-ttu-id="615fa-208">可取值为：`notConfigured`、`institutionalRecoveryKey`、`personalRecoveryKey`。</span><span class="sxs-lookup"><span data-stu-id="615fa-208">Possible values are: `notConfigured`, `institutionalRecoveryKey`, `personalRecoveryKey`.</span></span>|
|<span data-ttu-id="615fa-209">fileVaultInstitutionalRecoveryKeyCertificate</span><span class="sxs-lookup"><span data-stu-id="615fa-209">fileVaultInstitutionalRecoveryKeyCertificate</span></span>|<span data-ttu-id="615fa-210">Binary</span><span class="sxs-lookup"><span data-stu-id="615fa-210">Binary</span></span>|<span data-ttu-id="615fa-211">如果所选恢复密钥类型 (s) 包含 InstitutionalRecoveryKey，则是必需的。</span><span class="sxs-lookup"><span data-stu-id="615fa-211">Required if selected recovery key type(s) include InstitutionalRecoveryKey.</span></span> <span data-ttu-id="615fa-212">用于设置机构恢复密钥的 DER 编码证书文件。</span><span class="sxs-lookup"><span data-stu-id="615fa-212">The DER Encoded certificate file used to set an institutional recovery key.</span></span>|
|<span data-ttu-id="615fa-213">fileVaultInstitutionalRecoveryKeyCertificateFileName</span><span class="sxs-lookup"><span data-stu-id="615fa-213">fileVaultInstitutionalRecoveryKeyCertificateFileName</span></span>|<span data-ttu-id="615fa-214">String</span><span class="sxs-lookup"><span data-stu-id="615fa-214">String</span></span>|<span data-ttu-id="615fa-215">要在 UI 中显示的机构恢复密钥证书的文件名。</span><span class="sxs-lookup"><span data-stu-id="615fa-215">File name of the institutional recovery key certificate to display in UI.</span></span> <span data-ttu-id="615fa-216"> (\ * der) 。</span><span class="sxs-lookup"><span data-stu-id="615fa-216">(\*.der).</span></span>|
|<span data-ttu-id="615fa-217">fileVaultPersonalRecoveryKeyHelpMessage</span><span class="sxs-lookup"><span data-stu-id="615fa-217">fileVaultPersonalRecoveryKeyHelpMessage</span></span>|<span data-ttu-id="615fa-218">String</span><span class="sxs-lookup"><span data-stu-id="615fa-218">String</span></span>|<span data-ttu-id="615fa-219">如果所选恢复密钥类型 (s) 包含 PersonalRecoveryKey，则是必需的。</span><span class="sxs-lookup"><span data-stu-id="615fa-219">Required if selected recovery key type(s) include PersonalRecoveryKey.</span></span> <span data-ttu-id="615fa-220">向用户显示一条简短消息，说明他们如何检索其个人恢复密钥。</span><span class="sxs-lookup"><span data-stu-id="615fa-220">A short message displayed to the user that explains how they can retrieve their personal recovery key.</span></span>|
|<span data-ttu-id="615fa-221">fileVaultAllowDeferralUntilSignOut</span><span class="sxs-lookup"><span data-stu-id="615fa-221">fileVaultAllowDeferralUntilSignOut</span></span>|<span data-ttu-id="615fa-222">Boolean</span><span class="sxs-lookup"><span data-stu-id="615fa-222">Boolean</span></span>|<span data-ttu-id="615fa-223">可选。</span><span class="sxs-lookup"><span data-stu-id="615fa-223">Optional.</span></span> <span data-ttu-id="615fa-224">如果设置为 true，则用户可以推迟启用 FileVault，直到他们注销。</span><span class="sxs-lookup"><span data-stu-id="615fa-224">If set to true, the user can defer the enabling of FileVault until they sign out.</span></span>|
|<span data-ttu-id="615fa-225">fileVaultNumberOfTimesUserCanIgnore</span><span class="sxs-lookup"><span data-stu-id="615fa-225">fileVaultNumberOfTimesUserCanIgnore</span></span>|<span data-ttu-id="615fa-226">Int32</span><span class="sxs-lookup"><span data-stu-id="615fa-226">Int32</span></span>|<span data-ttu-id="615fa-227">可选。</span><span class="sxs-lookup"><span data-stu-id="615fa-227">Optional.</span></span> <span data-ttu-id="615fa-228">使用 Defer 选项时，此值是用户可以在 FileVault 之前忽略启用 FileVault 的提示的最大次数，用户将需要这些用户才能登录。</span><span class="sxs-lookup"><span data-stu-id="615fa-228">When using the Defer option, this is the maximum number of times the user can ignore prompts to enable FileVault before FileVault will be required for the user to sign in.</span></span> <span data-ttu-id="615fa-229">如果设置为-1，则在启用 FileVault 之前，它将始终提示启用 FileVault，但它将允许用户绕过启用 FileVault。</span><span class="sxs-lookup"><span data-stu-id="615fa-229">If set to -1, it will always prompt to enable FileVault until FileVault is enabled, though it will allow the user to bypass enabling FileVault.</span></span> <span data-ttu-id="615fa-230">将此设置为0将禁用该功能。</span><span class="sxs-lookup"><span data-stu-id="615fa-230">Setting this to 0 will disable the feature.</span></span>|
|<span data-ttu-id="615fa-231">fileVaultDisablePromptAtSignOut</span><span class="sxs-lookup"><span data-stu-id="615fa-231">fileVaultDisablePromptAtSignOut</span></span>|<span data-ttu-id="615fa-232">Boolean</span><span class="sxs-lookup"><span data-stu-id="615fa-232">Boolean</span></span>|<span data-ttu-id="615fa-233">可选。</span><span class="sxs-lookup"><span data-stu-id="615fa-233">Optional.</span></span> <span data-ttu-id="615fa-234">使用 Defer 选项时，如果设置为 true，则不提示用户在注销时启用 FileVault。</span><span class="sxs-lookup"><span data-stu-id="615fa-234">When using the Defer option, if set to true, the user is not prompted to enable FileVault at sign-out.</span></span>|
|<span data-ttu-id="615fa-235">fileVaultPersonalRecoveryKeyRotationInMonths</span><span class="sxs-lookup"><span data-stu-id="615fa-235">fileVaultPersonalRecoveryKeyRotationInMonths</span></span>|<span data-ttu-id="615fa-236">Int32</span><span class="sxs-lookup"><span data-stu-id="615fa-236">Int32</span></span>|<span data-ttu-id="615fa-237">可选。</span><span class="sxs-lookup"><span data-stu-id="615fa-237">Optional.</span></span> <span data-ttu-id="615fa-238">如果所选恢复密钥类型 (s) 包含 PersonalRecoveryKey，则以月为单位旋转该密钥的频率。</span><span class="sxs-lookup"><span data-stu-id="615fa-238">If selected recovery key type(s) include PersonalRecoveryKey, the frequency to rotate that key, in months.</span></span>|
|<span data-ttu-id="615fa-239">fileVaultHidePersonalRecoveryKey</span><span class="sxs-lookup"><span data-stu-id="615fa-239">fileVaultHidePersonalRecoveryKey</span></span>|<span data-ttu-id="615fa-240">Boolean</span><span class="sxs-lookup"><span data-stu-id="615fa-240">Boolean</span></span>|<span data-ttu-id="615fa-241">可选。</span><span class="sxs-lookup"><span data-stu-id="615fa-241">Optional.</span></span> <span data-ttu-id="615fa-242">在 FileVault 加密过程中，隐藏的个人恢复密钥不会显示在用户的屏幕上，从而降低了在错误的手中出现的最终风险。</span><span class="sxs-lookup"><span data-stu-id="615fa-242">A hidden personal recovery key does not appear on the user's screen during FileVault encryption, reducing the risk of it ending up in the wrong hands.</span></span>|
|<span data-ttu-id="615fa-243">advancedThreatProtectionRealTime</span><span class="sxs-lookup"><span data-stu-id="615fa-243">advancedThreatProtectionRealTime</span></span>|[<span data-ttu-id="615fa-244">启用</span><span class="sxs-lookup"><span data-stu-id="615fa-244">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="615fa-245">确定是否在 macOS 上为 Microsoft Defender 高级威胁防护启用实时保护。</span><span class="sxs-lookup"><span data-stu-id="615fa-245">Determines whether or not to enable real-time protection for Microsoft Defender Advanced Threat Protection on macOS.</span></span> <span data-ttu-id="615fa-246">可取值为：`notConfigured`、`enabled`、`disabled`。</span><span class="sxs-lookup"><span data-stu-id="615fa-246">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="615fa-247">advancedThreatProtectionCloudDelivered</span><span class="sxs-lookup"><span data-stu-id="615fa-247">advancedThreatProtectionCloudDelivered</span></span>|[<span data-ttu-id="615fa-248">启用</span><span class="sxs-lookup"><span data-stu-id="615fa-248">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="615fa-249">确定是否在 macOS 上为 Microsoft Defender 高级威胁防护启用云提供的保护。</span><span class="sxs-lookup"><span data-stu-id="615fa-249">Determines whether or not to enable cloud-delivered protection for Microsoft Defender Advanced Threat Protection on macOS.</span></span> <span data-ttu-id="615fa-250">可取值为：`notConfigured`、`enabled`、`disabled`。</span><span class="sxs-lookup"><span data-stu-id="615fa-250">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="615fa-251">advancedThreatProtectionAutomaticSampleSubmission</span><span class="sxs-lookup"><span data-stu-id="615fa-251">advancedThreatProtectionAutomaticSampleSubmission</span></span>|[<span data-ttu-id="615fa-252">启用</span><span class="sxs-lookup"><span data-stu-id="615fa-252">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="615fa-253">确定是否在 macOS 上为 Microsoft Defender 高级威胁防护启用自动文件示例提交。</span><span class="sxs-lookup"><span data-stu-id="615fa-253">Determines whether or not to enable automatic file sample submission for Microsoft Defender Advanced Threat Protection on macOS.</span></span> <span data-ttu-id="615fa-254">可取值为：`notConfigured`、`enabled`、`disabled`。</span><span class="sxs-lookup"><span data-stu-id="615fa-254">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="615fa-255">advancedThreatProtectionDiagnosticDataCollection</span><span class="sxs-lookup"><span data-stu-id="615fa-255">advancedThreatProtectionDiagnosticDataCollection</span></span>|[<span data-ttu-id="615fa-256">启用</span><span class="sxs-lookup"><span data-stu-id="615fa-256">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="615fa-257">确定是否在 macOS 上为 Microsoft Defender 高级威胁防护启用诊断和使用情况数据收集。</span><span class="sxs-lookup"><span data-stu-id="615fa-257">Determines whether or not to enable diagnostic and usage data collection for Microsoft Defender Advanced Threat Protection on macOS.</span></span> <span data-ttu-id="615fa-258">可取值为：`notConfigured`、`enabled`、`disabled`。</span><span class="sxs-lookup"><span data-stu-id="615fa-258">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="615fa-259">advancedThreatProtectionExcludedFolders</span><span class="sxs-lookup"><span data-stu-id="615fa-259">advancedThreatProtectionExcludedFolders</span></span>|<span data-ttu-id="615fa-260">String 集合</span><span class="sxs-lookup"><span data-stu-id="615fa-260">String collection</span></span>|<span data-ttu-id="615fa-261">要从 macOS 的 Microsoft Defender 高级威胁防护的防病毒扫描中排除的文件夹路径的列表。</span><span class="sxs-lookup"><span data-stu-id="615fa-261">A list of paths to folders to exclude from antivirus scanning for Microsoft Defender Advanced Threat Protection on macOS.</span></span>|
|<span data-ttu-id="615fa-262">advancedThreatProtectionExcludedFiles</span><span class="sxs-lookup"><span data-stu-id="615fa-262">advancedThreatProtectionExcludedFiles</span></span>|<span data-ttu-id="615fa-263">String 集合</span><span class="sxs-lookup"><span data-stu-id="615fa-263">String collection</span></span>|<span data-ttu-id="615fa-264">要从 macOS 中的 Microsoft Defender 高级威胁防护的防病毒扫描中排除的文件的路径列表。</span><span class="sxs-lookup"><span data-stu-id="615fa-264">A list of paths to files to exclude from antivirus scanning for Microsoft Defender Advanced Threat Protection on macOS.</span></span>|
|<span data-ttu-id="615fa-265">advancedThreatProtectionExcludedExtensions</span><span class="sxs-lookup"><span data-stu-id="615fa-265">advancedThreatProtectionExcludedExtensions</span></span>|<span data-ttu-id="615fa-266">String 集合</span><span class="sxs-lookup"><span data-stu-id="615fa-266">String collection</span></span>|<span data-ttu-id="615fa-267">要从 macOS 中的 Microsoft Defender 高级威胁防护的防病毒扫描中排除的文件扩展名的列表。</span><span class="sxs-lookup"><span data-stu-id="615fa-267">A list of file extensions to exclude from antivirus scanning for Microsoft Defender Advanced Threat Protection on macOS.</span></span>|
|<span data-ttu-id="615fa-268">advancedThreatProtectionExcludedProcesses</span><span class="sxs-lookup"><span data-stu-id="615fa-268">advancedThreatProtectionExcludedProcesses</span></span>|<span data-ttu-id="615fa-269">String 集合</span><span class="sxs-lookup"><span data-stu-id="615fa-269">String collection</span></span>|<span data-ttu-id="615fa-270">要从 macOS 中的 Microsoft Defender 高级威胁防护的防病毒扫描中排除的进程名称的列表。</span><span class="sxs-lookup"><span data-stu-id="615fa-270">A list of process names to exclude from antivirus scanning for Microsoft Defender Advanced Threat Protection on macOS.</span></span>|



## <a name="response"></a><span data-ttu-id="615fa-271">响应</span><span class="sxs-lookup"><span data-stu-id="615fa-271">Response</span></span>
<span data-ttu-id="615fa-272">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和更新的 [macOSEndpointProtectionConfiguration](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="615fa-272">If successful, this method returns a `200 OK` response code and an updated [macOSEndpointProtectionConfiguration](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="615fa-273">示例</span><span class="sxs-lookup"><span data-stu-id="615fa-273">Example</span></span>

### <a name="request"></a><span data-ttu-id="615fa-274">请求</span><span class="sxs-lookup"><span data-stu-id="615fa-274">Request</span></span>
<span data-ttu-id="615fa-275">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="615fa-275">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 2786

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
  "fileVaultPersonalRecoveryKeyRotationInMonths": 12,
  "fileVaultHidePersonalRecoveryKey": true,
  "advancedThreatProtectionRealTime": "enabled",
  "advancedThreatProtectionCloudDelivered": "enabled",
  "advancedThreatProtectionAutomaticSampleSubmission": "enabled",
  "advancedThreatProtectionDiagnosticDataCollection": "enabled",
  "advancedThreatProtectionExcludedFolders": [
    "Advanced Threat Protection Excluded Folders value"
  ],
  "advancedThreatProtectionExcludedFiles": [
    "Advanced Threat Protection Excluded Files value"
  ],
  "advancedThreatProtectionExcludedExtensions": [
    "Advanced Threat Protection Excluded Extensions value"
  ],
  "advancedThreatProtectionExcludedProcesses": [
    "Advanced Threat Protection Excluded Processes value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="615fa-276">响应</span><span class="sxs-lookup"><span data-stu-id="615fa-276">Response</span></span>
<span data-ttu-id="615fa-p128">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="615fa-p128">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2958

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
  "fileVaultPersonalRecoveryKeyRotationInMonths": 12,
  "fileVaultHidePersonalRecoveryKey": true,
  "advancedThreatProtectionRealTime": "enabled",
  "advancedThreatProtectionCloudDelivered": "enabled",
  "advancedThreatProtectionAutomaticSampleSubmission": "enabled",
  "advancedThreatProtectionDiagnosticDataCollection": "enabled",
  "advancedThreatProtectionExcludedFolders": [
    "Advanced Threat Protection Excluded Folders value"
  ],
  "advancedThreatProtectionExcludedFiles": [
    "Advanced Threat Protection Excluded Files value"
  ],
  "advancedThreatProtectionExcludedExtensions": [
    "Advanced Threat Protection Excluded Extensions value"
  ],
  "advancedThreatProtectionExcludedProcesses": [
    "Advanced Threat Protection Excluded Processes value"
  ]
}
```




