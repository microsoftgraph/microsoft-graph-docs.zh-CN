---
title: 创建 windows10EndpointProtectionConfiguration
description: 创建新的 windows10EndpointProtectionConfiguration 对象。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 9bdc31fed7797a448239bc7ed19ac57750692646
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29402585"
---
# <a name="create-windows10endpointprotectionconfiguration"></a><span data-ttu-id="6b27b-103">创建 windows10EndpointProtectionConfiguration</span><span class="sxs-lookup"><span data-stu-id="6b27b-103">Create windows10EndpointProtectionConfiguration</span></span>

> <span data-ttu-id="6b27b-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="6b27b-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="6b27b-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="6b27b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="6b27b-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="6b27b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6b27b-107">创建新的 [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="6b27b-107">Create a new [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6b27b-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="6b27b-108">Prerequisites</span></span>
<span data-ttu-id="6b27b-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="6b27b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="6b27b-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="6b27b-111">Permission type</span></span>|<span data-ttu-id="6b27b-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="6b27b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6b27b-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6b27b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6b27b-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6b27b-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="6b27b-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6b27b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6b27b-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="6b27b-116">Not supported.</span></span>|
|<span data-ttu-id="6b27b-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="6b27b-117">Application</span></span>|<span data-ttu-id="6b27b-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="6b27b-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6b27b-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6b27b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="6b27b-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="6b27b-120">Request headers</span></span>
|<span data-ttu-id="6b27b-121">标头</span><span class="sxs-lookup"><span data-stu-id="6b27b-121">Header</span></span>|<span data-ttu-id="6b27b-122">值</span><span class="sxs-lookup"><span data-stu-id="6b27b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6b27b-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="6b27b-123">Authorization</span></span>|<span data-ttu-id="6b27b-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="6b27b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6b27b-125">Accept</span><span class="sxs-lookup"><span data-stu-id="6b27b-125">Accept</span></span>|<span data-ttu-id="6b27b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6b27b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6b27b-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="6b27b-127">Request body</span></span>
<span data-ttu-id="6b27b-128">在请求正文中，提供 windows10EndpointProtectionConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6b27b-128">In the request body, supply a JSON representation for the windows10EndpointProtectionConfiguration object.</span></span>

<span data-ttu-id="6b27b-129">下表显示了创建 windows10EndpointProtectionConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="6b27b-129">The following table shows the properties that are required when you create the windows10EndpointProtectionConfiguration.</span></span>

|<span data-ttu-id="6b27b-130">属性</span><span class="sxs-lookup"><span data-stu-id="6b27b-130">Property</span></span>|<span data-ttu-id="6b27b-131">类型</span><span class="sxs-lookup"><span data-stu-id="6b27b-131">Type</span></span>|<span data-ttu-id="6b27b-132">说明</span><span class="sxs-lookup"><span data-stu-id="6b27b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6b27b-133">id</span><span class="sxs-lookup"><span data-stu-id="6b27b-133">id</span></span>|<span data-ttu-id="6b27b-134">String</span><span class="sxs-lookup"><span data-stu-id="6b27b-134">String</span></span>|<span data-ttu-id="6b27b-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="6b27b-135">Key of the entity.</span></span> <span data-ttu-id="6b27b-136">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6b27b-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6b27b-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6b27b-137">lastModifiedDateTime</span></span>|<span data-ttu-id="6b27b-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6b27b-138">DateTimeOffset</span></span>|<span data-ttu-id="6b27b-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="6b27b-139">DateTime the object was last modified.</span></span> <span data-ttu-id="6b27b-140">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6b27b-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6b27b-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="6b27b-141">roleScopeTagIds</span></span>|<span data-ttu-id="6b27b-142">String 集合</span><span class="sxs-lookup"><span data-stu-id="6b27b-142">String collection</span></span>|<span data-ttu-id="6b27b-143">此实体实例范围标记的列表。</span><span class="sxs-lookup"><span data-stu-id="6b27b-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="6b27b-144">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6b27b-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6b27b-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="6b27b-145">supportsScopeTags</span></span>|<span data-ttu-id="6b27b-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="6b27b-146">Boolean</span></span>|<span data-ttu-id="6b27b-147">指示基础的设备配置支持分配的范围标记。</span><span class="sxs-lookup"><span data-stu-id="6b27b-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="6b27b-148">此值为 false，并且实体将不会对作用域的用户可见时，不允许将分配给 ScopeTags 属性。</span><span class="sxs-lookup"><span data-stu-id="6b27b-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="6b27b-149">这将发生在 Silverlight 中创建的旧策略，并可以解析通过删除并重新创建 Azure 门户中的策略。</span><span class="sxs-lookup"><span data-stu-id="6b27b-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="6b27b-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="6b27b-150">This property is read-only.</span></span> <span data-ttu-id="6b27b-151">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6b27b-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6b27b-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6b27b-152">createdDateTime</span></span>|<span data-ttu-id="6b27b-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6b27b-153">DateTimeOffset</span></span>|<span data-ttu-id="6b27b-154">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="6b27b-154">DateTime the object was created.</span></span> <span data-ttu-id="6b27b-155">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6b27b-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6b27b-156">description</span><span class="sxs-lookup"><span data-stu-id="6b27b-156">description</span></span>|<span data-ttu-id="6b27b-157">String</span><span class="sxs-lookup"><span data-stu-id="6b27b-157">String</span></span>|<span data-ttu-id="6b27b-158">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="6b27b-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="6b27b-159">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6b27b-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6b27b-160">displayName</span><span class="sxs-lookup"><span data-stu-id="6b27b-160">displayName</span></span>|<span data-ttu-id="6b27b-161">String</span><span class="sxs-lookup"><span data-stu-id="6b27b-161">String</span></span>|<span data-ttu-id="6b27b-162">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="6b27b-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="6b27b-163">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6b27b-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6b27b-164">version</span><span class="sxs-lookup"><span data-stu-id="6b27b-164">version</span></span>|<span data-ttu-id="6b27b-165">Int32</span><span class="sxs-lookup"><span data-stu-id="6b27b-165">Int32</span></span>|<span data-ttu-id="6b27b-166">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="6b27b-166">Version of the device configuration.</span></span> <span data-ttu-id="6b27b-167">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6b27b-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6b27b-168">dmaGuardDeviceEnumerationPolicy</span><span class="sxs-lookup"><span data-stu-id="6b27b-168">dmaGuardDeviceEnumerationPolicy</span></span>|[<span data-ttu-id="6b27b-169">dmaGuardDeviceEnumerationPolicyType</span><span class="sxs-lookup"><span data-stu-id="6b27b-169">dmaGuardDeviceEnumerationPolicyType</span></span>](../resources/intune-deviceconfig-dmaguarddeviceenumerationpolicytype.md)|<span data-ttu-id="6b27b-170">此策略旨在提供针对外部 DMA 功能的设备的其他安全。</span><span class="sxs-lookup"><span data-stu-id="6b27b-170">This policy is intended to provide additional security against external DMA capable devices.</span></span> <span data-ttu-id="6b27b-171">允许更好地控制外部 DMA 能够设备枚举与 DMA Remapping/设备内存隔离和沙盒不兼容。</span><span class="sxs-lookup"><span data-stu-id="6b27b-171">It allows for more control over the enumeration of external DMA capable devices incompatible with DMA Remapping/device memory isolation and sandboxing.</span></span> <span data-ttu-id="6b27b-172">支持并由系统固件启用内核 DMA 保护时，此策略才能起作用。</span><span class="sxs-lookup"><span data-stu-id="6b27b-172">This policy only takes effect when Kernel DMA Protection is supported and enabled by the system firmware.</span></span> <span data-ttu-id="6b27b-173">内核 DMA 保护是通过策略或最终用户无法控制平台功能。</span><span class="sxs-lookup"><span data-stu-id="6b27b-173">Kernel DMA Protection is a platform feature that cannot be controlled via policy or by end user.</span></span> <span data-ttu-id="6b27b-174">它具有制造时，系统必须支持。</span><span class="sxs-lookup"><span data-stu-id="6b27b-174">It has to be supported by the system at the time of manufacturing.</span></span> <span data-ttu-id="6b27b-175">若要检查系统是否支持内核 DMA 保护，请检查的 MSINFO32.exe 摘要页中的内核 DMA 保护字段。</span><span class="sxs-lookup"><span data-stu-id="6b27b-175">To check if the system supports Kernel DMA Protection, please check the Kernel DMA Protection field in the Summary page of MSINFO32.exe.</span></span> <span data-ttu-id="6b27b-176">可取值为：`deviceDefault`、`blockAll`、`allowAll`。</span><span class="sxs-lookup"><span data-stu-id="6b27b-176">Possible values are: `deviceDefault`, `blockAll`, `allowAll`.</span></span>|
|<span data-ttu-id="6b27b-177">userRightsAccessCredentialManagerAsTrustedCaller</span><span class="sxs-lookup"><span data-stu-id="6b27b-177">userRightsAccessCredentialManagerAsTrustedCaller</span></span>|[<span data-ttu-id="6b27b-178">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="6b27b-178">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="6b27b-179">此用户权限备份/还原过程中使用的凭据管理器中。</span><span class="sxs-lookup"><span data-stu-id="6b27b-179">This user right is used by Credential Manager during Backup/Restore.</span></span> <span data-ttu-id="6b27b-180">用户的已保存的凭据可能受到威胁，如果此权限授予的其他实体。</span><span class="sxs-lookup"><span data-stu-id="6b27b-180">Users' saved credentials might be compromised if this privilege is given to other entities.</span></span> <span data-ttu-id="6b27b-181">支持状态 NotConfigured 和允许</span><span class="sxs-lookup"><span data-stu-id="6b27b-181">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="6b27b-182">userRightsAllowAccessFromNetwork</span><span class="sxs-lookup"><span data-stu-id="6b27b-182">userRightsAllowAccessFromNetwork</span></span>|[<span data-ttu-id="6b27b-183">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="6b27b-183">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="6b27b-184">此用户权限确定哪些用户和组允许通过网络连接到计算机。</span><span class="sxs-lookup"><span data-stu-id="6b27b-184">This user right determines which users and groups are allowed to connect to the computer over the network.</span></span> <span data-ttu-id="6b27b-185">支持状态允许。</span><span class="sxs-lookup"><span data-stu-id="6b27b-185">State Allowed is supported.</span></span>|
|<span data-ttu-id="6b27b-186">userRightsBlockAccessFromNetwork</span><span class="sxs-lookup"><span data-stu-id="6b27b-186">userRightsBlockAccessFromNetwork</span></span>|[<span data-ttu-id="6b27b-187">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="6b27b-187">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="6b27b-188">此用户权限确定哪些用户和组是通过网络连接到计算机的块。</span><span class="sxs-lookup"><span data-stu-id="6b27b-188">This user right determines which users and groups are block from connecting to the computer over the network.</span></span> <span data-ttu-id="6b27b-189">支持状态块。</span><span class="sxs-lookup"><span data-stu-id="6b27b-189">State Block is supported.</span></span>|
|<span data-ttu-id="6b27b-190">userRightsActAsPartOfTheOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="6b27b-190">userRightsActAsPartOfTheOperatingSystem</span></span>|[<span data-ttu-id="6b27b-191">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="6b27b-191">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="6b27b-192">此用户权限允许模拟任何用户无需身份验证的过程。</span><span class="sxs-lookup"><span data-stu-id="6b27b-192">This user right allows a process to impersonate any user without authentication.</span></span> <span data-ttu-id="6b27b-193">过程因此可以访问与该用户相同的本地资源。</span><span class="sxs-lookup"><span data-stu-id="6b27b-193">The process can therefore gain access to the same local resources as that user.</span></span> <span data-ttu-id="6b27b-194">支持状态 NotConfigured 和允许</span><span class="sxs-lookup"><span data-stu-id="6b27b-194">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="6b27b-195">userRightsLocalLogOn</span><span class="sxs-lookup"><span data-stu-id="6b27b-195">userRightsLocalLogOn</span></span>|[<span data-ttu-id="6b27b-196">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="6b27b-196">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="6b27b-197">此用户权限确定哪些用户可以登录到计算机。</span><span class="sxs-lookup"><span data-stu-id="6b27b-197">This user right determines which users can log on to the computer.</span></span> <span data-ttu-id="6b27b-198">状态 NotConfigured、 允许和已阻止所有支持</span><span class="sxs-lookup"><span data-stu-id="6b27b-198">States NotConfigured, Allowed and Blocked are all supported</span></span> |
|<span data-ttu-id="6b27b-199">userRightsBackupData</span><span class="sxs-lookup"><span data-stu-id="6b27b-199">userRightsBackupData</span></span>|[<span data-ttu-id="6b27b-200">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="6b27b-200">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="6b27b-201">此用户权限确定哪些用户可以跳过文件、 目录、 注册表和其他永久对象权限时备份文件和目录。</span><span class="sxs-lookup"><span data-stu-id="6b27b-201">This user right determines which users can bypass file, directory, registry, and other persistent objects permissions when backing up files and directories.</span></span> <span data-ttu-id="6b27b-202">支持状态 NotConfigured 和允许</span><span class="sxs-lookup"><span data-stu-id="6b27b-202">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="6b27b-203">userRightsChangeSystemTime</span><span class="sxs-lookup"><span data-stu-id="6b27b-203">userRightsChangeSystemTime</span></span>|[<span data-ttu-id="6b27b-204">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="6b27b-204">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="6b27b-205">此用户权限确定哪些用户和组可以更改计算机内部时钟的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="6b27b-205">This user right determines which users and groups can change the time and date on the internal clock of the computer.</span></span> <span data-ttu-id="6b27b-206">支持状态 NotConfigured 和允许</span><span class="sxs-lookup"><span data-stu-id="6b27b-206">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="6b27b-207">userRightsCreateGlobalObjects</span><span class="sxs-lookup"><span data-stu-id="6b27b-207">userRightsCreateGlobalObjects</span></span>|[<span data-ttu-id="6b27b-208">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="6b27b-208">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="6b27b-209">此安全设置确定用户是否可以创建可供所有会话的全局对象。</span><span class="sxs-lookup"><span data-stu-id="6b27b-209">This security setting determines whether users can create global objects that are available to all sessions.</span></span> <span data-ttu-id="6b27b-210">可以创建全局对象的用户可能会影响其他用户的会话，这可能导致应用程序故障或数据损坏下运行的进程。</span><span class="sxs-lookup"><span data-stu-id="6b27b-210">Users who can create global objects could affect processes that run under other users' sessions, which could lead to application failure or data corruption.</span></span> <span data-ttu-id="6b27b-211">支持状态 NotConfigured 和允许</span><span class="sxs-lookup"><span data-stu-id="6b27b-211">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="6b27b-212">userRightsCreatePageFile</span><span class="sxs-lookup"><span data-stu-id="6b27b-212">userRightsCreatePageFile</span></span>|[<span data-ttu-id="6b27b-213">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="6b27b-213">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="6b27b-214">此用户权限确定哪些用户和组可以呼叫内部 API 创建和更改页面文件的大小。</span><span class="sxs-lookup"><span data-stu-id="6b27b-214">This user right determines which users and groups can call an internal API to create and change the size of a page file.</span></span> <span data-ttu-id="6b27b-215">支持状态 NotConfigured 和允许</span><span class="sxs-lookup"><span data-stu-id="6b27b-215">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="6b27b-216">userRightsCreatePermanentSharedObjects</span><span class="sxs-lookup"><span data-stu-id="6b27b-216">userRightsCreatePermanentSharedObjects</span></span>|[<span data-ttu-id="6b27b-217">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="6b27b-217">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="6b27b-218">此用户权限确定哪些帐户可用于通过流程管理器中创建使用对象的目录对象。</span><span class="sxs-lookup"><span data-stu-id="6b27b-218">This user right determines which accounts can be used by processes to create a directory object using the object manager.</span></span> <span data-ttu-id="6b27b-219">支持状态 NotConfigured 和允许</span><span class="sxs-lookup"><span data-stu-id="6b27b-219">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="6b27b-220">userRightsCreateSymbolicLinks</span><span class="sxs-lookup"><span data-stu-id="6b27b-220">userRightsCreateSymbolicLinks</span></span>|[<span data-ttu-id="6b27b-221">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="6b27b-221">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="6b27b-222">此用户权限确定是否用户可以从与他们登录到计算机创建符号链接。</span><span class="sxs-lookup"><span data-stu-id="6b27b-222">This user right determines if the user can create a symbolic link from the computer to which they are logged on.</span></span> <span data-ttu-id="6b27b-223">支持状态 NotConfigured 和允许</span><span class="sxs-lookup"><span data-stu-id="6b27b-223">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="6b27b-224">userRightsCreateToken</span><span class="sxs-lookup"><span data-stu-id="6b27b-224">userRightsCreateToken</span></span>|[<span data-ttu-id="6b27b-225">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="6b27b-225">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="6b27b-226">此用户权限确定哪些用户/组可以由进程来创建用于时过程使用内部 API 来创建访问令牌获取对任何本地资源的访问令牌。</span><span class="sxs-lookup"><span data-stu-id="6b27b-226">This user right determines which users/groups can be used by processes to create a token that can then be used to get access to any local resources when the process uses an internal API to create an access token.</span></span> <span data-ttu-id="6b27b-227">支持状态 NotConfigured 和允许</span><span class="sxs-lookup"><span data-stu-id="6b27b-227">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="6b27b-228">userRightsDebugPrograms</span><span class="sxs-lookup"><span data-stu-id="6b27b-228">userRightsDebugPrograms</span></span>|[<span data-ttu-id="6b27b-229">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="6b27b-229">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="6b27b-230">此用户权限确定哪些用户可以将调试器附加到任何进程或内核。</span><span class="sxs-lookup"><span data-stu-id="6b27b-230">This user right determines which users can attach a debugger to any process or to the kernel.</span></span> <span data-ttu-id="6b27b-231">支持状态 NotConfigured 和允许</span><span class="sxs-lookup"><span data-stu-id="6b27b-231">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="6b27b-232">userRightsRemoteDesktopServicesLogOn</span><span class="sxs-lookup"><span data-stu-id="6b27b-232">userRightsRemoteDesktopServicesLogOn</span></span>|[<span data-ttu-id="6b27b-233">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="6b27b-233">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="6b27b-234">此用户权限确定禁止哪些用户和组作为远程桌面服务客户端登录。</span><span class="sxs-lookup"><span data-stu-id="6b27b-234">This user right determines which users and groups are prohibited from logging on as a Remote Desktop Services client.</span></span> <span data-ttu-id="6b27b-235">支持状态 NotConfigured 和被阻止</span><span class="sxs-lookup"><span data-stu-id="6b27b-235">Only states NotConfigured and Blocked are supported</span></span>|
|<span data-ttu-id="6b27b-236">userRightsDelegation</span><span class="sxs-lookup"><span data-stu-id="6b27b-236">userRightsDelegation</span></span>|[<span data-ttu-id="6b27b-237">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="6b27b-237">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="6b27b-238">此用户权限确定哪些用户可以在用户或计算机对象上设置委派设置受信任。</span><span class="sxs-lookup"><span data-stu-id="6b27b-238">This user right determines which users can set the Trusted for Delegation setting on a user or computer object.</span></span> <span data-ttu-id="6b27b-239">支持状态 NotConfigured 和允许。</span><span class="sxs-lookup"><span data-stu-id="6b27b-239">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="6b27b-240">userRightsGenerateSecurityAudits</span><span class="sxs-lookup"><span data-stu-id="6b27b-240">userRightsGenerateSecurityAudits</span></span>|[<span data-ttu-id="6b27b-241">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="6b27b-241">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="6b27b-242">此用户权限确定哪些帐户可用于由进程将条目添加到安全日志。</span><span class="sxs-lookup"><span data-stu-id="6b27b-242">This user right determines which accounts can be used by a process to add entries to the security log.</span></span> <span data-ttu-id="6b27b-243">安全日志用于跟踪未经授权的系统的访问。</span><span class="sxs-lookup"><span data-stu-id="6b27b-243">The security log is used to trace unauthorized system access.</span></span>  <span data-ttu-id="6b27b-244">支持状态 NotConfigured 和允许。</span><span class="sxs-lookup"><span data-stu-id="6b27b-244">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="6b27b-245">userRightsImpersonateClient</span><span class="sxs-lookup"><span data-stu-id="6b27b-245">userRightsImpersonateClient</span></span>|[<span data-ttu-id="6b27b-246">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="6b27b-246">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="6b27b-247">分配给用户此用户权限允许代表该用户模拟客户端运行的程序。</span><span class="sxs-lookup"><span data-stu-id="6b27b-247">Assigning this user right to a user allows programs running on behalf of that user to impersonate a client.</span></span> <span data-ttu-id="6b27b-248">对于此种模拟需要此用户权限可防止未经授权的用户从诱使客户端连接到他们创建的服务，然后这样可以将提升未经授权的用户的权限模拟该客户端，管理或系统级别。</span><span class="sxs-lookup"><span data-stu-id="6b27b-248">Requiring this user right for this kind of impersonation prevents an unauthorized user from convincing a client to connect to a service that they have created and then impersonating that client, which can elevate the unauthorized user's permissions to administrative or system levels.</span></span> <span data-ttu-id="6b27b-249">支持状态 NotConfigured 和允许。</span><span class="sxs-lookup"><span data-stu-id="6b27b-249">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="6b27b-250">userRightsIncreaseSchedulingPriority</span><span class="sxs-lookup"><span data-stu-id="6b27b-250">userRightsIncreaseSchedulingPriority</span></span>|[<span data-ttu-id="6b27b-251">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="6b27b-251">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="6b27b-252">此用户权限确定哪些帐户可用于过程写入属性访问另一个进程增加分配给其他进程的执行优先级。</span><span class="sxs-lookup"><span data-stu-id="6b27b-252">This user right determines which accounts can use a process with Write Property access to another process to increase the execution priority assigned to the other process.</span></span> <span data-ttu-id="6b27b-253">支持状态 NotConfigured 和允许。</span><span class="sxs-lookup"><span data-stu-id="6b27b-253">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="6b27b-254">userRightsLoadUnloadDrivers</span><span class="sxs-lookup"><span data-stu-id="6b27b-254">userRightsLoadUnloadDrivers</span></span>|[<span data-ttu-id="6b27b-255">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="6b27b-255">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="6b27b-256">此用户权限确定哪些用户可以动态加载和卸载设备驱动程序或内核模式中的其他代码。</span><span class="sxs-lookup"><span data-stu-id="6b27b-256">This user right determines which users can dynamically load and unload device drivers or other code in to kernel mode.</span></span> <span data-ttu-id="6b27b-257">支持状态 NotConfigured 和允许。</span><span class="sxs-lookup"><span data-stu-id="6b27b-257">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="6b27b-258">userRightsLockMemory</span><span class="sxs-lookup"><span data-stu-id="6b27b-258">userRightsLockMemory</span></span>|[<span data-ttu-id="6b27b-259">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="6b27b-259">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="6b27b-260">此用户权限确定哪些帐户可使用过程可在物理内存，防止系统分页数据写到磁盘上的虚拟内存中保留数据。</span><span class="sxs-lookup"><span data-stu-id="6b27b-260">This user right determines which accounts can use a process to keep data in physical memory, which prevents the system from paging the data to virtual memory on disk.</span></span> <span data-ttu-id="6b27b-261">支持状态 NotConfigured 和允许。</span><span class="sxs-lookup"><span data-stu-id="6b27b-261">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="6b27b-262">userRightsManageAuditingAndSecurityLogs</span><span class="sxs-lookup"><span data-stu-id="6b27b-262">userRightsManageAuditingAndSecurityLogs</span></span>|[<span data-ttu-id="6b27b-263">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="6b27b-263">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="6b27b-264">此用户权限确定哪些用户可以指定对象访问审核各个资源，如文件、 Active Directory 对象和注册表项选项。</span><span class="sxs-lookup"><span data-stu-id="6b27b-264">This user right determines which users can specify object access auditing options for individual resources, such as files, Active Directory objects, and registry keys.</span></span> <span data-ttu-id="6b27b-265">支持状态 NotConfigured 和允许。</span><span class="sxs-lookup"><span data-stu-id="6b27b-265">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="6b27b-266">userRightsManageVolumes</span><span class="sxs-lookup"><span data-stu-id="6b27b-266">userRightsManageVolumes</span></span>|[<span data-ttu-id="6b27b-267">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="6b27b-267">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="6b27b-268">此用户权限确定哪些用户和组可以在卷上，如远程磁盘碎片整理运行维护任务。</span><span class="sxs-lookup"><span data-stu-id="6b27b-268">This user right determines which users and groups can run maintenance tasks on a volume, such as remote defragmentation.</span></span> <span data-ttu-id="6b27b-269">支持状态 NotConfigured 和允许。</span><span class="sxs-lookup"><span data-stu-id="6b27b-269">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="6b27b-270">userRightsModifyFirmwareEnvironment</span><span class="sxs-lookup"><span data-stu-id="6b27b-270">userRightsModifyFirmwareEnvironment</span></span>|[<span data-ttu-id="6b27b-271">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="6b27b-271">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="6b27b-272">此用户权限确定谁可以修改固件环境值。</span><span class="sxs-lookup"><span data-stu-id="6b27b-272">This user right determines who can modify firmware environment values.</span></span> <span data-ttu-id="6b27b-273">支持状态 NotConfigured 和允许。</span><span class="sxs-lookup"><span data-stu-id="6b27b-273">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="6b27b-274">userRightsModifyObjectLabels</span><span class="sxs-lookup"><span data-stu-id="6b27b-274">userRightsModifyObjectLabels</span></span>|[<span data-ttu-id="6b27b-275">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="6b27b-275">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="6b27b-276">此用户权限确定哪些用户帐户可以修改对象，如文件、 注册表项或由其他用户拥有的进程的完整性标签。</span><span class="sxs-lookup"><span data-stu-id="6b27b-276">This user right determines which user accounts can modify the integrity label of objects, such as files, registry keys, or processes owned by other users.</span></span> <span data-ttu-id="6b27b-277">支持状态 NotConfigured 和允许。</span><span class="sxs-lookup"><span data-stu-id="6b27b-277">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="6b27b-278">userRightsProfileSingleProcess</span><span class="sxs-lookup"><span data-stu-id="6b27b-278">userRightsProfileSingleProcess</span></span>|[<span data-ttu-id="6b27b-279">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="6b27b-279">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="6b27b-280">此用户权限确定哪些用户可以使用性能监视工具来监视系统进程的性能。</span><span class="sxs-lookup"><span data-stu-id="6b27b-280">This user right determines which users can use performance monitoring tools to monitor the performance of system processes.</span></span> <span data-ttu-id="6b27b-281">支持状态 NotConfigured 和允许。</span><span class="sxs-lookup"><span data-stu-id="6b27b-281">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="6b27b-282">userRightsRemoteShutdown</span><span class="sxs-lookup"><span data-stu-id="6b27b-282">userRightsRemoteShutdown</span></span>|[<span data-ttu-id="6b27b-283">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="6b27b-283">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="6b27b-284">此用户权限确定允许哪些用户关闭，将计算机从网络上的远程位置。</span><span class="sxs-lookup"><span data-stu-id="6b27b-284">This user right determines which users are allowed to shut down a computer from a remote location on the network.</span></span> <span data-ttu-id="6b27b-285">此用户权限的误用会导致拒绝服务。</span><span class="sxs-lookup"><span data-stu-id="6b27b-285">Misuse of this user right can result in a denial of service.</span></span> <span data-ttu-id="6b27b-286">支持状态 NotConfigured 和允许。</span><span class="sxs-lookup"><span data-stu-id="6b27b-286">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="6b27b-287">userRightsRestoreData</span><span class="sxs-lookup"><span data-stu-id="6b27b-287">userRightsRestoreData</span></span>|[<span data-ttu-id="6b27b-288">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="6b27b-288">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="6b27b-289">此用户权限决定哪些用户可以跳过文件、 目录、 注册表和权限还原时备份文件和目录，其他持久对象，决定哪些用户可以设置为对象的所有者的任何有效的安全主体。</span><span class="sxs-lookup"><span data-stu-id="6b27b-289">This user right determines which users can bypass file, directory, registry, and other persistent objects permissions when restoring backed up files and directories, and determines which users can set any valid security principal as the owner of an object.</span></span> <span data-ttu-id="6b27b-290">支持状态 NotConfigured 和允许。</span><span class="sxs-lookup"><span data-stu-id="6b27b-290">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="6b27b-291">userRightsTakeOwnership</span><span class="sxs-lookup"><span data-stu-id="6b27b-291">userRightsTakeOwnership</span></span>|[<span data-ttu-id="6b27b-292">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="6b27b-292">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="6b27b-293">此用户权限决定哪些用户可以在系统中，包括 Active Directory 对象、 文件和文件夹、 打印机、 注册表项、 流程和线程执行任何安全对象的所有权。</span><span class="sxs-lookup"><span data-stu-id="6b27b-293">This user right determines which users can take ownership of any securable object in the system, including Active Directory objects, files and folders, printers, registry keys, processes, and threads.</span></span> <span data-ttu-id="6b27b-294">支持状态 NotConfigured 和允许。</span><span class="sxs-lookup"><span data-stu-id="6b27b-294">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="6b27b-295">userRightsRegisterProcessAsService</span><span class="sxs-lookup"><span data-stu-id="6b27b-295">userRightsRegisterProcessAsService</span></span>|[<span data-ttu-id="6b27b-296">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="6b27b-296">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="6b27b-297">此安全设置确定被阻止的服务帐户注册为服务的进程。</span><span class="sxs-lookup"><span data-stu-id="6b27b-297">This security setting determines which service accounts are prevented from registering a process as a service.</span></span> <span data-ttu-id="6b27b-298">注意： 此安全设置不适用于系统、 本地服务或网络服务帐户。</span><span class="sxs-lookup"><span data-stu-id="6b27b-298">Note: This security setting does not apply to the System, Local Service, or Network Service accounts.</span></span> <span data-ttu-id="6b27b-299">仅支持已阻止的状态。</span><span class="sxs-lookup"><span data-stu-id="6b27b-299">Only state Blocked is supported.</span></span>|
|<span data-ttu-id="6b27b-300">xboxServicesEnableXboxGameSaveTask</span><span class="sxs-lookup"><span data-stu-id="6b27b-300">xboxServicesEnableXboxGameSaveTask</span></span>|<span data-ttu-id="6b27b-301">Boolean</span><span class="sxs-lookup"><span data-stu-id="6b27b-301">Boolean</span></span>|<span data-ttu-id="6b27b-302">此设置确定 xbox 游戏保存是否启用 (1) 或禁用 (0)。</span><span class="sxs-lookup"><span data-stu-id="6b27b-302">This setting determines whether xbox game save is enabled (1) or disabled (0).</span></span>|
|<span data-ttu-id="6b27b-303">xboxServicesAccessoryManagementServiceStartupMode</span><span class="sxs-lookup"><span data-stu-id="6b27b-303">xboxServicesAccessoryManagementServiceStartupMode</span></span>|[<span data-ttu-id="6b27b-304">serviceStartType</span><span class="sxs-lookup"><span data-stu-id="6b27b-304">serviceStartType</span></span>](../resources/intune-deviceconfig-servicestarttype.md)|<span data-ttu-id="6b27b-305">此设置确定的附件管理服务启动类型是 Automatic(2) Manual(3)、 Disabled(4)。</span><span class="sxs-lookup"><span data-stu-id="6b27b-305">This setting determines whether the Accessory management service's start type is Automatic(2), Manual(3), Disabled(4).</span></span> <span data-ttu-id="6b27b-306">默认： 手动。</span><span class="sxs-lookup"><span data-stu-id="6b27b-306">Default: Manual.</span></span> <span data-ttu-id="6b27b-307">可取值为：`manual`、`automatic`、`disabled`。</span><span class="sxs-lookup"><span data-stu-id="6b27b-307">Possible values are: `manual`, `automatic`, `disabled`.</span></span>|
|<span data-ttu-id="6b27b-308">xboxServicesLiveAuthManagerServiceStartupMode</span><span class="sxs-lookup"><span data-stu-id="6b27b-308">xboxServicesLiveAuthManagerServiceStartupMode</span></span>|[<span data-ttu-id="6b27b-309">serviceStartType</span><span class="sxs-lookup"><span data-stu-id="6b27b-309">serviceStartType</span></span>](../resources/intune-deviceconfig-servicestarttype.md)|<span data-ttu-id="6b27b-310">此设置确定 Live 身份验证管理器服务启动类型是 Automatic(2) Manual(3)、 Disabled(4)。</span><span class="sxs-lookup"><span data-stu-id="6b27b-310">This setting determines whether Live Auth Manager service's start type is Automatic(2), Manual(3), Disabled(4).</span></span> <span data-ttu-id="6b27b-311">默认： 手动。</span><span class="sxs-lookup"><span data-stu-id="6b27b-311">Default: Manual.</span></span> <span data-ttu-id="6b27b-312">可取值为：`manual`、`automatic`、`disabled`。</span><span class="sxs-lookup"><span data-stu-id="6b27b-312">Possible values are: `manual`, `automatic`, `disabled`.</span></span>|
|<span data-ttu-id="6b27b-313">xboxServicesLiveGameSaveServiceStartupMode</span><span class="sxs-lookup"><span data-stu-id="6b27b-313">xboxServicesLiveGameSaveServiceStartupMode</span></span>|[<span data-ttu-id="6b27b-314">serviceStartType</span><span class="sxs-lookup"><span data-stu-id="6b27b-314">serviceStartType</span></span>](../resources/intune-deviceconfig-servicestarttype.md)|<span data-ttu-id="6b27b-315">此设置确定是否 Automatic(2) Manual(3)、 Disabled(4) Live 保存服务的启动类型的游戏。</span><span class="sxs-lookup"><span data-stu-id="6b27b-315">This setting determines whether Live Game save service's start type is Automatic(2), Manual(3), Disabled(4).</span></span> <span data-ttu-id="6b27b-316">默认： 手动。</span><span class="sxs-lookup"><span data-stu-id="6b27b-316">Default: Manual.</span></span> <span data-ttu-id="6b27b-317">可取值为：`manual`、`automatic`、`disabled`。</span><span class="sxs-lookup"><span data-stu-id="6b27b-317">Possible values are: `manual`, `automatic`, `disabled`.</span></span>|
|<span data-ttu-id="6b27b-318">xboxServicesLiveNetworkingServiceStartupMode</span><span class="sxs-lookup"><span data-stu-id="6b27b-318">xboxServicesLiveNetworkingServiceStartupMode</span></span>|[<span data-ttu-id="6b27b-319">serviceStartType</span><span class="sxs-lookup"><span data-stu-id="6b27b-319">serviceStartType</span></span>](../resources/intune-deviceconfig-servicestarttype.md)|<span data-ttu-id="6b27b-320">此设置确定网络服务启动类型是 Automatic(2) Manual(3)、 Disabled(4)。</span><span class="sxs-lookup"><span data-stu-id="6b27b-320">This setting determines whether Networking service's start type is Automatic(2), Manual(3), Disabled(4).</span></span> <span data-ttu-id="6b27b-321">默认： 手动。</span><span class="sxs-lookup"><span data-stu-id="6b27b-321">Default: Manual.</span></span> <span data-ttu-id="6b27b-322">可取值为：`manual`、`automatic`、`disabled`。</span><span class="sxs-lookup"><span data-stu-id="6b27b-322">Possible values are: `manual`, `automatic`, `disabled`.</span></span>|
|<span data-ttu-id="6b27b-323">localSecurityOptionsBlockMicrosoftAccounts</span><span class="sxs-lookup"><span data-stu-id="6b27b-323">localSecurityOptionsBlockMicrosoftAccounts</span></span>|<span data-ttu-id="6b27b-324">Boolean</span><span class="sxs-lookup"><span data-stu-id="6b27b-324">Boolean</span></span>|<span data-ttu-id="6b27b-325">禁止用户添加到此计算机的新的 Microsoft 帐户。</span><span class="sxs-lookup"><span data-stu-id="6b27b-325">Prevent users from adding new Microsoft accounts to this computer.</span></span>|
|<span data-ttu-id="6b27b-326">localSecurityOptionsBlockRemoteLogonWithBlankPassword</span><span class="sxs-lookup"><span data-stu-id="6b27b-326">localSecurityOptionsBlockRemoteLogonWithBlankPassword</span></span>|<span data-ttu-id="6b27b-327">Boolean</span><span class="sxs-lookup"><span data-stu-id="6b27b-327">Boolean</span></span>|<span data-ttu-id="6b27b-328">启用本地帐户不受密码保护登录从物理设备以外的位置。将启用默认值</span><span class="sxs-lookup"><span data-stu-id="6b27b-328">Enable Local accounts that are not password protected to log on from locations other than the physical device.Default is enabled</span></span>|
|<span data-ttu-id="6b27b-329">localSecurityOptionsDisableAdministratorAccount</span><span class="sxs-lookup"><span data-stu-id="6b27b-329">localSecurityOptionsDisableAdministratorAccount</span></span>|<span data-ttu-id="6b27b-330">Boolean</span><span class="sxs-lookup"><span data-stu-id="6b27b-330">Boolean</span></span>|<span data-ttu-id="6b27b-331">确定是否启用或禁用的本地管理员帐户。</span><span class="sxs-lookup"><span data-stu-id="6b27b-331">Determines whether the Local Administrator account is enabled or disabled.</span></span>|
|<span data-ttu-id="6b27b-332">localSecurityOptionsAdministratorAccountName</span><span class="sxs-lookup"><span data-stu-id="6b27b-332">localSecurityOptionsAdministratorAccountName</span></span>|<span data-ttu-id="6b27b-333">String</span><span class="sxs-lookup"><span data-stu-id="6b27b-333">String</span></span>|<span data-ttu-id="6b27b-334">定义要与"管理员"的帐户的安全标识符 (SID) 关联的不同的帐户名称。</span><span class="sxs-lookup"><span data-stu-id="6b27b-334">Define a different account name to be associated with the security identifier (SID) for the account “Administrator”.</span></span>|
|<span data-ttu-id="6b27b-335">localSecurityOptionsDisableGuestAccount</span><span class="sxs-lookup"><span data-stu-id="6b27b-335">localSecurityOptionsDisableGuestAccount</span></span>|<span data-ttu-id="6b27b-336">Boolean</span><span class="sxs-lookup"><span data-stu-id="6b27b-336">Boolean</span></span>|<span data-ttu-id="6b27b-337">确定是启用还是禁用来宾帐户。</span><span class="sxs-lookup"><span data-stu-id="6b27b-337">Determines if the Guest account is enabled or disabled.</span></span>|
|<span data-ttu-id="6b27b-338">localSecurityOptionsGuestAccountName</span><span class="sxs-lookup"><span data-stu-id="6b27b-338">localSecurityOptionsGuestAccountName</span></span>|<span data-ttu-id="6b27b-339">String</span><span class="sxs-lookup"><span data-stu-id="6b27b-339">String</span></span>|<span data-ttu-id="6b27b-340">定义要为"来宾"的帐户的安全标识符 (SID) 关联的不同的帐户名称。</span><span class="sxs-lookup"><span data-stu-id="6b27b-340">Define a different account name to be associated with the security identifier (SID) for the account “Guest”.</span></span>|
|<span data-ttu-id="6b27b-341">localSecurityOptionsAllowUndockWithoutHavingToLogon</span><span class="sxs-lookup"><span data-stu-id="6b27b-341">localSecurityOptionsAllowUndockWithoutHavingToLogon</span></span>|<span data-ttu-id="6b27b-342">Boolean</span><span class="sxs-lookup"><span data-stu-id="6b27b-342">Boolean</span></span>|<span data-ttu-id="6b27b-343">正在取消停靠而无需登录阻止便携式计算机。</span><span class="sxs-lookup"><span data-stu-id="6b27b-343">Prevent a portable computer from being undocked without having to log in.</span></span>|
|<span data-ttu-id="6b27b-344">localSecurityOptionsBlockUsersInstallingPrinterDrivers</span><span class="sxs-lookup"><span data-stu-id="6b27b-344">localSecurityOptionsBlockUsersInstallingPrinterDrivers</span></span>|<span data-ttu-id="6b27b-345">Boolean</span><span class="sxs-lookup"><span data-stu-id="6b27b-345">Boolean</span></span>|<span data-ttu-id="6b27b-346">限制为连接到向管理员仅共享打印机的一部分安装的打印机驱动程序。</span><span class="sxs-lookup"><span data-stu-id="6b27b-346">Restrict installing printer drivers as part of connecting to a shared printer to admins only.</span></span>|
|<span data-ttu-id="6b27b-347">localSecurityOptionsBlockRemoteOpticalDriveAccess</span><span class="sxs-lookup"><span data-stu-id="6b27b-347">localSecurityOptionsBlockRemoteOpticalDriveAccess</span></span>|<span data-ttu-id="6b27b-348">Boolean</span><span class="sxs-lookup"><span data-stu-id="6b27b-348">Boolean</span></span>|<span data-ttu-id="6b27b-349">启用此设置允许访问 CD-ROM 媒体仅以交互方式登录的用户。</span><span class="sxs-lookup"><span data-stu-id="6b27b-349">Enabling this settings allows only interactively logged on user to access CD-ROM media.</span></span>|
|<span data-ttu-id="6b27b-350">localSecurityOptionsFormatAndEjectOfRemovableMediaAllowedUser</span><span class="sxs-lookup"><span data-stu-id="6b27b-350">localSecurityOptionsFormatAndEjectOfRemovableMediaAllowedUser</span></span>|[<span data-ttu-id="6b27b-351">localSecurityOptionsFormatAndEjectOfRemovableMediaAllowedUserType</span><span class="sxs-lookup"><span data-stu-id="6b27b-351">localSecurityOptionsFormatAndEjectOfRemovableMediaAllowedUserType</span></span>](../resources/intune-deviceconfig-localsecurityoptionsformatandejectofremovablemediaallowedusertype.md)|<span data-ttu-id="6b27b-352">定义允许谁格式化和弹出可移动 NTFS 媒体。</span><span class="sxs-lookup"><span data-stu-id="6b27b-352">Define who is allowed to format and eject removable NTFS media.</span></span> <span data-ttu-id="6b27b-353">可取值为：`notConfigured`、`administrators`、`administratorsAndPowerUsers`、`administratorsAndInteractiveUsers`。</span><span class="sxs-lookup"><span data-stu-id="6b27b-353">Possible values are: `notConfigured`, `administrators`, `administratorsAndPowerUsers`, `administratorsAndInteractiveUsers`.</span></span>|
|<span data-ttu-id="6b27b-354">localSecurityOptionsMachineInactivityLimit</span><span class="sxs-lookup"><span data-stu-id="6b27b-354">localSecurityOptionsMachineInactivityLimit</span></span>|<span data-ttu-id="6b27b-355">Int32</span><span class="sxs-lookup"><span data-stu-id="6b27b-355">Int32</span></span>|<span data-ttu-id="6b27b-356">交互式桌面上登录屏幕上定义最大分钟无活动，直到屏幕保护程序运行。</span><span class="sxs-lookup"><span data-stu-id="6b27b-356">Define maximum minutes of inactivity on the interactive desktop’s login screen until the screen saver runs.</span></span> <span data-ttu-id="6b27b-357">有效的值 0 到 9999 之间</span><span class="sxs-lookup"><span data-stu-id="6b27b-357">Valid values 0 to 9999</span></span>|
|<span data-ttu-id="6b27b-358">localSecurityOptionsMachineInactivityLimitInMinutes</span><span class="sxs-lookup"><span data-stu-id="6b27b-358">localSecurityOptionsMachineInactivityLimitInMinutes</span></span>|<span data-ttu-id="6b27b-359">Int32</span><span class="sxs-lookup"><span data-stu-id="6b27b-359">Int32</span></span>|<span data-ttu-id="6b27b-360">交互式桌面上登录屏幕上定义最大分钟无活动，直到屏幕保护程序运行。</span><span class="sxs-lookup"><span data-stu-id="6b27b-360">Define maximum minutes of inactivity on the interactive desktop’s login screen until the screen saver runs.</span></span> <span data-ttu-id="6b27b-361">有效的值 0 到 9999 之间</span><span class="sxs-lookup"><span data-stu-id="6b27b-361">Valid values 0 to 9999</span></span>|
|<span data-ttu-id="6b27b-362">localSecurityOptionsDoNotRequireCtrlAltDel</span><span class="sxs-lookup"><span data-stu-id="6b27b-362">localSecurityOptionsDoNotRequireCtrlAltDel</span></span>|<span data-ttu-id="6b27b-363">Boolean</span><span class="sxs-lookup"><span data-stu-id="6b27b-363">Boolean</span></span>|<span data-ttu-id="6b27b-364">需要 CTRL + ALT + DEL 要按用户登录之前。</span><span class="sxs-lookup"><span data-stu-id="6b27b-364">Require CTRL+ALT+DEL to be pressed before a user can log on.</span></span>|
|<span data-ttu-id="6b27b-365">localSecurityOptionsHideLastSignedInUser</span><span class="sxs-lookup"><span data-stu-id="6b27b-365">localSecurityOptionsHideLastSignedInUser</span></span>|<span data-ttu-id="6b27b-366">Boolean</span><span class="sxs-lookup"><span data-stu-id="6b27b-366">Boolean</span></span>|<span data-ttu-id="6b27b-367">不在此设备上显示的签名的最后一个人的用户名。</span><span class="sxs-lookup"><span data-stu-id="6b27b-367">Do not display the username of the last person who signed in on this device.</span></span>|
|<span data-ttu-id="6b27b-368">localSecurityOptionsHideUsernameAtSignIn</span><span class="sxs-lookup"><span data-stu-id="6b27b-368">localSecurityOptionsHideUsernameAtSignIn</span></span>|<span data-ttu-id="6b27b-369">Boolean</span><span class="sxs-lookup"><span data-stu-id="6b27b-369">Boolean</span></span>|<span data-ttu-id="6b27b-370">不显示登录到此设备输入凭据之后和之前显示设备的桌面的人员的用户名。</span><span class="sxs-lookup"><span data-stu-id="6b27b-370">Do not display the username of the person signing in to this device after credentials are entered and before the device’s desktop is shown.</span></span>|
|<span data-ttu-id="6b27b-371">localSecurityOptionsLogOnMessageTitle</span><span class="sxs-lookup"><span data-stu-id="6b27b-371">localSecurityOptionsLogOnMessageTitle</span></span>|<span data-ttu-id="6b27b-372">String</span><span class="sxs-lookup"><span data-stu-id="6b27b-372">String</span></span>|<span data-ttu-id="6b27b-373">用户尝试登录的设置邮件标题。</span><span class="sxs-lookup"><span data-stu-id="6b27b-373">Set message title for users attempting to log in.</span></span>|
|<span data-ttu-id="6b27b-374">localSecurityOptionsLogOnMessageText</span><span class="sxs-lookup"><span data-stu-id="6b27b-374">localSecurityOptionsLogOnMessageText</span></span>|<span data-ttu-id="6b27b-375">String</span><span class="sxs-lookup"><span data-stu-id="6b27b-375">String</span></span>|<span data-ttu-id="6b27b-376">设置用户试图登录消息文本。</span><span class="sxs-lookup"><span data-stu-id="6b27b-376">Set message text for users attempting to log in.</span></span>|
|<span data-ttu-id="6b27b-377">localSecurityOptionsAllowPKU2UAuthenticationRequests</span><span class="sxs-lookup"><span data-stu-id="6b27b-377">localSecurityOptionsAllowPKU2UAuthenticationRequests</span></span>|<span data-ttu-id="6b27b-378">Boolean</span><span class="sxs-lookup"><span data-stu-id="6b27b-378">Boolean</span></span>|<span data-ttu-id="6b27b-379">对此设备块 PKU2U 身份验证请求使用联机标识。</span><span class="sxs-lookup"><span data-stu-id="6b27b-379">Block PKU2U authentication requests to this device to use online identities.</span></span>|
|<span data-ttu-id="6b27b-380">localSecurityOptionsAllowRemoteCallsToSecurityAccountsManagerHelperBool</span><span class="sxs-lookup"><span data-stu-id="6b27b-380">localSecurityOptionsAllowRemoteCallsToSecurityAccountsManagerHelperBool</span></span>|<span data-ttu-id="6b27b-381">Boolean</span><span class="sxs-lookup"><span data-stu-id="6b27b-381">Boolean</span></span>|<span data-ttu-id="6b27b-382">用户界面帮助程序布尔 LocalSecurityOptionsAllowRemoteCallsToSecurityAccountsManager 实体</span><span class="sxs-lookup"><span data-stu-id="6b27b-382">UI helper boolean for LocalSecurityOptionsAllowRemoteCallsToSecurityAccountsManager entity</span></span>|
|<span data-ttu-id="6b27b-383">localSecurityOptionsAllowRemoteCallsToSecurityAccountsManager</span><span class="sxs-lookup"><span data-stu-id="6b27b-383">localSecurityOptionsAllowRemoteCallsToSecurityAccountsManager</span></span>|<span data-ttu-id="6b27b-384">String</span><span class="sxs-lookup"><span data-stu-id="6b27b-384">String</span></span>|<span data-ttu-id="6b27b-385">编辑默认安全描述符定义语言字符串，以允许或拒绝远程调用 SAM 用户和组。</span><span class="sxs-lookup"><span data-stu-id="6b27b-385">Edit the default Security Descriptor Definition Language string to allow or deny users and groups to make remote calls to the SAM.</span></span>|
|<span data-ttu-id="6b27b-386">localSecurityOptionsMinimumSessionSecurityForNtlmSspBasedClients</span><span class="sxs-lookup"><span data-stu-id="6b27b-386">localSecurityOptionsMinimumSessionSecurityForNtlmSspBasedClients</span></span>|[<span data-ttu-id="6b27b-387">localSecurityOptionsMinimumSessionSecurity</span><span class="sxs-lookup"><span data-stu-id="6b27b-387">localSecurityOptionsMinimumSessionSecurity</span></span>](../resources/intune-deviceconfig-localsecurityoptionsminimumsessionsecurity.md)|<span data-ttu-id="6b27b-388">此安全设置允许客户端要求 128 位加密和/或 NTLMv2 会话安全协商。</span><span class="sxs-lookup"><span data-stu-id="6b27b-388">This security setting allows a client to require the negotiation of 128-bit encryption and/or NTLMv2 session security.</span></span> <span data-ttu-id="6b27b-389">可取值为：`none`、`requireNtmlV2SessionSecurity`、`require128BitEncryption`、`ntlmV2And128BitEncryption`。</span><span class="sxs-lookup"><span data-stu-id="6b27b-389">Possible values are: `none`, `requireNtmlV2SessionSecurity`, `require128BitEncryption`, `ntlmV2And128BitEncryption`.</span></span>|
|<span data-ttu-id="6b27b-390">localSecurityOptionsMinimumSessionSecurityForNtlmSspBasedServers</span><span class="sxs-lookup"><span data-stu-id="6b27b-390">localSecurityOptionsMinimumSessionSecurityForNtlmSspBasedServers</span></span>|[<span data-ttu-id="6b27b-391">localSecurityOptionsMinimumSessionSecurity</span><span class="sxs-lookup"><span data-stu-id="6b27b-391">localSecurityOptionsMinimumSessionSecurity</span></span>](../resources/intune-deviceconfig-localsecurityoptionsminimumsessionsecurity.md)|<span data-ttu-id="6b27b-392">此安全设置允许服务器要求 128 位加密和/或 NTLMv2 会话安全协商。</span><span class="sxs-lookup"><span data-stu-id="6b27b-392">This security setting allows a server to require the negotiation of 128-bit encryption and/or NTLMv2 session security.</span></span> <span data-ttu-id="6b27b-393">可取值为：`none`、`requireNtmlV2SessionSecurity`、`require128BitEncryption`、`ntlmV2And128BitEncryption`。</span><span class="sxs-lookup"><span data-stu-id="6b27b-393">Possible values are: `none`, `requireNtmlV2SessionSecurity`, `require128BitEncryption`, `ntlmV2And128BitEncryption`.</span></span>|
|<span data-ttu-id="6b27b-394">lanManagerAuthenticationLevel</span><span class="sxs-lookup"><span data-stu-id="6b27b-394">lanManagerAuthenticationLevel</span></span>|[<span data-ttu-id="6b27b-395">lanManagerAuthenticationLevel</span><span class="sxs-lookup"><span data-stu-id="6b27b-395">lanManagerAuthenticationLevel</span></span>](../resources/intune-deviceconfig-lanmanagerauthenticationlevel.md)|<span data-ttu-id="6b27b-396">此安全设置确定哪个质询/响应身份验证协议用于网络登录。</span><span class="sxs-lookup"><span data-stu-id="6b27b-396">This security setting determines which challenge/response authentication protocol is used for network logons.</span></span> <span data-ttu-id="6b27b-397">可取值为：`lmAndNltm`、`lmNtlmAndNtlmV2`、`lmAndNtlmOnly`、`lmAndNtlmV2`、`lmNtlmV2AndNotLm`、`lmNtlmV2AndNotLmOrNtm`。</span><span class="sxs-lookup"><span data-stu-id="6b27b-397">Possible values are: `lmAndNltm`, `lmNtlmAndNtlmV2`, `lmAndNtlmOnly`, `lmAndNtlmV2`, `lmNtlmV2AndNotLm`, `lmNtlmV2AndNotLmOrNtm`.</span></span>|
|<span data-ttu-id="6b27b-398">lanManagerWorkstationDisableInsecureGuestLogons</span><span class="sxs-lookup"><span data-stu-id="6b27b-398">lanManagerWorkstationDisableInsecureGuestLogons</span></span>|<span data-ttu-id="6b27b-399">Boolean</span><span class="sxs-lookup"><span data-stu-id="6b27b-399">Boolean</span></span>|<span data-ttu-id="6b27b-400">如果启用，则 SMB 客户端将允许不安全的来宾登录。</span><span class="sxs-lookup"><span data-stu-id="6b27b-400">If enabled,the SMB client will allow insecure guest logons.</span></span> <span data-ttu-id="6b27b-401">如果未配置，SMB 客户端将拒绝不安全的来宾登录。</span><span class="sxs-lookup"><span data-stu-id="6b27b-401">If not configured, the SMB client will reject insecure guest logons.</span></span>|
|<span data-ttu-id="6b27b-402">localSecurityOptionsClearVirtualMemoryPageFile</span><span class="sxs-lookup"><span data-stu-id="6b27b-402">localSecurityOptionsClearVirtualMemoryPageFile</span></span>|<span data-ttu-id="6b27b-403">Boolean</span><span class="sxs-lookup"><span data-stu-id="6b27b-403">Boolean</span></span>|<span data-ttu-id="6b27b-404">此安全设置确定系统关闭时是否清除虚拟内存页面文件。</span><span class="sxs-lookup"><span data-stu-id="6b27b-404">This security setting determines whether the virtual memory pagefile is cleared when the system is shut down.</span></span>|
|<span data-ttu-id="6b27b-405">localSecurityOptionsAllowSystemToBeShutDownWithoutHavingToLogOn</span><span class="sxs-lookup"><span data-stu-id="6b27b-405">localSecurityOptionsAllowSystemToBeShutDownWithoutHavingToLogOn</span></span>|<span data-ttu-id="6b27b-406">Boolean</span><span class="sxs-lookup"><span data-stu-id="6b27b-406">Boolean</span></span>|<span data-ttu-id="6b27b-407">此安全设置确定是否可以关闭计算机而无需登录到 Windows。</span><span class="sxs-lookup"><span data-stu-id="6b27b-407">This security setting determines whether a computer can be shut down without having to log on to Windows.</span></span>|
|<span data-ttu-id="6b27b-408">localSecurityOptionsAllowUIAccessApplicationElevation</span><span class="sxs-lookup"><span data-stu-id="6b27b-408">localSecurityOptionsAllowUIAccessApplicationElevation</span></span>|<span data-ttu-id="6b27b-409">Boolean</span><span class="sxs-lookup"><span data-stu-id="6b27b-409">Boolean</span></span>|<span data-ttu-id="6b27b-410">允许 UIAccess 应用程序无需使用安全桌面提示提升。</span><span class="sxs-lookup"><span data-stu-id="6b27b-410">Allow UIAccess apps to prompt for elevation without using the secure desktop.</span></span>|
|<span data-ttu-id="6b27b-411">localSecurityOptionsVirtualizeFileAndRegistryWriteFailuresToPerUserLocations</span><span class="sxs-lookup"><span data-stu-id="6b27b-411">localSecurityOptionsVirtualizeFileAndRegistryWriteFailuresToPerUserLocations</span></span>|<span data-ttu-id="6b27b-412">Boolean</span><span class="sxs-lookup"><span data-stu-id="6b27b-412">Boolean</span></span>|<span data-ttu-id="6b27b-413">虚拟化文件和注册表写入失败次数为每用户位置</span><span class="sxs-lookup"><span data-stu-id="6b27b-413">Virtualize file and registry write failures to per user locations</span></span>|
|<span data-ttu-id="6b27b-414">localSecurityOptionsOnlyElevateSignedExecutables</span><span class="sxs-lookup"><span data-stu-id="6b27b-414">localSecurityOptionsOnlyElevateSignedExecutables</span></span>|<span data-ttu-id="6b27b-415">Boolean</span><span class="sxs-lookup"><span data-stu-id="6b27b-415">Boolean</span></span>|<span data-ttu-id="6b27b-416">允许运行之前，强制实施 PKI 证书路径验证给定的可执行文件。</span><span class="sxs-lookup"><span data-stu-id="6b27b-416">Enforce PKI certification path validation for a given executable file before it is permitted to run.</span></span>|
|<span data-ttu-id="6b27b-417">localSecurityOptionsAdministratorElevationPromptBehavior</span><span class="sxs-lookup"><span data-stu-id="6b27b-417">localSecurityOptionsAdministratorElevationPromptBehavior</span></span>|[<span data-ttu-id="6b27b-418">localSecurityOptionsAdministratorElevationPromptBehaviorType</span><span class="sxs-lookup"><span data-stu-id="6b27b-418">localSecurityOptionsAdministratorElevationPromptBehaviorType</span></span>](../resources/intune-deviceconfig-localsecurityoptionsadministratorelevationpromptbehaviortype.md)|<span data-ttu-id="6b27b-419">管理员批准模式中定义管理员的提升提示的行为。</span><span class="sxs-lookup"><span data-stu-id="6b27b-419">Define the behavior of the elevation prompt for admins in Admin Approval Mode.</span></span> <span data-ttu-id="6b27b-420">可取值为：`notConfigured`、`elevateWithoutPrompting`、`promptForCredentialsOnTheSecureDesktop`、`promptForConsentOnTheSecureDesktop`、`promptForCredentials`、`promptForConsent`、`promptForConsentForNonWindowsBinaries`。</span><span class="sxs-lookup"><span data-stu-id="6b27b-420">Possible values are: `notConfigured`, `elevateWithoutPrompting`, `promptForCredentialsOnTheSecureDesktop`, `promptForConsentOnTheSecureDesktop`, `promptForCredentials`, `promptForConsent`, `promptForConsentForNonWindowsBinaries`.</span></span>|
|<span data-ttu-id="6b27b-421">localSecurityOptionsStandardUserElevationPromptBehavior</span><span class="sxs-lookup"><span data-stu-id="6b27b-421">localSecurityOptionsStandardUserElevationPromptBehavior</span></span>|[<span data-ttu-id="6b27b-422">localSecurityOptionsStandardUserElevationPromptBehaviorType</span><span class="sxs-lookup"><span data-stu-id="6b27b-422">localSecurityOptionsStandardUserElevationPromptBehaviorType</span></span>](../resources/intune-deviceconfig-localsecurityoptionsstandarduserelevationpromptbehaviortype.md)|<span data-ttu-id="6b27b-423">定义标准用户的提升提示的行为。</span><span class="sxs-lookup"><span data-stu-id="6b27b-423">Define the behavior of the elevation prompt for standard users.</span></span> <span data-ttu-id="6b27b-424">可取值为：`notConfigured`、`automaticallyDenyElevationRequests`、`promptForCredentialsOnTheSecureDesktop`、`promptForCredentials`。</span><span class="sxs-lookup"><span data-stu-id="6b27b-424">Possible values are: `notConfigured`, `automaticallyDenyElevationRequests`, `promptForCredentialsOnTheSecureDesktop`, `promptForCredentials`.</span></span>|
|<span data-ttu-id="6b27b-425">localSecurityOptionsSwitchToSecureDesktopWhenPromptingForElevation</span><span class="sxs-lookup"><span data-stu-id="6b27b-425">localSecurityOptionsSwitchToSecureDesktopWhenPromptingForElevation</span></span>|<span data-ttu-id="6b27b-426">Boolean</span><span class="sxs-lookup"><span data-stu-id="6b27b-426">Boolean</span></span>|<span data-ttu-id="6b27b-427">启用所有提升请求，以转到交互式用户的桌面，而不是安全的桌面。</span><span class="sxs-lookup"><span data-stu-id="6b27b-427">Enable all elevation requests to go to the interactive user's desktop rather than the secure desktop.</span></span> <span data-ttu-id="6b27b-428">使用提示行为 admins 和标准用户的策略设置。</span><span class="sxs-lookup"><span data-stu-id="6b27b-428">Prompt behavior policy settings for admins and standard users are used.</span></span>|
|<span data-ttu-id="6b27b-429">localSecurityOptionsDetectApplicationInstallationsAndPromptForElevation</span><span class="sxs-lookup"><span data-stu-id="6b27b-429">localSecurityOptionsDetectApplicationInstallationsAndPromptForElevation</span></span>|<span data-ttu-id="6b27b-430">Boolean</span><span class="sxs-lookup"><span data-stu-id="6b27b-430">Boolean</span></span>|<span data-ttu-id="6b27b-431">需要提升的权限的应用程序安装将会进行提示管理员凭据。将启用默认值</span><span class="sxs-lookup"><span data-stu-id="6b27b-431">App installations requiring elevated privileges will prompt for admin credentials.Default is enabled</span></span>|
|<span data-ttu-id="6b27b-432">localSecurityOptionsAllowUIAccessApplicationsForSecureLocations</span><span class="sxs-lookup"><span data-stu-id="6b27b-432">localSecurityOptionsAllowUIAccessApplicationsForSecureLocations</span></span>|<span data-ttu-id="6b27b-433">Boolean</span><span class="sxs-lookup"><span data-stu-id="6b27b-433">Boolean</span></span>|<span data-ttu-id="6b27b-434">允许 UIAccess 应用程序无需使用安全桌面提示提升。将启用默认值</span><span class="sxs-lookup"><span data-stu-id="6b27b-434">Allow UIAccess apps to prompt for elevation without using the secure desktop.Default is enabled</span></span>|
|<span data-ttu-id="6b27b-435">localSecurityOptionsUseAdminApprovalMode</span><span class="sxs-lookup"><span data-stu-id="6b27b-435">localSecurityOptionsUseAdminApprovalMode</span></span>|<span data-ttu-id="6b27b-436">Boolean</span><span class="sxs-lookup"><span data-stu-id="6b27b-436">Boolean</span></span>|<span data-ttu-id="6b27b-437">定义的内置的管理帐户使用管理员批准模式还是具有完整的管理员权限运行所有应用程序。将启用默认值</span><span class="sxs-lookup"><span data-stu-id="6b27b-437">Defines whether the built-in admin account uses Admin Approval Mode or runs all apps with full admin privileges.Default is enabled</span></span>|
|<span data-ttu-id="6b27b-438">localSecurityOptionsUseAdminApprovalModeForAdministrators</span><span class="sxs-lookup"><span data-stu-id="6b27b-438">localSecurityOptionsUseAdminApprovalModeForAdministrators</span></span>|<span data-ttu-id="6b27b-439">Boolean</span><span class="sxs-lookup"><span data-stu-id="6b27b-439">Boolean</span></span>|<span data-ttu-id="6b27b-440">定义是否启用管理员批准模式和所有 UAC 策略设置，将启用默认值</span><span class="sxs-lookup"><span data-stu-id="6b27b-440">Define whether Admin Approval Mode and all UAC policy settings are enabled, default is enabled</span></span>|
|<span data-ttu-id="6b27b-441">localSecurityOptionsInformationShownOnLockScreen</span><span class="sxs-lookup"><span data-stu-id="6b27b-441">localSecurityOptionsInformationShownOnLockScreen</span></span>|[<span data-ttu-id="6b27b-442">localSecurityOptionsInformationShownOnLockScreenType</span><span class="sxs-lookup"><span data-stu-id="6b27b-442">localSecurityOptionsInformationShownOnLockScreenType</span></span>](../resources/intune-deviceconfig-localsecurityoptionsinformationshownonlockscreentype.md)|<span data-ttu-id="6b27b-443">配置会话已被锁定时显示的用户信息。</span><span class="sxs-lookup"><span data-stu-id="6b27b-443">Configure the user information that is displayed when the session is locked.</span></span> <span data-ttu-id="6b27b-444">如果未配置，将显示用户的显示名称、 域和用户名。</span><span class="sxs-lookup"><span data-stu-id="6b27b-444">If not configured, user display name, domain and username are shown.</span></span> <span data-ttu-id="6b27b-445">可取值为：`notConfigured`、`userDisplayNameDomainUser`、`userDisplayNameOnly`、`doNotDisplayUser`。</span><span class="sxs-lookup"><span data-stu-id="6b27b-445">Possible values are: `notConfigured`, `userDisplayNameDomainUser`, `userDisplayNameOnly`, `doNotDisplayUser`.</span></span>|
|<span data-ttu-id="6b27b-446">localSecurityOptionsInformationDisplayedOnLockScreen</span><span class="sxs-lookup"><span data-stu-id="6b27b-446">localSecurityOptionsInformationDisplayedOnLockScreen</span></span>|[<span data-ttu-id="6b27b-447">localSecurityOptionsInformationDisplayedOnLockScreenType</span><span class="sxs-lookup"><span data-stu-id="6b27b-447">localSecurityOptionsInformationDisplayedOnLockScreenType</span></span>](../resources/intune-deviceconfig-localsecurityoptionsinformationdisplayedonlockscreentype.md)|<span data-ttu-id="6b27b-448">配置会话已被锁定时显示的用户信息。</span><span class="sxs-lookup"><span data-stu-id="6b27b-448">Configure the user information that is displayed when the session is locked.</span></span> <span data-ttu-id="6b27b-449">如果未配置，将显示用户的显示名称、 域和用户名。</span><span class="sxs-lookup"><span data-stu-id="6b27b-449">If not configured, user display name, domain and username are shown.</span></span> <span data-ttu-id="6b27b-450">可取值为：`notConfigured`、`administrators`、`administratorsAndPowerUsers`、`administratorsAndInteractiveUsers`。</span><span class="sxs-lookup"><span data-stu-id="6b27b-450">Possible values are: `notConfigured`, `administrators`, `administratorsAndPowerUsers`, `administratorsAndInteractiveUsers`.</span></span>|
|<span data-ttu-id="6b27b-451">localSecurityOptionsDisableClientDigitallySignCommunicationsIfServerAgrees</span><span class="sxs-lookup"><span data-stu-id="6b27b-451">localSecurityOptionsDisableClientDigitallySignCommunicationsIfServerAgrees</span></span>|<span data-ttu-id="6b27b-452">Boolean</span><span class="sxs-lookup"><span data-stu-id="6b27b-452">Boolean</span></span>|<span data-ttu-id="6b27b-453">此安全设置确定是否 SMB 客户端尝试协商 SMB 数据包签名。</span><span class="sxs-lookup"><span data-stu-id="6b27b-453">This security setting determines whether the SMB client attempts to negotiate SMB packet signing.</span></span>|
|<span data-ttu-id="6b27b-454">localSecurityOptionsClientDigitallySignCommunicationsAlways</span><span class="sxs-lookup"><span data-stu-id="6b27b-454">localSecurityOptionsClientDigitallySignCommunicationsAlways</span></span>|<span data-ttu-id="6b27b-455">Boolean</span><span class="sxs-lookup"><span data-stu-id="6b27b-455">Boolean</span></span>|<span data-ttu-id="6b27b-456">此安全设置确定是否数据包签名所需 SMB 客户端组件。</span><span class="sxs-lookup"><span data-stu-id="6b27b-456">This security setting determines whether packet signing is required by the SMB client component.</span></span>|
|<span data-ttu-id="6b27b-457">localSecurityOptionsClientSendUnencryptedPasswordToThirdPartySMBServers</span><span class="sxs-lookup"><span data-stu-id="6b27b-457">localSecurityOptionsClientSendUnencryptedPasswordToThirdPartySMBServers</span></span>|<span data-ttu-id="6b27b-458">Boolean</span><span class="sxs-lookup"><span data-stu-id="6b27b-458">Boolean</span></span>|<span data-ttu-id="6b27b-459">如果启用此安全设置，则允许服务器消息块 (SMB) 重定向到不支持期间身份验证的密码加密的非 Microsoft SMB 服务器发送纯文本密码。</span><span class="sxs-lookup"><span data-stu-id="6b27b-459">If this security setting is enabled, the Server Message Block (SMB) redirector is allowed to send plaintext passwords to non-Microsoft SMB servers that do not support password encryption during authentication.</span></span>|
|<span data-ttu-id="6b27b-460">localSecurityOptionsDisableServerDigitallySignCommunicationsAlways</span><span class="sxs-lookup"><span data-stu-id="6b27b-460">localSecurityOptionsDisableServerDigitallySignCommunicationsAlways</span></span>|<span data-ttu-id="6b27b-461">Boolean</span><span class="sxs-lookup"><span data-stu-id="6b27b-461">Boolean</span></span>|<span data-ttu-id="6b27b-462">此安全设置确定是否由 SMB 服务器组件要求签名数据包。</span><span class="sxs-lookup"><span data-stu-id="6b27b-462">This security setting determines whether packet signing is required by the SMB server component.</span></span>|
|<span data-ttu-id="6b27b-463">localSecurityOptionsDisableServerDigitallySignCommunicationsIfClientAgrees</span><span class="sxs-lookup"><span data-stu-id="6b27b-463">localSecurityOptionsDisableServerDigitallySignCommunicationsIfClientAgrees</span></span>|<span data-ttu-id="6b27b-464">Boolean</span><span class="sxs-lookup"><span data-stu-id="6b27b-464">Boolean</span></span>|<span data-ttu-id="6b27b-465">此安全设置确定 SMB 服务器是否协商 SMB 数据包签名与请求的客户端。</span><span class="sxs-lookup"><span data-stu-id="6b27b-465">This security setting determines whether the SMB server will negotiate SMB packet signing with clients that request it.</span></span>|
|<span data-ttu-id="6b27b-466">localSecurityOptionsRestrictAnonymousAccessToNamedPipesAndShares</span><span class="sxs-lookup"><span data-stu-id="6b27b-466">localSecurityOptionsRestrictAnonymousAccessToNamedPipesAndShares</span></span>|<span data-ttu-id="6b27b-467">Boolean</span><span class="sxs-lookup"><span data-stu-id="6b27b-467">Boolean</span></span>|<span data-ttu-id="6b27b-468">默认情况下，此安全设置将匿名访问限制为共享和管道的可匿名访问的命名的管道和可匿名访问的共享的设置</span><span class="sxs-lookup"><span data-stu-id="6b27b-468">By default, this security setting restricts anonymous access to shares and pipes to the settings for named pipes that can be accessed anonymously and Shares that can be accessed anonymously</span></span>|
|<span data-ttu-id="6b27b-469">localSecurityOptionsDoNotAllowAnonymousEnumerationOfSAMAccounts</span><span class="sxs-lookup"><span data-stu-id="6b27b-469">localSecurityOptionsDoNotAllowAnonymousEnumerationOfSAMAccounts</span></span>|<span data-ttu-id="6b27b-470">Boolean</span><span class="sxs-lookup"><span data-stu-id="6b27b-470">Boolean</span></span>|<span data-ttu-id="6b27b-471">此安全设置确定将对匿名连接到计算机上授予其他权限。</span><span class="sxs-lookup"><span data-stu-id="6b27b-471">This security setting determines what additional permissions will be granted for anonymous connections to the computer.</span></span>|
|<span data-ttu-id="6b27b-472">localSecurityOptionsAllowAnonymousEnumerationOfSAMAccountsAndShares</span><span class="sxs-lookup"><span data-stu-id="6b27b-472">localSecurityOptionsAllowAnonymousEnumerationOfSAMAccountsAndShares</span></span>|<span data-ttu-id="6b27b-473">Boolean</span><span class="sxs-lookup"><span data-stu-id="6b27b-473">Boolean</span></span>|<span data-ttu-id="6b27b-474">此安全设置确定是否允许匿名用户执行某些活动，如枚举的域帐户和网络共享名称。</span><span class="sxs-lookup"><span data-stu-id="6b27b-474">This security setting determines whether to allows anonymous users to perform certain activities, such as enumerating the names of domain accounts and network shares.</span></span>|
|<span data-ttu-id="6b27b-475">localSecurityOptionsDoNotStoreLANManagerHashValueOnNextPasswordChange</span><span class="sxs-lookup"><span data-stu-id="6b27b-475">localSecurityOptionsDoNotStoreLANManagerHashValueOnNextPasswordChange</span></span>|<span data-ttu-id="6b27b-476">Boolean</span><span class="sxs-lookup"><span data-stu-id="6b27b-476">Boolean</span></span>|<span data-ttu-id="6b27b-477">此安全设置确定，是否在下次密码更改，存储新密码的 LAN Manager (LM) 哈希值。</span><span class="sxs-lookup"><span data-stu-id="6b27b-477">This security setting determines if, at the next password change, the LAN Manager (LM) hash value for the new password is stored.</span></span> <span data-ttu-id="6b27b-478">默认情况下，它不存储。</span><span class="sxs-lookup"><span data-stu-id="6b27b-478">It’s not stored by default.</span></span>|
|<span data-ttu-id="6b27b-479">localSecurityOptionsSmartCardRemovalBehavior</span><span class="sxs-lookup"><span data-stu-id="6b27b-479">localSecurityOptionsSmartCardRemovalBehavior</span></span>|[<span data-ttu-id="6b27b-480">localSecurityOptionsSmartCardRemovalBehaviorType</span><span class="sxs-lookup"><span data-stu-id="6b27b-480">localSecurityOptionsSmartCardRemovalBehaviorType</span></span>](../resources/intune-deviceconfig-localsecurityoptionssmartcardremovalbehaviortype.md)|<span data-ttu-id="6b27b-481">此安全设置确定智能卡读卡器从移除智能卡登录的用户时，会发生什么情况。</span><span class="sxs-lookup"><span data-stu-id="6b27b-481">This security setting determines what happens when the smart card for a logged-on user is removed from the smart card reader.</span></span> <span data-ttu-id="6b27b-482">可取值为：`lockWorkstation`、`noAction`、`forceLogoff`、`disconnectRemoteDesktopSession`。</span><span class="sxs-lookup"><span data-stu-id="6b27b-482">Possible values are: `lockWorkstation`, `noAction`, `forceLogoff`, `disconnectRemoteDesktopSession`.</span></span>|
|<span data-ttu-id="6b27b-483">defenderSecurityCenterDisableAppBrowserUI</span><span class="sxs-lookup"><span data-stu-id="6b27b-483">defenderSecurityCenterDisableAppBrowserUI</span></span>|<span data-ttu-id="6b27b-484">Boolean</span><span class="sxs-lookup"><span data-stu-id="6b27b-484">Boolean</span></span>|<span data-ttu-id="6b27b-485">用于禁用的应用程序和浏览器的保护区域显示。</span><span class="sxs-lookup"><span data-stu-id="6b27b-485">Used to disable the display of the app and browser protection area.</span></span>|
|<span data-ttu-id="6b27b-486">defenderSecurityCenterDisableFamilyUI</span><span class="sxs-lookup"><span data-stu-id="6b27b-486">defenderSecurityCenterDisableFamilyUI</span></span>|<span data-ttu-id="6b27b-487">Boolean</span><span class="sxs-lookup"><span data-stu-id="6b27b-487">Boolean</span></span>|<span data-ttu-id="6b27b-488">用于禁用系列选项区域的显示。</span><span class="sxs-lookup"><span data-stu-id="6b27b-488">Used to disable the display of the family options area.</span></span>|
|<span data-ttu-id="6b27b-489">defenderSecurityCenterDisableHealthUI</span><span class="sxs-lookup"><span data-stu-id="6b27b-489">defenderSecurityCenterDisableHealthUI</span></span>|<span data-ttu-id="6b27b-490">Boolean</span><span class="sxs-lookup"><span data-stu-id="6b27b-490">Boolean</span></span>|<span data-ttu-id="6b27b-491">用于禁用设备性能和运行状况区域的显示。</span><span class="sxs-lookup"><span data-stu-id="6b27b-491">Used to disable the display of the device performance and health area.</span></span>|
|<span data-ttu-id="6b27b-492">defenderSecurityCenterDisableNetworkUI</span><span class="sxs-lookup"><span data-stu-id="6b27b-492">defenderSecurityCenterDisableNetworkUI</span></span>|<span data-ttu-id="6b27b-493">Boolean</span><span class="sxs-lookup"><span data-stu-id="6b27b-493">Boolean</span></span>|<span data-ttu-id="6b27b-494">用于禁用防火墙和网络保护区域的显示。</span><span class="sxs-lookup"><span data-stu-id="6b27b-494">Used to disable the display of the firewall and network protection area.</span></span>|
|<span data-ttu-id="6b27b-495">defenderSecurityCenterDisableVirusUI</span><span class="sxs-lookup"><span data-stu-id="6b27b-495">defenderSecurityCenterDisableVirusUI</span></span>|<span data-ttu-id="6b27b-496">Boolean</span><span class="sxs-lookup"><span data-stu-id="6b27b-496">Boolean</span></span>|<span data-ttu-id="6b27b-497">用于禁用病毒和威胁保护区域的显示。</span><span class="sxs-lookup"><span data-stu-id="6b27b-497">Used to disable the display of the virus and threat protection area.</span></span>|
|<span data-ttu-id="6b27b-498">defenderSecurityCenterDisableAccountUI</span><span class="sxs-lookup"><span data-stu-id="6b27b-498">defenderSecurityCenterDisableAccountUI</span></span>|<span data-ttu-id="6b27b-499">Boolean</span><span class="sxs-lookup"><span data-stu-id="6b27b-499">Boolean</span></span>|<span data-ttu-id="6b27b-500">用于禁用帐户保护区域的显示。</span><span class="sxs-lookup"><span data-stu-id="6b27b-500">Used to disable the display of the account protection area.</span></span>|
|<span data-ttu-id="6b27b-501">defenderSecurityCenterDisableHardwareUI</span><span class="sxs-lookup"><span data-stu-id="6b27b-501">defenderSecurityCenterDisableHardwareUI</span></span>|<span data-ttu-id="6b27b-502">Boolean</span><span class="sxs-lookup"><span data-stu-id="6b27b-502">Boolean</span></span>|<span data-ttu-id="6b27b-503">用于禁用硬件保护区域的显示。</span><span class="sxs-lookup"><span data-stu-id="6b27b-503">Used to disable the display of the hardware protection area.</span></span>|
|<span data-ttu-id="6b27b-504">defenderSecurityCenterDisableRansomwareUI</span><span class="sxs-lookup"><span data-stu-id="6b27b-504">defenderSecurityCenterDisableRansomwareUI</span></span>|<span data-ttu-id="6b27b-505">Boolean</span><span class="sxs-lookup"><span data-stu-id="6b27b-505">Boolean</span></span>|<span data-ttu-id="6b27b-506">用于禁用勒索软件保护区域的显示。</span><span class="sxs-lookup"><span data-stu-id="6b27b-506">Used to disable the display of the ransomware protection area.</span></span> |
|<span data-ttu-id="6b27b-507">defenderSecurityCenterDisableSecureBootUI</span><span class="sxs-lookup"><span data-stu-id="6b27b-507">defenderSecurityCenterDisableSecureBootUI</span></span>|<span data-ttu-id="6b27b-508">Boolean</span><span class="sxs-lookup"><span data-stu-id="6b27b-508">Boolean</span></span>|<span data-ttu-id="6b27b-509">用于禁用的设备安全下的安全启动区域显示。</span><span class="sxs-lookup"><span data-stu-id="6b27b-509">Used to disable the display of the secure boot area under Device security.</span></span>|
|<span data-ttu-id="6b27b-510">defenderSecurityCenterDisableTroubleshootingUI</span><span class="sxs-lookup"><span data-stu-id="6b27b-510">defenderSecurityCenterDisableTroubleshootingUI</span></span>|<span data-ttu-id="6b27b-511">Boolean</span><span class="sxs-lookup"><span data-stu-id="6b27b-511">Boolean</span></span>|<span data-ttu-id="6b27b-512">用于禁用安全过程下设备安全疑难解答的显示。</span><span class="sxs-lookup"><span data-stu-id="6b27b-512">Used to disable the display of the security process troubleshooting under Device security.</span></span>|
|<span data-ttu-id="6b27b-513">defenderSecurityCenterOrganizationDisplayName</span><span class="sxs-lookup"><span data-stu-id="6b27b-513">defenderSecurityCenterOrganizationDisplayName</span></span>|<span data-ttu-id="6b27b-514">String</span><span class="sxs-lookup"><span data-stu-id="6b27b-514">String</span></span>|<span data-ttu-id="6b27b-515">向用户显示公司名称。</span><span class="sxs-lookup"><span data-stu-id="6b27b-515">The company name that is displayed to the users.</span></span>|
|<span data-ttu-id="6b27b-516">defenderSecurityCenterHelpEmail</span><span class="sxs-lookup"><span data-stu-id="6b27b-516">defenderSecurityCenterHelpEmail</span></span>|<span data-ttu-id="6b27b-517">String</span><span class="sxs-lookup"><span data-stu-id="6b27b-517">String</span></span>|<span data-ttu-id="6b27b-518">向用户显示的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="6b27b-518">The email address that is displayed to users.</span></span>|
|<span data-ttu-id="6b27b-519">defenderSecurityCenterHelpPhone</span><span class="sxs-lookup"><span data-stu-id="6b27b-519">defenderSecurityCenterHelpPhone</span></span>|<span data-ttu-id="6b27b-520">String</span><span class="sxs-lookup"><span data-stu-id="6b27b-520">String</span></span>|<span data-ttu-id="6b27b-521">电话号码或向用户显示的 Skype ID 中。</span><span class="sxs-lookup"><span data-stu-id="6b27b-521">The phone number or Skype ID that is displayed to users.</span></span>|
|<span data-ttu-id="6b27b-522">defenderSecurityCenterHelpURL</span><span class="sxs-lookup"><span data-stu-id="6b27b-522">defenderSecurityCenterHelpURL</span></span>|<span data-ttu-id="6b27b-523">String</span><span class="sxs-lookup"><span data-stu-id="6b27b-523">String</span></span>|<span data-ttu-id="6b27b-524">帮助门户这向用户显示的 URL。</span><span class="sxs-lookup"><span data-stu-id="6b27b-524">The help portal URL this is displayed to users.</span></span>|
|<span data-ttu-id="6b27b-525">defenderSecurityCenterNotificationsFromApp</span><span class="sxs-lookup"><span data-stu-id="6b27b-525">defenderSecurityCenterNotificationsFromApp</span></span>|[<span data-ttu-id="6b27b-526">defenderSecurityCenterNotificationsFromAppType</span><span class="sxs-lookup"><span data-stu-id="6b27b-526">defenderSecurityCenterNotificationsFromAppType</span></span>](../resources/intune-deviceconfig-defendersecuritycenternotificationsfromapptype.md)|<span data-ttu-id="6b27b-527">若要从应用程序的显示区域显示的通知。</span><span class="sxs-lookup"><span data-stu-id="6b27b-527">Notifications to show from the displayed areas of app.</span></span> <span data-ttu-id="6b27b-528">可取值为：`notConfigured`、`blockNoncriticalNotifications`、`blockAllNotifications`。</span><span class="sxs-lookup"><span data-stu-id="6b27b-528">Possible values are: `notConfigured`, `blockNoncriticalNotifications`, `blockAllNotifications`.</span></span>|
|<span data-ttu-id="6b27b-529">defenderSecurityCenterITContactDisplay</span><span class="sxs-lookup"><span data-stu-id="6b27b-529">defenderSecurityCenterITContactDisplay</span></span>|[<span data-ttu-id="6b27b-530">defenderSecurityCenterITContactDisplayType</span><span class="sxs-lookup"><span data-stu-id="6b27b-530">defenderSecurityCenterITContactDisplayType</span></span>](../resources/intune-deviceconfig-defendersecuritycenteritcontactdisplaytype.md)|<span data-ttu-id="6b27b-531">配置显示 IT 联系人位置向最终用户的信息。</span><span class="sxs-lookup"><span data-stu-id="6b27b-531">Configure where to display IT contact information to end users.</span></span> <span data-ttu-id="6b27b-532">可取值为：`notConfigured`、`displayInAppAndInNotifications`、`displayOnlyInApp`、`displayOnlyInNotifications`。</span><span class="sxs-lookup"><span data-stu-id="6b27b-532">Possible values are: `notConfigured`, `displayInAppAndInNotifications`, `displayOnlyInApp`, `displayOnlyInNotifications`.</span></span>|
|<span data-ttu-id="6b27b-533">firewallBlockStatefulFTP</span><span class="sxs-lookup"><span data-stu-id="6b27b-533">firewallBlockStatefulFTP</span></span>|<span data-ttu-id="6b27b-534">Boolean</span><span class="sxs-lookup"><span data-stu-id="6b27b-534">Boolean</span></span>|<span data-ttu-id="6b27b-535">阻止到设备的有状态 FTP 连接</span><span class="sxs-lookup"><span data-stu-id="6b27b-535">Blocks stateful FTP connections to the device</span></span>|
|<span data-ttu-id="6b27b-536">firewallIdleTimeoutForSecurityAssociationInSeconds</span><span class="sxs-lookup"><span data-stu-id="6b27b-536">firewallIdleTimeoutForSecurityAssociationInSeconds</span></span>|<span data-ttu-id="6b27b-537">Int32</span><span class="sxs-lookup"><span data-stu-id="6b27b-537">Int32</span></span>|<span data-ttu-id="6b27b-538">配置安全关联的空闲超时（以秒为单位），值范围为 300 到 3600（包括这两个值）。</span><span class="sxs-lookup"><span data-stu-id="6b27b-538">Configures the idle timeout for security associations, in seconds, from 300 to 3600 inclusive.</span></span> <span data-ttu-id="6b27b-539">这是一个时间段，在此之后安全关联将过期并被删除。</span><span class="sxs-lookup"><span data-stu-id="6b27b-539">This is the period after which security associations will expire and be deleted.</span></span> <span data-ttu-id="6b27b-540">有效值为 300 至 3600。</span><span class="sxs-lookup"><span data-stu-id="6b27b-540">Valid values 300 to 3600</span></span>|
|<span data-ttu-id="6b27b-541">firewallPreSharedKeyEncodingMethod</span><span class="sxs-lookup"><span data-stu-id="6b27b-541">firewallPreSharedKeyEncodingMethod</span></span>|[<span data-ttu-id="6b27b-542">firewallPreSharedKeyEncodingMethodType</span><span class="sxs-lookup"><span data-stu-id="6b27b-542">firewallPreSharedKeyEncodingMethodType</span></span>](../resources/intune-deviceconfig-firewallpresharedkeyencodingmethodtype.md)|<span data-ttu-id="6b27b-543">选择要使用编码的预共享的键。</span><span class="sxs-lookup"><span data-stu-id="6b27b-543">Select the preshared key encoding to be used.</span></span> <span data-ttu-id="6b27b-544">可取值为：`deviceDefault`、`none`、`utF8`。</span><span class="sxs-lookup"><span data-stu-id="6b27b-544">Possible values are: `deviceDefault`, `none`, `utF8`.</span></span>|
|<span data-ttu-id="6b27b-545">firewallIPSecExemptionsAllowNeighborDiscovery</span><span class="sxs-lookup"><span data-stu-id="6b27b-545">firewallIPSecExemptionsAllowNeighborDiscovery</span></span>|<span data-ttu-id="6b27b-546">Boolean</span><span class="sxs-lookup"><span data-stu-id="6b27b-546">Boolean</span></span>|<span data-ttu-id="6b27b-547">配置 IPSec 免除项以允许邻居发现 IPv6 ICMP 类型代码</span><span class="sxs-lookup"><span data-stu-id="6b27b-547">Configures IPSec exemptions to allow neighbor discovery IPv6 ICMP type-codes</span></span>|
|<span data-ttu-id="6b27b-548">firewallIPSecExemptionsAllowICMP</span><span class="sxs-lookup"><span data-stu-id="6b27b-548">firewallIPSecExemptionsAllowICMP</span></span>|<span data-ttu-id="6b27b-549">Boolean</span><span class="sxs-lookup"><span data-stu-id="6b27b-549">Boolean</span></span>|<span data-ttu-id="6b27b-550">配置 IPSec 免除项以允许 ICMP</span><span class="sxs-lookup"><span data-stu-id="6b27b-550">Configures IPSec exemptions to allow ICMP</span></span>|
|<span data-ttu-id="6b27b-551">firewallIPSecExemptionsAllowRouterDiscovery</span><span class="sxs-lookup"><span data-stu-id="6b27b-551">firewallIPSecExemptionsAllowRouterDiscovery</span></span>|<span data-ttu-id="6b27b-552">Boolean</span><span class="sxs-lookup"><span data-stu-id="6b27b-552">Boolean</span></span>|<span data-ttu-id="6b27b-553">配置 IPSec 免除项以允许路由器发现 IPv6 ICMP 类型代码</span><span class="sxs-lookup"><span data-stu-id="6b27b-553">Configures IPSec exemptions to allow router discovery IPv6 ICMP type-codes</span></span>|
|<span data-ttu-id="6b27b-554">firewallIPSecExemptionsAllowDHCP</span><span class="sxs-lookup"><span data-stu-id="6b27b-554">firewallIPSecExemptionsAllowDHCP</span></span>|<span data-ttu-id="6b27b-555">Boolean</span><span class="sxs-lookup"><span data-stu-id="6b27b-555">Boolean</span></span>|<span data-ttu-id="6b27b-556">配置 IPSec 免除项以允许 IPv4 和 IPv6 DHCP 通信</span><span class="sxs-lookup"><span data-stu-id="6b27b-556">Configures IPSec exemptions to allow both IPv4 and IPv6 DHCP traffic</span></span>|
|<span data-ttu-id="6b27b-557">firewallCertificateRevocationListCheckMethod</span><span class="sxs-lookup"><span data-stu-id="6b27b-557">firewallCertificateRevocationListCheckMethod</span></span>|[<span data-ttu-id="6b27b-558">firewallCertificateRevocationListCheckMethodType</span><span class="sxs-lookup"><span data-stu-id="6b27b-558">firewallCertificateRevocationListCheckMethodType</span></span>](../resources/intune-deviceconfig-firewallcertificaterevocationlistcheckmethodtype.md)|<span data-ttu-id="6b27b-559">指定如何强制实施证书吊销列表。</span><span class="sxs-lookup"><span data-stu-id="6b27b-559">Specify how the certificate revocation list is to be enforced.</span></span> <span data-ttu-id="6b27b-560">可取值为：`deviceDefault`、`none`、`attempt`、`require`。</span><span class="sxs-lookup"><span data-stu-id="6b27b-560">Possible values are: `deviceDefault`, `none`, `attempt`, `require`.</span></span>|
|<span data-ttu-id="6b27b-561">firewallMergeKeyingModuleSettings</span><span class="sxs-lookup"><span data-stu-id="6b27b-561">firewallMergeKeyingModuleSettings</span></span>|<span data-ttu-id="6b27b-562">Boolean</span><span class="sxs-lookup"><span data-stu-id="6b27b-562">Boolean</span></span>|<span data-ttu-id="6b27b-563">如果键控模块不完全支持身份验证集，请指示模块仅忽略不受支持的身份验证套件而不是整个集</span><span class="sxs-lookup"><span data-stu-id="6b27b-563">If an authentication set is not fully supported by a keying module, direct the module to ignore only unsupported authentication suites rather than the entire set</span></span>|
|<span data-ttu-id="6b27b-564">firewallPacketQueueingMethod</span><span class="sxs-lookup"><span data-stu-id="6b27b-564">firewallPacketQueueingMethod</span></span>|[<span data-ttu-id="6b27b-565">firewallPacketQueueingMethodType</span><span class="sxs-lookup"><span data-stu-id="6b27b-565">firewallPacketQueueingMethodType</span></span>](../resources/intune-deviceconfig-firewallpacketqueueingmethodtype.md)|<span data-ttu-id="6b27b-566">配置数据包 queueing 应如何应用隧道网关方案中。</span><span class="sxs-lookup"><span data-stu-id="6b27b-566">Configures how packet queueing should be applied in the tunnel gateway scenario.</span></span> <span data-ttu-id="6b27b-567">可取值为：`deviceDefault`、`disabled`、`queueInbound`、`queueOutbound`、`queueBoth`。</span><span class="sxs-lookup"><span data-stu-id="6b27b-567">Possible values are: `deviceDefault`, `disabled`, `queueInbound`, `queueOutbound`, `queueBoth`.</span></span>|
|<span data-ttu-id="6b27b-568">firewallProfileDomain</span><span class="sxs-lookup"><span data-stu-id="6b27b-568">firewallProfileDomain</span></span>|[<span data-ttu-id="6b27b-569">windowsFirewallNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="6b27b-569">windowsFirewallNetworkProfile</span></span>](../resources/intune-deviceconfig-windowsfirewallnetworkprofile.md)|<span data-ttu-id="6b27b-570">配置域网络的防火墙配置文件设置</span><span class="sxs-lookup"><span data-stu-id="6b27b-570">Configures the firewall profile settings for domain networks</span></span>|
|<span data-ttu-id="6b27b-571">firewallProfilePublic</span><span class="sxs-lookup"><span data-stu-id="6b27b-571">firewallProfilePublic</span></span>|[<span data-ttu-id="6b27b-572">windowsFirewallNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="6b27b-572">windowsFirewallNetworkProfile</span></span>](../resources/intune-deviceconfig-windowsfirewallnetworkprofile.md)|<span data-ttu-id="6b27b-573">配置公用网络的防火墙配置文件设置</span><span class="sxs-lookup"><span data-stu-id="6b27b-573">Configures the firewall profile settings for public networks</span></span>|
|<span data-ttu-id="6b27b-574">firewallProfilePrivate</span><span class="sxs-lookup"><span data-stu-id="6b27b-574">firewallProfilePrivate</span></span>|[<span data-ttu-id="6b27b-575">windowsFirewallNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="6b27b-575">windowsFirewallNetworkProfile</span></span>](../resources/intune-deviceconfig-windowsfirewallnetworkprofile.md)|<span data-ttu-id="6b27b-576">配置专用网络的防火墙配置文件设置</span><span class="sxs-lookup"><span data-stu-id="6b27b-576">Configures the firewall profile settings for private networks</span></span>|
|<span data-ttu-id="6b27b-577">defenderAttackSurfaceReductionExcludedPaths</span><span class="sxs-lookup"><span data-stu-id="6b27b-577">defenderAttackSurfaceReductionExcludedPaths</span></span>|<span data-ttu-id="6b27b-578">String 集合</span><span class="sxs-lookup"><span data-stu-id="6b27b-578">String collection</span></span>|<span data-ttu-id="6b27b-579">要从攻击面减少规则中排除的 exe 文件和文件夹的列表</span><span class="sxs-lookup"><span data-stu-id="6b27b-579">List of exe files and folders to be excluded from attack surface reduction rules</span></span>|
|<span data-ttu-id="6b27b-580">defenderOfficeAppsOtherProcessInjectionType</span><span class="sxs-lookup"><span data-stu-id="6b27b-580">defenderOfficeAppsOtherProcessInjectionType</span></span>|[<span data-ttu-id="6b27b-581">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="6b27b-581">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="6b27b-582">值，指示将到其他进程的 Office 应用程序的行为。</span><span class="sxs-lookup"><span data-stu-id="6b27b-582">Value indicating the behavior of Office applications injecting into other processes.</span></span> <span data-ttu-id="6b27b-583">可取值为：`userDefined`、`block`、`auditMode`。</span><span class="sxs-lookup"><span data-stu-id="6b27b-583">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="6b27b-584">defenderOfficeAppsOtherProcessInjection</span><span class="sxs-lookup"><span data-stu-id="6b27b-584">defenderOfficeAppsOtherProcessInjection</span></span>|[<span data-ttu-id="6b27b-585">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="6b27b-585">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="6b27b-586">值，指示将到其他进程的 Office 应用程序的行为。</span><span class="sxs-lookup"><span data-stu-id="6b27b-586">Value indicating the behavior of  Office applications injecting into other processes.</span></span> <span data-ttu-id="6b27b-587">可取值为：`userDefined`、`enable`、`auditMode`。</span><span class="sxs-lookup"><span data-stu-id="6b27b-587">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="6b27b-588">defenderOfficeAppsExecutableContentCreationOrLaunchType</span><span class="sxs-lookup"><span data-stu-id="6b27b-588">defenderOfficeAppsExecutableContentCreationOrLaunchType</span></span>|[<span data-ttu-id="6b27b-589">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="6b27b-589">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="6b27b-590">指示 Office 应用程序/宏创建或启动可执行文件内容的行为的值。</span><span class="sxs-lookup"><span data-stu-id="6b27b-590">Value indicating the behavior of Office applications/macros creating or launching executable content.</span></span> <span data-ttu-id="6b27b-591">可取值为：`userDefined`、`block`、`auditMode`。</span><span class="sxs-lookup"><span data-stu-id="6b27b-591">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="6b27b-592">defenderOfficeAppsExecutableContentCreationOrLaunch</span><span class="sxs-lookup"><span data-stu-id="6b27b-592">defenderOfficeAppsExecutableContentCreationOrLaunch</span></span>|[<span data-ttu-id="6b27b-593">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="6b27b-593">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="6b27b-594">指示 Office 应用程序/宏创建或启动可执行文件内容的行为的值。</span><span class="sxs-lookup"><span data-stu-id="6b27b-594">Value indicating the behavior of Office applications/macros creating or launching executable content.</span></span> <span data-ttu-id="6b27b-595">可取值为：`userDefined`、`enable`、`auditMode`。</span><span class="sxs-lookup"><span data-stu-id="6b27b-595">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="6b27b-596">defenderOfficeAppsLaunchChildProcessType</span><span class="sxs-lookup"><span data-stu-id="6b27b-596">defenderOfficeAppsLaunchChildProcessType</span></span>|[<span data-ttu-id="6b27b-597">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="6b27b-597">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="6b27b-598">指示启动子进程的 Office 应用程序的行为的值。</span><span class="sxs-lookup"><span data-stu-id="6b27b-598">Value indicating the behavior of Office application launching child processes.</span></span> <span data-ttu-id="6b27b-599">可取值为：`userDefined`、`block`、`auditMode`。</span><span class="sxs-lookup"><span data-stu-id="6b27b-599">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="6b27b-600">defenderOfficeAppsLaunchChildProcess</span><span class="sxs-lookup"><span data-stu-id="6b27b-600">defenderOfficeAppsLaunchChildProcess</span></span>|[<span data-ttu-id="6b27b-601">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="6b27b-601">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="6b27b-602">指示启动子进程的 Office 应用程序的行为的值。</span><span class="sxs-lookup"><span data-stu-id="6b27b-602">Value indicating the behavior of Office application launching child processes.</span></span> <span data-ttu-id="6b27b-603">可取值为：`userDefined`、`enable`、`auditMode`。</span><span class="sxs-lookup"><span data-stu-id="6b27b-603">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="6b27b-604">defenderOfficeMacroCodeAllowWin32ImportsType</span><span class="sxs-lookup"><span data-stu-id="6b27b-604">defenderOfficeMacroCodeAllowWin32ImportsType</span></span>|[<span data-ttu-id="6b27b-605">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="6b27b-605">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="6b27b-606">值，该值指示的 Win32 行为导入从 Office 中的宏代码。</span><span class="sxs-lookup"><span data-stu-id="6b27b-606">Value indicating the behavior of Win32 imports from Macro code in Office.</span></span> <span data-ttu-id="6b27b-607">可取值为：`userDefined`、`block`、`auditMode`。</span><span class="sxs-lookup"><span data-stu-id="6b27b-607">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="6b27b-608">defenderOfficeMacroCodeAllowWin32Imports</span><span class="sxs-lookup"><span data-stu-id="6b27b-608">defenderOfficeMacroCodeAllowWin32Imports</span></span>|[<span data-ttu-id="6b27b-609">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="6b27b-609">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="6b27b-610">值，该值指示的 Win32 行为导入从 Office 中的宏代码。</span><span class="sxs-lookup"><span data-stu-id="6b27b-610">Value indicating the behavior of Win32 imports from Macro code in Office.</span></span> <span data-ttu-id="6b27b-611">可取值为：`userDefined`、`enable`、`auditMode`。</span><span class="sxs-lookup"><span data-stu-id="6b27b-611">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="6b27b-612">defenderScriptObfuscatedMacroCodeType</span><span class="sxs-lookup"><span data-stu-id="6b27b-612">defenderScriptObfuscatedMacroCodeType</span></span>|[<span data-ttu-id="6b27b-613">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="6b27b-613">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="6b27b-614">值，该值指示经过模糊处理 js/vbs/ps/macro 代码的行为。</span><span class="sxs-lookup"><span data-stu-id="6b27b-614">Value indicating the behavior of obfuscated js/vbs/ps/macro code.</span></span> <span data-ttu-id="6b27b-615">可取值为：`userDefined`、`block`、`auditMode`。</span><span class="sxs-lookup"><span data-stu-id="6b27b-615">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="6b27b-616">defenderScriptObfuscatedMacroCode</span><span class="sxs-lookup"><span data-stu-id="6b27b-616">defenderScriptObfuscatedMacroCode</span></span>|[<span data-ttu-id="6b27b-617">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="6b27b-617">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="6b27b-618">值，该值指示经过模糊处理 js/vbs/ps/macro 代码的行为。</span><span class="sxs-lookup"><span data-stu-id="6b27b-618">Value indicating the behavior of obfuscated js/vbs/ps/macro code.</span></span> <span data-ttu-id="6b27b-619">可取值为：`userDefined`、`enable`、`auditMode`。</span><span class="sxs-lookup"><span data-stu-id="6b27b-619">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="6b27b-620">defenderScriptDownloadedPayloadExecutionType</span><span class="sxs-lookup"><span data-stu-id="6b27b-620">defenderScriptDownloadedPayloadExecutionType</span></span>|[<span data-ttu-id="6b27b-621">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="6b27b-621">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="6b27b-622">从 Internet 下载的值，该值指示 js/vbs 执行负载的行为。</span><span class="sxs-lookup"><span data-stu-id="6b27b-622">Value indicating the behavior of js/vbs executing payload downloaded from Internet.</span></span> <span data-ttu-id="6b27b-623">可取值为：`userDefined`、`block`、`auditMode`。</span><span class="sxs-lookup"><span data-stu-id="6b27b-623">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="6b27b-624">defenderScriptDownloadedPayloadExecution</span><span class="sxs-lookup"><span data-stu-id="6b27b-624">defenderScriptDownloadedPayloadExecution</span></span>|[<span data-ttu-id="6b27b-625">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="6b27b-625">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="6b27b-626">从 Internet 下载的值，该值指示 js/vbs 执行负载的行为。</span><span class="sxs-lookup"><span data-stu-id="6b27b-626">Value indicating the behavior of js/vbs executing payload downloaded from Internet.</span></span> <span data-ttu-id="6b27b-627">可取值为：`userDefined`、`enable`、`auditMode`。</span><span class="sxs-lookup"><span data-stu-id="6b27b-627">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="6b27b-628">defenderPreventCredentialStealingType</span><span class="sxs-lookup"><span data-stu-id="6b27b-628">defenderPreventCredentialStealingType</span></span>|[<span data-ttu-id="6b27b-629">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="6b27b-629">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="6b27b-630">值，该值指示是否允许从 Windows 本地安全机构子系统窃取的凭据。</span><span class="sxs-lookup"><span data-stu-id="6b27b-630">Value indicating if credential stealing from the Windows local security authority subsystem is permitted.</span></span> <span data-ttu-id="6b27b-631">可取值为：`userDefined`、`enable`、`auditMode`。</span><span class="sxs-lookup"><span data-stu-id="6b27b-631">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="6b27b-632">defenderProcessCreationType</span><span class="sxs-lookup"><span data-stu-id="6b27b-632">defenderProcessCreationType</span></span>|[<span data-ttu-id="6b27b-633">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="6b27b-633">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="6b27b-634">值，该值指示响应来自 PSExec 和 WMI 命令的过程创建。</span><span class="sxs-lookup"><span data-stu-id="6b27b-634">Value indicating response to process creations originating from PSExec and WMI commands.</span></span> <span data-ttu-id="6b27b-635">可取值为：`userDefined`、`block`、`auditMode`。</span><span class="sxs-lookup"><span data-stu-id="6b27b-635">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="6b27b-636">defenderProcessCreation</span><span class="sxs-lookup"><span data-stu-id="6b27b-636">defenderProcessCreation</span></span>|[<span data-ttu-id="6b27b-637">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="6b27b-637">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="6b27b-638">值，该值指示响应来自 PSExec 和 WMI 命令的过程创建。</span><span class="sxs-lookup"><span data-stu-id="6b27b-638">Value indicating response to process creations originating from PSExec and WMI commands.</span></span> <span data-ttu-id="6b27b-639">可取值为：`userDefined`、`enable`、`auditMode`。</span><span class="sxs-lookup"><span data-stu-id="6b27b-639">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="6b27b-640">defenderUntrustedUSBProcessType</span><span class="sxs-lookup"><span data-stu-id="6b27b-640">defenderUntrustedUSBProcessType</span></span>|[<span data-ttu-id="6b27b-641">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="6b27b-641">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="6b27b-642">值，该值指示从 USB 运行的受信任和无符号流程的响应。</span><span class="sxs-lookup"><span data-stu-id="6b27b-642">Value indicating response to untrusted and unsigned processes that run from USB.</span></span> <span data-ttu-id="6b27b-643">可取值为：`userDefined`、`block`、`auditMode`。</span><span class="sxs-lookup"><span data-stu-id="6b27b-643">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="6b27b-644">defenderUntrustedUSBProcess</span><span class="sxs-lookup"><span data-stu-id="6b27b-644">defenderUntrustedUSBProcess</span></span>|[<span data-ttu-id="6b27b-645">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="6b27b-645">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="6b27b-646">值，该值指示从 USB 运行的受信任和无符号流程的响应。</span><span class="sxs-lookup"><span data-stu-id="6b27b-646">Value indicating response to untrusted and unsigned processes that run from USB.</span></span> <span data-ttu-id="6b27b-647">可取值为：`userDefined`、`enable`、`auditMode`。</span><span class="sxs-lookup"><span data-stu-id="6b27b-647">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="6b27b-648">defenderUntrustedExecutableType</span><span class="sxs-lookup"><span data-stu-id="6b27b-648">defenderUntrustedExecutableType</span></span>|[<span data-ttu-id="6b27b-649">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="6b27b-649">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="6b27b-650">值，该值指示响应可执行文件的传播、 年龄或受信任的列表不满足条件。</span><span class="sxs-lookup"><span data-stu-id="6b27b-650">Value indicating response to executables that don't meet a prevalence, age, or trusted list criteria.</span></span> <span data-ttu-id="6b27b-651">可取值为：`userDefined`、`block`、`auditMode`。</span><span class="sxs-lookup"><span data-stu-id="6b27b-651">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="6b27b-652">defenderUntrustedExecutable</span><span class="sxs-lookup"><span data-stu-id="6b27b-652">defenderUntrustedExecutable</span></span>|[<span data-ttu-id="6b27b-653">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="6b27b-653">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="6b27b-654">值，该值指示响应可执行文件的传播、 年龄或受信任的列表不满足条件。</span><span class="sxs-lookup"><span data-stu-id="6b27b-654">Value indicating response to executables that don't meet a prevalence, age, or trusted list criteria.</span></span> <span data-ttu-id="6b27b-655">可取值为：`userDefined`、`enable`、`auditMode`。</span><span class="sxs-lookup"><span data-stu-id="6b27b-655">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="6b27b-656">defenderEmailContentExecutionType</span><span class="sxs-lookup"><span data-stu-id="6b27b-656">defenderEmailContentExecutionType</span></span>|[<span data-ttu-id="6b27b-657">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="6b27b-657">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="6b27b-658">指示是否应该从电子邮件 （客户端 webmail/邮件） 放执行 （exe、 dll，ps、 js、 vbs 等） 的可执行内容的值。</span><span class="sxs-lookup"><span data-stu-id="6b27b-658">Value indicating if execution of executable content (exe, dll, ps, js, vbs, etc) should be dropped from email (webmail/mail-client).</span></span> <span data-ttu-id="6b27b-659">可取值为：`userDefined`、`block`、`auditMode`。</span><span class="sxs-lookup"><span data-stu-id="6b27b-659">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="6b27b-660">defenderEmailContentExecution</span><span class="sxs-lookup"><span data-stu-id="6b27b-660">defenderEmailContentExecution</span></span>|[<span data-ttu-id="6b27b-661">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="6b27b-661">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="6b27b-662">指示是否应该从电子邮件 （客户端 webmail/邮件） 放执行 （exe、 dll，ps、 js、 vbs 等） 的可执行内容的值。</span><span class="sxs-lookup"><span data-stu-id="6b27b-662">Value indicating if execution of executable content (exe, dll, ps, js, vbs, etc) should be dropped from email (webmail/mail-client).</span></span> <span data-ttu-id="6b27b-663">可取值为：`userDefined`、`enable`、`auditMode`。</span><span class="sxs-lookup"><span data-stu-id="6b27b-663">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="6b27b-664">defenderAdvancedRansomewareProtectionType</span><span class="sxs-lookup"><span data-stu-id="6b27b-664">defenderAdvancedRansomewareProtectionType</span></span>|[<span data-ttu-id="6b27b-665">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="6b27b-665">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="6b27b-666">指示使用高级防范 ransomeware 值。</span><span class="sxs-lookup"><span data-stu-id="6b27b-666">Value indicating use of advanced protection against ransomeware.</span></span> <span data-ttu-id="6b27b-667">可取值为：`userDefined`、`enable`、`auditMode`。</span><span class="sxs-lookup"><span data-stu-id="6b27b-667">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="6b27b-668">defenderGuardMyFoldersType</span><span class="sxs-lookup"><span data-stu-id="6b27b-668">defenderGuardMyFoldersType</span></span>|[<span data-ttu-id="6b27b-669">folderProtectionType</span><span class="sxs-lookup"><span data-stu-id="6b27b-669">folderProtectionType</span></span>](../resources/intune-deviceconfig-folderprotectiontype.md)|<span data-ttu-id="6b27b-670">指示受保护的文件夹的行为的值。</span><span class="sxs-lookup"><span data-stu-id="6b27b-670">Value indicating the behavior of protected folders.</span></span> <span data-ttu-id="6b27b-671">可取值为：`userDefined`、`enable`、`auditMode`、`blockDiskModification`、`auditDiskModification`。</span><span class="sxs-lookup"><span data-stu-id="6b27b-671">Possible values are: `userDefined`, `enable`, `auditMode`, `blockDiskModification`, `auditDiskModification`.</span></span>|
|<span data-ttu-id="6b27b-672">defenderGuardedFoldersAllowedAppPaths</span><span class="sxs-lookup"><span data-stu-id="6b27b-672">defenderGuardedFoldersAllowedAppPaths</span></span>|<span data-ttu-id="6b27b-673">String 集合</span><span class="sxs-lookup"><span data-stu-id="6b27b-673">String collection</span></span>|<span data-ttu-id="6b27b-674">允许访问受保护文件夹的 exe 路径列表</span><span class="sxs-lookup"><span data-stu-id="6b27b-674">List of paths to exe that are allowed to access protected folders</span></span>|
|<span data-ttu-id="6b27b-675">defenderAdditionalGuardedFolders</span><span class="sxs-lookup"><span data-stu-id="6b27b-675">defenderAdditionalGuardedFolders</span></span>|<span data-ttu-id="6b27b-676">String 集合</span><span class="sxs-lookup"><span data-stu-id="6b27b-676">String collection</span></span>|<span data-ttu-id="6b27b-677">要添加到受保护文件夹列表的文件夹路径列表</span><span class="sxs-lookup"><span data-stu-id="6b27b-677">List of folder paths to be added to the list of protected folders</span></span>|
|<span data-ttu-id="6b27b-678">defenderNetworkProtectionType</span><span class="sxs-lookup"><span data-stu-id="6b27b-678">defenderNetworkProtectionType</span></span>|[<span data-ttu-id="6b27b-679">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="6b27b-679">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="6b27b-680">指示 NetworkProtection 的行为的值。</span><span class="sxs-lookup"><span data-stu-id="6b27b-680">Value indicating the behavior of NetworkProtection.</span></span> <span data-ttu-id="6b27b-681">可取值为：`userDefined`、`enable`、`auditMode`。</span><span class="sxs-lookup"><span data-stu-id="6b27b-681">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="6b27b-682">defenderExploitProtectionXml</span><span class="sxs-lookup"><span data-stu-id="6b27b-682">defenderExploitProtectionXml</span></span>|<span data-ttu-id="6b27b-683">Binary</span><span class="sxs-lookup"><span data-stu-id="6b27b-683">Binary</span></span>|<span data-ttu-id="6b27b-684">包含有关 Exploit Protection 详细信息的 xml 内容。</span><span class="sxs-lookup"><span data-stu-id="6b27b-684">Xml content containing information regarding exploit protection details.</span></span>|
|<span data-ttu-id="6b27b-685">defenderExploitProtectionXmlFileName</span><span class="sxs-lookup"><span data-stu-id="6b27b-685">defenderExploitProtectionXmlFileName</span></span>|<span data-ttu-id="6b27b-686">String</span><span class="sxs-lookup"><span data-stu-id="6b27b-686">String</span></span>|<span data-ttu-id="6b27b-687">从中获取 DefenderExploitProtectionXml 的文件的名称。</span><span class="sxs-lookup"><span data-stu-id="6b27b-687">Name of the file from which DefenderExploitProtectionXml was obtained.</span></span>|
|<span data-ttu-id="6b27b-688">defenderSecurityCenterBlockExploitProtectionOverride</span><span class="sxs-lookup"><span data-stu-id="6b27b-688">defenderSecurityCenterBlockExploitProtectionOverride</span></span>|<span data-ttu-id="6b27b-689">Boolean</span><span class="sxs-lookup"><span data-stu-id="6b27b-689">Boolean</span></span>|<span data-ttu-id="6b27b-690">指示是否阻止用户覆盖 Exploit Protection 设置。</span><span class="sxs-lookup"><span data-stu-id="6b27b-690">Indicates whether or not to block user from overriding Exploit Protection settings.</span></span>|
|<span data-ttu-id="6b27b-691">appLockerApplicationControl</span><span class="sxs-lookup"><span data-stu-id="6b27b-691">appLockerApplicationControl</span></span>|[<span data-ttu-id="6b27b-692">appLockerApplicationControlType</span><span class="sxs-lookup"><span data-stu-id="6b27b-692">appLockerApplicationControlType</span></span>](../resources/intune-deviceconfig-applockerapplicationcontroltype.md)|<span data-ttu-id="6b27b-693">使管理员能够选择在设备上允许哪些类型的应用。</span><span class="sxs-lookup"><span data-stu-id="6b27b-693">Enables the Admin to choose what types of app to allow on devices.</span></span> <span data-ttu-id="6b27b-694">可取值为：`notConfigured`、`enforceComponentsAndStoreApps`、`auditComponentsAndStoreApps`、`enforceComponentsStoreAppsAndSmartlocker`、`auditComponentsStoreAppsAndSmartlocker`。</span><span class="sxs-lookup"><span data-stu-id="6b27b-694">Possible values are: `notConfigured`, `enforceComponentsAndStoreApps`, `auditComponentsAndStoreApps`, `enforceComponentsStoreAppsAndSmartlocker`, `auditComponentsStoreAppsAndSmartlocker`.</span></span>|
|<span data-ttu-id="6b27b-695">deviceGuardLocalSystemAuthorityCredentialGuardSettings</span><span class="sxs-lookup"><span data-stu-id="6b27b-695">deviceGuardLocalSystemAuthorityCredentialGuardSettings</span></span>|[<span data-ttu-id="6b27b-696">deviceGuardLocalSystemAuthorityCredentialGuardType</span><span class="sxs-lookup"><span data-stu-id="6b27b-696">deviceGuardLocalSystemAuthorityCredentialGuardType</span></span>](../resources/intune-deviceconfig-deviceguardlocalsystemauthoritycredentialguardtype.md)|<span data-ttu-id="6b27b-697">在凭据 Guard 时同时启用对安全启动和虚拟化基于安全平台安全级别打开。</span><span class="sxs-lookup"><span data-stu-id="6b27b-697">Turn on Credential Guard when Platform Security Level with Secure Boot and Virtualization Based Security are both enabled.</span></span> <span data-ttu-id="6b27b-698">可取值为：`notConfigured`、`enableWithUEFILock`、`enableWithoutUEFILock`。</span><span class="sxs-lookup"><span data-stu-id="6b27b-698">Possible values are: `notConfigured`, `enableWithUEFILock`, `enableWithoutUEFILock`.</span></span>|
|<span data-ttu-id="6b27b-699">deviceGuardEnableVirtualizationBasedSecurity</span><span class="sxs-lookup"><span data-stu-id="6b27b-699">deviceGuardEnableVirtualizationBasedSecurity</span></span>|<span data-ttu-id="6b27b-700">Boolean</span><span class="sxs-lookup"><span data-stu-id="6b27b-700">Boolean</span></span>|<span data-ttu-id="6b27b-701">虚拟化选项会启用基于 Security(VBS)。</span><span class="sxs-lookup"><span data-stu-id="6b27b-701">Turns On Virtualization Based Security(VBS).</span></span>|
|<span data-ttu-id="6b27b-702">deviceGuardEnableSecureBootWithDMA</span><span class="sxs-lookup"><span data-stu-id="6b27b-702">deviceGuardEnableSecureBootWithDMA</span></span>|<span data-ttu-id="6b27b-703">Boolean</span><span class="sxs-lookup"><span data-stu-id="6b27b-703">Boolean</span></span>|<span data-ttu-id="6b27b-704">指定是否将在下次重新启动启用平台安全级别。</span><span class="sxs-lookup"><span data-stu-id="6b27b-704">Specifies whether Platform Security Level is enabled at next reboot.</span></span>|
|<span data-ttu-id="6b27b-705">deviceGuardLaunchSystemGuard</span><span class="sxs-lookup"><span data-stu-id="6b27b-705">deviceGuardLaunchSystemGuard</span></span>|<span data-ttu-id="6b27b-706">[启用](../resources/intune-shared-enablement</span><span class="sxs-lookup"><span data-stu-id="6b27b-706">[enablement](../resources/intune-shared-enablement</span></span>
<span data-ttu-id="6b27b-707">.md)</span><span class="sxs-lookup"><span data-stu-id="6b27b-707">.md)</span></span>|<span data-ttu-id="6b27b-708">允许 IT 管理员配置的系统 Guard 启动。</span><span class="sxs-lookup"><span data-stu-id="6b27b-708">Allows the IT admin to configure the launch of System Guard.</span></span> <span data-ttu-id="6b27b-709">可取值为：`notConfigured`、`enabled`、`disabled`。</span><span class="sxs-lookup"><span data-stu-id="6b27b-709">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="6b27b-710">smartScreenEnableInShell</span><span class="sxs-lookup"><span data-stu-id="6b27b-710">smartScreenEnableInShell</span></span>|<span data-ttu-id="6b27b-711">Boolean</span><span class="sxs-lookup"><span data-stu-id="6b27b-711">Boolean</span></span>|<span data-ttu-id="6b27b-712">允许 IT 管理员配置适用于 Windows 的 SmartScreen。</span><span class="sxs-lookup"><span data-stu-id="6b27b-712">Allows IT Admins to configure SmartScreen for Windows.</span></span>|
|<span data-ttu-id="6b27b-713">smartScreenBlockOverrideForFiles</span><span class="sxs-lookup"><span data-stu-id="6b27b-713">smartScreenBlockOverrideForFiles</span></span>|<span data-ttu-id="6b27b-714">Boolean</span><span class="sxs-lookup"><span data-stu-id="6b27b-714">Boolean</span></span>|<span data-ttu-id="6b27b-715">允许 IT 管理员控制用户是否可以忽略 SmartScreen 警告并运行恶意文件。</span><span class="sxs-lookup"><span data-stu-id="6b27b-715">Allows IT Admins to control whether users can can ignore SmartScreen warnings and run malicious files.</span></span>|
|<span data-ttu-id="6b27b-716">applicationGuardEnabled</span><span class="sxs-lookup"><span data-stu-id="6b27b-716">applicationGuardEnabled</span></span>|<span data-ttu-id="6b27b-717">Boolean</span><span class="sxs-lookup"><span data-stu-id="6b27b-717">Boolean</span></span>|<span data-ttu-id="6b27b-718">启用 Windows Defender 应用程序防护</span><span class="sxs-lookup"><span data-stu-id="6b27b-718">Enable Windows Defender Application Guard</span></span>|
|<span data-ttu-id="6b27b-719">applicationGuardEnabledOptions</span><span class="sxs-lookup"><span data-stu-id="6b27b-719">applicationGuardEnabledOptions</span></span>|[<span data-ttu-id="6b27b-720">applicationGuardEnabledOptions</span><span class="sxs-lookup"><span data-stu-id="6b27b-720">applicationGuardEnabledOptions</span></span>](../resources/intune-deviceconfig-applicationguardenabledoptions.md)|<span data-ttu-id="6b27b-721">Windows Defender 应用程序 Guard 启用更高版本的 Windows 版本。</span><span class="sxs-lookup"><span data-stu-id="6b27b-721">Enable Windows Defender Application Guard for newer Windows builds.</span></span> <span data-ttu-id="6b27b-722">可取值为：`notConfigured`、`enabledForEdge`、`enabledForOffice`、`enabledForEdgeAndOffice`。</span><span class="sxs-lookup"><span data-stu-id="6b27b-722">Possible values are: `notConfigured`, `enabledForEdge`, `enabledForOffice`, `enabledForEdgeAndOffice`.</span></span>|
|<span data-ttu-id="6b27b-723">applicationGuardBlockFileTransfer</span><span class="sxs-lookup"><span data-stu-id="6b27b-723">applicationGuardBlockFileTransfer</span></span>|[<span data-ttu-id="6b27b-724">applicationGuardBlockFileTransferType</span><span class="sxs-lookup"><span data-stu-id="6b27b-724">applicationGuardBlockFileTransferType</span></span>](../resources/intune-deviceconfig-applicationguardblockfiletransfertype.md)|<span data-ttu-id="6b27b-725">阻止传输图像文件、 文本文件或两者到剪贴板。</span><span class="sxs-lookup"><span data-stu-id="6b27b-725">Block clipboard to transfer image file, text file or neither of them.</span></span> <span data-ttu-id="6b27b-726">可取值为：`notConfigured`、`blockImageAndTextFile`、`blockImageFile`、`blockNone`、`blockTextFile`。</span><span class="sxs-lookup"><span data-stu-id="6b27b-726">Possible values are: `notConfigured`, `blockImageAndTextFile`, `blockImageFile`, `blockNone`, `blockTextFile`.</span></span>|
|<span data-ttu-id="6b27b-727">applicationGuardBlockNonEnterpriseContent</span><span class="sxs-lookup"><span data-stu-id="6b27b-727">applicationGuardBlockNonEnterpriseContent</span></span>|<span data-ttu-id="6b27b-728">Boolean</span><span class="sxs-lookup"><span data-stu-id="6b27b-728">Boolean</span></span>|<span data-ttu-id="6b27b-729">阻止企业站点加载非企业内容，例如第三方插件</span><span class="sxs-lookup"><span data-stu-id="6b27b-729">Block enterprise sites to load non-enterprise content, such as third party plug-ins</span></span>|
|<span data-ttu-id="6b27b-730">applicationGuardAllowPersistence</span><span class="sxs-lookup"><span data-stu-id="6b27b-730">applicationGuardAllowPersistence</span></span>|<span data-ttu-id="6b27b-731">Boolean</span><span class="sxs-lookup"><span data-stu-id="6b27b-731">Boolean</span></span>|<span data-ttu-id="6b27b-732">允许 App Guard 容器（收藏夹、Cookie、Web 密码等）内的持久用户生成数据</span><span class="sxs-lookup"><span data-stu-id="6b27b-732">Allow persisting user generated data inside the App Guard Containter (favorites, cookies, web passwords, etc.)</span></span>|
|<span data-ttu-id="6b27b-733">applicationGuardForceAuditing</span><span class="sxs-lookup"><span data-stu-id="6b27b-733">applicationGuardForceAuditing</span></span>|<span data-ttu-id="6b27b-734">Boolean</span><span class="sxs-lookup"><span data-stu-id="6b27b-734">Boolean</span></span>|<span data-ttu-id="6b27b-735">强制审核将存留 Windows 日志和事件以满足安全/符合性条件（示例事件是用户登录注销、特权使用、软件安装、系统更改等）</span><span class="sxs-lookup"><span data-stu-id="6b27b-735">Force auditing will persist Windows logs and events to meet security/compliance criteria (sample events are user login-logoff, use of privilege rights, software installation, system changes, etc.)</span></span>|
|<span data-ttu-id="6b27b-736">applicationGuardBlockClipboardSharing</span><span class="sxs-lookup"><span data-stu-id="6b27b-736">applicationGuardBlockClipboardSharing</span></span>|[<span data-ttu-id="6b27b-737">applicationGuardBlockClipboardSharingType</span><span class="sxs-lookup"><span data-stu-id="6b27b-737">applicationGuardBlockClipboardSharingType</span></span>](../resources/intune-deviceconfig-applicationguardblockclipboardsharingtype.md)|<span data-ttu-id="6b27b-738">阻止剪贴板将数据从主机共享到容器或从容器共享到主机，或阻止两种方式，或两种方式均不阻止。</span><span class="sxs-lookup"><span data-stu-id="6b27b-738">Block clipboard to share data from Host to Container, or from Container to Host, or both ways, or neither ways.</span></span> <span data-ttu-id="6b27b-739">可取值为：`notConfigured`、`blockBoth`、`blockHostToContainer`、`blockContainerToHost`、`blockNone`。</span><span class="sxs-lookup"><span data-stu-id="6b27b-739">Possible values are: `notConfigured`, `blockBoth`, `blockHostToContainer`, `blockContainerToHost`, `blockNone`.</span></span>|
|<span data-ttu-id="6b27b-740">applicationGuardAllowPrintToPDF</span><span class="sxs-lookup"><span data-stu-id="6b27b-740">applicationGuardAllowPrintToPDF</span></span>|<span data-ttu-id="6b27b-741">Boolean</span><span class="sxs-lookup"><span data-stu-id="6b27b-741">Boolean</span></span>|<span data-ttu-id="6b27b-742">允许从容器打印为 PDF 格式</span><span class="sxs-lookup"><span data-stu-id="6b27b-742">Allow printing to PDF from Container</span></span>|
|<span data-ttu-id="6b27b-743">applicationGuardAllowPrintToXPS</span><span class="sxs-lookup"><span data-stu-id="6b27b-743">applicationGuardAllowPrintToXPS</span></span>|<span data-ttu-id="6b27b-744">Boolean</span><span class="sxs-lookup"><span data-stu-id="6b27b-744">Boolean</span></span>|<span data-ttu-id="6b27b-745">允许从容器打印为 XPS 格式</span><span class="sxs-lookup"><span data-stu-id="6b27b-745">Allow printing to XPS from Container</span></span>|
|<span data-ttu-id="6b27b-746">applicationGuardAllowPrintToLocalPrinters</span><span class="sxs-lookup"><span data-stu-id="6b27b-746">applicationGuardAllowPrintToLocalPrinters</span></span>|<span data-ttu-id="6b27b-747">Boolean</span><span class="sxs-lookup"><span data-stu-id="6b27b-747">Boolean</span></span>|<span data-ttu-id="6b27b-748">允许从容器打印到本地打印机</span><span class="sxs-lookup"><span data-stu-id="6b27b-748">Allow printing to Local Printers from Container</span></span>|
|<span data-ttu-id="6b27b-749">applicationGuardAllowPrintToNetworkPrinters</span><span class="sxs-lookup"><span data-stu-id="6b27b-749">applicationGuardAllowPrintToNetworkPrinters</span></span>|<span data-ttu-id="6b27b-750">Boolean</span><span class="sxs-lookup"><span data-stu-id="6b27b-750">Boolean</span></span>|<span data-ttu-id="6b27b-751">允许从容器打印到网络打印机</span><span class="sxs-lookup"><span data-stu-id="6b27b-751">Allow printing to Network Printers from Container</span></span>|
|<span data-ttu-id="6b27b-752">applicationGuardAllowVirtualGPU</span><span class="sxs-lookup"><span data-stu-id="6b27b-752">applicationGuardAllowVirtualGPU</span></span>|<span data-ttu-id="6b27b-753">Boolean</span><span class="sxs-lookup"><span data-stu-id="6b27b-753">Boolean</span></span>|<span data-ttu-id="6b27b-754">允许应用程序 guard 用于虚拟 GPU</span><span class="sxs-lookup"><span data-stu-id="6b27b-754">Allow application guard to use virtual GPU</span></span>|
|<span data-ttu-id="6b27b-755">applicationGuardAllowFileSaveOnHost</span><span class="sxs-lookup"><span data-stu-id="6b27b-755">applicationGuardAllowFileSaveOnHost</span></span>|<span data-ttu-id="6b27b-756">Boolean</span><span class="sxs-lookup"><span data-stu-id="6b27b-756">Boolean</span></span>|<span data-ttu-id="6b27b-757">允许用户从应用程序 guard 容器中的边缘下载文件并将其保存在主机上文件系统</span><span class="sxs-lookup"><span data-stu-id="6b27b-757">Allow users to download files from Edge in the application guard container and save them on the host file system</span></span>|
|<span data-ttu-id="6b27b-758">bitLockerAllowStandardUserEncryption</span><span class="sxs-lookup"><span data-stu-id="6b27b-758">bitLockerAllowStandardUserEncryption</span></span>|<span data-ttu-id="6b27b-759">Boolean</span><span class="sxs-lookup"><span data-stu-id="6b27b-759">Boolean</span></span>|<span data-ttu-id="6b27b-760">允许管理员允许在 Azure AD 加入过程中启用 encrpytion 标准用户。</span><span class="sxs-lookup"><span data-stu-id="6b27b-760">Allows the admin to allow standard users to enable encrpytion during Azure AD Join.</span></span>|
|<span data-ttu-id="6b27b-761">bitLockerDisableWarningForOtherDiskEncryption</span><span class="sxs-lookup"><span data-stu-id="6b27b-761">bitLockerDisableWarningForOtherDiskEncryption</span></span>|<span data-ttu-id="6b27b-762">Boolean</span><span class="sxs-lookup"><span data-stu-id="6b27b-762">Boolean</span></span>|<span data-ttu-id="6b27b-763">允许管理员禁用对用户计算机上其他磁盘加密的警告提示。</span><span class="sxs-lookup"><span data-stu-id="6b27b-763">Allows the Admin to disable the warning prompt for other disk encryption on the user machines.</span></span>|
|<span data-ttu-id="6b27b-764">bitLockerEnableStorageCardEncryptionOnMobile</span><span class="sxs-lookup"><span data-stu-id="6b27b-764">bitLockerEnableStorageCardEncryptionOnMobile</span></span>|<span data-ttu-id="6b27b-765">Boolean</span><span class="sxs-lookup"><span data-stu-id="6b27b-765">Boolean</span></span>|<span data-ttu-id="6b27b-766">允许管理员要求使用 BitLocker 开启加密功能。</span><span class="sxs-lookup"><span data-stu-id="6b27b-766">Allows the admin to require encryption to be turned on using BitLocker.</span></span> <span data-ttu-id="6b27b-767">此策略仅适用于移动 SKU。</span><span class="sxs-lookup"><span data-stu-id="6b27b-767">This policy is valid only for a mobile SKU.</span></span>|
|<span data-ttu-id="6b27b-768">bitLockerEncryptDevice</span><span class="sxs-lookup"><span data-stu-id="6b27b-768">bitLockerEncryptDevice</span></span>|<span data-ttu-id="6b27b-769">Boolean</span><span class="sxs-lookup"><span data-stu-id="6b27b-769">Boolean</span></span>|<span data-ttu-id="6b27b-770">允许管理员要求使用 BitLocker 开启加密功能。</span><span class="sxs-lookup"><span data-stu-id="6b27b-770">Allows the admin to require encryption to be turned on using BitLocker.</span></span>|
|<span data-ttu-id="6b27b-771">bitLockerSystemDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="6b27b-771">bitLockerSystemDrivePolicy</span></span>|[<span data-ttu-id="6b27b-772">bitLockerSystemDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="6b27b-772">bitLockerSystemDrivePolicy</span></span>](../resources/intune-deviceconfig-bitlockersystemdrivepolicy.md)|<span data-ttu-id="6b27b-773">BitLocker 系统驱动器策略。</span><span class="sxs-lookup"><span data-stu-id="6b27b-773">BitLocker System Drive Policy.</span></span>|
|<span data-ttu-id="6b27b-774">bitLockerFixedDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="6b27b-774">bitLockerFixedDrivePolicy</span></span>|[<span data-ttu-id="6b27b-775">bitLockerFixedDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="6b27b-775">bitLockerFixedDrivePolicy</span></span>](../resources/intune-deviceconfig-bitlockerfixeddrivepolicy.md)|<span data-ttu-id="6b27b-776">BitLocker 固定驱动器策略。</span><span class="sxs-lookup"><span data-stu-id="6b27b-776">BitLocker Fixed Drive Policy.</span></span>|
|<span data-ttu-id="6b27b-777">bitLockerRemovableDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="6b27b-777">bitLockerRemovableDrivePolicy</span></span>|[<span data-ttu-id="6b27b-778">bitLockerRemovableDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="6b27b-778">bitLockerRemovableDrivePolicy</span></span>](../resources/intune-deviceconfig-bitlockerremovabledrivepolicy.md)|<span data-ttu-id="6b27b-779">BitLocker 可移动驱动器策略。</span><span class="sxs-lookup"><span data-stu-id="6b27b-779">BitLocker Removable Drive Policy.</span></span>|



## <a name="response"></a><span data-ttu-id="6b27b-780">响应</span><span class="sxs-lookup"><span data-stu-id="6b27b-780">Response</span></span>
<span data-ttu-id="6b27b-781">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="6b27b-781">If successful, this method returns a `201 Created` response code and a [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6b27b-782">示例</span><span class="sxs-lookup"><span data-stu-id="6b27b-782">Example</span></span>

### <a name="request"></a><span data-ttu-id="6b27b-783">请求</span><span class="sxs-lookup"><span data-stu-id="6b27b-783">Request</span></span>
<span data-ttu-id="6b27b-784">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="6b27b-784">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 26475

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
  "defenderSecurityCenterDisableHardwareUI": true,
  "defenderSecurityCenterDisableRansomwareUI": true,
  "defenderSecurityCenterDisableSecureBootUI": true,
  "defenderSecurityCenterDisableTroubleshootingUI": true,
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
  "defenderAttackSurfaceReductionExcludedPaths": [
    "Defender Attack Surface Reduction Excluded Paths value"
  ],
  "defenderOfficeAppsOtherProcessInjectionType": "block",
  "defenderOfficeAppsOtherProcessInjection": "enable",
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

### <a name="response"></a><span data-ttu-id="6b27b-785">响应</span><span class="sxs-lookup"><span data-stu-id="6b27b-785">Response</span></span>
<span data-ttu-id="6b27b-p196">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="6b27b-p196">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 26647

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
  "defenderSecurityCenterDisableHardwareUI": true,
  "defenderSecurityCenterDisableRansomwareUI": true,
  "defenderSecurityCenterDisableSecureBootUI": true,
  "defenderSecurityCenterDisableTroubleshootingUI": true,
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
  "defenderAttackSurfaceReductionExcludedPaths": [
    "Defender Attack Surface Reduction Excluded Paths value"
  ],
  "defenderOfficeAppsOtherProcessInjectionType": "block",
  "defenderOfficeAppsOtherProcessInjection": "enable",
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




