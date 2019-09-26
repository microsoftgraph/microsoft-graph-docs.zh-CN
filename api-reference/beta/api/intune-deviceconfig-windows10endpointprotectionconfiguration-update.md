---
title: 更新 windows10EndpointProtectionConfiguration
description: 更新 windows10EndpointProtectionConfiguration 对象的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 1306fbe6f661abe5189b70d19c3fe66a08956812
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/26/2019
ms.locfileid: "37182755"
---
# <a name="update-windows10endpointprotectionconfiguration"></a><span data-ttu-id="1e76e-103">更新 windows10EndpointProtectionConfiguration</span><span class="sxs-lookup"><span data-stu-id="1e76e-103">Update windows10EndpointProtectionConfiguration</span></span>

> <span data-ttu-id="1e76e-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="1e76e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1e76e-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="1e76e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1e76e-106">更新 [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="1e76e-106">Update the properties of a [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1e76e-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="1e76e-107">Prerequisites</span></span>
<span data-ttu-id="1e76e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="1e76e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1e76e-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="1e76e-110">Permission type</span></span>|<span data-ttu-id="1e76e-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="1e76e-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1e76e-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1e76e-112">Delegated (work or school account)</span></span>|<span data-ttu-id="1e76e-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1e76e-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="1e76e-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1e76e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1e76e-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="1e76e-115">Not supported.</span></span>|
|<span data-ttu-id="1e76e-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="1e76e-116">Application</span></span>|<span data-ttu-id="1e76e-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1e76e-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1e76e-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1e76e-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="1e76e-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="1e76e-119">Request headers</span></span>
|<span data-ttu-id="1e76e-120">标头</span><span class="sxs-lookup"><span data-stu-id="1e76e-120">Header</span></span>|<span data-ttu-id="1e76e-121">值</span><span class="sxs-lookup"><span data-stu-id="1e76e-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1e76e-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="1e76e-122">Authorization</span></span>|<span data-ttu-id="1e76e-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="1e76e-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1e76e-124">接受</span><span class="sxs-lookup"><span data-stu-id="1e76e-124">Accept</span></span>|<span data-ttu-id="1e76e-125">application/json</span><span class="sxs-lookup"><span data-stu-id="1e76e-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1e76e-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="1e76e-126">Request body</span></span>
<span data-ttu-id="1e76e-127">在请求正文中，提供 [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1e76e-127">In the request body, supply a JSON representation for the [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) object.</span></span>

<span data-ttu-id="1e76e-128">下表显示了创建 [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="1e76e-128">The following table shows the properties that are required when you create the [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md).</span></span>

|<span data-ttu-id="1e76e-129">属性</span><span class="sxs-lookup"><span data-stu-id="1e76e-129">Property</span></span>|<span data-ttu-id="1e76e-130">类型</span><span class="sxs-lookup"><span data-stu-id="1e76e-130">Type</span></span>|<span data-ttu-id="1e76e-131">说明</span><span class="sxs-lookup"><span data-stu-id="1e76e-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1e76e-132">id</span><span class="sxs-lookup"><span data-stu-id="1e76e-132">id</span></span>|<span data-ttu-id="1e76e-133">字符串</span><span class="sxs-lookup"><span data-stu-id="1e76e-133">String</span></span>|<span data-ttu-id="1e76e-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="1e76e-134">Key of the entity.</span></span> <span data-ttu-id="1e76e-135">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1e76e-135">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1e76e-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1e76e-136">lastModifiedDateTime</span></span>|<span data-ttu-id="1e76e-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1e76e-137">DateTimeOffset</span></span>|<span data-ttu-id="1e76e-138">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="1e76e-138">DateTime the object was last modified.</span></span> <span data-ttu-id="1e76e-139">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1e76e-139">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1e76e-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="1e76e-140">roleScopeTagIds</span></span>|<span data-ttu-id="1e76e-141">String collection</span><span class="sxs-lookup"><span data-stu-id="1e76e-141">String collection</span></span>|<span data-ttu-id="1e76e-142">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="1e76e-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="1e76e-143">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1e76e-143">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1e76e-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="1e76e-144">supportsScopeTags</span></span>|<span data-ttu-id="1e76e-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="1e76e-145">Boolean</span></span>|<span data-ttu-id="1e76e-146">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="1e76e-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="1e76e-147">如果此值为 false，则不允许分配给 ScopeTags 属性，并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="1e76e-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="1e76e-148">这适用于在 Silverlight 中创建的旧版策略，可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="1e76e-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="1e76e-149">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="1e76e-149">This property is read-only.</span></span> <span data-ttu-id="1e76e-150">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1e76e-150">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1e76e-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="1e76e-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="1e76e-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="1e76e-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="1e76e-153">适用于此策略的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="1e76e-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="1e76e-154">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1e76e-154">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1e76e-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="1e76e-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="1e76e-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="1e76e-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="1e76e-157">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="1e76e-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="1e76e-158">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1e76e-158">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1e76e-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="1e76e-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="1e76e-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="1e76e-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="1e76e-161">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="1e76e-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="1e76e-162">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1e76e-162">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1e76e-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1e76e-163">createdDateTime</span></span>|<span data-ttu-id="1e76e-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1e76e-164">DateTimeOffset</span></span>|<span data-ttu-id="1e76e-165">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="1e76e-165">DateTime the object was created.</span></span> <span data-ttu-id="1e76e-166">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1e76e-166">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1e76e-167">说明</span><span class="sxs-lookup"><span data-stu-id="1e76e-167">description</span></span>|<span data-ttu-id="1e76e-168">String</span><span class="sxs-lookup"><span data-stu-id="1e76e-168">String</span></span>|<span data-ttu-id="1e76e-169">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="1e76e-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="1e76e-170">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1e76e-170">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1e76e-171">displayName</span><span class="sxs-lookup"><span data-stu-id="1e76e-171">displayName</span></span>|<span data-ttu-id="1e76e-172">String</span><span class="sxs-lookup"><span data-stu-id="1e76e-172">String</span></span>|<span data-ttu-id="1e76e-173">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="1e76e-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="1e76e-174">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1e76e-174">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1e76e-175">version</span><span class="sxs-lookup"><span data-stu-id="1e76e-175">version</span></span>|<span data-ttu-id="1e76e-176">Int32</span><span class="sxs-lookup"><span data-stu-id="1e76e-176">Int32</span></span>|<span data-ttu-id="1e76e-177">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="1e76e-177">Version of the device configuration.</span></span> <span data-ttu-id="1e76e-178">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1e76e-178">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1e76e-179">dmaGuardDeviceEnumerationPolicy</span><span class="sxs-lookup"><span data-stu-id="1e76e-179">dmaGuardDeviceEnumerationPolicy</span></span>|[<span data-ttu-id="1e76e-180">dmaGuardDeviceEnumerationPolicyType</span><span class="sxs-lookup"><span data-stu-id="1e76e-180">dmaGuardDeviceEnumerationPolicyType</span></span>](../resources/intune-deviceconfig-dmaguarddeviceenumerationpolicytype.md)|<span data-ttu-id="1e76e-181">此策略旨在提供针对支持外部 DMA 的设备的额外安全性。</span><span class="sxs-lookup"><span data-stu-id="1e76e-181">This policy is intended to provide additional security against external DMA capable devices.</span></span> <span data-ttu-id="1e76e-182">通过它，可以更好地控制支持外部 DMA 的设备与 DMA 重新映射/设备内存隔离和沙盒不兼容的枚举。</span><span class="sxs-lookup"><span data-stu-id="1e76e-182">It allows for more control over the enumeration of external DMA capable devices incompatible with DMA Remapping/device memory isolation and sandboxing.</span></span> <span data-ttu-id="1e76e-183">仅当系统固件支持和启用内核 DMA 保护时，此策略才会生效。</span><span class="sxs-lookup"><span data-stu-id="1e76e-183">This policy only takes effect when Kernel DMA Protection is supported and enabled by the system firmware.</span></span> <span data-ttu-id="1e76e-184">内核 DMA 保护是一项平台功能，不能通过策略或最终用户进行控制。</span><span class="sxs-lookup"><span data-stu-id="1e76e-184">Kernel DMA Protection is a platform feature that cannot be controlled via policy or by end user.</span></span> <span data-ttu-id="1e76e-185">在制造时，系统必须支持它。</span><span class="sxs-lookup"><span data-stu-id="1e76e-185">It has to be supported by the system at the time of manufacturing.</span></span> <span data-ttu-id="1e76e-186">若要检查系统是否支持内核 DMA 保护，请在 MSINFO32 的摘要页中检查 "内核 DMA 保护" 字段。</span><span class="sxs-lookup"><span data-stu-id="1e76e-186">To check if the system supports Kernel DMA Protection, please check the Kernel DMA Protection field in the Summary page of MSINFO32.exe.</span></span> <span data-ttu-id="1e76e-187">可取值为：`deviceDefault`、`blockAll`、`allowAll`。</span><span class="sxs-lookup"><span data-stu-id="1e76e-187">Possible values are: `deviceDefault`, `blockAll`, `allowAll`.</span></span>|
|<span data-ttu-id="1e76e-188">firewallRules</span><span class="sxs-lookup"><span data-stu-id="1e76e-188">firewallRules</span></span>|<span data-ttu-id="1e76e-189">[windowsFirewallRule](../resources/intune-deviceconfig-windowsfirewallrule.md)集合</span><span class="sxs-lookup"><span data-stu-id="1e76e-189">[windowsFirewallRule](../resources/intune-deviceconfig-windowsfirewallrule.md) collection</span></span>|<span data-ttu-id="1e76e-190">配置防火墙规则设置。</span><span class="sxs-lookup"><span data-stu-id="1e76e-190">Configures the firewall rule settings.</span></span> <span data-ttu-id="1e76e-191">此集合最多可包含150个元素。</span><span class="sxs-lookup"><span data-stu-id="1e76e-191">This collection can contain a maximum of 150 elements.</span></span>|
|<span data-ttu-id="1e76e-192">userRightsAccessCredentialManagerAsTrustedCaller</span><span class="sxs-lookup"><span data-stu-id="1e76e-192">userRightsAccessCredentialManagerAsTrustedCaller</span></span>|[<span data-ttu-id="1e76e-193">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="1e76e-193">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="1e76e-194">此用户权限由凭据管理器在备份/还原过程中使用。</span><span class="sxs-lookup"><span data-stu-id="1e76e-194">This user right is used by Credential Manager during Backup/Restore.</span></span> <span data-ttu-id="1e76e-195">如果为其他实体提供此权限，则用户保存的凭据可能会受到威胁。</span><span class="sxs-lookup"><span data-stu-id="1e76e-195">Users' saved credentials might be compromised if this privilege is given to other entities.</span></span> <span data-ttu-id="1e76e-196">仅支持 NotConfigured 和允许的状态</span><span class="sxs-lookup"><span data-stu-id="1e76e-196">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="1e76e-197">userRightsAllowAccessFromNetwork</span><span class="sxs-lookup"><span data-stu-id="1e76e-197">userRightsAllowAccessFromNetwork</span></span>|[<span data-ttu-id="1e76e-198">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="1e76e-198">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="1e76e-199">此用户权限确定允许哪些用户和组通过网络连接到计算机。</span><span class="sxs-lookup"><span data-stu-id="1e76e-199">This user right determines which users and groups are allowed to connect to the computer over the network.</span></span> <span data-ttu-id="1e76e-200">支持的状态为 "允许"。</span><span class="sxs-lookup"><span data-stu-id="1e76e-200">State Allowed is supported.</span></span>|
|<span data-ttu-id="1e76e-201">userRightsBlockAccessFromNetwork</span><span class="sxs-lookup"><span data-stu-id="1e76e-201">userRightsBlockAccessFromNetwork</span></span>|[<span data-ttu-id="1e76e-202">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="1e76e-202">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="1e76e-203">此用户权限决定了阻止哪些用户和组通过网络连接到计算机。</span><span class="sxs-lookup"><span data-stu-id="1e76e-203">This user right determines which users and groups are block from connecting to the computer over the network.</span></span> <span data-ttu-id="1e76e-204">支持状态块。</span><span class="sxs-lookup"><span data-stu-id="1e76e-204">State Block is supported.</span></span>|
|<span data-ttu-id="1e76e-205">userRightsActAsPartOfTheOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="1e76e-205">userRightsActAsPartOfTheOperatingSystem</span></span>|[<span data-ttu-id="1e76e-206">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="1e76e-206">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="1e76e-207">此用户权限允许进程在不进行身份验证的情况下模拟任何用户。</span><span class="sxs-lookup"><span data-stu-id="1e76e-207">This user right allows a process to impersonate any user without authentication.</span></span> <span data-ttu-id="1e76e-208">因此，该过程可以获得与该用户相同的本地资源的访问权限。</span><span class="sxs-lookup"><span data-stu-id="1e76e-208">The process can therefore gain access to the same local resources as that user.</span></span> <span data-ttu-id="1e76e-209">仅支持 NotConfigured 和允许的状态</span><span class="sxs-lookup"><span data-stu-id="1e76e-209">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="1e76e-210">userRightsLocalLogOn</span><span class="sxs-lookup"><span data-stu-id="1e76e-210">userRightsLocalLogOn</span></span>|[<span data-ttu-id="1e76e-211">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="1e76e-211">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="1e76e-212">此用户权限确定哪些用户可以登录到计算机。</span><span class="sxs-lookup"><span data-stu-id="1e76e-212">This user right determines which users can log on to the computer.</span></span> <span data-ttu-id="1e76e-213">支持的状态 NotConfigured （允许）</span><span class="sxs-lookup"><span data-stu-id="1e76e-213">States NotConfigured, Allowed are supported</span></span> |
|<span data-ttu-id="1e76e-214">userRightsDenyLocalLogOn</span><span class="sxs-lookup"><span data-stu-id="1e76e-214">userRightsDenyLocalLogOn</span></span>|[<span data-ttu-id="1e76e-215">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="1e76e-215">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="1e76e-216">此用户权限确定哪些用户无法登录到计算机。</span><span class="sxs-lookup"><span data-stu-id="1e76e-216">This user right determines which users cannot log on to the computer.</span></span> <span data-ttu-id="1e76e-217">状态 NotConfigured，受阻止</span><span class="sxs-lookup"><span data-stu-id="1e76e-217">States NotConfigured, Blocked are supported</span></span> |
|<span data-ttu-id="1e76e-218">userRightsBackupData</span><span class="sxs-lookup"><span data-stu-id="1e76e-218">userRightsBackupData</span></span>|[<span data-ttu-id="1e76e-219">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="1e76e-219">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="1e76e-220">此用户权限确定在备份文件和目录时，哪些用户可以绕过文件、目录、注册表和其他持久对象权限。</span><span class="sxs-lookup"><span data-stu-id="1e76e-220">This user right determines which users can bypass file, directory, registry, and other persistent objects permissions when backing up files and directories.</span></span> <span data-ttu-id="1e76e-221">仅支持 NotConfigured 和允许的状态</span><span class="sxs-lookup"><span data-stu-id="1e76e-221">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="1e76e-222">userRightsChangeSystemTime</span><span class="sxs-lookup"><span data-stu-id="1e76e-222">userRightsChangeSystemTime</span></span>|[<span data-ttu-id="1e76e-223">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="1e76e-223">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="1e76e-224">此用户权限确定哪些用户和组可以更改计算机内部时钟上的时间和日期。</span><span class="sxs-lookup"><span data-stu-id="1e76e-224">This user right determines which users and groups can change the time and date on the internal clock of the computer.</span></span> <span data-ttu-id="1e76e-225">仅支持 NotConfigured 和允许的状态</span><span class="sxs-lookup"><span data-stu-id="1e76e-225">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="1e76e-226">userRightsCreateGlobalObjects</span><span class="sxs-lookup"><span data-stu-id="1e76e-226">userRightsCreateGlobalObjects</span></span>|[<span data-ttu-id="1e76e-227">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="1e76e-227">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="1e76e-228">此安全设置确定用户是否可以创建可用于所有会话的全局对象。</span><span class="sxs-lookup"><span data-stu-id="1e76e-228">This security setting determines whether users can create global objects that are available to all sessions.</span></span> <span data-ttu-id="1e76e-229">可以创建全局对象的用户可能会影响在其他用户的会话下运行的进程，这可能导致应用程序故障或数据损坏。</span><span class="sxs-lookup"><span data-stu-id="1e76e-229">Users who can create global objects could affect processes that run under other users' sessions, which could lead to application failure or data corruption.</span></span> <span data-ttu-id="1e76e-230">仅支持 NotConfigured 和允许的状态</span><span class="sxs-lookup"><span data-stu-id="1e76e-230">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="1e76e-231">userRightsCreatePageFile</span><span class="sxs-lookup"><span data-stu-id="1e76e-231">userRightsCreatePageFile</span></span>|[<span data-ttu-id="1e76e-232">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="1e76e-232">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="1e76e-233">此用户权限确定哪些用户和组可以调用内部 API 来创建和更改页面文件的大小。</span><span class="sxs-lookup"><span data-stu-id="1e76e-233">This user right determines which users and groups can call an internal API to create and change the size of a page file.</span></span> <span data-ttu-id="1e76e-234">仅支持 NotConfigured 和允许的状态</span><span class="sxs-lookup"><span data-stu-id="1e76e-234">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="1e76e-235">userRightsCreatePermanentSharedObjects</span><span class="sxs-lookup"><span data-stu-id="1e76e-235">userRightsCreatePermanentSharedObjects</span></span>|[<span data-ttu-id="1e76e-236">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="1e76e-236">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="1e76e-237">此用户权限决定了进程可以使用哪些帐户使用对象管理器创建目录对象。</span><span class="sxs-lookup"><span data-stu-id="1e76e-237">This user right determines which accounts can be used by processes to create a directory object using the object manager.</span></span> <span data-ttu-id="1e76e-238">仅支持 NotConfigured 和允许的状态</span><span class="sxs-lookup"><span data-stu-id="1e76e-238">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="1e76e-239">userRightsCreateSymbolicLinks</span><span class="sxs-lookup"><span data-stu-id="1e76e-239">userRightsCreateSymbolicLinks</span></span>|[<span data-ttu-id="1e76e-240">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="1e76e-240">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="1e76e-241">此用户权限确定用户是否可以从其登录到的计算机创建符号链接。</span><span class="sxs-lookup"><span data-stu-id="1e76e-241">This user right determines if the user can create a symbolic link from the computer to which they are logged on.</span></span> <span data-ttu-id="1e76e-242">仅支持 NotConfigured 和允许的状态</span><span class="sxs-lookup"><span data-stu-id="1e76e-242">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="1e76e-243">userRightsCreateToken</span><span class="sxs-lookup"><span data-stu-id="1e76e-243">userRightsCreateToken</span></span>|[<span data-ttu-id="1e76e-244">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="1e76e-244">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="1e76e-245">此用户权限确定进程在使用内部 API 创建访问令牌时，可以使用哪些用户/组来创建令牌，然后可以使用这些用户/组来获取对任何本地资源的访问权限。</span><span class="sxs-lookup"><span data-stu-id="1e76e-245">This user right determines which users/groups can be used by processes to create a token that can then be used to get access to any local resources when the process uses an internal API to create an access token.</span></span> <span data-ttu-id="1e76e-246">仅支持 NotConfigured 和允许的状态</span><span class="sxs-lookup"><span data-stu-id="1e76e-246">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="1e76e-247">userRightsDebugPrograms</span><span class="sxs-lookup"><span data-stu-id="1e76e-247">userRightsDebugPrograms</span></span>|[<span data-ttu-id="1e76e-248">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="1e76e-248">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="1e76e-249">此用户权限确定哪些用户可以将调试程序附加到任何进程或内核。</span><span class="sxs-lookup"><span data-stu-id="1e76e-249">This user right determines which users can attach a debugger to any process or to the kernel.</span></span> <span data-ttu-id="1e76e-250">仅支持 NotConfigured 和允许的状态</span><span class="sxs-lookup"><span data-stu-id="1e76e-250">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="1e76e-251">userRightsRemoteDesktopServicesLogOn</span><span class="sxs-lookup"><span data-stu-id="1e76e-251">userRightsRemoteDesktopServicesLogOn</span></span>|[<span data-ttu-id="1e76e-252">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="1e76e-252">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="1e76e-253">此用户权限确定禁止哪些用户和组作为远程桌面服务客户端进行登录。</span><span class="sxs-lookup"><span data-stu-id="1e76e-253">This user right determines which users and groups are prohibited from logging on as a Remote Desktop Services client.</span></span> <span data-ttu-id="1e76e-254">仅支持状态 NotConfigured 和阻止</span><span class="sxs-lookup"><span data-stu-id="1e76e-254">Only states NotConfigured and Blocked are supported</span></span>|
|<span data-ttu-id="1e76e-255">userRightsDelegation</span><span class="sxs-lookup"><span data-stu-id="1e76e-255">userRightsDelegation</span></span>|[<span data-ttu-id="1e76e-256">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="1e76e-256">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="1e76e-257">此用户权限确定哪些用户可以在用户或计算机对象上设置受信任委派设置。</span><span class="sxs-lookup"><span data-stu-id="1e76e-257">This user right determines which users can set the Trusted for Delegation setting on a user or computer object.</span></span> <span data-ttu-id="1e76e-258">仅支持 NotConfigured 和允许的状态。</span><span class="sxs-lookup"><span data-stu-id="1e76e-258">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="1e76e-259">userRightsGenerateSecurityAudits</span><span class="sxs-lookup"><span data-stu-id="1e76e-259">userRightsGenerateSecurityAudits</span></span>|[<span data-ttu-id="1e76e-260">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="1e76e-260">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="1e76e-261">此用户权限确定进程可使用哪些帐户向安全日志中添加条目。</span><span class="sxs-lookup"><span data-stu-id="1e76e-261">This user right determines which accounts can be used by a process to add entries to the security log.</span></span> <span data-ttu-id="1e76e-262">安全日志用于跟踪未经授权的系统访问。</span><span class="sxs-lookup"><span data-stu-id="1e76e-262">The security log is used to trace unauthorized system access.</span></span>  <span data-ttu-id="1e76e-263">仅支持 NotConfigured 和允许的状态。</span><span class="sxs-lookup"><span data-stu-id="1e76e-263">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="1e76e-264">userRightsImpersonateClient</span><span class="sxs-lookup"><span data-stu-id="1e76e-264">userRightsImpersonateClient</span></span>|[<span data-ttu-id="1e76e-265">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="1e76e-265">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="1e76e-266">将此用户权限分配给用户将允许代表该用户运行的程序模拟客户端。</span><span class="sxs-lookup"><span data-stu-id="1e76e-266">Assigning this user right to a user allows programs running on behalf of that user to impersonate a client.</span></span> <span data-ttu-id="1e76e-267">如果此类型的模拟要求此用户权限，则可以防止未经授权的用户说服客户端连接到已创建的服务，然后模拟该客户端，这样可以将未经授权的用户的权限提升到管理级别或系统级别。</span><span class="sxs-lookup"><span data-stu-id="1e76e-267">Requiring this user right for this kind of impersonation prevents an unauthorized user from convincing a client to connect to a service that they have created and then impersonating that client, which can elevate the unauthorized user's permissions to administrative or system levels.</span></span> <span data-ttu-id="1e76e-268">仅支持 NotConfigured 和允许的状态。</span><span class="sxs-lookup"><span data-stu-id="1e76e-268">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="1e76e-269">userRightsIncreaseSchedulingPriority</span><span class="sxs-lookup"><span data-stu-id="1e76e-269">userRightsIncreaseSchedulingPriority</span></span>|[<span data-ttu-id="1e76e-270">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="1e76e-270">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="1e76e-271">此用户权限确定哪些帐户可以使用具有对另一进程的 Write 属性访问权限的进程，以增加分配给其他进程的执行优先级。</span><span class="sxs-lookup"><span data-stu-id="1e76e-271">This user right determines which accounts can use a process with Write Property access to another process to increase the execution priority assigned to the other process.</span></span> <span data-ttu-id="1e76e-272">仅支持 NotConfigured 和允许的状态。</span><span class="sxs-lookup"><span data-stu-id="1e76e-272">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="1e76e-273">userRightsLoadUnloadDrivers</span><span class="sxs-lookup"><span data-stu-id="1e76e-273">userRightsLoadUnloadDrivers</span></span>|[<span data-ttu-id="1e76e-274">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="1e76e-274">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="1e76e-275">此用户权限确定哪些用户可以在内核模式下将设备驱动程序或其他代码动态加载和卸载。</span><span class="sxs-lookup"><span data-stu-id="1e76e-275">This user right determines which users can dynamically load and unload device drivers or other code in to kernel mode.</span></span> <span data-ttu-id="1e76e-276">仅支持 NotConfigured 和允许的状态。</span><span class="sxs-lookup"><span data-stu-id="1e76e-276">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="1e76e-277">userRightsLockMemory</span><span class="sxs-lookup"><span data-stu-id="1e76e-277">userRightsLockMemory</span></span>|[<span data-ttu-id="1e76e-278">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="1e76e-278">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="1e76e-279">此用户权限确定哪些帐户可以使用进程将数据保存在物理内存中，这会阻止系统将数据分页到磁盘上的虚拟内存中。</span><span class="sxs-lookup"><span data-stu-id="1e76e-279">This user right determines which accounts can use a process to keep data in physical memory, which prevents the system from paging the data to virtual memory on disk.</span></span> <span data-ttu-id="1e76e-280">仅支持 NotConfigured 和允许的状态。</span><span class="sxs-lookup"><span data-stu-id="1e76e-280">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="1e76e-281">userRightsManageAuditingAndSecurityLogs</span><span class="sxs-lookup"><span data-stu-id="1e76e-281">userRightsManageAuditingAndSecurityLogs</span></span>|[<span data-ttu-id="1e76e-282">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="1e76e-282">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="1e76e-283">此用户权限确定哪些用户可以为各个资源（如文件、Active Directory 对象和注册表项）指定对象访问审核选项。</span><span class="sxs-lookup"><span data-stu-id="1e76e-283">This user right determines which users can specify object access auditing options for individual resources, such as files, Active Directory objects, and registry keys.</span></span> <span data-ttu-id="1e76e-284">仅支持 NotConfigured 和允许的状态。</span><span class="sxs-lookup"><span data-stu-id="1e76e-284">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="1e76e-285">userRightsManageVolumes</span><span class="sxs-lookup"><span data-stu-id="1e76e-285">userRightsManageVolumes</span></span>|[<span data-ttu-id="1e76e-286">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="1e76e-286">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="1e76e-287">此用户权限确定哪些用户和组可以在某个卷（如远程碎片整理）上运行维护任务。</span><span class="sxs-lookup"><span data-stu-id="1e76e-287">This user right determines which users and groups can run maintenance tasks on a volume, such as remote defragmentation.</span></span> <span data-ttu-id="1e76e-288">仅支持 NotConfigured 和允许的状态。</span><span class="sxs-lookup"><span data-stu-id="1e76e-288">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="1e76e-289">userRightsModifyFirmwareEnvironment</span><span class="sxs-lookup"><span data-stu-id="1e76e-289">userRightsModifyFirmwareEnvironment</span></span>|[<span data-ttu-id="1e76e-290">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="1e76e-290">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="1e76e-291">此用户权限决定了可以修改固件环境值的用户。</span><span class="sxs-lookup"><span data-stu-id="1e76e-291">This user right determines who can modify firmware environment values.</span></span> <span data-ttu-id="1e76e-292">仅支持 NotConfigured 和允许的状态。</span><span class="sxs-lookup"><span data-stu-id="1e76e-292">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="1e76e-293">userRightsModifyObjectLabels</span><span class="sxs-lookup"><span data-stu-id="1e76e-293">userRightsModifyObjectLabels</span></span>|[<span data-ttu-id="1e76e-294">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="1e76e-294">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="1e76e-295">此用户权限确定哪些用户帐户可以修改对象的完整性标签，例如，文件、注册表项或其他用户所拥有的进程。</span><span class="sxs-lookup"><span data-stu-id="1e76e-295">This user right determines which user accounts can modify the integrity label of objects, such as files, registry keys, or processes owned by other users.</span></span> <span data-ttu-id="1e76e-296">仅支持 NotConfigured 和允许的状态。</span><span class="sxs-lookup"><span data-stu-id="1e76e-296">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="1e76e-297">userRightsProfileSingleProcess</span><span class="sxs-lookup"><span data-stu-id="1e76e-297">userRightsProfileSingleProcess</span></span>|[<span data-ttu-id="1e76e-298">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="1e76e-298">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="1e76e-299">此用户权限确定哪些用户可以使用性能监视工具来监视系统进程的性能。</span><span class="sxs-lookup"><span data-stu-id="1e76e-299">This user right determines which users can use performance monitoring tools to monitor the performance of system processes.</span></span> <span data-ttu-id="1e76e-300">仅支持 NotConfigured 和允许的状态。</span><span class="sxs-lookup"><span data-stu-id="1e76e-300">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="1e76e-301">userRightsRemoteShutdown</span><span class="sxs-lookup"><span data-stu-id="1e76e-301">userRightsRemoteShutdown</span></span>|[<span data-ttu-id="1e76e-302">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="1e76e-302">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="1e76e-303">此用户权限确定允许哪些用户从网络上的远程位置关闭计算机。</span><span class="sxs-lookup"><span data-stu-id="1e76e-303">This user right determines which users are allowed to shut down a computer from a remote location on the network.</span></span> <span data-ttu-id="1e76e-304">误用此用户权限可能会导致拒绝服务。</span><span class="sxs-lookup"><span data-stu-id="1e76e-304">Misuse of this user right can result in a denial of service.</span></span> <span data-ttu-id="1e76e-305">仅支持 NotConfigured 和允许的状态。</span><span class="sxs-lookup"><span data-stu-id="1e76e-305">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="1e76e-306">userRightsRestoreData</span><span class="sxs-lookup"><span data-stu-id="1e76e-306">userRightsRestoreData</span></span>|[<span data-ttu-id="1e76e-307">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="1e76e-307">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="1e76e-308">此用户权限确定在还原备份的文件和目录时，哪些用户可以绕过文件、目录、注册表和其他持久对象权限，并确定哪些用户可以将任何有效的安全主体设置为对象的所有者。</span><span class="sxs-lookup"><span data-stu-id="1e76e-308">This user right determines which users can bypass file, directory, registry, and other persistent objects permissions when restoring backed up files and directories, and determines which users can set any valid security principal as the owner of an object.</span></span> <span data-ttu-id="1e76e-309">仅支持 NotConfigured 和允许的状态。</span><span class="sxs-lookup"><span data-stu-id="1e76e-309">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="1e76e-310">userRightsTakeOwnership</span><span class="sxs-lookup"><span data-stu-id="1e76e-310">userRightsTakeOwnership</span></span>|[<span data-ttu-id="1e76e-311">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="1e76e-311">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="1e76e-312">此用户权限确定哪些用户可以获得系统中任何安全对象的所有权，包括 Active Directory 对象、文件和文件夹、打印机、注册表项、进程和线程。</span><span class="sxs-lookup"><span data-stu-id="1e76e-312">This user right determines which users can take ownership of any securable object in the system, including Active Directory objects, files and folders, printers, registry keys, processes, and threads.</span></span> <span data-ttu-id="1e76e-313">仅支持 NotConfigured 和允许的状态。</span><span class="sxs-lookup"><span data-stu-id="1e76e-313">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="1e76e-314">xboxServicesEnableXboxGameSaveTask</span><span class="sxs-lookup"><span data-stu-id="1e76e-314">xboxServicesEnableXboxGameSaveTask</span></span>|<span data-ttu-id="1e76e-315">Boolean</span><span class="sxs-lookup"><span data-stu-id="1e76e-315">Boolean</span></span>|<span data-ttu-id="1e76e-316">此设置确定是否启用了 xbox 游戏保存（1）或禁用（0）。</span><span class="sxs-lookup"><span data-stu-id="1e76e-316">This setting determines whether xbox game save is enabled (1) or disabled (0).</span></span>|
|<span data-ttu-id="1e76e-317">xboxServicesAccessoryManagementServiceStartupMode</span><span class="sxs-lookup"><span data-stu-id="1e76e-317">xboxServicesAccessoryManagementServiceStartupMode</span></span>|[<span data-ttu-id="1e76e-318">serviceStartType</span><span class="sxs-lookup"><span data-stu-id="1e76e-318">serviceStartType</span></span>](../resources/intune-deviceconfig-servicestarttype.md)|<span data-ttu-id="1e76e-319">此设置确定附件管理服务的启动类型是 "自动" （2）、"手动" （3）、"已禁用" （4）。</span><span class="sxs-lookup"><span data-stu-id="1e76e-319">This setting determines whether the Accessory management service's start type is Automatic(2), Manual(3), Disabled(4).</span></span> <span data-ttu-id="1e76e-320">默认：手动。</span><span class="sxs-lookup"><span data-stu-id="1e76e-320">Default: Manual.</span></span> <span data-ttu-id="1e76e-321">可取值为：`manual`、`automatic`、`disabled`。</span><span class="sxs-lookup"><span data-stu-id="1e76e-321">Possible values are: `manual`, `automatic`, `disabled`.</span></span>|
|<span data-ttu-id="1e76e-322">xboxServicesLiveAuthManagerServiceStartupMode</span><span class="sxs-lookup"><span data-stu-id="1e76e-322">xboxServicesLiveAuthManagerServiceStartupMode</span></span>|[<span data-ttu-id="1e76e-323">serviceStartType</span><span class="sxs-lookup"><span data-stu-id="1e76e-323">serviceStartType</span></span>](../resources/intune-deviceconfig-servicestarttype.md)|<span data-ttu-id="1e76e-324">此设置确定 Live Auth Manager 服务的启动类型是否为自动（2）、手动（3）、已禁用（4）。</span><span class="sxs-lookup"><span data-stu-id="1e76e-324">This setting determines whether Live Auth Manager service's start type is Automatic(2), Manual(3), Disabled(4).</span></span> <span data-ttu-id="1e76e-325">默认：手动。</span><span class="sxs-lookup"><span data-stu-id="1e76e-325">Default: Manual.</span></span> <span data-ttu-id="1e76e-326">可取值为：`manual`、`automatic`、`disabled`。</span><span class="sxs-lookup"><span data-stu-id="1e76e-326">Possible values are: `manual`, `automatic`, `disabled`.</span></span>|
|<span data-ttu-id="1e76e-327">xboxServicesLiveGameSaveServiceStartupMode</span><span class="sxs-lookup"><span data-stu-id="1e76e-327">xboxServicesLiveGameSaveServiceStartupMode</span></span>|[<span data-ttu-id="1e76e-328">serviceStartType</span><span class="sxs-lookup"><span data-stu-id="1e76e-328">serviceStartType</span></span>](../resources/intune-deviceconfig-servicestarttype.md)|<span data-ttu-id="1e76e-329">此设置确定实时游戏是否保存服务的启动类型为自动（2）、手动（3）、已禁用（4）。</span><span class="sxs-lookup"><span data-stu-id="1e76e-329">This setting determines whether Live Game save service's start type is Automatic(2), Manual(3), Disabled(4).</span></span> <span data-ttu-id="1e76e-330">默认：手动。</span><span class="sxs-lookup"><span data-stu-id="1e76e-330">Default: Manual.</span></span> <span data-ttu-id="1e76e-331">可取值为：`manual`、`automatic`、`disabled`。</span><span class="sxs-lookup"><span data-stu-id="1e76e-331">Possible values are: `manual`, `automatic`, `disabled`.</span></span>|
|<span data-ttu-id="1e76e-332">xboxServicesLiveNetworkingServiceStartupMode</span><span class="sxs-lookup"><span data-stu-id="1e76e-332">xboxServicesLiveNetworkingServiceStartupMode</span></span>|[<span data-ttu-id="1e76e-333">serviceStartType</span><span class="sxs-lookup"><span data-stu-id="1e76e-333">serviceStartType</span></span>](../resources/intune-deviceconfig-servicestarttype.md)|<span data-ttu-id="1e76e-334">此设置确定网络服务的启动类型是否为自动（2）、手动（3）、已禁用（4）。</span><span class="sxs-lookup"><span data-stu-id="1e76e-334">This setting determines whether Networking service's start type is Automatic(2), Manual(3), Disabled(4).</span></span> <span data-ttu-id="1e76e-335">默认：手动。</span><span class="sxs-lookup"><span data-stu-id="1e76e-335">Default: Manual.</span></span> <span data-ttu-id="1e76e-336">可取值为：`manual`、`automatic`、`disabled`。</span><span class="sxs-lookup"><span data-stu-id="1e76e-336">Possible values are: `manual`, `automatic`, `disabled`.</span></span>|
|<span data-ttu-id="1e76e-337">localSecurityOptionsBlockMicrosoftAccounts</span><span class="sxs-lookup"><span data-stu-id="1e76e-337">localSecurityOptionsBlockMicrosoftAccounts</span></span>|<span data-ttu-id="1e76e-338">Boolean</span><span class="sxs-lookup"><span data-stu-id="1e76e-338">Boolean</span></span>|<span data-ttu-id="1e76e-339">阻止用户向此计算机添加新的 Microsoft 帐户。</span><span class="sxs-lookup"><span data-stu-id="1e76e-339">Prevent users from adding new Microsoft accounts to this computer.</span></span>|
|<span data-ttu-id="1e76e-340">localSecurityOptionsBlockRemoteLogonWithBlankPassword</span><span class="sxs-lookup"><span data-stu-id="1e76e-340">localSecurityOptionsBlockRemoteLogonWithBlankPassword</span></span>|<span data-ttu-id="1e76e-341">Boolean</span><span class="sxs-lookup"><span data-stu-id="1e76e-341">Boolean</span></span>|<span data-ttu-id="1e76e-342">启用不受密码保护的本地帐户从物理设备以外的位置进行登录。默认值为已启用</span><span class="sxs-lookup"><span data-stu-id="1e76e-342">Enable Local accounts that are not password protected to log on from locations other than the physical device.Default is enabled</span></span>|
|<span data-ttu-id="1e76e-343">localSecurityOptionsDisableAdministratorAccount</span><span class="sxs-lookup"><span data-stu-id="1e76e-343">localSecurityOptionsDisableAdministratorAccount</span></span>|<span data-ttu-id="1e76e-344">Boolean</span><span class="sxs-lookup"><span data-stu-id="1e76e-344">Boolean</span></span>|<span data-ttu-id="1e76e-345">确定是否启用或禁用本地管理员帐户。</span><span class="sxs-lookup"><span data-stu-id="1e76e-345">Determines whether the Local Administrator account is enabled or disabled.</span></span>|
|<span data-ttu-id="1e76e-346">localSecurityOptionsAdministratorAccountName</span><span class="sxs-lookup"><span data-stu-id="1e76e-346">localSecurityOptionsAdministratorAccountName</span></span>|<span data-ttu-id="1e76e-347">String</span><span class="sxs-lookup"><span data-stu-id="1e76e-347">String</span></span>|<span data-ttu-id="1e76e-348">定义要与帐户 "管理员" 的安全标识符（SID）相关联的不同帐户名称。</span><span class="sxs-lookup"><span data-stu-id="1e76e-348">Define a different account name to be associated with the security identifier (SID) for the account “Administrator”.</span></span>|
|<span data-ttu-id="1e76e-349">localSecurityOptionsDisableGuestAccount</span><span class="sxs-lookup"><span data-stu-id="1e76e-349">localSecurityOptionsDisableGuestAccount</span></span>|<span data-ttu-id="1e76e-350">Boolean</span><span class="sxs-lookup"><span data-stu-id="1e76e-350">Boolean</span></span>|<span data-ttu-id="1e76e-351">确定来宾帐户是否已启用或已禁用。</span><span class="sxs-lookup"><span data-stu-id="1e76e-351">Determines if the Guest account is enabled or disabled.</span></span>|
|<span data-ttu-id="1e76e-352">localSecurityOptionsGuestAccountName</span><span class="sxs-lookup"><span data-stu-id="1e76e-352">localSecurityOptionsGuestAccountName</span></span>|<span data-ttu-id="1e76e-353">String</span><span class="sxs-lookup"><span data-stu-id="1e76e-353">String</span></span>|<span data-ttu-id="1e76e-354">定义要与帐户 "来宾" 的安全标识符（SID）相关联的不同帐户名称。</span><span class="sxs-lookup"><span data-stu-id="1e76e-354">Define a different account name to be associated with the security identifier (SID) for the account “Guest”.</span></span>|
|<span data-ttu-id="1e76e-355">localSecurityOptionsAllowUndockWithoutHavingToLogon</span><span class="sxs-lookup"><span data-stu-id="1e76e-355">localSecurityOptionsAllowUndockWithoutHavingToLogon</span></span>|<span data-ttu-id="1e76e-356">Boolean</span><span class="sxs-lookup"><span data-stu-id="1e76e-356">Boolean</span></span>|<span data-ttu-id="1e76e-357">阻止便携式计算机在无需登录的情况下被移除。</span><span class="sxs-lookup"><span data-stu-id="1e76e-357">Prevent a portable computer from being undocked without having to log in.</span></span>|
|<span data-ttu-id="1e76e-358">localSecurityOptionsBlockUsersInstallingPrinterDrivers</span><span class="sxs-lookup"><span data-stu-id="1e76e-358">localSecurityOptionsBlockUsersInstallingPrinterDrivers</span></span>|<span data-ttu-id="1e76e-359">Boolean</span><span class="sxs-lookup"><span data-stu-id="1e76e-359">Boolean</span></span>|<span data-ttu-id="1e76e-360">仅在将打印机驱动程序连接到共享打印机时，才将其限制为仅供管理员安装。</span><span class="sxs-lookup"><span data-stu-id="1e76e-360">Restrict installing printer drivers as part of connecting to a shared printer to admins only.</span></span>|
|<span data-ttu-id="1e76e-361">localSecurityOptionsBlockRemoteOpticalDriveAccess</span><span class="sxs-lookup"><span data-stu-id="1e76e-361">localSecurityOptionsBlockRemoteOpticalDriveAccess</span></span>|<span data-ttu-id="1e76e-362">Boolean</span><span class="sxs-lookup"><span data-stu-id="1e76e-362">Boolean</span></span>|<span data-ttu-id="1e76e-363">如果启用此设置，则仅允许交互式登录用户访问 CD-ROM 媒体。</span><span class="sxs-lookup"><span data-stu-id="1e76e-363">Enabling this settings allows only interactively logged on user to access CD-ROM media.</span></span>|
|<span data-ttu-id="1e76e-364">localSecurityOptionsFormatAndEjectOfRemovableMediaAllowedUser</span><span class="sxs-lookup"><span data-stu-id="1e76e-364">localSecurityOptionsFormatAndEjectOfRemovableMediaAllowedUser</span></span>|[<span data-ttu-id="1e76e-365">localSecurityOptionsFormatAndEjectOfRemovableMediaAllowedUserType</span><span class="sxs-lookup"><span data-stu-id="1e76e-365">localSecurityOptionsFormatAndEjectOfRemovableMediaAllowedUserType</span></span>](../resources/intune-deviceconfig-localsecurityoptionsformatandejectofremovablemediaallowedusertype.md)|<span data-ttu-id="1e76e-366">定义允许格式化和弹出可移动 NTFS 媒体的权限。</span><span class="sxs-lookup"><span data-stu-id="1e76e-366">Define who is allowed to format and eject removable NTFS media.</span></span> <span data-ttu-id="1e76e-367">可取值为：`notConfigured`、`administrators`、`administratorsAndPowerUsers`、`administratorsAndInteractiveUsers`。</span><span class="sxs-lookup"><span data-stu-id="1e76e-367">Possible values are: `notConfigured`, `administrators`, `administratorsAndPowerUsers`, `administratorsAndInteractiveUsers`.</span></span>|
|<span data-ttu-id="1e76e-368">localSecurityOptionsMachineInactivityLimit</span><span class="sxs-lookup"><span data-stu-id="1e76e-368">localSecurityOptionsMachineInactivityLimit</span></span>|<span data-ttu-id="1e76e-369">Int32</span><span class="sxs-lookup"><span data-stu-id="1e76e-369">Int32</span></span>|<span data-ttu-id="1e76e-370">在屏幕保护程序运行之前，定义交互式桌面登录屏幕上不活动的最长分钟数。</span><span class="sxs-lookup"><span data-stu-id="1e76e-370">Define maximum minutes of inactivity on the interactive desktop’s login screen until the screen saver runs.</span></span> <span data-ttu-id="1e76e-371">有效值为0至9999</span><span class="sxs-lookup"><span data-stu-id="1e76e-371">Valid values 0 to 9999</span></span>|
|<span data-ttu-id="1e76e-372">localSecurityOptionsMachineInactivityLimitInMinutes</span><span class="sxs-lookup"><span data-stu-id="1e76e-372">localSecurityOptionsMachineInactivityLimitInMinutes</span></span>|<span data-ttu-id="1e76e-373">Int32</span><span class="sxs-lookup"><span data-stu-id="1e76e-373">Int32</span></span>|<span data-ttu-id="1e76e-374">在屏幕保护程序运行之前，定义交互式桌面登录屏幕上不活动的最长分钟数。</span><span class="sxs-lookup"><span data-stu-id="1e76e-374">Define maximum minutes of inactivity on the interactive desktop’s login screen until the screen saver runs.</span></span> <span data-ttu-id="1e76e-375">有效值为0至9999</span><span class="sxs-lookup"><span data-stu-id="1e76e-375">Valid values 0 to 9999</span></span>|
|<span data-ttu-id="1e76e-376">localSecurityOptionsDoNotRequireCtrlAltDel</span><span class="sxs-lookup"><span data-stu-id="1e76e-376">localSecurityOptionsDoNotRequireCtrlAltDel</span></span>|<span data-ttu-id="1e76e-377">Boolean</span><span class="sxs-lookup"><span data-stu-id="1e76e-377">Boolean</span></span>|<span data-ttu-id="1e76e-378">要求用户在登录前按 CTRL + ALT + DEL。</span><span class="sxs-lookup"><span data-stu-id="1e76e-378">Require CTRL+ALT+DEL to be pressed before a user can log on.</span></span>|
|<span data-ttu-id="1e76e-379">localSecurityOptionsHideLastSignedInUser</span><span class="sxs-lookup"><span data-stu-id="1e76e-379">localSecurityOptionsHideLastSignedInUser</span></span>|<span data-ttu-id="1e76e-380">Boolean</span><span class="sxs-lookup"><span data-stu-id="1e76e-380">Boolean</span></span>|<span data-ttu-id="1e76e-381">不显示上次在此设备上登录的用户的用户名。</span><span class="sxs-lookup"><span data-stu-id="1e76e-381">Do not display the username of the last person who signed in on this device.</span></span>|
|<span data-ttu-id="1e76e-382">localSecurityOptionsHideUsernameAtSignIn</span><span class="sxs-lookup"><span data-stu-id="1e76e-382">localSecurityOptionsHideUsernameAtSignIn</span></span>|<span data-ttu-id="1e76e-383">Boolean</span><span class="sxs-lookup"><span data-stu-id="1e76e-383">Boolean</span></span>|<span data-ttu-id="1e76e-384">在输入凭据后以及显示设备桌面之前，请勿显示登录此设备的人员的用户名。</span><span class="sxs-lookup"><span data-stu-id="1e76e-384">Do not display the username of the person signing in to this device after credentials are entered and before the device’s desktop is shown.</span></span>|
|<span data-ttu-id="1e76e-385">localSecurityOptionsLogOnMessageTitle</span><span class="sxs-lookup"><span data-stu-id="1e76e-385">localSecurityOptionsLogOnMessageTitle</span></span>|<span data-ttu-id="1e76e-386">String</span><span class="sxs-lookup"><span data-stu-id="1e76e-386">String</span></span>|<span data-ttu-id="1e76e-387">为尝试登录的用户设置消息标题。</span><span class="sxs-lookup"><span data-stu-id="1e76e-387">Set message title for users attempting to log in.</span></span>|
|<span data-ttu-id="1e76e-388">localSecurityOptionsLogOnMessageText</span><span class="sxs-lookup"><span data-stu-id="1e76e-388">localSecurityOptionsLogOnMessageText</span></span>|<span data-ttu-id="1e76e-389">String</span><span class="sxs-lookup"><span data-stu-id="1e76e-389">String</span></span>|<span data-ttu-id="1e76e-390">为尝试登录的用户设置消息文本。</span><span class="sxs-lookup"><span data-stu-id="1e76e-390">Set message text for users attempting to log in.</span></span>|
|<span data-ttu-id="1e76e-391">localSecurityOptionsAllowPKU2UAuthenticationRequests</span><span class="sxs-lookup"><span data-stu-id="1e76e-391">localSecurityOptionsAllowPKU2UAuthenticationRequests</span></span>|<span data-ttu-id="1e76e-392">Boolean</span><span class="sxs-lookup"><span data-stu-id="1e76e-392">Boolean</span></span>|<span data-ttu-id="1e76e-393">阻止 PKU2U 对此设备的身份验证请求，以使用联机标识。</span><span class="sxs-lookup"><span data-stu-id="1e76e-393">Block PKU2U authentication requests to this device to use online identities.</span></span>|
|<span data-ttu-id="1e76e-394">localSecurityOptionsAllowRemoteCallsToSecurityAccountsManagerHelperBool</span><span class="sxs-lookup"><span data-stu-id="1e76e-394">localSecurityOptionsAllowRemoteCallsToSecurityAccountsManagerHelperBool</span></span>|<span data-ttu-id="1e76e-395">Boolean</span><span class="sxs-lookup"><span data-stu-id="1e76e-395">Boolean</span></span>|<span data-ttu-id="1e76e-396">LocalSecurityOptionsAllowRemoteCallsToSecurityAccountsManager 实体的 UI 帮助程序布尔值</span><span class="sxs-lookup"><span data-stu-id="1e76e-396">UI helper boolean for LocalSecurityOptionsAllowRemoteCallsToSecurityAccountsManager entity</span></span>|
|<span data-ttu-id="1e76e-397">localSecurityOptionsAllowRemoteCallsToSecurityAccountsManager</span><span class="sxs-lookup"><span data-stu-id="1e76e-397">localSecurityOptionsAllowRemoteCallsToSecurityAccountsManager</span></span>|<span data-ttu-id="1e76e-398">String</span><span class="sxs-lookup"><span data-stu-id="1e76e-398">String</span></span>|<span data-ttu-id="1e76e-399">编辑默认的安全描述符定义语言字符串，以允许或拒绝用户和组对 SAM 进行远程调用。</span><span class="sxs-lookup"><span data-stu-id="1e76e-399">Edit the default Security Descriptor Definition Language string to allow or deny users and groups to make remote calls to the SAM.</span></span>|
|<span data-ttu-id="1e76e-400">localSecurityOptionsMinimumSessionSecurityForNtlmSspBasedClients</span><span class="sxs-lookup"><span data-stu-id="1e76e-400">localSecurityOptionsMinimumSessionSecurityForNtlmSspBasedClients</span></span>|[<span data-ttu-id="1e76e-401">localSecurityOptionsMinimumSessionSecurity</span><span class="sxs-lookup"><span data-stu-id="1e76e-401">localSecurityOptionsMinimumSessionSecurity</span></span>](../resources/intune-deviceconfig-localsecurityoptionsminimumsessionsecurity.md)|<span data-ttu-id="1e76e-402">此安全设置允许客户端要求协商128位加密和/或 NTLMv2 会话安全性。</span><span class="sxs-lookup"><span data-stu-id="1e76e-402">This security setting allows a client to require the negotiation of 128-bit encryption and/or NTLMv2 session security.</span></span> <span data-ttu-id="1e76e-403">可取值为：`none`、`requireNtmlV2SessionSecurity`、`require128BitEncryption`、`ntlmV2And128BitEncryption`。</span><span class="sxs-lookup"><span data-stu-id="1e76e-403">Possible values are: `none`, `requireNtmlV2SessionSecurity`, `require128BitEncryption`, `ntlmV2And128BitEncryption`.</span></span>|
|<span data-ttu-id="1e76e-404">localSecurityOptionsMinimumSessionSecurityForNtlmSspBasedServers</span><span class="sxs-lookup"><span data-stu-id="1e76e-404">localSecurityOptionsMinimumSessionSecurityForNtlmSspBasedServers</span></span>|[<span data-ttu-id="1e76e-405">localSecurityOptionsMinimumSessionSecurity</span><span class="sxs-lookup"><span data-stu-id="1e76e-405">localSecurityOptionsMinimumSessionSecurity</span></span>](../resources/intune-deviceconfig-localsecurityoptionsminimumsessionsecurity.md)|<span data-ttu-id="1e76e-406">此安全设置允许服务器要求协商128位加密和/或 NTLMv2 会话安全性。</span><span class="sxs-lookup"><span data-stu-id="1e76e-406">This security setting allows a server to require the negotiation of 128-bit encryption and/or NTLMv2 session security.</span></span> <span data-ttu-id="1e76e-407">可取值为：`none`、`requireNtmlV2SessionSecurity`、`require128BitEncryption`、`ntlmV2And128BitEncryption`。</span><span class="sxs-lookup"><span data-stu-id="1e76e-407">Possible values are: `none`, `requireNtmlV2SessionSecurity`, `require128BitEncryption`, `ntlmV2And128BitEncryption`.</span></span>|
|<span data-ttu-id="1e76e-408">lanManagerAuthenticationLevel</span><span class="sxs-lookup"><span data-stu-id="1e76e-408">lanManagerAuthenticationLevel</span></span>|[<span data-ttu-id="1e76e-409">lanManagerAuthenticationLevel</span><span class="sxs-lookup"><span data-stu-id="1e76e-409">lanManagerAuthenticationLevel</span></span>](../resources/intune-deviceconfig-lanmanagerauthenticationlevel.md)|<span data-ttu-id="1e76e-410">此安全设置确定用于网络登录的质询/响应身份验证协议。</span><span class="sxs-lookup"><span data-stu-id="1e76e-410">This security setting determines which challenge/response authentication protocol is used for network logons.</span></span> <span data-ttu-id="1e76e-411">可取值为：`lmAndNltm`、`lmNtlmAndNtlmV2`、`lmAndNtlmOnly`、`lmAndNtlmV2`、`lmNtlmV2AndNotLm`、`lmNtlmV2AndNotLmOrNtm`。</span><span class="sxs-lookup"><span data-stu-id="1e76e-411">Possible values are: `lmAndNltm`, `lmNtlmAndNtlmV2`, `lmAndNtlmOnly`, `lmAndNtlmV2`, `lmNtlmV2AndNotLm`, `lmNtlmV2AndNotLmOrNtm`.</span></span>|
|<span data-ttu-id="1e76e-412">lanManagerWorkstationDisableInsecureGuestLogons</span><span class="sxs-lookup"><span data-stu-id="1e76e-412">lanManagerWorkstationDisableInsecureGuestLogons</span></span>|<span data-ttu-id="1e76e-413">Boolean</span><span class="sxs-lookup"><span data-stu-id="1e76e-413">Boolean</span></span>|<span data-ttu-id="1e76e-414">如果启用，SMB 客户端将允许不安全的来宾登录。</span><span class="sxs-lookup"><span data-stu-id="1e76e-414">If enabled,the SMB client will allow insecure guest logons.</span></span> <span data-ttu-id="1e76e-415">如果未配置，SMB 客户端将拒绝不安全的来宾登录。</span><span class="sxs-lookup"><span data-stu-id="1e76e-415">If not configured, the SMB client will reject insecure guest logons.</span></span>|
|<span data-ttu-id="1e76e-416">localSecurityOptionsClearVirtualMemoryPageFile</span><span class="sxs-lookup"><span data-stu-id="1e76e-416">localSecurityOptionsClearVirtualMemoryPageFile</span></span>|<span data-ttu-id="1e76e-417">Boolean</span><span class="sxs-lookup"><span data-stu-id="1e76e-417">Boolean</span></span>|<span data-ttu-id="1e76e-418">此安全设置确定在关闭系统时是否清除虚拟内存页面文件。</span><span class="sxs-lookup"><span data-stu-id="1e76e-418">This security setting determines whether the virtual memory pagefile is cleared when the system is shut down.</span></span>|
|<span data-ttu-id="1e76e-419">localSecurityOptionsAllowSystemToBeShutDownWithoutHavingToLogOn</span><span class="sxs-lookup"><span data-stu-id="1e76e-419">localSecurityOptionsAllowSystemToBeShutDownWithoutHavingToLogOn</span></span>|<span data-ttu-id="1e76e-420">Boolean</span><span class="sxs-lookup"><span data-stu-id="1e76e-420">Boolean</span></span>|<span data-ttu-id="1e76e-421">此安全设置确定是否可以在不登录 Windows 的情况下关闭计算机。</span><span class="sxs-lookup"><span data-stu-id="1e76e-421">This security setting determines whether a computer can be shut down without having to log on to Windows.</span></span>|
|<span data-ttu-id="1e76e-422">localSecurityOptionsAllowUIAccessApplicationElevation</span><span class="sxs-lookup"><span data-stu-id="1e76e-422">localSecurityOptionsAllowUIAccessApplicationElevation</span></span>|<span data-ttu-id="1e76e-423">Boolean</span><span class="sxs-lookup"><span data-stu-id="1e76e-423">Boolean</span></span>|<span data-ttu-id="1e76e-424">允许 UIAccess 应用在不使用安全桌面的情况下提示提升。</span><span class="sxs-lookup"><span data-stu-id="1e76e-424">Allow UIAccess apps to prompt for elevation without using the secure desktop.</span></span>|
|<span data-ttu-id="1e76e-425">localSecurityOptionsVirtualizeFileAndRegistryWriteFailuresToPerUserLocations</span><span class="sxs-lookup"><span data-stu-id="1e76e-425">localSecurityOptionsVirtualizeFileAndRegistryWriteFailuresToPerUserLocations</span></span>|<span data-ttu-id="1e76e-426">Boolean</span><span class="sxs-lookup"><span data-stu-id="1e76e-426">Boolean</span></span>|<span data-ttu-id="1e76e-427">将文件和注册表写入失败虚拟化到每个用户位置</span><span class="sxs-lookup"><span data-stu-id="1e76e-427">Virtualize file and registry write failures to per user locations</span></span>|
|<span data-ttu-id="1e76e-428">localSecurityOptionsOnlyElevateSignedExecutables</span><span class="sxs-lookup"><span data-stu-id="1e76e-428">localSecurityOptionsOnlyElevateSignedExecutables</span></span>|<span data-ttu-id="1e76e-429">Boolean</span><span class="sxs-lookup"><span data-stu-id="1e76e-429">Boolean</span></span>|<span data-ttu-id="1e76e-430">对给定的可执行文件强制执行 PKI 证书路径验证，然后再允许运行该文件。</span><span class="sxs-lookup"><span data-stu-id="1e76e-430">Enforce PKI certification path validation for a given executable file before it is permitted to run.</span></span>|
|<span data-ttu-id="1e76e-431">localSecurityOptionsAdministratorElevationPromptBehavior</span><span class="sxs-lookup"><span data-stu-id="1e76e-431">localSecurityOptionsAdministratorElevationPromptBehavior</span></span>|[<span data-ttu-id="1e76e-432">localSecurityOptionsAdministratorElevationPromptBehaviorType</span><span class="sxs-lookup"><span data-stu-id="1e76e-432">localSecurityOptionsAdministratorElevationPromptBehaviorType</span></span>](../resources/intune-deviceconfig-localsecurityoptionsadministratorelevationpromptbehaviortype.md)|<span data-ttu-id="1e76e-433">在管理员审批模式中定义管理员的提升提示行为。</span><span class="sxs-lookup"><span data-stu-id="1e76e-433">Define the behavior of the elevation prompt for admins in Admin Approval Mode.</span></span> <span data-ttu-id="1e76e-434">可取值为：`notConfigured`、`elevateWithoutPrompting`、`promptForCredentialsOnTheSecureDesktop`、`promptForConsentOnTheSecureDesktop`、`promptForCredentials`、`promptForConsent` 或 `promptForConsentForNonWindowsBinaries`。</span><span class="sxs-lookup"><span data-stu-id="1e76e-434">Possible values are: `notConfigured`, `elevateWithoutPrompting`, `promptForCredentialsOnTheSecureDesktop`, `promptForConsentOnTheSecureDesktop`, `promptForCredentials`, `promptForConsent`, `promptForConsentForNonWindowsBinaries`.</span></span>|
|<span data-ttu-id="1e76e-435">localSecurityOptionsStandardUserElevationPromptBehavior</span><span class="sxs-lookup"><span data-stu-id="1e76e-435">localSecurityOptionsStandardUserElevationPromptBehavior</span></span>|[<span data-ttu-id="1e76e-436">localSecurityOptionsStandardUserElevationPromptBehaviorType</span><span class="sxs-lookup"><span data-stu-id="1e76e-436">localSecurityOptionsStandardUserElevationPromptBehaviorType</span></span>](../resources/intune-deviceconfig-localsecurityoptionsstandarduserelevationpromptbehaviortype.md)|<span data-ttu-id="1e76e-437">定义标准用户的提升提示行为。</span><span class="sxs-lookup"><span data-stu-id="1e76e-437">Define the behavior of the elevation prompt for standard users.</span></span> <span data-ttu-id="1e76e-438">可取值为：`notConfigured`、`automaticallyDenyElevationRequests`、`promptForCredentialsOnTheSecureDesktop`、`promptForCredentials`。</span><span class="sxs-lookup"><span data-stu-id="1e76e-438">Possible values are: `notConfigured`, `automaticallyDenyElevationRequests`, `promptForCredentialsOnTheSecureDesktop`, `promptForCredentials`.</span></span>|
|<span data-ttu-id="1e76e-439">localSecurityOptionsSwitchToSecureDesktopWhenPromptingForElevation</span><span class="sxs-lookup"><span data-stu-id="1e76e-439">localSecurityOptionsSwitchToSecureDesktopWhenPromptingForElevation</span></span>|<span data-ttu-id="1e76e-440">Boolean</span><span class="sxs-lookup"><span data-stu-id="1e76e-440">Boolean</span></span>|<span data-ttu-id="1e76e-441">启用所有提升请求以转到交互式用户的桌面，而不是安全桌面。</span><span class="sxs-lookup"><span data-stu-id="1e76e-441">Enable all elevation requests to go to the interactive user's desktop rather than the secure desktop.</span></span> <span data-ttu-id="1e76e-442">使用管理员和标准用户的提示行为策略设置。</span><span class="sxs-lookup"><span data-stu-id="1e76e-442">Prompt behavior policy settings for admins and standard users are used.</span></span>|
|<span data-ttu-id="1e76e-443">localSecurityOptionsDetectApplicationInstallationsAndPromptForElevation</span><span class="sxs-lookup"><span data-stu-id="1e76e-443">localSecurityOptionsDetectApplicationInstallationsAndPromptForElevation</span></span>|<span data-ttu-id="1e76e-444">Boolean</span><span class="sxs-lookup"><span data-stu-id="1e76e-444">Boolean</span></span>|<span data-ttu-id="1e76e-445">需要提升权限的应用程序安装将提示管理凭据。默认值为已启用</span><span class="sxs-lookup"><span data-stu-id="1e76e-445">App installations requiring elevated privileges will prompt for admin credentials.Default is enabled</span></span>|
|<span data-ttu-id="1e76e-446">localSecurityOptionsAllowUIAccessApplicationsForSecureLocations</span><span class="sxs-lookup"><span data-stu-id="1e76e-446">localSecurityOptionsAllowUIAccessApplicationsForSecureLocations</span></span>|<span data-ttu-id="1e76e-447">Boolean</span><span class="sxs-lookup"><span data-stu-id="1e76e-447">Boolean</span></span>|<span data-ttu-id="1e76e-448">允许 UIAccess 应用在不使用安全桌面的情况下提示提升。默认值为已启用</span><span class="sxs-lookup"><span data-stu-id="1e76e-448">Allow UIAccess apps to prompt for elevation without using the secure desktop.Default is enabled</span></span>|
|<span data-ttu-id="1e76e-449">localSecurityOptionsUseAdminApprovalMode</span><span class="sxs-lookup"><span data-stu-id="1e76e-449">localSecurityOptionsUseAdminApprovalMode</span></span>|<span data-ttu-id="1e76e-450">Boolean</span><span class="sxs-lookup"><span data-stu-id="1e76e-450">Boolean</span></span>|<span data-ttu-id="1e76e-451">定义内置管理员帐户是使用管理员审批模式，还是运行所有具有完全管理员权限的应用程序。默认值为已启用</span><span class="sxs-lookup"><span data-stu-id="1e76e-451">Defines whether the built-in admin account uses Admin Approval Mode or runs all apps with full admin privileges.Default is enabled</span></span>|
|<span data-ttu-id="1e76e-452">localSecurityOptionsUseAdminApprovalModeForAdministrators</span><span class="sxs-lookup"><span data-stu-id="1e76e-452">localSecurityOptionsUseAdminApprovalModeForAdministrators</span></span>|<span data-ttu-id="1e76e-453">Boolean</span><span class="sxs-lookup"><span data-stu-id="1e76e-453">Boolean</span></span>|<span data-ttu-id="1e76e-454">定义是否启用管理员批准模式和所有 UAC 策略设置，默认为启用</span><span class="sxs-lookup"><span data-stu-id="1e76e-454">Define whether Admin Approval Mode and all UAC policy settings are enabled, default is enabled</span></span>|
|<span data-ttu-id="1e76e-455">localSecurityOptionsInformationShownOnLockScreen</span><span class="sxs-lookup"><span data-stu-id="1e76e-455">localSecurityOptionsInformationShownOnLockScreen</span></span>|[<span data-ttu-id="1e76e-456">localSecurityOptionsInformationShownOnLockScreenType</span><span class="sxs-lookup"><span data-stu-id="1e76e-456">localSecurityOptionsInformationShownOnLockScreenType</span></span>](../resources/intune-deviceconfig-localsecurityoptionsinformationshownonlockscreentype.md)|<span data-ttu-id="1e76e-457">配置在会话锁定时显示的用户信息。</span><span class="sxs-lookup"><span data-stu-id="1e76e-457">Configure the user information that is displayed when the session is locked.</span></span> <span data-ttu-id="1e76e-458">如果未配置，则显示用户显示名称、域和用户名。</span><span class="sxs-lookup"><span data-stu-id="1e76e-458">If not configured, user display name, domain and username are shown.</span></span> <span data-ttu-id="1e76e-459">可取值为：`notConfigured`、`userDisplayNameDomainUser`、`userDisplayNameOnly`、`doNotDisplayUser`。</span><span class="sxs-lookup"><span data-stu-id="1e76e-459">Possible values are: `notConfigured`, `userDisplayNameDomainUser`, `userDisplayNameOnly`, `doNotDisplayUser`.</span></span>|
|<span data-ttu-id="1e76e-460">localSecurityOptionsInformationDisplayedOnLockScreen</span><span class="sxs-lookup"><span data-stu-id="1e76e-460">localSecurityOptionsInformationDisplayedOnLockScreen</span></span>|[<span data-ttu-id="1e76e-461">localSecurityOptionsInformationDisplayedOnLockScreenType</span><span class="sxs-lookup"><span data-stu-id="1e76e-461">localSecurityOptionsInformationDisplayedOnLockScreenType</span></span>](../resources/intune-deviceconfig-localsecurityoptionsinformationdisplayedonlockscreentype.md)|<span data-ttu-id="1e76e-462">配置在会话锁定时显示的用户信息。</span><span class="sxs-lookup"><span data-stu-id="1e76e-462">Configure the user information that is displayed when the session is locked.</span></span> <span data-ttu-id="1e76e-463">如果未配置，则显示用户显示名称、域和用户名。</span><span class="sxs-lookup"><span data-stu-id="1e76e-463">If not configured, user display name, domain and username are shown.</span></span> <span data-ttu-id="1e76e-464">可取值为：`notConfigured`、`administrators`、`administratorsAndPowerUsers`、`administratorsAndInteractiveUsers`。</span><span class="sxs-lookup"><span data-stu-id="1e76e-464">Possible values are: `notConfigured`, `administrators`, `administratorsAndPowerUsers`, `administratorsAndInteractiveUsers`.</span></span>|
|<span data-ttu-id="1e76e-465">localSecurityOptionsDisableClientDigitallySignCommunicationsIfServerAgrees</span><span class="sxs-lookup"><span data-stu-id="1e76e-465">localSecurityOptionsDisableClientDigitallySignCommunicationsIfServerAgrees</span></span>|<span data-ttu-id="1e76e-466">Boolean</span><span class="sxs-lookup"><span data-stu-id="1e76e-466">Boolean</span></span>|<span data-ttu-id="1e76e-467">此安全设置确定 SMB 客户端是否尝试协商 SMB 数据包签名。</span><span class="sxs-lookup"><span data-stu-id="1e76e-467">This security setting determines whether the SMB client attempts to negotiate SMB packet signing.</span></span>|
|<span data-ttu-id="1e76e-468">localSecurityOptionsClientDigitallySignCommunicationsAlways</span><span class="sxs-lookup"><span data-stu-id="1e76e-468">localSecurityOptionsClientDigitallySignCommunicationsAlways</span></span>|<span data-ttu-id="1e76e-469">Boolean</span><span class="sxs-lookup"><span data-stu-id="1e76e-469">Boolean</span></span>|<span data-ttu-id="1e76e-470">此安全设置确定 SMB 客户端组件是否需要数据包签名。</span><span class="sxs-lookup"><span data-stu-id="1e76e-470">This security setting determines whether packet signing is required by the SMB client component.</span></span>|
|<span data-ttu-id="1e76e-471">localSecurityOptionsClientSendUnencryptedPasswordToThirdPartySMBServers</span><span class="sxs-lookup"><span data-stu-id="1e76e-471">localSecurityOptionsClientSendUnencryptedPasswordToThirdPartySMBServers</span></span>|<span data-ttu-id="1e76e-472">Boolean</span><span class="sxs-lookup"><span data-stu-id="1e76e-472">Boolean</span></span>|<span data-ttu-id="1e76e-473">如果启用此安全设置，则允许服务器消息块（SMB）重定向程序将纯文本密码发送到在身份验证过程中不支持密码加密的非 Microsoft SMB 服务器。</span><span class="sxs-lookup"><span data-stu-id="1e76e-473">If this security setting is enabled, the Server Message Block (SMB) redirector is allowed to send plaintext passwords to non-Microsoft SMB servers that do not support password encryption during authentication.</span></span>|
|<span data-ttu-id="1e76e-474">localSecurityOptionsDisableServerDigitallySignCommunicationsAlways</span><span class="sxs-lookup"><span data-stu-id="1e76e-474">localSecurityOptionsDisableServerDigitallySignCommunicationsAlways</span></span>|<span data-ttu-id="1e76e-475">Boolean</span><span class="sxs-lookup"><span data-stu-id="1e76e-475">Boolean</span></span>|<span data-ttu-id="1e76e-476">此安全设置确定 SMB 服务器组件是否需要数据包签名。</span><span class="sxs-lookup"><span data-stu-id="1e76e-476">This security setting determines whether packet signing is required by the SMB server component.</span></span>|
|<span data-ttu-id="1e76e-477">localSecurityOptionsDisableServerDigitallySignCommunicationsIfClientAgrees</span><span class="sxs-lookup"><span data-stu-id="1e76e-477">localSecurityOptionsDisableServerDigitallySignCommunicationsIfClientAgrees</span></span>|<span data-ttu-id="1e76e-478">Boolean</span><span class="sxs-lookup"><span data-stu-id="1e76e-478">Boolean</span></span>|<span data-ttu-id="1e76e-479">此安全设置确定 SMB 服务器是否将 SMB 数据包签名与请求的客户端协商。</span><span class="sxs-lookup"><span data-stu-id="1e76e-479">This security setting determines whether the SMB server will negotiate SMB packet signing with clients that request it.</span></span>|
|<span data-ttu-id="1e76e-480">localSecurityOptionsRestrictAnonymousAccessToNamedPipesAndShares</span><span class="sxs-lookup"><span data-stu-id="1e76e-480">localSecurityOptionsRestrictAnonymousAccessToNamedPipesAndShares</span></span>|<span data-ttu-id="1e76e-481">Boolean</span><span class="sxs-lookup"><span data-stu-id="1e76e-481">Boolean</span></span>|<span data-ttu-id="1e76e-482">默认情况下，此安全设置限制可匿名访问且可匿名访问的共享的命名管道设置对共享和管道的匿名访问权限</span><span class="sxs-lookup"><span data-stu-id="1e76e-482">By default, this security setting restricts anonymous access to shares and pipes to the settings for named pipes that can be accessed anonymously and Shares that can be accessed anonymously</span></span>|
|<span data-ttu-id="1e76e-483">localSecurityOptionsDoNotAllowAnonymousEnumerationOfSAMAccounts</span><span class="sxs-lookup"><span data-stu-id="1e76e-483">localSecurityOptionsDoNotAllowAnonymousEnumerationOfSAMAccounts</span></span>|<span data-ttu-id="1e76e-484">Boolean</span><span class="sxs-lookup"><span data-stu-id="1e76e-484">Boolean</span></span>|<span data-ttu-id="1e76e-485">此安全设置确定将向计算机的匿名连接授予的其他权限。</span><span class="sxs-lookup"><span data-stu-id="1e76e-485">This security setting determines what additional permissions will be granted for anonymous connections to the computer.</span></span>|
|<span data-ttu-id="1e76e-486">localSecurityOptionsAllowAnonymousEnumerationOfSAMAccountsAndShares</span><span class="sxs-lookup"><span data-stu-id="1e76e-486">localSecurityOptionsAllowAnonymousEnumerationOfSAMAccountsAndShares</span></span>|<span data-ttu-id="1e76e-487">Boolean</span><span class="sxs-lookup"><span data-stu-id="1e76e-487">Boolean</span></span>|<span data-ttu-id="1e76e-488">此安全设置确定是否允许匿名用户执行某些活动，如枚举域帐户和网络共享的名称。</span><span class="sxs-lookup"><span data-stu-id="1e76e-488">This security setting determines whether to allows anonymous users to perform certain activities, such as enumerating the names of domain accounts and network shares.</span></span>|
|<span data-ttu-id="1e76e-489">localSecurityOptionsDoNotStoreLANManagerHashValueOnNextPasswordChange</span><span class="sxs-lookup"><span data-stu-id="1e76e-489">localSecurityOptionsDoNotStoreLANManagerHashValueOnNextPasswordChange</span></span>|<span data-ttu-id="1e76e-490">Boolean</span><span class="sxs-lookup"><span data-stu-id="1e76e-490">Boolean</span></span>|<span data-ttu-id="1e76e-491">此安全设置确定在下一次更改密码时，是否存储新密码的 LAN Manager （LM）哈希值。</span><span class="sxs-lookup"><span data-stu-id="1e76e-491">This security setting determines if, at the next password change, the LAN Manager (LM) hash value for the new password is stored.</span></span> <span data-ttu-id="1e76e-492">默认情况下不存储它。</span><span class="sxs-lookup"><span data-stu-id="1e76e-492">It’s not stored by default.</span></span>|
|<span data-ttu-id="1e76e-493">localSecurityOptionsSmartCardRemovalBehavior</span><span class="sxs-lookup"><span data-stu-id="1e76e-493">localSecurityOptionsSmartCardRemovalBehavior</span></span>|[<span data-ttu-id="1e76e-494">localSecurityOptionsSmartCardRemovalBehaviorType</span><span class="sxs-lookup"><span data-stu-id="1e76e-494">localSecurityOptionsSmartCardRemovalBehaviorType</span></span>](../resources/intune-deviceconfig-localsecurityoptionssmartcardremovalbehaviortype.md)|<span data-ttu-id="1e76e-495">此安全设置确定将已登录用户的智能卡从智能卡读卡器中删除时发生的情况。</span><span class="sxs-lookup"><span data-stu-id="1e76e-495">This security setting determines what happens when the smart card for a logged-on user is removed from the smart card reader.</span></span> <span data-ttu-id="1e76e-496">可取值为：`lockWorkstation`、`noAction`、`forceLogoff`、`disconnectRemoteDesktopSession`。</span><span class="sxs-lookup"><span data-stu-id="1e76e-496">Possible values are: `lockWorkstation`, `noAction`, `forceLogoff`, `disconnectRemoteDesktopSession`.</span></span>|
|<span data-ttu-id="1e76e-497">defenderSecurityCenterDisableAppBrowserUI</span><span class="sxs-lookup"><span data-stu-id="1e76e-497">defenderSecurityCenterDisableAppBrowserUI</span></span>|<span data-ttu-id="1e76e-498">Boolean</span><span class="sxs-lookup"><span data-stu-id="1e76e-498">Boolean</span></span>|<span data-ttu-id="1e76e-499">用于禁用应用程序和浏览器保护区域的显示。</span><span class="sxs-lookup"><span data-stu-id="1e76e-499">Used to disable the display of the app and browser protection area.</span></span>|
|<span data-ttu-id="1e76e-500">defenderSecurityCenterDisableFamilyUI</span><span class="sxs-lookup"><span data-stu-id="1e76e-500">defenderSecurityCenterDisableFamilyUI</span></span>|<span data-ttu-id="1e76e-501">Boolean</span><span class="sxs-lookup"><span data-stu-id="1e76e-501">Boolean</span></span>|<span data-ttu-id="1e76e-502">用于禁用 "家庭选项" 区域的显示。</span><span class="sxs-lookup"><span data-stu-id="1e76e-502">Used to disable the display of the family options area.</span></span>|
|<span data-ttu-id="1e76e-503">defenderSecurityCenterDisableHealthUI</span><span class="sxs-lookup"><span data-stu-id="1e76e-503">defenderSecurityCenterDisableHealthUI</span></span>|<span data-ttu-id="1e76e-504">Boolean</span><span class="sxs-lookup"><span data-stu-id="1e76e-504">Boolean</span></span>|<span data-ttu-id="1e76e-505">用于禁用设备性能和运行状况区域的显示。</span><span class="sxs-lookup"><span data-stu-id="1e76e-505">Used to disable the display of the device performance and health area.</span></span>|
|<span data-ttu-id="1e76e-506">defenderSecurityCenterDisableNetworkUI</span><span class="sxs-lookup"><span data-stu-id="1e76e-506">defenderSecurityCenterDisableNetworkUI</span></span>|<span data-ttu-id="1e76e-507">Boolean</span><span class="sxs-lookup"><span data-stu-id="1e76e-507">Boolean</span></span>|<span data-ttu-id="1e76e-508">用于禁用防火墙和网络防护区域的显示。</span><span class="sxs-lookup"><span data-stu-id="1e76e-508">Used to disable the display of the firewall and network protection area.</span></span>|
|<span data-ttu-id="1e76e-509">defenderSecurityCenterDisableVirusUI</span><span class="sxs-lookup"><span data-stu-id="1e76e-509">defenderSecurityCenterDisableVirusUI</span></span>|<span data-ttu-id="1e76e-510">Boolean</span><span class="sxs-lookup"><span data-stu-id="1e76e-510">Boolean</span></span>|<span data-ttu-id="1e76e-511">用于禁用病毒和威胁防护区域的显示。</span><span class="sxs-lookup"><span data-stu-id="1e76e-511">Used to disable the display of the virus and threat protection area.</span></span>|
|<span data-ttu-id="1e76e-512">defenderSecurityCenterDisableAccountUI</span><span class="sxs-lookup"><span data-stu-id="1e76e-512">defenderSecurityCenterDisableAccountUI</span></span>|<span data-ttu-id="1e76e-513">Boolean</span><span class="sxs-lookup"><span data-stu-id="1e76e-513">Boolean</span></span>|<span data-ttu-id="1e76e-514">用于禁用帐户保护区域的显示。</span><span class="sxs-lookup"><span data-stu-id="1e76e-514">Used to disable the display of the account protection area.</span></span>|
|<span data-ttu-id="1e76e-515">defenderSecurityCenterDisableClearTpmUI</span><span class="sxs-lookup"><span data-stu-id="1e76e-515">defenderSecurityCenterDisableClearTpmUI</span></span>|<span data-ttu-id="1e76e-516">Boolean</span><span class="sxs-lookup"><span data-stu-id="1e76e-516">Boolean</span></span>|<span data-ttu-id="1e76e-517">用于禁用 "清除 TPM" 按钮的显示。</span><span class="sxs-lookup"><span data-stu-id="1e76e-517">Used to disable the display of the Clear TPM button.</span></span>|
|<span data-ttu-id="1e76e-518">defenderSecurityCenterDisableHardwareUI</span><span class="sxs-lookup"><span data-stu-id="1e76e-518">defenderSecurityCenterDisableHardwareUI</span></span>|<span data-ttu-id="1e76e-519">Boolean</span><span class="sxs-lookup"><span data-stu-id="1e76e-519">Boolean</span></span>|<span data-ttu-id="1e76e-520">用于禁用硬件保护区域的显示。</span><span class="sxs-lookup"><span data-stu-id="1e76e-520">Used to disable the display of the hardware protection area.</span></span>|
|<span data-ttu-id="1e76e-521">defenderSecurityCenterDisableNotificationAreaUI</span><span class="sxs-lookup"><span data-stu-id="1e76e-521">defenderSecurityCenterDisableNotificationAreaUI</span></span>|<span data-ttu-id="1e76e-522">Boolean</span><span class="sxs-lookup"><span data-stu-id="1e76e-522">Boolean</span></span>|<span data-ttu-id="1e76e-523">用于禁用通知区域控件的显示。</span><span class="sxs-lookup"><span data-stu-id="1e76e-523">Used to disable the display of the notification area control.</span></span> <span data-ttu-id="1e76e-524">用户需要注销并登录或重新启动计算机，此设置才会生效。</span><span class="sxs-lookup"><span data-stu-id="1e76e-524">The user needs to either sign out and sign in or reboot the computer for this setting to take effect.</span></span>|
|<span data-ttu-id="1e76e-525">defenderSecurityCenterDisableRansomwareUI</span><span class="sxs-lookup"><span data-stu-id="1e76e-525">defenderSecurityCenterDisableRansomwareUI</span></span>|<span data-ttu-id="1e76e-526">Boolean</span><span class="sxs-lookup"><span data-stu-id="1e76e-526">Boolean</span></span>|<span data-ttu-id="1e76e-527">用于禁用勒索软件防护区域的显示。</span><span class="sxs-lookup"><span data-stu-id="1e76e-527">Used to disable the display of the ransomware protection area.</span></span> |
|<span data-ttu-id="1e76e-528">defenderSecurityCenterDisableSecureBootUI</span><span class="sxs-lookup"><span data-stu-id="1e76e-528">defenderSecurityCenterDisableSecureBootUI</span></span>|<span data-ttu-id="1e76e-529">Boolean</span><span class="sxs-lookup"><span data-stu-id="1e76e-529">Boolean</span></span>|<span data-ttu-id="1e76e-530">用于在 "设备安全性" 下禁用安全引导区域的显示。</span><span class="sxs-lookup"><span data-stu-id="1e76e-530">Used to disable the display of the secure boot area under Device security.</span></span>|
|<span data-ttu-id="1e76e-531">defenderSecurityCenterDisableTroubleshootingUI</span><span class="sxs-lookup"><span data-stu-id="1e76e-531">defenderSecurityCenterDisableTroubleshootingUI</span></span>|<span data-ttu-id="1e76e-532">Boolean</span><span class="sxs-lookup"><span data-stu-id="1e76e-532">Boolean</span></span>|<span data-ttu-id="1e76e-533">用于在 "设备安全性" 下禁用安全过程故障排除的显示。</span><span class="sxs-lookup"><span data-stu-id="1e76e-533">Used to disable the display of the security process troubleshooting under Device security.</span></span>|
|<span data-ttu-id="1e76e-534">defenderSecurityCenterDisableVulnerableTpmFirmwareUpdateUI</span><span class="sxs-lookup"><span data-stu-id="1e76e-534">defenderSecurityCenterDisableVulnerableTpmFirmwareUpdateUI</span></span>|<span data-ttu-id="1e76e-535">Boolean</span><span class="sxs-lookup"><span data-stu-id="1e76e-535">Boolean</span></span>|<span data-ttu-id="1e76e-536">用于在检测到易受攻击的固件时禁用显示更新 TPM 固件。</span><span class="sxs-lookup"><span data-stu-id="1e76e-536">Used to disable the display of update TPM Firmware when a vulnerable firmware is detected.</span></span>|
|<span data-ttu-id="1e76e-537">defenderSecurityCenterOrganizationDisplayName</span><span class="sxs-lookup"><span data-stu-id="1e76e-537">defenderSecurityCenterOrganizationDisplayName</span></span>|<span data-ttu-id="1e76e-538">String</span><span class="sxs-lookup"><span data-stu-id="1e76e-538">String</span></span>|<span data-ttu-id="1e76e-539">向用户显示的公司名称。</span><span class="sxs-lookup"><span data-stu-id="1e76e-539">The company name that is displayed to the users.</span></span>|
|<span data-ttu-id="1e76e-540">defenderSecurityCenterHelpEmail</span><span class="sxs-lookup"><span data-stu-id="1e76e-540">defenderSecurityCenterHelpEmail</span></span>|<span data-ttu-id="1e76e-541">String</span><span class="sxs-lookup"><span data-stu-id="1e76e-541">String</span></span>|<span data-ttu-id="1e76e-542">向用户显示的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="1e76e-542">The email address that is displayed to users.</span></span>|
|<span data-ttu-id="1e76e-543">defenderSecurityCenterHelpPhone</span><span class="sxs-lookup"><span data-stu-id="1e76e-543">defenderSecurityCenterHelpPhone</span></span>|<span data-ttu-id="1e76e-544">String</span><span class="sxs-lookup"><span data-stu-id="1e76e-544">String</span></span>|<span data-ttu-id="1e76e-545">向用户显示的电话号码或 Skype ID。</span><span class="sxs-lookup"><span data-stu-id="1e76e-545">The phone number or Skype ID that is displayed to users.</span></span>|
|<span data-ttu-id="1e76e-546">defenderSecurityCenterHelpURL</span><span class="sxs-lookup"><span data-stu-id="1e76e-546">defenderSecurityCenterHelpURL</span></span>|<span data-ttu-id="1e76e-547">String</span><span class="sxs-lookup"><span data-stu-id="1e76e-547">String</span></span>|<span data-ttu-id="1e76e-548">"帮助" 门户 URL 将向用户显示。</span><span class="sxs-lookup"><span data-stu-id="1e76e-548">The help portal URL this is displayed to users.</span></span>|
|<span data-ttu-id="1e76e-549">defenderSecurityCenterNotificationsFromApp</span><span class="sxs-lookup"><span data-stu-id="1e76e-549">defenderSecurityCenterNotificationsFromApp</span></span>|[<span data-ttu-id="1e76e-550">defenderSecurityCenterNotificationsFromAppType</span><span class="sxs-lookup"><span data-stu-id="1e76e-550">defenderSecurityCenterNotificationsFromAppType</span></span>](../resources/intune-deviceconfig-defendersecuritycenternotificationsfromapptype.md)|<span data-ttu-id="1e76e-551">要从应用程序的显示区域中显示的通知。</span><span class="sxs-lookup"><span data-stu-id="1e76e-551">Notifications to show from the displayed areas of app.</span></span> <span data-ttu-id="1e76e-552">可取值为：`notConfigured`、`blockNoncriticalNotifications`、`blockAllNotifications`。</span><span class="sxs-lookup"><span data-stu-id="1e76e-552">Possible values are: `notConfigured`, `blockNoncriticalNotifications`, `blockAllNotifications`.</span></span>|
|<span data-ttu-id="1e76e-553">defenderSecurityCenterITContactDisplay</span><span class="sxs-lookup"><span data-stu-id="1e76e-553">defenderSecurityCenterITContactDisplay</span></span>|[<span data-ttu-id="1e76e-554">defenderSecurityCenterITContactDisplayType</span><span class="sxs-lookup"><span data-stu-id="1e76e-554">defenderSecurityCenterITContactDisplayType</span></span>](../resources/intune-deviceconfig-defendersecuritycenteritcontactdisplaytype.md)|<span data-ttu-id="1e76e-555">配置向最终用户显示 IT 联系人信息的位置。</span><span class="sxs-lookup"><span data-stu-id="1e76e-555">Configure where to display IT contact information to end users.</span></span> <span data-ttu-id="1e76e-556">可取值为：`notConfigured`、`displayInAppAndInNotifications`、`displayOnlyInApp`、`displayOnlyInNotifications`。</span><span class="sxs-lookup"><span data-stu-id="1e76e-556">Possible values are: `notConfigured`, `displayInAppAndInNotifications`, `displayOnlyInApp`, `displayOnlyInNotifications`.</span></span>|
|<span data-ttu-id="1e76e-557">windowsDefenderTamperProtection</span><span class="sxs-lookup"><span data-stu-id="1e76e-557">windowsDefenderTamperProtection</span></span>|[<span data-ttu-id="1e76e-558">windowsDefenderTamperProtectionOptions</span><span class="sxs-lookup"><span data-stu-id="1e76e-558">windowsDefenderTamperProtectionOptions</span></span>](../resources/intune-deviceconfig-windowsdefendertamperprotectionoptions.md)|<span data-ttu-id="1e76e-559">配置 windows defender TamperProtection 设置。</span><span class="sxs-lookup"><span data-stu-id="1e76e-559">Configure windows defender TamperProtection settings.</span></span> <span data-ttu-id="1e76e-560">可取值为：`notConfigured`、`enable`、`disable`。</span><span class="sxs-lookup"><span data-stu-id="1e76e-560">Possible values are: `notConfigured`, `enable`, `disable`.</span></span>|
|<span data-ttu-id="1e76e-561">firewallBlockStatefulFTP</span><span class="sxs-lookup"><span data-stu-id="1e76e-561">firewallBlockStatefulFTP</span></span>|<span data-ttu-id="1e76e-562">Boolean</span><span class="sxs-lookup"><span data-stu-id="1e76e-562">Boolean</span></span>|<span data-ttu-id="1e76e-563">阻止到设备的有状态 FTP 连接</span><span class="sxs-lookup"><span data-stu-id="1e76e-563">Blocks stateful FTP connections to the device</span></span>|
|<span data-ttu-id="1e76e-564">firewallIdleTimeoutForSecurityAssociationInSeconds</span><span class="sxs-lookup"><span data-stu-id="1e76e-564">firewallIdleTimeoutForSecurityAssociationInSeconds</span></span>|<span data-ttu-id="1e76e-565">Int32</span><span class="sxs-lookup"><span data-stu-id="1e76e-565">Int32</span></span>|<span data-ttu-id="1e76e-566">配置安全关联的空闲超时（以秒为单位），值范围为 300 到 3600（包括这两个值）。</span><span class="sxs-lookup"><span data-stu-id="1e76e-566">Configures the idle timeout for security associations, in seconds, from 300 to 3600 inclusive.</span></span> <span data-ttu-id="1e76e-567">这是一个时间段，在此之后安全关联将过期并被删除。</span><span class="sxs-lookup"><span data-stu-id="1e76e-567">This is the period after which security associations will expire and be deleted.</span></span> <span data-ttu-id="1e76e-568">有效值为 300 至 3600</span><span class="sxs-lookup"><span data-stu-id="1e76e-568">Valid values 300 to 3600</span></span>|
|<span data-ttu-id="1e76e-569">firewallPreSharedKeyEncodingMethod</span><span class="sxs-lookup"><span data-stu-id="1e76e-569">firewallPreSharedKeyEncodingMethod</span></span>|[<span data-ttu-id="1e76e-570">firewallPreSharedKeyEncodingMethodType</span><span class="sxs-lookup"><span data-stu-id="1e76e-570">firewallPreSharedKeyEncodingMethodType</span></span>](../resources/intune-deviceconfig-firewallpresharedkeyencodingmethodtype.md)|<span data-ttu-id="1e76e-571">选择要使用的预共享密钥编码。</span><span class="sxs-lookup"><span data-stu-id="1e76e-571">Select the preshared key encoding to be used.</span></span> <span data-ttu-id="1e76e-572">可取值为：`deviceDefault`、`none`、`utF8`。</span><span class="sxs-lookup"><span data-stu-id="1e76e-572">Possible values are: `deviceDefault`, `none`, `utF8`.</span></span>|
|<span data-ttu-id="1e76e-573">firewallIPSecExemptionsAllowNeighborDiscovery</span><span class="sxs-lookup"><span data-stu-id="1e76e-573">firewallIPSecExemptionsAllowNeighborDiscovery</span></span>|<span data-ttu-id="1e76e-574">Boolean</span><span class="sxs-lookup"><span data-stu-id="1e76e-574">Boolean</span></span>|<span data-ttu-id="1e76e-575">配置 IPSec 免除项以允许邻居发现 IPv6 ICMP 类型代码</span><span class="sxs-lookup"><span data-stu-id="1e76e-575">Configures IPSec exemptions to allow neighbor discovery IPv6 ICMP type-codes</span></span>|
|<span data-ttu-id="1e76e-576">firewallIPSecExemptionsAllowICMP</span><span class="sxs-lookup"><span data-stu-id="1e76e-576">firewallIPSecExemptionsAllowICMP</span></span>|<span data-ttu-id="1e76e-577">Boolean</span><span class="sxs-lookup"><span data-stu-id="1e76e-577">Boolean</span></span>|<span data-ttu-id="1e76e-578">配置 IPSec 免除项以允许 ICMP</span><span class="sxs-lookup"><span data-stu-id="1e76e-578">Configures IPSec exemptions to allow ICMP</span></span>|
|<span data-ttu-id="1e76e-579">firewallIPSecExemptionsAllowRouterDiscovery</span><span class="sxs-lookup"><span data-stu-id="1e76e-579">firewallIPSecExemptionsAllowRouterDiscovery</span></span>|<span data-ttu-id="1e76e-580">Boolean</span><span class="sxs-lookup"><span data-stu-id="1e76e-580">Boolean</span></span>|<span data-ttu-id="1e76e-581">配置 IPSec 免除项以允许路由器发现 IPv6 ICMP 类型代码</span><span class="sxs-lookup"><span data-stu-id="1e76e-581">Configures IPSec exemptions to allow router discovery IPv6 ICMP type-codes</span></span>|
|<span data-ttu-id="1e76e-582">firewallIPSecExemptionsAllowDHCP</span><span class="sxs-lookup"><span data-stu-id="1e76e-582">firewallIPSecExemptionsAllowDHCP</span></span>|<span data-ttu-id="1e76e-583">Boolean</span><span class="sxs-lookup"><span data-stu-id="1e76e-583">Boolean</span></span>|<span data-ttu-id="1e76e-584">配置 IPSec 免除项以允许 IPv4 和 IPv6 DHCP 通信</span><span class="sxs-lookup"><span data-stu-id="1e76e-584">Configures IPSec exemptions to allow both IPv4 and IPv6 DHCP traffic</span></span>|
|<span data-ttu-id="1e76e-585">firewallCertificateRevocationListCheckMethod</span><span class="sxs-lookup"><span data-stu-id="1e76e-585">firewallCertificateRevocationListCheckMethod</span></span>|[<span data-ttu-id="1e76e-586">firewallCertificateRevocationListCheckMethodType</span><span class="sxs-lookup"><span data-stu-id="1e76e-586">firewallCertificateRevocationListCheckMethodType</span></span>](../resources/intune-deviceconfig-firewallcertificaterevocationlistcheckmethodtype.md)|<span data-ttu-id="1e76e-587">指定如何强制执行证书吊销列表。</span><span class="sxs-lookup"><span data-stu-id="1e76e-587">Specify how the certificate revocation list is to be enforced.</span></span> <span data-ttu-id="1e76e-588">可取值为：`deviceDefault`、`none`、`attempt`、`require`。</span><span class="sxs-lookup"><span data-stu-id="1e76e-588">Possible values are: `deviceDefault`, `none`, `attempt`, `require`.</span></span>|
|<span data-ttu-id="1e76e-589">firewallMergeKeyingModuleSettings</span><span class="sxs-lookup"><span data-stu-id="1e76e-589">firewallMergeKeyingModuleSettings</span></span>|<span data-ttu-id="1e76e-590">Boolean</span><span class="sxs-lookup"><span data-stu-id="1e76e-590">Boolean</span></span>|<span data-ttu-id="1e76e-591">如果键控模块不完全支持身份验证集，请指示模块仅忽略不受支持的身份验证套件而不是整个集</span><span class="sxs-lookup"><span data-stu-id="1e76e-591">If an authentication set is not fully supported by a keying module, direct the module to ignore only unsupported authentication suites rather than the entire set</span></span>|
|<span data-ttu-id="1e76e-592">firewallPacketQueueingMethod</span><span class="sxs-lookup"><span data-stu-id="1e76e-592">firewallPacketQueueingMethod</span></span>|[<span data-ttu-id="1e76e-593">firewallPacketQueueingMethodType</span><span class="sxs-lookup"><span data-stu-id="1e76e-593">firewallPacketQueueingMethodType</span></span>](../resources/intune-deviceconfig-firewallpacketqueueingmethodtype.md)|<span data-ttu-id="1e76e-594">配置如何在隧道网关应用场景中应用数据包排队。</span><span class="sxs-lookup"><span data-stu-id="1e76e-594">Configures how packet queueing should be applied in the tunnel gateway scenario.</span></span> <span data-ttu-id="1e76e-595">可取值为：`deviceDefault`、`disabled`、`queueInbound`、`queueOutbound`、`queueBoth`。</span><span class="sxs-lookup"><span data-stu-id="1e76e-595">Possible values are: `deviceDefault`, `disabled`, `queueInbound`, `queueOutbound`, `queueBoth`.</span></span>|
|<span data-ttu-id="1e76e-596">firewallProfileDomain</span><span class="sxs-lookup"><span data-stu-id="1e76e-596">firewallProfileDomain</span></span>|[<span data-ttu-id="1e76e-597">windowsFirewallNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="1e76e-597">windowsFirewallNetworkProfile</span></span>](../resources/intune-deviceconfig-windowsfirewallnetworkprofile.md)|<span data-ttu-id="1e76e-598">配置域网络的防火墙配置文件设置</span><span class="sxs-lookup"><span data-stu-id="1e76e-598">Configures the firewall profile settings for domain networks</span></span>|
|<span data-ttu-id="1e76e-599">firewallProfilePublic</span><span class="sxs-lookup"><span data-stu-id="1e76e-599">firewallProfilePublic</span></span>|[<span data-ttu-id="1e76e-600">windowsFirewallNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="1e76e-600">windowsFirewallNetworkProfile</span></span>](../resources/intune-deviceconfig-windowsfirewallnetworkprofile.md)|<span data-ttu-id="1e76e-601">配置公用网络的防火墙配置文件设置</span><span class="sxs-lookup"><span data-stu-id="1e76e-601">Configures the firewall profile settings for public networks</span></span>|
|<span data-ttu-id="1e76e-602">firewallProfilePrivate</span><span class="sxs-lookup"><span data-stu-id="1e76e-602">firewallProfilePrivate</span></span>|[<span data-ttu-id="1e76e-603">windowsFirewallNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="1e76e-603">windowsFirewallNetworkProfile</span></span>](../resources/intune-deviceconfig-windowsfirewallnetworkprofile.md)|<span data-ttu-id="1e76e-604">配置专用网络的防火墙配置文件设置</span><span class="sxs-lookup"><span data-stu-id="1e76e-604">Configures the firewall profile settings for private networks</span></span>|
|<span data-ttu-id="1e76e-605">attackSurfaceReductionRules</span><span class="sxs-lookup"><span data-stu-id="1e76e-605">attackSurfaceReductionRules</span></span>|<span data-ttu-id="1e76e-606">String</span><span class="sxs-lookup"><span data-stu-id="1e76e-606">String</span></span>|<span data-ttu-id="1e76e-607">攻击面减少规则</span><span class="sxs-lookup"><span data-stu-id="1e76e-607">Attack surface reduction rules</span></span>|
|<span data-ttu-id="1e76e-608">defenderAdobeReaderLaunchChildProcess</span><span class="sxs-lookup"><span data-stu-id="1e76e-608">defenderAdobeReaderLaunchChildProcess</span></span>|[<span data-ttu-id="1e76e-609">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="1e76e-609">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="1e76e-610">值，该值指示 Adobe Reader 创建子进程的行为。</span><span class="sxs-lookup"><span data-stu-id="1e76e-610">Value indicating the behavior of Adobe Reader from creating child processes.</span></span> <span data-ttu-id="1e76e-611">可取值为：`userDefined`、`enable`、`auditMode`。</span><span class="sxs-lookup"><span data-stu-id="1e76e-611">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="1e76e-612">defenderAttackSurfaceReductionExcludedPaths</span><span class="sxs-lookup"><span data-stu-id="1e76e-612">defenderAttackSurfaceReductionExcludedPaths</span></span>|<span data-ttu-id="1e76e-613">String 集合</span><span class="sxs-lookup"><span data-stu-id="1e76e-613">String collection</span></span>|<span data-ttu-id="1e76e-614">要从攻击面减少规则中排除的 exe 文件和文件夹的列表</span><span class="sxs-lookup"><span data-stu-id="1e76e-614">List of exe files and folders to be excluded from attack surface reduction rules</span></span>|
|<span data-ttu-id="1e76e-615">defenderOfficeAppsOtherProcessInjectionType</span><span class="sxs-lookup"><span data-stu-id="1e76e-615">defenderOfficeAppsOtherProcessInjectionType</span></span>|[<span data-ttu-id="1e76e-616">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="1e76e-616">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="1e76e-617">值，该值指示插入到其他进程中的 Office 应用程序的行为。</span><span class="sxs-lookup"><span data-stu-id="1e76e-617">Value indicating the behavior of Office applications injecting into other processes.</span></span> <span data-ttu-id="1e76e-618">可取值为：`userDefined`、`block`、`auditMode`。</span><span class="sxs-lookup"><span data-stu-id="1e76e-618">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="1e76e-619">defenderOfficeAppsOtherProcessInjection</span><span class="sxs-lookup"><span data-stu-id="1e76e-619">defenderOfficeAppsOtherProcessInjection</span></span>|[<span data-ttu-id="1e76e-620">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="1e76e-620">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="1e76e-621">值，该值指示插入到其他进程中的 Office 应用程序的行为。</span><span class="sxs-lookup"><span data-stu-id="1e76e-621">Value indicating the behavior of  Office applications injecting into other processes.</span></span> <span data-ttu-id="1e76e-622">可取值为：`userDefined`、`enable`、`auditMode`。</span><span class="sxs-lookup"><span data-stu-id="1e76e-622">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="1e76e-623">defenderOfficeCommunicationAppsLaunchChildProcess</span><span class="sxs-lookup"><span data-stu-id="1e76e-623">defenderOfficeCommunicationAppsLaunchChildProcess</span></span>|[<span data-ttu-id="1e76e-624">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="1e76e-624">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="1e76e-625">值，该值指示 Office 通信应用程序（包括 Microsoft Outlook）在创建子进程时的行为。</span><span class="sxs-lookup"><span data-stu-id="1e76e-625">Value indicating the behavior of Office communication applications, including Microsoft Outlook, from creating child processes.</span></span> <span data-ttu-id="1e76e-626">可取值为：`userDefined`、`enable`、`auditMode`。</span><span class="sxs-lookup"><span data-stu-id="1e76e-626">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="1e76e-627">defenderOfficeAppsExecutableContentCreationOrLaunchType</span><span class="sxs-lookup"><span data-stu-id="1e76e-627">defenderOfficeAppsExecutableContentCreationOrLaunchType</span></span>|[<span data-ttu-id="1e76e-628">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="1e76e-628">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="1e76e-629">值，该值指示 Office 应用程序/宏创建或启动可执行内容的行为。</span><span class="sxs-lookup"><span data-stu-id="1e76e-629">Value indicating the behavior of Office applications/macros creating or launching executable content.</span></span> <span data-ttu-id="1e76e-630">可取值为：`userDefined`、`block`、`auditMode`。</span><span class="sxs-lookup"><span data-stu-id="1e76e-630">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="1e76e-631">defenderOfficeAppsExecutableContentCreationOrLaunch</span><span class="sxs-lookup"><span data-stu-id="1e76e-631">defenderOfficeAppsExecutableContentCreationOrLaunch</span></span>|[<span data-ttu-id="1e76e-632">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="1e76e-632">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="1e76e-633">值，该值指示 Office 应用程序/宏创建或启动可执行内容的行为。</span><span class="sxs-lookup"><span data-stu-id="1e76e-633">Value indicating the behavior of Office applications/macros creating or launching executable content.</span></span> <span data-ttu-id="1e76e-634">可取值为：`userDefined`、`enable`、`auditMode`。</span><span class="sxs-lookup"><span data-stu-id="1e76e-634">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="1e76e-635">defenderOfficeAppsLaunchChildProcessType</span><span class="sxs-lookup"><span data-stu-id="1e76e-635">defenderOfficeAppsLaunchChildProcessType</span></span>|[<span data-ttu-id="1e76e-636">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="1e76e-636">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="1e76e-637">值，该值指示 Office 应用程序启动子进程的行为。</span><span class="sxs-lookup"><span data-stu-id="1e76e-637">Value indicating the behavior of Office application launching child processes.</span></span> <span data-ttu-id="1e76e-638">可取值为：`userDefined`、`block`、`auditMode`。</span><span class="sxs-lookup"><span data-stu-id="1e76e-638">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="1e76e-639">defenderOfficeAppsLaunchChildProcess</span><span class="sxs-lookup"><span data-stu-id="1e76e-639">defenderOfficeAppsLaunchChildProcess</span></span>|[<span data-ttu-id="1e76e-640">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="1e76e-640">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="1e76e-641">值，该值指示 Office 应用程序启动子进程的行为。</span><span class="sxs-lookup"><span data-stu-id="1e76e-641">Value indicating the behavior of Office application launching child processes.</span></span> <span data-ttu-id="1e76e-642">可取值为：`userDefined`、`enable`、`auditMode`。</span><span class="sxs-lookup"><span data-stu-id="1e76e-642">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="1e76e-643">defenderOfficeMacroCodeAllowWin32ImportsType</span><span class="sxs-lookup"><span data-stu-id="1e76e-643">defenderOfficeMacroCodeAllowWin32ImportsType</span></span>|[<span data-ttu-id="1e76e-644">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="1e76e-644">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="1e76e-645">值，该值指示从 Office 中的宏代码的 Win32 导入行为。</span><span class="sxs-lookup"><span data-stu-id="1e76e-645">Value indicating the behavior of Win32 imports from Macro code in Office.</span></span> <span data-ttu-id="1e76e-646">可取值为：`userDefined`、`block`、`auditMode`。</span><span class="sxs-lookup"><span data-stu-id="1e76e-646">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="1e76e-647">defenderOfficeMacroCodeAllowWin32Imports</span><span class="sxs-lookup"><span data-stu-id="1e76e-647">defenderOfficeMacroCodeAllowWin32Imports</span></span>|[<span data-ttu-id="1e76e-648">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="1e76e-648">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="1e76e-649">值，该值指示从 Office 中的宏代码的 Win32 导入行为。</span><span class="sxs-lookup"><span data-stu-id="1e76e-649">Value indicating the behavior of Win32 imports from Macro code in Office.</span></span> <span data-ttu-id="1e76e-650">可取值为：`userDefined`、`enable`、`auditMode`。</span><span class="sxs-lookup"><span data-stu-id="1e76e-650">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="1e76e-651">defenderScriptObfuscatedMacroCodeType</span><span class="sxs-lookup"><span data-stu-id="1e76e-651">defenderScriptObfuscatedMacroCodeType</span></span>|[<span data-ttu-id="1e76e-652">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="1e76e-652">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="1e76e-653">值，该值指示模糊的 js/vbs/ps/宏代码的行为。</span><span class="sxs-lookup"><span data-stu-id="1e76e-653">Value indicating the behavior of obfuscated js/vbs/ps/macro code.</span></span> <span data-ttu-id="1e76e-654">可取值为：`userDefined`、`block`、`auditMode`。</span><span class="sxs-lookup"><span data-stu-id="1e76e-654">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="1e76e-655">defenderScriptObfuscatedMacroCode</span><span class="sxs-lookup"><span data-stu-id="1e76e-655">defenderScriptObfuscatedMacroCode</span></span>|[<span data-ttu-id="1e76e-656">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="1e76e-656">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="1e76e-657">值，该值指示模糊的 js/vbs/ps/宏代码的行为。</span><span class="sxs-lookup"><span data-stu-id="1e76e-657">Value indicating the behavior of obfuscated js/vbs/ps/macro code.</span></span> <span data-ttu-id="1e76e-658">可取值为：`userDefined`、`enable`、`auditMode`。</span><span class="sxs-lookup"><span data-stu-id="1e76e-658">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="1e76e-659">defenderScriptDownloadedPayloadExecutionType</span><span class="sxs-lookup"><span data-stu-id="1e76e-659">defenderScriptDownloadedPayloadExecutionType</span></span>|[<span data-ttu-id="1e76e-660">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="1e76e-660">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="1e76e-661">值，该值指示从 Internet 下载的 js/vbs 执行负载的行为。</span><span class="sxs-lookup"><span data-stu-id="1e76e-661">Value indicating the behavior of js/vbs executing payload downloaded from Internet.</span></span> <span data-ttu-id="1e76e-662">可取值为：`userDefined`、`block`、`auditMode`。</span><span class="sxs-lookup"><span data-stu-id="1e76e-662">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="1e76e-663">defenderScriptDownloadedPayloadExecution</span><span class="sxs-lookup"><span data-stu-id="1e76e-663">defenderScriptDownloadedPayloadExecution</span></span>|[<span data-ttu-id="1e76e-664">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="1e76e-664">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="1e76e-665">值，该值指示从 Internet 下载的 js/vbs 执行负载的行为。</span><span class="sxs-lookup"><span data-stu-id="1e76e-665">Value indicating the behavior of js/vbs executing payload downloaded from Internet.</span></span> <span data-ttu-id="1e76e-666">可取值为：`userDefined`、`enable`、`auditMode`。</span><span class="sxs-lookup"><span data-stu-id="1e76e-666">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="1e76e-667">defenderPreventCredentialStealingType</span><span class="sxs-lookup"><span data-stu-id="1e76e-667">defenderPreventCredentialStealingType</span></span>|[<span data-ttu-id="1e76e-668">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="1e76e-668">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="1e76e-669">值，该值指示是否允许从 Windows 本地安全机构子系统中盗取凭据。</span><span class="sxs-lookup"><span data-stu-id="1e76e-669">Value indicating if credential stealing from the Windows local security authority subsystem is permitted.</span></span> <span data-ttu-id="1e76e-670">可取值为：`userDefined`、`enable`、`auditMode`。</span><span class="sxs-lookup"><span data-stu-id="1e76e-670">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="1e76e-671">defenderProcessCreationType</span><span class="sxs-lookup"><span data-stu-id="1e76e-671">defenderProcessCreationType</span></span>|[<span data-ttu-id="1e76e-672">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="1e76e-672">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="1e76e-673">一个值，该值指示对源自 PSExec 和 WMI 命令的进程创建的响应。</span><span class="sxs-lookup"><span data-stu-id="1e76e-673">Value indicating response to process creations originating from PSExec and WMI commands.</span></span> <span data-ttu-id="1e76e-674">可取值为：`userDefined`、`block`、`auditMode`。</span><span class="sxs-lookup"><span data-stu-id="1e76e-674">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="1e76e-675">defenderProcessCreation</span><span class="sxs-lookup"><span data-stu-id="1e76e-675">defenderProcessCreation</span></span>|[<span data-ttu-id="1e76e-676">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="1e76e-676">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="1e76e-677">一个值，该值指示对源自 PSExec 和 WMI 命令的进程创建的响应。</span><span class="sxs-lookup"><span data-stu-id="1e76e-677">Value indicating response to process creations originating from PSExec and WMI commands.</span></span> <span data-ttu-id="1e76e-678">可取值为：`userDefined`、`enable`、`auditMode`。</span><span class="sxs-lookup"><span data-stu-id="1e76e-678">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="1e76e-679">defenderUntrustedUSBProcessType</span><span class="sxs-lookup"><span data-stu-id="1e76e-679">defenderUntrustedUSBProcessType</span></span>|[<span data-ttu-id="1e76e-680">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="1e76e-680">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="1e76e-681">指示对从 USB 运行的不受信任和未签名进程的响应的值。</span><span class="sxs-lookup"><span data-stu-id="1e76e-681">Value indicating response to untrusted and unsigned processes that run from USB.</span></span> <span data-ttu-id="1e76e-682">可取值为：`userDefined`、`block`、`auditMode`。</span><span class="sxs-lookup"><span data-stu-id="1e76e-682">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="1e76e-683">defenderUntrustedUSBProcess</span><span class="sxs-lookup"><span data-stu-id="1e76e-683">defenderUntrustedUSBProcess</span></span>|[<span data-ttu-id="1e76e-684">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="1e76e-684">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="1e76e-685">指示对从 USB 运行的不受信任和未签名进程的响应的值。</span><span class="sxs-lookup"><span data-stu-id="1e76e-685">Value indicating response to untrusted and unsigned processes that run from USB.</span></span> <span data-ttu-id="1e76e-686">可取值为：`userDefined`、`enable`、`auditMode`。</span><span class="sxs-lookup"><span data-stu-id="1e76e-686">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="1e76e-687">defenderUntrustedExecutableType</span><span class="sxs-lookup"><span data-stu-id="1e76e-687">defenderUntrustedExecutableType</span></span>|[<span data-ttu-id="1e76e-688">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="1e76e-688">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="1e76e-689">指示对不符合流行、年龄或受信任列表条件的可执行文件的响应的值。</span><span class="sxs-lookup"><span data-stu-id="1e76e-689">Value indicating response to executables that don't meet a prevalence, age, or trusted list criteria.</span></span> <span data-ttu-id="1e76e-690">可取值为：`userDefined`、`block`、`auditMode`。</span><span class="sxs-lookup"><span data-stu-id="1e76e-690">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="1e76e-691">defenderUntrustedExecutable</span><span class="sxs-lookup"><span data-stu-id="1e76e-691">defenderUntrustedExecutable</span></span>|[<span data-ttu-id="1e76e-692">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="1e76e-692">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="1e76e-693">指示对不符合流行、年龄或受信任列表条件的可执行文件的响应的值。</span><span class="sxs-lookup"><span data-stu-id="1e76e-693">Value indicating response to executables that don't meet a prevalence, age, or trusted list criteria.</span></span> <span data-ttu-id="1e76e-694">可取值为：`userDefined`、`enable`、`auditMode`。</span><span class="sxs-lookup"><span data-stu-id="1e76e-694">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="1e76e-695">defenderEmailContentExecutionType</span><span class="sxs-lookup"><span data-stu-id="1e76e-695">defenderEmailContentExecutionType</span></span>|[<span data-ttu-id="1e76e-696">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="1e76e-696">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="1e76e-697">一个值，该值指示是否应从电子邮件（web 邮件/邮件客户端）中删除可执行内容（exe、dll、ps、js、vbs 等）的执行。</span><span class="sxs-lookup"><span data-stu-id="1e76e-697">Value indicating if execution of executable content (exe, dll, ps, js, vbs, etc) should be dropped from email (webmail/mail-client).</span></span> <span data-ttu-id="1e76e-698">可取值为：`userDefined`、`block`、`auditMode`。</span><span class="sxs-lookup"><span data-stu-id="1e76e-698">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="1e76e-699">defenderEmailContentExecution</span><span class="sxs-lookup"><span data-stu-id="1e76e-699">defenderEmailContentExecution</span></span>|[<span data-ttu-id="1e76e-700">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="1e76e-700">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="1e76e-701">一个值，该值指示是否应从电子邮件（web 邮件/邮件客户端）中删除可执行内容（exe、dll、ps、js、vbs 等）的执行。</span><span class="sxs-lookup"><span data-stu-id="1e76e-701">Value indicating if execution of executable content (exe, dll, ps, js, vbs, etc) should be dropped from email (webmail/mail-client).</span></span> <span data-ttu-id="1e76e-702">可取值为：`userDefined`、`enable`、`auditMode`。</span><span class="sxs-lookup"><span data-stu-id="1e76e-702">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="1e76e-703">defenderAdvancedRansomewareProtectionType</span><span class="sxs-lookup"><span data-stu-id="1e76e-703">defenderAdvancedRansomewareProtectionType</span></span>|[<span data-ttu-id="1e76e-704">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="1e76e-704">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="1e76e-705">指示使用针对 ransomeware 的高级防护的值。</span><span class="sxs-lookup"><span data-stu-id="1e76e-705">Value indicating use of advanced protection against ransomeware.</span></span> <span data-ttu-id="1e76e-706">可取值为：`userDefined`、`enable`、`auditMode`。</span><span class="sxs-lookup"><span data-stu-id="1e76e-706">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="1e76e-707">defenderGuardMyFoldersType</span><span class="sxs-lookup"><span data-stu-id="1e76e-707">defenderGuardMyFoldersType</span></span>|[<span data-ttu-id="1e76e-708">folderProtectionType</span><span class="sxs-lookup"><span data-stu-id="1e76e-708">folderProtectionType</span></span>](../resources/intune-deviceconfig-folderprotectiontype.md)|<span data-ttu-id="1e76e-709">值，该值指示受保护文件夹的行为。</span><span class="sxs-lookup"><span data-stu-id="1e76e-709">Value indicating the behavior of protected folders.</span></span> <span data-ttu-id="1e76e-710">可取值为：`userDefined`、`enable`、`auditMode`、`blockDiskModification`、`auditDiskModification`。</span><span class="sxs-lookup"><span data-stu-id="1e76e-710">Possible values are: `userDefined`, `enable`, `auditMode`, `blockDiskModification`, `auditDiskModification`.</span></span>|
|<span data-ttu-id="1e76e-711">defenderGuardedFoldersAllowedAppPaths</span><span class="sxs-lookup"><span data-stu-id="1e76e-711">defenderGuardedFoldersAllowedAppPaths</span></span>|<span data-ttu-id="1e76e-712">String collection</span><span class="sxs-lookup"><span data-stu-id="1e76e-712">String collection</span></span>|<span data-ttu-id="1e76e-713">允许访问受保护文件夹的 exe 路径列表</span><span class="sxs-lookup"><span data-stu-id="1e76e-713">List of paths to exe that are allowed to access protected folders</span></span>|
|<span data-ttu-id="1e76e-714">defenderAdditionalGuardedFolders</span><span class="sxs-lookup"><span data-stu-id="1e76e-714">defenderAdditionalGuardedFolders</span></span>|<span data-ttu-id="1e76e-715">String 集合</span><span class="sxs-lookup"><span data-stu-id="1e76e-715">String collection</span></span>|<span data-ttu-id="1e76e-716">要添加到受保护文件夹列表的文件夹路径列表</span><span class="sxs-lookup"><span data-stu-id="1e76e-716">List of folder paths to be added to the list of protected folders</span></span>|
|<span data-ttu-id="1e76e-717">defenderNetworkProtectionType</span><span class="sxs-lookup"><span data-stu-id="1e76e-717">defenderNetworkProtectionType</span></span>|[<span data-ttu-id="1e76e-718">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="1e76e-718">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="1e76e-719">值，该值指示 NetworkProtection 的行为。</span><span class="sxs-lookup"><span data-stu-id="1e76e-719">Value indicating the behavior of NetworkProtection.</span></span> <span data-ttu-id="1e76e-720">可取值为：`userDefined`、`enable`、`auditMode`。</span><span class="sxs-lookup"><span data-stu-id="1e76e-720">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="1e76e-721">defenderExploitProtectionXml</span><span class="sxs-lookup"><span data-stu-id="1e76e-721">defenderExploitProtectionXml</span></span>|<span data-ttu-id="1e76e-722">Binary</span><span class="sxs-lookup"><span data-stu-id="1e76e-722">Binary</span></span>|<span data-ttu-id="1e76e-723">包含有关 Exploit Protection 详细信息的 xml 内容。</span><span class="sxs-lookup"><span data-stu-id="1e76e-723">Xml content containing information regarding exploit protection details.</span></span>|
|<span data-ttu-id="1e76e-724">defenderExploitProtectionXmlFileName</span><span class="sxs-lookup"><span data-stu-id="1e76e-724">defenderExploitProtectionXmlFileName</span></span>|<span data-ttu-id="1e76e-725">String</span><span class="sxs-lookup"><span data-stu-id="1e76e-725">String</span></span>|<span data-ttu-id="1e76e-726">从中获取 DefenderExploitProtectionXml 的文件的名称。</span><span class="sxs-lookup"><span data-stu-id="1e76e-726">Name of the file from which DefenderExploitProtectionXml was obtained.</span></span>|
|<span data-ttu-id="1e76e-727">defenderSecurityCenterBlockExploitProtectionOverride</span><span class="sxs-lookup"><span data-stu-id="1e76e-727">defenderSecurityCenterBlockExploitProtectionOverride</span></span>|<span data-ttu-id="1e76e-728">Boolean</span><span class="sxs-lookup"><span data-stu-id="1e76e-728">Boolean</span></span>|<span data-ttu-id="1e76e-729">指示是否阻止用户覆盖 Exploit Protection 设置。</span><span class="sxs-lookup"><span data-stu-id="1e76e-729">Indicates whether or not to block user from overriding Exploit Protection settings.</span></span>|
|<span data-ttu-id="1e76e-730">appLockerApplicationControl</span><span class="sxs-lookup"><span data-stu-id="1e76e-730">appLockerApplicationControl</span></span>|[<span data-ttu-id="1e76e-731">appLockerApplicationControlType</span><span class="sxs-lookup"><span data-stu-id="1e76e-731">appLockerApplicationControlType</span></span>](../resources/intune-deviceconfig-applockerapplicationcontroltype.md)|<span data-ttu-id="1e76e-732">使管理员能够选择在设备上允许哪些类型的应用。</span><span class="sxs-lookup"><span data-stu-id="1e76e-732">Enables the Admin to choose what types of app to allow on devices.</span></span> <span data-ttu-id="1e76e-733">可取值为：`notConfigured`、`enforceComponentsAndStoreApps`、`auditComponentsAndStoreApps`、`enforceComponentsStoreAppsAndSmartlocker`、`auditComponentsStoreAppsAndSmartlocker`。</span><span class="sxs-lookup"><span data-stu-id="1e76e-733">Possible values are: `notConfigured`, `enforceComponentsAndStoreApps`, `auditComponentsAndStoreApps`, `enforceComponentsStoreAppsAndSmartlocker`, `auditComponentsStoreAppsAndSmartlocker`.</span></span>|
|<span data-ttu-id="1e76e-734">deviceGuardLocalSystemAuthorityCredentialGuardSettings</span><span class="sxs-lookup"><span data-stu-id="1e76e-734">deviceGuardLocalSystemAuthorityCredentialGuardSettings</span></span>|[<span data-ttu-id="1e76e-735">deviceGuardLocalSystemAuthorityCredentialGuardType</span><span class="sxs-lookup"><span data-stu-id="1e76e-735">deviceGuardLocalSystemAuthorityCredentialGuardType</span></span>](../resources/intune-deviceconfig-deviceguardlocalsystemauthoritycredentialguardtype.md)|<span data-ttu-id="1e76e-736">如果平台安全级别具有安全启动和基于虚拟化的安全性均已启用，则打开 Credential Guard。</span><span class="sxs-lookup"><span data-stu-id="1e76e-736">Turn on Credential Guard when Platform Security Level with Secure Boot and Virtualization Based Security are both enabled.</span></span> <span data-ttu-id="1e76e-737">可取值为：`notConfigured`、`enableWithUEFILock`、`enableWithoutUEFILock`。</span><span class="sxs-lookup"><span data-stu-id="1e76e-737">Possible values are: `notConfigured`, `enableWithUEFILock`, `enableWithoutUEFILock`.</span></span>|
|<span data-ttu-id="1e76e-738">deviceGuardEnableVirtualizationBasedSecurity</span><span class="sxs-lookup"><span data-stu-id="1e76e-738">deviceGuardEnableVirtualizationBasedSecurity</span></span>|<span data-ttu-id="1e76e-739">Boolean</span><span class="sxs-lookup"><span data-stu-id="1e76e-739">Boolean</span></span>|<span data-ttu-id="1e76e-740">启用基于虚拟化的安全性（VBS）。</span><span class="sxs-lookup"><span data-stu-id="1e76e-740">Turns On Virtualization Based Security(VBS).</span></span>|
|<span data-ttu-id="1e76e-741">deviceGuardEnableSecureBootWithDMA</span><span class="sxs-lookup"><span data-stu-id="1e76e-741">deviceGuardEnableSecureBootWithDMA</span></span>|<span data-ttu-id="1e76e-742">Boolean</span><span class="sxs-lookup"><span data-stu-id="1e76e-742">Boolean</span></span>|<span data-ttu-id="1e76e-743">此属性将在5月2019中被弃用，并将替换为属性 DeviceGuardSecureBootWithDMA。</span><span class="sxs-lookup"><span data-stu-id="1e76e-743">This property will be deprecated in May 2019 and will be replaced with property DeviceGuardSecureBootWithDMA.</span></span> <span data-ttu-id="1e76e-744">指定是否在下次重新启动时启用平台安全级别。</span><span class="sxs-lookup"><span data-stu-id="1e76e-744">Specifies whether Platform Security Level is enabled at next reboot.</span></span>|
|<span data-ttu-id="1e76e-745">deviceGuardSecureBootWithDMA</span><span class="sxs-lookup"><span data-stu-id="1e76e-745">deviceGuardSecureBootWithDMA</span></span>|[<span data-ttu-id="1e76e-746">secureBootWithDMAType</span><span class="sxs-lookup"><span data-stu-id="1e76e-746">secureBootWithDMAType</span></span>](../resources/intune-deviceconfig-securebootwithdmatype.md)|<span data-ttu-id="1e76e-747">指定是否在下次重新启动时启用平台安全级别。</span><span class="sxs-lookup"><span data-stu-id="1e76e-747">Specifies whether Platform Security Level is enabled at next reboot.</span></span> <span data-ttu-id="1e76e-748">可取值为：`notConfigured`、`withoutDMA`、`withDMA`。</span><span class="sxs-lookup"><span data-stu-id="1e76e-748">Possible values are: `notConfigured`, `withoutDMA`, `withDMA`.</span></span>|
|<span data-ttu-id="1e76e-749">deviceGuardLaunchSystemGuard</span><span class="sxs-lookup"><span data-stu-id="1e76e-749">deviceGuardLaunchSystemGuard</span></span>|[<span data-ttu-id="1e76e-750">启用</span><span class="sxs-lookup"><span data-stu-id="1e76e-750">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="1e76e-751">允许 IT 管理员配置启动 "系统防护"。</span><span class="sxs-lookup"><span data-stu-id="1e76e-751">Allows the IT admin to configure the launch of System Guard.</span></span> <span data-ttu-id="1e76e-752">可取值为：`notConfigured`、`enabled`、`disabled`。</span><span class="sxs-lookup"><span data-stu-id="1e76e-752">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="1e76e-753">smartScreenEnableInShell</span><span class="sxs-lookup"><span data-stu-id="1e76e-753">smartScreenEnableInShell</span></span>|<span data-ttu-id="1e76e-754">Boolean</span><span class="sxs-lookup"><span data-stu-id="1e76e-754">Boolean</span></span>|<span data-ttu-id="1e76e-755">允许 IT 管理员配置适用于 Windows 的 SmartScreen。</span><span class="sxs-lookup"><span data-stu-id="1e76e-755">Allows IT Admins to configure SmartScreen for Windows.</span></span>|
|<span data-ttu-id="1e76e-756">smartScreenBlockOverrideForFiles</span><span class="sxs-lookup"><span data-stu-id="1e76e-756">smartScreenBlockOverrideForFiles</span></span>|<span data-ttu-id="1e76e-757">Boolean</span><span class="sxs-lookup"><span data-stu-id="1e76e-757">Boolean</span></span>|<span data-ttu-id="1e76e-758">允许 IT 管理员控制用户是否可以忽略 SmartScreen 警告并运行恶意文件。</span><span class="sxs-lookup"><span data-stu-id="1e76e-758">Allows IT Admins to control whether users can can ignore SmartScreen warnings and run malicious files.</span></span>|
|<span data-ttu-id="1e76e-759">applicationGuardEnabled</span><span class="sxs-lookup"><span data-stu-id="1e76e-759">applicationGuardEnabled</span></span>|<span data-ttu-id="1e76e-760">Boolean</span><span class="sxs-lookup"><span data-stu-id="1e76e-760">Boolean</span></span>|<span data-ttu-id="1e76e-761">启用 Windows Defender 应用程序防护</span><span class="sxs-lookup"><span data-stu-id="1e76e-761">Enable Windows Defender Application Guard</span></span>|
|<span data-ttu-id="1e76e-762">applicationGuardEnabledOptions</span><span class="sxs-lookup"><span data-stu-id="1e76e-762">applicationGuardEnabledOptions</span></span>|[<span data-ttu-id="1e76e-763">applicationGuardEnabledOptions</span><span class="sxs-lookup"><span data-stu-id="1e76e-763">applicationGuardEnabledOptions</span></span>](../resources/intune-deviceconfig-applicationguardenabledoptions.md)|<span data-ttu-id="1e76e-764">为较新的 Windows 版本启用 Windows Defender 应用程序防护。</span><span class="sxs-lookup"><span data-stu-id="1e76e-764">Enable Windows Defender Application Guard for newer Windows builds.</span></span> <span data-ttu-id="1e76e-765">可取值为：`notConfigured`、`enabledForEdge`、`enabledForOffice`、`enabledForEdgeAndOffice`。</span><span class="sxs-lookup"><span data-stu-id="1e76e-765">Possible values are: `notConfigured`, `enabledForEdge`, `enabledForOffice`, `enabledForEdgeAndOffice`.</span></span>|
|<span data-ttu-id="1e76e-766">applicationGuardBlockFileTransfer</span><span class="sxs-lookup"><span data-stu-id="1e76e-766">applicationGuardBlockFileTransfer</span></span>|[<span data-ttu-id="1e76e-767">applicationGuardBlockFileTransferType</span><span class="sxs-lookup"><span data-stu-id="1e76e-767">applicationGuardBlockFileTransferType</span></span>](../resources/intune-deviceconfig-applicationguardblockfiletransfertype.md)|<span data-ttu-id="1e76e-768">阻止剪贴板传输图像文件、文本文件或二者都不。</span><span class="sxs-lookup"><span data-stu-id="1e76e-768">Block clipboard to transfer image file, text file or neither of them.</span></span> <span data-ttu-id="1e76e-769">可取值为：`notConfigured`、`blockImageAndTextFile`、`blockImageFile`、`blockNone`、`blockTextFile`。</span><span class="sxs-lookup"><span data-stu-id="1e76e-769">Possible values are: `notConfigured`, `blockImageAndTextFile`, `blockImageFile`, `blockNone`, `blockTextFile`.</span></span>|
|<span data-ttu-id="1e76e-770">applicationGuardBlockNonEnterpriseContent</span><span class="sxs-lookup"><span data-stu-id="1e76e-770">applicationGuardBlockNonEnterpriseContent</span></span>|<span data-ttu-id="1e76e-771">Boolean</span><span class="sxs-lookup"><span data-stu-id="1e76e-771">Boolean</span></span>|<span data-ttu-id="1e76e-772">阻止企业站点加载非企业内容，例如第三方插件</span><span class="sxs-lookup"><span data-stu-id="1e76e-772">Block enterprise sites to load non-enterprise content, such as third party plug-ins</span></span>|
|<span data-ttu-id="1e76e-773">applicationGuardAllowPersistence</span><span class="sxs-lookup"><span data-stu-id="1e76e-773">applicationGuardAllowPersistence</span></span>|<span data-ttu-id="1e76e-774">Boolean</span><span class="sxs-lookup"><span data-stu-id="1e76e-774">Boolean</span></span>|<span data-ttu-id="1e76e-775">允许 App Guard 容器（收藏夹、Cookie、Web 密码等）内的持久用户生成数据</span><span class="sxs-lookup"><span data-stu-id="1e76e-775">Allow persisting user generated data inside the App Guard Containter (favorites, cookies, web passwords, etc.)</span></span>|
|<span data-ttu-id="1e76e-776">applicationGuardForceAuditing</span><span class="sxs-lookup"><span data-stu-id="1e76e-776">applicationGuardForceAuditing</span></span>|<span data-ttu-id="1e76e-777">Boolean</span><span class="sxs-lookup"><span data-stu-id="1e76e-777">Boolean</span></span>|<span data-ttu-id="1e76e-778">强制审核将存留 Windows 日志和事件以满足安全/符合性条件（示例事件是用户登录注销、特权使用、软件安装、系统更改等）</span><span class="sxs-lookup"><span data-stu-id="1e76e-778">Force auditing will persist Windows logs and events to meet security/compliance criteria (sample events are user login-logoff, use of privilege rights, software installation, system changes, etc.)</span></span>|
|<span data-ttu-id="1e76e-779">applicationGuardBlockClipboardSharing</span><span class="sxs-lookup"><span data-stu-id="1e76e-779">applicationGuardBlockClipboardSharing</span></span>|[<span data-ttu-id="1e76e-780">applicationGuardBlockClipboardSharingType</span><span class="sxs-lookup"><span data-stu-id="1e76e-780">applicationGuardBlockClipboardSharingType</span></span>](../resources/intune-deviceconfig-applicationguardblockclipboardsharingtype.md)|<span data-ttu-id="1e76e-781">阻止剪贴板将数据从主机共享到容器或从容器共享到主机，或阻止两种方式，或两种方式均不阻止。</span><span class="sxs-lookup"><span data-stu-id="1e76e-781">Block clipboard to share data from Host to Container, or from Container to Host, or both ways, or neither ways.</span></span> <span data-ttu-id="1e76e-782">可取值为：`notConfigured`、`blockBoth`、`blockHostToContainer`、`blockContainerToHost`、`blockNone`。</span><span class="sxs-lookup"><span data-stu-id="1e76e-782">Possible values are: `notConfigured`, `blockBoth`, `blockHostToContainer`, `blockContainerToHost`, `blockNone`.</span></span>|
|<span data-ttu-id="1e76e-783">applicationGuardAllowPrintToPDF</span><span class="sxs-lookup"><span data-stu-id="1e76e-783">applicationGuardAllowPrintToPDF</span></span>|<span data-ttu-id="1e76e-784">Boolean</span><span class="sxs-lookup"><span data-stu-id="1e76e-784">Boolean</span></span>|<span data-ttu-id="1e76e-785">允许从容器打印为 PDF 格式</span><span class="sxs-lookup"><span data-stu-id="1e76e-785">Allow printing to PDF from Container</span></span>|
|<span data-ttu-id="1e76e-786">applicationGuardAllowPrintToXPS</span><span class="sxs-lookup"><span data-stu-id="1e76e-786">applicationGuardAllowPrintToXPS</span></span>|<span data-ttu-id="1e76e-787">Boolean</span><span class="sxs-lookup"><span data-stu-id="1e76e-787">Boolean</span></span>|<span data-ttu-id="1e76e-788">允许从容器打印为 XPS 格式</span><span class="sxs-lookup"><span data-stu-id="1e76e-788">Allow printing to XPS from Container</span></span>|
|<span data-ttu-id="1e76e-789">applicationGuardAllowPrintToLocalPrinters</span><span class="sxs-lookup"><span data-stu-id="1e76e-789">applicationGuardAllowPrintToLocalPrinters</span></span>|<span data-ttu-id="1e76e-790">Boolean</span><span class="sxs-lookup"><span data-stu-id="1e76e-790">Boolean</span></span>|<span data-ttu-id="1e76e-791">允许从容器打印到本地打印机</span><span class="sxs-lookup"><span data-stu-id="1e76e-791">Allow printing to Local Printers from Container</span></span>|
|<span data-ttu-id="1e76e-792">applicationGuardAllowPrintToNetworkPrinters</span><span class="sxs-lookup"><span data-stu-id="1e76e-792">applicationGuardAllowPrintToNetworkPrinters</span></span>|<span data-ttu-id="1e76e-793">Boolean</span><span class="sxs-lookup"><span data-stu-id="1e76e-793">Boolean</span></span>|<span data-ttu-id="1e76e-794">允许从容器打印到网络打印机</span><span class="sxs-lookup"><span data-stu-id="1e76e-794">Allow printing to Network Printers from Container</span></span>|
|<span data-ttu-id="1e76e-795">applicationGuardAllowVirtualGPU</span><span class="sxs-lookup"><span data-stu-id="1e76e-795">applicationGuardAllowVirtualGPU</span></span>|<span data-ttu-id="1e76e-796">Boolean</span><span class="sxs-lookup"><span data-stu-id="1e76e-796">Boolean</span></span>|<span data-ttu-id="1e76e-797">允许应用程序防护使用虚拟 GPU</span><span class="sxs-lookup"><span data-stu-id="1e76e-797">Allow application guard to use virtual GPU</span></span>|
|<span data-ttu-id="1e76e-798">applicationGuardAllowFileSaveOnHost</span><span class="sxs-lookup"><span data-stu-id="1e76e-798">applicationGuardAllowFileSaveOnHost</span></span>|<span data-ttu-id="1e76e-799">Boolean</span><span class="sxs-lookup"><span data-stu-id="1e76e-799">Boolean</span></span>|<span data-ttu-id="1e76e-800">允许用户从应用程序防护容器中的边缘下载文件并将其保存在主机文件系统上</span><span class="sxs-lookup"><span data-stu-id="1e76e-800">Allow users to download files from Edge in the application guard container and save them on the host file system</span></span>|
|<span data-ttu-id="1e76e-801">bitLockerAllowStandardUserEncryption</span><span class="sxs-lookup"><span data-stu-id="1e76e-801">bitLockerAllowStandardUserEncryption</span></span>|<span data-ttu-id="1e76e-802">Boolean</span><span class="sxs-lookup"><span data-stu-id="1e76e-802">Boolean</span></span>|<span data-ttu-id="1e76e-803">允许管理员允许标准用户在 Azure AD 加入过程中启用 encrpytion。</span><span class="sxs-lookup"><span data-stu-id="1e76e-803">Allows the admin to allow standard users to enable encrpytion during Azure AD Join.</span></span>|
|<span data-ttu-id="1e76e-804">bitLockerDisableWarningForOtherDiskEncryption</span><span class="sxs-lookup"><span data-stu-id="1e76e-804">bitLockerDisableWarningForOtherDiskEncryption</span></span>|<span data-ttu-id="1e76e-805">Boolean</span><span class="sxs-lookup"><span data-stu-id="1e76e-805">Boolean</span></span>|<span data-ttu-id="1e76e-806">允许管理员禁用对用户计算机上其他磁盘加密的警告提示。</span><span class="sxs-lookup"><span data-stu-id="1e76e-806">Allows the Admin to disable the warning prompt for other disk encryption on the user machines.</span></span>|
|<span data-ttu-id="1e76e-807">bitLockerEnableStorageCardEncryptionOnMobile</span><span class="sxs-lookup"><span data-stu-id="1e76e-807">bitLockerEnableStorageCardEncryptionOnMobile</span></span>|<span data-ttu-id="1e76e-808">Boolean</span><span class="sxs-lookup"><span data-stu-id="1e76e-808">Boolean</span></span>|<span data-ttu-id="1e76e-809">允许管理员要求使用 BitLocker 开启加密功能。</span><span class="sxs-lookup"><span data-stu-id="1e76e-809">Allows the admin to require encryption to be turned on using BitLocker.</span></span> <span data-ttu-id="1e76e-810">此策略仅适用于移动 SKU。</span><span class="sxs-lookup"><span data-stu-id="1e76e-810">This policy is valid only for a mobile SKU.</span></span>|
|<span data-ttu-id="1e76e-811">bitLockerEncryptDevice</span><span class="sxs-lookup"><span data-stu-id="1e76e-811">bitLockerEncryptDevice</span></span>|<span data-ttu-id="1e76e-812">Boolean</span><span class="sxs-lookup"><span data-stu-id="1e76e-812">Boolean</span></span>|<span data-ttu-id="1e76e-813">允许管理员要求使用 BitLocker 开启加密功能。</span><span class="sxs-lookup"><span data-stu-id="1e76e-813">Allows the admin to require encryption to be turned on using BitLocker.</span></span>|
|<span data-ttu-id="1e76e-814">bitLockerSystemDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="1e76e-814">bitLockerSystemDrivePolicy</span></span>|[<span data-ttu-id="1e76e-815">bitLockerSystemDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="1e76e-815">bitLockerSystemDrivePolicy</span></span>](../resources/intune-deviceconfig-bitlockersystemdrivepolicy.md)|<span data-ttu-id="1e76e-816">BitLocker 系统驱动器策略。</span><span class="sxs-lookup"><span data-stu-id="1e76e-816">BitLocker System Drive Policy.</span></span>|
|<span data-ttu-id="1e76e-817">bitLockerFixedDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="1e76e-817">bitLockerFixedDrivePolicy</span></span>|[<span data-ttu-id="1e76e-818">bitLockerFixedDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="1e76e-818">bitLockerFixedDrivePolicy</span></span>](../resources/intune-deviceconfig-bitlockerfixeddrivepolicy.md)|<span data-ttu-id="1e76e-819">BitLocker 固定驱动器策略。</span><span class="sxs-lookup"><span data-stu-id="1e76e-819">BitLocker Fixed Drive Policy.</span></span>|
|<span data-ttu-id="1e76e-820">bitLockerRemovableDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="1e76e-820">bitLockerRemovableDrivePolicy</span></span>|[<span data-ttu-id="1e76e-821">bitLockerRemovableDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="1e76e-821">bitLockerRemovableDrivePolicy</span></span>](../resources/intune-deviceconfig-bitlockerremovabledrivepolicy.md)|<span data-ttu-id="1e76e-822">BitLocker 可移动驱动器策略。</span><span class="sxs-lookup"><span data-stu-id="1e76e-822">BitLocker Removable Drive Policy.</span></span>|
|<span data-ttu-id="1e76e-823">bitLockerRecoveryPasswordRotation</span><span class="sxs-lookup"><span data-stu-id="1e76e-823">bitLockerRecoveryPasswordRotation</span></span>|[<span data-ttu-id="1e76e-824">bitLockerRecoveryPasswordRotationType</span><span class="sxs-lookup"><span data-stu-id="1e76e-824">bitLockerRecoveryPasswordRotationType</span></span>](../resources/intune-deviceconfig-bitlockerrecoverypasswordrotationtype.md)|<span data-ttu-id="1e76e-825">此设置在操作系统驱动器恢复后启动客户端驱动的恢复密码轮替（使用 bootmgr 或 WinRE）。</span><span class="sxs-lookup"><span data-stu-id="1e76e-825">This setting initiates a client-driven recovery password rotation after an OS drive recovery (either by using bootmgr or WinRE).</span></span> <span data-ttu-id="1e76e-826">可取值为：`notConfigured`、`disabled`、`enabledForAzureAd`、`enabledForAzureAdAndHybrid`。</span><span class="sxs-lookup"><span data-stu-id="1e76e-826">Possible values are: `notConfigured`, `disabled`, `enabledForAzureAd`, `enabledForAzureAdAndHybrid`.</span></span>|



## <a name="response"></a><span data-ttu-id="1e76e-827">响应</span><span class="sxs-lookup"><span data-stu-id="1e76e-827">Response</span></span>
<span data-ttu-id="1e76e-828">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="1e76e-828">If successful, this method returns a `200 OK` response code and an updated [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1e76e-829">示例</span><span class="sxs-lookup"><span data-stu-id="1e76e-829">Example</span></span>

### <a name="request"></a><span data-ttu-id="1e76e-830">请求</span><span class="sxs-lookup"><span data-stu-id="1e76e-830">Request</span></span>
<span data-ttu-id="1e76e-831">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="1e76e-831">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 28662

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
  "attackSurfaceReductionRules": "Attack Surface Reduction Rules value",
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
  "bitLockerRecoveryPasswordRotation": "disabled"
}
```

### <a name="response"></a><span data-ttu-id="1e76e-832">响应</span><span class="sxs-lookup"><span data-stu-id="1e76e-832">Response</span></span>
<span data-ttu-id="1e76e-p206">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="1e76e-p206">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 28834

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
  "attackSurfaceReductionRules": "Attack Surface Reduction Rules value",
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
  "bitLockerRecoveryPasswordRotation": "disabled"
}
```




