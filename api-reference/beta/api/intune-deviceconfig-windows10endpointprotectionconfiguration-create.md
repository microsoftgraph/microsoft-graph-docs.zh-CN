---
title: 创建 windows10EndpointProtectionConfiguration
description: 创建新的 windows10EndpointProtectionConfiguration 对象。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5b6a9f73f7e44b288ec5fa60851c193392c42508
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/14/2019
ms.locfileid: "34976076"
---
# <a name="create-windows10endpointprotectionconfiguration"></a><span data-ttu-id="65bc6-103">创建 windows10EndpointProtectionConfiguration</span><span class="sxs-lookup"><span data-stu-id="65bc6-103">Create windows10EndpointProtectionConfiguration</span></span>

> <span data-ttu-id="65bc6-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="65bc6-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="65bc6-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="65bc6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="65bc6-106">创建新的 [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="65bc6-106">Create a new [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="65bc6-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="65bc6-107">Prerequisites</span></span>
<span data-ttu-id="65bc6-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="65bc6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="65bc6-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="65bc6-110">Permission type</span></span>|<span data-ttu-id="65bc6-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="65bc6-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="65bc6-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="65bc6-112">Delegated (work or school account)</span></span>|<span data-ttu-id="65bc6-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="65bc6-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="65bc6-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="65bc6-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="65bc6-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="65bc6-115">Not supported.</span></span>|
|<span data-ttu-id="65bc6-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="65bc6-116">Application</span></span>|<span data-ttu-id="65bc6-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="65bc6-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="65bc6-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="65bc6-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="65bc6-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="65bc6-119">Request headers</span></span>
|<span data-ttu-id="65bc6-120">标头</span><span class="sxs-lookup"><span data-stu-id="65bc6-120">Header</span></span>|<span data-ttu-id="65bc6-121">值</span><span class="sxs-lookup"><span data-stu-id="65bc6-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="65bc6-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="65bc6-122">Authorization</span></span>|<span data-ttu-id="65bc6-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="65bc6-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="65bc6-124">接受</span><span class="sxs-lookup"><span data-stu-id="65bc6-124">Accept</span></span>|<span data-ttu-id="65bc6-125">application/json</span><span class="sxs-lookup"><span data-stu-id="65bc6-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="65bc6-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="65bc6-126">Request body</span></span>
<span data-ttu-id="65bc6-127">在请求正文中，提供 windows10EndpointProtectionConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="65bc6-127">In the request body, supply a JSON representation for the windows10EndpointProtectionConfiguration object.</span></span>

<span data-ttu-id="65bc6-128">下表显示了创建 windows10EndpointProtectionConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="65bc6-128">The following table shows the properties that are required when you create the windows10EndpointProtectionConfiguration.</span></span>

|<span data-ttu-id="65bc6-129">属性</span><span class="sxs-lookup"><span data-stu-id="65bc6-129">Property</span></span>|<span data-ttu-id="65bc6-130">类型</span><span class="sxs-lookup"><span data-stu-id="65bc6-130">Type</span></span>|<span data-ttu-id="65bc6-131">说明</span><span class="sxs-lookup"><span data-stu-id="65bc6-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="65bc6-132">id</span><span class="sxs-lookup"><span data-stu-id="65bc6-132">id</span></span>|<span data-ttu-id="65bc6-133">字符串</span><span class="sxs-lookup"><span data-stu-id="65bc6-133">String</span></span>|<span data-ttu-id="65bc6-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="65bc6-134">Key of the entity.</span></span> <span data-ttu-id="65bc6-135">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="65bc6-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="65bc6-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="65bc6-136">lastModifiedDateTime</span></span>|<span data-ttu-id="65bc6-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="65bc6-137">DateTimeOffset</span></span>|<span data-ttu-id="65bc6-138">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="65bc6-138">DateTime the object was last modified.</span></span> <span data-ttu-id="65bc6-139">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="65bc6-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="65bc6-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="65bc6-140">roleScopeTagIds</span></span>|<span data-ttu-id="65bc6-141">String collection</span><span class="sxs-lookup"><span data-stu-id="65bc6-141">String collection</span></span>|<span data-ttu-id="65bc6-142">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="65bc6-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="65bc6-143">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="65bc6-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="65bc6-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="65bc6-144">supportsScopeTags</span></span>|<span data-ttu-id="65bc6-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="65bc6-145">Boolean</span></span>|<span data-ttu-id="65bc6-146">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="65bc6-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="65bc6-147">如果此值为 false, 则不允许分配给 ScopeTags 属性, 并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="65bc6-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="65bc6-148">这适用于在 Silverlight 中创建的旧版策略, 可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="65bc6-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="65bc6-149">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="65bc6-149">This property is read-only.</span></span> <span data-ttu-id="65bc6-150">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="65bc6-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="65bc6-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="65bc6-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="65bc6-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="65bc6-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="65bc6-153">适用于此策略的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="65bc6-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="65bc6-154">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="65bc6-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="65bc6-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="65bc6-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="65bc6-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="65bc6-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="65bc6-157">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="65bc6-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="65bc6-158">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="65bc6-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="65bc6-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="65bc6-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="65bc6-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="65bc6-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="65bc6-161">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="65bc6-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="65bc6-162">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="65bc6-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="65bc6-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="65bc6-163">createdDateTime</span></span>|<span data-ttu-id="65bc6-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="65bc6-164">DateTimeOffset</span></span>|<span data-ttu-id="65bc6-165">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="65bc6-165">DateTime the object was created.</span></span> <span data-ttu-id="65bc6-166">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="65bc6-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="65bc6-167">说明</span><span class="sxs-lookup"><span data-stu-id="65bc6-167">description</span></span>|<span data-ttu-id="65bc6-168">String</span><span class="sxs-lookup"><span data-stu-id="65bc6-168">String</span></span>|<span data-ttu-id="65bc6-169">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="65bc6-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="65bc6-170">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="65bc6-170">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="65bc6-171">displayName</span><span class="sxs-lookup"><span data-stu-id="65bc6-171">displayName</span></span>|<span data-ttu-id="65bc6-172">String</span><span class="sxs-lookup"><span data-stu-id="65bc6-172">String</span></span>|<span data-ttu-id="65bc6-173">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="65bc6-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="65bc6-174">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="65bc6-174">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="65bc6-175">version</span><span class="sxs-lookup"><span data-stu-id="65bc6-175">version</span></span>|<span data-ttu-id="65bc6-176">Int32</span><span class="sxs-lookup"><span data-stu-id="65bc6-176">Int32</span></span>|<span data-ttu-id="65bc6-177">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="65bc6-177">Version of the device configuration.</span></span> <span data-ttu-id="65bc6-178">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="65bc6-178">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="65bc6-179">dmaGuardDeviceEnumerationPolicy</span><span class="sxs-lookup"><span data-stu-id="65bc6-179">dmaGuardDeviceEnumerationPolicy</span></span>|[<span data-ttu-id="65bc6-180">dmaGuardDeviceEnumerationPolicyType</span><span class="sxs-lookup"><span data-stu-id="65bc6-180">dmaGuardDeviceEnumerationPolicyType</span></span>](../resources/intune-deviceconfig-dmaguarddeviceenumerationpolicytype.md)|<span data-ttu-id="65bc6-181">此策略旨在提供针对支持外部 DMA 的设备的额外安全性。</span><span class="sxs-lookup"><span data-stu-id="65bc6-181">This policy is intended to provide additional security against external DMA capable devices.</span></span> <span data-ttu-id="65bc6-182">通过它, 可以更好地控制支持外部 DMA 的设备与 DMA 重新映射/设备内存隔离和沙盒不兼容的枚举。</span><span class="sxs-lookup"><span data-stu-id="65bc6-182">It allows for more control over the enumeration of external DMA capable devices incompatible with DMA Remapping/device memory isolation and sandboxing.</span></span> <span data-ttu-id="65bc6-183">仅当系统固件支持和启用内核 DMA 保护时, 此策略才会生效。</span><span class="sxs-lookup"><span data-stu-id="65bc6-183">This policy only takes effect when Kernel DMA Protection is supported and enabled by the system firmware.</span></span> <span data-ttu-id="65bc6-184">内核 DMA 保护是一项平台功能, 不能通过策略或最终用户进行控制。</span><span class="sxs-lookup"><span data-stu-id="65bc6-184">Kernel DMA Protection is a platform feature that cannot be controlled via policy or by end user.</span></span> <span data-ttu-id="65bc6-185">在制造时, 系统必须支持它。</span><span class="sxs-lookup"><span data-stu-id="65bc6-185">It has to be supported by the system at the time of manufacturing.</span></span> <span data-ttu-id="65bc6-186">若要检查系统是否支持内核 DMA 保护, 请在 MSINFO32 的摘要页中检查 "内核 DMA 保护" 字段。</span><span class="sxs-lookup"><span data-stu-id="65bc6-186">To check if the system supports Kernel DMA Protection, please check the Kernel DMA Protection field in the Summary page of MSINFO32.exe.</span></span> <span data-ttu-id="65bc6-187">可取值为：`deviceDefault`、`blockAll`、`allowAll`。</span><span class="sxs-lookup"><span data-stu-id="65bc6-187">Possible values are: `deviceDefault`, `blockAll`, `allowAll`.</span></span>|
|<span data-ttu-id="65bc6-188">firewallRules</span><span class="sxs-lookup"><span data-stu-id="65bc6-188">firewallRules</span></span>|<span data-ttu-id="65bc6-189">[windowsFirewallRule](../resources/intune-deviceconfig-windowsfirewallrule.md)集合</span><span class="sxs-lookup"><span data-stu-id="65bc6-189">[windowsFirewallRule](../resources/intune-deviceconfig-windowsfirewallrule.md) collection</span></span>|<span data-ttu-id="65bc6-190">配置防火墙规则设置。</span><span class="sxs-lookup"><span data-stu-id="65bc6-190">Configures the firewall rule settings.</span></span> <span data-ttu-id="65bc6-191">此集合最多可包含150个元素。</span><span class="sxs-lookup"><span data-stu-id="65bc6-191">This collection can contain a maximum of 150 elements.</span></span>|
|<span data-ttu-id="65bc6-192">userRightsAccessCredentialManagerAsTrustedCaller</span><span class="sxs-lookup"><span data-stu-id="65bc6-192">userRightsAccessCredentialManagerAsTrustedCaller</span></span>|[<span data-ttu-id="65bc6-193">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="65bc6-193">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="65bc6-194">此用户权限由凭据管理器在备份/还原过程中使用。</span><span class="sxs-lookup"><span data-stu-id="65bc6-194">This user right is used by Credential Manager during Backup/Restore.</span></span> <span data-ttu-id="65bc6-195">如果为其他实体提供此权限, 则用户保存的凭据可能会受到威胁。</span><span class="sxs-lookup"><span data-stu-id="65bc6-195">Users' saved credentials might be compromised if this privilege is given to other entities.</span></span> <span data-ttu-id="65bc6-196">仅支持 NotConfigured 和允许的状态</span><span class="sxs-lookup"><span data-stu-id="65bc6-196">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="65bc6-197">userRightsAllowAccessFromNetwork</span><span class="sxs-lookup"><span data-stu-id="65bc6-197">userRightsAllowAccessFromNetwork</span></span>|[<span data-ttu-id="65bc6-198">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="65bc6-198">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="65bc6-199">此用户权限确定允许哪些用户和组通过网络连接到计算机。</span><span class="sxs-lookup"><span data-stu-id="65bc6-199">This user right determines which users and groups are allowed to connect to the computer over the network.</span></span> <span data-ttu-id="65bc6-200">支持的状态为 "允许"。</span><span class="sxs-lookup"><span data-stu-id="65bc6-200">State Allowed is supported.</span></span>|
|<span data-ttu-id="65bc6-201">userRightsBlockAccessFromNetwork</span><span class="sxs-lookup"><span data-stu-id="65bc6-201">userRightsBlockAccessFromNetwork</span></span>|[<span data-ttu-id="65bc6-202">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="65bc6-202">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="65bc6-203">此用户权限决定了阻止哪些用户和组通过网络连接到计算机。</span><span class="sxs-lookup"><span data-stu-id="65bc6-203">This user right determines which users and groups are block from connecting to the computer over the network.</span></span> <span data-ttu-id="65bc6-204">支持状态块。</span><span class="sxs-lookup"><span data-stu-id="65bc6-204">State Block is supported.</span></span>|
|<span data-ttu-id="65bc6-205">userRightsActAsPartOfTheOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="65bc6-205">userRightsActAsPartOfTheOperatingSystem</span></span>|[<span data-ttu-id="65bc6-206">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="65bc6-206">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="65bc6-207">此用户权限允许进程在不进行身份验证的情况下模拟任何用户。</span><span class="sxs-lookup"><span data-stu-id="65bc6-207">This user right allows a process to impersonate any user without authentication.</span></span> <span data-ttu-id="65bc6-208">因此, 该过程可以获得与该用户相同的本地资源的访问权限。</span><span class="sxs-lookup"><span data-stu-id="65bc6-208">The process can therefore gain access to the same local resources as that user.</span></span> <span data-ttu-id="65bc6-209">仅支持 NotConfigured 和允许的状态</span><span class="sxs-lookup"><span data-stu-id="65bc6-209">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="65bc6-210">userRightsLocalLogOn</span><span class="sxs-lookup"><span data-stu-id="65bc6-210">userRightsLocalLogOn</span></span>|[<span data-ttu-id="65bc6-211">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="65bc6-211">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="65bc6-212">此用户权限确定哪些用户可以登录到计算机。</span><span class="sxs-lookup"><span data-stu-id="65bc6-212">This user right determines which users can log on to the computer.</span></span> <span data-ttu-id="65bc6-213">所有支持的状态 NotConfigured、允许和阻止</span><span class="sxs-lookup"><span data-stu-id="65bc6-213">States NotConfigured, Allowed and Blocked are all supported</span></span> |
|<span data-ttu-id="65bc6-214">userRightsBackupData</span><span class="sxs-lookup"><span data-stu-id="65bc6-214">userRightsBackupData</span></span>|[<span data-ttu-id="65bc6-215">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="65bc6-215">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="65bc6-216">此用户权限确定在备份文件和目录时, 哪些用户可以绕过文件、目录、注册表和其他持久对象权限。</span><span class="sxs-lookup"><span data-stu-id="65bc6-216">This user right determines which users can bypass file, directory, registry, and other persistent objects permissions when backing up files and directories.</span></span> <span data-ttu-id="65bc6-217">仅支持 NotConfigured 和允许的状态</span><span class="sxs-lookup"><span data-stu-id="65bc6-217">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="65bc6-218">userRightsChangeSystemTime</span><span class="sxs-lookup"><span data-stu-id="65bc6-218">userRightsChangeSystemTime</span></span>|[<span data-ttu-id="65bc6-219">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="65bc6-219">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="65bc6-220">此用户权限确定哪些用户和组可以更改计算机内部时钟上的时间和日期。</span><span class="sxs-lookup"><span data-stu-id="65bc6-220">This user right determines which users and groups can change the time and date on the internal clock of the computer.</span></span> <span data-ttu-id="65bc6-221">仅支持 NotConfigured 和允许的状态</span><span class="sxs-lookup"><span data-stu-id="65bc6-221">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="65bc6-222">userRightsCreateGlobalObjects</span><span class="sxs-lookup"><span data-stu-id="65bc6-222">userRightsCreateGlobalObjects</span></span>|[<span data-ttu-id="65bc6-223">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="65bc6-223">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="65bc6-224">此安全设置确定用户是否可以创建可用于所有会话的全局对象。</span><span class="sxs-lookup"><span data-stu-id="65bc6-224">This security setting determines whether users can create global objects that are available to all sessions.</span></span> <span data-ttu-id="65bc6-225">可以创建全局对象的用户可能会影响在其他用户的会话下运行的进程, 这可能导致应用程序故障或数据损坏。</span><span class="sxs-lookup"><span data-stu-id="65bc6-225">Users who can create global objects could affect processes that run under other users' sessions, which could lead to application failure or data corruption.</span></span> <span data-ttu-id="65bc6-226">仅支持 NotConfigured 和允许的状态</span><span class="sxs-lookup"><span data-stu-id="65bc6-226">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="65bc6-227">userRightsCreatePageFile</span><span class="sxs-lookup"><span data-stu-id="65bc6-227">userRightsCreatePageFile</span></span>|[<span data-ttu-id="65bc6-228">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="65bc6-228">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="65bc6-229">此用户权限确定哪些用户和组可以调用内部 API 来创建和更改页面文件的大小。</span><span class="sxs-lookup"><span data-stu-id="65bc6-229">This user right determines which users and groups can call an internal API to create and change the size of a page file.</span></span> <span data-ttu-id="65bc6-230">仅支持 NotConfigured 和允许的状态</span><span class="sxs-lookup"><span data-stu-id="65bc6-230">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="65bc6-231">userRightsCreatePermanentSharedObjects</span><span class="sxs-lookup"><span data-stu-id="65bc6-231">userRightsCreatePermanentSharedObjects</span></span>|[<span data-ttu-id="65bc6-232">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="65bc6-232">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="65bc6-233">此用户权限决定了进程可以使用哪些帐户使用对象管理器创建目录对象。</span><span class="sxs-lookup"><span data-stu-id="65bc6-233">This user right determines which accounts can be used by processes to create a directory object using the object manager.</span></span> <span data-ttu-id="65bc6-234">仅支持 NotConfigured 和允许的状态</span><span class="sxs-lookup"><span data-stu-id="65bc6-234">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="65bc6-235">userRightsCreateSymbolicLinks</span><span class="sxs-lookup"><span data-stu-id="65bc6-235">userRightsCreateSymbolicLinks</span></span>|[<span data-ttu-id="65bc6-236">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="65bc6-236">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="65bc6-237">此用户权限确定用户是否可以从其登录到的计算机创建符号链接。</span><span class="sxs-lookup"><span data-stu-id="65bc6-237">This user right determines if the user can create a symbolic link from the computer to which they are logged on.</span></span> <span data-ttu-id="65bc6-238">仅支持 NotConfigured 和允许的状态</span><span class="sxs-lookup"><span data-stu-id="65bc6-238">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="65bc6-239">userRightsCreateToken</span><span class="sxs-lookup"><span data-stu-id="65bc6-239">userRightsCreateToken</span></span>|[<span data-ttu-id="65bc6-240">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="65bc6-240">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="65bc6-241">此用户权限确定进程在使用内部 API 创建访问令牌时, 可以使用哪些用户/组来创建令牌, 然后可以使用这些用户/组来获取对任何本地资源的访问权限。</span><span class="sxs-lookup"><span data-stu-id="65bc6-241">This user right determines which users/groups can be used by processes to create a token that can then be used to get access to any local resources when the process uses an internal API to create an access token.</span></span> <span data-ttu-id="65bc6-242">仅支持 NotConfigured 和允许的状态</span><span class="sxs-lookup"><span data-stu-id="65bc6-242">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="65bc6-243">userRightsDebugPrograms</span><span class="sxs-lookup"><span data-stu-id="65bc6-243">userRightsDebugPrograms</span></span>|[<span data-ttu-id="65bc6-244">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="65bc6-244">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="65bc6-245">此用户权限确定哪些用户可以将调试程序附加到任何进程或内核。</span><span class="sxs-lookup"><span data-stu-id="65bc6-245">This user right determines which users can attach a debugger to any process or to the kernel.</span></span> <span data-ttu-id="65bc6-246">仅支持 NotConfigured 和允许的状态</span><span class="sxs-lookup"><span data-stu-id="65bc6-246">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="65bc6-247">userRightsRemoteDesktopServicesLogOn</span><span class="sxs-lookup"><span data-stu-id="65bc6-247">userRightsRemoteDesktopServicesLogOn</span></span>|[<span data-ttu-id="65bc6-248">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="65bc6-248">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="65bc6-249">此用户权限确定禁止哪些用户和组作为远程桌面服务客户端进行登录。</span><span class="sxs-lookup"><span data-stu-id="65bc6-249">This user right determines which users and groups are prohibited from logging on as a Remote Desktop Services client.</span></span> <span data-ttu-id="65bc6-250">仅支持状态 NotConfigured 和阻止</span><span class="sxs-lookup"><span data-stu-id="65bc6-250">Only states NotConfigured and Blocked are supported</span></span>|
|<span data-ttu-id="65bc6-251">userRightsDelegation</span><span class="sxs-lookup"><span data-stu-id="65bc6-251">userRightsDelegation</span></span>|[<span data-ttu-id="65bc6-252">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="65bc6-252">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="65bc6-253">此用户权限确定哪些用户可以在用户或计算机对象上设置受信任委派设置。</span><span class="sxs-lookup"><span data-stu-id="65bc6-253">This user right determines which users can set the Trusted for Delegation setting on a user or computer object.</span></span> <span data-ttu-id="65bc6-254">仅支持 NotConfigured 和允许的状态。</span><span class="sxs-lookup"><span data-stu-id="65bc6-254">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="65bc6-255">userRightsGenerateSecurityAudits</span><span class="sxs-lookup"><span data-stu-id="65bc6-255">userRightsGenerateSecurityAudits</span></span>|[<span data-ttu-id="65bc6-256">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="65bc6-256">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="65bc6-257">此用户权限确定进程可使用哪些帐户向安全日志中添加条目。</span><span class="sxs-lookup"><span data-stu-id="65bc6-257">This user right determines which accounts can be used by a process to add entries to the security log.</span></span> <span data-ttu-id="65bc6-258">安全日志用于跟踪未经授权的系统访问。</span><span class="sxs-lookup"><span data-stu-id="65bc6-258">The security log is used to trace unauthorized system access.</span></span>  <span data-ttu-id="65bc6-259">仅支持 NotConfigured 和允许的状态。</span><span class="sxs-lookup"><span data-stu-id="65bc6-259">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="65bc6-260">userRightsImpersonateClient</span><span class="sxs-lookup"><span data-stu-id="65bc6-260">userRightsImpersonateClient</span></span>|[<span data-ttu-id="65bc6-261">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="65bc6-261">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="65bc6-262">将此用户权限分配给用户将允许代表该用户运行的程序模拟客户端。</span><span class="sxs-lookup"><span data-stu-id="65bc6-262">Assigning this user right to a user allows programs running on behalf of that user to impersonate a client.</span></span> <span data-ttu-id="65bc6-263">如果此类型的模拟要求此用户权限, 则可以防止未经授权的用户说服客户端连接到已创建的服务, 然后模拟该客户端, 这样可以将未经授权的用户的权限提升到管理级别或系统级别。</span><span class="sxs-lookup"><span data-stu-id="65bc6-263">Requiring this user right for this kind of impersonation prevents an unauthorized user from convincing a client to connect to a service that they have created and then impersonating that client, which can elevate the unauthorized user's permissions to administrative or system levels.</span></span> <span data-ttu-id="65bc6-264">仅支持 NotConfigured 和允许的状态。</span><span class="sxs-lookup"><span data-stu-id="65bc6-264">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="65bc6-265">userRightsIncreaseSchedulingPriority</span><span class="sxs-lookup"><span data-stu-id="65bc6-265">userRightsIncreaseSchedulingPriority</span></span>|[<span data-ttu-id="65bc6-266">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="65bc6-266">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="65bc6-267">此用户权限确定哪些帐户可以使用具有对另一进程的 Write 属性访问权限的进程, 以增加分配给其他进程的执行优先级。</span><span class="sxs-lookup"><span data-stu-id="65bc6-267">This user right determines which accounts can use a process with Write Property access to another process to increase the execution priority assigned to the other process.</span></span> <span data-ttu-id="65bc6-268">仅支持 NotConfigured 和允许的状态。</span><span class="sxs-lookup"><span data-stu-id="65bc6-268">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="65bc6-269">userRightsLoadUnloadDrivers</span><span class="sxs-lookup"><span data-stu-id="65bc6-269">userRightsLoadUnloadDrivers</span></span>|[<span data-ttu-id="65bc6-270">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="65bc6-270">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="65bc6-271">此用户权限确定哪些用户可以在内核模式下将设备驱动程序或其他代码动态加载和卸载。</span><span class="sxs-lookup"><span data-stu-id="65bc6-271">This user right determines which users can dynamically load and unload device drivers or other code in to kernel mode.</span></span> <span data-ttu-id="65bc6-272">仅支持 NotConfigured 和允许的状态。</span><span class="sxs-lookup"><span data-stu-id="65bc6-272">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="65bc6-273">userRightsLockMemory</span><span class="sxs-lookup"><span data-stu-id="65bc6-273">userRightsLockMemory</span></span>|[<span data-ttu-id="65bc6-274">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="65bc6-274">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="65bc6-275">此用户权限确定哪些帐户可以使用进程将数据保存在物理内存中, 这会阻止系统将数据分页到磁盘上的虚拟内存中。</span><span class="sxs-lookup"><span data-stu-id="65bc6-275">This user right determines which accounts can use a process to keep data in physical memory, which prevents the system from paging the data to virtual memory on disk.</span></span> <span data-ttu-id="65bc6-276">仅支持 NotConfigured 和允许的状态。</span><span class="sxs-lookup"><span data-stu-id="65bc6-276">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="65bc6-277">userRightsManageAuditingAndSecurityLogs</span><span class="sxs-lookup"><span data-stu-id="65bc6-277">userRightsManageAuditingAndSecurityLogs</span></span>|[<span data-ttu-id="65bc6-278">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="65bc6-278">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="65bc6-279">此用户权限确定哪些用户可以为各个资源 (如文件、Active Directory 对象和注册表项) 指定对象访问审核选项。</span><span class="sxs-lookup"><span data-stu-id="65bc6-279">This user right determines which users can specify object access auditing options for individual resources, such as files, Active Directory objects, and registry keys.</span></span> <span data-ttu-id="65bc6-280">仅支持 NotConfigured 和允许的状态。</span><span class="sxs-lookup"><span data-stu-id="65bc6-280">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="65bc6-281">userRightsManageVolumes</span><span class="sxs-lookup"><span data-stu-id="65bc6-281">userRightsManageVolumes</span></span>|[<span data-ttu-id="65bc6-282">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="65bc6-282">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="65bc6-283">此用户权限确定哪些用户和组可以在某个卷 (如远程碎片整理) 上运行维护任务。</span><span class="sxs-lookup"><span data-stu-id="65bc6-283">This user right determines which users and groups can run maintenance tasks on a volume, such as remote defragmentation.</span></span> <span data-ttu-id="65bc6-284">仅支持 NotConfigured 和允许的状态。</span><span class="sxs-lookup"><span data-stu-id="65bc6-284">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="65bc6-285">userRightsModifyFirmwareEnvironment</span><span class="sxs-lookup"><span data-stu-id="65bc6-285">userRightsModifyFirmwareEnvironment</span></span>|[<span data-ttu-id="65bc6-286">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="65bc6-286">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="65bc6-287">此用户权限决定了可以修改固件环境值的用户。</span><span class="sxs-lookup"><span data-stu-id="65bc6-287">This user right determines who can modify firmware environment values.</span></span> <span data-ttu-id="65bc6-288">仅支持 NotConfigured 和允许的状态。</span><span class="sxs-lookup"><span data-stu-id="65bc6-288">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="65bc6-289">userRightsModifyObjectLabels</span><span class="sxs-lookup"><span data-stu-id="65bc6-289">userRightsModifyObjectLabels</span></span>|[<span data-ttu-id="65bc6-290">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="65bc6-290">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="65bc6-291">此用户权限确定哪些用户帐户可以修改对象的完整性标签, 例如, 文件、注册表项或其他用户所拥有的进程。</span><span class="sxs-lookup"><span data-stu-id="65bc6-291">This user right determines which user accounts can modify the integrity label of objects, such as files, registry keys, or processes owned by other users.</span></span> <span data-ttu-id="65bc6-292">仅支持 NotConfigured 和允许的状态。</span><span class="sxs-lookup"><span data-stu-id="65bc6-292">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="65bc6-293">userRightsProfileSingleProcess</span><span class="sxs-lookup"><span data-stu-id="65bc6-293">userRightsProfileSingleProcess</span></span>|[<span data-ttu-id="65bc6-294">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="65bc6-294">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="65bc6-295">此用户权限确定哪些用户可以使用性能监视工具来监视系统进程的性能。</span><span class="sxs-lookup"><span data-stu-id="65bc6-295">This user right determines which users can use performance monitoring tools to monitor the performance of system processes.</span></span> <span data-ttu-id="65bc6-296">仅支持 NotConfigured 和允许的状态。</span><span class="sxs-lookup"><span data-stu-id="65bc6-296">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="65bc6-297">userRightsRemoteShutdown</span><span class="sxs-lookup"><span data-stu-id="65bc6-297">userRightsRemoteShutdown</span></span>|[<span data-ttu-id="65bc6-298">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="65bc6-298">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="65bc6-299">此用户权限确定允许哪些用户从网络上的远程位置关闭计算机。</span><span class="sxs-lookup"><span data-stu-id="65bc6-299">This user right determines which users are allowed to shut down a computer from a remote location on the network.</span></span> <span data-ttu-id="65bc6-300">误用此用户权限可能会导致拒绝服务。</span><span class="sxs-lookup"><span data-stu-id="65bc6-300">Misuse of this user right can result in a denial of service.</span></span> <span data-ttu-id="65bc6-301">仅支持 NotConfigured 和允许的状态。</span><span class="sxs-lookup"><span data-stu-id="65bc6-301">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="65bc6-302">userRightsRestoreData</span><span class="sxs-lookup"><span data-stu-id="65bc6-302">userRightsRestoreData</span></span>|[<span data-ttu-id="65bc6-303">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="65bc6-303">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="65bc6-304">此用户权限确定在还原备份的文件和目录时, 哪些用户可以绕过文件、目录、注册表和其他持久对象权限, 并确定哪些用户可以将任何有效的安全主体设置为对象的所有者。</span><span class="sxs-lookup"><span data-stu-id="65bc6-304">This user right determines which users can bypass file, directory, registry, and other persistent objects permissions when restoring backed up files and directories, and determines which users can set any valid security principal as the owner of an object.</span></span> <span data-ttu-id="65bc6-305">仅支持 NotConfigured 和允许的状态。</span><span class="sxs-lookup"><span data-stu-id="65bc6-305">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="65bc6-306">userRightsTakeOwnership</span><span class="sxs-lookup"><span data-stu-id="65bc6-306">userRightsTakeOwnership</span></span>|[<span data-ttu-id="65bc6-307">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="65bc6-307">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="65bc6-308">此用户权限确定哪些用户可以获得系统中任何安全对象的所有权, 包括 Active Directory 对象、文件和文件夹、打印机、注册表项、进程和线程。</span><span class="sxs-lookup"><span data-stu-id="65bc6-308">This user right determines which users can take ownership of any securable object in the system, including Active Directory objects, files and folders, printers, registry keys, processes, and threads.</span></span> <span data-ttu-id="65bc6-309">仅支持 NotConfigured 和允许的状态。</span><span class="sxs-lookup"><span data-stu-id="65bc6-309">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="65bc6-310">userRightsRegisterProcessAsService</span><span class="sxs-lookup"><span data-stu-id="65bc6-310">userRightsRegisterProcessAsService</span></span>|[<span data-ttu-id="65bc6-311">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="65bc6-311">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="65bc6-312">此安全设置确定阻止将进程注册为服务的服务帐户。</span><span class="sxs-lookup"><span data-stu-id="65bc6-312">This security setting determines which service accounts are prevented from registering a process as a service.</span></span> <span data-ttu-id="65bc6-313">注意: 此安全设置不适用于系统、本地服务或网络服务帐户。</span><span class="sxs-lookup"><span data-stu-id="65bc6-313">Note: This security setting does not apply to the System, Local Service, or Network Service accounts.</span></span> <span data-ttu-id="65bc6-314">仅支持阻止状态。</span><span class="sxs-lookup"><span data-stu-id="65bc6-314">Only state Blocked is supported.</span></span>|
|<span data-ttu-id="65bc6-315">xboxServicesEnableXboxGameSaveTask</span><span class="sxs-lookup"><span data-stu-id="65bc6-315">xboxServicesEnableXboxGameSaveTask</span></span>|<span data-ttu-id="65bc6-316">Boolean</span><span class="sxs-lookup"><span data-stu-id="65bc6-316">Boolean</span></span>|<span data-ttu-id="65bc6-317">此设置确定是否启用了 xbox 游戏保存 (1) 或禁用 (0)。</span><span class="sxs-lookup"><span data-stu-id="65bc6-317">This setting determines whether xbox game save is enabled (1) or disabled (0).</span></span>|
|<span data-ttu-id="65bc6-318">xboxServicesAccessoryManagementServiceStartupMode</span><span class="sxs-lookup"><span data-stu-id="65bc6-318">xboxServicesAccessoryManagementServiceStartupMode</span></span>|[<span data-ttu-id="65bc6-319">serviceStartType</span><span class="sxs-lookup"><span data-stu-id="65bc6-319">serviceStartType</span></span>](../resources/intune-deviceconfig-servicestarttype.md)|<span data-ttu-id="65bc6-320">此设置确定附件管理服务的启动类型是 "自动" (2)、"手动" (3)、"已禁用" (4)。</span><span class="sxs-lookup"><span data-stu-id="65bc6-320">This setting determines whether the Accessory management service's start type is Automatic(2), Manual(3), Disabled(4).</span></span> <span data-ttu-id="65bc6-321">默认: 手动。</span><span class="sxs-lookup"><span data-stu-id="65bc6-321">Default: Manual.</span></span> <span data-ttu-id="65bc6-322">可取值为：`manual`、`automatic`、`disabled`。</span><span class="sxs-lookup"><span data-stu-id="65bc6-322">Possible values are: `manual`, `automatic`, `disabled`.</span></span>|
|<span data-ttu-id="65bc6-323">xboxServicesLiveAuthManagerServiceStartupMode</span><span class="sxs-lookup"><span data-stu-id="65bc6-323">xboxServicesLiveAuthManagerServiceStartupMode</span></span>|[<span data-ttu-id="65bc6-324">serviceStartType</span><span class="sxs-lookup"><span data-stu-id="65bc6-324">serviceStartType</span></span>](../resources/intune-deviceconfig-servicestarttype.md)|<span data-ttu-id="65bc6-325">此设置确定 Live Auth Manager 服务的启动类型是否为自动 (2)、手动 (3)、已禁用 (4)。</span><span class="sxs-lookup"><span data-stu-id="65bc6-325">This setting determines whether Live Auth Manager service's start type is Automatic(2), Manual(3), Disabled(4).</span></span> <span data-ttu-id="65bc6-326">默认: 手动。</span><span class="sxs-lookup"><span data-stu-id="65bc6-326">Default: Manual.</span></span> <span data-ttu-id="65bc6-327">可取值为：`manual`、`automatic`、`disabled`。</span><span class="sxs-lookup"><span data-stu-id="65bc6-327">Possible values are: `manual`, `automatic`, `disabled`.</span></span>|
|<span data-ttu-id="65bc6-328">xboxServicesLiveGameSaveServiceStartupMode</span><span class="sxs-lookup"><span data-stu-id="65bc6-328">xboxServicesLiveGameSaveServiceStartupMode</span></span>|[<span data-ttu-id="65bc6-329">serviceStartType</span><span class="sxs-lookup"><span data-stu-id="65bc6-329">serviceStartType</span></span>](../resources/intune-deviceconfig-servicestarttype.md)|<span data-ttu-id="65bc6-330">此设置确定实时游戏是否保存服务的启动类型为自动 (2)、手动 (3)、已禁用 (4)。</span><span class="sxs-lookup"><span data-stu-id="65bc6-330">This setting determines whether Live Game save service's start type is Automatic(2), Manual(3), Disabled(4).</span></span> <span data-ttu-id="65bc6-331">默认: 手动。</span><span class="sxs-lookup"><span data-stu-id="65bc6-331">Default: Manual.</span></span> <span data-ttu-id="65bc6-332">可取值为：`manual`、`automatic`、`disabled`。</span><span class="sxs-lookup"><span data-stu-id="65bc6-332">Possible values are: `manual`, `automatic`, `disabled`.</span></span>|
|<span data-ttu-id="65bc6-333">xboxServicesLiveNetworkingServiceStartupMode</span><span class="sxs-lookup"><span data-stu-id="65bc6-333">xboxServicesLiveNetworkingServiceStartupMode</span></span>|[<span data-ttu-id="65bc6-334">serviceStartType</span><span class="sxs-lookup"><span data-stu-id="65bc6-334">serviceStartType</span></span>](../resources/intune-deviceconfig-servicestarttype.md)|<span data-ttu-id="65bc6-335">此设置确定网络服务的启动类型是否为自动 (2)、手动 (3)、已禁用 (4)。</span><span class="sxs-lookup"><span data-stu-id="65bc6-335">This setting determines whether Networking service's start type is Automatic(2), Manual(3), Disabled(4).</span></span> <span data-ttu-id="65bc6-336">默认: 手动。</span><span class="sxs-lookup"><span data-stu-id="65bc6-336">Default: Manual.</span></span> <span data-ttu-id="65bc6-337">可取值为：`manual`、`automatic`、`disabled`。</span><span class="sxs-lookup"><span data-stu-id="65bc6-337">Possible values are: `manual`, `automatic`, `disabled`.</span></span>|
|<span data-ttu-id="65bc6-338">localSecurityOptionsBlockMicrosoftAccounts</span><span class="sxs-lookup"><span data-stu-id="65bc6-338">localSecurityOptionsBlockMicrosoftAccounts</span></span>|<span data-ttu-id="65bc6-339">Boolean</span><span class="sxs-lookup"><span data-stu-id="65bc6-339">Boolean</span></span>|<span data-ttu-id="65bc6-340">阻止用户向此计算机添加新的 Microsoft 帐户。</span><span class="sxs-lookup"><span data-stu-id="65bc6-340">Prevent users from adding new Microsoft accounts to this computer.</span></span>|
|<span data-ttu-id="65bc6-341">localSecurityOptionsBlockRemoteLogonWithBlankPassword</span><span class="sxs-lookup"><span data-stu-id="65bc6-341">localSecurityOptionsBlockRemoteLogonWithBlankPassword</span></span>|<span data-ttu-id="65bc6-342">Boolean</span><span class="sxs-lookup"><span data-stu-id="65bc6-342">Boolean</span></span>|<span data-ttu-id="65bc6-343">启用不受密码保护的本地帐户从物理设备以外的位置进行登录。默认值为已启用</span><span class="sxs-lookup"><span data-stu-id="65bc6-343">Enable Local accounts that are not password protected to log on from locations other than the physical device.Default is enabled</span></span>|
|<span data-ttu-id="65bc6-344">localSecurityOptionsDisableAdministratorAccount</span><span class="sxs-lookup"><span data-stu-id="65bc6-344">localSecurityOptionsDisableAdministratorAccount</span></span>|<span data-ttu-id="65bc6-345">Boolean</span><span class="sxs-lookup"><span data-stu-id="65bc6-345">Boolean</span></span>|<span data-ttu-id="65bc6-346">确定是否启用或禁用本地管理员帐户。</span><span class="sxs-lookup"><span data-stu-id="65bc6-346">Determines whether the Local Administrator account is enabled or disabled.</span></span>|
|<span data-ttu-id="65bc6-347">localSecurityOptionsAdministratorAccountName</span><span class="sxs-lookup"><span data-stu-id="65bc6-347">localSecurityOptionsAdministratorAccountName</span></span>|<span data-ttu-id="65bc6-348">String</span><span class="sxs-lookup"><span data-stu-id="65bc6-348">String</span></span>|<span data-ttu-id="65bc6-349">定义要与帐户 "管理员" 的安全标识符 (SID) 相关联的不同帐户名称。</span><span class="sxs-lookup"><span data-stu-id="65bc6-349">Define a different account name to be associated with the security identifier (SID) for the account “Administrator”.</span></span>|
|<span data-ttu-id="65bc6-350">localSecurityOptionsDisableGuestAccount</span><span class="sxs-lookup"><span data-stu-id="65bc6-350">localSecurityOptionsDisableGuestAccount</span></span>|<span data-ttu-id="65bc6-351">Boolean</span><span class="sxs-lookup"><span data-stu-id="65bc6-351">Boolean</span></span>|<span data-ttu-id="65bc6-352">确定来宾帐户是否已启用或已禁用。</span><span class="sxs-lookup"><span data-stu-id="65bc6-352">Determines if the Guest account is enabled or disabled.</span></span>|
|<span data-ttu-id="65bc6-353">localSecurityOptionsGuestAccountName</span><span class="sxs-lookup"><span data-stu-id="65bc6-353">localSecurityOptionsGuestAccountName</span></span>|<span data-ttu-id="65bc6-354">String</span><span class="sxs-lookup"><span data-stu-id="65bc6-354">String</span></span>|<span data-ttu-id="65bc6-355">定义要与帐户 "来宾" 的安全标识符 (SID) 相关联的不同帐户名称。</span><span class="sxs-lookup"><span data-stu-id="65bc6-355">Define a different account name to be associated with the security identifier (SID) for the account “Guest”.</span></span>|
|<span data-ttu-id="65bc6-356">localSecurityOptionsAllowUndockWithoutHavingToLogon</span><span class="sxs-lookup"><span data-stu-id="65bc6-356">localSecurityOptionsAllowUndockWithoutHavingToLogon</span></span>|<span data-ttu-id="65bc6-357">Boolean</span><span class="sxs-lookup"><span data-stu-id="65bc6-357">Boolean</span></span>|<span data-ttu-id="65bc6-358">阻止便携式计算机在无需登录的情况下被移除。</span><span class="sxs-lookup"><span data-stu-id="65bc6-358">Prevent a portable computer from being undocked without having to log in.</span></span>|
|<span data-ttu-id="65bc6-359">localSecurityOptionsBlockUsersInstallingPrinterDrivers</span><span class="sxs-lookup"><span data-stu-id="65bc6-359">localSecurityOptionsBlockUsersInstallingPrinterDrivers</span></span>|<span data-ttu-id="65bc6-360">Boolean</span><span class="sxs-lookup"><span data-stu-id="65bc6-360">Boolean</span></span>|<span data-ttu-id="65bc6-361">仅在将打印机驱动程序连接到共享打印机时, 才将其限制为仅供管理员安装。</span><span class="sxs-lookup"><span data-stu-id="65bc6-361">Restrict installing printer drivers as part of connecting to a shared printer to admins only.</span></span>|
|<span data-ttu-id="65bc6-362">localSecurityOptionsBlockRemoteOpticalDriveAccess</span><span class="sxs-lookup"><span data-stu-id="65bc6-362">localSecurityOptionsBlockRemoteOpticalDriveAccess</span></span>|<span data-ttu-id="65bc6-363">Boolean</span><span class="sxs-lookup"><span data-stu-id="65bc6-363">Boolean</span></span>|<span data-ttu-id="65bc6-364">如果启用此设置, 则仅允许交互式登录用户访问 CD-ROM 媒体。</span><span class="sxs-lookup"><span data-stu-id="65bc6-364">Enabling this settings allows only interactively logged on user to access CD-ROM media.</span></span>|
|<span data-ttu-id="65bc6-365">localSecurityOptionsFormatAndEjectOfRemovableMediaAllowedUser</span><span class="sxs-lookup"><span data-stu-id="65bc6-365">localSecurityOptionsFormatAndEjectOfRemovableMediaAllowedUser</span></span>|[<span data-ttu-id="65bc6-366">localSecurityOptionsFormatAndEjectOfRemovableMediaAllowedUserType</span><span class="sxs-lookup"><span data-stu-id="65bc6-366">localSecurityOptionsFormatAndEjectOfRemovableMediaAllowedUserType</span></span>](../resources/intune-deviceconfig-localsecurityoptionsformatandejectofremovablemediaallowedusertype.md)|<span data-ttu-id="65bc6-367">定义允许格式化和弹出可移动 NTFS 媒体的权限。</span><span class="sxs-lookup"><span data-stu-id="65bc6-367">Define who is allowed to format and eject removable NTFS media.</span></span> <span data-ttu-id="65bc6-368">可取值为：`notConfigured`、`administrators`、`administratorsAndPowerUsers`、`administratorsAndInteractiveUsers`。</span><span class="sxs-lookup"><span data-stu-id="65bc6-368">Possible values are: `notConfigured`, `administrators`, `administratorsAndPowerUsers`, `administratorsAndInteractiveUsers`.</span></span>|
|<span data-ttu-id="65bc6-369">localSecurityOptionsMachineInactivityLimit</span><span class="sxs-lookup"><span data-stu-id="65bc6-369">localSecurityOptionsMachineInactivityLimit</span></span>|<span data-ttu-id="65bc6-370">Int32</span><span class="sxs-lookup"><span data-stu-id="65bc6-370">Int32</span></span>|<span data-ttu-id="65bc6-371">在屏幕保护程序运行之前, 定义交互式桌面登录屏幕上不活动的最长分钟数。</span><span class="sxs-lookup"><span data-stu-id="65bc6-371">Define maximum minutes of inactivity on the interactive desktop’s login screen until the screen saver runs.</span></span> <span data-ttu-id="65bc6-372">有效值为0至9999</span><span class="sxs-lookup"><span data-stu-id="65bc6-372">Valid values 0 to 9999</span></span>|
|<span data-ttu-id="65bc6-373">localSecurityOptionsMachineInactivityLimitInMinutes</span><span class="sxs-lookup"><span data-stu-id="65bc6-373">localSecurityOptionsMachineInactivityLimitInMinutes</span></span>|<span data-ttu-id="65bc6-374">Int32</span><span class="sxs-lookup"><span data-stu-id="65bc6-374">Int32</span></span>|<span data-ttu-id="65bc6-375">在屏幕保护程序运行之前, 定义交互式桌面登录屏幕上不活动的最长分钟数。</span><span class="sxs-lookup"><span data-stu-id="65bc6-375">Define maximum minutes of inactivity on the interactive desktop’s login screen until the screen saver runs.</span></span> <span data-ttu-id="65bc6-376">有效值为0至9999</span><span class="sxs-lookup"><span data-stu-id="65bc6-376">Valid values 0 to 9999</span></span>|
|<span data-ttu-id="65bc6-377">localSecurityOptionsDoNotRequireCtrlAltDel</span><span class="sxs-lookup"><span data-stu-id="65bc6-377">localSecurityOptionsDoNotRequireCtrlAltDel</span></span>|<span data-ttu-id="65bc6-378">Boolean</span><span class="sxs-lookup"><span data-stu-id="65bc6-378">Boolean</span></span>|<span data-ttu-id="65bc6-379">要求用户在登录前按 CTRL + ALT + DEL。</span><span class="sxs-lookup"><span data-stu-id="65bc6-379">Require CTRL+ALT+DEL to be pressed before a user can log on.</span></span>|
|<span data-ttu-id="65bc6-380">localSecurityOptionsHideLastSignedInUser</span><span class="sxs-lookup"><span data-stu-id="65bc6-380">localSecurityOptionsHideLastSignedInUser</span></span>|<span data-ttu-id="65bc6-381">Boolean</span><span class="sxs-lookup"><span data-stu-id="65bc6-381">Boolean</span></span>|<span data-ttu-id="65bc6-382">不显示上次在此设备上登录的用户的用户名。</span><span class="sxs-lookup"><span data-stu-id="65bc6-382">Do not display the username of the last person who signed in on this device.</span></span>|
|<span data-ttu-id="65bc6-383">localSecurityOptionsHideUsernameAtSignIn</span><span class="sxs-lookup"><span data-stu-id="65bc6-383">localSecurityOptionsHideUsernameAtSignIn</span></span>|<span data-ttu-id="65bc6-384">Boolean</span><span class="sxs-lookup"><span data-stu-id="65bc6-384">Boolean</span></span>|<span data-ttu-id="65bc6-385">在输入凭据后以及显示设备桌面之前, 请勿显示登录此设备的人员的用户名。</span><span class="sxs-lookup"><span data-stu-id="65bc6-385">Do not display the username of the person signing in to this device after credentials are entered and before the device’s desktop is shown.</span></span>|
|<span data-ttu-id="65bc6-386">localSecurityOptionsLogOnMessageTitle</span><span class="sxs-lookup"><span data-stu-id="65bc6-386">localSecurityOptionsLogOnMessageTitle</span></span>|<span data-ttu-id="65bc6-387">String</span><span class="sxs-lookup"><span data-stu-id="65bc6-387">String</span></span>|<span data-ttu-id="65bc6-388">为尝试登录的用户设置消息标题。</span><span class="sxs-lookup"><span data-stu-id="65bc6-388">Set message title for users attempting to log in.</span></span>|
|<span data-ttu-id="65bc6-389">localSecurityOptionsLogOnMessageText</span><span class="sxs-lookup"><span data-stu-id="65bc6-389">localSecurityOptionsLogOnMessageText</span></span>|<span data-ttu-id="65bc6-390">String</span><span class="sxs-lookup"><span data-stu-id="65bc6-390">String</span></span>|<span data-ttu-id="65bc6-391">为尝试登录的用户设置消息文本。</span><span class="sxs-lookup"><span data-stu-id="65bc6-391">Set message text for users attempting to log in.</span></span>|
|<span data-ttu-id="65bc6-392">localSecurityOptionsAllowPKU2UAuthenticationRequests</span><span class="sxs-lookup"><span data-stu-id="65bc6-392">localSecurityOptionsAllowPKU2UAuthenticationRequests</span></span>|<span data-ttu-id="65bc6-393">Boolean</span><span class="sxs-lookup"><span data-stu-id="65bc6-393">Boolean</span></span>|<span data-ttu-id="65bc6-394">阻止 PKU2U 对此设备的身份验证请求, 以使用联机标识。</span><span class="sxs-lookup"><span data-stu-id="65bc6-394">Block PKU2U authentication requests to this device to use online identities.</span></span>|
|<span data-ttu-id="65bc6-395">localSecurityOptionsAllowRemoteCallsToSecurityAccountsManagerHelperBool</span><span class="sxs-lookup"><span data-stu-id="65bc6-395">localSecurityOptionsAllowRemoteCallsToSecurityAccountsManagerHelperBool</span></span>|<span data-ttu-id="65bc6-396">Boolean</span><span class="sxs-lookup"><span data-stu-id="65bc6-396">Boolean</span></span>|<span data-ttu-id="65bc6-397">LocalSecurityOptionsAllowRemoteCallsToSecurityAccountsManager 实体的 UI 帮助程序布尔值</span><span class="sxs-lookup"><span data-stu-id="65bc6-397">UI helper boolean for LocalSecurityOptionsAllowRemoteCallsToSecurityAccountsManager entity</span></span>|
|<span data-ttu-id="65bc6-398">localSecurityOptionsAllowRemoteCallsToSecurityAccountsManager</span><span class="sxs-lookup"><span data-stu-id="65bc6-398">localSecurityOptionsAllowRemoteCallsToSecurityAccountsManager</span></span>|<span data-ttu-id="65bc6-399">String</span><span class="sxs-lookup"><span data-stu-id="65bc6-399">String</span></span>|<span data-ttu-id="65bc6-400">编辑默认的安全描述符定义语言字符串, 以允许或拒绝用户和组对 SAM 进行远程调用。</span><span class="sxs-lookup"><span data-stu-id="65bc6-400">Edit the default Security Descriptor Definition Language string to allow or deny users and groups to make remote calls to the SAM.</span></span>|
|<span data-ttu-id="65bc6-401">localSecurityOptionsMinimumSessionSecurityForNtlmSspBasedClients</span><span class="sxs-lookup"><span data-stu-id="65bc6-401">localSecurityOptionsMinimumSessionSecurityForNtlmSspBasedClients</span></span>|[<span data-ttu-id="65bc6-402">localSecurityOptionsMinimumSessionSecurity</span><span class="sxs-lookup"><span data-stu-id="65bc6-402">localSecurityOptionsMinimumSessionSecurity</span></span>](../resources/intune-deviceconfig-localsecurityoptionsminimumsessionsecurity.md)|<span data-ttu-id="65bc6-403">此安全设置允许客户端要求协商128位加密和/或 NTLMv2 会话安全性。</span><span class="sxs-lookup"><span data-stu-id="65bc6-403">This security setting allows a client to require the negotiation of 128-bit encryption and/or NTLMv2 session security.</span></span> <span data-ttu-id="65bc6-404">可取值为：`none`、`requireNtmlV2SessionSecurity`、`require128BitEncryption`、`ntlmV2And128BitEncryption`。</span><span class="sxs-lookup"><span data-stu-id="65bc6-404">Possible values are: `none`, `requireNtmlV2SessionSecurity`, `require128BitEncryption`, `ntlmV2And128BitEncryption`.</span></span>|
|<span data-ttu-id="65bc6-405">localSecurityOptionsMinimumSessionSecurityForNtlmSspBasedServers</span><span class="sxs-lookup"><span data-stu-id="65bc6-405">localSecurityOptionsMinimumSessionSecurityForNtlmSspBasedServers</span></span>|[<span data-ttu-id="65bc6-406">localSecurityOptionsMinimumSessionSecurity</span><span class="sxs-lookup"><span data-stu-id="65bc6-406">localSecurityOptionsMinimumSessionSecurity</span></span>](../resources/intune-deviceconfig-localsecurityoptionsminimumsessionsecurity.md)|<span data-ttu-id="65bc6-407">此安全设置允许服务器要求协商128位加密和/或 NTLMv2 会话安全性。</span><span class="sxs-lookup"><span data-stu-id="65bc6-407">This security setting allows a server to require the negotiation of 128-bit encryption and/or NTLMv2 session security.</span></span> <span data-ttu-id="65bc6-408">可取值为：`none`、`requireNtmlV2SessionSecurity`、`require128BitEncryption`、`ntlmV2And128BitEncryption`。</span><span class="sxs-lookup"><span data-stu-id="65bc6-408">Possible values are: `none`, `requireNtmlV2SessionSecurity`, `require128BitEncryption`, `ntlmV2And128BitEncryption`.</span></span>|
|<span data-ttu-id="65bc6-409">lanManagerAuthenticationLevel</span><span class="sxs-lookup"><span data-stu-id="65bc6-409">lanManagerAuthenticationLevel</span></span>|[<span data-ttu-id="65bc6-410">lanManagerAuthenticationLevel</span><span class="sxs-lookup"><span data-stu-id="65bc6-410">lanManagerAuthenticationLevel</span></span>](../resources/intune-deviceconfig-lanmanagerauthenticationlevel.md)|<span data-ttu-id="65bc6-411">此安全设置确定用于网络登录的质询/响应身份验证协议。</span><span class="sxs-lookup"><span data-stu-id="65bc6-411">This security setting determines which challenge/response authentication protocol is used for network logons.</span></span> <span data-ttu-id="65bc6-412">可取值为：`lmAndNltm`、`lmNtlmAndNtlmV2`、`lmAndNtlmOnly`、`lmAndNtlmV2`、`lmNtlmV2AndNotLm`、`lmNtlmV2AndNotLmOrNtm`。</span><span class="sxs-lookup"><span data-stu-id="65bc6-412">Possible values are: `lmAndNltm`, `lmNtlmAndNtlmV2`, `lmAndNtlmOnly`, `lmAndNtlmV2`, `lmNtlmV2AndNotLm`, `lmNtlmV2AndNotLmOrNtm`.</span></span>|
|<span data-ttu-id="65bc6-413">lanManagerWorkstationDisableInsecureGuestLogons</span><span class="sxs-lookup"><span data-stu-id="65bc6-413">lanManagerWorkstationDisableInsecureGuestLogons</span></span>|<span data-ttu-id="65bc6-414">Boolean</span><span class="sxs-lookup"><span data-stu-id="65bc6-414">Boolean</span></span>|<span data-ttu-id="65bc6-415">如果启用, SMB 客户端将允许不安全的来宾登录。</span><span class="sxs-lookup"><span data-stu-id="65bc6-415">If enabled,the SMB client will allow insecure guest logons.</span></span> <span data-ttu-id="65bc6-416">如果未配置, SMB 客户端将拒绝不安全的来宾登录。</span><span class="sxs-lookup"><span data-stu-id="65bc6-416">If not configured, the SMB client will reject insecure guest logons.</span></span>|
|<span data-ttu-id="65bc6-417">localSecurityOptionsClearVirtualMemoryPageFile</span><span class="sxs-lookup"><span data-stu-id="65bc6-417">localSecurityOptionsClearVirtualMemoryPageFile</span></span>|<span data-ttu-id="65bc6-418">Boolean</span><span class="sxs-lookup"><span data-stu-id="65bc6-418">Boolean</span></span>|<span data-ttu-id="65bc6-419">此安全设置确定在关闭系统时是否清除虚拟内存页面文件。</span><span class="sxs-lookup"><span data-stu-id="65bc6-419">This security setting determines whether the virtual memory pagefile is cleared when the system is shut down.</span></span>|
|<span data-ttu-id="65bc6-420">localSecurityOptionsAllowSystemToBeShutDownWithoutHavingToLogOn</span><span class="sxs-lookup"><span data-stu-id="65bc6-420">localSecurityOptionsAllowSystemToBeShutDownWithoutHavingToLogOn</span></span>|<span data-ttu-id="65bc6-421">Boolean</span><span class="sxs-lookup"><span data-stu-id="65bc6-421">Boolean</span></span>|<span data-ttu-id="65bc6-422">此安全设置确定是否可以在不登录 Windows 的情况下关闭计算机。</span><span class="sxs-lookup"><span data-stu-id="65bc6-422">This security setting determines whether a computer can be shut down without having to log on to Windows.</span></span>|
|<span data-ttu-id="65bc6-423">localSecurityOptionsAllowUIAccessApplicationElevation</span><span class="sxs-lookup"><span data-stu-id="65bc6-423">localSecurityOptionsAllowUIAccessApplicationElevation</span></span>|<span data-ttu-id="65bc6-424">Boolean</span><span class="sxs-lookup"><span data-stu-id="65bc6-424">Boolean</span></span>|<span data-ttu-id="65bc6-425">允许 UIAccess 应用在不使用安全桌面的情况下提示提升。</span><span class="sxs-lookup"><span data-stu-id="65bc6-425">Allow UIAccess apps to prompt for elevation without using the secure desktop.</span></span>|
|<span data-ttu-id="65bc6-426">localSecurityOptionsVirtualizeFileAndRegistryWriteFailuresToPerUserLocations</span><span class="sxs-lookup"><span data-stu-id="65bc6-426">localSecurityOptionsVirtualizeFileAndRegistryWriteFailuresToPerUserLocations</span></span>|<span data-ttu-id="65bc6-427">Boolean</span><span class="sxs-lookup"><span data-stu-id="65bc6-427">Boolean</span></span>|<span data-ttu-id="65bc6-428">将文件和注册表写入失败虚拟化到每个用户位置</span><span class="sxs-lookup"><span data-stu-id="65bc6-428">Virtualize file and registry write failures to per user locations</span></span>|
|<span data-ttu-id="65bc6-429">localSecurityOptionsOnlyElevateSignedExecutables</span><span class="sxs-lookup"><span data-stu-id="65bc6-429">localSecurityOptionsOnlyElevateSignedExecutables</span></span>|<span data-ttu-id="65bc6-430">Boolean</span><span class="sxs-lookup"><span data-stu-id="65bc6-430">Boolean</span></span>|<span data-ttu-id="65bc6-431">对给定的可执行文件强制执行 PKI 证书路径验证, 然后再允许运行该文件。</span><span class="sxs-lookup"><span data-stu-id="65bc6-431">Enforce PKI certification path validation for a given executable file before it is permitted to run.</span></span>|
|<span data-ttu-id="65bc6-432">localSecurityOptionsAdministratorElevationPromptBehavior</span><span class="sxs-lookup"><span data-stu-id="65bc6-432">localSecurityOptionsAdministratorElevationPromptBehavior</span></span>|[<span data-ttu-id="65bc6-433">localSecurityOptionsAdministratorElevationPromptBehaviorType</span><span class="sxs-lookup"><span data-stu-id="65bc6-433">localSecurityOptionsAdministratorElevationPromptBehaviorType</span></span>](../resources/intune-deviceconfig-localsecurityoptionsadministratorelevationpromptbehaviortype.md)|<span data-ttu-id="65bc6-434">在管理员审批模式中定义管理员的提升提示行为。</span><span class="sxs-lookup"><span data-stu-id="65bc6-434">Define the behavior of the elevation prompt for admins in Admin Approval Mode.</span></span> <span data-ttu-id="65bc6-435">可取值为：`notConfigured`、`elevateWithoutPrompting`、`promptForCredentialsOnTheSecureDesktop`、`promptForConsentOnTheSecureDesktop`、`promptForCredentials`、`promptForConsent` 或 `promptForConsentForNonWindowsBinaries`。</span><span class="sxs-lookup"><span data-stu-id="65bc6-435">Possible values are: `notConfigured`, `elevateWithoutPrompting`, `promptForCredentialsOnTheSecureDesktop`, `promptForConsentOnTheSecureDesktop`, `promptForCredentials`, `promptForConsent`, `promptForConsentForNonWindowsBinaries`.</span></span>|
|<span data-ttu-id="65bc6-436">localSecurityOptionsStandardUserElevationPromptBehavior</span><span class="sxs-lookup"><span data-stu-id="65bc6-436">localSecurityOptionsStandardUserElevationPromptBehavior</span></span>|[<span data-ttu-id="65bc6-437">localSecurityOptionsStandardUserElevationPromptBehaviorType</span><span class="sxs-lookup"><span data-stu-id="65bc6-437">localSecurityOptionsStandardUserElevationPromptBehaviorType</span></span>](../resources/intune-deviceconfig-localsecurityoptionsstandarduserelevationpromptbehaviortype.md)|<span data-ttu-id="65bc6-438">定义标准用户的提升提示行为。</span><span class="sxs-lookup"><span data-stu-id="65bc6-438">Define the behavior of the elevation prompt for standard users.</span></span> <span data-ttu-id="65bc6-439">可取值为：`notConfigured`、`automaticallyDenyElevationRequests`、`promptForCredentialsOnTheSecureDesktop`、`promptForCredentials`。</span><span class="sxs-lookup"><span data-stu-id="65bc6-439">Possible values are: `notConfigured`, `automaticallyDenyElevationRequests`, `promptForCredentialsOnTheSecureDesktop`, `promptForCredentials`.</span></span>|
|<span data-ttu-id="65bc6-440">localSecurityOptionsSwitchToSecureDesktopWhenPromptingForElevation</span><span class="sxs-lookup"><span data-stu-id="65bc6-440">localSecurityOptionsSwitchToSecureDesktopWhenPromptingForElevation</span></span>|<span data-ttu-id="65bc6-441">Boolean</span><span class="sxs-lookup"><span data-stu-id="65bc6-441">Boolean</span></span>|<span data-ttu-id="65bc6-442">启用所有提升请求以转到交互式用户的桌面, 而不是安全桌面。</span><span class="sxs-lookup"><span data-stu-id="65bc6-442">Enable all elevation requests to go to the interactive user's desktop rather than the secure desktop.</span></span> <span data-ttu-id="65bc6-443">使用管理员和标准用户的提示行为策略设置。</span><span class="sxs-lookup"><span data-stu-id="65bc6-443">Prompt behavior policy settings for admins and standard users are used.</span></span>|
|<span data-ttu-id="65bc6-444">localSecurityOptionsDetectApplicationInstallationsAndPromptForElevation</span><span class="sxs-lookup"><span data-stu-id="65bc6-444">localSecurityOptionsDetectApplicationInstallationsAndPromptForElevation</span></span>|<span data-ttu-id="65bc6-445">Boolean</span><span class="sxs-lookup"><span data-stu-id="65bc6-445">Boolean</span></span>|<span data-ttu-id="65bc6-446">需要提升权限的应用程序安装将提示管理凭据。默认值为已启用</span><span class="sxs-lookup"><span data-stu-id="65bc6-446">App installations requiring elevated privileges will prompt for admin credentials.Default is enabled</span></span>|
|<span data-ttu-id="65bc6-447">localSecurityOptionsAllowUIAccessApplicationsForSecureLocations</span><span class="sxs-lookup"><span data-stu-id="65bc6-447">localSecurityOptionsAllowUIAccessApplicationsForSecureLocations</span></span>|<span data-ttu-id="65bc6-448">Boolean</span><span class="sxs-lookup"><span data-stu-id="65bc6-448">Boolean</span></span>|<span data-ttu-id="65bc6-449">允许 UIAccess 应用在不使用安全桌面的情况下提示提升。默认值为已启用</span><span class="sxs-lookup"><span data-stu-id="65bc6-449">Allow UIAccess apps to prompt for elevation without using the secure desktop.Default is enabled</span></span>|
|<span data-ttu-id="65bc6-450">localSecurityOptionsUseAdminApprovalMode</span><span class="sxs-lookup"><span data-stu-id="65bc6-450">localSecurityOptionsUseAdminApprovalMode</span></span>|<span data-ttu-id="65bc6-451">Boolean</span><span class="sxs-lookup"><span data-stu-id="65bc6-451">Boolean</span></span>|<span data-ttu-id="65bc6-452">定义内置管理员帐户是使用管理员审批模式, 还是运行所有具有完全管理员权限的应用程序。默认值为已启用</span><span class="sxs-lookup"><span data-stu-id="65bc6-452">Defines whether the built-in admin account uses Admin Approval Mode or runs all apps with full admin privileges.Default is enabled</span></span>|
|<span data-ttu-id="65bc6-453">localSecurityOptionsUseAdminApprovalModeForAdministrators</span><span class="sxs-lookup"><span data-stu-id="65bc6-453">localSecurityOptionsUseAdminApprovalModeForAdministrators</span></span>|<span data-ttu-id="65bc6-454">Boolean</span><span class="sxs-lookup"><span data-stu-id="65bc6-454">Boolean</span></span>|<span data-ttu-id="65bc6-455">定义是否启用管理员批准模式和所有 UAC 策略设置, 默认为启用</span><span class="sxs-lookup"><span data-stu-id="65bc6-455">Define whether Admin Approval Mode and all UAC policy settings are enabled, default is enabled</span></span>|
|<span data-ttu-id="65bc6-456">localSecurityOptionsInformationShownOnLockScreen</span><span class="sxs-lookup"><span data-stu-id="65bc6-456">localSecurityOptionsInformationShownOnLockScreen</span></span>|[<span data-ttu-id="65bc6-457">localSecurityOptionsInformationShownOnLockScreenType</span><span class="sxs-lookup"><span data-stu-id="65bc6-457">localSecurityOptionsInformationShownOnLockScreenType</span></span>](../resources/intune-deviceconfig-localsecurityoptionsinformationshownonlockscreentype.md)|<span data-ttu-id="65bc6-458">配置在会话锁定时显示的用户信息。</span><span class="sxs-lookup"><span data-stu-id="65bc6-458">Configure the user information that is displayed when the session is locked.</span></span> <span data-ttu-id="65bc6-459">如果未配置, 则显示用户显示名称、域和用户名。</span><span class="sxs-lookup"><span data-stu-id="65bc6-459">If not configured, user display name, domain and username are shown.</span></span> <span data-ttu-id="65bc6-460">可取值为：`notConfigured`、`userDisplayNameDomainUser`、`userDisplayNameOnly`、`doNotDisplayUser`。</span><span class="sxs-lookup"><span data-stu-id="65bc6-460">Possible values are: `notConfigured`, `userDisplayNameDomainUser`, `userDisplayNameOnly`, `doNotDisplayUser`.</span></span>|
|<span data-ttu-id="65bc6-461">localSecurityOptionsInformationDisplayedOnLockScreen</span><span class="sxs-lookup"><span data-stu-id="65bc6-461">localSecurityOptionsInformationDisplayedOnLockScreen</span></span>|[<span data-ttu-id="65bc6-462">localSecurityOptionsInformationDisplayedOnLockScreenType</span><span class="sxs-lookup"><span data-stu-id="65bc6-462">localSecurityOptionsInformationDisplayedOnLockScreenType</span></span>](../resources/intune-deviceconfig-localsecurityoptionsinformationdisplayedonlockscreentype.md)|<span data-ttu-id="65bc6-463">配置在会话锁定时显示的用户信息。</span><span class="sxs-lookup"><span data-stu-id="65bc6-463">Configure the user information that is displayed when the session is locked.</span></span> <span data-ttu-id="65bc6-464">如果未配置, 则显示用户显示名称、域和用户名。</span><span class="sxs-lookup"><span data-stu-id="65bc6-464">If not configured, user display name, domain and username are shown.</span></span> <span data-ttu-id="65bc6-465">可取值为：`notConfigured`、`administrators`、`administratorsAndPowerUsers`、`administratorsAndInteractiveUsers`。</span><span class="sxs-lookup"><span data-stu-id="65bc6-465">Possible values are: `notConfigured`, `administrators`, `administratorsAndPowerUsers`, `administratorsAndInteractiveUsers`.</span></span>|
|<span data-ttu-id="65bc6-466">localSecurityOptionsDisableClientDigitallySignCommunicationsIfServerAgrees</span><span class="sxs-lookup"><span data-stu-id="65bc6-466">localSecurityOptionsDisableClientDigitallySignCommunicationsIfServerAgrees</span></span>|<span data-ttu-id="65bc6-467">Boolean</span><span class="sxs-lookup"><span data-stu-id="65bc6-467">Boolean</span></span>|<span data-ttu-id="65bc6-468">此安全设置确定 SMB 客户端是否尝试协商 SMB 数据包签名。</span><span class="sxs-lookup"><span data-stu-id="65bc6-468">This security setting determines whether the SMB client attempts to negotiate SMB packet signing.</span></span>|
|<span data-ttu-id="65bc6-469">localSecurityOptionsClientDigitallySignCommunicationsAlways</span><span class="sxs-lookup"><span data-stu-id="65bc6-469">localSecurityOptionsClientDigitallySignCommunicationsAlways</span></span>|<span data-ttu-id="65bc6-470">Boolean</span><span class="sxs-lookup"><span data-stu-id="65bc6-470">Boolean</span></span>|<span data-ttu-id="65bc6-471">此安全设置确定 SMB 客户端组件是否需要数据包签名。</span><span class="sxs-lookup"><span data-stu-id="65bc6-471">This security setting determines whether packet signing is required by the SMB client component.</span></span>|
|<span data-ttu-id="65bc6-472">localSecurityOptionsClientSendUnencryptedPasswordToThirdPartySMBServers</span><span class="sxs-lookup"><span data-stu-id="65bc6-472">localSecurityOptionsClientSendUnencryptedPasswordToThirdPartySMBServers</span></span>|<span data-ttu-id="65bc6-473">Boolean</span><span class="sxs-lookup"><span data-stu-id="65bc6-473">Boolean</span></span>|<span data-ttu-id="65bc6-474">如果启用此安全设置, 则允许服务器消息块 (SMB) 重定向程序将纯文本密码发送到在身份验证过程中不支持密码加密的非 Microsoft SMB 服务器。</span><span class="sxs-lookup"><span data-stu-id="65bc6-474">If this security setting is enabled, the Server Message Block (SMB) redirector is allowed to send plaintext passwords to non-Microsoft SMB servers that do not support password encryption during authentication.</span></span>|
|<span data-ttu-id="65bc6-475">localSecurityOptionsDisableServerDigitallySignCommunicationsAlways</span><span class="sxs-lookup"><span data-stu-id="65bc6-475">localSecurityOptionsDisableServerDigitallySignCommunicationsAlways</span></span>|<span data-ttu-id="65bc6-476">Boolean</span><span class="sxs-lookup"><span data-stu-id="65bc6-476">Boolean</span></span>|<span data-ttu-id="65bc6-477">此安全设置确定 SMB 服务器组件是否需要数据包签名。</span><span class="sxs-lookup"><span data-stu-id="65bc6-477">This security setting determines whether packet signing is required by the SMB server component.</span></span>|
|<span data-ttu-id="65bc6-478">localSecurityOptionsDisableServerDigitallySignCommunicationsIfClientAgrees</span><span class="sxs-lookup"><span data-stu-id="65bc6-478">localSecurityOptionsDisableServerDigitallySignCommunicationsIfClientAgrees</span></span>|<span data-ttu-id="65bc6-479">Boolean</span><span class="sxs-lookup"><span data-stu-id="65bc6-479">Boolean</span></span>|<span data-ttu-id="65bc6-480">此安全设置确定 SMB 服务器是否将 SMB 数据包签名与请求的客户端协商。</span><span class="sxs-lookup"><span data-stu-id="65bc6-480">This security setting determines whether the SMB server will negotiate SMB packet signing with clients that request it.</span></span>|
|<span data-ttu-id="65bc6-481">localSecurityOptionsRestrictAnonymousAccessToNamedPipesAndShares</span><span class="sxs-lookup"><span data-stu-id="65bc6-481">localSecurityOptionsRestrictAnonymousAccessToNamedPipesAndShares</span></span>|<span data-ttu-id="65bc6-482">Boolean</span><span class="sxs-lookup"><span data-stu-id="65bc6-482">Boolean</span></span>|<span data-ttu-id="65bc6-483">默认情况下, 此安全设置限制可匿名访问且可匿名访问的共享的命名管道设置对共享和管道的匿名访问权限</span><span class="sxs-lookup"><span data-stu-id="65bc6-483">By default, this security setting restricts anonymous access to shares and pipes to the settings for named pipes that can be accessed anonymously and Shares that can be accessed anonymously</span></span>|
|<span data-ttu-id="65bc6-484">localSecurityOptionsDoNotAllowAnonymousEnumerationOfSAMAccounts</span><span class="sxs-lookup"><span data-stu-id="65bc6-484">localSecurityOptionsDoNotAllowAnonymousEnumerationOfSAMAccounts</span></span>|<span data-ttu-id="65bc6-485">Boolean</span><span class="sxs-lookup"><span data-stu-id="65bc6-485">Boolean</span></span>|<span data-ttu-id="65bc6-486">此安全设置确定将向计算机的匿名连接授予的其他权限。</span><span class="sxs-lookup"><span data-stu-id="65bc6-486">This security setting determines what additional permissions will be granted for anonymous connections to the computer.</span></span>|
|<span data-ttu-id="65bc6-487">localSecurityOptionsAllowAnonymousEnumerationOfSAMAccountsAndShares</span><span class="sxs-lookup"><span data-stu-id="65bc6-487">localSecurityOptionsAllowAnonymousEnumerationOfSAMAccountsAndShares</span></span>|<span data-ttu-id="65bc6-488">Boolean</span><span class="sxs-lookup"><span data-stu-id="65bc6-488">Boolean</span></span>|<span data-ttu-id="65bc6-489">此安全设置确定是否允许匿名用户执行某些活动, 如枚举域帐户和网络共享的名称。</span><span class="sxs-lookup"><span data-stu-id="65bc6-489">This security setting determines whether to allows anonymous users to perform certain activities, such as enumerating the names of domain accounts and network shares.</span></span>|
|<span data-ttu-id="65bc6-490">localSecurityOptionsDoNotStoreLANManagerHashValueOnNextPasswordChange</span><span class="sxs-lookup"><span data-stu-id="65bc6-490">localSecurityOptionsDoNotStoreLANManagerHashValueOnNextPasswordChange</span></span>|<span data-ttu-id="65bc6-491">Boolean</span><span class="sxs-lookup"><span data-stu-id="65bc6-491">Boolean</span></span>|<span data-ttu-id="65bc6-492">此安全设置确定在下一次更改密码时, 是否存储新密码的 LAN Manager (LM) 哈希值。</span><span class="sxs-lookup"><span data-stu-id="65bc6-492">This security setting determines if, at the next password change, the LAN Manager (LM) hash value for the new password is stored.</span></span> <span data-ttu-id="65bc6-493">默认情况下不存储它。</span><span class="sxs-lookup"><span data-stu-id="65bc6-493">It’s not stored by default.</span></span>|
|<span data-ttu-id="65bc6-494">localSecurityOptionsSmartCardRemovalBehavior</span><span class="sxs-lookup"><span data-stu-id="65bc6-494">localSecurityOptionsSmartCardRemovalBehavior</span></span>|[<span data-ttu-id="65bc6-495">localSecurityOptionsSmartCardRemovalBehaviorType</span><span class="sxs-lookup"><span data-stu-id="65bc6-495">localSecurityOptionsSmartCardRemovalBehaviorType</span></span>](../resources/intune-deviceconfig-localsecurityoptionssmartcardremovalbehaviortype.md)|<span data-ttu-id="65bc6-496">此安全设置确定将已登录用户的智能卡从智能卡读卡器中删除时发生的情况。</span><span class="sxs-lookup"><span data-stu-id="65bc6-496">This security setting determines what happens when the smart card for a logged-on user is removed from the smart card reader.</span></span> <span data-ttu-id="65bc6-497">可取值为：`lockWorkstation`、`noAction`、`forceLogoff`、`disconnectRemoteDesktopSession`。</span><span class="sxs-lookup"><span data-stu-id="65bc6-497">Possible values are: `lockWorkstation`, `noAction`, `forceLogoff`, `disconnectRemoteDesktopSession`.</span></span>|
|<span data-ttu-id="65bc6-498">defenderSecurityCenterDisableAppBrowserUI</span><span class="sxs-lookup"><span data-stu-id="65bc6-498">defenderSecurityCenterDisableAppBrowserUI</span></span>|<span data-ttu-id="65bc6-499">Boolean</span><span class="sxs-lookup"><span data-stu-id="65bc6-499">Boolean</span></span>|<span data-ttu-id="65bc6-500">用于禁用应用程序和浏览器保护区域的显示。</span><span class="sxs-lookup"><span data-stu-id="65bc6-500">Used to disable the display of the app and browser protection area.</span></span>|
|<span data-ttu-id="65bc6-501">defenderSecurityCenterDisableFamilyUI</span><span class="sxs-lookup"><span data-stu-id="65bc6-501">defenderSecurityCenterDisableFamilyUI</span></span>|<span data-ttu-id="65bc6-502">Boolean</span><span class="sxs-lookup"><span data-stu-id="65bc6-502">Boolean</span></span>|<span data-ttu-id="65bc6-503">用于禁用 "家庭选项" 区域的显示。</span><span class="sxs-lookup"><span data-stu-id="65bc6-503">Used to disable the display of the family options area.</span></span>|
|<span data-ttu-id="65bc6-504">defenderSecurityCenterDisableHealthUI</span><span class="sxs-lookup"><span data-stu-id="65bc6-504">defenderSecurityCenterDisableHealthUI</span></span>|<span data-ttu-id="65bc6-505">Boolean</span><span class="sxs-lookup"><span data-stu-id="65bc6-505">Boolean</span></span>|<span data-ttu-id="65bc6-506">用于禁用设备性能和运行状况区域的显示。</span><span class="sxs-lookup"><span data-stu-id="65bc6-506">Used to disable the display of the device performance and health area.</span></span>|
|<span data-ttu-id="65bc6-507">defenderSecurityCenterDisableNetworkUI</span><span class="sxs-lookup"><span data-stu-id="65bc6-507">defenderSecurityCenterDisableNetworkUI</span></span>|<span data-ttu-id="65bc6-508">Boolean</span><span class="sxs-lookup"><span data-stu-id="65bc6-508">Boolean</span></span>|<span data-ttu-id="65bc6-509">用于禁用防火墙和网络防护区域的显示。</span><span class="sxs-lookup"><span data-stu-id="65bc6-509">Used to disable the display of the firewall and network protection area.</span></span>|
|<span data-ttu-id="65bc6-510">defenderSecurityCenterDisableVirusUI</span><span class="sxs-lookup"><span data-stu-id="65bc6-510">defenderSecurityCenterDisableVirusUI</span></span>|<span data-ttu-id="65bc6-511">Boolean</span><span class="sxs-lookup"><span data-stu-id="65bc6-511">Boolean</span></span>|<span data-ttu-id="65bc6-512">用于禁用病毒和威胁防护区域的显示。</span><span class="sxs-lookup"><span data-stu-id="65bc6-512">Used to disable the display of the virus and threat protection area.</span></span>|
|<span data-ttu-id="65bc6-513">defenderSecurityCenterDisableAccountUI</span><span class="sxs-lookup"><span data-stu-id="65bc6-513">defenderSecurityCenterDisableAccountUI</span></span>|<span data-ttu-id="65bc6-514">Boolean</span><span class="sxs-lookup"><span data-stu-id="65bc6-514">Boolean</span></span>|<span data-ttu-id="65bc6-515">用于禁用帐户保护区域的显示。</span><span class="sxs-lookup"><span data-stu-id="65bc6-515">Used to disable the display of the account protection area.</span></span>|
|<span data-ttu-id="65bc6-516">defenderSecurityCenterDisableClearTpmUI</span><span class="sxs-lookup"><span data-stu-id="65bc6-516">defenderSecurityCenterDisableClearTpmUI</span></span>|<span data-ttu-id="65bc6-517">Boolean</span><span class="sxs-lookup"><span data-stu-id="65bc6-517">Boolean</span></span>|<span data-ttu-id="65bc6-518">用于禁用 "清除 TPM" 按钮的显示。</span><span class="sxs-lookup"><span data-stu-id="65bc6-518">Used to disable the display of the Clear TPM button.</span></span>|
|<span data-ttu-id="65bc6-519">defenderSecurityCenterDisableHardwareUI</span><span class="sxs-lookup"><span data-stu-id="65bc6-519">defenderSecurityCenterDisableHardwareUI</span></span>|<span data-ttu-id="65bc6-520">Boolean</span><span class="sxs-lookup"><span data-stu-id="65bc6-520">Boolean</span></span>|<span data-ttu-id="65bc6-521">用于禁用硬件保护区域的显示。</span><span class="sxs-lookup"><span data-stu-id="65bc6-521">Used to disable the display of the hardware protection area.</span></span>|
|<span data-ttu-id="65bc6-522">defenderSecurityCenterDisableNotificationAreaUI</span><span class="sxs-lookup"><span data-stu-id="65bc6-522">defenderSecurityCenterDisableNotificationAreaUI</span></span>|<span data-ttu-id="65bc6-523">Boolean</span><span class="sxs-lookup"><span data-stu-id="65bc6-523">Boolean</span></span>|<span data-ttu-id="65bc6-524">用于禁用通知区域控件的显示。</span><span class="sxs-lookup"><span data-stu-id="65bc6-524">Used to disable the display of the notification area control.</span></span> <span data-ttu-id="65bc6-525">用户需要注销并登录或重新启动计算机, 此设置才会生效。</span><span class="sxs-lookup"><span data-stu-id="65bc6-525">The user needs to either sign out and sign in or reboot the computer for this setting to take effect.</span></span>|
|<span data-ttu-id="65bc6-526">defenderSecurityCenterDisableRansomwareUI</span><span class="sxs-lookup"><span data-stu-id="65bc6-526">defenderSecurityCenterDisableRansomwareUI</span></span>|<span data-ttu-id="65bc6-527">Boolean</span><span class="sxs-lookup"><span data-stu-id="65bc6-527">Boolean</span></span>|<span data-ttu-id="65bc6-528">用于禁用勒索软件防护区域的显示。</span><span class="sxs-lookup"><span data-stu-id="65bc6-528">Used to disable the display of the ransomware protection area.</span></span> |
|<span data-ttu-id="65bc6-529">defenderSecurityCenterDisableSecureBootUI</span><span class="sxs-lookup"><span data-stu-id="65bc6-529">defenderSecurityCenterDisableSecureBootUI</span></span>|<span data-ttu-id="65bc6-530">Boolean</span><span class="sxs-lookup"><span data-stu-id="65bc6-530">Boolean</span></span>|<span data-ttu-id="65bc6-531">用于在 "设备安全性" 下禁用安全引导区域的显示。</span><span class="sxs-lookup"><span data-stu-id="65bc6-531">Used to disable the display of the secure boot area under Device security.</span></span>|
|<span data-ttu-id="65bc6-532">defenderSecurityCenterDisableTroubleshootingUI</span><span class="sxs-lookup"><span data-stu-id="65bc6-532">defenderSecurityCenterDisableTroubleshootingUI</span></span>|<span data-ttu-id="65bc6-533">Boolean</span><span class="sxs-lookup"><span data-stu-id="65bc6-533">Boolean</span></span>|<span data-ttu-id="65bc6-534">用于在 "设备安全性" 下禁用安全过程故障排除的显示。</span><span class="sxs-lookup"><span data-stu-id="65bc6-534">Used to disable the display of the security process troubleshooting under Device security.</span></span>|
|<span data-ttu-id="65bc6-535">defenderSecurityCenterDisableVulnerableTpmFirmwareUpdateUI</span><span class="sxs-lookup"><span data-stu-id="65bc6-535">defenderSecurityCenterDisableVulnerableTpmFirmwareUpdateUI</span></span>|<span data-ttu-id="65bc6-536">Boolean</span><span class="sxs-lookup"><span data-stu-id="65bc6-536">Boolean</span></span>|<span data-ttu-id="65bc6-537">用于在检测到易受攻击的固件时禁用显示更新 TPM 固件。</span><span class="sxs-lookup"><span data-stu-id="65bc6-537">Used to disable the display of update TPM Firmware when a vulnerable firmware is detected.</span></span>|
|<span data-ttu-id="65bc6-538">defenderSecurityCenterOrganizationDisplayName</span><span class="sxs-lookup"><span data-stu-id="65bc6-538">defenderSecurityCenterOrganizationDisplayName</span></span>|<span data-ttu-id="65bc6-539">String</span><span class="sxs-lookup"><span data-stu-id="65bc6-539">String</span></span>|<span data-ttu-id="65bc6-540">向用户显示的公司名称。</span><span class="sxs-lookup"><span data-stu-id="65bc6-540">The company name that is displayed to the users.</span></span>|
|<span data-ttu-id="65bc6-541">defenderSecurityCenterHelpEmail</span><span class="sxs-lookup"><span data-stu-id="65bc6-541">defenderSecurityCenterHelpEmail</span></span>|<span data-ttu-id="65bc6-542">String</span><span class="sxs-lookup"><span data-stu-id="65bc6-542">String</span></span>|<span data-ttu-id="65bc6-543">向用户显示的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="65bc6-543">The email address that is displayed to users.</span></span>|
|<span data-ttu-id="65bc6-544">defenderSecurityCenterHelpPhone</span><span class="sxs-lookup"><span data-stu-id="65bc6-544">defenderSecurityCenterHelpPhone</span></span>|<span data-ttu-id="65bc6-545">String</span><span class="sxs-lookup"><span data-stu-id="65bc6-545">String</span></span>|<span data-ttu-id="65bc6-546">向用户显示的电话号码或 Skype ID。</span><span class="sxs-lookup"><span data-stu-id="65bc6-546">The phone number or Skype ID that is displayed to users.</span></span>|
|<span data-ttu-id="65bc6-547">defenderSecurityCenterHelpURL</span><span class="sxs-lookup"><span data-stu-id="65bc6-547">defenderSecurityCenterHelpURL</span></span>|<span data-ttu-id="65bc6-548">String</span><span class="sxs-lookup"><span data-stu-id="65bc6-548">String</span></span>|<span data-ttu-id="65bc6-549">"帮助" 门户 URL 将向用户显示。</span><span class="sxs-lookup"><span data-stu-id="65bc6-549">The help portal URL this is displayed to users.</span></span>|
|<span data-ttu-id="65bc6-550">defenderSecurityCenterNotificationsFromApp</span><span class="sxs-lookup"><span data-stu-id="65bc6-550">defenderSecurityCenterNotificationsFromApp</span></span>|[<span data-ttu-id="65bc6-551">defenderSecurityCenterNotificationsFromAppType</span><span class="sxs-lookup"><span data-stu-id="65bc6-551">defenderSecurityCenterNotificationsFromAppType</span></span>](../resources/intune-deviceconfig-defendersecuritycenternotificationsfromapptype.md)|<span data-ttu-id="65bc6-552">要从应用程序的显示区域中显示的通知。</span><span class="sxs-lookup"><span data-stu-id="65bc6-552">Notifications to show from the displayed areas of app.</span></span> <span data-ttu-id="65bc6-553">可取值为：`notConfigured`、`blockNoncriticalNotifications`、`blockAllNotifications`。</span><span class="sxs-lookup"><span data-stu-id="65bc6-553">Possible values are: `notConfigured`, `blockNoncriticalNotifications`, `blockAllNotifications`.</span></span>|
|<span data-ttu-id="65bc6-554">defenderSecurityCenterITContactDisplay</span><span class="sxs-lookup"><span data-stu-id="65bc6-554">defenderSecurityCenterITContactDisplay</span></span>|[<span data-ttu-id="65bc6-555">defenderSecurityCenterITContactDisplayType</span><span class="sxs-lookup"><span data-stu-id="65bc6-555">defenderSecurityCenterITContactDisplayType</span></span>](../resources/intune-deviceconfig-defendersecuritycenteritcontactdisplaytype.md)|<span data-ttu-id="65bc6-556">配置向最终用户显示 IT 联系人信息的位置。</span><span class="sxs-lookup"><span data-stu-id="65bc6-556">Configure where to display IT contact information to end users.</span></span> <span data-ttu-id="65bc6-557">可取值为：`notConfigured`、`displayInAppAndInNotifications`、`displayOnlyInApp`、`displayOnlyInNotifications`。</span><span class="sxs-lookup"><span data-stu-id="65bc6-557">Possible values are: `notConfigured`, `displayInAppAndInNotifications`, `displayOnlyInApp`, `displayOnlyInNotifications`.</span></span>|
|<span data-ttu-id="65bc6-558">firewallBlockStatefulFTP</span><span class="sxs-lookup"><span data-stu-id="65bc6-558">firewallBlockStatefulFTP</span></span>|<span data-ttu-id="65bc6-559">Boolean</span><span class="sxs-lookup"><span data-stu-id="65bc6-559">Boolean</span></span>|<span data-ttu-id="65bc6-560">阻止到设备的有状态 FTP 连接</span><span class="sxs-lookup"><span data-stu-id="65bc6-560">Blocks stateful FTP connections to the device</span></span>|
|<span data-ttu-id="65bc6-561">firewallIdleTimeoutForSecurityAssociationInSeconds</span><span class="sxs-lookup"><span data-stu-id="65bc6-561">firewallIdleTimeoutForSecurityAssociationInSeconds</span></span>|<span data-ttu-id="65bc6-562">Int32</span><span class="sxs-lookup"><span data-stu-id="65bc6-562">Int32</span></span>|<span data-ttu-id="65bc6-563">配置安全关联的空闲超时（以秒为单位），值范围为 300 到 3600（包括这两个值）。</span><span class="sxs-lookup"><span data-stu-id="65bc6-563">Configures the idle timeout for security associations, in seconds, from 300 to 3600 inclusive.</span></span> <span data-ttu-id="65bc6-564">这是一个时间段，在此之后安全关联将过期并被删除。</span><span class="sxs-lookup"><span data-stu-id="65bc6-564">This is the period after which security associations will expire and be deleted.</span></span> <span data-ttu-id="65bc6-565">有效值为 300 至 3600</span><span class="sxs-lookup"><span data-stu-id="65bc6-565">Valid values 300 to 3600</span></span>|
|<span data-ttu-id="65bc6-566">firewallPreSharedKeyEncodingMethod</span><span class="sxs-lookup"><span data-stu-id="65bc6-566">firewallPreSharedKeyEncodingMethod</span></span>|[<span data-ttu-id="65bc6-567">firewallPreSharedKeyEncodingMethodType</span><span class="sxs-lookup"><span data-stu-id="65bc6-567">firewallPreSharedKeyEncodingMethodType</span></span>](../resources/intune-deviceconfig-firewallpresharedkeyencodingmethodtype.md)|<span data-ttu-id="65bc6-568">选择要使用的预共享密钥编码。</span><span class="sxs-lookup"><span data-stu-id="65bc6-568">Select the preshared key encoding to be used.</span></span> <span data-ttu-id="65bc6-569">可取值为：`deviceDefault`、`none`、`utF8`。</span><span class="sxs-lookup"><span data-stu-id="65bc6-569">Possible values are: `deviceDefault`, `none`, `utF8`.</span></span>|
|<span data-ttu-id="65bc6-570">firewallIPSecExemptionsAllowNeighborDiscovery</span><span class="sxs-lookup"><span data-stu-id="65bc6-570">firewallIPSecExemptionsAllowNeighborDiscovery</span></span>|<span data-ttu-id="65bc6-571">Boolean</span><span class="sxs-lookup"><span data-stu-id="65bc6-571">Boolean</span></span>|<span data-ttu-id="65bc6-572">配置 IPSec 免除项以允许邻居发现 IPv6 ICMP 类型代码</span><span class="sxs-lookup"><span data-stu-id="65bc6-572">Configures IPSec exemptions to allow neighbor discovery IPv6 ICMP type-codes</span></span>|
|<span data-ttu-id="65bc6-573">firewallIPSecExemptionsAllowICMP</span><span class="sxs-lookup"><span data-stu-id="65bc6-573">firewallIPSecExemptionsAllowICMP</span></span>|<span data-ttu-id="65bc6-574">Boolean</span><span class="sxs-lookup"><span data-stu-id="65bc6-574">Boolean</span></span>|<span data-ttu-id="65bc6-575">配置 IPSec 免除项以允许 ICMP</span><span class="sxs-lookup"><span data-stu-id="65bc6-575">Configures IPSec exemptions to allow ICMP</span></span>|
|<span data-ttu-id="65bc6-576">firewallIPSecExemptionsAllowRouterDiscovery</span><span class="sxs-lookup"><span data-stu-id="65bc6-576">firewallIPSecExemptionsAllowRouterDiscovery</span></span>|<span data-ttu-id="65bc6-577">Boolean</span><span class="sxs-lookup"><span data-stu-id="65bc6-577">Boolean</span></span>|<span data-ttu-id="65bc6-578">配置 IPSec 免除项以允许路由器发现 IPv6 ICMP 类型代码</span><span class="sxs-lookup"><span data-stu-id="65bc6-578">Configures IPSec exemptions to allow router discovery IPv6 ICMP type-codes</span></span>|
|<span data-ttu-id="65bc6-579">firewallIPSecExemptionsAllowDHCP</span><span class="sxs-lookup"><span data-stu-id="65bc6-579">firewallIPSecExemptionsAllowDHCP</span></span>|<span data-ttu-id="65bc6-580">Boolean</span><span class="sxs-lookup"><span data-stu-id="65bc6-580">Boolean</span></span>|<span data-ttu-id="65bc6-581">配置 IPSec 免除项以允许 IPv4 和 IPv6 DHCP 通信</span><span class="sxs-lookup"><span data-stu-id="65bc6-581">Configures IPSec exemptions to allow both IPv4 and IPv6 DHCP traffic</span></span>|
|<span data-ttu-id="65bc6-582">firewallCertificateRevocationListCheckMethod</span><span class="sxs-lookup"><span data-stu-id="65bc6-582">firewallCertificateRevocationListCheckMethod</span></span>|[<span data-ttu-id="65bc6-583">firewallCertificateRevocationListCheckMethodType</span><span class="sxs-lookup"><span data-stu-id="65bc6-583">firewallCertificateRevocationListCheckMethodType</span></span>](../resources/intune-deviceconfig-firewallcertificaterevocationlistcheckmethodtype.md)|<span data-ttu-id="65bc6-584">指定如何强制执行证书吊销列表。</span><span class="sxs-lookup"><span data-stu-id="65bc6-584">Specify how the certificate revocation list is to be enforced.</span></span> <span data-ttu-id="65bc6-585">可取值为：`deviceDefault`、`none`、`attempt`、`require`。</span><span class="sxs-lookup"><span data-stu-id="65bc6-585">Possible values are: `deviceDefault`, `none`, `attempt`, `require`.</span></span>|
|<span data-ttu-id="65bc6-586">firewallMergeKeyingModuleSettings</span><span class="sxs-lookup"><span data-stu-id="65bc6-586">firewallMergeKeyingModuleSettings</span></span>|<span data-ttu-id="65bc6-587">Boolean</span><span class="sxs-lookup"><span data-stu-id="65bc6-587">Boolean</span></span>|<span data-ttu-id="65bc6-588">如果键控模块不完全支持身份验证集，请指示模块仅忽略不受支持的身份验证套件而不是整个集</span><span class="sxs-lookup"><span data-stu-id="65bc6-588">If an authentication set is not fully supported by a keying module, direct the module to ignore only unsupported authentication suites rather than the entire set</span></span>|
|<span data-ttu-id="65bc6-589">firewallPacketQueueingMethod</span><span class="sxs-lookup"><span data-stu-id="65bc6-589">firewallPacketQueueingMethod</span></span>|[<span data-ttu-id="65bc6-590">firewallPacketQueueingMethodType</span><span class="sxs-lookup"><span data-stu-id="65bc6-590">firewallPacketQueueingMethodType</span></span>](../resources/intune-deviceconfig-firewallpacketqueueingmethodtype.md)|<span data-ttu-id="65bc6-591">配置如何在隧道网关应用场景中应用数据包排队。</span><span class="sxs-lookup"><span data-stu-id="65bc6-591">Configures how packet queueing should be applied in the tunnel gateway scenario.</span></span> <span data-ttu-id="65bc6-592">可取值为：`deviceDefault`、`disabled`、`queueInbound`、`queueOutbound`、`queueBoth`。</span><span class="sxs-lookup"><span data-stu-id="65bc6-592">Possible values are: `deviceDefault`, `disabled`, `queueInbound`, `queueOutbound`, `queueBoth`.</span></span>|
|<span data-ttu-id="65bc6-593">firewallProfileDomain</span><span class="sxs-lookup"><span data-stu-id="65bc6-593">firewallProfileDomain</span></span>|[<span data-ttu-id="65bc6-594">windowsFirewallNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="65bc6-594">windowsFirewallNetworkProfile</span></span>](../resources/intune-deviceconfig-windowsfirewallnetworkprofile.md)|<span data-ttu-id="65bc6-595">配置域网络的防火墙配置文件设置</span><span class="sxs-lookup"><span data-stu-id="65bc6-595">Configures the firewall profile settings for domain networks</span></span>|
|<span data-ttu-id="65bc6-596">firewallProfilePublic</span><span class="sxs-lookup"><span data-stu-id="65bc6-596">firewallProfilePublic</span></span>|[<span data-ttu-id="65bc6-597">windowsFirewallNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="65bc6-597">windowsFirewallNetworkProfile</span></span>](../resources/intune-deviceconfig-windowsfirewallnetworkprofile.md)|<span data-ttu-id="65bc6-598">配置公用网络的防火墙配置文件设置</span><span class="sxs-lookup"><span data-stu-id="65bc6-598">Configures the firewall profile settings for public networks</span></span>|
|<span data-ttu-id="65bc6-599">firewallProfilePrivate</span><span class="sxs-lookup"><span data-stu-id="65bc6-599">firewallProfilePrivate</span></span>|[<span data-ttu-id="65bc6-600">windowsFirewallNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="65bc6-600">windowsFirewallNetworkProfile</span></span>](../resources/intune-deviceconfig-windowsfirewallnetworkprofile.md)|<span data-ttu-id="65bc6-601">配置专用网络的防火墙配置文件设置</span><span class="sxs-lookup"><span data-stu-id="65bc6-601">Configures the firewall profile settings for private networks</span></span>|
|<span data-ttu-id="65bc6-602">defenderAdobeReaderLaunchChildProcess</span><span class="sxs-lookup"><span data-stu-id="65bc6-602">defenderAdobeReaderLaunchChildProcess</span></span>|[<span data-ttu-id="65bc6-603">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="65bc6-603">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="65bc6-604">值, 该值指示 Adobe Reader 创建子进程的行为。</span><span class="sxs-lookup"><span data-stu-id="65bc6-604">Value indicating the behavior of Adobe Reader from creating child processes.</span></span> <span data-ttu-id="65bc6-605">可取值为：`userDefined`、`enable`、`auditMode`。</span><span class="sxs-lookup"><span data-stu-id="65bc6-605">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="65bc6-606">defenderAttackSurfaceReductionExcludedPaths</span><span class="sxs-lookup"><span data-stu-id="65bc6-606">defenderAttackSurfaceReductionExcludedPaths</span></span>|<span data-ttu-id="65bc6-607">String 集合</span><span class="sxs-lookup"><span data-stu-id="65bc6-607">String collection</span></span>|<span data-ttu-id="65bc6-608">要从攻击面减少规则中排除的 exe 文件和文件夹的列表</span><span class="sxs-lookup"><span data-stu-id="65bc6-608">List of exe files and folders to be excluded from attack surface reduction rules</span></span>|
|<span data-ttu-id="65bc6-609">defenderOfficeAppsOtherProcessInjectionType</span><span class="sxs-lookup"><span data-stu-id="65bc6-609">defenderOfficeAppsOtherProcessInjectionType</span></span>|[<span data-ttu-id="65bc6-610">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="65bc6-610">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="65bc6-611">值, 该值指示插入到其他进程中的 Office 应用程序的行为。</span><span class="sxs-lookup"><span data-stu-id="65bc6-611">Value indicating the behavior of Office applications injecting into other processes.</span></span> <span data-ttu-id="65bc6-612">可取值为：`userDefined`、`block`、`auditMode`。</span><span class="sxs-lookup"><span data-stu-id="65bc6-612">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="65bc6-613">defenderOfficeAppsOtherProcessInjection</span><span class="sxs-lookup"><span data-stu-id="65bc6-613">defenderOfficeAppsOtherProcessInjection</span></span>|[<span data-ttu-id="65bc6-614">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="65bc6-614">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="65bc6-615">值, 该值指示插入到其他进程中的 Office 应用程序的行为。</span><span class="sxs-lookup"><span data-stu-id="65bc6-615">Value indicating the behavior of  Office applications injecting into other processes.</span></span> <span data-ttu-id="65bc6-616">可取值为：`userDefined`、`enable`、`auditMode`。</span><span class="sxs-lookup"><span data-stu-id="65bc6-616">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="65bc6-617">defenderOfficeCommunicationAppsLaunchChildProcess</span><span class="sxs-lookup"><span data-stu-id="65bc6-617">defenderOfficeCommunicationAppsLaunchChildProcess</span></span>|[<span data-ttu-id="65bc6-618">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="65bc6-618">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="65bc6-619">值, 该值指示 Office 通信应用程序 (包括 Microsoft Outlook) 在创建子进程时的行为。</span><span class="sxs-lookup"><span data-stu-id="65bc6-619">Value indicating the behavior of Office communication applications, including Microsoft Outlook, from creating child processes.</span></span> <span data-ttu-id="65bc6-620">可取值为：`userDefined`、`enable`、`auditMode`。</span><span class="sxs-lookup"><span data-stu-id="65bc6-620">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="65bc6-621">defenderOfficeAppsExecutableContentCreationOrLaunchType</span><span class="sxs-lookup"><span data-stu-id="65bc6-621">defenderOfficeAppsExecutableContentCreationOrLaunchType</span></span>|[<span data-ttu-id="65bc6-622">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="65bc6-622">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="65bc6-623">值, 该值指示 Office 应用程序/宏创建或启动可执行内容的行为。</span><span class="sxs-lookup"><span data-stu-id="65bc6-623">Value indicating the behavior of Office applications/macros creating or launching executable content.</span></span> <span data-ttu-id="65bc6-624">可取值为：`userDefined`、`block`、`auditMode`。</span><span class="sxs-lookup"><span data-stu-id="65bc6-624">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="65bc6-625">defenderOfficeAppsExecutableContentCreationOrLaunch</span><span class="sxs-lookup"><span data-stu-id="65bc6-625">defenderOfficeAppsExecutableContentCreationOrLaunch</span></span>|[<span data-ttu-id="65bc6-626">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="65bc6-626">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="65bc6-627">值, 该值指示 Office 应用程序/宏创建或启动可执行内容的行为。</span><span class="sxs-lookup"><span data-stu-id="65bc6-627">Value indicating the behavior of Office applications/macros creating or launching executable content.</span></span> <span data-ttu-id="65bc6-628">可取值为：`userDefined`、`enable`、`auditMode`。</span><span class="sxs-lookup"><span data-stu-id="65bc6-628">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="65bc6-629">defenderOfficeAppsLaunchChildProcessType</span><span class="sxs-lookup"><span data-stu-id="65bc6-629">defenderOfficeAppsLaunchChildProcessType</span></span>|[<span data-ttu-id="65bc6-630">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="65bc6-630">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="65bc6-631">值, 该值指示 Office 应用程序启动子进程的行为。</span><span class="sxs-lookup"><span data-stu-id="65bc6-631">Value indicating the behavior of Office application launching child processes.</span></span> <span data-ttu-id="65bc6-632">可取值为：`userDefined`、`block`、`auditMode`。</span><span class="sxs-lookup"><span data-stu-id="65bc6-632">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="65bc6-633">defenderOfficeAppsLaunchChildProcess</span><span class="sxs-lookup"><span data-stu-id="65bc6-633">defenderOfficeAppsLaunchChildProcess</span></span>|[<span data-ttu-id="65bc6-634">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="65bc6-634">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="65bc6-635">值, 该值指示 Office 应用程序启动子进程的行为。</span><span class="sxs-lookup"><span data-stu-id="65bc6-635">Value indicating the behavior of Office application launching child processes.</span></span> <span data-ttu-id="65bc6-636">可取值为：`userDefined`、`enable`、`auditMode`。</span><span class="sxs-lookup"><span data-stu-id="65bc6-636">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="65bc6-637">defenderOfficeMacroCodeAllowWin32ImportsType</span><span class="sxs-lookup"><span data-stu-id="65bc6-637">defenderOfficeMacroCodeAllowWin32ImportsType</span></span>|[<span data-ttu-id="65bc6-638">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="65bc6-638">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="65bc6-639">值, 该值指示从 Office 中的宏代码的 Win32 导入行为。</span><span class="sxs-lookup"><span data-stu-id="65bc6-639">Value indicating the behavior of Win32 imports from Macro code in Office.</span></span> <span data-ttu-id="65bc6-640">可取值为：`userDefined`、`block`、`auditMode`。</span><span class="sxs-lookup"><span data-stu-id="65bc6-640">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="65bc6-641">defenderOfficeMacroCodeAllowWin32Imports</span><span class="sxs-lookup"><span data-stu-id="65bc6-641">defenderOfficeMacroCodeAllowWin32Imports</span></span>|[<span data-ttu-id="65bc6-642">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="65bc6-642">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="65bc6-643">值, 该值指示从 Office 中的宏代码的 Win32 导入行为。</span><span class="sxs-lookup"><span data-stu-id="65bc6-643">Value indicating the behavior of Win32 imports from Macro code in Office.</span></span> <span data-ttu-id="65bc6-644">可取值为：`userDefined`、`enable`、`auditMode`。</span><span class="sxs-lookup"><span data-stu-id="65bc6-644">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="65bc6-645">defenderScriptObfuscatedMacroCodeType</span><span class="sxs-lookup"><span data-stu-id="65bc6-645">defenderScriptObfuscatedMacroCodeType</span></span>|[<span data-ttu-id="65bc6-646">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="65bc6-646">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="65bc6-647">值, 该值指示模糊的 js/vbs/ps/宏代码的行为。</span><span class="sxs-lookup"><span data-stu-id="65bc6-647">Value indicating the behavior of obfuscated js/vbs/ps/macro code.</span></span> <span data-ttu-id="65bc6-648">可取值为：`userDefined`、`block`、`auditMode`。</span><span class="sxs-lookup"><span data-stu-id="65bc6-648">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="65bc6-649">defenderScriptObfuscatedMacroCode</span><span class="sxs-lookup"><span data-stu-id="65bc6-649">defenderScriptObfuscatedMacroCode</span></span>|[<span data-ttu-id="65bc6-650">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="65bc6-650">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="65bc6-651">值, 该值指示模糊的 js/vbs/ps/宏代码的行为。</span><span class="sxs-lookup"><span data-stu-id="65bc6-651">Value indicating the behavior of obfuscated js/vbs/ps/macro code.</span></span> <span data-ttu-id="65bc6-652">可取值为：`userDefined`、`enable`、`auditMode`。</span><span class="sxs-lookup"><span data-stu-id="65bc6-652">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="65bc6-653">defenderScriptDownloadedPayloadExecutionType</span><span class="sxs-lookup"><span data-stu-id="65bc6-653">defenderScriptDownloadedPayloadExecutionType</span></span>|[<span data-ttu-id="65bc6-654">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="65bc6-654">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="65bc6-655">值, 该值指示从 Internet 下载的 js/vbs 执行负载的行为。</span><span class="sxs-lookup"><span data-stu-id="65bc6-655">Value indicating the behavior of js/vbs executing payload downloaded from Internet.</span></span> <span data-ttu-id="65bc6-656">可取值为：`userDefined`、`block`、`auditMode`。</span><span class="sxs-lookup"><span data-stu-id="65bc6-656">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="65bc6-657">defenderScriptDownloadedPayloadExecution</span><span class="sxs-lookup"><span data-stu-id="65bc6-657">defenderScriptDownloadedPayloadExecution</span></span>|[<span data-ttu-id="65bc6-658">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="65bc6-658">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="65bc6-659">值, 该值指示从 Internet 下载的 js/vbs 执行负载的行为。</span><span class="sxs-lookup"><span data-stu-id="65bc6-659">Value indicating the behavior of js/vbs executing payload downloaded from Internet.</span></span> <span data-ttu-id="65bc6-660">可取值为：`userDefined`、`enable`、`auditMode`。</span><span class="sxs-lookup"><span data-stu-id="65bc6-660">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="65bc6-661">defenderPreventCredentialStealingType</span><span class="sxs-lookup"><span data-stu-id="65bc6-661">defenderPreventCredentialStealingType</span></span>|[<span data-ttu-id="65bc6-662">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="65bc6-662">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="65bc6-663">值, 该值指示是否允许从 Windows 本地安全机构子系统中盗取凭据。</span><span class="sxs-lookup"><span data-stu-id="65bc6-663">Value indicating if credential stealing from the Windows local security authority subsystem is permitted.</span></span> <span data-ttu-id="65bc6-664">可取值为：`userDefined`、`enable`、`auditMode`。</span><span class="sxs-lookup"><span data-stu-id="65bc6-664">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="65bc6-665">defenderProcessCreationType</span><span class="sxs-lookup"><span data-stu-id="65bc6-665">defenderProcessCreationType</span></span>|[<span data-ttu-id="65bc6-666">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="65bc6-666">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="65bc6-667">一个值, 该值指示对源自 PSExec 和 WMI 命令的进程创建的响应。</span><span class="sxs-lookup"><span data-stu-id="65bc6-667">Value indicating response to process creations originating from PSExec and WMI commands.</span></span> <span data-ttu-id="65bc6-668">可取值为：`userDefined`、`block`、`auditMode`。</span><span class="sxs-lookup"><span data-stu-id="65bc6-668">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="65bc6-669">defenderProcessCreation</span><span class="sxs-lookup"><span data-stu-id="65bc6-669">defenderProcessCreation</span></span>|[<span data-ttu-id="65bc6-670">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="65bc6-670">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="65bc6-671">一个值, 该值指示对源自 PSExec 和 WMI 命令的进程创建的响应。</span><span class="sxs-lookup"><span data-stu-id="65bc6-671">Value indicating response to process creations originating from PSExec and WMI commands.</span></span> <span data-ttu-id="65bc6-672">可取值为：`userDefined`、`enable`、`auditMode`。</span><span class="sxs-lookup"><span data-stu-id="65bc6-672">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="65bc6-673">defenderUntrustedUSBProcessType</span><span class="sxs-lookup"><span data-stu-id="65bc6-673">defenderUntrustedUSBProcessType</span></span>|[<span data-ttu-id="65bc6-674">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="65bc6-674">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="65bc6-675">指示对从 USB 运行的不受信任和未签名进程的响应的值。</span><span class="sxs-lookup"><span data-stu-id="65bc6-675">Value indicating response to untrusted and unsigned processes that run from USB.</span></span> <span data-ttu-id="65bc6-676">可取值为：`userDefined`、`block`、`auditMode`。</span><span class="sxs-lookup"><span data-stu-id="65bc6-676">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="65bc6-677">defenderUntrustedUSBProcess</span><span class="sxs-lookup"><span data-stu-id="65bc6-677">defenderUntrustedUSBProcess</span></span>|[<span data-ttu-id="65bc6-678">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="65bc6-678">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="65bc6-679">指示对从 USB 运行的不受信任和未签名进程的响应的值。</span><span class="sxs-lookup"><span data-stu-id="65bc6-679">Value indicating response to untrusted and unsigned processes that run from USB.</span></span> <span data-ttu-id="65bc6-680">可取值为：`userDefined`、`enable`、`auditMode`。</span><span class="sxs-lookup"><span data-stu-id="65bc6-680">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="65bc6-681">defenderUntrustedExecutableType</span><span class="sxs-lookup"><span data-stu-id="65bc6-681">defenderUntrustedExecutableType</span></span>|[<span data-ttu-id="65bc6-682">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="65bc6-682">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="65bc6-683">指示对不符合流行、年龄或受信任列表条件的可执行文件的响应的值。</span><span class="sxs-lookup"><span data-stu-id="65bc6-683">Value indicating response to executables that don't meet a prevalence, age, or trusted list criteria.</span></span> <span data-ttu-id="65bc6-684">可取值为：`userDefined`、`block`、`auditMode`。</span><span class="sxs-lookup"><span data-stu-id="65bc6-684">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="65bc6-685">defenderUntrustedExecutable</span><span class="sxs-lookup"><span data-stu-id="65bc6-685">defenderUntrustedExecutable</span></span>|[<span data-ttu-id="65bc6-686">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="65bc6-686">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="65bc6-687">指示对不符合流行、年龄或受信任列表条件的可执行文件的响应的值。</span><span class="sxs-lookup"><span data-stu-id="65bc6-687">Value indicating response to executables that don't meet a prevalence, age, or trusted list criteria.</span></span> <span data-ttu-id="65bc6-688">可取值为：`userDefined`、`enable`、`auditMode`。</span><span class="sxs-lookup"><span data-stu-id="65bc6-688">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="65bc6-689">defenderEmailContentExecutionType</span><span class="sxs-lookup"><span data-stu-id="65bc6-689">defenderEmailContentExecutionType</span></span>|[<span data-ttu-id="65bc6-690">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="65bc6-690">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="65bc6-691">一个值, 该值指示是否应从电子邮件 (web 邮件/邮件客户端) 中删除可执行内容 (exe、dll、ps、js、vbs 等) 的执行。</span><span class="sxs-lookup"><span data-stu-id="65bc6-691">Value indicating if execution of executable content (exe, dll, ps, js, vbs, etc) should be dropped from email (webmail/mail-client).</span></span> <span data-ttu-id="65bc6-692">可取值为：`userDefined`、`block`、`auditMode`。</span><span class="sxs-lookup"><span data-stu-id="65bc6-692">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="65bc6-693">defenderEmailContentExecution</span><span class="sxs-lookup"><span data-stu-id="65bc6-693">defenderEmailContentExecution</span></span>|[<span data-ttu-id="65bc6-694">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="65bc6-694">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="65bc6-695">一个值, 该值指示是否应从电子邮件 (web 邮件/邮件客户端) 中删除可执行内容 (exe、dll、ps、js、vbs 等) 的执行。</span><span class="sxs-lookup"><span data-stu-id="65bc6-695">Value indicating if execution of executable content (exe, dll, ps, js, vbs, etc) should be dropped from email (webmail/mail-client).</span></span> <span data-ttu-id="65bc6-696">可取值为：`userDefined`、`enable`、`auditMode`。</span><span class="sxs-lookup"><span data-stu-id="65bc6-696">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="65bc6-697">defenderAdvancedRansomewareProtectionType</span><span class="sxs-lookup"><span data-stu-id="65bc6-697">defenderAdvancedRansomewareProtectionType</span></span>|[<span data-ttu-id="65bc6-698">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="65bc6-698">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="65bc6-699">指示使用针对 ransomeware 的高级防护的值。</span><span class="sxs-lookup"><span data-stu-id="65bc6-699">Value indicating use of advanced protection against ransomeware.</span></span> <span data-ttu-id="65bc6-700">可取值为：`userDefined`、`enable`、`auditMode`。</span><span class="sxs-lookup"><span data-stu-id="65bc6-700">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="65bc6-701">defenderGuardMyFoldersType</span><span class="sxs-lookup"><span data-stu-id="65bc6-701">defenderGuardMyFoldersType</span></span>|[<span data-ttu-id="65bc6-702">folderProtectionType</span><span class="sxs-lookup"><span data-stu-id="65bc6-702">folderProtectionType</span></span>](../resources/intune-deviceconfig-folderprotectiontype.md)|<span data-ttu-id="65bc6-703">值, 该值指示受保护文件夹的行为。</span><span class="sxs-lookup"><span data-stu-id="65bc6-703">Value indicating the behavior of protected folders.</span></span> <span data-ttu-id="65bc6-704">可取值为：`userDefined`、`enable`、`auditMode`、`blockDiskModification`、`auditDiskModification`。</span><span class="sxs-lookup"><span data-stu-id="65bc6-704">Possible values are: `userDefined`, `enable`, `auditMode`, `blockDiskModification`, `auditDiskModification`.</span></span>|
|<span data-ttu-id="65bc6-705">defenderGuardedFoldersAllowedAppPaths</span><span class="sxs-lookup"><span data-stu-id="65bc6-705">defenderGuardedFoldersAllowedAppPaths</span></span>|<span data-ttu-id="65bc6-706">String collection</span><span class="sxs-lookup"><span data-stu-id="65bc6-706">String collection</span></span>|<span data-ttu-id="65bc6-707">允许访问受保护文件夹的 exe 路径列表</span><span class="sxs-lookup"><span data-stu-id="65bc6-707">List of paths to exe that are allowed to access protected folders</span></span>|
|<span data-ttu-id="65bc6-708">defenderAdditionalGuardedFolders</span><span class="sxs-lookup"><span data-stu-id="65bc6-708">defenderAdditionalGuardedFolders</span></span>|<span data-ttu-id="65bc6-709">String 集合</span><span class="sxs-lookup"><span data-stu-id="65bc6-709">String collection</span></span>|<span data-ttu-id="65bc6-710">要添加到受保护文件夹列表的文件夹路径列表</span><span class="sxs-lookup"><span data-stu-id="65bc6-710">List of folder paths to be added to the list of protected folders</span></span>|
|<span data-ttu-id="65bc6-711">defenderNetworkProtectionType</span><span class="sxs-lookup"><span data-stu-id="65bc6-711">defenderNetworkProtectionType</span></span>|[<span data-ttu-id="65bc6-712">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="65bc6-712">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="65bc6-713">值, 该值指示 NetworkProtection 的行为。</span><span class="sxs-lookup"><span data-stu-id="65bc6-713">Value indicating the behavior of NetworkProtection.</span></span> <span data-ttu-id="65bc6-714">可取值为：`userDefined`、`enable`、`auditMode`。</span><span class="sxs-lookup"><span data-stu-id="65bc6-714">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="65bc6-715">defenderExploitProtectionXml</span><span class="sxs-lookup"><span data-stu-id="65bc6-715">defenderExploitProtectionXml</span></span>|<span data-ttu-id="65bc6-716">Binary</span><span class="sxs-lookup"><span data-stu-id="65bc6-716">Binary</span></span>|<span data-ttu-id="65bc6-717">包含有关 Exploit Protection 详细信息的 xml 内容。</span><span class="sxs-lookup"><span data-stu-id="65bc6-717">Xml content containing information regarding exploit protection details.</span></span>|
|<span data-ttu-id="65bc6-718">defenderExploitProtectionXmlFileName</span><span class="sxs-lookup"><span data-stu-id="65bc6-718">defenderExploitProtectionXmlFileName</span></span>|<span data-ttu-id="65bc6-719">String</span><span class="sxs-lookup"><span data-stu-id="65bc6-719">String</span></span>|<span data-ttu-id="65bc6-720">从中获取 DefenderExploitProtectionXml 的文件的名称。</span><span class="sxs-lookup"><span data-stu-id="65bc6-720">Name of the file from which DefenderExploitProtectionXml was obtained.</span></span>|
|<span data-ttu-id="65bc6-721">defenderSecurityCenterBlockExploitProtectionOverride</span><span class="sxs-lookup"><span data-stu-id="65bc6-721">defenderSecurityCenterBlockExploitProtectionOverride</span></span>|<span data-ttu-id="65bc6-722">Boolean</span><span class="sxs-lookup"><span data-stu-id="65bc6-722">Boolean</span></span>|<span data-ttu-id="65bc6-723">指示是否阻止用户覆盖 Exploit Protection 设置。</span><span class="sxs-lookup"><span data-stu-id="65bc6-723">Indicates whether or not to block user from overriding Exploit Protection settings.</span></span>|
|<span data-ttu-id="65bc6-724">appLockerApplicationControl</span><span class="sxs-lookup"><span data-stu-id="65bc6-724">appLockerApplicationControl</span></span>|[<span data-ttu-id="65bc6-725">appLockerApplicationControlType</span><span class="sxs-lookup"><span data-stu-id="65bc6-725">appLockerApplicationControlType</span></span>](../resources/intune-deviceconfig-applockerapplicationcontroltype.md)|<span data-ttu-id="65bc6-726">使管理员能够选择在设备上允许哪些类型的应用。</span><span class="sxs-lookup"><span data-stu-id="65bc6-726">Enables the Admin to choose what types of app to allow on devices.</span></span> <span data-ttu-id="65bc6-727">可取值为：`notConfigured`、`enforceComponentsAndStoreApps`、`auditComponentsAndStoreApps`、`enforceComponentsStoreAppsAndSmartlocker`、`auditComponentsStoreAppsAndSmartlocker`。</span><span class="sxs-lookup"><span data-stu-id="65bc6-727">Possible values are: `notConfigured`, `enforceComponentsAndStoreApps`, `auditComponentsAndStoreApps`, `enforceComponentsStoreAppsAndSmartlocker`, `auditComponentsStoreAppsAndSmartlocker`.</span></span>|
|<span data-ttu-id="65bc6-728">deviceGuardLocalSystemAuthorityCredentialGuardSettings</span><span class="sxs-lookup"><span data-stu-id="65bc6-728">deviceGuardLocalSystemAuthorityCredentialGuardSettings</span></span>|[<span data-ttu-id="65bc6-729">deviceGuardLocalSystemAuthorityCredentialGuardType</span><span class="sxs-lookup"><span data-stu-id="65bc6-729">deviceGuardLocalSystemAuthorityCredentialGuardType</span></span>](../resources/intune-deviceconfig-deviceguardlocalsystemauthoritycredentialguardtype.md)|<span data-ttu-id="65bc6-730">如果平台安全级别具有安全启动和基于虚拟化的安全性均已启用, 则打开 Credential Guard。</span><span class="sxs-lookup"><span data-stu-id="65bc6-730">Turn on Credential Guard when Platform Security Level with Secure Boot and Virtualization Based Security are both enabled.</span></span> <span data-ttu-id="65bc6-731">可取值为：`notConfigured`、`enableWithUEFILock`、`enableWithoutUEFILock`。</span><span class="sxs-lookup"><span data-stu-id="65bc6-731">Possible values are: `notConfigured`, `enableWithUEFILock`, `enableWithoutUEFILock`.</span></span>|
|<span data-ttu-id="65bc6-732">deviceGuardEnableVirtualizationBasedSecurity</span><span class="sxs-lookup"><span data-stu-id="65bc6-732">deviceGuardEnableVirtualizationBasedSecurity</span></span>|<span data-ttu-id="65bc6-733">Boolean</span><span class="sxs-lookup"><span data-stu-id="65bc6-733">Boolean</span></span>|<span data-ttu-id="65bc6-734">启用基于虚拟化的安全性 (VBS)。</span><span class="sxs-lookup"><span data-stu-id="65bc6-734">Turns On Virtualization Based Security(VBS).</span></span>|
|<span data-ttu-id="65bc6-735">deviceGuardEnableSecureBootWithDMA</span><span class="sxs-lookup"><span data-stu-id="65bc6-735">deviceGuardEnableSecureBootWithDMA</span></span>|<span data-ttu-id="65bc6-736">Boolean</span><span class="sxs-lookup"><span data-stu-id="65bc6-736">Boolean</span></span>|<span data-ttu-id="65bc6-737">此属性将在5月2019中被弃用, 并将替换为属性 DeviceGuardSecureBootWithDMA。</span><span class="sxs-lookup"><span data-stu-id="65bc6-737">This property will be deprecated in May 2019 and will be replaced with property DeviceGuardSecureBootWithDMA.</span></span> <span data-ttu-id="65bc6-738">指定是否在下次重新启动时启用平台安全级别。</span><span class="sxs-lookup"><span data-stu-id="65bc6-738">Specifies whether Platform Security Level is enabled at next reboot.</span></span>|
|<span data-ttu-id="65bc6-739">deviceGuardSecureBootWithDMA</span><span class="sxs-lookup"><span data-stu-id="65bc6-739">deviceGuardSecureBootWithDMA</span></span>|[<span data-ttu-id="65bc6-740">secureBootWithDMAType</span><span class="sxs-lookup"><span data-stu-id="65bc6-740">secureBootWithDMAType</span></span>](../resources/intune-deviceconfig-securebootwithdmatype.md)|<span data-ttu-id="65bc6-741">指定是否在下次重新启动时启用平台安全级别。</span><span class="sxs-lookup"><span data-stu-id="65bc6-741">Specifies whether Platform Security Level is enabled at next reboot.</span></span> <span data-ttu-id="65bc6-742">可取值为：`notConfigured`、`withoutDMA`、`withDMA`。</span><span class="sxs-lookup"><span data-stu-id="65bc6-742">Possible values are: `notConfigured`, `withoutDMA`, `withDMA`.</span></span>|
|<span data-ttu-id="65bc6-743">deviceGuardLaunchSystemGuard</span><span class="sxs-lookup"><span data-stu-id="65bc6-743">deviceGuardLaunchSystemGuard</span></span>|[<span data-ttu-id="65bc6-744">启用</span><span class="sxs-lookup"><span data-stu-id="65bc6-744">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="65bc6-745">允许 IT 管理员配置启动 "系统防护"。</span><span class="sxs-lookup"><span data-stu-id="65bc6-745">Allows the IT admin to configure the launch of System Guard.</span></span> <span data-ttu-id="65bc6-746">可取值为：`notConfigured`、`enabled`、`disabled`。</span><span class="sxs-lookup"><span data-stu-id="65bc6-746">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="65bc6-747">smartScreenEnableInShell</span><span class="sxs-lookup"><span data-stu-id="65bc6-747">smartScreenEnableInShell</span></span>|<span data-ttu-id="65bc6-748">Boolean</span><span class="sxs-lookup"><span data-stu-id="65bc6-748">Boolean</span></span>|<span data-ttu-id="65bc6-749">允许 IT 管理员配置适用于 Windows 的 SmartScreen。</span><span class="sxs-lookup"><span data-stu-id="65bc6-749">Allows IT Admins to configure SmartScreen for Windows.</span></span>|
|<span data-ttu-id="65bc6-750">smartScreenBlockOverrideForFiles</span><span class="sxs-lookup"><span data-stu-id="65bc6-750">smartScreenBlockOverrideForFiles</span></span>|<span data-ttu-id="65bc6-751">Boolean</span><span class="sxs-lookup"><span data-stu-id="65bc6-751">Boolean</span></span>|<span data-ttu-id="65bc6-752">允许 IT 管理员控制用户是否可以忽略 SmartScreen 警告并运行恶意文件。</span><span class="sxs-lookup"><span data-stu-id="65bc6-752">Allows IT Admins to control whether users can can ignore SmartScreen warnings and run malicious files.</span></span>|
|<span data-ttu-id="65bc6-753">applicationGuardEnabled</span><span class="sxs-lookup"><span data-stu-id="65bc6-753">applicationGuardEnabled</span></span>|<span data-ttu-id="65bc6-754">Boolean</span><span class="sxs-lookup"><span data-stu-id="65bc6-754">Boolean</span></span>|<span data-ttu-id="65bc6-755">启用 Windows Defender 应用程序防护</span><span class="sxs-lookup"><span data-stu-id="65bc6-755">Enable Windows Defender Application Guard</span></span>|
|<span data-ttu-id="65bc6-756">applicationGuardEnabledOptions</span><span class="sxs-lookup"><span data-stu-id="65bc6-756">applicationGuardEnabledOptions</span></span>|[<span data-ttu-id="65bc6-757">applicationGuardEnabledOptions</span><span class="sxs-lookup"><span data-stu-id="65bc6-757">applicationGuardEnabledOptions</span></span>](../resources/intune-deviceconfig-applicationguardenabledoptions.md)|<span data-ttu-id="65bc6-758">为较新的 Windows 版本启用 Windows Defender 应用程序防护。</span><span class="sxs-lookup"><span data-stu-id="65bc6-758">Enable Windows Defender Application Guard for newer Windows builds.</span></span> <span data-ttu-id="65bc6-759">可取值为：`notConfigured`、`enabledForEdge`、`enabledForOffice`、`enabledForEdgeAndOffice`。</span><span class="sxs-lookup"><span data-stu-id="65bc6-759">Possible values are: `notConfigured`, `enabledForEdge`, `enabledForOffice`, `enabledForEdgeAndOffice`.</span></span>|
|<span data-ttu-id="65bc6-760">applicationGuardBlockFileTransfer</span><span class="sxs-lookup"><span data-stu-id="65bc6-760">applicationGuardBlockFileTransfer</span></span>|[<span data-ttu-id="65bc6-761">applicationGuardBlockFileTransferType</span><span class="sxs-lookup"><span data-stu-id="65bc6-761">applicationGuardBlockFileTransferType</span></span>](../resources/intune-deviceconfig-applicationguardblockfiletransfertype.md)|<span data-ttu-id="65bc6-762">阻止剪贴板传输图像文件、文本文件或二者都不。</span><span class="sxs-lookup"><span data-stu-id="65bc6-762">Block clipboard to transfer image file, text file or neither of them.</span></span> <span data-ttu-id="65bc6-763">可取值为：`notConfigured`、`blockImageAndTextFile`、`blockImageFile`、`blockNone`、`blockTextFile`。</span><span class="sxs-lookup"><span data-stu-id="65bc6-763">Possible values are: `notConfigured`, `blockImageAndTextFile`, `blockImageFile`, `blockNone`, `blockTextFile`.</span></span>|
|<span data-ttu-id="65bc6-764">applicationGuardBlockNonEnterpriseContent</span><span class="sxs-lookup"><span data-stu-id="65bc6-764">applicationGuardBlockNonEnterpriseContent</span></span>|<span data-ttu-id="65bc6-765">Boolean</span><span class="sxs-lookup"><span data-stu-id="65bc6-765">Boolean</span></span>|<span data-ttu-id="65bc6-766">阻止企业站点加载非企业内容，例如第三方插件</span><span class="sxs-lookup"><span data-stu-id="65bc6-766">Block enterprise sites to load non-enterprise content, such as third party plug-ins</span></span>|
|<span data-ttu-id="65bc6-767">applicationGuardAllowPersistence</span><span class="sxs-lookup"><span data-stu-id="65bc6-767">applicationGuardAllowPersistence</span></span>|<span data-ttu-id="65bc6-768">Boolean</span><span class="sxs-lookup"><span data-stu-id="65bc6-768">Boolean</span></span>|<span data-ttu-id="65bc6-769">允许 App Guard 容器（收藏夹、Cookie、Web 密码等）内的持久用户生成数据</span><span class="sxs-lookup"><span data-stu-id="65bc6-769">Allow persisting user generated data inside the App Guard Containter (favorites, cookies, web passwords, etc.)</span></span>|
|<span data-ttu-id="65bc6-770">applicationGuardForceAuditing</span><span class="sxs-lookup"><span data-stu-id="65bc6-770">applicationGuardForceAuditing</span></span>|<span data-ttu-id="65bc6-771">Boolean</span><span class="sxs-lookup"><span data-stu-id="65bc6-771">Boolean</span></span>|<span data-ttu-id="65bc6-772">强制审核将存留 Windows 日志和事件以满足安全/符合性条件（示例事件是用户登录注销、特权使用、软件安装、系统更改等）</span><span class="sxs-lookup"><span data-stu-id="65bc6-772">Force auditing will persist Windows logs and events to meet security/compliance criteria (sample events are user login-logoff, use of privilege rights, software installation, system changes, etc.)</span></span>|
|<span data-ttu-id="65bc6-773">applicationGuardBlockClipboardSharing</span><span class="sxs-lookup"><span data-stu-id="65bc6-773">applicationGuardBlockClipboardSharing</span></span>|[<span data-ttu-id="65bc6-774">applicationGuardBlockClipboardSharingType</span><span class="sxs-lookup"><span data-stu-id="65bc6-774">applicationGuardBlockClipboardSharingType</span></span>](../resources/intune-deviceconfig-applicationguardblockclipboardsharingtype.md)|<span data-ttu-id="65bc6-775">阻止剪贴板将数据从主机共享到容器或从容器共享到主机，或阻止两种方式，或两种方式均不阻止。</span><span class="sxs-lookup"><span data-stu-id="65bc6-775">Block clipboard to share data from Host to Container, or from Container to Host, or both ways, or neither ways.</span></span> <span data-ttu-id="65bc6-776">可取值为：`notConfigured`、`blockBoth`、`blockHostToContainer`、`blockContainerToHost`、`blockNone`。</span><span class="sxs-lookup"><span data-stu-id="65bc6-776">Possible values are: `notConfigured`, `blockBoth`, `blockHostToContainer`, `blockContainerToHost`, `blockNone`.</span></span>|
|<span data-ttu-id="65bc6-777">applicationGuardAllowPrintToPDF</span><span class="sxs-lookup"><span data-stu-id="65bc6-777">applicationGuardAllowPrintToPDF</span></span>|<span data-ttu-id="65bc6-778">Boolean</span><span class="sxs-lookup"><span data-stu-id="65bc6-778">Boolean</span></span>|<span data-ttu-id="65bc6-779">允许从容器打印为 PDF 格式</span><span class="sxs-lookup"><span data-stu-id="65bc6-779">Allow printing to PDF from Container</span></span>|
|<span data-ttu-id="65bc6-780">applicationGuardAllowPrintToXPS</span><span class="sxs-lookup"><span data-stu-id="65bc6-780">applicationGuardAllowPrintToXPS</span></span>|<span data-ttu-id="65bc6-781">Boolean</span><span class="sxs-lookup"><span data-stu-id="65bc6-781">Boolean</span></span>|<span data-ttu-id="65bc6-782">允许从容器打印为 XPS 格式</span><span class="sxs-lookup"><span data-stu-id="65bc6-782">Allow printing to XPS from Container</span></span>|
|<span data-ttu-id="65bc6-783">applicationGuardAllowPrintToLocalPrinters</span><span class="sxs-lookup"><span data-stu-id="65bc6-783">applicationGuardAllowPrintToLocalPrinters</span></span>|<span data-ttu-id="65bc6-784">Boolean</span><span class="sxs-lookup"><span data-stu-id="65bc6-784">Boolean</span></span>|<span data-ttu-id="65bc6-785">允许从容器打印到本地打印机</span><span class="sxs-lookup"><span data-stu-id="65bc6-785">Allow printing to Local Printers from Container</span></span>|
|<span data-ttu-id="65bc6-786">applicationGuardAllowPrintToNetworkPrinters</span><span class="sxs-lookup"><span data-stu-id="65bc6-786">applicationGuardAllowPrintToNetworkPrinters</span></span>|<span data-ttu-id="65bc6-787">Boolean</span><span class="sxs-lookup"><span data-stu-id="65bc6-787">Boolean</span></span>|<span data-ttu-id="65bc6-788">允许从容器打印到网络打印机</span><span class="sxs-lookup"><span data-stu-id="65bc6-788">Allow printing to Network Printers from Container</span></span>|
|<span data-ttu-id="65bc6-789">applicationGuardAllowVirtualGPU</span><span class="sxs-lookup"><span data-stu-id="65bc6-789">applicationGuardAllowVirtualGPU</span></span>|<span data-ttu-id="65bc6-790">Boolean</span><span class="sxs-lookup"><span data-stu-id="65bc6-790">Boolean</span></span>|<span data-ttu-id="65bc6-791">允许应用程序防护使用虚拟 GPU</span><span class="sxs-lookup"><span data-stu-id="65bc6-791">Allow application guard to use virtual GPU</span></span>|
|<span data-ttu-id="65bc6-792">applicationGuardAllowFileSaveOnHost</span><span class="sxs-lookup"><span data-stu-id="65bc6-792">applicationGuardAllowFileSaveOnHost</span></span>|<span data-ttu-id="65bc6-793">Boolean</span><span class="sxs-lookup"><span data-stu-id="65bc6-793">Boolean</span></span>|<span data-ttu-id="65bc6-794">允许用户从应用程序防护容器中的边缘下载文件并将其保存在主机文件系统上</span><span class="sxs-lookup"><span data-stu-id="65bc6-794">Allow users to download files from Edge in the application guard container and save them on the host file system</span></span>|
|<span data-ttu-id="65bc6-795">bitLockerAllowStandardUserEncryption</span><span class="sxs-lookup"><span data-stu-id="65bc6-795">bitLockerAllowStandardUserEncryption</span></span>|<span data-ttu-id="65bc6-796">Boolean</span><span class="sxs-lookup"><span data-stu-id="65bc6-796">Boolean</span></span>|<span data-ttu-id="65bc6-797">允许管理员允许标准用户在 Azure AD 加入过程中启用 encrpytion。</span><span class="sxs-lookup"><span data-stu-id="65bc6-797">Allows the admin to allow standard users to enable encrpytion during Azure AD Join.</span></span>|
|<span data-ttu-id="65bc6-798">bitLockerDisableWarningForOtherDiskEncryption</span><span class="sxs-lookup"><span data-stu-id="65bc6-798">bitLockerDisableWarningForOtherDiskEncryption</span></span>|<span data-ttu-id="65bc6-799">Boolean</span><span class="sxs-lookup"><span data-stu-id="65bc6-799">Boolean</span></span>|<span data-ttu-id="65bc6-800">允许管理员禁用对用户计算机上其他磁盘加密的警告提示。</span><span class="sxs-lookup"><span data-stu-id="65bc6-800">Allows the Admin to disable the warning prompt for other disk encryption on the user machines.</span></span>|
|<span data-ttu-id="65bc6-801">bitLockerEnableStorageCardEncryptionOnMobile</span><span class="sxs-lookup"><span data-stu-id="65bc6-801">bitLockerEnableStorageCardEncryptionOnMobile</span></span>|<span data-ttu-id="65bc6-802">Boolean</span><span class="sxs-lookup"><span data-stu-id="65bc6-802">Boolean</span></span>|<span data-ttu-id="65bc6-803">允许管理员要求使用 BitLocker 开启加密功能。</span><span class="sxs-lookup"><span data-stu-id="65bc6-803">Allows the admin to require encryption to be turned on using BitLocker.</span></span> <span data-ttu-id="65bc6-804">此策略仅适用于移动 SKU。</span><span class="sxs-lookup"><span data-stu-id="65bc6-804">This policy is valid only for a mobile SKU.</span></span>|
|<span data-ttu-id="65bc6-805">bitLockerEncryptDevice</span><span class="sxs-lookup"><span data-stu-id="65bc6-805">bitLockerEncryptDevice</span></span>|<span data-ttu-id="65bc6-806">Boolean</span><span class="sxs-lookup"><span data-stu-id="65bc6-806">Boolean</span></span>|<span data-ttu-id="65bc6-807">允许管理员要求使用 BitLocker 开启加密功能。</span><span class="sxs-lookup"><span data-stu-id="65bc6-807">Allows the admin to require encryption to be turned on using BitLocker.</span></span>|
|<span data-ttu-id="65bc6-808">bitLockerSystemDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="65bc6-808">bitLockerSystemDrivePolicy</span></span>|[<span data-ttu-id="65bc6-809">bitLockerSystemDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="65bc6-809">bitLockerSystemDrivePolicy</span></span>](../resources/intune-deviceconfig-bitlockersystemdrivepolicy.md)|<span data-ttu-id="65bc6-810">BitLocker 系统驱动器策略。</span><span class="sxs-lookup"><span data-stu-id="65bc6-810">BitLocker System Drive Policy.</span></span>|
|<span data-ttu-id="65bc6-811">bitLockerFixedDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="65bc6-811">bitLockerFixedDrivePolicy</span></span>|[<span data-ttu-id="65bc6-812">bitLockerFixedDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="65bc6-812">bitLockerFixedDrivePolicy</span></span>](../resources/intune-deviceconfig-bitlockerfixeddrivepolicy.md)|<span data-ttu-id="65bc6-813">BitLocker 固定驱动器策略。</span><span class="sxs-lookup"><span data-stu-id="65bc6-813">BitLocker Fixed Drive Policy.</span></span>|
|<span data-ttu-id="65bc6-814">bitLockerRemovableDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="65bc6-814">bitLockerRemovableDrivePolicy</span></span>|[<span data-ttu-id="65bc6-815">bitLockerRemovableDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="65bc6-815">bitLockerRemovableDrivePolicy</span></span>](../resources/intune-deviceconfig-bitlockerremovabledrivepolicy.md)|<span data-ttu-id="65bc6-816">BitLocker 可移动驱动器策略。</span><span class="sxs-lookup"><span data-stu-id="65bc6-816">BitLocker Removable Drive Policy.</span></span>|



## <a name="response"></a><span data-ttu-id="65bc6-817">响应</span><span class="sxs-lookup"><span data-stu-id="65bc6-817">Response</span></span>
<span data-ttu-id="65bc6-818">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="65bc6-818">If successful, this method returns a `201 Created` response code and a [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="65bc6-819">示例</span><span class="sxs-lookup"><span data-stu-id="65bc6-819">Example</span></span>

### <a name="request"></a><span data-ttu-id="65bc6-820">请求</span><span class="sxs-lookup"><span data-stu-id="65bc6-820">Request</span></span>
<span data-ttu-id="65bc6-821">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="65bc6-821">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 28463

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
  "userRightsRegisterProcessAsService": {
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
  }
}
```

### <a name="response"></a><span data-ttu-id="65bc6-822">响应</span><span class="sxs-lookup"><span data-stu-id="65bc6-822">Response</span></span>
<span data-ttu-id="65bc6-p204">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="65bc6-p204">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 28635

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
  "userRightsRegisterProcessAsService": {
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
  }
}
```





