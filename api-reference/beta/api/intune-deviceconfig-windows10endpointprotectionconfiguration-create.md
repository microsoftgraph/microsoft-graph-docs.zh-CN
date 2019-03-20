---
title: 创建 windows10EndpointProtectionConfiguration
description: 创建新的 windows10EndpointProtectionConfiguration 对象。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: af33879df37b1c3bcb77fe85cbecc66d2640f4a1
ms.sourcegitcommit: f58ff560fa02ac95e296375c143b0922fb6a425c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/19/2019
ms.locfileid: "30572234"
---
# <a name="create-windows10endpointprotectionconfiguration"></a><span data-ttu-id="a7082-103">创建 windows10EndpointProtectionConfiguration</span><span class="sxs-lookup"><span data-stu-id="a7082-103">Create windows10EndpointProtectionConfiguration</span></span>

> <span data-ttu-id="a7082-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="a7082-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a7082-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="a7082-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a7082-106">创建新的 [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="a7082-106">Create a new [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a7082-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="a7082-107">Prerequisites</span></span>
<span data-ttu-id="a7082-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="a7082-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="a7082-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="a7082-110">Permission type</span></span>|<span data-ttu-id="a7082-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="a7082-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a7082-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a7082-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a7082-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a7082-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a7082-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a7082-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a7082-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="a7082-115">Not supported.</span></span>|
|<span data-ttu-id="a7082-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="a7082-116">Application</span></span>|<span data-ttu-id="a7082-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="a7082-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a7082-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a7082-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="a7082-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="a7082-119">Request headers</span></span>
|<span data-ttu-id="a7082-120">标头</span><span class="sxs-lookup"><span data-stu-id="a7082-120">Header</span></span>|<span data-ttu-id="a7082-121">值</span><span class="sxs-lookup"><span data-stu-id="a7082-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a7082-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="a7082-122">Authorization</span></span>|<span data-ttu-id="a7082-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="a7082-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a7082-124">接受</span><span class="sxs-lookup"><span data-stu-id="a7082-124">Accept</span></span>|<span data-ttu-id="a7082-125">application/json</span><span class="sxs-lookup"><span data-stu-id="a7082-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a7082-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="a7082-126">Request body</span></span>
<span data-ttu-id="a7082-127">在请求正文中，提供 windows10EndpointProtectionConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a7082-127">In the request body, supply a JSON representation for the windows10EndpointProtectionConfiguration object.</span></span>

<span data-ttu-id="a7082-128">下表显示了创建 windows10EndpointProtectionConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="a7082-128">The following table shows the properties that are required when you create the windows10EndpointProtectionConfiguration.</span></span>

|<span data-ttu-id="a7082-129">属性</span><span class="sxs-lookup"><span data-stu-id="a7082-129">Property</span></span>|<span data-ttu-id="a7082-130">类型</span><span class="sxs-lookup"><span data-stu-id="a7082-130">Type</span></span>|<span data-ttu-id="a7082-131">说明</span><span class="sxs-lookup"><span data-stu-id="a7082-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a7082-132">id</span><span class="sxs-lookup"><span data-stu-id="a7082-132">id</span></span>|<span data-ttu-id="a7082-133">String</span><span class="sxs-lookup"><span data-stu-id="a7082-133">String</span></span>|<span data-ttu-id="a7082-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="a7082-134">Key of the entity.</span></span> <span data-ttu-id="a7082-135">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a7082-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a7082-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a7082-136">lastModifiedDateTime</span></span>|<span data-ttu-id="a7082-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a7082-137">DateTimeOffset</span></span>|<span data-ttu-id="a7082-138">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="a7082-138">DateTime the object was last modified.</span></span> <span data-ttu-id="a7082-139">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a7082-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a7082-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="a7082-140">roleScopeTagIds</span></span>|<span data-ttu-id="a7082-141">String collection</span><span class="sxs-lookup"><span data-stu-id="a7082-141">String collection</span></span>|<span data-ttu-id="a7082-142">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="a7082-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="a7082-143">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a7082-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a7082-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="a7082-144">supportsScopeTags</span></span>|<span data-ttu-id="a7082-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="a7082-145">Boolean</span></span>|<span data-ttu-id="a7082-146">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="a7082-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="a7082-147">如果此值为 false, 则不允许分配给 ScopeTags 属性, 并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="a7082-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="a7082-148">这适用于在 Silverlight 中创建的旧版策略, 可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="a7082-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="a7082-149">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="a7082-149">This property is read-only.</span></span> <span data-ttu-id="a7082-150">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a7082-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a7082-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a7082-151">createdDateTime</span></span>|<span data-ttu-id="a7082-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a7082-152">DateTimeOffset</span></span>|<span data-ttu-id="a7082-153">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="a7082-153">DateTime the object was created.</span></span> <span data-ttu-id="a7082-154">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a7082-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a7082-155">说明</span><span class="sxs-lookup"><span data-stu-id="a7082-155">description</span></span>|<span data-ttu-id="a7082-156">字符串</span><span class="sxs-lookup"><span data-stu-id="a7082-156">String</span></span>|<span data-ttu-id="a7082-157">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="a7082-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="a7082-158">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a7082-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a7082-159">displayName</span><span class="sxs-lookup"><span data-stu-id="a7082-159">displayName</span></span>|<span data-ttu-id="a7082-160">String</span><span class="sxs-lookup"><span data-stu-id="a7082-160">String</span></span>|<span data-ttu-id="a7082-161">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="a7082-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="a7082-162">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a7082-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a7082-163">version</span><span class="sxs-lookup"><span data-stu-id="a7082-163">version</span></span>|<span data-ttu-id="a7082-164">Int32</span><span class="sxs-lookup"><span data-stu-id="a7082-164">Int32</span></span>|<span data-ttu-id="a7082-165">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="a7082-165">Version of the device configuration.</span></span> <span data-ttu-id="a7082-166">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a7082-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a7082-167">dmaGuardDeviceEnumerationPolicy</span><span class="sxs-lookup"><span data-stu-id="a7082-167">dmaGuardDeviceEnumerationPolicy</span></span>|[<span data-ttu-id="a7082-168">dmaGuardDeviceEnumerationPolicyType</span><span class="sxs-lookup"><span data-stu-id="a7082-168">dmaGuardDeviceEnumerationPolicyType</span></span>](../resources/intune-deviceconfig-dmaguarddeviceenumerationpolicytype.md)|<span data-ttu-id="a7082-169">此策略旨在提供针对支持外部 DMA 的设备的额外安全性。</span><span class="sxs-lookup"><span data-stu-id="a7082-169">This policy is intended to provide additional security against external DMA capable devices.</span></span> <span data-ttu-id="a7082-170">通过它, 可以更好地控制支持外部 dma 的设备与 dma 重新映射/设备内存隔离和沙盒不兼容的枚举。</span><span class="sxs-lookup"><span data-stu-id="a7082-170">It allows for more control over the enumeration of external DMA capable devices incompatible with DMA Remapping/device memory isolation and sandboxing.</span></span> <span data-ttu-id="a7082-171">仅当系统固件支持和启用内核 DMA 保护时, 此策略才会生效。</span><span class="sxs-lookup"><span data-stu-id="a7082-171">This policy only takes effect when Kernel DMA Protection is supported and enabled by the system firmware.</span></span> <span data-ttu-id="a7082-172">内核 DMA 保护是一项平台功能, 不能通过策略或最终用户进行控制。</span><span class="sxs-lookup"><span data-stu-id="a7082-172">Kernel DMA Protection is a platform feature that cannot be controlled via policy or by end user.</span></span> <span data-ttu-id="a7082-173">在制造时, 系统必须支持它。</span><span class="sxs-lookup"><span data-stu-id="a7082-173">It has to be supported by the system at the time of manufacturing.</span></span> <span data-ttu-id="a7082-174">若要检查系统是否支持内核 dma 保护, 请在 MSINFO32 的摘要页中检查 "内核 dma 保护" 字段。</span><span class="sxs-lookup"><span data-stu-id="a7082-174">To check if the system supports Kernel DMA Protection, please check the Kernel DMA Protection field in the Summary page of MSINFO32.exe.</span></span> <span data-ttu-id="a7082-175">可取值为：`deviceDefault`、`blockAll`、`allowAll`。</span><span class="sxs-lookup"><span data-stu-id="a7082-175">Possible values are: `deviceDefault`, `blockAll`, `allowAll`.</span></span>|
|<span data-ttu-id="a7082-176">firewallRules</span><span class="sxs-lookup"><span data-stu-id="a7082-176">firewallRules</span></span>|<span data-ttu-id="a7082-177">[windowsFirewallRule](../resources/intune-deviceconfig-windowsfirewallrule.md)集合</span><span class="sxs-lookup"><span data-stu-id="a7082-177">[windowsFirewallRule](../resources/intune-deviceconfig-windowsfirewallrule.md) collection</span></span>|<span data-ttu-id="a7082-178">配置防火墙规则设置。</span><span class="sxs-lookup"><span data-stu-id="a7082-178">Configures the firewall rule settings.</span></span> <span data-ttu-id="a7082-179">此集合最多可包含150个元素。</span><span class="sxs-lookup"><span data-stu-id="a7082-179">This collection can contain a maximum of 150 elements.</span></span>|
|<span data-ttu-id="a7082-180">userRightsAccessCredentialManagerAsTrustedCaller</span><span class="sxs-lookup"><span data-stu-id="a7082-180">userRightsAccessCredentialManagerAsTrustedCaller</span></span>|[<span data-ttu-id="a7082-181">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="a7082-181">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="a7082-182">此用户权限由凭据管理器在备份/还原过程中使用。</span><span class="sxs-lookup"><span data-stu-id="a7082-182">This user right is used by Credential Manager during Backup/Restore.</span></span> <span data-ttu-id="a7082-183">如果为其他实体提供此权限, 则用户保存的凭据可能会受到威胁。</span><span class="sxs-lookup"><span data-stu-id="a7082-183">Users' saved credentials might be compromised if this privilege is given to other entities.</span></span> <span data-ttu-id="a7082-184">仅支持 NotConfigured 和允许的状态</span><span class="sxs-lookup"><span data-stu-id="a7082-184">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="a7082-185">userRightsAllowAccessFromNetwork</span><span class="sxs-lookup"><span data-stu-id="a7082-185">userRightsAllowAccessFromNetwork</span></span>|[<span data-ttu-id="a7082-186">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="a7082-186">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="a7082-187">此用户权限确定允许哪些用户和组通过网络连接到计算机。</span><span class="sxs-lookup"><span data-stu-id="a7082-187">This user right determines which users and groups are allowed to connect to the computer over the network.</span></span> <span data-ttu-id="a7082-188">支持的状态为 "允许"。</span><span class="sxs-lookup"><span data-stu-id="a7082-188">State Allowed is supported.</span></span>|
|<span data-ttu-id="a7082-189">userRightsBlockAccessFromNetwork</span><span class="sxs-lookup"><span data-stu-id="a7082-189">userRightsBlockAccessFromNetwork</span></span>|[<span data-ttu-id="a7082-190">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="a7082-190">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="a7082-191">此用户权限决定了阻止哪些用户和组通过网络连接到计算机。</span><span class="sxs-lookup"><span data-stu-id="a7082-191">This user right determines which users and groups are block from connecting to the computer over the network.</span></span> <span data-ttu-id="a7082-192">支持状态块。</span><span class="sxs-lookup"><span data-stu-id="a7082-192">State Block is supported.</span></span>|
|<span data-ttu-id="a7082-193">userRightsActAsPartOfTheOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="a7082-193">userRightsActAsPartOfTheOperatingSystem</span></span>|[<span data-ttu-id="a7082-194">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="a7082-194">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="a7082-195">此用户权限允许进程在不进行身份验证的情况下模拟任何用户。</span><span class="sxs-lookup"><span data-stu-id="a7082-195">This user right allows a process to impersonate any user without authentication.</span></span> <span data-ttu-id="a7082-196">因此, 该过程可以获得与该用户相同的本地资源的访问权限。</span><span class="sxs-lookup"><span data-stu-id="a7082-196">The process can therefore gain access to the same local resources as that user.</span></span> <span data-ttu-id="a7082-197">仅支持 NotConfigured 和允许的状态</span><span class="sxs-lookup"><span data-stu-id="a7082-197">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="a7082-198">userRightsLocalLogOn</span><span class="sxs-lookup"><span data-stu-id="a7082-198">userRightsLocalLogOn</span></span>|[<span data-ttu-id="a7082-199">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="a7082-199">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="a7082-200">此用户权限确定哪些用户可以登录到计算机。</span><span class="sxs-lookup"><span data-stu-id="a7082-200">This user right determines which users can log on to the computer.</span></span> <span data-ttu-id="a7082-201">所有支持的状态 NotConfigured、允许和阻止</span><span class="sxs-lookup"><span data-stu-id="a7082-201">States NotConfigured, Allowed and Blocked are all supported</span></span> |
|<span data-ttu-id="a7082-202">userRightsBackupData</span><span class="sxs-lookup"><span data-stu-id="a7082-202">userRightsBackupData</span></span>|[<span data-ttu-id="a7082-203">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="a7082-203">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="a7082-204">此用户权限确定在备份文件和目录时, 哪些用户可以绕过文件、目录、注册表和其他持久对象权限。</span><span class="sxs-lookup"><span data-stu-id="a7082-204">This user right determines which users can bypass file, directory, registry, and other persistent objects permissions when backing up files and directories.</span></span> <span data-ttu-id="a7082-205">仅支持 NotConfigured 和允许的状态</span><span class="sxs-lookup"><span data-stu-id="a7082-205">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="a7082-206">userRightsChangeSystemTime</span><span class="sxs-lookup"><span data-stu-id="a7082-206">userRightsChangeSystemTime</span></span>|[<span data-ttu-id="a7082-207">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="a7082-207">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="a7082-208">此用户权限确定哪些用户和组可以更改计算机内部时钟上的时间和日期。</span><span class="sxs-lookup"><span data-stu-id="a7082-208">This user right determines which users and groups can change the time and date on the internal clock of the computer.</span></span> <span data-ttu-id="a7082-209">仅支持 NotConfigured 和允许的状态</span><span class="sxs-lookup"><span data-stu-id="a7082-209">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="a7082-210">userRightsCreateGlobalObjects</span><span class="sxs-lookup"><span data-stu-id="a7082-210">userRightsCreateGlobalObjects</span></span>|[<span data-ttu-id="a7082-211">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="a7082-211">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="a7082-212">此安全设置确定用户是否可以创建可用于所有会话的全局对象。</span><span class="sxs-lookup"><span data-stu-id="a7082-212">This security setting determines whether users can create global objects that are available to all sessions.</span></span> <span data-ttu-id="a7082-213">可以创建全局对象的用户可能会影响在其他用户的会话下运行的进程, 这可能导致应用程序故障或数据损坏。</span><span class="sxs-lookup"><span data-stu-id="a7082-213">Users who can create global objects could affect processes that run under other users' sessions, which could lead to application failure or data corruption.</span></span> <span data-ttu-id="a7082-214">仅支持 NotConfigured 和允许的状态</span><span class="sxs-lookup"><span data-stu-id="a7082-214">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="a7082-215">userRightsCreatePageFile</span><span class="sxs-lookup"><span data-stu-id="a7082-215">userRightsCreatePageFile</span></span>|[<span data-ttu-id="a7082-216">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="a7082-216">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="a7082-217">此用户权限确定哪些用户和组可以调用内部 API 来创建和更改页面文件的大小。</span><span class="sxs-lookup"><span data-stu-id="a7082-217">This user right determines which users and groups can call an internal API to create and change the size of a page file.</span></span> <span data-ttu-id="a7082-218">仅支持 NotConfigured 和允许的状态</span><span class="sxs-lookup"><span data-stu-id="a7082-218">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="a7082-219">userRightsCreatePermanentSharedObjects</span><span class="sxs-lookup"><span data-stu-id="a7082-219">userRightsCreatePermanentSharedObjects</span></span>|[<span data-ttu-id="a7082-220">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="a7082-220">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="a7082-221">此用户权限决定了进程可以使用哪些帐户使用对象管理器创建目录对象。</span><span class="sxs-lookup"><span data-stu-id="a7082-221">This user right determines which accounts can be used by processes to create a directory object using the object manager.</span></span> <span data-ttu-id="a7082-222">仅支持 NotConfigured 和允许的状态</span><span class="sxs-lookup"><span data-stu-id="a7082-222">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="a7082-223">userRightsCreateSymbolicLinks</span><span class="sxs-lookup"><span data-stu-id="a7082-223">userRightsCreateSymbolicLinks</span></span>|[<span data-ttu-id="a7082-224">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="a7082-224">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="a7082-225">此用户权限确定用户是否可以从其登录到的计算机创建符号链接。</span><span class="sxs-lookup"><span data-stu-id="a7082-225">This user right determines if the user can create a symbolic link from the computer to which they are logged on.</span></span> <span data-ttu-id="a7082-226">仅支持 NotConfigured 和允许的状态</span><span class="sxs-lookup"><span data-stu-id="a7082-226">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="a7082-227">userRightsCreateToken</span><span class="sxs-lookup"><span data-stu-id="a7082-227">userRightsCreateToken</span></span>|[<span data-ttu-id="a7082-228">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="a7082-228">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="a7082-229">此用户权限确定进程在使用内部 API 创建访问令牌时, 可以使用哪些用户/组来创建令牌, 然后可以使用这些用户/组来获取对任何本地资源的访问权限。</span><span class="sxs-lookup"><span data-stu-id="a7082-229">This user right determines which users/groups can be used by processes to create a token that can then be used to get access to any local resources when the process uses an internal API to create an access token.</span></span> <span data-ttu-id="a7082-230">仅支持 NotConfigured 和允许的状态</span><span class="sxs-lookup"><span data-stu-id="a7082-230">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="a7082-231">userRightsDebugPrograms</span><span class="sxs-lookup"><span data-stu-id="a7082-231">userRightsDebugPrograms</span></span>|[<span data-ttu-id="a7082-232">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="a7082-232">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="a7082-233">此用户权限确定哪些用户可以将调试程序附加到任何进程或内核。</span><span class="sxs-lookup"><span data-stu-id="a7082-233">This user right determines which users can attach a debugger to any process or to the kernel.</span></span> <span data-ttu-id="a7082-234">仅支持 NotConfigured 和允许的状态</span><span class="sxs-lookup"><span data-stu-id="a7082-234">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="a7082-235">userRightsRemoteDesktopServicesLogOn</span><span class="sxs-lookup"><span data-stu-id="a7082-235">userRightsRemoteDesktopServicesLogOn</span></span>|[<span data-ttu-id="a7082-236">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="a7082-236">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="a7082-237">此用户权限确定禁止哪些用户和组作为远程桌面服务客户端进行登录。</span><span class="sxs-lookup"><span data-stu-id="a7082-237">This user right determines which users and groups are prohibited from logging on as a Remote Desktop Services client.</span></span> <span data-ttu-id="a7082-238">仅支持状态 NotConfigured 和阻止</span><span class="sxs-lookup"><span data-stu-id="a7082-238">Only states NotConfigured and Blocked are supported</span></span>|
|<span data-ttu-id="a7082-239">userRightsDelegation</span><span class="sxs-lookup"><span data-stu-id="a7082-239">userRightsDelegation</span></span>|[<span data-ttu-id="a7082-240">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="a7082-240">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="a7082-241">此用户权限确定哪些用户可以在用户或计算机对象上设置受信任委派设置。</span><span class="sxs-lookup"><span data-stu-id="a7082-241">This user right determines which users can set the Trusted for Delegation setting on a user or computer object.</span></span> <span data-ttu-id="a7082-242">仅支持 NotConfigured 和允许的状态。</span><span class="sxs-lookup"><span data-stu-id="a7082-242">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="a7082-243">userRightsGenerateSecurityAudits</span><span class="sxs-lookup"><span data-stu-id="a7082-243">userRightsGenerateSecurityAudits</span></span>|[<span data-ttu-id="a7082-244">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="a7082-244">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="a7082-245">此用户权限确定进程可使用哪些帐户向安全日志中添加条目。</span><span class="sxs-lookup"><span data-stu-id="a7082-245">This user right determines which accounts can be used by a process to add entries to the security log.</span></span> <span data-ttu-id="a7082-246">安全日志用于跟踪未经授权的系统访问。</span><span class="sxs-lookup"><span data-stu-id="a7082-246">The security log is used to trace unauthorized system access.</span></span>  <span data-ttu-id="a7082-247">仅支持 NotConfigured 和允许的状态。</span><span class="sxs-lookup"><span data-stu-id="a7082-247">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="a7082-248">userRightsImpersonateClient</span><span class="sxs-lookup"><span data-stu-id="a7082-248">userRightsImpersonateClient</span></span>|[<span data-ttu-id="a7082-249">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="a7082-249">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="a7082-250">将此用户权限分配给用户将允许代表该用户运行的程序模拟客户端。</span><span class="sxs-lookup"><span data-stu-id="a7082-250">Assigning this user right to a user allows programs running on behalf of that user to impersonate a client.</span></span> <span data-ttu-id="a7082-251">如果此类型的模拟要求此用户权限, 则可以防止未经授权的用户说服客户端连接到已创建的服务, 然后模拟该客户端, 这样可以将未经授权的用户的权限提升到管理级别或系统级别。</span><span class="sxs-lookup"><span data-stu-id="a7082-251">Requiring this user right for this kind of impersonation prevents an unauthorized user from convincing a client to connect to a service that they have created and then impersonating that client, which can elevate the unauthorized user's permissions to administrative or system levels.</span></span> <span data-ttu-id="a7082-252">仅支持 NotConfigured 和允许的状态。</span><span class="sxs-lookup"><span data-stu-id="a7082-252">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="a7082-253">userRightsIncreaseSchedulingPriority</span><span class="sxs-lookup"><span data-stu-id="a7082-253">userRightsIncreaseSchedulingPriority</span></span>|[<span data-ttu-id="a7082-254">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="a7082-254">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="a7082-255">此用户权限确定哪些帐户可以使用具有对另一进程的 Write 属性访问权限的进程, 以增加分配给其他进程的执行优先级。</span><span class="sxs-lookup"><span data-stu-id="a7082-255">This user right determines which accounts can use a process with Write Property access to another process to increase the execution priority assigned to the other process.</span></span> <span data-ttu-id="a7082-256">仅支持 NotConfigured 和允许的状态。</span><span class="sxs-lookup"><span data-stu-id="a7082-256">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="a7082-257">userRightsLoadUnloadDrivers</span><span class="sxs-lookup"><span data-stu-id="a7082-257">userRightsLoadUnloadDrivers</span></span>|[<span data-ttu-id="a7082-258">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="a7082-258">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="a7082-259">此用户权限确定哪些用户可以在内核模式下将设备驱动程序或其他代码动态加载和卸载。</span><span class="sxs-lookup"><span data-stu-id="a7082-259">This user right determines which users can dynamically load and unload device drivers or other code in to kernel mode.</span></span> <span data-ttu-id="a7082-260">仅支持 NotConfigured 和允许的状态。</span><span class="sxs-lookup"><span data-stu-id="a7082-260">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="a7082-261">userRightsLockMemory</span><span class="sxs-lookup"><span data-stu-id="a7082-261">userRightsLockMemory</span></span>|[<span data-ttu-id="a7082-262">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="a7082-262">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="a7082-263">此用户权限确定哪些帐户可以使用进程将数据保存在物理内存中, 这会阻止系统将数据分页到磁盘上的虚拟内存中。</span><span class="sxs-lookup"><span data-stu-id="a7082-263">This user right determines which accounts can use a process to keep data in physical memory, which prevents the system from paging the data to virtual memory on disk.</span></span> <span data-ttu-id="a7082-264">仅支持 NotConfigured 和允许的状态。</span><span class="sxs-lookup"><span data-stu-id="a7082-264">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="a7082-265">userRightsManageAuditingAndSecurityLogs</span><span class="sxs-lookup"><span data-stu-id="a7082-265">userRightsManageAuditingAndSecurityLogs</span></span>|[<span data-ttu-id="a7082-266">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="a7082-266">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="a7082-267">此用户权限确定哪些用户可以为各个资源 (如文件、Active Directory 对象和注册表项) 指定对象访问审核选项。</span><span class="sxs-lookup"><span data-stu-id="a7082-267">This user right determines which users can specify object access auditing options for individual resources, such as files, Active Directory objects, and registry keys.</span></span> <span data-ttu-id="a7082-268">仅支持 NotConfigured 和允许的状态。</span><span class="sxs-lookup"><span data-stu-id="a7082-268">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="a7082-269">userRightsManageVolumes</span><span class="sxs-lookup"><span data-stu-id="a7082-269">userRightsManageVolumes</span></span>|[<span data-ttu-id="a7082-270">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="a7082-270">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="a7082-271">此用户权限确定哪些用户和组可以在某个卷 (如远程碎片整理) 上运行维护任务。</span><span class="sxs-lookup"><span data-stu-id="a7082-271">This user right determines which users and groups can run maintenance tasks on a volume, such as remote defragmentation.</span></span> <span data-ttu-id="a7082-272">仅支持 NotConfigured 和允许的状态。</span><span class="sxs-lookup"><span data-stu-id="a7082-272">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="a7082-273">userRightsModifyFirmwareEnvironment</span><span class="sxs-lookup"><span data-stu-id="a7082-273">userRightsModifyFirmwareEnvironment</span></span>|[<span data-ttu-id="a7082-274">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="a7082-274">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="a7082-275">此用户权限决定了可以修改固件环境值的用户。</span><span class="sxs-lookup"><span data-stu-id="a7082-275">This user right determines who can modify firmware environment values.</span></span> <span data-ttu-id="a7082-276">仅支持 NotConfigured 和允许的状态。</span><span class="sxs-lookup"><span data-stu-id="a7082-276">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="a7082-277">userRightsModifyObjectLabels</span><span class="sxs-lookup"><span data-stu-id="a7082-277">userRightsModifyObjectLabels</span></span>|[<span data-ttu-id="a7082-278">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="a7082-278">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="a7082-279">此用户权限确定哪些用户帐户可以修改对象的完整性标签, 例如, 文件、注册表项或其他用户所拥有的进程。</span><span class="sxs-lookup"><span data-stu-id="a7082-279">This user right determines which user accounts can modify the integrity label of objects, such as files, registry keys, or processes owned by other users.</span></span> <span data-ttu-id="a7082-280">仅支持 NotConfigured 和允许的状态。</span><span class="sxs-lookup"><span data-stu-id="a7082-280">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="a7082-281">userRightsProfileSingleProcess</span><span class="sxs-lookup"><span data-stu-id="a7082-281">userRightsProfileSingleProcess</span></span>|[<span data-ttu-id="a7082-282">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="a7082-282">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="a7082-283">此用户权限确定哪些用户可以使用性能监视工具来监视系统进程的性能。</span><span class="sxs-lookup"><span data-stu-id="a7082-283">This user right determines which users can use performance monitoring tools to monitor the performance of system processes.</span></span> <span data-ttu-id="a7082-284">仅支持 NotConfigured 和允许的状态。</span><span class="sxs-lookup"><span data-stu-id="a7082-284">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="a7082-285">userRightsRemoteShutdown</span><span class="sxs-lookup"><span data-stu-id="a7082-285">userRightsRemoteShutdown</span></span>|[<span data-ttu-id="a7082-286">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="a7082-286">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="a7082-287">此用户权限确定允许哪些用户从网络上的远程位置关闭计算机。</span><span class="sxs-lookup"><span data-stu-id="a7082-287">This user right determines which users are allowed to shut down a computer from a remote location on the network.</span></span> <span data-ttu-id="a7082-288">误用此用户权限可能会导致拒绝服务。</span><span class="sxs-lookup"><span data-stu-id="a7082-288">Misuse of this user right can result in a denial of service.</span></span> <span data-ttu-id="a7082-289">仅支持 NotConfigured 和允许的状态。</span><span class="sxs-lookup"><span data-stu-id="a7082-289">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="a7082-290">userRightsRestoreData</span><span class="sxs-lookup"><span data-stu-id="a7082-290">userRightsRestoreData</span></span>|[<span data-ttu-id="a7082-291">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="a7082-291">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="a7082-292">此用户权限确定在还原备份的文件和目录时, 哪些用户可以绕过文件、目录、注册表和其他持久对象权限, 并确定哪些用户可以将任何有效的安全主体设置为对象的所有者。</span><span class="sxs-lookup"><span data-stu-id="a7082-292">This user right determines which users can bypass file, directory, registry, and other persistent objects permissions when restoring backed up files and directories, and determines which users can set any valid security principal as the owner of an object.</span></span> <span data-ttu-id="a7082-293">仅支持 NotConfigured 和允许的状态。</span><span class="sxs-lookup"><span data-stu-id="a7082-293">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="a7082-294">userRightsTakeOwnership</span><span class="sxs-lookup"><span data-stu-id="a7082-294">userRightsTakeOwnership</span></span>|[<span data-ttu-id="a7082-295">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="a7082-295">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="a7082-296">此用户权限确定哪些用户可以获得系统中任何安全对象的所有权, 包括 Active Directory 对象、文件和文件夹、打印机、注册表项、进程和线程。</span><span class="sxs-lookup"><span data-stu-id="a7082-296">This user right determines which users can take ownership of any securable object in the system, including Active Directory objects, files and folders, printers, registry keys, processes, and threads.</span></span> <span data-ttu-id="a7082-297">仅支持 NotConfigured 和允许的状态。</span><span class="sxs-lookup"><span data-stu-id="a7082-297">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="a7082-298">userRightsRegisterProcessAsService</span><span class="sxs-lookup"><span data-stu-id="a7082-298">userRightsRegisterProcessAsService</span></span>|[<span data-ttu-id="a7082-299">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="a7082-299">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="a7082-300">此安全设置确定阻止将进程注册为服务的服务帐户。</span><span class="sxs-lookup"><span data-stu-id="a7082-300">This security setting determines which service accounts are prevented from registering a process as a service.</span></span> <span data-ttu-id="a7082-301">注意: 此安全设置不适用于系统、本地服务或网络服务帐户。</span><span class="sxs-lookup"><span data-stu-id="a7082-301">Note: This security setting does not apply to the System, Local Service, or Network Service accounts.</span></span> <span data-ttu-id="a7082-302">仅支持阻止状态。</span><span class="sxs-lookup"><span data-stu-id="a7082-302">Only state Blocked is supported.</span></span>|
|<span data-ttu-id="a7082-303">xboxServicesEnableXboxGameSaveTask</span><span class="sxs-lookup"><span data-stu-id="a7082-303">xboxServicesEnableXboxGameSaveTask</span></span>|<span data-ttu-id="a7082-304">Boolean</span><span class="sxs-lookup"><span data-stu-id="a7082-304">Boolean</span></span>|<span data-ttu-id="a7082-305">此设置确定是否启用了 xbox 游戏保存 (1) 或禁用 (0)。</span><span class="sxs-lookup"><span data-stu-id="a7082-305">This setting determines whether xbox game save is enabled (1) or disabled (0).</span></span>|
|<span data-ttu-id="a7082-306">xboxServicesAccessoryManagementServiceStartupMode</span><span class="sxs-lookup"><span data-stu-id="a7082-306">xboxServicesAccessoryManagementServiceStartupMode</span></span>|[<span data-ttu-id="a7082-307">serviceStartType</span><span class="sxs-lookup"><span data-stu-id="a7082-307">serviceStartType</span></span>](../resources/intune-deviceconfig-servicestarttype.md)|<span data-ttu-id="a7082-308">此设置确定附件管理服务的启动类型是 "自动" (2)、"手动" (3)、"已禁用" (4)。</span><span class="sxs-lookup"><span data-stu-id="a7082-308">This setting determines whether the Accessory management service's start type is Automatic(2), Manual(3), Disabled(4).</span></span> <span data-ttu-id="a7082-309">默认: 手动。</span><span class="sxs-lookup"><span data-stu-id="a7082-309">Default: Manual.</span></span> <span data-ttu-id="a7082-310">可取值为：`manual`、`automatic`、`disabled`。</span><span class="sxs-lookup"><span data-stu-id="a7082-310">Possible values are: `manual`, `automatic`, `disabled`.</span></span>|
|<span data-ttu-id="a7082-311">xboxServicesLiveAuthManagerServiceStartupMode</span><span class="sxs-lookup"><span data-stu-id="a7082-311">xboxServicesLiveAuthManagerServiceStartupMode</span></span>|[<span data-ttu-id="a7082-312">serviceStartType</span><span class="sxs-lookup"><span data-stu-id="a7082-312">serviceStartType</span></span>](../resources/intune-deviceconfig-servicestarttype.md)|<span data-ttu-id="a7082-313">此设置确定 Live Auth Manager 服务的启动类型是否为自动 (2)、手动 (3)、已禁用 (4)。</span><span class="sxs-lookup"><span data-stu-id="a7082-313">This setting determines whether Live Auth Manager service's start type is Automatic(2), Manual(3), Disabled(4).</span></span> <span data-ttu-id="a7082-314">默认: 手动。</span><span class="sxs-lookup"><span data-stu-id="a7082-314">Default: Manual.</span></span> <span data-ttu-id="a7082-315">可取值为：`manual`、`automatic`、`disabled`。</span><span class="sxs-lookup"><span data-stu-id="a7082-315">Possible values are: `manual`, `automatic`, `disabled`.</span></span>|
|<span data-ttu-id="a7082-316">xboxServicesLiveGameSaveServiceStartupMode</span><span class="sxs-lookup"><span data-stu-id="a7082-316">xboxServicesLiveGameSaveServiceStartupMode</span></span>|[<span data-ttu-id="a7082-317">serviceStartType</span><span class="sxs-lookup"><span data-stu-id="a7082-317">serviceStartType</span></span>](../resources/intune-deviceconfig-servicestarttype.md)|<span data-ttu-id="a7082-318">此设置确定实时游戏是否保存服务的启动类型为自动 (2)、手动 (3)、已禁用 (4)。</span><span class="sxs-lookup"><span data-stu-id="a7082-318">This setting determines whether Live Game save service's start type is Automatic(2), Manual(3), Disabled(4).</span></span> <span data-ttu-id="a7082-319">默认: 手动。</span><span class="sxs-lookup"><span data-stu-id="a7082-319">Default: Manual.</span></span> <span data-ttu-id="a7082-320">可取值为：`manual`、`automatic`、`disabled`。</span><span class="sxs-lookup"><span data-stu-id="a7082-320">Possible values are: `manual`, `automatic`, `disabled`.</span></span>|
|<span data-ttu-id="a7082-321">xboxServicesLiveNetworkingServiceStartupMode</span><span class="sxs-lookup"><span data-stu-id="a7082-321">xboxServicesLiveNetworkingServiceStartupMode</span></span>|[<span data-ttu-id="a7082-322">serviceStartType</span><span class="sxs-lookup"><span data-stu-id="a7082-322">serviceStartType</span></span>](../resources/intune-deviceconfig-servicestarttype.md)|<span data-ttu-id="a7082-323">此设置确定网络服务的启动类型是否为自动 (2)、手动 (3)、已禁用 (4)。</span><span class="sxs-lookup"><span data-stu-id="a7082-323">This setting determines whether Networking service's start type is Automatic(2), Manual(3), Disabled(4).</span></span> <span data-ttu-id="a7082-324">默认: 手动。</span><span class="sxs-lookup"><span data-stu-id="a7082-324">Default: Manual.</span></span> <span data-ttu-id="a7082-325">可取值为：`manual`、`automatic`、`disabled`。</span><span class="sxs-lookup"><span data-stu-id="a7082-325">Possible values are: `manual`, `automatic`, `disabled`.</span></span>|
|<span data-ttu-id="a7082-326">localSecurityOptionsBlockMicrosoftAccounts</span><span class="sxs-lookup"><span data-stu-id="a7082-326">localSecurityOptionsBlockMicrosoftAccounts</span></span>|<span data-ttu-id="a7082-327">Boolean</span><span class="sxs-lookup"><span data-stu-id="a7082-327">Boolean</span></span>|<span data-ttu-id="a7082-328">阻止用户向此计算机添加新的 Microsoft 帐户。</span><span class="sxs-lookup"><span data-stu-id="a7082-328">Prevent users from adding new Microsoft accounts to this computer.</span></span>|
|<span data-ttu-id="a7082-329">localSecurityOptionsBlockRemoteLogonWithBlankPassword</span><span class="sxs-lookup"><span data-stu-id="a7082-329">localSecurityOptionsBlockRemoteLogonWithBlankPassword</span></span>|<span data-ttu-id="a7082-330">Boolean</span><span class="sxs-lookup"><span data-stu-id="a7082-330">Boolean</span></span>|<span data-ttu-id="a7082-331">启用不受密码保护的本地帐户从物理设备以外的位置进行登录。默认值为已启用</span><span class="sxs-lookup"><span data-stu-id="a7082-331">Enable Local accounts that are not password protected to log on from locations other than the physical device.Default is enabled</span></span>|
|<span data-ttu-id="a7082-332">localSecurityOptionsDisableAdministratorAccount</span><span class="sxs-lookup"><span data-stu-id="a7082-332">localSecurityOptionsDisableAdministratorAccount</span></span>|<span data-ttu-id="a7082-333">Boolean</span><span class="sxs-lookup"><span data-stu-id="a7082-333">Boolean</span></span>|<span data-ttu-id="a7082-334">确定是否启用或禁用本地管理员帐户。</span><span class="sxs-lookup"><span data-stu-id="a7082-334">Determines whether the Local Administrator account is enabled or disabled.</span></span>|
|<span data-ttu-id="a7082-335">localSecurityOptionsAdministratorAccountName</span><span class="sxs-lookup"><span data-stu-id="a7082-335">localSecurityOptionsAdministratorAccountName</span></span>|<span data-ttu-id="a7082-336">字符串</span><span class="sxs-lookup"><span data-stu-id="a7082-336">String</span></span>|<span data-ttu-id="a7082-337">定义要与帐户 "管理员" 的安全标识符 (SID) 相关联的不同帐户名称。</span><span class="sxs-lookup"><span data-stu-id="a7082-337">Define a different account name to be associated with the security identifier (SID) for the account “Administrator”.</span></span>|
|<span data-ttu-id="a7082-338">localSecurityOptionsDisableGuestAccount</span><span class="sxs-lookup"><span data-stu-id="a7082-338">localSecurityOptionsDisableGuestAccount</span></span>|<span data-ttu-id="a7082-339">Boolean</span><span class="sxs-lookup"><span data-stu-id="a7082-339">Boolean</span></span>|<span data-ttu-id="a7082-340">确定来宾帐户是否已启用或已禁用。</span><span class="sxs-lookup"><span data-stu-id="a7082-340">Determines if the Guest account is enabled or disabled.</span></span>|
|<span data-ttu-id="a7082-341">localSecurityOptionsGuestAccountName</span><span class="sxs-lookup"><span data-stu-id="a7082-341">localSecurityOptionsGuestAccountName</span></span>|<span data-ttu-id="a7082-342">字符串</span><span class="sxs-lookup"><span data-stu-id="a7082-342">String</span></span>|<span data-ttu-id="a7082-343">定义要与帐户 "来宾" 的安全标识符 (SID) 相关联的不同帐户名称。</span><span class="sxs-lookup"><span data-stu-id="a7082-343">Define a different account name to be associated with the security identifier (SID) for the account “Guest”.</span></span>|
|<span data-ttu-id="a7082-344">localSecurityOptionsAllowUndockWithoutHavingToLogon</span><span class="sxs-lookup"><span data-stu-id="a7082-344">localSecurityOptionsAllowUndockWithoutHavingToLogon</span></span>|<span data-ttu-id="a7082-345">Boolean</span><span class="sxs-lookup"><span data-stu-id="a7082-345">Boolean</span></span>|<span data-ttu-id="a7082-346">阻止便携式计算机在无需登录的情况下被移除。</span><span class="sxs-lookup"><span data-stu-id="a7082-346">Prevent a portable computer from being undocked without having to log in.</span></span>|
|<span data-ttu-id="a7082-347">localSecurityOptionsBlockUsersInstallingPrinterDrivers</span><span class="sxs-lookup"><span data-stu-id="a7082-347">localSecurityOptionsBlockUsersInstallingPrinterDrivers</span></span>|<span data-ttu-id="a7082-348">Boolean</span><span class="sxs-lookup"><span data-stu-id="a7082-348">Boolean</span></span>|<span data-ttu-id="a7082-349">仅在将打印机驱动程序连接到共享打印机时, 才将其限制为仅供管理员安装。</span><span class="sxs-lookup"><span data-stu-id="a7082-349">Restrict installing printer drivers as part of connecting to a shared printer to admins only.</span></span>|
|<span data-ttu-id="a7082-350">localSecurityOptionsBlockRemoteOpticalDriveAccess</span><span class="sxs-lookup"><span data-stu-id="a7082-350">localSecurityOptionsBlockRemoteOpticalDriveAccess</span></span>|<span data-ttu-id="a7082-351">Boolean</span><span class="sxs-lookup"><span data-stu-id="a7082-351">Boolean</span></span>|<span data-ttu-id="a7082-352">如果启用此设置, 则仅允许交互式登录用户访问 cd-rom 媒体。</span><span class="sxs-lookup"><span data-stu-id="a7082-352">Enabling this settings allows only interactively logged on user to access CD-ROM media.</span></span>|
|<span data-ttu-id="a7082-353">localSecurityOptionsFormatAndEjectOfRemovableMediaAllowedUser</span><span class="sxs-lookup"><span data-stu-id="a7082-353">localSecurityOptionsFormatAndEjectOfRemovableMediaAllowedUser</span></span>|[<span data-ttu-id="a7082-354">localSecurityOptionsFormatAndEjectOfRemovableMediaAllowedUserType</span><span class="sxs-lookup"><span data-stu-id="a7082-354">localSecurityOptionsFormatAndEjectOfRemovableMediaAllowedUserType</span></span>](../resources/intune-deviceconfig-localsecurityoptionsformatandejectofremovablemediaallowedusertype.md)|<span data-ttu-id="a7082-355">定义允许格式化和弹出可移动 NTFS 媒体的权限。</span><span class="sxs-lookup"><span data-stu-id="a7082-355">Define who is allowed to format and eject removable NTFS media.</span></span> <span data-ttu-id="a7082-356">可取值为：`notConfigured`、`administrators`、`administratorsAndPowerUsers`、`administratorsAndInteractiveUsers`。</span><span class="sxs-lookup"><span data-stu-id="a7082-356">Possible values are: `notConfigured`, `administrators`, `administratorsAndPowerUsers`, `administratorsAndInteractiveUsers`.</span></span>|
|<span data-ttu-id="a7082-357">localSecurityOptionsMachineInactivityLimit</span><span class="sxs-lookup"><span data-stu-id="a7082-357">localSecurityOptionsMachineInactivityLimit</span></span>|<span data-ttu-id="a7082-358">Int32</span><span class="sxs-lookup"><span data-stu-id="a7082-358">Int32</span></span>|<span data-ttu-id="a7082-359">在屏幕保护程序运行之前, 定义交互式桌面登录屏幕上不活动的最长分钟数。</span><span class="sxs-lookup"><span data-stu-id="a7082-359">Define maximum minutes of inactivity on the interactive desktop’s login screen until the screen saver runs.</span></span> <span data-ttu-id="a7082-360">有效值为0至9999</span><span class="sxs-lookup"><span data-stu-id="a7082-360">Valid values 0 to 9999</span></span>|
|<span data-ttu-id="a7082-361">localSecurityOptionsMachineInactivityLimitInMinutes</span><span class="sxs-lookup"><span data-stu-id="a7082-361">localSecurityOptionsMachineInactivityLimitInMinutes</span></span>|<span data-ttu-id="a7082-362">Int32</span><span class="sxs-lookup"><span data-stu-id="a7082-362">Int32</span></span>|<span data-ttu-id="a7082-363">在屏幕保护程序运行之前, 定义交互式桌面登录屏幕上不活动的最长分钟数。</span><span class="sxs-lookup"><span data-stu-id="a7082-363">Define maximum minutes of inactivity on the interactive desktop’s login screen until the screen saver runs.</span></span> <span data-ttu-id="a7082-364">有效值为0至9999</span><span class="sxs-lookup"><span data-stu-id="a7082-364">Valid values 0 to 9999</span></span>|
|<span data-ttu-id="a7082-365">localSecurityOptionsDoNotRequireCtrlAltDel</span><span class="sxs-lookup"><span data-stu-id="a7082-365">localSecurityOptionsDoNotRequireCtrlAltDel</span></span>|<span data-ttu-id="a7082-366">Boolean</span><span class="sxs-lookup"><span data-stu-id="a7082-366">Boolean</span></span>|<span data-ttu-id="a7082-367">要求用户在登录前按 CTRL + ALT + DEL。</span><span class="sxs-lookup"><span data-stu-id="a7082-367">Require CTRL+ALT+DEL to be pressed before a user can log on.</span></span>|
|<span data-ttu-id="a7082-368">localSecurityOptionsHideLastSignedInUser</span><span class="sxs-lookup"><span data-stu-id="a7082-368">localSecurityOptionsHideLastSignedInUser</span></span>|<span data-ttu-id="a7082-369">Boolean</span><span class="sxs-lookup"><span data-stu-id="a7082-369">Boolean</span></span>|<span data-ttu-id="a7082-370">不显示上次在此设备上登录的用户的用户名。</span><span class="sxs-lookup"><span data-stu-id="a7082-370">Do not display the username of the last person who signed in on this device.</span></span>|
|<span data-ttu-id="a7082-371">localSecurityOptionsHideUsernameAtSignIn</span><span class="sxs-lookup"><span data-stu-id="a7082-371">localSecurityOptionsHideUsernameAtSignIn</span></span>|<span data-ttu-id="a7082-372">Boolean</span><span class="sxs-lookup"><span data-stu-id="a7082-372">Boolean</span></span>|<span data-ttu-id="a7082-373">在输入凭据后以及显示设备桌面之前, 请勿显示登录此设备的人员的用户名。</span><span class="sxs-lookup"><span data-stu-id="a7082-373">Do not display the username of the person signing in to this device after credentials are entered and before the device’s desktop is shown.</span></span>|
|<span data-ttu-id="a7082-374">localSecurityOptionsLogOnMessageTitle</span><span class="sxs-lookup"><span data-stu-id="a7082-374">localSecurityOptionsLogOnMessageTitle</span></span>|<span data-ttu-id="a7082-375">字符串</span><span class="sxs-lookup"><span data-stu-id="a7082-375">String</span></span>|<span data-ttu-id="a7082-376">为尝试登录的用户设置消息标题。</span><span class="sxs-lookup"><span data-stu-id="a7082-376">Set message title for users attempting to log in.</span></span>|
|<span data-ttu-id="a7082-377">localSecurityOptionsLogOnMessageText</span><span class="sxs-lookup"><span data-stu-id="a7082-377">localSecurityOptionsLogOnMessageText</span></span>|<span data-ttu-id="a7082-378">字符串</span><span class="sxs-lookup"><span data-stu-id="a7082-378">String</span></span>|<span data-ttu-id="a7082-379">为尝试登录的用户设置消息文本。</span><span class="sxs-lookup"><span data-stu-id="a7082-379">Set message text for users attempting to log in.</span></span>|
|<span data-ttu-id="a7082-380">localSecurityOptionsAllowPKU2UAuthenticationRequests</span><span class="sxs-lookup"><span data-stu-id="a7082-380">localSecurityOptionsAllowPKU2UAuthenticationRequests</span></span>|<span data-ttu-id="a7082-381">Boolean</span><span class="sxs-lookup"><span data-stu-id="a7082-381">Boolean</span></span>|<span data-ttu-id="a7082-382">阻止 PKU2U 对此设备的身份验证请求, 以使用联机标识。</span><span class="sxs-lookup"><span data-stu-id="a7082-382">Block PKU2U authentication requests to this device to use online identities.</span></span>|
|<span data-ttu-id="a7082-383">localSecurityOptionsAllowRemoteCallsToSecurityAccountsManagerHelperBool</span><span class="sxs-lookup"><span data-stu-id="a7082-383">localSecurityOptionsAllowRemoteCallsToSecurityAccountsManagerHelperBool</span></span>|<span data-ttu-id="a7082-384">Boolean</span><span class="sxs-lookup"><span data-stu-id="a7082-384">Boolean</span></span>|<span data-ttu-id="a7082-385">LocalSecurityOptionsAllowRemoteCallsToSecurityAccountsManager 实体的 UI 帮助程序布尔值</span><span class="sxs-lookup"><span data-stu-id="a7082-385">UI helper boolean for LocalSecurityOptionsAllowRemoteCallsToSecurityAccountsManager entity</span></span>|
|<span data-ttu-id="a7082-386">localSecurityOptionsAllowRemoteCallsToSecurityAccountsManager</span><span class="sxs-lookup"><span data-stu-id="a7082-386">localSecurityOptionsAllowRemoteCallsToSecurityAccountsManager</span></span>|<span data-ttu-id="a7082-387">字符串</span><span class="sxs-lookup"><span data-stu-id="a7082-387">String</span></span>|<span data-ttu-id="a7082-388">编辑默认的安全描述符定义语言字符串, 以允许或拒绝用户和组对 SAM 进行远程调用。</span><span class="sxs-lookup"><span data-stu-id="a7082-388">Edit the default Security Descriptor Definition Language string to allow or deny users and groups to make remote calls to the SAM.</span></span>|
|<span data-ttu-id="a7082-389">localSecurityOptionsMinimumSessionSecurityForNtlmSspBasedClients</span><span class="sxs-lookup"><span data-stu-id="a7082-389">localSecurityOptionsMinimumSessionSecurityForNtlmSspBasedClients</span></span>|[<span data-ttu-id="a7082-390">localSecurityOptionsMinimumSessionSecurity</span><span class="sxs-lookup"><span data-stu-id="a7082-390">localSecurityOptionsMinimumSessionSecurity</span></span>](../resources/intune-deviceconfig-localsecurityoptionsminimumsessionsecurity.md)|<span data-ttu-id="a7082-391">此安全设置允许客户端要求协商128位加密和/或 NTLMv2 会话安全性。</span><span class="sxs-lookup"><span data-stu-id="a7082-391">This security setting allows a client to require the negotiation of 128-bit encryption and/or NTLMv2 session security.</span></span> <span data-ttu-id="a7082-392">可取值为：`none`、`requireNtmlV2SessionSecurity`、`require128BitEncryption`、`ntlmV2And128BitEncryption`。</span><span class="sxs-lookup"><span data-stu-id="a7082-392">Possible values are: `none`, `requireNtmlV2SessionSecurity`, `require128BitEncryption`, `ntlmV2And128BitEncryption`.</span></span>|
|<span data-ttu-id="a7082-393">localSecurityOptionsMinimumSessionSecurityForNtlmSspBasedServers</span><span class="sxs-lookup"><span data-stu-id="a7082-393">localSecurityOptionsMinimumSessionSecurityForNtlmSspBasedServers</span></span>|[<span data-ttu-id="a7082-394">localSecurityOptionsMinimumSessionSecurity</span><span class="sxs-lookup"><span data-stu-id="a7082-394">localSecurityOptionsMinimumSessionSecurity</span></span>](../resources/intune-deviceconfig-localsecurityoptionsminimumsessionsecurity.md)|<span data-ttu-id="a7082-395">此安全设置允许服务器要求协商128位加密和/或 NTLMv2 会话安全性。</span><span class="sxs-lookup"><span data-stu-id="a7082-395">This security setting allows a server to require the negotiation of 128-bit encryption and/or NTLMv2 session security.</span></span> <span data-ttu-id="a7082-396">可取值为：`none`、`requireNtmlV2SessionSecurity`、`require128BitEncryption`、`ntlmV2And128BitEncryption`。</span><span class="sxs-lookup"><span data-stu-id="a7082-396">Possible values are: `none`, `requireNtmlV2SessionSecurity`, `require128BitEncryption`, `ntlmV2And128BitEncryption`.</span></span>|
|<span data-ttu-id="a7082-397">lanManagerAuthenticationLevel</span><span class="sxs-lookup"><span data-stu-id="a7082-397">lanManagerAuthenticationLevel</span></span>|[<span data-ttu-id="a7082-398">lanManagerAuthenticationLevel</span><span class="sxs-lookup"><span data-stu-id="a7082-398">lanManagerAuthenticationLevel</span></span>](../resources/intune-deviceconfig-lanmanagerauthenticationlevel.md)|<span data-ttu-id="a7082-399">此安全设置确定用于网络登录的质询/响应身份验证协议。</span><span class="sxs-lookup"><span data-stu-id="a7082-399">This security setting determines which challenge/response authentication protocol is used for network logons.</span></span> <span data-ttu-id="a7082-400">可取值为：`lmAndNltm`、`lmNtlmAndNtlmV2`、`lmAndNtlmOnly`、`lmAndNtlmV2`、`lmNtlmV2AndNotLm`、`lmNtlmV2AndNotLmOrNtm`。</span><span class="sxs-lookup"><span data-stu-id="a7082-400">Possible values are: `lmAndNltm`, `lmNtlmAndNtlmV2`, `lmAndNtlmOnly`, `lmAndNtlmV2`, `lmNtlmV2AndNotLm`, `lmNtlmV2AndNotLmOrNtm`.</span></span>|
|<span data-ttu-id="a7082-401">lanManagerWorkstationDisableInsecureGuestLogons</span><span class="sxs-lookup"><span data-stu-id="a7082-401">lanManagerWorkstationDisableInsecureGuestLogons</span></span>|<span data-ttu-id="a7082-402">Boolean</span><span class="sxs-lookup"><span data-stu-id="a7082-402">Boolean</span></span>|<span data-ttu-id="a7082-403">如果启用, SMB 客户端将允许不安全的来宾登录。</span><span class="sxs-lookup"><span data-stu-id="a7082-403">If enabled,the SMB client will allow insecure guest logons.</span></span> <span data-ttu-id="a7082-404">如果未配置, SMB 客户端将拒绝不安全的来宾登录。</span><span class="sxs-lookup"><span data-stu-id="a7082-404">If not configured, the SMB client will reject insecure guest logons.</span></span>|
|<span data-ttu-id="a7082-405">localSecurityOptionsClearVirtualMemoryPageFile</span><span class="sxs-lookup"><span data-stu-id="a7082-405">localSecurityOptionsClearVirtualMemoryPageFile</span></span>|<span data-ttu-id="a7082-406">Boolean</span><span class="sxs-lookup"><span data-stu-id="a7082-406">Boolean</span></span>|<span data-ttu-id="a7082-407">此安全设置确定在关闭系统时是否清除虚拟内存页面文件。</span><span class="sxs-lookup"><span data-stu-id="a7082-407">This security setting determines whether the virtual memory pagefile is cleared when the system is shut down.</span></span>|
|<span data-ttu-id="a7082-408">localSecurityOptionsAllowSystemToBeShutDownWithoutHavingToLogOn</span><span class="sxs-lookup"><span data-stu-id="a7082-408">localSecurityOptionsAllowSystemToBeShutDownWithoutHavingToLogOn</span></span>|<span data-ttu-id="a7082-409">Boolean</span><span class="sxs-lookup"><span data-stu-id="a7082-409">Boolean</span></span>|<span data-ttu-id="a7082-410">此安全设置确定是否可以在不登录 Windows 的情况下关闭计算机。</span><span class="sxs-lookup"><span data-stu-id="a7082-410">This security setting determines whether a computer can be shut down without having to log on to Windows.</span></span>|
|<span data-ttu-id="a7082-411">localSecurityOptionsAllowUIAccessApplicationElevation</span><span class="sxs-lookup"><span data-stu-id="a7082-411">localSecurityOptionsAllowUIAccessApplicationElevation</span></span>|<span data-ttu-id="a7082-412">Boolean</span><span class="sxs-lookup"><span data-stu-id="a7082-412">Boolean</span></span>|<span data-ttu-id="a7082-413">允许 UIAccess 应用在不使用安全桌面的情况下提示提升。</span><span class="sxs-lookup"><span data-stu-id="a7082-413">Allow UIAccess apps to prompt for elevation without using the secure desktop.</span></span>|
|<span data-ttu-id="a7082-414">localSecurityOptionsVirtualizeFileAndRegistryWriteFailuresToPerUserLocations</span><span class="sxs-lookup"><span data-stu-id="a7082-414">localSecurityOptionsVirtualizeFileAndRegistryWriteFailuresToPerUserLocations</span></span>|<span data-ttu-id="a7082-415">Boolean</span><span class="sxs-lookup"><span data-stu-id="a7082-415">Boolean</span></span>|<span data-ttu-id="a7082-416">将文件和注册表写入失败虚拟化到每个用户位置</span><span class="sxs-lookup"><span data-stu-id="a7082-416">Virtualize file and registry write failures to per user locations</span></span>|
|<span data-ttu-id="a7082-417">localSecurityOptionsOnlyElevateSignedExecutables</span><span class="sxs-lookup"><span data-stu-id="a7082-417">localSecurityOptionsOnlyElevateSignedExecutables</span></span>|<span data-ttu-id="a7082-418">Boolean</span><span class="sxs-lookup"><span data-stu-id="a7082-418">Boolean</span></span>|<span data-ttu-id="a7082-419">对给定的可执行文件强制执行 PKI 证书路径验证, 然后再允许运行该文件。</span><span class="sxs-lookup"><span data-stu-id="a7082-419">Enforce PKI certification path validation for a given executable file before it is permitted to run.</span></span>|
|<span data-ttu-id="a7082-420">localSecurityOptionsAdministratorElevationPromptBehavior</span><span class="sxs-lookup"><span data-stu-id="a7082-420">localSecurityOptionsAdministratorElevationPromptBehavior</span></span>|[<span data-ttu-id="a7082-421">localSecurityOptionsAdministratorElevationPromptBehaviorType</span><span class="sxs-lookup"><span data-stu-id="a7082-421">localSecurityOptionsAdministratorElevationPromptBehaviorType</span></span>](../resources/intune-deviceconfig-localsecurityoptionsadministratorelevationpromptbehaviortype.md)|<span data-ttu-id="a7082-422">在管理员审批模式中定义管理员的提升提示行为。</span><span class="sxs-lookup"><span data-stu-id="a7082-422">Define the behavior of the elevation prompt for admins in Admin Approval Mode.</span></span> <span data-ttu-id="a7082-423">可取值为：`notConfigured`、`elevateWithoutPrompting`、`promptForCredentialsOnTheSecureDesktop`、`promptForConsentOnTheSecureDesktop`、`promptForCredentials`、`promptForConsent` 或 `promptForConsentForNonWindowsBinaries`。</span><span class="sxs-lookup"><span data-stu-id="a7082-423">Possible values are: `notConfigured`, `elevateWithoutPrompting`, `promptForCredentialsOnTheSecureDesktop`, `promptForConsentOnTheSecureDesktop`, `promptForCredentials`, `promptForConsent`, `promptForConsentForNonWindowsBinaries`.</span></span>|
|<span data-ttu-id="a7082-424">localSecurityOptionsStandardUserElevationPromptBehavior</span><span class="sxs-lookup"><span data-stu-id="a7082-424">localSecurityOptionsStandardUserElevationPromptBehavior</span></span>|[<span data-ttu-id="a7082-425">localSecurityOptionsStandardUserElevationPromptBehaviorType</span><span class="sxs-lookup"><span data-stu-id="a7082-425">localSecurityOptionsStandardUserElevationPromptBehaviorType</span></span>](../resources/intune-deviceconfig-localsecurityoptionsstandarduserelevationpromptbehaviortype.md)|<span data-ttu-id="a7082-426">定义标准用户的提升提示行为。</span><span class="sxs-lookup"><span data-stu-id="a7082-426">Define the behavior of the elevation prompt for standard users.</span></span> <span data-ttu-id="a7082-427">可取值为：`notConfigured`、`automaticallyDenyElevationRequests`、`promptForCredentialsOnTheSecureDesktop`、`promptForCredentials`。</span><span class="sxs-lookup"><span data-stu-id="a7082-427">Possible values are: `notConfigured`, `automaticallyDenyElevationRequests`, `promptForCredentialsOnTheSecureDesktop`, `promptForCredentials`.</span></span>|
|<span data-ttu-id="a7082-428">localSecurityOptionsSwitchToSecureDesktopWhenPromptingForElevation</span><span class="sxs-lookup"><span data-stu-id="a7082-428">localSecurityOptionsSwitchToSecureDesktopWhenPromptingForElevation</span></span>|<span data-ttu-id="a7082-429">Boolean</span><span class="sxs-lookup"><span data-stu-id="a7082-429">Boolean</span></span>|<span data-ttu-id="a7082-430">启用所有提升请求以转到交互式用户的桌面, 而不是安全桌面。</span><span class="sxs-lookup"><span data-stu-id="a7082-430">Enable all elevation requests to go to the interactive user's desktop rather than the secure desktop.</span></span> <span data-ttu-id="a7082-431">使用管理员和标准用户的提示行为策略设置。</span><span class="sxs-lookup"><span data-stu-id="a7082-431">Prompt behavior policy settings for admins and standard users are used.</span></span>|
|<span data-ttu-id="a7082-432">localSecurityOptionsDetectApplicationInstallationsAndPromptForElevation</span><span class="sxs-lookup"><span data-stu-id="a7082-432">localSecurityOptionsDetectApplicationInstallationsAndPromptForElevation</span></span>|<span data-ttu-id="a7082-433">Boolean</span><span class="sxs-lookup"><span data-stu-id="a7082-433">Boolean</span></span>|<span data-ttu-id="a7082-434">需要提升权限的应用程序安装将提示管理凭据。默认值为已启用</span><span class="sxs-lookup"><span data-stu-id="a7082-434">App installations requiring elevated privileges will prompt for admin credentials.Default is enabled</span></span>|
|<span data-ttu-id="a7082-435">localSecurityOptionsAllowUIAccessApplicationsForSecureLocations</span><span class="sxs-lookup"><span data-stu-id="a7082-435">localSecurityOptionsAllowUIAccessApplicationsForSecureLocations</span></span>|<span data-ttu-id="a7082-436">Boolean</span><span class="sxs-lookup"><span data-stu-id="a7082-436">Boolean</span></span>|<span data-ttu-id="a7082-437">允许 UIAccess 应用在不使用安全桌面的情况下提示提升。默认值为已启用</span><span class="sxs-lookup"><span data-stu-id="a7082-437">Allow UIAccess apps to prompt for elevation without using the secure desktop.Default is enabled</span></span>|
|<span data-ttu-id="a7082-438">localSecurityOptionsUseAdminApprovalMode</span><span class="sxs-lookup"><span data-stu-id="a7082-438">localSecurityOptionsUseAdminApprovalMode</span></span>|<span data-ttu-id="a7082-439">Boolean</span><span class="sxs-lookup"><span data-stu-id="a7082-439">Boolean</span></span>|<span data-ttu-id="a7082-440">定义内置管理员帐户是使用管理员审批模式, 还是运行所有具有完全管理员权限的应用程序。默认值为已启用</span><span class="sxs-lookup"><span data-stu-id="a7082-440">Defines whether the built-in admin account uses Admin Approval Mode or runs all apps with full admin privileges.Default is enabled</span></span>|
|<span data-ttu-id="a7082-441">localSecurityOptionsUseAdminApprovalModeForAdministrators</span><span class="sxs-lookup"><span data-stu-id="a7082-441">localSecurityOptionsUseAdminApprovalModeForAdministrators</span></span>|<span data-ttu-id="a7082-442">Boolean</span><span class="sxs-lookup"><span data-stu-id="a7082-442">Boolean</span></span>|<span data-ttu-id="a7082-443">定义是否启用管理员批准模式和所有 UAC 策略设置, 默认为启用</span><span class="sxs-lookup"><span data-stu-id="a7082-443">Define whether Admin Approval Mode and all UAC policy settings are enabled, default is enabled</span></span>|
|<span data-ttu-id="a7082-444">localSecurityOptionsInformationShownOnLockScreen</span><span class="sxs-lookup"><span data-stu-id="a7082-444">localSecurityOptionsInformationShownOnLockScreen</span></span>|[<span data-ttu-id="a7082-445">localSecurityOptionsInformationShownOnLockScreenType</span><span class="sxs-lookup"><span data-stu-id="a7082-445">localSecurityOptionsInformationShownOnLockScreenType</span></span>](../resources/intune-deviceconfig-localsecurityoptionsinformationshownonlockscreentype.md)|<span data-ttu-id="a7082-446">配置在会话锁定时显示的用户信息。</span><span class="sxs-lookup"><span data-stu-id="a7082-446">Configure the user information that is displayed when the session is locked.</span></span> <span data-ttu-id="a7082-447">如果未配置, 则显示用户显示名称、域和用户名。</span><span class="sxs-lookup"><span data-stu-id="a7082-447">If not configured, user display name, domain and username are shown.</span></span> <span data-ttu-id="a7082-448">可取值为：`notConfigured`、`userDisplayNameDomainUser`、`userDisplayNameOnly`、`doNotDisplayUser`。</span><span class="sxs-lookup"><span data-stu-id="a7082-448">Possible values are: `notConfigured`, `userDisplayNameDomainUser`, `userDisplayNameOnly`, `doNotDisplayUser`.</span></span>|
|<span data-ttu-id="a7082-449">localSecurityOptionsInformationDisplayedOnLockScreen</span><span class="sxs-lookup"><span data-stu-id="a7082-449">localSecurityOptionsInformationDisplayedOnLockScreen</span></span>|[<span data-ttu-id="a7082-450">localSecurityOptionsInformationDisplayedOnLockScreenType</span><span class="sxs-lookup"><span data-stu-id="a7082-450">localSecurityOptionsInformationDisplayedOnLockScreenType</span></span>](../resources/intune-deviceconfig-localsecurityoptionsinformationdisplayedonlockscreentype.md)|<span data-ttu-id="a7082-451">配置在会话锁定时显示的用户信息。</span><span class="sxs-lookup"><span data-stu-id="a7082-451">Configure the user information that is displayed when the session is locked.</span></span> <span data-ttu-id="a7082-452">如果未配置, 则显示用户显示名称、域和用户名。</span><span class="sxs-lookup"><span data-stu-id="a7082-452">If not configured, user display name, domain and username are shown.</span></span> <span data-ttu-id="a7082-453">可取值为：`notConfigured`、`administrators`、`administratorsAndPowerUsers`、`administratorsAndInteractiveUsers`。</span><span class="sxs-lookup"><span data-stu-id="a7082-453">Possible values are: `notConfigured`, `administrators`, `administratorsAndPowerUsers`, `administratorsAndInteractiveUsers`.</span></span>|
|<span data-ttu-id="a7082-454">localSecurityOptionsDisableClientDigitallySignCommunicationsIfServerAgrees</span><span class="sxs-lookup"><span data-stu-id="a7082-454">localSecurityOptionsDisableClientDigitallySignCommunicationsIfServerAgrees</span></span>|<span data-ttu-id="a7082-455">Boolean</span><span class="sxs-lookup"><span data-stu-id="a7082-455">Boolean</span></span>|<span data-ttu-id="a7082-456">此安全设置确定 smb 客户端是否尝试协商 smb 数据包签名。</span><span class="sxs-lookup"><span data-stu-id="a7082-456">This security setting determines whether the SMB client attempts to negotiate SMB packet signing.</span></span>|
|<span data-ttu-id="a7082-457">localSecurityOptionsClientDigitallySignCommunicationsAlways</span><span class="sxs-lookup"><span data-stu-id="a7082-457">localSecurityOptionsClientDigitallySignCommunicationsAlways</span></span>|<span data-ttu-id="a7082-458">Boolean</span><span class="sxs-lookup"><span data-stu-id="a7082-458">Boolean</span></span>|<span data-ttu-id="a7082-459">此安全设置确定 SMB 客户端组件是否需要数据包签名。</span><span class="sxs-lookup"><span data-stu-id="a7082-459">This security setting determines whether packet signing is required by the SMB client component.</span></span>|
|<span data-ttu-id="a7082-460">localSecurityOptionsClientSendUnencryptedPasswordToThirdPartySMBServers</span><span class="sxs-lookup"><span data-stu-id="a7082-460">localSecurityOptionsClientSendUnencryptedPasswordToThirdPartySMBServers</span></span>|<span data-ttu-id="a7082-461">Boolean</span><span class="sxs-lookup"><span data-stu-id="a7082-461">Boolean</span></span>|<span data-ttu-id="a7082-462">如果启用此安全设置, 则允许服务器消息块 (SMB) 重定向程序将纯文本密码发送到在身份验证过程中不支持密码加密的非 Microsoft SMB 服务器。</span><span class="sxs-lookup"><span data-stu-id="a7082-462">If this security setting is enabled, the Server Message Block (SMB) redirector is allowed to send plaintext passwords to non-Microsoft SMB servers that do not support password encryption during authentication.</span></span>|
|<span data-ttu-id="a7082-463">localSecurityOptionsDisableServerDigitallySignCommunicationsAlways</span><span class="sxs-lookup"><span data-stu-id="a7082-463">localSecurityOptionsDisableServerDigitallySignCommunicationsAlways</span></span>|<span data-ttu-id="a7082-464">Boolean</span><span class="sxs-lookup"><span data-stu-id="a7082-464">Boolean</span></span>|<span data-ttu-id="a7082-465">此安全设置确定 SMB 服务器组件是否需要数据包签名。</span><span class="sxs-lookup"><span data-stu-id="a7082-465">This security setting determines whether packet signing is required by the SMB server component.</span></span>|
|<span data-ttu-id="a7082-466">localSecurityOptionsDisableServerDigitallySignCommunicationsIfClientAgrees</span><span class="sxs-lookup"><span data-stu-id="a7082-466">localSecurityOptionsDisableServerDigitallySignCommunicationsIfClientAgrees</span></span>|<span data-ttu-id="a7082-467">Boolean</span><span class="sxs-lookup"><span data-stu-id="a7082-467">Boolean</span></span>|<span data-ttu-id="a7082-468">此安全设置确定 smb 服务器是否将 smb 数据包签名与请求的客户端协商。</span><span class="sxs-lookup"><span data-stu-id="a7082-468">This security setting determines whether the SMB server will negotiate SMB packet signing with clients that request it.</span></span>|
|<span data-ttu-id="a7082-469">localSecurityOptionsRestrictAnonymousAccessToNamedPipesAndShares</span><span class="sxs-lookup"><span data-stu-id="a7082-469">localSecurityOptionsRestrictAnonymousAccessToNamedPipesAndShares</span></span>|<span data-ttu-id="a7082-470">Boolean</span><span class="sxs-lookup"><span data-stu-id="a7082-470">Boolean</span></span>|<span data-ttu-id="a7082-471">默认情况下, 此安全设置限制可匿名访问且可匿名访问的共享的命名管道设置对共享和管道的匿名访问权限</span><span class="sxs-lookup"><span data-stu-id="a7082-471">By default, this security setting restricts anonymous access to shares and pipes to the settings for named pipes that can be accessed anonymously and Shares that can be accessed anonymously</span></span>|
|<span data-ttu-id="a7082-472">localSecurityOptionsDoNotAllowAnonymousEnumerationOfSAMAccounts</span><span class="sxs-lookup"><span data-stu-id="a7082-472">localSecurityOptionsDoNotAllowAnonymousEnumerationOfSAMAccounts</span></span>|<span data-ttu-id="a7082-473">Boolean</span><span class="sxs-lookup"><span data-stu-id="a7082-473">Boolean</span></span>|<span data-ttu-id="a7082-474">此安全设置确定将向计算机的匿名连接授予的其他权限。</span><span class="sxs-lookup"><span data-stu-id="a7082-474">This security setting determines what additional permissions will be granted for anonymous connections to the computer.</span></span>|
|<span data-ttu-id="a7082-475">localSecurityOptionsAllowAnonymousEnumerationOfSAMAccountsAndShares</span><span class="sxs-lookup"><span data-stu-id="a7082-475">localSecurityOptionsAllowAnonymousEnumerationOfSAMAccountsAndShares</span></span>|<span data-ttu-id="a7082-476">Boolean</span><span class="sxs-lookup"><span data-stu-id="a7082-476">Boolean</span></span>|<span data-ttu-id="a7082-477">此安全设置确定是否允许匿名用户执行某些活动, 如枚举域帐户和网络共享的名称。</span><span class="sxs-lookup"><span data-stu-id="a7082-477">This security setting determines whether to allows anonymous users to perform certain activities, such as enumerating the names of domain accounts and network shares.</span></span>|
|<span data-ttu-id="a7082-478">localSecurityOptionsDoNotStoreLANManagerHashValueOnNextPasswordChange</span><span class="sxs-lookup"><span data-stu-id="a7082-478">localSecurityOptionsDoNotStoreLANManagerHashValueOnNextPasswordChange</span></span>|<span data-ttu-id="a7082-479">Boolean</span><span class="sxs-lookup"><span data-stu-id="a7082-479">Boolean</span></span>|<span data-ttu-id="a7082-480">此安全设置确定在下一次更改密码时, 是否存储新密码的 LAN Manager (LM) 哈希值。</span><span class="sxs-lookup"><span data-stu-id="a7082-480">This security setting determines if, at the next password change, the LAN Manager (LM) hash value for the new password is stored.</span></span> <span data-ttu-id="a7082-481">默认情况下不存储它。</span><span class="sxs-lookup"><span data-stu-id="a7082-481">It’s not stored by default.</span></span>|
|<span data-ttu-id="a7082-482">localSecurityOptionsSmartCardRemovalBehavior</span><span class="sxs-lookup"><span data-stu-id="a7082-482">localSecurityOptionsSmartCardRemovalBehavior</span></span>|[<span data-ttu-id="a7082-483">localSecurityOptionsSmartCardRemovalBehaviorType</span><span class="sxs-lookup"><span data-stu-id="a7082-483">localSecurityOptionsSmartCardRemovalBehaviorType</span></span>](../resources/intune-deviceconfig-localsecurityoptionssmartcardremovalbehaviortype.md)|<span data-ttu-id="a7082-484">此安全设置确定将已登录用户的智能卡从智能卡读卡器中删除时发生的情况。</span><span class="sxs-lookup"><span data-stu-id="a7082-484">This security setting determines what happens when the smart card for a logged-on user is removed from the smart card reader.</span></span> <span data-ttu-id="a7082-485">可取值为：`lockWorkstation`、`noAction`、`forceLogoff`、`disconnectRemoteDesktopSession`。</span><span class="sxs-lookup"><span data-stu-id="a7082-485">Possible values are: `lockWorkstation`, `noAction`, `forceLogoff`, `disconnectRemoteDesktopSession`.</span></span>|
|<span data-ttu-id="a7082-486">defenderSecurityCenterDisableAppBrowserUI</span><span class="sxs-lookup"><span data-stu-id="a7082-486">defenderSecurityCenterDisableAppBrowserUI</span></span>|<span data-ttu-id="a7082-487">Boolean</span><span class="sxs-lookup"><span data-stu-id="a7082-487">Boolean</span></span>|<span data-ttu-id="a7082-488">用于禁用应用程序和浏览器保护区域的显示。</span><span class="sxs-lookup"><span data-stu-id="a7082-488">Used to disable the display of the app and browser protection area.</span></span>|
|<span data-ttu-id="a7082-489">defenderSecurityCenterDisableFamilyUI</span><span class="sxs-lookup"><span data-stu-id="a7082-489">defenderSecurityCenterDisableFamilyUI</span></span>|<span data-ttu-id="a7082-490">Boolean</span><span class="sxs-lookup"><span data-stu-id="a7082-490">Boolean</span></span>|<span data-ttu-id="a7082-491">用于禁用 "家庭选项" 区域的显示。</span><span class="sxs-lookup"><span data-stu-id="a7082-491">Used to disable the display of the family options area.</span></span>|
|<span data-ttu-id="a7082-492">defenderSecurityCenterDisableHealthUI</span><span class="sxs-lookup"><span data-stu-id="a7082-492">defenderSecurityCenterDisableHealthUI</span></span>|<span data-ttu-id="a7082-493">Boolean</span><span class="sxs-lookup"><span data-stu-id="a7082-493">Boolean</span></span>|<span data-ttu-id="a7082-494">用于禁用设备性能和运行状况区域的显示。</span><span class="sxs-lookup"><span data-stu-id="a7082-494">Used to disable the display of the device performance and health area.</span></span>|
|<span data-ttu-id="a7082-495">defenderSecurityCenterDisableNetworkUI</span><span class="sxs-lookup"><span data-stu-id="a7082-495">defenderSecurityCenterDisableNetworkUI</span></span>|<span data-ttu-id="a7082-496">Boolean</span><span class="sxs-lookup"><span data-stu-id="a7082-496">Boolean</span></span>|<span data-ttu-id="a7082-497">用于禁用防火墙和网络防护区域的显示。</span><span class="sxs-lookup"><span data-stu-id="a7082-497">Used to disable the display of the firewall and network protection area.</span></span>|
|<span data-ttu-id="a7082-498">defenderSecurityCenterDisableVirusUI</span><span class="sxs-lookup"><span data-stu-id="a7082-498">defenderSecurityCenterDisableVirusUI</span></span>|<span data-ttu-id="a7082-499">Boolean</span><span class="sxs-lookup"><span data-stu-id="a7082-499">Boolean</span></span>|<span data-ttu-id="a7082-500">用于禁用病毒和威胁防护区域的显示。</span><span class="sxs-lookup"><span data-stu-id="a7082-500">Used to disable the display of the virus and threat protection area.</span></span>|
|<span data-ttu-id="a7082-501">defenderSecurityCenterDisableAccountUI</span><span class="sxs-lookup"><span data-stu-id="a7082-501">defenderSecurityCenterDisableAccountUI</span></span>|<span data-ttu-id="a7082-502">Boolean</span><span class="sxs-lookup"><span data-stu-id="a7082-502">Boolean</span></span>|<span data-ttu-id="a7082-503">用于禁用帐户保护区域的显示。</span><span class="sxs-lookup"><span data-stu-id="a7082-503">Used to disable the display of the account protection area.</span></span>|
|<span data-ttu-id="a7082-504">defenderSecurityCenterDisableClearTpmUI</span><span class="sxs-lookup"><span data-stu-id="a7082-504">defenderSecurityCenterDisableClearTpmUI</span></span>|<span data-ttu-id="a7082-505">Boolean</span><span class="sxs-lookup"><span data-stu-id="a7082-505">Boolean</span></span>|<span data-ttu-id="a7082-506">用于禁用 "清除 TPM" 按钮的显示。</span><span class="sxs-lookup"><span data-stu-id="a7082-506">Used to disable the display of the Clear TPM button.</span></span>|
|<span data-ttu-id="a7082-507">defenderSecurityCenterDisableHardwareUI</span><span class="sxs-lookup"><span data-stu-id="a7082-507">defenderSecurityCenterDisableHardwareUI</span></span>|<span data-ttu-id="a7082-508">Boolean</span><span class="sxs-lookup"><span data-stu-id="a7082-508">Boolean</span></span>|<span data-ttu-id="a7082-509">用于禁用硬件保护区域的显示。</span><span class="sxs-lookup"><span data-stu-id="a7082-509">Used to disable the display of the hardware protection area.</span></span>|
|<span data-ttu-id="a7082-510">defenderSecurityCenterDisableNotificationAreaUI</span><span class="sxs-lookup"><span data-stu-id="a7082-510">defenderSecurityCenterDisableNotificationAreaUI</span></span>|<span data-ttu-id="a7082-511">Boolean</span><span class="sxs-lookup"><span data-stu-id="a7082-511">Boolean</span></span>|<span data-ttu-id="a7082-512">用于禁用通知区域控件的显示。</span><span class="sxs-lookup"><span data-stu-id="a7082-512">Used to disable the display of the notification area control.</span></span> <span data-ttu-id="a7082-513">用户需要注销并登录或重新启动计算机, 此设置才会生效。</span><span class="sxs-lookup"><span data-stu-id="a7082-513">The user needs to either sign out and sign in or reboot the computer for this setting to take effect.</span></span>|
|<span data-ttu-id="a7082-514">defenderSecurityCenterDisableRansomwareUI</span><span class="sxs-lookup"><span data-stu-id="a7082-514">defenderSecurityCenterDisableRansomwareUI</span></span>|<span data-ttu-id="a7082-515">Boolean</span><span class="sxs-lookup"><span data-stu-id="a7082-515">Boolean</span></span>|<span data-ttu-id="a7082-516">用于禁用勒索软件防护区域的显示。</span><span class="sxs-lookup"><span data-stu-id="a7082-516">Used to disable the display of the ransomware protection area.</span></span> |
|<span data-ttu-id="a7082-517">defenderSecurityCenterDisableSecureBootUI</span><span class="sxs-lookup"><span data-stu-id="a7082-517">defenderSecurityCenterDisableSecureBootUI</span></span>|<span data-ttu-id="a7082-518">Boolean</span><span class="sxs-lookup"><span data-stu-id="a7082-518">Boolean</span></span>|<span data-ttu-id="a7082-519">用于在 "设备安全性" 下禁用安全引导区域的显示。</span><span class="sxs-lookup"><span data-stu-id="a7082-519">Used to disable the display of the secure boot area under Device security.</span></span>|
|<span data-ttu-id="a7082-520">defenderSecurityCenterDisableTroubleshootingUI</span><span class="sxs-lookup"><span data-stu-id="a7082-520">defenderSecurityCenterDisableTroubleshootingUI</span></span>|<span data-ttu-id="a7082-521">Boolean</span><span class="sxs-lookup"><span data-stu-id="a7082-521">Boolean</span></span>|<span data-ttu-id="a7082-522">用于在 "设备安全性" 下禁用安全过程故障排除的显示。</span><span class="sxs-lookup"><span data-stu-id="a7082-522">Used to disable the display of the security process troubleshooting under Device security.</span></span>|
|<span data-ttu-id="a7082-523">defenderSecurityCenterDisableVulnerableTpmFirmwareUpdateUI</span><span class="sxs-lookup"><span data-stu-id="a7082-523">defenderSecurityCenterDisableVulnerableTpmFirmwareUpdateUI</span></span>|<span data-ttu-id="a7082-524">Boolean</span><span class="sxs-lookup"><span data-stu-id="a7082-524">Boolean</span></span>|<span data-ttu-id="a7082-525">用于在检测到易受攻击的固件时禁用显示更新 TPM 固件。</span><span class="sxs-lookup"><span data-stu-id="a7082-525">Used to disable the display of update TPM Firmware when a vulnerable firmware is detected.</span></span>|
|<span data-ttu-id="a7082-526">defenderSecurityCenterOrganizationDisplayName</span><span class="sxs-lookup"><span data-stu-id="a7082-526">defenderSecurityCenterOrganizationDisplayName</span></span>|<span data-ttu-id="a7082-527">字符串</span><span class="sxs-lookup"><span data-stu-id="a7082-527">String</span></span>|<span data-ttu-id="a7082-528">向用户显示的公司名称。</span><span class="sxs-lookup"><span data-stu-id="a7082-528">The company name that is displayed to the users.</span></span>|
|<span data-ttu-id="a7082-529">defenderSecurityCenterHelpEmail</span><span class="sxs-lookup"><span data-stu-id="a7082-529">defenderSecurityCenterHelpEmail</span></span>|<span data-ttu-id="a7082-530">字符串</span><span class="sxs-lookup"><span data-stu-id="a7082-530">String</span></span>|<span data-ttu-id="a7082-531">向用户显示的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="a7082-531">The email address that is displayed to users.</span></span>|
|<span data-ttu-id="a7082-532">defenderSecurityCenterHelpPhone</span><span class="sxs-lookup"><span data-stu-id="a7082-532">defenderSecurityCenterHelpPhone</span></span>|<span data-ttu-id="a7082-533">字符串</span><span class="sxs-lookup"><span data-stu-id="a7082-533">String</span></span>|<span data-ttu-id="a7082-534">向用户显示的电话号码或 Skype ID。</span><span class="sxs-lookup"><span data-stu-id="a7082-534">The phone number or Skype ID that is displayed to users.</span></span>|
|<span data-ttu-id="a7082-535">defenderSecurityCenterHelpURL</span><span class="sxs-lookup"><span data-stu-id="a7082-535">defenderSecurityCenterHelpURL</span></span>|<span data-ttu-id="a7082-536">字符串</span><span class="sxs-lookup"><span data-stu-id="a7082-536">String</span></span>|<span data-ttu-id="a7082-537">"帮助" 门户 URL 将向用户显示。</span><span class="sxs-lookup"><span data-stu-id="a7082-537">The help portal URL this is displayed to users.</span></span>|
|<span data-ttu-id="a7082-538">defenderSecurityCenterNotificationsFromApp</span><span class="sxs-lookup"><span data-stu-id="a7082-538">defenderSecurityCenterNotificationsFromApp</span></span>|[<span data-ttu-id="a7082-539">defenderSecurityCenterNotificationsFromAppType</span><span class="sxs-lookup"><span data-stu-id="a7082-539">defenderSecurityCenterNotificationsFromAppType</span></span>](../resources/intune-deviceconfig-defendersecuritycenternotificationsfromapptype.md)|<span data-ttu-id="a7082-540">要从应用程序的显示区域中显示的通知。</span><span class="sxs-lookup"><span data-stu-id="a7082-540">Notifications to show from the displayed areas of app.</span></span> <span data-ttu-id="a7082-541">可取值为：`notConfigured`、`blockNoncriticalNotifications`、`blockAllNotifications`。</span><span class="sxs-lookup"><span data-stu-id="a7082-541">Possible values are: `notConfigured`, `blockNoncriticalNotifications`, `blockAllNotifications`.</span></span>|
|<span data-ttu-id="a7082-542">defenderSecurityCenterITContactDisplay</span><span class="sxs-lookup"><span data-stu-id="a7082-542">defenderSecurityCenterITContactDisplay</span></span>|[<span data-ttu-id="a7082-543">defenderSecurityCenterITContactDisplayType</span><span class="sxs-lookup"><span data-stu-id="a7082-543">defenderSecurityCenterITContactDisplayType</span></span>](../resources/intune-deviceconfig-defendersecuritycenteritcontactdisplaytype.md)|<span data-ttu-id="a7082-544">配置向最终用户显示 IT 联系人信息的位置。</span><span class="sxs-lookup"><span data-stu-id="a7082-544">Configure where to display IT contact information to end users.</span></span> <span data-ttu-id="a7082-545">可取值为：`notConfigured`、`displayInAppAndInNotifications`、`displayOnlyInApp`、`displayOnlyInNotifications`。</span><span class="sxs-lookup"><span data-stu-id="a7082-545">Possible values are: `notConfigured`, `displayInAppAndInNotifications`, `displayOnlyInApp`, `displayOnlyInNotifications`.</span></span>|
|<span data-ttu-id="a7082-546">firewallBlockStatefulFTP</span><span class="sxs-lookup"><span data-stu-id="a7082-546">firewallBlockStatefulFTP</span></span>|<span data-ttu-id="a7082-547">Boolean</span><span class="sxs-lookup"><span data-stu-id="a7082-547">Boolean</span></span>|<span data-ttu-id="a7082-548">阻止到设备的有状态 FTP 连接</span><span class="sxs-lookup"><span data-stu-id="a7082-548">Blocks stateful FTP connections to the device</span></span>|
|<span data-ttu-id="a7082-549">firewallIdleTimeoutForSecurityAssociationInSeconds</span><span class="sxs-lookup"><span data-stu-id="a7082-549">firewallIdleTimeoutForSecurityAssociationInSeconds</span></span>|<span data-ttu-id="a7082-550">Int32</span><span class="sxs-lookup"><span data-stu-id="a7082-550">Int32</span></span>|<span data-ttu-id="a7082-551">配置安全关联的空闲超时（以秒为单位），值范围为 300 到 3600（包括这两个值）。</span><span class="sxs-lookup"><span data-stu-id="a7082-551">Configures the idle timeout for security associations, in seconds, from 300 to 3600 inclusive.</span></span> <span data-ttu-id="a7082-552">这是一个时间段，在此之后安全关联将过期并被删除。</span><span class="sxs-lookup"><span data-stu-id="a7082-552">This is the period after which security associations will expire and be deleted.</span></span> <span data-ttu-id="a7082-553">有效值为 300 至 3600</span><span class="sxs-lookup"><span data-stu-id="a7082-553">Valid values 300 to 3600</span></span>|
|<span data-ttu-id="a7082-554">firewallPreSharedKeyEncodingMethod</span><span class="sxs-lookup"><span data-stu-id="a7082-554">firewallPreSharedKeyEncodingMethod</span></span>|[<span data-ttu-id="a7082-555">firewallPreSharedKeyEncodingMethodType</span><span class="sxs-lookup"><span data-stu-id="a7082-555">firewallPreSharedKeyEncodingMethodType</span></span>](../resources/intune-deviceconfig-firewallpresharedkeyencodingmethodtype.md)|<span data-ttu-id="a7082-556">选择要使用的预共享密钥编码。</span><span class="sxs-lookup"><span data-stu-id="a7082-556">Select the preshared key encoding to be used.</span></span> <span data-ttu-id="a7082-557">可取值为：`deviceDefault`、`none`、`utF8`。</span><span class="sxs-lookup"><span data-stu-id="a7082-557">Possible values are: `deviceDefault`, `none`, `utF8`.</span></span>|
|<span data-ttu-id="a7082-558">firewallIPSecExemptionsAllowNeighborDiscovery</span><span class="sxs-lookup"><span data-stu-id="a7082-558">firewallIPSecExemptionsAllowNeighborDiscovery</span></span>|<span data-ttu-id="a7082-559">Boolean</span><span class="sxs-lookup"><span data-stu-id="a7082-559">Boolean</span></span>|<span data-ttu-id="a7082-560">配置 IPSec 免除项以允许邻居发现 IPv6 ICMP 类型代码</span><span class="sxs-lookup"><span data-stu-id="a7082-560">Configures IPSec exemptions to allow neighbor discovery IPv6 ICMP type-codes</span></span>|
|<span data-ttu-id="a7082-561">firewallIPSecExemptionsAllowICMP</span><span class="sxs-lookup"><span data-stu-id="a7082-561">firewallIPSecExemptionsAllowICMP</span></span>|<span data-ttu-id="a7082-562">Boolean</span><span class="sxs-lookup"><span data-stu-id="a7082-562">Boolean</span></span>|<span data-ttu-id="a7082-563">配置 IPSec 免除项以允许 ICMP</span><span class="sxs-lookup"><span data-stu-id="a7082-563">Configures IPSec exemptions to allow ICMP</span></span>|
|<span data-ttu-id="a7082-564">firewallIPSecExemptionsAllowRouterDiscovery</span><span class="sxs-lookup"><span data-stu-id="a7082-564">firewallIPSecExemptionsAllowRouterDiscovery</span></span>|<span data-ttu-id="a7082-565">Boolean</span><span class="sxs-lookup"><span data-stu-id="a7082-565">Boolean</span></span>|<span data-ttu-id="a7082-566">配置 IPSec 免除项以允许路由器发现 IPv6 ICMP 类型代码</span><span class="sxs-lookup"><span data-stu-id="a7082-566">Configures IPSec exemptions to allow router discovery IPv6 ICMP type-codes</span></span>|
|<span data-ttu-id="a7082-567">firewallIPSecExemptionsAllowDHCP</span><span class="sxs-lookup"><span data-stu-id="a7082-567">firewallIPSecExemptionsAllowDHCP</span></span>|<span data-ttu-id="a7082-568">Boolean</span><span class="sxs-lookup"><span data-stu-id="a7082-568">Boolean</span></span>|<span data-ttu-id="a7082-569">配置 IPSec 免除项以允许 IPv4 和 IPv6 DHCP 通信</span><span class="sxs-lookup"><span data-stu-id="a7082-569">Configures IPSec exemptions to allow both IPv4 and IPv6 DHCP traffic</span></span>|
|<span data-ttu-id="a7082-570">firewallCertificateRevocationListCheckMethod</span><span class="sxs-lookup"><span data-stu-id="a7082-570">firewallCertificateRevocationListCheckMethod</span></span>|[<span data-ttu-id="a7082-571">firewallCertificateRevocationListCheckMethodType</span><span class="sxs-lookup"><span data-stu-id="a7082-571">firewallCertificateRevocationListCheckMethodType</span></span>](../resources/intune-deviceconfig-firewallcertificaterevocationlistcheckmethodtype.md)|<span data-ttu-id="a7082-572">指定如何强制执行证书吊销列表。</span><span class="sxs-lookup"><span data-stu-id="a7082-572">Specify how the certificate revocation list is to be enforced.</span></span> <span data-ttu-id="a7082-573">可取值为：`deviceDefault`、`none`、`attempt`、`require`。</span><span class="sxs-lookup"><span data-stu-id="a7082-573">Possible values are: `deviceDefault`, `none`, `attempt`, `require`.</span></span>|
|<span data-ttu-id="a7082-574">firewallMergeKeyingModuleSettings</span><span class="sxs-lookup"><span data-stu-id="a7082-574">firewallMergeKeyingModuleSettings</span></span>|<span data-ttu-id="a7082-575">Boolean</span><span class="sxs-lookup"><span data-stu-id="a7082-575">Boolean</span></span>|<span data-ttu-id="a7082-576">如果键控模块不完全支持身份验证集，请指示模块仅忽略不受支持的身份验证套件而不是整个集</span><span class="sxs-lookup"><span data-stu-id="a7082-576">If an authentication set is not fully supported by a keying module, direct the module to ignore only unsupported authentication suites rather than the entire set</span></span>|
|<span data-ttu-id="a7082-577">firewallPacketQueueingMethod</span><span class="sxs-lookup"><span data-stu-id="a7082-577">firewallPacketQueueingMethod</span></span>|[<span data-ttu-id="a7082-578">firewallPacketQueueingMethodType</span><span class="sxs-lookup"><span data-stu-id="a7082-578">firewallPacketQueueingMethodType</span></span>](../resources/intune-deviceconfig-firewallpacketqueueingmethodtype.md)|<span data-ttu-id="a7082-579">配置如何在隧道网关应用场景中应用数据包排队。</span><span class="sxs-lookup"><span data-stu-id="a7082-579">Configures how packet queueing should be applied in the tunnel gateway scenario.</span></span> <span data-ttu-id="a7082-580">可取值为：`deviceDefault`、`disabled`、`queueInbound`、`queueOutbound` 或 `queueBoth`。</span><span class="sxs-lookup"><span data-stu-id="a7082-580">Possible values are: `deviceDefault`, `disabled`, `queueInbound`, `queueOutbound`, `queueBoth`.</span></span>|
|<span data-ttu-id="a7082-581">firewallProfileDomain</span><span class="sxs-lookup"><span data-stu-id="a7082-581">firewallProfileDomain</span></span>|[<span data-ttu-id="a7082-582">windowsFirewallNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="a7082-582">windowsFirewallNetworkProfile</span></span>](../resources/intune-deviceconfig-windowsfirewallnetworkprofile.md)|<span data-ttu-id="a7082-583">配置域网络的防火墙配置文件设置</span><span class="sxs-lookup"><span data-stu-id="a7082-583">Configures the firewall profile settings for domain networks</span></span>|
|<span data-ttu-id="a7082-584">firewallProfilePublic</span><span class="sxs-lookup"><span data-stu-id="a7082-584">firewallProfilePublic</span></span>|[<span data-ttu-id="a7082-585">windowsFirewallNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="a7082-585">windowsFirewallNetworkProfile</span></span>](../resources/intune-deviceconfig-windowsfirewallnetworkprofile.md)|<span data-ttu-id="a7082-586">配置公用网络的防火墙配置文件设置</span><span class="sxs-lookup"><span data-stu-id="a7082-586">Configures the firewall profile settings for public networks</span></span>|
|<span data-ttu-id="a7082-587">firewallProfilePrivate</span><span class="sxs-lookup"><span data-stu-id="a7082-587">firewallProfilePrivate</span></span>|[<span data-ttu-id="a7082-588">windowsFirewallNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="a7082-588">windowsFirewallNetworkProfile</span></span>](../resources/intune-deviceconfig-windowsfirewallnetworkprofile.md)|<span data-ttu-id="a7082-589">配置专用网络的防火墙配置文件设置</span><span class="sxs-lookup"><span data-stu-id="a7082-589">Configures the firewall profile settings for private networks</span></span>|
|<span data-ttu-id="a7082-590">defenderAdobeReaderLaunchChildProcess</span><span class="sxs-lookup"><span data-stu-id="a7082-590">defenderAdobeReaderLaunchChildProcess</span></span>|[<span data-ttu-id="a7082-591">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="a7082-591">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="a7082-592">值, 该值指示 Adobe Reader 创建子进程的行为。</span><span class="sxs-lookup"><span data-stu-id="a7082-592">Value indicating the behavior of Adobe Reader from creating child processes.</span></span> <span data-ttu-id="a7082-593">可取值为：`userDefined`、`enable`、`auditMode`。</span><span class="sxs-lookup"><span data-stu-id="a7082-593">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="a7082-594">defenderAttackSurfaceReductionExcludedPaths</span><span class="sxs-lookup"><span data-stu-id="a7082-594">defenderAttackSurfaceReductionExcludedPaths</span></span>|<span data-ttu-id="a7082-595">String 集合</span><span class="sxs-lookup"><span data-stu-id="a7082-595">String collection</span></span>|<span data-ttu-id="a7082-596">要从攻击面减少规则中排除的 exe 文件和文件夹的列表</span><span class="sxs-lookup"><span data-stu-id="a7082-596">List of exe files and folders to be excluded from attack surface reduction rules</span></span>|
|<span data-ttu-id="a7082-597">defenderOfficeAppsOtherProcessInjectionType</span><span class="sxs-lookup"><span data-stu-id="a7082-597">defenderOfficeAppsOtherProcessInjectionType</span></span>|[<span data-ttu-id="a7082-598">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="a7082-598">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="a7082-599">值, 该值指示插入到其他进程中的 Office 应用程序的行为。</span><span class="sxs-lookup"><span data-stu-id="a7082-599">Value indicating the behavior of Office applications injecting into other processes.</span></span> <span data-ttu-id="a7082-600">可取值为：`userDefined`、`block`、`auditMode`。</span><span class="sxs-lookup"><span data-stu-id="a7082-600">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="a7082-601">defenderOfficeAppsOtherProcessInjection</span><span class="sxs-lookup"><span data-stu-id="a7082-601">defenderOfficeAppsOtherProcessInjection</span></span>|[<span data-ttu-id="a7082-602">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="a7082-602">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="a7082-603">值, 该值指示插入到其他进程中的 Office 应用程序的行为。</span><span class="sxs-lookup"><span data-stu-id="a7082-603">Value indicating the behavior of  Office applications injecting into other processes.</span></span> <span data-ttu-id="a7082-604">可取值为：`userDefined`、`enable`、`auditMode`。</span><span class="sxs-lookup"><span data-stu-id="a7082-604">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="a7082-605">defenderOfficeCommunicationAppsLaunchChildProcess</span><span class="sxs-lookup"><span data-stu-id="a7082-605">defenderOfficeCommunicationAppsLaunchChildProcess</span></span>|[<span data-ttu-id="a7082-606">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="a7082-606">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="a7082-607">值, 该值指示 Office 通信应用程序 (包括 Microsoft Outlook) 在创建子进程时的行为。</span><span class="sxs-lookup"><span data-stu-id="a7082-607">Value indicating the behavior of Office communication applications, including Microsoft Outlook, from creating child processes.</span></span> <span data-ttu-id="a7082-608">可取值为：`userDefined`、`enable`、`auditMode`。</span><span class="sxs-lookup"><span data-stu-id="a7082-608">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="a7082-609">defenderOfficeAppsExecutableContentCreationOrLaunchType</span><span class="sxs-lookup"><span data-stu-id="a7082-609">defenderOfficeAppsExecutableContentCreationOrLaunchType</span></span>|[<span data-ttu-id="a7082-610">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="a7082-610">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="a7082-611">值, 该值指示 Office 应用程序/宏创建或启动可执行内容的行为。</span><span class="sxs-lookup"><span data-stu-id="a7082-611">Value indicating the behavior of Office applications/macros creating or launching executable content.</span></span> <span data-ttu-id="a7082-612">可取值为：`userDefined`、`block`、`auditMode`。</span><span class="sxs-lookup"><span data-stu-id="a7082-612">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="a7082-613">defenderOfficeAppsExecutableContentCreationOrLaunch</span><span class="sxs-lookup"><span data-stu-id="a7082-613">defenderOfficeAppsExecutableContentCreationOrLaunch</span></span>|[<span data-ttu-id="a7082-614">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="a7082-614">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="a7082-615">值, 该值指示 Office 应用程序/宏创建或启动可执行内容的行为。</span><span class="sxs-lookup"><span data-stu-id="a7082-615">Value indicating the behavior of Office applications/macros creating or launching executable content.</span></span> <span data-ttu-id="a7082-616">可取值为：`userDefined`、`enable`、`auditMode`。</span><span class="sxs-lookup"><span data-stu-id="a7082-616">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="a7082-617">defenderOfficeAppsLaunchChildProcessType</span><span class="sxs-lookup"><span data-stu-id="a7082-617">defenderOfficeAppsLaunchChildProcessType</span></span>|[<span data-ttu-id="a7082-618">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="a7082-618">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="a7082-619">值, 该值指示 Office 应用程序启动子进程的行为。</span><span class="sxs-lookup"><span data-stu-id="a7082-619">Value indicating the behavior of Office application launching child processes.</span></span> <span data-ttu-id="a7082-620">可取值为：`userDefined`、`block`、`auditMode`。</span><span class="sxs-lookup"><span data-stu-id="a7082-620">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="a7082-621">defenderOfficeAppsLaunchChildProcess</span><span class="sxs-lookup"><span data-stu-id="a7082-621">defenderOfficeAppsLaunchChildProcess</span></span>|[<span data-ttu-id="a7082-622">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="a7082-622">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="a7082-623">值, 该值指示 Office 应用程序启动子进程的行为。</span><span class="sxs-lookup"><span data-stu-id="a7082-623">Value indicating the behavior of Office application launching child processes.</span></span> <span data-ttu-id="a7082-624">可取值为：`userDefined`、`enable`、`auditMode`。</span><span class="sxs-lookup"><span data-stu-id="a7082-624">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="a7082-625">defenderOfficeMacroCodeAllowWin32ImportsType</span><span class="sxs-lookup"><span data-stu-id="a7082-625">defenderOfficeMacroCodeAllowWin32ImportsType</span></span>|[<span data-ttu-id="a7082-626">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="a7082-626">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="a7082-627">值, 该值指示从 Office 中的宏代码的 Win32 导入行为。</span><span class="sxs-lookup"><span data-stu-id="a7082-627">Value indicating the behavior of Win32 imports from Macro code in Office.</span></span> <span data-ttu-id="a7082-628">可取值为：`userDefined`、`block`、`auditMode`。</span><span class="sxs-lookup"><span data-stu-id="a7082-628">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="a7082-629">defenderOfficeMacroCodeAllowWin32Imports</span><span class="sxs-lookup"><span data-stu-id="a7082-629">defenderOfficeMacroCodeAllowWin32Imports</span></span>|[<span data-ttu-id="a7082-630">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="a7082-630">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="a7082-631">值, 该值指示从 Office 中的宏代码的 Win32 导入行为。</span><span class="sxs-lookup"><span data-stu-id="a7082-631">Value indicating the behavior of Win32 imports from Macro code in Office.</span></span> <span data-ttu-id="a7082-632">可取值为：`userDefined`、`enable`、`auditMode`。</span><span class="sxs-lookup"><span data-stu-id="a7082-632">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="a7082-633">defenderScriptObfuscatedMacroCodeType</span><span class="sxs-lookup"><span data-stu-id="a7082-633">defenderScriptObfuscatedMacroCodeType</span></span>|[<span data-ttu-id="a7082-634">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="a7082-634">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="a7082-635">值, 该值指示模糊的 js/vbs/ps/宏代码的行为。</span><span class="sxs-lookup"><span data-stu-id="a7082-635">Value indicating the behavior of obfuscated js/vbs/ps/macro code.</span></span> <span data-ttu-id="a7082-636">可取值为：`userDefined`、`block`、`auditMode`。</span><span class="sxs-lookup"><span data-stu-id="a7082-636">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="a7082-637">defenderScriptObfuscatedMacroCode</span><span class="sxs-lookup"><span data-stu-id="a7082-637">defenderScriptObfuscatedMacroCode</span></span>|[<span data-ttu-id="a7082-638">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="a7082-638">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="a7082-639">值, 该值指示模糊的 js/vbs/ps/宏代码的行为。</span><span class="sxs-lookup"><span data-stu-id="a7082-639">Value indicating the behavior of obfuscated js/vbs/ps/macro code.</span></span> <span data-ttu-id="a7082-640">可取值为：`userDefined`、`enable`、`auditMode`。</span><span class="sxs-lookup"><span data-stu-id="a7082-640">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="a7082-641">defenderScriptDownloadedPayloadExecutionType</span><span class="sxs-lookup"><span data-stu-id="a7082-641">defenderScriptDownloadedPayloadExecutionType</span></span>|[<span data-ttu-id="a7082-642">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="a7082-642">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="a7082-643">值, 该值指示从 Internet 下载的 js/vbs 执行负载的行为。</span><span class="sxs-lookup"><span data-stu-id="a7082-643">Value indicating the behavior of js/vbs executing payload downloaded from Internet.</span></span> <span data-ttu-id="a7082-644">可取值为：`userDefined`、`block`、`auditMode`。</span><span class="sxs-lookup"><span data-stu-id="a7082-644">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="a7082-645">defenderScriptDownloadedPayloadExecution</span><span class="sxs-lookup"><span data-stu-id="a7082-645">defenderScriptDownloadedPayloadExecution</span></span>|[<span data-ttu-id="a7082-646">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="a7082-646">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="a7082-647">值, 该值指示从 Internet 下载的 js/vbs 执行负载的行为。</span><span class="sxs-lookup"><span data-stu-id="a7082-647">Value indicating the behavior of js/vbs executing payload downloaded from Internet.</span></span> <span data-ttu-id="a7082-648">可取值为：`userDefined`、`enable`、`auditMode`。</span><span class="sxs-lookup"><span data-stu-id="a7082-648">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="a7082-649">defenderPreventCredentialStealingType</span><span class="sxs-lookup"><span data-stu-id="a7082-649">defenderPreventCredentialStealingType</span></span>|[<span data-ttu-id="a7082-650">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="a7082-650">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="a7082-651">值, 该值指示是否允许从 Windows 本地安全机构子系统中盗取凭据。</span><span class="sxs-lookup"><span data-stu-id="a7082-651">Value indicating if credential stealing from the Windows local security authority subsystem is permitted.</span></span> <span data-ttu-id="a7082-652">可取值为：`userDefined`、`enable`、`auditMode`。</span><span class="sxs-lookup"><span data-stu-id="a7082-652">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="a7082-653">defenderProcessCreationType</span><span class="sxs-lookup"><span data-stu-id="a7082-653">defenderProcessCreationType</span></span>|[<span data-ttu-id="a7082-654">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="a7082-654">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="a7082-655">一个值, 该值指示对源自 PSExec 和 WMI 命令的进程创建的响应。</span><span class="sxs-lookup"><span data-stu-id="a7082-655">Value indicating response to process creations originating from PSExec and WMI commands.</span></span> <span data-ttu-id="a7082-656">可取值为：`userDefined`、`block`、`auditMode`。</span><span class="sxs-lookup"><span data-stu-id="a7082-656">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="a7082-657">defenderProcessCreation</span><span class="sxs-lookup"><span data-stu-id="a7082-657">defenderProcessCreation</span></span>|[<span data-ttu-id="a7082-658">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="a7082-658">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="a7082-659">一个值, 该值指示对源自 PSExec 和 WMI 命令的进程创建的响应。</span><span class="sxs-lookup"><span data-stu-id="a7082-659">Value indicating response to process creations originating from PSExec and WMI commands.</span></span> <span data-ttu-id="a7082-660">可取值为：`userDefined`、`enable`、`auditMode`。</span><span class="sxs-lookup"><span data-stu-id="a7082-660">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="a7082-661">defenderUntrustedUSBProcessType</span><span class="sxs-lookup"><span data-stu-id="a7082-661">defenderUntrustedUSBProcessType</span></span>|[<span data-ttu-id="a7082-662">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="a7082-662">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="a7082-663">指示对从 USB 运行的不受信任和未签名进程的响应的值。</span><span class="sxs-lookup"><span data-stu-id="a7082-663">Value indicating response to untrusted and unsigned processes that run from USB.</span></span> <span data-ttu-id="a7082-664">可取值为：`userDefined`、`block`、`auditMode`。</span><span class="sxs-lookup"><span data-stu-id="a7082-664">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="a7082-665">defenderUntrustedUSBProcess</span><span class="sxs-lookup"><span data-stu-id="a7082-665">defenderUntrustedUSBProcess</span></span>|[<span data-ttu-id="a7082-666">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="a7082-666">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="a7082-667">指示对从 USB 运行的不受信任和未签名进程的响应的值。</span><span class="sxs-lookup"><span data-stu-id="a7082-667">Value indicating response to untrusted and unsigned processes that run from USB.</span></span> <span data-ttu-id="a7082-668">可取值为：`userDefined`、`enable`、`auditMode`。</span><span class="sxs-lookup"><span data-stu-id="a7082-668">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="a7082-669">defenderUntrustedExecutableType</span><span class="sxs-lookup"><span data-stu-id="a7082-669">defenderUntrustedExecutableType</span></span>|[<span data-ttu-id="a7082-670">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="a7082-670">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="a7082-671">指示对不符合流行、年龄或受信任列表条件的可执行文件的响应的值。</span><span class="sxs-lookup"><span data-stu-id="a7082-671">Value indicating response to executables that don't meet a prevalence, age, or trusted list criteria.</span></span> <span data-ttu-id="a7082-672">可取值为：`userDefined`、`block`、`auditMode`。</span><span class="sxs-lookup"><span data-stu-id="a7082-672">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="a7082-673">defenderUntrustedExecutable</span><span class="sxs-lookup"><span data-stu-id="a7082-673">defenderUntrustedExecutable</span></span>|[<span data-ttu-id="a7082-674">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="a7082-674">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="a7082-675">指示对不符合流行、年龄或受信任列表条件的可执行文件的响应的值。</span><span class="sxs-lookup"><span data-stu-id="a7082-675">Value indicating response to executables that don't meet a prevalence, age, or trusted list criteria.</span></span> <span data-ttu-id="a7082-676">可取值为：`userDefined`、`enable`、`auditMode`。</span><span class="sxs-lookup"><span data-stu-id="a7082-676">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="a7082-677">defenderEmailContentExecutionType</span><span class="sxs-lookup"><span data-stu-id="a7082-677">defenderEmailContentExecutionType</span></span>|[<span data-ttu-id="a7082-678">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="a7082-678">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="a7082-679">一个值, 该值指示是否应从电子邮件 (web 邮件/邮件客户端) 中删除可执行内容 (exe、dll、ps、js、vbs 等) 的执行。</span><span class="sxs-lookup"><span data-stu-id="a7082-679">Value indicating if execution of executable content (exe, dll, ps, js, vbs, etc) should be dropped from email (webmail/mail-client).</span></span> <span data-ttu-id="a7082-680">可取值为：`userDefined`、`block`、`auditMode`。</span><span class="sxs-lookup"><span data-stu-id="a7082-680">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="a7082-681">defenderEmailContentExecution</span><span class="sxs-lookup"><span data-stu-id="a7082-681">defenderEmailContentExecution</span></span>|[<span data-ttu-id="a7082-682">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="a7082-682">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="a7082-683">一个值, 该值指示是否应从电子邮件 (web 邮件/邮件客户端) 中删除可执行内容 (exe、dll、ps、js、vbs 等) 的执行。</span><span class="sxs-lookup"><span data-stu-id="a7082-683">Value indicating if execution of executable content (exe, dll, ps, js, vbs, etc) should be dropped from email (webmail/mail-client).</span></span> <span data-ttu-id="a7082-684">可取值为：`userDefined`、`enable`、`auditMode`。</span><span class="sxs-lookup"><span data-stu-id="a7082-684">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="a7082-685">defenderAdvancedRansomewareProtectionType</span><span class="sxs-lookup"><span data-stu-id="a7082-685">defenderAdvancedRansomewareProtectionType</span></span>|[<span data-ttu-id="a7082-686">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="a7082-686">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="a7082-687">指示使用针对 ransomeware 的高级防护的值。</span><span class="sxs-lookup"><span data-stu-id="a7082-687">Value indicating use of advanced protection against ransomeware.</span></span> <span data-ttu-id="a7082-688">可取值为：`userDefined`、`enable`、`auditMode`。</span><span class="sxs-lookup"><span data-stu-id="a7082-688">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="a7082-689">defenderGuardMyFoldersType</span><span class="sxs-lookup"><span data-stu-id="a7082-689">defenderGuardMyFoldersType</span></span>|[<span data-ttu-id="a7082-690">folderProtectionType</span><span class="sxs-lookup"><span data-stu-id="a7082-690">folderProtectionType</span></span>](../resources/intune-deviceconfig-folderprotectiontype.md)|<span data-ttu-id="a7082-691">值, 该值指示受保护文件夹的行为。</span><span class="sxs-lookup"><span data-stu-id="a7082-691">Value indicating the behavior of protected folders.</span></span> <span data-ttu-id="a7082-692">可取值为：`userDefined`、`enable`、`auditMode`、`blockDiskModification` 或 `auditDiskModification`。</span><span class="sxs-lookup"><span data-stu-id="a7082-692">Possible values are: `userDefined`, `enable`, `auditMode`, `blockDiskModification`, `auditDiskModification`.</span></span>|
|<span data-ttu-id="a7082-693">defenderGuardedFoldersAllowedAppPaths</span><span class="sxs-lookup"><span data-stu-id="a7082-693">defenderGuardedFoldersAllowedAppPaths</span></span>|<span data-ttu-id="a7082-694">String collection</span><span class="sxs-lookup"><span data-stu-id="a7082-694">String collection</span></span>|<span data-ttu-id="a7082-695">允许访问受保护文件夹的 exe 路径列表</span><span class="sxs-lookup"><span data-stu-id="a7082-695">List of paths to exe that are allowed to access protected folders</span></span>|
|<span data-ttu-id="a7082-696">defenderAdditionalGuardedFolders</span><span class="sxs-lookup"><span data-stu-id="a7082-696">defenderAdditionalGuardedFolders</span></span>|<span data-ttu-id="a7082-697">String 集合</span><span class="sxs-lookup"><span data-stu-id="a7082-697">String collection</span></span>|<span data-ttu-id="a7082-698">要添加到受保护文件夹列表的文件夹路径列表</span><span class="sxs-lookup"><span data-stu-id="a7082-698">List of folder paths to be added to the list of protected folders</span></span>|
|<span data-ttu-id="a7082-699">defenderNetworkProtectionType</span><span class="sxs-lookup"><span data-stu-id="a7082-699">defenderNetworkProtectionType</span></span>|[<span data-ttu-id="a7082-700">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="a7082-700">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="a7082-701">值, 该值指示 NetworkProtection 的行为。</span><span class="sxs-lookup"><span data-stu-id="a7082-701">Value indicating the behavior of NetworkProtection.</span></span> <span data-ttu-id="a7082-702">可取值为：`userDefined`、`enable`、`auditMode`。</span><span class="sxs-lookup"><span data-stu-id="a7082-702">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="a7082-703">defenderExploitProtectionXml</span><span class="sxs-lookup"><span data-stu-id="a7082-703">defenderExploitProtectionXml</span></span>|<span data-ttu-id="a7082-704">Binary</span><span class="sxs-lookup"><span data-stu-id="a7082-704">Binary</span></span>|<span data-ttu-id="a7082-705">包含有关 Exploit Protection 详细信息的 xml 内容。</span><span class="sxs-lookup"><span data-stu-id="a7082-705">Xml content containing information regarding exploit protection details.</span></span>|
|<span data-ttu-id="a7082-706">defenderExploitProtectionXmlFileName</span><span class="sxs-lookup"><span data-stu-id="a7082-706">defenderExploitProtectionXmlFileName</span></span>|<span data-ttu-id="a7082-707">String</span><span class="sxs-lookup"><span data-stu-id="a7082-707">String</span></span>|<span data-ttu-id="a7082-708">从中获取 DefenderExploitProtectionXml 的文件的名称。</span><span class="sxs-lookup"><span data-stu-id="a7082-708">Name of the file from which DefenderExploitProtectionXml was obtained.</span></span>|
|<span data-ttu-id="a7082-709">defenderSecurityCenterBlockExploitProtectionOverride</span><span class="sxs-lookup"><span data-stu-id="a7082-709">defenderSecurityCenterBlockExploitProtectionOverride</span></span>|<span data-ttu-id="a7082-710">Boolean</span><span class="sxs-lookup"><span data-stu-id="a7082-710">Boolean</span></span>|<span data-ttu-id="a7082-711">指示是否阻止用户覆盖 Exploit Protection 设置。</span><span class="sxs-lookup"><span data-stu-id="a7082-711">Indicates whether or not to block user from overriding Exploit Protection settings.</span></span>|
|<span data-ttu-id="a7082-712">appLockerApplicationControl</span><span class="sxs-lookup"><span data-stu-id="a7082-712">appLockerApplicationControl</span></span>|[<span data-ttu-id="a7082-713">appLockerApplicationControlType</span><span class="sxs-lookup"><span data-stu-id="a7082-713">appLockerApplicationControlType</span></span>](../resources/intune-deviceconfig-applockerapplicationcontroltype.md)|<span data-ttu-id="a7082-714">使管理员能够选择在设备上允许哪些类型的应用。</span><span class="sxs-lookup"><span data-stu-id="a7082-714">Enables the Admin to choose what types of app to allow on devices.</span></span> <span data-ttu-id="a7082-715">可取值为：`notConfigured`、`enforceComponentsAndStoreApps`、`auditComponentsAndStoreApps`、`enforceComponentsStoreAppsAndSmartlocker`、`auditComponentsStoreAppsAndSmartlocker`。</span><span class="sxs-lookup"><span data-stu-id="a7082-715">Possible values are: `notConfigured`, `enforceComponentsAndStoreApps`, `auditComponentsAndStoreApps`, `enforceComponentsStoreAppsAndSmartlocker`, `auditComponentsStoreAppsAndSmartlocker`.</span></span>|
|<span data-ttu-id="a7082-716">deviceGuardLocalSystemAuthorityCredentialGuardSettings</span><span class="sxs-lookup"><span data-stu-id="a7082-716">deviceGuardLocalSystemAuthorityCredentialGuardSettings</span></span>|[<span data-ttu-id="a7082-717">deviceGuardLocalSystemAuthorityCredentialGuardType</span><span class="sxs-lookup"><span data-stu-id="a7082-717">deviceGuardLocalSystemAuthorityCredentialGuardType</span></span>](../resources/intune-deviceconfig-deviceguardlocalsystemauthoritycredentialguardtype.md)|<span data-ttu-id="a7082-718">如果平台安全级别具有安全启动和基于虚拟化的安全性均已启用, 则打开 Credential Guard。</span><span class="sxs-lookup"><span data-stu-id="a7082-718">Turn on Credential Guard when Platform Security Level with Secure Boot and Virtualization Based Security are both enabled.</span></span> <span data-ttu-id="a7082-719">可取值为：`notConfigured`、`enableWithUEFILock`、`enableWithoutUEFILock`。</span><span class="sxs-lookup"><span data-stu-id="a7082-719">Possible values are: `notConfigured`, `enableWithUEFILock`, `enableWithoutUEFILock`.</span></span>|
|<span data-ttu-id="a7082-720">deviceGuardEnableVirtualizationBasedSecurity</span><span class="sxs-lookup"><span data-stu-id="a7082-720">deviceGuardEnableVirtualizationBasedSecurity</span></span>|<span data-ttu-id="a7082-721">Boolean</span><span class="sxs-lookup"><span data-stu-id="a7082-721">Boolean</span></span>|<span data-ttu-id="a7082-722">启用基于虚拟化的安全性 (VBS)。</span><span class="sxs-lookup"><span data-stu-id="a7082-722">Turns On Virtualization Based Security(VBS).</span></span>|
|<span data-ttu-id="a7082-723">deviceGuardEnableSecureBootWithDMA</span><span class="sxs-lookup"><span data-stu-id="a7082-723">deviceGuardEnableSecureBootWithDMA</span></span>|<span data-ttu-id="a7082-724">Boolean</span><span class="sxs-lookup"><span data-stu-id="a7082-724">Boolean</span></span>|<span data-ttu-id="a7082-725">指定是否在下次重新启动时启用平台安全级别。</span><span class="sxs-lookup"><span data-stu-id="a7082-725">Specifies whether Platform Security Level is enabled at next reboot.</span></span>|
|<span data-ttu-id="a7082-726">deviceGuardLaunchSystemGuard</span><span class="sxs-lookup"><span data-stu-id="a7082-726">deviceGuardLaunchSystemGuard</span></span>|[<span data-ttu-id="a7082-727">启用</span><span class="sxs-lookup"><span data-stu-id="a7082-727">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="a7082-728">允许 IT 管理员配置启动 "系统防护"。</span><span class="sxs-lookup"><span data-stu-id="a7082-728">Allows the IT admin to configure the launch of System Guard.</span></span> <span data-ttu-id="a7082-729">可取值为：`notConfigured`、`enabled`、`disabled`。</span><span class="sxs-lookup"><span data-stu-id="a7082-729">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="a7082-730">smartScreenEnableInShell</span><span class="sxs-lookup"><span data-stu-id="a7082-730">smartScreenEnableInShell</span></span>|<span data-ttu-id="a7082-731">Boolean</span><span class="sxs-lookup"><span data-stu-id="a7082-731">Boolean</span></span>|<span data-ttu-id="a7082-732">允许 IT 管理员配置适用于 Windows 的 SmartScreen。</span><span class="sxs-lookup"><span data-stu-id="a7082-732">Allows IT Admins to configure SmartScreen for Windows.</span></span>|
|<span data-ttu-id="a7082-733">smartScreenBlockOverrideForFiles</span><span class="sxs-lookup"><span data-stu-id="a7082-733">smartScreenBlockOverrideForFiles</span></span>|<span data-ttu-id="a7082-734">Boolean</span><span class="sxs-lookup"><span data-stu-id="a7082-734">Boolean</span></span>|<span data-ttu-id="a7082-735">允许 IT 管理员控制用户是否可以忽略 SmartScreen 警告并运行恶意文件。</span><span class="sxs-lookup"><span data-stu-id="a7082-735">Allows IT Admins to control whether users can can ignore SmartScreen warnings and run malicious files.</span></span>|
|<span data-ttu-id="a7082-736">applicationGuardEnabled</span><span class="sxs-lookup"><span data-stu-id="a7082-736">applicationGuardEnabled</span></span>|<span data-ttu-id="a7082-737">Boolean</span><span class="sxs-lookup"><span data-stu-id="a7082-737">Boolean</span></span>|<span data-ttu-id="a7082-738">启用 Windows Defender 应用程序防护</span><span class="sxs-lookup"><span data-stu-id="a7082-738">Enable Windows Defender Application Guard</span></span>|
|<span data-ttu-id="a7082-739">applicationGuardEnabledOptions</span><span class="sxs-lookup"><span data-stu-id="a7082-739">applicationGuardEnabledOptions</span></span>|[<span data-ttu-id="a7082-740">applicationGuardEnabledOptions</span><span class="sxs-lookup"><span data-stu-id="a7082-740">applicationGuardEnabledOptions</span></span>](../resources/intune-deviceconfig-applicationguardenabledoptions.md)|<span data-ttu-id="a7082-741">为较新的 windows 版本启用 windows Defender 应用程序防护。</span><span class="sxs-lookup"><span data-stu-id="a7082-741">Enable Windows Defender Application Guard for newer Windows builds.</span></span> <span data-ttu-id="a7082-742">可取值为：`notConfigured`、`enabledForEdge`、`enabledForOffice`、`enabledForEdgeAndOffice`。</span><span class="sxs-lookup"><span data-stu-id="a7082-742">Possible values are: `notConfigured`, `enabledForEdge`, `enabledForOffice`, `enabledForEdgeAndOffice`.</span></span>|
|<span data-ttu-id="a7082-743">applicationGuardBlockFileTransfer</span><span class="sxs-lookup"><span data-stu-id="a7082-743">applicationGuardBlockFileTransfer</span></span>|[<span data-ttu-id="a7082-744">applicationGuardBlockFileTransferType</span><span class="sxs-lookup"><span data-stu-id="a7082-744">applicationGuardBlockFileTransferType</span></span>](../resources/intune-deviceconfig-applicationguardblockfiletransfertype.md)|<span data-ttu-id="a7082-745">阻止剪贴板传输图像文件、文本文件或二者都不。</span><span class="sxs-lookup"><span data-stu-id="a7082-745">Block clipboard to transfer image file, text file or neither of them.</span></span> <span data-ttu-id="a7082-746">可取值为：`notConfigured`、`blockImageAndTextFile`、`blockImageFile`、`blockNone` 或 `blockTextFile`。</span><span class="sxs-lookup"><span data-stu-id="a7082-746">Possible values are: `notConfigured`, `blockImageAndTextFile`, `blockImageFile`, `blockNone`, `blockTextFile`.</span></span>|
|<span data-ttu-id="a7082-747">applicationGuardBlockNonEnterpriseContent</span><span class="sxs-lookup"><span data-stu-id="a7082-747">applicationGuardBlockNonEnterpriseContent</span></span>|<span data-ttu-id="a7082-748">Boolean</span><span class="sxs-lookup"><span data-stu-id="a7082-748">Boolean</span></span>|<span data-ttu-id="a7082-749">阻止企业站点加载非企业内容，例如第三方插件</span><span class="sxs-lookup"><span data-stu-id="a7082-749">Block enterprise sites to load non-enterprise content, such as third party plug-ins</span></span>|
|<span data-ttu-id="a7082-750">applicationGuardAllowPersistence</span><span class="sxs-lookup"><span data-stu-id="a7082-750">applicationGuardAllowPersistence</span></span>|<span data-ttu-id="a7082-751">Boolean</span><span class="sxs-lookup"><span data-stu-id="a7082-751">Boolean</span></span>|<span data-ttu-id="a7082-752">允许 App Guard 容器（收藏夹、Cookie、Web 密码等）内的持久用户生成数据</span><span class="sxs-lookup"><span data-stu-id="a7082-752">Allow persisting user generated data inside the App Guard Containter (favorites, cookies, web passwords, etc.)</span></span>|
|<span data-ttu-id="a7082-753">applicationGuardForceAuditing</span><span class="sxs-lookup"><span data-stu-id="a7082-753">applicationGuardForceAuditing</span></span>|<span data-ttu-id="a7082-754">Boolean</span><span class="sxs-lookup"><span data-stu-id="a7082-754">Boolean</span></span>|<span data-ttu-id="a7082-755">强制审核将存留 Windows 日志和事件以满足安全/符合性条件（示例事件是用户登录注销、特权使用、软件安装、系统更改等）</span><span class="sxs-lookup"><span data-stu-id="a7082-755">Force auditing will persist Windows logs and events to meet security/compliance criteria (sample events are user login-logoff, use of privilege rights, software installation, system changes, etc.)</span></span>|
|<span data-ttu-id="a7082-756">applicationGuardBlockClipboardSharing</span><span class="sxs-lookup"><span data-stu-id="a7082-756">applicationGuardBlockClipboardSharing</span></span>|[<span data-ttu-id="a7082-757">applicationGuardBlockClipboardSharingType</span><span class="sxs-lookup"><span data-stu-id="a7082-757">applicationGuardBlockClipboardSharingType</span></span>](../resources/intune-deviceconfig-applicationguardblockclipboardsharingtype.md)|<span data-ttu-id="a7082-758">阻止剪贴板将数据从主机共享到容器或从容器共享到主机，或阻止两种方式，或两种方式均不阻止。</span><span class="sxs-lookup"><span data-stu-id="a7082-758">Block clipboard to share data from Host to Container, or from Container to Host, or both ways, or neither ways.</span></span> <span data-ttu-id="a7082-759">可取值为：`notConfigured`、`blockBoth`、`blockHostToContainer`、`blockContainerToHost`、`blockNone`。</span><span class="sxs-lookup"><span data-stu-id="a7082-759">Possible values are: `notConfigured`, `blockBoth`, `blockHostToContainer`, `blockContainerToHost`, `blockNone`.</span></span>|
|<span data-ttu-id="a7082-760">applicationGuardAllowPrintToPDF</span><span class="sxs-lookup"><span data-stu-id="a7082-760">applicationGuardAllowPrintToPDF</span></span>|<span data-ttu-id="a7082-761">Boolean</span><span class="sxs-lookup"><span data-stu-id="a7082-761">Boolean</span></span>|<span data-ttu-id="a7082-762">允许从容器打印为 PDF 格式</span><span class="sxs-lookup"><span data-stu-id="a7082-762">Allow printing to PDF from Container</span></span>|
|<span data-ttu-id="a7082-763">applicationGuardAllowPrintToXPS</span><span class="sxs-lookup"><span data-stu-id="a7082-763">applicationGuardAllowPrintToXPS</span></span>|<span data-ttu-id="a7082-764">Boolean</span><span class="sxs-lookup"><span data-stu-id="a7082-764">Boolean</span></span>|<span data-ttu-id="a7082-765">允许从容器打印为 XPS 格式</span><span class="sxs-lookup"><span data-stu-id="a7082-765">Allow printing to XPS from Container</span></span>|
|<span data-ttu-id="a7082-766">applicationGuardAllowPrintToLocalPrinters</span><span class="sxs-lookup"><span data-stu-id="a7082-766">applicationGuardAllowPrintToLocalPrinters</span></span>|<span data-ttu-id="a7082-767">Boolean</span><span class="sxs-lookup"><span data-stu-id="a7082-767">Boolean</span></span>|<span data-ttu-id="a7082-768">允许从容器打印到本地打印机</span><span class="sxs-lookup"><span data-stu-id="a7082-768">Allow printing to Local Printers from Container</span></span>|
|<span data-ttu-id="a7082-769">applicationGuardAllowPrintToNetworkPrinters</span><span class="sxs-lookup"><span data-stu-id="a7082-769">applicationGuardAllowPrintToNetworkPrinters</span></span>|<span data-ttu-id="a7082-770">Boolean</span><span class="sxs-lookup"><span data-stu-id="a7082-770">Boolean</span></span>|<span data-ttu-id="a7082-771">允许从容器打印到网络打印机</span><span class="sxs-lookup"><span data-stu-id="a7082-771">Allow printing to Network Printers from Container</span></span>|
|<span data-ttu-id="a7082-772">applicationGuardAllowVirtualGPU</span><span class="sxs-lookup"><span data-stu-id="a7082-772">applicationGuardAllowVirtualGPU</span></span>|<span data-ttu-id="a7082-773">Boolean</span><span class="sxs-lookup"><span data-stu-id="a7082-773">Boolean</span></span>|<span data-ttu-id="a7082-774">允许应用程序防护使用虚拟 GPU</span><span class="sxs-lookup"><span data-stu-id="a7082-774">Allow application guard to use virtual GPU</span></span>|
|<span data-ttu-id="a7082-775">applicationGuardAllowFileSaveOnHost</span><span class="sxs-lookup"><span data-stu-id="a7082-775">applicationGuardAllowFileSaveOnHost</span></span>|<span data-ttu-id="a7082-776">Boolean</span><span class="sxs-lookup"><span data-stu-id="a7082-776">Boolean</span></span>|<span data-ttu-id="a7082-777">允许用户从应用程序防护容器中的边缘下载文件并将其保存在主机文件系统上</span><span class="sxs-lookup"><span data-stu-id="a7082-777">Allow users to download files from Edge in the application guard container and save them on the host file system</span></span>|
|<span data-ttu-id="a7082-778">bitLockerAllowStandardUserEncryption</span><span class="sxs-lookup"><span data-stu-id="a7082-778">bitLockerAllowStandardUserEncryption</span></span>|<span data-ttu-id="a7082-779">Boolean</span><span class="sxs-lookup"><span data-stu-id="a7082-779">Boolean</span></span>|<span data-ttu-id="a7082-780">允许管理员允许标准用户在 Azure AD 加入过程中启用 encrpytion。</span><span class="sxs-lookup"><span data-stu-id="a7082-780">Allows the admin to allow standard users to enable encrpytion during Azure AD Join.</span></span>|
|<span data-ttu-id="a7082-781">bitLockerDisableWarningForOtherDiskEncryption</span><span class="sxs-lookup"><span data-stu-id="a7082-781">bitLockerDisableWarningForOtherDiskEncryption</span></span>|<span data-ttu-id="a7082-782">Boolean</span><span class="sxs-lookup"><span data-stu-id="a7082-782">Boolean</span></span>|<span data-ttu-id="a7082-783">允许管理员禁用对用户计算机上其他磁盘加密的警告提示。</span><span class="sxs-lookup"><span data-stu-id="a7082-783">Allows the Admin to disable the warning prompt for other disk encryption on the user machines.</span></span>|
|<span data-ttu-id="a7082-784">bitLockerEnableStorageCardEncryptionOnMobile</span><span class="sxs-lookup"><span data-stu-id="a7082-784">bitLockerEnableStorageCardEncryptionOnMobile</span></span>|<span data-ttu-id="a7082-785">Boolean</span><span class="sxs-lookup"><span data-stu-id="a7082-785">Boolean</span></span>|<span data-ttu-id="a7082-786">允许管理员要求使用 BitLocker 开启加密功能。</span><span class="sxs-lookup"><span data-stu-id="a7082-786">Allows the admin to require encryption to be turned on using BitLocker.</span></span> <span data-ttu-id="a7082-787">此策略仅适用于移动 SKU。</span><span class="sxs-lookup"><span data-stu-id="a7082-787">This policy is valid only for a mobile SKU.</span></span>|
|<span data-ttu-id="a7082-788">bitLockerEncryptDevice</span><span class="sxs-lookup"><span data-stu-id="a7082-788">bitLockerEncryptDevice</span></span>|<span data-ttu-id="a7082-789">Boolean</span><span class="sxs-lookup"><span data-stu-id="a7082-789">Boolean</span></span>|<span data-ttu-id="a7082-790">允许管理员要求使用 BitLocker 开启加密功能。</span><span class="sxs-lookup"><span data-stu-id="a7082-790">Allows the admin to require encryption to be turned on using BitLocker.</span></span>|
|<span data-ttu-id="a7082-791">bitLockerSystemDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="a7082-791">bitLockerSystemDrivePolicy</span></span>|[<span data-ttu-id="a7082-792">bitLockerSystemDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="a7082-792">bitLockerSystemDrivePolicy</span></span>](../resources/intune-deviceconfig-bitlockersystemdrivepolicy.md)|<span data-ttu-id="a7082-793">BitLocker 系统驱动器策略。</span><span class="sxs-lookup"><span data-stu-id="a7082-793">BitLocker System Drive Policy.</span></span>|
|<span data-ttu-id="a7082-794">bitLockerFixedDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="a7082-794">bitLockerFixedDrivePolicy</span></span>|[<span data-ttu-id="a7082-795">bitLockerFixedDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="a7082-795">bitLockerFixedDrivePolicy</span></span>](../resources/intune-deviceconfig-bitlockerfixeddrivepolicy.md)|<span data-ttu-id="a7082-796">BitLocker 固定驱动器策略。</span><span class="sxs-lookup"><span data-stu-id="a7082-796">BitLocker Fixed Drive Policy.</span></span>|
|<span data-ttu-id="a7082-797">bitLockerRemovableDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="a7082-797">bitLockerRemovableDrivePolicy</span></span>|[<span data-ttu-id="a7082-798">bitLockerRemovableDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="a7082-798">bitLockerRemovableDrivePolicy</span></span>](../resources/intune-deviceconfig-bitlockerremovabledrivepolicy.md)|<span data-ttu-id="a7082-799">BitLocker 可移动驱动器策略。</span><span class="sxs-lookup"><span data-stu-id="a7082-799">BitLocker Removable Drive Policy.</span></span>|



## <a name="response"></a><span data-ttu-id="a7082-800">响应</span><span class="sxs-lookup"><span data-stu-id="a7082-800">Response</span></span>
<span data-ttu-id="a7082-801">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="a7082-801">If successful, this method returns a `201 Created` response code and a [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a7082-802">示例</span><span class="sxs-lookup"><span data-stu-id="a7082-802">Example</span></span>

### <a name="request"></a><span data-ttu-id="a7082-803">请求</span><span class="sxs-lookup"><span data-stu-id="a7082-803">Request</span></span>
<span data-ttu-id="a7082-804">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="a7082-804">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 27641

{
  "@odata.type": "#microsoft.graph.windows10EndpointProtectionConfiguration",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
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

### <a name="response"></a><span data-ttu-id="a7082-805">响应</span><span class="sxs-lookup"><span data-stu-id="a7082-805">Response</span></span>
<span data-ttu-id="a7082-p199">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="a7082-p199">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 27813

{
  "@odata.type": "#microsoft.graph.windows10EndpointProtectionConfiguration",
  "id": "09709403-9403-0970-0394-700903947009",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
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




