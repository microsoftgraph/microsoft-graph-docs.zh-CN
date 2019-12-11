---
title: 创建 windows10EndpointProtectionConfiguration
description: 创建新的 windows10EndpointProtectionConfiguration 对象。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 5330720aac87f6a538b01b756ad0ce927e610a36
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/10/2019
ms.locfileid: "39947517"
---
# <a name="create-windows10endpointprotectionconfiguration"></a><span data-ttu-id="4db07-103">创建 windows10EndpointProtectionConfiguration</span><span class="sxs-lookup"><span data-stu-id="4db07-103">Create windows10EndpointProtectionConfiguration</span></span>

> <span data-ttu-id="4db07-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="4db07-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4db07-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="4db07-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4db07-106">创建新的 [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="4db07-106">Create a new [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4db07-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="4db07-107">Prerequisites</span></span>
<span data-ttu-id="4db07-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4db07-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4db07-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="4db07-110">Permission type</span></span>|<span data-ttu-id="4db07-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="4db07-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4db07-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4db07-112">Delegated (work or school account)</span></span>|<span data-ttu-id="4db07-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4db07-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="4db07-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4db07-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4db07-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="4db07-115">Not supported.</span></span>|
|<span data-ttu-id="4db07-116">Application</span><span class="sxs-lookup"><span data-stu-id="4db07-116">Application</span></span>|<span data-ttu-id="4db07-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4db07-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4db07-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4db07-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="4db07-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="4db07-119">Request headers</span></span>
|<span data-ttu-id="4db07-120">标头</span><span class="sxs-lookup"><span data-stu-id="4db07-120">Header</span></span>|<span data-ttu-id="4db07-121">值</span><span class="sxs-lookup"><span data-stu-id="4db07-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4db07-122">授权</span><span class="sxs-lookup"><span data-stu-id="4db07-122">Authorization</span></span>|<span data-ttu-id="4db07-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="4db07-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4db07-124">接受</span><span class="sxs-lookup"><span data-stu-id="4db07-124">Accept</span></span>|<span data-ttu-id="4db07-125">application/json</span><span class="sxs-lookup"><span data-stu-id="4db07-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4db07-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="4db07-126">Request body</span></span>
<span data-ttu-id="4db07-127">在请求正文中，提供 windows10EndpointProtectionConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4db07-127">In the request body, supply a JSON representation for the windows10EndpointProtectionConfiguration object.</span></span>

<span data-ttu-id="4db07-128">下表显示了创建 windows10EndpointProtectionConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="4db07-128">The following table shows the properties that are required when you create the windows10EndpointProtectionConfiguration.</span></span>

|<span data-ttu-id="4db07-129">属性</span><span class="sxs-lookup"><span data-stu-id="4db07-129">Property</span></span>|<span data-ttu-id="4db07-130">类型</span><span class="sxs-lookup"><span data-stu-id="4db07-130">Type</span></span>|<span data-ttu-id="4db07-131">说明</span><span class="sxs-lookup"><span data-stu-id="4db07-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4db07-132">id</span><span class="sxs-lookup"><span data-stu-id="4db07-132">id</span></span>|<span data-ttu-id="4db07-133">字符串</span><span class="sxs-lookup"><span data-stu-id="4db07-133">String</span></span>|<span data-ttu-id="4db07-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="4db07-134">Key of the entity.</span></span> <span data-ttu-id="4db07-135">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4db07-135">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4db07-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4db07-136">lastModifiedDateTime</span></span>|<span data-ttu-id="4db07-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4db07-137">DateTimeOffset</span></span>|<span data-ttu-id="4db07-138">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="4db07-138">DateTime the object was last modified.</span></span> <span data-ttu-id="4db07-139">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4db07-139">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4db07-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="4db07-140">roleScopeTagIds</span></span>|<span data-ttu-id="4db07-141">String collection</span><span class="sxs-lookup"><span data-stu-id="4db07-141">String collection</span></span>|<span data-ttu-id="4db07-142">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="4db07-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="4db07-143">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4db07-143">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4db07-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="4db07-144">supportsScopeTags</span></span>|<span data-ttu-id="4db07-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="4db07-145">Boolean</span></span>|<span data-ttu-id="4db07-146">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="4db07-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="4db07-147">如果此值为 false，则不允许分配给 ScopeTags 属性，并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="4db07-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="4db07-148">这适用于在 Silverlight 中创建的旧版策略，可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="4db07-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="4db07-149">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="4db07-149">This property is read-only.</span></span> <span data-ttu-id="4db07-150">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4db07-150">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4db07-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="4db07-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="4db07-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="4db07-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="4db07-153">适用于此策略的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="4db07-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="4db07-154">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4db07-154">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4db07-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="4db07-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="4db07-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="4db07-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="4db07-157">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="4db07-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="4db07-158">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4db07-158">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4db07-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="4db07-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="4db07-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="4db07-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="4db07-161">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="4db07-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="4db07-162">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4db07-162">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4db07-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="4db07-163">createdDateTime</span></span>|<span data-ttu-id="4db07-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4db07-164">DateTimeOffset</span></span>|<span data-ttu-id="4db07-165">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="4db07-165">DateTime the object was created.</span></span> <span data-ttu-id="4db07-166">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4db07-166">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4db07-167">说明</span><span class="sxs-lookup"><span data-stu-id="4db07-167">description</span></span>|<span data-ttu-id="4db07-168">String</span><span class="sxs-lookup"><span data-stu-id="4db07-168">String</span></span>|<span data-ttu-id="4db07-169">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="4db07-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="4db07-170">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4db07-170">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4db07-171">displayName</span><span class="sxs-lookup"><span data-stu-id="4db07-171">displayName</span></span>|<span data-ttu-id="4db07-172">String</span><span class="sxs-lookup"><span data-stu-id="4db07-172">String</span></span>|<span data-ttu-id="4db07-173">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="4db07-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="4db07-174">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4db07-174">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4db07-175">version</span><span class="sxs-lookup"><span data-stu-id="4db07-175">version</span></span>|<span data-ttu-id="4db07-176">Int32</span><span class="sxs-lookup"><span data-stu-id="4db07-176">Int32</span></span>|<span data-ttu-id="4db07-177">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="4db07-177">Version of the device configuration.</span></span> <span data-ttu-id="4db07-178">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4db07-178">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4db07-179">dmaGuardDeviceEnumerationPolicy</span><span class="sxs-lookup"><span data-stu-id="4db07-179">dmaGuardDeviceEnumerationPolicy</span></span>|[<span data-ttu-id="4db07-180">dmaGuardDeviceEnumerationPolicyType</span><span class="sxs-lookup"><span data-stu-id="4db07-180">dmaGuardDeviceEnumerationPolicyType</span></span>](../resources/intune-deviceconfig-dmaguarddeviceenumerationpolicytype.md)|<span data-ttu-id="4db07-181">此策略旨在提供针对支持外部 DMA 的设备的额外安全性。</span><span class="sxs-lookup"><span data-stu-id="4db07-181">This policy is intended to provide additional security against external DMA capable devices.</span></span> <span data-ttu-id="4db07-182">通过它，可以更好地控制支持外部 DMA 的设备与 DMA 重新映射/设备内存隔离和沙盒不兼容的枚举。</span><span class="sxs-lookup"><span data-stu-id="4db07-182">It allows for more control over the enumeration of external DMA capable devices incompatible with DMA Remapping/device memory isolation and sandboxing.</span></span> <span data-ttu-id="4db07-183">仅当系统固件支持和启用内核 DMA 保护时，此策略才会生效。</span><span class="sxs-lookup"><span data-stu-id="4db07-183">This policy only takes effect when Kernel DMA Protection is supported and enabled by the system firmware.</span></span> <span data-ttu-id="4db07-184">内核 DMA 保护是一项平台功能，不能通过策略或最终用户进行控制。</span><span class="sxs-lookup"><span data-stu-id="4db07-184">Kernel DMA Protection is a platform feature that cannot be controlled via policy or by end user.</span></span> <span data-ttu-id="4db07-185">在制造时，系统必须支持它。</span><span class="sxs-lookup"><span data-stu-id="4db07-185">It has to be supported by the system at the time of manufacturing.</span></span> <span data-ttu-id="4db07-186">若要检查系统是否支持内核 DMA 保护，请在 MSINFO32 的摘要页中检查 "内核 DMA 保护" 字段。</span><span class="sxs-lookup"><span data-stu-id="4db07-186">To check if the system supports Kernel DMA Protection, please check the Kernel DMA Protection field in the Summary page of MSINFO32.exe.</span></span> <span data-ttu-id="4db07-187">可取值为：`deviceDefault`、`blockAll`、`allowAll`。</span><span class="sxs-lookup"><span data-stu-id="4db07-187">Possible values are: `deviceDefault`, `blockAll`, `allowAll`.</span></span>|
|<span data-ttu-id="4db07-188">firewallRules</span><span class="sxs-lookup"><span data-stu-id="4db07-188">firewallRules</span></span>|<span data-ttu-id="4db07-189">[windowsFirewallRule](../resources/intune-deviceconfig-windowsfirewallrule.md)集合</span><span class="sxs-lookup"><span data-stu-id="4db07-189">[windowsFirewallRule](../resources/intune-deviceconfig-windowsfirewallrule.md) collection</span></span>|<span data-ttu-id="4db07-190">配置防火墙规则设置。</span><span class="sxs-lookup"><span data-stu-id="4db07-190">Configures the firewall rule settings.</span></span> <span data-ttu-id="4db07-191">此集合最多可包含150个元素。</span><span class="sxs-lookup"><span data-stu-id="4db07-191">This collection can contain a maximum of 150 elements.</span></span>|
|<span data-ttu-id="4db07-192">userRightsAccessCredentialManagerAsTrustedCaller</span><span class="sxs-lookup"><span data-stu-id="4db07-192">userRightsAccessCredentialManagerAsTrustedCaller</span></span>|[<span data-ttu-id="4db07-193">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="4db07-193">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="4db07-194">此用户权限由凭据管理器在备份/还原过程中使用。</span><span class="sxs-lookup"><span data-stu-id="4db07-194">This user right is used by Credential Manager during Backup/Restore.</span></span> <span data-ttu-id="4db07-195">如果为其他实体提供此权限，则用户保存的凭据可能会受到威胁。</span><span class="sxs-lookup"><span data-stu-id="4db07-195">Users' saved credentials might be compromised if this privilege is given to other entities.</span></span> <span data-ttu-id="4db07-196">仅支持 NotConfigured 和允许的状态</span><span class="sxs-lookup"><span data-stu-id="4db07-196">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="4db07-197">userRightsAllowAccessFromNetwork</span><span class="sxs-lookup"><span data-stu-id="4db07-197">userRightsAllowAccessFromNetwork</span></span>|[<span data-ttu-id="4db07-198">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="4db07-198">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="4db07-199">此用户权限确定允许哪些用户和组通过网络连接到计算机。</span><span class="sxs-lookup"><span data-stu-id="4db07-199">This user right determines which users and groups are allowed to connect to the computer over the network.</span></span> <span data-ttu-id="4db07-200">支持的状态为 "允许"。</span><span class="sxs-lookup"><span data-stu-id="4db07-200">State Allowed is supported.</span></span>|
|<span data-ttu-id="4db07-201">userRightsBlockAccessFromNetwork</span><span class="sxs-lookup"><span data-stu-id="4db07-201">userRightsBlockAccessFromNetwork</span></span>|[<span data-ttu-id="4db07-202">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="4db07-202">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="4db07-203">此用户权限决定了阻止哪些用户和组通过网络连接到计算机。</span><span class="sxs-lookup"><span data-stu-id="4db07-203">This user right determines which users and groups are block from connecting to the computer over the network.</span></span> <span data-ttu-id="4db07-204">支持状态块。</span><span class="sxs-lookup"><span data-stu-id="4db07-204">State Block is supported.</span></span>|
|<span data-ttu-id="4db07-205">userRightsActAsPartOfTheOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="4db07-205">userRightsActAsPartOfTheOperatingSystem</span></span>|[<span data-ttu-id="4db07-206">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="4db07-206">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="4db07-207">此用户权限允许进程在不进行身份验证的情况下模拟任何用户。</span><span class="sxs-lookup"><span data-stu-id="4db07-207">This user right allows a process to impersonate any user without authentication.</span></span> <span data-ttu-id="4db07-208">因此，该过程可以获得与该用户相同的本地资源的访问权限。</span><span class="sxs-lookup"><span data-stu-id="4db07-208">The process can therefore gain access to the same local resources as that user.</span></span> <span data-ttu-id="4db07-209">仅支持 NotConfigured 和允许的状态</span><span class="sxs-lookup"><span data-stu-id="4db07-209">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="4db07-210">userRightsLocalLogOn</span><span class="sxs-lookup"><span data-stu-id="4db07-210">userRightsLocalLogOn</span></span>|[<span data-ttu-id="4db07-211">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="4db07-211">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="4db07-212">此用户权限确定哪些用户可以登录到计算机。</span><span class="sxs-lookup"><span data-stu-id="4db07-212">This user right determines which users can log on to the computer.</span></span> <span data-ttu-id="4db07-213">支持的状态 NotConfigured （允许）</span><span class="sxs-lookup"><span data-stu-id="4db07-213">States NotConfigured, Allowed are supported</span></span> |
|<span data-ttu-id="4db07-214">userRightsDenyLocalLogOn</span><span class="sxs-lookup"><span data-stu-id="4db07-214">userRightsDenyLocalLogOn</span></span>|[<span data-ttu-id="4db07-215">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="4db07-215">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="4db07-216">此用户权限确定哪些用户无法登录到计算机。</span><span class="sxs-lookup"><span data-stu-id="4db07-216">This user right determines which users cannot log on to the computer.</span></span> <span data-ttu-id="4db07-217">状态 NotConfigured，受阻止</span><span class="sxs-lookup"><span data-stu-id="4db07-217">States NotConfigured, Blocked are supported</span></span> |
|<span data-ttu-id="4db07-218">userRightsBackupData</span><span class="sxs-lookup"><span data-stu-id="4db07-218">userRightsBackupData</span></span>|[<span data-ttu-id="4db07-219">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="4db07-219">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="4db07-220">此用户权限确定在备份文件和目录时，哪些用户可以绕过文件、目录、注册表和其他持久对象权限。</span><span class="sxs-lookup"><span data-stu-id="4db07-220">This user right determines which users can bypass file, directory, registry, and other persistent objects permissions when backing up files and directories.</span></span> <span data-ttu-id="4db07-221">仅支持 NotConfigured 和允许的状态</span><span class="sxs-lookup"><span data-stu-id="4db07-221">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="4db07-222">userRightsChangeSystemTime</span><span class="sxs-lookup"><span data-stu-id="4db07-222">userRightsChangeSystemTime</span></span>|[<span data-ttu-id="4db07-223">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="4db07-223">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="4db07-224">此用户权限确定哪些用户和组可以更改计算机内部时钟上的时间和日期。</span><span class="sxs-lookup"><span data-stu-id="4db07-224">This user right determines which users and groups can change the time and date on the internal clock of the computer.</span></span> <span data-ttu-id="4db07-225">仅支持 NotConfigured 和允许的状态</span><span class="sxs-lookup"><span data-stu-id="4db07-225">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="4db07-226">userRightsCreateGlobalObjects</span><span class="sxs-lookup"><span data-stu-id="4db07-226">userRightsCreateGlobalObjects</span></span>|[<span data-ttu-id="4db07-227">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="4db07-227">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="4db07-228">此安全设置确定用户是否可以创建可用于所有会话的全局对象。</span><span class="sxs-lookup"><span data-stu-id="4db07-228">This security setting determines whether users can create global objects that are available to all sessions.</span></span> <span data-ttu-id="4db07-229">可以创建全局对象的用户可能会影响在其他用户的会话下运行的进程，这可能导致应用程序故障或数据损坏。</span><span class="sxs-lookup"><span data-stu-id="4db07-229">Users who can create global objects could affect processes that run under other users' sessions, which could lead to application failure or data corruption.</span></span> <span data-ttu-id="4db07-230">仅支持 NotConfigured 和允许的状态</span><span class="sxs-lookup"><span data-stu-id="4db07-230">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="4db07-231">userRightsCreatePageFile</span><span class="sxs-lookup"><span data-stu-id="4db07-231">userRightsCreatePageFile</span></span>|[<span data-ttu-id="4db07-232">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="4db07-232">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="4db07-233">此用户权限确定哪些用户和组可以调用内部 API 来创建和更改页面文件的大小。</span><span class="sxs-lookup"><span data-stu-id="4db07-233">This user right determines which users and groups can call an internal API to create and change the size of a page file.</span></span> <span data-ttu-id="4db07-234">仅支持 NotConfigured 和允许的状态</span><span class="sxs-lookup"><span data-stu-id="4db07-234">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="4db07-235">userRightsCreatePermanentSharedObjects</span><span class="sxs-lookup"><span data-stu-id="4db07-235">userRightsCreatePermanentSharedObjects</span></span>|[<span data-ttu-id="4db07-236">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="4db07-236">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="4db07-237">此用户权限决定了进程可以使用哪些帐户使用对象管理器创建目录对象。</span><span class="sxs-lookup"><span data-stu-id="4db07-237">This user right determines which accounts can be used by processes to create a directory object using the object manager.</span></span> <span data-ttu-id="4db07-238">仅支持 NotConfigured 和允许的状态</span><span class="sxs-lookup"><span data-stu-id="4db07-238">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="4db07-239">userRightsCreateSymbolicLinks</span><span class="sxs-lookup"><span data-stu-id="4db07-239">userRightsCreateSymbolicLinks</span></span>|[<span data-ttu-id="4db07-240">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="4db07-240">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="4db07-241">此用户权限确定用户是否可以从其登录到的计算机创建符号链接。</span><span class="sxs-lookup"><span data-stu-id="4db07-241">This user right determines if the user can create a symbolic link from the computer to which they are logged on.</span></span> <span data-ttu-id="4db07-242">仅支持 NotConfigured 和允许的状态</span><span class="sxs-lookup"><span data-stu-id="4db07-242">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="4db07-243">userRightsCreateToken</span><span class="sxs-lookup"><span data-stu-id="4db07-243">userRightsCreateToken</span></span>|[<span data-ttu-id="4db07-244">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="4db07-244">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="4db07-245">此用户权限确定进程在使用内部 API 创建访问令牌时，可以使用哪些用户/组来创建令牌，然后可以使用这些用户/组来获取对任何本地资源的访问权限。</span><span class="sxs-lookup"><span data-stu-id="4db07-245">This user right determines which users/groups can be used by processes to create a token that can then be used to get access to any local resources when the process uses an internal API to create an access token.</span></span> <span data-ttu-id="4db07-246">仅支持 NotConfigured 和允许的状态</span><span class="sxs-lookup"><span data-stu-id="4db07-246">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="4db07-247">userRightsDebugPrograms</span><span class="sxs-lookup"><span data-stu-id="4db07-247">userRightsDebugPrograms</span></span>|[<span data-ttu-id="4db07-248">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="4db07-248">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="4db07-249">此用户权限确定哪些用户可以将调试程序附加到任何进程或内核。</span><span class="sxs-lookup"><span data-stu-id="4db07-249">This user right determines which users can attach a debugger to any process or to the kernel.</span></span> <span data-ttu-id="4db07-250">仅支持 NotConfigured 和允许的状态</span><span class="sxs-lookup"><span data-stu-id="4db07-250">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="4db07-251">userRightsRemoteDesktopServicesLogOn</span><span class="sxs-lookup"><span data-stu-id="4db07-251">userRightsRemoteDesktopServicesLogOn</span></span>|[<span data-ttu-id="4db07-252">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="4db07-252">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="4db07-253">此用户权限确定禁止哪些用户和组作为远程桌面服务客户端进行登录。</span><span class="sxs-lookup"><span data-stu-id="4db07-253">This user right determines which users and groups are prohibited from logging on as a Remote Desktop Services client.</span></span> <span data-ttu-id="4db07-254">仅支持状态 NotConfigured 和阻止</span><span class="sxs-lookup"><span data-stu-id="4db07-254">Only states NotConfigured and Blocked are supported</span></span>|
|<span data-ttu-id="4db07-255">userRightsDelegation</span><span class="sxs-lookup"><span data-stu-id="4db07-255">userRightsDelegation</span></span>|[<span data-ttu-id="4db07-256">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="4db07-256">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="4db07-257">此用户权限确定哪些用户可以在用户或计算机对象上设置受信任委派设置。</span><span class="sxs-lookup"><span data-stu-id="4db07-257">This user right determines which users can set the Trusted for Delegation setting on a user or computer object.</span></span> <span data-ttu-id="4db07-258">仅支持 NotConfigured 和允许的状态。</span><span class="sxs-lookup"><span data-stu-id="4db07-258">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="4db07-259">userRightsGenerateSecurityAudits</span><span class="sxs-lookup"><span data-stu-id="4db07-259">userRightsGenerateSecurityAudits</span></span>|[<span data-ttu-id="4db07-260">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="4db07-260">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="4db07-261">此用户权限确定进程可使用哪些帐户向安全日志中添加条目。</span><span class="sxs-lookup"><span data-stu-id="4db07-261">This user right determines which accounts can be used by a process to add entries to the security log.</span></span> <span data-ttu-id="4db07-262">安全日志用于跟踪未经授权的系统访问。</span><span class="sxs-lookup"><span data-stu-id="4db07-262">The security log is used to trace unauthorized system access.</span></span>  <span data-ttu-id="4db07-263">仅支持 NotConfigured 和允许的状态。</span><span class="sxs-lookup"><span data-stu-id="4db07-263">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="4db07-264">userRightsImpersonateClient</span><span class="sxs-lookup"><span data-stu-id="4db07-264">userRightsImpersonateClient</span></span>|[<span data-ttu-id="4db07-265">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="4db07-265">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="4db07-266">将此用户权限分配给用户将允许代表该用户运行的程序模拟客户端。</span><span class="sxs-lookup"><span data-stu-id="4db07-266">Assigning this user right to a user allows programs running on behalf of that user to impersonate a client.</span></span> <span data-ttu-id="4db07-267">如果此类型的模拟要求此用户权限，则可以防止未经授权的用户说服客户端连接到已创建的服务，然后模拟该客户端，这样可以将未经授权的用户的权限提升到管理级别或系统级别。</span><span class="sxs-lookup"><span data-stu-id="4db07-267">Requiring this user right for this kind of impersonation prevents an unauthorized user from convincing a client to connect to a service that they have created and then impersonating that client, which can elevate the unauthorized user's permissions to administrative or system levels.</span></span> <span data-ttu-id="4db07-268">仅支持 NotConfigured 和允许的状态。</span><span class="sxs-lookup"><span data-stu-id="4db07-268">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="4db07-269">userRightsIncreaseSchedulingPriority</span><span class="sxs-lookup"><span data-stu-id="4db07-269">userRightsIncreaseSchedulingPriority</span></span>|[<span data-ttu-id="4db07-270">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="4db07-270">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="4db07-271">此用户权限确定哪些帐户可以使用具有对另一进程的 Write 属性访问权限的进程，以增加分配给其他进程的执行优先级。</span><span class="sxs-lookup"><span data-stu-id="4db07-271">This user right determines which accounts can use a process with Write Property access to another process to increase the execution priority assigned to the other process.</span></span> <span data-ttu-id="4db07-272">仅支持 NotConfigured 和允许的状态。</span><span class="sxs-lookup"><span data-stu-id="4db07-272">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="4db07-273">userRightsLoadUnloadDrivers</span><span class="sxs-lookup"><span data-stu-id="4db07-273">userRightsLoadUnloadDrivers</span></span>|[<span data-ttu-id="4db07-274">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="4db07-274">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="4db07-275">此用户权限确定哪些用户可以在内核模式下将设备驱动程序或其他代码动态加载和卸载。</span><span class="sxs-lookup"><span data-stu-id="4db07-275">This user right determines which users can dynamically load and unload device drivers or other code in to kernel mode.</span></span> <span data-ttu-id="4db07-276">仅支持 NotConfigured 和允许的状态。</span><span class="sxs-lookup"><span data-stu-id="4db07-276">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="4db07-277">userRightsLockMemory</span><span class="sxs-lookup"><span data-stu-id="4db07-277">userRightsLockMemory</span></span>|[<span data-ttu-id="4db07-278">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="4db07-278">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="4db07-279">此用户权限确定哪些帐户可以使用进程将数据保存在物理内存中，这会阻止系统将数据分页到磁盘上的虚拟内存中。</span><span class="sxs-lookup"><span data-stu-id="4db07-279">This user right determines which accounts can use a process to keep data in physical memory, which prevents the system from paging the data to virtual memory on disk.</span></span> <span data-ttu-id="4db07-280">仅支持 NotConfigured 和允许的状态。</span><span class="sxs-lookup"><span data-stu-id="4db07-280">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="4db07-281">userRightsManageAuditingAndSecurityLogs</span><span class="sxs-lookup"><span data-stu-id="4db07-281">userRightsManageAuditingAndSecurityLogs</span></span>|[<span data-ttu-id="4db07-282">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="4db07-282">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="4db07-283">此用户权限确定哪些用户可以为各个资源（如文件、Active Directory 对象和注册表项）指定对象访问审核选项。</span><span class="sxs-lookup"><span data-stu-id="4db07-283">This user right determines which users can specify object access auditing options for individual resources, such as files, Active Directory objects, and registry keys.</span></span> <span data-ttu-id="4db07-284">仅支持 NotConfigured 和允许的状态。</span><span class="sxs-lookup"><span data-stu-id="4db07-284">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="4db07-285">userRightsManageVolumes</span><span class="sxs-lookup"><span data-stu-id="4db07-285">userRightsManageVolumes</span></span>|[<span data-ttu-id="4db07-286">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="4db07-286">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="4db07-287">此用户权限确定哪些用户和组可以在某个卷（如远程碎片整理）上运行维护任务。</span><span class="sxs-lookup"><span data-stu-id="4db07-287">This user right determines which users and groups can run maintenance tasks on a volume, such as remote defragmentation.</span></span> <span data-ttu-id="4db07-288">仅支持 NotConfigured 和允许的状态。</span><span class="sxs-lookup"><span data-stu-id="4db07-288">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="4db07-289">userRightsModifyFirmwareEnvironment</span><span class="sxs-lookup"><span data-stu-id="4db07-289">userRightsModifyFirmwareEnvironment</span></span>|[<span data-ttu-id="4db07-290">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="4db07-290">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="4db07-291">此用户权限决定了可以修改固件环境值的用户。</span><span class="sxs-lookup"><span data-stu-id="4db07-291">This user right determines who can modify firmware environment values.</span></span> <span data-ttu-id="4db07-292">仅支持 NotConfigured 和允许的状态。</span><span class="sxs-lookup"><span data-stu-id="4db07-292">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="4db07-293">userRightsModifyObjectLabels</span><span class="sxs-lookup"><span data-stu-id="4db07-293">userRightsModifyObjectLabels</span></span>|[<span data-ttu-id="4db07-294">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="4db07-294">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="4db07-295">此用户权限确定哪些用户帐户可以修改对象的完整性标签，例如，文件、注册表项或其他用户所拥有的进程。</span><span class="sxs-lookup"><span data-stu-id="4db07-295">This user right determines which user accounts can modify the integrity label of objects, such as files, registry keys, or processes owned by other users.</span></span> <span data-ttu-id="4db07-296">仅支持 NotConfigured 和允许的状态。</span><span class="sxs-lookup"><span data-stu-id="4db07-296">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="4db07-297">userRightsProfileSingleProcess</span><span class="sxs-lookup"><span data-stu-id="4db07-297">userRightsProfileSingleProcess</span></span>|[<span data-ttu-id="4db07-298">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="4db07-298">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="4db07-299">此用户权限确定哪些用户可以使用性能监视工具来监视系统进程的性能。</span><span class="sxs-lookup"><span data-stu-id="4db07-299">This user right determines which users can use performance monitoring tools to monitor the performance of system processes.</span></span> <span data-ttu-id="4db07-300">仅支持 NotConfigured 和允许的状态。</span><span class="sxs-lookup"><span data-stu-id="4db07-300">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="4db07-301">userRightsRemoteShutdown</span><span class="sxs-lookup"><span data-stu-id="4db07-301">userRightsRemoteShutdown</span></span>|[<span data-ttu-id="4db07-302">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="4db07-302">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="4db07-303">此用户权限确定允许哪些用户从网络上的远程位置关闭计算机。</span><span class="sxs-lookup"><span data-stu-id="4db07-303">This user right determines which users are allowed to shut down a computer from a remote location on the network.</span></span> <span data-ttu-id="4db07-304">误用此用户权限可能会导致拒绝服务。</span><span class="sxs-lookup"><span data-stu-id="4db07-304">Misuse of this user right can result in a denial of service.</span></span> <span data-ttu-id="4db07-305">仅支持 NotConfigured 和允许的状态。</span><span class="sxs-lookup"><span data-stu-id="4db07-305">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="4db07-306">userRightsRestoreData</span><span class="sxs-lookup"><span data-stu-id="4db07-306">userRightsRestoreData</span></span>|[<span data-ttu-id="4db07-307">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="4db07-307">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="4db07-308">此用户权限确定在还原备份的文件和目录时，哪些用户可以绕过文件、目录、注册表和其他持久对象权限，并确定哪些用户可以将任何有效的安全主体设置为对象的所有者。</span><span class="sxs-lookup"><span data-stu-id="4db07-308">This user right determines which users can bypass file, directory, registry, and other persistent objects permissions when restoring backed up files and directories, and determines which users can set any valid security principal as the owner of an object.</span></span> <span data-ttu-id="4db07-309">仅支持 NotConfigured 和允许的状态。</span><span class="sxs-lookup"><span data-stu-id="4db07-309">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="4db07-310">userRightsTakeOwnership</span><span class="sxs-lookup"><span data-stu-id="4db07-310">userRightsTakeOwnership</span></span>|[<span data-ttu-id="4db07-311">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="4db07-311">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="4db07-312">此用户权限确定哪些用户可以获得系统中任何安全对象的所有权，包括 Active Directory 对象、文件和文件夹、打印机、注册表项、进程和线程。</span><span class="sxs-lookup"><span data-stu-id="4db07-312">This user right determines which users can take ownership of any securable object in the system, including Active Directory objects, files and folders, printers, registry keys, processes, and threads.</span></span> <span data-ttu-id="4db07-313">仅支持 NotConfigured 和允许的状态。</span><span class="sxs-lookup"><span data-stu-id="4db07-313">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="4db07-314">xboxServicesEnableXboxGameSaveTask</span><span class="sxs-lookup"><span data-stu-id="4db07-314">xboxServicesEnableXboxGameSaveTask</span></span>|<span data-ttu-id="4db07-315">Boolean</span><span class="sxs-lookup"><span data-stu-id="4db07-315">Boolean</span></span>|<span data-ttu-id="4db07-316">此设置确定是否启用了 xbox 游戏保存（1）或禁用（0）。</span><span class="sxs-lookup"><span data-stu-id="4db07-316">This setting determines whether xbox game save is enabled (1) or disabled (0).</span></span>|
|<span data-ttu-id="4db07-317">xboxServicesAccessoryManagementServiceStartupMode</span><span class="sxs-lookup"><span data-stu-id="4db07-317">xboxServicesAccessoryManagementServiceStartupMode</span></span>|[<span data-ttu-id="4db07-318">serviceStartType</span><span class="sxs-lookup"><span data-stu-id="4db07-318">serviceStartType</span></span>](../resources/intune-deviceconfig-servicestarttype.md)|<span data-ttu-id="4db07-319">此设置确定附件管理服务的启动类型是 "自动" （2）、"手动" （3）、"已禁用" （4）。</span><span class="sxs-lookup"><span data-stu-id="4db07-319">This setting determines whether the Accessory management service's start type is Automatic(2), Manual(3), Disabled(4).</span></span> <span data-ttu-id="4db07-320">默认：手动。</span><span class="sxs-lookup"><span data-stu-id="4db07-320">Default: Manual.</span></span> <span data-ttu-id="4db07-321">可取值为：`manual`、`automatic`、`disabled`。</span><span class="sxs-lookup"><span data-stu-id="4db07-321">Possible values are: `manual`, `automatic`, `disabled`.</span></span>|
|<span data-ttu-id="4db07-322">xboxServicesLiveAuthManagerServiceStartupMode</span><span class="sxs-lookup"><span data-stu-id="4db07-322">xboxServicesLiveAuthManagerServiceStartupMode</span></span>|[<span data-ttu-id="4db07-323">serviceStartType</span><span class="sxs-lookup"><span data-stu-id="4db07-323">serviceStartType</span></span>](../resources/intune-deviceconfig-servicestarttype.md)|<span data-ttu-id="4db07-324">此设置确定 Live Auth Manager 服务的启动类型是否为自动（2）、手动（3）、已禁用（4）。</span><span class="sxs-lookup"><span data-stu-id="4db07-324">This setting determines whether Live Auth Manager service's start type is Automatic(2), Manual(3), Disabled(4).</span></span> <span data-ttu-id="4db07-325">默认：手动。</span><span class="sxs-lookup"><span data-stu-id="4db07-325">Default: Manual.</span></span> <span data-ttu-id="4db07-326">可取值为：`manual`、`automatic`、`disabled`。</span><span class="sxs-lookup"><span data-stu-id="4db07-326">Possible values are: `manual`, `automatic`, `disabled`.</span></span>|
|<span data-ttu-id="4db07-327">xboxServicesLiveGameSaveServiceStartupMode</span><span class="sxs-lookup"><span data-stu-id="4db07-327">xboxServicesLiveGameSaveServiceStartupMode</span></span>|[<span data-ttu-id="4db07-328">serviceStartType</span><span class="sxs-lookup"><span data-stu-id="4db07-328">serviceStartType</span></span>](../resources/intune-deviceconfig-servicestarttype.md)|<span data-ttu-id="4db07-329">此设置确定实时游戏是否保存服务的启动类型为自动（2）、手动（3）、已禁用（4）。</span><span class="sxs-lookup"><span data-stu-id="4db07-329">This setting determines whether Live Game save service's start type is Automatic(2), Manual(3), Disabled(4).</span></span> <span data-ttu-id="4db07-330">默认：手动。</span><span class="sxs-lookup"><span data-stu-id="4db07-330">Default: Manual.</span></span> <span data-ttu-id="4db07-331">可取值为：`manual`、`automatic`、`disabled`。</span><span class="sxs-lookup"><span data-stu-id="4db07-331">Possible values are: `manual`, `automatic`, `disabled`.</span></span>|
|<span data-ttu-id="4db07-332">xboxServicesLiveNetworkingServiceStartupMode</span><span class="sxs-lookup"><span data-stu-id="4db07-332">xboxServicesLiveNetworkingServiceStartupMode</span></span>|[<span data-ttu-id="4db07-333">serviceStartType</span><span class="sxs-lookup"><span data-stu-id="4db07-333">serviceStartType</span></span>](../resources/intune-deviceconfig-servicestarttype.md)|<span data-ttu-id="4db07-334">此设置确定网络服务的启动类型是否为自动（2）、手动（3）、已禁用（4）。</span><span class="sxs-lookup"><span data-stu-id="4db07-334">This setting determines whether Networking service's start type is Automatic(2), Manual(3), Disabled(4).</span></span> <span data-ttu-id="4db07-335">默认：手动。</span><span class="sxs-lookup"><span data-stu-id="4db07-335">Default: Manual.</span></span> <span data-ttu-id="4db07-336">可取值为：`manual`、`automatic`、`disabled`。</span><span class="sxs-lookup"><span data-stu-id="4db07-336">Possible values are: `manual`, `automatic`, `disabled`.</span></span>|
|<span data-ttu-id="4db07-337">localSecurityOptionsBlockMicrosoftAccounts</span><span class="sxs-lookup"><span data-stu-id="4db07-337">localSecurityOptionsBlockMicrosoftAccounts</span></span>|<span data-ttu-id="4db07-338">Boolean</span><span class="sxs-lookup"><span data-stu-id="4db07-338">Boolean</span></span>|<span data-ttu-id="4db07-339">阻止用户向此计算机添加新的 Microsoft 帐户。</span><span class="sxs-lookup"><span data-stu-id="4db07-339">Prevent users from adding new Microsoft accounts to this computer.</span></span>|
|<span data-ttu-id="4db07-340">localSecurityOptionsBlockRemoteLogonWithBlankPassword</span><span class="sxs-lookup"><span data-stu-id="4db07-340">localSecurityOptionsBlockRemoteLogonWithBlankPassword</span></span>|<span data-ttu-id="4db07-341">Boolean</span><span class="sxs-lookup"><span data-stu-id="4db07-341">Boolean</span></span>|<span data-ttu-id="4db07-342">启用不受密码保护的本地帐户从物理设备以外的位置进行登录。默认值为已启用</span><span class="sxs-lookup"><span data-stu-id="4db07-342">Enable Local accounts that are not password protected to log on from locations other than the physical device.Default is enabled</span></span>|
|<span data-ttu-id="4db07-343">localSecurityOptionsDisableAdministratorAccount</span><span class="sxs-lookup"><span data-stu-id="4db07-343">localSecurityOptionsDisableAdministratorAccount</span></span>|<span data-ttu-id="4db07-344">Boolean</span><span class="sxs-lookup"><span data-stu-id="4db07-344">Boolean</span></span>|<span data-ttu-id="4db07-345">确定是否启用或禁用本地管理员帐户。</span><span class="sxs-lookup"><span data-stu-id="4db07-345">Determines whether the Local Administrator account is enabled or disabled.</span></span>|
|<span data-ttu-id="4db07-346">localSecurityOptionsAdministratorAccountName</span><span class="sxs-lookup"><span data-stu-id="4db07-346">localSecurityOptionsAdministratorAccountName</span></span>|<span data-ttu-id="4db07-347">字符串</span><span class="sxs-lookup"><span data-stu-id="4db07-347">String</span></span>|<span data-ttu-id="4db07-348">定义要与帐户 "管理员" 的安全标识符（SID）相关联的不同帐户名称。</span><span class="sxs-lookup"><span data-stu-id="4db07-348">Define a different account name to be associated with the security identifier (SID) for the account “Administrator”.</span></span>|
|<span data-ttu-id="4db07-349">localSecurityOptionsDisableGuestAccount</span><span class="sxs-lookup"><span data-stu-id="4db07-349">localSecurityOptionsDisableGuestAccount</span></span>|<span data-ttu-id="4db07-350">Boolean</span><span class="sxs-lookup"><span data-stu-id="4db07-350">Boolean</span></span>|<span data-ttu-id="4db07-351">确定来宾帐户是否已启用或已禁用。</span><span class="sxs-lookup"><span data-stu-id="4db07-351">Determines if the Guest account is enabled or disabled.</span></span>|
|<span data-ttu-id="4db07-352">localSecurityOptionsGuestAccountName</span><span class="sxs-lookup"><span data-stu-id="4db07-352">localSecurityOptionsGuestAccountName</span></span>|<span data-ttu-id="4db07-353">字符串</span><span class="sxs-lookup"><span data-stu-id="4db07-353">String</span></span>|<span data-ttu-id="4db07-354">定义要与帐户 "来宾" 的安全标识符（SID）相关联的不同帐户名称。</span><span class="sxs-lookup"><span data-stu-id="4db07-354">Define a different account name to be associated with the security identifier (SID) for the account “Guest”.</span></span>|
|<span data-ttu-id="4db07-355">localSecurityOptionsAllowUndockWithoutHavingToLogon</span><span class="sxs-lookup"><span data-stu-id="4db07-355">localSecurityOptionsAllowUndockWithoutHavingToLogon</span></span>|<span data-ttu-id="4db07-356">Boolean</span><span class="sxs-lookup"><span data-stu-id="4db07-356">Boolean</span></span>|<span data-ttu-id="4db07-357">阻止便携式计算机在无需登录的情况下被移除。</span><span class="sxs-lookup"><span data-stu-id="4db07-357">Prevent a portable computer from being undocked without having to log in.</span></span>|
|<span data-ttu-id="4db07-358">localSecurityOptionsBlockUsersInstallingPrinterDrivers</span><span class="sxs-lookup"><span data-stu-id="4db07-358">localSecurityOptionsBlockUsersInstallingPrinterDrivers</span></span>|<span data-ttu-id="4db07-359">Boolean</span><span class="sxs-lookup"><span data-stu-id="4db07-359">Boolean</span></span>|<span data-ttu-id="4db07-360">仅在将打印机驱动程序连接到共享打印机时，才将其限制为仅供管理员安装。</span><span class="sxs-lookup"><span data-stu-id="4db07-360">Restrict installing printer drivers as part of connecting to a shared printer to admins only.</span></span>|
|<span data-ttu-id="4db07-361">localSecurityOptionsBlockRemoteOpticalDriveAccess</span><span class="sxs-lookup"><span data-stu-id="4db07-361">localSecurityOptionsBlockRemoteOpticalDriveAccess</span></span>|<span data-ttu-id="4db07-362">Boolean</span><span class="sxs-lookup"><span data-stu-id="4db07-362">Boolean</span></span>|<span data-ttu-id="4db07-363">如果启用此设置，则仅允许交互式登录用户访问 CD-ROM 媒体。</span><span class="sxs-lookup"><span data-stu-id="4db07-363">Enabling this settings allows only interactively logged on user to access CD-ROM media.</span></span>|
|<span data-ttu-id="4db07-364">localSecurityOptionsFormatAndEjectOfRemovableMediaAllowedUser</span><span class="sxs-lookup"><span data-stu-id="4db07-364">localSecurityOptionsFormatAndEjectOfRemovableMediaAllowedUser</span></span>|[<span data-ttu-id="4db07-365">localSecurityOptionsFormatAndEjectOfRemovableMediaAllowedUserType</span><span class="sxs-lookup"><span data-stu-id="4db07-365">localSecurityOptionsFormatAndEjectOfRemovableMediaAllowedUserType</span></span>](../resources/intune-deviceconfig-localsecurityoptionsformatandejectofremovablemediaallowedusertype.md)|<span data-ttu-id="4db07-366">定义允许格式化和弹出可移动 NTFS 媒体的权限。</span><span class="sxs-lookup"><span data-stu-id="4db07-366">Define who is allowed to format and eject removable NTFS media.</span></span> <span data-ttu-id="4db07-367">可取值为：`notConfigured`、`administrators`、`administratorsAndPowerUsers`、`administratorsAndInteractiveUsers`。</span><span class="sxs-lookup"><span data-stu-id="4db07-367">Possible values are: `notConfigured`, `administrators`, `administratorsAndPowerUsers`, `administratorsAndInteractiveUsers`.</span></span>|
|<span data-ttu-id="4db07-368">localSecurityOptionsMachineInactivityLimit</span><span class="sxs-lookup"><span data-stu-id="4db07-368">localSecurityOptionsMachineInactivityLimit</span></span>|<span data-ttu-id="4db07-369">Int32</span><span class="sxs-lookup"><span data-stu-id="4db07-369">Int32</span></span>|<span data-ttu-id="4db07-370">在屏幕保护程序运行之前，定义交互式桌面登录屏幕上不活动的最长分钟数。</span><span class="sxs-lookup"><span data-stu-id="4db07-370">Define maximum minutes of inactivity on the interactive desktop’s login screen until the screen saver runs.</span></span> <span data-ttu-id="4db07-371">有效值为0至9999</span><span class="sxs-lookup"><span data-stu-id="4db07-371">Valid values 0 to 9999</span></span>|
|<span data-ttu-id="4db07-372">localSecurityOptionsMachineInactivityLimitInMinutes</span><span class="sxs-lookup"><span data-stu-id="4db07-372">localSecurityOptionsMachineInactivityLimitInMinutes</span></span>|<span data-ttu-id="4db07-373">Int32</span><span class="sxs-lookup"><span data-stu-id="4db07-373">Int32</span></span>|<span data-ttu-id="4db07-374">在屏幕保护程序运行之前，定义交互式桌面登录屏幕上不活动的最长分钟数。</span><span class="sxs-lookup"><span data-stu-id="4db07-374">Define maximum minutes of inactivity on the interactive desktop’s login screen until the screen saver runs.</span></span> <span data-ttu-id="4db07-375">有效值为0至9999</span><span class="sxs-lookup"><span data-stu-id="4db07-375">Valid values 0 to 9999</span></span>|
|<span data-ttu-id="4db07-376">localSecurityOptionsDoNotRequireCtrlAltDel</span><span class="sxs-lookup"><span data-stu-id="4db07-376">localSecurityOptionsDoNotRequireCtrlAltDel</span></span>|<span data-ttu-id="4db07-377">Boolean</span><span class="sxs-lookup"><span data-stu-id="4db07-377">Boolean</span></span>|<span data-ttu-id="4db07-378">要求用户在登录前按 CTRL + ALT + DEL。</span><span class="sxs-lookup"><span data-stu-id="4db07-378">Require CTRL+ALT+DEL to be pressed before a user can log on.</span></span>|
|<span data-ttu-id="4db07-379">localSecurityOptionsHideLastSignedInUser</span><span class="sxs-lookup"><span data-stu-id="4db07-379">localSecurityOptionsHideLastSignedInUser</span></span>|<span data-ttu-id="4db07-380">Boolean</span><span class="sxs-lookup"><span data-stu-id="4db07-380">Boolean</span></span>|<span data-ttu-id="4db07-381">不显示上次在此设备上登录的用户的用户名。</span><span class="sxs-lookup"><span data-stu-id="4db07-381">Do not display the username of the last person who signed in on this device.</span></span>|
|<span data-ttu-id="4db07-382">localSecurityOptionsHideUsernameAtSignIn</span><span class="sxs-lookup"><span data-stu-id="4db07-382">localSecurityOptionsHideUsernameAtSignIn</span></span>|<span data-ttu-id="4db07-383">Boolean</span><span class="sxs-lookup"><span data-stu-id="4db07-383">Boolean</span></span>|<span data-ttu-id="4db07-384">在输入凭据后以及显示设备桌面之前，请勿显示登录此设备的人员的用户名。</span><span class="sxs-lookup"><span data-stu-id="4db07-384">Do not display the username of the person signing in to this device after credentials are entered and before the device’s desktop is shown.</span></span>|
|<span data-ttu-id="4db07-385">localSecurityOptionsLogOnMessageTitle</span><span class="sxs-lookup"><span data-stu-id="4db07-385">localSecurityOptionsLogOnMessageTitle</span></span>|<span data-ttu-id="4db07-386">字符串</span><span class="sxs-lookup"><span data-stu-id="4db07-386">String</span></span>|<span data-ttu-id="4db07-387">为尝试登录的用户设置消息标题。</span><span class="sxs-lookup"><span data-stu-id="4db07-387">Set message title for users attempting to log in.</span></span>|
|<span data-ttu-id="4db07-388">localSecurityOptionsLogOnMessageText</span><span class="sxs-lookup"><span data-stu-id="4db07-388">localSecurityOptionsLogOnMessageText</span></span>|<span data-ttu-id="4db07-389">字符串</span><span class="sxs-lookup"><span data-stu-id="4db07-389">String</span></span>|<span data-ttu-id="4db07-390">为尝试登录的用户设置消息文本。</span><span class="sxs-lookup"><span data-stu-id="4db07-390">Set message text for users attempting to log in.</span></span>|
|<span data-ttu-id="4db07-391">localSecurityOptionsAllowPKU2UAuthenticationRequests</span><span class="sxs-lookup"><span data-stu-id="4db07-391">localSecurityOptionsAllowPKU2UAuthenticationRequests</span></span>|<span data-ttu-id="4db07-392">Boolean</span><span class="sxs-lookup"><span data-stu-id="4db07-392">Boolean</span></span>|<span data-ttu-id="4db07-393">阻止 PKU2U 对此设备的身份验证请求，以使用联机标识。</span><span class="sxs-lookup"><span data-stu-id="4db07-393">Block PKU2U authentication requests to this device to use online identities.</span></span>|
|<span data-ttu-id="4db07-394">localSecurityOptionsAllowRemoteCallsToSecurityAccountsManagerHelperBool</span><span class="sxs-lookup"><span data-stu-id="4db07-394">localSecurityOptionsAllowRemoteCallsToSecurityAccountsManagerHelperBool</span></span>|<span data-ttu-id="4db07-395">Boolean</span><span class="sxs-lookup"><span data-stu-id="4db07-395">Boolean</span></span>|<span data-ttu-id="4db07-396">LocalSecurityOptionsAllowRemoteCallsToSecurityAccountsManager 实体的 UI 帮助程序布尔值</span><span class="sxs-lookup"><span data-stu-id="4db07-396">UI helper boolean for LocalSecurityOptionsAllowRemoteCallsToSecurityAccountsManager entity</span></span>|
|<span data-ttu-id="4db07-397">localSecurityOptionsAllowRemoteCallsToSecurityAccountsManager</span><span class="sxs-lookup"><span data-stu-id="4db07-397">localSecurityOptionsAllowRemoteCallsToSecurityAccountsManager</span></span>|<span data-ttu-id="4db07-398">字符串</span><span class="sxs-lookup"><span data-stu-id="4db07-398">String</span></span>|<span data-ttu-id="4db07-399">编辑默认的安全描述符定义语言字符串，以允许或拒绝用户和组对 SAM 进行远程调用。</span><span class="sxs-lookup"><span data-stu-id="4db07-399">Edit the default Security Descriptor Definition Language string to allow or deny users and groups to make remote calls to the SAM.</span></span>|
|<span data-ttu-id="4db07-400">localSecurityOptionsMinimumSessionSecurityForNtlmSspBasedClients</span><span class="sxs-lookup"><span data-stu-id="4db07-400">localSecurityOptionsMinimumSessionSecurityForNtlmSspBasedClients</span></span>|[<span data-ttu-id="4db07-401">localSecurityOptionsMinimumSessionSecurity</span><span class="sxs-lookup"><span data-stu-id="4db07-401">localSecurityOptionsMinimumSessionSecurity</span></span>](../resources/intune-deviceconfig-localsecurityoptionsminimumsessionsecurity.md)|<span data-ttu-id="4db07-402">此安全设置允许客户端要求协商128位加密和/或 NTLMv2 会话安全性。</span><span class="sxs-lookup"><span data-stu-id="4db07-402">This security setting allows a client to require the negotiation of 128-bit encryption and/or NTLMv2 session security.</span></span> <span data-ttu-id="4db07-403">可取值为：`none`、`requireNtmlV2SessionSecurity`、`require128BitEncryption`、`ntlmV2And128BitEncryption`。</span><span class="sxs-lookup"><span data-stu-id="4db07-403">Possible values are: `none`, `requireNtmlV2SessionSecurity`, `require128BitEncryption`, `ntlmV2And128BitEncryption`.</span></span>|
|<span data-ttu-id="4db07-404">localSecurityOptionsMinimumSessionSecurityForNtlmSspBasedServers</span><span class="sxs-lookup"><span data-stu-id="4db07-404">localSecurityOptionsMinimumSessionSecurityForNtlmSspBasedServers</span></span>|[<span data-ttu-id="4db07-405">localSecurityOptionsMinimumSessionSecurity</span><span class="sxs-lookup"><span data-stu-id="4db07-405">localSecurityOptionsMinimumSessionSecurity</span></span>](../resources/intune-deviceconfig-localsecurityoptionsminimumsessionsecurity.md)|<span data-ttu-id="4db07-406">此安全设置允许服务器要求协商128位加密和/或 NTLMv2 会话安全性。</span><span class="sxs-lookup"><span data-stu-id="4db07-406">This security setting allows a server to require the negotiation of 128-bit encryption and/or NTLMv2 session security.</span></span> <span data-ttu-id="4db07-407">可取值为：`none`、`requireNtmlV2SessionSecurity`、`require128BitEncryption`、`ntlmV2And128BitEncryption`。</span><span class="sxs-lookup"><span data-stu-id="4db07-407">Possible values are: `none`, `requireNtmlV2SessionSecurity`, `require128BitEncryption`, `ntlmV2And128BitEncryption`.</span></span>|
|<span data-ttu-id="4db07-408">lanManagerAuthenticationLevel</span><span class="sxs-lookup"><span data-stu-id="4db07-408">lanManagerAuthenticationLevel</span></span>|[<span data-ttu-id="4db07-409">lanManagerAuthenticationLevel</span><span class="sxs-lookup"><span data-stu-id="4db07-409">lanManagerAuthenticationLevel</span></span>](../resources/intune-deviceconfig-lanmanagerauthenticationlevel.md)|<span data-ttu-id="4db07-410">此安全设置确定用于网络登录的质询/响应身份验证协议。</span><span class="sxs-lookup"><span data-stu-id="4db07-410">This security setting determines which challenge/response authentication protocol is used for network logons.</span></span> <span data-ttu-id="4db07-411">可取值为：`lmAndNltm`、`lmNtlmAndNtlmV2`、`lmAndNtlmOnly`、`lmAndNtlmV2`、`lmNtlmV2AndNotLm`、`lmNtlmV2AndNotLmOrNtm`。</span><span class="sxs-lookup"><span data-stu-id="4db07-411">Possible values are: `lmAndNltm`, `lmNtlmAndNtlmV2`, `lmAndNtlmOnly`, `lmAndNtlmV2`, `lmNtlmV2AndNotLm`, `lmNtlmV2AndNotLmOrNtm`.</span></span>|
|<span data-ttu-id="4db07-412">lanManagerWorkstationDisableInsecureGuestLogons</span><span class="sxs-lookup"><span data-stu-id="4db07-412">lanManagerWorkstationDisableInsecureGuestLogons</span></span>|<span data-ttu-id="4db07-413">Boolean</span><span class="sxs-lookup"><span data-stu-id="4db07-413">Boolean</span></span>|<span data-ttu-id="4db07-414">如果启用，SMB 客户端将允许不安全的来宾登录。</span><span class="sxs-lookup"><span data-stu-id="4db07-414">If enabled,the SMB client will allow insecure guest logons.</span></span> <span data-ttu-id="4db07-415">如果未配置，SMB 客户端将拒绝不安全的来宾登录。</span><span class="sxs-lookup"><span data-stu-id="4db07-415">If not configured, the SMB client will reject insecure guest logons.</span></span>|
|<span data-ttu-id="4db07-416">localSecurityOptionsClearVirtualMemoryPageFile</span><span class="sxs-lookup"><span data-stu-id="4db07-416">localSecurityOptionsClearVirtualMemoryPageFile</span></span>|<span data-ttu-id="4db07-417">Boolean</span><span class="sxs-lookup"><span data-stu-id="4db07-417">Boolean</span></span>|<span data-ttu-id="4db07-418">此安全设置确定在关闭系统时是否清除虚拟内存页面文件。</span><span class="sxs-lookup"><span data-stu-id="4db07-418">This security setting determines whether the virtual memory pagefile is cleared when the system is shut down.</span></span>|
|<span data-ttu-id="4db07-419">localSecurityOptionsAllowSystemToBeShutDownWithoutHavingToLogOn</span><span class="sxs-lookup"><span data-stu-id="4db07-419">localSecurityOptionsAllowSystemToBeShutDownWithoutHavingToLogOn</span></span>|<span data-ttu-id="4db07-420">Boolean</span><span class="sxs-lookup"><span data-stu-id="4db07-420">Boolean</span></span>|<span data-ttu-id="4db07-421">此安全设置确定是否可以在不登录 Windows 的情况下关闭计算机。</span><span class="sxs-lookup"><span data-stu-id="4db07-421">This security setting determines whether a computer can be shut down without having to log on to Windows.</span></span>|
|<span data-ttu-id="4db07-422">localSecurityOptionsAllowUIAccessApplicationElevation</span><span class="sxs-lookup"><span data-stu-id="4db07-422">localSecurityOptionsAllowUIAccessApplicationElevation</span></span>|<span data-ttu-id="4db07-423">Boolean</span><span class="sxs-lookup"><span data-stu-id="4db07-423">Boolean</span></span>|<span data-ttu-id="4db07-424">允许 UIAccess 应用在不使用安全桌面的情况下提示提升。</span><span class="sxs-lookup"><span data-stu-id="4db07-424">Allow UIAccess apps to prompt for elevation without using the secure desktop.</span></span>|
|<span data-ttu-id="4db07-425">localSecurityOptionsVirtualizeFileAndRegistryWriteFailuresToPerUserLocations</span><span class="sxs-lookup"><span data-stu-id="4db07-425">localSecurityOptionsVirtualizeFileAndRegistryWriteFailuresToPerUserLocations</span></span>|<span data-ttu-id="4db07-426">Boolean</span><span class="sxs-lookup"><span data-stu-id="4db07-426">Boolean</span></span>|<span data-ttu-id="4db07-427">将文件和注册表写入失败虚拟化到每个用户位置</span><span class="sxs-lookup"><span data-stu-id="4db07-427">Virtualize file and registry write failures to per user locations</span></span>|
|<span data-ttu-id="4db07-428">localSecurityOptionsOnlyElevateSignedExecutables</span><span class="sxs-lookup"><span data-stu-id="4db07-428">localSecurityOptionsOnlyElevateSignedExecutables</span></span>|<span data-ttu-id="4db07-429">Boolean</span><span class="sxs-lookup"><span data-stu-id="4db07-429">Boolean</span></span>|<span data-ttu-id="4db07-430">对给定的可执行文件强制执行 PKI 证书路径验证，然后再允许运行该文件。</span><span class="sxs-lookup"><span data-stu-id="4db07-430">Enforce PKI certification path validation for a given executable file before it is permitted to run.</span></span>|
|<span data-ttu-id="4db07-431">localSecurityOptionsAdministratorElevationPromptBehavior</span><span class="sxs-lookup"><span data-stu-id="4db07-431">localSecurityOptionsAdministratorElevationPromptBehavior</span></span>|[<span data-ttu-id="4db07-432">localSecurityOptionsAdministratorElevationPromptBehaviorType</span><span class="sxs-lookup"><span data-stu-id="4db07-432">localSecurityOptionsAdministratorElevationPromptBehaviorType</span></span>](../resources/intune-deviceconfig-localsecurityoptionsadministratorelevationpromptbehaviortype.md)|<span data-ttu-id="4db07-433">在管理员审批模式中定义管理员的提升提示行为。</span><span class="sxs-lookup"><span data-stu-id="4db07-433">Define the behavior of the elevation prompt for admins in Admin Approval Mode.</span></span> <span data-ttu-id="4db07-434">可取值为：`notConfigured`、`elevateWithoutPrompting`、`promptForCredentialsOnTheSecureDesktop`、`promptForConsentOnTheSecureDesktop`、`promptForCredentials`、`promptForConsent` 或 `promptForConsentForNonWindowsBinaries`。</span><span class="sxs-lookup"><span data-stu-id="4db07-434">Possible values are: `notConfigured`, `elevateWithoutPrompting`, `promptForCredentialsOnTheSecureDesktop`, `promptForConsentOnTheSecureDesktop`, `promptForCredentials`, `promptForConsent`, `promptForConsentForNonWindowsBinaries`.</span></span>|
|<span data-ttu-id="4db07-435">localSecurityOptionsStandardUserElevationPromptBehavior</span><span class="sxs-lookup"><span data-stu-id="4db07-435">localSecurityOptionsStandardUserElevationPromptBehavior</span></span>|[<span data-ttu-id="4db07-436">localSecurityOptionsStandardUserElevationPromptBehaviorType</span><span class="sxs-lookup"><span data-stu-id="4db07-436">localSecurityOptionsStandardUserElevationPromptBehaviorType</span></span>](../resources/intune-deviceconfig-localsecurityoptionsstandarduserelevationpromptbehaviortype.md)|<span data-ttu-id="4db07-437">定义标准用户的提升提示行为。</span><span class="sxs-lookup"><span data-stu-id="4db07-437">Define the behavior of the elevation prompt for standard users.</span></span> <span data-ttu-id="4db07-438">可取值为：`notConfigured`、`automaticallyDenyElevationRequests`、`promptForCredentialsOnTheSecureDesktop`、`promptForCredentials`。</span><span class="sxs-lookup"><span data-stu-id="4db07-438">Possible values are: `notConfigured`, `automaticallyDenyElevationRequests`, `promptForCredentialsOnTheSecureDesktop`, `promptForCredentials`.</span></span>|
|<span data-ttu-id="4db07-439">localSecurityOptionsSwitchToSecureDesktopWhenPromptingForElevation</span><span class="sxs-lookup"><span data-stu-id="4db07-439">localSecurityOptionsSwitchToSecureDesktopWhenPromptingForElevation</span></span>|<span data-ttu-id="4db07-440">Boolean</span><span class="sxs-lookup"><span data-stu-id="4db07-440">Boolean</span></span>|<span data-ttu-id="4db07-441">启用所有提升请求以转到交互式用户的桌面，而不是安全桌面。</span><span class="sxs-lookup"><span data-stu-id="4db07-441">Enable all elevation requests to go to the interactive user's desktop rather than the secure desktop.</span></span> <span data-ttu-id="4db07-442">使用管理员和标准用户的提示行为策略设置。</span><span class="sxs-lookup"><span data-stu-id="4db07-442">Prompt behavior policy settings for admins and standard users are used.</span></span>|
|<span data-ttu-id="4db07-443">localSecurityOptionsDetectApplicationInstallationsAndPromptForElevation</span><span class="sxs-lookup"><span data-stu-id="4db07-443">localSecurityOptionsDetectApplicationInstallationsAndPromptForElevation</span></span>|<span data-ttu-id="4db07-444">Boolean</span><span class="sxs-lookup"><span data-stu-id="4db07-444">Boolean</span></span>|<span data-ttu-id="4db07-445">需要提升权限的应用程序安装将提示管理凭据。默认值为已启用</span><span class="sxs-lookup"><span data-stu-id="4db07-445">App installations requiring elevated privileges will prompt for admin credentials.Default is enabled</span></span>|
|<span data-ttu-id="4db07-446">localSecurityOptionsAllowUIAccessApplicationsForSecureLocations</span><span class="sxs-lookup"><span data-stu-id="4db07-446">localSecurityOptionsAllowUIAccessApplicationsForSecureLocations</span></span>|<span data-ttu-id="4db07-447">Boolean</span><span class="sxs-lookup"><span data-stu-id="4db07-447">Boolean</span></span>|<span data-ttu-id="4db07-448">允许 UIAccess 应用在不使用安全桌面的情况下提示提升。默认值为已启用</span><span class="sxs-lookup"><span data-stu-id="4db07-448">Allow UIAccess apps to prompt for elevation without using the secure desktop.Default is enabled</span></span>|
|<span data-ttu-id="4db07-449">localSecurityOptionsUseAdminApprovalMode</span><span class="sxs-lookup"><span data-stu-id="4db07-449">localSecurityOptionsUseAdminApprovalMode</span></span>|<span data-ttu-id="4db07-450">Boolean</span><span class="sxs-lookup"><span data-stu-id="4db07-450">Boolean</span></span>|<span data-ttu-id="4db07-451">定义内置管理员帐户是使用管理员审批模式，还是运行所有具有完全管理员权限的应用程序。默认值为已启用</span><span class="sxs-lookup"><span data-stu-id="4db07-451">Defines whether the built-in admin account uses Admin Approval Mode or runs all apps with full admin privileges.Default is enabled</span></span>|
|<span data-ttu-id="4db07-452">localSecurityOptionsUseAdminApprovalModeForAdministrators</span><span class="sxs-lookup"><span data-stu-id="4db07-452">localSecurityOptionsUseAdminApprovalModeForAdministrators</span></span>|<span data-ttu-id="4db07-453">Boolean</span><span class="sxs-lookup"><span data-stu-id="4db07-453">Boolean</span></span>|<span data-ttu-id="4db07-454">定义是否启用管理员批准模式和所有 UAC 策略设置，默认为启用</span><span class="sxs-lookup"><span data-stu-id="4db07-454">Define whether Admin Approval Mode and all UAC policy settings are enabled, default is enabled</span></span>|
|<span data-ttu-id="4db07-455">localSecurityOptionsInformationShownOnLockScreen</span><span class="sxs-lookup"><span data-stu-id="4db07-455">localSecurityOptionsInformationShownOnLockScreen</span></span>|[<span data-ttu-id="4db07-456">localSecurityOptionsInformationShownOnLockScreenType</span><span class="sxs-lookup"><span data-stu-id="4db07-456">localSecurityOptionsInformationShownOnLockScreenType</span></span>](../resources/intune-deviceconfig-localsecurityoptionsinformationshownonlockscreentype.md)|<span data-ttu-id="4db07-457">配置在会话锁定时显示的用户信息。</span><span class="sxs-lookup"><span data-stu-id="4db07-457">Configure the user information that is displayed when the session is locked.</span></span> <span data-ttu-id="4db07-458">如果未配置，则显示用户显示名称、域和用户名。</span><span class="sxs-lookup"><span data-stu-id="4db07-458">If not configured, user display name, domain and username are shown.</span></span> <span data-ttu-id="4db07-459">可取值为：`notConfigured`、`userDisplayNameDomainUser`、`userDisplayNameOnly`、`doNotDisplayUser`。</span><span class="sxs-lookup"><span data-stu-id="4db07-459">Possible values are: `notConfigured`, `userDisplayNameDomainUser`, `userDisplayNameOnly`, `doNotDisplayUser`.</span></span>|
|<span data-ttu-id="4db07-460">localSecurityOptionsInformationDisplayedOnLockScreen</span><span class="sxs-lookup"><span data-stu-id="4db07-460">localSecurityOptionsInformationDisplayedOnLockScreen</span></span>|[<span data-ttu-id="4db07-461">localSecurityOptionsInformationDisplayedOnLockScreenType</span><span class="sxs-lookup"><span data-stu-id="4db07-461">localSecurityOptionsInformationDisplayedOnLockScreenType</span></span>](../resources/intune-deviceconfig-localsecurityoptionsinformationdisplayedonlockscreentype.md)|<span data-ttu-id="4db07-462">配置在会话锁定时显示的用户信息。</span><span class="sxs-lookup"><span data-stu-id="4db07-462">Configure the user information that is displayed when the session is locked.</span></span> <span data-ttu-id="4db07-463">如果未配置，则显示用户显示名称、域和用户名。</span><span class="sxs-lookup"><span data-stu-id="4db07-463">If not configured, user display name, domain and username are shown.</span></span> <span data-ttu-id="4db07-464">可取值为：`notConfigured`、`administrators`、`administratorsAndPowerUsers`、`administratorsAndInteractiveUsers`。</span><span class="sxs-lookup"><span data-stu-id="4db07-464">Possible values are: `notConfigured`, `administrators`, `administratorsAndPowerUsers`, `administratorsAndInteractiveUsers`.</span></span>|
|<span data-ttu-id="4db07-465">localSecurityOptionsDisableClientDigitallySignCommunicationsIfServerAgrees</span><span class="sxs-lookup"><span data-stu-id="4db07-465">localSecurityOptionsDisableClientDigitallySignCommunicationsIfServerAgrees</span></span>|<span data-ttu-id="4db07-466">Boolean</span><span class="sxs-lookup"><span data-stu-id="4db07-466">Boolean</span></span>|<span data-ttu-id="4db07-467">此安全设置确定 SMB 客户端是否尝试协商 SMB 数据包签名。</span><span class="sxs-lookup"><span data-stu-id="4db07-467">This security setting determines whether the SMB client attempts to negotiate SMB packet signing.</span></span>|
|<span data-ttu-id="4db07-468">localSecurityOptionsClientDigitallySignCommunicationsAlways</span><span class="sxs-lookup"><span data-stu-id="4db07-468">localSecurityOptionsClientDigitallySignCommunicationsAlways</span></span>|<span data-ttu-id="4db07-469">Boolean</span><span class="sxs-lookup"><span data-stu-id="4db07-469">Boolean</span></span>|<span data-ttu-id="4db07-470">此安全设置确定 SMB 客户端组件是否需要数据包签名。</span><span class="sxs-lookup"><span data-stu-id="4db07-470">This security setting determines whether packet signing is required by the SMB client component.</span></span>|
|<span data-ttu-id="4db07-471">localSecurityOptionsClientSendUnencryptedPasswordToThirdPartySMBServers</span><span class="sxs-lookup"><span data-stu-id="4db07-471">localSecurityOptionsClientSendUnencryptedPasswordToThirdPartySMBServers</span></span>|<span data-ttu-id="4db07-472">Boolean</span><span class="sxs-lookup"><span data-stu-id="4db07-472">Boolean</span></span>|<span data-ttu-id="4db07-473">如果启用此安全设置，则允许服务器消息块（SMB）重定向程序将纯文本密码发送到在身份验证过程中不支持密码加密的非 Microsoft SMB 服务器。</span><span class="sxs-lookup"><span data-stu-id="4db07-473">If this security setting is enabled, the Server Message Block (SMB) redirector is allowed to send plaintext passwords to non-Microsoft SMB servers that do not support password encryption during authentication.</span></span>|
|<span data-ttu-id="4db07-474">localSecurityOptionsDisableServerDigitallySignCommunicationsAlways</span><span class="sxs-lookup"><span data-stu-id="4db07-474">localSecurityOptionsDisableServerDigitallySignCommunicationsAlways</span></span>|<span data-ttu-id="4db07-475">Boolean</span><span class="sxs-lookup"><span data-stu-id="4db07-475">Boolean</span></span>|<span data-ttu-id="4db07-476">此安全设置确定 SMB 服务器组件是否需要数据包签名。</span><span class="sxs-lookup"><span data-stu-id="4db07-476">This security setting determines whether packet signing is required by the SMB server component.</span></span>|
|<span data-ttu-id="4db07-477">localSecurityOptionsDisableServerDigitallySignCommunicationsIfClientAgrees</span><span class="sxs-lookup"><span data-stu-id="4db07-477">localSecurityOptionsDisableServerDigitallySignCommunicationsIfClientAgrees</span></span>|<span data-ttu-id="4db07-478">Boolean</span><span class="sxs-lookup"><span data-stu-id="4db07-478">Boolean</span></span>|<span data-ttu-id="4db07-479">此安全设置确定 SMB 服务器是否将 SMB 数据包签名与请求的客户端协商。</span><span class="sxs-lookup"><span data-stu-id="4db07-479">This security setting determines whether the SMB server will negotiate SMB packet signing with clients that request it.</span></span>|
|<span data-ttu-id="4db07-480">localSecurityOptionsRestrictAnonymousAccessToNamedPipesAndShares</span><span class="sxs-lookup"><span data-stu-id="4db07-480">localSecurityOptionsRestrictAnonymousAccessToNamedPipesAndShares</span></span>|<span data-ttu-id="4db07-481">Boolean</span><span class="sxs-lookup"><span data-stu-id="4db07-481">Boolean</span></span>|<span data-ttu-id="4db07-482">默认情况下，此安全设置限制可匿名访问且可匿名访问的共享的命名管道设置对共享和管道的匿名访问权限</span><span class="sxs-lookup"><span data-stu-id="4db07-482">By default, this security setting restricts anonymous access to shares and pipes to the settings for named pipes that can be accessed anonymously and Shares that can be accessed anonymously</span></span>|
|<span data-ttu-id="4db07-483">localSecurityOptionsDoNotAllowAnonymousEnumerationOfSAMAccounts</span><span class="sxs-lookup"><span data-stu-id="4db07-483">localSecurityOptionsDoNotAllowAnonymousEnumerationOfSAMAccounts</span></span>|<span data-ttu-id="4db07-484">Boolean</span><span class="sxs-lookup"><span data-stu-id="4db07-484">Boolean</span></span>|<span data-ttu-id="4db07-485">此安全设置确定将向计算机的匿名连接授予的其他权限。</span><span class="sxs-lookup"><span data-stu-id="4db07-485">This security setting determines what additional permissions will be granted for anonymous connections to the computer.</span></span>|
|<span data-ttu-id="4db07-486">localSecurityOptionsAllowAnonymousEnumerationOfSAMAccountsAndShares</span><span class="sxs-lookup"><span data-stu-id="4db07-486">localSecurityOptionsAllowAnonymousEnumerationOfSAMAccountsAndShares</span></span>|<span data-ttu-id="4db07-487">Boolean</span><span class="sxs-lookup"><span data-stu-id="4db07-487">Boolean</span></span>|<span data-ttu-id="4db07-488">此安全设置确定是否允许匿名用户执行某些活动，如枚举域帐户和网络共享的名称。</span><span class="sxs-lookup"><span data-stu-id="4db07-488">This security setting determines whether to allows anonymous users to perform certain activities, such as enumerating the names of domain accounts and network shares.</span></span>|
|<span data-ttu-id="4db07-489">localSecurityOptionsDoNotStoreLANManagerHashValueOnNextPasswordChange</span><span class="sxs-lookup"><span data-stu-id="4db07-489">localSecurityOptionsDoNotStoreLANManagerHashValueOnNextPasswordChange</span></span>|<span data-ttu-id="4db07-490">Boolean</span><span class="sxs-lookup"><span data-stu-id="4db07-490">Boolean</span></span>|<span data-ttu-id="4db07-491">此安全设置确定在下一次更改密码时，是否存储新密码的 LAN Manager （LM）哈希值。</span><span class="sxs-lookup"><span data-stu-id="4db07-491">This security setting determines if, at the next password change, the LAN Manager (LM) hash value for the new password is stored.</span></span> <span data-ttu-id="4db07-492">默认情况下不存储它。</span><span class="sxs-lookup"><span data-stu-id="4db07-492">It’s not stored by default.</span></span>|
|<span data-ttu-id="4db07-493">localSecurityOptionsSmartCardRemovalBehavior</span><span class="sxs-lookup"><span data-stu-id="4db07-493">localSecurityOptionsSmartCardRemovalBehavior</span></span>|[<span data-ttu-id="4db07-494">localSecurityOptionsSmartCardRemovalBehaviorType</span><span class="sxs-lookup"><span data-stu-id="4db07-494">localSecurityOptionsSmartCardRemovalBehaviorType</span></span>](../resources/intune-deviceconfig-localsecurityoptionssmartcardremovalbehaviortype.md)|<span data-ttu-id="4db07-495">此安全设置确定将已登录用户的智能卡从智能卡读卡器中删除时发生的情况。</span><span class="sxs-lookup"><span data-stu-id="4db07-495">This security setting determines what happens when the smart card for a logged-on user is removed from the smart card reader.</span></span> <span data-ttu-id="4db07-496">可取值为：`lockWorkstation`、`noAction`、`forceLogoff`、`disconnectRemoteDesktopSession`。</span><span class="sxs-lookup"><span data-stu-id="4db07-496">Possible values are: `lockWorkstation`, `noAction`, `forceLogoff`, `disconnectRemoteDesktopSession`.</span></span>|
|<span data-ttu-id="4db07-497">defenderSecurityCenterDisableAppBrowserUI</span><span class="sxs-lookup"><span data-stu-id="4db07-497">defenderSecurityCenterDisableAppBrowserUI</span></span>|<span data-ttu-id="4db07-498">Boolean</span><span class="sxs-lookup"><span data-stu-id="4db07-498">Boolean</span></span>|<span data-ttu-id="4db07-499">用于禁用应用程序和浏览器保护区域的显示。</span><span class="sxs-lookup"><span data-stu-id="4db07-499">Used to disable the display of the app and browser protection area.</span></span>|
|<span data-ttu-id="4db07-500">defenderSecurityCenterDisableFamilyUI</span><span class="sxs-lookup"><span data-stu-id="4db07-500">defenderSecurityCenterDisableFamilyUI</span></span>|<span data-ttu-id="4db07-501">Boolean</span><span class="sxs-lookup"><span data-stu-id="4db07-501">Boolean</span></span>|<span data-ttu-id="4db07-502">用于禁用 "家庭选项" 区域的显示。</span><span class="sxs-lookup"><span data-stu-id="4db07-502">Used to disable the display of the family options area.</span></span>|
|<span data-ttu-id="4db07-503">defenderSecurityCenterDisableHealthUI</span><span class="sxs-lookup"><span data-stu-id="4db07-503">defenderSecurityCenterDisableHealthUI</span></span>|<span data-ttu-id="4db07-504">Boolean</span><span class="sxs-lookup"><span data-stu-id="4db07-504">Boolean</span></span>|<span data-ttu-id="4db07-505">用于禁用设备性能和运行状况区域的显示。</span><span class="sxs-lookup"><span data-stu-id="4db07-505">Used to disable the display of the device performance and health area.</span></span>|
|<span data-ttu-id="4db07-506">defenderSecurityCenterDisableNetworkUI</span><span class="sxs-lookup"><span data-stu-id="4db07-506">defenderSecurityCenterDisableNetworkUI</span></span>|<span data-ttu-id="4db07-507">Boolean</span><span class="sxs-lookup"><span data-stu-id="4db07-507">Boolean</span></span>|<span data-ttu-id="4db07-508">用于禁用防火墙和网络防护区域的显示。</span><span class="sxs-lookup"><span data-stu-id="4db07-508">Used to disable the display of the firewall and network protection area.</span></span>|
|<span data-ttu-id="4db07-509">defenderSecurityCenterDisableVirusUI</span><span class="sxs-lookup"><span data-stu-id="4db07-509">defenderSecurityCenterDisableVirusUI</span></span>|<span data-ttu-id="4db07-510">Boolean</span><span class="sxs-lookup"><span data-stu-id="4db07-510">Boolean</span></span>|<span data-ttu-id="4db07-511">用于禁用病毒和威胁防护区域的显示。</span><span class="sxs-lookup"><span data-stu-id="4db07-511">Used to disable the display of the virus and threat protection area.</span></span>|
|<span data-ttu-id="4db07-512">defenderSecurityCenterDisableAccountUI</span><span class="sxs-lookup"><span data-stu-id="4db07-512">defenderSecurityCenterDisableAccountUI</span></span>|<span data-ttu-id="4db07-513">Boolean</span><span class="sxs-lookup"><span data-stu-id="4db07-513">Boolean</span></span>|<span data-ttu-id="4db07-514">用于禁用帐户保护区域的显示。</span><span class="sxs-lookup"><span data-stu-id="4db07-514">Used to disable the display of the account protection area.</span></span>|
|<span data-ttu-id="4db07-515">defenderSecurityCenterDisableClearTpmUI</span><span class="sxs-lookup"><span data-stu-id="4db07-515">defenderSecurityCenterDisableClearTpmUI</span></span>|<span data-ttu-id="4db07-516">Boolean</span><span class="sxs-lookup"><span data-stu-id="4db07-516">Boolean</span></span>|<span data-ttu-id="4db07-517">用于禁用 "清除 TPM" 按钮的显示。</span><span class="sxs-lookup"><span data-stu-id="4db07-517">Used to disable the display of the Clear TPM button.</span></span>|
|<span data-ttu-id="4db07-518">defenderSecurityCenterDisableHardwareUI</span><span class="sxs-lookup"><span data-stu-id="4db07-518">defenderSecurityCenterDisableHardwareUI</span></span>|<span data-ttu-id="4db07-519">Boolean</span><span class="sxs-lookup"><span data-stu-id="4db07-519">Boolean</span></span>|<span data-ttu-id="4db07-520">用于禁用硬件保护区域的显示。</span><span class="sxs-lookup"><span data-stu-id="4db07-520">Used to disable the display of the hardware protection area.</span></span>|
|<span data-ttu-id="4db07-521">defenderSecurityCenterDisableNotificationAreaUI</span><span class="sxs-lookup"><span data-stu-id="4db07-521">defenderSecurityCenterDisableNotificationAreaUI</span></span>|<span data-ttu-id="4db07-522">Boolean</span><span class="sxs-lookup"><span data-stu-id="4db07-522">Boolean</span></span>|<span data-ttu-id="4db07-523">用于禁用通知区域控件的显示。</span><span class="sxs-lookup"><span data-stu-id="4db07-523">Used to disable the display of the notification area control.</span></span> <span data-ttu-id="4db07-524">用户需要注销并登录或重新启动计算机，此设置才会生效。</span><span class="sxs-lookup"><span data-stu-id="4db07-524">The user needs to either sign out and sign in or reboot the computer for this setting to take effect.</span></span>|
|<span data-ttu-id="4db07-525">defenderSecurityCenterDisableRansomwareUI</span><span class="sxs-lookup"><span data-stu-id="4db07-525">defenderSecurityCenterDisableRansomwareUI</span></span>|<span data-ttu-id="4db07-526">Boolean</span><span class="sxs-lookup"><span data-stu-id="4db07-526">Boolean</span></span>|<span data-ttu-id="4db07-527">用于禁用勒索软件防护区域的显示。</span><span class="sxs-lookup"><span data-stu-id="4db07-527">Used to disable the display of the ransomware protection area.</span></span> |
|<span data-ttu-id="4db07-528">defenderSecurityCenterDisableSecureBootUI</span><span class="sxs-lookup"><span data-stu-id="4db07-528">defenderSecurityCenterDisableSecureBootUI</span></span>|<span data-ttu-id="4db07-529">Boolean</span><span class="sxs-lookup"><span data-stu-id="4db07-529">Boolean</span></span>|<span data-ttu-id="4db07-530">用于在 "设备安全性" 下禁用安全引导区域的显示。</span><span class="sxs-lookup"><span data-stu-id="4db07-530">Used to disable the display of the secure boot area under Device security.</span></span>|
|<span data-ttu-id="4db07-531">defenderSecurityCenterDisableTroubleshootingUI</span><span class="sxs-lookup"><span data-stu-id="4db07-531">defenderSecurityCenterDisableTroubleshootingUI</span></span>|<span data-ttu-id="4db07-532">Boolean</span><span class="sxs-lookup"><span data-stu-id="4db07-532">Boolean</span></span>|<span data-ttu-id="4db07-533">用于在 "设备安全性" 下禁用安全过程故障排除的显示。</span><span class="sxs-lookup"><span data-stu-id="4db07-533">Used to disable the display of the security process troubleshooting under Device security.</span></span>|
|<span data-ttu-id="4db07-534">defenderSecurityCenterDisableVulnerableTpmFirmwareUpdateUI</span><span class="sxs-lookup"><span data-stu-id="4db07-534">defenderSecurityCenterDisableVulnerableTpmFirmwareUpdateUI</span></span>|<span data-ttu-id="4db07-535">Boolean</span><span class="sxs-lookup"><span data-stu-id="4db07-535">Boolean</span></span>|<span data-ttu-id="4db07-536">用于在检测到易受攻击的固件时禁用显示更新 TPM 固件。</span><span class="sxs-lookup"><span data-stu-id="4db07-536">Used to disable the display of update TPM Firmware when a vulnerable firmware is detected.</span></span>|
|<span data-ttu-id="4db07-537">defenderSecurityCenterOrganizationDisplayName</span><span class="sxs-lookup"><span data-stu-id="4db07-537">defenderSecurityCenterOrganizationDisplayName</span></span>|<span data-ttu-id="4db07-538">字符串</span><span class="sxs-lookup"><span data-stu-id="4db07-538">String</span></span>|<span data-ttu-id="4db07-539">向用户显示的公司名称。</span><span class="sxs-lookup"><span data-stu-id="4db07-539">The company name that is displayed to the users.</span></span>|
|<span data-ttu-id="4db07-540">defenderSecurityCenterHelpEmail</span><span class="sxs-lookup"><span data-stu-id="4db07-540">defenderSecurityCenterHelpEmail</span></span>|<span data-ttu-id="4db07-541">字符串</span><span class="sxs-lookup"><span data-stu-id="4db07-541">String</span></span>|<span data-ttu-id="4db07-542">向用户显示的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="4db07-542">The email address that is displayed to users.</span></span>|
|<span data-ttu-id="4db07-543">defenderSecurityCenterHelpPhone</span><span class="sxs-lookup"><span data-stu-id="4db07-543">defenderSecurityCenterHelpPhone</span></span>|<span data-ttu-id="4db07-544">字符串</span><span class="sxs-lookup"><span data-stu-id="4db07-544">String</span></span>|<span data-ttu-id="4db07-545">向用户显示的电话号码或 Skype ID。</span><span class="sxs-lookup"><span data-stu-id="4db07-545">The phone number or Skype ID that is displayed to users.</span></span>|
|<span data-ttu-id="4db07-546">defenderSecurityCenterHelpURL</span><span class="sxs-lookup"><span data-stu-id="4db07-546">defenderSecurityCenterHelpURL</span></span>|<span data-ttu-id="4db07-547">字符串</span><span class="sxs-lookup"><span data-stu-id="4db07-547">String</span></span>|<span data-ttu-id="4db07-548">"帮助" 门户 URL 将向用户显示。</span><span class="sxs-lookup"><span data-stu-id="4db07-548">The help portal URL this is displayed to users.</span></span>|
|<span data-ttu-id="4db07-549">defenderSecurityCenterNotificationsFromApp</span><span class="sxs-lookup"><span data-stu-id="4db07-549">defenderSecurityCenterNotificationsFromApp</span></span>|[<span data-ttu-id="4db07-550">defenderSecurityCenterNotificationsFromAppType</span><span class="sxs-lookup"><span data-stu-id="4db07-550">defenderSecurityCenterNotificationsFromAppType</span></span>](../resources/intune-deviceconfig-defendersecuritycenternotificationsfromapptype.md)|<span data-ttu-id="4db07-551">要从应用程序的显示区域中显示的通知。</span><span class="sxs-lookup"><span data-stu-id="4db07-551">Notifications to show from the displayed areas of app.</span></span> <span data-ttu-id="4db07-552">可取值为：`notConfigured`、`blockNoncriticalNotifications`、`blockAllNotifications`。</span><span class="sxs-lookup"><span data-stu-id="4db07-552">Possible values are: `notConfigured`, `blockNoncriticalNotifications`, `blockAllNotifications`.</span></span>|
|<span data-ttu-id="4db07-553">defenderSecurityCenterITContactDisplay</span><span class="sxs-lookup"><span data-stu-id="4db07-553">defenderSecurityCenterITContactDisplay</span></span>|[<span data-ttu-id="4db07-554">defenderSecurityCenterITContactDisplayType</span><span class="sxs-lookup"><span data-stu-id="4db07-554">defenderSecurityCenterITContactDisplayType</span></span>](../resources/intune-deviceconfig-defendersecuritycenteritcontactdisplaytype.md)|<span data-ttu-id="4db07-555">配置向最终用户显示 IT 联系人信息的位置。</span><span class="sxs-lookup"><span data-stu-id="4db07-555">Configure where to display IT contact information to end users.</span></span> <span data-ttu-id="4db07-556">可取值为：`notConfigured`、`displayInAppAndInNotifications`、`displayOnlyInApp`、`displayOnlyInNotifications`。</span><span class="sxs-lookup"><span data-stu-id="4db07-556">Possible values are: `notConfigured`, `displayInAppAndInNotifications`, `displayOnlyInApp`, `displayOnlyInNotifications`.</span></span>|
|<span data-ttu-id="4db07-557">windowsDefenderTamperProtection</span><span class="sxs-lookup"><span data-stu-id="4db07-557">windowsDefenderTamperProtection</span></span>|[<span data-ttu-id="4db07-558">windowsDefenderTamperProtectionOptions</span><span class="sxs-lookup"><span data-stu-id="4db07-558">windowsDefenderTamperProtectionOptions</span></span>](../resources/intune-deviceconfig-windowsdefendertamperprotectionoptions.md)|<span data-ttu-id="4db07-559">配置 windows defender TamperProtection 设置。</span><span class="sxs-lookup"><span data-stu-id="4db07-559">Configure windows defender TamperProtection settings.</span></span> <span data-ttu-id="4db07-560">可取值为：`notConfigured`、`enable`、`disable`。</span><span class="sxs-lookup"><span data-stu-id="4db07-560">Possible values are: `notConfigured`, `enable`, `disable`.</span></span>|
|<span data-ttu-id="4db07-561">firewallBlockStatefulFTP</span><span class="sxs-lookup"><span data-stu-id="4db07-561">firewallBlockStatefulFTP</span></span>|<span data-ttu-id="4db07-562">Boolean</span><span class="sxs-lookup"><span data-stu-id="4db07-562">Boolean</span></span>|<span data-ttu-id="4db07-563">阻止到设备的有状态 FTP 连接</span><span class="sxs-lookup"><span data-stu-id="4db07-563">Blocks stateful FTP connections to the device</span></span>|
|<span data-ttu-id="4db07-564">firewallIdleTimeoutForSecurityAssociationInSeconds</span><span class="sxs-lookup"><span data-stu-id="4db07-564">firewallIdleTimeoutForSecurityAssociationInSeconds</span></span>|<span data-ttu-id="4db07-565">Int32</span><span class="sxs-lookup"><span data-stu-id="4db07-565">Int32</span></span>|<span data-ttu-id="4db07-566">配置安全关联的空闲超时（以秒为单位），值范围为 300 到 3600（包括这两个值）。</span><span class="sxs-lookup"><span data-stu-id="4db07-566">Configures the idle timeout for security associations, in seconds, from 300 to 3600 inclusive.</span></span> <span data-ttu-id="4db07-567">这是一个时间段，在此之后安全关联将过期并被删除。</span><span class="sxs-lookup"><span data-stu-id="4db07-567">This is the period after which security associations will expire and be deleted.</span></span> <span data-ttu-id="4db07-568">有效值为 300 至 3600</span><span class="sxs-lookup"><span data-stu-id="4db07-568">Valid values 300 to 3600</span></span>|
|<span data-ttu-id="4db07-569">firewallPreSharedKeyEncodingMethod</span><span class="sxs-lookup"><span data-stu-id="4db07-569">firewallPreSharedKeyEncodingMethod</span></span>|[<span data-ttu-id="4db07-570">firewallPreSharedKeyEncodingMethodType</span><span class="sxs-lookup"><span data-stu-id="4db07-570">firewallPreSharedKeyEncodingMethodType</span></span>](../resources/intune-deviceconfig-firewallpresharedkeyencodingmethodtype.md)|<span data-ttu-id="4db07-571">选择要使用的预共享密钥编码。</span><span class="sxs-lookup"><span data-stu-id="4db07-571">Select the preshared key encoding to be used.</span></span> <span data-ttu-id="4db07-572">可取值为：`deviceDefault`、`none`、`utF8`。</span><span class="sxs-lookup"><span data-stu-id="4db07-572">Possible values are: `deviceDefault`, `none`, `utF8`.</span></span>|
|<span data-ttu-id="4db07-573">firewallIPSecExemptionsAllowNeighborDiscovery</span><span class="sxs-lookup"><span data-stu-id="4db07-573">firewallIPSecExemptionsAllowNeighborDiscovery</span></span>|<span data-ttu-id="4db07-574">Boolean</span><span class="sxs-lookup"><span data-stu-id="4db07-574">Boolean</span></span>|<span data-ttu-id="4db07-575">配置 IPSec 免除项以允许邻居发现 IPv6 ICMP 类型代码</span><span class="sxs-lookup"><span data-stu-id="4db07-575">Configures IPSec exemptions to allow neighbor discovery IPv6 ICMP type-codes</span></span>|
|<span data-ttu-id="4db07-576">firewallIPSecExemptionsAllowICMP</span><span class="sxs-lookup"><span data-stu-id="4db07-576">firewallIPSecExemptionsAllowICMP</span></span>|<span data-ttu-id="4db07-577">Boolean</span><span class="sxs-lookup"><span data-stu-id="4db07-577">Boolean</span></span>|<span data-ttu-id="4db07-578">配置 IPSec 免除项以允许 ICMP</span><span class="sxs-lookup"><span data-stu-id="4db07-578">Configures IPSec exemptions to allow ICMP</span></span>|
|<span data-ttu-id="4db07-579">firewallIPSecExemptionsAllowRouterDiscovery</span><span class="sxs-lookup"><span data-stu-id="4db07-579">firewallIPSecExemptionsAllowRouterDiscovery</span></span>|<span data-ttu-id="4db07-580">Boolean</span><span class="sxs-lookup"><span data-stu-id="4db07-580">Boolean</span></span>|<span data-ttu-id="4db07-581">配置 IPSec 免除项以允许路由器发现 IPv6 ICMP 类型代码</span><span class="sxs-lookup"><span data-stu-id="4db07-581">Configures IPSec exemptions to allow router discovery IPv6 ICMP type-codes</span></span>|
|<span data-ttu-id="4db07-582">firewallIPSecExemptionsAllowDHCP</span><span class="sxs-lookup"><span data-stu-id="4db07-582">firewallIPSecExemptionsAllowDHCP</span></span>|<span data-ttu-id="4db07-583">Boolean</span><span class="sxs-lookup"><span data-stu-id="4db07-583">Boolean</span></span>|<span data-ttu-id="4db07-584">配置 IPSec 免除项以允许 IPv4 和 IPv6 DHCP 通信</span><span class="sxs-lookup"><span data-stu-id="4db07-584">Configures IPSec exemptions to allow both IPv4 and IPv6 DHCP traffic</span></span>|
|<span data-ttu-id="4db07-585">firewallCertificateRevocationListCheckMethod</span><span class="sxs-lookup"><span data-stu-id="4db07-585">firewallCertificateRevocationListCheckMethod</span></span>|[<span data-ttu-id="4db07-586">firewallCertificateRevocationListCheckMethodType</span><span class="sxs-lookup"><span data-stu-id="4db07-586">firewallCertificateRevocationListCheckMethodType</span></span>](../resources/intune-deviceconfig-firewallcertificaterevocationlistcheckmethodtype.md)|<span data-ttu-id="4db07-587">指定如何强制执行证书吊销列表。</span><span class="sxs-lookup"><span data-stu-id="4db07-587">Specify how the certificate revocation list is to be enforced.</span></span> <span data-ttu-id="4db07-588">可取值为：`deviceDefault`、`none`、`attempt`、`require`。</span><span class="sxs-lookup"><span data-stu-id="4db07-588">Possible values are: `deviceDefault`, `none`, `attempt`, `require`.</span></span>|
|<span data-ttu-id="4db07-589">firewallMergeKeyingModuleSettings</span><span class="sxs-lookup"><span data-stu-id="4db07-589">firewallMergeKeyingModuleSettings</span></span>|<span data-ttu-id="4db07-590">Boolean</span><span class="sxs-lookup"><span data-stu-id="4db07-590">Boolean</span></span>|<span data-ttu-id="4db07-591">如果键控模块不完全支持身份验证集，请指示模块仅忽略不受支持的身份验证套件而不是整个集</span><span class="sxs-lookup"><span data-stu-id="4db07-591">If an authentication set is not fully supported by a keying module, direct the module to ignore only unsupported authentication suites rather than the entire set</span></span>|
|<span data-ttu-id="4db07-592">firewallPacketQueueingMethod</span><span class="sxs-lookup"><span data-stu-id="4db07-592">firewallPacketQueueingMethod</span></span>|[<span data-ttu-id="4db07-593">firewallPacketQueueingMethodType</span><span class="sxs-lookup"><span data-stu-id="4db07-593">firewallPacketQueueingMethodType</span></span>](../resources/intune-deviceconfig-firewallpacketqueueingmethodtype.md)|<span data-ttu-id="4db07-594">配置如何在隧道网关应用场景中应用数据包排队。</span><span class="sxs-lookup"><span data-stu-id="4db07-594">Configures how packet queueing should be applied in the tunnel gateway scenario.</span></span> <span data-ttu-id="4db07-595">可取值为：`deviceDefault`、`disabled`、`queueInbound`、`queueOutbound`、`queueBoth`。</span><span class="sxs-lookup"><span data-stu-id="4db07-595">Possible values are: `deviceDefault`, `disabled`, `queueInbound`, `queueOutbound`, `queueBoth`.</span></span>|
|<span data-ttu-id="4db07-596">firewallProfileDomain</span><span class="sxs-lookup"><span data-stu-id="4db07-596">firewallProfileDomain</span></span>|[<span data-ttu-id="4db07-597">windowsFirewallNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="4db07-597">windowsFirewallNetworkProfile</span></span>](../resources/intune-deviceconfig-windowsfirewallnetworkprofile.md)|<span data-ttu-id="4db07-598">配置域网络的防火墙配置文件设置</span><span class="sxs-lookup"><span data-stu-id="4db07-598">Configures the firewall profile settings for domain networks</span></span>|
|<span data-ttu-id="4db07-599">firewallProfilePublic</span><span class="sxs-lookup"><span data-stu-id="4db07-599">firewallProfilePublic</span></span>|[<span data-ttu-id="4db07-600">windowsFirewallNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="4db07-600">windowsFirewallNetworkProfile</span></span>](../resources/intune-deviceconfig-windowsfirewallnetworkprofile.md)|<span data-ttu-id="4db07-601">配置公用网络的防火墙配置文件设置</span><span class="sxs-lookup"><span data-stu-id="4db07-601">Configures the firewall profile settings for public networks</span></span>|
|<span data-ttu-id="4db07-602">firewallProfilePrivate</span><span class="sxs-lookup"><span data-stu-id="4db07-602">firewallProfilePrivate</span></span>|[<span data-ttu-id="4db07-603">windowsFirewallNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="4db07-603">windowsFirewallNetworkProfile</span></span>](../resources/intune-deviceconfig-windowsfirewallnetworkprofile.md)|<span data-ttu-id="4db07-604">配置专用网络的防火墙配置文件设置</span><span class="sxs-lookup"><span data-stu-id="4db07-604">Configures the firewall profile settings for private networks</span></span>|
|<span data-ttu-id="4db07-605">defenderAdobeReaderLaunchChildProcess</span><span class="sxs-lookup"><span data-stu-id="4db07-605">defenderAdobeReaderLaunchChildProcess</span></span>|[<span data-ttu-id="4db07-606">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="4db07-606">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="4db07-607">值，该值指示 Adobe Reader 创建子进程的行为。</span><span class="sxs-lookup"><span data-stu-id="4db07-607">Value indicating the behavior of Adobe Reader from creating child processes.</span></span> <span data-ttu-id="4db07-608">可取值为：`userDefined`、`enable`、`auditMode`。</span><span class="sxs-lookup"><span data-stu-id="4db07-608">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="4db07-609">defenderAttackSurfaceReductionExcludedPaths</span><span class="sxs-lookup"><span data-stu-id="4db07-609">defenderAttackSurfaceReductionExcludedPaths</span></span>|<span data-ttu-id="4db07-610">String 集合</span><span class="sxs-lookup"><span data-stu-id="4db07-610">String collection</span></span>|<span data-ttu-id="4db07-611">要从攻击面减少规则中排除的 exe 文件和文件夹的列表</span><span class="sxs-lookup"><span data-stu-id="4db07-611">List of exe files and folders to be excluded from attack surface reduction rules</span></span>|
|<span data-ttu-id="4db07-612">defenderOfficeAppsOtherProcessInjectionType</span><span class="sxs-lookup"><span data-stu-id="4db07-612">defenderOfficeAppsOtherProcessInjectionType</span></span>|[<span data-ttu-id="4db07-613">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="4db07-613">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="4db07-614">值，该值指示插入到其他进程中的 Office 应用程序的行为。</span><span class="sxs-lookup"><span data-stu-id="4db07-614">Value indicating the behavior of Office applications injecting into other processes.</span></span> <span data-ttu-id="4db07-615">可取值为：`userDefined`、`block`、`auditMode`。</span><span class="sxs-lookup"><span data-stu-id="4db07-615">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="4db07-616">defenderOfficeAppsOtherProcessInjection</span><span class="sxs-lookup"><span data-stu-id="4db07-616">defenderOfficeAppsOtherProcessInjection</span></span>|[<span data-ttu-id="4db07-617">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="4db07-617">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="4db07-618">值，该值指示插入到其他进程中的 Office 应用程序的行为。</span><span class="sxs-lookup"><span data-stu-id="4db07-618">Value indicating the behavior of  Office applications injecting into other processes.</span></span> <span data-ttu-id="4db07-619">可取值为：`userDefined`、`enable`、`auditMode`。</span><span class="sxs-lookup"><span data-stu-id="4db07-619">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="4db07-620">defenderOfficeCommunicationAppsLaunchChildProcess</span><span class="sxs-lookup"><span data-stu-id="4db07-620">defenderOfficeCommunicationAppsLaunchChildProcess</span></span>|[<span data-ttu-id="4db07-621">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="4db07-621">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="4db07-622">值，该值指示 Office 通信应用程序（包括 Microsoft Outlook）在创建子进程时的行为。</span><span class="sxs-lookup"><span data-stu-id="4db07-622">Value indicating the behavior of Office communication applications, including Microsoft Outlook, from creating child processes.</span></span> <span data-ttu-id="4db07-623">可取值为：`userDefined`、`enable`、`auditMode`。</span><span class="sxs-lookup"><span data-stu-id="4db07-623">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="4db07-624">defenderOfficeAppsExecutableContentCreationOrLaunchType</span><span class="sxs-lookup"><span data-stu-id="4db07-624">defenderOfficeAppsExecutableContentCreationOrLaunchType</span></span>|[<span data-ttu-id="4db07-625">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="4db07-625">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="4db07-626">值，该值指示 Office 应用程序/宏创建或启动可执行内容的行为。</span><span class="sxs-lookup"><span data-stu-id="4db07-626">Value indicating the behavior of Office applications/macros creating or launching executable content.</span></span> <span data-ttu-id="4db07-627">可取值为：`userDefined`、`block`、`auditMode`。</span><span class="sxs-lookup"><span data-stu-id="4db07-627">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="4db07-628">defenderOfficeAppsExecutableContentCreationOrLaunch</span><span class="sxs-lookup"><span data-stu-id="4db07-628">defenderOfficeAppsExecutableContentCreationOrLaunch</span></span>|[<span data-ttu-id="4db07-629">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="4db07-629">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="4db07-630">值，该值指示 Office 应用程序/宏创建或启动可执行内容的行为。</span><span class="sxs-lookup"><span data-stu-id="4db07-630">Value indicating the behavior of Office applications/macros creating or launching executable content.</span></span> <span data-ttu-id="4db07-631">可取值为：`userDefined`、`enable`、`auditMode`。</span><span class="sxs-lookup"><span data-stu-id="4db07-631">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="4db07-632">defenderOfficeAppsLaunchChildProcessType</span><span class="sxs-lookup"><span data-stu-id="4db07-632">defenderOfficeAppsLaunchChildProcessType</span></span>|[<span data-ttu-id="4db07-633">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="4db07-633">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="4db07-634">值，该值指示 Office 应用程序启动子进程的行为。</span><span class="sxs-lookup"><span data-stu-id="4db07-634">Value indicating the behavior of Office application launching child processes.</span></span> <span data-ttu-id="4db07-635">可取值为：`userDefined`、`block`、`auditMode`。</span><span class="sxs-lookup"><span data-stu-id="4db07-635">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="4db07-636">defenderOfficeAppsLaunchChildProcess</span><span class="sxs-lookup"><span data-stu-id="4db07-636">defenderOfficeAppsLaunchChildProcess</span></span>|[<span data-ttu-id="4db07-637">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="4db07-637">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="4db07-638">值，该值指示 Office 应用程序启动子进程的行为。</span><span class="sxs-lookup"><span data-stu-id="4db07-638">Value indicating the behavior of Office application launching child processes.</span></span> <span data-ttu-id="4db07-639">可取值为：`userDefined`、`enable`、`auditMode`。</span><span class="sxs-lookup"><span data-stu-id="4db07-639">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="4db07-640">defenderOfficeMacroCodeAllowWin32ImportsType</span><span class="sxs-lookup"><span data-stu-id="4db07-640">defenderOfficeMacroCodeAllowWin32ImportsType</span></span>|[<span data-ttu-id="4db07-641">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="4db07-641">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="4db07-642">值，该值指示从 Office 中的宏代码的 Win32 导入行为。</span><span class="sxs-lookup"><span data-stu-id="4db07-642">Value indicating the behavior of Win32 imports from Macro code in Office.</span></span> <span data-ttu-id="4db07-643">可取值为：`userDefined`、`block`、`auditMode`。</span><span class="sxs-lookup"><span data-stu-id="4db07-643">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="4db07-644">defenderOfficeMacroCodeAllowWin32Imports</span><span class="sxs-lookup"><span data-stu-id="4db07-644">defenderOfficeMacroCodeAllowWin32Imports</span></span>|[<span data-ttu-id="4db07-645">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="4db07-645">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="4db07-646">值，该值指示从 Office 中的宏代码的 Win32 导入行为。</span><span class="sxs-lookup"><span data-stu-id="4db07-646">Value indicating the behavior of Win32 imports from Macro code in Office.</span></span> <span data-ttu-id="4db07-647">可取值为：`userDefined`、`enable`、`auditMode`。</span><span class="sxs-lookup"><span data-stu-id="4db07-647">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="4db07-648">defenderScriptObfuscatedMacroCodeType</span><span class="sxs-lookup"><span data-stu-id="4db07-648">defenderScriptObfuscatedMacroCodeType</span></span>|[<span data-ttu-id="4db07-649">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="4db07-649">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="4db07-650">值，该值指示模糊的 js/vbs/ps/宏代码的行为。</span><span class="sxs-lookup"><span data-stu-id="4db07-650">Value indicating the behavior of obfuscated js/vbs/ps/macro code.</span></span> <span data-ttu-id="4db07-651">可取值为：`userDefined`、`block`、`auditMode`。</span><span class="sxs-lookup"><span data-stu-id="4db07-651">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="4db07-652">defenderScriptObfuscatedMacroCode</span><span class="sxs-lookup"><span data-stu-id="4db07-652">defenderScriptObfuscatedMacroCode</span></span>|[<span data-ttu-id="4db07-653">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="4db07-653">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="4db07-654">值，该值指示模糊的 js/vbs/ps/宏代码的行为。</span><span class="sxs-lookup"><span data-stu-id="4db07-654">Value indicating the behavior of obfuscated js/vbs/ps/macro code.</span></span> <span data-ttu-id="4db07-655">可取值为：`userDefined`、`enable`、`auditMode`。</span><span class="sxs-lookup"><span data-stu-id="4db07-655">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="4db07-656">defenderScriptDownloadedPayloadExecutionType</span><span class="sxs-lookup"><span data-stu-id="4db07-656">defenderScriptDownloadedPayloadExecutionType</span></span>|[<span data-ttu-id="4db07-657">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="4db07-657">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="4db07-658">值，该值指示从 Internet 下载的 js/vbs 执行负载的行为。</span><span class="sxs-lookup"><span data-stu-id="4db07-658">Value indicating the behavior of js/vbs executing payload downloaded from Internet.</span></span> <span data-ttu-id="4db07-659">可取值为：`userDefined`、`block`、`auditMode`。</span><span class="sxs-lookup"><span data-stu-id="4db07-659">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="4db07-660">defenderScriptDownloadedPayloadExecution</span><span class="sxs-lookup"><span data-stu-id="4db07-660">defenderScriptDownloadedPayloadExecution</span></span>|[<span data-ttu-id="4db07-661">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="4db07-661">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="4db07-662">值，该值指示从 Internet 下载的 js/vbs 执行负载的行为。</span><span class="sxs-lookup"><span data-stu-id="4db07-662">Value indicating the behavior of js/vbs executing payload downloaded from Internet.</span></span> <span data-ttu-id="4db07-663">可取值为：`userDefined`、`enable`、`auditMode`。</span><span class="sxs-lookup"><span data-stu-id="4db07-663">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="4db07-664">defenderPreventCredentialStealingType</span><span class="sxs-lookup"><span data-stu-id="4db07-664">defenderPreventCredentialStealingType</span></span>|[<span data-ttu-id="4db07-665">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="4db07-665">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="4db07-666">值，该值指示是否允许从 Windows 本地安全机构子系统中盗取凭据。</span><span class="sxs-lookup"><span data-stu-id="4db07-666">Value indicating if credential stealing from the Windows local security authority subsystem is permitted.</span></span> <span data-ttu-id="4db07-667">可取值为：`userDefined`、`enable`、`auditMode`。</span><span class="sxs-lookup"><span data-stu-id="4db07-667">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="4db07-668">defenderProcessCreationType</span><span class="sxs-lookup"><span data-stu-id="4db07-668">defenderProcessCreationType</span></span>|[<span data-ttu-id="4db07-669">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="4db07-669">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="4db07-670">一个值，该值指示对源自 PSExec 和 WMI 命令的进程创建的响应。</span><span class="sxs-lookup"><span data-stu-id="4db07-670">Value indicating response to process creations originating from PSExec and WMI commands.</span></span> <span data-ttu-id="4db07-671">可取值为：`userDefined`、`block`、`auditMode`。</span><span class="sxs-lookup"><span data-stu-id="4db07-671">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="4db07-672">defenderProcessCreation</span><span class="sxs-lookup"><span data-stu-id="4db07-672">defenderProcessCreation</span></span>|[<span data-ttu-id="4db07-673">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="4db07-673">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="4db07-674">一个值，该值指示对源自 PSExec 和 WMI 命令的进程创建的响应。</span><span class="sxs-lookup"><span data-stu-id="4db07-674">Value indicating response to process creations originating from PSExec and WMI commands.</span></span> <span data-ttu-id="4db07-675">可取值为：`userDefined`、`enable`、`auditMode`。</span><span class="sxs-lookup"><span data-stu-id="4db07-675">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="4db07-676">defenderUntrustedUSBProcessType</span><span class="sxs-lookup"><span data-stu-id="4db07-676">defenderUntrustedUSBProcessType</span></span>|[<span data-ttu-id="4db07-677">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="4db07-677">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="4db07-678">指示对从 USB 运行的不受信任和未签名进程的响应的值。</span><span class="sxs-lookup"><span data-stu-id="4db07-678">Value indicating response to untrusted and unsigned processes that run from USB.</span></span> <span data-ttu-id="4db07-679">可取值为：`userDefined`、`block`、`auditMode`。</span><span class="sxs-lookup"><span data-stu-id="4db07-679">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="4db07-680">defenderUntrustedUSBProcess</span><span class="sxs-lookup"><span data-stu-id="4db07-680">defenderUntrustedUSBProcess</span></span>|[<span data-ttu-id="4db07-681">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="4db07-681">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="4db07-682">指示对从 USB 运行的不受信任和未签名进程的响应的值。</span><span class="sxs-lookup"><span data-stu-id="4db07-682">Value indicating response to untrusted and unsigned processes that run from USB.</span></span> <span data-ttu-id="4db07-683">可取值为：`userDefined`、`enable`、`auditMode`。</span><span class="sxs-lookup"><span data-stu-id="4db07-683">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="4db07-684">defenderUntrustedExecutableType</span><span class="sxs-lookup"><span data-stu-id="4db07-684">defenderUntrustedExecutableType</span></span>|[<span data-ttu-id="4db07-685">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="4db07-685">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="4db07-686">指示对不符合流行、年龄或受信任列表条件的可执行文件的响应的值。</span><span class="sxs-lookup"><span data-stu-id="4db07-686">Value indicating response to executables that don't meet a prevalence, age, or trusted list criteria.</span></span> <span data-ttu-id="4db07-687">可取值为：`userDefined`、`block`、`auditMode`。</span><span class="sxs-lookup"><span data-stu-id="4db07-687">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="4db07-688">defenderUntrustedExecutable</span><span class="sxs-lookup"><span data-stu-id="4db07-688">defenderUntrustedExecutable</span></span>|[<span data-ttu-id="4db07-689">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="4db07-689">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="4db07-690">指示对不符合流行、年龄或受信任列表条件的可执行文件的响应的值。</span><span class="sxs-lookup"><span data-stu-id="4db07-690">Value indicating response to executables that don't meet a prevalence, age, or trusted list criteria.</span></span> <span data-ttu-id="4db07-691">可取值为：`userDefined`、`enable`、`auditMode`。</span><span class="sxs-lookup"><span data-stu-id="4db07-691">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="4db07-692">defenderEmailContentExecutionType</span><span class="sxs-lookup"><span data-stu-id="4db07-692">defenderEmailContentExecutionType</span></span>|[<span data-ttu-id="4db07-693">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="4db07-693">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="4db07-694">一个值，该值指示是否应从电子邮件（web 邮件/邮件客户端）中删除可执行内容（exe、dll、ps、js、vbs 等）的执行。</span><span class="sxs-lookup"><span data-stu-id="4db07-694">Value indicating if execution of executable content (exe, dll, ps, js, vbs, etc) should be dropped from email (webmail/mail-client).</span></span> <span data-ttu-id="4db07-695">可取值为：`userDefined`、`block`、`auditMode`。</span><span class="sxs-lookup"><span data-stu-id="4db07-695">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="4db07-696">defenderEmailContentExecution</span><span class="sxs-lookup"><span data-stu-id="4db07-696">defenderEmailContentExecution</span></span>|[<span data-ttu-id="4db07-697">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="4db07-697">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="4db07-698">一个值，该值指示是否应从电子邮件（web 邮件/邮件客户端）中删除可执行内容（exe、dll、ps、js、vbs 等）的执行。</span><span class="sxs-lookup"><span data-stu-id="4db07-698">Value indicating if execution of executable content (exe, dll, ps, js, vbs, etc) should be dropped from email (webmail/mail-client).</span></span> <span data-ttu-id="4db07-699">可取值为：`userDefined`、`enable`、`auditMode`。</span><span class="sxs-lookup"><span data-stu-id="4db07-699">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="4db07-700">defenderAdvancedRansomewareProtectionType</span><span class="sxs-lookup"><span data-stu-id="4db07-700">defenderAdvancedRansomewareProtectionType</span></span>|[<span data-ttu-id="4db07-701">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="4db07-701">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="4db07-702">指示使用针对 ransomeware 的高级防护的值。</span><span class="sxs-lookup"><span data-stu-id="4db07-702">Value indicating use of advanced protection against ransomeware.</span></span> <span data-ttu-id="4db07-703">可取值为：`userDefined`、`enable`、`auditMode`。</span><span class="sxs-lookup"><span data-stu-id="4db07-703">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="4db07-704">defenderGuardMyFoldersType</span><span class="sxs-lookup"><span data-stu-id="4db07-704">defenderGuardMyFoldersType</span></span>|[<span data-ttu-id="4db07-705">folderProtectionType</span><span class="sxs-lookup"><span data-stu-id="4db07-705">folderProtectionType</span></span>](../resources/intune-deviceconfig-folderprotectiontype.md)|<span data-ttu-id="4db07-706">值，该值指示受保护文件夹的行为。</span><span class="sxs-lookup"><span data-stu-id="4db07-706">Value indicating the behavior of protected folders.</span></span> <span data-ttu-id="4db07-707">可取值为：`userDefined`、`enable`、`auditMode`、`blockDiskModification`、`auditDiskModification`。</span><span class="sxs-lookup"><span data-stu-id="4db07-707">Possible values are: `userDefined`, `enable`, `auditMode`, `blockDiskModification`, `auditDiskModification`.</span></span>|
|<span data-ttu-id="4db07-708">defenderGuardedFoldersAllowedAppPaths</span><span class="sxs-lookup"><span data-stu-id="4db07-708">defenderGuardedFoldersAllowedAppPaths</span></span>|<span data-ttu-id="4db07-709">String collection</span><span class="sxs-lookup"><span data-stu-id="4db07-709">String collection</span></span>|<span data-ttu-id="4db07-710">允许访问受保护文件夹的 exe 路径列表</span><span class="sxs-lookup"><span data-stu-id="4db07-710">List of paths to exe that are allowed to access protected folders</span></span>|
|<span data-ttu-id="4db07-711">defenderAdditionalGuardedFolders</span><span class="sxs-lookup"><span data-stu-id="4db07-711">defenderAdditionalGuardedFolders</span></span>|<span data-ttu-id="4db07-712">String 集合</span><span class="sxs-lookup"><span data-stu-id="4db07-712">String collection</span></span>|<span data-ttu-id="4db07-713">要添加到受保护文件夹列表的文件夹路径列表</span><span class="sxs-lookup"><span data-stu-id="4db07-713">List of folder paths to be added to the list of protected folders</span></span>|
|<span data-ttu-id="4db07-714">defenderNetworkProtectionType</span><span class="sxs-lookup"><span data-stu-id="4db07-714">defenderNetworkProtectionType</span></span>|[<span data-ttu-id="4db07-715">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="4db07-715">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="4db07-716">值，该值指示 NetworkProtection 的行为。</span><span class="sxs-lookup"><span data-stu-id="4db07-716">Value indicating the behavior of NetworkProtection.</span></span> <span data-ttu-id="4db07-717">可取值为：`userDefined`、`enable`、`auditMode`。</span><span class="sxs-lookup"><span data-stu-id="4db07-717">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="4db07-718">defenderExploitProtectionXml</span><span class="sxs-lookup"><span data-stu-id="4db07-718">defenderExploitProtectionXml</span></span>|<span data-ttu-id="4db07-719">Binary</span><span class="sxs-lookup"><span data-stu-id="4db07-719">Binary</span></span>|<span data-ttu-id="4db07-720">包含有关 Exploit Protection 详细信息的 xml 内容。</span><span class="sxs-lookup"><span data-stu-id="4db07-720">Xml content containing information regarding exploit protection details.</span></span>|
|<span data-ttu-id="4db07-721">defenderExploitProtectionXmlFileName</span><span class="sxs-lookup"><span data-stu-id="4db07-721">defenderExploitProtectionXmlFileName</span></span>|<span data-ttu-id="4db07-722">String</span><span class="sxs-lookup"><span data-stu-id="4db07-722">String</span></span>|<span data-ttu-id="4db07-723">从中获取 DefenderExploitProtectionXml 的文件的名称。</span><span class="sxs-lookup"><span data-stu-id="4db07-723">Name of the file from which DefenderExploitProtectionXml was obtained.</span></span>|
|<span data-ttu-id="4db07-724">defenderSecurityCenterBlockExploitProtectionOverride</span><span class="sxs-lookup"><span data-stu-id="4db07-724">defenderSecurityCenterBlockExploitProtectionOverride</span></span>|<span data-ttu-id="4db07-725">Boolean</span><span class="sxs-lookup"><span data-stu-id="4db07-725">Boolean</span></span>|<span data-ttu-id="4db07-726">指示是否阻止用户覆盖 Exploit Protection 设置。</span><span class="sxs-lookup"><span data-stu-id="4db07-726">Indicates whether or not to block user from overriding Exploit Protection settings.</span></span>|
|<span data-ttu-id="4db07-727">appLockerApplicationControl</span><span class="sxs-lookup"><span data-stu-id="4db07-727">appLockerApplicationControl</span></span>|[<span data-ttu-id="4db07-728">appLockerApplicationControlType</span><span class="sxs-lookup"><span data-stu-id="4db07-728">appLockerApplicationControlType</span></span>](../resources/intune-deviceconfig-applockerapplicationcontroltype.md)|<span data-ttu-id="4db07-729">使管理员能够选择在设备上允许哪些类型的应用。</span><span class="sxs-lookup"><span data-stu-id="4db07-729">Enables the Admin to choose what types of app to allow on devices.</span></span> <span data-ttu-id="4db07-730">可取值为：`notConfigured`、`enforceComponentsAndStoreApps`、`auditComponentsAndStoreApps`、`enforceComponentsStoreAppsAndSmartlocker`、`auditComponentsStoreAppsAndSmartlocker`。</span><span class="sxs-lookup"><span data-stu-id="4db07-730">Possible values are: `notConfigured`, `enforceComponentsAndStoreApps`, `auditComponentsAndStoreApps`, `enforceComponentsStoreAppsAndSmartlocker`, `auditComponentsStoreAppsAndSmartlocker`.</span></span>|
|<span data-ttu-id="4db07-731">deviceGuardLocalSystemAuthorityCredentialGuardSettings</span><span class="sxs-lookup"><span data-stu-id="4db07-731">deviceGuardLocalSystemAuthorityCredentialGuardSettings</span></span>|[<span data-ttu-id="4db07-732">deviceGuardLocalSystemAuthorityCredentialGuardType</span><span class="sxs-lookup"><span data-stu-id="4db07-732">deviceGuardLocalSystemAuthorityCredentialGuardType</span></span>](../resources/intune-deviceconfig-deviceguardlocalsystemauthoritycredentialguardtype.md)|<span data-ttu-id="4db07-733">如果平台安全级别具有安全启动和基于虚拟化的安全性均已启用，则打开 Credential Guard。</span><span class="sxs-lookup"><span data-stu-id="4db07-733">Turn on Credential Guard when Platform Security Level with Secure Boot and Virtualization Based Security are both enabled.</span></span> <span data-ttu-id="4db07-734">可取值为：`notConfigured`、`enableWithUEFILock`、`enableWithoutUEFILock`。</span><span class="sxs-lookup"><span data-stu-id="4db07-734">Possible values are: `notConfigured`, `enableWithUEFILock`, `enableWithoutUEFILock`.</span></span>|
|<span data-ttu-id="4db07-735">deviceGuardEnableVirtualizationBasedSecurity</span><span class="sxs-lookup"><span data-stu-id="4db07-735">deviceGuardEnableVirtualizationBasedSecurity</span></span>|<span data-ttu-id="4db07-736">Boolean</span><span class="sxs-lookup"><span data-stu-id="4db07-736">Boolean</span></span>|<span data-ttu-id="4db07-737">启用基于虚拟化的安全性（VBS）。</span><span class="sxs-lookup"><span data-stu-id="4db07-737">Turns On Virtualization Based Security(VBS).</span></span>|
|<span data-ttu-id="4db07-738">deviceGuardEnableSecureBootWithDMA</span><span class="sxs-lookup"><span data-stu-id="4db07-738">deviceGuardEnableSecureBootWithDMA</span></span>|<span data-ttu-id="4db07-739">Boolean</span><span class="sxs-lookup"><span data-stu-id="4db07-739">Boolean</span></span>|<span data-ttu-id="4db07-740">此属性将在5月2019中被弃用，并将替换为属性 DeviceGuardSecureBootWithDMA。</span><span class="sxs-lookup"><span data-stu-id="4db07-740">This property will be deprecated in May 2019 and will be replaced with property DeviceGuardSecureBootWithDMA.</span></span> <span data-ttu-id="4db07-741">指定是否在下次重新启动时启用平台安全级别。</span><span class="sxs-lookup"><span data-stu-id="4db07-741">Specifies whether Platform Security Level is enabled at next reboot.</span></span>|
|<span data-ttu-id="4db07-742">deviceGuardSecureBootWithDMA</span><span class="sxs-lookup"><span data-stu-id="4db07-742">deviceGuardSecureBootWithDMA</span></span>|[<span data-ttu-id="4db07-743">secureBootWithDMAType</span><span class="sxs-lookup"><span data-stu-id="4db07-743">secureBootWithDMAType</span></span>](../resources/intune-deviceconfig-securebootwithdmatype.md)|<span data-ttu-id="4db07-744">指定是否在下次重新启动时启用平台安全级别。</span><span class="sxs-lookup"><span data-stu-id="4db07-744">Specifies whether Platform Security Level is enabled at next reboot.</span></span> <span data-ttu-id="4db07-745">可取值为：`notConfigured`、`withoutDMA`、`withDMA`。</span><span class="sxs-lookup"><span data-stu-id="4db07-745">Possible values are: `notConfigured`, `withoutDMA`, `withDMA`.</span></span>|
|<span data-ttu-id="4db07-746">deviceGuardLaunchSystemGuard</span><span class="sxs-lookup"><span data-stu-id="4db07-746">deviceGuardLaunchSystemGuard</span></span>|[<span data-ttu-id="4db07-747">启用</span><span class="sxs-lookup"><span data-stu-id="4db07-747">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="4db07-748">允许 IT 管理员配置启动 "系统防护"。</span><span class="sxs-lookup"><span data-stu-id="4db07-748">Allows the IT admin to configure the launch of System Guard.</span></span> <span data-ttu-id="4db07-749">可取值为：`notConfigured`、`enabled`、`disabled`。</span><span class="sxs-lookup"><span data-stu-id="4db07-749">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="4db07-750">smartScreenEnableInShell</span><span class="sxs-lookup"><span data-stu-id="4db07-750">smartScreenEnableInShell</span></span>|<span data-ttu-id="4db07-751">Boolean</span><span class="sxs-lookup"><span data-stu-id="4db07-751">Boolean</span></span>|<span data-ttu-id="4db07-752">允许 IT 管理员配置适用于 Windows 的 SmartScreen。</span><span class="sxs-lookup"><span data-stu-id="4db07-752">Allows IT Admins to configure SmartScreen for Windows.</span></span>|
|<span data-ttu-id="4db07-753">smartScreenBlockOverrideForFiles</span><span class="sxs-lookup"><span data-stu-id="4db07-753">smartScreenBlockOverrideForFiles</span></span>|<span data-ttu-id="4db07-754">Boolean</span><span class="sxs-lookup"><span data-stu-id="4db07-754">Boolean</span></span>|<span data-ttu-id="4db07-755">允许 IT 管理员控制用户是否可以忽略 SmartScreen 警告并运行恶意文件。</span><span class="sxs-lookup"><span data-stu-id="4db07-755">Allows IT Admins to control whether users can can ignore SmartScreen warnings and run malicious files.</span></span>|
|<span data-ttu-id="4db07-756">applicationGuardEnabled</span><span class="sxs-lookup"><span data-stu-id="4db07-756">applicationGuardEnabled</span></span>|<span data-ttu-id="4db07-757">Boolean</span><span class="sxs-lookup"><span data-stu-id="4db07-757">Boolean</span></span>|<span data-ttu-id="4db07-758">启用 Windows Defender 应用程序防护</span><span class="sxs-lookup"><span data-stu-id="4db07-758">Enable Windows Defender Application Guard</span></span>|
|<span data-ttu-id="4db07-759">applicationGuardEnabledOptions</span><span class="sxs-lookup"><span data-stu-id="4db07-759">applicationGuardEnabledOptions</span></span>|[<span data-ttu-id="4db07-760">applicationGuardEnabledOptions</span><span class="sxs-lookup"><span data-stu-id="4db07-760">applicationGuardEnabledOptions</span></span>](../resources/intune-deviceconfig-applicationguardenabledoptions.md)|<span data-ttu-id="4db07-761">为较新的 Windows 版本启用 Windows Defender 应用程序防护。</span><span class="sxs-lookup"><span data-stu-id="4db07-761">Enable Windows Defender Application Guard for newer Windows builds.</span></span> <span data-ttu-id="4db07-762">可取值为：`notConfigured`、`enabledForEdge`、`enabledForOffice`、`enabledForEdgeAndOffice`。</span><span class="sxs-lookup"><span data-stu-id="4db07-762">Possible values are: `notConfigured`, `enabledForEdge`, `enabledForOffice`, `enabledForEdgeAndOffice`.</span></span>|
|<span data-ttu-id="4db07-763">applicationGuardBlockFileTransfer</span><span class="sxs-lookup"><span data-stu-id="4db07-763">applicationGuardBlockFileTransfer</span></span>|[<span data-ttu-id="4db07-764">applicationGuardBlockFileTransferType</span><span class="sxs-lookup"><span data-stu-id="4db07-764">applicationGuardBlockFileTransferType</span></span>](../resources/intune-deviceconfig-applicationguardblockfiletransfertype.md)|<span data-ttu-id="4db07-765">阻止剪贴板传输图像文件、文本文件或二者都不。</span><span class="sxs-lookup"><span data-stu-id="4db07-765">Block clipboard to transfer image file, text file or neither of them.</span></span> <span data-ttu-id="4db07-766">可取值为：`notConfigured`、`blockImageAndTextFile`、`blockImageFile`、`blockNone`、`blockTextFile`。</span><span class="sxs-lookup"><span data-stu-id="4db07-766">Possible values are: `notConfigured`, `blockImageAndTextFile`, `blockImageFile`, `blockNone`, `blockTextFile`.</span></span>|
|<span data-ttu-id="4db07-767">applicationGuardBlockNonEnterpriseContent</span><span class="sxs-lookup"><span data-stu-id="4db07-767">applicationGuardBlockNonEnterpriseContent</span></span>|<span data-ttu-id="4db07-768">Boolean</span><span class="sxs-lookup"><span data-stu-id="4db07-768">Boolean</span></span>|<span data-ttu-id="4db07-769">阻止企业站点加载非企业内容，例如第三方插件</span><span class="sxs-lookup"><span data-stu-id="4db07-769">Block enterprise sites to load non-enterprise content, such as third party plug-ins</span></span>|
|<span data-ttu-id="4db07-770">applicationGuardAllowPersistence</span><span class="sxs-lookup"><span data-stu-id="4db07-770">applicationGuardAllowPersistence</span></span>|<span data-ttu-id="4db07-771">Boolean</span><span class="sxs-lookup"><span data-stu-id="4db07-771">Boolean</span></span>|<span data-ttu-id="4db07-772">允许 App Guard 容器（收藏夹、Cookie、Web 密码等）内的持久用户生成数据</span><span class="sxs-lookup"><span data-stu-id="4db07-772">Allow persisting user generated data inside the App Guard Containter (favorites, cookies, web passwords, etc.)</span></span>|
|<span data-ttu-id="4db07-773">applicationGuardForceAuditing</span><span class="sxs-lookup"><span data-stu-id="4db07-773">applicationGuardForceAuditing</span></span>|<span data-ttu-id="4db07-774">Boolean</span><span class="sxs-lookup"><span data-stu-id="4db07-774">Boolean</span></span>|<span data-ttu-id="4db07-775">强制审核将存留 Windows 日志和事件以满足安全/符合性条件（示例事件是用户登录注销、特权使用、软件安装、系统更改等）</span><span class="sxs-lookup"><span data-stu-id="4db07-775">Force auditing will persist Windows logs and events to meet security/compliance criteria (sample events are user login-logoff, use of privilege rights, software installation, system changes, etc.)</span></span>|
|<span data-ttu-id="4db07-776">applicationGuardBlockClipboardSharing</span><span class="sxs-lookup"><span data-stu-id="4db07-776">applicationGuardBlockClipboardSharing</span></span>|[<span data-ttu-id="4db07-777">applicationGuardBlockClipboardSharingType</span><span class="sxs-lookup"><span data-stu-id="4db07-777">applicationGuardBlockClipboardSharingType</span></span>](../resources/intune-deviceconfig-applicationguardblockclipboardsharingtype.md)|<span data-ttu-id="4db07-778">阻止剪贴板将数据从主机共享到容器或从容器共享到主机，或阻止两种方式，或两种方式均不阻止。</span><span class="sxs-lookup"><span data-stu-id="4db07-778">Block clipboard to share data from Host to Container, or from Container to Host, or both ways, or neither ways.</span></span> <span data-ttu-id="4db07-779">可取值为：`notConfigured`、`blockBoth`、`blockHostToContainer`、`blockContainerToHost`、`blockNone`。</span><span class="sxs-lookup"><span data-stu-id="4db07-779">Possible values are: `notConfigured`, `blockBoth`, `blockHostToContainer`, `blockContainerToHost`, `blockNone`.</span></span>|
|<span data-ttu-id="4db07-780">applicationGuardAllowPrintToPDF</span><span class="sxs-lookup"><span data-stu-id="4db07-780">applicationGuardAllowPrintToPDF</span></span>|<span data-ttu-id="4db07-781">Boolean</span><span class="sxs-lookup"><span data-stu-id="4db07-781">Boolean</span></span>|<span data-ttu-id="4db07-782">允许从容器打印为 PDF 格式</span><span class="sxs-lookup"><span data-stu-id="4db07-782">Allow printing to PDF from Container</span></span>|
|<span data-ttu-id="4db07-783">applicationGuardAllowPrintToXPS</span><span class="sxs-lookup"><span data-stu-id="4db07-783">applicationGuardAllowPrintToXPS</span></span>|<span data-ttu-id="4db07-784">Boolean</span><span class="sxs-lookup"><span data-stu-id="4db07-784">Boolean</span></span>|<span data-ttu-id="4db07-785">允许从容器打印为 XPS 格式</span><span class="sxs-lookup"><span data-stu-id="4db07-785">Allow printing to XPS from Container</span></span>|
|<span data-ttu-id="4db07-786">applicationGuardAllowPrintToLocalPrinters</span><span class="sxs-lookup"><span data-stu-id="4db07-786">applicationGuardAllowPrintToLocalPrinters</span></span>|<span data-ttu-id="4db07-787">Boolean</span><span class="sxs-lookup"><span data-stu-id="4db07-787">Boolean</span></span>|<span data-ttu-id="4db07-788">允许从容器打印到本地打印机</span><span class="sxs-lookup"><span data-stu-id="4db07-788">Allow printing to Local Printers from Container</span></span>|
|<span data-ttu-id="4db07-789">applicationGuardAllowPrintToNetworkPrinters</span><span class="sxs-lookup"><span data-stu-id="4db07-789">applicationGuardAllowPrintToNetworkPrinters</span></span>|<span data-ttu-id="4db07-790">Boolean</span><span class="sxs-lookup"><span data-stu-id="4db07-790">Boolean</span></span>|<span data-ttu-id="4db07-791">允许从容器打印到网络打印机</span><span class="sxs-lookup"><span data-stu-id="4db07-791">Allow printing to Network Printers from Container</span></span>|
|<span data-ttu-id="4db07-792">applicationGuardAllowVirtualGPU</span><span class="sxs-lookup"><span data-stu-id="4db07-792">applicationGuardAllowVirtualGPU</span></span>|<span data-ttu-id="4db07-793">Boolean</span><span class="sxs-lookup"><span data-stu-id="4db07-793">Boolean</span></span>|<span data-ttu-id="4db07-794">允许应用程序防护使用虚拟 GPU</span><span class="sxs-lookup"><span data-stu-id="4db07-794">Allow application guard to use virtual GPU</span></span>|
|<span data-ttu-id="4db07-795">applicationGuardAllowFileSaveOnHost</span><span class="sxs-lookup"><span data-stu-id="4db07-795">applicationGuardAllowFileSaveOnHost</span></span>|<span data-ttu-id="4db07-796">Boolean</span><span class="sxs-lookup"><span data-stu-id="4db07-796">Boolean</span></span>|<span data-ttu-id="4db07-797">允许用户从应用程序防护容器中的边缘下载文件并将其保存在主机文件系统上</span><span class="sxs-lookup"><span data-stu-id="4db07-797">Allow users to download files from Edge in the application guard container and save them on the host file system</span></span>|
|<span data-ttu-id="4db07-798">bitLockerAllowStandardUserEncryption</span><span class="sxs-lookup"><span data-stu-id="4db07-798">bitLockerAllowStandardUserEncryption</span></span>|<span data-ttu-id="4db07-799">Boolean</span><span class="sxs-lookup"><span data-stu-id="4db07-799">Boolean</span></span>|<span data-ttu-id="4db07-800">允许管理员允许标准用户在 Azure AD 加入过程中启用 encrpytion。</span><span class="sxs-lookup"><span data-stu-id="4db07-800">Allows the admin to allow standard users to enable encrpytion during Azure AD Join.</span></span>|
|<span data-ttu-id="4db07-801">bitLockerDisableWarningForOtherDiskEncryption</span><span class="sxs-lookup"><span data-stu-id="4db07-801">bitLockerDisableWarningForOtherDiskEncryption</span></span>|<span data-ttu-id="4db07-802">Boolean</span><span class="sxs-lookup"><span data-stu-id="4db07-802">Boolean</span></span>|<span data-ttu-id="4db07-803">允许管理员禁用对用户计算机上其他磁盘加密的警告提示。</span><span class="sxs-lookup"><span data-stu-id="4db07-803">Allows the Admin to disable the warning prompt for other disk encryption on the user machines.</span></span>|
|<span data-ttu-id="4db07-804">bitLockerEnableStorageCardEncryptionOnMobile</span><span class="sxs-lookup"><span data-stu-id="4db07-804">bitLockerEnableStorageCardEncryptionOnMobile</span></span>|<span data-ttu-id="4db07-805">Boolean</span><span class="sxs-lookup"><span data-stu-id="4db07-805">Boolean</span></span>|<span data-ttu-id="4db07-806">允许管理员要求使用 BitLocker 开启加密功能。</span><span class="sxs-lookup"><span data-stu-id="4db07-806">Allows the admin to require encryption to be turned on using BitLocker.</span></span> <span data-ttu-id="4db07-807">此策略仅适用于移动 SKU。</span><span class="sxs-lookup"><span data-stu-id="4db07-807">This policy is valid only for a mobile SKU.</span></span>|
|<span data-ttu-id="4db07-808">bitLockerEncryptDevice</span><span class="sxs-lookup"><span data-stu-id="4db07-808">bitLockerEncryptDevice</span></span>|<span data-ttu-id="4db07-809">Boolean</span><span class="sxs-lookup"><span data-stu-id="4db07-809">Boolean</span></span>|<span data-ttu-id="4db07-810">允许管理员要求使用 BitLocker 开启加密功能。</span><span class="sxs-lookup"><span data-stu-id="4db07-810">Allows the admin to require encryption to be turned on using BitLocker.</span></span>|
|<span data-ttu-id="4db07-811">bitLockerSystemDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="4db07-811">bitLockerSystemDrivePolicy</span></span>|[<span data-ttu-id="4db07-812">bitLockerSystemDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="4db07-812">bitLockerSystemDrivePolicy</span></span>](../resources/intune-deviceconfig-bitlockersystemdrivepolicy.md)|<span data-ttu-id="4db07-813">BitLocker 系统驱动器策略。</span><span class="sxs-lookup"><span data-stu-id="4db07-813">BitLocker System Drive Policy.</span></span>|
|<span data-ttu-id="4db07-814">bitLockerFixedDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="4db07-814">bitLockerFixedDrivePolicy</span></span>|[<span data-ttu-id="4db07-815">bitLockerFixedDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="4db07-815">bitLockerFixedDrivePolicy</span></span>](../resources/intune-deviceconfig-bitlockerfixeddrivepolicy.md)|<span data-ttu-id="4db07-816">BitLocker 固定驱动器策略。</span><span class="sxs-lookup"><span data-stu-id="4db07-816">BitLocker Fixed Drive Policy.</span></span>|
|<span data-ttu-id="4db07-817">bitLockerRemovableDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="4db07-817">bitLockerRemovableDrivePolicy</span></span>|[<span data-ttu-id="4db07-818">bitLockerRemovableDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="4db07-818">bitLockerRemovableDrivePolicy</span></span>](../resources/intune-deviceconfig-bitlockerremovabledrivepolicy.md)|<span data-ttu-id="4db07-819">BitLocker 可移动驱动器策略。</span><span class="sxs-lookup"><span data-stu-id="4db07-819">BitLocker Removable Drive Policy.</span></span>|
|<span data-ttu-id="4db07-820">bitLockerRecoveryPasswordRotation</span><span class="sxs-lookup"><span data-stu-id="4db07-820">bitLockerRecoveryPasswordRotation</span></span>|[<span data-ttu-id="4db07-821">bitLockerRecoveryPasswordRotationType</span><span class="sxs-lookup"><span data-stu-id="4db07-821">bitLockerRecoveryPasswordRotationType</span></span>](../resources/intune-shared-bitlockerrecoverypasswordrotationtype.md)|<span data-ttu-id="4db07-822">此设置在操作系统驱动器恢复后启动客户端驱动的恢复密码轮替（使用 bootmgr 或 WinRE）。</span><span class="sxs-lookup"><span data-stu-id="4db07-822">This setting initiates a client-driven recovery password rotation after an OS drive recovery (either by using bootmgr or WinRE).</span></span> <span data-ttu-id="4db07-823">可取值为：`notConfigured`、`disabled`、`enabledForAzureAd`、`enabledForAzureAdAndHybrid`。</span><span class="sxs-lookup"><span data-stu-id="4db07-823">Possible values are: `notConfigured`, `disabled`, `enabledForAzureAd`, `enabledForAzureAdAndHybrid`.</span></span>|
|<span data-ttu-id="4db07-824">defenderDisableScanArchiveFiles</span><span class="sxs-lookup"><span data-stu-id="4db07-824">defenderDisableScanArchiveFiles</span></span>|<span data-ttu-id="4db07-825">Boolean</span><span class="sxs-lookup"><span data-stu-id="4db07-825">Boolean</span></span>|<span data-ttu-id="4db07-826">允许或禁止扫描存档。</span><span class="sxs-lookup"><span data-stu-id="4db07-826">Allows or disallows scanning of archives.</span></span>|
|<span data-ttu-id="4db07-827">defenderDisableBehaviorMonitoring</span><span class="sxs-lookup"><span data-stu-id="4db07-827">defenderDisableBehaviorMonitoring</span></span>|<span data-ttu-id="4db07-828">Boolean</span><span class="sxs-lookup"><span data-stu-id="4db07-828">Boolean</span></span>|<span data-ttu-id="4db07-829">允许或禁止 Windows Defender 行为监控功能。</span><span class="sxs-lookup"><span data-stu-id="4db07-829">Allows or disallows Windows Defender Behavior Monitoring functionality.</span></span>|
|<span data-ttu-id="4db07-830">defenderDisableCloudProtection</span><span class="sxs-lookup"><span data-stu-id="4db07-830">defenderDisableCloudProtection</span></span>|<span data-ttu-id="4db07-831">Boolean</span><span class="sxs-lookup"><span data-stu-id="4db07-831">Boolean</span></span>|<span data-ttu-id="4db07-832">为最大限度地保护你的电脑，Windows Defender 将向 Microsoft 发送有关发现的任何问题的信息。</span><span class="sxs-lookup"><span data-stu-id="4db07-832">To best protect your PC, Windows Defender will send information to Microsoft about any problems it finds.</span></span> <span data-ttu-id="4db07-833">Microsoft 将分析该信息，详细了解影响您和其他客户的问题，并提供改进的解决方案。</span><span class="sxs-lookup"><span data-stu-id="4db07-833">Microsoft will analyze that information, learn more about problems affecting you and other customers, and offer improved solutions.</span></span>|
|<span data-ttu-id="4db07-834">defenderEnableScanIncomingMail</span><span class="sxs-lookup"><span data-stu-id="4db07-834">defenderEnableScanIncomingMail</span></span>|<span data-ttu-id="4db07-835">Boolean</span><span class="sxs-lookup"><span data-stu-id="4db07-835">Boolean</span></span>|<span data-ttu-id="4db07-836">允许或禁止扫描电子邮件。</span><span class="sxs-lookup"><span data-stu-id="4db07-836">Allows or disallows scanning of email.</span></span>|
|<span data-ttu-id="4db07-837">defenderEnableScanMappedNetworkDrivesDuringFullScan</span><span class="sxs-lookup"><span data-stu-id="4db07-837">defenderEnableScanMappedNetworkDrivesDuringFullScan</span></span>|<span data-ttu-id="4db07-838">Boolean</span><span class="sxs-lookup"><span data-stu-id="4db07-838">Boolean</span></span>|<span data-ttu-id="4db07-839">允许或禁止对映射的网络驱动器进行完全扫描。</span><span class="sxs-lookup"><span data-stu-id="4db07-839">Allows or disallows a full scan of mapped network drives.</span></span>|
|<span data-ttu-id="4db07-840">defenderDisableScanRemovableDrivesDuringFullScan</span><span class="sxs-lookup"><span data-stu-id="4db07-840">defenderDisableScanRemovableDrivesDuringFullScan</span></span>|<span data-ttu-id="4db07-841">Boolean</span><span class="sxs-lookup"><span data-stu-id="4db07-841">Boolean</span></span>|<span data-ttu-id="4db07-842">允许或禁止对可移动驱动器进行完全扫描。</span><span class="sxs-lookup"><span data-stu-id="4db07-842">Allows or disallows a full scan of removable drives.</span></span> <span data-ttu-id="4db07-843">在快速扫描过程中，可能仍会扫描可移动驱动器。</span><span class="sxs-lookup"><span data-stu-id="4db07-843">During a quick scan, removable drives may still be scanned.</span></span>|
|<span data-ttu-id="4db07-844">defenderDisableScanDownloads</span><span class="sxs-lookup"><span data-stu-id="4db07-844">defenderDisableScanDownloads</span></span>|<span data-ttu-id="4db07-845">Boolean</span><span class="sxs-lookup"><span data-stu-id="4db07-845">Boolean</span></span>|<span data-ttu-id="4db07-846">允许或禁止 Windows Defender IOAVP 保护功能。</span><span class="sxs-lookup"><span data-stu-id="4db07-846">Allows or disallows Windows Defender IOAVP Protection functionality.</span></span>|
|<span data-ttu-id="4db07-847">defenderDisableIntrusionPreventionSystem</span><span class="sxs-lookup"><span data-stu-id="4db07-847">defenderDisableIntrusionPreventionSystem</span></span>|<span data-ttu-id="4db07-848">Boolean</span><span class="sxs-lookup"><span data-stu-id="4db07-848">Boolean</span></span>|<span data-ttu-id="4db07-849">允许或禁止 Windows Defender 入侵防护功能。</span><span class="sxs-lookup"><span data-stu-id="4db07-849">Allows or disallows Windows Defender Intrusion Prevention functionality.</span></span>|
|<span data-ttu-id="4db07-850">defenderDisableOnAccessProtection</span><span class="sxs-lookup"><span data-stu-id="4db07-850">defenderDisableOnAccessProtection</span></span>|<span data-ttu-id="4db07-851">Boolean</span><span class="sxs-lookup"><span data-stu-id="4db07-851">Boolean</span></span>|<span data-ttu-id="4db07-852">允许或禁止 Windows Defender 访问保护功能。</span><span class="sxs-lookup"><span data-stu-id="4db07-852">Allows or disallows Windows Defender On Access Protection functionality.</span></span>|
|<span data-ttu-id="4db07-853">defenderDisableRealTimeMonitoring</span><span class="sxs-lookup"><span data-stu-id="4db07-853">defenderDisableRealTimeMonitoring</span></span>|<span data-ttu-id="4db07-854">Boolean</span><span class="sxs-lookup"><span data-stu-id="4db07-854">Boolean</span></span>|<span data-ttu-id="4db07-855">允许或禁止 Windows Defender 实时监视功能。</span><span class="sxs-lookup"><span data-stu-id="4db07-855">Allows or disallows Windows Defender Realtime Monitoring functionality.</span></span>|
|<span data-ttu-id="4db07-856">defenderDisableScanNetworkFiles</span><span class="sxs-lookup"><span data-stu-id="4db07-856">defenderDisableScanNetworkFiles</span></span>|<span data-ttu-id="4db07-857">Boolean</span><span class="sxs-lookup"><span data-stu-id="4db07-857">Boolean</span></span>|<span data-ttu-id="4db07-858">允许或禁止扫描网络文件。</span><span class="sxs-lookup"><span data-stu-id="4db07-858">Allows or disallows a scanning of network files.</span></span>|
|<span data-ttu-id="4db07-859">defenderDisableScanScriptsLoadedInInternetExplorer</span><span class="sxs-lookup"><span data-stu-id="4db07-859">defenderDisableScanScriptsLoadedInInternetExplorer</span></span>|<span data-ttu-id="4db07-860">Boolean</span><span class="sxs-lookup"><span data-stu-id="4db07-860">Boolean</span></span>|<span data-ttu-id="4db07-861">允许或禁止 Windows Defender 脚本扫描功能。</span><span class="sxs-lookup"><span data-stu-id="4db07-861">Allows or disallows Windows Defender Script Scanning functionality.</span></span>|
|<span data-ttu-id="4db07-862">defenderBlockEndUserAccess</span><span class="sxs-lookup"><span data-stu-id="4db07-862">defenderBlockEndUserAccess</span></span>|<span data-ttu-id="4db07-863">Boolean</span><span class="sxs-lookup"><span data-stu-id="4db07-863">Boolean</span></span>|<span data-ttu-id="4db07-864">允许或禁止用户访问 Windows Defender UI。</span><span class="sxs-lookup"><span data-stu-id="4db07-864">Allows or disallows user access to the Windows Defender UI.</span></span> <span data-ttu-id="4db07-865">如果不允许，将同时禁止显示所有 Windows Defender 通知。</span><span class="sxs-lookup"><span data-stu-id="4db07-865">If disallowed, all Windows Defender notifications will also be suppressed.</span></span>|
|<span data-ttu-id="4db07-866">defenderScanMaxCpuPercentage</span><span class="sxs-lookup"><span data-stu-id="4db07-866">defenderScanMaxCpuPercentage</span></span>|<span data-ttu-id="4db07-867">Int32</span><span class="sxs-lookup"><span data-stu-id="4db07-867">Int32</span></span>|<span data-ttu-id="4db07-868">表示 Windows Defender 扫描的平均 CPU 负载因子（以百分比为单位）。</span><span class="sxs-lookup"><span data-stu-id="4db07-868">Represents the average CPU load factor for the Windows Defender scan (in percent).</span></span> <span data-ttu-id="4db07-869">默认值为 50。</span><span class="sxs-lookup"><span data-stu-id="4db07-869">The default value is 50.</span></span> <span data-ttu-id="4db07-870">有效值为 0 至 100</span><span class="sxs-lookup"><span data-stu-id="4db07-870">Valid values 0 to 100</span></span>|
|<span data-ttu-id="4db07-871">defenderCheckForSignaturesBeforeRunningScan</span><span class="sxs-lookup"><span data-stu-id="4db07-871">defenderCheckForSignaturesBeforeRunningScan</span></span>|<span data-ttu-id="4db07-872">Boolean</span><span class="sxs-lookup"><span data-stu-id="4db07-872">Boolean</span></span>|<span data-ttu-id="4db07-873">通过此策略设置，您可以管理在运行扫描前是否检查新病毒和间谍软件定义。</span><span class="sxs-lookup"><span data-stu-id="4db07-873">This policy setting allows you to manage whether a check for new virus and spyware definitions will occur before running a scan.</span></span>|
|<span data-ttu-id="4db07-874">defenderCloudBlockLevel</span><span class="sxs-lookup"><span data-stu-id="4db07-874">defenderCloudBlockLevel</span></span>|[<span data-ttu-id="4db07-875">defenderCloudBlockLevelType</span><span class="sxs-lookup"><span data-stu-id="4db07-875">defenderCloudBlockLevelType</span></span>](../resources/intune-deviceconfig-defendercloudblockleveltype.md)|<span data-ttu-id="4db07-876">在 Windows 10 版本1709中添加。</span><span class="sxs-lookup"><span data-stu-id="4db07-876">Added in Windows 10, version 1709.</span></span> <span data-ttu-id="4db07-877">此策略设置确定 Windows Defender 防病毒在阻止和扫描可疑文件时的积极程度。</span><span class="sxs-lookup"><span data-stu-id="4db07-877">This policy setting determines how aggressive Windows Defender Antivirus will be in blocking and scanning suspicious files.</span></span> <span data-ttu-id="4db07-878">值类型为 integer。</span><span class="sxs-lookup"><span data-stu-id="4db07-878">Value type is integer.</span></span> <span data-ttu-id="4db07-879">此功能需要启用 "加入 Microsoft MAPS" 设置，才能正常运行。</span><span class="sxs-lookup"><span data-stu-id="4db07-879">This feature requires the "Join Microsoft MAPS" setting enabled in order to function.</span></span> <span data-ttu-id="4db07-880">可取值为：`notConfigured`、`high`、`highPlus`、`zeroTolerance`。</span><span class="sxs-lookup"><span data-stu-id="4db07-880">Possible values are: `notConfigured`, `high`, `highPlus`, `zeroTolerance`.</span></span>|
|<span data-ttu-id="4db07-881">defenderCloudExtendedTimeoutInSeconds</span><span class="sxs-lookup"><span data-stu-id="4db07-881">defenderCloudExtendedTimeoutInSeconds</span></span>|<span data-ttu-id="4db07-882">Int32</span><span class="sxs-lookup"><span data-stu-id="4db07-882">Int32</span></span>|<span data-ttu-id="4db07-883">在 Windows 10 版本1709中添加。</span><span class="sxs-lookup"><span data-stu-id="4db07-883">Added in Windows 10, version 1709.</span></span> <span data-ttu-id="4db07-884">此功能允许 Windows Defender 防病毒阻止可疑文件长达60秒，并在云中对其进行扫描以确保其安全。</span><span class="sxs-lookup"><span data-stu-id="4db07-884">This feature allows Windows Defender Antivirus to block a suspicious file for up to 60 seconds, and scan it in the cloud to make sure it's safe.</span></span> <span data-ttu-id="4db07-885">值类型为 integer，范围为 0-50。</span><span class="sxs-lookup"><span data-stu-id="4db07-885">Value type is integer, range is 0 - 50.</span></span> <span data-ttu-id="4db07-886">此功能依赖于其他三个映射设置必须全部启用-"配置 ' 在首次看到时阻止 '" 功能; "加入 Microsoft MAPS ";"需要进一步分析时发送文件示例"。</span><span class="sxs-lookup"><span data-stu-id="4db07-886">This feature depends on three other MAPS settings the must all be enabled- "Configure the 'Block at First Sight' feature; "Join Microsoft MAPS"; "Send file samples when further analysis is required".</span></span> <span data-ttu-id="4db07-887">有效值为 0 至 50</span><span class="sxs-lookup"><span data-stu-id="4db07-887">Valid values 0 to 50</span></span>|
|<span data-ttu-id="4db07-888">defenderDaysBeforeDeletingQuarantinedMalware</span><span class="sxs-lookup"><span data-stu-id="4db07-888">defenderDaysBeforeDeletingQuarantinedMalware</span></span>|<span data-ttu-id="4db07-889">Int32</span><span class="sxs-lookup"><span data-stu-id="4db07-889">Int32</span></span>|<span data-ttu-id="4db07-890">隔离项目将存储在系统上的时间段（以天为单位）。</span><span class="sxs-lookup"><span data-stu-id="4db07-890">Time period (in days) that quarantine items will be stored on the system.</span></span> <span data-ttu-id="4db07-891">有效值为 0 至 90</span><span class="sxs-lookup"><span data-stu-id="4db07-891">Valid values 0 to 90</span></span>|
|<span data-ttu-id="4db07-892">defenderDisableCatchupFullScan</span><span class="sxs-lookup"><span data-stu-id="4db07-892">defenderDisableCatchupFullScan</span></span>|<span data-ttu-id="4db07-893">Boolean</span><span class="sxs-lookup"><span data-stu-id="4db07-893">Boolean</span></span>|<span data-ttu-id="4db07-894">通过此策略设置，您可以配置计划完全扫描的追赶扫描。</span><span class="sxs-lookup"><span data-stu-id="4db07-894">This policy setting allows you to configure catch-up scans for scheduled full scans.</span></span> <span data-ttu-id="4db07-895">追赶扫描是由于错过了定期计划的扫描而启动的扫描。</span><span class="sxs-lookup"><span data-stu-id="4db07-895">A catch-up scan is a scan that is initiated because a regularly scheduled scan was missed.</span></span> <span data-ttu-id="4db07-896">通常情况下，这些计划扫描会因计算机在计划时间关闭而丢失。</span><span class="sxs-lookup"><span data-stu-id="4db07-896">Usually these scheduled scans are missed because the computer was turned off at the scheduled time.</span></span>|
|<span data-ttu-id="4db07-897">defenderDisableCatchupQuickScan</span><span class="sxs-lookup"><span data-stu-id="4db07-897">defenderDisableCatchupQuickScan</span></span>|<span data-ttu-id="4db07-898">Boolean</span><span class="sxs-lookup"><span data-stu-id="4db07-898">Boolean</span></span>|<span data-ttu-id="4db07-899">通过此策略设置，您可以配置计划快速扫描的追赶扫描。</span><span class="sxs-lookup"><span data-stu-id="4db07-899">This policy setting allows you to configure catch-up scans for scheduled quick scans.</span></span> <span data-ttu-id="4db07-900">追赶扫描是由于错过了定期计划的扫描而启动的扫描。</span><span class="sxs-lookup"><span data-stu-id="4db07-900">A catch-up scan is a scan that is initiated because a regularly scheduled scan was missed.</span></span> <span data-ttu-id="4db07-901">通常情况下，这些计划扫描会因计算机在计划时间关闭而丢失。</span><span class="sxs-lookup"><span data-stu-id="4db07-901">Usually these scheduled scans are missed because the computer was turned off at the scheduled time.</span></span>|
|<span data-ttu-id="4db07-902">defenderEnableLowCpuPriority</span><span class="sxs-lookup"><span data-stu-id="4db07-902">defenderEnableLowCpuPriority</span></span>|<span data-ttu-id="4db07-903">Boolean</span><span class="sxs-lookup"><span data-stu-id="4db07-903">Boolean</span></span>|<span data-ttu-id="4db07-904">通过此策略设置，您可以启用或禁用计划扫描的 CPU 低优先级。</span><span class="sxs-lookup"><span data-stu-id="4db07-904">This policy setting allows you to enable or disable low CPU priority for scheduled scans.</span></span>|
|<span data-ttu-id="4db07-905">defenderFileExtensionsToExclude</span><span class="sxs-lookup"><span data-stu-id="4db07-905">defenderFileExtensionsToExclude</span></span>|<span data-ttu-id="4db07-906">String collection</span><span class="sxs-lookup"><span data-stu-id="4db07-906">String collection</span></span>|<span data-ttu-id="4db07-907">要从扫描和实时保护中排除的文件扩展名。</span><span class="sxs-lookup"><span data-stu-id="4db07-907">File extensions to exclude from scans and real time protection.</span></span>|
|<span data-ttu-id="4db07-908">defenderFilesAndFoldersToExclude</span><span class="sxs-lookup"><span data-stu-id="4db07-908">defenderFilesAndFoldersToExclude</span></span>|<span data-ttu-id="4db07-909">String collection</span><span class="sxs-lookup"><span data-stu-id="4db07-909">String collection</span></span>|<span data-ttu-id="4db07-910">要从扫描和实时保护中排除的文件和文件夹。</span><span class="sxs-lookup"><span data-stu-id="4db07-910">Files and folder to exclude from scans and real time protection.</span></span>|
|<span data-ttu-id="4db07-911">defenderProcessesToExclude</span><span class="sxs-lookup"><span data-stu-id="4db07-911">defenderProcessesToExclude</span></span>|<span data-ttu-id="4db07-912">String 集合</span><span class="sxs-lookup"><span data-stu-id="4db07-912">String collection</span></span>|<span data-ttu-id="4db07-913">要从扫描和实时保护中排除的进程。</span><span class="sxs-lookup"><span data-stu-id="4db07-913">Processes to exclude from scans and real time protection.</span></span>|
|<span data-ttu-id="4db07-914">defenderPotentiallyUnwantedAppAction</span><span class="sxs-lookup"><span data-stu-id="4db07-914">defenderPotentiallyUnwantedAppAction</span></span>|[<span data-ttu-id="4db07-915">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="4db07-915">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="4db07-916">已添加到 Windows 10 版本 1607 中。</span><span class="sxs-lookup"><span data-stu-id="4db07-916">Added in Windows 10, version 1607.</span></span> <span data-ttu-id="4db07-917">指定对可能有害的应用程序（PUAs）的检测级别。</span><span class="sxs-lookup"><span data-stu-id="4db07-917">Specifies the level of detection for potentially unwanted applications (PUAs).</span></span> <span data-ttu-id="4db07-918">Windows Defender 会在下载可能不需要的软件或尝试在你的计算机上安装自己时向你发出警告。</span><span class="sxs-lookup"><span data-stu-id="4db07-918">Windows Defender alerts you when potentially unwanted software is being downloaded or attempts to install itself on your computer.</span></span> <span data-ttu-id="4db07-919">可取值为：`userDefined`、`enable`、`auditMode`。</span><span class="sxs-lookup"><span data-stu-id="4db07-919">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="4db07-920">defenderScanDirection</span><span class="sxs-lookup"><span data-stu-id="4db07-920">defenderScanDirection</span></span>|[<span data-ttu-id="4db07-921">defenderRealtimeScanDirection</span><span class="sxs-lookup"><span data-stu-id="4db07-921">defenderRealtimeScanDirection</span></span>](../resources/intune-deviceconfig-defenderrealtimescandirection.md)|<span data-ttu-id="4db07-922">控制应监视的文件集。</span><span class="sxs-lookup"><span data-stu-id="4db07-922">Controls which sets of files should be monitored.</span></span> <span data-ttu-id="4db07-923">可取值为：`monitorAllFiles`、`monitorIncomingFilesOnly`、`monitorOutgoingFilesOnly`。</span><span class="sxs-lookup"><span data-stu-id="4db07-923">Possible values are: `monitorAllFiles`, `monitorIncomingFilesOnly`, `monitorOutgoingFilesOnly`.</span></span>|
|<span data-ttu-id="4db07-924">defenderScanType</span><span class="sxs-lookup"><span data-stu-id="4db07-924">defenderScanType</span></span>|[<span data-ttu-id="4db07-925">defenderScanType</span><span class="sxs-lookup"><span data-stu-id="4db07-925">defenderScanType</span></span>](../resources/intune-deviceconfig-defenderscantype.md)|<span data-ttu-id="4db07-926">选择是否执行快速扫描或完全扫描。</span><span class="sxs-lookup"><span data-stu-id="4db07-926">Selects whether to perform a quick scan or full scan.</span></span> <span data-ttu-id="4db07-927">可取值为：`userDefined`、`disabled`、`quick`、`full`。</span><span class="sxs-lookup"><span data-stu-id="4db07-927">Possible values are: `userDefined`, `disabled`, `quick`, `full`.</span></span>|
|<span data-ttu-id="4db07-928">defenderScheduledQuickScanTime</span><span class="sxs-lookup"><span data-stu-id="4db07-928">defenderScheduledQuickScanTime</span></span>|<span data-ttu-id="4db07-929">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="4db07-929">TimeOfDay</span></span>|<span data-ttu-id="4db07-930">选择 Windows Defender 快速扫描应在一天的哪一时间运行。</span><span class="sxs-lookup"><span data-stu-id="4db07-930">Selects the time of day that the Windows Defender quick scan should run.</span></span> <span data-ttu-id="4db07-931">例如，值为 0 = 12：00AM，值为 60 = 1：00AM，值 120 = 2：00，等等，最高为 1380 = 11：00PM 的值。</span><span class="sxs-lookup"><span data-stu-id="4db07-931">For example, a value of 0=12:00AM, a value of 60=1:00AM, a value of 120=2:00, and so on, up to a value of 1380=11:00PM.</span></span> <span data-ttu-id="4db07-932">默认值为120</span><span class="sxs-lookup"><span data-stu-id="4db07-932">The default value is 120</span></span>|
|<span data-ttu-id="4db07-933">defenderScheduledScanDay</span><span class="sxs-lookup"><span data-stu-id="4db07-933">defenderScheduledScanDay</span></span>|[<span data-ttu-id="4db07-934">weeklySchedule</span><span class="sxs-lookup"><span data-stu-id="4db07-934">weeklySchedule</span></span>](../resources/intune-deviceconfig-weeklyschedule.md)|<span data-ttu-id="4db07-935">选择 Windows Defender 扫描应运行的日期。</span><span class="sxs-lookup"><span data-stu-id="4db07-935">Selects the day that the Windows Defender scan should run.</span></span> <span data-ttu-id="4db07-936">可取值为：`userDefined`、`everyday`、`sunday`、`monday`、`tuesday`、`wednesday`、`thursday`、`friday`、`saturday`、`noScheduledScan`。</span><span class="sxs-lookup"><span data-stu-id="4db07-936">Possible values are: `userDefined`, `everyday`, `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`, `noScheduledScan`.</span></span>|
|<span data-ttu-id="4db07-937">defenderScheduledScanTime</span><span class="sxs-lookup"><span data-stu-id="4db07-937">defenderScheduledScanTime</span></span>|<span data-ttu-id="4db07-938">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="4db07-938">TimeOfDay</span></span>|<span data-ttu-id="4db07-939">选择 Windows Defender 扫描应在一天的哪一时间运行。</span><span class="sxs-lookup"><span data-stu-id="4db07-939">Selects the time of day that the Windows Defender scan should run.</span></span>|
|<span data-ttu-id="4db07-940">defenderSubmitSamplesConsentType</span><span class="sxs-lookup"><span data-stu-id="4db07-940">defenderSubmitSamplesConsentType</span></span>|[<span data-ttu-id="4db07-941">defenderSubmitSamplesConsentType</span><span class="sxs-lookup"><span data-stu-id="4db07-941">defenderSubmitSamplesConsentType</span></span>](../resources/intune-deviceconfig-defendersubmitsamplesconsenttype.md)|<span data-ttu-id="4db07-942">检查 Windows Defender 中的用户同意级别以发送数据。</span><span class="sxs-lookup"><span data-stu-id="4db07-942">Checks for the user consent level in Windows Defender to send data.</span></span> <span data-ttu-id="4db07-943">可取值为：`sendSafeSamplesAutomatically`、`alwaysPrompt`、`neverSend`、`sendAllSamplesAutomatically`。</span><span class="sxs-lookup"><span data-stu-id="4db07-943">Possible values are: `sendSafeSamplesAutomatically`, `alwaysPrompt`, `neverSend`, `sendAllSamplesAutomatically`.</span></span>|
|<span data-ttu-id="4db07-944">defenderDetectedMalwareActions</span><span class="sxs-lookup"><span data-stu-id="4db07-944">defenderDetectedMalwareActions</span></span>|[<span data-ttu-id="4db07-945">defenderDetectedMalwareActions</span><span class="sxs-lookup"><span data-stu-id="4db07-945">defenderDetectedMalwareActions</span></span>](../resources/intune-deviceconfig-defenderdetectedmalwareactions.md)|<span data-ttu-id="4db07-946">允许管理员指定任何有效的威胁严重级别和相应的默认操作 ID 进行。</span><span class="sxs-lookup"><span data-stu-id="4db07-946">Allows an administrator to specify any valid threat severity levels and the corresponding default action ID to take.</span></span>|



## <a name="response"></a><span data-ttu-id="4db07-947">响应</span><span class="sxs-lookup"><span data-stu-id="4db07-947">Response</span></span>
<span data-ttu-id="4db07-948">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="4db07-948">If successful, this method returns a `201 Created` response code and a [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4db07-949">示例</span><span class="sxs-lookup"><span data-stu-id="4db07-949">Example</span></span>

### <a name="request"></a><span data-ttu-id="4db07-950">请求</span><span class="sxs-lookup"><span data-stu-id="4db07-950">Request</span></span>
<span data-ttu-id="4db07-951">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="4db07-951">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 30451

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
  "defenderDisableBehaviorMonitoring": true,
  "defenderDisableCloudProtection": true,
  "defenderEnableScanIncomingMail": true,
  "defenderEnableScanMappedNetworkDrivesDuringFullScan": true,
  "defenderDisableScanRemovableDrivesDuringFullScan": true,
  "defenderDisableScanDownloads": true,
  "defenderDisableIntrusionPreventionSystem": true,
  "defenderDisableOnAccessProtection": true,
  "defenderDisableRealTimeMonitoring": true,
  "defenderDisableScanNetworkFiles": true,
  "defenderDisableScanScriptsLoadedInInternetExplorer": true,
  "defenderBlockEndUserAccess": true,
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

### <a name="response"></a><span data-ttu-id="4db07-952">响应</span><span class="sxs-lookup"><span data-stu-id="4db07-952">Response</span></span>
<span data-ttu-id="4db07-p221">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="4db07-p221">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 30623

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
  "defenderDisableBehaviorMonitoring": true,
  "defenderDisableCloudProtection": true,
  "defenderEnableScanIncomingMail": true,
  "defenderEnableScanMappedNetworkDrivesDuringFullScan": true,
  "defenderDisableScanRemovableDrivesDuringFullScan": true,
  "defenderDisableScanDownloads": true,
  "defenderDisableIntrusionPreventionSystem": true,
  "defenderDisableOnAccessProtection": true,
  "defenderDisableRealTimeMonitoring": true,
  "defenderDisableScanNetworkFiles": true,
  "defenderDisableScanScriptsLoadedInInternetExplorer": true,
  "defenderBlockEndUserAccess": true,
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





