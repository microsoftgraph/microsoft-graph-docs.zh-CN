---
title: 更新 windows10EndpointProtectionConfiguration
description: 更新 windows10EndpointProtectionConfiguration 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 101433d2fc51f4a3eb1f1b896cc65c7e6ee3c7a0
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32516614"
---
# <a name="update-windows10endpointprotectionconfiguration"></a><span data-ttu-id="f1e58-103">更新 windows10EndpointProtectionConfiguration</span><span class="sxs-lookup"><span data-stu-id="f1e58-103">Update windows10EndpointProtectionConfiguration</span></span>

> <span data-ttu-id="f1e58-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="f1e58-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f1e58-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f1e58-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f1e58-106">更新 [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="f1e58-106">Update the properties of a [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f1e58-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="f1e58-107">Prerequisites</span></span>
<span data-ttu-id="f1e58-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f1e58-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f1e58-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="f1e58-110">Permission type</span></span>|<span data-ttu-id="f1e58-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="f1e58-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f1e58-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f1e58-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f1e58-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f1e58-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f1e58-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f1e58-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f1e58-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="f1e58-115">Not supported.</span></span>|
|<span data-ttu-id="f1e58-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="f1e58-116">Application</span></span>|<span data-ttu-id="f1e58-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="f1e58-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f1e58-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f1e58-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="f1e58-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="f1e58-119">Request headers</span></span>
|<span data-ttu-id="f1e58-120">标头</span><span class="sxs-lookup"><span data-stu-id="f1e58-120">Header</span></span>|<span data-ttu-id="f1e58-121">值</span><span class="sxs-lookup"><span data-stu-id="f1e58-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f1e58-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="f1e58-122">Authorization</span></span>|<span data-ttu-id="f1e58-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="f1e58-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f1e58-124">接受</span><span class="sxs-lookup"><span data-stu-id="f1e58-124">Accept</span></span>|<span data-ttu-id="f1e58-125">application/json</span><span class="sxs-lookup"><span data-stu-id="f1e58-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f1e58-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="f1e58-126">Request body</span></span>
<span data-ttu-id="f1e58-127">在请求正文中，提供 [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f1e58-127">In the request body, supply a JSON representation for the [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) object.</span></span>

<span data-ttu-id="f1e58-128">下表显示了创建 [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="f1e58-128">The following table shows the properties that are required when you create the [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md).</span></span>

|<span data-ttu-id="f1e58-129">属性</span><span class="sxs-lookup"><span data-stu-id="f1e58-129">Property</span></span>|<span data-ttu-id="f1e58-130">类型</span><span class="sxs-lookup"><span data-stu-id="f1e58-130">Type</span></span>|<span data-ttu-id="f1e58-131">说明</span><span class="sxs-lookup"><span data-stu-id="f1e58-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f1e58-132">id</span><span class="sxs-lookup"><span data-stu-id="f1e58-132">id</span></span>|<span data-ttu-id="f1e58-133">String</span><span class="sxs-lookup"><span data-stu-id="f1e58-133">String</span></span>|<span data-ttu-id="f1e58-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="f1e58-134">Key of the entity.</span></span> <span data-ttu-id="f1e58-135">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f1e58-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f1e58-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f1e58-136">lastModifiedDateTime</span></span>|<span data-ttu-id="f1e58-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f1e58-137">DateTimeOffset</span></span>|<span data-ttu-id="f1e58-138">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="f1e58-138">DateTime the object was last modified.</span></span> <span data-ttu-id="f1e58-139">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f1e58-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f1e58-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="f1e58-140">roleScopeTagIds</span></span>|<span data-ttu-id="f1e58-141">String collection</span><span class="sxs-lookup"><span data-stu-id="f1e58-141">String collection</span></span>|<span data-ttu-id="f1e58-142">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="f1e58-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="f1e58-143">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f1e58-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f1e58-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="f1e58-144">supportsScopeTags</span></span>|<span data-ttu-id="f1e58-145">布尔</span><span class="sxs-lookup"><span data-stu-id="f1e58-145">Boolean</span></span>|<span data-ttu-id="f1e58-146">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="f1e58-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="f1e58-147">如果此值为 false, 则不允许分配给 ScopeTags 属性, 并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="f1e58-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="f1e58-148">这适用于在 Silverlight 中创建的旧版策略, 可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="f1e58-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="f1e58-149">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="f1e58-149">This property is read-only.</span></span> <span data-ttu-id="f1e58-150">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f1e58-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f1e58-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f1e58-151">createdDateTime</span></span>|<span data-ttu-id="f1e58-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f1e58-152">DateTimeOffset</span></span>|<span data-ttu-id="f1e58-153">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="f1e58-153">DateTime the object was created.</span></span> <span data-ttu-id="f1e58-154">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f1e58-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f1e58-155">description</span><span class="sxs-lookup"><span data-stu-id="f1e58-155">description</span></span>|<span data-ttu-id="f1e58-156">字符串</span><span class="sxs-lookup"><span data-stu-id="f1e58-156">String</span></span>|<span data-ttu-id="f1e58-157">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="f1e58-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="f1e58-158">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f1e58-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f1e58-159">displayName</span><span class="sxs-lookup"><span data-stu-id="f1e58-159">displayName</span></span>|<span data-ttu-id="f1e58-160">String</span><span class="sxs-lookup"><span data-stu-id="f1e58-160">String</span></span>|<span data-ttu-id="f1e58-161">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="f1e58-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="f1e58-162">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f1e58-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f1e58-163">version</span><span class="sxs-lookup"><span data-stu-id="f1e58-163">version</span></span>|<span data-ttu-id="f1e58-164">Int32</span><span class="sxs-lookup"><span data-stu-id="f1e58-164">Int32</span></span>|<span data-ttu-id="f1e58-165">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="f1e58-165">Version of the device configuration.</span></span> <span data-ttu-id="f1e58-166">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f1e58-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f1e58-167">dmaGuardDeviceEnumerationPolicy</span><span class="sxs-lookup"><span data-stu-id="f1e58-167">dmaGuardDeviceEnumerationPolicy</span></span>|[<span data-ttu-id="f1e58-168">dmaGuardDeviceEnumerationPolicyType</span><span class="sxs-lookup"><span data-stu-id="f1e58-168">dmaGuardDeviceEnumerationPolicyType</span></span>](../resources/intune-deviceconfig-dmaguarddeviceenumerationpolicytype.md)|<span data-ttu-id="f1e58-169">此策略旨在提供针对支持外部 DMA 的设备的额外安全性。</span><span class="sxs-lookup"><span data-stu-id="f1e58-169">This policy is intended to provide additional security against external DMA capable devices.</span></span> <span data-ttu-id="f1e58-170">通过它, 可以更好地控制支持外部 dma 的设备与 dma 重新映射/设备内存隔离和沙盒不兼容的枚举。</span><span class="sxs-lookup"><span data-stu-id="f1e58-170">It allows for more control over the enumeration of external DMA capable devices incompatible with DMA Remapping/device memory isolation and sandboxing.</span></span> <span data-ttu-id="f1e58-171">仅当系统固件支持和启用内核 DMA 保护时, 此策略才会生效。</span><span class="sxs-lookup"><span data-stu-id="f1e58-171">This policy only takes effect when Kernel DMA Protection is supported and enabled by the system firmware.</span></span> <span data-ttu-id="f1e58-172">内核 DMA 保护是一项平台功能, 不能通过策略或最终用户进行控制。</span><span class="sxs-lookup"><span data-stu-id="f1e58-172">Kernel DMA Protection is a platform feature that cannot be controlled via policy or by end user.</span></span> <span data-ttu-id="f1e58-173">在制造时, 系统必须支持它。</span><span class="sxs-lookup"><span data-stu-id="f1e58-173">It has to be supported by the system at the time of manufacturing.</span></span> <span data-ttu-id="f1e58-174">若要检查系统是否支持内核 dma 保护, 请在 MSINFO32 的摘要页中检查 "内核 dma 保护" 字段。</span><span class="sxs-lookup"><span data-stu-id="f1e58-174">To check if the system supports Kernel DMA Protection, please check the Kernel DMA Protection field in the Summary page of MSINFO32.exe.</span></span> <span data-ttu-id="f1e58-175">可取值为：`deviceDefault`、`blockAll`、`allowAll`。</span><span class="sxs-lookup"><span data-stu-id="f1e58-175">Possible values are: `deviceDefault`, `blockAll`, `allowAll`.</span></span>|
|<span data-ttu-id="f1e58-176">firewallRules</span><span class="sxs-lookup"><span data-stu-id="f1e58-176">firewallRules</span></span>|<span data-ttu-id="f1e58-177">[windowsFirewallRule](../resources/intune-deviceconfig-windowsfirewallrule.md)集合</span><span class="sxs-lookup"><span data-stu-id="f1e58-177">[windowsFirewallRule](../resources/intune-deviceconfig-windowsfirewallrule.md) collection</span></span>|<span data-ttu-id="f1e58-178">配置防火墙规则设置。</span><span class="sxs-lookup"><span data-stu-id="f1e58-178">Configures the firewall rule settings.</span></span> <span data-ttu-id="f1e58-179">此集合最多可包含150个元素。</span><span class="sxs-lookup"><span data-stu-id="f1e58-179">This collection can contain a maximum of 150 elements.</span></span>|
|<span data-ttu-id="f1e58-180">userRightsAccessCredentialManagerAsTrustedCaller</span><span class="sxs-lookup"><span data-stu-id="f1e58-180">userRightsAccessCredentialManagerAsTrustedCaller</span></span>|[<span data-ttu-id="f1e58-181">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="f1e58-181">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="f1e58-182">此用户权限由凭据管理器在备份/还原过程中使用。</span><span class="sxs-lookup"><span data-stu-id="f1e58-182">This user right is used by Credential Manager during Backup/Restore.</span></span> <span data-ttu-id="f1e58-183">如果为其他实体提供此权限, 则用户保存的凭据可能会受到威胁。</span><span class="sxs-lookup"><span data-stu-id="f1e58-183">Users' saved credentials might be compromised if this privilege is given to other entities.</span></span> <span data-ttu-id="f1e58-184">仅支持 NotConfigured 和允许的状态</span><span class="sxs-lookup"><span data-stu-id="f1e58-184">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="f1e58-185">userRightsAllowAccessFromNetwork</span><span class="sxs-lookup"><span data-stu-id="f1e58-185">userRightsAllowAccessFromNetwork</span></span>|[<span data-ttu-id="f1e58-186">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="f1e58-186">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="f1e58-187">此用户权限确定允许哪些用户和组通过网络连接到计算机。</span><span class="sxs-lookup"><span data-stu-id="f1e58-187">This user right determines which users and groups are allowed to connect to the computer over the network.</span></span> <span data-ttu-id="f1e58-188">支持的状态为 "允许"。</span><span class="sxs-lookup"><span data-stu-id="f1e58-188">State Allowed is supported.</span></span>|
|<span data-ttu-id="f1e58-189">userRightsBlockAccessFromNetwork</span><span class="sxs-lookup"><span data-stu-id="f1e58-189">userRightsBlockAccessFromNetwork</span></span>|[<span data-ttu-id="f1e58-190">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="f1e58-190">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="f1e58-191">此用户权限决定了阻止哪些用户和组通过网络连接到计算机。</span><span class="sxs-lookup"><span data-stu-id="f1e58-191">This user right determines which users and groups are block from connecting to the computer over the network.</span></span> <span data-ttu-id="f1e58-192">支持状态块。</span><span class="sxs-lookup"><span data-stu-id="f1e58-192">State Block is supported.</span></span>|
|<span data-ttu-id="f1e58-193">userRightsActAsPartOfTheOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="f1e58-193">userRightsActAsPartOfTheOperatingSystem</span></span>|[<span data-ttu-id="f1e58-194">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="f1e58-194">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="f1e58-195">此用户权限允许进程在不进行身份验证的情况下模拟任何用户。</span><span class="sxs-lookup"><span data-stu-id="f1e58-195">This user right allows a process to impersonate any user without authentication.</span></span> <span data-ttu-id="f1e58-196">因此, 该过程可以获得与该用户相同的本地资源的访问权限。</span><span class="sxs-lookup"><span data-stu-id="f1e58-196">The process can therefore gain access to the same local resources as that user.</span></span> <span data-ttu-id="f1e58-197">仅支持 NotConfigured 和允许的状态</span><span class="sxs-lookup"><span data-stu-id="f1e58-197">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="f1e58-198">userRightsLocalLogOn</span><span class="sxs-lookup"><span data-stu-id="f1e58-198">userRightsLocalLogOn</span></span>|[<span data-ttu-id="f1e58-199">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="f1e58-199">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="f1e58-200">此用户权限确定哪些用户可以登录到计算机。</span><span class="sxs-lookup"><span data-stu-id="f1e58-200">This user right determines which users can log on to the computer.</span></span> <span data-ttu-id="f1e58-201">所有支持的状态 NotConfigured、允许和阻止</span><span class="sxs-lookup"><span data-stu-id="f1e58-201">States NotConfigured, Allowed and Blocked are all supported</span></span> |
|<span data-ttu-id="f1e58-202">userRightsBackupData</span><span class="sxs-lookup"><span data-stu-id="f1e58-202">userRightsBackupData</span></span>|[<span data-ttu-id="f1e58-203">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="f1e58-203">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="f1e58-204">此用户权限确定在备份文件和目录时, 哪些用户可以绕过文件、目录、注册表和其他持久对象权限。</span><span class="sxs-lookup"><span data-stu-id="f1e58-204">This user right determines which users can bypass file, directory, registry, and other persistent objects permissions when backing up files and directories.</span></span> <span data-ttu-id="f1e58-205">仅支持 NotConfigured 和允许的状态</span><span class="sxs-lookup"><span data-stu-id="f1e58-205">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="f1e58-206">userRightsChangeSystemTime</span><span class="sxs-lookup"><span data-stu-id="f1e58-206">userRightsChangeSystemTime</span></span>|[<span data-ttu-id="f1e58-207">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="f1e58-207">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="f1e58-208">此用户权限确定哪些用户和组可以更改计算机内部时钟上的时间和日期。</span><span class="sxs-lookup"><span data-stu-id="f1e58-208">This user right determines which users and groups can change the time and date on the internal clock of the computer.</span></span> <span data-ttu-id="f1e58-209">仅支持 NotConfigured 和允许的状态</span><span class="sxs-lookup"><span data-stu-id="f1e58-209">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="f1e58-210">userRightsCreateGlobalObjects</span><span class="sxs-lookup"><span data-stu-id="f1e58-210">userRightsCreateGlobalObjects</span></span>|[<span data-ttu-id="f1e58-211">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="f1e58-211">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="f1e58-212">此安全设置确定用户是否可以创建可用于所有会话的全局对象。</span><span class="sxs-lookup"><span data-stu-id="f1e58-212">This security setting determines whether users can create global objects that are available to all sessions.</span></span> <span data-ttu-id="f1e58-213">可以创建全局对象的用户可能会影响在其他用户的会话下运行的进程, 这可能导致应用程序故障或数据损坏。</span><span class="sxs-lookup"><span data-stu-id="f1e58-213">Users who can create global objects could affect processes that run under other users' sessions, which could lead to application failure or data corruption.</span></span> <span data-ttu-id="f1e58-214">仅支持 NotConfigured 和允许的状态</span><span class="sxs-lookup"><span data-stu-id="f1e58-214">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="f1e58-215">userRightsCreatePageFile</span><span class="sxs-lookup"><span data-stu-id="f1e58-215">userRightsCreatePageFile</span></span>|[<span data-ttu-id="f1e58-216">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="f1e58-216">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="f1e58-217">此用户权限确定哪些用户和组可以调用内部 API 来创建和更改页面文件的大小。</span><span class="sxs-lookup"><span data-stu-id="f1e58-217">This user right determines which users and groups can call an internal API to create and change the size of a page file.</span></span> <span data-ttu-id="f1e58-218">仅支持 NotConfigured 和允许的状态</span><span class="sxs-lookup"><span data-stu-id="f1e58-218">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="f1e58-219">userRightsCreatePermanentSharedObjects</span><span class="sxs-lookup"><span data-stu-id="f1e58-219">userRightsCreatePermanentSharedObjects</span></span>|[<span data-ttu-id="f1e58-220">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="f1e58-220">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="f1e58-221">此用户权限决定了进程可以使用哪些帐户使用对象管理器创建目录对象。</span><span class="sxs-lookup"><span data-stu-id="f1e58-221">This user right determines which accounts can be used by processes to create a directory object using the object manager.</span></span> <span data-ttu-id="f1e58-222">仅支持 NotConfigured 和允许的状态</span><span class="sxs-lookup"><span data-stu-id="f1e58-222">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="f1e58-223">userRightsCreateSymbolicLinks</span><span class="sxs-lookup"><span data-stu-id="f1e58-223">userRightsCreateSymbolicLinks</span></span>|[<span data-ttu-id="f1e58-224">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="f1e58-224">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="f1e58-225">此用户权限确定用户是否可以从其登录到的计算机创建符号链接。</span><span class="sxs-lookup"><span data-stu-id="f1e58-225">This user right determines if the user can create a symbolic link from the computer to which they are logged on.</span></span> <span data-ttu-id="f1e58-226">仅支持 NotConfigured 和允许的状态</span><span class="sxs-lookup"><span data-stu-id="f1e58-226">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="f1e58-227">userRightsCreateToken</span><span class="sxs-lookup"><span data-stu-id="f1e58-227">userRightsCreateToken</span></span>|[<span data-ttu-id="f1e58-228">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="f1e58-228">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="f1e58-229">此用户权限确定进程在使用内部 API 创建访问令牌时, 可以使用哪些用户/组来创建令牌, 然后可以使用这些用户/组来获取对任何本地资源的访问权限。</span><span class="sxs-lookup"><span data-stu-id="f1e58-229">This user right determines which users/groups can be used by processes to create a token that can then be used to get access to any local resources when the process uses an internal API to create an access token.</span></span> <span data-ttu-id="f1e58-230">仅支持 NotConfigured 和允许的状态</span><span class="sxs-lookup"><span data-stu-id="f1e58-230">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="f1e58-231">userRightsDebugPrograms</span><span class="sxs-lookup"><span data-stu-id="f1e58-231">userRightsDebugPrograms</span></span>|[<span data-ttu-id="f1e58-232">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="f1e58-232">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="f1e58-233">此用户权限确定哪些用户可以将调试程序附加到任何进程或内核。</span><span class="sxs-lookup"><span data-stu-id="f1e58-233">This user right determines which users can attach a debugger to any process or to the kernel.</span></span> <span data-ttu-id="f1e58-234">仅支持 NotConfigured 和允许的状态</span><span class="sxs-lookup"><span data-stu-id="f1e58-234">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="f1e58-235">userRightsRemoteDesktopServicesLogOn</span><span class="sxs-lookup"><span data-stu-id="f1e58-235">userRightsRemoteDesktopServicesLogOn</span></span>|[<span data-ttu-id="f1e58-236">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="f1e58-236">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="f1e58-237">此用户权限确定禁止哪些用户和组作为远程桌面服务客户端进行登录。</span><span class="sxs-lookup"><span data-stu-id="f1e58-237">This user right determines which users and groups are prohibited from logging on as a Remote Desktop Services client.</span></span> <span data-ttu-id="f1e58-238">仅支持状态 NotConfigured 和阻止</span><span class="sxs-lookup"><span data-stu-id="f1e58-238">Only states NotConfigured and Blocked are supported</span></span>|
|<span data-ttu-id="f1e58-239">userRightsDelegation</span><span class="sxs-lookup"><span data-stu-id="f1e58-239">userRightsDelegation</span></span>|[<span data-ttu-id="f1e58-240">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="f1e58-240">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="f1e58-241">此用户权限确定哪些用户可以在用户或计算机对象上设置受信任委派设置。</span><span class="sxs-lookup"><span data-stu-id="f1e58-241">This user right determines which users can set the Trusted for Delegation setting on a user or computer object.</span></span> <span data-ttu-id="f1e58-242">仅支持 NotConfigured 和允许的状态。</span><span class="sxs-lookup"><span data-stu-id="f1e58-242">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="f1e58-243">userRightsGenerateSecurityAudits</span><span class="sxs-lookup"><span data-stu-id="f1e58-243">userRightsGenerateSecurityAudits</span></span>|[<span data-ttu-id="f1e58-244">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="f1e58-244">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="f1e58-245">此用户权限确定进程可使用哪些帐户向安全日志中添加条目。</span><span class="sxs-lookup"><span data-stu-id="f1e58-245">This user right determines which accounts can be used by a process to add entries to the security log.</span></span> <span data-ttu-id="f1e58-246">安全日志用于跟踪未经授权的系统访问。</span><span class="sxs-lookup"><span data-stu-id="f1e58-246">The security log is used to trace unauthorized system access.</span></span>  <span data-ttu-id="f1e58-247">仅支持 NotConfigured 和允许的状态。</span><span class="sxs-lookup"><span data-stu-id="f1e58-247">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="f1e58-248">userRightsImpersonateClient</span><span class="sxs-lookup"><span data-stu-id="f1e58-248">userRightsImpersonateClient</span></span>|[<span data-ttu-id="f1e58-249">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="f1e58-249">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="f1e58-250">将此用户权限分配给用户将允许代表该用户运行的程序模拟客户端。</span><span class="sxs-lookup"><span data-stu-id="f1e58-250">Assigning this user right to a user allows programs running on behalf of that user to impersonate a client.</span></span> <span data-ttu-id="f1e58-251">如果此类型的模拟要求此用户权限, 则可以防止未经授权的用户说服客户端连接到已创建的服务, 然后模拟该客户端, 这样可以将未经授权的用户的权限提升到管理级别或系统级别。</span><span class="sxs-lookup"><span data-stu-id="f1e58-251">Requiring this user right for this kind of impersonation prevents an unauthorized user from convincing a client to connect to a service that they have created and then impersonating that client, which can elevate the unauthorized user's permissions to administrative or system levels.</span></span> <span data-ttu-id="f1e58-252">仅支持 NotConfigured 和允许的状态。</span><span class="sxs-lookup"><span data-stu-id="f1e58-252">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="f1e58-253">userRightsIncreaseSchedulingPriority</span><span class="sxs-lookup"><span data-stu-id="f1e58-253">userRightsIncreaseSchedulingPriority</span></span>|[<span data-ttu-id="f1e58-254">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="f1e58-254">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="f1e58-255">此用户权限确定哪些帐户可以使用具有对另一进程的 Write 属性访问权限的进程, 以增加分配给其他进程的执行优先级。</span><span class="sxs-lookup"><span data-stu-id="f1e58-255">This user right determines which accounts can use a process with Write Property access to another process to increase the execution priority assigned to the other process.</span></span> <span data-ttu-id="f1e58-256">仅支持 NotConfigured 和允许的状态。</span><span class="sxs-lookup"><span data-stu-id="f1e58-256">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="f1e58-257">userRightsLoadUnloadDrivers</span><span class="sxs-lookup"><span data-stu-id="f1e58-257">userRightsLoadUnloadDrivers</span></span>|[<span data-ttu-id="f1e58-258">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="f1e58-258">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="f1e58-259">此用户权限确定哪些用户可以在内核模式下将设备驱动程序或其他代码动态加载和卸载。</span><span class="sxs-lookup"><span data-stu-id="f1e58-259">This user right determines which users can dynamically load and unload device drivers or other code in to kernel mode.</span></span> <span data-ttu-id="f1e58-260">仅支持 NotConfigured 和允许的状态。</span><span class="sxs-lookup"><span data-stu-id="f1e58-260">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="f1e58-261">userRightsLockMemory</span><span class="sxs-lookup"><span data-stu-id="f1e58-261">userRightsLockMemory</span></span>|[<span data-ttu-id="f1e58-262">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="f1e58-262">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="f1e58-263">此用户权限确定哪些帐户可以使用进程将数据保存在物理内存中, 这会阻止系统将数据分页到磁盘上的虚拟内存中。</span><span class="sxs-lookup"><span data-stu-id="f1e58-263">This user right determines which accounts can use a process to keep data in physical memory, which prevents the system from paging the data to virtual memory on disk.</span></span> <span data-ttu-id="f1e58-264">仅支持 NotConfigured 和允许的状态。</span><span class="sxs-lookup"><span data-stu-id="f1e58-264">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="f1e58-265">userRightsManageAuditingAndSecurityLogs</span><span class="sxs-lookup"><span data-stu-id="f1e58-265">userRightsManageAuditingAndSecurityLogs</span></span>|[<span data-ttu-id="f1e58-266">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="f1e58-266">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="f1e58-267">此用户权限确定哪些用户可以为各个资源 (如文件、Active Directory 对象和注册表项) 指定对象访问审核选项。</span><span class="sxs-lookup"><span data-stu-id="f1e58-267">This user right determines which users can specify object access auditing options for individual resources, such as files, Active Directory objects, and registry keys.</span></span> <span data-ttu-id="f1e58-268">仅支持 NotConfigured 和允许的状态。</span><span class="sxs-lookup"><span data-stu-id="f1e58-268">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="f1e58-269">userRightsManageVolumes</span><span class="sxs-lookup"><span data-stu-id="f1e58-269">userRightsManageVolumes</span></span>|[<span data-ttu-id="f1e58-270">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="f1e58-270">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="f1e58-271">此用户权限确定哪些用户和组可以在某个卷 (如远程碎片整理) 上运行维护任务。</span><span class="sxs-lookup"><span data-stu-id="f1e58-271">This user right determines which users and groups can run maintenance tasks on a volume, such as remote defragmentation.</span></span> <span data-ttu-id="f1e58-272">仅支持 NotConfigured 和允许的状态。</span><span class="sxs-lookup"><span data-stu-id="f1e58-272">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="f1e58-273">userRightsModifyFirmwareEnvironment</span><span class="sxs-lookup"><span data-stu-id="f1e58-273">userRightsModifyFirmwareEnvironment</span></span>|[<span data-ttu-id="f1e58-274">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="f1e58-274">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="f1e58-275">此用户权限决定了可以修改固件环境值的用户。</span><span class="sxs-lookup"><span data-stu-id="f1e58-275">This user right determines who can modify firmware environment values.</span></span> <span data-ttu-id="f1e58-276">仅支持 NotConfigured 和允许的状态。</span><span class="sxs-lookup"><span data-stu-id="f1e58-276">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="f1e58-277">userRightsModifyObjectLabels</span><span class="sxs-lookup"><span data-stu-id="f1e58-277">userRightsModifyObjectLabels</span></span>|[<span data-ttu-id="f1e58-278">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="f1e58-278">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="f1e58-279">此用户权限确定哪些用户帐户可以修改对象的完整性标签, 例如, 文件、注册表项或其他用户所拥有的进程。</span><span class="sxs-lookup"><span data-stu-id="f1e58-279">This user right determines which user accounts can modify the integrity label of objects, such as files, registry keys, or processes owned by other users.</span></span> <span data-ttu-id="f1e58-280">仅支持 NotConfigured 和允许的状态。</span><span class="sxs-lookup"><span data-stu-id="f1e58-280">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="f1e58-281">userRightsProfileSingleProcess</span><span class="sxs-lookup"><span data-stu-id="f1e58-281">userRightsProfileSingleProcess</span></span>|[<span data-ttu-id="f1e58-282">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="f1e58-282">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="f1e58-283">此用户权限确定哪些用户可以使用性能监视工具来监视系统进程的性能。</span><span class="sxs-lookup"><span data-stu-id="f1e58-283">This user right determines which users can use performance monitoring tools to monitor the performance of system processes.</span></span> <span data-ttu-id="f1e58-284">仅支持 NotConfigured 和允许的状态。</span><span class="sxs-lookup"><span data-stu-id="f1e58-284">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="f1e58-285">userRightsRemoteShutdown</span><span class="sxs-lookup"><span data-stu-id="f1e58-285">userRightsRemoteShutdown</span></span>|[<span data-ttu-id="f1e58-286">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="f1e58-286">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="f1e58-287">此用户权限确定允许哪些用户从网络上的远程位置关闭计算机。</span><span class="sxs-lookup"><span data-stu-id="f1e58-287">This user right determines which users are allowed to shut down a computer from a remote location on the network.</span></span> <span data-ttu-id="f1e58-288">误用此用户权限可能会导致拒绝服务。</span><span class="sxs-lookup"><span data-stu-id="f1e58-288">Misuse of this user right can result in a denial of service.</span></span> <span data-ttu-id="f1e58-289">仅支持 NotConfigured 和允许的状态。</span><span class="sxs-lookup"><span data-stu-id="f1e58-289">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="f1e58-290">userRightsRestoreData</span><span class="sxs-lookup"><span data-stu-id="f1e58-290">userRightsRestoreData</span></span>|[<span data-ttu-id="f1e58-291">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="f1e58-291">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="f1e58-292">此用户权限确定在还原备份的文件和目录时, 哪些用户可以绕过文件、目录、注册表和其他持久对象权限, 并确定哪些用户可以将任何有效的安全主体设置为对象的所有者。</span><span class="sxs-lookup"><span data-stu-id="f1e58-292">This user right determines which users can bypass file, directory, registry, and other persistent objects permissions when restoring backed up files and directories, and determines which users can set any valid security principal as the owner of an object.</span></span> <span data-ttu-id="f1e58-293">仅支持 NotConfigured 和允许的状态。</span><span class="sxs-lookup"><span data-stu-id="f1e58-293">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="f1e58-294">userRightsTakeOwnership</span><span class="sxs-lookup"><span data-stu-id="f1e58-294">userRightsTakeOwnership</span></span>|[<span data-ttu-id="f1e58-295">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="f1e58-295">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="f1e58-296">此用户权限确定哪些用户可以获得系统中任何安全对象的所有权, 包括 Active Directory 对象、文件和文件夹、打印机、注册表项、进程和线程。</span><span class="sxs-lookup"><span data-stu-id="f1e58-296">This user right determines which users can take ownership of any securable object in the system, including Active Directory objects, files and folders, printers, registry keys, processes, and threads.</span></span> <span data-ttu-id="f1e58-297">仅支持 NotConfigured 和允许的状态。</span><span class="sxs-lookup"><span data-stu-id="f1e58-297">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="f1e58-298">userRightsRegisterProcessAsService</span><span class="sxs-lookup"><span data-stu-id="f1e58-298">userRightsRegisterProcessAsService</span></span>|[<span data-ttu-id="f1e58-299">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="f1e58-299">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="f1e58-300">此安全设置确定阻止将进程注册为服务的服务帐户。</span><span class="sxs-lookup"><span data-stu-id="f1e58-300">This security setting determines which service accounts are prevented from registering a process as a service.</span></span> <span data-ttu-id="f1e58-301">注意: 此安全设置不适用于系统、本地服务或网络服务帐户。</span><span class="sxs-lookup"><span data-stu-id="f1e58-301">Note: This security setting does not apply to the System, Local Service, or Network Service accounts.</span></span> <span data-ttu-id="f1e58-302">仅支持阻止状态。</span><span class="sxs-lookup"><span data-stu-id="f1e58-302">Only state Blocked is supported.</span></span>|
|<span data-ttu-id="f1e58-303">xboxServicesEnableXboxGameSaveTask</span><span class="sxs-lookup"><span data-stu-id="f1e58-303">xboxServicesEnableXboxGameSaveTask</span></span>|<span data-ttu-id="f1e58-304">布尔</span><span class="sxs-lookup"><span data-stu-id="f1e58-304">Boolean</span></span>|<span data-ttu-id="f1e58-305">此设置确定是否启用了 xbox 游戏保存 (1) 或禁用 (0)。</span><span class="sxs-lookup"><span data-stu-id="f1e58-305">This setting determines whether xbox game save is enabled (1) or disabled (0).</span></span>|
|<span data-ttu-id="f1e58-306">xboxServicesAccessoryManagementServiceStartupMode</span><span class="sxs-lookup"><span data-stu-id="f1e58-306">xboxServicesAccessoryManagementServiceStartupMode</span></span>|[<span data-ttu-id="f1e58-307">serviceStartType</span><span class="sxs-lookup"><span data-stu-id="f1e58-307">serviceStartType</span></span>](../resources/intune-deviceconfig-servicestarttype.md)|<span data-ttu-id="f1e58-308">此设置确定附件管理服务的启动类型是 "自动" (2)、"手动" (3)、"已禁用" (4)。</span><span class="sxs-lookup"><span data-stu-id="f1e58-308">This setting determines whether the Accessory management service's start type is Automatic(2), Manual(3), Disabled(4).</span></span> <span data-ttu-id="f1e58-309">默认: 手动。</span><span class="sxs-lookup"><span data-stu-id="f1e58-309">Default: Manual.</span></span> <span data-ttu-id="f1e58-310">可取值为：`manual`、`automatic`、`disabled`。</span><span class="sxs-lookup"><span data-stu-id="f1e58-310">Possible values are: `manual`, `automatic`, `disabled`.</span></span>|
|<span data-ttu-id="f1e58-311">xboxServicesLiveAuthManagerServiceStartupMode</span><span class="sxs-lookup"><span data-stu-id="f1e58-311">xboxServicesLiveAuthManagerServiceStartupMode</span></span>|[<span data-ttu-id="f1e58-312">serviceStartType</span><span class="sxs-lookup"><span data-stu-id="f1e58-312">serviceStartType</span></span>](../resources/intune-deviceconfig-servicestarttype.md)|<span data-ttu-id="f1e58-313">此设置确定 Live Auth Manager 服务的启动类型是否为自动 (2)、手动 (3)、已禁用 (4)。</span><span class="sxs-lookup"><span data-stu-id="f1e58-313">This setting determines whether Live Auth Manager service's start type is Automatic(2), Manual(3), Disabled(4).</span></span> <span data-ttu-id="f1e58-314">默认: 手动。</span><span class="sxs-lookup"><span data-stu-id="f1e58-314">Default: Manual.</span></span> <span data-ttu-id="f1e58-315">可取值为：`manual`、`automatic`、`disabled`。</span><span class="sxs-lookup"><span data-stu-id="f1e58-315">Possible values are: `manual`, `automatic`, `disabled`.</span></span>|
|<span data-ttu-id="f1e58-316">xboxServicesLiveGameSaveServiceStartupMode</span><span class="sxs-lookup"><span data-stu-id="f1e58-316">xboxServicesLiveGameSaveServiceStartupMode</span></span>|[<span data-ttu-id="f1e58-317">serviceStartType</span><span class="sxs-lookup"><span data-stu-id="f1e58-317">serviceStartType</span></span>](../resources/intune-deviceconfig-servicestarttype.md)|<span data-ttu-id="f1e58-318">此设置确定实时游戏是否保存服务的启动类型为自动 (2)、手动 (3)、已禁用 (4)。</span><span class="sxs-lookup"><span data-stu-id="f1e58-318">This setting determines whether Live Game save service's start type is Automatic(2), Manual(3), Disabled(4).</span></span> <span data-ttu-id="f1e58-319">默认: 手动。</span><span class="sxs-lookup"><span data-stu-id="f1e58-319">Default: Manual.</span></span> <span data-ttu-id="f1e58-320">可取值为：`manual`、`automatic`、`disabled`。</span><span class="sxs-lookup"><span data-stu-id="f1e58-320">Possible values are: `manual`, `automatic`, `disabled`.</span></span>|
|<span data-ttu-id="f1e58-321">xboxServicesLiveNetworkingServiceStartupMode</span><span class="sxs-lookup"><span data-stu-id="f1e58-321">xboxServicesLiveNetworkingServiceStartupMode</span></span>|[<span data-ttu-id="f1e58-322">serviceStartType</span><span class="sxs-lookup"><span data-stu-id="f1e58-322">serviceStartType</span></span>](../resources/intune-deviceconfig-servicestarttype.md)|<span data-ttu-id="f1e58-323">此设置确定网络服务的启动类型是否为自动 (2)、手动 (3)、已禁用 (4)。</span><span class="sxs-lookup"><span data-stu-id="f1e58-323">This setting determines whether Networking service's start type is Automatic(2), Manual(3), Disabled(4).</span></span> <span data-ttu-id="f1e58-324">默认: 手动。</span><span class="sxs-lookup"><span data-stu-id="f1e58-324">Default: Manual.</span></span> <span data-ttu-id="f1e58-325">可取值为：`manual`、`automatic`、`disabled`。</span><span class="sxs-lookup"><span data-stu-id="f1e58-325">Possible values are: `manual`, `automatic`, `disabled`.</span></span>|
|<span data-ttu-id="f1e58-326">localSecurityOptionsBlockMicrosoftAccounts</span><span class="sxs-lookup"><span data-stu-id="f1e58-326">localSecurityOptionsBlockMicrosoftAccounts</span></span>|<span data-ttu-id="f1e58-327">布尔</span><span class="sxs-lookup"><span data-stu-id="f1e58-327">Boolean</span></span>|<span data-ttu-id="f1e58-328">阻止用户向此计算机添加新的 Microsoft 帐户。</span><span class="sxs-lookup"><span data-stu-id="f1e58-328">Prevent users from adding new Microsoft accounts to this computer.</span></span>|
|<span data-ttu-id="f1e58-329">localSecurityOptionsBlockRemoteLogonWithBlankPassword</span><span class="sxs-lookup"><span data-stu-id="f1e58-329">localSecurityOptionsBlockRemoteLogonWithBlankPassword</span></span>|<span data-ttu-id="f1e58-330">布尔</span><span class="sxs-lookup"><span data-stu-id="f1e58-330">Boolean</span></span>|<span data-ttu-id="f1e58-331">启用不受密码保护的本地帐户从物理设备以外的位置进行登录。默认值为已启用</span><span class="sxs-lookup"><span data-stu-id="f1e58-331">Enable Local accounts that are not password protected to log on from locations other than the physical device.Default is enabled</span></span>|
|<span data-ttu-id="f1e58-332">localSecurityOptionsDisableAdministratorAccount</span><span class="sxs-lookup"><span data-stu-id="f1e58-332">localSecurityOptionsDisableAdministratorAccount</span></span>|<span data-ttu-id="f1e58-333">布尔</span><span class="sxs-lookup"><span data-stu-id="f1e58-333">Boolean</span></span>|<span data-ttu-id="f1e58-334">确定是否启用或禁用本地管理员帐户。</span><span class="sxs-lookup"><span data-stu-id="f1e58-334">Determines whether the Local Administrator account is enabled or disabled.</span></span>|
|<span data-ttu-id="f1e58-335">localSecurityOptionsAdministratorAccountName</span><span class="sxs-lookup"><span data-stu-id="f1e58-335">localSecurityOptionsAdministratorAccountName</span></span>|<span data-ttu-id="f1e58-336">字符串</span><span class="sxs-lookup"><span data-stu-id="f1e58-336">String</span></span>|<span data-ttu-id="f1e58-337">定义要与帐户 "管理员" 的安全标识符 (SID) 相关联的不同帐户名称。</span><span class="sxs-lookup"><span data-stu-id="f1e58-337">Define a different account name to be associated with the security identifier (SID) for the account “Administrator”.</span></span>|
|<span data-ttu-id="f1e58-338">localSecurityOptionsDisableGuestAccount</span><span class="sxs-lookup"><span data-stu-id="f1e58-338">localSecurityOptionsDisableGuestAccount</span></span>|<span data-ttu-id="f1e58-339">布尔</span><span class="sxs-lookup"><span data-stu-id="f1e58-339">Boolean</span></span>|<span data-ttu-id="f1e58-340">确定来宾帐户是否已启用或已禁用。</span><span class="sxs-lookup"><span data-stu-id="f1e58-340">Determines if the Guest account is enabled or disabled.</span></span>|
|<span data-ttu-id="f1e58-341">localSecurityOptionsGuestAccountName</span><span class="sxs-lookup"><span data-stu-id="f1e58-341">localSecurityOptionsGuestAccountName</span></span>|<span data-ttu-id="f1e58-342">字符串</span><span class="sxs-lookup"><span data-stu-id="f1e58-342">String</span></span>|<span data-ttu-id="f1e58-343">定义要与帐户 "来宾" 的安全标识符 (SID) 相关联的不同帐户名称。</span><span class="sxs-lookup"><span data-stu-id="f1e58-343">Define a different account name to be associated with the security identifier (SID) for the account “Guest”.</span></span>|
|<span data-ttu-id="f1e58-344">localSecurityOptionsAllowUndockWithoutHavingToLogon</span><span class="sxs-lookup"><span data-stu-id="f1e58-344">localSecurityOptionsAllowUndockWithoutHavingToLogon</span></span>|<span data-ttu-id="f1e58-345">布尔</span><span class="sxs-lookup"><span data-stu-id="f1e58-345">Boolean</span></span>|<span data-ttu-id="f1e58-346">阻止便携式计算机在无需登录的情况下被移除。</span><span class="sxs-lookup"><span data-stu-id="f1e58-346">Prevent a portable computer from being undocked without having to log in.</span></span>|
|<span data-ttu-id="f1e58-347">localSecurityOptionsBlockUsersInstallingPrinterDrivers</span><span class="sxs-lookup"><span data-stu-id="f1e58-347">localSecurityOptionsBlockUsersInstallingPrinterDrivers</span></span>|<span data-ttu-id="f1e58-348">布尔</span><span class="sxs-lookup"><span data-stu-id="f1e58-348">Boolean</span></span>|<span data-ttu-id="f1e58-349">仅在将打印机驱动程序连接到共享打印机时, 才将其限制为仅供管理员安装。</span><span class="sxs-lookup"><span data-stu-id="f1e58-349">Restrict installing printer drivers as part of connecting to a shared printer to admins only.</span></span>|
|<span data-ttu-id="f1e58-350">localSecurityOptionsBlockRemoteOpticalDriveAccess</span><span class="sxs-lookup"><span data-stu-id="f1e58-350">localSecurityOptionsBlockRemoteOpticalDriveAccess</span></span>|<span data-ttu-id="f1e58-351">布尔</span><span class="sxs-lookup"><span data-stu-id="f1e58-351">Boolean</span></span>|<span data-ttu-id="f1e58-352">如果启用此设置, 则仅允许交互式登录用户访问 cd-rom 媒体。</span><span class="sxs-lookup"><span data-stu-id="f1e58-352">Enabling this settings allows only interactively logged on user to access CD-ROM media.</span></span>|
|<span data-ttu-id="f1e58-353">localSecurityOptionsFormatAndEjectOfRemovableMediaAllowedUser</span><span class="sxs-lookup"><span data-stu-id="f1e58-353">localSecurityOptionsFormatAndEjectOfRemovableMediaAllowedUser</span></span>|[<span data-ttu-id="f1e58-354">localSecurityOptionsFormatAndEjectOfRemovableMediaAllowedUserType</span><span class="sxs-lookup"><span data-stu-id="f1e58-354">localSecurityOptionsFormatAndEjectOfRemovableMediaAllowedUserType</span></span>](../resources/intune-deviceconfig-localsecurityoptionsformatandejectofremovablemediaallowedusertype.md)|<span data-ttu-id="f1e58-355">定义允许格式化和弹出可移动 NTFS 媒体的权限。</span><span class="sxs-lookup"><span data-stu-id="f1e58-355">Define who is allowed to format and eject removable NTFS media.</span></span> <span data-ttu-id="f1e58-356">可取值为：`notConfigured`、`administrators`、`administratorsAndPowerUsers`、`administratorsAndInteractiveUsers`。</span><span class="sxs-lookup"><span data-stu-id="f1e58-356">Possible values are: `notConfigured`, `administrators`, `administratorsAndPowerUsers`, `administratorsAndInteractiveUsers`.</span></span>|
|<span data-ttu-id="f1e58-357">localSecurityOptionsMachineInactivityLimit</span><span class="sxs-lookup"><span data-stu-id="f1e58-357">localSecurityOptionsMachineInactivityLimit</span></span>|<span data-ttu-id="f1e58-358">Int32</span><span class="sxs-lookup"><span data-stu-id="f1e58-358">Int32</span></span>|<span data-ttu-id="f1e58-359">在屏幕保护程序运行之前, 定义交互式桌面登录屏幕上不活动的最长分钟数。</span><span class="sxs-lookup"><span data-stu-id="f1e58-359">Define maximum minutes of inactivity on the interactive desktop’s login screen until the screen saver runs.</span></span> <span data-ttu-id="f1e58-360">有效值为0至9999</span><span class="sxs-lookup"><span data-stu-id="f1e58-360">Valid values 0 to 9999</span></span>|
|<span data-ttu-id="f1e58-361">localSecurityOptionsMachineInactivityLimitInMinutes</span><span class="sxs-lookup"><span data-stu-id="f1e58-361">localSecurityOptionsMachineInactivityLimitInMinutes</span></span>|<span data-ttu-id="f1e58-362">Int32</span><span class="sxs-lookup"><span data-stu-id="f1e58-362">Int32</span></span>|<span data-ttu-id="f1e58-363">在屏幕保护程序运行之前, 定义交互式桌面登录屏幕上不活动的最长分钟数。</span><span class="sxs-lookup"><span data-stu-id="f1e58-363">Define maximum minutes of inactivity on the interactive desktop’s login screen until the screen saver runs.</span></span> <span data-ttu-id="f1e58-364">有效值为0至9999</span><span class="sxs-lookup"><span data-stu-id="f1e58-364">Valid values 0 to 9999</span></span>|
|<span data-ttu-id="f1e58-365">localSecurityOptionsDoNotRequireCtrlAltDel</span><span class="sxs-lookup"><span data-stu-id="f1e58-365">localSecurityOptionsDoNotRequireCtrlAltDel</span></span>|<span data-ttu-id="f1e58-366">布尔</span><span class="sxs-lookup"><span data-stu-id="f1e58-366">Boolean</span></span>|<span data-ttu-id="f1e58-367">要求用户在登录前按 CTRL + ALT + DEL。</span><span class="sxs-lookup"><span data-stu-id="f1e58-367">Require CTRL+ALT+DEL to be pressed before a user can log on.</span></span>|
|<span data-ttu-id="f1e58-368">localSecurityOptionsHideLastSignedInUser</span><span class="sxs-lookup"><span data-stu-id="f1e58-368">localSecurityOptionsHideLastSignedInUser</span></span>|<span data-ttu-id="f1e58-369">布尔</span><span class="sxs-lookup"><span data-stu-id="f1e58-369">Boolean</span></span>|<span data-ttu-id="f1e58-370">不显示上次在此设备上登录的用户的用户名。</span><span class="sxs-lookup"><span data-stu-id="f1e58-370">Do not display the username of the last person who signed in on this device.</span></span>|
|<span data-ttu-id="f1e58-371">localSecurityOptionsHideUsernameAtSignIn</span><span class="sxs-lookup"><span data-stu-id="f1e58-371">localSecurityOptionsHideUsernameAtSignIn</span></span>|<span data-ttu-id="f1e58-372">布尔</span><span class="sxs-lookup"><span data-stu-id="f1e58-372">Boolean</span></span>|<span data-ttu-id="f1e58-373">在输入凭据后以及显示设备桌面之前, 请勿显示登录此设备的人员的用户名。</span><span class="sxs-lookup"><span data-stu-id="f1e58-373">Do not display the username of the person signing in to this device after credentials are entered and before the device’s desktop is shown.</span></span>|
|<span data-ttu-id="f1e58-374">localSecurityOptionsLogOnMessageTitle</span><span class="sxs-lookup"><span data-stu-id="f1e58-374">localSecurityOptionsLogOnMessageTitle</span></span>|<span data-ttu-id="f1e58-375">字符串</span><span class="sxs-lookup"><span data-stu-id="f1e58-375">String</span></span>|<span data-ttu-id="f1e58-376">为尝试登录的用户设置消息标题。</span><span class="sxs-lookup"><span data-stu-id="f1e58-376">Set message title for users attempting to log in.</span></span>|
|<span data-ttu-id="f1e58-377">localSecurityOptionsLogOnMessageText</span><span class="sxs-lookup"><span data-stu-id="f1e58-377">localSecurityOptionsLogOnMessageText</span></span>|<span data-ttu-id="f1e58-378">字符串</span><span class="sxs-lookup"><span data-stu-id="f1e58-378">String</span></span>|<span data-ttu-id="f1e58-379">为尝试登录的用户设置消息文本。</span><span class="sxs-lookup"><span data-stu-id="f1e58-379">Set message text for users attempting to log in.</span></span>|
|<span data-ttu-id="f1e58-380">localSecurityOptionsAllowPKU2UAuthenticationRequests</span><span class="sxs-lookup"><span data-stu-id="f1e58-380">localSecurityOptionsAllowPKU2UAuthenticationRequests</span></span>|<span data-ttu-id="f1e58-381">布尔</span><span class="sxs-lookup"><span data-stu-id="f1e58-381">Boolean</span></span>|<span data-ttu-id="f1e58-382">阻止 PKU2U 对此设备的身份验证请求, 以使用联机标识。</span><span class="sxs-lookup"><span data-stu-id="f1e58-382">Block PKU2U authentication requests to this device to use online identities.</span></span>|
|<span data-ttu-id="f1e58-383">localSecurityOptionsAllowRemoteCallsToSecurityAccountsManagerHelperBool</span><span class="sxs-lookup"><span data-stu-id="f1e58-383">localSecurityOptionsAllowRemoteCallsToSecurityAccountsManagerHelperBool</span></span>|<span data-ttu-id="f1e58-384">布尔</span><span class="sxs-lookup"><span data-stu-id="f1e58-384">Boolean</span></span>|<span data-ttu-id="f1e58-385">LocalSecurityOptionsAllowRemoteCallsToSecurityAccountsManager 实体的 UI 帮助程序布尔值</span><span class="sxs-lookup"><span data-stu-id="f1e58-385">UI helper boolean for LocalSecurityOptionsAllowRemoteCallsToSecurityAccountsManager entity</span></span>|
|<span data-ttu-id="f1e58-386">localSecurityOptionsAllowRemoteCallsToSecurityAccountsManager</span><span class="sxs-lookup"><span data-stu-id="f1e58-386">localSecurityOptionsAllowRemoteCallsToSecurityAccountsManager</span></span>|<span data-ttu-id="f1e58-387">字符串</span><span class="sxs-lookup"><span data-stu-id="f1e58-387">String</span></span>|<span data-ttu-id="f1e58-388">编辑默认的安全描述符定义语言字符串, 以允许或拒绝用户和组对 SAM 进行远程调用。</span><span class="sxs-lookup"><span data-stu-id="f1e58-388">Edit the default Security Descriptor Definition Language string to allow or deny users and groups to make remote calls to the SAM.</span></span>|
|<span data-ttu-id="f1e58-389">localSecurityOptionsMinimumSessionSecurityForNtlmSspBasedClients</span><span class="sxs-lookup"><span data-stu-id="f1e58-389">localSecurityOptionsMinimumSessionSecurityForNtlmSspBasedClients</span></span>|[<span data-ttu-id="f1e58-390">localSecurityOptionsMinimumSessionSecurity</span><span class="sxs-lookup"><span data-stu-id="f1e58-390">localSecurityOptionsMinimumSessionSecurity</span></span>](../resources/intune-deviceconfig-localsecurityoptionsminimumsessionsecurity.md)|<span data-ttu-id="f1e58-391">此安全设置允许客户端要求协商128位加密和/或 NTLMv2 会话安全性。</span><span class="sxs-lookup"><span data-stu-id="f1e58-391">This security setting allows a client to require the negotiation of 128-bit encryption and/or NTLMv2 session security.</span></span> <span data-ttu-id="f1e58-392">可取值为：`none`、`requireNtmlV2SessionSecurity`、`require128BitEncryption`、`ntlmV2And128BitEncryption`。</span><span class="sxs-lookup"><span data-stu-id="f1e58-392">Possible values are: `none`, `requireNtmlV2SessionSecurity`, `require128BitEncryption`, `ntlmV2And128BitEncryption`.</span></span>|
|<span data-ttu-id="f1e58-393">localSecurityOptionsMinimumSessionSecurityForNtlmSspBasedServers</span><span class="sxs-lookup"><span data-stu-id="f1e58-393">localSecurityOptionsMinimumSessionSecurityForNtlmSspBasedServers</span></span>|[<span data-ttu-id="f1e58-394">localSecurityOptionsMinimumSessionSecurity</span><span class="sxs-lookup"><span data-stu-id="f1e58-394">localSecurityOptionsMinimumSessionSecurity</span></span>](../resources/intune-deviceconfig-localsecurityoptionsminimumsessionsecurity.md)|<span data-ttu-id="f1e58-395">此安全设置允许服务器要求协商128位加密和/或 NTLMv2 会话安全性。</span><span class="sxs-lookup"><span data-stu-id="f1e58-395">This security setting allows a server to require the negotiation of 128-bit encryption and/or NTLMv2 session security.</span></span> <span data-ttu-id="f1e58-396">可取值为：`none`、`requireNtmlV2SessionSecurity`、`require128BitEncryption`、`ntlmV2And128BitEncryption`。</span><span class="sxs-lookup"><span data-stu-id="f1e58-396">Possible values are: `none`, `requireNtmlV2SessionSecurity`, `require128BitEncryption`, `ntlmV2And128BitEncryption`.</span></span>|
|<span data-ttu-id="f1e58-397">lanManagerAuthenticationLevel</span><span class="sxs-lookup"><span data-stu-id="f1e58-397">lanManagerAuthenticationLevel</span></span>|[<span data-ttu-id="f1e58-398">lanManagerAuthenticationLevel</span><span class="sxs-lookup"><span data-stu-id="f1e58-398">lanManagerAuthenticationLevel</span></span>](../resources/intune-deviceconfig-lanmanagerauthenticationlevel.md)|<span data-ttu-id="f1e58-399">此安全设置确定用于网络登录的质询/响应身份验证协议。</span><span class="sxs-lookup"><span data-stu-id="f1e58-399">This security setting determines which challenge/response authentication protocol is used for network logons.</span></span> <span data-ttu-id="f1e58-400">可取值为：`lmAndNltm`、`lmNtlmAndNtlmV2`、`lmAndNtlmOnly`、`lmAndNtlmV2`、`lmNtlmV2AndNotLm`、`lmNtlmV2AndNotLmOrNtm`。</span><span class="sxs-lookup"><span data-stu-id="f1e58-400">Possible values are: `lmAndNltm`, `lmNtlmAndNtlmV2`, `lmAndNtlmOnly`, `lmAndNtlmV2`, `lmNtlmV2AndNotLm`, `lmNtlmV2AndNotLmOrNtm`.</span></span>|
|<span data-ttu-id="f1e58-401">lanManagerWorkstationDisableInsecureGuestLogons</span><span class="sxs-lookup"><span data-stu-id="f1e58-401">lanManagerWorkstationDisableInsecureGuestLogons</span></span>|<span data-ttu-id="f1e58-402">布尔</span><span class="sxs-lookup"><span data-stu-id="f1e58-402">Boolean</span></span>|<span data-ttu-id="f1e58-403">如果启用, SMB 客户端将允许不安全的来宾登录。</span><span class="sxs-lookup"><span data-stu-id="f1e58-403">If enabled,the SMB client will allow insecure guest logons.</span></span> <span data-ttu-id="f1e58-404">如果未配置, SMB 客户端将拒绝不安全的来宾登录。</span><span class="sxs-lookup"><span data-stu-id="f1e58-404">If not configured, the SMB client will reject insecure guest logons.</span></span>|
|<span data-ttu-id="f1e58-405">localSecurityOptionsClearVirtualMemoryPageFile</span><span class="sxs-lookup"><span data-stu-id="f1e58-405">localSecurityOptionsClearVirtualMemoryPageFile</span></span>|<span data-ttu-id="f1e58-406">布尔</span><span class="sxs-lookup"><span data-stu-id="f1e58-406">Boolean</span></span>|<span data-ttu-id="f1e58-407">此安全设置确定在关闭系统时是否清除虚拟内存页面文件。</span><span class="sxs-lookup"><span data-stu-id="f1e58-407">This security setting determines whether the virtual memory pagefile is cleared when the system is shut down.</span></span>|
|<span data-ttu-id="f1e58-408">localSecurityOptionsAllowSystemToBeShutDownWithoutHavingToLogOn</span><span class="sxs-lookup"><span data-stu-id="f1e58-408">localSecurityOptionsAllowSystemToBeShutDownWithoutHavingToLogOn</span></span>|<span data-ttu-id="f1e58-409">布尔</span><span class="sxs-lookup"><span data-stu-id="f1e58-409">Boolean</span></span>|<span data-ttu-id="f1e58-410">此安全设置确定是否可以在不登录 Windows 的情况下关闭计算机。</span><span class="sxs-lookup"><span data-stu-id="f1e58-410">This security setting determines whether a computer can be shut down without having to log on to Windows.</span></span>|
|<span data-ttu-id="f1e58-411">localSecurityOptionsAllowUIAccessApplicationElevation</span><span class="sxs-lookup"><span data-stu-id="f1e58-411">localSecurityOptionsAllowUIAccessApplicationElevation</span></span>|<span data-ttu-id="f1e58-412">布尔</span><span class="sxs-lookup"><span data-stu-id="f1e58-412">Boolean</span></span>|<span data-ttu-id="f1e58-413">允许 UIAccess 应用在不使用安全桌面的情况下提示提升。</span><span class="sxs-lookup"><span data-stu-id="f1e58-413">Allow UIAccess apps to prompt for elevation without using the secure desktop.</span></span>|
|<span data-ttu-id="f1e58-414">localSecurityOptionsVirtualizeFileAndRegistryWriteFailuresToPerUserLocations</span><span class="sxs-lookup"><span data-stu-id="f1e58-414">localSecurityOptionsVirtualizeFileAndRegistryWriteFailuresToPerUserLocations</span></span>|<span data-ttu-id="f1e58-415">布尔</span><span class="sxs-lookup"><span data-stu-id="f1e58-415">Boolean</span></span>|<span data-ttu-id="f1e58-416">将文件和注册表写入失败虚拟化到每个用户位置</span><span class="sxs-lookup"><span data-stu-id="f1e58-416">Virtualize file and registry write failures to per user locations</span></span>|
|<span data-ttu-id="f1e58-417">localSecurityOptionsOnlyElevateSignedExecutables</span><span class="sxs-lookup"><span data-stu-id="f1e58-417">localSecurityOptionsOnlyElevateSignedExecutables</span></span>|<span data-ttu-id="f1e58-418">布尔</span><span class="sxs-lookup"><span data-stu-id="f1e58-418">Boolean</span></span>|<span data-ttu-id="f1e58-419">对给定的可执行文件强制执行 PKI 证书路径验证, 然后再允许运行该文件。</span><span class="sxs-lookup"><span data-stu-id="f1e58-419">Enforce PKI certification path validation for a given executable file before it is permitted to run.</span></span>|
|<span data-ttu-id="f1e58-420">localSecurityOptionsAdministratorElevationPromptBehavior</span><span class="sxs-lookup"><span data-stu-id="f1e58-420">localSecurityOptionsAdministratorElevationPromptBehavior</span></span>|[<span data-ttu-id="f1e58-421">localSecurityOptionsAdministratorElevationPromptBehaviorType</span><span class="sxs-lookup"><span data-stu-id="f1e58-421">localSecurityOptionsAdministratorElevationPromptBehaviorType</span></span>](../resources/intune-deviceconfig-localsecurityoptionsadministratorelevationpromptbehaviortype.md)|<span data-ttu-id="f1e58-422">在管理员审批模式中定义管理员的提升提示行为。</span><span class="sxs-lookup"><span data-stu-id="f1e58-422">Define the behavior of the elevation prompt for admins in Admin Approval Mode.</span></span> <span data-ttu-id="f1e58-423">可取值为：`notConfigured`、`elevateWithoutPrompting`、`promptForCredentialsOnTheSecureDesktop`、`promptForConsentOnTheSecureDesktop`、`promptForCredentials`、`promptForConsent` 或 `promptForConsentForNonWindowsBinaries`。</span><span class="sxs-lookup"><span data-stu-id="f1e58-423">Possible values are: `notConfigured`, `elevateWithoutPrompting`, `promptForCredentialsOnTheSecureDesktop`, `promptForConsentOnTheSecureDesktop`, `promptForCredentials`, `promptForConsent`, `promptForConsentForNonWindowsBinaries`.</span></span>|
|<span data-ttu-id="f1e58-424">localSecurityOptionsStandardUserElevationPromptBehavior</span><span class="sxs-lookup"><span data-stu-id="f1e58-424">localSecurityOptionsStandardUserElevationPromptBehavior</span></span>|[<span data-ttu-id="f1e58-425">localSecurityOptionsStandardUserElevationPromptBehaviorType</span><span class="sxs-lookup"><span data-stu-id="f1e58-425">localSecurityOptionsStandardUserElevationPromptBehaviorType</span></span>](../resources/intune-deviceconfig-localsecurityoptionsstandarduserelevationpromptbehaviortype.md)|<span data-ttu-id="f1e58-426">定义标准用户的提升提示行为。</span><span class="sxs-lookup"><span data-stu-id="f1e58-426">Define the behavior of the elevation prompt for standard users.</span></span> <span data-ttu-id="f1e58-427">可取值为：`notConfigured`、`automaticallyDenyElevationRequests`、`promptForCredentialsOnTheSecureDesktop`、`promptForCredentials`。</span><span class="sxs-lookup"><span data-stu-id="f1e58-427">Possible values are: `notConfigured`, `automaticallyDenyElevationRequests`, `promptForCredentialsOnTheSecureDesktop`, `promptForCredentials`.</span></span>|
|<span data-ttu-id="f1e58-428">localSecurityOptionsSwitchToSecureDesktopWhenPromptingForElevation</span><span class="sxs-lookup"><span data-stu-id="f1e58-428">localSecurityOptionsSwitchToSecureDesktopWhenPromptingForElevation</span></span>|<span data-ttu-id="f1e58-429">布尔</span><span class="sxs-lookup"><span data-stu-id="f1e58-429">Boolean</span></span>|<span data-ttu-id="f1e58-430">启用所有提升请求以转到交互式用户的桌面, 而不是安全桌面。</span><span class="sxs-lookup"><span data-stu-id="f1e58-430">Enable all elevation requests to go to the interactive user's desktop rather than the secure desktop.</span></span> <span data-ttu-id="f1e58-431">使用管理员和标准用户的提示行为策略设置。</span><span class="sxs-lookup"><span data-stu-id="f1e58-431">Prompt behavior policy settings for admins and standard users are used.</span></span>|
|<span data-ttu-id="f1e58-432">localSecurityOptionsDetectApplicationInstallationsAndPromptForElevation</span><span class="sxs-lookup"><span data-stu-id="f1e58-432">localSecurityOptionsDetectApplicationInstallationsAndPromptForElevation</span></span>|<span data-ttu-id="f1e58-433">布尔</span><span class="sxs-lookup"><span data-stu-id="f1e58-433">Boolean</span></span>|<span data-ttu-id="f1e58-434">需要提升权限的应用程序安装将提示管理凭据。默认值为已启用</span><span class="sxs-lookup"><span data-stu-id="f1e58-434">App installations requiring elevated privileges will prompt for admin credentials.Default is enabled</span></span>|
|<span data-ttu-id="f1e58-435">localSecurityOptionsAllowUIAccessApplicationsForSecureLocations</span><span class="sxs-lookup"><span data-stu-id="f1e58-435">localSecurityOptionsAllowUIAccessApplicationsForSecureLocations</span></span>|<span data-ttu-id="f1e58-436">布尔</span><span class="sxs-lookup"><span data-stu-id="f1e58-436">Boolean</span></span>|<span data-ttu-id="f1e58-437">允许 UIAccess 应用在不使用安全桌面的情况下提示提升。默认值为已启用</span><span class="sxs-lookup"><span data-stu-id="f1e58-437">Allow UIAccess apps to prompt for elevation without using the secure desktop.Default is enabled</span></span>|
|<span data-ttu-id="f1e58-438">localSecurityOptionsUseAdminApprovalMode</span><span class="sxs-lookup"><span data-stu-id="f1e58-438">localSecurityOptionsUseAdminApprovalMode</span></span>|<span data-ttu-id="f1e58-439">布尔</span><span class="sxs-lookup"><span data-stu-id="f1e58-439">Boolean</span></span>|<span data-ttu-id="f1e58-440">定义内置管理员帐户是使用管理员审批模式, 还是运行所有具有完全管理员权限的应用程序。默认值为已启用</span><span class="sxs-lookup"><span data-stu-id="f1e58-440">Defines whether the built-in admin account uses Admin Approval Mode or runs all apps with full admin privileges.Default is enabled</span></span>|
|<span data-ttu-id="f1e58-441">localSecurityOptionsUseAdminApprovalModeForAdministrators</span><span class="sxs-lookup"><span data-stu-id="f1e58-441">localSecurityOptionsUseAdminApprovalModeForAdministrators</span></span>|<span data-ttu-id="f1e58-442">布尔</span><span class="sxs-lookup"><span data-stu-id="f1e58-442">Boolean</span></span>|<span data-ttu-id="f1e58-443">定义是否启用管理员批准模式和所有 UAC 策略设置, 默认为启用</span><span class="sxs-lookup"><span data-stu-id="f1e58-443">Define whether Admin Approval Mode and all UAC policy settings are enabled, default is enabled</span></span>|
|<span data-ttu-id="f1e58-444">localSecurityOptionsInformationShownOnLockScreen</span><span class="sxs-lookup"><span data-stu-id="f1e58-444">localSecurityOptionsInformationShownOnLockScreen</span></span>|[<span data-ttu-id="f1e58-445">localSecurityOptionsInformationShownOnLockScreenType</span><span class="sxs-lookup"><span data-stu-id="f1e58-445">localSecurityOptionsInformationShownOnLockScreenType</span></span>](../resources/intune-deviceconfig-localsecurityoptionsinformationshownonlockscreentype.md)|<span data-ttu-id="f1e58-446">配置在会话锁定时显示的用户信息。</span><span class="sxs-lookup"><span data-stu-id="f1e58-446">Configure the user information that is displayed when the session is locked.</span></span> <span data-ttu-id="f1e58-447">如果未配置, 则显示用户显示名称、域和用户名。</span><span class="sxs-lookup"><span data-stu-id="f1e58-447">If not configured, user display name, domain and username are shown.</span></span> <span data-ttu-id="f1e58-448">可取值为：`notConfigured`、`userDisplayNameDomainUser`、`userDisplayNameOnly`、`doNotDisplayUser`。</span><span class="sxs-lookup"><span data-stu-id="f1e58-448">Possible values are: `notConfigured`, `userDisplayNameDomainUser`, `userDisplayNameOnly`, `doNotDisplayUser`.</span></span>|
|<span data-ttu-id="f1e58-449">localSecurityOptionsInformationDisplayedOnLockScreen</span><span class="sxs-lookup"><span data-stu-id="f1e58-449">localSecurityOptionsInformationDisplayedOnLockScreen</span></span>|[<span data-ttu-id="f1e58-450">localSecurityOptionsInformationDisplayedOnLockScreenType</span><span class="sxs-lookup"><span data-stu-id="f1e58-450">localSecurityOptionsInformationDisplayedOnLockScreenType</span></span>](../resources/intune-deviceconfig-localsecurityoptionsinformationdisplayedonlockscreentype.md)|<span data-ttu-id="f1e58-451">配置在会话锁定时显示的用户信息。</span><span class="sxs-lookup"><span data-stu-id="f1e58-451">Configure the user information that is displayed when the session is locked.</span></span> <span data-ttu-id="f1e58-452">如果未配置, 则显示用户显示名称、域和用户名。</span><span class="sxs-lookup"><span data-stu-id="f1e58-452">If not configured, user display name, domain and username are shown.</span></span> <span data-ttu-id="f1e58-453">可取值为：`notConfigured`、`administrators`、`administratorsAndPowerUsers`、`administratorsAndInteractiveUsers`。</span><span class="sxs-lookup"><span data-stu-id="f1e58-453">Possible values are: `notConfigured`, `administrators`, `administratorsAndPowerUsers`, `administratorsAndInteractiveUsers`.</span></span>|
|<span data-ttu-id="f1e58-454">localSecurityOptionsDisableClientDigitallySignCommunicationsIfServerAgrees</span><span class="sxs-lookup"><span data-stu-id="f1e58-454">localSecurityOptionsDisableClientDigitallySignCommunicationsIfServerAgrees</span></span>|<span data-ttu-id="f1e58-455">布尔</span><span class="sxs-lookup"><span data-stu-id="f1e58-455">Boolean</span></span>|<span data-ttu-id="f1e58-456">此安全设置确定 smb 客户端是否尝试协商 smb 数据包签名。</span><span class="sxs-lookup"><span data-stu-id="f1e58-456">This security setting determines whether the SMB client attempts to negotiate SMB packet signing.</span></span>|
|<span data-ttu-id="f1e58-457">localSecurityOptionsClientDigitallySignCommunicationsAlways</span><span class="sxs-lookup"><span data-stu-id="f1e58-457">localSecurityOptionsClientDigitallySignCommunicationsAlways</span></span>|<span data-ttu-id="f1e58-458">布尔</span><span class="sxs-lookup"><span data-stu-id="f1e58-458">Boolean</span></span>|<span data-ttu-id="f1e58-459">此安全设置确定 SMB 客户端组件是否需要数据包签名。</span><span class="sxs-lookup"><span data-stu-id="f1e58-459">This security setting determines whether packet signing is required by the SMB client component.</span></span>|
|<span data-ttu-id="f1e58-460">localSecurityOptionsClientSendUnencryptedPasswordToThirdPartySMBServers</span><span class="sxs-lookup"><span data-stu-id="f1e58-460">localSecurityOptionsClientSendUnencryptedPasswordToThirdPartySMBServers</span></span>|<span data-ttu-id="f1e58-461">布尔</span><span class="sxs-lookup"><span data-stu-id="f1e58-461">Boolean</span></span>|<span data-ttu-id="f1e58-462">如果启用此安全设置, 则允许服务器消息块 (SMB) 重定向程序将纯文本密码发送到在身份验证过程中不支持密码加密的非 Microsoft SMB 服务器。</span><span class="sxs-lookup"><span data-stu-id="f1e58-462">If this security setting is enabled, the Server Message Block (SMB) redirector is allowed to send plaintext passwords to non-Microsoft SMB servers that do not support password encryption during authentication.</span></span>|
|<span data-ttu-id="f1e58-463">localSecurityOptionsDisableServerDigitallySignCommunicationsAlways</span><span class="sxs-lookup"><span data-stu-id="f1e58-463">localSecurityOptionsDisableServerDigitallySignCommunicationsAlways</span></span>|<span data-ttu-id="f1e58-464">布尔</span><span class="sxs-lookup"><span data-stu-id="f1e58-464">Boolean</span></span>|<span data-ttu-id="f1e58-465">此安全设置确定 SMB 服务器组件是否需要数据包签名。</span><span class="sxs-lookup"><span data-stu-id="f1e58-465">This security setting determines whether packet signing is required by the SMB server component.</span></span>|
|<span data-ttu-id="f1e58-466">localSecurityOptionsDisableServerDigitallySignCommunicationsIfClientAgrees</span><span class="sxs-lookup"><span data-stu-id="f1e58-466">localSecurityOptionsDisableServerDigitallySignCommunicationsIfClientAgrees</span></span>|<span data-ttu-id="f1e58-467">布尔</span><span class="sxs-lookup"><span data-stu-id="f1e58-467">Boolean</span></span>|<span data-ttu-id="f1e58-468">此安全设置确定 smb 服务器是否将 smb 数据包签名与请求的客户端协商。</span><span class="sxs-lookup"><span data-stu-id="f1e58-468">This security setting determines whether the SMB server will negotiate SMB packet signing with clients that request it.</span></span>|
|<span data-ttu-id="f1e58-469">localSecurityOptionsRestrictAnonymousAccessToNamedPipesAndShares</span><span class="sxs-lookup"><span data-stu-id="f1e58-469">localSecurityOptionsRestrictAnonymousAccessToNamedPipesAndShares</span></span>|<span data-ttu-id="f1e58-470">布尔</span><span class="sxs-lookup"><span data-stu-id="f1e58-470">Boolean</span></span>|<span data-ttu-id="f1e58-471">默认情况下, 此安全设置限制可匿名访问且可匿名访问的共享的命名管道设置对共享和管道的匿名访问权限</span><span class="sxs-lookup"><span data-stu-id="f1e58-471">By default, this security setting restricts anonymous access to shares and pipes to the settings for named pipes that can be accessed anonymously and Shares that can be accessed anonymously</span></span>|
|<span data-ttu-id="f1e58-472">localSecurityOptionsDoNotAllowAnonymousEnumerationOfSAMAccounts</span><span class="sxs-lookup"><span data-stu-id="f1e58-472">localSecurityOptionsDoNotAllowAnonymousEnumerationOfSAMAccounts</span></span>|<span data-ttu-id="f1e58-473">布尔</span><span class="sxs-lookup"><span data-stu-id="f1e58-473">Boolean</span></span>|<span data-ttu-id="f1e58-474">此安全设置确定将向计算机的匿名连接授予的其他权限。</span><span class="sxs-lookup"><span data-stu-id="f1e58-474">This security setting determines what additional permissions will be granted for anonymous connections to the computer.</span></span>|
|<span data-ttu-id="f1e58-475">localSecurityOptionsAllowAnonymousEnumerationOfSAMAccountsAndShares</span><span class="sxs-lookup"><span data-stu-id="f1e58-475">localSecurityOptionsAllowAnonymousEnumerationOfSAMAccountsAndShares</span></span>|<span data-ttu-id="f1e58-476">布尔</span><span class="sxs-lookup"><span data-stu-id="f1e58-476">Boolean</span></span>|<span data-ttu-id="f1e58-477">此安全设置确定是否允许匿名用户执行某些活动, 如枚举域帐户和网络共享的名称。</span><span class="sxs-lookup"><span data-stu-id="f1e58-477">This security setting determines whether to allows anonymous users to perform certain activities, such as enumerating the names of domain accounts and network shares.</span></span>|
|<span data-ttu-id="f1e58-478">localSecurityOptionsDoNotStoreLANManagerHashValueOnNextPasswordChange</span><span class="sxs-lookup"><span data-stu-id="f1e58-478">localSecurityOptionsDoNotStoreLANManagerHashValueOnNextPasswordChange</span></span>|<span data-ttu-id="f1e58-479">布尔</span><span class="sxs-lookup"><span data-stu-id="f1e58-479">Boolean</span></span>|<span data-ttu-id="f1e58-480">此安全设置确定在下一次更改密码时, 是否存储新密码的 LAN Manager (LM) 哈希值。</span><span class="sxs-lookup"><span data-stu-id="f1e58-480">This security setting determines if, at the next password change, the LAN Manager (LM) hash value for the new password is stored.</span></span> <span data-ttu-id="f1e58-481">默认情况下不存储它。</span><span class="sxs-lookup"><span data-stu-id="f1e58-481">It’s not stored by default.</span></span>|
|<span data-ttu-id="f1e58-482">localSecurityOptionsSmartCardRemovalBehavior</span><span class="sxs-lookup"><span data-stu-id="f1e58-482">localSecurityOptionsSmartCardRemovalBehavior</span></span>|[<span data-ttu-id="f1e58-483">localSecurityOptionsSmartCardRemovalBehaviorType</span><span class="sxs-lookup"><span data-stu-id="f1e58-483">localSecurityOptionsSmartCardRemovalBehaviorType</span></span>](../resources/intune-deviceconfig-localsecurityoptionssmartcardremovalbehaviortype.md)|<span data-ttu-id="f1e58-484">此安全设置确定将已登录用户的智能卡从智能卡读卡器中删除时发生的情况。</span><span class="sxs-lookup"><span data-stu-id="f1e58-484">This security setting determines what happens when the smart card for a logged-on user is removed from the smart card reader.</span></span> <span data-ttu-id="f1e58-485">可取值为：`lockWorkstation`、`noAction`、`forceLogoff`、`disconnectRemoteDesktopSession`。</span><span class="sxs-lookup"><span data-stu-id="f1e58-485">Possible values are: `lockWorkstation`, `noAction`, `forceLogoff`, `disconnectRemoteDesktopSession`.</span></span>|
|<span data-ttu-id="f1e58-486">defenderSecurityCenterDisableAppBrowserUI</span><span class="sxs-lookup"><span data-stu-id="f1e58-486">defenderSecurityCenterDisableAppBrowserUI</span></span>|<span data-ttu-id="f1e58-487">布尔</span><span class="sxs-lookup"><span data-stu-id="f1e58-487">Boolean</span></span>|<span data-ttu-id="f1e58-488">用于禁用应用程序和浏览器保护区域的显示。</span><span class="sxs-lookup"><span data-stu-id="f1e58-488">Used to disable the display of the app and browser protection area.</span></span>|
|<span data-ttu-id="f1e58-489">defenderSecurityCenterDisableFamilyUI</span><span class="sxs-lookup"><span data-stu-id="f1e58-489">defenderSecurityCenterDisableFamilyUI</span></span>|<span data-ttu-id="f1e58-490">布尔</span><span class="sxs-lookup"><span data-stu-id="f1e58-490">Boolean</span></span>|<span data-ttu-id="f1e58-491">用于禁用 "家庭选项" 区域的显示。</span><span class="sxs-lookup"><span data-stu-id="f1e58-491">Used to disable the display of the family options area.</span></span>|
|<span data-ttu-id="f1e58-492">defenderSecurityCenterDisableHealthUI</span><span class="sxs-lookup"><span data-stu-id="f1e58-492">defenderSecurityCenterDisableHealthUI</span></span>|<span data-ttu-id="f1e58-493">布尔</span><span class="sxs-lookup"><span data-stu-id="f1e58-493">Boolean</span></span>|<span data-ttu-id="f1e58-494">用于禁用设备性能和运行状况区域的显示。</span><span class="sxs-lookup"><span data-stu-id="f1e58-494">Used to disable the display of the device performance and health area.</span></span>|
|<span data-ttu-id="f1e58-495">defenderSecurityCenterDisableNetworkUI</span><span class="sxs-lookup"><span data-stu-id="f1e58-495">defenderSecurityCenterDisableNetworkUI</span></span>|<span data-ttu-id="f1e58-496">布尔</span><span class="sxs-lookup"><span data-stu-id="f1e58-496">Boolean</span></span>|<span data-ttu-id="f1e58-497">用于禁用防火墙和网络防护区域的显示。</span><span class="sxs-lookup"><span data-stu-id="f1e58-497">Used to disable the display of the firewall and network protection area.</span></span>|
|<span data-ttu-id="f1e58-498">defenderSecurityCenterDisableVirusUI</span><span class="sxs-lookup"><span data-stu-id="f1e58-498">defenderSecurityCenterDisableVirusUI</span></span>|<span data-ttu-id="f1e58-499">布尔</span><span class="sxs-lookup"><span data-stu-id="f1e58-499">Boolean</span></span>|<span data-ttu-id="f1e58-500">用于禁用病毒和威胁防护区域的显示。</span><span class="sxs-lookup"><span data-stu-id="f1e58-500">Used to disable the display of the virus and threat protection area.</span></span>|
|<span data-ttu-id="f1e58-501">defenderSecurityCenterDisableAccountUI</span><span class="sxs-lookup"><span data-stu-id="f1e58-501">defenderSecurityCenterDisableAccountUI</span></span>|<span data-ttu-id="f1e58-502">布尔</span><span class="sxs-lookup"><span data-stu-id="f1e58-502">Boolean</span></span>|<span data-ttu-id="f1e58-503">用于禁用帐户保护区域的显示。</span><span class="sxs-lookup"><span data-stu-id="f1e58-503">Used to disable the display of the account protection area.</span></span>|
|<span data-ttu-id="f1e58-504">defenderSecurityCenterDisableClearTpmUI</span><span class="sxs-lookup"><span data-stu-id="f1e58-504">defenderSecurityCenterDisableClearTpmUI</span></span>|<span data-ttu-id="f1e58-505">布尔</span><span class="sxs-lookup"><span data-stu-id="f1e58-505">Boolean</span></span>|<span data-ttu-id="f1e58-506">用于禁用 "清除 TPM" 按钮的显示。</span><span class="sxs-lookup"><span data-stu-id="f1e58-506">Used to disable the display of the Clear TPM button.</span></span>|
|<span data-ttu-id="f1e58-507">defenderSecurityCenterDisableHardwareUI</span><span class="sxs-lookup"><span data-stu-id="f1e58-507">defenderSecurityCenterDisableHardwareUI</span></span>|<span data-ttu-id="f1e58-508">布尔</span><span class="sxs-lookup"><span data-stu-id="f1e58-508">Boolean</span></span>|<span data-ttu-id="f1e58-509">用于禁用硬件保护区域的显示。</span><span class="sxs-lookup"><span data-stu-id="f1e58-509">Used to disable the display of the hardware protection area.</span></span>|
|<span data-ttu-id="f1e58-510">defenderSecurityCenterDisableNotificationAreaUI</span><span class="sxs-lookup"><span data-stu-id="f1e58-510">defenderSecurityCenterDisableNotificationAreaUI</span></span>|<span data-ttu-id="f1e58-511">布尔</span><span class="sxs-lookup"><span data-stu-id="f1e58-511">Boolean</span></span>|<span data-ttu-id="f1e58-512">用于禁用通知区域控件的显示。</span><span class="sxs-lookup"><span data-stu-id="f1e58-512">Used to disable the display of the notification area control.</span></span> <span data-ttu-id="f1e58-513">用户需要注销并登录或重新启动计算机, 此设置才会生效。</span><span class="sxs-lookup"><span data-stu-id="f1e58-513">The user needs to either sign out and sign in or reboot the computer for this setting to take effect.</span></span>|
|<span data-ttu-id="f1e58-514">defenderSecurityCenterDisableRansomwareUI</span><span class="sxs-lookup"><span data-stu-id="f1e58-514">defenderSecurityCenterDisableRansomwareUI</span></span>|<span data-ttu-id="f1e58-515">布尔</span><span class="sxs-lookup"><span data-stu-id="f1e58-515">Boolean</span></span>|<span data-ttu-id="f1e58-516">用于禁用勒索软件防护区域的显示。</span><span class="sxs-lookup"><span data-stu-id="f1e58-516">Used to disable the display of the ransomware protection area.</span></span> |
|<span data-ttu-id="f1e58-517">defenderSecurityCenterDisableSecureBootUI</span><span class="sxs-lookup"><span data-stu-id="f1e58-517">defenderSecurityCenterDisableSecureBootUI</span></span>|<span data-ttu-id="f1e58-518">布尔</span><span class="sxs-lookup"><span data-stu-id="f1e58-518">Boolean</span></span>|<span data-ttu-id="f1e58-519">用于在 "设备安全性" 下禁用安全引导区域的显示。</span><span class="sxs-lookup"><span data-stu-id="f1e58-519">Used to disable the display of the secure boot area under Device security.</span></span>|
|<span data-ttu-id="f1e58-520">defenderSecurityCenterDisableTroubleshootingUI</span><span class="sxs-lookup"><span data-stu-id="f1e58-520">defenderSecurityCenterDisableTroubleshootingUI</span></span>|<span data-ttu-id="f1e58-521">布尔</span><span class="sxs-lookup"><span data-stu-id="f1e58-521">Boolean</span></span>|<span data-ttu-id="f1e58-522">用于在 "设备安全性" 下禁用安全过程故障排除的显示。</span><span class="sxs-lookup"><span data-stu-id="f1e58-522">Used to disable the display of the security process troubleshooting under Device security.</span></span>|
|<span data-ttu-id="f1e58-523">defenderSecurityCenterDisableVulnerableTpmFirmwareUpdateUI</span><span class="sxs-lookup"><span data-stu-id="f1e58-523">defenderSecurityCenterDisableVulnerableTpmFirmwareUpdateUI</span></span>|<span data-ttu-id="f1e58-524">布尔</span><span class="sxs-lookup"><span data-stu-id="f1e58-524">Boolean</span></span>|<span data-ttu-id="f1e58-525">用于在检测到易受攻击的固件时禁用显示更新 TPM 固件。</span><span class="sxs-lookup"><span data-stu-id="f1e58-525">Used to disable the display of update TPM Firmware when a vulnerable firmware is detected.</span></span>|
|<span data-ttu-id="f1e58-526">defenderSecurityCenterOrganizationDisplayName</span><span class="sxs-lookup"><span data-stu-id="f1e58-526">defenderSecurityCenterOrganizationDisplayName</span></span>|<span data-ttu-id="f1e58-527">字符串</span><span class="sxs-lookup"><span data-stu-id="f1e58-527">String</span></span>|<span data-ttu-id="f1e58-528">向用户显示的公司名称。</span><span class="sxs-lookup"><span data-stu-id="f1e58-528">The company name that is displayed to the users.</span></span>|
|<span data-ttu-id="f1e58-529">defenderSecurityCenterHelpEmail</span><span class="sxs-lookup"><span data-stu-id="f1e58-529">defenderSecurityCenterHelpEmail</span></span>|<span data-ttu-id="f1e58-530">字符串</span><span class="sxs-lookup"><span data-stu-id="f1e58-530">String</span></span>|<span data-ttu-id="f1e58-531">向用户显示的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="f1e58-531">The email address that is displayed to users.</span></span>|
|<span data-ttu-id="f1e58-532">defenderSecurityCenterHelpPhone</span><span class="sxs-lookup"><span data-stu-id="f1e58-532">defenderSecurityCenterHelpPhone</span></span>|<span data-ttu-id="f1e58-533">字符串</span><span class="sxs-lookup"><span data-stu-id="f1e58-533">String</span></span>|<span data-ttu-id="f1e58-534">向用户显示的电话号码或 Skype ID。</span><span class="sxs-lookup"><span data-stu-id="f1e58-534">The phone number or Skype ID that is displayed to users.</span></span>|
|<span data-ttu-id="f1e58-535">defenderSecurityCenterHelpURL</span><span class="sxs-lookup"><span data-stu-id="f1e58-535">defenderSecurityCenterHelpURL</span></span>|<span data-ttu-id="f1e58-536">字符串</span><span class="sxs-lookup"><span data-stu-id="f1e58-536">String</span></span>|<span data-ttu-id="f1e58-537">"帮助" 门户 URL 将向用户显示。</span><span class="sxs-lookup"><span data-stu-id="f1e58-537">The help portal URL this is displayed to users.</span></span>|
|<span data-ttu-id="f1e58-538">defenderSecurityCenterNotificationsFromApp</span><span class="sxs-lookup"><span data-stu-id="f1e58-538">defenderSecurityCenterNotificationsFromApp</span></span>|[<span data-ttu-id="f1e58-539">defenderSecurityCenterNotificationsFromAppType</span><span class="sxs-lookup"><span data-stu-id="f1e58-539">defenderSecurityCenterNotificationsFromAppType</span></span>](../resources/intune-deviceconfig-defendersecuritycenternotificationsfromapptype.md)|<span data-ttu-id="f1e58-540">要从应用程序的显示区域中显示的通知。</span><span class="sxs-lookup"><span data-stu-id="f1e58-540">Notifications to show from the displayed areas of app.</span></span> <span data-ttu-id="f1e58-541">可取值为：`notConfigured`、`blockNoncriticalNotifications`、`blockAllNotifications`。</span><span class="sxs-lookup"><span data-stu-id="f1e58-541">Possible values are: `notConfigured`, `blockNoncriticalNotifications`, `blockAllNotifications`.</span></span>|
|<span data-ttu-id="f1e58-542">defenderSecurityCenterITContactDisplay</span><span class="sxs-lookup"><span data-stu-id="f1e58-542">defenderSecurityCenterITContactDisplay</span></span>|[<span data-ttu-id="f1e58-543">defenderSecurityCenterITContactDisplayType</span><span class="sxs-lookup"><span data-stu-id="f1e58-543">defenderSecurityCenterITContactDisplayType</span></span>](../resources/intune-deviceconfig-defendersecuritycenteritcontactdisplaytype.md)|<span data-ttu-id="f1e58-544">配置向最终用户显示 IT 联系人信息的位置。</span><span class="sxs-lookup"><span data-stu-id="f1e58-544">Configure where to display IT contact information to end users.</span></span> <span data-ttu-id="f1e58-545">可取值为：`notConfigured`、`displayInAppAndInNotifications`、`displayOnlyInApp`、`displayOnlyInNotifications`。</span><span class="sxs-lookup"><span data-stu-id="f1e58-545">Possible values are: `notConfigured`, `displayInAppAndInNotifications`, `displayOnlyInApp`, `displayOnlyInNotifications`.</span></span>|
|<span data-ttu-id="f1e58-546">firewallBlockStatefulFTP</span><span class="sxs-lookup"><span data-stu-id="f1e58-546">firewallBlockStatefulFTP</span></span>|<span data-ttu-id="f1e58-547">布尔</span><span class="sxs-lookup"><span data-stu-id="f1e58-547">Boolean</span></span>|<span data-ttu-id="f1e58-548">阻止到设备的有状态 FTP 连接</span><span class="sxs-lookup"><span data-stu-id="f1e58-548">Blocks stateful FTP connections to the device</span></span>|
|<span data-ttu-id="f1e58-549">firewallIdleTimeoutForSecurityAssociationInSeconds</span><span class="sxs-lookup"><span data-stu-id="f1e58-549">firewallIdleTimeoutForSecurityAssociationInSeconds</span></span>|<span data-ttu-id="f1e58-550">Int32</span><span class="sxs-lookup"><span data-stu-id="f1e58-550">Int32</span></span>|<span data-ttu-id="f1e58-551">配置安全关联的空闲超时（以秒为单位），值范围为 300 到 3600（包括这两个值）。</span><span class="sxs-lookup"><span data-stu-id="f1e58-551">Configures the idle timeout for security associations, in seconds, from 300 to 3600 inclusive.</span></span> <span data-ttu-id="f1e58-552">这是一个时间段，在此之后安全关联将过期并被删除。</span><span class="sxs-lookup"><span data-stu-id="f1e58-552">This is the period after which security associations will expire and be deleted.</span></span> <span data-ttu-id="f1e58-553">有效值为 300 至 3600</span><span class="sxs-lookup"><span data-stu-id="f1e58-553">Valid values 300 to 3600</span></span>|
|<span data-ttu-id="f1e58-554">firewallPreSharedKeyEncodingMethod</span><span class="sxs-lookup"><span data-stu-id="f1e58-554">firewallPreSharedKeyEncodingMethod</span></span>|[<span data-ttu-id="f1e58-555">firewallPreSharedKeyEncodingMethodType</span><span class="sxs-lookup"><span data-stu-id="f1e58-555">firewallPreSharedKeyEncodingMethodType</span></span>](../resources/intune-deviceconfig-firewallpresharedkeyencodingmethodtype.md)|<span data-ttu-id="f1e58-556">选择要使用的预共享密钥编码。</span><span class="sxs-lookup"><span data-stu-id="f1e58-556">Select the preshared key encoding to be used.</span></span> <span data-ttu-id="f1e58-557">可取值为：`deviceDefault`、`none`、`utF8`。</span><span class="sxs-lookup"><span data-stu-id="f1e58-557">Possible values are: `deviceDefault`, `none`, `utF8`.</span></span>|
|<span data-ttu-id="f1e58-558">firewallIPSecExemptionsAllowNeighborDiscovery</span><span class="sxs-lookup"><span data-stu-id="f1e58-558">firewallIPSecExemptionsAllowNeighborDiscovery</span></span>|<span data-ttu-id="f1e58-559">布尔</span><span class="sxs-lookup"><span data-stu-id="f1e58-559">Boolean</span></span>|<span data-ttu-id="f1e58-560">配置 IPSec 免除项以允许邻居发现 IPv6 ICMP 类型代码</span><span class="sxs-lookup"><span data-stu-id="f1e58-560">Configures IPSec exemptions to allow neighbor discovery IPv6 ICMP type-codes</span></span>|
|<span data-ttu-id="f1e58-561">firewallIPSecExemptionsAllowICMP</span><span class="sxs-lookup"><span data-stu-id="f1e58-561">firewallIPSecExemptionsAllowICMP</span></span>|<span data-ttu-id="f1e58-562">布尔</span><span class="sxs-lookup"><span data-stu-id="f1e58-562">Boolean</span></span>|<span data-ttu-id="f1e58-563">配置 IPSec 免除项以允许 ICMP</span><span class="sxs-lookup"><span data-stu-id="f1e58-563">Configures IPSec exemptions to allow ICMP</span></span>|
|<span data-ttu-id="f1e58-564">firewallIPSecExemptionsAllowRouterDiscovery</span><span class="sxs-lookup"><span data-stu-id="f1e58-564">firewallIPSecExemptionsAllowRouterDiscovery</span></span>|<span data-ttu-id="f1e58-565">布尔</span><span class="sxs-lookup"><span data-stu-id="f1e58-565">Boolean</span></span>|<span data-ttu-id="f1e58-566">配置 IPSec 免除项以允许路由器发现 IPv6 ICMP 类型代码</span><span class="sxs-lookup"><span data-stu-id="f1e58-566">Configures IPSec exemptions to allow router discovery IPv6 ICMP type-codes</span></span>|
|<span data-ttu-id="f1e58-567">firewallIPSecExemptionsAllowDHCP</span><span class="sxs-lookup"><span data-stu-id="f1e58-567">firewallIPSecExemptionsAllowDHCP</span></span>|<span data-ttu-id="f1e58-568">布尔</span><span class="sxs-lookup"><span data-stu-id="f1e58-568">Boolean</span></span>|<span data-ttu-id="f1e58-569">配置 IPSec 免除项以允许 IPv4 和 IPv6 DHCP 通信</span><span class="sxs-lookup"><span data-stu-id="f1e58-569">Configures IPSec exemptions to allow both IPv4 and IPv6 DHCP traffic</span></span>|
|<span data-ttu-id="f1e58-570">firewallCertificateRevocationListCheckMethod</span><span class="sxs-lookup"><span data-stu-id="f1e58-570">firewallCertificateRevocationListCheckMethod</span></span>|[<span data-ttu-id="f1e58-571">firewallCertificateRevocationListCheckMethodType</span><span class="sxs-lookup"><span data-stu-id="f1e58-571">firewallCertificateRevocationListCheckMethodType</span></span>](../resources/intune-deviceconfig-firewallcertificaterevocationlistcheckmethodtype.md)|<span data-ttu-id="f1e58-572">指定如何强制执行证书吊销列表。</span><span class="sxs-lookup"><span data-stu-id="f1e58-572">Specify how the certificate revocation list is to be enforced.</span></span> <span data-ttu-id="f1e58-573">可取值为：`deviceDefault`、`none`、`attempt`、`require`。</span><span class="sxs-lookup"><span data-stu-id="f1e58-573">Possible values are: `deviceDefault`, `none`, `attempt`, `require`.</span></span>|
|<span data-ttu-id="f1e58-574">firewallMergeKeyingModuleSettings</span><span class="sxs-lookup"><span data-stu-id="f1e58-574">firewallMergeKeyingModuleSettings</span></span>|<span data-ttu-id="f1e58-575">Boolean</span><span class="sxs-lookup"><span data-stu-id="f1e58-575">Boolean</span></span>|<span data-ttu-id="f1e58-576">如果键控模块不完全支持身份验证集，请指示模块仅忽略不受支持的身份验证套件而不是整个集</span><span class="sxs-lookup"><span data-stu-id="f1e58-576">If an authentication set is not fully supported by a keying module, direct the module to ignore only unsupported authentication suites rather than the entire set</span></span>|
|<span data-ttu-id="f1e58-577">firewallPacketQueueingMethod</span><span class="sxs-lookup"><span data-stu-id="f1e58-577">firewallPacketQueueingMethod</span></span>|[<span data-ttu-id="f1e58-578">firewallPacketQueueingMethodType</span><span class="sxs-lookup"><span data-stu-id="f1e58-578">firewallPacketQueueingMethodType</span></span>](../resources/intune-deviceconfig-firewallpacketqueueingmethodtype.md)|<span data-ttu-id="f1e58-579">配置如何在隧道网关应用场景中应用数据包排队。</span><span class="sxs-lookup"><span data-stu-id="f1e58-579">Configures how packet queueing should be applied in the tunnel gateway scenario.</span></span> <span data-ttu-id="f1e58-580">可取值为：`deviceDefault`、`disabled`、`queueInbound`、`queueOutbound` 或 `queueBoth`。</span><span class="sxs-lookup"><span data-stu-id="f1e58-580">Possible values are: `deviceDefault`, `disabled`, `queueInbound`, `queueOutbound`, `queueBoth`.</span></span>|
|<span data-ttu-id="f1e58-581">firewallProfileDomain</span><span class="sxs-lookup"><span data-stu-id="f1e58-581">firewallProfileDomain</span></span>|[<span data-ttu-id="f1e58-582">windowsFirewallNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="f1e58-582">windowsFirewallNetworkProfile</span></span>](../resources/intune-deviceconfig-windowsfirewallnetworkprofile.md)|<span data-ttu-id="f1e58-583">配置域网络的防火墙配置文件设置</span><span class="sxs-lookup"><span data-stu-id="f1e58-583">Configures the firewall profile settings for domain networks</span></span>|
|<span data-ttu-id="f1e58-584">firewallProfilePublic</span><span class="sxs-lookup"><span data-stu-id="f1e58-584">firewallProfilePublic</span></span>|[<span data-ttu-id="f1e58-585">windowsFirewallNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="f1e58-585">windowsFirewallNetworkProfile</span></span>](../resources/intune-deviceconfig-windowsfirewallnetworkprofile.md)|<span data-ttu-id="f1e58-586">配置公用网络的防火墙配置文件设置</span><span class="sxs-lookup"><span data-stu-id="f1e58-586">Configures the firewall profile settings for public networks</span></span>|
|<span data-ttu-id="f1e58-587">firewallProfilePrivate</span><span class="sxs-lookup"><span data-stu-id="f1e58-587">firewallProfilePrivate</span></span>|[<span data-ttu-id="f1e58-588">windowsFirewallNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="f1e58-588">windowsFirewallNetworkProfile</span></span>](../resources/intune-deviceconfig-windowsfirewallnetworkprofile.md)|<span data-ttu-id="f1e58-589">配置专用网络的防火墙配置文件设置</span><span class="sxs-lookup"><span data-stu-id="f1e58-589">Configures the firewall profile settings for private networks</span></span>|
|<span data-ttu-id="f1e58-590">defenderAdobeReaderLaunchChildProcess</span><span class="sxs-lookup"><span data-stu-id="f1e58-590">defenderAdobeReaderLaunchChildProcess</span></span>|[<span data-ttu-id="f1e58-591">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="f1e58-591">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="f1e58-592">值, 该值指示 Adobe Reader 创建子进程的行为。</span><span class="sxs-lookup"><span data-stu-id="f1e58-592">Value indicating the behavior of Adobe Reader from creating child processes.</span></span> <span data-ttu-id="f1e58-593">可取值为：`userDefined`、`enable`、`auditMode`。</span><span class="sxs-lookup"><span data-stu-id="f1e58-593">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="f1e58-594">defenderAttackSurfaceReductionExcludedPaths</span><span class="sxs-lookup"><span data-stu-id="f1e58-594">defenderAttackSurfaceReductionExcludedPaths</span></span>|<span data-ttu-id="f1e58-595">String 集合</span><span class="sxs-lookup"><span data-stu-id="f1e58-595">String collection</span></span>|<span data-ttu-id="f1e58-596">要从攻击面减少规则中排除的 exe 文件和文件夹的列表</span><span class="sxs-lookup"><span data-stu-id="f1e58-596">List of exe files and folders to be excluded from attack surface reduction rules</span></span>|
|<span data-ttu-id="f1e58-597">defenderOfficeAppsOtherProcessInjectionType</span><span class="sxs-lookup"><span data-stu-id="f1e58-597">defenderOfficeAppsOtherProcessInjectionType</span></span>|[<span data-ttu-id="f1e58-598">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="f1e58-598">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="f1e58-599">值, 该值指示插入到其他进程中的 Office 应用程序的行为。</span><span class="sxs-lookup"><span data-stu-id="f1e58-599">Value indicating the behavior of Office applications injecting into other processes.</span></span> <span data-ttu-id="f1e58-600">可取值为：`userDefined`、`block`、`auditMode`。</span><span class="sxs-lookup"><span data-stu-id="f1e58-600">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="f1e58-601">defenderOfficeAppsOtherProcessInjection</span><span class="sxs-lookup"><span data-stu-id="f1e58-601">defenderOfficeAppsOtherProcessInjection</span></span>|[<span data-ttu-id="f1e58-602">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="f1e58-602">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="f1e58-603">值, 该值指示插入到其他进程中的 Office 应用程序的行为。</span><span class="sxs-lookup"><span data-stu-id="f1e58-603">Value indicating the behavior of  Office applications injecting into other processes.</span></span> <span data-ttu-id="f1e58-604">可取值为：`userDefined`、`enable`、`auditMode`。</span><span class="sxs-lookup"><span data-stu-id="f1e58-604">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="f1e58-605">defenderOfficeCommunicationAppsLaunchChildProcess</span><span class="sxs-lookup"><span data-stu-id="f1e58-605">defenderOfficeCommunicationAppsLaunchChildProcess</span></span>|[<span data-ttu-id="f1e58-606">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="f1e58-606">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="f1e58-607">值, 该值指示 Office 通信应用程序 (包括 Microsoft Outlook) 在创建子进程时的行为。</span><span class="sxs-lookup"><span data-stu-id="f1e58-607">Value indicating the behavior of Office communication applications, including Microsoft Outlook, from creating child processes.</span></span> <span data-ttu-id="f1e58-608">可取值为：`userDefined`、`enable`、`auditMode`。</span><span class="sxs-lookup"><span data-stu-id="f1e58-608">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="f1e58-609">defenderOfficeAppsExecutableContentCreationOrLaunchType</span><span class="sxs-lookup"><span data-stu-id="f1e58-609">defenderOfficeAppsExecutableContentCreationOrLaunchType</span></span>|[<span data-ttu-id="f1e58-610">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="f1e58-610">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="f1e58-611">值, 该值指示 Office 应用程序/宏创建或启动可执行内容的行为。</span><span class="sxs-lookup"><span data-stu-id="f1e58-611">Value indicating the behavior of Office applications/macros creating or launching executable content.</span></span> <span data-ttu-id="f1e58-612">可取值为：`userDefined`、`block`、`auditMode`。</span><span class="sxs-lookup"><span data-stu-id="f1e58-612">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="f1e58-613">defenderOfficeAppsExecutableContentCreationOrLaunch</span><span class="sxs-lookup"><span data-stu-id="f1e58-613">defenderOfficeAppsExecutableContentCreationOrLaunch</span></span>|[<span data-ttu-id="f1e58-614">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="f1e58-614">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="f1e58-615">值, 该值指示 Office 应用程序/宏创建或启动可执行内容的行为。</span><span class="sxs-lookup"><span data-stu-id="f1e58-615">Value indicating the behavior of Office applications/macros creating or launching executable content.</span></span> <span data-ttu-id="f1e58-616">可取值为：`userDefined`、`enable`、`auditMode`。</span><span class="sxs-lookup"><span data-stu-id="f1e58-616">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="f1e58-617">defenderOfficeAppsLaunchChildProcessType</span><span class="sxs-lookup"><span data-stu-id="f1e58-617">defenderOfficeAppsLaunchChildProcessType</span></span>|[<span data-ttu-id="f1e58-618">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="f1e58-618">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="f1e58-619">值, 该值指示 Office 应用程序启动子进程的行为。</span><span class="sxs-lookup"><span data-stu-id="f1e58-619">Value indicating the behavior of Office application launching child processes.</span></span> <span data-ttu-id="f1e58-620">可取值为：`userDefined`、`block`、`auditMode`。</span><span class="sxs-lookup"><span data-stu-id="f1e58-620">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="f1e58-621">defenderOfficeAppsLaunchChildProcess</span><span class="sxs-lookup"><span data-stu-id="f1e58-621">defenderOfficeAppsLaunchChildProcess</span></span>|[<span data-ttu-id="f1e58-622">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="f1e58-622">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="f1e58-623">值, 该值指示 Office 应用程序启动子进程的行为。</span><span class="sxs-lookup"><span data-stu-id="f1e58-623">Value indicating the behavior of Office application launching child processes.</span></span> <span data-ttu-id="f1e58-624">可取值为：`userDefined`、`enable`、`auditMode`。</span><span class="sxs-lookup"><span data-stu-id="f1e58-624">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="f1e58-625">defenderOfficeMacroCodeAllowWin32ImportsType</span><span class="sxs-lookup"><span data-stu-id="f1e58-625">defenderOfficeMacroCodeAllowWin32ImportsType</span></span>|[<span data-ttu-id="f1e58-626">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="f1e58-626">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="f1e58-627">值, 该值指示从 Office 中的宏代码的 Win32 导入行为。</span><span class="sxs-lookup"><span data-stu-id="f1e58-627">Value indicating the behavior of Win32 imports from Macro code in Office.</span></span> <span data-ttu-id="f1e58-628">可取值为：`userDefined`、`block`、`auditMode`。</span><span class="sxs-lookup"><span data-stu-id="f1e58-628">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="f1e58-629">defenderOfficeMacroCodeAllowWin32Imports</span><span class="sxs-lookup"><span data-stu-id="f1e58-629">defenderOfficeMacroCodeAllowWin32Imports</span></span>|[<span data-ttu-id="f1e58-630">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="f1e58-630">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="f1e58-631">值, 该值指示从 Office 中的宏代码的 Win32 导入行为。</span><span class="sxs-lookup"><span data-stu-id="f1e58-631">Value indicating the behavior of Win32 imports from Macro code in Office.</span></span> <span data-ttu-id="f1e58-632">可取值为：`userDefined`、`enable`、`auditMode`。</span><span class="sxs-lookup"><span data-stu-id="f1e58-632">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="f1e58-633">defenderScriptObfuscatedMacroCodeType</span><span class="sxs-lookup"><span data-stu-id="f1e58-633">defenderScriptObfuscatedMacroCodeType</span></span>|[<span data-ttu-id="f1e58-634">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="f1e58-634">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="f1e58-635">值, 该值指示模糊的 js/vbs/ps/宏代码的行为。</span><span class="sxs-lookup"><span data-stu-id="f1e58-635">Value indicating the behavior of obfuscated js/vbs/ps/macro code.</span></span> <span data-ttu-id="f1e58-636">可取值为：`userDefined`、`block`、`auditMode`。</span><span class="sxs-lookup"><span data-stu-id="f1e58-636">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="f1e58-637">defenderScriptObfuscatedMacroCode</span><span class="sxs-lookup"><span data-stu-id="f1e58-637">defenderScriptObfuscatedMacroCode</span></span>|[<span data-ttu-id="f1e58-638">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="f1e58-638">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="f1e58-639">值, 该值指示模糊的 js/vbs/ps/宏代码的行为。</span><span class="sxs-lookup"><span data-stu-id="f1e58-639">Value indicating the behavior of obfuscated js/vbs/ps/macro code.</span></span> <span data-ttu-id="f1e58-640">可取值为：`userDefined`、`enable`、`auditMode`。</span><span class="sxs-lookup"><span data-stu-id="f1e58-640">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="f1e58-641">defenderScriptDownloadedPayloadExecutionType</span><span class="sxs-lookup"><span data-stu-id="f1e58-641">defenderScriptDownloadedPayloadExecutionType</span></span>|[<span data-ttu-id="f1e58-642">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="f1e58-642">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="f1e58-643">值, 该值指示从 Internet 下载的 js/vbs 执行负载的行为。</span><span class="sxs-lookup"><span data-stu-id="f1e58-643">Value indicating the behavior of js/vbs executing payload downloaded from Internet.</span></span> <span data-ttu-id="f1e58-644">可取值为：`userDefined`、`block`、`auditMode`。</span><span class="sxs-lookup"><span data-stu-id="f1e58-644">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="f1e58-645">defenderScriptDownloadedPayloadExecution</span><span class="sxs-lookup"><span data-stu-id="f1e58-645">defenderScriptDownloadedPayloadExecution</span></span>|[<span data-ttu-id="f1e58-646">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="f1e58-646">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="f1e58-647">值, 该值指示从 Internet 下载的 js/vbs 执行负载的行为。</span><span class="sxs-lookup"><span data-stu-id="f1e58-647">Value indicating the behavior of js/vbs executing payload downloaded from Internet.</span></span> <span data-ttu-id="f1e58-648">可取值为：`userDefined`、`enable`、`auditMode`。</span><span class="sxs-lookup"><span data-stu-id="f1e58-648">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="f1e58-649">defenderPreventCredentialStealingType</span><span class="sxs-lookup"><span data-stu-id="f1e58-649">defenderPreventCredentialStealingType</span></span>|[<span data-ttu-id="f1e58-650">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="f1e58-650">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="f1e58-651">值, 该值指示是否允许从 Windows 本地安全机构子系统中盗取凭据。</span><span class="sxs-lookup"><span data-stu-id="f1e58-651">Value indicating if credential stealing from the Windows local security authority subsystem is permitted.</span></span> <span data-ttu-id="f1e58-652">可取值为：`userDefined`、`enable`、`auditMode`。</span><span class="sxs-lookup"><span data-stu-id="f1e58-652">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="f1e58-653">defenderProcessCreationType</span><span class="sxs-lookup"><span data-stu-id="f1e58-653">defenderProcessCreationType</span></span>|[<span data-ttu-id="f1e58-654">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="f1e58-654">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="f1e58-655">一个值, 该值指示对源自 PSExec 和 WMI 命令的进程创建的响应。</span><span class="sxs-lookup"><span data-stu-id="f1e58-655">Value indicating response to process creations originating from PSExec and WMI commands.</span></span> <span data-ttu-id="f1e58-656">可取值为：`userDefined`、`block`、`auditMode`。</span><span class="sxs-lookup"><span data-stu-id="f1e58-656">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="f1e58-657">defenderProcessCreation</span><span class="sxs-lookup"><span data-stu-id="f1e58-657">defenderProcessCreation</span></span>|[<span data-ttu-id="f1e58-658">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="f1e58-658">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="f1e58-659">一个值, 该值指示对源自 PSExec 和 WMI 命令的进程创建的响应。</span><span class="sxs-lookup"><span data-stu-id="f1e58-659">Value indicating response to process creations originating from PSExec and WMI commands.</span></span> <span data-ttu-id="f1e58-660">可取值为：`userDefined`、`enable`、`auditMode`。</span><span class="sxs-lookup"><span data-stu-id="f1e58-660">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="f1e58-661">defenderUntrustedUSBProcessType</span><span class="sxs-lookup"><span data-stu-id="f1e58-661">defenderUntrustedUSBProcessType</span></span>|[<span data-ttu-id="f1e58-662">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="f1e58-662">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="f1e58-663">指示对从 USB 运行的不受信任和未签名进程的响应的值。</span><span class="sxs-lookup"><span data-stu-id="f1e58-663">Value indicating response to untrusted and unsigned processes that run from USB.</span></span> <span data-ttu-id="f1e58-664">可取值为：`userDefined`、`block`、`auditMode`。</span><span class="sxs-lookup"><span data-stu-id="f1e58-664">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="f1e58-665">defenderUntrustedUSBProcess</span><span class="sxs-lookup"><span data-stu-id="f1e58-665">defenderUntrustedUSBProcess</span></span>|[<span data-ttu-id="f1e58-666">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="f1e58-666">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="f1e58-667">指示对从 USB 运行的不受信任和未签名进程的响应的值。</span><span class="sxs-lookup"><span data-stu-id="f1e58-667">Value indicating response to untrusted and unsigned processes that run from USB.</span></span> <span data-ttu-id="f1e58-668">可取值为：`userDefined`、`enable`、`auditMode`。</span><span class="sxs-lookup"><span data-stu-id="f1e58-668">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="f1e58-669">defenderUntrustedExecutableType</span><span class="sxs-lookup"><span data-stu-id="f1e58-669">defenderUntrustedExecutableType</span></span>|[<span data-ttu-id="f1e58-670">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="f1e58-670">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="f1e58-671">指示对不符合流行、年龄或受信任列表条件的可执行文件的响应的值。</span><span class="sxs-lookup"><span data-stu-id="f1e58-671">Value indicating response to executables that don't meet a prevalence, age, or trusted list criteria.</span></span> <span data-ttu-id="f1e58-672">可取值为：`userDefined`、`block`、`auditMode`。</span><span class="sxs-lookup"><span data-stu-id="f1e58-672">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="f1e58-673">defenderUntrustedExecutable</span><span class="sxs-lookup"><span data-stu-id="f1e58-673">defenderUntrustedExecutable</span></span>|[<span data-ttu-id="f1e58-674">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="f1e58-674">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="f1e58-675">指示对不符合流行、年龄或受信任列表条件的可执行文件的响应的值。</span><span class="sxs-lookup"><span data-stu-id="f1e58-675">Value indicating response to executables that don't meet a prevalence, age, or trusted list criteria.</span></span> <span data-ttu-id="f1e58-676">可取值为：`userDefined`、`enable`、`auditMode`。</span><span class="sxs-lookup"><span data-stu-id="f1e58-676">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="f1e58-677">defenderEmailContentExecutionType</span><span class="sxs-lookup"><span data-stu-id="f1e58-677">defenderEmailContentExecutionType</span></span>|[<span data-ttu-id="f1e58-678">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="f1e58-678">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="f1e58-679">一个值, 该值指示是否应从电子邮件 (web 邮件/邮件客户端) 中删除可执行内容 (exe、dll、ps、js、vbs 等) 的执行。</span><span class="sxs-lookup"><span data-stu-id="f1e58-679">Value indicating if execution of executable content (exe, dll, ps, js, vbs, etc) should be dropped from email (webmail/mail-client).</span></span> <span data-ttu-id="f1e58-680">可取值为：`userDefined`、`block`、`auditMode`。</span><span class="sxs-lookup"><span data-stu-id="f1e58-680">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="f1e58-681">defenderEmailContentExecution</span><span class="sxs-lookup"><span data-stu-id="f1e58-681">defenderEmailContentExecution</span></span>|[<span data-ttu-id="f1e58-682">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="f1e58-682">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="f1e58-683">一个值, 该值指示是否应从电子邮件 (web 邮件/邮件客户端) 中删除可执行内容 (exe、dll、ps、js、vbs 等) 的执行。</span><span class="sxs-lookup"><span data-stu-id="f1e58-683">Value indicating if execution of executable content (exe, dll, ps, js, vbs, etc) should be dropped from email (webmail/mail-client).</span></span> <span data-ttu-id="f1e58-684">可取值为：`userDefined`、`enable`、`auditMode`。</span><span class="sxs-lookup"><span data-stu-id="f1e58-684">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="f1e58-685">defenderAdvancedRansomewareProtectionType</span><span class="sxs-lookup"><span data-stu-id="f1e58-685">defenderAdvancedRansomewareProtectionType</span></span>|[<span data-ttu-id="f1e58-686">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="f1e58-686">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="f1e58-687">指示使用针对 ransomeware 的高级防护的值。</span><span class="sxs-lookup"><span data-stu-id="f1e58-687">Value indicating use of advanced protection against ransomeware.</span></span> <span data-ttu-id="f1e58-688">可取值为：`userDefined`、`enable`、`auditMode`。</span><span class="sxs-lookup"><span data-stu-id="f1e58-688">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="f1e58-689">defenderGuardMyFoldersType</span><span class="sxs-lookup"><span data-stu-id="f1e58-689">defenderGuardMyFoldersType</span></span>|[<span data-ttu-id="f1e58-690">folderProtectionType</span><span class="sxs-lookup"><span data-stu-id="f1e58-690">folderProtectionType</span></span>](../resources/intune-deviceconfig-folderprotectiontype.md)|<span data-ttu-id="f1e58-691">值, 该值指示受保护文件夹的行为。</span><span class="sxs-lookup"><span data-stu-id="f1e58-691">Value indicating the behavior of protected folders.</span></span> <span data-ttu-id="f1e58-692">可取值为：`userDefined`、`enable`、`auditMode`、`blockDiskModification` 或 `auditDiskModification`。</span><span class="sxs-lookup"><span data-stu-id="f1e58-692">Possible values are: `userDefined`, `enable`, `auditMode`, `blockDiskModification`, `auditDiskModification`.</span></span>|
|<span data-ttu-id="f1e58-693">defenderGuardedFoldersAllowedAppPaths</span><span class="sxs-lookup"><span data-stu-id="f1e58-693">defenderGuardedFoldersAllowedAppPaths</span></span>|<span data-ttu-id="f1e58-694">String collection</span><span class="sxs-lookup"><span data-stu-id="f1e58-694">String collection</span></span>|<span data-ttu-id="f1e58-695">允许访问受保护文件夹的 exe 路径列表</span><span class="sxs-lookup"><span data-stu-id="f1e58-695">List of paths to exe that are allowed to access protected folders</span></span>|
|<span data-ttu-id="f1e58-696">defenderAdditionalGuardedFolders</span><span class="sxs-lookup"><span data-stu-id="f1e58-696">defenderAdditionalGuardedFolders</span></span>|<span data-ttu-id="f1e58-697">String 集合</span><span class="sxs-lookup"><span data-stu-id="f1e58-697">String collection</span></span>|<span data-ttu-id="f1e58-698">要添加到受保护文件夹列表的文件夹路径列表</span><span class="sxs-lookup"><span data-stu-id="f1e58-698">List of folder paths to be added to the list of protected folders</span></span>|
|<span data-ttu-id="f1e58-699">defenderNetworkProtectionType</span><span class="sxs-lookup"><span data-stu-id="f1e58-699">defenderNetworkProtectionType</span></span>|[<span data-ttu-id="f1e58-700">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="f1e58-700">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="f1e58-701">值, 该值指示 NetworkProtection 的行为。</span><span class="sxs-lookup"><span data-stu-id="f1e58-701">Value indicating the behavior of NetworkProtection.</span></span> <span data-ttu-id="f1e58-702">可取值为：`userDefined`、`enable`、`auditMode`。</span><span class="sxs-lookup"><span data-stu-id="f1e58-702">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="f1e58-703">defenderExploitProtectionXml</span><span class="sxs-lookup"><span data-stu-id="f1e58-703">defenderExploitProtectionXml</span></span>|<span data-ttu-id="f1e58-704">Binary</span><span class="sxs-lookup"><span data-stu-id="f1e58-704">Binary</span></span>|<span data-ttu-id="f1e58-705">包含有关 Exploit Protection 详细信息的 xml 内容。</span><span class="sxs-lookup"><span data-stu-id="f1e58-705">Xml content containing information regarding exploit protection details.</span></span>|
|<span data-ttu-id="f1e58-706">defenderExploitProtectionXmlFileName</span><span class="sxs-lookup"><span data-stu-id="f1e58-706">defenderExploitProtectionXmlFileName</span></span>|<span data-ttu-id="f1e58-707">String</span><span class="sxs-lookup"><span data-stu-id="f1e58-707">String</span></span>|<span data-ttu-id="f1e58-708">从中获取 DefenderExploitProtectionXml 的文件的名称。</span><span class="sxs-lookup"><span data-stu-id="f1e58-708">Name of the file from which DefenderExploitProtectionXml was obtained.</span></span>|
|<span data-ttu-id="f1e58-709">defenderSecurityCenterBlockExploitProtectionOverride</span><span class="sxs-lookup"><span data-stu-id="f1e58-709">defenderSecurityCenterBlockExploitProtectionOverride</span></span>|<span data-ttu-id="f1e58-710">Boolean</span><span class="sxs-lookup"><span data-stu-id="f1e58-710">Boolean</span></span>|<span data-ttu-id="f1e58-711">指示是否阻止用户覆盖 Exploit Protection 设置。</span><span class="sxs-lookup"><span data-stu-id="f1e58-711">Indicates whether or not to block user from overriding Exploit Protection settings.</span></span>|
|<span data-ttu-id="f1e58-712">appLockerApplicationControl</span><span class="sxs-lookup"><span data-stu-id="f1e58-712">appLockerApplicationControl</span></span>|[<span data-ttu-id="f1e58-713">appLockerApplicationControlType</span><span class="sxs-lookup"><span data-stu-id="f1e58-713">appLockerApplicationControlType</span></span>](../resources/intune-deviceconfig-applockerapplicationcontroltype.md)|<span data-ttu-id="f1e58-714">使管理员能够选择在设备上允许哪些类型的应用。</span><span class="sxs-lookup"><span data-stu-id="f1e58-714">Enables the Admin to choose what types of app to allow on devices.</span></span> <span data-ttu-id="f1e58-715">可取值为：`notConfigured`、`enforceComponentsAndStoreApps`、`auditComponentsAndStoreApps`、`enforceComponentsStoreAppsAndSmartlocker`、`auditComponentsStoreAppsAndSmartlocker`。</span><span class="sxs-lookup"><span data-stu-id="f1e58-715">Possible values are: `notConfigured`, `enforceComponentsAndStoreApps`, `auditComponentsAndStoreApps`, `enforceComponentsStoreAppsAndSmartlocker`, `auditComponentsStoreAppsAndSmartlocker`.</span></span>|
|<span data-ttu-id="f1e58-716">deviceGuardLocalSystemAuthorityCredentialGuardSettings</span><span class="sxs-lookup"><span data-stu-id="f1e58-716">deviceGuardLocalSystemAuthorityCredentialGuardSettings</span></span>|[<span data-ttu-id="f1e58-717">deviceGuardLocalSystemAuthorityCredentialGuardType</span><span class="sxs-lookup"><span data-stu-id="f1e58-717">deviceGuardLocalSystemAuthorityCredentialGuardType</span></span>](../resources/intune-deviceconfig-deviceguardlocalsystemauthoritycredentialguardtype.md)|<span data-ttu-id="f1e58-718">如果平台安全级别具有安全启动和基于虚拟化的安全性均已启用, 则打开 Credential Guard。</span><span class="sxs-lookup"><span data-stu-id="f1e58-718">Turn on Credential Guard when Platform Security Level with Secure Boot and Virtualization Based Security are both enabled.</span></span> <span data-ttu-id="f1e58-719">可取值为：`notConfigured`、`enableWithUEFILock`、`enableWithoutUEFILock`。</span><span class="sxs-lookup"><span data-stu-id="f1e58-719">Possible values are: `notConfigured`, `enableWithUEFILock`, `enableWithoutUEFILock`.</span></span>|
|<span data-ttu-id="f1e58-720">deviceGuardEnableVirtualizationBasedSecurity</span><span class="sxs-lookup"><span data-stu-id="f1e58-720">deviceGuardEnableVirtualizationBasedSecurity</span></span>|<span data-ttu-id="f1e58-721">布尔</span><span class="sxs-lookup"><span data-stu-id="f1e58-721">Boolean</span></span>|<span data-ttu-id="f1e58-722">启用基于虚拟化的安全性 (VBS)。</span><span class="sxs-lookup"><span data-stu-id="f1e58-722">Turns On Virtualization Based Security(VBS).</span></span>|
|<span data-ttu-id="f1e58-723">deviceGuardEnableSecureBootWithDMA</span><span class="sxs-lookup"><span data-stu-id="f1e58-723">deviceGuardEnableSecureBootWithDMA</span></span>|<span data-ttu-id="f1e58-724">布尔</span><span class="sxs-lookup"><span data-stu-id="f1e58-724">Boolean</span></span>|<span data-ttu-id="f1e58-725">指定是否在下次重新启动时启用平台安全级别。</span><span class="sxs-lookup"><span data-stu-id="f1e58-725">Specifies whether Platform Security Level is enabled at next reboot.</span></span>|
|<span data-ttu-id="f1e58-726">deviceGuardLaunchSystemGuard</span><span class="sxs-lookup"><span data-stu-id="f1e58-726">deviceGuardLaunchSystemGuard</span></span>|[<span data-ttu-id="f1e58-727">启用</span><span class="sxs-lookup"><span data-stu-id="f1e58-727">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="f1e58-728">允许 IT 管理员配置启动 "系统防护"。</span><span class="sxs-lookup"><span data-stu-id="f1e58-728">Allows the IT admin to configure the launch of System Guard.</span></span> <span data-ttu-id="f1e58-729">可取值为：`notConfigured`、`enabled`、`disabled`。</span><span class="sxs-lookup"><span data-stu-id="f1e58-729">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="f1e58-730">smartScreenEnableInShell</span><span class="sxs-lookup"><span data-stu-id="f1e58-730">smartScreenEnableInShell</span></span>|<span data-ttu-id="f1e58-731">布尔</span><span class="sxs-lookup"><span data-stu-id="f1e58-731">Boolean</span></span>|<span data-ttu-id="f1e58-732">允许 IT 管理员配置适用于 Windows 的 SmartScreen。</span><span class="sxs-lookup"><span data-stu-id="f1e58-732">Allows IT Admins to configure SmartScreen for Windows.</span></span>|
|<span data-ttu-id="f1e58-733">smartScreenBlockOverrideForFiles</span><span class="sxs-lookup"><span data-stu-id="f1e58-733">smartScreenBlockOverrideForFiles</span></span>|<span data-ttu-id="f1e58-734">布尔</span><span class="sxs-lookup"><span data-stu-id="f1e58-734">Boolean</span></span>|<span data-ttu-id="f1e58-735">允许 IT 管理员控制用户是否可以忽略 SmartScreen 警告并运行恶意文件。</span><span class="sxs-lookup"><span data-stu-id="f1e58-735">Allows IT Admins to control whether users can can ignore SmartScreen warnings and run malicious files.</span></span>|
|<span data-ttu-id="f1e58-736">applicationGuardEnabled</span><span class="sxs-lookup"><span data-stu-id="f1e58-736">applicationGuardEnabled</span></span>|<span data-ttu-id="f1e58-737">布尔</span><span class="sxs-lookup"><span data-stu-id="f1e58-737">Boolean</span></span>|<span data-ttu-id="f1e58-738">启用 Windows Defender 应用程序防护</span><span class="sxs-lookup"><span data-stu-id="f1e58-738">Enable Windows Defender Application Guard</span></span>|
|<span data-ttu-id="f1e58-739">applicationGuardEnabledOptions</span><span class="sxs-lookup"><span data-stu-id="f1e58-739">applicationGuardEnabledOptions</span></span>|[<span data-ttu-id="f1e58-740">applicationGuardEnabledOptions</span><span class="sxs-lookup"><span data-stu-id="f1e58-740">applicationGuardEnabledOptions</span></span>](../resources/intune-deviceconfig-applicationguardenabledoptions.md)|<span data-ttu-id="f1e58-741">为较新的 windows 版本启用 windows Defender 应用程序防护。</span><span class="sxs-lookup"><span data-stu-id="f1e58-741">Enable Windows Defender Application Guard for newer Windows builds.</span></span> <span data-ttu-id="f1e58-742">可取值为：`notConfigured`、`enabledForEdge`、`enabledForOffice`、`enabledForEdgeAndOffice`。</span><span class="sxs-lookup"><span data-stu-id="f1e58-742">Possible values are: `notConfigured`, `enabledForEdge`, `enabledForOffice`, `enabledForEdgeAndOffice`.</span></span>|
|<span data-ttu-id="f1e58-743">applicationGuardBlockFileTransfer</span><span class="sxs-lookup"><span data-stu-id="f1e58-743">applicationGuardBlockFileTransfer</span></span>|[<span data-ttu-id="f1e58-744">applicationGuardBlockFileTransferType</span><span class="sxs-lookup"><span data-stu-id="f1e58-744">applicationGuardBlockFileTransferType</span></span>](../resources/intune-deviceconfig-applicationguardblockfiletransfertype.md)|<span data-ttu-id="f1e58-745">阻止剪贴板传输图像文件、文本文件或二者都不。</span><span class="sxs-lookup"><span data-stu-id="f1e58-745">Block clipboard to transfer image file, text file or neither of them.</span></span> <span data-ttu-id="f1e58-746">可取值为：`notConfigured`、`blockImageAndTextFile`、`blockImageFile`、`blockNone` 或 `blockTextFile`。</span><span class="sxs-lookup"><span data-stu-id="f1e58-746">Possible values are: `notConfigured`, `blockImageAndTextFile`, `blockImageFile`, `blockNone`, `blockTextFile`.</span></span>|
|<span data-ttu-id="f1e58-747">applicationGuardBlockNonEnterpriseContent</span><span class="sxs-lookup"><span data-stu-id="f1e58-747">applicationGuardBlockNonEnterpriseContent</span></span>|<span data-ttu-id="f1e58-748">布尔</span><span class="sxs-lookup"><span data-stu-id="f1e58-748">Boolean</span></span>|<span data-ttu-id="f1e58-749">阻止企业站点加载非企业内容，例如第三方插件</span><span class="sxs-lookup"><span data-stu-id="f1e58-749">Block enterprise sites to load non-enterprise content, such as third party plug-ins</span></span>|
|<span data-ttu-id="f1e58-750">applicationGuardAllowPersistence</span><span class="sxs-lookup"><span data-stu-id="f1e58-750">applicationGuardAllowPersistence</span></span>|<span data-ttu-id="f1e58-751">布尔</span><span class="sxs-lookup"><span data-stu-id="f1e58-751">Boolean</span></span>|<span data-ttu-id="f1e58-752">允许 App Guard 容器（收藏夹、Cookie、Web 密码等）内的持久用户生成数据</span><span class="sxs-lookup"><span data-stu-id="f1e58-752">Allow persisting user generated data inside the App Guard Containter (favorites, cookies, web passwords, etc.)</span></span>|
|<span data-ttu-id="f1e58-753">applicationGuardForceAuditing</span><span class="sxs-lookup"><span data-stu-id="f1e58-753">applicationGuardForceAuditing</span></span>|<span data-ttu-id="f1e58-754">布尔</span><span class="sxs-lookup"><span data-stu-id="f1e58-754">Boolean</span></span>|<span data-ttu-id="f1e58-755">强制审核将存留 Windows 日志和事件以满足安全/符合性条件（示例事件是用户登录注销、特权使用、软件安装、系统更改等）</span><span class="sxs-lookup"><span data-stu-id="f1e58-755">Force auditing will persist Windows logs and events to meet security/compliance criteria (sample events are user login-logoff, use of privilege rights, software installation, system changes, etc.)</span></span>|
|<span data-ttu-id="f1e58-756">applicationGuardBlockClipboardSharing</span><span class="sxs-lookup"><span data-stu-id="f1e58-756">applicationGuardBlockClipboardSharing</span></span>|[<span data-ttu-id="f1e58-757">applicationGuardBlockClipboardSharingType</span><span class="sxs-lookup"><span data-stu-id="f1e58-757">applicationGuardBlockClipboardSharingType</span></span>](../resources/intune-deviceconfig-applicationguardblockclipboardsharingtype.md)|<span data-ttu-id="f1e58-758">阻止剪贴板将数据从主机共享到容器或从容器共享到主机，或阻止两种方式，或两种方式均不阻止。</span><span class="sxs-lookup"><span data-stu-id="f1e58-758">Block clipboard to share data from Host to Container, or from Container to Host, or both ways, or neither ways.</span></span> <span data-ttu-id="f1e58-759">可取值为：`notConfigured`、`blockBoth`、`blockHostToContainer`、`blockContainerToHost`、`blockNone`。</span><span class="sxs-lookup"><span data-stu-id="f1e58-759">Possible values are: `notConfigured`, `blockBoth`, `blockHostToContainer`, `blockContainerToHost`, `blockNone`.</span></span>|
|<span data-ttu-id="f1e58-760">applicationGuardAllowPrintToPDF</span><span class="sxs-lookup"><span data-stu-id="f1e58-760">applicationGuardAllowPrintToPDF</span></span>|<span data-ttu-id="f1e58-761">布尔</span><span class="sxs-lookup"><span data-stu-id="f1e58-761">Boolean</span></span>|<span data-ttu-id="f1e58-762">允许从容器打印为 PDF 格式</span><span class="sxs-lookup"><span data-stu-id="f1e58-762">Allow printing to PDF from Container</span></span>|
|<span data-ttu-id="f1e58-763">applicationGuardAllowPrintToXPS</span><span class="sxs-lookup"><span data-stu-id="f1e58-763">applicationGuardAllowPrintToXPS</span></span>|<span data-ttu-id="f1e58-764">布尔</span><span class="sxs-lookup"><span data-stu-id="f1e58-764">Boolean</span></span>|<span data-ttu-id="f1e58-765">允许从容器打印为 XPS 格式</span><span class="sxs-lookup"><span data-stu-id="f1e58-765">Allow printing to XPS from Container</span></span>|
|<span data-ttu-id="f1e58-766">applicationGuardAllowPrintToLocalPrinters</span><span class="sxs-lookup"><span data-stu-id="f1e58-766">applicationGuardAllowPrintToLocalPrinters</span></span>|<span data-ttu-id="f1e58-767">布尔</span><span class="sxs-lookup"><span data-stu-id="f1e58-767">Boolean</span></span>|<span data-ttu-id="f1e58-768">允许从容器打印到本地打印机</span><span class="sxs-lookup"><span data-stu-id="f1e58-768">Allow printing to Local Printers from Container</span></span>|
|<span data-ttu-id="f1e58-769">applicationGuardAllowPrintToNetworkPrinters</span><span class="sxs-lookup"><span data-stu-id="f1e58-769">applicationGuardAllowPrintToNetworkPrinters</span></span>|<span data-ttu-id="f1e58-770">布尔</span><span class="sxs-lookup"><span data-stu-id="f1e58-770">Boolean</span></span>|<span data-ttu-id="f1e58-771">允许从容器打印到网络打印机</span><span class="sxs-lookup"><span data-stu-id="f1e58-771">Allow printing to Network Printers from Container</span></span>|
|<span data-ttu-id="f1e58-772">applicationGuardAllowVirtualGPU</span><span class="sxs-lookup"><span data-stu-id="f1e58-772">applicationGuardAllowVirtualGPU</span></span>|<span data-ttu-id="f1e58-773">布尔</span><span class="sxs-lookup"><span data-stu-id="f1e58-773">Boolean</span></span>|<span data-ttu-id="f1e58-774">允许应用程序防护使用虚拟 GPU</span><span class="sxs-lookup"><span data-stu-id="f1e58-774">Allow application guard to use virtual GPU</span></span>|
|<span data-ttu-id="f1e58-775">applicationGuardAllowFileSaveOnHost</span><span class="sxs-lookup"><span data-stu-id="f1e58-775">applicationGuardAllowFileSaveOnHost</span></span>|<span data-ttu-id="f1e58-776">布尔</span><span class="sxs-lookup"><span data-stu-id="f1e58-776">Boolean</span></span>|<span data-ttu-id="f1e58-777">允许用户从应用程序防护容器中的边缘下载文件并将其保存在主机文件系统上</span><span class="sxs-lookup"><span data-stu-id="f1e58-777">Allow users to download files from Edge in the application guard container and save them on the host file system</span></span>|
|<span data-ttu-id="f1e58-778">bitLockerAllowStandardUserEncryption</span><span class="sxs-lookup"><span data-stu-id="f1e58-778">bitLockerAllowStandardUserEncryption</span></span>|<span data-ttu-id="f1e58-779">布尔</span><span class="sxs-lookup"><span data-stu-id="f1e58-779">Boolean</span></span>|<span data-ttu-id="f1e58-780">允许管理员允许标准用户在 Azure AD 加入过程中启用 encrpytion。</span><span class="sxs-lookup"><span data-stu-id="f1e58-780">Allows the admin to allow standard users to enable encrpytion during Azure AD Join.</span></span>|
|<span data-ttu-id="f1e58-781">bitLockerDisableWarningForOtherDiskEncryption</span><span class="sxs-lookup"><span data-stu-id="f1e58-781">bitLockerDisableWarningForOtherDiskEncryption</span></span>|<span data-ttu-id="f1e58-782">布尔</span><span class="sxs-lookup"><span data-stu-id="f1e58-782">Boolean</span></span>|<span data-ttu-id="f1e58-783">允许管理员禁用对用户计算机上其他磁盘加密的警告提示。</span><span class="sxs-lookup"><span data-stu-id="f1e58-783">Allows the Admin to disable the warning prompt for other disk encryption on the user machines.</span></span>|
|<span data-ttu-id="f1e58-784">bitLockerEnableStorageCardEncryptionOnMobile</span><span class="sxs-lookup"><span data-stu-id="f1e58-784">bitLockerEnableStorageCardEncryptionOnMobile</span></span>|<span data-ttu-id="f1e58-785">Boolean</span><span class="sxs-lookup"><span data-stu-id="f1e58-785">Boolean</span></span>|<span data-ttu-id="f1e58-786">允许管理员要求使用 BitLocker 开启加密功能。</span><span class="sxs-lookup"><span data-stu-id="f1e58-786">Allows the admin to require encryption to be turned on using BitLocker.</span></span> <span data-ttu-id="f1e58-787">此策略仅适用于移动 SKU。</span><span class="sxs-lookup"><span data-stu-id="f1e58-787">This policy is valid only for a mobile SKU.</span></span>|
|<span data-ttu-id="f1e58-788">bitLockerEncryptDevice</span><span class="sxs-lookup"><span data-stu-id="f1e58-788">bitLockerEncryptDevice</span></span>|<span data-ttu-id="f1e58-789">Boolean</span><span class="sxs-lookup"><span data-stu-id="f1e58-789">Boolean</span></span>|<span data-ttu-id="f1e58-790">允许管理员要求使用 BitLocker 开启加密功能。</span><span class="sxs-lookup"><span data-stu-id="f1e58-790">Allows the admin to require encryption to be turned on using BitLocker.</span></span>|
|<span data-ttu-id="f1e58-791">bitLockerSystemDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="f1e58-791">bitLockerSystemDrivePolicy</span></span>|[<span data-ttu-id="f1e58-792">bitLockerSystemDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="f1e58-792">bitLockerSystemDrivePolicy</span></span>](../resources/intune-deviceconfig-bitlockersystemdrivepolicy.md)|<span data-ttu-id="f1e58-793">BitLocker 系统驱动器策略。</span><span class="sxs-lookup"><span data-stu-id="f1e58-793">BitLocker System Drive Policy.</span></span>|
|<span data-ttu-id="f1e58-794">bitLockerFixedDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="f1e58-794">bitLockerFixedDrivePolicy</span></span>|[<span data-ttu-id="f1e58-795">bitLockerFixedDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="f1e58-795">bitLockerFixedDrivePolicy</span></span>](../resources/intune-deviceconfig-bitlockerfixeddrivepolicy.md)|<span data-ttu-id="f1e58-796">BitLocker 固定驱动器策略。</span><span class="sxs-lookup"><span data-stu-id="f1e58-796">BitLocker Fixed Drive Policy.</span></span>|
|<span data-ttu-id="f1e58-797">bitLockerRemovableDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="f1e58-797">bitLockerRemovableDrivePolicy</span></span>|[<span data-ttu-id="f1e58-798">bitLockerRemovableDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="f1e58-798">bitLockerRemovableDrivePolicy</span></span>](../resources/intune-deviceconfig-bitlockerremovabledrivepolicy.md)|<span data-ttu-id="f1e58-799">BitLocker 可移动驱动器策略。</span><span class="sxs-lookup"><span data-stu-id="f1e58-799">BitLocker Removable Drive Policy.</span></span>|



## <a name="response"></a><span data-ttu-id="f1e58-800">响应</span><span class="sxs-lookup"><span data-stu-id="f1e58-800">Response</span></span>
<span data-ttu-id="f1e58-801">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="f1e58-801">If successful, this method returns a `200 OK` response code and an updated [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f1e58-802">示例</span><span class="sxs-lookup"><span data-stu-id="f1e58-802">Example</span></span>

### <a name="request"></a><span data-ttu-id="f1e58-803">请求</span><span class="sxs-lookup"><span data-stu-id="f1e58-803">Request</span></span>
<span data-ttu-id="f1e58-804">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="f1e58-804">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
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

### <a name="response"></a><span data-ttu-id="f1e58-805">响应</span><span class="sxs-lookup"><span data-stu-id="f1e58-805">Response</span></span>
<span data-ttu-id="f1e58-p199">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="f1e58-p199">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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





