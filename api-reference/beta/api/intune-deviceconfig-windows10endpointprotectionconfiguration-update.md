---
title: 更新 windows10EndpointProtectionConfiguration
description: 更新 windows10EndpointProtectionConfiguration 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 19593b4e70b839513c305c153324c868f4adcc1d
ms.sourcegitcommit: d4114bac58628527611e83e436132c6581a19c52
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/13/2020
ms.locfileid: "43431194"
---
# <a name="update-windows10endpointprotectionconfiguration"></a><span data-ttu-id="801ab-103">更新 windows10EndpointProtectionConfiguration</span><span class="sxs-lookup"><span data-stu-id="801ab-103">Update windows10EndpointProtectionConfiguration</span></span>

<span data-ttu-id="801ab-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="801ab-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="801ab-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="801ab-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="801ab-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="801ab-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="801ab-107">更新 [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="801ab-107">Update the properties of a [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="801ab-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="801ab-108">Prerequisites</span></span>
<span data-ttu-id="801ab-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="801ab-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="801ab-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="801ab-111">Permission type</span></span>|<span data-ttu-id="801ab-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="801ab-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="801ab-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="801ab-113">Delegated (work or school account)</span></span>|<span data-ttu-id="801ab-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="801ab-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="801ab-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="801ab-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="801ab-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="801ab-116">Not supported.</span></span>|
|<span data-ttu-id="801ab-117">Application</span><span class="sxs-lookup"><span data-stu-id="801ab-117">Application</span></span>|<span data-ttu-id="801ab-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="801ab-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="801ab-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="801ab-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="801ab-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="801ab-120">Request headers</span></span>
|<span data-ttu-id="801ab-121">标头</span><span class="sxs-lookup"><span data-stu-id="801ab-121">Header</span></span>|<span data-ttu-id="801ab-122">值</span><span class="sxs-lookup"><span data-stu-id="801ab-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="801ab-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="801ab-123">Authorization</span></span>|<span data-ttu-id="801ab-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="801ab-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="801ab-125">接受</span><span class="sxs-lookup"><span data-stu-id="801ab-125">Accept</span></span>|<span data-ttu-id="801ab-126">application/json</span><span class="sxs-lookup"><span data-stu-id="801ab-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="801ab-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="801ab-127">Request body</span></span>
<span data-ttu-id="801ab-128">在请求正文中，提供 [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="801ab-128">In the request body, supply a JSON representation for the [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) object.</span></span>

<span data-ttu-id="801ab-129">下表显示了创建 [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="801ab-129">The following table shows the properties that are required when you create the [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md).</span></span>

|<span data-ttu-id="801ab-130">属性</span><span class="sxs-lookup"><span data-stu-id="801ab-130">Property</span></span>|<span data-ttu-id="801ab-131">类型</span><span class="sxs-lookup"><span data-stu-id="801ab-131">Type</span></span>|<span data-ttu-id="801ab-132">说明</span><span class="sxs-lookup"><span data-stu-id="801ab-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="801ab-133">id</span><span class="sxs-lookup"><span data-stu-id="801ab-133">id</span></span>|<span data-ttu-id="801ab-134">字符串</span><span class="sxs-lookup"><span data-stu-id="801ab-134">String</span></span>|<span data-ttu-id="801ab-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="801ab-135">Key of the entity.</span></span> <span data-ttu-id="801ab-136">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="801ab-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="801ab-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="801ab-137">lastModifiedDateTime</span></span>|<span data-ttu-id="801ab-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="801ab-138">DateTimeOffset</span></span>|<span data-ttu-id="801ab-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="801ab-139">DateTime the object was last modified.</span></span> <span data-ttu-id="801ab-140">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="801ab-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="801ab-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="801ab-141">roleScopeTagIds</span></span>|<span data-ttu-id="801ab-142">字符串集合</span><span class="sxs-lookup"><span data-stu-id="801ab-142">String collection</span></span>|<span data-ttu-id="801ab-143">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="801ab-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="801ab-144">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="801ab-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="801ab-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="801ab-145">supportsScopeTags</span></span>|<span data-ttu-id="801ab-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="801ab-146">Boolean</span></span>|<span data-ttu-id="801ab-147">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="801ab-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="801ab-148">如果此值为 false，则不允许分配给 ScopeTags 属性，并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="801ab-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="801ab-149">这适用于在 Silverlight 中创建的旧版策略，可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="801ab-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="801ab-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="801ab-150">This property is read-only.</span></span> <span data-ttu-id="801ab-151">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="801ab-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="801ab-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="801ab-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="801ab-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="801ab-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="801ab-154">适用于此策略的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="801ab-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="801ab-155">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="801ab-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="801ab-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="801ab-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="801ab-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="801ab-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="801ab-158">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="801ab-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="801ab-159">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="801ab-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="801ab-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="801ab-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="801ab-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="801ab-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="801ab-162">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="801ab-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="801ab-163">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="801ab-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="801ab-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="801ab-164">createdDateTime</span></span>|<span data-ttu-id="801ab-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="801ab-165">DateTimeOffset</span></span>|<span data-ttu-id="801ab-166">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="801ab-166">DateTime the object was created.</span></span> <span data-ttu-id="801ab-167">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="801ab-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="801ab-168">说明</span><span class="sxs-lookup"><span data-stu-id="801ab-168">description</span></span>|<span data-ttu-id="801ab-169">String</span><span class="sxs-lookup"><span data-stu-id="801ab-169">String</span></span>|<span data-ttu-id="801ab-170">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="801ab-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="801ab-171">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="801ab-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="801ab-172">displayName</span><span class="sxs-lookup"><span data-stu-id="801ab-172">displayName</span></span>|<span data-ttu-id="801ab-173">String</span><span class="sxs-lookup"><span data-stu-id="801ab-173">String</span></span>|<span data-ttu-id="801ab-174">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="801ab-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="801ab-175">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="801ab-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="801ab-176">version</span><span class="sxs-lookup"><span data-stu-id="801ab-176">version</span></span>|<span data-ttu-id="801ab-177">Int32</span><span class="sxs-lookup"><span data-stu-id="801ab-177">Int32</span></span>|<span data-ttu-id="801ab-178">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="801ab-178">Version of the device configuration.</span></span> <span data-ttu-id="801ab-179">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="801ab-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="801ab-180">dmaGuardDeviceEnumerationPolicy</span><span class="sxs-lookup"><span data-stu-id="801ab-180">dmaGuardDeviceEnumerationPolicy</span></span>|[<span data-ttu-id="801ab-181">dmaGuardDeviceEnumerationPolicyType</span><span class="sxs-lookup"><span data-stu-id="801ab-181">dmaGuardDeviceEnumerationPolicyType</span></span>](../resources/intune-deviceconfig-dmaguarddeviceenumerationpolicytype.md)|<span data-ttu-id="801ab-182">此策略旨在提供针对支持外部 DMA 的设备的额外安全性。</span><span class="sxs-lookup"><span data-stu-id="801ab-182">This policy is intended to provide additional security against external DMA capable devices.</span></span> <span data-ttu-id="801ab-183">通过它，可以更好地控制支持外部 DMA 的设备与 DMA 重新映射/设备内存隔离和沙盒不兼容的枚举。</span><span class="sxs-lookup"><span data-stu-id="801ab-183">It allows for more control over the enumeration of external DMA capable devices incompatible with DMA Remapping/device memory isolation and sandboxing.</span></span> <span data-ttu-id="801ab-184">仅当系统固件支持和启用内核 DMA 保护时，此策略才会生效。</span><span class="sxs-lookup"><span data-stu-id="801ab-184">This policy only takes effect when Kernel DMA Protection is supported and enabled by the system firmware.</span></span> <span data-ttu-id="801ab-185">内核 DMA 保护是一项平台功能，不能通过策略或最终用户进行控制。</span><span class="sxs-lookup"><span data-stu-id="801ab-185">Kernel DMA Protection is a platform feature that cannot be controlled via policy or by end user.</span></span> <span data-ttu-id="801ab-186">在制造时，系统必须支持它。</span><span class="sxs-lookup"><span data-stu-id="801ab-186">It has to be supported by the system at the time of manufacturing.</span></span> <span data-ttu-id="801ab-187">若要检查系统是否支持内核 DMA 保护，请在 MSINFO32 的摘要页中检查 "内核 DMA 保护" 字段。</span><span class="sxs-lookup"><span data-stu-id="801ab-187">To check if the system supports Kernel DMA Protection, please check the Kernel DMA Protection field in the Summary page of MSINFO32.exe.</span></span> <span data-ttu-id="801ab-188">可取值为：`deviceDefault`、`blockAll`、`allowAll`。</span><span class="sxs-lookup"><span data-stu-id="801ab-188">Possible values are: `deviceDefault`, `blockAll`, `allowAll`.</span></span>|
|<span data-ttu-id="801ab-189">firewallRules</span><span class="sxs-lookup"><span data-stu-id="801ab-189">firewallRules</span></span>|<span data-ttu-id="801ab-190">[windowsFirewallRule](../resources/intune-deviceconfig-windowsfirewallrule.md)集合</span><span class="sxs-lookup"><span data-stu-id="801ab-190">[windowsFirewallRule](../resources/intune-deviceconfig-windowsfirewallrule.md) collection</span></span>|<span data-ttu-id="801ab-191">配置防火墙规则设置。</span><span class="sxs-lookup"><span data-stu-id="801ab-191">Configures the firewall rule settings.</span></span> <span data-ttu-id="801ab-192">此集合最多可包含150个元素。</span><span class="sxs-lookup"><span data-stu-id="801ab-192">This collection can contain a maximum of 150 elements.</span></span>|
|<span data-ttu-id="801ab-193">userRightsAccessCredentialManagerAsTrustedCaller</span><span class="sxs-lookup"><span data-stu-id="801ab-193">userRightsAccessCredentialManagerAsTrustedCaller</span></span>|[<span data-ttu-id="801ab-194">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="801ab-194">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="801ab-195">此用户权限由凭据管理器在备份/还原过程中使用。</span><span class="sxs-lookup"><span data-stu-id="801ab-195">This user right is used by Credential Manager during Backup/Restore.</span></span> <span data-ttu-id="801ab-196">如果为其他实体提供此权限，则用户保存的凭据可能会受到威胁。</span><span class="sxs-lookup"><span data-stu-id="801ab-196">Users' saved credentials might be compromised if this privilege is given to other entities.</span></span> <span data-ttu-id="801ab-197">仅支持 NotConfigured 和允许的状态</span><span class="sxs-lookup"><span data-stu-id="801ab-197">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="801ab-198">userRightsAllowAccessFromNetwork</span><span class="sxs-lookup"><span data-stu-id="801ab-198">userRightsAllowAccessFromNetwork</span></span>|[<span data-ttu-id="801ab-199">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="801ab-199">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="801ab-200">此用户权限确定允许哪些用户和组通过网络连接到计算机。</span><span class="sxs-lookup"><span data-stu-id="801ab-200">This user right determines which users and groups are allowed to connect to the computer over the network.</span></span> <span data-ttu-id="801ab-201">支持的状态为 "允许"。</span><span class="sxs-lookup"><span data-stu-id="801ab-201">State Allowed is supported.</span></span>|
|<span data-ttu-id="801ab-202">userRightsBlockAccessFromNetwork</span><span class="sxs-lookup"><span data-stu-id="801ab-202">userRightsBlockAccessFromNetwork</span></span>|[<span data-ttu-id="801ab-203">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="801ab-203">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="801ab-204">此用户权限决定了阻止哪些用户和组通过网络连接到计算机。</span><span class="sxs-lookup"><span data-stu-id="801ab-204">This user right determines which users and groups are block from connecting to the computer over the network.</span></span> <span data-ttu-id="801ab-205">支持状态块。</span><span class="sxs-lookup"><span data-stu-id="801ab-205">State Block is supported.</span></span>|
|<span data-ttu-id="801ab-206">userRightsActAsPartOfTheOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="801ab-206">userRightsActAsPartOfTheOperatingSystem</span></span>|[<span data-ttu-id="801ab-207">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="801ab-207">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="801ab-208">此用户权限允许进程在不进行身份验证的情况下模拟任何用户。</span><span class="sxs-lookup"><span data-stu-id="801ab-208">This user right allows a process to impersonate any user without authentication.</span></span> <span data-ttu-id="801ab-209">因此，该过程可以获得与该用户相同的本地资源的访问权限。</span><span class="sxs-lookup"><span data-stu-id="801ab-209">The process can therefore gain access to the same local resources as that user.</span></span> <span data-ttu-id="801ab-210">仅支持 NotConfigured 和允许的状态</span><span class="sxs-lookup"><span data-stu-id="801ab-210">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="801ab-211">userRightsLocalLogOn</span><span class="sxs-lookup"><span data-stu-id="801ab-211">userRightsLocalLogOn</span></span>|[<span data-ttu-id="801ab-212">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="801ab-212">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="801ab-213">此用户权限确定哪些用户可以登录到计算机。</span><span class="sxs-lookup"><span data-stu-id="801ab-213">This user right determines which users can log on to the computer.</span></span> <span data-ttu-id="801ab-214">支持的状态 NotConfigured （允许）</span><span class="sxs-lookup"><span data-stu-id="801ab-214">States NotConfigured, Allowed are supported</span></span> |
|<span data-ttu-id="801ab-215">userRightsDenyLocalLogOn</span><span class="sxs-lookup"><span data-stu-id="801ab-215">userRightsDenyLocalLogOn</span></span>|[<span data-ttu-id="801ab-216">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="801ab-216">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="801ab-217">此用户权限确定哪些用户无法登录到计算机。</span><span class="sxs-lookup"><span data-stu-id="801ab-217">This user right determines which users cannot log on to the computer.</span></span> <span data-ttu-id="801ab-218">状态 NotConfigured，受阻止</span><span class="sxs-lookup"><span data-stu-id="801ab-218">States NotConfigured, Blocked are supported</span></span> |
|<span data-ttu-id="801ab-219">userRightsBackupData</span><span class="sxs-lookup"><span data-stu-id="801ab-219">userRightsBackupData</span></span>|[<span data-ttu-id="801ab-220">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="801ab-220">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="801ab-221">此用户权限确定在备份文件和目录时，哪些用户可以绕过文件、目录、注册表和其他持久对象权限。</span><span class="sxs-lookup"><span data-stu-id="801ab-221">This user right determines which users can bypass file, directory, registry, and other persistent objects permissions when backing up files and directories.</span></span> <span data-ttu-id="801ab-222">仅支持 NotConfigured 和允许的状态</span><span class="sxs-lookup"><span data-stu-id="801ab-222">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="801ab-223">userRightsChangeSystemTime</span><span class="sxs-lookup"><span data-stu-id="801ab-223">userRightsChangeSystemTime</span></span>|[<span data-ttu-id="801ab-224">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="801ab-224">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="801ab-225">此用户权限确定哪些用户和组可以更改计算机内部时钟上的时间和日期。</span><span class="sxs-lookup"><span data-stu-id="801ab-225">This user right determines which users and groups can change the time and date on the internal clock of the computer.</span></span> <span data-ttu-id="801ab-226">仅支持 NotConfigured 和允许的状态</span><span class="sxs-lookup"><span data-stu-id="801ab-226">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="801ab-227">userRightsCreateGlobalObjects</span><span class="sxs-lookup"><span data-stu-id="801ab-227">userRightsCreateGlobalObjects</span></span>|[<span data-ttu-id="801ab-228">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="801ab-228">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="801ab-229">此安全设置确定用户是否可以创建可用于所有会话的全局对象。</span><span class="sxs-lookup"><span data-stu-id="801ab-229">This security setting determines whether users can create global objects that are available to all sessions.</span></span> <span data-ttu-id="801ab-230">可以创建全局对象的用户可能会影响在其他用户的会话下运行的进程，这可能导致应用程序故障或数据损坏。</span><span class="sxs-lookup"><span data-stu-id="801ab-230">Users who can create global objects could affect processes that run under other users' sessions, which could lead to application failure or data corruption.</span></span> <span data-ttu-id="801ab-231">仅支持 NotConfigured 和允许的状态</span><span class="sxs-lookup"><span data-stu-id="801ab-231">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="801ab-232">userRightsCreatePageFile</span><span class="sxs-lookup"><span data-stu-id="801ab-232">userRightsCreatePageFile</span></span>|[<span data-ttu-id="801ab-233">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="801ab-233">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="801ab-234">此用户权限确定哪些用户和组可以调用内部 API 来创建和更改页面文件的大小。</span><span class="sxs-lookup"><span data-stu-id="801ab-234">This user right determines which users and groups can call an internal API to create and change the size of a page file.</span></span> <span data-ttu-id="801ab-235">仅支持 NotConfigured 和允许的状态</span><span class="sxs-lookup"><span data-stu-id="801ab-235">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="801ab-236">userRightsCreatePermanentSharedObjects</span><span class="sxs-lookup"><span data-stu-id="801ab-236">userRightsCreatePermanentSharedObjects</span></span>|[<span data-ttu-id="801ab-237">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="801ab-237">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="801ab-238">此用户权限决定了进程可以使用哪些帐户使用对象管理器创建目录对象。</span><span class="sxs-lookup"><span data-stu-id="801ab-238">This user right determines which accounts can be used by processes to create a directory object using the object manager.</span></span> <span data-ttu-id="801ab-239">仅支持 NotConfigured 和允许的状态</span><span class="sxs-lookup"><span data-stu-id="801ab-239">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="801ab-240">userRightsCreateSymbolicLinks</span><span class="sxs-lookup"><span data-stu-id="801ab-240">userRightsCreateSymbolicLinks</span></span>|[<span data-ttu-id="801ab-241">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="801ab-241">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="801ab-242">此用户权限确定用户是否可以从其登录到的计算机创建符号链接。</span><span class="sxs-lookup"><span data-stu-id="801ab-242">This user right determines if the user can create a symbolic link from the computer to which they are logged on.</span></span> <span data-ttu-id="801ab-243">仅支持 NotConfigured 和允许的状态</span><span class="sxs-lookup"><span data-stu-id="801ab-243">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="801ab-244">userRightsCreateToken</span><span class="sxs-lookup"><span data-stu-id="801ab-244">userRightsCreateToken</span></span>|[<span data-ttu-id="801ab-245">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="801ab-245">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="801ab-246">此用户权限确定进程在使用内部 API 创建访问令牌时，可以使用哪些用户/组来创建令牌，然后可以使用这些用户/组来获取对任何本地资源的访问权限。</span><span class="sxs-lookup"><span data-stu-id="801ab-246">This user right determines which users/groups can be used by processes to create a token that can then be used to get access to any local resources when the process uses an internal API to create an access token.</span></span> <span data-ttu-id="801ab-247">仅支持 NotConfigured 和允许的状态</span><span class="sxs-lookup"><span data-stu-id="801ab-247">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="801ab-248">userRightsDebugPrograms</span><span class="sxs-lookup"><span data-stu-id="801ab-248">userRightsDebugPrograms</span></span>|[<span data-ttu-id="801ab-249">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="801ab-249">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="801ab-250">此用户权限确定哪些用户可以将调试程序附加到任何进程或内核。</span><span class="sxs-lookup"><span data-stu-id="801ab-250">This user right determines which users can attach a debugger to any process or to the kernel.</span></span> <span data-ttu-id="801ab-251">仅支持 NotConfigured 和允许的状态</span><span class="sxs-lookup"><span data-stu-id="801ab-251">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="801ab-252">userRightsRemoteDesktopServicesLogOn</span><span class="sxs-lookup"><span data-stu-id="801ab-252">userRightsRemoteDesktopServicesLogOn</span></span>|[<span data-ttu-id="801ab-253">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="801ab-253">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="801ab-254">此用户权限确定禁止哪些用户和组作为远程桌面服务客户端进行登录。</span><span class="sxs-lookup"><span data-stu-id="801ab-254">This user right determines which users and groups are prohibited from logging on as a Remote Desktop Services client.</span></span> <span data-ttu-id="801ab-255">仅支持状态 NotConfigured 和阻止</span><span class="sxs-lookup"><span data-stu-id="801ab-255">Only states NotConfigured and Blocked are supported</span></span>|
|<span data-ttu-id="801ab-256">userRightsDelegation</span><span class="sxs-lookup"><span data-stu-id="801ab-256">userRightsDelegation</span></span>|[<span data-ttu-id="801ab-257">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="801ab-257">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="801ab-258">此用户权限确定哪些用户可以在用户或计算机对象上设置受信任委派设置。</span><span class="sxs-lookup"><span data-stu-id="801ab-258">This user right determines which users can set the Trusted for Delegation setting on a user or computer object.</span></span> <span data-ttu-id="801ab-259">仅支持 NotConfigured 和允许的状态。</span><span class="sxs-lookup"><span data-stu-id="801ab-259">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="801ab-260">userRightsGenerateSecurityAudits</span><span class="sxs-lookup"><span data-stu-id="801ab-260">userRightsGenerateSecurityAudits</span></span>|[<span data-ttu-id="801ab-261">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="801ab-261">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="801ab-262">此用户权限确定进程可使用哪些帐户向安全日志中添加条目。</span><span class="sxs-lookup"><span data-stu-id="801ab-262">This user right determines which accounts can be used by a process to add entries to the security log.</span></span> <span data-ttu-id="801ab-263">安全日志用于跟踪未经授权的系统访问。</span><span class="sxs-lookup"><span data-stu-id="801ab-263">The security log is used to trace unauthorized system access.</span></span>  <span data-ttu-id="801ab-264">仅支持 NotConfigured 和允许的状态。</span><span class="sxs-lookup"><span data-stu-id="801ab-264">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="801ab-265">userRightsImpersonateClient</span><span class="sxs-lookup"><span data-stu-id="801ab-265">userRightsImpersonateClient</span></span>|[<span data-ttu-id="801ab-266">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="801ab-266">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="801ab-267">将此用户权限分配给用户将允许代表该用户运行的程序模拟客户端。</span><span class="sxs-lookup"><span data-stu-id="801ab-267">Assigning this user right to a user allows programs running on behalf of that user to impersonate a client.</span></span> <span data-ttu-id="801ab-268">如果此类型的模拟要求此用户权限，则可以防止未经授权的用户说服客户端连接到已创建的服务，然后模拟该客户端，这样可以将未经授权的用户的权限提升到管理级别或系统级别。</span><span class="sxs-lookup"><span data-stu-id="801ab-268">Requiring this user right for this kind of impersonation prevents an unauthorized user from convincing a client to connect to a service that they have created and then impersonating that client, which can elevate the unauthorized user's permissions to administrative or system levels.</span></span> <span data-ttu-id="801ab-269">仅支持 NotConfigured 和允许的状态。</span><span class="sxs-lookup"><span data-stu-id="801ab-269">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="801ab-270">userRightsIncreaseSchedulingPriority</span><span class="sxs-lookup"><span data-stu-id="801ab-270">userRightsIncreaseSchedulingPriority</span></span>|[<span data-ttu-id="801ab-271">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="801ab-271">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="801ab-272">此用户权限确定哪些帐户可以使用具有对另一进程的 Write 属性访问权限的进程，以增加分配给其他进程的执行优先级。</span><span class="sxs-lookup"><span data-stu-id="801ab-272">This user right determines which accounts can use a process with Write Property access to another process to increase the execution priority assigned to the other process.</span></span> <span data-ttu-id="801ab-273">仅支持 NotConfigured 和允许的状态。</span><span class="sxs-lookup"><span data-stu-id="801ab-273">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="801ab-274">userRightsLoadUnloadDrivers</span><span class="sxs-lookup"><span data-stu-id="801ab-274">userRightsLoadUnloadDrivers</span></span>|[<span data-ttu-id="801ab-275">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="801ab-275">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="801ab-276">此用户权限确定哪些用户可以在内核模式下将设备驱动程序或其他代码动态加载和卸载。</span><span class="sxs-lookup"><span data-stu-id="801ab-276">This user right determines which users can dynamically load and unload device drivers or other code in to kernel mode.</span></span> <span data-ttu-id="801ab-277">仅支持 NotConfigured 和允许的状态。</span><span class="sxs-lookup"><span data-stu-id="801ab-277">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="801ab-278">userRightsLockMemory</span><span class="sxs-lookup"><span data-stu-id="801ab-278">userRightsLockMemory</span></span>|[<span data-ttu-id="801ab-279">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="801ab-279">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="801ab-280">此用户权限确定哪些帐户可以使用进程将数据保存在物理内存中，这会阻止系统将数据分页到磁盘上的虚拟内存中。</span><span class="sxs-lookup"><span data-stu-id="801ab-280">This user right determines which accounts can use a process to keep data in physical memory, which prevents the system from paging the data to virtual memory on disk.</span></span> <span data-ttu-id="801ab-281">仅支持 NotConfigured 和允许的状态。</span><span class="sxs-lookup"><span data-stu-id="801ab-281">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="801ab-282">userRightsManageAuditingAndSecurityLogs</span><span class="sxs-lookup"><span data-stu-id="801ab-282">userRightsManageAuditingAndSecurityLogs</span></span>|[<span data-ttu-id="801ab-283">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="801ab-283">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="801ab-284">此用户权限确定哪些用户可以为各个资源（如文件、Active Directory 对象和注册表项）指定对象访问审核选项。</span><span class="sxs-lookup"><span data-stu-id="801ab-284">This user right determines which users can specify object access auditing options for individual resources, such as files, Active Directory objects, and registry keys.</span></span> <span data-ttu-id="801ab-285">仅支持 NotConfigured 和允许的状态。</span><span class="sxs-lookup"><span data-stu-id="801ab-285">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="801ab-286">userRightsManageVolumes</span><span class="sxs-lookup"><span data-stu-id="801ab-286">userRightsManageVolumes</span></span>|[<span data-ttu-id="801ab-287">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="801ab-287">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="801ab-288">此用户权限确定哪些用户和组可以在某个卷（如远程碎片整理）上运行维护任务。</span><span class="sxs-lookup"><span data-stu-id="801ab-288">This user right determines which users and groups can run maintenance tasks on a volume, such as remote defragmentation.</span></span> <span data-ttu-id="801ab-289">仅支持 NotConfigured 和允许的状态。</span><span class="sxs-lookup"><span data-stu-id="801ab-289">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="801ab-290">userRightsModifyFirmwareEnvironment</span><span class="sxs-lookup"><span data-stu-id="801ab-290">userRightsModifyFirmwareEnvironment</span></span>|[<span data-ttu-id="801ab-291">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="801ab-291">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="801ab-292">此用户权限决定了可以修改固件环境值的用户。</span><span class="sxs-lookup"><span data-stu-id="801ab-292">This user right determines who can modify firmware environment values.</span></span> <span data-ttu-id="801ab-293">仅支持 NotConfigured 和允许的状态。</span><span class="sxs-lookup"><span data-stu-id="801ab-293">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="801ab-294">userRightsModifyObjectLabels</span><span class="sxs-lookup"><span data-stu-id="801ab-294">userRightsModifyObjectLabels</span></span>|[<span data-ttu-id="801ab-295">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="801ab-295">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="801ab-296">此用户权限确定哪些用户帐户可以修改对象的完整性标签，例如，文件、注册表项或其他用户所拥有的进程。</span><span class="sxs-lookup"><span data-stu-id="801ab-296">This user right determines which user accounts can modify the integrity label of objects, such as files, registry keys, or processes owned by other users.</span></span> <span data-ttu-id="801ab-297">仅支持 NotConfigured 和允许的状态。</span><span class="sxs-lookup"><span data-stu-id="801ab-297">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="801ab-298">userRightsProfileSingleProcess</span><span class="sxs-lookup"><span data-stu-id="801ab-298">userRightsProfileSingleProcess</span></span>|[<span data-ttu-id="801ab-299">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="801ab-299">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="801ab-300">此用户权限确定哪些用户可以使用性能监视工具来监视系统进程的性能。</span><span class="sxs-lookup"><span data-stu-id="801ab-300">This user right determines which users can use performance monitoring tools to monitor the performance of system processes.</span></span> <span data-ttu-id="801ab-301">仅支持 NotConfigured 和允许的状态。</span><span class="sxs-lookup"><span data-stu-id="801ab-301">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="801ab-302">userRightsRemoteShutdown</span><span class="sxs-lookup"><span data-stu-id="801ab-302">userRightsRemoteShutdown</span></span>|[<span data-ttu-id="801ab-303">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="801ab-303">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="801ab-304">此用户权限确定允许哪些用户从网络上的远程位置关闭计算机。</span><span class="sxs-lookup"><span data-stu-id="801ab-304">This user right determines which users are allowed to shut down a computer from a remote location on the network.</span></span> <span data-ttu-id="801ab-305">误用此用户权限可能会导致拒绝服务。</span><span class="sxs-lookup"><span data-stu-id="801ab-305">Misuse of this user right can result in a denial of service.</span></span> <span data-ttu-id="801ab-306">仅支持 NotConfigured 和允许的状态。</span><span class="sxs-lookup"><span data-stu-id="801ab-306">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="801ab-307">userRightsRestoreData</span><span class="sxs-lookup"><span data-stu-id="801ab-307">userRightsRestoreData</span></span>|[<span data-ttu-id="801ab-308">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="801ab-308">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="801ab-309">此用户权限确定在还原备份的文件和目录时，哪些用户可以绕过文件、目录、注册表和其他持久对象权限，并确定哪些用户可以将任何有效的安全主体设置为对象的所有者。</span><span class="sxs-lookup"><span data-stu-id="801ab-309">This user right determines which users can bypass file, directory, registry, and other persistent objects permissions when restoring backed up files and directories, and determines which users can set any valid security principal as the owner of an object.</span></span> <span data-ttu-id="801ab-310">仅支持 NotConfigured 和允许的状态。</span><span class="sxs-lookup"><span data-stu-id="801ab-310">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="801ab-311">userRightsTakeOwnership</span><span class="sxs-lookup"><span data-stu-id="801ab-311">userRightsTakeOwnership</span></span>|[<span data-ttu-id="801ab-312">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="801ab-312">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="801ab-313">此用户权限确定哪些用户可以获得系统中任何安全对象的所有权，包括 Active Directory 对象、文件和文件夹、打印机、注册表项、进程和线程。</span><span class="sxs-lookup"><span data-stu-id="801ab-313">This user right determines which users can take ownership of any securable object in the system, including Active Directory objects, files and folders, printers, registry keys, processes, and threads.</span></span> <span data-ttu-id="801ab-314">仅支持 NotConfigured 和允许的状态。</span><span class="sxs-lookup"><span data-stu-id="801ab-314">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="801ab-315">xboxServicesEnableXboxGameSaveTask</span><span class="sxs-lookup"><span data-stu-id="801ab-315">xboxServicesEnableXboxGameSaveTask</span></span>|<span data-ttu-id="801ab-316">Boolean</span><span class="sxs-lookup"><span data-stu-id="801ab-316">Boolean</span></span>|<span data-ttu-id="801ab-317">此设置确定是否启用了 xbox 游戏保存（1）或禁用（0）。</span><span class="sxs-lookup"><span data-stu-id="801ab-317">This setting determines whether xbox game save is enabled (1) or disabled (0).</span></span>|
|<span data-ttu-id="801ab-318">xboxServicesAccessoryManagementServiceStartupMode</span><span class="sxs-lookup"><span data-stu-id="801ab-318">xboxServicesAccessoryManagementServiceStartupMode</span></span>|[<span data-ttu-id="801ab-319">serviceStartType</span><span class="sxs-lookup"><span data-stu-id="801ab-319">serviceStartType</span></span>](../resources/intune-deviceconfig-servicestarttype.md)|<span data-ttu-id="801ab-320">此设置确定附件管理服务的启动类型是 "自动" （2）、"手动" （3）、"已禁用" （4）。</span><span class="sxs-lookup"><span data-stu-id="801ab-320">This setting determines whether the Accessory management service's start type is Automatic(2), Manual(3), Disabled(4).</span></span> <span data-ttu-id="801ab-321">默认：手动。</span><span class="sxs-lookup"><span data-stu-id="801ab-321">Default: Manual.</span></span> <span data-ttu-id="801ab-322">可取值为：`manual`、`automatic`、`disabled`。</span><span class="sxs-lookup"><span data-stu-id="801ab-322">Possible values are: `manual`, `automatic`, `disabled`.</span></span>|
|<span data-ttu-id="801ab-323">xboxServicesLiveAuthManagerServiceStartupMode</span><span class="sxs-lookup"><span data-stu-id="801ab-323">xboxServicesLiveAuthManagerServiceStartupMode</span></span>|[<span data-ttu-id="801ab-324">serviceStartType</span><span class="sxs-lookup"><span data-stu-id="801ab-324">serviceStartType</span></span>](../resources/intune-deviceconfig-servicestarttype.md)|<span data-ttu-id="801ab-325">此设置确定 Live Auth Manager 服务的启动类型是否为自动（2）、手动（3）、已禁用（4）。</span><span class="sxs-lookup"><span data-stu-id="801ab-325">This setting determines whether Live Auth Manager service's start type is Automatic(2), Manual(3), Disabled(4).</span></span> <span data-ttu-id="801ab-326">默认：手动。</span><span class="sxs-lookup"><span data-stu-id="801ab-326">Default: Manual.</span></span> <span data-ttu-id="801ab-327">可取值为：`manual`、`automatic`、`disabled`。</span><span class="sxs-lookup"><span data-stu-id="801ab-327">Possible values are: `manual`, `automatic`, `disabled`.</span></span>|
|<span data-ttu-id="801ab-328">xboxServicesLiveGameSaveServiceStartupMode</span><span class="sxs-lookup"><span data-stu-id="801ab-328">xboxServicesLiveGameSaveServiceStartupMode</span></span>|[<span data-ttu-id="801ab-329">serviceStartType</span><span class="sxs-lookup"><span data-stu-id="801ab-329">serviceStartType</span></span>](../resources/intune-deviceconfig-servicestarttype.md)|<span data-ttu-id="801ab-330">此设置确定实时游戏是否保存服务的启动类型为自动（2）、手动（3）、已禁用（4）。</span><span class="sxs-lookup"><span data-stu-id="801ab-330">This setting determines whether Live Game save service's start type is Automatic(2), Manual(3), Disabled(4).</span></span> <span data-ttu-id="801ab-331">默认：手动。</span><span class="sxs-lookup"><span data-stu-id="801ab-331">Default: Manual.</span></span> <span data-ttu-id="801ab-332">可取值为：`manual`、`automatic`、`disabled`。</span><span class="sxs-lookup"><span data-stu-id="801ab-332">Possible values are: `manual`, `automatic`, `disabled`.</span></span>|
|<span data-ttu-id="801ab-333">xboxServicesLiveNetworkingServiceStartupMode</span><span class="sxs-lookup"><span data-stu-id="801ab-333">xboxServicesLiveNetworkingServiceStartupMode</span></span>|[<span data-ttu-id="801ab-334">serviceStartType</span><span class="sxs-lookup"><span data-stu-id="801ab-334">serviceStartType</span></span>](../resources/intune-deviceconfig-servicestarttype.md)|<span data-ttu-id="801ab-335">此设置确定网络服务的启动类型是否为自动（2）、手动（3）、已禁用（4）。</span><span class="sxs-lookup"><span data-stu-id="801ab-335">This setting determines whether Networking service's start type is Automatic(2), Manual(3), Disabled(4).</span></span> <span data-ttu-id="801ab-336">默认：手动。</span><span class="sxs-lookup"><span data-stu-id="801ab-336">Default: Manual.</span></span> <span data-ttu-id="801ab-337">可取值为：`manual`、`automatic`、`disabled`。</span><span class="sxs-lookup"><span data-stu-id="801ab-337">Possible values are: `manual`, `automatic`, `disabled`.</span></span>|
|<span data-ttu-id="801ab-338">localSecurityOptionsBlockMicrosoftAccounts</span><span class="sxs-lookup"><span data-stu-id="801ab-338">localSecurityOptionsBlockMicrosoftAccounts</span></span>|<span data-ttu-id="801ab-339">Boolean</span><span class="sxs-lookup"><span data-stu-id="801ab-339">Boolean</span></span>|<span data-ttu-id="801ab-340">阻止用户向此计算机添加新的 Microsoft 帐户。</span><span class="sxs-lookup"><span data-stu-id="801ab-340">Prevent users from adding new Microsoft accounts to this computer.</span></span>|
|<span data-ttu-id="801ab-341">localSecurityOptionsBlockRemoteLogonWithBlankPassword</span><span class="sxs-lookup"><span data-stu-id="801ab-341">localSecurityOptionsBlockRemoteLogonWithBlankPassword</span></span>|<span data-ttu-id="801ab-342">Boolean</span><span class="sxs-lookup"><span data-stu-id="801ab-342">Boolean</span></span>|<span data-ttu-id="801ab-343">启用不受密码保护的本地帐户从物理设备以外的位置进行登录。默认值为已启用</span><span class="sxs-lookup"><span data-stu-id="801ab-343">Enable Local accounts that are not password protected to log on from locations other than the physical device.Default is enabled</span></span>|
|<span data-ttu-id="801ab-344">localSecurityOptionsDisableAdministratorAccount</span><span class="sxs-lookup"><span data-stu-id="801ab-344">localSecurityOptionsDisableAdministratorAccount</span></span>|<span data-ttu-id="801ab-345">Boolean</span><span class="sxs-lookup"><span data-stu-id="801ab-345">Boolean</span></span>|<span data-ttu-id="801ab-346">确定是否启用或禁用本地管理员帐户。</span><span class="sxs-lookup"><span data-stu-id="801ab-346">Determines whether the Local Administrator account is enabled or disabled.</span></span>|
|<span data-ttu-id="801ab-347">localSecurityOptionsAdministratorAccountName</span><span class="sxs-lookup"><span data-stu-id="801ab-347">localSecurityOptionsAdministratorAccountName</span></span>|<span data-ttu-id="801ab-348">String</span><span class="sxs-lookup"><span data-stu-id="801ab-348">String</span></span>|<span data-ttu-id="801ab-349">定义要与帐户 "管理员" 的安全标识符（SID）相关联的不同帐户名称。</span><span class="sxs-lookup"><span data-stu-id="801ab-349">Define a different account name to be associated with the security identifier (SID) for the account “Administrator”.</span></span>|
|<span data-ttu-id="801ab-350">localSecurityOptionsDisableGuestAccount</span><span class="sxs-lookup"><span data-stu-id="801ab-350">localSecurityOptionsDisableGuestAccount</span></span>|<span data-ttu-id="801ab-351">Boolean</span><span class="sxs-lookup"><span data-stu-id="801ab-351">Boolean</span></span>|<span data-ttu-id="801ab-352">确定来宾帐户是否已启用或已禁用。</span><span class="sxs-lookup"><span data-stu-id="801ab-352">Determines if the Guest account is enabled or disabled.</span></span>|
|<span data-ttu-id="801ab-353">localSecurityOptionsGuestAccountName</span><span class="sxs-lookup"><span data-stu-id="801ab-353">localSecurityOptionsGuestAccountName</span></span>|<span data-ttu-id="801ab-354">String</span><span class="sxs-lookup"><span data-stu-id="801ab-354">String</span></span>|<span data-ttu-id="801ab-355">定义要与帐户 "来宾" 的安全标识符（SID）相关联的不同帐户名称。</span><span class="sxs-lookup"><span data-stu-id="801ab-355">Define a different account name to be associated with the security identifier (SID) for the account “Guest”.</span></span>|
|<span data-ttu-id="801ab-356">localSecurityOptionsAllowUndockWithoutHavingToLogon</span><span class="sxs-lookup"><span data-stu-id="801ab-356">localSecurityOptionsAllowUndockWithoutHavingToLogon</span></span>|<span data-ttu-id="801ab-357">Boolean</span><span class="sxs-lookup"><span data-stu-id="801ab-357">Boolean</span></span>|<span data-ttu-id="801ab-358">阻止便携式计算机在无需登录的情况下被移除。</span><span class="sxs-lookup"><span data-stu-id="801ab-358">Prevent a portable computer from being undocked without having to log in.</span></span>|
|<span data-ttu-id="801ab-359">localSecurityOptionsBlockUsersInstallingPrinterDrivers</span><span class="sxs-lookup"><span data-stu-id="801ab-359">localSecurityOptionsBlockUsersInstallingPrinterDrivers</span></span>|<span data-ttu-id="801ab-360">Boolean</span><span class="sxs-lookup"><span data-stu-id="801ab-360">Boolean</span></span>|<span data-ttu-id="801ab-361">仅在将打印机驱动程序连接到共享打印机时，才将其限制为仅供管理员安装。</span><span class="sxs-lookup"><span data-stu-id="801ab-361">Restrict installing printer drivers as part of connecting to a shared printer to admins only.</span></span>|
|<span data-ttu-id="801ab-362">localSecurityOptionsBlockRemoteOpticalDriveAccess</span><span class="sxs-lookup"><span data-stu-id="801ab-362">localSecurityOptionsBlockRemoteOpticalDriveAccess</span></span>|<span data-ttu-id="801ab-363">Boolean</span><span class="sxs-lookup"><span data-stu-id="801ab-363">Boolean</span></span>|<span data-ttu-id="801ab-364">如果启用此设置，则仅允许交互式登录用户访问 CD-ROM 媒体。</span><span class="sxs-lookup"><span data-stu-id="801ab-364">Enabling this settings allows only interactively logged on user to access CD-ROM media.</span></span>|
|<span data-ttu-id="801ab-365">localSecurityOptionsFormatAndEjectOfRemovableMediaAllowedUser</span><span class="sxs-lookup"><span data-stu-id="801ab-365">localSecurityOptionsFormatAndEjectOfRemovableMediaAllowedUser</span></span>|[<span data-ttu-id="801ab-366">localSecurityOptionsFormatAndEjectOfRemovableMediaAllowedUserType</span><span class="sxs-lookup"><span data-stu-id="801ab-366">localSecurityOptionsFormatAndEjectOfRemovableMediaAllowedUserType</span></span>](../resources/intune-deviceconfig-localsecurityoptionsformatandejectofremovablemediaallowedusertype.md)|<span data-ttu-id="801ab-367">定义允许格式化和弹出可移动 NTFS 媒体的权限。</span><span class="sxs-lookup"><span data-stu-id="801ab-367">Define who is allowed to format and eject removable NTFS media.</span></span> <span data-ttu-id="801ab-368">可取值为：`notConfigured`、`administrators`、`administratorsAndPowerUsers`、`administratorsAndInteractiveUsers`。</span><span class="sxs-lookup"><span data-stu-id="801ab-368">Possible values are: `notConfigured`, `administrators`, `administratorsAndPowerUsers`, `administratorsAndInteractiveUsers`.</span></span>|
|<span data-ttu-id="801ab-369">localSecurityOptionsMachineInactivityLimit</span><span class="sxs-lookup"><span data-stu-id="801ab-369">localSecurityOptionsMachineInactivityLimit</span></span>|<span data-ttu-id="801ab-370">Int32</span><span class="sxs-lookup"><span data-stu-id="801ab-370">Int32</span></span>|<span data-ttu-id="801ab-371">在屏幕保护程序运行之前，定义交互式桌面登录屏幕上不活动的最长分钟数。</span><span class="sxs-lookup"><span data-stu-id="801ab-371">Define maximum minutes of inactivity on the interactive desktop’s login screen until the screen saver runs.</span></span> <span data-ttu-id="801ab-372">有效值为0至9999</span><span class="sxs-lookup"><span data-stu-id="801ab-372">Valid values 0 to 9999</span></span>|
|<span data-ttu-id="801ab-373">localSecurityOptionsMachineInactivityLimitInMinutes</span><span class="sxs-lookup"><span data-stu-id="801ab-373">localSecurityOptionsMachineInactivityLimitInMinutes</span></span>|<span data-ttu-id="801ab-374">Int32</span><span class="sxs-lookup"><span data-stu-id="801ab-374">Int32</span></span>|<span data-ttu-id="801ab-375">在屏幕保护程序运行之前，定义交互式桌面登录屏幕上不活动的最长分钟数。</span><span class="sxs-lookup"><span data-stu-id="801ab-375">Define maximum minutes of inactivity on the interactive desktop’s login screen until the screen saver runs.</span></span> <span data-ttu-id="801ab-376">有效值为0至9999</span><span class="sxs-lookup"><span data-stu-id="801ab-376">Valid values 0 to 9999</span></span>|
|<span data-ttu-id="801ab-377">localSecurityOptionsDoNotRequireCtrlAltDel</span><span class="sxs-lookup"><span data-stu-id="801ab-377">localSecurityOptionsDoNotRequireCtrlAltDel</span></span>|<span data-ttu-id="801ab-378">Boolean</span><span class="sxs-lookup"><span data-stu-id="801ab-378">Boolean</span></span>|<span data-ttu-id="801ab-379">要求用户在登录前按 CTRL + ALT + DEL。</span><span class="sxs-lookup"><span data-stu-id="801ab-379">Require CTRL+ALT+DEL to be pressed before a user can log on.</span></span>|
|<span data-ttu-id="801ab-380">localSecurityOptionsHideLastSignedInUser</span><span class="sxs-lookup"><span data-stu-id="801ab-380">localSecurityOptionsHideLastSignedInUser</span></span>|<span data-ttu-id="801ab-381">Boolean</span><span class="sxs-lookup"><span data-stu-id="801ab-381">Boolean</span></span>|<span data-ttu-id="801ab-382">不显示上次在此设备上登录的用户的用户名。</span><span class="sxs-lookup"><span data-stu-id="801ab-382">Do not display the username of the last person who signed in on this device.</span></span>|
|<span data-ttu-id="801ab-383">localSecurityOptionsHideUsernameAtSignIn</span><span class="sxs-lookup"><span data-stu-id="801ab-383">localSecurityOptionsHideUsernameAtSignIn</span></span>|<span data-ttu-id="801ab-384">Boolean</span><span class="sxs-lookup"><span data-stu-id="801ab-384">Boolean</span></span>|<span data-ttu-id="801ab-385">在输入凭据后以及显示设备桌面之前，请勿显示登录此设备的人员的用户名。</span><span class="sxs-lookup"><span data-stu-id="801ab-385">Do not display the username of the person signing in to this device after credentials are entered and before the device’s desktop is shown.</span></span>|
|<span data-ttu-id="801ab-386">localSecurityOptionsLogOnMessageTitle</span><span class="sxs-lookup"><span data-stu-id="801ab-386">localSecurityOptionsLogOnMessageTitle</span></span>|<span data-ttu-id="801ab-387">String</span><span class="sxs-lookup"><span data-stu-id="801ab-387">String</span></span>|<span data-ttu-id="801ab-388">为尝试登录的用户设置消息标题。</span><span class="sxs-lookup"><span data-stu-id="801ab-388">Set message title for users attempting to log in.</span></span>|
|<span data-ttu-id="801ab-389">localSecurityOptionsLogOnMessageText</span><span class="sxs-lookup"><span data-stu-id="801ab-389">localSecurityOptionsLogOnMessageText</span></span>|<span data-ttu-id="801ab-390">String</span><span class="sxs-lookup"><span data-stu-id="801ab-390">String</span></span>|<span data-ttu-id="801ab-391">为尝试登录的用户设置消息文本。</span><span class="sxs-lookup"><span data-stu-id="801ab-391">Set message text for users attempting to log in.</span></span>|
|<span data-ttu-id="801ab-392">localSecurityOptionsAllowPKU2UAuthenticationRequests</span><span class="sxs-lookup"><span data-stu-id="801ab-392">localSecurityOptionsAllowPKU2UAuthenticationRequests</span></span>|<span data-ttu-id="801ab-393">Boolean</span><span class="sxs-lookup"><span data-stu-id="801ab-393">Boolean</span></span>|<span data-ttu-id="801ab-394">阻止 PKU2U 对此设备的身份验证请求，以使用联机标识。</span><span class="sxs-lookup"><span data-stu-id="801ab-394">Block PKU2U authentication requests to this device to use online identities.</span></span>|
|<span data-ttu-id="801ab-395">localSecurityOptionsAllowRemoteCallsToSecurityAccountsManagerHelperBool</span><span class="sxs-lookup"><span data-stu-id="801ab-395">localSecurityOptionsAllowRemoteCallsToSecurityAccountsManagerHelperBool</span></span>|<span data-ttu-id="801ab-396">Boolean</span><span class="sxs-lookup"><span data-stu-id="801ab-396">Boolean</span></span>|<span data-ttu-id="801ab-397">LocalSecurityOptionsAllowRemoteCallsToSecurityAccountsManager 实体的 UI 帮助程序布尔值</span><span class="sxs-lookup"><span data-stu-id="801ab-397">UI helper boolean for LocalSecurityOptionsAllowRemoteCallsToSecurityAccountsManager entity</span></span>|
|<span data-ttu-id="801ab-398">localSecurityOptionsAllowRemoteCallsToSecurityAccountsManager</span><span class="sxs-lookup"><span data-stu-id="801ab-398">localSecurityOptionsAllowRemoteCallsToSecurityAccountsManager</span></span>|<span data-ttu-id="801ab-399">String</span><span class="sxs-lookup"><span data-stu-id="801ab-399">String</span></span>|<span data-ttu-id="801ab-400">编辑默认的安全描述符定义语言字符串，以允许或拒绝用户和组对 SAM 进行远程调用。</span><span class="sxs-lookup"><span data-stu-id="801ab-400">Edit the default Security Descriptor Definition Language string to allow or deny users and groups to make remote calls to the SAM.</span></span>|
|<span data-ttu-id="801ab-401">localSecurityOptionsMinimumSessionSecurityForNtlmSspBasedClients</span><span class="sxs-lookup"><span data-stu-id="801ab-401">localSecurityOptionsMinimumSessionSecurityForNtlmSspBasedClients</span></span>|[<span data-ttu-id="801ab-402">localSecurityOptionsMinimumSessionSecurity</span><span class="sxs-lookup"><span data-stu-id="801ab-402">localSecurityOptionsMinimumSessionSecurity</span></span>](../resources/intune-deviceconfig-localsecurityoptionsminimumsessionsecurity.md)|<span data-ttu-id="801ab-403">此安全设置允许客户端要求协商128位加密和/或 NTLMv2 会话安全性。</span><span class="sxs-lookup"><span data-stu-id="801ab-403">This security setting allows a client to require the negotiation of 128-bit encryption and/or NTLMv2 session security.</span></span> <span data-ttu-id="801ab-404">可取值为：`none`、`requireNtmlV2SessionSecurity`、`require128BitEncryption`、`ntlmV2And128BitEncryption`。</span><span class="sxs-lookup"><span data-stu-id="801ab-404">Possible values are: `none`, `requireNtmlV2SessionSecurity`, `require128BitEncryption`, `ntlmV2And128BitEncryption`.</span></span>|
|<span data-ttu-id="801ab-405">localSecurityOptionsMinimumSessionSecurityForNtlmSspBasedServers</span><span class="sxs-lookup"><span data-stu-id="801ab-405">localSecurityOptionsMinimumSessionSecurityForNtlmSspBasedServers</span></span>|[<span data-ttu-id="801ab-406">localSecurityOptionsMinimumSessionSecurity</span><span class="sxs-lookup"><span data-stu-id="801ab-406">localSecurityOptionsMinimumSessionSecurity</span></span>](../resources/intune-deviceconfig-localsecurityoptionsminimumsessionsecurity.md)|<span data-ttu-id="801ab-407">此安全设置允许服务器要求协商128位加密和/或 NTLMv2 会话安全性。</span><span class="sxs-lookup"><span data-stu-id="801ab-407">This security setting allows a server to require the negotiation of 128-bit encryption and/or NTLMv2 session security.</span></span> <span data-ttu-id="801ab-408">可取值为：`none`、`requireNtmlV2SessionSecurity`、`require128BitEncryption`、`ntlmV2And128BitEncryption`。</span><span class="sxs-lookup"><span data-stu-id="801ab-408">Possible values are: `none`, `requireNtmlV2SessionSecurity`, `require128BitEncryption`, `ntlmV2And128BitEncryption`.</span></span>|
|<span data-ttu-id="801ab-409">lanManagerAuthenticationLevel</span><span class="sxs-lookup"><span data-stu-id="801ab-409">lanManagerAuthenticationLevel</span></span>|[<span data-ttu-id="801ab-410">lanManagerAuthenticationLevel</span><span class="sxs-lookup"><span data-stu-id="801ab-410">lanManagerAuthenticationLevel</span></span>](../resources/intune-deviceconfig-lanmanagerauthenticationlevel.md)|<span data-ttu-id="801ab-411">此安全设置确定用于网络登录的质询/响应身份验证协议。</span><span class="sxs-lookup"><span data-stu-id="801ab-411">This security setting determines which challenge/response authentication protocol is used for network logons.</span></span> <span data-ttu-id="801ab-412">可取值为：`lmAndNltm`、`lmNtlmAndNtlmV2`、`lmAndNtlmOnly`、`lmAndNtlmV2`、`lmNtlmV2AndNotLm`、`lmNtlmV2AndNotLmOrNtm`。</span><span class="sxs-lookup"><span data-stu-id="801ab-412">Possible values are: `lmAndNltm`, `lmNtlmAndNtlmV2`, `lmAndNtlmOnly`, `lmAndNtlmV2`, `lmNtlmV2AndNotLm`, `lmNtlmV2AndNotLmOrNtm`.</span></span>|
|<span data-ttu-id="801ab-413">lanManagerWorkstationDisableInsecureGuestLogons</span><span class="sxs-lookup"><span data-stu-id="801ab-413">lanManagerWorkstationDisableInsecureGuestLogons</span></span>|<span data-ttu-id="801ab-414">Boolean</span><span class="sxs-lookup"><span data-stu-id="801ab-414">Boolean</span></span>|<span data-ttu-id="801ab-415">如果启用，SMB 客户端将允许不安全的来宾登录。</span><span class="sxs-lookup"><span data-stu-id="801ab-415">If enabled,the SMB client will allow insecure guest logons.</span></span> <span data-ttu-id="801ab-416">如果未配置，SMB 客户端将拒绝不安全的来宾登录。</span><span class="sxs-lookup"><span data-stu-id="801ab-416">If not configured, the SMB client will reject insecure guest logons.</span></span>|
|<span data-ttu-id="801ab-417">localSecurityOptionsClearVirtualMemoryPageFile</span><span class="sxs-lookup"><span data-stu-id="801ab-417">localSecurityOptionsClearVirtualMemoryPageFile</span></span>|<span data-ttu-id="801ab-418">Boolean</span><span class="sxs-lookup"><span data-stu-id="801ab-418">Boolean</span></span>|<span data-ttu-id="801ab-419">此安全设置确定在关闭系统时是否清除虚拟内存页面文件。</span><span class="sxs-lookup"><span data-stu-id="801ab-419">This security setting determines whether the virtual memory pagefile is cleared when the system is shut down.</span></span>|
|<span data-ttu-id="801ab-420">localSecurityOptionsAllowSystemToBeShutDownWithoutHavingToLogOn</span><span class="sxs-lookup"><span data-stu-id="801ab-420">localSecurityOptionsAllowSystemToBeShutDownWithoutHavingToLogOn</span></span>|<span data-ttu-id="801ab-421">Boolean</span><span class="sxs-lookup"><span data-stu-id="801ab-421">Boolean</span></span>|<span data-ttu-id="801ab-422">此安全设置确定是否可以在不登录 Windows 的情况下关闭计算机。</span><span class="sxs-lookup"><span data-stu-id="801ab-422">This security setting determines whether a computer can be shut down without having to log on to Windows.</span></span>|
|<span data-ttu-id="801ab-423">localSecurityOptionsAllowUIAccessApplicationElevation</span><span class="sxs-lookup"><span data-stu-id="801ab-423">localSecurityOptionsAllowUIAccessApplicationElevation</span></span>|<span data-ttu-id="801ab-424">Boolean</span><span class="sxs-lookup"><span data-stu-id="801ab-424">Boolean</span></span>|<span data-ttu-id="801ab-425">允许 UIAccess 应用在不使用安全桌面的情况下提示提升。</span><span class="sxs-lookup"><span data-stu-id="801ab-425">Allow UIAccess apps to prompt for elevation without using the secure desktop.</span></span>|
|<span data-ttu-id="801ab-426">localSecurityOptionsVirtualizeFileAndRegistryWriteFailuresToPerUserLocations</span><span class="sxs-lookup"><span data-stu-id="801ab-426">localSecurityOptionsVirtualizeFileAndRegistryWriteFailuresToPerUserLocations</span></span>|<span data-ttu-id="801ab-427">Boolean</span><span class="sxs-lookup"><span data-stu-id="801ab-427">Boolean</span></span>|<span data-ttu-id="801ab-428">将文件和注册表写入失败虚拟化到每个用户位置</span><span class="sxs-lookup"><span data-stu-id="801ab-428">Virtualize file and registry write failures to per user locations</span></span>|
|<span data-ttu-id="801ab-429">localSecurityOptionsOnlyElevateSignedExecutables</span><span class="sxs-lookup"><span data-stu-id="801ab-429">localSecurityOptionsOnlyElevateSignedExecutables</span></span>|<span data-ttu-id="801ab-430">Boolean</span><span class="sxs-lookup"><span data-stu-id="801ab-430">Boolean</span></span>|<span data-ttu-id="801ab-431">对给定的可执行文件强制执行 PKI 证书路径验证，然后再允许运行该文件。</span><span class="sxs-lookup"><span data-stu-id="801ab-431">Enforce PKI certification path validation for a given executable file before it is permitted to run.</span></span>|
|<span data-ttu-id="801ab-432">localSecurityOptionsAdministratorElevationPromptBehavior</span><span class="sxs-lookup"><span data-stu-id="801ab-432">localSecurityOptionsAdministratorElevationPromptBehavior</span></span>|[<span data-ttu-id="801ab-433">localSecurityOptionsAdministratorElevationPromptBehaviorType</span><span class="sxs-lookup"><span data-stu-id="801ab-433">localSecurityOptionsAdministratorElevationPromptBehaviorType</span></span>](../resources/intune-deviceconfig-localsecurityoptionsadministratorelevationpromptbehaviortype.md)|<span data-ttu-id="801ab-434">在管理员审批模式中定义管理员的提升提示行为。</span><span class="sxs-lookup"><span data-stu-id="801ab-434">Define the behavior of the elevation prompt for admins in Admin Approval Mode.</span></span> <span data-ttu-id="801ab-435">可取值为：`notConfigured`、`elevateWithoutPrompting`、`promptForCredentialsOnTheSecureDesktop`、`promptForConsentOnTheSecureDesktop`、`promptForCredentials`、`promptForConsent` 或 `promptForConsentForNonWindowsBinaries`。</span><span class="sxs-lookup"><span data-stu-id="801ab-435">Possible values are: `notConfigured`, `elevateWithoutPrompting`, `promptForCredentialsOnTheSecureDesktop`, `promptForConsentOnTheSecureDesktop`, `promptForCredentials`, `promptForConsent`, `promptForConsentForNonWindowsBinaries`.</span></span>|
|<span data-ttu-id="801ab-436">localSecurityOptionsStandardUserElevationPromptBehavior</span><span class="sxs-lookup"><span data-stu-id="801ab-436">localSecurityOptionsStandardUserElevationPromptBehavior</span></span>|[<span data-ttu-id="801ab-437">localSecurityOptionsStandardUserElevationPromptBehaviorType</span><span class="sxs-lookup"><span data-stu-id="801ab-437">localSecurityOptionsStandardUserElevationPromptBehaviorType</span></span>](../resources/intune-deviceconfig-localsecurityoptionsstandarduserelevationpromptbehaviortype.md)|<span data-ttu-id="801ab-438">定义标准用户的提升提示行为。</span><span class="sxs-lookup"><span data-stu-id="801ab-438">Define the behavior of the elevation prompt for standard users.</span></span> <span data-ttu-id="801ab-439">可取值为：`notConfigured`、`automaticallyDenyElevationRequests`、`promptForCredentialsOnTheSecureDesktop`、`promptForCredentials`。</span><span class="sxs-lookup"><span data-stu-id="801ab-439">Possible values are: `notConfigured`, `automaticallyDenyElevationRequests`, `promptForCredentialsOnTheSecureDesktop`, `promptForCredentials`.</span></span>|
|<span data-ttu-id="801ab-440">localSecurityOptionsSwitchToSecureDesktopWhenPromptingForElevation</span><span class="sxs-lookup"><span data-stu-id="801ab-440">localSecurityOptionsSwitchToSecureDesktopWhenPromptingForElevation</span></span>|<span data-ttu-id="801ab-441">Boolean</span><span class="sxs-lookup"><span data-stu-id="801ab-441">Boolean</span></span>|<span data-ttu-id="801ab-442">启用所有提升请求以转到交互式用户的桌面，而不是安全桌面。</span><span class="sxs-lookup"><span data-stu-id="801ab-442">Enable all elevation requests to go to the interactive user's desktop rather than the secure desktop.</span></span> <span data-ttu-id="801ab-443">使用管理员和标准用户的提示行为策略设置。</span><span class="sxs-lookup"><span data-stu-id="801ab-443">Prompt behavior policy settings for admins and standard users are used.</span></span>|
|<span data-ttu-id="801ab-444">localSecurityOptionsDetectApplicationInstallationsAndPromptForElevation</span><span class="sxs-lookup"><span data-stu-id="801ab-444">localSecurityOptionsDetectApplicationInstallationsAndPromptForElevation</span></span>|<span data-ttu-id="801ab-445">Boolean</span><span class="sxs-lookup"><span data-stu-id="801ab-445">Boolean</span></span>|<span data-ttu-id="801ab-446">需要提升权限的应用程序安装将提示管理凭据。默认值为已启用</span><span class="sxs-lookup"><span data-stu-id="801ab-446">App installations requiring elevated privileges will prompt for admin credentials.Default is enabled</span></span>|
|<span data-ttu-id="801ab-447">localSecurityOptionsAllowUIAccessApplicationsForSecureLocations</span><span class="sxs-lookup"><span data-stu-id="801ab-447">localSecurityOptionsAllowUIAccessApplicationsForSecureLocations</span></span>|<span data-ttu-id="801ab-448">Boolean</span><span class="sxs-lookup"><span data-stu-id="801ab-448">Boolean</span></span>|<span data-ttu-id="801ab-449">允许 UIAccess 应用在不使用安全桌面的情况下提示提升。默认值为已启用</span><span class="sxs-lookup"><span data-stu-id="801ab-449">Allow UIAccess apps to prompt for elevation without using the secure desktop.Default is enabled</span></span>|
|<span data-ttu-id="801ab-450">localSecurityOptionsUseAdminApprovalMode</span><span class="sxs-lookup"><span data-stu-id="801ab-450">localSecurityOptionsUseAdminApprovalMode</span></span>|<span data-ttu-id="801ab-451">Boolean</span><span class="sxs-lookup"><span data-stu-id="801ab-451">Boolean</span></span>|<span data-ttu-id="801ab-452">定义内置管理员帐户是使用管理员审批模式，还是运行所有具有完全管理员权限的应用程序。默认值为已启用</span><span class="sxs-lookup"><span data-stu-id="801ab-452">Defines whether the built-in admin account uses Admin Approval Mode or runs all apps with full admin privileges.Default is enabled</span></span>|
|<span data-ttu-id="801ab-453">localSecurityOptionsUseAdminApprovalModeForAdministrators</span><span class="sxs-lookup"><span data-stu-id="801ab-453">localSecurityOptionsUseAdminApprovalModeForAdministrators</span></span>|<span data-ttu-id="801ab-454">Boolean</span><span class="sxs-lookup"><span data-stu-id="801ab-454">Boolean</span></span>|<span data-ttu-id="801ab-455">定义是否启用管理员批准模式和所有 UAC 策略设置，默认为启用</span><span class="sxs-lookup"><span data-stu-id="801ab-455">Define whether Admin Approval Mode and all UAC policy settings are enabled, default is enabled</span></span>|
|<span data-ttu-id="801ab-456">localSecurityOptionsInformationShownOnLockScreen</span><span class="sxs-lookup"><span data-stu-id="801ab-456">localSecurityOptionsInformationShownOnLockScreen</span></span>|[<span data-ttu-id="801ab-457">localSecurityOptionsInformationShownOnLockScreenType</span><span class="sxs-lookup"><span data-stu-id="801ab-457">localSecurityOptionsInformationShownOnLockScreenType</span></span>](../resources/intune-deviceconfig-localsecurityoptionsinformationshownonlockscreentype.md)|<span data-ttu-id="801ab-458">配置在会话锁定时显示的用户信息。</span><span class="sxs-lookup"><span data-stu-id="801ab-458">Configure the user information that is displayed when the session is locked.</span></span> <span data-ttu-id="801ab-459">如果未配置，则显示用户显示名称、域和用户名。</span><span class="sxs-lookup"><span data-stu-id="801ab-459">If not configured, user display name, domain and username are shown.</span></span> <span data-ttu-id="801ab-460">可取值为：`notConfigured`、`userDisplayNameDomainUser`、`userDisplayNameOnly`、`doNotDisplayUser`。</span><span class="sxs-lookup"><span data-stu-id="801ab-460">Possible values are: `notConfigured`, `userDisplayNameDomainUser`, `userDisplayNameOnly`, `doNotDisplayUser`.</span></span>|
|<span data-ttu-id="801ab-461">localSecurityOptionsInformationDisplayedOnLockScreen</span><span class="sxs-lookup"><span data-stu-id="801ab-461">localSecurityOptionsInformationDisplayedOnLockScreen</span></span>|[<span data-ttu-id="801ab-462">localSecurityOptionsInformationDisplayedOnLockScreenType</span><span class="sxs-lookup"><span data-stu-id="801ab-462">localSecurityOptionsInformationDisplayedOnLockScreenType</span></span>](../resources/intune-deviceconfig-localsecurityoptionsinformationdisplayedonlockscreentype.md)|<span data-ttu-id="801ab-463">配置在会话锁定时显示的用户信息。</span><span class="sxs-lookup"><span data-stu-id="801ab-463">Configure the user information that is displayed when the session is locked.</span></span> <span data-ttu-id="801ab-464">如果未配置，则显示用户显示名称、域和用户名。</span><span class="sxs-lookup"><span data-stu-id="801ab-464">If not configured, user display name, domain and username are shown.</span></span> <span data-ttu-id="801ab-465">可取值为：`notConfigured`、`administrators`、`administratorsAndPowerUsers`、`administratorsAndInteractiveUsers`。</span><span class="sxs-lookup"><span data-stu-id="801ab-465">Possible values are: `notConfigured`, `administrators`, `administratorsAndPowerUsers`, `administratorsAndInteractiveUsers`.</span></span>|
|<span data-ttu-id="801ab-466">localSecurityOptionsDisableClientDigitallySignCommunicationsIfServerAgrees</span><span class="sxs-lookup"><span data-stu-id="801ab-466">localSecurityOptionsDisableClientDigitallySignCommunicationsIfServerAgrees</span></span>|<span data-ttu-id="801ab-467">Boolean</span><span class="sxs-lookup"><span data-stu-id="801ab-467">Boolean</span></span>|<span data-ttu-id="801ab-468">此安全设置确定 SMB 客户端是否尝试协商 SMB 数据包签名。</span><span class="sxs-lookup"><span data-stu-id="801ab-468">This security setting determines whether the SMB client attempts to negotiate SMB packet signing.</span></span>|
|<span data-ttu-id="801ab-469">localSecurityOptionsClientDigitallySignCommunicationsAlways</span><span class="sxs-lookup"><span data-stu-id="801ab-469">localSecurityOptionsClientDigitallySignCommunicationsAlways</span></span>|<span data-ttu-id="801ab-470">Boolean</span><span class="sxs-lookup"><span data-stu-id="801ab-470">Boolean</span></span>|<span data-ttu-id="801ab-471">此安全设置确定 SMB 客户端组件是否需要数据包签名。</span><span class="sxs-lookup"><span data-stu-id="801ab-471">This security setting determines whether packet signing is required by the SMB client component.</span></span>|
|<span data-ttu-id="801ab-472">localSecurityOptionsClientSendUnencryptedPasswordToThirdPartySMBServers</span><span class="sxs-lookup"><span data-stu-id="801ab-472">localSecurityOptionsClientSendUnencryptedPasswordToThirdPartySMBServers</span></span>|<span data-ttu-id="801ab-473">Boolean</span><span class="sxs-lookup"><span data-stu-id="801ab-473">Boolean</span></span>|<span data-ttu-id="801ab-474">如果启用此安全设置，则允许服务器消息块（SMB）重定向程序将纯文本密码发送到在身份验证过程中不支持密码加密的非 Microsoft SMB 服务器。</span><span class="sxs-lookup"><span data-stu-id="801ab-474">If this security setting is enabled, the Server Message Block (SMB) redirector is allowed to send plaintext passwords to non-Microsoft SMB servers that do not support password encryption during authentication.</span></span>|
|<span data-ttu-id="801ab-475">localSecurityOptionsDisableServerDigitallySignCommunicationsAlways</span><span class="sxs-lookup"><span data-stu-id="801ab-475">localSecurityOptionsDisableServerDigitallySignCommunicationsAlways</span></span>|<span data-ttu-id="801ab-476">Boolean</span><span class="sxs-lookup"><span data-stu-id="801ab-476">Boolean</span></span>|<span data-ttu-id="801ab-477">此安全设置确定 SMB 服务器组件是否需要数据包签名。</span><span class="sxs-lookup"><span data-stu-id="801ab-477">This security setting determines whether packet signing is required by the SMB server component.</span></span>|
|<span data-ttu-id="801ab-478">localSecurityOptionsDisableServerDigitallySignCommunicationsIfClientAgrees</span><span class="sxs-lookup"><span data-stu-id="801ab-478">localSecurityOptionsDisableServerDigitallySignCommunicationsIfClientAgrees</span></span>|<span data-ttu-id="801ab-479">Boolean</span><span class="sxs-lookup"><span data-stu-id="801ab-479">Boolean</span></span>|<span data-ttu-id="801ab-480">此安全设置确定 SMB 服务器是否将 SMB 数据包签名与请求的客户端协商。</span><span class="sxs-lookup"><span data-stu-id="801ab-480">This security setting determines whether the SMB server will negotiate SMB packet signing with clients that request it.</span></span>|
|<span data-ttu-id="801ab-481">localSecurityOptionsRestrictAnonymousAccessToNamedPipesAndShares</span><span class="sxs-lookup"><span data-stu-id="801ab-481">localSecurityOptionsRestrictAnonymousAccessToNamedPipesAndShares</span></span>|<span data-ttu-id="801ab-482">Boolean</span><span class="sxs-lookup"><span data-stu-id="801ab-482">Boolean</span></span>|<span data-ttu-id="801ab-483">默认情况下，此安全设置限制可匿名访问且可匿名访问的共享的命名管道设置对共享和管道的匿名访问权限</span><span class="sxs-lookup"><span data-stu-id="801ab-483">By default, this security setting restricts anonymous access to shares and pipes to the settings for named pipes that can be accessed anonymously and Shares that can be accessed anonymously</span></span>|
|<span data-ttu-id="801ab-484">localSecurityOptionsDoNotAllowAnonymousEnumerationOfSAMAccounts</span><span class="sxs-lookup"><span data-stu-id="801ab-484">localSecurityOptionsDoNotAllowAnonymousEnumerationOfSAMAccounts</span></span>|<span data-ttu-id="801ab-485">Boolean</span><span class="sxs-lookup"><span data-stu-id="801ab-485">Boolean</span></span>|<span data-ttu-id="801ab-486">此安全设置确定将向计算机的匿名连接授予的其他权限。</span><span class="sxs-lookup"><span data-stu-id="801ab-486">This security setting determines what additional permissions will be granted for anonymous connections to the computer.</span></span>|
|<span data-ttu-id="801ab-487">localSecurityOptionsAllowAnonymousEnumerationOfSAMAccountsAndShares</span><span class="sxs-lookup"><span data-stu-id="801ab-487">localSecurityOptionsAllowAnonymousEnumerationOfSAMAccountsAndShares</span></span>|<span data-ttu-id="801ab-488">Boolean</span><span class="sxs-lookup"><span data-stu-id="801ab-488">Boolean</span></span>|<span data-ttu-id="801ab-489">此安全设置确定是否允许匿名用户执行某些活动，如枚举域帐户和网络共享的名称。</span><span class="sxs-lookup"><span data-stu-id="801ab-489">This security setting determines whether to allows anonymous users to perform certain activities, such as enumerating the names of domain accounts and network shares.</span></span>|
|<span data-ttu-id="801ab-490">localSecurityOptionsDoNotStoreLANManagerHashValueOnNextPasswordChange</span><span class="sxs-lookup"><span data-stu-id="801ab-490">localSecurityOptionsDoNotStoreLANManagerHashValueOnNextPasswordChange</span></span>|<span data-ttu-id="801ab-491">Boolean</span><span class="sxs-lookup"><span data-stu-id="801ab-491">Boolean</span></span>|<span data-ttu-id="801ab-492">此安全设置确定在下一次更改密码时，是否存储新密码的 LAN Manager （LM）哈希值。</span><span class="sxs-lookup"><span data-stu-id="801ab-492">This security setting determines if, at the next password change, the LAN Manager (LM) hash value for the new password is stored.</span></span> <span data-ttu-id="801ab-493">默认情况下不存储它。</span><span class="sxs-lookup"><span data-stu-id="801ab-493">It’s not stored by default.</span></span>|
|<span data-ttu-id="801ab-494">localSecurityOptionsSmartCardRemovalBehavior</span><span class="sxs-lookup"><span data-stu-id="801ab-494">localSecurityOptionsSmartCardRemovalBehavior</span></span>|[<span data-ttu-id="801ab-495">localSecurityOptionsSmartCardRemovalBehaviorType</span><span class="sxs-lookup"><span data-stu-id="801ab-495">localSecurityOptionsSmartCardRemovalBehaviorType</span></span>](../resources/intune-deviceconfig-localsecurityoptionssmartcardremovalbehaviortype.md)|<span data-ttu-id="801ab-496">此安全设置确定将已登录用户的智能卡从智能卡读卡器中删除时发生的情况。</span><span class="sxs-lookup"><span data-stu-id="801ab-496">This security setting determines what happens when the smart card for a logged-on user is removed from the smart card reader.</span></span> <span data-ttu-id="801ab-497">可取值为：`lockWorkstation`、`noAction`、`forceLogoff`、`disconnectRemoteDesktopSession`。</span><span class="sxs-lookup"><span data-stu-id="801ab-497">Possible values are: `lockWorkstation`, `noAction`, `forceLogoff`, `disconnectRemoteDesktopSession`.</span></span>|
|<span data-ttu-id="801ab-498">defenderSecurityCenterDisableAppBrowserUI</span><span class="sxs-lookup"><span data-stu-id="801ab-498">defenderSecurityCenterDisableAppBrowserUI</span></span>|<span data-ttu-id="801ab-499">Boolean</span><span class="sxs-lookup"><span data-stu-id="801ab-499">Boolean</span></span>|<span data-ttu-id="801ab-500">用于禁用应用程序和浏览器保护区域的显示。</span><span class="sxs-lookup"><span data-stu-id="801ab-500">Used to disable the display of the app and browser protection area.</span></span>|
|<span data-ttu-id="801ab-501">defenderSecurityCenterDisableFamilyUI</span><span class="sxs-lookup"><span data-stu-id="801ab-501">defenderSecurityCenterDisableFamilyUI</span></span>|<span data-ttu-id="801ab-502">Boolean</span><span class="sxs-lookup"><span data-stu-id="801ab-502">Boolean</span></span>|<span data-ttu-id="801ab-503">用于禁用 "家庭选项" 区域的显示。</span><span class="sxs-lookup"><span data-stu-id="801ab-503">Used to disable the display of the family options area.</span></span>|
|<span data-ttu-id="801ab-504">defenderSecurityCenterDisableHealthUI</span><span class="sxs-lookup"><span data-stu-id="801ab-504">defenderSecurityCenterDisableHealthUI</span></span>|<span data-ttu-id="801ab-505">Boolean</span><span class="sxs-lookup"><span data-stu-id="801ab-505">Boolean</span></span>|<span data-ttu-id="801ab-506">用于禁用设备性能和运行状况区域的显示。</span><span class="sxs-lookup"><span data-stu-id="801ab-506">Used to disable the display of the device performance and health area.</span></span>|
|<span data-ttu-id="801ab-507">defenderSecurityCenterDisableNetworkUI</span><span class="sxs-lookup"><span data-stu-id="801ab-507">defenderSecurityCenterDisableNetworkUI</span></span>|<span data-ttu-id="801ab-508">Boolean</span><span class="sxs-lookup"><span data-stu-id="801ab-508">Boolean</span></span>|<span data-ttu-id="801ab-509">用于禁用防火墙和网络防护区域的显示。</span><span class="sxs-lookup"><span data-stu-id="801ab-509">Used to disable the display of the firewall and network protection area.</span></span>|
|<span data-ttu-id="801ab-510">defenderSecurityCenterDisableVirusUI</span><span class="sxs-lookup"><span data-stu-id="801ab-510">defenderSecurityCenterDisableVirusUI</span></span>|<span data-ttu-id="801ab-511">Boolean</span><span class="sxs-lookup"><span data-stu-id="801ab-511">Boolean</span></span>|<span data-ttu-id="801ab-512">用于禁用病毒和威胁防护区域的显示。</span><span class="sxs-lookup"><span data-stu-id="801ab-512">Used to disable the display of the virus and threat protection area.</span></span>|
|<span data-ttu-id="801ab-513">defenderSecurityCenterDisableAccountUI</span><span class="sxs-lookup"><span data-stu-id="801ab-513">defenderSecurityCenterDisableAccountUI</span></span>|<span data-ttu-id="801ab-514">Boolean</span><span class="sxs-lookup"><span data-stu-id="801ab-514">Boolean</span></span>|<span data-ttu-id="801ab-515">用于禁用帐户保护区域的显示。</span><span class="sxs-lookup"><span data-stu-id="801ab-515">Used to disable the display of the account protection area.</span></span>|
|<span data-ttu-id="801ab-516">defenderSecurityCenterDisableClearTpmUI</span><span class="sxs-lookup"><span data-stu-id="801ab-516">defenderSecurityCenterDisableClearTpmUI</span></span>|<span data-ttu-id="801ab-517">Boolean</span><span class="sxs-lookup"><span data-stu-id="801ab-517">Boolean</span></span>|<span data-ttu-id="801ab-518">用于禁用 "清除 TPM" 按钮的显示。</span><span class="sxs-lookup"><span data-stu-id="801ab-518">Used to disable the display of the Clear TPM button.</span></span>|
|<span data-ttu-id="801ab-519">defenderSecurityCenterDisableHardwareUI</span><span class="sxs-lookup"><span data-stu-id="801ab-519">defenderSecurityCenterDisableHardwareUI</span></span>|<span data-ttu-id="801ab-520">Boolean</span><span class="sxs-lookup"><span data-stu-id="801ab-520">Boolean</span></span>|<span data-ttu-id="801ab-521">用于禁用硬件保护区域的显示。</span><span class="sxs-lookup"><span data-stu-id="801ab-521">Used to disable the display of the hardware protection area.</span></span>|
|<span data-ttu-id="801ab-522">defenderSecurityCenterDisableNotificationAreaUI</span><span class="sxs-lookup"><span data-stu-id="801ab-522">defenderSecurityCenterDisableNotificationAreaUI</span></span>|<span data-ttu-id="801ab-523">Boolean</span><span class="sxs-lookup"><span data-stu-id="801ab-523">Boolean</span></span>|<span data-ttu-id="801ab-524">用于禁用通知区域控件的显示。</span><span class="sxs-lookup"><span data-stu-id="801ab-524">Used to disable the display of the notification area control.</span></span> <span data-ttu-id="801ab-525">用户需要注销并登录或重新启动计算机，此设置才会生效。</span><span class="sxs-lookup"><span data-stu-id="801ab-525">The user needs to either sign out and sign in or reboot the computer for this setting to take effect.</span></span>|
|<span data-ttu-id="801ab-526">defenderSecurityCenterDisableRansomwareUI</span><span class="sxs-lookup"><span data-stu-id="801ab-526">defenderSecurityCenterDisableRansomwareUI</span></span>|<span data-ttu-id="801ab-527">Boolean</span><span class="sxs-lookup"><span data-stu-id="801ab-527">Boolean</span></span>|<span data-ttu-id="801ab-528">用于禁用勒索软件防护区域的显示。</span><span class="sxs-lookup"><span data-stu-id="801ab-528">Used to disable the display of the ransomware protection area.</span></span> |
|<span data-ttu-id="801ab-529">defenderSecurityCenterDisableSecureBootUI</span><span class="sxs-lookup"><span data-stu-id="801ab-529">defenderSecurityCenterDisableSecureBootUI</span></span>|<span data-ttu-id="801ab-530">Boolean</span><span class="sxs-lookup"><span data-stu-id="801ab-530">Boolean</span></span>|<span data-ttu-id="801ab-531">用于在 "设备安全性" 下禁用安全引导区域的显示。</span><span class="sxs-lookup"><span data-stu-id="801ab-531">Used to disable the display of the secure boot area under Device security.</span></span>|
|<span data-ttu-id="801ab-532">defenderSecurityCenterDisableTroubleshootingUI</span><span class="sxs-lookup"><span data-stu-id="801ab-532">defenderSecurityCenterDisableTroubleshootingUI</span></span>|<span data-ttu-id="801ab-533">Boolean</span><span class="sxs-lookup"><span data-stu-id="801ab-533">Boolean</span></span>|<span data-ttu-id="801ab-534">用于在 "设备安全性" 下禁用安全过程故障排除的显示。</span><span class="sxs-lookup"><span data-stu-id="801ab-534">Used to disable the display of the security process troubleshooting under Device security.</span></span>|
|<span data-ttu-id="801ab-535">defenderSecurityCenterDisableVulnerableTpmFirmwareUpdateUI</span><span class="sxs-lookup"><span data-stu-id="801ab-535">defenderSecurityCenterDisableVulnerableTpmFirmwareUpdateUI</span></span>|<span data-ttu-id="801ab-536">Boolean</span><span class="sxs-lookup"><span data-stu-id="801ab-536">Boolean</span></span>|<span data-ttu-id="801ab-537">用于在检测到易受攻击的固件时禁用显示更新 TPM 固件。</span><span class="sxs-lookup"><span data-stu-id="801ab-537">Used to disable the display of update TPM Firmware when a vulnerable firmware is detected.</span></span>|
|<span data-ttu-id="801ab-538">defenderSecurityCenterOrganizationDisplayName</span><span class="sxs-lookup"><span data-stu-id="801ab-538">defenderSecurityCenterOrganizationDisplayName</span></span>|<span data-ttu-id="801ab-539">String</span><span class="sxs-lookup"><span data-stu-id="801ab-539">String</span></span>|<span data-ttu-id="801ab-540">向用户显示的公司名称。</span><span class="sxs-lookup"><span data-stu-id="801ab-540">The company name that is displayed to the users.</span></span>|
|<span data-ttu-id="801ab-541">defenderSecurityCenterHelpEmail</span><span class="sxs-lookup"><span data-stu-id="801ab-541">defenderSecurityCenterHelpEmail</span></span>|<span data-ttu-id="801ab-542">String</span><span class="sxs-lookup"><span data-stu-id="801ab-542">String</span></span>|<span data-ttu-id="801ab-543">向用户显示的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="801ab-543">The email address that is displayed to users.</span></span>|
|<span data-ttu-id="801ab-544">defenderSecurityCenterHelpPhone</span><span class="sxs-lookup"><span data-stu-id="801ab-544">defenderSecurityCenterHelpPhone</span></span>|<span data-ttu-id="801ab-545">String</span><span class="sxs-lookup"><span data-stu-id="801ab-545">String</span></span>|<span data-ttu-id="801ab-546">向用户显示的电话号码或 Skype ID。</span><span class="sxs-lookup"><span data-stu-id="801ab-546">The phone number or Skype ID that is displayed to users.</span></span>|
|<span data-ttu-id="801ab-547">defenderSecurityCenterHelpURL</span><span class="sxs-lookup"><span data-stu-id="801ab-547">defenderSecurityCenterHelpURL</span></span>|<span data-ttu-id="801ab-548">String</span><span class="sxs-lookup"><span data-stu-id="801ab-548">String</span></span>|<span data-ttu-id="801ab-549">"帮助" 门户 URL 将向用户显示。</span><span class="sxs-lookup"><span data-stu-id="801ab-549">The help portal URL this is displayed to users.</span></span>|
|<span data-ttu-id="801ab-550">defenderSecurityCenterNotificationsFromApp</span><span class="sxs-lookup"><span data-stu-id="801ab-550">defenderSecurityCenterNotificationsFromApp</span></span>|[<span data-ttu-id="801ab-551">defenderSecurityCenterNotificationsFromAppType</span><span class="sxs-lookup"><span data-stu-id="801ab-551">defenderSecurityCenterNotificationsFromAppType</span></span>](../resources/intune-deviceconfig-defendersecuritycenternotificationsfromapptype.md)|<span data-ttu-id="801ab-552">要从应用程序的显示区域中显示的通知。</span><span class="sxs-lookup"><span data-stu-id="801ab-552">Notifications to show from the displayed areas of app.</span></span> <span data-ttu-id="801ab-553">可取值为：`notConfigured`、`blockNoncriticalNotifications`、`blockAllNotifications`。</span><span class="sxs-lookup"><span data-stu-id="801ab-553">Possible values are: `notConfigured`, `blockNoncriticalNotifications`, `blockAllNotifications`.</span></span>|
|<span data-ttu-id="801ab-554">defenderSecurityCenterITContactDisplay</span><span class="sxs-lookup"><span data-stu-id="801ab-554">defenderSecurityCenterITContactDisplay</span></span>|[<span data-ttu-id="801ab-555">defenderSecurityCenterITContactDisplayType</span><span class="sxs-lookup"><span data-stu-id="801ab-555">defenderSecurityCenterITContactDisplayType</span></span>](../resources/intune-deviceconfig-defendersecuritycenteritcontactdisplaytype.md)|<span data-ttu-id="801ab-556">配置向最终用户显示 IT 联系人信息的位置。</span><span class="sxs-lookup"><span data-stu-id="801ab-556">Configure where to display IT contact information to end users.</span></span> <span data-ttu-id="801ab-557">可取值为：`notConfigured`、`displayInAppAndInNotifications`、`displayOnlyInApp`、`displayOnlyInNotifications`。</span><span class="sxs-lookup"><span data-stu-id="801ab-557">Possible values are: `notConfigured`, `displayInAppAndInNotifications`, `displayOnlyInApp`, `displayOnlyInNotifications`.</span></span>|
|<span data-ttu-id="801ab-558">windowsDefenderTamperProtection</span><span class="sxs-lookup"><span data-stu-id="801ab-558">windowsDefenderTamperProtection</span></span>|[<span data-ttu-id="801ab-559">windowsDefenderTamperProtectionOptions</span><span class="sxs-lookup"><span data-stu-id="801ab-559">windowsDefenderTamperProtectionOptions</span></span>](../resources/intune-deviceconfig-windowsdefendertamperprotectionoptions.md)|<span data-ttu-id="801ab-560">配置 windows defender TamperProtection 设置。</span><span class="sxs-lookup"><span data-stu-id="801ab-560">Configure windows defender TamperProtection settings.</span></span> <span data-ttu-id="801ab-561">可取值为：`notConfigured`、`enable`、`disable`。</span><span class="sxs-lookup"><span data-stu-id="801ab-561">Possible values are: `notConfigured`, `enable`, `disable`.</span></span>|
|<span data-ttu-id="801ab-562">firewallBlockStatefulFTP</span><span class="sxs-lookup"><span data-stu-id="801ab-562">firewallBlockStatefulFTP</span></span>|<span data-ttu-id="801ab-563">Boolean</span><span class="sxs-lookup"><span data-stu-id="801ab-563">Boolean</span></span>|<span data-ttu-id="801ab-564">阻止到设备的有状态 FTP 连接</span><span class="sxs-lookup"><span data-stu-id="801ab-564">Blocks stateful FTP connections to the device</span></span>|
|<span data-ttu-id="801ab-565">firewallIdleTimeoutForSecurityAssociationInSeconds</span><span class="sxs-lookup"><span data-stu-id="801ab-565">firewallIdleTimeoutForSecurityAssociationInSeconds</span></span>|<span data-ttu-id="801ab-566">Int32</span><span class="sxs-lookup"><span data-stu-id="801ab-566">Int32</span></span>|<span data-ttu-id="801ab-567">配置安全关联的空闲超时（以秒为单位），值范围为 300 到 3600（包括这两个值）。</span><span class="sxs-lookup"><span data-stu-id="801ab-567">Configures the idle timeout for security associations, in seconds, from 300 to 3600 inclusive.</span></span> <span data-ttu-id="801ab-568">这是一个时间段，在此之后安全关联将过期并被删除。</span><span class="sxs-lookup"><span data-stu-id="801ab-568">This is the period after which security associations will expire and be deleted.</span></span> <span data-ttu-id="801ab-569">有效值为 300 至 3600</span><span class="sxs-lookup"><span data-stu-id="801ab-569">Valid values 300 to 3600</span></span>|
|<span data-ttu-id="801ab-570">firewallPreSharedKeyEncodingMethod</span><span class="sxs-lookup"><span data-stu-id="801ab-570">firewallPreSharedKeyEncodingMethod</span></span>|[<span data-ttu-id="801ab-571">firewallPreSharedKeyEncodingMethodType</span><span class="sxs-lookup"><span data-stu-id="801ab-571">firewallPreSharedKeyEncodingMethodType</span></span>](../resources/intune-deviceconfig-firewallpresharedkeyencodingmethodtype.md)|<span data-ttu-id="801ab-572">选择要使用的预共享密钥编码。</span><span class="sxs-lookup"><span data-stu-id="801ab-572">Select the preshared key encoding to be used.</span></span> <span data-ttu-id="801ab-573">可取值为：`deviceDefault`、`none`、`utF8`。</span><span class="sxs-lookup"><span data-stu-id="801ab-573">Possible values are: `deviceDefault`, `none`, `utF8`.</span></span>|
|<span data-ttu-id="801ab-574">firewallIPSecExemptionsAllowNeighborDiscovery</span><span class="sxs-lookup"><span data-stu-id="801ab-574">firewallIPSecExemptionsAllowNeighborDiscovery</span></span>|<span data-ttu-id="801ab-575">Boolean</span><span class="sxs-lookup"><span data-stu-id="801ab-575">Boolean</span></span>|<span data-ttu-id="801ab-576">配置 IPSec 免除项以允许邻居发现 IPv6 ICMP 类型代码</span><span class="sxs-lookup"><span data-stu-id="801ab-576">Configures IPSec exemptions to allow neighbor discovery IPv6 ICMP type-codes</span></span>|
|<span data-ttu-id="801ab-577">firewallIPSecExemptionsAllowICMP</span><span class="sxs-lookup"><span data-stu-id="801ab-577">firewallIPSecExemptionsAllowICMP</span></span>|<span data-ttu-id="801ab-578">Boolean</span><span class="sxs-lookup"><span data-stu-id="801ab-578">Boolean</span></span>|<span data-ttu-id="801ab-579">配置 IPSec 免除项以允许 ICMP</span><span class="sxs-lookup"><span data-stu-id="801ab-579">Configures IPSec exemptions to allow ICMP</span></span>|
|<span data-ttu-id="801ab-580">firewallIPSecExemptionsAllowRouterDiscovery</span><span class="sxs-lookup"><span data-stu-id="801ab-580">firewallIPSecExemptionsAllowRouterDiscovery</span></span>|<span data-ttu-id="801ab-581">Boolean</span><span class="sxs-lookup"><span data-stu-id="801ab-581">Boolean</span></span>|<span data-ttu-id="801ab-582">配置 IPSec 免除项以允许路由器发现 IPv6 ICMP 类型代码</span><span class="sxs-lookup"><span data-stu-id="801ab-582">Configures IPSec exemptions to allow router discovery IPv6 ICMP type-codes</span></span>|
|<span data-ttu-id="801ab-583">firewallIPSecExemptionsAllowDHCP</span><span class="sxs-lookup"><span data-stu-id="801ab-583">firewallIPSecExemptionsAllowDHCP</span></span>|<span data-ttu-id="801ab-584">Boolean</span><span class="sxs-lookup"><span data-stu-id="801ab-584">Boolean</span></span>|<span data-ttu-id="801ab-585">配置 IPSec 免除项以允许 IPv4 和 IPv6 DHCP 通信</span><span class="sxs-lookup"><span data-stu-id="801ab-585">Configures IPSec exemptions to allow both IPv4 and IPv6 DHCP traffic</span></span>|
|<span data-ttu-id="801ab-586">firewallCertificateRevocationListCheckMethod</span><span class="sxs-lookup"><span data-stu-id="801ab-586">firewallCertificateRevocationListCheckMethod</span></span>|[<span data-ttu-id="801ab-587">firewallCertificateRevocationListCheckMethodType</span><span class="sxs-lookup"><span data-stu-id="801ab-587">firewallCertificateRevocationListCheckMethodType</span></span>](../resources/intune-deviceconfig-firewallcertificaterevocationlistcheckmethodtype.md)|<span data-ttu-id="801ab-588">指定如何强制执行证书吊销列表。</span><span class="sxs-lookup"><span data-stu-id="801ab-588">Specify how the certificate revocation list is to be enforced.</span></span> <span data-ttu-id="801ab-589">可取值为：`deviceDefault`、`none`、`attempt`、`require`。</span><span class="sxs-lookup"><span data-stu-id="801ab-589">Possible values are: `deviceDefault`, `none`, `attempt`, `require`.</span></span>|
|<span data-ttu-id="801ab-590">firewallMergeKeyingModuleSettings</span><span class="sxs-lookup"><span data-stu-id="801ab-590">firewallMergeKeyingModuleSettings</span></span>|<span data-ttu-id="801ab-591">Boolean</span><span class="sxs-lookup"><span data-stu-id="801ab-591">Boolean</span></span>|<span data-ttu-id="801ab-592">如果键控模块不完全支持身份验证集，请指示模块仅忽略不受支持的身份验证套件而不是整个集</span><span class="sxs-lookup"><span data-stu-id="801ab-592">If an authentication set is not fully supported by a keying module, direct the module to ignore only unsupported authentication suites rather than the entire set</span></span>|
|<span data-ttu-id="801ab-593">firewallPacketQueueingMethod</span><span class="sxs-lookup"><span data-stu-id="801ab-593">firewallPacketQueueingMethod</span></span>|[<span data-ttu-id="801ab-594">firewallPacketQueueingMethodType</span><span class="sxs-lookup"><span data-stu-id="801ab-594">firewallPacketQueueingMethodType</span></span>](../resources/intune-deviceconfig-firewallpacketqueueingmethodtype.md)|<span data-ttu-id="801ab-595">配置如何在隧道网关应用场景中应用数据包排队。</span><span class="sxs-lookup"><span data-stu-id="801ab-595">Configures how packet queueing should be applied in the tunnel gateway scenario.</span></span> <span data-ttu-id="801ab-596">可取值为：`deviceDefault`、`disabled`、`queueInbound`、`queueOutbound`、`queueBoth`。</span><span class="sxs-lookup"><span data-stu-id="801ab-596">Possible values are: `deviceDefault`, `disabled`, `queueInbound`, `queueOutbound`, `queueBoth`.</span></span>|
|<span data-ttu-id="801ab-597">firewallProfileDomain</span><span class="sxs-lookup"><span data-stu-id="801ab-597">firewallProfileDomain</span></span>|[<span data-ttu-id="801ab-598">windowsFirewallNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="801ab-598">windowsFirewallNetworkProfile</span></span>](../resources/intune-deviceconfig-windowsfirewallnetworkprofile.md)|<span data-ttu-id="801ab-599">配置域网络的防火墙配置文件设置</span><span class="sxs-lookup"><span data-stu-id="801ab-599">Configures the firewall profile settings for domain networks</span></span>|
|<span data-ttu-id="801ab-600">firewallProfilePublic</span><span class="sxs-lookup"><span data-stu-id="801ab-600">firewallProfilePublic</span></span>|[<span data-ttu-id="801ab-601">windowsFirewallNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="801ab-601">windowsFirewallNetworkProfile</span></span>](../resources/intune-deviceconfig-windowsfirewallnetworkprofile.md)|<span data-ttu-id="801ab-602">配置公用网络的防火墙配置文件设置</span><span class="sxs-lookup"><span data-stu-id="801ab-602">Configures the firewall profile settings for public networks</span></span>|
|<span data-ttu-id="801ab-603">firewallProfilePrivate</span><span class="sxs-lookup"><span data-stu-id="801ab-603">firewallProfilePrivate</span></span>|[<span data-ttu-id="801ab-604">windowsFirewallNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="801ab-604">windowsFirewallNetworkProfile</span></span>](../resources/intune-deviceconfig-windowsfirewallnetworkprofile.md)|<span data-ttu-id="801ab-605">配置专用网络的防火墙配置文件设置</span><span class="sxs-lookup"><span data-stu-id="801ab-605">Configures the firewall profile settings for private networks</span></span>|
|<span data-ttu-id="801ab-606">defenderAdobeReaderLaunchChildProcess</span><span class="sxs-lookup"><span data-stu-id="801ab-606">defenderAdobeReaderLaunchChildProcess</span></span>|[<span data-ttu-id="801ab-607">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="801ab-607">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="801ab-608">值，该值指示 Adobe Reader 创建子进程的行为。</span><span class="sxs-lookup"><span data-stu-id="801ab-608">Value indicating the behavior of Adobe Reader from creating child processes.</span></span> <span data-ttu-id="801ab-609">可取值为：`userDefined`、`enable`、`auditMode`。</span><span class="sxs-lookup"><span data-stu-id="801ab-609">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="801ab-610">defenderAttackSurfaceReductionExcludedPaths</span><span class="sxs-lookup"><span data-stu-id="801ab-610">defenderAttackSurfaceReductionExcludedPaths</span></span>|<span data-ttu-id="801ab-611">String 集合</span><span class="sxs-lookup"><span data-stu-id="801ab-611">String collection</span></span>|<span data-ttu-id="801ab-612">要从攻击面减少规则中排除的 exe 文件和文件夹的列表</span><span class="sxs-lookup"><span data-stu-id="801ab-612">List of exe files and folders to be excluded from attack surface reduction rules</span></span>|
|<span data-ttu-id="801ab-613">defenderOfficeAppsOtherProcessInjectionType</span><span class="sxs-lookup"><span data-stu-id="801ab-613">defenderOfficeAppsOtherProcessInjectionType</span></span>|[<span data-ttu-id="801ab-614">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="801ab-614">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="801ab-615">值，该值指示插入到其他进程中的 Office 应用程序的行为。</span><span class="sxs-lookup"><span data-stu-id="801ab-615">Value indicating the behavior of Office applications injecting into other processes.</span></span> <span data-ttu-id="801ab-616">可取值为：`userDefined`、`block`、`auditMode`。</span><span class="sxs-lookup"><span data-stu-id="801ab-616">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="801ab-617">defenderOfficeAppsOtherProcessInjection</span><span class="sxs-lookup"><span data-stu-id="801ab-617">defenderOfficeAppsOtherProcessInjection</span></span>|[<span data-ttu-id="801ab-618">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="801ab-618">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="801ab-619">值，该值指示插入到其他进程中的 Office 应用程序的行为。</span><span class="sxs-lookup"><span data-stu-id="801ab-619">Value indicating the behavior of  Office applications injecting into other processes.</span></span> <span data-ttu-id="801ab-620">可取值为：`userDefined`、`enable`、`auditMode`。</span><span class="sxs-lookup"><span data-stu-id="801ab-620">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="801ab-621">defenderOfficeCommunicationAppsLaunchChildProcess</span><span class="sxs-lookup"><span data-stu-id="801ab-621">defenderOfficeCommunicationAppsLaunchChildProcess</span></span>|[<span data-ttu-id="801ab-622">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="801ab-622">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="801ab-623">值，该值指示 Office 通信应用程序（包括 Microsoft Outlook）在创建子进程时的行为。</span><span class="sxs-lookup"><span data-stu-id="801ab-623">Value indicating the behavior of Office communication applications, including Microsoft Outlook, from creating child processes.</span></span> <span data-ttu-id="801ab-624">可取值为：`userDefined`、`enable`、`auditMode`。</span><span class="sxs-lookup"><span data-stu-id="801ab-624">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="801ab-625">defenderOfficeAppsExecutableContentCreationOrLaunchType</span><span class="sxs-lookup"><span data-stu-id="801ab-625">defenderOfficeAppsExecutableContentCreationOrLaunchType</span></span>|[<span data-ttu-id="801ab-626">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="801ab-626">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="801ab-627">值，该值指示 Office 应用程序/宏创建或启动可执行内容的行为。</span><span class="sxs-lookup"><span data-stu-id="801ab-627">Value indicating the behavior of Office applications/macros creating or launching executable content.</span></span> <span data-ttu-id="801ab-628">可取值为：`userDefined`、`block`、`auditMode`。</span><span class="sxs-lookup"><span data-stu-id="801ab-628">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="801ab-629">defenderOfficeAppsExecutableContentCreationOrLaunch</span><span class="sxs-lookup"><span data-stu-id="801ab-629">defenderOfficeAppsExecutableContentCreationOrLaunch</span></span>|[<span data-ttu-id="801ab-630">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="801ab-630">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="801ab-631">值，该值指示 Office 应用程序/宏创建或启动可执行内容的行为。</span><span class="sxs-lookup"><span data-stu-id="801ab-631">Value indicating the behavior of Office applications/macros creating or launching executable content.</span></span> <span data-ttu-id="801ab-632">可取值为：`userDefined`、`enable`、`auditMode`。</span><span class="sxs-lookup"><span data-stu-id="801ab-632">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="801ab-633">defenderOfficeAppsLaunchChildProcessType</span><span class="sxs-lookup"><span data-stu-id="801ab-633">defenderOfficeAppsLaunchChildProcessType</span></span>|[<span data-ttu-id="801ab-634">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="801ab-634">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="801ab-635">值，该值指示 Office 应用程序启动子进程的行为。</span><span class="sxs-lookup"><span data-stu-id="801ab-635">Value indicating the behavior of Office application launching child processes.</span></span> <span data-ttu-id="801ab-636">可取值为：`userDefined`、`block`、`auditMode`。</span><span class="sxs-lookup"><span data-stu-id="801ab-636">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="801ab-637">defenderOfficeAppsLaunchChildProcess</span><span class="sxs-lookup"><span data-stu-id="801ab-637">defenderOfficeAppsLaunchChildProcess</span></span>|[<span data-ttu-id="801ab-638">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="801ab-638">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="801ab-639">值，该值指示 Office 应用程序启动子进程的行为。</span><span class="sxs-lookup"><span data-stu-id="801ab-639">Value indicating the behavior of Office application launching child processes.</span></span> <span data-ttu-id="801ab-640">可取值为：`userDefined`、`enable`、`auditMode`。</span><span class="sxs-lookup"><span data-stu-id="801ab-640">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="801ab-641">defenderOfficeMacroCodeAllowWin32ImportsType</span><span class="sxs-lookup"><span data-stu-id="801ab-641">defenderOfficeMacroCodeAllowWin32ImportsType</span></span>|[<span data-ttu-id="801ab-642">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="801ab-642">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="801ab-643">值，该值指示从 Office 中的宏代码的 Win32 导入行为。</span><span class="sxs-lookup"><span data-stu-id="801ab-643">Value indicating the behavior of Win32 imports from Macro code in Office.</span></span> <span data-ttu-id="801ab-644">可取值为：`userDefined`、`block`、`auditMode`。</span><span class="sxs-lookup"><span data-stu-id="801ab-644">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="801ab-645">defenderOfficeMacroCodeAllowWin32Imports</span><span class="sxs-lookup"><span data-stu-id="801ab-645">defenderOfficeMacroCodeAllowWin32Imports</span></span>|[<span data-ttu-id="801ab-646">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="801ab-646">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="801ab-647">值，该值指示从 Office 中的宏代码的 Win32 导入行为。</span><span class="sxs-lookup"><span data-stu-id="801ab-647">Value indicating the behavior of Win32 imports from Macro code in Office.</span></span> <span data-ttu-id="801ab-648">可取值为：`userDefined`、`enable`、`auditMode`。</span><span class="sxs-lookup"><span data-stu-id="801ab-648">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="801ab-649">defenderScriptObfuscatedMacroCodeType</span><span class="sxs-lookup"><span data-stu-id="801ab-649">defenderScriptObfuscatedMacroCodeType</span></span>|[<span data-ttu-id="801ab-650">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="801ab-650">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="801ab-651">值，该值指示模糊的 js/vbs/ps/宏代码的行为。</span><span class="sxs-lookup"><span data-stu-id="801ab-651">Value indicating the behavior of obfuscated js/vbs/ps/macro code.</span></span> <span data-ttu-id="801ab-652">可取值为：`userDefined`、`block`、`auditMode`。</span><span class="sxs-lookup"><span data-stu-id="801ab-652">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="801ab-653">defenderScriptObfuscatedMacroCode</span><span class="sxs-lookup"><span data-stu-id="801ab-653">defenderScriptObfuscatedMacroCode</span></span>|[<span data-ttu-id="801ab-654">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="801ab-654">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="801ab-655">值，该值指示模糊的 js/vbs/ps/宏代码的行为。</span><span class="sxs-lookup"><span data-stu-id="801ab-655">Value indicating the behavior of obfuscated js/vbs/ps/macro code.</span></span> <span data-ttu-id="801ab-656">可取值为：`userDefined`、`enable`、`auditMode`。</span><span class="sxs-lookup"><span data-stu-id="801ab-656">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="801ab-657">defenderScriptDownloadedPayloadExecutionType</span><span class="sxs-lookup"><span data-stu-id="801ab-657">defenderScriptDownloadedPayloadExecutionType</span></span>|[<span data-ttu-id="801ab-658">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="801ab-658">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="801ab-659">值，该值指示从 Internet 下载的 js/vbs 执行负载的行为。</span><span class="sxs-lookup"><span data-stu-id="801ab-659">Value indicating the behavior of js/vbs executing payload downloaded from Internet.</span></span> <span data-ttu-id="801ab-660">可取值为：`userDefined`、`block`、`auditMode`。</span><span class="sxs-lookup"><span data-stu-id="801ab-660">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="801ab-661">defenderScriptDownloadedPayloadExecution</span><span class="sxs-lookup"><span data-stu-id="801ab-661">defenderScriptDownloadedPayloadExecution</span></span>|[<span data-ttu-id="801ab-662">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="801ab-662">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="801ab-663">值，该值指示从 Internet 下载的 js/vbs 执行负载的行为。</span><span class="sxs-lookup"><span data-stu-id="801ab-663">Value indicating the behavior of js/vbs executing payload downloaded from Internet.</span></span> <span data-ttu-id="801ab-664">可取值为：`userDefined`、`enable`、`auditMode`。</span><span class="sxs-lookup"><span data-stu-id="801ab-664">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="801ab-665">defenderPreventCredentialStealingType</span><span class="sxs-lookup"><span data-stu-id="801ab-665">defenderPreventCredentialStealingType</span></span>|[<span data-ttu-id="801ab-666">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="801ab-666">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="801ab-667">值，该值指示是否允许从 Windows 本地安全机构子系统中盗取凭据。</span><span class="sxs-lookup"><span data-stu-id="801ab-667">Value indicating if credential stealing from the Windows local security authority subsystem is permitted.</span></span> <span data-ttu-id="801ab-668">可取值为：`userDefined`、`enable`、`auditMode`。</span><span class="sxs-lookup"><span data-stu-id="801ab-668">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="801ab-669">defenderProcessCreationType</span><span class="sxs-lookup"><span data-stu-id="801ab-669">defenderProcessCreationType</span></span>|[<span data-ttu-id="801ab-670">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="801ab-670">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="801ab-671">一个值，该值指示对源自 PSExec 和 WMI 命令的进程创建的响应。</span><span class="sxs-lookup"><span data-stu-id="801ab-671">Value indicating response to process creations originating from PSExec and WMI commands.</span></span> <span data-ttu-id="801ab-672">可取值为：`userDefined`、`block`、`auditMode`。</span><span class="sxs-lookup"><span data-stu-id="801ab-672">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="801ab-673">defenderProcessCreation</span><span class="sxs-lookup"><span data-stu-id="801ab-673">defenderProcessCreation</span></span>|[<span data-ttu-id="801ab-674">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="801ab-674">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="801ab-675">一个值，该值指示对源自 PSExec 和 WMI 命令的进程创建的响应。</span><span class="sxs-lookup"><span data-stu-id="801ab-675">Value indicating response to process creations originating from PSExec and WMI commands.</span></span> <span data-ttu-id="801ab-676">可取值为：`userDefined`、`enable`、`auditMode`。</span><span class="sxs-lookup"><span data-stu-id="801ab-676">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="801ab-677">defenderUntrustedUSBProcessType</span><span class="sxs-lookup"><span data-stu-id="801ab-677">defenderUntrustedUSBProcessType</span></span>|[<span data-ttu-id="801ab-678">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="801ab-678">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="801ab-679">指示对从 USB 运行的不受信任和未签名进程的响应的值。</span><span class="sxs-lookup"><span data-stu-id="801ab-679">Value indicating response to untrusted and unsigned processes that run from USB.</span></span> <span data-ttu-id="801ab-680">可取值为：`userDefined`、`block`、`auditMode`。</span><span class="sxs-lookup"><span data-stu-id="801ab-680">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="801ab-681">defenderUntrustedUSBProcess</span><span class="sxs-lookup"><span data-stu-id="801ab-681">defenderUntrustedUSBProcess</span></span>|[<span data-ttu-id="801ab-682">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="801ab-682">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="801ab-683">指示对从 USB 运行的不受信任和未签名进程的响应的值。</span><span class="sxs-lookup"><span data-stu-id="801ab-683">Value indicating response to untrusted and unsigned processes that run from USB.</span></span> <span data-ttu-id="801ab-684">可取值为：`userDefined`、`enable`、`auditMode`。</span><span class="sxs-lookup"><span data-stu-id="801ab-684">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="801ab-685">defenderUntrustedExecutableType</span><span class="sxs-lookup"><span data-stu-id="801ab-685">defenderUntrustedExecutableType</span></span>|[<span data-ttu-id="801ab-686">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="801ab-686">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="801ab-687">指示对不符合流行、年龄或受信任列表条件的可执行文件的响应的值。</span><span class="sxs-lookup"><span data-stu-id="801ab-687">Value indicating response to executables that don't meet a prevalence, age, or trusted list criteria.</span></span> <span data-ttu-id="801ab-688">可取值为：`userDefined`、`block`、`auditMode`。</span><span class="sxs-lookup"><span data-stu-id="801ab-688">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="801ab-689">defenderUntrustedExecutable</span><span class="sxs-lookup"><span data-stu-id="801ab-689">defenderUntrustedExecutable</span></span>|[<span data-ttu-id="801ab-690">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="801ab-690">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="801ab-691">指示对不符合流行、年龄或受信任列表条件的可执行文件的响应的值。</span><span class="sxs-lookup"><span data-stu-id="801ab-691">Value indicating response to executables that don't meet a prevalence, age, or trusted list criteria.</span></span> <span data-ttu-id="801ab-692">可取值为：`userDefined`、`enable`、`auditMode`。</span><span class="sxs-lookup"><span data-stu-id="801ab-692">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="801ab-693">defenderEmailContentExecutionType</span><span class="sxs-lookup"><span data-stu-id="801ab-693">defenderEmailContentExecutionType</span></span>|[<span data-ttu-id="801ab-694">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="801ab-694">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="801ab-695">一个值，该值指示是否应从电子邮件（web 邮件/邮件客户端）中删除可执行内容（exe、dll、ps、js、vbs 等）的执行。</span><span class="sxs-lookup"><span data-stu-id="801ab-695">Value indicating if execution of executable content (exe, dll, ps, js, vbs, etc) should be dropped from email (webmail/mail-client).</span></span> <span data-ttu-id="801ab-696">可取值为：`userDefined`、`block`、`auditMode`。</span><span class="sxs-lookup"><span data-stu-id="801ab-696">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="801ab-697">defenderEmailContentExecution</span><span class="sxs-lookup"><span data-stu-id="801ab-697">defenderEmailContentExecution</span></span>|[<span data-ttu-id="801ab-698">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="801ab-698">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="801ab-699">一个值，该值指示是否应从电子邮件（web 邮件/邮件客户端）中删除可执行内容（exe、dll、ps、js、vbs 等）的执行。</span><span class="sxs-lookup"><span data-stu-id="801ab-699">Value indicating if execution of executable content (exe, dll, ps, js, vbs, etc) should be dropped from email (webmail/mail-client).</span></span> <span data-ttu-id="801ab-700">可取值为：`userDefined`、`enable`、`auditMode`。</span><span class="sxs-lookup"><span data-stu-id="801ab-700">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="801ab-701">defenderAdvancedRansomewareProtectionType</span><span class="sxs-lookup"><span data-stu-id="801ab-701">defenderAdvancedRansomewareProtectionType</span></span>|[<span data-ttu-id="801ab-702">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="801ab-702">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="801ab-703">指示使用针对 ransomeware 的高级防护的值。</span><span class="sxs-lookup"><span data-stu-id="801ab-703">Value indicating use of advanced protection against ransomeware.</span></span> <span data-ttu-id="801ab-704">可取值为：`userDefined`、`enable`、`auditMode`。</span><span class="sxs-lookup"><span data-stu-id="801ab-704">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="801ab-705">defenderGuardMyFoldersType</span><span class="sxs-lookup"><span data-stu-id="801ab-705">defenderGuardMyFoldersType</span></span>|[<span data-ttu-id="801ab-706">folderProtectionType</span><span class="sxs-lookup"><span data-stu-id="801ab-706">folderProtectionType</span></span>](../resources/intune-deviceconfig-folderprotectiontype.md)|<span data-ttu-id="801ab-707">值，该值指示受保护文件夹的行为。</span><span class="sxs-lookup"><span data-stu-id="801ab-707">Value indicating the behavior of protected folders.</span></span> <span data-ttu-id="801ab-708">可取值为：`userDefined`、`enable`、`auditMode`、`blockDiskModification`、`auditDiskModification`。</span><span class="sxs-lookup"><span data-stu-id="801ab-708">Possible values are: `userDefined`, `enable`, `auditMode`, `blockDiskModification`, `auditDiskModification`.</span></span>|
|<span data-ttu-id="801ab-709">defenderGuardedFoldersAllowedAppPaths</span><span class="sxs-lookup"><span data-stu-id="801ab-709">defenderGuardedFoldersAllowedAppPaths</span></span>|<span data-ttu-id="801ab-710">字符串集合</span><span class="sxs-lookup"><span data-stu-id="801ab-710">String collection</span></span>|<span data-ttu-id="801ab-711">允许访问受保护文件夹的 exe 路径列表</span><span class="sxs-lookup"><span data-stu-id="801ab-711">List of paths to exe that are allowed to access protected folders</span></span>|
|<span data-ttu-id="801ab-712">defenderAdditionalGuardedFolders</span><span class="sxs-lookup"><span data-stu-id="801ab-712">defenderAdditionalGuardedFolders</span></span>|<span data-ttu-id="801ab-713">String 集合</span><span class="sxs-lookup"><span data-stu-id="801ab-713">String collection</span></span>|<span data-ttu-id="801ab-714">要添加到受保护文件夹列表的文件夹路径列表</span><span class="sxs-lookup"><span data-stu-id="801ab-714">List of folder paths to be added to the list of protected folders</span></span>|
|<span data-ttu-id="801ab-715">defenderNetworkProtectionType</span><span class="sxs-lookup"><span data-stu-id="801ab-715">defenderNetworkProtectionType</span></span>|[<span data-ttu-id="801ab-716">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="801ab-716">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="801ab-717">值，该值指示 NetworkProtection 的行为。</span><span class="sxs-lookup"><span data-stu-id="801ab-717">Value indicating the behavior of NetworkProtection.</span></span> <span data-ttu-id="801ab-718">可取值为：`userDefined`、`enable`、`auditMode`。</span><span class="sxs-lookup"><span data-stu-id="801ab-718">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="801ab-719">defenderExploitProtectionXml</span><span class="sxs-lookup"><span data-stu-id="801ab-719">defenderExploitProtectionXml</span></span>|<span data-ttu-id="801ab-720">Binary</span><span class="sxs-lookup"><span data-stu-id="801ab-720">Binary</span></span>|<span data-ttu-id="801ab-721">包含有关 Exploit Protection 详细信息的 xml 内容。</span><span class="sxs-lookup"><span data-stu-id="801ab-721">Xml content containing information regarding exploit protection details.</span></span>|
|<span data-ttu-id="801ab-722">defenderExploitProtectionXmlFileName</span><span class="sxs-lookup"><span data-stu-id="801ab-722">defenderExploitProtectionXmlFileName</span></span>|<span data-ttu-id="801ab-723">String</span><span class="sxs-lookup"><span data-stu-id="801ab-723">String</span></span>|<span data-ttu-id="801ab-724">从中获取 DefenderExploitProtectionXml 的文件的名称。</span><span class="sxs-lookup"><span data-stu-id="801ab-724">Name of the file from which DefenderExploitProtectionXml was obtained.</span></span>|
|<span data-ttu-id="801ab-725">defenderSecurityCenterBlockExploitProtectionOverride</span><span class="sxs-lookup"><span data-stu-id="801ab-725">defenderSecurityCenterBlockExploitProtectionOverride</span></span>|<span data-ttu-id="801ab-726">Boolean</span><span class="sxs-lookup"><span data-stu-id="801ab-726">Boolean</span></span>|<span data-ttu-id="801ab-727">指示是否阻止用户覆盖 Exploit Protection 设置。</span><span class="sxs-lookup"><span data-stu-id="801ab-727">Indicates whether or not to block user from overriding Exploit Protection settings.</span></span>|
|<span data-ttu-id="801ab-728">appLockerApplicationControl</span><span class="sxs-lookup"><span data-stu-id="801ab-728">appLockerApplicationControl</span></span>|[<span data-ttu-id="801ab-729">appLockerApplicationControlType</span><span class="sxs-lookup"><span data-stu-id="801ab-729">appLockerApplicationControlType</span></span>](../resources/intune-deviceconfig-applockerapplicationcontroltype.md)|<span data-ttu-id="801ab-730">使管理员能够选择在设备上允许哪些类型的应用。</span><span class="sxs-lookup"><span data-stu-id="801ab-730">Enables the Admin to choose what types of app to allow on devices.</span></span> <span data-ttu-id="801ab-731">可取值为：`notConfigured`、`enforceComponentsAndStoreApps`、`auditComponentsAndStoreApps`、`enforceComponentsStoreAppsAndSmartlocker`、`auditComponentsStoreAppsAndSmartlocker`。</span><span class="sxs-lookup"><span data-stu-id="801ab-731">Possible values are: `notConfigured`, `enforceComponentsAndStoreApps`, `auditComponentsAndStoreApps`, `enforceComponentsStoreAppsAndSmartlocker`, `auditComponentsStoreAppsAndSmartlocker`.</span></span>|
|<span data-ttu-id="801ab-732">deviceGuardLocalSystemAuthorityCredentialGuardSettings</span><span class="sxs-lookup"><span data-stu-id="801ab-732">deviceGuardLocalSystemAuthorityCredentialGuardSettings</span></span>|[<span data-ttu-id="801ab-733">deviceGuardLocalSystemAuthorityCredentialGuardType</span><span class="sxs-lookup"><span data-stu-id="801ab-733">deviceGuardLocalSystemAuthorityCredentialGuardType</span></span>](../resources/intune-deviceconfig-deviceguardlocalsystemauthoritycredentialguardtype.md)|<span data-ttu-id="801ab-734">如果平台安全级别具有安全启动和基于虚拟化的安全性均已启用，则打开 Credential Guard。</span><span class="sxs-lookup"><span data-stu-id="801ab-734">Turn on Credential Guard when Platform Security Level with Secure Boot and Virtualization Based Security are both enabled.</span></span> <span data-ttu-id="801ab-735">可取值为：`notConfigured`、`enableWithUEFILock`、`enableWithoutUEFILock`。</span><span class="sxs-lookup"><span data-stu-id="801ab-735">Possible values are: `notConfigured`, `enableWithUEFILock`, `enableWithoutUEFILock`.</span></span>|
|<span data-ttu-id="801ab-736">deviceGuardEnableVirtualizationBasedSecurity</span><span class="sxs-lookup"><span data-stu-id="801ab-736">deviceGuardEnableVirtualizationBasedSecurity</span></span>|<span data-ttu-id="801ab-737">Boolean</span><span class="sxs-lookup"><span data-stu-id="801ab-737">Boolean</span></span>|<span data-ttu-id="801ab-738">启用基于虚拟化的安全性（VBS）。</span><span class="sxs-lookup"><span data-stu-id="801ab-738">Turns On Virtualization Based Security(VBS).</span></span>|
|<span data-ttu-id="801ab-739">deviceGuardEnableSecureBootWithDMA</span><span class="sxs-lookup"><span data-stu-id="801ab-739">deviceGuardEnableSecureBootWithDMA</span></span>|<span data-ttu-id="801ab-740">Boolean</span><span class="sxs-lookup"><span data-stu-id="801ab-740">Boolean</span></span>|<span data-ttu-id="801ab-741">此属性将在5月2019中被弃用，并将替换为属性 DeviceGuardSecureBootWithDMA。</span><span class="sxs-lookup"><span data-stu-id="801ab-741">This property will be deprecated in May 2019 and will be replaced with property DeviceGuardSecureBootWithDMA.</span></span> <span data-ttu-id="801ab-742">指定是否在下次重新启动时启用平台安全级别。</span><span class="sxs-lookup"><span data-stu-id="801ab-742">Specifies whether Platform Security Level is enabled at next reboot.</span></span>|
|<span data-ttu-id="801ab-743">deviceGuardSecureBootWithDMA</span><span class="sxs-lookup"><span data-stu-id="801ab-743">deviceGuardSecureBootWithDMA</span></span>|[<span data-ttu-id="801ab-744">secureBootWithDMAType</span><span class="sxs-lookup"><span data-stu-id="801ab-744">secureBootWithDMAType</span></span>](../resources/intune-deviceconfig-securebootwithdmatype.md)|<span data-ttu-id="801ab-745">指定是否在下次重新启动时启用平台安全级别。</span><span class="sxs-lookup"><span data-stu-id="801ab-745">Specifies whether Platform Security Level is enabled at next reboot.</span></span> <span data-ttu-id="801ab-746">可取值为：`notConfigured`、`withoutDMA`、`withDMA`。</span><span class="sxs-lookup"><span data-stu-id="801ab-746">Possible values are: `notConfigured`, `withoutDMA`, `withDMA`.</span></span>|
|<span data-ttu-id="801ab-747">deviceGuardLaunchSystemGuard</span><span class="sxs-lookup"><span data-stu-id="801ab-747">deviceGuardLaunchSystemGuard</span></span>|[<span data-ttu-id="801ab-748">启用</span><span class="sxs-lookup"><span data-stu-id="801ab-748">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="801ab-749">允许 IT 管理员配置启动 "系统防护"。</span><span class="sxs-lookup"><span data-stu-id="801ab-749">Allows the IT admin to configure the launch of System Guard.</span></span> <span data-ttu-id="801ab-750">可取值为：`notConfigured`、`enabled`、`disabled`。</span><span class="sxs-lookup"><span data-stu-id="801ab-750">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="801ab-751">smartScreenEnableInShell</span><span class="sxs-lookup"><span data-stu-id="801ab-751">smartScreenEnableInShell</span></span>|<span data-ttu-id="801ab-752">Boolean</span><span class="sxs-lookup"><span data-stu-id="801ab-752">Boolean</span></span>|<span data-ttu-id="801ab-753">允许 IT 管理员配置适用于 Windows 的 SmartScreen。</span><span class="sxs-lookup"><span data-stu-id="801ab-753">Allows IT Admins to configure SmartScreen for Windows.</span></span>|
|<span data-ttu-id="801ab-754">smartScreenBlockOverrideForFiles</span><span class="sxs-lookup"><span data-stu-id="801ab-754">smartScreenBlockOverrideForFiles</span></span>|<span data-ttu-id="801ab-755">Boolean</span><span class="sxs-lookup"><span data-stu-id="801ab-755">Boolean</span></span>|<span data-ttu-id="801ab-756">允许 IT 管理员控制用户是否可以忽略 SmartScreen 警告并运行恶意文件。</span><span class="sxs-lookup"><span data-stu-id="801ab-756">Allows IT Admins to control whether users can can ignore SmartScreen warnings and run malicious files.</span></span>|
|<span data-ttu-id="801ab-757">applicationGuardEnabled</span><span class="sxs-lookup"><span data-stu-id="801ab-757">applicationGuardEnabled</span></span>|<span data-ttu-id="801ab-758">Boolean</span><span class="sxs-lookup"><span data-stu-id="801ab-758">Boolean</span></span>|<span data-ttu-id="801ab-759">启用 Windows Defender 应用程序防护</span><span class="sxs-lookup"><span data-stu-id="801ab-759">Enable Windows Defender Application Guard</span></span>|
|<span data-ttu-id="801ab-760">applicationGuardEnabledOptions</span><span class="sxs-lookup"><span data-stu-id="801ab-760">applicationGuardEnabledOptions</span></span>|[<span data-ttu-id="801ab-761">applicationGuardEnabledOptions</span><span class="sxs-lookup"><span data-stu-id="801ab-761">applicationGuardEnabledOptions</span></span>](../resources/intune-deviceconfig-applicationguardenabledoptions.md)|<span data-ttu-id="801ab-762">为较新的 Windows 版本启用 Windows Defender 应用程序防护。</span><span class="sxs-lookup"><span data-stu-id="801ab-762">Enable Windows Defender Application Guard for newer Windows builds.</span></span> <span data-ttu-id="801ab-763">可取值为：`notConfigured`、`enabledForEdge`、`enabledForOffice`、`enabledForEdgeAndOffice`。</span><span class="sxs-lookup"><span data-stu-id="801ab-763">Possible values are: `notConfigured`, `enabledForEdge`, `enabledForOffice`, `enabledForEdgeAndOffice`.</span></span>|
|<span data-ttu-id="801ab-764">applicationGuardBlockFileTransfer</span><span class="sxs-lookup"><span data-stu-id="801ab-764">applicationGuardBlockFileTransfer</span></span>|[<span data-ttu-id="801ab-765">applicationGuardBlockFileTransferType</span><span class="sxs-lookup"><span data-stu-id="801ab-765">applicationGuardBlockFileTransferType</span></span>](../resources/intune-deviceconfig-applicationguardblockfiletransfertype.md)|<span data-ttu-id="801ab-766">阻止剪贴板传输图像文件、文本文件或二者都不。</span><span class="sxs-lookup"><span data-stu-id="801ab-766">Block clipboard to transfer image file, text file or neither of them.</span></span> <span data-ttu-id="801ab-767">可取值为：`notConfigured`、`blockImageAndTextFile`、`blockImageFile`、`blockNone`、`blockTextFile`。</span><span class="sxs-lookup"><span data-stu-id="801ab-767">Possible values are: `notConfigured`, `blockImageAndTextFile`, `blockImageFile`, `blockNone`, `blockTextFile`.</span></span>|
|<span data-ttu-id="801ab-768">applicationGuardBlockNonEnterpriseContent</span><span class="sxs-lookup"><span data-stu-id="801ab-768">applicationGuardBlockNonEnterpriseContent</span></span>|<span data-ttu-id="801ab-769">Boolean</span><span class="sxs-lookup"><span data-stu-id="801ab-769">Boolean</span></span>|<span data-ttu-id="801ab-770">阻止企业站点加载非企业内容，例如第三方插件</span><span class="sxs-lookup"><span data-stu-id="801ab-770">Block enterprise sites to load non-enterprise content, such as third party plug-ins</span></span>|
|<span data-ttu-id="801ab-771">applicationGuardAllowPersistence</span><span class="sxs-lookup"><span data-stu-id="801ab-771">applicationGuardAllowPersistence</span></span>|<span data-ttu-id="801ab-772">Boolean</span><span class="sxs-lookup"><span data-stu-id="801ab-772">Boolean</span></span>|<span data-ttu-id="801ab-773">允许 App Guard 容器（收藏夹、Cookie、Web 密码等）内的持久用户生成数据</span><span class="sxs-lookup"><span data-stu-id="801ab-773">Allow persisting user generated data inside the App Guard Containter (favorites, cookies, web passwords, etc.)</span></span>|
|<span data-ttu-id="801ab-774">applicationGuardForceAuditing</span><span class="sxs-lookup"><span data-stu-id="801ab-774">applicationGuardForceAuditing</span></span>|<span data-ttu-id="801ab-775">Boolean</span><span class="sxs-lookup"><span data-stu-id="801ab-775">Boolean</span></span>|<span data-ttu-id="801ab-776">强制审核将存留 Windows 日志和事件以满足安全/符合性条件（示例事件是用户登录注销、特权使用、软件安装、系统更改等）</span><span class="sxs-lookup"><span data-stu-id="801ab-776">Force auditing will persist Windows logs and events to meet security/compliance criteria (sample events are user login-logoff, use of privilege rights, software installation, system changes, etc.)</span></span>|
|<span data-ttu-id="801ab-777">applicationGuardBlockClipboardSharing</span><span class="sxs-lookup"><span data-stu-id="801ab-777">applicationGuardBlockClipboardSharing</span></span>|[<span data-ttu-id="801ab-778">applicationGuardBlockClipboardSharingType</span><span class="sxs-lookup"><span data-stu-id="801ab-778">applicationGuardBlockClipboardSharingType</span></span>](../resources/intune-deviceconfig-applicationguardblockclipboardsharingtype.md)|<span data-ttu-id="801ab-779">阻止剪贴板将数据从主机共享到容器或从容器共享到主机，或阻止两种方式，或两种方式均不阻止。</span><span class="sxs-lookup"><span data-stu-id="801ab-779">Block clipboard to share data from Host to Container, or from Container to Host, or both ways, or neither ways.</span></span> <span data-ttu-id="801ab-780">可取值为：`notConfigured`、`blockBoth`、`blockHostToContainer`、`blockContainerToHost`、`blockNone`。</span><span class="sxs-lookup"><span data-stu-id="801ab-780">Possible values are: `notConfigured`, `blockBoth`, `blockHostToContainer`, `blockContainerToHost`, `blockNone`.</span></span>|
|<span data-ttu-id="801ab-781">applicationGuardAllowPrintToPDF</span><span class="sxs-lookup"><span data-stu-id="801ab-781">applicationGuardAllowPrintToPDF</span></span>|<span data-ttu-id="801ab-782">Boolean</span><span class="sxs-lookup"><span data-stu-id="801ab-782">Boolean</span></span>|<span data-ttu-id="801ab-783">允许从容器打印为 PDF 格式</span><span class="sxs-lookup"><span data-stu-id="801ab-783">Allow printing to PDF from Container</span></span>|
|<span data-ttu-id="801ab-784">applicationGuardAllowPrintToXPS</span><span class="sxs-lookup"><span data-stu-id="801ab-784">applicationGuardAllowPrintToXPS</span></span>|<span data-ttu-id="801ab-785">Boolean</span><span class="sxs-lookup"><span data-stu-id="801ab-785">Boolean</span></span>|<span data-ttu-id="801ab-786">允许从容器打印为 XPS 格式</span><span class="sxs-lookup"><span data-stu-id="801ab-786">Allow printing to XPS from Container</span></span>|
|<span data-ttu-id="801ab-787">applicationGuardAllowPrintToLocalPrinters</span><span class="sxs-lookup"><span data-stu-id="801ab-787">applicationGuardAllowPrintToLocalPrinters</span></span>|<span data-ttu-id="801ab-788">Boolean</span><span class="sxs-lookup"><span data-stu-id="801ab-788">Boolean</span></span>|<span data-ttu-id="801ab-789">允许从容器打印到本地打印机</span><span class="sxs-lookup"><span data-stu-id="801ab-789">Allow printing to Local Printers from Container</span></span>|
|<span data-ttu-id="801ab-790">applicationGuardAllowPrintToNetworkPrinters</span><span class="sxs-lookup"><span data-stu-id="801ab-790">applicationGuardAllowPrintToNetworkPrinters</span></span>|<span data-ttu-id="801ab-791">Boolean</span><span class="sxs-lookup"><span data-stu-id="801ab-791">Boolean</span></span>|<span data-ttu-id="801ab-792">允许从容器打印到网络打印机</span><span class="sxs-lookup"><span data-stu-id="801ab-792">Allow printing to Network Printers from Container</span></span>|
|<span data-ttu-id="801ab-793">applicationGuardAllowVirtualGPU</span><span class="sxs-lookup"><span data-stu-id="801ab-793">applicationGuardAllowVirtualGPU</span></span>|<span data-ttu-id="801ab-794">Boolean</span><span class="sxs-lookup"><span data-stu-id="801ab-794">Boolean</span></span>|<span data-ttu-id="801ab-795">允许应用程序防护使用虚拟 GPU</span><span class="sxs-lookup"><span data-stu-id="801ab-795">Allow application guard to use virtual GPU</span></span>|
|<span data-ttu-id="801ab-796">applicationGuardAllowFileSaveOnHost</span><span class="sxs-lookup"><span data-stu-id="801ab-796">applicationGuardAllowFileSaveOnHost</span></span>|<span data-ttu-id="801ab-797">Boolean</span><span class="sxs-lookup"><span data-stu-id="801ab-797">Boolean</span></span>|<span data-ttu-id="801ab-798">允许用户从应用程序防护容器中的边缘下载文件并将其保存在主机文件系统上</span><span class="sxs-lookup"><span data-stu-id="801ab-798">Allow users to download files from Edge in the application guard container and save them on the host file system</span></span>|
|<span data-ttu-id="801ab-799">bitLockerAllowStandardUserEncryption</span><span class="sxs-lookup"><span data-stu-id="801ab-799">bitLockerAllowStandardUserEncryption</span></span>|<span data-ttu-id="801ab-800">Boolean</span><span class="sxs-lookup"><span data-stu-id="801ab-800">Boolean</span></span>|<span data-ttu-id="801ab-801">允许管理员允许标准用户在 Azure AD 加入过程中启用 encrpytion。</span><span class="sxs-lookup"><span data-stu-id="801ab-801">Allows the admin to allow standard users to enable encrpytion during Azure AD Join.</span></span>|
|<span data-ttu-id="801ab-802">bitLockerDisableWarningForOtherDiskEncryption</span><span class="sxs-lookup"><span data-stu-id="801ab-802">bitLockerDisableWarningForOtherDiskEncryption</span></span>|<span data-ttu-id="801ab-803">Boolean</span><span class="sxs-lookup"><span data-stu-id="801ab-803">Boolean</span></span>|<span data-ttu-id="801ab-804">允许管理员禁用对用户计算机上其他磁盘加密的警告提示。</span><span class="sxs-lookup"><span data-stu-id="801ab-804">Allows the Admin to disable the warning prompt for other disk encryption on the user machines.</span></span>|
|<span data-ttu-id="801ab-805">bitLockerEnableStorageCardEncryptionOnMobile</span><span class="sxs-lookup"><span data-stu-id="801ab-805">bitLockerEnableStorageCardEncryptionOnMobile</span></span>|<span data-ttu-id="801ab-806">Boolean</span><span class="sxs-lookup"><span data-stu-id="801ab-806">Boolean</span></span>|<span data-ttu-id="801ab-807">允许管理员要求使用 BitLocker 开启加密功能。</span><span class="sxs-lookup"><span data-stu-id="801ab-807">Allows the admin to require encryption to be turned on using BitLocker.</span></span> <span data-ttu-id="801ab-808">此策略仅适用于移动 SKU。</span><span class="sxs-lookup"><span data-stu-id="801ab-808">This policy is valid only for a mobile SKU.</span></span>|
|<span data-ttu-id="801ab-809">bitLockerEncryptDevice</span><span class="sxs-lookup"><span data-stu-id="801ab-809">bitLockerEncryptDevice</span></span>|<span data-ttu-id="801ab-810">Boolean</span><span class="sxs-lookup"><span data-stu-id="801ab-810">Boolean</span></span>|<span data-ttu-id="801ab-811">允许管理员要求使用 BitLocker 开启加密功能。</span><span class="sxs-lookup"><span data-stu-id="801ab-811">Allows the admin to require encryption to be turned on using BitLocker.</span></span>|
|<span data-ttu-id="801ab-812">bitLockerSystemDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="801ab-812">bitLockerSystemDrivePolicy</span></span>|[<span data-ttu-id="801ab-813">bitLockerSystemDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="801ab-813">bitLockerSystemDrivePolicy</span></span>](../resources/intune-deviceconfig-bitlockersystemdrivepolicy.md)|<span data-ttu-id="801ab-814">BitLocker 系统驱动器策略。</span><span class="sxs-lookup"><span data-stu-id="801ab-814">BitLocker System Drive Policy.</span></span>|
|<span data-ttu-id="801ab-815">bitLockerFixedDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="801ab-815">bitLockerFixedDrivePolicy</span></span>|[<span data-ttu-id="801ab-816">bitLockerFixedDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="801ab-816">bitLockerFixedDrivePolicy</span></span>](../resources/intune-deviceconfig-bitlockerfixeddrivepolicy.md)|<span data-ttu-id="801ab-817">BitLocker 固定驱动器策略。</span><span class="sxs-lookup"><span data-stu-id="801ab-817">BitLocker Fixed Drive Policy.</span></span>|
|<span data-ttu-id="801ab-818">bitLockerRemovableDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="801ab-818">bitLockerRemovableDrivePolicy</span></span>|[<span data-ttu-id="801ab-819">bitLockerRemovableDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="801ab-819">bitLockerRemovableDrivePolicy</span></span>](../resources/intune-deviceconfig-bitlockerremovabledrivepolicy.md)|<span data-ttu-id="801ab-820">BitLocker 可移动驱动器策略。</span><span class="sxs-lookup"><span data-stu-id="801ab-820">BitLocker Removable Drive Policy.</span></span>|
|<span data-ttu-id="801ab-821">bitLockerRecoveryPasswordRotation</span><span class="sxs-lookup"><span data-stu-id="801ab-821">bitLockerRecoveryPasswordRotation</span></span>|[<span data-ttu-id="801ab-822">bitLockerRecoveryPasswordRotationType</span><span class="sxs-lookup"><span data-stu-id="801ab-822">bitLockerRecoveryPasswordRotationType</span></span>](../resources/intune-deviceconfig-bitlockerrecoverypasswordrotationtype.md)|<span data-ttu-id="801ab-823">此设置在操作系统驱动器恢复后启动客户端驱动的恢复密码轮替（使用 bootmgr 或 WinRE）。</span><span class="sxs-lookup"><span data-stu-id="801ab-823">This setting initiates a client-driven recovery password rotation after an OS drive recovery (either by using bootmgr or WinRE).</span></span> <span data-ttu-id="801ab-824">可取值为：`notConfigured`、`disabled`、`enabledForAzureAd`、`enabledForAzureAdAndHybrid`。</span><span class="sxs-lookup"><span data-stu-id="801ab-824">Possible values are: `notConfigured`, `disabled`, `enabledForAzureAd`, `enabledForAzureAdAndHybrid`.</span></span>|
|<span data-ttu-id="801ab-825">defenderDisableScanArchiveFiles</span><span class="sxs-lookup"><span data-stu-id="801ab-825">defenderDisableScanArchiveFiles</span></span>|<span data-ttu-id="801ab-826">Boolean</span><span class="sxs-lookup"><span data-stu-id="801ab-826">Boolean</span></span>|<span data-ttu-id="801ab-827">允许或禁止扫描存档。</span><span class="sxs-lookup"><span data-stu-id="801ab-827">Allows or disallows scanning of archives.</span></span>|
|<span data-ttu-id="801ab-828">defenderAllowScanArchiveFiles</span><span class="sxs-lookup"><span data-stu-id="801ab-828">defenderAllowScanArchiveFiles</span></span>|<span data-ttu-id="801ab-829">Boolean</span><span class="sxs-lookup"><span data-stu-id="801ab-829">Boolean</span></span>|<span data-ttu-id="801ab-830">允许或禁止扫描存档。</span><span class="sxs-lookup"><span data-stu-id="801ab-830">Allows or disallows scanning of archives.</span></span>|
|<span data-ttu-id="801ab-831">defenderDisableBehaviorMonitoring</span><span class="sxs-lookup"><span data-stu-id="801ab-831">defenderDisableBehaviorMonitoring</span></span>|<span data-ttu-id="801ab-832">Boolean</span><span class="sxs-lookup"><span data-stu-id="801ab-832">Boolean</span></span>|<span data-ttu-id="801ab-833">允许或禁止 Windows Defender 行为监控功能。</span><span class="sxs-lookup"><span data-stu-id="801ab-833">Allows or disallows Windows Defender Behavior Monitoring functionality.</span></span>|
|<span data-ttu-id="801ab-834">defenderAllowBehaviorMonitoring</span><span class="sxs-lookup"><span data-stu-id="801ab-834">defenderAllowBehaviorMonitoring</span></span>|<span data-ttu-id="801ab-835">Boolean</span><span class="sxs-lookup"><span data-stu-id="801ab-835">Boolean</span></span>|<span data-ttu-id="801ab-836">允许或禁止 Windows Defender 行为监控功能。</span><span class="sxs-lookup"><span data-stu-id="801ab-836">Allows or disallows Windows Defender Behavior Monitoring functionality.</span></span>|
|<span data-ttu-id="801ab-837">defenderDisableCloudProtection</span><span class="sxs-lookup"><span data-stu-id="801ab-837">defenderDisableCloudProtection</span></span>|<span data-ttu-id="801ab-838">Boolean</span><span class="sxs-lookup"><span data-stu-id="801ab-838">Boolean</span></span>|<span data-ttu-id="801ab-839">为最大限度地保护你的电脑，Windows Defender 将向 Microsoft 发送有关发现的任何问题的信息。</span><span class="sxs-lookup"><span data-stu-id="801ab-839">To best protect your PC, Windows Defender will send information to Microsoft about any problems it finds.</span></span> <span data-ttu-id="801ab-840">Microsoft 将分析该信息，详细了解影响您和其他客户的问题，并提供改进的解决方案。</span><span class="sxs-lookup"><span data-stu-id="801ab-840">Microsoft will analyze that information, learn more about problems affecting you and other customers, and offer improved solutions.</span></span>|
|<span data-ttu-id="801ab-841">defenderAllowCloudProtection</span><span class="sxs-lookup"><span data-stu-id="801ab-841">defenderAllowCloudProtection</span></span>|<span data-ttu-id="801ab-842">Boolean</span><span class="sxs-lookup"><span data-stu-id="801ab-842">Boolean</span></span>|<span data-ttu-id="801ab-843">为最大限度地保护你的电脑，Windows Defender 将向 Microsoft 发送有关发现的任何问题的信息。</span><span class="sxs-lookup"><span data-stu-id="801ab-843">To best protect your PC, Windows Defender will send information to Microsoft about any problems it finds.</span></span> <span data-ttu-id="801ab-844">Microsoft 将分析该信息，详细了解影响您和其他客户的问题，并提供改进的解决方案。</span><span class="sxs-lookup"><span data-stu-id="801ab-844">Microsoft will analyze that information, learn more about problems affecting you and other customers, and offer improved solutions.</span></span>|
|<span data-ttu-id="801ab-845">defenderEnableScanIncomingMail</span><span class="sxs-lookup"><span data-stu-id="801ab-845">defenderEnableScanIncomingMail</span></span>|<span data-ttu-id="801ab-846">Boolean</span><span class="sxs-lookup"><span data-stu-id="801ab-846">Boolean</span></span>|<span data-ttu-id="801ab-847">允许或禁止扫描电子邮件。</span><span class="sxs-lookup"><span data-stu-id="801ab-847">Allows or disallows scanning of email.</span></span>|
|<span data-ttu-id="801ab-848">defenderEnableScanMappedNetworkDrivesDuringFullScan</span><span class="sxs-lookup"><span data-stu-id="801ab-848">defenderEnableScanMappedNetworkDrivesDuringFullScan</span></span>|<span data-ttu-id="801ab-849">Boolean</span><span class="sxs-lookup"><span data-stu-id="801ab-849">Boolean</span></span>|<span data-ttu-id="801ab-850">允许或禁止对映射的网络驱动器进行完全扫描。</span><span class="sxs-lookup"><span data-stu-id="801ab-850">Allows or disallows a full scan of mapped network drives.</span></span>|
|<span data-ttu-id="801ab-851">defenderDisableScanRemovableDrivesDuringFullScan</span><span class="sxs-lookup"><span data-stu-id="801ab-851">defenderDisableScanRemovableDrivesDuringFullScan</span></span>|<span data-ttu-id="801ab-852">Boolean</span><span class="sxs-lookup"><span data-stu-id="801ab-852">Boolean</span></span>|<span data-ttu-id="801ab-853">允许或禁止对可移动驱动器进行完全扫描。</span><span class="sxs-lookup"><span data-stu-id="801ab-853">Allows or disallows a full scan of removable drives.</span></span> <span data-ttu-id="801ab-854">在快速扫描过程中，可能仍会扫描可移动驱动器。</span><span class="sxs-lookup"><span data-stu-id="801ab-854">During a quick scan, removable drives may still be scanned.</span></span>|
|<span data-ttu-id="801ab-855">defenderAllowScanRemovableDrivesDuringFullScan</span><span class="sxs-lookup"><span data-stu-id="801ab-855">defenderAllowScanRemovableDrivesDuringFullScan</span></span>|<span data-ttu-id="801ab-856">Boolean</span><span class="sxs-lookup"><span data-stu-id="801ab-856">Boolean</span></span>|<span data-ttu-id="801ab-857">允许或禁止对可移动驱动器进行完全扫描。</span><span class="sxs-lookup"><span data-stu-id="801ab-857">Allows or disallows a full scan of removable drives.</span></span> <span data-ttu-id="801ab-858">在快速扫描过程中，可能仍会扫描可移动驱动器。</span><span class="sxs-lookup"><span data-stu-id="801ab-858">During a quick scan, removable drives may still be scanned.</span></span>|
|<span data-ttu-id="801ab-859">defenderDisableScanDownloads</span><span class="sxs-lookup"><span data-stu-id="801ab-859">defenderDisableScanDownloads</span></span>|<span data-ttu-id="801ab-860">Boolean</span><span class="sxs-lookup"><span data-stu-id="801ab-860">Boolean</span></span>|<span data-ttu-id="801ab-861">允许或禁止 Windows Defender IOAVP 保护功能。</span><span class="sxs-lookup"><span data-stu-id="801ab-861">Allows or disallows Windows Defender IOAVP Protection functionality.</span></span>|
|<span data-ttu-id="801ab-862">defenderAllowScanDownloads</span><span class="sxs-lookup"><span data-stu-id="801ab-862">defenderAllowScanDownloads</span></span>|<span data-ttu-id="801ab-863">Boolean</span><span class="sxs-lookup"><span data-stu-id="801ab-863">Boolean</span></span>|<span data-ttu-id="801ab-864">允许或禁止 Windows Defender IOAVP 保护功能。</span><span class="sxs-lookup"><span data-stu-id="801ab-864">Allows or disallows Windows Defender IOAVP Protection functionality.</span></span>|
|<span data-ttu-id="801ab-865">defenderDisableIntrusionPreventionSystem</span><span class="sxs-lookup"><span data-stu-id="801ab-865">defenderDisableIntrusionPreventionSystem</span></span>|<span data-ttu-id="801ab-866">Boolean</span><span class="sxs-lookup"><span data-stu-id="801ab-866">Boolean</span></span>|<span data-ttu-id="801ab-867">允许或禁止 Windows Defender 入侵防护功能。</span><span class="sxs-lookup"><span data-stu-id="801ab-867">Allows or disallows Windows Defender Intrusion Prevention functionality.</span></span>|
|<span data-ttu-id="801ab-868">defenderAllowIntrusionPreventionSystem</span><span class="sxs-lookup"><span data-stu-id="801ab-868">defenderAllowIntrusionPreventionSystem</span></span>|<span data-ttu-id="801ab-869">Boolean</span><span class="sxs-lookup"><span data-stu-id="801ab-869">Boolean</span></span>|<span data-ttu-id="801ab-870">允许或禁止 Windows Defender 入侵防护功能。</span><span class="sxs-lookup"><span data-stu-id="801ab-870">Allows or disallows Windows Defender Intrusion Prevention functionality.</span></span>|
|<span data-ttu-id="801ab-871">defenderDisableOnAccessProtection</span><span class="sxs-lookup"><span data-stu-id="801ab-871">defenderDisableOnAccessProtection</span></span>|<span data-ttu-id="801ab-872">Boolean</span><span class="sxs-lookup"><span data-stu-id="801ab-872">Boolean</span></span>|<span data-ttu-id="801ab-873">允许或禁止 Windows Defender 访问保护功能。</span><span class="sxs-lookup"><span data-stu-id="801ab-873">Allows or disallows Windows Defender On Access Protection functionality.</span></span>|
|<span data-ttu-id="801ab-874">defenderAllowOnAccessProtection</span><span class="sxs-lookup"><span data-stu-id="801ab-874">defenderAllowOnAccessProtection</span></span>|<span data-ttu-id="801ab-875">Boolean</span><span class="sxs-lookup"><span data-stu-id="801ab-875">Boolean</span></span>|<span data-ttu-id="801ab-876">允许或禁止 Windows Defender 访问保护功能。</span><span class="sxs-lookup"><span data-stu-id="801ab-876">Allows or disallows Windows Defender On Access Protection functionality.</span></span>|
|<span data-ttu-id="801ab-877">defenderDisableRealTimeMonitoring</span><span class="sxs-lookup"><span data-stu-id="801ab-877">defenderDisableRealTimeMonitoring</span></span>|<span data-ttu-id="801ab-878">Boolean</span><span class="sxs-lookup"><span data-stu-id="801ab-878">Boolean</span></span>|<span data-ttu-id="801ab-879">允许或禁止 Windows Defender 实时监视功能。</span><span class="sxs-lookup"><span data-stu-id="801ab-879">Allows or disallows Windows Defender Realtime Monitoring functionality.</span></span>|
|<span data-ttu-id="801ab-880">defenderAllowRealTimeMonitoring</span><span class="sxs-lookup"><span data-stu-id="801ab-880">defenderAllowRealTimeMonitoring</span></span>|<span data-ttu-id="801ab-881">Boolean</span><span class="sxs-lookup"><span data-stu-id="801ab-881">Boolean</span></span>|<span data-ttu-id="801ab-882">允许或禁止 Windows Defender 实时监视功能。</span><span class="sxs-lookup"><span data-stu-id="801ab-882">Allows or disallows Windows Defender Realtime Monitoring functionality.</span></span>|
|<span data-ttu-id="801ab-883">defenderDisableScanNetworkFiles</span><span class="sxs-lookup"><span data-stu-id="801ab-883">defenderDisableScanNetworkFiles</span></span>|<span data-ttu-id="801ab-884">Boolean</span><span class="sxs-lookup"><span data-stu-id="801ab-884">Boolean</span></span>|<span data-ttu-id="801ab-885">允许或禁止扫描网络文件。</span><span class="sxs-lookup"><span data-stu-id="801ab-885">Allows or disallows a scanning of network files.</span></span>|
|<span data-ttu-id="801ab-886">defenderAllowScanNetworkFiles</span><span class="sxs-lookup"><span data-stu-id="801ab-886">defenderAllowScanNetworkFiles</span></span>|<span data-ttu-id="801ab-887">Boolean</span><span class="sxs-lookup"><span data-stu-id="801ab-887">Boolean</span></span>|<span data-ttu-id="801ab-888">允许或禁止扫描网络文件。</span><span class="sxs-lookup"><span data-stu-id="801ab-888">Allows or disallows a scanning of network files.</span></span>|
|<span data-ttu-id="801ab-889">defenderDisableScanScriptsLoadedInInternetExplorer</span><span class="sxs-lookup"><span data-stu-id="801ab-889">defenderDisableScanScriptsLoadedInInternetExplorer</span></span>|<span data-ttu-id="801ab-890">Boolean</span><span class="sxs-lookup"><span data-stu-id="801ab-890">Boolean</span></span>|<span data-ttu-id="801ab-891">允许或禁止 Windows Defender 脚本扫描功能。</span><span class="sxs-lookup"><span data-stu-id="801ab-891">Allows or disallows Windows Defender Script Scanning functionality.</span></span>|
|<span data-ttu-id="801ab-892">defenderAllowScanScriptsLoadedInInternetExplorer</span><span class="sxs-lookup"><span data-stu-id="801ab-892">defenderAllowScanScriptsLoadedInInternetExplorer</span></span>|<span data-ttu-id="801ab-893">Boolean</span><span class="sxs-lookup"><span data-stu-id="801ab-893">Boolean</span></span>|<span data-ttu-id="801ab-894">允许或禁止 Windows Defender 脚本扫描功能。</span><span class="sxs-lookup"><span data-stu-id="801ab-894">Allows or disallows Windows Defender Script Scanning functionality.</span></span>|
|<span data-ttu-id="801ab-895">defenderBlockEndUserAccess</span><span class="sxs-lookup"><span data-stu-id="801ab-895">defenderBlockEndUserAccess</span></span>|<span data-ttu-id="801ab-896">Boolean</span><span class="sxs-lookup"><span data-stu-id="801ab-896">Boolean</span></span>|<span data-ttu-id="801ab-897">允许或禁止用户访问 Windows Defender UI。</span><span class="sxs-lookup"><span data-stu-id="801ab-897">Allows or disallows user access to the Windows Defender UI.</span></span> <span data-ttu-id="801ab-898">如果不允许，将同时禁止显示所有 Windows Defender 通知。</span><span class="sxs-lookup"><span data-stu-id="801ab-898">If disallowed, all Windows Defender notifications will also be suppressed.</span></span>|
|<span data-ttu-id="801ab-899">defenderAllowEndUserAccess</span><span class="sxs-lookup"><span data-stu-id="801ab-899">defenderAllowEndUserAccess</span></span>|<span data-ttu-id="801ab-900">Boolean</span><span class="sxs-lookup"><span data-stu-id="801ab-900">Boolean</span></span>|<span data-ttu-id="801ab-901">允许或禁止用户访问 Windows Defender UI。</span><span class="sxs-lookup"><span data-stu-id="801ab-901">Allows or disallows user access to the Windows Defender UI.</span></span> <span data-ttu-id="801ab-902">如果不允许，将同时禁止显示所有 Windows Defender 通知。</span><span class="sxs-lookup"><span data-stu-id="801ab-902">If disallowed, all Windows Defender notifications will also be suppressed.</span></span>|
|<span data-ttu-id="801ab-903">defenderScanMaxCpuPercentage</span><span class="sxs-lookup"><span data-stu-id="801ab-903">defenderScanMaxCpuPercentage</span></span>|<span data-ttu-id="801ab-904">Int32</span><span class="sxs-lookup"><span data-stu-id="801ab-904">Int32</span></span>|<span data-ttu-id="801ab-905">表示 Windows Defender 扫描的平均 CPU 负载因子（以百分比为单位）。</span><span class="sxs-lookup"><span data-stu-id="801ab-905">Represents the average CPU load factor for the Windows Defender scan (in percent).</span></span> <span data-ttu-id="801ab-906">默认值为 50。</span><span class="sxs-lookup"><span data-stu-id="801ab-906">The default value is 50.</span></span> <span data-ttu-id="801ab-907">有效值为 0 至 100</span><span class="sxs-lookup"><span data-stu-id="801ab-907">Valid values 0 to 100</span></span>|
|<span data-ttu-id="801ab-908">defenderCheckForSignaturesBeforeRunningScan</span><span class="sxs-lookup"><span data-stu-id="801ab-908">defenderCheckForSignaturesBeforeRunningScan</span></span>|<span data-ttu-id="801ab-909">Boolean</span><span class="sxs-lookup"><span data-stu-id="801ab-909">Boolean</span></span>|<span data-ttu-id="801ab-910">通过此策略设置，您可以管理在运行扫描前是否检查新病毒和间谍软件定义。</span><span class="sxs-lookup"><span data-stu-id="801ab-910">This policy setting allows you to manage whether a check for new virus and spyware definitions will occur before running a scan.</span></span>|
|<span data-ttu-id="801ab-911">defenderCloudBlockLevel</span><span class="sxs-lookup"><span data-stu-id="801ab-911">defenderCloudBlockLevel</span></span>|[<span data-ttu-id="801ab-912">defenderCloudBlockLevelType</span><span class="sxs-lookup"><span data-stu-id="801ab-912">defenderCloudBlockLevelType</span></span>](../resources/intune-deviceconfig-defendercloudblockleveltype.md)|<span data-ttu-id="801ab-913">在 Windows 10 版本1709中添加。</span><span class="sxs-lookup"><span data-stu-id="801ab-913">Added in Windows 10, version 1709.</span></span> <span data-ttu-id="801ab-914">此策略设置确定 Windows Defender 防病毒在阻止和扫描可疑文件时的积极程度。</span><span class="sxs-lookup"><span data-stu-id="801ab-914">This policy setting determines how aggressive Windows Defender Antivirus will be in blocking and scanning suspicious files.</span></span> <span data-ttu-id="801ab-915">值类型为 integer。</span><span class="sxs-lookup"><span data-stu-id="801ab-915">Value type is integer.</span></span> <span data-ttu-id="801ab-916">此功能需要启用 "加入 Microsoft MAPS" 设置，才能正常运行。</span><span class="sxs-lookup"><span data-stu-id="801ab-916">This feature requires the "Join Microsoft MAPS" setting enabled in order to function.</span></span> <span data-ttu-id="801ab-917">可取值为：`notConfigured`、`high`、`highPlus`、`zeroTolerance`。</span><span class="sxs-lookup"><span data-stu-id="801ab-917">Possible values are: `notConfigured`, `high`, `highPlus`, `zeroTolerance`.</span></span>|
|<span data-ttu-id="801ab-918">defenderCloudExtendedTimeoutInSeconds</span><span class="sxs-lookup"><span data-stu-id="801ab-918">defenderCloudExtendedTimeoutInSeconds</span></span>|<span data-ttu-id="801ab-919">Int32</span><span class="sxs-lookup"><span data-stu-id="801ab-919">Int32</span></span>|<span data-ttu-id="801ab-920">在 Windows 10 版本1709中添加。</span><span class="sxs-lookup"><span data-stu-id="801ab-920">Added in Windows 10, version 1709.</span></span> <span data-ttu-id="801ab-921">此功能允许 Windows Defender 防病毒阻止可疑文件长达60秒，并在云中对其进行扫描以确保其安全。</span><span class="sxs-lookup"><span data-stu-id="801ab-921">This feature allows Windows Defender Antivirus to block a suspicious file for up to 60 seconds, and scan it in the cloud to make sure it's safe.</span></span> <span data-ttu-id="801ab-922">值类型为 integer，范围为 0-50。</span><span class="sxs-lookup"><span data-stu-id="801ab-922">Value type is integer, range is 0 - 50.</span></span> <span data-ttu-id="801ab-923">此功能依赖于其他三个映射设置必须全部启用-"配置 ' 在首次看到时阻止 '" 功能; "加入 Microsoft MAPS ";"需要进一步分析时发送文件示例"。</span><span class="sxs-lookup"><span data-stu-id="801ab-923">This feature depends on three other MAPS settings the must all be enabled- "Configure the 'Block at First Sight' feature; "Join Microsoft MAPS"; "Send file samples when further analysis is required".</span></span> <span data-ttu-id="801ab-924">有效值为 0 至 50</span><span class="sxs-lookup"><span data-stu-id="801ab-924">Valid values 0 to 50</span></span>|
|<span data-ttu-id="801ab-925">defenderDaysBeforeDeletingQuarantinedMalware</span><span class="sxs-lookup"><span data-stu-id="801ab-925">defenderDaysBeforeDeletingQuarantinedMalware</span></span>|<span data-ttu-id="801ab-926">Int32</span><span class="sxs-lookup"><span data-stu-id="801ab-926">Int32</span></span>|<span data-ttu-id="801ab-927">隔离项目将存储在系统上的时间段（以天为单位）。</span><span class="sxs-lookup"><span data-stu-id="801ab-927">Time period (in days) that quarantine items will be stored on the system.</span></span> <span data-ttu-id="801ab-928">有效值为 0 至 90</span><span class="sxs-lookup"><span data-stu-id="801ab-928">Valid values 0 to 90</span></span>|
|<span data-ttu-id="801ab-929">defenderDisableCatchupFullScan</span><span class="sxs-lookup"><span data-stu-id="801ab-929">defenderDisableCatchupFullScan</span></span>|<span data-ttu-id="801ab-930">Boolean</span><span class="sxs-lookup"><span data-stu-id="801ab-930">Boolean</span></span>|<span data-ttu-id="801ab-931">通过此策略设置，您可以配置计划完全扫描的追赶扫描。</span><span class="sxs-lookup"><span data-stu-id="801ab-931">This policy setting allows you to configure catch-up scans for scheduled full scans.</span></span> <span data-ttu-id="801ab-932">追赶扫描是由于错过了定期计划的扫描而启动的扫描。</span><span class="sxs-lookup"><span data-stu-id="801ab-932">A catch-up scan is a scan that is initiated because a regularly scheduled scan was missed.</span></span> <span data-ttu-id="801ab-933">通常情况下，这些计划扫描会因计算机在计划时间关闭而丢失。</span><span class="sxs-lookup"><span data-stu-id="801ab-933">Usually these scheduled scans are missed because the computer was turned off at the scheduled time.</span></span>|
|<span data-ttu-id="801ab-934">defenderDisableCatchupQuickScan</span><span class="sxs-lookup"><span data-stu-id="801ab-934">defenderDisableCatchupQuickScan</span></span>|<span data-ttu-id="801ab-935">Boolean</span><span class="sxs-lookup"><span data-stu-id="801ab-935">Boolean</span></span>|<span data-ttu-id="801ab-936">通过此策略设置，您可以配置计划快速扫描的追赶扫描。</span><span class="sxs-lookup"><span data-stu-id="801ab-936">This policy setting allows you to configure catch-up scans for scheduled quick scans.</span></span> <span data-ttu-id="801ab-937">追赶扫描是由于错过了定期计划的扫描而启动的扫描。</span><span class="sxs-lookup"><span data-stu-id="801ab-937">A catch-up scan is a scan that is initiated because a regularly scheduled scan was missed.</span></span> <span data-ttu-id="801ab-938">通常情况下，这些计划扫描会因计算机在计划时间关闭而丢失。</span><span class="sxs-lookup"><span data-stu-id="801ab-938">Usually these scheduled scans are missed because the computer was turned off at the scheduled time.</span></span>|
|<span data-ttu-id="801ab-939">defenderEnableLowCpuPriority</span><span class="sxs-lookup"><span data-stu-id="801ab-939">defenderEnableLowCpuPriority</span></span>|<span data-ttu-id="801ab-940">Boolean</span><span class="sxs-lookup"><span data-stu-id="801ab-940">Boolean</span></span>|<span data-ttu-id="801ab-941">通过此策略设置，您可以启用或禁用计划扫描的 CPU 低优先级。</span><span class="sxs-lookup"><span data-stu-id="801ab-941">This policy setting allows you to enable or disable low CPU priority for scheduled scans.</span></span>|
|<span data-ttu-id="801ab-942">defenderFileExtensionsToExclude</span><span class="sxs-lookup"><span data-stu-id="801ab-942">defenderFileExtensionsToExclude</span></span>|<span data-ttu-id="801ab-943">字符串集合</span><span class="sxs-lookup"><span data-stu-id="801ab-943">String collection</span></span>|<span data-ttu-id="801ab-944">要从扫描和实时保护中排除的文件扩展名。</span><span class="sxs-lookup"><span data-stu-id="801ab-944">File extensions to exclude from scans and real time protection.</span></span>|
|<span data-ttu-id="801ab-945">defenderFilesAndFoldersToExclude</span><span class="sxs-lookup"><span data-stu-id="801ab-945">defenderFilesAndFoldersToExclude</span></span>|<span data-ttu-id="801ab-946">字符串集合</span><span class="sxs-lookup"><span data-stu-id="801ab-946">String collection</span></span>|<span data-ttu-id="801ab-947">要从扫描和实时保护中排除的文件和文件夹。</span><span class="sxs-lookup"><span data-stu-id="801ab-947">Files and folder to exclude from scans and real time protection.</span></span>|
|<span data-ttu-id="801ab-948">defenderProcessesToExclude</span><span class="sxs-lookup"><span data-stu-id="801ab-948">defenderProcessesToExclude</span></span>|<span data-ttu-id="801ab-949">String 集合</span><span class="sxs-lookup"><span data-stu-id="801ab-949">String collection</span></span>|<span data-ttu-id="801ab-950">要从扫描和实时保护中排除的进程。</span><span class="sxs-lookup"><span data-stu-id="801ab-950">Processes to exclude from scans and real time protection.</span></span>|
|<span data-ttu-id="801ab-951">defenderPotentiallyUnwantedAppAction</span><span class="sxs-lookup"><span data-stu-id="801ab-951">defenderPotentiallyUnwantedAppAction</span></span>|[<span data-ttu-id="801ab-952">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="801ab-952">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="801ab-953">已添加到 Windows 10 版本 1607 中。</span><span class="sxs-lookup"><span data-stu-id="801ab-953">Added in Windows 10, version 1607.</span></span> <span data-ttu-id="801ab-954">指定对可能有害的应用程序（PUAs）的检测级别。</span><span class="sxs-lookup"><span data-stu-id="801ab-954">Specifies the level of detection for potentially unwanted applications (PUAs).</span></span> <span data-ttu-id="801ab-955">Windows Defender 会在下载可能不需要的软件或尝试在你的计算机上安装自己时向你发出警告。</span><span class="sxs-lookup"><span data-stu-id="801ab-955">Windows Defender alerts you when potentially unwanted software is being downloaded or attempts to install itself on your computer.</span></span> <span data-ttu-id="801ab-956">可取值为：`userDefined`、`enable`、`auditMode`。</span><span class="sxs-lookup"><span data-stu-id="801ab-956">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="801ab-957">defenderScanDirection</span><span class="sxs-lookup"><span data-stu-id="801ab-957">defenderScanDirection</span></span>|[<span data-ttu-id="801ab-958">defenderRealtimeScanDirection</span><span class="sxs-lookup"><span data-stu-id="801ab-958">defenderRealtimeScanDirection</span></span>](../resources/intune-deviceconfig-defenderrealtimescandirection.md)|<span data-ttu-id="801ab-959">控制应监视的文件集。</span><span class="sxs-lookup"><span data-stu-id="801ab-959">Controls which sets of files should be monitored.</span></span> <span data-ttu-id="801ab-960">可取值为：`monitorAllFiles`、`monitorIncomingFilesOnly`、`monitorOutgoingFilesOnly`。</span><span class="sxs-lookup"><span data-stu-id="801ab-960">Possible values are: `monitorAllFiles`, `monitorIncomingFilesOnly`, `monitorOutgoingFilesOnly`.</span></span>|
|<span data-ttu-id="801ab-961">defenderScanType</span><span class="sxs-lookup"><span data-stu-id="801ab-961">defenderScanType</span></span>|[<span data-ttu-id="801ab-962">defenderScanType</span><span class="sxs-lookup"><span data-stu-id="801ab-962">defenderScanType</span></span>](../resources/intune-deviceconfig-defenderscantype.md)|<span data-ttu-id="801ab-963">选择是否执行快速扫描或完全扫描。</span><span class="sxs-lookup"><span data-stu-id="801ab-963">Selects whether to perform a quick scan or full scan.</span></span> <span data-ttu-id="801ab-964">可取值为：`userDefined`、`disabled`、`quick`、`full`。</span><span class="sxs-lookup"><span data-stu-id="801ab-964">Possible values are: `userDefined`, `disabled`, `quick`, `full`.</span></span>|
|<span data-ttu-id="801ab-965">defenderScheduledQuickScanTime</span><span class="sxs-lookup"><span data-stu-id="801ab-965">defenderScheduledQuickScanTime</span></span>|<span data-ttu-id="801ab-966">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="801ab-966">TimeOfDay</span></span>|<span data-ttu-id="801ab-967">选择 Windows Defender 快速扫描应在一天的哪一时间运行。</span><span class="sxs-lookup"><span data-stu-id="801ab-967">Selects the time of day that the Windows Defender quick scan should run.</span></span> <span data-ttu-id="801ab-968">例如，值为 0 = 12：00AM，值为 60 = 1：00AM，值 120 = 2：00，等等，最高为 1380 = 11：00PM 的值。</span><span class="sxs-lookup"><span data-stu-id="801ab-968">For example, a value of 0=12:00AM, a value of 60=1:00AM, a value of 120=2:00, and so on, up to a value of 1380=11:00PM.</span></span> <span data-ttu-id="801ab-969">默认值为120</span><span class="sxs-lookup"><span data-stu-id="801ab-969">The default value is 120</span></span>|
|<span data-ttu-id="801ab-970">defenderScheduledScanDay</span><span class="sxs-lookup"><span data-stu-id="801ab-970">defenderScheduledScanDay</span></span>|[<span data-ttu-id="801ab-971">weeklySchedule</span><span class="sxs-lookup"><span data-stu-id="801ab-971">weeklySchedule</span></span>](../resources/intune-deviceconfig-weeklyschedule.md)|<span data-ttu-id="801ab-972">选择 Windows Defender 扫描应运行的日期。</span><span class="sxs-lookup"><span data-stu-id="801ab-972">Selects the day that the Windows Defender scan should run.</span></span> <span data-ttu-id="801ab-973">可取值为：`userDefined`、`everyday`、`sunday`、`monday`、`tuesday`、`wednesday`、`thursday`、`friday`、`saturday`、`noScheduledScan`。</span><span class="sxs-lookup"><span data-stu-id="801ab-973">Possible values are: `userDefined`, `everyday`, `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`, `noScheduledScan`.</span></span>|
|<span data-ttu-id="801ab-974">defenderScheduledScanTime</span><span class="sxs-lookup"><span data-stu-id="801ab-974">defenderScheduledScanTime</span></span>|<span data-ttu-id="801ab-975">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="801ab-975">TimeOfDay</span></span>|<span data-ttu-id="801ab-976">选择 Windows Defender 扫描应在一天的哪一时间运行。</span><span class="sxs-lookup"><span data-stu-id="801ab-976">Selects the time of day that the Windows Defender scan should run.</span></span>|
|<span data-ttu-id="801ab-977">defenderSignatureUpdateIntervalInHours</span><span class="sxs-lookup"><span data-stu-id="801ab-977">defenderSignatureUpdateIntervalInHours</span></span>|<span data-ttu-id="801ab-978">Int32</span><span class="sxs-lookup"><span data-stu-id="801ab-978">Int32</span></span>|<span data-ttu-id="801ab-979">指定将用于检查签名的间隔（以小时为单位），因此，不使用 ScheduleDay 和 ScheduleTime。将根据间隔设置检查是否有新的签名。</span><span class="sxs-lookup"><span data-stu-id="801ab-979">Specifies the interval (in hours) that will be used to check for signatures, so instead of using the ScheduleDay and ScheduleTime the check for new signatures will be set according to the interval.</span></span> <span data-ttu-id="801ab-980">有效值为 0 至 24</span><span class="sxs-lookup"><span data-stu-id="801ab-980">Valid values 0 to 24</span></span>|
|<span data-ttu-id="801ab-981">defenderSubmitSamplesConsentType</span><span class="sxs-lookup"><span data-stu-id="801ab-981">defenderSubmitSamplesConsentType</span></span>|[<span data-ttu-id="801ab-982">defenderSubmitSamplesConsentType</span><span class="sxs-lookup"><span data-stu-id="801ab-982">defenderSubmitSamplesConsentType</span></span>](../resources/intune-deviceconfig-defendersubmitsamplesconsenttype.md)|<span data-ttu-id="801ab-983">检查 Windows Defender 中的用户同意级别以发送数据。</span><span class="sxs-lookup"><span data-stu-id="801ab-983">Checks for the user consent level in Windows Defender to send data.</span></span> <span data-ttu-id="801ab-984">可取值为：`sendSafeSamplesAutomatically`、`alwaysPrompt`、`neverSend`、`sendAllSamplesAutomatically`。</span><span class="sxs-lookup"><span data-stu-id="801ab-984">Possible values are: `sendSafeSamplesAutomatically`, `alwaysPrompt`, `neverSend`, `sendAllSamplesAutomatically`.</span></span>|
|<span data-ttu-id="801ab-985">defenderDetectedMalwareActions</span><span class="sxs-lookup"><span data-stu-id="801ab-985">defenderDetectedMalwareActions</span></span>|[<span data-ttu-id="801ab-986">defenderDetectedMalwareActions</span><span class="sxs-lookup"><span data-stu-id="801ab-986">defenderDetectedMalwareActions</span></span>](../resources/intune-deviceconfig-defenderdetectedmalwareactions.md)|<span data-ttu-id="801ab-987">允许管理员指定任何有效的威胁严重级别和相应的默认操作 ID 进行。</span><span class="sxs-lookup"><span data-stu-id="801ab-987">Allows an administrator to specify any valid threat severity levels and the corresponding default action ID to take.</span></span>|



## <a name="response"></a><span data-ttu-id="801ab-988">响应</span><span class="sxs-lookup"><span data-stu-id="801ab-988">Response</span></span>
<span data-ttu-id="801ab-989">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="801ab-989">If successful, this method returns a `200 OK` response code and an updated [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="801ab-990">示例</span><span class="sxs-lookup"><span data-stu-id="801ab-990">Example</span></span>

### <a name="request"></a><span data-ttu-id="801ab-991">请求</span><span class="sxs-lookup"><span data-stu-id="801ab-991">Request</span></span>
<span data-ttu-id="801ab-992">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="801ab-992">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 31005

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

### <a name="response"></a><span data-ttu-id="801ab-993">响应</span><span class="sxs-lookup"><span data-stu-id="801ab-993">Response</span></span>
<span data-ttu-id="801ab-p225">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="801ab-p225">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 31177

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



