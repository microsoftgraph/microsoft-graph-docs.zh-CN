---
title: 更新 windows10EndpointProtectionConfiguration
description: 更新 windows10EndpointProtectionConfiguration 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 0a46dd9dfa046ad638f6c0518442324809324828
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51147488"
---
# <a name="update-windows10endpointprotectionconfiguration"></a><span data-ttu-id="22833-103">更新 windows10EndpointProtectionConfiguration</span><span class="sxs-lookup"><span data-stu-id="22833-103">Update windows10EndpointProtectionConfiguration</span></span>

<span data-ttu-id="22833-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="22833-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="22833-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="22833-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="22833-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="22833-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="22833-107">更新 [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="22833-107">Update the properties of a [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="22833-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="22833-108">Prerequisites</span></span>
<span data-ttu-id="22833-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="22833-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="22833-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="22833-111">Permission type</span></span>|<span data-ttu-id="22833-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="22833-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="22833-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="22833-113">Delegated (work or school account)</span></span>|<span data-ttu-id="22833-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="22833-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="22833-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="22833-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="22833-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="22833-116">Not supported.</span></span>|
|<span data-ttu-id="22833-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="22833-117">Application</span></span>|<span data-ttu-id="22833-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="22833-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="22833-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="22833-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="22833-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="22833-120">Request headers</span></span>
|<span data-ttu-id="22833-121">标头</span><span class="sxs-lookup"><span data-stu-id="22833-121">Header</span></span>|<span data-ttu-id="22833-122">值</span><span class="sxs-lookup"><span data-stu-id="22833-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="22833-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="22833-123">Authorization</span></span>|<span data-ttu-id="22833-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="22833-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="22833-125">接受</span><span class="sxs-lookup"><span data-stu-id="22833-125">Accept</span></span>|<span data-ttu-id="22833-126">application/json</span><span class="sxs-lookup"><span data-stu-id="22833-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="22833-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="22833-127">Request body</span></span>
<span data-ttu-id="22833-128">在请求正文中，提供 [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="22833-128">In the request body, supply a JSON representation for the [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) object.</span></span>

<span data-ttu-id="22833-129">下表显示了创建 [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="22833-129">The following table shows the properties that are required when you create the [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md).</span></span>

|<span data-ttu-id="22833-130">属性</span><span class="sxs-lookup"><span data-stu-id="22833-130">Property</span></span>|<span data-ttu-id="22833-131">类型</span><span class="sxs-lookup"><span data-stu-id="22833-131">Type</span></span>|<span data-ttu-id="22833-132">说明</span><span class="sxs-lookup"><span data-stu-id="22833-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="22833-133">id</span><span class="sxs-lookup"><span data-stu-id="22833-133">id</span></span>|<span data-ttu-id="22833-134">String</span><span class="sxs-lookup"><span data-stu-id="22833-134">String</span></span>|<span data-ttu-id="22833-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="22833-135">Key of the entity.</span></span> <span data-ttu-id="22833-136">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="22833-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="22833-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="22833-137">lastModifiedDateTime</span></span>|<span data-ttu-id="22833-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="22833-138">DateTimeOffset</span></span>|<span data-ttu-id="22833-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="22833-139">DateTime the object was last modified.</span></span> <span data-ttu-id="22833-140">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="22833-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="22833-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="22833-141">roleScopeTagIds</span></span>|<span data-ttu-id="22833-142">String collection</span><span class="sxs-lookup"><span data-stu-id="22833-142">String collection</span></span>|<span data-ttu-id="22833-143">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="22833-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="22833-144">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="22833-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="22833-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="22833-145">supportsScopeTags</span></span>|<span data-ttu-id="22833-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="22833-146">Boolean</span></span>|<span data-ttu-id="22833-147">指示基础设备配置是否支持分配范围标记。</span><span class="sxs-lookup"><span data-stu-id="22833-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="22833-148">当此值为 false 且实体对作用域用户不可见时，不允许分配给 ScopeTags 属性。</span><span class="sxs-lookup"><span data-stu-id="22833-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="22833-149">这适用于在 Silverlight 中创建的旧版策略，可通过在 Azure 门户中删除和重新创建策略来解决。</span><span class="sxs-lookup"><span data-stu-id="22833-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="22833-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="22833-150">This property is read-only.</span></span> <span data-ttu-id="22833-151">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="22833-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="22833-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="22833-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="22833-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="22833-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="22833-154">此策略的操作系统版本适用性。</span><span class="sxs-lookup"><span data-stu-id="22833-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="22833-155">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="22833-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="22833-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="22833-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="22833-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="22833-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="22833-158">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="22833-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="22833-159">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="22833-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="22833-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="22833-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="22833-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="22833-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="22833-162">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="22833-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="22833-163">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="22833-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="22833-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="22833-164">createdDateTime</span></span>|<span data-ttu-id="22833-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="22833-165">DateTimeOffset</span></span>|<span data-ttu-id="22833-166">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="22833-166">DateTime the object was created.</span></span> <span data-ttu-id="22833-167">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="22833-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="22833-168">说明</span><span class="sxs-lookup"><span data-stu-id="22833-168">description</span></span>|<span data-ttu-id="22833-169">String</span><span class="sxs-lookup"><span data-stu-id="22833-169">String</span></span>|<span data-ttu-id="22833-170">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="22833-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="22833-171">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="22833-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="22833-172">displayName</span><span class="sxs-lookup"><span data-stu-id="22833-172">displayName</span></span>|<span data-ttu-id="22833-173">String</span><span class="sxs-lookup"><span data-stu-id="22833-173">String</span></span>|<span data-ttu-id="22833-174">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="22833-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="22833-175">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="22833-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="22833-176">version</span><span class="sxs-lookup"><span data-stu-id="22833-176">version</span></span>|<span data-ttu-id="22833-177">Int32</span><span class="sxs-lookup"><span data-stu-id="22833-177">Int32</span></span>|<span data-ttu-id="22833-178">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="22833-178">Version of the device configuration.</span></span> <span data-ttu-id="22833-179">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="22833-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="22833-180">dmaGuardDeviceEnumerationPolicy</span><span class="sxs-lookup"><span data-stu-id="22833-180">dmaGuardDeviceEnumerationPolicy</span></span>|[<span data-ttu-id="22833-181">dmaGuardDeviceEnumerationPolicyType</span><span class="sxs-lookup"><span data-stu-id="22833-181">dmaGuardDeviceEnumerationPolicyType</span></span>](../resources/intune-deviceconfig-dmaguarddeviceenumerationpolicytype.md)|<span data-ttu-id="22833-182">此策略旨在针对支持外部 DMA 的设备提供额外的安全性。</span><span class="sxs-lookup"><span data-stu-id="22833-182">This policy is intended to provide additional security against external DMA capable devices.</span></span> <span data-ttu-id="22833-183">它允许对与 DMA 重新映射/设备内存隔离和沙盒不兼容的外部支持 DMA 的设备枚举进行更多控制。</span><span class="sxs-lookup"><span data-stu-id="22833-183">It allows for more control over the enumeration of external DMA capable devices incompatible with DMA Remapping/device memory isolation and sandboxing.</span></span> <span data-ttu-id="22833-184">此策略仅在系统固件支持并启用内核 DMA 保护时生效。</span><span class="sxs-lookup"><span data-stu-id="22833-184">This policy only takes effect when Kernel DMA Protection is supported and enabled by the system firmware.</span></span> <span data-ttu-id="22833-185">内核 DMA 保护是一项平台功能，无法通过策略或最终用户控制。</span><span class="sxs-lookup"><span data-stu-id="22833-185">Kernel DMA Protection is a platform feature that cannot be controlled via policy or by end user.</span></span> <span data-ttu-id="22833-186">它在制造时必须受系统支持。</span><span class="sxs-lookup"><span data-stu-id="22833-186">It has to be supported by the system at the time of manufacturing.</span></span> <span data-ttu-id="22833-187">若要检查系统是否支持内核 DMA 保护，请检查内核 DMA 保护字段，在 MSINFO32.exe 的摘要页中。</span><span class="sxs-lookup"><span data-stu-id="22833-187">To check if the system supports Kernel DMA Protection, please check the Kernel DMA Protection field in the Summary page of MSINFO32.exe.</span></span> <span data-ttu-id="22833-188">可取值为：`deviceDefault`、`blockAll`、`allowAll`。</span><span class="sxs-lookup"><span data-stu-id="22833-188">Possible values are: `deviceDefault`, `blockAll`, `allowAll`.</span></span>|
|<span data-ttu-id="22833-189">firewallRules</span><span class="sxs-lookup"><span data-stu-id="22833-189">firewallRules</span></span>|<span data-ttu-id="22833-190">[windowsFirewallRule](../resources/intune-deviceconfig-windowsfirewallrule.md) 集合</span><span class="sxs-lookup"><span data-stu-id="22833-190">[windowsFirewallRule](../resources/intune-deviceconfig-windowsfirewallrule.md) collection</span></span>|<span data-ttu-id="22833-191">配置防火墙规则设置。</span><span class="sxs-lookup"><span data-stu-id="22833-191">Configures the firewall rule settings.</span></span> <span data-ttu-id="22833-192">此集合最多可包含 150 个元素。</span><span class="sxs-lookup"><span data-stu-id="22833-192">This collection can contain a maximum of 150 elements.</span></span>|
|<span data-ttu-id="22833-193">userRightsAccessCredentialManagerAsTrustedCaller</span><span class="sxs-lookup"><span data-stu-id="22833-193">userRightsAccessCredentialManagerAsTrustedCaller</span></span>|[<span data-ttu-id="22833-194">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="22833-194">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="22833-195">此用户权限在备份/还原期间由凭据管理器使用。</span><span class="sxs-lookup"><span data-stu-id="22833-195">This user right is used by Credential Manager during Backup/Restore.</span></span> <span data-ttu-id="22833-196">如果向其他实体授予此权限，则用户保存的凭据可能会泄露。</span><span class="sxs-lookup"><span data-stu-id="22833-196">Users' saved credentials might be compromised if this privilege is given to other entities.</span></span> <span data-ttu-id="22833-197">仅支持状态 NotConfigured 和 Allowed</span><span class="sxs-lookup"><span data-stu-id="22833-197">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="22833-198">userRightsAllowAccessFromNetwork</span><span class="sxs-lookup"><span data-stu-id="22833-198">userRightsAllowAccessFromNetwork</span></span>|[<span data-ttu-id="22833-199">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="22833-199">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="22833-200">此用户权限确定允许哪些用户和组通过网络连接到计算机。</span><span class="sxs-lookup"><span data-stu-id="22833-200">This user right determines which users and groups are allowed to connect to the computer over the network.</span></span> <span data-ttu-id="22833-201">支持允许的状态。</span><span class="sxs-lookup"><span data-stu-id="22833-201">State Allowed is supported.</span></span>|
|<span data-ttu-id="22833-202">userRightsBlockAccessFromNetwork</span><span class="sxs-lookup"><span data-stu-id="22833-202">userRightsBlockAccessFromNetwork</span></span>|[<span data-ttu-id="22833-203">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="22833-203">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="22833-204">此用户权限确定阻止哪些用户和组通过网络连接到计算机。</span><span class="sxs-lookup"><span data-stu-id="22833-204">This user right determines which users and groups are block from connecting to the computer over the network.</span></span> <span data-ttu-id="22833-205">支持状态块。</span><span class="sxs-lookup"><span data-stu-id="22833-205">State Block is supported.</span></span>|
|<span data-ttu-id="22833-206">userRightsActAsPartOfTheOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="22833-206">userRightsActAsPartOfTheOperatingSystem</span></span>|[<span data-ttu-id="22833-207">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="22833-207">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="22833-208">此用户权限允许进程模拟任何用户而不进行身份验证。</span><span class="sxs-lookup"><span data-stu-id="22833-208">This user right allows a process to impersonate any user without authentication.</span></span> <span data-ttu-id="22833-209">因此，该过程可以获得与该用户相同的本地资源的访问权限。</span><span class="sxs-lookup"><span data-stu-id="22833-209">The process can therefore gain access to the same local resources as that user.</span></span> <span data-ttu-id="22833-210">仅支持状态 NotConfigured 和 Allowed</span><span class="sxs-lookup"><span data-stu-id="22833-210">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="22833-211">userRightsLocalLogOn</span><span class="sxs-lookup"><span data-stu-id="22833-211">userRightsLocalLogOn</span></span>|[<span data-ttu-id="22833-212">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="22833-212">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="22833-213">此用户权限确定哪些用户可以登录到计算机。</span><span class="sxs-lookup"><span data-stu-id="22833-213">This user right determines which users can log on to the computer.</span></span> <span data-ttu-id="22833-214">支持状态 NotConfigured、Allowed</span><span class="sxs-lookup"><span data-stu-id="22833-214">States NotConfigured, Allowed are supported</span></span> |
|<span data-ttu-id="22833-215">userRightsDenyLocalLogOn</span><span class="sxs-lookup"><span data-stu-id="22833-215">userRightsDenyLocalLogOn</span></span>|[<span data-ttu-id="22833-216">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="22833-216">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="22833-217">此用户权限确定哪些用户无法登录计算机。</span><span class="sxs-lookup"><span data-stu-id="22833-217">This user right determines which users cannot log on to the computer.</span></span> <span data-ttu-id="22833-218">状态 NotConfigured、Blocked 受支持</span><span class="sxs-lookup"><span data-stu-id="22833-218">States NotConfigured, Blocked are supported</span></span> |
|<span data-ttu-id="22833-219">userRightsBackupData</span><span class="sxs-lookup"><span data-stu-id="22833-219">userRightsBackupData</span></span>|[<span data-ttu-id="22833-220">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="22833-220">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="22833-221">此用户权限确定哪些用户在备份文件和目录时可以绕过文件、目录、注册表和其他永久对象权限。</span><span class="sxs-lookup"><span data-stu-id="22833-221">This user right determines which users can bypass file, directory, registry, and other persistent objects permissions when backing up files and directories.</span></span> <span data-ttu-id="22833-222">仅支持状态 NotConfigured 和 Allowed</span><span class="sxs-lookup"><span data-stu-id="22833-222">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="22833-223">userRightsChangeSystemTime</span><span class="sxs-lookup"><span data-stu-id="22833-223">userRightsChangeSystemTime</span></span>|[<span data-ttu-id="22833-224">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="22833-224">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="22833-225">此用户权限确定哪些用户和组可以更改计算机内部时钟的时间和日期。</span><span class="sxs-lookup"><span data-stu-id="22833-225">This user right determines which users and groups can change the time and date on the internal clock of the computer.</span></span> <span data-ttu-id="22833-226">仅支持状态 NotConfigured 和 Allowed</span><span class="sxs-lookup"><span data-stu-id="22833-226">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="22833-227">userRightsCreateGlobalObjects</span><span class="sxs-lookup"><span data-stu-id="22833-227">userRightsCreateGlobalObjects</span></span>|[<span data-ttu-id="22833-228">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="22833-228">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="22833-229">此安全性设置确定用户能否创建可用于所有会话的全局对象。</span><span class="sxs-lookup"><span data-stu-id="22833-229">This security setting determines whether users can create global objects that are available to all sessions.</span></span> <span data-ttu-id="22833-230">可以创建全局对象的用户可能会影响在其他用户的会话下运行的进程，这可能会导致应用程序失败或数据损坏。</span><span class="sxs-lookup"><span data-stu-id="22833-230">Users who can create global objects could affect processes that run under other users' sessions, which could lead to application failure or data corruption.</span></span> <span data-ttu-id="22833-231">仅支持状态 NotConfigured 和 Allowed</span><span class="sxs-lookup"><span data-stu-id="22833-231">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="22833-232">userRightsCreatePageFile</span><span class="sxs-lookup"><span data-stu-id="22833-232">userRightsCreatePageFile</span></span>|[<span data-ttu-id="22833-233">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="22833-233">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="22833-234">此用户权限确定哪些用户和组可以调用内部 API 来创建和更改页面文件的大小。</span><span class="sxs-lookup"><span data-stu-id="22833-234">This user right determines which users and groups can call an internal API to create and change the size of a page file.</span></span> <span data-ttu-id="22833-235">仅支持状态 NotConfigured 和 Allowed</span><span class="sxs-lookup"><span data-stu-id="22833-235">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="22833-236">userRightsCreatePermanentSharedObjects</span><span class="sxs-lookup"><span data-stu-id="22833-236">userRightsCreatePermanentSharedObjects</span></span>|[<span data-ttu-id="22833-237">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="22833-237">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="22833-238">此用户权限确定进程可以使用哪些帐户来创建使用对象管理器的目录对象。</span><span class="sxs-lookup"><span data-stu-id="22833-238">This user right determines which accounts can be used by processes to create a directory object using the object manager.</span></span> <span data-ttu-id="22833-239">仅支持状态 NotConfigured 和 Allowed</span><span class="sxs-lookup"><span data-stu-id="22833-239">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="22833-240">userRightsCreateSymb创建Links</span><span class="sxs-lookup"><span data-stu-id="22833-240">userRightsCreateSymbolicLinks</span></span>|[<span data-ttu-id="22833-241">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="22833-241">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="22833-242">此用户权限确定用户能否从登录的计算机创建符号链接。</span><span class="sxs-lookup"><span data-stu-id="22833-242">This user right determines if the user can create a symbolic link from the computer to which they are logged on.</span></span> <span data-ttu-id="22833-243">仅支持状态 NotConfigured 和 Allowed</span><span class="sxs-lookup"><span data-stu-id="22833-243">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="22833-244">userRightsCreateToken</span><span class="sxs-lookup"><span data-stu-id="22833-244">userRightsCreateToken</span></span>|[<span data-ttu-id="22833-245">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="22833-245">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="22833-246">此用户权限确定进程可以使用哪些用户/组来创建令牌，然后当进程使用内部 API 创建访问令牌时，该令牌可用于获取任何本地资源的访问权限。</span><span class="sxs-lookup"><span data-stu-id="22833-246">This user right determines which users/groups can be used by processes to create a token that can then be used to get access to any local resources when the process uses an internal API to create an access token.</span></span> <span data-ttu-id="22833-247">仅支持状态 NotConfigured 和 Allowed</span><span class="sxs-lookup"><span data-stu-id="22833-247">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="22833-248">userRightsDebugPrograms</span><span class="sxs-lookup"><span data-stu-id="22833-248">userRightsDebugPrograms</span></span>|[<span data-ttu-id="22833-249">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="22833-249">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="22833-250">此用户权限确定哪些用户可以将调试器附加到任何进程或内核。</span><span class="sxs-lookup"><span data-stu-id="22833-250">This user right determines which users can attach a debugger to any process or to the kernel.</span></span> <span data-ttu-id="22833-251">仅支持状态 NotConfigured 和 Allowed</span><span class="sxs-lookup"><span data-stu-id="22833-251">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="22833-252">userRightsRemoteDesktopServicesLogOn</span><span class="sxs-lookup"><span data-stu-id="22833-252">userRightsRemoteDesktopServicesLogOn</span></span>|[<span data-ttu-id="22833-253">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="22833-253">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="22833-254">此用户权限确定禁止哪些用户和组以远程桌面服务客户端登录。</span><span class="sxs-lookup"><span data-stu-id="22833-254">This user right determines which users and groups are prohibited from logging on as a Remote Desktop Services client.</span></span> <span data-ttu-id="22833-255">仅支持状态 NotConfigured 和 Blocked</span><span class="sxs-lookup"><span data-stu-id="22833-255">Only states NotConfigured and Blocked are supported</span></span>|
|<span data-ttu-id="22833-256">userRightsDelegation</span><span class="sxs-lookup"><span data-stu-id="22833-256">userRightsDelegation</span></span>|[<span data-ttu-id="22833-257">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="22833-257">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="22833-258">此用户权限确定哪些用户可以在用户或计算机对象上设置"受信任的委派"设置。</span><span class="sxs-lookup"><span data-stu-id="22833-258">This user right determines which users can set the Trusted for Delegation setting on a user or computer object.</span></span> <span data-ttu-id="22833-259">仅支持状态 NotConfigured 和 Allowed。</span><span class="sxs-lookup"><span data-stu-id="22833-259">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="22833-260">userRightsGenerateSecurityAudits</span><span class="sxs-lookup"><span data-stu-id="22833-260">userRightsGenerateSecurityAudits</span></span>|[<span data-ttu-id="22833-261">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="22833-261">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="22833-262">此用户权限确定进程可以使用哪些帐户向安全日志添加条目。</span><span class="sxs-lookup"><span data-stu-id="22833-262">This user right determines which accounts can be used by a process to add entries to the security log.</span></span> <span data-ttu-id="22833-263">安全日志用于跟踪未经授权的系统访问。</span><span class="sxs-lookup"><span data-stu-id="22833-263">The security log is used to trace unauthorized system access.</span></span>  <span data-ttu-id="22833-264">仅支持状态 NotConfigured 和 Allowed。</span><span class="sxs-lookup"><span data-stu-id="22833-264">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="22833-265">userRightsImpersonateClient</span><span class="sxs-lookup"><span data-stu-id="22833-265">userRightsImpersonateClient</span></span>|[<span data-ttu-id="22833-266">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="22833-266">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="22833-267">向用户分配此用户权限允许代表该用户运行的程序模拟客户端。</span><span class="sxs-lookup"><span data-stu-id="22833-267">Assigning this user right to a user allows programs running on behalf of that user to impersonate a client.</span></span> <span data-ttu-id="22833-268">要求此用户具有此用户权限进行这种模拟可防止未经授权的用户冒充客户端连接到他们创建的服务，然后模拟该客户端，从而将未经授权的用户权限提升到管理级别或系统级别。</span><span class="sxs-lookup"><span data-stu-id="22833-268">Requiring this user right for this kind of impersonation prevents an unauthorized user from convincing a client to connect to a service that they have created and then impersonating that client, which can elevate the unauthorized user's permissions to administrative or system levels.</span></span> <span data-ttu-id="22833-269">仅支持状态 NotConfigured 和 Allowed。</span><span class="sxs-lookup"><span data-stu-id="22833-269">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="22833-270">userRightsIncreaseSchedulingPriority</span><span class="sxs-lookup"><span data-stu-id="22833-270">userRightsIncreaseSchedulingPriority</span></span>|[<span data-ttu-id="22833-271">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="22833-271">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="22833-272">此用户权限确定哪些帐户可以使用具有对另一个进程的 Write Property 访问权限的进程来增加分配给另一个进程的执行优先级。</span><span class="sxs-lookup"><span data-stu-id="22833-272">This user right determines which accounts can use a process with Write Property access to another process to increase the execution priority assigned to the other process.</span></span> <span data-ttu-id="22833-273">仅支持状态 NotConfigured 和 Allowed。</span><span class="sxs-lookup"><span data-stu-id="22833-273">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="22833-274">userRightsLoadUnloadDrivers</span><span class="sxs-lookup"><span data-stu-id="22833-274">userRightsLoadUnloadDrivers</span></span>|[<span data-ttu-id="22833-275">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="22833-275">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="22833-276">此用户权限确定哪些用户可以在内核模式下动态加载和卸载设备驱动程序或其他代码。</span><span class="sxs-lookup"><span data-stu-id="22833-276">This user right determines which users can dynamically load and unload device drivers or other code in to kernel mode.</span></span> <span data-ttu-id="22833-277">仅支持状态 NotConfigured 和 Allowed。</span><span class="sxs-lookup"><span data-stu-id="22833-277">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="22833-278">userRightsLockMemory</span><span class="sxs-lookup"><span data-stu-id="22833-278">userRightsLockMemory</span></span>|[<span data-ttu-id="22833-279">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="22833-279">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="22833-280">此用户权限确定哪些帐户可以使用进程将数据保留于物理内存中，这可以防止系统将数据分页到磁盘上的虚拟内存中。</span><span class="sxs-lookup"><span data-stu-id="22833-280">This user right determines which accounts can use a process to keep data in physical memory, which prevents the system from paging the data to virtual memory on disk.</span></span> <span data-ttu-id="22833-281">仅支持状态 NotConfigured 和 Allowed。</span><span class="sxs-lookup"><span data-stu-id="22833-281">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="22833-282">userRightsManageAuditingAndSecurityLogs</span><span class="sxs-lookup"><span data-stu-id="22833-282">userRightsManageAuditingAndSecurityLogs</span></span>|[<span data-ttu-id="22833-283">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="22833-283">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="22833-284">此用户权限确定哪些用户可以为单个资源（如文件、Active Directory 对象和注册表项）指定对象访问审核选项。</span><span class="sxs-lookup"><span data-stu-id="22833-284">This user right determines which users can specify object access auditing options for individual resources, such as files, Active Directory objects, and registry keys.</span></span> <span data-ttu-id="22833-285">仅支持状态 NotConfigured 和 Allowed。</span><span class="sxs-lookup"><span data-stu-id="22833-285">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="22833-286">userRightsManageVolumes</span><span class="sxs-lookup"><span data-stu-id="22833-286">userRightsManageVolumes</span></span>|[<span data-ttu-id="22833-287">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="22833-287">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="22833-288">此用户权限确定哪些用户和组可以在卷上运行维护任务，例如远程碎片整理。</span><span class="sxs-lookup"><span data-stu-id="22833-288">This user right determines which users and groups can run maintenance tasks on a volume, such as remote defragmentation.</span></span> <span data-ttu-id="22833-289">仅支持状态 NotConfigured 和 Allowed。</span><span class="sxs-lookup"><span data-stu-id="22833-289">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="22833-290">userRightsModifyFirmwareEnvironment</span><span class="sxs-lookup"><span data-stu-id="22833-290">userRightsModifyFirmwareEnvironment</span></span>|[<span data-ttu-id="22833-291">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="22833-291">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="22833-292">此用户权限确定可以修改固件环境值的用户。</span><span class="sxs-lookup"><span data-stu-id="22833-292">This user right determines who can modify firmware environment values.</span></span> <span data-ttu-id="22833-293">仅支持状态 NotConfigured 和 Allowed。</span><span class="sxs-lookup"><span data-stu-id="22833-293">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="22833-294">userRightsModifyObjectLabels</span><span class="sxs-lookup"><span data-stu-id="22833-294">userRightsModifyObjectLabels</span></span>|[<span data-ttu-id="22833-295">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="22833-295">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="22833-296">此用户权限确定哪些用户帐户可以修改对象（如文件、注册表项或其他用户拥有的进程）的完整性标签。</span><span class="sxs-lookup"><span data-stu-id="22833-296">This user right determines which user accounts can modify the integrity label of objects, such as files, registry keys, or processes owned by other users.</span></span> <span data-ttu-id="22833-297">仅支持状态 NotConfigured 和 Allowed。</span><span class="sxs-lookup"><span data-stu-id="22833-297">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="22833-298">userRightsProfileSingleProcess</span><span class="sxs-lookup"><span data-stu-id="22833-298">userRightsProfileSingleProcess</span></span>|[<span data-ttu-id="22833-299">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="22833-299">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="22833-300">此用户权限确定哪些用户可以使用性能监视工具来监视系统进程的性能。</span><span class="sxs-lookup"><span data-stu-id="22833-300">This user right determines which users can use performance monitoring tools to monitor the performance of system processes.</span></span> <span data-ttu-id="22833-301">仅支持状态 NotConfigured 和 Allowed。</span><span class="sxs-lookup"><span data-stu-id="22833-301">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="22833-302">userRightsRemoteShutdown</span><span class="sxs-lookup"><span data-stu-id="22833-302">userRightsRemoteShutdown</span></span>|[<span data-ttu-id="22833-303">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="22833-303">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="22833-304">此用户权限确定允许哪些用户从网络远程位置关闭计算机。</span><span class="sxs-lookup"><span data-stu-id="22833-304">This user right determines which users are allowed to shut down a computer from a remote location on the network.</span></span> <span data-ttu-id="22833-305">滥用此用户权限可能会导致拒绝服务。</span><span class="sxs-lookup"><span data-stu-id="22833-305">Misuse of this user right can result in a denial of service.</span></span> <span data-ttu-id="22833-306">仅支持状态 NotConfigured 和 Allowed。</span><span class="sxs-lookup"><span data-stu-id="22833-306">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="22833-307">userRightsRestoreData</span><span class="sxs-lookup"><span data-stu-id="22833-307">userRightsRestoreData</span></span>|[<span data-ttu-id="22833-308">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="22833-308">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="22833-309">此用户权限确定哪些用户在还原备份的文件和目录时可以绕过文件、目录、注册表和其他永久对象权限，并确定哪些用户可以将任何有效的安全主体设置为对象的所有者。</span><span class="sxs-lookup"><span data-stu-id="22833-309">This user right determines which users can bypass file, directory, registry, and other persistent objects permissions when restoring backed up files and directories, and determines which users can set any valid security principal as the owner of an object.</span></span> <span data-ttu-id="22833-310">仅支持状态 NotConfigured 和 Allowed。</span><span class="sxs-lookup"><span data-stu-id="22833-310">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="22833-311">userRightsOwnership</span><span class="sxs-lookup"><span data-stu-id="22833-311">userRightsTakeOwnership</span></span>|[<span data-ttu-id="22833-312">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="22833-312">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="22833-313">此用户权限确定哪些用户可以获得系统中任何安全对象的所有权，包括 Active Directory 对象、文件和文件夹、打印机、注册表项、进程和线程。</span><span class="sxs-lookup"><span data-stu-id="22833-313">This user right determines which users can take ownership of any securable object in the system, including Active Directory objects, files and folders, printers, registry keys, processes, and threads.</span></span> <span data-ttu-id="22833-314">仅支持状态 NotConfigured 和 Allowed。</span><span class="sxs-lookup"><span data-stu-id="22833-314">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="22833-315">xboxServicesEnableXboxGameSaveTask</span><span class="sxs-lookup"><span data-stu-id="22833-315">xboxServicesEnableXboxGameSaveTask</span></span>|<span data-ttu-id="22833-316">Boolean</span><span class="sxs-lookup"><span data-stu-id="22833-316">Boolean</span></span>|<span data-ttu-id="22833-317">此设置确定 xbox 游戏保存是在 1 (1) 还是从 0 (禁用) 。</span><span class="sxs-lookup"><span data-stu-id="22833-317">This setting determines whether xbox game save is enabled (1) or disabled (0).</span></span>|
|<span data-ttu-id="22833-318">xboxServicesAccessoryManagementServiceStartupMode</span><span class="sxs-lookup"><span data-stu-id="22833-318">xboxServicesAccessoryManagementServiceStartupMode</span></span>|[<span data-ttu-id="22833-319">serviceStartType</span><span class="sxs-lookup"><span data-stu-id="22833-319">serviceStartType</span></span>](../resources/intune-deviceconfig-servicestarttype.md)|<span data-ttu-id="22833-320">此设置确定附件管理服务的启动类型是自动 (2) 、手动 (3) 、禁用 (4) 。</span><span class="sxs-lookup"><span data-stu-id="22833-320">This setting determines whether the Accessory management service's start type is Automatic(2), Manual(3), Disabled(4).</span></span> <span data-ttu-id="22833-321">默认值：手动。</span><span class="sxs-lookup"><span data-stu-id="22833-321">Default: Manual.</span></span> <span data-ttu-id="22833-322">可取值为：`manual`、`automatic`、`disabled`。</span><span class="sxs-lookup"><span data-stu-id="22833-322">Possible values are: `manual`, `automatic`, `disabled`.</span></span>|
|<span data-ttu-id="22833-323">xboxServicesLiveAuthManagerServiceStartupMode</span><span class="sxs-lookup"><span data-stu-id="22833-323">xboxServicesLiveAuthManagerServiceStartupMode</span></span>|[<span data-ttu-id="22833-324">serviceStartType</span><span class="sxs-lookup"><span data-stu-id="22833-324">serviceStartType</span></span>](../resources/intune-deviceconfig-servicestarttype.md)|<span data-ttu-id="22833-325">此设置确定 Live Auth Manager 服务的启动类型是自动 (2) 、手动 (3) 、禁用 (4) 。</span><span class="sxs-lookup"><span data-stu-id="22833-325">This setting determines whether Live Auth Manager service's start type is Automatic(2), Manual(3), Disabled(4).</span></span> <span data-ttu-id="22833-326">默认值：手动。</span><span class="sxs-lookup"><span data-stu-id="22833-326">Default: Manual.</span></span> <span data-ttu-id="22833-327">可取值为：`manual`、`automatic`、`disabled`。</span><span class="sxs-lookup"><span data-stu-id="22833-327">Possible values are: `manual`, `automatic`, `disabled`.</span></span>|
|<span data-ttu-id="22833-328">xboxServicesLiveGameSaveServiceStartupMode</span><span class="sxs-lookup"><span data-stu-id="22833-328">xboxServicesLiveGameSaveServiceStartupMode</span></span>|[<span data-ttu-id="22833-329">serviceStartType</span><span class="sxs-lookup"><span data-stu-id="22833-329">serviceStartType</span></span>](../resources/intune-deviceconfig-servicestarttype.md)|<span data-ttu-id="22833-330">此设置确定 Live Game 保存服务的启动类型是 4 (2) 、手动 (3) 、禁用 (4) 。</span><span class="sxs-lookup"><span data-stu-id="22833-330">This setting determines whether Live Game save service's start type is Automatic(2), Manual(3), Disabled(4).</span></span> <span data-ttu-id="22833-331">默认值：手动。</span><span class="sxs-lookup"><span data-stu-id="22833-331">Default: Manual.</span></span> <span data-ttu-id="22833-332">可取值为：`manual`、`automatic`、`disabled`。</span><span class="sxs-lookup"><span data-stu-id="22833-332">Possible values are: `manual`, `automatic`, `disabled`.</span></span>|
|<span data-ttu-id="22833-333">xboxServicesLiveNetworkingServiceStartupMode</span><span class="sxs-lookup"><span data-stu-id="22833-333">xboxServicesLiveNetworkingServiceStartupMode</span></span>|[<span data-ttu-id="22833-334">serviceStartType</span><span class="sxs-lookup"><span data-stu-id="22833-334">serviceStartType</span></span>](../resources/intune-deviceconfig-servicestarttype.md)|<span data-ttu-id="22833-335">此设置确定网络服务的启动类型是自动 (2) 、手动 (3) 、禁用 (4) 。</span><span class="sxs-lookup"><span data-stu-id="22833-335">This setting determines whether Networking service's start type is Automatic(2), Manual(3), Disabled(4).</span></span> <span data-ttu-id="22833-336">默认值：手动。</span><span class="sxs-lookup"><span data-stu-id="22833-336">Default: Manual.</span></span> <span data-ttu-id="22833-337">可取值为：`manual`、`automatic`、`disabled`。</span><span class="sxs-lookup"><span data-stu-id="22833-337">Possible values are: `manual`, `automatic`, `disabled`.</span></span>|
|<span data-ttu-id="22833-338">localSecurityOptionsBlockMicrosoftAccounts</span><span class="sxs-lookup"><span data-stu-id="22833-338">localSecurityOptionsBlockMicrosoftAccounts</span></span>|<span data-ttu-id="22833-339">Boolean</span><span class="sxs-lookup"><span data-stu-id="22833-339">Boolean</span></span>|<span data-ttu-id="22833-340">阻止用户向此计算机添加新的 Microsoft 帐户。</span><span class="sxs-lookup"><span data-stu-id="22833-340">Prevent users from adding new Microsoft accounts to this computer.</span></span>|
|<span data-ttu-id="22833-341">localSecurityOptionsBlockRemoteLogonWithBlankPassword</span><span class="sxs-lookup"><span data-stu-id="22833-341">localSecurityOptionsBlockRemoteLogonWithBlankPassword</span></span>|<span data-ttu-id="22833-342">Boolean</span><span class="sxs-lookup"><span data-stu-id="22833-342">Boolean</span></span>|<span data-ttu-id="22833-343">启用未受密码保护的本地帐户，以便从物理设备外的位置登录。默认为启用</span><span class="sxs-lookup"><span data-stu-id="22833-343">Enable Local accounts that are not password protected to log on from locations other than the physical device.Default is enabled</span></span>|
|<span data-ttu-id="22833-344">localSecurityOptionsDisableAdministratorAccount</span><span class="sxs-lookup"><span data-stu-id="22833-344">localSecurityOptionsDisableAdministratorAccount</span></span>|<span data-ttu-id="22833-345">Boolean</span><span class="sxs-lookup"><span data-stu-id="22833-345">Boolean</span></span>|<span data-ttu-id="22833-346">确定是启用还是禁用本地管理员帐户。</span><span class="sxs-lookup"><span data-stu-id="22833-346">Determines whether the Local Administrator account is enabled or disabled.</span></span>|
|<span data-ttu-id="22833-347">localSecurityOptionsAdministratorAccountName</span><span class="sxs-lookup"><span data-stu-id="22833-347">localSecurityOptionsAdministratorAccountName</span></span>|<span data-ttu-id="22833-348">String</span><span class="sxs-lookup"><span data-stu-id="22833-348">String</span></span>|<span data-ttu-id="22833-349">为帐户"管理员"定义与 SID (关联的) 名称。</span><span class="sxs-lookup"><span data-stu-id="22833-349">Define a different account name to be associated with the security identifier (SID) for the account “Administrator”.</span></span>|
|<span data-ttu-id="22833-350">localSecurityOptionsDisableGuestAccount</span><span class="sxs-lookup"><span data-stu-id="22833-350">localSecurityOptionsDisableGuestAccount</span></span>|<span data-ttu-id="22833-351">Boolean</span><span class="sxs-lookup"><span data-stu-id="22833-351">Boolean</span></span>|<span data-ttu-id="22833-352">确定是否启用或禁用来宾帐户。</span><span class="sxs-lookup"><span data-stu-id="22833-352">Determines if the Guest account is enabled or disabled.</span></span>|
|<span data-ttu-id="22833-353">localSecurityOptionsGuestAccountName</span><span class="sxs-lookup"><span data-stu-id="22833-353">localSecurityOptionsGuestAccountName</span></span>|<span data-ttu-id="22833-354">String</span><span class="sxs-lookup"><span data-stu-id="22833-354">String</span></span>|<span data-ttu-id="22833-355">定义一个不同的帐户名称，以与"来宾" (SID) 安全标识符相关联。</span><span class="sxs-lookup"><span data-stu-id="22833-355">Define a different account name to be associated with the security identifier (SID) for the account “Guest”.</span></span>|
|<span data-ttu-id="22833-356">localSecurityOptionsAllowUndockWithoutHavingToLogon</span><span class="sxs-lookup"><span data-stu-id="22833-356">localSecurityOptionsAllowUndockWithoutHavingToLogon</span></span>|<span data-ttu-id="22833-357">Boolean</span><span class="sxs-lookup"><span data-stu-id="22833-357">Boolean</span></span>|<span data-ttu-id="22833-358">防止便携计算机在无需登录的情况下被移除。</span><span class="sxs-lookup"><span data-stu-id="22833-358">Prevent a portable computer from being undocked without having to log in.</span></span>|
|<span data-ttu-id="22833-359">localSecurityOptionsBlockUsersInstallingPrinterDrivers</span><span class="sxs-lookup"><span data-stu-id="22833-359">localSecurityOptionsBlockUsersInstallingPrinterDrivers</span></span>|<span data-ttu-id="22833-360">Boolean</span><span class="sxs-lookup"><span data-stu-id="22833-360">Boolean</span></span>|<span data-ttu-id="22833-361">限制为仅将打印机驱动程序安装为连接到共享打印机的一部分。</span><span class="sxs-lookup"><span data-stu-id="22833-361">Restrict installing printer drivers as part of connecting to a shared printer to admins only.</span></span>|
|<span data-ttu-id="22833-362">localSecurityOptionsBlockRemoteOpticalDriveAccess</span><span class="sxs-lookup"><span data-stu-id="22833-362">localSecurityOptionsBlockRemoteOpticalDriveAccess</span></span>|<span data-ttu-id="22833-363">Boolean</span><span class="sxs-lookup"><span data-stu-id="22833-363">Boolean</span></span>|<span data-ttu-id="22833-364">启用这些设置仅允许以交互方式登录的用户访问 CD-ROM 媒体。</span><span class="sxs-lookup"><span data-stu-id="22833-364">Enabling this settings allows only interactively logged on user to access CD-ROM media.</span></span>|
|<span data-ttu-id="22833-365">localSecurityOptionsFormatAndEjectOfRemovableMediaAllowedUser</span><span class="sxs-lookup"><span data-stu-id="22833-365">localSecurityOptionsFormatAndEjectOfRemovableMediaAllowedUser</span></span>|[<span data-ttu-id="22833-366">localSecurityOptionsFormatAndEjectOfRemovableMediaAllowedUserType</span><span class="sxs-lookup"><span data-stu-id="22833-366">localSecurityOptionsFormatAndEjectOfRemovableMediaAllowedUserType</span></span>](../resources/intune-deviceconfig-localsecurityoptionsformatandejectofremovablemediaallowedusertype.md)|<span data-ttu-id="22833-367">定义允许谁格式化和弹出可移动 NTFS 媒体。</span><span class="sxs-lookup"><span data-stu-id="22833-367">Define who is allowed to format and eject removable NTFS media.</span></span> <span data-ttu-id="22833-368">可取值为：`notConfigured`、`administrators`、`administratorsAndPowerUsers`、`administratorsAndInteractiveUsers`。</span><span class="sxs-lookup"><span data-stu-id="22833-368">Possible values are: `notConfigured`, `administrators`, `administratorsAndPowerUsers`, `administratorsAndInteractiveUsers`.</span></span>|
|<span data-ttu-id="22833-369">localSecurityOptionsMachineInactivityLimit</span><span class="sxs-lookup"><span data-stu-id="22833-369">localSecurityOptionsMachineInactivityLimit</span></span>|<span data-ttu-id="22833-370">Int32</span><span class="sxs-lookup"><span data-stu-id="22833-370">Int32</span></span>|<span data-ttu-id="22833-371">定义交互式桌面登录屏幕上不活动的最大分钟数，直到屏幕保护程序运行。</span><span class="sxs-lookup"><span data-stu-id="22833-371">Define maximum minutes of inactivity on the interactive desktop’s login screen until the screen saver runs.</span></span> <span data-ttu-id="22833-372">有效值为 0 至 9999</span><span class="sxs-lookup"><span data-stu-id="22833-372">Valid values 0 to 9999</span></span>|
|<span data-ttu-id="22833-373">localSecurityOptionsMachineInactivityLimitInMinutes</span><span class="sxs-lookup"><span data-stu-id="22833-373">localSecurityOptionsMachineInactivityLimitInMinutes</span></span>|<span data-ttu-id="22833-374">Int32</span><span class="sxs-lookup"><span data-stu-id="22833-374">Int32</span></span>|<span data-ttu-id="22833-375">定义交互式桌面登录屏幕上不活动的最大分钟数，直到屏幕保护程序运行。</span><span class="sxs-lookup"><span data-stu-id="22833-375">Define maximum minutes of inactivity on the interactive desktop’s login screen until the screen saver runs.</span></span> <span data-ttu-id="22833-376">有效值为 0 至 9999</span><span class="sxs-lookup"><span data-stu-id="22833-376">Valid values 0 to 9999</span></span>|
|<span data-ttu-id="22833-377">localSecurityOptionsDoNotRequireCtrlAltDel</span><span class="sxs-lookup"><span data-stu-id="22833-377">localSecurityOptionsDoNotRequireCtrlAltDel</span></span>|<span data-ttu-id="22833-378">Boolean</span><span class="sxs-lookup"><span data-stu-id="22833-378">Boolean</span></span>|<span data-ttu-id="22833-379">要求在用户登录前按 Ctrl+Alt+DEL。</span><span class="sxs-lookup"><span data-stu-id="22833-379">Require CTRL+ALT+DEL to be pressed before a user can log on.</span></span>|
|<span data-ttu-id="22833-380">localSecurityOptionsHideLastSignedInUser</span><span class="sxs-lookup"><span data-stu-id="22833-380">localSecurityOptionsHideLastSignedInUser</span></span>|<span data-ttu-id="22833-381">Boolean</span><span class="sxs-lookup"><span data-stu-id="22833-381">Boolean</span></span>|<span data-ttu-id="22833-382">不显示最后一个登录此设备的用户的用户名。</span><span class="sxs-lookup"><span data-stu-id="22833-382">Do not display the username of the last person who signed in on this device.</span></span>|
|<span data-ttu-id="22833-383">localSecurityOptionsHideUsernameAtSignIn</span><span class="sxs-lookup"><span data-stu-id="22833-383">localSecurityOptionsHideUsernameAtSignIn</span></span>|<span data-ttu-id="22833-384">Boolean</span><span class="sxs-lookup"><span data-stu-id="22833-384">Boolean</span></span>|<span data-ttu-id="22833-385">输入凭据后和显示设备桌面之前，不显示登录此设备的用户的用户名。</span><span class="sxs-lookup"><span data-stu-id="22833-385">Do not display the username of the person signing in to this device after credentials are entered and before the device’s desktop is shown.</span></span>|
|<span data-ttu-id="22833-386">localSecurityOptionsLogOnMessageTitle</span><span class="sxs-lookup"><span data-stu-id="22833-386">localSecurityOptionsLogOnMessageTitle</span></span>|<span data-ttu-id="22833-387">String</span><span class="sxs-lookup"><span data-stu-id="22833-387">String</span></span>|<span data-ttu-id="22833-388">为尝试登录的用户设置消息标题。</span><span class="sxs-lookup"><span data-stu-id="22833-388">Set message title for users attempting to log in.</span></span>|
|<span data-ttu-id="22833-389">localSecurityOptionsLogOnMessageText</span><span class="sxs-lookup"><span data-stu-id="22833-389">localSecurityOptionsLogOnMessageText</span></span>|<span data-ttu-id="22833-390">String</span><span class="sxs-lookup"><span data-stu-id="22833-390">String</span></span>|<span data-ttu-id="22833-391">设置尝试登录的用户的消息文本。</span><span class="sxs-lookup"><span data-stu-id="22833-391">Set message text for users attempting to log in.</span></span>|
|<span data-ttu-id="22833-392">localSecurityOptionsAllowPKU2UAuthenticationRequests</span><span class="sxs-lookup"><span data-stu-id="22833-392">localSecurityOptionsAllowPKU2UAuthenticationRequests</span></span>|<span data-ttu-id="22833-393">Boolean</span><span class="sxs-lookup"><span data-stu-id="22833-393">Boolean</span></span>|<span data-ttu-id="22833-394">阻止对此设备的 PKU2U 身份验证请求使用联机标识。</span><span class="sxs-lookup"><span data-stu-id="22833-394">Block PKU2U authentication requests to this device to use online identities.</span></span>|
|<span data-ttu-id="22833-395">localSecurityOptionsAllowRemoteCallsToSecurityAccountsManagerHelperBool</span><span class="sxs-lookup"><span data-stu-id="22833-395">localSecurityOptionsAllowRemoteCallsToSecurityAccountsManagerHelperBool</span></span>|<span data-ttu-id="22833-396">Boolean</span><span class="sxs-lookup"><span data-stu-id="22833-396">Boolean</span></span>|<span data-ttu-id="22833-397">LocalSecurityOptionsAllowRemoteCallsToSecurityAccountsManager 实体的 UI 帮助程序布尔值</span><span class="sxs-lookup"><span data-stu-id="22833-397">UI helper boolean for LocalSecurityOptionsAllowRemoteCallsToSecurityAccountsManager entity</span></span>|
|<span data-ttu-id="22833-398">localSecurityOptionsAllowRemoteCallsToSecurityAccountsManager</span><span class="sxs-lookup"><span data-stu-id="22833-398">localSecurityOptionsAllowRemoteCallsToSecurityAccountsManager</span></span>|<span data-ttu-id="22833-399">String</span><span class="sxs-lookup"><span data-stu-id="22833-399">String</span></span>|<span data-ttu-id="22833-400">编辑默认安全描述符定义语言字符串以允许或拒绝用户和组对 SAM 进行远程调用。</span><span class="sxs-lookup"><span data-stu-id="22833-400">Edit the default Security Descriptor Definition Language string to allow or deny users and groups to make remote calls to the SAM.</span></span>|
|<span data-ttu-id="22833-401">localSecurityOptionsMinimumSessionSecurityForNtlmSspBasedClients</span><span class="sxs-lookup"><span data-stu-id="22833-401">localSecurityOptionsMinimumSessionSecurityForNtlmSspBasedClients</span></span>|[<span data-ttu-id="22833-402">localSecurityOptionsMinimumSessionSecurity</span><span class="sxs-lookup"><span data-stu-id="22833-402">localSecurityOptionsMinimumSessionSecurity</span></span>](../resources/intune-deviceconfig-localsecurityoptionsminimumsessionsecurity.md)|<span data-ttu-id="22833-403">此安全性设置允许客户端要求协商 128 位加密和/或 NTLMv2 会话安全性。</span><span class="sxs-lookup"><span data-stu-id="22833-403">This security setting allows a client to require the negotiation of 128-bit encryption and/or NTLMv2 session security.</span></span> <span data-ttu-id="22833-404">可取值为：`none`、`requireNtmlV2SessionSecurity`、`require128BitEncryption`、`ntlmV2And128BitEncryption`。</span><span class="sxs-lookup"><span data-stu-id="22833-404">Possible values are: `none`, `requireNtmlV2SessionSecurity`, `require128BitEncryption`, `ntlmV2And128BitEncryption`.</span></span>|
|<span data-ttu-id="22833-405">localSecurityOptionsMinimumSessionSecurityForNtlmSspBasedServers</span><span class="sxs-lookup"><span data-stu-id="22833-405">localSecurityOptionsMinimumSessionSecurityForNtlmSspBasedServers</span></span>|[<span data-ttu-id="22833-406">localSecurityOptionsMinimumSessionSecurity</span><span class="sxs-lookup"><span data-stu-id="22833-406">localSecurityOptionsMinimumSessionSecurity</span></span>](../resources/intune-deviceconfig-localsecurityoptionsminimumsessionsecurity.md)|<span data-ttu-id="22833-407">此安全性设置允许服务器要求协商 128 位加密和/或 NTLMv2 会话安全性。</span><span class="sxs-lookup"><span data-stu-id="22833-407">This security setting allows a server to require the negotiation of 128-bit encryption and/or NTLMv2 session security.</span></span> <span data-ttu-id="22833-408">可取值为：`none`、`requireNtmlV2SessionSecurity`、`require128BitEncryption`、`ntlmV2And128BitEncryption`。</span><span class="sxs-lookup"><span data-stu-id="22833-408">Possible values are: `none`, `requireNtmlV2SessionSecurity`, `require128BitEncryption`, `ntlmV2And128BitEncryption`.</span></span>|
|<span data-ttu-id="22833-409">lanManagerAuthenticationLevel</span><span class="sxs-lookup"><span data-stu-id="22833-409">lanManagerAuthenticationLevel</span></span>|[<span data-ttu-id="22833-410">lanManagerAuthenticationLevel</span><span class="sxs-lookup"><span data-stu-id="22833-410">lanManagerAuthenticationLevel</span></span>](../resources/intune-deviceconfig-lanmanagerauthenticationlevel.md)|<span data-ttu-id="22833-411">此安全性设置确定用于网络登录的质询/响应身份验证协议。</span><span class="sxs-lookup"><span data-stu-id="22833-411">This security setting determines which challenge/response authentication protocol is used for network logons.</span></span> <span data-ttu-id="22833-412">可取值为：`lmAndNltm`、`lmNtlmAndNtlmV2`、`lmAndNtlmOnly`、`lmAndNtlmV2`、`lmNtlmV2AndNotLm`、`lmNtlmV2AndNotLmOrNtm`。</span><span class="sxs-lookup"><span data-stu-id="22833-412">Possible values are: `lmAndNltm`, `lmNtlmAndNtlmV2`, `lmAndNtlmOnly`, `lmAndNtlmV2`, `lmNtlmV2AndNotLm`, `lmNtlmV2AndNotLmOrNtm`.</span></span>|
|<span data-ttu-id="22833-413">lanManagerWorkstationDisableInsecureGuestLogons</span><span class="sxs-lookup"><span data-stu-id="22833-413">lanManagerWorkstationDisableInsecureGuestLogons</span></span>|<span data-ttu-id="22833-414">Boolean</span><span class="sxs-lookup"><span data-stu-id="22833-414">Boolean</span></span>|<span data-ttu-id="22833-415">如果启用，SMB 客户端将允许不安全的来宾徽标。</span><span class="sxs-lookup"><span data-stu-id="22833-415">If enabled,the SMB client will allow insecure guest logons.</span></span> <span data-ttu-id="22833-416">如果未配置，SMB 客户端将拒绝不安全的来宾徽标。</span><span class="sxs-lookup"><span data-stu-id="22833-416">If not configured, the SMB client will reject insecure guest logons.</span></span>|
|<span data-ttu-id="22833-417">localSecurityOptionsClearVirtualMemoryPageFile</span><span class="sxs-lookup"><span data-stu-id="22833-417">localSecurityOptionsClearVirtualMemoryPageFile</span></span>|<span data-ttu-id="22833-418">Boolean</span><span class="sxs-lookup"><span data-stu-id="22833-418">Boolean</span></span>|<span data-ttu-id="22833-419">此安全设置确定是否在系统关闭时清除虚拟内存页面文件。</span><span class="sxs-lookup"><span data-stu-id="22833-419">This security setting determines whether the virtual memory pagefile is cleared when the system is shut down.</span></span>|
|<span data-ttu-id="22833-420">localSecurityOptionsAllowSystemToBeShutDownWithoutHavingToLogOn</span><span class="sxs-lookup"><span data-stu-id="22833-420">localSecurityOptionsAllowSystemToBeShutDownWithoutHavingToLogOn</span></span>|<span data-ttu-id="22833-421">Boolean</span><span class="sxs-lookup"><span data-stu-id="22833-421">Boolean</span></span>|<span data-ttu-id="22833-422">此安全设置确定是否可以关闭计算机而无需登录到 Windows。</span><span class="sxs-lookup"><span data-stu-id="22833-422">This security setting determines whether a computer can be shut down without having to log on to Windows.</span></span>|
|<span data-ttu-id="22833-423">localSecurityOptionsAllowUIAccessApplicationElevation</span><span class="sxs-lookup"><span data-stu-id="22833-423">localSecurityOptionsAllowUIAccessApplicationElevation</span></span>|<span data-ttu-id="22833-424">Boolean</span><span class="sxs-lookup"><span data-stu-id="22833-424">Boolean</span></span>|<span data-ttu-id="22833-425">允许 UIAccess 应用在没有使用安全桌面的情况下提示提升。</span><span class="sxs-lookup"><span data-stu-id="22833-425">Allow UIAccess apps to prompt for elevation without using the secure desktop.</span></span>|
|<span data-ttu-id="22833-426">localSecurityOptionsVirtualizeFileAndRegistryWriteFailuresToPerUserLocations</span><span class="sxs-lookup"><span data-stu-id="22833-426">localSecurityOptionsVirtualizeFileAndRegistryWriteFailuresToPerUserLocations</span></span>|<span data-ttu-id="22833-427">Boolean</span><span class="sxs-lookup"><span data-stu-id="22833-427">Boolean</span></span>|<span data-ttu-id="22833-428">将文件和注册表写入故障虚拟化到每个用户位置</span><span class="sxs-lookup"><span data-stu-id="22833-428">Virtualize file and registry write failures to per user locations</span></span>|
|<span data-ttu-id="22833-429">localSecurityOptionsOnlyElevateSignedExecutables</span><span class="sxs-lookup"><span data-stu-id="22833-429">localSecurityOptionsOnlyElevateSignedExecutables</span></span>|<span data-ttu-id="22833-430">Boolean</span><span class="sxs-lookup"><span data-stu-id="22833-430">Boolean</span></span>|<span data-ttu-id="22833-431">在允许运行给定可执行文件之前，对该文件强制执行 PKI 证书路径验证。</span><span class="sxs-lookup"><span data-stu-id="22833-431">Enforce PKI certification path validation for a given executable file before it is permitted to run.</span></span>|
|<span data-ttu-id="22833-432">localSecurityOptionsAdministratorElevationPromptBehavior</span><span class="sxs-lookup"><span data-stu-id="22833-432">localSecurityOptionsAdministratorElevationPromptBehavior</span></span>|[<span data-ttu-id="22833-433">localSecurityOptionsAdministratorElevationPromptBehaviorType</span><span class="sxs-lookup"><span data-stu-id="22833-433">localSecurityOptionsAdministratorElevationPromptBehaviorType</span></span>](../resources/intune-deviceconfig-localsecurityoptionsadministratorelevationpromptbehaviortype.md)|<span data-ttu-id="22833-434">定义管理员审批模式下管理员的提升权限提示行为。</span><span class="sxs-lookup"><span data-stu-id="22833-434">Define the behavior of the elevation prompt for admins in Admin Approval Mode.</span></span> <span data-ttu-id="22833-435">可取值为：`notConfigured`、`elevateWithoutPrompting`、`promptForCredentialsOnTheSecureDesktop`、`promptForConsentOnTheSecureDesktop`、`promptForCredentials`、`promptForConsent` 或 `promptForConsentForNonWindowsBinaries`。</span><span class="sxs-lookup"><span data-stu-id="22833-435">Possible values are: `notConfigured`, `elevateWithoutPrompting`, `promptForCredentialsOnTheSecureDesktop`, `promptForConsentOnTheSecureDesktop`, `promptForCredentials`, `promptForConsent`, `promptForConsentForNonWindowsBinaries`.</span></span>|
|<span data-ttu-id="22833-436">localSecurityOptionsStandardUserElevationPromptBehavior</span><span class="sxs-lookup"><span data-stu-id="22833-436">localSecurityOptionsStandardUserElevationPromptBehavior</span></span>|[<span data-ttu-id="22833-437">localSecurityOptionsStandardUserElevationPromptBehaviorType</span><span class="sxs-lookup"><span data-stu-id="22833-437">localSecurityOptionsStandardUserElevationPromptBehaviorType</span></span>](../resources/intune-deviceconfig-localsecurityoptionsstandarduserelevationpromptbehaviortype.md)|<span data-ttu-id="22833-438">定义标准用户的提升权限提示的行为。</span><span class="sxs-lookup"><span data-stu-id="22833-438">Define the behavior of the elevation prompt for standard users.</span></span> <span data-ttu-id="22833-439">可取值为：`notConfigured`、`automaticallyDenyElevationRequests`、`promptForCredentialsOnTheSecureDesktop`、`promptForCredentials`。</span><span class="sxs-lookup"><span data-stu-id="22833-439">Possible values are: `notConfigured`, `automaticallyDenyElevationRequests`, `promptForCredentialsOnTheSecureDesktop`, `promptForCredentials`.</span></span>|
|<span data-ttu-id="22833-440">localSecurityOptionsSwitchToSecureDesktopWhenPromptingForElevation</span><span class="sxs-lookup"><span data-stu-id="22833-440">localSecurityOptionsSwitchToSecureDesktopWhenPromptingForElevation</span></span>|<span data-ttu-id="22833-441">Boolean</span><span class="sxs-lookup"><span data-stu-id="22833-441">Boolean</span></span>|<span data-ttu-id="22833-442">启用所有提升请求以转到交互式用户的桌面，而不是安全桌面。</span><span class="sxs-lookup"><span data-stu-id="22833-442">Enable all elevation requests to go to the interactive user's desktop rather than the secure desktop.</span></span> <span data-ttu-id="22833-443">使用管理员和标准用户的提示行为策略设置。</span><span class="sxs-lookup"><span data-stu-id="22833-443">Prompt behavior policy settings for admins and standard users are used.</span></span>|
|<span data-ttu-id="22833-444">localSecurityOptionsDetectApplicationInstallationsAndPromptForElevation</span><span class="sxs-lookup"><span data-stu-id="22833-444">localSecurityOptionsDetectApplicationInstallationsAndPromptForElevation</span></span>|<span data-ttu-id="22833-445">Boolean</span><span class="sxs-lookup"><span data-stu-id="22833-445">Boolean</span></span>|<span data-ttu-id="22833-446">需要提升特权的应用安装将提示输入管理员凭据。默认为启用</span><span class="sxs-lookup"><span data-stu-id="22833-446">App installations requiring elevated privileges will prompt for admin credentials.Default is enabled</span></span>|
|<span data-ttu-id="22833-447">localSecurityOptionsAllowUIAccessApplicationsForSecureLocations</span><span class="sxs-lookup"><span data-stu-id="22833-447">localSecurityOptionsAllowUIAccessApplicationsForSecureLocations</span></span>|<span data-ttu-id="22833-448">Boolean</span><span class="sxs-lookup"><span data-stu-id="22833-448">Boolean</span></span>|<span data-ttu-id="22833-449">允许 UIAccess 应用在没有使用安全桌面的情况下提示提升。默认为启用</span><span class="sxs-lookup"><span data-stu-id="22833-449">Allow UIAccess apps to prompt for elevation without using the secure desktop.Default is enabled</span></span>|
|<span data-ttu-id="22833-450">localSecurityOptionsUseAdminApprovalMode</span><span class="sxs-lookup"><span data-stu-id="22833-450">localSecurityOptionsUseAdminApprovalMode</span></span>|<span data-ttu-id="22833-451">Boolean</span><span class="sxs-lookup"><span data-stu-id="22833-451">Boolean</span></span>|<span data-ttu-id="22833-452">定义内置管理员帐户是使用管理员审批模式还是运行具有完全管理员权限的所有应用。默认为启用</span><span class="sxs-lookup"><span data-stu-id="22833-452">Defines whether the built-in admin account uses Admin Approval Mode or runs all apps with full admin privileges.Default is enabled</span></span>|
|<span data-ttu-id="22833-453">localSecurityOptionsUseAdminApprovalModeForAdministrators</span><span class="sxs-lookup"><span data-stu-id="22833-453">localSecurityOptionsUseAdminApprovalModeForAdministrators</span></span>|<span data-ttu-id="22833-454">Boolean</span><span class="sxs-lookup"><span data-stu-id="22833-454">Boolean</span></span>|<span data-ttu-id="22833-455">定义是否启用管理员审批模式以及所有 UAC 策略设置，默认为启用</span><span class="sxs-lookup"><span data-stu-id="22833-455">Define whether Admin Approval Mode and all UAC policy settings are enabled, default is enabled</span></span>|
|<span data-ttu-id="22833-456">localSecurityOptionsInformationShownOnLockScreen</span><span class="sxs-lookup"><span data-stu-id="22833-456">localSecurityOptionsInformationShownOnLockScreen</span></span>|[<span data-ttu-id="22833-457">localSecurityOptionsInformationShownOnLockScreenType</span><span class="sxs-lookup"><span data-stu-id="22833-457">localSecurityOptionsInformationShownOnLockScreenType</span></span>](../resources/intune-deviceconfig-localsecurityoptionsinformationshownonlockscreentype.md)|<span data-ttu-id="22833-458">配置在会话锁定时显示的用户信息。</span><span class="sxs-lookup"><span data-stu-id="22833-458">Configure the user information that is displayed when the session is locked.</span></span> <span data-ttu-id="22833-459">如果未配置，将显示显示名称、域和用户名。</span><span class="sxs-lookup"><span data-stu-id="22833-459">If not configured, user display name, domain and username are shown.</span></span> <span data-ttu-id="22833-460">可取值为：`notConfigured`、`userDisplayNameDomainUser`、`userDisplayNameOnly`、`doNotDisplayUser`。</span><span class="sxs-lookup"><span data-stu-id="22833-460">Possible values are: `notConfigured`, `userDisplayNameDomainUser`, `userDisplayNameOnly`, `doNotDisplayUser`.</span></span>|
|<span data-ttu-id="22833-461">localSecurityOptionsInformationDisplayedOnLockScreen</span><span class="sxs-lookup"><span data-stu-id="22833-461">localSecurityOptionsInformationDisplayedOnLockScreen</span></span>|[<span data-ttu-id="22833-462">localSecurityOptionsInformationDisplayedOnLockScreenType</span><span class="sxs-lookup"><span data-stu-id="22833-462">localSecurityOptionsInformationDisplayedOnLockScreenType</span></span>](../resources/intune-deviceconfig-localsecurityoptionsinformationdisplayedonlockscreentype.md)|<span data-ttu-id="22833-463">配置在会话锁定时显示的用户信息。</span><span class="sxs-lookup"><span data-stu-id="22833-463">Configure the user information that is displayed when the session is locked.</span></span> <span data-ttu-id="22833-464">如果未配置，将显示显示名称、域和用户名。</span><span class="sxs-lookup"><span data-stu-id="22833-464">If not configured, user display name, domain and username are shown.</span></span> <span data-ttu-id="22833-465">可取值为：`notConfigured`、`administrators`、`administratorsAndPowerUsers`、`administratorsAndInteractiveUsers`。</span><span class="sxs-lookup"><span data-stu-id="22833-465">Possible values are: `notConfigured`, `administrators`, `administratorsAndPowerUsers`, `administratorsAndInteractiveUsers`.</span></span>|
|<span data-ttu-id="22833-466">localSecurityOptionsDisableClientDigitallySignCommunicationsIfServerAgrees</span><span class="sxs-lookup"><span data-stu-id="22833-466">localSecurityOptionsDisableClientDigitallySignCommunicationsIfServerAgrees</span></span>|<span data-ttu-id="22833-467">Boolean</span><span class="sxs-lookup"><span data-stu-id="22833-467">Boolean</span></span>|<span data-ttu-id="22833-468">此安全性设置确定 SMB 客户端是否尝试协商 SMB 数据包签名。</span><span class="sxs-lookup"><span data-stu-id="22833-468">This security setting determines whether the SMB client attempts to negotiate SMB packet signing.</span></span>|
|<span data-ttu-id="22833-469">localSecurityOptionsClientDigitallySignCommunicationsAlways</span><span class="sxs-lookup"><span data-stu-id="22833-469">localSecurityOptionsClientDigitallySignCommunicationsAlways</span></span>|<span data-ttu-id="22833-470">Boolean</span><span class="sxs-lookup"><span data-stu-id="22833-470">Boolean</span></span>|<span data-ttu-id="22833-471">此安全性设置确定 SMB 客户端组件是否需要数据包签名。</span><span class="sxs-lookup"><span data-stu-id="22833-471">This security setting determines whether packet signing is required by the SMB client component.</span></span>|
|<span data-ttu-id="22833-472">localSecurityOptionsClientSendUnencryptedPasswordToThirdPartySMBServers</span><span class="sxs-lookup"><span data-stu-id="22833-472">localSecurityOptionsClientSendUnencryptedPasswordToThirdPartySMBServers</span></span>|<span data-ttu-id="22833-473">Boolean</span><span class="sxs-lookup"><span data-stu-id="22833-473">Boolean</span></span>|<span data-ttu-id="22833-474">如果启用此安全性设置，则允许服务器消息阻止 (SMB) 重定向程序向在身份验证期间不支持密码加密的非 Microsoft SMB 服务器发送纯文本密码。</span><span class="sxs-lookup"><span data-stu-id="22833-474">If this security setting is enabled, the Server Message Block (SMB) redirector is allowed to send plaintext passwords to non-Microsoft SMB servers that do not support password encryption during authentication.</span></span>|
|<span data-ttu-id="22833-475">localSecurityOptionsDisableServerDigitallySignCommunicationsAlways</span><span class="sxs-lookup"><span data-stu-id="22833-475">localSecurityOptionsDisableServerDigitallySignCommunicationsAlways</span></span>|<span data-ttu-id="22833-476">Boolean</span><span class="sxs-lookup"><span data-stu-id="22833-476">Boolean</span></span>|<span data-ttu-id="22833-477">此安全性设置确定 SMB 服务器组件是否需要数据包签名。</span><span class="sxs-lookup"><span data-stu-id="22833-477">This security setting determines whether packet signing is required by the SMB server component.</span></span>|
|<span data-ttu-id="22833-478">localSecurityOptionsDisableServerDigitallySignCommunicationsIfClientAgrees</span><span class="sxs-lookup"><span data-stu-id="22833-478">localSecurityOptionsDisableServerDigitallySignCommunicationsIfClientAgrees</span></span>|<span data-ttu-id="22833-479">Boolean</span><span class="sxs-lookup"><span data-stu-id="22833-479">Boolean</span></span>|<span data-ttu-id="22833-480">此安全性设置确定 SMB 服务器是否与请求它的客户端协商 SMB 数据包签名。</span><span class="sxs-lookup"><span data-stu-id="22833-480">This security setting determines whether the SMB server will negotiate SMB packet signing with clients that request it.</span></span>|
|<span data-ttu-id="22833-481">localSecurityOptionsRestrictAnonymousAccessToNamedPipesAndShares</span><span class="sxs-lookup"><span data-stu-id="22833-481">localSecurityOptionsRestrictAnonymousAccessToNamedPipesAndShares</span></span>|<span data-ttu-id="22833-482">Boolean</span><span class="sxs-lookup"><span data-stu-id="22833-482">Boolean</span></span>|<span data-ttu-id="22833-483">默认情况下，此安全设置限制匿名访问共享和通过管道访问可匿名访问的命名管道和可匿名访问的共享的设置</span><span class="sxs-lookup"><span data-stu-id="22833-483">By default, this security setting restricts anonymous access to shares and pipes to the settings for named pipes that can be accessed anonymously and Shares that can be accessed anonymously</span></span>|
|<span data-ttu-id="22833-484">localSecurityOptionsDoNotAllowAnonymousEnumerationOfSAMAccounts</span><span class="sxs-lookup"><span data-stu-id="22833-484">localSecurityOptionsDoNotAllowAnonymousEnumerationOfSAMAccounts</span></span>|<span data-ttu-id="22833-485">Boolean</span><span class="sxs-lookup"><span data-stu-id="22833-485">Boolean</span></span>|<span data-ttu-id="22833-486">此安全性设置确定将为与计算机的匿名连接授予哪些附加权限。</span><span class="sxs-lookup"><span data-stu-id="22833-486">This security setting determines what additional permissions will be granted for anonymous connections to the computer.</span></span>|
|<span data-ttu-id="22833-487">localSecurityOptionsAllowAnonymousEnumerationOfSAMAccountsAndShares</span><span class="sxs-lookup"><span data-stu-id="22833-487">localSecurityOptionsAllowAnonymousEnumerationOfSAMAccountsAndShares</span></span>|<span data-ttu-id="22833-488">Boolean</span><span class="sxs-lookup"><span data-stu-id="22833-488">Boolean</span></span>|<span data-ttu-id="22833-489">此安全设置确定是否允许匿名用户执行某些活动，例如枚举域帐户和网络共享的名称。</span><span class="sxs-lookup"><span data-stu-id="22833-489">This security setting determines whether to allows anonymous users to perform certain activities, such as enumerating the names of domain accounts and network shares.</span></span>|
|<span data-ttu-id="22833-490">localSecurityOptionsDoNotStoreLANManagerHashValueOnNextPasswordChange</span><span class="sxs-lookup"><span data-stu-id="22833-490">localSecurityOptionsDoNotStoreLANManagerHashValueOnNextPasswordChange</span></span>|<span data-ttu-id="22833-491">Boolean</span><span class="sxs-lookup"><span data-stu-id="22833-491">Boolean</span></span>|<span data-ttu-id="22833-492">此安全设置确定是否在下次更改密码时存储 LAN 管理器 (LM) 存储新密码的哈希值。</span><span class="sxs-lookup"><span data-stu-id="22833-492">This security setting determines if, at the next password change, the LAN Manager (LM) hash value for the new password is stored.</span></span> <span data-ttu-id="22833-493">默认情况下不存储它。</span><span class="sxs-lookup"><span data-stu-id="22833-493">It’s not stored by default.</span></span>|
|<span data-ttu-id="22833-494">localSecurityOptionsSmartCardRemovalBehavior</span><span class="sxs-lookup"><span data-stu-id="22833-494">localSecurityOptionsSmartCardRemovalBehavior</span></span>|[<span data-ttu-id="22833-495">localSecurityOptionsSmartCardRemovalBehaviorType</span><span class="sxs-lookup"><span data-stu-id="22833-495">localSecurityOptionsSmartCardRemovalBehaviorType</span></span>](../resources/intune-deviceconfig-localsecurityoptionssmartcardremovalbehaviortype.md)|<span data-ttu-id="22833-496">此安全设置确定从智能卡读卡器中删除已登录用户的智能卡时会发生什么情况。</span><span class="sxs-lookup"><span data-stu-id="22833-496">This security setting determines what happens when the smart card for a logged-on user is removed from the smart card reader.</span></span> <span data-ttu-id="22833-497">可取值为：`lockWorkstation`、`noAction`、`forceLogoff`、`disconnectRemoteDesktopSession`。</span><span class="sxs-lookup"><span data-stu-id="22833-497">Possible values are: `lockWorkstation`, `noAction`, `forceLogoff`, `disconnectRemoteDesktopSession`.</span></span>|
|<span data-ttu-id="22833-498">defenderSecurityCenterDisableAppBrowserUI</span><span class="sxs-lookup"><span data-stu-id="22833-498">defenderSecurityCenterDisableAppBrowserUI</span></span>|<span data-ttu-id="22833-499">Boolean</span><span class="sxs-lookup"><span data-stu-id="22833-499">Boolean</span></span>|<span data-ttu-id="22833-500">用于禁止显示应用和浏览器保护区域。</span><span class="sxs-lookup"><span data-stu-id="22833-500">Used to disable the display of the app and browser protection area.</span></span>|
|<span data-ttu-id="22833-501">defenderSecurityCenterDisableFamilyUI</span><span class="sxs-lookup"><span data-stu-id="22833-501">defenderSecurityCenterDisableFamilyUI</span></span>|<span data-ttu-id="22833-502">Boolean</span><span class="sxs-lookup"><span data-stu-id="22833-502">Boolean</span></span>|<span data-ttu-id="22833-503">用于禁止显示家庭选项区域。</span><span class="sxs-lookup"><span data-stu-id="22833-503">Used to disable the display of the family options area.</span></span>|
|<span data-ttu-id="22833-504">defenderSecurityCenterDisableHealthUI</span><span class="sxs-lookup"><span data-stu-id="22833-504">defenderSecurityCenterDisableHealthUI</span></span>|<span data-ttu-id="22833-505">Boolean</span><span class="sxs-lookup"><span data-stu-id="22833-505">Boolean</span></span>|<span data-ttu-id="22833-506">用于禁止显示设备性能和运行状况区域。</span><span class="sxs-lookup"><span data-stu-id="22833-506">Used to disable the display of the device performance and health area.</span></span>|
|<span data-ttu-id="22833-507">defenderSecurityCenterDisableNetworkUI</span><span class="sxs-lookup"><span data-stu-id="22833-507">defenderSecurityCenterDisableNetworkUI</span></span>|<span data-ttu-id="22833-508">Boolean</span><span class="sxs-lookup"><span data-stu-id="22833-508">Boolean</span></span>|<span data-ttu-id="22833-509">用于禁止显示防火墙和网络保护区域。</span><span class="sxs-lookup"><span data-stu-id="22833-509">Used to disable the display of the firewall and network protection area.</span></span>|
|<span data-ttu-id="22833-510">defenderSecurityCenterDisableVirusUI</span><span class="sxs-lookup"><span data-stu-id="22833-510">defenderSecurityCenterDisableVirusUI</span></span>|<span data-ttu-id="22833-511">Boolean</span><span class="sxs-lookup"><span data-stu-id="22833-511">Boolean</span></span>|<span data-ttu-id="22833-512">用于禁止显示病毒和威胁防护区域。</span><span class="sxs-lookup"><span data-stu-id="22833-512">Used to disable the display of the virus and threat protection area.</span></span>|
|<span data-ttu-id="22833-513">defenderSecurityCenterDisableAccountUI</span><span class="sxs-lookup"><span data-stu-id="22833-513">defenderSecurityCenterDisableAccountUI</span></span>|<span data-ttu-id="22833-514">Boolean</span><span class="sxs-lookup"><span data-stu-id="22833-514">Boolean</span></span>|<span data-ttu-id="22833-515">用于禁止显示帐户保护区域。</span><span class="sxs-lookup"><span data-stu-id="22833-515">Used to disable the display of the account protection area.</span></span>|
|<span data-ttu-id="22833-516">defenderSecurityCenterDisableClearTpmUI</span><span class="sxs-lookup"><span data-stu-id="22833-516">defenderSecurityCenterDisableClearTpmUI</span></span>|<span data-ttu-id="22833-517">Boolean</span><span class="sxs-lookup"><span data-stu-id="22833-517">Boolean</span></span>|<span data-ttu-id="22833-518">用于禁用"清除 TPM"按钮的显示。</span><span class="sxs-lookup"><span data-stu-id="22833-518">Used to disable the display of the Clear TPM button.</span></span>|
|<span data-ttu-id="22833-519">defenderSecurityCenterDisableHardwareUI</span><span class="sxs-lookup"><span data-stu-id="22833-519">defenderSecurityCenterDisableHardwareUI</span></span>|<span data-ttu-id="22833-520">Boolean</span><span class="sxs-lookup"><span data-stu-id="22833-520">Boolean</span></span>|<span data-ttu-id="22833-521">用于禁止显示硬件保护区域。</span><span class="sxs-lookup"><span data-stu-id="22833-521">Used to disable the display of the hardware protection area.</span></span>|
|<span data-ttu-id="22833-522">defenderSecurityCenterDisableNotificationAreaUI</span><span class="sxs-lookup"><span data-stu-id="22833-522">defenderSecurityCenterDisableNotificationAreaUI</span></span>|<span data-ttu-id="22833-523">Boolean</span><span class="sxs-lookup"><span data-stu-id="22833-523">Boolean</span></span>|<span data-ttu-id="22833-524">用于禁用通知区域控件的显示。</span><span class="sxs-lookup"><span data-stu-id="22833-524">Used to disable the display of the notification area control.</span></span> <span data-ttu-id="22833-525">用户需要注销并登录或重新启动计算机，此设置才能生效。</span><span class="sxs-lookup"><span data-stu-id="22833-525">The user needs to either sign out and sign in or reboot the computer for this setting to take effect.</span></span>|
|<span data-ttu-id="22833-526">defenderSecurityCenterDisableRansomwareUI</span><span class="sxs-lookup"><span data-stu-id="22833-526">defenderSecurityCenterDisableRansomwareUI</span></span>|<span data-ttu-id="22833-527">Boolean</span><span class="sxs-lookup"><span data-stu-id="22833-527">Boolean</span></span>|<span data-ttu-id="22833-528">用于禁止显示勒索软件保护区域。</span><span class="sxs-lookup"><span data-stu-id="22833-528">Used to disable the display of the ransomware protection area.</span></span> |
|<span data-ttu-id="22833-529">defenderSecurityCenterDisableSecureBootUI</span><span class="sxs-lookup"><span data-stu-id="22833-529">defenderSecurityCenterDisableSecureBootUI</span></span>|<span data-ttu-id="22833-530">Boolean</span><span class="sxs-lookup"><span data-stu-id="22833-530">Boolean</span></span>|<span data-ttu-id="22833-531">用于在"设备安全性"下禁止显示安全启动区域。</span><span class="sxs-lookup"><span data-stu-id="22833-531">Used to disable the display of the secure boot area under Device security.</span></span>|
|<span data-ttu-id="22833-532">defenderSecurityCenterDisableTroubleshootingUI</span><span class="sxs-lookup"><span data-stu-id="22833-532">defenderSecurityCenterDisableTroubleshootingUI</span></span>|<span data-ttu-id="22833-533">Boolean</span><span class="sxs-lookup"><span data-stu-id="22833-533">Boolean</span></span>|<span data-ttu-id="22833-534">用于在"设备安全性"下禁止显示安全过程疑难解答。</span><span class="sxs-lookup"><span data-stu-id="22833-534">Used to disable the display of the security process troubleshooting under Device security.</span></span>|
|<span data-ttu-id="22833-535">defenderSecurityCenterDisableVulnerableTpmFirmwareUpdateUI</span><span class="sxs-lookup"><span data-stu-id="22833-535">defenderSecurityCenterDisableVulnerableTpmFirmwareUpdateUI</span></span>|<span data-ttu-id="22833-536">Boolean</span><span class="sxs-lookup"><span data-stu-id="22833-536">Boolean</span></span>|<span data-ttu-id="22833-537">用于在检测到易受攻击的固件时禁用更新 TPM 固件的显示。</span><span class="sxs-lookup"><span data-stu-id="22833-537">Used to disable the display of update TPM Firmware when a vulnerable firmware is detected.</span></span>|
|<span data-ttu-id="22833-538">defenderSecurityCenterOrganizationDisplayName</span><span class="sxs-lookup"><span data-stu-id="22833-538">defenderSecurityCenterOrganizationDisplayName</span></span>|<span data-ttu-id="22833-539">String</span><span class="sxs-lookup"><span data-stu-id="22833-539">String</span></span>|<span data-ttu-id="22833-540">向用户显示的公司名称。</span><span class="sxs-lookup"><span data-stu-id="22833-540">The company name that is displayed to the users.</span></span>|
|<span data-ttu-id="22833-541">defenderSecurityCenterHelpEmail</span><span class="sxs-lookup"><span data-stu-id="22833-541">defenderSecurityCenterHelpEmail</span></span>|<span data-ttu-id="22833-542">String</span><span class="sxs-lookup"><span data-stu-id="22833-542">String</span></span>|<span data-ttu-id="22833-543">向用户显示的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="22833-543">The email address that is displayed to users.</span></span>|
|<span data-ttu-id="22833-544">defenderSecurityCenterHelpPhone</span><span class="sxs-lookup"><span data-stu-id="22833-544">defenderSecurityCenterHelpPhone</span></span>|<span data-ttu-id="22833-545">String</span><span class="sxs-lookup"><span data-stu-id="22833-545">String</span></span>|<span data-ttu-id="22833-546">向用户显示的电话号码或 Skype ID。</span><span class="sxs-lookup"><span data-stu-id="22833-546">The phone number or Skype ID that is displayed to users.</span></span>|
|<span data-ttu-id="22833-547">defenderSecurityCenterHelpURL</span><span class="sxs-lookup"><span data-stu-id="22833-547">defenderSecurityCenterHelpURL</span></span>|<span data-ttu-id="22833-548">String</span><span class="sxs-lookup"><span data-stu-id="22833-548">String</span></span>|<span data-ttu-id="22833-549">向用户显示的帮助门户 URL。</span><span class="sxs-lookup"><span data-stu-id="22833-549">The help portal URL this is displayed to users.</span></span>|
|<span data-ttu-id="22833-550">defenderSecurityCenterNotificationsFromApp</span><span class="sxs-lookup"><span data-stu-id="22833-550">defenderSecurityCenterNotificationsFromApp</span></span>|[<span data-ttu-id="22833-551">defenderSecurityCenterNotificationsFromAppType</span><span class="sxs-lookup"><span data-stu-id="22833-551">defenderSecurityCenterNotificationsFromAppType</span></span>](../resources/intune-deviceconfig-defendersecuritycenternotificationsfromapptype.md)|<span data-ttu-id="22833-552">从应用的显示区域显示的通知。</span><span class="sxs-lookup"><span data-stu-id="22833-552">Notifications to show from the displayed areas of app.</span></span> <span data-ttu-id="22833-553">可取值为：`notConfigured`、`blockNoncriticalNotifications`、`blockAllNotifications`。</span><span class="sxs-lookup"><span data-stu-id="22833-553">Possible values are: `notConfigured`, `blockNoncriticalNotifications`, `blockAllNotifications`.</span></span>|
|<span data-ttu-id="22833-554">defenderSecurityCenterITContactDisplay</span><span class="sxs-lookup"><span data-stu-id="22833-554">defenderSecurityCenterITContactDisplay</span></span>|[<span data-ttu-id="22833-555">defenderSecurityCenterITContactDisplayType</span><span class="sxs-lookup"><span data-stu-id="22833-555">defenderSecurityCenterITContactDisplayType</span></span>](../resources/intune-deviceconfig-defendersecuritycenteritcontactdisplaytype.md)|<span data-ttu-id="22833-556">配置向最终用户显示 IT 联系人信息的地方。</span><span class="sxs-lookup"><span data-stu-id="22833-556">Configure where to display IT contact information to end users.</span></span> <span data-ttu-id="22833-557">可取值为：`notConfigured`、`displayInAppAndInNotifications`、`displayOnlyInApp`、`displayOnlyInNotifications`。</span><span class="sxs-lookup"><span data-stu-id="22833-557">Possible values are: `notConfigured`, `displayInAppAndInNotifications`, `displayOnlyInApp`, `displayOnlyInNotifications`.</span></span>|
|<span data-ttu-id="22833-558">windowsDefenderTamperProtection</span><span class="sxs-lookup"><span data-stu-id="22833-558">windowsDefenderTamperProtection</span></span>|[<span data-ttu-id="22833-559">windowsDefenderTamperProtectionOptions</span><span class="sxs-lookup"><span data-stu-id="22833-559">windowsDefenderTamperProtectionOptions</span></span>](../resources/intune-deviceconfig-windowsdefendertamperprotectionoptions.md)|<span data-ttu-id="22833-560">配置 windows defender TamperProtection 设置。</span><span class="sxs-lookup"><span data-stu-id="22833-560">Configure windows defender TamperProtection settings.</span></span> <span data-ttu-id="22833-561">可取值为：`notConfigured`、`enable`、`disable`。</span><span class="sxs-lookup"><span data-stu-id="22833-561">Possible values are: `notConfigured`, `enable`, `disable`.</span></span>|
|<span data-ttu-id="22833-562">firewallBlockStatefulFTP</span><span class="sxs-lookup"><span data-stu-id="22833-562">firewallBlockStatefulFTP</span></span>|<span data-ttu-id="22833-563">Boolean</span><span class="sxs-lookup"><span data-stu-id="22833-563">Boolean</span></span>|<span data-ttu-id="22833-564">阻止到设备的有状态 FTP 连接</span><span class="sxs-lookup"><span data-stu-id="22833-564">Blocks stateful FTP connections to the device</span></span>|
|<span data-ttu-id="22833-565">firewallIdleTimeoutForSecurityAssociationInSeconds</span><span class="sxs-lookup"><span data-stu-id="22833-565">firewallIdleTimeoutForSecurityAssociationInSeconds</span></span>|<span data-ttu-id="22833-566">Int32</span><span class="sxs-lookup"><span data-stu-id="22833-566">Int32</span></span>|<span data-ttu-id="22833-567">配置安全关联的空闲超时（以秒为单位），值范围为 300 到 3600（包括这两个值）。</span><span class="sxs-lookup"><span data-stu-id="22833-567">Configures the idle timeout for security associations, in seconds, from 300 to 3600 inclusive.</span></span> <span data-ttu-id="22833-568">这是一个时间段，在此之后安全关联将过期并被删除。</span><span class="sxs-lookup"><span data-stu-id="22833-568">This is the period after which security associations will expire and be deleted.</span></span> <span data-ttu-id="22833-569">有效值为 300 至 3600</span><span class="sxs-lookup"><span data-stu-id="22833-569">Valid values 300 to 3600</span></span>|
|<span data-ttu-id="22833-570">firewallPreSharedKeyEncodingMethod</span><span class="sxs-lookup"><span data-stu-id="22833-570">firewallPreSharedKeyEncodingMethod</span></span>|[<span data-ttu-id="22833-571">firewallPreSharedKeyEncodingMethodType</span><span class="sxs-lookup"><span data-stu-id="22833-571">firewallPreSharedKeyEncodingMethodType</span></span>](../resources/intune-deviceconfig-firewallpresharedkeyencodingmethodtype.md)|<span data-ttu-id="22833-572">选择要使用的预共享密钥编码。</span><span class="sxs-lookup"><span data-stu-id="22833-572">Select the preshared key encoding to be used.</span></span> <span data-ttu-id="22833-573">可取值为：`deviceDefault`、`none`、`utF8`。</span><span class="sxs-lookup"><span data-stu-id="22833-573">Possible values are: `deviceDefault`, `none`, `utF8`.</span></span>|
|<span data-ttu-id="22833-574">firewallIPSecExemptionsNone</span><span class="sxs-lookup"><span data-stu-id="22833-574">firewallIPSecExemptionsNone</span></span>|<span data-ttu-id="22833-575">Boolean</span><span class="sxs-lookup"><span data-stu-id="22833-575">Boolean</span></span>|<span data-ttu-id="22833-576">将 IPSec 豁免配置为无免除</span><span class="sxs-lookup"><span data-stu-id="22833-576">Configures IPSec exemptions to no exemptions</span></span>|
|<span data-ttu-id="22833-577">firewallIPSecExemptionsAllowNeighborDiscovery</span><span class="sxs-lookup"><span data-stu-id="22833-577">firewallIPSecExemptionsAllowNeighborDiscovery</span></span>|<span data-ttu-id="22833-578">Boolean</span><span class="sxs-lookup"><span data-stu-id="22833-578">Boolean</span></span>|<span data-ttu-id="22833-579">配置 IPSec 免除项以允许邻居发现 IPv6 ICMP 类型代码</span><span class="sxs-lookup"><span data-stu-id="22833-579">Configures IPSec exemptions to allow neighbor discovery IPv6 ICMP type-codes</span></span>|
|<span data-ttu-id="22833-580">firewallIPSecExemptionsAllowICMP</span><span class="sxs-lookup"><span data-stu-id="22833-580">firewallIPSecExemptionsAllowICMP</span></span>|<span data-ttu-id="22833-581">Boolean</span><span class="sxs-lookup"><span data-stu-id="22833-581">Boolean</span></span>|<span data-ttu-id="22833-582">配置 IPSec 免除项以允许 ICMP</span><span class="sxs-lookup"><span data-stu-id="22833-582">Configures IPSec exemptions to allow ICMP</span></span>|
|<span data-ttu-id="22833-583">firewallIPSecExemptionsAllowRouterDiscovery</span><span class="sxs-lookup"><span data-stu-id="22833-583">firewallIPSecExemptionsAllowRouterDiscovery</span></span>|<span data-ttu-id="22833-584">Boolean</span><span class="sxs-lookup"><span data-stu-id="22833-584">Boolean</span></span>|<span data-ttu-id="22833-585">配置 IPSec 免除项以允许路由器发现 IPv6 ICMP 类型代码</span><span class="sxs-lookup"><span data-stu-id="22833-585">Configures IPSec exemptions to allow router discovery IPv6 ICMP type-codes</span></span>|
|<span data-ttu-id="22833-586">firewallIPSecExemptionsAllowDHCP</span><span class="sxs-lookup"><span data-stu-id="22833-586">firewallIPSecExemptionsAllowDHCP</span></span>|<span data-ttu-id="22833-587">Boolean</span><span class="sxs-lookup"><span data-stu-id="22833-587">Boolean</span></span>|<span data-ttu-id="22833-588">配置 IPSec 免除项以允许 IPv4 和 IPv6 DHCP 通信</span><span class="sxs-lookup"><span data-stu-id="22833-588">Configures IPSec exemptions to allow both IPv4 and IPv6 DHCP traffic</span></span>|
|<span data-ttu-id="22833-589">firewallCertificateRevocationListCheckMethod</span><span class="sxs-lookup"><span data-stu-id="22833-589">firewallCertificateRevocationListCheckMethod</span></span>|[<span data-ttu-id="22833-590">firewallCertificateRevocationListCheckMethodType</span><span class="sxs-lookup"><span data-stu-id="22833-590">firewallCertificateRevocationListCheckMethodType</span></span>](../resources/intune-deviceconfig-firewallcertificaterevocationlistcheckmethodtype.md)|<span data-ttu-id="22833-591">指定如何强制执行证书吊销列表。</span><span class="sxs-lookup"><span data-stu-id="22833-591">Specify how the certificate revocation list is to be enforced.</span></span> <span data-ttu-id="22833-592">可取值为：`deviceDefault`、`none`、`attempt`、`require`。</span><span class="sxs-lookup"><span data-stu-id="22833-592">Possible values are: `deviceDefault`, `none`, `attempt`, `require`.</span></span>|
|<span data-ttu-id="22833-593">firewallMergeKeyingModuleSettings</span><span class="sxs-lookup"><span data-stu-id="22833-593">firewallMergeKeyingModuleSettings</span></span>|<span data-ttu-id="22833-594">Boolean</span><span class="sxs-lookup"><span data-stu-id="22833-594">Boolean</span></span>|<span data-ttu-id="22833-595">如果键控模块不完全支持身份验证集，请指示模块仅忽略不受支持的身份验证套件而不是整个集</span><span class="sxs-lookup"><span data-stu-id="22833-595">If an authentication set is not fully supported by a keying module, direct the module to ignore only unsupported authentication suites rather than the entire set</span></span>|
|<span data-ttu-id="22833-596">firewallPacketQueueingMethod</span><span class="sxs-lookup"><span data-stu-id="22833-596">firewallPacketQueueingMethod</span></span>|[<span data-ttu-id="22833-597">firewallPacketQueueingMethodType</span><span class="sxs-lookup"><span data-stu-id="22833-597">firewallPacketQueueingMethodType</span></span>](../resources/intune-deviceconfig-firewallpacketqueueingmethodtype.md)|<span data-ttu-id="22833-598">配置如何在隧道网关方案中应用数据包排队。</span><span class="sxs-lookup"><span data-stu-id="22833-598">Configures how packet queueing should be applied in the tunnel gateway scenario.</span></span> <span data-ttu-id="22833-599">可取值为：`deviceDefault`、`disabled`、`queueInbound`、`queueOutbound`、`queueBoth`。</span><span class="sxs-lookup"><span data-stu-id="22833-599">Possible values are: `deviceDefault`, `disabled`, `queueInbound`, `queueOutbound`, `queueBoth`.</span></span>|
|<span data-ttu-id="22833-600">firewallProfileDomain</span><span class="sxs-lookup"><span data-stu-id="22833-600">firewallProfileDomain</span></span>|[<span data-ttu-id="22833-601">windowsFirewallNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="22833-601">windowsFirewallNetworkProfile</span></span>](../resources/intune-deviceconfig-windowsfirewallnetworkprofile.md)|<span data-ttu-id="22833-602">配置域网络的防火墙配置文件设置</span><span class="sxs-lookup"><span data-stu-id="22833-602">Configures the firewall profile settings for domain networks</span></span>|
|<span data-ttu-id="22833-603">firewallProfilePublic</span><span class="sxs-lookup"><span data-stu-id="22833-603">firewallProfilePublic</span></span>|[<span data-ttu-id="22833-604">windowsFirewallNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="22833-604">windowsFirewallNetworkProfile</span></span>](../resources/intune-deviceconfig-windowsfirewallnetworkprofile.md)|<span data-ttu-id="22833-605">配置公用网络的防火墙配置文件设置</span><span class="sxs-lookup"><span data-stu-id="22833-605">Configures the firewall profile settings for public networks</span></span>|
|<span data-ttu-id="22833-606">firewallProfilePrivate</span><span class="sxs-lookup"><span data-stu-id="22833-606">firewallProfilePrivate</span></span>|[<span data-ttu-id="22833-607">windowsFirewallNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="22833-607">windowsFirewallNetworkProfile</span></span>](../resources/intune-deviceconfig-windowsfirewallnetworkprofile.md)|<span data-ttu-id="22833-608">配置专用网络的防火墙配置文件设置</span><span class="sxs-lookup"><span data-stu-id="22833-608">Configures the firewall profile settings for private networks</span></span>|
|<span data-ttu-id="22833-609">defenderAdobeReaderLaunchChildProcess</span><span class="sxs-lookup"><span data-stu-id="22833-609">defenderAdobeReaderLaunchChildProcess</span></span>|[<span data-ttu-id="22833-610">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="22833-610">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="22833-611">指示 Adobe Reader 创建子进程的行为的值。</span><span class="sxs-lookup"><span data-stu-id="22833-611">Value indicating the behavior of Adobe Reader from creating child processes.</span></span> <span data-ttu-id="22833-612">可取值为：`userDefined`、`enable`、`auditMode`、`warn`、`notConfigured`。</span><span class="sxs-lookup"><span data-stu-id="22833-612">Possible values are: `userDefined`, `enable`, `auditMode`, `warn`, `notConfigured`.</span></span>|
|<span data-ttu-id="22833-613">defenderAttackSurfaceReductionExcludedPaths</span><span class="sxs-lookup"><span data-stu-id="22833-613">defenderAttackSurfaceReductionExcludedPaths</span></span>|<span data-ttu-id="22833-614">String 集合</span><span class="sxs-lookup"><span data-stu-id="22833-614">String collection</span></span>|<span data-ttu-id="22833-615">要从攻击面减少规则中排除的 exe 文件和文件夹的列表</span><span class="sxs-lookup"><span data-stu-id="22833-615">List of exe files and folders to be excluded from attack surface reduction rules</span></span>|
|<span data-ttu-id="22833-616">defenderOfficeAppsOtherProcessInjectionType</span><span class="sxs-lookup"><span data-stu-id="22833-616">defenderOfficeAppsOtherProcessInjectionType</span></span>|[<span data-ttu-id="22833-617">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="22833-617">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="22833-618">指示注入其他进程中的 Office 应用程序的行为的值。</span><span class="sxs-lookup"><span data-stu-id="22833-618">Value indicating the behavior of Office applications injecting into other processes.</span></span> <span data-ttu-id="22833-619">可取值为：`userDefined`、`block`、`auditMode`、`warn`、`disable`。</span><span class="sxs-lookup"><span data-stu-id="22833-619">Possible values are: `userDefined`, `block`, `auditMode`, `warn`, `disable`.</span></span>|
|<span data-ttu-id="22833-620">defenderOfficeAppsOtherProcessInjection</span><span class="sxs-lookup"><span data-stu-id="22833-620">defenderOfficeAppsOtherProcessInjection</span></span>|[<span data-ttu-id="22833-621">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="22833-621">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="22833-622">指示注入其他进程中的 Office 应用程序的行为的值。</span><span class="sxs-lookup"><span data-stu-id="22833-622">Value indicating the behavior of  Office applications injecting into other processes.</span></span> <span data-ttu-id="22833-623">可取值为：`userDefined`、`enable`、`auditMode`、`warn`、`notConfigured`。</span><span class="sxs-lookup"><span data-stu-id="22833-623">Possible values are: `userDefined`, `enable`, `auditMode`, `warn`, `notConfigured`.</span></span>|
|<span data-ttu-id="22833-624">defenderOfficeCommunicationAppsLaunchChildProcess</span><span class="sxs-lookup"><span data-stu-id="22833-624">defenderOfficeCommunicationAppsLaunchChildProcess</span></span>|[<span data-ttu-id="22833-625">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="22833-625">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="22833-626">指示 Office 通信应用程序（包括 Microsoft Outlook）创建子进程的行为的值。</span><span class="sxs-lookup"><span data-stu-id="22833-626">Value indicating the behavior of Office communication applications, including Microsoft Outlook, from creating child processes.</span></span> <span data-ttu-id="22833-627">可取值为：`userDefined`、`enable`、`auditMode`、`warn`、`notConfigured`。</span><span class="sxs-lookup"><span data-stu-id="22833-627">Possible values are: `userDefined`, `enable`, `auditMode`, `warn`, `notConfigured`.</span></span>|
|<span data-ttu-id="22833-628">defenderOfficeAppsExecutableContentCreationOrLaunchType</span><span class="sxs-lookup"><span data-stu-id="22833-628">defenderOfficeAppsExecutableContentCreationOrLaunchType</span></span>|[<span data-ttu-id="22833-629">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="22833-629">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="22833-630">指示 Office 应用程序/宏创建或启动可执行内容的行为的值。</span><span class="sxs-lookup"><span data-stu-id="22833-630">Value indicating the behavior of Office applications/macros creating or launching executable content.</span></span> <span data-ttu-id="22833-631">可取值为：`userDefined`、`block`、`auditMode`、`warn`、`disable`。</span><span class="sxs-lookup"><span data-stu-id="22833-631">Possible values are: `userDefined`, `block`, `auditMode`, `warn`, `disable`.</span></span>|
|<span data-ttu-id="22833-632">defenderOfficeAppsExecutableContentCreationOrLaunch</span><span class="sxs-lookup"><span data-stu-id="22833-632">defenderOfficeAppsExecutableContentCreationOrLaunch</span></span>|[<span data-ttu-id="22833-633">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="22833-633">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="22833-634">指示 Office 应用程序/宏创建或启动可执行内容的行为的值。</span><span class="sxs-lookup"><span data-stu-id="22833-634">Value indicating the behavior of Office applications/macros creating or launching executable content.</span></span> <span data-ttu-id="22833-635">可取值为：`userDefined`、`enable`、`auditMode`、`warn`、`notConfigured`。</span><span class="sxs-lookup"><span data-stu-id="22833-635">Possible values are: `userDefined`, `enable`, `auditMode`, `warn`, `notConfigured`.</span></span>|
|<span data-ttu-id="22833-636">defenderOfficeAppsLaunchChildProcessType</span><span class="sxs-lookup"><span data-stu-id="22833-636">defenderOfficeAppsLaunchChildProcessType</span></span>|[<span data-ttu-id="22833-637">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="22833-637">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="22833-638">指示 Office 应用程序启动子进程的行为的值。</span><span class="sxs-lookup"><span data-stu-id="22833-638">Value indicating the behavior of Office application launching child processes.</span></span> <span data-ttu-id="22833-639">可取值为：`userDefined`、`block`、`auditMode`、`warn`、`disable`。</span><span class="sxs-lookup"><span data-stu-id="22833-639">Possible values are: `userDefined`, `block`, `auditMode`, `warn`, `disable`.</span></span>|
|<span data-ttu-id="22833-640">defenderOfficeAppsLaunchChildProcess</span><span class="sxs-lookup"><span data-stu-id="22833-640">defenderOfficeAppsLaunchChildProcess</span></span>|[<span data-ttu-id="22833-641">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="22833-641">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="22833-642">指示 Office 应用程序启动子进程的行为的值。</span><span class="sxs-lookup"><span data-stu-id="22833-642">Value indicating the behavior of Office application launching child processes.</span></span> <span data-ttu-id="22833-643">可取值为：`userDefined`、`enable`、`auditMode`、`warn`、`notConfigured`。</span><span class="sxs-lookup"><span data-stu-id="22833-643">Possible values are: `userDefined`, `enable`, `auditMode`, `warn`, `notConfigured`.</span></span>|
|<span data-ttu-id="22833-644">defenderOfficeMacroCodeAllowWin32ImportsType</span><span class="sxs-lookup"><span data-stu-id="22833-644">defenderOfficeMacroCodeAllowWin32ImportsType</span></span>|[<span data-ttu-id="22833-645">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="22833-645">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="22833-646">指示 Win32 从 Office 中的宏代码导入的行为的值。</span><span class="sxs-lookup"><span data-stu-id="22833-646">Value indicating the behavior of Win32 imports from Macro code in Office.</span></span> <span data-ttu-id="22833-647">可取值为：`userDefined`、`block`、`auditMode`、`warn`、`disable`。</span><span class="sxs-lookup"><span data-stu-id="22833-647">Possible values are: `userDefined`, `block`, `auditMode`, `warn`, `disable`.</span></span>|
|<span data-ttu-id="22833-648">defenderOfficeMacroCodeAllowWin32Imports</span><span class="sxs-lookup"><span data-stu-id="22833-648">defenderOfficeMacroCodeAllowWin32Imports</span></span>|[<span data-ttu-id="22833-649">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="22833-649">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="22833-650">指示 Win32 从 Office 中的宏代码导入的行为的值。</span><span class="sxs-lookup"><span data-stu-id="22833-650">Value indicating the behavior of Win32 imports from Macro code in Office.</span></span> <span data-ttu-id="22833-651">可取值为：`userDefined`、`enable`、`auditMode`、`warn`、`notConfigured`。</span><span class="sxs-lookup"><span data-stu-id="22833-651">Possible values are: `userDefined`, `enable`, `auditMode`, `warn`, `notConfigured`.</span></span>|
|<span data-ttu-id="22833-652">defenderScriptObfuscatedMacroCodeType</span><span class="sxs-lookup"><span data-stu-id="22833-652">defenderScriptObfuscatedMacroCodeType</span></span>|[<span data-ttu-id="22833-653">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="22833-653">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="22833-654">指示混淆的 js/vbs/ps/宏代码的行为的值。</span><span class="sxs-lookup"><span data-stu-id="22833-654">Value indicating the behavior of obfuscated js/vbs/ps/macro code.</span></span> <span data-ttu-id="22833-655">可取值为：`userDefined`、`block`、`auditMode`、`warn`、`disable`。</span><span class="sxs-lookup"><span data-stu-id="22833-655">Possible values are: `userDefined`, `block`, `auditMode`, `warn`, `disable`.</span></span>|
|<span data-ttu-id="22833-656">defenderScriptObfuscatedMacroCode</span><span class="sxs-lookup"><span data-stu-id="22833-656">defenderScriptObfuscatedMacroCode</span></span>|[<span data-ttu-id="22833-657">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="22833-657">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="22833-658">指示混淆的 js/vbs/ps/宏代码的行为的值。</span><span class="sxs-lookup"><span data-stu-id="22833-658">Value indicating the behavior of obfuscated js/vbs/ps/macro code.</span></span> <span data-ttu-id="22833-659">可取值为：`userDefined`、`enable`、`auditMode`、`warn`、`notConfigured`。</span><span class="sxs-lookup"><span data-stu-id="22833-659">Possible values are: `userDefined`, `enable`, `auditMode`, `warn`, `notConfigured`.</span></span>|
|<span data-ttu-id="22833-660">defenderScriptDownloadedPayloadExecutionType</span><span class="sxs-lookup"><span data-stu-id="22833-660">defenderScriptDownloadedPayloadExecutionType</span></span>|[<span data-ttu-id="22833-661">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="22833-661">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="22833-662">指示 js/vbs 执行从 Internet 下载的有效负载的行为的值。</span><span class="sxs-lookup"><span data-stu-id="22833-662">Value indicating the behavior of js/vbs executing payload downloaded from Internet.</span></span> <span data-ttu-id="22833-663">可取值为：`userDefined`、`block`、`auditMode`、`warn`、`disable`。</span><span class="sxs-lookup"><span data-stu-id="22833-663">Possible values are: `userDefined`, `block`, `auditMode`, `warn`, `disable`.</span></span>|
|<span data-ttu-id="22833-664">defenderScriptDownloadedPayloadExecution</span><span class="sxs-lookup"><span data-stu-id="22833-664">defenderScriptDownloadedPayloadExecution</span></span>|[<span data-ttu-id="22833-665">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="22833-665">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="22833-666">指示 js/vbs 执行从 Internet 下载的有效负载的行为的值。</span><span class="sxs-lookup"><span data-stu-id="22833-666">Value indicating the behavior of js/vbs executing payload downloaded from Internet.</span></span> <span data-ttu-id="22833-667">可取值为：`userDefined`、`enable`、`auditMode`、`warn`、`notConfigured`。</span><span class="sxs-lookup"><span data-stu-id="22833-667">Possible values are: `userDefined`, `enable`, `auditMode`, `warn`, `notConfigured`.</span></span>|
|<span data-ttu-id="22833-668">defenderPreventCredentialStealingType</span><span class="sxs-lookup"><span data-stu-id="22833-668">defenderPreventCredentialStealingType</span></span>|[<span data-ttu-id="22833-669">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="22833-669">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="22833-670">指示是否允许从 Windows 本地安全机构子系统窃取凭据的值。</span><span class="sxs-lookup"><span data-stu-id="22833-670">Value indicating if credential stealing from the Windows local security authority subsystem is permitted.</span></span> <span data-ttu-id="22833-671">可取值为：`userDefined`、`enable`、`auditMode`、`warn`、`notConfigured`。</span><span class="sxs-lookup"><span data-stu-id="22833-671">Possible values are: `userDefined`, `enable`, `auditMode`, `warn`, `notConfigured`.</span></span>|
|<span data-ttu-id="22833-672">defenderProcessCreationType</span><span class="sxs-lookup"><span data-stu-id="22833-672">defenderProcessCreationType</span></span>|[<span data-ttu-id="22833-673">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="22833-673">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="22833-674">指示对源自 PSExec 和 WMI 命令的进程创建的响应的值。</span><span class="sxs-lookup"><span data-stu-id="22833-674">Value indicating response to process creations originating from PSExec and WMI commands.</span></span> <span data-ttu-id="22833-675">可取值为：`userDefined`、`block`、`auditMode`、`warn`、`disable`。</span><span class="sxs-lookup"><span data-stu-id="22833-675">Possible values are: `userDefined`, `block`, `auditMode`, `warn`, `disable`.</span></span>|
|<span data-ttu-id="22833-676">defenderProcessCreation</span><span class="sxs-lookup"><span data-stu-id="22833-676">defenderProcessCreation</span></span>|[<span data-ttu-id="22833-677">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="22833-677">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="22833-678">指示对源自 PSExec 和 WMI 命令的进程创建的响应的值。</span><span class="sxs-lookup"><span data-stu-id="22833-678">Value indicating response to process creations originating from PSExec and WMI commands.</span></span> <span data-ttu-id="22833-679">可取值为：`userDefined`、`enable`、`auditMode`、`warn`、`notConfigured`。</span><span class="sxs-lookup"><span data-stu-id="22833-679">Possible values are: `userDefined`, `enable`, `auditMode`, `warn`, `notConfigured`.</span></span>|
|<span data-ttu-id="22833-680">defenderUntrustedUSBProcessType</span><span class="sxs-lookup"><span data-stu-id="22833-680">defenderUntrustedUSBProcessType</span></span>|[<span data-ttu-id="22833-681">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="22833-681">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="22833-682">指示对从 USB 运行的不受信任的和未签名进程的响应的值。</span><span class="sxs-lookup"><span data-stu-id="22833-682">Value indicating response to untrusted and unsigned processes that run from USB.</span></span> <span data-ttu-id="22833-683">可取值为：`userDefined`、`block`、`auditMode`、`warn`、`disable`。</span><span class="sxs-lookup"><span data-stu-id="22833-683">Possible values are: `userDefined`, `block`, `auditMode`, `warn`, `disable`.</span></span>|
|<span data-ttu-id="22833-684">defenderUntrustedUSBProcess</span><span class="sxs-lookup"><span data-stu-id="22833-684">defenderUntrustedUSBProcess</span></span>|[<span data-ttu-id="22833-685">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="22833-685">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="22833-686">指示对从 USB 运行的不受信任的和未签名进程的响应的值。</span><span class="sxs-lookup"><span data-stu-id="22833-686">Value indicating response to untrusted and unsigned processes that run from USB.</span></span> <span data-ttu-id="22833-687">可取值为：`userDefined`、`enable`、`auditMode`、`warn`、`notConfigured`。</span><span class="sxs-lookup"><span data-stu-id="22833-687">Possible values are: `userDefined`, `enable`, `auditMode`, `warn`, `notConfigured`.</span></span>|
|<span data-ttu-id="22833-688">defenderUntrustedExecutableType</span><span class="sxs-lookup"><span data-stu-id="22833-688">defenderUntrustedExecutableType</span></span>|[<span data-ttu-id="22833-689">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="22833-689">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="22833-690">指示对不符合普遍程度、年龄或受信任列表条件的可执行文件的响应的值。</span><span class="sxs-lookup"><span data-stu-id="22833-690">Value indicating response to executables that don't meet a prevalence, age, or trusted list criteria.</span></span> <span data-ttu-id="22833-691">可取值为：`userDefined`、`block`、`auditMode`、`warn`、`disable`。</span><span class="sxs-lookup"><span data-stu-id="22833-691">Possible values are: `userDefined`, `block`, `auditMode`, `warn`, `disable`.</span></span>|
|<span data-ttu-id="22833-692">defenderUntrustedExecutable</span><span class="sxs-lookup"><span data-stu-id="22833-692">defenderUntrustedExecutable</span></span>|[<span data-ttu-id="22833-693">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="22833-693">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="22833-694">指示对不符合普遍程度、年龄或受信任列表条件的可执行文件的响应的值。</span><span class="sxs-lookup"><span data-stu-id="22833-694">Value indicating response to executables that don't meet a prevalence, age, or trusted list criteria.</span></span> <span data-ttu-id="22833-695">可取值为：`userDefined`、`enable`、`auditMode`、`warn`、`notConfigured`。</span><span class="sxs-lookup"><span data-stu-id="22833-695">Possible values are: `userDefined`, `enable`, `auditMode`, `warn`, `notConfigured`.</span></span>|
|<span data-ttu-id="22833-696">defenderEmailContentExecutionType</span><span class="sxs-lookup"><span data-stu-id="22833-696">defenderEmailContentExecutionType</span></span>|[<span data-ttu-id="22833-697">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="22833-697">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="22833-698">指示执行可执行内容 (exe、dll、ps、js、vbs 等) 应从电子邮件 (webmail/mail-client) 。</span><span class="sxs-lookup"><span data-stu-id="22833-698">Value indicating if execution of executable content (exe, dll, ps, js, vbs, etc) should be dropped from email (webmail/mail-client).</span></span> <span data-ttu-id="22833-699">可取值为：`userDefined`、`block`、`auditMode`、`warn`、`disable`。</span><span class="sxs-lookup"><span data-stu-id="22833-699">Possible values are: `userDefined`, `block`, `auditMode`, `warn`, `disable`.</span></span>|
|<span data-ttu-id="22833-700">defenderEmailContentExecution</span><span class="sxs-lookup"><span data-stu-id="22833-700">defenderEmailContentExecution</span></span>|[<span data-ttu-id="22833-701">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="22833-701">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="22833-702">指示执行可执行内容 (exe、dll、ps、js、vbs 等) 应从电子邮件 (webmail/mail-client) 。</span><span class="sxs-lookup"><span data-stu-id="22833-702">Value indicating if execution of executable content (exe, dll, ps, js, vbs, etc) should be dropped from email (webmail/mail-client).</span></span> <span data-ttu-id="22833-703">可取值为：`userDefined`、`enable`、`auditMode`、`warn`、`notConfigured`。</span><span class="sxs-lookup"><span data-stu-id="22833-703">Possible values are: `userDefined`, `enable`, `auditMode`, `warn`, `notConfigured`.</span></span>|
|<span data-ttu-id="22833-704">defenderAdvancedRansomewareProtectionType</span><span class="sxs-lookup"><span data-stu-id="22833-704">defenderAdvancedRansomewareProtectionType</span></span>|[<span data-ttu-id="22833-705">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="22833-705">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="22833-706">指示对勒索软件使用高级保护的值。</span><span class="sxs-lookup"><span data-stu-id="22833-706">Value indicating use of advanced protection against ransomeware.</span></span> <span data-ttu-id="22833-707">可取值为：`userDefined`、`enable`、`auditMode`、`warn`、`notConfigured`。</span><span class="sxs-lookup"><span data-stu-id="22833-707">Possible values are: `userDefined`, `enable`, `auditMode`, `warn`, `notConfigured`.</span></span>|
|<span data-ttu-id="22833-708">defenderGuardMyFoldersType</span><span class="sxs-lookup"><span data-stu-id="22833-708">defenderGuardMyFoldersType</span></span>|[<span data-ttu-id="22833-709">folderProtectionType</span><span class="sxs-lookup"><span data-stu-id="22833-709">folderProtectionType</span></span>](../resources/intune-deviceconfig-folderprotectiontype.md)|<span data-ttu-id="22833-710">指示受保护文件夹行为的值。</span><span class="sxs-lookup"><span data-stu-id="22833-710">Value indicating the behavior of protected folders.</span></span> <span data-ttu-id="22833-711">可取值为：`userDefined`、`enable`、`auditMode`、`blockDiskModification`、`auditDiskModification`。</span><span class="sxs-lookup"><span data-stu-id="22833-711">Possible values are: `userDefined`, `enable`, `auditMode`, `blockDiskModification`, `auditDiskModification`.</span></span>|
|<span data-ttu-id="22833-712">defenderGuardedFoldersAllowedAppPaths</span><span class="sxs-lookup"><span data-stu-id="22833-712">defenderGuardedFoldersAllowedAppPaths</span></span>|<span data-ttu-id="22833-713">String 集合</span><span class="sxs-lookup"><span data-stu-id="22833-713">String collection</span></span>|<span data-ttu-id="22833-714">允许访问受保护文件夹的 exe 路径列表</span><span class="sxs-lookup"><span data-stu-id="22833-714">List of paths to exe that are allowed to access protected folders</span></span>|
|<span data-ttu-id="22833-715">defenderAdditionalGuardedFolders</span><span class="sxs-lookup"><span data-stu-id="22833-715">defenderAdditionalGuardedFolders</span></span>|<span data-ttu-id="22833-716">String 集合</span><span class="sxs-lookup"><span data-stu-id="22833-716">String collection</span></span>|<span data-ttu-id="22833-717">要添加到受保护文件夹列表的文件夹路径列表</span><span class="sxs-lookup"><span data-stu-id="22833-717">List of folder paths to be added to the list of protected folders</span></span>|
|<span data-ttu-id="22833-718">defenderNetworkProtectionType</span><span class="sxs-lookup"><span data-stu-id="22833-718">defenderNetworkProtectionType</span></span>|[<span data-ttu-id="22833-719">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="22833-719">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="22833-720">指示 NetworkProtection 行为的值。</span><span class="sxs-lookup"><span data-stu-id="22833-720">Value indicating the behavior of NetworkProtection.</span></span> <span data-ttu-id="22833-721">可取值为：`userDefined`、`enable`、`auditMode`、`warn`、`notConfigured`。</span><span class="sxs-lookup"><span data-stu-id="22833-721">Possible values are: `userDefined`, `enable`, `auditMode`, `warn`, `notConfigured`.</span></span>|
|<span data-ttu-id="22833-722">defenderExploitProtectionXml</span><span class="sxs-lookup"><span data-stu-id="22833-722">defenderExploitProtectionXml</span></span>|<span data-ttu-id="22833-723">Binary</span><span class="sxs-lookup"><span data-stu-id="22833-723">Binary</span></span>|<span data-ttu-id="22833-724">包含有关 Exploit Protection 详细信息的 xml 内容。</span><span class="sxs-lookup"><span data-stu-id="22833-724">Xml content containing information regarding exploit protection details.</span></span>|
|<span data-ttu-id="22833-725">defenderExploitProtectionXmlFileName</span><span class="sxs-lookup"><span data-stu-id="22833-725">defenderExploitProtectionXmlFileName</span></span>|<span data-ttu-id="22833-726">String</span><span class="sxs-lookup"><span data-stu-id="22833-726">String</span></span>|<span data-ttu-id="22833-727">从中获取 DefenderExploitProtectionXml 的文件的名称。</span><span class="sxs-lookup"><span data-stu-id="22833-727">Name of the file from which DefenderExploitProtectionXml was obtained.</span></span>|
|<span data-ttu-id="22833-728">defenderSecurityCenterBlockExploitProtectionOverride</span><span class="sxs-lookup"><span data-stu-id="22833-728">defenderSecurityCenterBlockExploitProtectionOverride</span></span>|<span data-ttu-id="22833-729">Boolean</span><span class="sxs-lookup"><span data-stu-id="22833-729">Boolean</span></span>|<span data-ttu-id="22833-730">指示是否阻止用户覆盖 Exploit Protection 设置。</span><span class="sxs-lookup"><span data-stu-id="22833-730">Indicates whether or not to block user from overriding Exploit Protection settings.</span></span>|
|<span data-ttu-id="22833-731">defenderBlockPersistenceThroughWmiType</span><span class="sxs-lookup"><span data-stu-id="22833-731">defenderBlockPersistenceThroughWmiType</span></span>|[<span data-ttu-id="22833-732">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="22833-732">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="22833-733">指示通过 WMI 事件订阅阻止持久性的行为的值。</span><span class="sxs-lookup"><span data-stu-id="22833-733">Value indicating the behavior of Block persistence through WMI event subscription.</span></span> <span data-ttu-id="22833-734">可取值为：`userDefined`、`block`、`auditMode`、`warn`、`disable`。</span><span class="sxs-lookup"><span data-stu-id="22833-734">Possible values are: `userDefined`, `block`, `auditMode`, `warn`, `disable`.</span></span>|
|<span data-ttu-id="22833-735">appLockerApplicationControl</span><span class="sxs-lookup"><span data-stu-id="22833-735">appLockerApplicationControl</span></span>|[<span data-ttu-id="22833-736">appLockerApplicationControlType</span><span class="sxs-lookup"><span data-stu-id="22833-736">appLockerApplicationControlType</span></span>](../resources/intune-deviceconfig-applockerapplicationcontroltype.md)|<span data-ttu-id="22833-737">使管理员能够选择在设备上允许哪些类型的应用。</span><span class="sxs-lookup"><span data-stu-id="22833-737">Enables the Admin to choose what types of app to allow on devices.</span></span> <span data-ttu-id="22833-738">可取值为：`notConfigured`、`enforceComponentsAndStoreApps`、`auditComponentsAndStoreApps`、`enforceComponentsStoreAppsAndSmartlocker`、`auditComponentsStoreAppsAndSmartlocker`。</span><span class="sxs-lookup"><span data-stu-id="22833-738">Possible values are: `notConfigured`, `enforceComponentsAndStoreApps`, `auditComponentsAndStoreApps`, `enforceComponentsStoreAppsAndSmartlocker`, `auditComponentsStoreAppsAndSmartlocker`.</span></span>|
|<span data-ttu-id="22833-739">deviceGuardLocalSystemAuthorityCredentialGuardSettings</span><span class="sxs-lookup"><span data-stu-id="22833-739">deviceGuardLocalSystemAuthorityCredentialGuardSettings</span></span>|[<span data-ttu-id="22833-740">deviceGuardLocalSystemAuthorityCredentialGuardType</span><span class="sxs-lookup"><span data-stu-id="22833-740">deviceGuardLocalSystemAuthorityCredentialGuardType</span></span>](../resources/intune-deviceconfig-deviceguardlocalsystemauthoritycredentialguardtype.md)|<span data-ttu-id="22833-741">启用基于安全启动和虚拟化的安全性的平台安全级别时启用 Credential Guard。</span><span class="sxs-lookup"><span data-stu-id="22833-741">Turn on Credential Guard when Platform Security Level with Secure Boot and Virtualization Based Security are both enabled.</span></span> <span data-ttu-id="22833-742">可取值为：`notConfigured`、`enableWithUEFILock`、`enableWithoutUEFILock`、`disable`。</span><span class="sxs-lookup"><span data-stu-id="22833-742">Possible values are: `notConfigured`, `enableWithUEFILock`, `enableWithoutUEFILock`, `disable`.</span></span>|
|<span data-ttu-id="22833-743">deviceGuardEnableVirtualizationBasedSecurity</span><span class="sxs-lookup"><span data-stu-id="22833-743">deviceGuardEnableVirtualizationBasedSecurity</span></span>|<span data-ttu-id="22833-744">Boolean</span><span class="sxs-lookup"><span data-stu-id="22833-744">Boolean</span></span>|<span data-ttu-id="22833-745">启用基于虚拟化的安全性 (VBS) 。</span><span class="sxs-lookup"><span data-stu-id="22833-745">Turns On Virtualization Based Security(VBS).</span></span>|
|<span data-ttu-id="22833-746">deviceGuardEnableSecureBootWithDMA</span><span class="sxs-lookup"><span data-stu-id="22833-746">deviceGuardEnableSecureBootWithDMA</span></span>|<span data-ttu-id="22833-747">Boolean</span><span class="sxs-lookup"><span data-stu-id="22833-747">Boolean</span></span>|<span data-ttu-id="22833-748">此属性将在 2019 年 5 月弃用，并替换为属性 DeviceGuardSecureBootWithDMA。</span><span class="sxs-lookup"><span data-stu-id="22833-748">This property will be deprecated in May 2019 and will be replaced with property DeviceGuardSecureBootWithDMA.</span></span> <span data-ttu-id="22833-749">指定下次重启时是否启用平台安全级别。</span><span class="sxs-lookup"><span data-stu-id="22833-749">Specifies whether Platform Security Level is enabled at next reboot.</span></span>|
|<span data-ttu-id="22833-750">deviceGuardSecureBootWithDMA</span><span class="sxs-lookup"><span data-stu-id="22833-750">deviceGuardSecureBootWithDMA</span></span>|[<span data-ttu-id="22833-751">secureBootWithDMAType</span><span class="sxs-lookup"><span data-stu-id="22833-751">secureBootWithDMAType</span></span>](../resources/intune-deviceconfig-securebootwithdmatype.md)|<span data-ttu-id="22833-752">指定下次重启时是否启用平台安全级别。</span><span class="sxs-lookup"><span data-stu-id="22833-752">Specifies whether Platform Security Level is enabled at next reboot.</span></span> <span data-ttu-id="22833-753">可取值为：`notConfigured`、`withoutDMA`、`withDMA`。</span><span class="sxs-lookup"><span data-stu-id="22833-753">Possible values are: `notConfigured`, `withoutDMA`, `withDMA`.</span></span>|
|<span data-ttu-id="22833-754">deviceGuardLaunchSystemGuard</span><span class="sxs-lookup"><span data-stu-id="22833-754">deviceGuardLaunchSystemGuard</span></span>|[<span data-ttu-id="22833-755">enablement</span><span class="sxs-lookup"><span data-stu-id="22833-755">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="22833-756">允许 IT 管理员配置 System Guard 的启动。</span><span class="sxs-lookup"><span data-stu-id="22833-756">Allows the IT admin to configure the launch of System Guard.</span></span> <span data-ttu-id="22833-757">可取值为：`notConfigured`、`enabled`、`disabled`。</span><span class="sxs-lookup"><span data-stu-id="22833-757">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="22833-758">smartScreenEnableInShell</span><span class="sxs-lookup"><span data-stu-id="22833-758">smartScreenEnableInShell</span></span>|<span data-ttu-id="22833-759">Boolean</span><span class="sxs-lookup"><span data-stu-id="22833-759">Boolean</span></span>|<span data-ttu-id="22833-760">允许 IT 管理员配置适用于 Windows 的 SmartScreen。</span><span class="sxs-lookup"><span data-stu-id="22833-760">Allows IT Admins to configure SmartScreen for Windows.</span></span>|
|<span data-ttu-id="22833-761">smartScreenBlockOverrideForFiles</span><span class="sxs-lookup"><span data-stu-id="22833-761">smartScreenBlockOverrideForFiles</span></span>|<span data-ttu-id="22833-762">Boolean</span><span class="sxs-lookup"><span data-stu-id="22833-762">Boolean</span></span>|<span data-ttu-id="22833-763">允许 IT 管理员控制用户是否可以忽略 SmartScreen 警告并运行恶意文件。</span><span class="sxs-lookup"><span data-stu-id="22833-763">Allows IT Admins to control whether users can can ignore SmartScreen warnings and run malicious files.</span></span>|
|<span data-ttu-id="22833-764">applicationGuardEnabled</span><span class="sxs-lookup"><span data-stu-id="22833-764">applicationGuardEnabled</span></span>|<span data-ttu-id="22833-765">Boolean</span><span class="sxs-lookup"><span data-stu-id="22833-765">Boolean</span></span>|<span data-ttu-id="22833-766">启用 Windows Defender 应用程序防护</span><span class="sxs-lookup"><span data-stu-id="22833-766">Enable Windows Defender Application Guard</span></span>|
|<span data-ttu-id="22833-767">applicationGuardEnabledOptions</span><span class="sxs-lookup"><span data-stu-id="22833-767">applicationGuardEnabledOptions</span></span>|[<span data-ttu-id="22833-768">applicationGuardEnabledOptions</span><span class="sxs-lookup"><span data-stu-id="22833-768">applicationGuardEnabledOptions</span></span>](../resources/intune-deviceconfig-applicationguardenabledoptions.md)|<span data-ttu-id="22833-769">为Windows Defender Windows 版本启用应用程序防护。</span><span class="sxs-lookup"><span data-stu-id="22833-769">Enable Windows Defender Application Guard for newer Windows builds.</span></span> <span data-ttu-id="22833-770">可取值为：`notConfigured`、`enabledForEdge`、`enabledForOffice`、`enabledForEdgeAndOffice`。</span><span class="sxs-lookup"><span data-stu-id="22833-770">Possible values are: `notConfigured`, `enabledForEdge`, `enabledForOffice`, `enabledForEdgeAndOffice`.</span></span>|
|<span data-ttu-id="22833-771">applicationGuardBlockFileTransfer</span><span class="sxs-lookup"><span data-stu-id="22833-771">applicationGuardBlockFileTransfer</span></span>|[<span data-ttu-id="22833-772">applicationGuardBlockFileTransferType</span><span class="sxs-lookup"><span data-stu-id="22833-772">applicationGuardBlockFileTransferType</span></span>](../resources/intune-deviceconfig-applicationguardblockfiletransfertype.md)|<span data-ttu-id="22833-773">阻止剪贴板传输图像文件、文本文件或两者都不传输。</span><span class="sxs-lookup"><span data-stu-id="22833-773">Block clipboard to transfer image file, text file or neither of them.</span></span> <span data-ttu-id="22833-774">可取值为：`notConfigured`、`blockImageAndTextFile`、`blockImageFile`、`blockNone`、`blockTextFile`。</span><span class="sxs-lookup"><span data-stu-id="22833-774">Possible values are: `notConfigured`, `blockImageAndTextFile`, `blockImageFile`, `blockNone`, `blockTextFile`.</span></span>|
|<span data-ttu-id="22833-775">applicationGuardBlockNonEnterpriseContent</span><span class="sxs-lookup"><span data-stu-id="22833-775">applicationGuardBlockNonEnterpriseContent</span></span>|<span data-ttu-id="22833-776">Boolean</span><span class="sxs-lookup"><span data-stu-id="22833-776">Boolean</span></span>|<span data-ttu-id="22833-777">阻止企业站点加载非企业内容，例如第三方插件</span><span class="sxs-lookup"><span data-stu-id="22833-777">Block enterprise sites to load non-enterprise content, such as third party plug-ins</span></span>|
|<span data-ttu-id="22833-778">applicationGuardAllowPersistence</span><span class="sxs-lookup"><span data-stu-id="22833-778">applicationGuardAllowPersistence</span></span>|<span data-ttu-id="22833-779">Boolean</span><span class="sxs-lookup"><span data-stu-id="22833-779">Boolean</span></span>|<span data-ttu-id="22833-780">允许 App Guard 容器（收藏夹、Cookie、Web 密码等）内的持久用户生成数据</span><span class="sxs-lookup"><span data-stu-id="22833-780">Allow persisting user generated data inside the App Guard Containter (favorites, cookies, web passwords, etc.)</span></span>|
|<span data-ttu-id="22833-781">applicationGuardForceAuditing</span><span class="sxs-lookup"><span data-stu-id="22833-781">applicationGuardForceAuditing</span></span>|<span data-ttu-id="22833-782">Boolean</span><span class="sxs-lookup"><span data-stu-id="22833-782">Boolean</span></span>|<span data-ttu-id="22833-783">强制审核将存留 Windows 日志和事件以满足安全/符合性条件（示例事件是用户登录注销、特权使用、软件安装、系统更改等）</span><span class="sxs-lookup"><span data-stu-id="22833-783">Force auditing will persist Windows logs and events to meet security/compliance criteria (sample events are user login-logoff, use of privilege rights, software installation, system changes, etc.)</span></span>|
|<span data-ttu-id="22833-784">applicationGuardBlockClipboardSharing</span><span class="sxs-lookup"><span data-stu-id="22833-784">applicationGuardBlockClipboardSharing</span></span>|[<span data-ttu-id="22833-785">applicationGuardBlockClipboardSharingType</span><span class="sxs-lookup"><span data-stu-id="22833-785">applicationGuardBlockClipboardSharingType</span></span>](../resources/intune-deviceconfig-applicationguardblockclipboardsharingtype.md)|<span data-ttu-id="22833-786">阻止剪贴板将数据从主机共享到容器或从容器共享到主机，或阻止两种方式，或两种方式均不阻止。</span><span class="sxs-lookup"><span data-stu-id="22833-786">Block clipboard to share data from Host to Container, or from Container to Host, or both ways, or neither ways.</span></span> <span data-ttu-id="22833-787">可取值为：`notConfigured`、`blockBoth`、`blockHostToContainer`、`blockContainerToHost`、`blockNone`。</span><span class="sxs-lookup"><span data-stu-id="22833-787">Possible values are: `notConfigured`, `blockBoth`, `blockHostToContainer`, `blockContainerToHost`, `blockNone`.</span></span>|
|<span data-ttu-id="22833-788">applicationGuardAllowPrintToPDF</span><span class="sxs-lookup"><span data-stu-id="22833-788">applicationGuardAllowPrintToPDF</span></span>|<span data-ttu-id="22833-789">Boolean</span><span class="sxs-lookup"><span data-stu-id="22833-789">Boolean</span></span>|<span data-ttu-id="22833-790">允许从容器打印为 PDF 格式</span><span class="sxs-lookup"><span data-stu-id="22833-790">Allow printing to PDF from Container</span></span>|
|<span data-ttu-id="22833-791">applicationGuardAllowPrintToXPS</span><span class="sxs-lookup"><span data-stu-id="22833-791">applicationGuardAllowPrintToXPS</span></span>|<span data-ttu-id="22833-792">Boolean</span><span class="sxs-lookup"><span data-stu-id="22833-792">Boolean</span></span>|<span data-ttu-id="22833-793">允许从容器打印为 XPS 格式</span><span class="sxs-lookup"><span data-stu-id="22833-793">Allow printing to XPS from Container</span></span>|
|<span data-ttu-id="22833-794">applicationGuardAllowPrintToLocalPrinters</span><span class="sxs-lookup"><span data-stu-id="22833-794">applicationGuardAllowPrintToLocalPrinters</span></span>|<span data-ttu-id="22833-795">Boolean</span><span class="sxs-lookup"><span data-stu-id="22833-795">Boolean</span></span>|<span data-ttu-id="22833-796">允许从容器打印到本地打印机</span><span class="sxs-lookup"><span data-stu-id="22833-796">Allow printing to Local Printers from Container</span></span>|
|<span data-ttu-id="22833-797">applicationGuardAllowPrintToNetworkPrinters</span><span class="sxs-lookup"><span data-stu-id="22833-797">applicationGuardAllowPrintToNetworkPrinters</span></span>|<span data-ttu-id="22833-798">Boolean</span><span class="sxs-lookup"><span data-stu-id="22833-798">Boolean</span></span>|<span data-ttu-id="22833-799">允许从容器打印到网络打印机</span><span class="sxs-lookup"><span data-stu-id="22833-799">Allow printing to Network Printers from Container</span></span>|
|<span data-ttu-id="22833-800">applicationGuardAllowVirtualGPU</span><span class="sxs-lookup"><span data-stu-id="22833-800">applicationGuardAllowVirtualGPU</span></span>|<span data-ttu-id="22833-801">Boolean</span><span class="sxs-lookup"><span data-stu-id="22833-801">Boolean</span></span>|<span data-ttu-id="22833-802">允许应用程序防护使用虚拟 GPU</span><span class="sxs-lookup"><span data-stu-id="22833-802">Allow application guard to use virtual GPU</span></span>|
|<span data-ttu-id="22833-803">applicationGuardAllowFileSaveOnHost</span><span class="sxs-lookup"><span data-stu-id="22833-803">applicationGuardAllowFileSaveOnHost</span></span>|<span data-ttu-id="22833-804">Boolean</span><span class="sxs-lookup"><span data-stu-id="22833-804">Boolean</span></span>|<span data-ttu-id="22833-805">允许用户从应用程序防护容器中的边缘下载文件并将其保存在主机文件系统上</span><span class="sxs-lookup"><span data-stu-id="22833-805">Allow users to download files from Edge in the application guard container and save them on the host file system</span></span>|
|<span data-ttu-id="22833-806">applicationGuardAllowCameraMicrophoneRedirection</span><span class="sxs-lookup"><span data-stu-id="22833-806">applicationGuardAllowCameraMicrophoneRedirection</span></span>|<span data-ttu-id="22833-807">Boolean</span><span class="sxs-lookup"><span data-stu-id="22833-807">Boolean</span></span>|<span data-ttu-id="22833-808">获取或设置 Microsoft Defender 应用程序防护中的应用程序是否可以访问设备的相机和麦克风。</span><span class="sxs-lookup"><span data-stu-id="22833-808">Gets or sets whether applications inside Microsoft Defender Application Guard can access the device’s camera and microphone.</span></span>|
|<span data-ttu-id="22833-809">applicationGuardCertificateThumbprints</span><span class="sxs-lookup"><span data-stu-id="22833-809">applicationGuardCertificateThumbprints</span></span>|<span data-ttu-id="22833-810">String collection</span><span class="sxs-lookup"><span data-stu-id="22833-810">String collection</span></span>|<span data-ttu-id="22833-811">允许与 Microsoft Defender 应用程序防护容器共享某些设备级别的根证书。</span><span class="sxs-lookup"><span data-stu-id="22833-811">Allows certain device level Root Certificates to be shared with the Microsoft Defender Application Guard container.</span></span>|
|<span data-ttu-id="22833-812">bitLockerAllowStandardUserEncryption</span><span class="sxs-lookup"><span data-stu-id="22833-812">bitLockerAllowStandardUserEncryption</span></span>|<span data-ttu-id="22833-813">Boolean</span><span class="sxs-lookup"><span data-stu-id="22833-813">Boolean</span></span>|<span data-ttu-id="22833-814">允许管理员允许标准用户在加入 Azure AD 期间启用订阅。</span><span class="sxs-lookup"><span data-stu-id="22833-814">Allows the admin to allow standard users to enable encrpytion during Azure AD Join.</span></span>|
|<span data-ttu-id="22833-815">bitLockerDisableWarningForOtherDiskEncryption</span><span class="sxs-lookup"><span data-stu-id="22833-815">bitLockerDisableWarningForOtherDiskEncryption</span></span>|<span data-ttu-id="22833-816">Boolean</span><span class="sxs-lookup"><span data-stu-id="22833-816">Boolean</span></span>|<span data-ttu-id="22833-817">允许管理员禁用对用户计算机上其他磁盘加密的警告提示。</span><span class="sxs-lookup"><span data-stu-id="22833-817">Allows the Admin to disable the warning prompt for other disk encryption on the user machines.</span></span>|
|<span data-ttu-id="22833-818">bitLockerEnableStorageCardEncryptionOnMobile</span><span class="sxs-lookup"><span data-stu-id="22833-818">bitLockerEnableStorageCardEncryptionOnMobile</span></span>|<span data-ttu-id="22833-819">Boolean</span><span class="sxs-lookup"><span data-stu-id="22833-819">Boolean</span></span>|<span data-ttu-id="22833-820">允许管理员要求使用 BitLocker 开启加密功能。</span><span class="sxs-lookup"><span data-stu-id="22833-820">Allows the admin to require encryption to be turned on using BitLocker.</span></span> <span data-ttu-id="22833-821">此策略仅适用于移动 SKU。</span><span class="sxs-lookup"><span data-stu-id="22833-821">This policy is valid only for a mobile SKU.</span></span>|
|<span data-ttu-id="22833-822">bitLockerEncryptDevice</span><span class="sxs-lookup"><span data-stu-id="22833-822">bitLockerEncryptDevice</span></span>|<span data-ttu-id="22833-823">Boolean</span><span class="sxs-lookup"><span data-stu-id="22833-823">Boolean</span></span>|<span data-ttu-id="22833-824">允许管理员要求使用 BitLocker 开启加密功能。</span><span class="sxs-lookup"><span data-stu-id="22833-824">Allows the admin to require encryption to be turned on using BitLocker.</span></span>|
|<span data-ttu-id="22833-825">bitLockerSystemDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="22833-825">bitLockerSystemDrivePolicy</span></span>|[<span data-ttu-id="22833-826">bitLockerSystemDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="22833-826">bitLockerSystemDrivePolicy</span></span>](../resources/intune-deviceconfig-bitlockersystemdrivepolicy.md)|<span data-ttu-id="22833-827">BitLocker 系统驱动器策略。</span><span class="sxs-lookup"><span data-stu-id="22833-827">BitLocker System Drive Policy.</span></span>|
|<span data-ttu-id="22833-828">bitLockerFixedDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="22833-828">bitLockerFixedDrivePolicy</span></span>|[<span data-ttu-id="22833-829">bitLockerFixedDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="22833-829">bitLockerFixedDrivePolicy</span></span>](../resources/intune-deviceconfig-bitlockerfixeddrivepolicy.md)|<span data-ttu-id="22833-830">BitLocker 固定驱动器策略。</span><span class="sxs-lookup"><span data-stu-id="22833-830">BitLocker Fixed Drive Policy.</span></span>|
|<span data-ttu-id="22833-831">bitLockerRemovableDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="22833-831">bitLockerRemovableDrivePolicy</span></span>|[<span data-ttu-id="22833-832">bitLockerRemovableDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="22833-832">bitLockerRemovableDrivePolicy</span></span>](../resources/intune-deviceconfig-bitlockerremovabledrivepolicy.md)|<span data-ttu-id="22833-833">BitLocker 可移动驱动器策略。</span><span class="sxs-lookup"><span data-stu-id="22833-833">BitLocker Removable Drive Policy.</span></span>|
|<span data-ttu-id="22833-834">bitLockerRecoveryPasswordRotation</span><span class="sxs-lookup"><span data-stu-id="22833-834">bitLockerRecoveryPasswordRotation</span></span>|[<span data-ttu-id="22833-835">bitLockerRecoveryPasswordRotationType</span><span class="sxs-lookup"><span data-stu-id="22833-835">bitLockerRecoveryPasswordRotationType</span></span>](../resources/intune-deviceconfig-bitlockerrecoverypasswordrotationtype.md)|<span data-ttu-id="22833-836">此设置通过使用 bootmgr 或 WinRE (操作系统驱动器恢复后启动客户端驱动的恢复密码) 。</span><span class="sxs-lookup"><span data-stu-id="22833-836">This setting initiates a client-driven recovery password rotation after an OS drive recovery (either by using bootmgr or WinRE).</span></span> <span data-ttu-id="22833-837">可取值为：`notConfigured`、`disabled`、`enabledForAzureAd`、`enabledForAzureAdAndHybrid`。</span><span class="sxs-lookup"><span data-stu-id="22833-837">Possible values are: `notConfigured`, `disabled`, `enabledForAzureAd`, `enabledForAzureAdAndHybrid`.</span></span>|
|<span data-ttu-id="22833-838">defenderDisableScanArchiveFiles</span><span class="sxs-lookup"><span data-stu-id="22833-838">defenderDisableScanArchiveFiles</span></span>|<span data-ttu-id="22833-839">Boolean</span><span class="sxs-lookup"><span data-stu-id="22833-839">Boolean</span></span>|<span data-ttu-id="22833-840">允许或禁止扫描存档。</span><span class="sxs-lookup"><span data-stu-id="22833-840">Allows or disallows scanning of archives.</span></span>|
|<span data-ttu-id="22833-841">defenderAllowScanArchiveFiles</span><span class="sxs-lookup"><span data-stu-id="22833-841">defenderAllowScanArchiveFiles</span></span>|<span data-ttu-id="22833-842">Boolean</span><span class="sxs-lookup"><span data-stu-id="22833-842">Boolean</span></span>|<span data-ttu-id="22833-843">允许或禁止扫描存档。</span><span class="sxs-lookup"><span data-stu-id="22833-843">Allows or disallows scanning of archives.</span></span>|
|<span data-ttu-id="22833-844">defenderDisableBehaviorMonitoring</span><span class="sxs-lookup"><span data-stu-id="22833-844">defenderDisableBehaviorMonitoring</span></span>|<span data-ttu-id="22833-845">Boolean</span><span class="sxs-lookup"><span data-stu-id="22833-845">Boolean</span></span>|<span data-ttu-id="22833-846">允许或禁止Windows Defender监视功能。</span><span class="sxs-lookup"><span data-stu-id="22833-846">Allows or disallows Windows Defender Behavior Monitoring functionality.</span></span>|
|<span data-ttu-id="22833-847">defenderAllowBehaviorMonitoring</span><span class="sxs-lookup"><span data-stu-id="22833-847">defenderAllowBehaviorMonitoring</span></span>|<span data-ttu-id="22833-848">Boolean</span><span class="sxs-lookup"><span data-stu-id="22833-848">Boolean</span></span>|<span data-ttu-id="22833-849">允许或禁止Windows Defender监视功能。</span><span class="sxs-lookup"><span data-stu-id="22833-849">Allows or disallows Windows Defender Behavior Monitoring functionality.</span></span>|
|<span data-ttu-id="22833-850">defenderDisableCloudProtection</span><span class="sxs-lookup"><span data-stu-id="22833-850">defenderDisableCloudProtection</span></span>|<span data-ttu-id="22833-851">Boolean</span><span class="sxs-lookup"><span data-stu-id="22833-851">Boolean</span></span>|<span data-ttu-id="22833-852">为了最好地保护你的电脑，Windows Defender向 Microsoft 发送有关它所发现任何问题的信息。</span><span class="sxs-lookup"><span data-stu-id="22833-852">To best protect your PC, Windows Defender will send information to Microsoft about any problems it finds.</span></span> <span data-ttu-id="22833-853">Microsoft 将分析该信息，了解有关影响您和其他客户的问题的更多信息，并提供改进的解决方案。</span><span class="sxs-lookup"><span data-stu-id="22833-853">Microsoft will analyze that information, learn more about problems affecting you and other customers, and offer improved solutions.</span></span>|
|<span data-ttu-id="22833-854">defenderAllowCloudProtection</span><span class="sxs-lookup"><span data-stu-id="22833-854">defenderAllowCloudProtection</span></span>|<span data-ttu-id="22833-855">Boolean</span><span class="sxs-lookup"><span data-stu-id="22833-855">Boolean</span></span>|<span data-ttu-id="22833-856">为了最好地保护你的电脑，Windows Defender向 Microsoft 发送有关它所发现任何问题的信息。</span><span class="sxs-lookup"><span data-stu-id="22833-856">To best protect your PC, Windows Defender will send information to Microsoft about any problems it finds.</span></span> <span data-ttu-id="22833-857">Microsoft 将分析该信息，了解有关影响您和其他客户的问题的更多信息，并提供改进的解决方案。</span><span class="sxs-lookup"><span data-stu-id="22833-857">Microsoft will analyze that information, learn more about problems affecting you and other customers, and offer improved solutions.</span></span>|
|<span data-ttu-id="22833-858">defenderEnableScanIncomingMail</span><span class="sxs-lookup"><span data-stu-id="22833-858">defenderEnableScanIncomingMail</span></span>|<span data-ttu-id="22833-859">Boolean</span><span class="sxs-lookup"><span data-stu-id="22833-859">Boolean</span></span>|<span data-ttu-id="22833-860">允许或禁止扫描电子邮件。</span><span class="sxs-lookup"><span data-stu-id="22833-860">Allows or disallows scanning of email.</span></span>|
|<span data-ttu-id="22833-861">defenderEnableScanMappedNetworkDrivesDuringFullScan</span><span class="sxs-lookup"><span data-stu-id="22833-861">defenderEnableScanMappedNetworkDrivesDuringFullScan</span></span>|<span data-ttu-id="22833-862">Boolean</span><span class="sxs-lookup"><span data-stu-id="22833-862">Boolean</span></span>|<span data-ttu-id="22833-863">允许或禁止对映射的网络驱动器进行完全扫描。</span><span class="sxs-lookup"><span data-stu-id="22833-863">Allows or disallows a full scan of mapped network drives.</span></span>|
|<span data-ttu-id="22833-864">defenderDisableScanRemovableDrivesDuringFullScan</span><span class="sxs-lookup"><span data-stu-id="22833-864">defenderDisableScanRemovableDrivesDuringFullScan</span></span>|<span data-ttu-id="22833-865">Boolean</span><span class="sxs-lookup"><span data-stu-id="22833-865">Boolean</span></span>|<span data-ttu-id="22833-866">允许或禁止对可移动驱动器进行完全扫描。</span><span class="sxs-lookup"><span data-stu-id="22833-866">Allows or disallows a full scan of removable drives.</span></span> <span data-ttu-id="22833-867">在快速扫描期间，仍可扫描可移动驱动器。</span><span class="sxs-lookup"><span data-stu-id="22833-867">During a quick scan, removable drives may still be scanned.</span></span>|
|<span data-ttu-id="22833-868">defenderAllowScanRemovableDrivesDuringFullScan</span><span class="sxs-lookup"><span data-stu-id="22833-868">defenderAllowScanRemovableDrivesDuringFullScan</span></span>|<span data-ttu-id="22833-869">Boolean</span><span class="sxs-lookup"><span data-stu-id="22833-869">Boolean</span></span>|<span data-ttu-id="22833-870">允许或禁止对可移动驱动器进行完全扫描。</span><span class="sxs-lookup"><span data-stu-id="22833-870">Allows or disallows a full scan of removable drives.</span></span> <span data-ttu-id="22833-871">在快速扫描期间，仍可扫描可移动驱动器。</span><span class="sxs-lookup"><span data-stu-id="22833-871">During a quick scan, removable drives may still be scanned.</span></span>|
|<span data-ttu-id="22833-872">defenderDisableScanDownloads</span><span class="sxs-lookup"><span data-stu-id="22833-872">defenderDisableScanDownloads</span></span>|<span data-ttu-id="22833-873">Boolean</span><span class="sxs-lookup"><span data-stu-id="22833-873">Boolean</span></span>|<span data-ttu-id="22833-874">允许或禁止Windows Defender IOAVP 保护功能。</span><span class="sxs-lookup"><span data-stu-id="22833-874">Allows or disallows Windows Defender IOAVP Protection functionality.</span></span>|
|<span data-ttu-id="22833-875">defenderAllowScanDownloads</span><span class="sxs-lookup"><span data-stu-id="22833-875">defenderAllowScanDownloads</span></span>|<span data-ttu-id="22833-876">Boolean</span><span class="sxs-lookup"><span data-stu-id="22833-876">Boolean</span></span>|<span data-ttu-id="22833-877">允许或禁止Windows Defender IOAVP 保护功能。</span><span class="sxs-lookup"><span data-stu-id="22833-877">Allows or disallows Windows Defender IOAVP Protection functionality.</span></span>|
|<span data-ttu-id="22833-878">defenderDisableIntrusionPreventionSystem</span><span class="sxs-lookup"><span data-stu-id="22833-878">defenderDisableIntrusionPreventionSystem</span></span>|<span data-ttu-id="22833-879">Boolean</span><span class="sxs-lookup"><span data-stu-id="22833-879">Boolean</span></span>|<span data-ttu-id="22833-880">允许或禁止Windows Defender入侵防护功能。</span><span class="sxs-lookup"><span data-stu-id="22833-880">Allows or disallows Windows Defender Intrusion Prevention functionality.</span></span>|
|<span data-ttu-id="22833-881">defenderAllowIntrusionPreventionSystem</span><span class="sxs-lookup"><span data-stu-id="22833-881">defenderAllowIntrusionPreventionSystem</span></span>|<span data-ttu-id="22833-882">Boolean</span><span class="sxs-lookup"><span data-stu-id="22833-882">Boolean</span></span>|<span data-ttu-id="22833-883">允许或禁止Windows Defender入侵防护功能。</span><span class="sxs-lookup"><span data-stu-id="22833-883">Allows or disallows Windows Defender Intrusion Prevention functionality.</span></span>|
|<span data-ttu-id="22833-884">defenderDisableOnAccessProtection</span><span class="sxs-lookup"><span data-stu-id="22833-884">defenderDisableOnAccessProtection</span></span>|<span data-ttu-id="22833-885">Boolean</span><span class="sxs-lookup"><span data-stu-id="22833-885">Boolean</span></span>|<span data-ttu-id="22833-886">允许或禁止Windows Defender访问保护功能。</span><span class="sxs-lookup"><span data-stu-id="22833-886">Allows or disallows Windows Defender On Access Protection functionality.</span></span>|
|<span data-ttu-id="22833-887">defenderAllowOnAccessProtection</span><span class="sxs-lookup"><span data-stu-id="22833-887">defenderAllowOnAccessProtection</span></span>|<span data-ttu-id="22833-888">Boolean</span><span class="sxs-lookup"><span data-stu-id="22833-888">Boolean</span></span>|<span data-ttu-id="22833-889">允许或禁止Windows Defender访问保护功能。</span><span class="sxs-lookup"><span data-stu-id="22833-889">Allows or disallows Windows Defender On Access Protection functionality.</span></span>|
|<span data-ttu-id="22833-890">defenderDisableRealTimeMonitoring</span><span class="sxs-lookup"><span data-stu-id="22833-890">defenderDisableRealTimeMonitoring</span></span>|<span data-ttu-id="22833-891">Boolean</span><span class="sxs-lookup"><span data-stu-id="22833-891">Boolean</span></span>|<span data-ttu-id="22833-892">允许或禁止Windows Defender实时监视功能。</span><span class="sxs-lookup"><span data-stu-id="22833-892">Allows or disallows Windows Defender Realtime Monitoring functionality.</span></span>|
|<span data-ttu-id="22833-893">defenderAllowRealTimeMonitoring</span><span class="sxs-lookup"><span data-stu-id="22833-893">defenderAllowRealTimeMonitoring</span></span>|<span data-ttu-id="22833-894">Boolean</span><span class="sxs-lookup"><span data-stu-id="22833-894">Boolean</span></span>|<span data-ttu-id="22833-895">允许或禁止Windows Defender实时监视功能。</span><span class="sxs-lookup"><span data-stu-id="22833-895">Allows or disallows Windows Defender Realtime Monitoring functionality.</span></span>|
|<span data-ttu-id="22833-896">defenderDisableScanNetworkFiles</span><span class="sxs-lookup"><span data-stu-id="22833-896">defenderDisableScanNetworkFiles</span></span>|<span data-ttu-id="22833-897">Boolean</span><span class="sxs-lookup"><span data-stu-id="22833-897">Boolean</span></span>|<span data-ttu-id="22833-898">允许或禁止扫描网络文件。</span><span class="sxs-lookup"><span data-stu-id="22833-898">Allows or disallows a scanning of network files.</span></span>|
|<span data-ttu-id="22833-899">defenderAllowScanNetworkFiles</span><span class="sxs-lookup"><span data-stu-id="22833-899">defenderAllowScanNetworkFiles</span></span>|<span data-ttu-id="22833-900">Boolean</span><span class="sxs-lookup"><span data-stu-id="22833-900">Boolean</span></span>|<span data-ttu-id="22833-901">允许或禁止扫描网络文件。</span><span class="sxs-lookup"><span data-stu-id="22833-901">Allows or disallows a scanning of network files.</span></span>|
|<span data-ttu-id="22833-902">defenderDisableScanScriptsLoadedInInternetExplorer</span><span class="sxs-lookup"><span data-stu-id="22833-902">defenderDisableScanScriptsLoadedInInternetExplorer</span></span>|<span data-ttu-id="22833-903">Boolean</span><span class="sxs-lookup"><span data-stu-id="22833-903">Boolean</span></span>|<span data-ttu-id="22833-904">允许或禁止Windows Defender脚本扫描功能。</span><span class="sxs-lookup"><span data-stu-id="22833-904">Allows or disallows Windows Defender Script Scanning functionality.</span></span>|
|<span data-ttu-id="22833-905">defenderAllowScanScriptsLoadedInInternetExplorer</span><span class="sxs-lookup"><span data-stu-id="22833-905">defenderAllowScanScriptsLoadedInInternetExplorer</span></span>|<span data-ttu-id="22833-906">Boolean</span><span class="sxs-lookup"><span data-stu-id="22833-906">Boolean</span></span>|<span data-ttu-id="22833-907">允许或禁止Windows Defender脚本扫描功能。</span><span class="sxs-lookup"><span data-stu-id="22833-907">Allows or disallows Windows Defender Script Scanning functionality.</span></span>|
|<span data-ttu-id="22833-908">defenderBlockEndUserAccess</span><span class="sxs-lookup"><span data-stu-id="22833-908">defenderBlockEndUserAccess</span></span>|<span data-ttu-id="22833-909">Boolean</span><span class="sxs-lookup"><span data-stu-id="22833-909">Boolean</span></span>|<span data-ttu-id="22833-910">允许或禁止用户访问 Windows Defender UI。</span><span class="sxs-lookup"><span data-stu-id="22833-910">Allows or disallows user access to the Windows Defender UI.</span></span> <span data-ttu-id="22833-911">如果不允许，还将Windows Defender所有通知。</span><span class="sxs-lookup"><span data-stu-id="22833-911">If disallowed, all Windows Defender notifications will also be suppressed.</span></span>|
|<span data-ttu-id="22833-912">defenderAllowEndUserAccess</span><span class="sxs-lookup"><span data-stu-id="22833-912">defenderAllowEndUserAccess</span></span>|<span data-ttu-id="22833-913">Boolean</span><span class="sxs-lookup"><span data-stu-id="22833-913">Boolean</span></span>|<span data-ttu-id="22833-914">允许或禁止用户访问 Windows Defender UI。</span><span class="sxs-lookup"><span data-stu-id="22833-914">Allows or disallows user access to the Windows Defender UI.</span></span> <span data-ttu-id="22833-915">如果不允许，还将Windows Defender所有通知。</span><span class="sxs-lookup"><span data-stu-id="22833-915">If disallowed, all Windows Defender notifications will also be suppressed.</span></span>|
|<span data-ttu-id="22833-916">defenderScanMaxCpuPercentage</span><span class="sxs-lookup"><span data-stu-id="22833-916">defenderScanMaxCpuPercentage</span></span>|<span data-ttu-id="22833-917">Int32</span><span class="sxs-lookup"><span data-stu-id="22833-917">Int32</span></span>|<span data-ttu-id="22833-918">表示服务器扫描的平均 CPU 负载Windows Defender， (百分比) 。</span><span class="sxs-lookup"><span data-stu-id="22833-918">Represents the average CPU load factor for the Windows Defender scan (in percent).</span></span> <span data-ttu-id="22833-919">默认值为 50。</span><span class="sxs-lookup"><span data-stu-id="22833-919">The default value is 50.</span></span> <span data-ttu-id="22833-920">有效值为 0 至 100</span><span class="sxs-lookup"><span data-stu-id="22833-920">Valid values 0 to 100</span></span>|
|<span data-ttu-id="22833-921">defenderCheckForSignaturesBeforeRunningScan</span><span class="sxs-lookup"><span data-stu-id="22833-921">defenderCheckForSignaturesBeforeRunningScan</span></span>|<span data-ttu-id="22833-922">Boolean</span><span class="sxs-lookup"><span data-stu-id="22833-922">Boolean</span></span>|<span data-ttu-id="22833-923">此策略设置允许你在运行扫描之前管理是否检查新的病毒定义和间谍软件定义。</span><span class="sxs-lookup"><span data-stu-id="22833-923">This policy setting allows you to manage whether a check for new virus and spyware definitions will occur before running a scan.</span></span>|
|<span data-ttu-id="22833-924">defenderCloudBlockLevel</span><span class="sxs-lookup"><span data-stu-id="22833-924">defenderCloudBlockLevel</span></span>|[<span data-ttu-id="22833-925">defenderCloudBlockLevelType</span><span class="sxs-lookup"><span data-stu-id="22833-925">defenderCloudBlockLevelType</span></span>](../resources/intune-deviceconfig-defendercloudblockleveltype.md)|<span data-ttu-id="22833-926">在 Windows 10 版本 1709 中添加。</span><span class="sxs-lookup"><span data-stu-id="22833-926">Added in Windows 10, version 1709.</span></span> <span data-ttu-id="22833-927">此策略设置确定Windows Defender阻止和扫描可疑文件时，防病毒将具有怎样的主动性。</span><span class="sxs-lookup"><span data-stu-id="22833-927">This policy setting determines how aggressive Windows Defender Antivirus will be in blocking and scanning suspicious files.</span></span> <span data-ttu-id="22833-928">值类型为整数。</span><span class="sxs-lookup"><span data-stu-id="22833-928">Value type is integer.</span></span> <span data-ttu-id="22833-929">此功能需要启用"加入 Microsoft MAPS"设置才能运行。</span><span class="sxs-lookup"><span data-stu-id="22833-929">This feature requires the "Join Microsoft MAPS" setting enabled in order to function.</span></span> <span data-ttu-id="22833-930">可取值为：`notConfigured`、`high`、`highPlus`、`zeroTolerance`。</span><span class="sxs-lookup"><span data-stu-id="22833-930">Possible values are: `notConfigured`, `high`, `highPlus`, `zeroTolerance`.</span></span>|
|<span data-ttu-id="22833-931">defenderCloudExtendedTimeoutInSeconds</span><span class="sxs-lookup"><span data-stu-id="22833-931">defenderCloudExtendedTimeoutInSeconds</span></span>|<span data-ttu-id="22833-932">Int32</span><span class="sxs-lookup"><span data-stu-id="22833-932">Int32</span></span>|<span data-ttu-id="22833-933">在 Windows 10 版本 1709 中添加。</span><span class="sxs-lookup"><span data-stu-id="22833-933">Added in Windows 10, version 1709.</span></span> <span data-ttu-id="22833-934">此功能允许Windows Defender防病毒阻止可疑文件最多 60 秒，并扫描它在云中以确保其安全。</span><span class="sxs-lookup"><span data-stu-id="22833-934">This feature allows Windows Defender Antivirus to block a suspicious file for up to 60 seconds, and scan it in the cloud to make sure it's safe.</span></span> <span data-ttu-id="22833-935">值类型为整数，范围为 0 - 50。</span><span class="sxs-lookup"><span data-stu-id="22833-935">Value type is integer, range is 0 - 50.</span></span> <span data-ttu-id="22833-936">此功能依赖于必须全部启用的其他三个 MAPS 设置："配置'首次看到时阻止'功能;"加入 Microsoft MAPS";"需要进一步分析时发送文件示例"。</span><span class="sxs-lookup"><span data-stu-id="22833-936">This feature depends on three other MAPS settings the must all be enabled- "Configure the 'Block at First Sight' feature; "Join Microsoft MAPS"; "Send file samples when further analysis is required".</span></span> <span data-ttu-id="22833-937">有效值为 0 至 50</span><span class="sxs-lookup"><span data-stu-id="22833-937">Valid values 0 to 50</span></span>|
|<span data-ttu-id="22833-938">defenderDaysBeforeDeletingQuarantinedMalware</span><span class="sxs-lookup"><span data-stu-id="22833-938">defenderDaysBeforeDeletingQuarantinedMalware</span></span>|<span data-ttu-id="22833-939">Int32</span><span class="sxs-lookup"><span data-stu-id="22833-939">Int32</span></span>|<span data-ttu-id="22833-940">时间段 (以) 隔离项目将存储在系统上的天数。</span><span class="sxs-lookup"><span data-stu-id="22833-940">Time period (in days) that quarantine items will be stored on the system.</span></span> <span data-ttu-id="22833-941">有效值为 0 至 90</span><span class="sxs-lookup"><span data-stu-id="22833-941">Valid values 0 to 90</span></span>|
|<span data-ttu-id="22833-942">defenderDisableCatchupFullScan</span><span class="sxs-lookup"><span data-stu-id="22833-942">defenderDisableCatchupFullScan</span></span>|<span data-ttu-id="22833-943">Boolean</span><span class="sxs-lookup"><span data-stu-id="22833-943">Boolean</span></span>|<span data-ttu-id="22833-944">此策略设置允许你为计划的完整扫描配置跟进扫描。</span><span class="sxs-lookup"><span data-stu-id="22833-944">This policy setting allows you to configure catch-up scans for scheduled full scans.</span></span> <span data-ttu-id="22833-945">跟进扫描是因错过定期计划扫描而启动的扫描。</span><span class="sxs-lookup"><span data-stu-id="22833-945">A catch-up scan is a scan that is initiated because a regularly scheduled scan was missed.</span></span> <span data-ttu-id="22833-946">通常，这些计划扫描会丢失，因为计算机在计划时间已关闭。</span><span class="sxs-lookup"><span data-stu-id="22833-946">Usually these scheduled scans are missed because the computer was turned off at the scheduled time.</span></span>|
|<span data-ttu-id="22833-947">defenderDisableCatchupQuickScan</span><span class="sxs-lookup"><span data-stu-id="22833-947">defenderDisableCatchupQuickScan</span></span>|<span data-ttu-id="22833-948">Boolean</span><span class="sxs-lookup"><span data-stu-id="22833-948">Boolean</span></span>|<span data-ttu-id="22833-949">此策略设置允许你配置计划快速扫描的捕获扫描。</span><span class="sxs-lookup"><span data-stu-id="22833-949">This policy setting allows you to configure catch-up scans for scheduled quick scans.</span></span> <span data-ttu-id="22833-950">跟进扫描是因错过定期计划扫描而启动的扫描。</span><span class="sxs-lookup"><span data-stu-id="22833-950">A catch-up scan is a scan that is initiated because a regularly scheduled scan was missed.</span></span> <span data-ttu-id="22833-951">通常，这些计划扫描会丢失，因为计算机在计划时间已关闭。</span><span class="sxs-lookup"><span data-stu-id="22833-951">Usually these scheduled scans are missed because the computer was turned off at the scheduled time.</span></span>|
|<span data-ttu-id="22833-952">defenderEnableLowCpuPriority</span><span class="sxs-lookup"><span data-stu-id="22833-952">defenderEnableLowCpuPriority</span></span>|<span data-ttu-id="22833-953">Boolean</span><span class="sxs-lookup"><span data-stu-id="22833-953">Boolean</span></span>|<span data-ttu-id="22833-954">此策略设置允许你为计划扫描启用或禁用低 CPU 优先级。</span><span class="sxs-lookup"><span data-stu-id="22833-954">This policy setting allows you to enable or disable low CPU priority for scheduled scans.</span></span>|
|<span data-ttu-id="22833-955">defenderFileExtensionsToExclude</span><span class="sxs-lookup"><span data-stu-id="22833-955">defenderFileExtensionsToExclude</span></span>|<span data-ttu-id="22833-956">String 集合</span><span class="sxs-lookup"><span data-stu-id="22833-956">String collection</span></span>|<span data-ttu-id="22833-957">要从扫描和实时保护中排除的文件扩展名。</span><span class="sxs-lookup"><span data-stu-id="22833-957">File extensions to exclude from scans and real time protection.</span></span>|
|<span data-ttu-id="22833-958">defenderFilesAndFoldersToExclude</span><span class="sxs-lookup"><span data-stu-id="22833-958">defenderFilesAndFoldersToExclude</span></span>|<span data-ttu-id="22833-959">String 集合</span><span class="sxs-lookup"><span data-stu-id="22833-959">String collection</span></span>|<span data-ttu-id="22833-960">要从扫描和实时保护中排除的文件和文件夹。</span><span class="sxs-lookup"><span data-stu-id="22833-960">Files and folder to exclude from scans and real time protection.</span></span>|
|<span data-ttu-id="22833-961">defenderProcessesToExclude</span><span class="sxs-lookup"><span data-stu-id="22833-961">defenderProcessesToExclude</span></span>|<span data-ttu-id="22833-962">String 集合</span><span class="sxs-lookup"><span data-stu-id="22833-962">String collection</span></span>|<span data-ttu-id="22833-963">要从扫描和实时保护中排除的进程。</span><span class="sxs-lookup"><span data-stu-id="22833-963">Processes to exclude from scans and real time protection.</span></span>|
|<span data-ttu-id="22833-964">defenderPotentiallyUnwantedAppAction</span><span class="sxs-lookup"><span data-stu-id="22833-964">defenderPotentiallyUnwantedAppAction</span></span>|[<span data-ttu-id="22833-965">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="22833-965">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="22833-966">已添加到 Windows 10 版本 1607 中。</span><span class="sxs-lookup"><span data-stu-id="22833-966">Added in Windows 10, version 1607.</span></span> <span data-ttu-id="22833-967">指定在 PUA 中检测可能不需要的应用程序 (级别) 。</span><span class="sxs-lookup"><span data-stu-id="22833-967">Specifies the level of detection for potentially unwanted applications (PUAs).</span></span> <span data-ttu-id="22833-968">Windows Defender下载可能不需要的软件或尝试在计算机上安装自身时发出警报。</span><span class="sxs-lookup"><span data-stu-id="22833-968">Windows Defender alerts you when potentially unwanted software is being downloaded or attempts to install itself on your computer.</span></span> <span data-ttu-id="22833-969">可取值为：`userDefined`、`enable`、`auditMode`、`warn`、`notConfigured`。</span><span class="sxs-lookup"><span data-stu-id="22833-969">Possible values are: `userDefined`, `enable`, `auditMode`, `warn`, `notConfigured`.</span></span>|
|<span data-ttu-id="22833-970">defenderScanDirection</span><span class="sxs-lookup"><span data-stu-id="22833-970">defenderScanDirection</span></span>|[<span data-ttu-id="22833-971">defenderRealtimeScanDirection</span><span class="sxs-lookup"><span data-stu-id="22833-971">defenderRealtimeScanDirection</span></span>](../resources/intune-deviceconfig-defenderrealtimescandirection.md)|<span data-ttu-id="22833-972">控制应监视哪些文件集。</span><span class="sxs-lookup"><span data-stu-id="22833-972">Controls which sets of files should be monitored.</span></span> <span data-ttu-id="22833-973">可取值为：`monitorAllFiles`、`monitorIncomingFilesOnly`、`monitorOutgoingFilesOnly`。</span><span class="sxs-lookup"><span data-stu-id="22833-973">Possible values are: `monitorAllFiles`, `monitorIncomingFilesOnly`, `monitorOutgoingFilesOnly`.</span></span>|
|<span data-ttu-id="22833-974">defenderScanType</span><span class="sxs-lookup"><span data-stu-id="22833-974">defenderScanType</span></span>|[<span data-ttu-id="22833-975">defenderScanType</span><span class="sxs-lookup"><span data-stu-id="22833-975">defenderScanType</span></span>](../resources/intune-deviceconfig-defenderscantype.md)|<span data-ttu-id="22833-976">选择是执行快速扫描还是完全扫描。</span><span class="sxs-lookup"><span data-stu-id="22833-976">Selects whether to perform a quick scan or full scan.</span></span> <span data-ttu-id="22833-977">可取值为：`userDefined`、`disabled`、`quick`、`full`。</span><span class="sxs-lookup"><span data-stu-id="22833-977">Possible values are: `userDefined`, `disabled`, `quick`, `full`.</span></span>|
|<span data-ttu-id="22833-978">defenderScheduledQuickScanTime</span><span class="sxs-lookup"><span data-stu-id="22833-978">defenderScheduledQuickScanTime</span></span>|<span data-ttu-id="22833-979">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="22833-979">TimeOfDay</span></span>|<span data-ttu-id="22833-980">选择应运行快速扫描Windows Defender的时间。</span><span class="sxs-lookup"><span data-stu-id="22833-980">Selects the time of day that the Windows Defender quick scan should run.</span></span> <span data-ttu-id="22833-981">例如，值 0=12：00AM、值 60=1：00AM、值 120=2：00 等，最多为值 1380=11：00PM。</span><span class="sxs-lookup"><span data-stu-id="22833-981">For example, a value of 0=12:00AM, a value of 60=1:00AM, a value of 120=2:00, and so on, up to a value of 1380=11:00PM.</span></span> <span data-ttu-id="22833-982">默认值为 120</span><span class="sxs-lookup"><span data-stu-id="22833-982">The default value is 120</span></span>|
|<span data-ttu-id="22833-983">defenderScheduledScanDay</span><span class="sxs-lookup"><span data-stu-id="22833-983">defenderScheduledScanDay</span></span>|[<span data-ttu-id="22833-984">weeklySchedule</span><span class="sxs-lookup"><span data-stu-id="22833-984">weeklySchedule</span></span>](../resources/intune-deviceconfig-weeklyschedule.md)|<span data-ttu-id="22833-985">选择运行扫描Windows Defender天。</span><span class="sxs-lookup"><span data-stu-id="22833-985">Selects the day that the Windows Defender scan should run.</span></span> <span data-ttu-id="22833-986">可取值为：`userDefined`、`everyday`、`sunday`、`monday`、`tuesday`、`wednesday`、`thursday`、`friday`、`saturday`、`noScheduledScan`。</span><span class="sxs-lookup"><span data-stu-id="22833-986">Possible values are: `userDefined`, `everyday`, `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`, `noScheduledScan`.</span></span>|
|<span data-ttu-id="22833-987">defenderScheduledScanTime</span><span class="sxs-lookup"><span data-stu-id="22833-987">defenderScheduledScanTime</span></span>|<span data-ttu-id="22833-988">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="22833-988">TimeOfDay</span></span>|<span data-ttu-id="22833-989">选择一天中应运行Windows Defender的时间。</span><span class="sxs-lookup"><span data-stu-id="22833-989">Selects the time of day that the Windows Defender scan should run.</span></span>|
|<span data-ttu-id="22833-990">defenderSignatureUpdateIntervalInHours</span><span class="sxs-lookup"><span data-stu-id="22833-990">defenderSignatureUpdateIntervalInHours</span></span>|<span data-ttu-id="22833-991">Int32</span><span class="sxs-lookup"><span data-stu-id="22833-991">Int32</span></span>|<span data-ttu-id="22833-992">指定 (检查签名的时间间隔) 以小时为单位，因此将按照间隔设置新签名的检查，而不是使用 ScheduleDay 和 ScheduleTime。</span><span class="sxs-lookup"><span data-stu-id="22833-992">Specifies the interval (in hours) that will be used to check for signatures, so instead of using the ScheduleDay and ScheduleTime the check for new signatures will be set according to the interval.</span></span> <span data-ttu-id="22833-993">有效值为 0 至 24</span><span class="sxs-lookup"><span data-stu-id="22833-993">Valid values 0 to 24</span></span>|
|<span data-ttu-id="22833-994">defenderSubmitSamplesConsentType</span><span class="sxs-lookup"><span data-stu-id="22833-994">defenderSubmitSamplesConsentType</span></span>|[<span data-ttu-id="22833-995">defenderSubmitSamplesConsentType</span><span class="sxs-lookup"><span data-stu-id="22833-995">defenderSubmitSamplesConsentType</span></span>](../resources/intune-deviceconfig-defendersubmitsamplesconsenttype.md)|<span data-ttu-id="22833-996">在发送数据时检查用户Windows Defender级别。</span><span class="sxs-lookup"><span data-stu-id="22833-996">Checks for the user consent level in Windows Defender to send data.</span></span> <span data-ttu-id="22833-997">可取值为：`sendSafeSamplesAutomatically`、`alwaysPrompt`、`neverSend`、`sendAllSamplesAutomatically`。</span><span class="sxs-lookup"><span data-stu-id="22833-997">Possible values are: `sendSafeSamplesAutomatically`, `alwaysPrompt`, `neverSend`, `sendAllSamplesAutomatically`.</span></span>|
|<span data-ttu-id="22833-998">defenderDetectedMalwareActions</span><span class="sxs-lookup"><span data-stu-id="22833-998">defenderDetectedMalwareActions</span></span>|[<span data-ttu-id="22833-999">defenderDetectedMalwareActions</span><span class="sxs-lookup"><span data-stu-id="22833-999">defenderDetectedMalwareActions</span></span>](../resources/intune-deviceconfig-defenderdetectedmalwareactions.md)|<span data-ttu-id="22833-1000">允许管理员指定任何有效的威胁严重性级别和要采取的相应默认操作 ID。</span><span class="sxs-lookup"><span data-stu-id="22833-1000">Allows an administrator to specify any valid threat severity levels and the corresponding default action ID to take.</span></span>|



## <a name="response"></a><span data-ttu-id="22833-1001">响应</span><span class="sxs-lookup"><span data-stu-id="22833-1001">Response</span></span>
<span data-ttu-id="22833-1002">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="22833-1002">If successful, this method returns a `200 OK` response code and an updated [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="22833-1003">示例</span><span class="sxs-lookup"><span data-stu-id="22833-1003">Example</span></span>

### <a name="request"></a><span data-ttu-id="22833-1004">请求</span><span class="sxs-lookup"><span data-stu-id="22833-1004">Request</span></span>
<span data-ttu-id="22833-1005">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="22833-1005">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 31268

{
  "@odata.type": "#microsoft.graph.windows10EndpointProtectionConfiguration",
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
  "dmaGuardDeviceEnumerationPolicy": "blockAll",
  "firewallRules": [
    {
      "@odata.type": "microsoft.graph.windowsFirewallRule",
      "displayName": "Display Name value",
      "description": "Description value",
      "packageFamilyName": "Package Family Name value",
      "filePath": "File Path value",
      "serviceName": "Service Name value",
      "protocol": 8,
      "localPortRanges": [
        "Local Port Ranges value"
      ],
      "remotePortRanges": [
        "Remote Port Ranges value"
      ],
      "localAddressRanges": [
        "Local Address Ranges value"
      ],
      "remoteAddressRanges": [
        "Remote Address Ranges value"
      ],
      "profileTypes": "domain",
      "action": "blocked",
      "trafficDirection": "out",
      "interfaceTypes": "remoteAccess",
      "edgeTraversal": "blocked",
      "localUserAuthorizations": "Local User Authorizations value"
    }
  ],
  "userRightsAccessCredentialManagerAsTrustedCaller": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsAllowAccessFromNetwork": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsBlockAccessFromNetwork": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsActAsPartOfTheOperatingSystem": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsLocalLogOn": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsDenyLocalLogOn": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsBackupData": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsChangeSystemTime": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsCreateGlobalObjects": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsCreatePageFile": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsCreatePermanentSharedObjects": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsCreateSymbolicLinks": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsCreateToken": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsDebugPrograms": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsRemoteDesktopServicesLogOn": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsDelegation": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsGenerateSecurityAudits": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsImpersonateClient": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsIncreaseSchedulingPriority": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsLoadUnloadDrivers": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsLockMemory": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsManageAuditingAndSecurityLogs": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsManageVolumes": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsModifyFirmwareEnvironment": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsModifyObjectLabels": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsProfileSingleProcess": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsRemoteShutdown": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsRestoreData": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsTakeOwnership": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "xboxServicesEnableXboxGameSaveTask": true,
  "xboxServicesAccessoryManagementServiceStartupMode": "automatic",
  "xboxServicesLiveAuthManagerServiceStartupMode": "automatic",
  "xboxServicesLiveGameSaveServiceStartupMode": "automatic",
  "xboxServicesLiveNetworkingServiceStartupMode": "automatic",
  "localSecurityOptionsBlockMicrosoftAccounts": true,
  "localSecurityOptionsBlockRemoteLogonWithBlankPassword": true,
  "localSecurityOptionsDisableAdministratorAccount": true,
  "localSecurityOptionsAdministratorAccountName": "Local Security Options Administrator Account Name value",
  "localSecurityOptionsDisableGuestAccount": true,
  "localSecurityOptionsGuestAccountName": "Local Security Options Guest Account Name value",
  "localSecurityOptionsAllowUndockWithoutHavingToLogon": true,
  "localSecurityOptionsBlockUsersInstallingPrinterDrivers": true,
  "localSecurityOptionsBlockRemoteOpticalDriveAccess": true,
  "localSecurityOptionsFormatAndEjectOfRemovableMediaAllowedUser": "administrators",
  "localSecurityOptionsMachineInactivityLimit": 10,
  "localSecurityOptionsMachineInactivityLimitInMinutes": 3,
  "localSecurityOptionsDoNotRequireCtrlAltDel": true,
  "localSecurityOptionsHideLastSignedInUser": true,
  "localSecurityOptionsHideUsernameAtSignIn": true,
  "localSecurityOptionsLogOnMessageTitle": "Local Security Options Log On Message Title value",
  "localSecurityOptionsLogOnMessageText": "Local Security Options Log On Message Text value",
  "localSecurityOptionsAllowPKU2UAuthenticationRequests": true,
  "localSecurityOptionsAllowRemoteCallsToSecurityAccountsManagerHelperBool": true,
  "localSecurityOptionsAllowRemoteCallsToSecurityAccountsManager": "Local Security Options Allow Remote Calls To Security Accounts Manager value",
  "localSecurityOptionsMinimumSessionSecurityForNtlmSspBasedClients": "requireNtmlV2SessionSecurity",
  "localSecurityOptionsMinimumSessionSecurityForNtlmSspBasedServers": "requireNtmlV2SessionSecurity",
  "lanManagerAuthenticationLevel": "lmNtlmAndNtlmV2",
  "lanManagerWorkstationDisableInsecureGuestLogons": true,
  "localSecurityOptionsClearVirtualMemoryPageFile": true,
  "localSecurityOptionsAllowSystemToBeShutDownWithoutHavingToLogOn": true,
  "localSecurityOptionsAllowUIAccessApplicationElevation": true,
  "localSecurityOptionsVirtualizeFileAndRegistryWriteFailuresToPerUserLocations": true,
  "localSecurityOptionsOnlyElevateSignedExecutables": true,
  "localSecurityOptionsAdministratorElevationPromptBehavior": "elevateWithoutPrompting",
  "localSecurityOptionsStandardUserElevationPromptBehavior": "automaticallyDenyElevationRequests",
  "localSecurityOptionsSwitchToSecureDesktopWhenPromptingForElevation": true,
  "localSecurityOptionsDetectApplicationInstallationsAndPromptForElevation": true,
  "localSecurityOptionsAllowUIAccessApplicationsForSecureLocations": true,
  "localSecurityOptionsUseAdminApprovalMode": true,
  "localSecurityOptionsUseAdminApprovalModeForAdministrators": true,
  "localSecurityOptionsInformationShownOnLockScreen": "userDisplayNameDomainUser",
  "localSecurityOptionsInformationDisplayedOnLockScreen": "administrators",
  "localSecurityOptionsDisableClientDigitallySignCommunicationsIfServerAgrees": true,
  "localSecurityOptionsClientDigitallySignCommunicationsAlways": true,
  "localSecurityOptionsClientSendUnencryptedPasswordToThirdPartySMBServers": true,
  "localSecurityOptionsDisableServerDigitallySignCommunicationsAlways": true,
  "localSecurityOptionsDisableServerDigitallySignCommunicationsIfClientAgrees": true,
  "localSecurityOptionsRestrictAnonymousAccessToNamedPipesAndShares": true,
  "localSecurityOptionsDoNotAllowAnonymousEnumerationOfSAMAccounts": true,
  "localSecurityOptionsAllowAnonymousEnumerationOfSAMAccountsAndShares": true,
  "localSecurityOptionsDoNotStoreLANManagerHashValueOnNextPasswordChange": true,
  "localSecurityOptionsSmartCardRemovalBehavior": "noAction",
  "defenderSecurityCenterDisableAppBrowserUI": true,
  "defenderSecurityCenterDisableFamilyUI": true,
  "defenderSecurityCenterDisableHealthUI": true,
  "defenderSecurityCenterDisableNetworkUI": true,
  "defenderSecurityCenterDisableVirusUI": true,
  "defenderSecurityCenterDisableAccountUI": true,
  "defenderSecurityCenterDisableClearTpmUI": true,
  "defenderSecurityCenterDisableHardwareUI": true,
  "defenderSecurityCenterDisableNotificationAreaUI": true,
  "defenderSecurityCenterDisableRansomwareUI": true,
  "defenderSecurityCenterDisableSecureBootUI": true,
  "defenderSecurityCenterDisableTroubleshootingUI": true,
  "defenderSecurityCenterDisableVulnerableTpmFirmwareUpdateUI": true,
  "defenderSecurityCenterOrganizationDisplayName": "Defender Security Center Organization Display Name value",
  "defenderSecurityCenterHelpEmail": "Defender Security Center Help Email value",
  "defenderSecurityCenterHelpPhone": "Defender Security Center Help Phone value",
  "defenderSecurityCenterHelpURL": "Defender Security Center Help URL value",
  "defenderSecurityCenterNotificationsFromApp": "blockNoncriticalNotifications",
  "defenderSecurityCenterITContactDisplay": "displayInAppAndInNotifications",
  "windowsDefenderTamperProtection": "enable",
  "firewallBlockStatefulFTP": true,
  "firewallIdleTimeoutForSecurityAssociationInSeconds": 2,
  "firewallPreSharedKeyEncodingMethod": "none",
  "firewallIPSecExemptionsNone": true,
  "firewallIPSecExemptionsAllowNeighborDiscovery": true,
  "firewallIPSecExemptionsAllowICMP": true,
  "firewallIPSecExemptionsAllowRouterDiscovery": true,
  "firewallIPSecExemptionsAllowDHCP": true,
  "firewallCertificateRevocationListCheckMethod": "none",
  "firewallMergeKeyingModuleSettings": true,
  "firewallPacketQueueingMethod": "disabled",
  "firewallProfileDomain": {
    "@odata.type": "microsoft.graph.windowsFirewallNetworkProfile",
    "firewallEnabled": "blocked",
    "stealthModeRequired": true,
    "stealthModeBlocked": true,
    "incomingTrafficRequired": true,
    "incomingTrafficBlocked": true,
    "unicastResponsesToMulticastBroadcastsRequired": true,
    "unicastResponsesToMulticastBroadcastsBlocked": true,
    "inboundNotificationsRequired": true,
    "inboundNotificationsBlocked": true,
    "authorizedApplicationRulesFromGroupPolicyMerged": true,
    "authorizedApplicationRulesFromGroupPolicyNotMerged": true,
    "globalPortRulesFromGroupPolicyMerged": true,
    "globalPortRulesFromGroupPolicyNotMerged": true,
    "connectionSecurityRulesFromGroupPolicyMerged": true,
    "connectionSecurityRulesFromGroupPolicyNotMerged": true,
    "outboundConnectionsRequired": true,
    "outboundConnectionsBlocked": true,
    "inboundConnectionsRequired": true,
    "inboundConnectionsBlocked": true,
    "securedPacketExemptionAllowed": true,
    "securedPacketExemptionBlocked": true,
    "policyRulesFromGroupPolicyMerged": true,
    "policyRulesFromGroupPolicyNotMerged": true
  },
  "firewallProfilePublic": {
    "@odata.type": "microsoft.graph.windowsFirewallNetworkProfile",
    "firewallEnabled": "blocked",
    "stealthModeRequired": true,
    "stealthModeBlocked": true,
    "incomingTrafficRequired": true,
    "incomingTrafficBlocked": true,
    "unicastResponsesToMulticastBroadcastsRequired": true,
    "unicastResponsesToMulticastBroadcastsBlocked": true,
    "inboundNotificationsRequired": true,
    "inboundNotificationsBlocked": true,
    "authorizedApplicationRulesFromGroupPolicyMerged": true,
    "authorizedApplicationRulesFromGroupPolicyNotMerged": true,
    "globalPortRulesFromGroupPolicyMerged": true,
    "globalPortRulesFromGroupPolicyNotMerged": true,
    "connectionSecurityRulesFromGroupPolicyMerged": true,
    "connectionSecurityRulesFromGroupPolicyNotMerged": true,
    "outboundConnectionsRequired": true,
    "outboundConnectionsBlocked": true,
    "inboundConnectionsRequired": true,
    "inboundConnectionsBlocked": true,
    "securedPacketExemptionAllowed": true,
    "securedPacketExemptionBlocked": true,
    "policyRulesFromGroupPolicyMerged": true,
    "policyRulesFromGroupPolicyNotMerged": true
  },
  "firewallProfilePrivate": {
    "@odata.type": "microsoft.graph.windowsFirewallNetworkProfile",
    "firewallEnabled": "blocked",
    "stealthModeRequired": true,
    "stealthModeBlocked": true,
    "incomingTrafficRequired": true,
    "incomingTrafficBlocked": true,
    "unicastResponsesToMulticastBroadcastsRequired": true,
    "unicastResponsesToMulticastBroadcastsBlocked": true,
    "inboundNotificationsRequired": true,
    "inboundNotificationsBlocked": true,
    "authorizedApplicationRulesFromGroupPolicyMerged": true,
    "authorizedApplicationRulesFromGroupPolicyNotMerged": true,
    "globalPortRulesFromGroupPolicyMerged": true,
    "globalPortRulesFromGroupPolicyNotMerged": true,
    "connectionSecurityRulesFromGroupPolicyMerged": true,
    "connectionSecurityRulesFromGroupPolicyNotMerged": true,
    "outboundConnectionsRequired": true,
    "outboundConnectionsBlocked": true,
    "inboundConnectionsRequired": true,
    "inboundConnectionsBlocked": true,
    "securedPacketExemptionAllowed": true,
    "securedPacketExemptionBlocked": true,
    "policyRulesFromGroupPolicyMerged": true,
    "policyRulesFromGroupPolicyNotMerged": true
  },
  "defenderAdobeReaderLaunchChildProcess": "enable",
  "defenderAttackSurfaceReductionExcludedPaths": [
    "Defender Attack Surface Reduction Excluded Paths value"
  ],
  "defenderOfficeAppsOtherProcessInjectionType": "block",
  "defenderOfficeAppsOtherProcessInjection": "enable",
  "defenderOfficeCommunicationAppsLaunchChildProcess": "enable",
  "defenderOfficeAppsExecutableContentCreationOrLaunchType": "block",
  "defenderOfficeAppsExecutableContentCreationOrLaunch": "enable",
  "defenderOfficeAppsLaunchChildProcessType": "block",
  "defenderOfficeAppsLaunchChildProcess": "enable",
  "defenderOfficeMacroCodeAllowWin32ImportsType": "block",
  "defenderOfficeMacroCodeAllowWin32Imports": "enable",
  "defenderScriptObfuscatedMacroCodeType": "block",
  "defenderScriptObfuscatedMacroCode": "enable",
  "defenderScriptDownloadedPayloadExecutionType": "block",
  "defenderScriptDownloadedPayloadExecution": "enable",
  "defenderPreventCredentialStealingType": "enable",
  "defenderProcessCreationType": "block",
  "defenderProcessCreation": "enable",
  "defenderUntrustedUSBProcessType": "block",
  "defenderUntrustedUSBProcess": "enable",
  "defenderUntrustedExecutableType": "block",
  "defenderUntrustedExecutable": "enable",
  "defenderEmailContentExecutionType": "block",
  "defenderEmailContentExecution": "enable",
  "defenderAdvancedRansomewareProtectionType": "enable",
  "defenderGuardMyFoldersType": "enable",
  "defenderGuardedFoldersAllowedAppPaths": [
    "Defender Guarded Folders Allowed App Paths value"
  ],
  "defenderAdditionalGuardedFolders": [
    "Defender Additional Guarded Folders value"
  ],
  "defenderNetworkProtectionType": "enable",
  "defenderExploitProtectionXml": "ZGVmZW5kZXJFeHBsb2l0UHJvdGVjdGlvblhtbA==",
  "defenderExploitProtectionXmlFileName": "Defender Exploit Protection Xml File Name value",
  "defenderSecurityCenterBlockExploitProtectionOverride": true,
  "defenderBlockPersistenceThroughWmiType": "block",
  "appLockerApplicationControl": "enforceComponentsAndStoreApps",
  "deviceGuardLocalSystemAuthorityCredentialGuardSettings": "enableWithUEFILock",
  "deviceGuardEnableVirtualizationBasedSecurity": true,
  "deviceGuardEnableSecureBootWithDMA": true,
  "deviceGuardSecureBootWithDMA": "withoutDMA",
  "deviceGuardLaunchSystemGuard": "enabled",
  "smartScreenEnableInShell": true,
  "smartScreenBlockOverrideForFiles": true,
  "applicationGuardEnabled": true,
  "applicationGuardEnabledOptions": "enabledForEdge",
  "applicationGuardBlockFileTransfer": "blockImageAndTextFile",
  "applicationGuardBlockNonEnterpriseContent": true,
  "applicationGuardAllowPersistence": true,
  "applicationGuardForceAuditing": true,
  "applicationGuardBlockClipboardSharing": "blockBoth",
  "applicationGuardAllowPrintToPDF": true,
  "applicationGuardAllowPrintToXPS": true,
  "applicationGuardAllowPrintToLocalPrinters": true,
  "applicationGuardAllowPrintToNetworkPrinters": true,
  "applicationGuardAllowVirtualGPU": true,
  "applicationGuardAllowFileSaveOnHost": true,
  "applicationGuardAllowCameraMicrophoneRedirection": true,
  "applicationGuardCertificateThumbprints": [
    "Application Guard Certificate Thumbprints value"
  ],
  "bitLockerAllowStandardUserEncryption": true,
  "bitLockerDisableWarningForOtherDiskEncryption": true,
  "bitLockerEnableStorageCardEncryptionOnMobile": true,
  "bitLockerEncryptDevice": true,
  "bitLockerSystemDrivePolicy": {
    "@odata.type": "microsoft.graph.bitLockerSystemDrivePolicy",
    "encryptionMethod": "aesCbc256",
    "startupAuthenticationRequired": true,
    "startupAuthenticationBlockWithoutTpmChip": true,
    "startupAuthenticationTpmUsage": "required",
    "startupAuthenticationTpmPinUsage": "required",
    "startupAuthenticationTpmKeyUsage": "required",
    "startupAuthenticationTpmPinAndKeyUsage": "required",
    "minimumPinLength": 0,
    "recoveryOptions": {
      "@odata.type": "microsoft.graph.bitLockerRecoveryOptions",
      "blockDataRecoveryAgent": true,
      "recoveryPasswordUsage": "required",
      "recoveryKeyUsage": "required",
      "hideRecoveryOptions": true,
      "enableRecoveryInformationSaveToStore": true,
      "recoveryInformationToStore": "passwordOnly",
      "enableBitLockerAfterRecoveryInformationToStore": true
    },
    "prebootRecoveryEnableMessageAndUrl": true,
    "prebootRecoveryMessage": "Preboot Recovery Message value",
    "prebootRecoveryUrl": "https://example.com/prebootRecoveryUrl/"
  },
  "bitLockerFixedDrivePolicy": {
    "@odata.type": "microsoft.graph.bitLockerFixedDrivePolicy",
    "encryptionMethod": "aesCbc256",
    "requireEncryptionForWriteAccess": true,
    "recoveryOptions": {
      "@odata.type": "microsoft.graph.bitLockerRecoveryOptions",
      "blockDataRecoveryAgent": true,
      "recoveryPasswordUsage": "required",
      "recoveryKeyUsage": "required",
      "hideRecoveryOptions": true,
      "enableRecoveryInformationSaveToStore": true,
      "recoveryInformationToStore": "passwordOnly",
      "enableBitLockerAfterRecoveryInformationToStore": true
    }
  },
  "bitLockerRemovableDrivePolicy": {
    "@odata.type": "microsoft.graph.bitLockerRemovableDrivePolicy",
    "encryptionMethod": "aesCbc256",
    "requireEncryptionForWriteAccess": true,
    "blockCrossOrganizationWriteAccess": true
  },
  "bitLockerRecoveryPasswordRotation": "disabled",
  "defenderDisableScanArchiveFiles": true,
  "defenderAllowScanArchiveFiles": true,
  "defenderDisableBehaviorMonitoring": true,
  "defenderAllowBehaviorMonitoring": true,
  "defenderDisableCloudProtection": true,
  "defenderAllowCloudProtection": true,
  "defenderEnableScanIncomingMail": true,
  "defenderEnableScanMappedNetworkDrivesDuringFullScan": true,
  "defenderDisableScanRemovableDrivesDuringFullScan": true,
  "defenderAllowScanRemovableDrivesDuringFullScan": true,
  "defenderDisableScanDownloads": true,
  "defenderAllowScanDownloads": true,
  "defenderDisableIntrusionPreventionSystem": true,
  "defenderAllowIntrusionPreventionSystem": true,
  "defenderDisableOnAccessProtection": true,
  "defenderAllowOnAccessProtection": true,
  "defenderDisableRealTimeMonitoring": true,
  "defenderAllowRealTimeMonitoring": true,
  "defenderDisableScanNetworkFiles": true,
  "defenderAllowScanNetworkFiles": true,
  "defenderDisableScanScriptsLoadedInInternetExplorer": true,
  "defenderAllowScanScriptsLoadedInInternetExplorer": true,
  "defenderBlockEndUserAccess": true,
  "defenderAllowEndUserAccess": true,
  "defenderScanMaxCpuPercentage": 12,
  "defenderCheckForSignaturesBeforeRunningScan": true,
  "defenderCloudBlockLevel": "high",
  "defenderCloudExtendedTimeoutInSeconds": 5,
  "defenderDaysBeforeDeletingQuarantinedMalware": 12,
  "defenderDisableCatchupFullScan": true,
  "defenderDisableCatchupQuickScan": true,
  "defenderEnableLowCpuPriority": true,
  "defenderFileExtensionsToExclude": [
    "Defender File Extensions To Exclude value"
  ],
  "defenderFilesAndFoldersToExclude": [
    "Defender Files And Folders To Exclude value"
  ],
  "defenderProcessesToExclude": [
    "Defender Processes To Exclude value"
  ],
  "defenderPotentiallyUnwantedAppAction": "enable",
  "defenderScanDirection": "monitorIncomingFilesOnly",
  "defenderScanType": "disabled",
  "defenderScheduledQuickScanTime": "11:58:49.3840000",
  "defenderScheduledScanDay": "everyday",
  "defenderScheduledScanTime": "11:59:10.9990000",
  "defenderSignatureUpdateIntervalInHours": 6,
  "defenderSubmitSamplesConsentType": "alwaysPrompt",
  "defenderDetectedMalwareActions": {
    "@odata.type": "microsoft.graph.defenderDetectedMalwareActions",
    "lowSeverity": "clean",
    "moderateSeverity": "clean",
    "highSeverity": "clean",
    "severeSeverity": "clean"
  }
}
```

### <a name="response"></a><span data-ttu-id="22833-1006">响应</span><span class="sxs-lookup"><span data-stu-id="22833-1006">Response</span></span>
<span data-ttu-id="22833-p226">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="22833-p226">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 31440

{
  "@odata.type": "#microsoft.graph.windows10EndpointProtectionConfiguration",
  "id": "09709403-9403-0970-0394-700903947009",
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
  "dmaGuardDeviceEnumerationPolicy": "blockAll",
  "firewallRules": [
    {
      "@odata.type": "microsoft.graph.windowsFirewallRule",
      "displayName": "Display Name value",
      "description": "Description value",
      "packageFamilyName": "Package Family Name value",
      "filePath": "File Path value",
      "serviceName": "Service Name value",
      "protocol": 8,
      "localPortRanges": [
        "Local Port Ranges value"
      ],
      "remotePortRanges": [
        "Remote Port Ranges value"
      ],
      "localAddressRanges": [
        "Local Address Ranges value"
      ],
      "remoteAddressRanges": [
        "Remote Address Ranges value"
      ],
      "profileTypes": "domain",
      "action": "blocked",
      "trafficDirection": "out",
      "interfaceTypes": "remoteAccess",
      "edgeTraversal": "blocked",
      "localUserAuthorizations": "Local User Authorizations value"
    }
  ],
  "userRightsAccessCredentialManagerAsTrustedCaller": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsAllowAccessFromNetwork": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsBlockAccessFromNetwork": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsActAsPartOfTheOperatingSystem": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsLocalLogOn": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsDenyLocalLogOn": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsBackupData": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsChangeSystemTime": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsCreateGlobalObjects": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsCreatePageFile": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsCreatePermanentSharedObjects": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsCreateSymbolicLinks": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsCreateToken": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsDebugPrograms": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsRemoteDesktopServicesLogOn": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsDelegation": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsGenerateSecurityAudits": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsImpersonateClient": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsIncreaseSchedulingPriority": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsLoadUnloadDrivers": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsLockMemory": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsManageAuditingAndSecurityLogs": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsManageVolumes": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsModifyFirmwareEnvironment": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsModifyObjectLabels": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsProfileSingleProcess": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsRemoteShutdown": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsRestoreData": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsTakeOwnership": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "xboxServicesEnableXboxGameSaveTask": true,
  "xboxServicesAccessoryManagementServiceStartupMode": "automatic",
  "xboxServicesLiveAuthManagerServiceStartupMode": "automatic",
  "xboxServicesLiveGameSaveServiceStartupMode": "automatic",
  "xboxServicesLiveNetworkingServiceStartupMode": "automatic",
  "localSecurityOptionsBlockMicrosoftAccounts": true,
  "localSecurityOptionsBlockRemoteLogonWithBlankPassword": true,
  "localSecurityOptionsDisableAdministratorAccount": true,
  "localSecurityOptionsAdministratorAccountName": "Local Security Options Administrator Account Name value",
  "localSecurityOptionsDisableGuestAccount": true,
  "localSecurityOptionsGuestAccountName": "Local Security Options Guest Account Name value",
  "localSecurityOptionsAllowUndockWithoutHavingToLogon": true,
  "localSecurityOptionsBlockUsersInstallingPrinterDrivers": true,
  "localSecurityOptionsBlockRemoteOpticalDriveAccess": true,
  "localSecurityOptionsFormatAndEjectOfRemovableMediaAllowedUser": "administrators",
  "localSecurityOptionsMachineInactivityLimit": 10,
  "localSecurityOptionsMachineInactivityLimitInMinutes": 3,
  "localSecurityOptionsDoNotRequireCtrlAltDel": true,
  "localSecurityOptionsHideLastSignedInUser": true,
  "localSecurityOptionsHideUsernameAtSignIn": true,
  "localSecurityOptionsLogOnMessageTitle": "Local Security Options Log On Message Title value",
  "localSecurityOptionsLogOnMessageText": "Local Security Options Log On Message Text value",
  "localSecurityOptionsAllowPKU2UAuthenticationRequests": true,
  "localSecurityOptionsAllowRemoteCallsToSecurityAccountsManagerHelperBool": true,
  "localSecurityOptionsAllowRemoteCallsToSecurityAccountsManager": "Local Security Options Allow Remote Calls To Security Accounts Manager value",
  "localSecurityOptionsMinimumSessionSecurityForNtlmSspBasedClients": "requireNtmlV2SessionSecurity",
  "localSecurityOptionsMinimumSessionSecurityForNtlmSspBasedServers": "requireNtmlV2SessionSecurity",
  "lanManagerAuthenticationLevel": "lmNtlmAndNtlmV2",
  "lanManagerWorkstationDisableInsecureGuestLogons": true,
  "localSecurityOptionsClearVirtualMemoryPageFile": true,
  "localSecurityOptionsAllowSystemToBeShutDownWithoutHavingToLogOn": true,
  "localSecurityOptionsAllowUIAccessApplicationElevation": true,
  "localSecurityOptionsVirtualizeFileAndRegistryWriteFailuresToPerUserLocations": true,
  "localSecurityOptionsOnlyElevateSignedExecutables": true,
  "localSecurityOptionsAdministratorElevationPromptBehavior": "elevateWithoutPrompting",
  "localSecurityOptionsStandardUserElevationPromptBehavior": "automaticallyDenyElevationRequests",
  "localSecurityOptionsSwitchToSecureDesktopWhenPromptingForElevation": true,
  "localSecurityOptionsDetectApplicationInstallationsAndPromptForElevation": true,
  "localSecurityOptionsAllowUIAccessApplicationsForSecureLocations": true,
  "localSecurityOptionsUseAdminApprovalMode": true,
  "localSecurityOptionsUseAdminApprovalModeForAdministrators": true,
  "localSecurityOptionsInformationShownOnLockScreen": "userDisplayNameDomainUser",
  "localSecurityOptionsInformationDisplayedOnLockScreen": "administrators",
  "localSecurityOptionsDisableClientDigitallySignCommunicationsIfServerAgrees": true,
  "localSecurityOptionsClientDigitallySignCommunicationsAlways": true,
  "localSecurityOptionsClientSendUnencryptedPasswordToThirdPartySMBServers": true,
  "localSecurityOptionsDisableServerDigitallySignCommunicationsAlways": true,
  "localSecurityOptionsDisableServerDigitallySignCommunicationsIfClientAgrees": true,
  "localSecurityOptionsRestrictAnonymousAccessToNamedPipesAndShares": true,
  "localSecurityOptionsDoNotAllowAnonymousEnumerationOfSAMAccounts": true,
  "localSecurityOptionsAllowAnonymousEnumerationOfSAMAccountsAndShares": true,
  "localSecurityOptionsDoNotStoreLANManagerHashValueOnNextPasswordChange": true,
  "localSecurityOptionsSmartCardRemovalBehavior": "noAction",
  "defenderSecurityCenterDisableAppBrowserUI": true,
  "defenderSecurityCenterDisableFamilyUI": true,
  "defenderSecurityCenterDisableHealthUI": true,
  "defenderSecurityCenterDisableNetworkUI": true,
  "defenderSecurityCenterDisableVirusUI": true,
  "defenderSecurityCenterDisableAccountUI": true,
  "defenderSecurityCenterDisableClearTpmUI": true,
  "defenderSecurityCenterDisableHardwareUI": true,
  "defenderSecurityCenterDisableNotificationAreaUI": true,
  "defenderSecurityCenterDisableRansomwareUI": true,
  "defenderSecurityCenterDisableSecureBootUI": true,
  "defenderSecurityCenterDisableTroubleshootingUI": true,
  "defenderSecurityCenterDisableVulnerableTpmFirmwareUpdateUI": true,
  "defenderSecurityCenterOrganizationDisplayName": "Defender Security Center Organization Display Name value",
  "defenderSecurityCenterHelpEmail": "Defender Security Center Help Email value",
  "defenderSecurityCenterHelpPhone": "Defender Security Center Help Phone value",
  "defenderSecurityCenterHelpURL": "Defender Security Center Help URL value",
  "defenderSecurityCenterNotificationsFromApp": "blockNoncriticalNotifications",
  "defenderSecurityCenterITContactDisplay": "displayInAppAndInNotifications",
  "windowsDefenderTamperProtection": "enable",
  "firewallBlockStatefulFTP": true,
  "firewallIdleTimeoutForSecurityAssociationInSeconds": 2,
  "firewallPreSharedKeyEncodingMethod": "none",
  "firewallIPSecExemptionsNone": true,
  "firewallIPSecExemptionsAllowNeighborDiscovery": true,
  "firewallIPSecExemptionsAllowICMP": true,
  "firewallIPSecExemptionsAllowRouterDiscovery": true,
  "firewallIPSecExemptionsAllowDHCP": true,
  "firewallCertificateRevocationListCheckMethod": "none",
  "firewallMergeKeyingModuleSettings": true,
  "firewallPacketQueueingMethod": "disabled",
  "firewallProfileDomain": {
    "@odata.type": "microsoft.graph.windowsFirewallNetworkProfile",
    "firewallEnabled": "blocked",
    "stealthModeRequired": true,
    "stealthModeBlocked": true,
    "incomingTrafficRequired": true,
    "incomingTrafficBlocked": true,
    "unicastResponsesToMulticastBroadcastsRequired": true,
    "unicastResponsesToMulticastBroadcastsBlocked": true,
    "inboundNotificationsRequired": true,
    "inboundNotificationsBlocked": true,
    "authorizedApplicationRulesFromGroupPolicyMerged": true,
    "authorizedApplicationRulesFromGroupPolicyNotMerged": true,
    "globalPortRulesFromGroupPolicyMerged": true,
    "globalPortRulesFromGroupPolicyNotMerged": true,
    "connectionSecurityRulesFromGroupPolicyMerged": true,
    "connectionSecurityRulesFromGroupPolicyNotMerged": true,
    "outboundConnectionsRequired": true,
    "outboundConnectionsBlocked": true,
    "inboundConnectionsRequired": true,
    "inboundConnectionsBlocked": true,
    "securedPacketExemptionAllowed": true,
    "securedPacketExemptionBlocked": true,
    "policyRulesFromGroupPolicyMerged": true,
    "policyRulesFromGroupPolicyNotMerged": true
  },
  "firewallProfilePublic": {
    "@odata.type": "microsoft.graph.windowsFirewallNetworkProfile",
    "firewallEnabled": "blocked",
    "stealthModeRequired": true,
    "stealthModeBlocked": true,
    "incomingTrafficRequired": true,
    "incomingTrafficBlocked": true,
    "unicastResponsesToMulticastBroadcastsRequired": true,
    "unicastResponsesToMulticastBroadcastsBlocked": true,
    "inboundNotificationsRequired": true,
    "inboundNotificationsBlocked": true,
    "authorizedApplicationRulesFromGroupPolicyMerged": true,
    "authorizedApplicationRulesFromGroupPolicyNotMerged": true,
    "globalPortRulesFromGroupPolicyMerged": true,
    "globalPortRulesFromGroupPolicyNotMerged": true,
    "connectionSecurityRulesFromGroupPolicyMerged": true,
    "connectionSecurityRulesFromGroupPolicyNotMerged": true,
    "outboundConnectionsRequired": true,
    "outboundConnectionsBlocked": true,
    "inboundConnectionsRequired": true,
    "inboundConnectionsBlocked": true,
    "securedPacketExemptionAllowed": true,
    "securedPacketExemptionBlocked": true,
    "policyRulesFromGroupPolicyMerged": true,
    "policyRulesFromGroupPolicyNotMerged": true
  },
  "firewallProfilePrivate": {
    "@odata.type": "microsoft.graph.windowsFirewallNetworkProfile",
    "firewallEnabled": "blocked",
    "stealthModeRequired": true,
    "stealthModeBlocked": true,
    "incomingTrafficRequired": true,
    "incomingTrafficBlocked": true,
    "unicastResponsesToMulticastBroadcastsRequired": true,
    "unicastResponsesToMulticastBroadcastsBlocked": true,
    "inboundNotificationsRequired": true,
    "inboundNotificationsBlocked": true,
    "authorizedApplicationRulesFromGroupPolicyMerged": true,
    "authorizedApplicationRulesFromGroupPolicyNotMerged": true,
    "globalPortRulesFromGroupPolicyMerged": true,
    "globalPortRulesFromGroupPolicyNotMerged": true,
    "connectionSecurityRulesFromGroupPolicyMerged": true,
    "connectionSecurityRulesFromGroupPolicyNotMerged": true,
    "outboundConnectionsRequired": true,
    "outboundConnectionsBlocked": true,
    "inboundConnectionsRequired": true,
    "inboundConnectionsBlocked": true,
    "securedPacketExemptionAllowed": true,
    "securedPacketExemptionBlocked": true,
    "policyRulesFromGroupPolicyMerged": true,
    "policyRulesFromGroupPolicyNotMerged": true
  },
  "defenderAdobeReaderLaunchChildProcess": "enable",
  "defenderAttackSurfaceReductionExcludedPaths": [
    "Defender Attack Surface Reduction Excluded Paths value"
  ],
  "defenderOfficeAppsOtherProcessInjectionType": "block",
  "defenderOfficeAppsOtherProcessInjection": "enable",
  "defenderOfficeCommunicationAppsLaunchChildProcess": "enable",
  "defenderOfficeAppsExecutableContentCreationOrLaunchType": "block",
  "defenderOfficeAppsExecutableContentCreationOrLaunch": "enable",
  "defenderOfficeAppsLaunchChildProcessType": "block",
  "defenderOfficeAppsLaunchChildProcess": "enable",
  "defenderOfficeMacroCodeAllowWin32ImportsType": "block",
  "defenderOfficeMacroCodeAllowWin32Imports": "enable",
  "defenderScriptObfuscatedMacroCodeType": "block",
  "defenderScriptObfuscatedMacroCode": "enable",
  "defenderScriptDownloadedPayloadExecutionType": "block",
  "defenderScriptDownloadedPayloadExecution": "enable",
  "defenderPreventCredentialStealingType": "enable",
  "defenderProcessCreationType": "block",
  "defenderProcessCreation": "enable",
  "defenderUntrustedUSBProcessType": "block",
  "defenderUntrustedUSBProcess": "enable",
  "defenderUntrustedExecutableType": "block",
  "defenderUntrustedExecutable": "enable",
  "defenderEmailContentExecutionType": "block",
  "defenderEmailContentExecution": "enable",
  "defenderAdvancedRansomewareProtectionType": "enable",
  "defenderGuardMyFoldersType": "enable",
  "defenderGuardedFoldersAllowedAppPaths": [
    "Defender Guarded Folders Allowed App Paths value"
  ],
  "defenderAdditionalGuardedFolders": [
    "Defender Additional Guarded Folders value"
  ],
  "defenderNetworkProtectionType": "enable",
  "defenderExploitProtectionXml": "ZGVmZW5kZXJFeHBsb2l0UHJvdGVjdGlvblhtbA==",
  "defenderExploitProtectionXmlFileName": "Defender Exploit Protection Xml File Name value",
  "defenderSecurityCenterBlockExploitProtectionOverride": true,
  "defenderBlockPersistenceThroughWmiType": "block",
  "appLockerApplicationControl": "enforceComponentsAndStoreApps",
  "deviceGuardLocalSystemAuthorityCredentialGuardSettings": "enableWithUEFILock",
  "deviceGuardEnableVirtualizationBasedSecurity": true,
  "deviceGuardEnableSecureBootWithDMA": true,
  "deviceGuardSecureBootWithDMA": "withoutDMA",
  "deviceGuardLaunchSystemGuard": "enabled",
  "smartScreenEnableInShell": true,
  "smartScreenBlockOverrideForFiles": true,
  "applicationGuardEnabled": true,
  "applicationGuardEnabledOptions": "enabledForEdge",
  "applicationGuardBlockFileTransfer": "blockImageAndTextFile",
  "applicationGuardBlockNonEnterpriseContent": true,
  "applicationGuardAllowPersistence": true,
  "applicationGuardForceAuditing": true,
  "applicationGuardBlockClipboardSharing": "blockBoth",
  "applicationGuardAllowPrintToPDF": true,
  "applicationGuardAllowPrintToXPS": true,
  "applicationGuardAllowPrintToLocalPrinters": true,
  "applicationGuardAllowPrintToNetworkPrinters": true,
  "applicationGuardAllowVirtualGPU": true,
  "applicationGuardAllowFileSaveOnHost": true,
  "applicationGuardAllowCameraMicrophoneRedirection": true,
  "applicationGuardCertificateThumbprints": [
    "Application Guard Certificate Thumbprints value"
  ],
  "bitLockerAllowStandardUserEncryption": true,
  "bitLockerDisableWarningForOtherDiskEncryption": true,
  "bitLockerEnableStorageCardEncryptionOnMobile": true,
  "bitLockerEncryptDevice": true,
  "bitLockerSystemDrivePolicy": {
    "@odata.type": "microsoft.graph.bitLockerSystemDrivePolicy",
    "encryptionMethod": "aesCbc256",
    "startupAuthenticationRequired": true,
    "startupAuthenticationBlockWithoutTpmChip": true,
    "startupAuthenticationTpmUsage": "required",
    "startupAuthenticationTpmPinUsage": "required",
    "startupAuthenticationTpmKeyUsage": "required",
    "startupAuthenticationTpmPinAndKeyUsage": "required",
    "minimumPinLength": 0,
    "recoveryOptions": {
      "@odata.type": "microsoft.graph.bitLockerRecoveryOptions",
      "blockDataRecoveryAgent": true,
      "recoveryPasswordUsage": "required",
      "recoveryKeyUsage": "required",
      "hideRecoveryOptions": true,
      "enableRecoveryInformationSaveToStore": true,
      "recoveryInformationToStore": "passwordOnly",
      "enableBitLockerAfterRecoveryInformationToStore": true
    },
    "prebootRecoveryEnableMessageAndUrl": true,
    "prebootRecoveryMessage": "Preboot Recovery Message value",
    "prebootRecoveryUrl": "https://example.com/prebootRecoveryUrl/"
  },
  "bitLockerFixedDrivePolicy": {
    "@odata.type": "microsoft.graph.bitLockerFixedDrivePolicy",
    "encryptionMethod": "aesCbc256",
    "requireEncryptionForWriteAccess": true,
    "recoveryOptions": {
      "@odata.type": "microsoft.graph.bitLockerRecoveryOptions",
      "blockDataRecoveryAgent": true,
      "recoveryPasswordUsage": "required",
      "recoveryKeyUsage": "required",
      "hideRecoveryOptions": true,
      "enableRecoveryInformationSaveToStore": true,
      "recoveryInformationToStore": "passwordOnly",
      "enableBitLockerAfterRecoveryInformationToStore": true
    }
  },
  "bitLockerRemovableDrivePolicy": {
    "@odata.type": "microsoft.graph.bitLockerRemovableDrivePolicy",
    "encryptionMethod": "aesCbc256",
    "requireEncryptionForWriteAccess": true,
    "blockCrossOrganizationWriteAccess": true
  },
  "bitLockerRecoveryPasswordRotation": "disabled",
  "defenderDisableScanArchiveFiles": true,
  "defenderAllowScanArchiveFiles": true,
  "defenderDisableBehaviorMonitoring": true,
  "defenderAllowBehaviorMonitoring": true,
  "defenderDisableCloudProtection": true,
  "defenderAllowCloudProtection": true,
  "defenderEnableScanIncomingMail": true,
  "defenderEnableScanMappedNetworkDrivesDuringFullScan": true,
  "defenderDisableScanRemovableDrivesDuringFullScan": true,
  "defenderAllowScanRemovableDrivesDuringFullScan": true,
  "defenderDisableScanDownloads": true,
  "defenderAllowScanDownloads": true,
  "defenderDisableIntrusionPreventionSystem": true,
  "defenderAllowIntrusionPreventionSystem": true,
  "defenderDisableOnAccessProtection": true,
  "defenderAllowOnAccessProtection": true,
  "defenderDisableRealTimeMonitoring": true,
  "defenderAllowRealTimeMonitoring": true,
  "defenderDisableScanNetworkFiles": true,
  "defenderAllowScanNetworkFiles": true,
  "defenderDisableScanScriptsLoadedInInternetExplorer": true,
  "defenderAllowScanScriptsLoadedInInternetExplorer": true,
  "defenderBlockEndUserAccess": true,
  "defenderAllowEndUserAccess": true,
  "defenderScanMaxCpuPercentage": 12,
  "defenderCheckForSignaturesBeforeRunningScan": true,
  "defenderCloudBlockLevel": "high",
  "defenderCloudExtendedTimeoutInSeconds": 5,
  "defenderDaysBeforeDeletingQuarantinedMalware": 12,
  "defenderDisableCatchupFullScan": true,
  "defenderDisableCatchupQuickScan": true,
  "defenderEnableLowCpuPriority": true,
  "defenderFileExtensionsToExclude": [
    "Defender File Extensions To Exclude value"
  ],
  "defenderFilesAndFoldersToExclude": [
    "Defender Files And Folders To Exclude value"
  ],
  "defenderProcessesToExclude": [
    "Defender Processes To Exclude value"
  ],
  "defenderPotentiallyUnwantedAppAction": "enable",
  "defenderScanDirection": "monitorIncomingFilesOnly",
  "defenderScanType": "disabled",
  "defenderScheduledQuickScanTime": "11:58:49.3840000",
  "defenderScheduledScanDay": "everyday",
  "defenderScheduledScanTime": "11:59:10.9990000",
  "defenderSignatureUpdateIntervalInHours": 6,
  "defenderSubmitSamplesConsentType": "alwaysPrompt",
  "defenderDetectedMalwareActions": {
    "@odata.type": "microsoft.graph.defenderDetectedMalwareActions",
    "lowSeverity": "clean",
    "moderateSeverity": "clean",
    "highSeverity": "clean",
    "severeSeverity": "clean"
  }
}
```




