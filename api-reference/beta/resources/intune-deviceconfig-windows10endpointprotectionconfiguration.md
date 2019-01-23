---
title: windows10EndpointProtectionConfiguration 资源类型
description: 本主题提供由 Windows10EndpointProtectionConfiguration 资源公开的已声明方法、属性和关系的说明。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: f759ee9601ce8afe53c73a2bfdb92f49fec38739
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29425972"
---
# <a name="windows10endpointprotectionconfiguration-resource-type"></a><span data-ttu-id="d9a52-103">windows10EndpointProtectionConfiguration 资源类型</span><span class="sxs-lookup"><span data-stu-id="d9a52-103">windows10EndpointProtectionConfiguration resource type</span></span>

> <span data-ttu-id="d9a52-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="d9a52-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="d9a52-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="d9a52-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d9a52-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d9a52-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d9a52-107">本主题提供由 Windows10EndpointProtectionConfiguration 资源公开的已声明方法、属性和关系的说明。</span><span class="sxs-lookup"><span data-stu-id="d9a52-107">This topic provides descriptions of the declared methods, properties and relationships exposed by the Windows10EndpointProtectionConfiguration resource.</span></span>


<span data-ttu-id="d9a52-108">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d9a52-108">Inherits from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>

## <a name="methods"></a><span data-ttu-id="d9a52-109">方法</span><span class="sxs-lookup"><span data-stu-id="d9a52-109">Methods</span></span>
|<span data-ttu-id="d9a52-110">方法</span><span class="sxs-lookup"><span data-stu-id="d9a52-110">Method</span></span>|<span data-ttu-id="d9a52-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="d9a52-111">Return Type</span></span>|<span data-ttu-id="d9a52-112">说明</span><span class="sxs-lookup"><span data-stu-id="d9a52-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="d9a52-113">List windows10EndpointProtectionConfigurations</span><span class="sxs-lookup"><span data-stu-id="d9a52-113">List windows10EndpointProtectionConfigurations</span></span>](../api/intune-deviceconfig-windows10endpointprotectionconfiguration-list.md)|<span data-ttu-id="d9a52-114">[windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) 集合</span><span class="sxs-lookup"><span data-stu-id="d9a52-114">[windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) collection</span></span>|<span data-ttu-id="d9a52-115">列出 [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="d9a52-115">List properties and relationships of the [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="d9a52-116">Get windows10EndpointProtectionConfiguration</span><span class="sxs-lookup"><span data-stu-id="d9a52-116">Get windows10EndpointProtectionConfiguration</span></span>](../api/intune-deviceconfig-windows10endpointprotectionconfiguration-get.md)|[<span data-ttu-id="d9a52-117">windows10EndpointProtectionConfiguration</span><span class="sxs-lookup"><span data-stu-id="d9a52-117">windows10EndpointProtectionConfiguration</span></span>](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md)|<span data-ttu-id="d9a52-118">读取 [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="d9a52-118">Read properties and relationships of the [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) object.</span></span>|
|[<span data-ttu-id="d9a52-119">Create windows10EndpointProtectionConfiguration</span><span class="sxs-lookup"><span data-stu-id="d9a52-119">Create windows10EndpointProtectionConfiguration</span></span>](../api/intune-deviceconfig-windows10endpointprotectionconfiguration-create.md)|[<span data-ttu-id="d9a52-120">windows10EndpointProtectionConfiguration</span><span class="sxs-lookup"><span data-stu-id="d9a52-120">windows10EndpointProtectionConfiguration</span></span>](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md)|<span data-ttu-id="d9a52-121">创建新的 [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="d9a52-121">Create a new [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) object.</span></span>|
|[<span data-ttu-id="d9a52-122">Delete windows10EndpointProtectionConfiguration</span><span class="sxs-lookup"><span data-stu-id="d9a52-122">Delete windows10EndpointProtectionConfiguration</span></span>](../api/intune-deviceconfig-windows10endpointprotectionconfiguration-delete.md)|<span data-ttu-id="d9a52-123">无</span><span class="sxs-lookup"><span data-stu-id="d9a52-123">None</span></span>|<span data-ttu-id="d9a52-124">删除 [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md)。</span><span class="sxs-lookup"><span data-stu-id="d9a52-124">Deletes a [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md).</span></span>|
|[<span data-ttu-id="d9a52-125">Update windows10EndpointProtectionConfiguration</span><span class="sxs-lookup"><span data-stu-id="d9a52-125">Update windows10EndpointProtectionConfiguration</span></span>](../api/intune-deviceconfig-windows10endpointprotectionconfiguration-update.md)|[<span data-ttu-id="d9a52-126">windows10EndpointProtectionConfiguration</span><span class="sxs-lookup"><span data-stu-id="d9a52-126">windows10EndpointProtectionConfiguration</span></span>](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md)|<span data-ttu-id="d9a52-127">更新 [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="d9a52-127">Update the properties of a [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="d9a52-128">属性</span><span class="sxs-lookup"><span data-stu-id="d9a52-128">Properties</span></span>
|<span data-ttu-id="d9a52-129">属性</span><span class="sxs-lookup"><span data-stu-id="d9a52-129">Property</span></span>|<span data-ttu-id="d9a52-130">类型</span><span class="sxs-lookup"><span data-stu-id="d9a52-130">Type</span></span>|<span data-ttu-id="d9a52-131">说明</span><span class="sxs-lookup"><span data-stu-id="d9a52-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d9a52-132">id</span><span class="sxs-lookup"><span data-stu-id="d9a52-132">id</span></span>|<span data-ttu-id="d9a52-133">String</span><span class="sxs-lookup"><span data-stu-id="d9a52-133">String</span></span>|<span data-ttu-id="d9a52-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="d9a52-134">Key of the entity.</span></span> <span data-ttu-id="d9a52-135">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d9a52-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d9a52-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d9a52-136">lastModifiedDateTime</span></span>|<span data-ttu-id="d9a52-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d9a52-137">DateTimeOffset</span></span>|<span data-ttu-id="d9a52-138">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="d9a52-138">DateTime the object was last modified.</span></span> <span data-ttu-id="d9a52-139">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d9a52-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d9a52-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="d9a52-140">roleScopeTagIds</span></span>|<span data-ttu-id="d9a52-141">String 集合</span><span class="sxs-lookup"><span data-stu-id="d9a52-141">String collection</span></span>|<span data-ttu-id="d9a52-142">此实体实例范围标记的列表。</span><span class="sxs-lookup"><span data-stu-id="d9a52-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="d9a52-143">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d9a52-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d9a52-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="d9a52-144">supportsScopeTags</span></span>|<span data-ttu-id="d9a52-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="d9a52-145">Boolean</span></span>|<span data-ttu-id="d9a52-146">指示基础的设备配置支持分配的范围标记。</span><span class="sxs-lookup"><span data-stu-id="d9a52-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="d9a52-147">此值为 false，并且实体将不会对作用域的用户可见时，不允许将分配给 ScopeTags 属性。</span><span class="sxs-lookup"><span data-stu-id="d9a52-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="d9a52-148">这将发生在 Silverlight 中创建的旧策略，并可以解析通过删除并重新创建 Azure 门户中的策略。</span><span class="sxs-lookup"><span data-stu-id="d9a52-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="d9a52-149">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="d9a52-149">This property is read-only.</span></span> <span data-ttu-id="d9a52-150">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d9a52-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d9a52-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d9a52-151">createdDateTime</span></span>|<span data-ttu-id="d9a52-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d9a52-152">DateTimeOffset</span></span>|<span data-ttu-id="d9a52-153">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="d9a52-153">DateTime the object was created.</span></span> <span data-ttu-id="d9a52-154">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d9a52-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d9a52-155">description</span><span class="sxs-lookup"><span data-stu-id="d9a52-155">description</span></span>|<span data-ttu-id="d9a52-156">String</span><span class="sxs-lookup"><span data-stu-id="d9a52-156">String</span></span>|<span data-ttu-id="d9a52-157">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="d9a52-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="d9a52-158">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d9a52-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d9a52-159">displayName</span><span class="sxs-lookup"><span data-stu-id="d9a52-159">displayName</span></span>|<span data-ttu-id="d9a52-160">String</span><span class="sxs-lookup"><span data-stu-id="d9a52-160">String</span></span>|<span data-ttu-id="d9a52-161">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="d9a52-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="d9a52-162">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d9a52-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d9a52-163">version</span><span class="sxs-lookup"><span data-stu-id="d9a52-163">version</span></span>|<span data-ttu-id="d9a52-164">Int32</span><span class="sxs-lookup"><span data-stu-id="d9a52-164">Int32</span></span>|<span data-ttu-id="d9a52-165">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="d9a52-165">Version of the device configuration.</span></span> <span data-ttu-id="d9a52-166">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d9a52-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d9a52-167">dmaGuardDeviceEnumerationPolicy</span><span class="sxs-lookup"><span data-stu-id="d9a52-167">dmaGuardDeviceEnumerationPolicy</span></span>|[<span data-ttu-id="d9a52-168">dmaGuardDeviceEnumerationPolicyType</span><span class="sxs-lookup"><span data-stu-id="d9a52-168">dmaGuardDeviceEnumerationPolicyType</span></span>](../resources/intune-deviceconfig-dmaguarddeviceenumerationpolicytype.md)|<span data-ttu-id="d9a52-169">此策略旨在提供针对外部 DMA 功能的设备的其他安全。</span><span class="sxs-lookup"><span data-stu-id="d9a52-169">This policy is intended to provide additional security against external DMA capable devices.</span></span> <span data-ttu-id="d9a52-170">允许更好地控制外部 DMA 能够设备枚举与 DMA Remapping/设备内存隔离和沙盒不兼容。</span><span class="sxs-lookup"><span data-stu-id="d9a52-170">It allows for more control over the enumeration of external DMA capable devices incompatible with DMA Remapping/device memory isolation and sandboxing.</span></span> <span data-ttu-id="d9a52-171">支持并由系统固件启用内核 DMA 保护时，此策略才能起作用。</span><span class="sxs-lookup"><span data-stu-id="d9a52-171">This policy only takes effect when Kernel DMA Protection is supported and enabled by the system firmware.</span></span> <span data-ttu-id="d9a52-172">内核 DMA 保护是通过策略或最终用户无法控制平台功能。</span><span class="sxs-lookup"><span data-stu-id="d9a52-172">Kernel DMA Protection is a platform feature that cannot be controlled via policy or by end user.</span></span> <span data-ttu-id="d9a52-173">它具有制造时，系统必须支持。</span><span class="sxs-lookup"><span data-stu-id="d9a52-173">It has to be supported by the system at the time of manufacturing.</span></span> <span data-ttu-id="d9a52-174">若要检查系统是否支持内核 DMA 保护，请检查的 MSINFO32.exe 摘要页中的内核 DMA 保护字段。</span><span class="sxs-lookup"><span data-stu-id="d9a52-174">To check if the system supports Kernel DMA Protection, please check the Kernel DMA Protection field in the Summary page of MSINFO32.exe.</span></span> <span data-ttu-id="d9a52-175">可取值为：`deviceDefault`、`blockAll`、`allowAll`。</span><span class="sxs-lookup"><span data-stu-id="d9a52-175">Possible values are: `deviceDefault`, `blockAll`, `allowAll`.</span></span>|
|<span data-ttu-id="d9a52-176">userRightsAccessCredentialManagerAsTrustedCaller</span><span class="sxs-lookup"><span data-stu-id="d9a52-176">userRightsAccessCredentialManagerAsTrustedCaller</span></span>|[<span data-ttu-id="d9a52-177">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="d9a52-177">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="d9a52-178">此用户权限备份/还原过程中使用的凭据管理器中。</span><span class="sxs-lookup"><span data-stu-id="d9a52-178">This user right is used by Credential Manager during Backup/Restore.</span></span> <span data-ttu-id="d9a52-179">用户的已保存的凭据可能受到威胁，如果此权限授予的其他实体。</span><span class="sxs-lookup"><span data-stu-id="d9a52-179">Users' saved credentials might be compromised if this privilege is given to other entities.</span></span> <span data-ttu-id="d9a52-180">支持状态 NotConfigured 和允许</span><span class="sxs-lookup"><span data-stu-id="d9a52-180">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="d9a52-181">userRightsAllowAccessFromNetwork</span><span class="sxs-lookup"><span data-stu-id="d9a52-181">userRightsAllowAccessFromNetwork</span></span>|[<span data-ttu-id="d9a52-182">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="d9a52-182">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="d9a52-183">此用户权限确定哪些用户和组允许通过网络连接到计算机。</span><span class="sxs-lookup"><span data-stu-id="d9a52-183">This user right determines which users and groups are allowed to connect to the computer over the network.</span></span> <span data-ttu-id="d9a52-184">支持状态允许。</span><span class="sxs-lookup"><span data-stu-id="d9a52-184">State Allowed is supported.</span></span>|
|<span data-ttu-id="d9a52-185">userRightsBlockAccessFromNetwork</span><span class="sxs-lookup"><span data-stu-id="d9a52-185">userRightsBlockAccessFromNetwork</span></span>|[<span data-ttu-id="d9a52-186">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="d9a52-186">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="d9a52-187">此用户权限确定哪些用户和组是通过网络连接到计算机的块。</span><span class="sxs-lookup"><span data-stu-id="d9a52-187">This user right determines which users and groups are block from connecting to the computer over the network.</span></span> <span data-ttu-id="d9a52-188">支持状态块。</span><span class="sxs-lookup"><span data-stu-id="d9a52-188">State Block is supported.</span></span>|
|<span data-ttu-id="d9a52-189">userRightsActAsPartOfTheOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="d9a52-189">userRightsActAsPartOfTheOperatingSystem</span></span>|[<span data-ttu-id="d9a52-190">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="d9a52-190">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="d9a52-191">此用户权限允许模拟任何用户无需身份验证的过程。</span><span class="sxs-lookup"><span data-stu-id="d9a52-191">This user right allows a process to impersonate any user without authentication.</span></span> <span data-ttu-id="d9a52-192">过程因此可以访问与该用户相同的本地资源。</span><span class="sxs-lookup"><span data-stu-id="d9a52-192">The process can therefore gain access to the same local resources as that user.</span></span> <span data-ttu-id="d9a52-193">支持状态 NotConfigured 和允许</span><span class="sxs-lookup"><span data-stu-id="d9a52-193">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="d9a52-194">userRightsLocalLogOn</span><span class="sxs-lookup"><span data-stu-id="d9a52-194">userRightsLocalLogOn</span></span>|[<span data-ttu-id="d9a52-195">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="d9a52-195">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="d9a52-196">此用户权限确定哪些用户可以登录到计算机。</span><span class="sxs-lookup"><span data-stu-id="d9a52-196">This user right determines which users can log on to the computer.</span></span> <span data-ttu-id="d9a52-197">状态 NotConfigured、 允许和已阻止所有支持</span><span class="sxs-lookup"><span data-stu-id="d9a52-197">States NotConfigured, Allowed and Blocked are all supported</span></span> |
|<span data-ttu-id="d9a52-198">userRightsBackupData</span><span class="sxs-lookup"><span data-stu-id="d9a52-198">userRightsBackupData</span></span>|[<span data-ttu-id="d9a52-199">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="d9a52-199">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="d9a52-200">此用户权限确定哪些用户可以跳过文件、 目录、 注册表和其他永久对象权限时备份文件和目录。</span><span class="sxs-lookup"><span data-stu-id="d9a52-200">This user right determines which users can bypass file, directory, registry, and other persistent objects permissions when backing up files and directories.</span></span> <span data-ttu-id="d9a52-201">支持状态 NotConfigured 和允许</span><span class="sxs-lookup"><span data-stu-id="d9a52-201">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="d9a52-202">userRightsChangeSystemTime</span><span class="sxs-lookup"><span data-stu-id="d9a52-202">userRightsChangeSystemTime</span></span>|[<span data-ttu-id="d9a52-203">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="d9a52-203">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="d9a52-204">此用户权限确定哪些用户和组可以更改计算机内部时钟的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="d9a52-204">This user right determines which users and groups can change the time and date on the internal clock of the computer.</span></span> <span data-ttu-id="d9a52-205">支持状态 NotConfigured 和允许</span><span class="sxs-lookup"><span data-stu-id="d9a52-205">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="d9a52-206">userRightsCreateGlobalObjects</span><span class="sxs-lookup"><span data-stu-id="d9a52-206">userRightsCreateGlobalObjects</span></span>|[<span data-ttu-id="d9a52-207">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="d9a52-207">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="d9a52-208">此安全设置确定用户是否可以创建可供所有会话的全局对象。</span><span class="sxs-lookup"><span data-stu-id="d9a52-208">This security setting determines whether users can create global objects that are available to all sessions.</span></span> <span data-ttu-id="d9a52-209">可以创建全局对象的用户可能会影响其他用户的会话，这可能导致应用程序故障或数据损坏下运行的进程。</span><span class="sxs-lookup"><span data-stu-id="d9a52-209">Users who can create global objects could affect processes that run under other users' sessions, which could lead to application failure or data corruption.</span></span> <span data-ttu-id="d9a52-210">支持状态 NotConfigured 和允许</span><span class="sxs-lookup"><span data-stu-id="d9a52-210">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="d9a52-211">userRightsCreatePageFile</span><span class="sxs-lookup"><span data-stu-id="d9a52-211">userRightsCreatePageFile</span></span>|[<span data-ttu-id="d9a52-212">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="d9a52-212">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="d9a52-213">此用户权限确定哪些用户和组可以呼叫内部 API 创建和更改页面文件的大小。</span><span class="sxs-lookup"><span data-stu-id="d9a52-213">This user right determines which users and groups can call an internal API to create and change the size of a page file.</span></span> <span data-ttu-id="d9a52-214">支持状态 NotConfigured 和允许</span><span class="sxs-lookup"><span data-stu-id="d9a52-214">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="d9a52-215">userRightsCreatePermanentSharedObjects</span><span class="sxs-lookup"><span data-stu-id="d9a52-215">userRightsCreatePermanentSharedObjects</span></span>|[<span data-ttu-id="d9a52-216">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="d9a52-216">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="d9a52-217">此用户权限确定哪些帐户可用于通过流程管理器中创建使用对象的目录对象。</span><span class="sxs-lookup"><span data-stu-id="d9a52-217">This user right determines which accounts can be used by processes to create a directory object using the object manager.</span></span> <span data-ttu-id="d9a52-218">支持状态 NotConfigured 和允许</span><span class="sxs-lookup"><span data-stu-id="d9a52-218">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="d9a52-219">userRightsCreateSymbolicLinks</span><span class="sxs-lookup"><span data-stu-id="d9a52-219">userRightsCreateSymbolicLinks</span></span>|[<span data-ttu-id="d9a52-220">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="d9a52-220">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="d9a52-221">此用户权限确定是否用户可以从与他们登录到计算机创建符号链接。</span><span class="sxs-lookup"><span data-stu-id="d9a52-221">This user right determines if the user can create a symbolic link from the computer to which they are logged on.</span></span> <span data-ttu-id="d9a52-222">支持状态 NotConfigured 和允许</span><span class="sxs-lookup"><span data-stu-id="d9a52-222">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="d9a52-223">userRightsCreateToken</span><span class="sxs-lookup"><span data-stu-id="d9a52-223">userRightsCreateToken</span></span>|[<span data-ttu-id="d9a52-224">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="d9a52-224">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="d9a52-225">此用户权限确定哪些用户/组可以由进程来创建用于时过程使用内部 API 来创建访问令牌获取对任何本地资源的访问令牌。</span><span class="sxs-lookup"><span data-stu-id="d9a52-225">This user right determines which users/groups can be used by processes to create a token that can then be used to get access to any local resources when the process uses an internal API to create an access token.</span></span> <span data-ttu-id="d9a52-226">支持状态 NotConfigured 和允许</span><span class="sxs-lookup"><span data-stu-id="d9a52-226">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="d9a52-227">userRightsDebugPrograms</span><span class="sxs-lookup"><span data-stu-id="d9a52-227">userRightsDebugPrograms</span></span>|[<span data-ttu-id="d9a52-228">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="d9a52-228">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="d9a52-229">此用户权限确定哪些用户可以将调试器附加到任何进程或内核。</span><span class="sxs-lookup"><span data-stu-id="d9a52-229">This user right determines which users can attach a debugger to any process or to the kernel.</span></span> <span data-ttu-id="d9a52-230">支持状态 NotConfigured 和允许</span><span class="sxs-lookup"><span data-stu-id="d9a52-230">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="d9a52-231">userRightsRemoteDesktopServicesLogOn</span><span class="sxs-lookup"><span data-stu-id="d9a52-231">userRightsRemoteDesktopServicesLogOn</span></span>|[<span data-ttu-id="d9a52-232">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="d9a52-232">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="d9a52-233">此用户权限确定禁止哪些用户和组作为远程桌面服务客户端登录。</span><span class="sxs-lookup"><span data-stu-id="d9a52-233">This user right determines which users and groups are prohibited from logging on as a Remote Desktop Services client.</span></span> <span data-ttu-id="d9a52-234">支持状态 NotConfigured 和被阻止</span><span class="sxs-lookup"><span data-stu-id="d9a52-234">Only states NotConfigured and Blocked are supported</span></span>|
|<span data-ttu-id="d9a52-235">userRightsDelegation</span><span class="sxs-lookup"><span data-stu-id="d9a52-235">userRightsDelegation</span></span>|[<span data-ttu-id="d9a52-236">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="d9a52-236">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="d9a52-237">此用户权限确定哪些用户可以在用户或计算机对象上设置委派设置受信任。</span><span class="sxs-lookup"><span data-stu-id="d9a52-237">This user right determines which users can set the Trusted for Delegation setting on a user or computer object.</span></span> <span data-ttu-id="d9a52-238">支持状态 NotConfigured 和允许。</span><span class="sxs-lookup"><span data-stu-id="d9a52-238">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="d9a52-239">userRightsGenerateSecurityAudits</span><span class="sxs-lookup"><span data-stu-id="d9a52-239">userRightsGenerateSecurityAudits</span></span>|[<span data-ttu-id="d9a52-240">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="d9a52-240">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="d9a52-241">此用户权限确定哪些帐户可用于由进程将条目添加到安全日志。</span><span class="sxs-lookup"><span data-stu-id="d9a52-241">This user right determines which accounts can be used by a process to add entries to the security log.</span></span> <span data-ttu-id="d9a52-242">安全日志用于跟踪未经授权的系统的访问。</span><span class="sxs-lookup"><span data-stu-id="d9a52-242">The security log is used to trace unauthorized system access.</span></span>  <span data-ttu-id="d9a52-243">支持状态 NotConfigured 和允许。</span><span class="sxs-lookup"><span data-stu-id="d9a52-243">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="d9a52-244">userRightsImpersonateClient</span><span class="sxs-lookup"><span data-stu-id="d9a52-244">userRightsImpersonateClient</span></span>|[<span data-ttu-id="d9a52-245">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="d9a52-245">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="d9a52-246">分配给用户此用户权限允许代表该用户模拟客户端运行的程序。</span><span class="sxs-lookup"><span data-stu-id="d9a52-246">Assigning this user right to a user allows programs running on behalf of that user to impersonate a client.</span></span> <span data-ttu-id="d9a52-247">对于此种模拟需要此用户权限可防止未经授权的用户从诱使客户端连接到他们创建的服务，然后这样可以将提升未经授权的用户的权限模拟该客户端，管理或系统级别。</span><span class="sxs-lookup"><span data-stu-id="d9a52-247">Requiring this user right for this kind of impersonation prevents an unauthorized user from convincing a client to connect to a service that they have created and then impersonating that client, which can elevate the unauthorized user's permissions to administrative or system levels.</span></span> <span data-ttu-id="d9a52-248">支持状态 NotConfigured 和允许。</span><span class="sxs-lookup"><span data-stu-id="d9a52-248">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="d9a52-249">userRightsIncreaseSchedulingPriority</span><span class="sxs-lookup"><span data-stu-id="d9a52-249">userRightsIncreaseSchedulingPriority</span></span>|[<span data-ttu-id="d9a52-250">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="d9a52-250">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="d9a52-251">此用户权限确定哪些帐户可用于过程写入属性访问另一个进程增加分配给其他进程的执行优先级。</span><span class="sxs-lookup"><span data-stu-id="d9a52-251">This user right determines which accounts can use a process with Write Property access to another process to increase the execution priority assigned to the other process.</span></span> <span data-ttu-id="d9a52-252">支持状态 NotConfigured 和允许。</span><span class="sxs-lookup"><span data-stu-id="d9a52-252">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="d9a52-253">userRightsLoadUnloadDrivers</span><span class="sxs-lookup"><span data-stu-id="d9a52-253">userRightsLoadUnloadDrivers</span></span>|[<span data-ttu-id="d9a52-254">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="d9a52-254">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="d9a52-255">此用户权限确定哪些用户可以动态加载和卸载设备驱动程序或内核模式中的其他代码。</span><span class="sxs-lookup"><span data-stu-id="d9a52-255">This user right determines which users can dynamically load and unload device drivers or other code in to kernel mode.</span></span> <span data-ttu-id="d9a52-256">支持状态 NotConfigured 和允许。</span><span class="sxs-lookup"><span data-stu-id="d9a52-256">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="d9a52-257">userRightsLockMemory</span><span class="sxs-lookup"><span data-stu-id="d9a52-257">userRightsLockMemory</span></span>|[<span data-ttu-id="d9a52-258">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="d9a52-258">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="d9a52-259">此用户权限确定哪些帐户可使用过程可在物理内存，防止系统分页数据写到磁盘上的虚拟内存中保留数据。</span><span class="sxs-lookup"><span data-stu-id="d9a52-259">This user right determines which accounts can use a process to keep data in physical memory, which prevents the system from paging the data to virtual memory on disk.</span></span> <span data-ttu-id="d9a52-260">支持状态 NotConfigured 和允许。</span><span class="sxs-lookup"><span data-stu-id="d9a52-260">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="d9a52-261">userRightsManageAuditingAndSecurityLogs</span><span class="sxs-lookup"><span data-stu-id="d9a52-261">userRightsManageAuditingAndSecurityLogs</span></span>|[<span data-ttu-id="d9a52-262">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="d9a52-262">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="d9a52-263">此用户权限确定哪些用户可以指定对象访问审核各个资源，如文件、 Active Directory 对象和注册表项选项。</span><span class="sxs-lookup"><span data-stu-id="d9a52-263">This user right determines which users can specify object access auditing options for individual resources, such as files, Active Directory objects, and registry keys.</span></span> <span data-ttu-id="d9a52-264">支持状态 NotConfigured 和允许。</span><span class="sxs-lookup"><span data-stu-id="d9a52-264">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="d9a52-265">userRightsManageVolumes</span><span class="sxs-lookup"><span data-stu-id="d9a52-265">userRightsManageVolumes</span></span>|[<span data-ttu-id="d9a52-266">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="d9a52-266">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="d9a52-267">此用户权限确定哪些用户和组可以在卷上，如远程磁盘碎片整理运行维护任务。</span><span class="sxs-lookup"><span data-stu-id="d9a52-267">This user right determines which users and groups can run maintenance tasks on a volume, such as remote defragmentation.</span></span> <span data-ttu-id="d9a52-268">支持状态 NotConfigured 和允许。</span><span class="sxs-lookup"><span data-stu-id="d9a52-268">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="d9a52-269">userRightsModifyFirmwareEnvironment</span><span class="sxs-lookup"><span data-stu-id="d9a52-269">userRightsModifyFirmwareEnvironment</span></span>|[<span data-ttu-id="d9a52-270">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="d9a52-270">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="d9a52-271">此用户权限确定谁可以修改固件环境值。</span><span class="sxs-lookup"><span data-stu-id="d9a52-271">This user right determines who can modify firmware environment values.</span></span> <span data-ttu-id="d9a52-272">支持状态 NotConfigured 和允许。</span><span class="sxs-lookup"><span data-stu-id="d9a52-272">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="d9a52-273">userRightsModifyObjectLabels</span><span class="sxs-lookup"><span data-stu-id="d9a52-273">userRightsModifyObjectLabels</span></span>|[<span data-ttu-id="d9a52-274">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="d9a52-274">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="d9a52-275">此用户权限确定哪些用户帐户可以修改对象，如文件、 注册表项或由其他用户拥有的进程的完整性标签。</span><span class="sxs-lookup"><span data-stu-id="d9a52-275">This user right determines which user accounts can modify the integrity label of objects, such as files, registry keys, or processes owned by other users.</span></span> <span data-ttu-id="d9a52-276">支持状态 NotConfigured 和允许。</span><span class="sxs-lookup"><span data-stu-id="d9a52-276">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="d9a52-277">userRightsProfileSingleProcess</span><span class="sxs-lookup"><span data-stu-id="d9a52-277">userRightsProfileSingleProcess</span></span>|[<span data-ttu-id="d9a52-278">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="d9a52-278">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="d9a52-279">此用户权限确定哪些用户可以使用性能监视工具来监视系统进程的性能。</span><span class="sxs-lookup"><span data-stu-id="d9a52-279">This user right determines which users can use performance monitoring tools to monitor the performance of system processes.</span></span> <span data-ttu-id="d9a52-280">支持状态 NotConfigured 和允许。</span><span class="sxs-lookup"><span data-stu-id="d9a52-280">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="d9a52-281">userRightsRemoteShutdown</span><span class="sxs-lookup"><span data-stu-id="d9a52-281">userRightsRemoteShutdown</span></span>|[<span data-ttu-id="d9a52-282">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="d9a52-282">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="d9a52-283">此用户权限确定允许哪些用户关闭，将计算机从网络上的远程位置。</span><span class="sxs-lookup"><span data-stu-id="d9a52-283">This user right determines which users are allowed to shut down a computer from a remote location on the network.</span></span> <span data-ttu-id="d9a52-284">此用户权限的误用会导致拒绝服务。</span><span class="sxs-lookup"><span data-stu-id="d9a52-284">Misuse of this user right can result in a denial of service.</span></span> <span data-ttu-id="d9a52-285">支持状态 NotConfigured 和允许。</span><span class="sxs-lookup"><span data-stu-id="d9a52-285">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="d9a52-286">userRightsRestoreData</span><span class="sxs-lookup"><span data-stu-id="d9a52-286">userRightsRestoreData</span></span>|[<span data-ttu-id="d9a52-287">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="d9a52-287">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="d9a52-288">此用户权限决定哪些用户可以跳过文件、 目录、 注册表和权限还原时备份文件和目录，其他持久对象，决定哪些用户可以设置为对象的所有者的任何有效的安全主体。</span><span class="sxs-lookup"><span data-stu-id="d9a52-288">This user right determines which users can bypass file, directory, registry, and other persistent objects permissions when restoring backed up files and directories, and determines which users can set any valid security principal as the owner of an object.</span></span> <span data-ttu-id="d9a52-289">支持状态 NotConfigured 和允许。</span><span class="sxs-lookup"><span data-stu-id="d9a52-289">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="d9a52-290">userRightsTakeOwnership</span><span class="sxs-lookup"><span data-stu-id="d9a52-290">userRightsTakeOwnership</span></span>|[<span data-ttu-id="d9a52-291">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="d9a52-291">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="d9a52-292">此用户权限决定哪些用户可以在系统中，包括 Active Directory 对象、 文件和文件夹、 打印机、 注册表项、 流程和线程执行任何安全对象的所有权。</span><span class="sxs-lookup"><span data-stu-id="d9a52-292">This user right determines which users can take ownership of any securable object in the system, including Active Directory objects, files and folders, printers, registry keys, processes, and threads.</span></span> <span data-ttu-id="d9a52-293">支持状态 NotConfigured 和允许。</span><span class="sxs-lookup"><span data-stu-id="d9a52-293">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="d9a52-294">userRightsRegisterProcessAsService</span><span class="sxs-lookup"><span data-stu-id="d9a52-294">userRightsRegisterProcessAsService</span></span>|[<span data-ttu-id="d9a52-295">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="d9a52-295">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="d9a52-296">此安全设置确定被阻止的服务帐户注册为服务的进程。</span><span class="sxs-lookup"><span data-stu-id="d9a52-296">This security setting determines which service accounts are prevented from registering a process as a service.</span></span> <span data-ttu-id="d9a52-297">注意： 此安全设置不适用于系统、 本地服务或网络服务帐户。</span><span class="sxs-lookup"><span data-stu-id="d9a52-297">Note: This security setting does not apply to the System, Local Service, or Network Service accounts.</span></span> <span data-ttu-id="d9a52-298">仅支持已阻止的状态。</span><span class="sxs-lookup"><span data-stu-id="d9a52-298">Only state Blocked is supported.</span></span>|
|<span data-ttu-id="d9a52-299">xboxServicesEnableXboxGameSaveTask</span><span class="sxs-lookup"><span data-stu-id="d9a52-299">xboxServicesEnableXboxGameSaveTask</span></span>|<span data-ttu-id="d9a52-300">Boolean</span><span class="sxs-lookup"><span data-stu-id="d9a52-300">Boolean</span></span>|<span data-ttu-id="d9a52-301">此设置确定 xbox 游戏保存是否启用 (1) 或禁用 (0)。</span><span class="sxs-lookup"><span data-stu-id="d9a52-301">This setting determines whether xbox game save is enabled (1) or disabled (0).</span></span>|
|<span data-ttu-id="d9a52-302">xboxServicesAccessoryManagementServiceStartupMode</span><span class="sxs-lookup"><span data-stu-id="d9a52-302">xboxServicesAccessoryManagementServiceStartupMode</span></span>|[<span data-ttu-id="d9a52-303">serviceStartType</span><span class="sxs-lookup"><span data-stu-id="d9a52-303">serviceStartType</span></span>](../resources/intune-deviceconfig-servicestarttype.md)|<span data-ttu-id="d9a52-304">此设置确定的附件管理服务启动类型是 Automatic(2) Manual(3)、 Disabled(4)。</span><span class="sxs-lookup"><span data-stu-id="d9a52-304">This setting determines whether the Accessory management service's start type is Automatic(2), Manual(3), Disabled(4).</span></span> <span data-ttu-id="d9a52-305">默认： 手动。</span><span class="sxs-lookup"><span data-stu-id="d9a52-305">Default: Manual.</span></span> <span data-ttu-id="d9a52-306">可取值为：`manual`、`automatic`、`disabled`。</span><span class="sxs-lookup"><span data-stu-id="d9a52-306">Possible values are: `manual`, `automatic`, `disabled`.</span></span>|
|<span data-ttu-id="d9a52-307">xboxServicesLiveAuthManagerServiceStartupMode</span><span class="sxs-lookup"><span data-stu-id="d9a52-307">xboxServicesLiveAuthManagerServiceStartupMode</span></span>|[<span data-ttu-id="d9a52-308">serviceStartType</span><span class="sxs-lookup"><span data-stu-id="d9a52-308">serviceStartType</span></span>](../resources/intune-deviceconfig-servicestarttype.md)|<span data-ttu-id="d9a52-309">此设置确定 Live 身份验证管理器服务启动类型是 Automatic(2) Manual(3)、 Disabled(4)。</span><span class="sxs-lookup"><span data-stu-id="d9a52-309">This setting determines whether Live Auth Manager service's start type is Automatic(2), Manual(3), Disabled(4).</span></span> <span data-ttu-id="d9a52-310">默认： 手动。</span><span class="sxs-lookup"><span data-stu-id="d9a52-310">Default: Manual.</span></span> <span data-ttu-id="d9a52-311">可取值为：`manual`、`automatic`、`disabled`。</span><span class="sxs-lookup"><span data-stu-id="d9a52-311">Possible values are: `manual`, `automatic`, `disabled`.</span></span>|
|<span data-ttu-id="d9a52-312">xboxServicesLiveGameSaveServiceStartupMode</span><span class="sxs-lookup"><span data-stu-id="d9a52-312">xboxServicesLiveGameSaveServiceStartupMode</span></span>|[<span data-ttu-id="d9a52-313">serviceStartType</span><span class="sxs-lookup"><span data-stu-id="d9a52-313">serviceStartType</span></span>](../resources/intune-deviceconfig-servicestarttype.md)|<span data-ttu-id="d9a52-314">此设置确定是否 Automatic(2) Manual(3)、 Disabled(4) Live 保存服务的启动类型的游戏。</span><span class="sxs-lookup"><span data-stu-id="d9a52-314">This setting determines whether Live Game save service's start type is Automatic(2), Manual(3), Disabled(4).</span></span> <span data-ttu-id="d9a52-315">默认： 手动。</span><span class="sxs-lookup"><span data-stu-id="d9a52-315">Default: Manual.</span></span> <span data-ttu-id="d9a52-316">可取值为：`manual`、`automatic`、`disabled`。</span><span class="sxs-lookup"><span data-stu-id="d9a52-316">Possible values are: `manual`, `automatic`, `disabled`.</span></span>|
|<span data-ttu-id="d9a52-317">xboxServicesLiveNetworkingServiceStartupMode</span><span class="sxs-lookup"><span data-stu-id="d9a52-317">xboxServicesLiveNetworkingServiceStartupMode</span></span>|[<span data-ttu-id="d9a52-318">serviceStartType</span><span class="sxs-lookup"><span data-stu-id="d9a52-318">serviceStartType</span></span>](../resources/intune-deviceconfig-servicestarttype.md)|<span data-ttu-id="d9a52-319">此设置确定网络服务启动类型是 Automatic(2) Manual(3)、 Disabled(4)。</span><span class="sxs-lookup"><span data-stu-id="d9a52-319">This setting determines whether Networking service's start type is Automatic(2), Manual(3), Disabled(4).</span></span> <span data-ttu-id="d9a52-320">默认： 手动。</span><span class="sxs-lookup"><span data-stu-id="d9a52-320">Default: Manual.</span></span> <span data-ttu-id="d9a52-321">可取值为：`manual`、`automatic`、`disabled`。</span><span class="sxs-lookup"><span data-stu-id="d9a52-321">Possible values are: `manual`, `automatic`, `disabled`.</span></span>|
|<span data-ttu-id="d9a52-322">localSecurityOptionsBlockMicrosoftAccounts</span><span class="sxs-lookup"><span data-stu-id="d9a52-322">localSecurityOptionsBlockMicrosoftAccounts</span></span>|<span data-ttu-id="d9a52-323">Boolean</span><span class="sxs-lookup"><span data-stu-id="d9a52-323">Boolean</span></span>|<span data-ttu-id="d9a52-324">禁止用户添加到此计算机的新的 Microsoft 帐户。</span><span class="sxs-lookup"><span data-stu-id="d9a52-324">Prevent users from adding new Microsoft accounts to this computer.</span></span>|
|<span data-ttu-id="d9a52-325">localSecurityOptionsBlockRemoteLogonWithBlankPassword</span><span class="sxs-lookup"><span data-stu-id="d9a52-325">localSecurityOptionsBlockRemoteLogonWithBlankPassword</span></span>|<span data-ttu-id="d9a52-326">Boolean</span><span class="sxs-lookup"><span data-stu-id="d9a52-326">Boolean</span></span>|<span data-ttu-id="d9a52-327">启用本地帐户不受密码保护登录从物理设备以外的位置。将启用默认值</span><span class="sxs-lookup"><span data-stu-id="d9a52-327">Enable Local accounts that are not password protected to log on from locations other than the physical device.Default is enabled</span></span>|
|<span data-ttu-id="d9a52-328">localSecurityOptionsDisableAdministratorAccount</span><span class="sxs-lookup"><span data-stu-id="d9a52-328">localSecurityOptionsDisableAdministratorAccount</span></span>|<span data-ttu-id="d9a52-329">Boolean</span><span class="sxs-lookup"><span data-stu-id="d9a52-329">Boolean</span></span>|<span data-ttu-id="d9a52-330">确定是否启用或禁用的本地管理员帐户。</span><span class="sxs-lookup"><span data-stu-id="d9a52-330">Determines whether the Local Administrator account is enabled or disabled.</span></span>|
|<span data-ttu-id="d9a52-331">localSecurityOptionsAdministratorAccountName</span><span class="sxs-lookup"><span data-stu-id="d9a52-331">localSecurityOptionsAdministratorAccountName</span></span>|<span data-ttu-id="d9a52-332">String</span><span class="sxs-lookup"><span data-stu-id="d9a52-332">String</span></span>|<span data-ttu-id="d9a52-333">定义要与"管理员"的帐户的安全标识符 (SID) 关联的不同的帐户名称。</span><span class="sxs-lookup"><span data-stu-id="d9a52-333">Define a different account name to be associated with the security identifier (SID) for the account “Administrator”.</span></span>|
|<span data-ttu-id="d9a52-334">localSecurityOptionsDisableGuestAccount</span><span class="sxs-lookup"><span data-stu-id="d9a52-334">localSecurityOptionsDisableGuestAccount</span></span>|<span data-ttu-id="d9a52-335">Boolean</span><span class="sxs-lookup"><span data-stu-id="d9a52-335">Boolean</span></span>|<span data-ttu-id="d9a52-336">确定是启用还是禁用来宾帐户。</span><span class="sxs-lookup"><span data-stu-id="d9a52-336">Determines if the Guest account is enabled or disabled.</span></span>|
|<span data-ttu-id="d9a52-337">localSecurityOptionsGuestAccountName</span><span class="sxs-lookup"><span data-stu-id="d9a52-337">localSecurityOptionsGuestAccountName</span></span>|<span data-ttu-id="d9a52-338">String</span><span class="sxs-lookup"><span data-stu-id="d9a52-338">String</span></span>|<span data-ttu-id="d9a52-339">定义要为"来宾"的帐户的安全标识符 (SID) 关联的不同的帐户名称。</span><span class="sxs-lookup"><span data-stu-id="d9a52-339">Define a different account name to be associated with the security identifier (SID) for the account “Guest”.</span></span>|
|<span data-ttu-id="d9a52-340">localSecurityOptionsAllowUndockWithoutHavingToLogon</span><span class="sxs-lookup"><span data-stu-id="d9a52-340">localSecurityOptionsAllowUndockWithoutHavingToLogon</span></span>|<span data-ttu-id="d9a52-341">Boolean</span><span class="sxs-lookup"><span data-stu-id="d9a52-341">Boolean</span></span>|<span data-ttu-id="d9a52-342">正在取消停靠而无需登录阻止便携式计算机。</span><span class="sxs-lookup"><span data-stu-id="d9a52-342">Prevent a portable computer from being undocked without having to log in.</span></span>|
|<span data-ttu-id="d9a52-343">localSecurityOptionsBlockUsersInstallingPrinterDrivers</span><span class="sxs-lookup"><span data-stu-id="d9a52-343">localSecurityOptionsBlockUsersInstallingPrinterDrivers</span></span>|<span data-ttu-id="d9a52-344">Boolean</span><span class="sxs-lookup"><span data-stu-id="d9a52-344">Boolean</span></span>|<span data-ttu-id="d9a52-345">限制为连接到向管理员仅共享打印机的一部分安装的打印机驱动程序。</span><span class="sxs-lookup"><span data-stu-id="d9a52-345">Restrict installing printer drivers as part of connecting to a shared printer to admins only.</span></span>|
|<span data-ttu-id="d9a52-346">localSecurityOptionsBlockRemoteOpticalDriveAccess</span><span class="sxs-lookup"><span data-stu-id="d9a52-346">localSecurityOptionsBlockRemoteOpticalDriveAccess</span></span>|<span data-ttu-id="d9a52-347">Boolean</span><span class="sxs-lookup"><span data-stu-id="d9a52-347">Boolean</span></span>|<span data-ttu-id="d9a52-348">启用此设置允许访问 CD-ROM 媒体仅以交互方式登录的用户。</span><span class="sxs-lookup"><span data-stu-id="d9a52-348">Enabling this settings allows only interactively logged on user to access CD-ROM media.</span></span>|
|<span data-ttu-id="d9a52-349">localSecurityOptionsFormatAndEjectOfRemovableMediaAllowedUser</span><span class="sxs-lookup"><span data-stu-id="d9a52-349">localSecurityOptionsFormatAndEjectOfRemovableMediaAllowedUser</span></span>|[<span data-ttu-id="d9a52-350">localSecurityOptionsFormatAndEjectOfRemovableMediaAllowedUserType</span><span class="sxs-lookup"><span data-stu-id="d9a52-350">localSecurityOptionsFormatAndEjectOfRemovableMediaAllowedUserType</span></span>](../resources/intune-deviceconfig-localsecurityoptionsformatandejectofremovablemediaallowedusertype.md)|<span data-ttu-id="d9a52-351">定义允许谁格式化和弹出可移动 NTFS 媒体。</span><span class="sxs-lookup"><span data-stu-id="d9a52-351">Define who is allowed to format and eject removable NTFS media.</span></span> <span data-ttu-id="d9a52-352">可取值为：`notConfigured`、`administrators`、`administratorsAndPowerUsers`、`administratorsAndInteractiveUsers`。</span><span class="sxs-lookup"><span data-stu-id="d9a52-352">Possible values are: `notConfigured`, `administrators`, `administratorsAndPowerUsers`, `administratorsAndInteractiveUsers`.</span></span>|
|<span data-ttu-id="d9a52-353">localSecurityOptionsMachineInactivityLimit</span><span class="sxs-lookup"><span data-stu-id="d9a52-353">localSecurityOptionsMachineInactivityLimit</span></span>|<span data-ttu-id="d9a52-354">Int32</span><span class="sxs-lookup"><span data-stu-id="d9a52-354">Int32</span></span>|<span data-ttu-id="d9a52-355">交互式桌面上登录屏幕上定义最大分钟无活动，直到屏幕保护程序运行。</span><span class="sxs-lookup"><span data-stu-id="d9a52-355">Define maximum minutes of inactivity on the interactive desktop’s login screen until the screen saver runs.</span></span> <span data-ttu-id="d9a52-356">有效的值 0 到 9999 之间</span><span class="sxs-lookup"><span data-stu-id="d9a52-356">Valid values 0 to 9999</span></span>|
|<span data-ttu-id="d9a52-357">localSecurityOptionsMachineInactivityLimitInMinutes</span><span class="sxs-lookup"><span data-stu-id="d9a52-357">localSecurityOptionsMachineInactivityLimitInMinutes</span></span>|<span data-ttu-id="d9a52-358">Int32</span><span class="sxs-lookup"><span data-stu-id="d9a52-358">Int32</span></span>|<span data-ttu-id="d9a52-359">交互式桌面上登录屏幕上定义最大分钟无活动，直到屏幕保护程序运行。</span><span class="sxs-lookup"><span data-stu-id="d9a52-359">Define maximum minutes of inactivity on the interactive desktop’s login screen until the screen saver runs.</span></span> <span data-ttu-id="d9a52-360">有效的值 0 到 9999 之间</span><span class="sxs-lookup"><span data-stu-id="d9a52-360">Valid values 0 to 9999</span></span>|
|<span data-ttu-id="d9a52-361">localSecurityOptionsDoNotRequireCtrlAltDel</span><span class="sxs-lookup"><span data-stu-id="d9a52-361">localSecurityOptionsDoNotRequireCtrlAltDel</span></span>|<span data-ttu-id="d9a52-362">Boolean</span><span class="sxs-lookup"><span data-stu-id="d9a52-362">Boolean</span></span>|<span data-ttu-id="d9a52-363">需要 CTRL + ALT + DEL 要按用户登录之前。</span><span class="sxs-lookup"><span data-stu-id="d9a52-363">Require CTRL+ALT+DEL to be pressed before a user can log on.</span></span>|
|<span data-ttu-id="d9a52-364">localSecurityOptionsHideLastSignedInUser</span><span class="sxs-lookup"><span data-stu-id="d9a52-364">localSecurityOptionsHideLastSignedInUser</span></span>|<span data-ttu-id="d9a52-365">Boolean</span><span class="sxs-lookup"><span data-stu-id="d9a52-365">Boolean</span></span>|<span data-ttu-id="d9a52-366">不在此设备上显示的签名的最后一个人的用户名。</span><span class="sxs-lookup"><span data-stu-id="d9a52-366">Do not display the username of the last person who signed in on this device.</span></span>|
|<span data-ttu-id="d9a52-367">localSecurityOptionsHideUsernameAtSignIn</span><span class="sxs-lookup"><span data-stu-id="d9a52-367">localSecurityOptionsHideUsernameAtSignIn</span></span>|<span data-ttu-id="d9a52-368">Boolean</span><span class="sxs-lookup"><span data-stu-id="d9a52-368">Boolean</span></span>|<span data-ttu-id="d9a52-369">不显示登录到此设备输入凭据之后和之前显示设备的桌面的人员的用户名。</span><span class="sxs-lookup"><span data-stu-id="d9a52-369">Do not display the username of the person signing in to this device after credentials are entered and before the device’s desktop is shown.</span></span>|
|<span data-ttu-id="d9a52-370">localSecurityOptionsLogOnMessageTitle</span><span class="sxs-lookup"><span data-stu-id="d9a52-370">localSecurityOptionsLogOnMessageTitle</span></span>|<span data-ttu-id="d9a52-371">String</span><span class="sxs-lookup"><span data-stu-id="d9a52-371">String</span></span>|<span data-ttu-id="d9a52-372">用户尝试登录的设置邮件标题。</span><span class="sxs-lookup"><span data-stu-id="d9a52-372">Set message title for users attempting to log in.</span></span>|
|<span data-ttu-id="d9a52-373">localSecurityOptionsLogOnMessageText</span><span class="sxs-lookup"><span data-stu-id="d9a52-373">localSecurityOptionsLogOnMessageText</span></span>|<span data-ttu-id="d9a52-374">String</span><span class="sxs-lookup"><span data-stu-id="d9a52-374">String</span></span>|<span data-ttu-id="d9a52-375">设置用户试图登录消息文本。</span><span class="sxs-lookup"><span data-stu-id="d9a52-375">Set message text for users attempting to log in.</span></span>|
|<span data-ttu-id="d9a52-376">localSecurityOptionsAllowPKU2UAuthenticationRequests</span><span class="sxs-lookup"><span data-stu-id="d9a52-376">localSecurityOptionsAllowPKU2UAuthenticationRequests</span></span>|<span data-ttu-id="d9a52-377">Boolean</span><span class="sxs-lookup"><span data-stu-id="d9a52-377">Boolean</span></span>|<span data-ttu-id="d9a52-378">对此设备块 PKU2U 身份验证请求使用联机标识。</span><span class="sxs-lookup"><span data-stu-id="d9a52-378">Block PKU2U authentication requests to this device to use online identities.</span></span>|
|<span data-ttu-id="d9a52-379">localSecurityOptionsAllowRemoteCallsToSecurityAccountsManagerHelperBool</span><span class="sxs-lookup"><span data-stu-id="d9a52-379">localSecurityOptionsAllowRemoteCallsToSecurityAccountsManagerHelperBool</span></span>|<span data-ttu-id="d9a52-380">Boolean</span><span class="sxs-lookup"><span data-stu-id="d9a52-380">Boolean</span></span>|<span data-ttu-id="d9a52-381">用户界面帮助程序布尔 LocalSecurityOptionsAllowRemoteCallsToSecurityAccountsManager 实体</span><span class="sxs-lookup"><span data-stu-id="d9a52-381">UI helper boolean for LocalSecurityOptionsAllowRemoteCallsToSecurityAccountsManager entity</span></span>|
|<span data-ttu-id="d9a52-382">localSecurityOptionsAllowRemoteCallsToSecurityAccountsManager</span><span class="sxs-lookup"><span data-stu-id="d9a52-382">localSecurityOptionsAllowRemoteCallsToSecurityAccountsManager</span></span>|<span data-ttu-id="d9a52-383">String</span><span class="sxs-lookup"><span data-stu-id="d9a52-383">String</span></span>|<span data-ttu-id="d9a52-384">编辑默认安全描述符定义语言字符串，以允许或拒绝远程调用 SAM 用户和组。</span><span class="sxs-lookup"><span data-stu-id="d9a52-384">Edit the default Security Descriptor Definition Language string to allow or deny users and groups to make remote calls to the SAM.</span></span>|
|<span data-ttu-id="d9a52-385">localSecurityOptionsMinimumSessionSecurityForNtlmSspBasedClients</span><span class="sxs-lookup"><span data-stu-id="d9a52-385">localSecurityOptionsMinimumSessionSecurityForNtlmSspBasedClients</span></span>|[<span data-ttu-id="d9a52-386">localSecurityOptionsMinimumSessionSecurity</span><span class="sxs-lookup"><span data-stu-id="d9a52-386">localSecurityOptionsMinimumSessionSecurity</span></span>](../resources/intune-deviceconfig-localsecurityoptionsminimumsessionsecurity.md)|<span data-ttu-id="d9a52-387">此安全设置允许客户端要求 128 位加密和/或 NTLMv2 会话安全协商。</span><span class="sxs-lookup"><span data-stu-id="d9a52-387">This security setting allows a client to require the negotiation of 128-bit encryption and/or NTLMv2 session security.</span></span> <span data-ttu-id="d9a52-388">可取值为：`none`、`requireNtmlV2SessionSecurity`、`require128BitEncryption`、`ntlmV2And128BitEncryption`。</span><span class="sxs-lookup"><span data-stu-id="d9a52-388">Possible values are: `none`, `requireNtmlV2SessionSecurity`, `require128BitEncryption`, `ntlmV2And128BitEncryption`.</span></span>|
|<span data-ttu-id="d9a52-389">localSecurityOptionsMinimumSessionSecurityForNtlmSspBasedServers</span><span class="sxs-lookup"><span data-stu-id="d9a52-389">localSecurityOptionsMinimumSessionSecurityForNtlmSspBasedServers</span></span>|[<span data-ttu-id="d9a52-390">localSecurityOptionsMinimumSessionSecurity</span><span class="sxs-lookup"><span data-stu-id="d9a52-390">localSecurityOptionsMinimumSessionSecurity</span></span>](../resources/intune-deviceconfig-localsecurityoptionsminimumsessionsecurity.md)|<span data-ttu-id="d9a52-391">此安全设置允许服务器要求 128 位加密和/或 NTLMv2 会话安全协商。</span><span class="sxs-lookup"><span data-stu-id="d9a52-391">This security setting allows a server to require the negotiation of 128-bit encryption and/or NTLMv2 session security.</span></span> <span data-ttu-id="d9a52-392">可取值为：`none`、`requireNtmlV2SessionSecurity`、`require128BitEncryption`、`ntlmV2And128BitEncryption`。</span><span class="sxs-lookup"><span data-stu-id="d9a52-392">Possible values are: `none`, `requireNtmlV2SessionSecurity`, `require128BitEncryption`, `ntlmV2And128BitEncryption`.</span></span>|
|<span data-ttu-id="d9a52-393">lanManagerAuthenticationLevel</span><span class="sxs-lookup"><span data-stu-id="d9a52-393">lanManagerAuthenticationLevel</span></span>|[<span data-ttu-id="d9a52-394">lanManagerAuthenticationLevel</span><span class="sxs-lookup"><span data-stu-id="d9a52-394">lanManagerAuthenticationLevel</span></span>](../resources/intune-deviceconfig-lanmanagerauthenticationlevel.md)|<span data-ttu-id="d9a52-395">此安全设置确定哪个质询/响应身份验证协议用于网络登录。</span><span class="sxs-lookup"><span data-stu-id="d9a52-395">This security setting determines which challenge/response authentication protocol is used for network logons.</span></span> <span data-ttu-id="d9a52-396">可取值为：`lmAndNltm`、`lmNtlmAndNtlmV2`、`lmAndNtlmOnly`、`lmAndNtlmV2`、`lmNtlmV2AndNotLm`、`lmNtlmV2AndNotLmOrNtm`。</span><span class="sxs-lookup"><span data-stu-id="d9a52-396">Possible values are: `lmAndNltm`, `lmNtlmAndNtlmV2`, `lmAndNtlmOnly`, `lmAndNtlmV2`, `lmNtlmV2AndNotLm`, `lmNtlmV2AndNotLmOrNtm`.</span></span>|
|<span data-ttu-id="d9a52-397">lanManagerWorkstationDisableInsecureGuestLogons</span><span class="sxs-lookup"><span data-stu-id="d9a52-397">lanManagerWorkstationDisableInsecureGuestLogons</span></span>|<span data-ttu-id="d9a52-398">Boolean</span><span class="sxs-lookup"><span data-stu-id="d9a52-398">Boolean</span></span>|<span data-ttu-id="d9a52-399">如果启用，则 SMB 客户端将允许不安全的来宾登录。</span><span class="sxs-lookup"><span data-stu-id="d9a52-399">If enabled,the SMB client will allow insecure guest logons.</span></span> <span data-ttu-id="d9a52-400">如果未配置，SMB 客户端将拒绝不安全的来宾登录。</span><span class="sxs-lookup"><span data-stu-id="d9a52-400">If not configured, the SMB client will reject insecure guest logons.</span></span>|
|<span data-ttu-id="d9a52-401">localSecurityOptionsClearVirtualMemoryPageFile</span><span class="sxs-lookup"><span data-stu-id="d9a52-401">localSecurityOptionsClearVirtualMemoryPageFile</span></span>|<span data-ttu-id="d9a52-402">Boolean</span><span class="sxs-lookup"><span data-stu-id="d9a52-402">Boolean</span></span>|<span data-ttu-id="d9a52-403">此安全设置确定系统关闭时是否清除虚拟内存页面文件。</span><span class="sxs-lookup"><span data-stu-id="d9a52-403">This security setting determines whether the virtual memory pagefile is cleared when the system is shut down.</span></span>|
|<span data-ttu-id="d9a52-404">localSecurityOptionsAllowSystemToBeShutDownWithoutHavingToLogOn</span><span class="sxs-lookup"><span data-stu-id="d9a52-404">localSecurityOptionsAllowSystemToBeShutDownWithoutHavingToLogOn</span></span>|<span data-ttu-id="d9a52-405">Boolean</span><span class="sxs-lookup"><span data-stu-id="d9a52-405">Boolean</span></span>|<span data-ttu-id="d9a52-406">此安全设置确定是否可以关闭计算机而无需登录到 Windows。</span><span class="sxs-lookup"><span data-stu-id="d9a52-406">This security setting determines whether a computer can be shut down without having to log on to Windows.</span></span>|
|<span data-ttu-id="d9a52-407">localSecurityOptionsAllowUIAccessApplicationElevation</span><span class="sxs-lookup"><span data-stu-id="d9a52-407">localSecurityOptionsAllowUIAccessApplicationElevation</span></span>|<span data-ttu-id="d9a52-408">Boolean</span><span class="sxs-lookup"><span data-stu-id="d9a52-408">Boolean</span></span>|<span data-ttu-id="d9a52-409">允许 UIAccess 应用程序无需使用安全桌面提示提升。</span><span class="sxs-lookup"><span data-stu-id="d9a52-409">Allow UIAccess apps to prompt for elevation without using the secure desktop.</span></span>|
|<span data-ttu-id="d9a52-410">localSecurityOptionsVirtualizeFileAndRegistryWriteFailuresToPerUserLocations</span><span class="sxs-lookup"><span data-stu-id="d9a52-410">localSecurityOptionsVirtualizeFileAndRegistryWriteFailuresToPerUserLocations</span></span>|<span data-ttu-id="d9a52-411">Boolean</span><span class="sxs-lookup"><span data-stu-id="d9a52-411">Boolean</span></span>|<span data-ttu-id="d9a52-412">虚拟化文件和注册表写入失败次数为每用户位置</span><span class="sxs-lookup"><span data-stu-id="d9a52-412">Virtualize file and registry write failures to per user locations</span></span>|
|<span data-ttu-id="d9a52-413">localSecurityOptionsOnlyElevateSignedExecutables</span><span class="sxs-lookup"><span data-stu-id="d9a52-413">localSecurityOptionsOnlyElevateSignedExecutables</span></span>|<span data-ttu-id="d9a52-414">Boolean</span><span class="sxs-lookup"><span data-stu-id="d9a52-414">Boolean</span></span>|<span data-ttu-id="d9a52-415">允许运行之前，强制实施 PKI 证书路径验证给定的可执行文件。</span><span class="sxs-lookup"><span data-stu-id="d9a52-415">Enforce PKI certification path validation for a given executable file before it is permitted to run.</span></span>|
|<span data-ttu-id="d9a52-416">localSecurityOptionsAdministratorElevationPromptBehavior</span><span class="sxs-lookup"><span data-stu-id="d9a52-416">localSecurityOptionsAdministratorElevationPromptBehavior</span></span>|[<span data-ttu-id="d9a52-417">localSecurityOptionsAdministratorElevationPromptBehaviorType</span><span class="sxs-lookup"><span data-stu-id="d9a52-417">localSecurityOptionsAdministratorElevationPromptBehaviorType</span></span>](../resources/intune-deviceconfig-localsecurityoptionsadministratorelevationpromptbehaviortype.md)|<span data-ttu-id="d9a52-418">管理员批准模式中定义管理员的提升提示的行为。</span><span class="sxs-lookup"><span data-stu-id="d9a52-418">Define the behavior of the elevation prompt for admins in Admin Approval Mode.</span></span> <span data-ttu-id="d9a52-419">可取值为：`notConfigured`、`elevateWithoutPrompting`、`promptForCredentialsOnTheSecureDesktop`、`promptForConsentOnTheSecureDesktop`、`promptForCredentials`、`promptForConsent`、`promptForConsentForNonWindowsBinaries`。</span><span class="sxs-lookup"><span data-stu-id="d9a52-419">Possible values are: `notConfigured`, `elevateWithoutPrompting`, `promptForCredentialsOnTheSecureDesktop`, `promptForConsentOnTheSecureDesktop`, `promptForCredentials`, `promptForConsent`, `promptForConsentForNonWindowsBinaries`.</span></span>|
|<span data-ttu-id="d9a52-420">localSecurityOptionsStandardUserElevationPromptBehavior</span><span class="sxs-lookup"><span data-stu-id="d9a52-420">localSecurityOptionsStandardUserElevationPromptBehavior</span></span>|[<span data-ttu-id="d9a52-421">localSecurityOptionsStandardUserElevationPromptBehaviorType</span><span class="sxs-lookup"><span data-stu-id="d9a52-421">localSecurityOptionsStandardUserElevationPromptBehaviorType</span></span>](../resources/intune-deviceconfig-localsecurityoptionsstandarduserelevationpromptbehaviortype.md)|<span data-ttu-id="d9a52-422">定义标准用户的提升提示的行为。</span><span class="sxs-lookup"><span data-stu-id="d9a52-422">Define the behavior of the elevation prompt for standard users.</span></span> <span data-ttu-id="d9a52-423">可取值为：`notConfigured`、`automaticallyDenyElevationRequests`、`promptForCredentialsOnTheSecureDesktop`、`promptForCredentials`。</span><span class="sxs-lookup"><span data-stu-id="d9a52-423">Possible values are: `notConfigured`, `automaticallyDenyElevationRequests`, `promptForCredentialsOnTheSecureDesktop`, `promptForCredentials`.</span></span>|
|<span data-ttu-id="d9a52-424">localSecurityOptionsSwitchToSecureDesktopWhenPromptingForElevation</span><span class="sxs-lookup"><span data-stu-id="d9a52-424">localSecurityOptionsSwitchToSecureDesktopWhenPromptingForElevation</span></span>|<span data-ttu-id="d9a52-425">Boolean</span><span class="sxs-lookup"><span data-stu-id="d9a52-425">Boolean</span></span>|<span data-ttu-id="d9a52-426">启用所有提升请求，以转到交互式用户的桌面，而不是安全的桌面。</span><span class="sxs-lookup"><span data-stu-id="d9a52-426">Enable all elevation requests to go to the interactive user's desktop rather than the secure desktop.</span></span> <span data-ttu-id="d9a52-427">使用提示行为 admins 和标准用户的策略设置。</span><span class="sxs-lookup"><span data-stu-id="d9a52-427">Prompt behavior policy settings for admins and standard users are used.</span></span>|
|<span data-ttu-id="d9a52-428">localSecurityOptionsDetectApplicationInstallationsAndPromptForElevation</span><span class="sxs-lookup"><span data-stu-id="d9a52-428">localSecurityOptionsDetectApplicationInstallationsAndPromptForElevation</span></span>|<span data-ttu-id="d9a52-429">Boolean</span><span class="sxs-lookup"><span data-stu-id="d9a52-429">Boolean</span></span>|<span data-ttu-id="d9a52-430">需要提升的权限的应用程序安装将会进行提示管理员凭据。将启用默认值</span><span class="sxs-lookup"><span data-stu-id="d9a52-430">App installations requiring elevated privileges will prompt for admin credentials.Default is enabled</span></span>|
|<span data-ttu-id="d9a52-431">localSecurityOptionsAllowUIAccessApplicationsForSecureLocations</span><span class="sxs-lookup"><span data-stu-id="d9a52-431">localSecurityOptionsAllowUIAccessApplicationsForSecureLocations</span></span>|<span data-ttu-id="d9a52-432">Boolean</span><span class="sxs-lookup"><span data-stu-id="d9a52-432">Boolean</span></span>|<span data-ttu-id="d9a52-433">允许 UIAccess 应用程序无需使用安全桌面提示提升。将启用默认值</span><span class="sxs-lookup"><span data-stu-id="d9a52-433">Allow UIAccess apps to prompt for elevation without using the secure desktop.Default is enabled</span></span>|
|<span data-ttu-id="d9a52-434">localSecurityOptionsUseAdminApprovalMode</span><span class="sxs-lookup"><span data-stu-id="d9a52-434">localSecurityOptionsUseAdminApprovalMode</span></span>|<span data-ttu-id="d9a52-435">Boolean</span><span class="sxs-lookup"><span data-stu-id="d9a52-435">Boolean</span></span>|<span data-ttu-id="d9a52-436">定义的内置的管理帐户使用管理员批准模式还是具有完整的管理员权限运行所有应用程序。将启用默认值</span><span class="sxs-lookup"><span data-stu-id="d9a52-436">Defines whether the built-in admin account uses Admin Approval Mode or runs all apps with full admin privileges.Default is enabled</span></span>|
|<span data-ttu-id="d9a52-437">localSecurityOptionsUseAdminApprovalModeForAdministrators</span><span class="sxs-lookup"><span data-stu-id="d9a52-437">localSecurityOptionsUseAdminApprovalModeForAdministrators</span></span>|<span data-ttu-id="d9a52-438">Boolean</span><span class="sxs-lookup"><span data-stu-id="d9a52-438">Boolean</span></span>|<span data-ttu-id="d9a52-439">定义是否启用管理员批准模式和所有 UAC 策略设置，将启用默认值</span><span class="sxs-lookup"><span data-stu-id="d9a52-439">Define whether Admin Approval Mode and all UAC policy settings are enabled, default is enabled</span></span>|
|<span data-ttu-id="d9a52-440">localSecurityOptionsInformationShownOnLockScreen</span><span class="sxs-lookup"><span data-stu-id="d9a52-440">localSecurityOptionsInformationShownOnLockScreen</span></span>|[<span data-ttu-id="d9a52-441">localSecurityOptionsInformationShownOnLockScreenType</span><span class="sxs-lookup"><span data-stu-id="d9a52-441">localSecurityOptionsInformationShownOnLockScreenType</span></span>](../resources/intune-deviceconfig-localsecurityoptionsinformationshownonlockscreentype.md)|<span data-ttu-id="d9a52-442">配置会话已被锁定时显示的用户信息。</span><span class="sxs-lookup"><span data-stu-id="d9a52-442">Configure the user information that is displayed when the session is locked.</span></span> <span data-ttu-id="d9a52-443">如果未配置，将显示用户的显示名称、 域和用户名。</span><span class="sxs-lookup"><span data-stu-id="d9a52-443">If not configured, user display name, domain and username are shown.</span></span> <span data-ttu-id="d9a52-444">可取值为：`notConfigured`、`userDisplayNameDomainUser`、`userDisplayNameOnly`、`doNotDisplayUser`。</span><span class="sxs-lookup"><span data-stu-id="d9a52-444">Possible values are: `notConfigured`, `userDisplayNameDomainUser`, `userDisplayNameOnly`, `doNotDisplayUser`.</span></span>|
|<span data-ttu-id="d9a52-445">localSecurityOptionsInformationDisplayedOnLockScreen</span><span class="sxs-lookup"><span data-stu-id="d9a52-445">localSecurityOptionsInformationDisplayedOnLockScreen</span></span>|[<span data-ttu-id="d9a52-446">localSecurityOptionsInformationDisplayedOnLockScreenType</span><span class="sxs-lookup"><span data-stu-id="d9a52-446">localSecurityOptionsInformationDisplayedOnLockScreenType</span></span>](../resources/intune-deviceconfig-localsecurityoptionsinformationdisplayedonlockscreentype.md)|<span data-ttu-id="d9a52-447">配置会话已被锁定时显示的用户信息。</span><span class="sxs-lookup"><span data-stu-id="d9a52-447">Configure the user information that is displayed when the session is locked.</span></span> <span data-ttu-id="d9a52-448">如果未配置，将显示用户的显示名称、 域和用户名。</span><span class="sxs-lookup"><span data-stu-id="d9a52-448">If not configured, user display name, domain and username are shown.</span></span> <span data-ttu-id="d9a52-449">可取值为：`notConfigured`、`administrators`、`administratorsAndPowerUsers`、`administratorsAndInteractiveUsers`。</span><span class="sxs-lookup"><span data-stu-id="d9a52-449">Possible values are: `notConfigured`, `administrators`, `administratorsAndPowerUsers`, `administratorsAndInteractiveUsers`.</span></span>|
|<span data-ttu-id="d9a52-450">localSecurityOptionsDisableClientDigitallySignCommunicationsIfServerAgrees</span><span class="sxs-lookup"><span data-stu-id="d9a52-450">localSecurityOptionsDisableClientDigitallySignCommunicationsIfServerAgrees</span></span>|<span data-ttu-id="d9a52-451">Boolean</span><span class="sxs-lookup"><span data-stu-id="d9a52-451">Boolean</span></span>|<span data-ttu-id="d9a52-452">此安全设置确定是否 SMB 客户端尝试协商 SMB 数据包签名。</span><span class="sxs-lookup"><span data-stu-id="d9a52-452">This security setting determines whether the SMB client attempts to negotiate SMB packet signing.</span></span>|
|<span data-ttu-id="d9a52-453">localSecurityOptionsClientDigitallySignCommunicationsAlways</span><span class="sxs-lookup"><span data-stu-id="d9a52-453">localSecurityOptionsClientDigitallySignCommunicationsAlways</span></span>|<span data-ttu-id="d9a52-454">Boolean</span><span class="sxs-lookup"><span data-stu-id="d9a52-454">Boolean</span></span>|<span data-ttu-id="d9a52-455">此安全设置确定是否数据包签名所需 SMB 客户端组件。</span><span class="sxs-lookup"><span data-stu-id="d9a52-455">This security setting determines whether packet signing is required by the SMB client component.</span></span>|
|<span data-ttu-id="d9a52-456">localSecurityOptionsClientSendUnencryptedPasswordToThirdPartySMBServers</span><span class="sxs-lookup"><span data-stu-id="d9a52-456">localSecurityOptionsClientSendUnencryptedPasswordToThirdPartySMBServers</span></span>|<span data-ttu-id="d9a52-457">Boolean</span><span class="sxs-lookup"><span data-stu-id="d9a52-457">Boolean</span></span>|<span data-ttu-id="d9a52-458">如果启用此安全设置，则允许服务器消息块 (SMB) 重定向到不支持期间身份验证的密码加密的非 Microsoft SMB 服务器发送纯文本密码。</span><span class="sxs-lookup"><span data-stu-id="d9a52-458">If this security setting is enabled, the Server Message Block (SMB) redirector is allowed to send plaintext passwords to non-Microsoft SMB servers that do not support password encryption during authentication.</span></span>|
|<span data-ttu-id="d9a52-459">localSecurityOptionsDisableServerDigitallySignCommunicationsAlways</span><span class="sxs-lookup"><span data-stu-id="d9a52-459">localSecurityOptionsDisableServerDigitallySignCommunicationsAlways</span></span>|<span data-ttu-id="d9a52-460">Boolean</span><span class="sxs-lookup"><span data-stu-id="d9a52-460">Boolean</span></span>|<span data-ttu-id="d9a52-461">此安全设置确定是否由 SMB 服务器组件要求签名数据包。</span><span class="sxs-lookup"><span data-stu-id="d9a52-461">This security setting determines whether packet signing is required by the SMB server component.</span></span>|
|<span data-ttu-id="d9a52-462">localSecurityOptionsDisableServerDigitallySignCommunicationsIfClientAgrees</span><span class="sxs-lookup"><span data-stu-id="d9a52-462">localSecurityOptionsDisableServerDigitallySignCommunicationsIfClientAgrees</span></span>|<span data-ttu-id="d9a52-463">Boolean</span><span class="sxs-lookup"><span data-stu-id="d9a52-463">Boolean</span></span>|<span data-ttu-id="d9a52-464">此安全设置确定 SMB 服务器是否协商 SMB 数据包签名与请求的客户端。</span><span class="sxs-lookup"><span data-stu-id="d9a52-464">This security setting determines whether the SMB server will negotiate SMB packet signing with clients that request it.</span></span>|
|<span data-ttu-id="d9a52-465">localSecurityOptionsRestrictAnonymousAccessToNamedPipesAndShares</span><span class="sxs-lookup"><span data-stu-id="d9a52-465">localSecurityOptionsRestrictAnonymousAccessToNamedPipesAndShares</span></span>|<span data-ttu-id="d9a52-466">Boolean</span><span class="sxs-lookup"><span data-stu-id="d9a52-466">Boolean</span></span>|<span data-ttu-id="d9a52-467">默认情况下，此安全设置将匿名访问限制为共享和管道的可匿名访问的命名的管道和可匿名访问的共享的设置</span><span class="sxs-lookup"><span data-stu-id="d9a52-467">By default, this security setting restricts anonymous access to shares and pipes to the settings for named pipes that can be accessed anonymously and Shares that can be accessed anonymously</span></span>|
|<span data-ttu-id="d9a52-468">localSecurityOptionsDoNotAllowAnonymousEnumerationOfSAMAccounts</span><span class="sxs-lookup"><span data-stu-id="d9a52-468">localSecurityOptionsDoNotAllowAnonymousEnumerationOfSAMAccounts</span></span>|<span data-ttu-id="d9a52-469">Boolean</span><span class="sxs-lookup"><span data-stu-id="d9a52-469">Boolean</span></span>|<span data-ttu-id="d9a52-470">此安全设置确定将对匿名连接到计算机上授予其他权限。</span><span class="sxs-lookup"><span data-stu-id="d9a52-470">This security setting determines what additional permissions will be granted for anonymous connections to the computer.</span></span>|
|<span data-ttu-id="d9a52-471">localSecurityOptionsAllowAnonymousEnumerationOfSAMAccountsAndShares</span><span class="sxs-lookup"><span data-stu-id="d9a52-471">localSecurityOptionsAllowAnonymousEnumerationOfSAMAccountsAndShares</span></span>|<span data-ttu-id="d9a52-472">Boolean</span><span class="sxs-lookup"><span data-stu-id="d9a52-472">Boolean</span></span>|<span data-ttu-id="d9a52-473">此安全设置确定是否允许匿名用户执行某些活动，如枚举的域帐户和网络共享名称。</span><span class="sxs-lookup"><span data-stu-id="d9a52-473">This security setting determines whether to allows anonymous users to perform certain activities, such as enumerating the names of domain accounts and network shares.</span></span>|
|<span data-ttu-id="d9a52-474">localSecurityOptionsDoNotStoreLANManagerHashValueOnNextPasswordChange</span><span class="sxs-lookup"><span data-stu-id="d9a52-474">localSecurityOptionsDoNotStoreLANManagerHashValueOnNextPasswordChange</span></span>|<span data-ttu-id="d9a52-475">Boolean</span><span class="sxs-lookup"><span data-stu-id="d9a52-475">Boolean</span></span>|<span data-ttu-id="d9a52-476">此安全设置确定，是否在下次密码更改，存储新密码的 LAN Manager (LM) 哈希值。</span><span class="sxs-lookup"><span data-stu-id="d9a52-476">This security setting determines if, at the next password change, the LAN Manager (LM) hash value for the new password is stored.</span></span> <span data-ttu-id="d9a52-477">默认情况下，它不存储。</span><span class="sxs-lookup"><span data-stu-id="d9a52-477">It’s not stored by default.</span></span>|
|<span data-ttu-id="d9a52-478">localSecurityOptionsSmartCardRemovalBehavior</span><span class="sxs-lookup"><span data-stu-id="d9a52-478">localSecurityOptionsSmartCardRemovalBehavior</span></span>|[<span data-ttu-id="d9a52-479">localSecurityOptionsSmartCardRemovalBehaviorType</span><span class="sxs-lookup"><span data-stu-id="d9a52-479">localSecurityOptionsSmartCardRemovalBehaviorType</span></span>](../resources/intune-deviceconfig-localsecurityoptionssmartcardremovalbehaviortype.md)|<span data-ttu-id="d9a52-480">此安全设置确定智能卡读卡器从移除智能卡登录的用户时，会发生什么情况。</span><span class="sxs-lookup"><span data-stu-id="d9a52-480">This security setting determines what happens when the smart card for a logged-on user is removed from the smart card reader.</span></span> <span data-ttu-id="d9a52-481">可取值为：`lockWorkstation`、`noAction`、`forceLogoff`、`disconnectRemoteDesktopSession`。</span><span class="sxs-lookup"><span data-stu-id="d9a52-481">Possible values are: `lockWorkstation`, `noAction`, `forceLogoff`, `disconnectRemoteDesktopSession`.</span></span>|
|<span data-ttu-id="d9a52-482">defenderSecurityCenterDisableAppBrowserUI</span><span class="sxs-lookup"><span data-stu-id="d9a52-482">defenderSecurityCenterDisableAppBrowserUI</span></span>|<span data-ttu-id="d9a52-483">Boolean</span><span class="sxs-lookup"><span data-stu-id="d9a52-483">Boolean</span></span>|<span data-ttu-id="d9a52-484">用于禁用的应用程序和浏览器的保护区域显示。</span><span class="sxs-lookup"><span data-stu-id="d9a52-484">Used to disable the display of the app and browser protection area.</span></span>|
|<span data-ttu-id="d9a52-485">defenderSecurityCenterDisableFamilyUI</span><span class="sxs-lookup"><span data-stu-id="d9a52-485">defenderSecurityCenterDisableFamilyUI</span></span>|<span data-ttu-id="d9a52-486">Boolean</span><span class="sxs-lookup"><span data-stu-id="d9a52-486">Boolean</span></span>|<span data-ttu-id="d9a52-487">用于禁用系列选项区域的显示。</span><span class="sxs-lookup"><span data-stu-id="d9a52-487">Used to disable the display of the family options area.</span></span>|
|<span data-ttu-id="d9a52-488">defenderSecurityCenterDisableHealthUI</span><span class="sxs-lookup"><span data-stu-id="d9a52-488">defenderSecurityCenterDisableHealthUI</span></span>|<span data-ttu-id="d9a52-489">Boolean</span><span class="sxs-lookup"><span data-stu-id="d9a52-489">Boolean</span></span>|<span data-ttu-id="d9a52-490">用于禁用设备性能和运行状况区域的显示。</span><span class="sxs-lookup"><span data-stu-id="d9a52-490">Used to disable the display of the device performance and health area.</span></span>|
|<span data-ttu-id="d9a52-491">defenderSecurityCenterDisableNetworkUI</span><span class="sxs-lookup"><span data-stu-id="d9a52-491">defenderSecurityCenterDisableNetworkUI</span></span>|<span data-ttu-id="d9a52-492">Boolean</span><span class="sxs-lookup"><span data-stu-id="d9a52-492">Boolean</span></span>|<span data-ttu-id="d9a52-493">用于禁用防火墙和网络保护区域的显示。</span><span class="sxs-lookup"><span data-stu-id="d9a52-493">Used to disable the display of the firewall and network protection area.</span></span>|
|<span data-ttu-id="d9a52-494">defenderSecurityCenterDisableVirusUI</span><span class="sxs-lookup"><span data-stu-id="d9a52-494">defenderSecurityCenterDisableVirusUI</span></span>|<span data-ttu-id="d9a52-495">Boolean</span><span class="sxs-lookup"><span data-stu-id="d9a52-495">Boolean</span></span>|<span data-ttu-id="d9a52-496">用于禁用病毒和威胁保护区域的显示。</span><span class="sxs-lookup"><span data-stu-id="d9a52-496">Used to disable the display of the virus and threat protection area.</span></span>|
|<span data-ttu-id="d9a52-497">defenderSecurityCenterDisableAccountUI</span><span class="sxs-lookup"><span data-stu-id="d9a52-497">defenderSecurityCenterDisableAccountUI</span></span>|<span data-ttu-id="d9a52-498">Boolean</span><span class="sxs-lookup"><span data-stu-id="d9a52-498">Boolean</span></span>|<span data-ttu-id="d9a52-499">用于禁用帐户保护区域的显示。</span><span class="sxs-lookup"><span data-stu-id="d9a52-499">Used to disable the display of the account protection area.</span></span>|
|<span data-ttu-id="d9a52-500">defenderSecurityCenterDisableHardwareUI</span><span class="sxs-lookup"><span data-stu-id="d9a52-500">defenderSecurityCenterDisableHardwareUI</span></span>|<span data-ttu-id="d9a52-501">Boolean</span><span class="sxs-lookup"><span data-stu-id="d9a52-501">Boolean</span></span>|<span data-ttu-id="d9a52-502">用于禁用硬件保护区域的显示。</span><span class="sxs-lookup"><span data-stu-id="d9a52-502">Used to disable the display of the hardware protection area.</span></span>|
|<span data-ttu-id="d9a52-503">defenderSecurityCenterDisableRansomwareUI</span><span class="sxs-lookup"><span data-stu-id="d9a52-503">defenderSecurityCenterDisableRansomwareUI</span></span>|<span data-ttu-id="d9a52-504">Boolean</span><span class="sxs-lookup"><span data-stu-id="d9a52-504">Boolean</span></span>|<span data-ttu-id="d9a52-505">用于禁用勒索软件保护区域的显示。</span><span class="sxs-lookup"><span data-stu-id="d9a52-505">Used to disable the display of the ransomware protection area.</span></span> |
|<span data-ttu-id="d9a52-506">defenderSecurityCenterDisableSecureBootUI</span><span class="sxs-lookup"><span data-stu-id="d9a52-506">defenderSecurityCenterDisableSecureBootUI</span></span>|<span data-ttu-id="d9a52-507">Boolean</span><span class="sxs-lookup"><span data-stu-id="d9a52-507">Boolean</span></span>|<span data-ttu-id="d9a52-508">用于禁用的设备安全下的安全启动区域显示。</span><span class="sxs-lookup"><span data-stu-id="d9a52-508">Used to disable the display of the secure boot area under Device security.</span></span>|
|<span data-ttu-id="d9a52-509">defenderSecurityCenterDisableTroubleshootingUI</span><span class="sxs-lookup"><span data-stu-id="d9a52-509">defenderSecurityCenterDisableTroubleshootingUI</span></span>|<span data-ttu-id="d9a52-510">Boolean</span><span class="sxs-lookup"><span data-stu-id="d9a52-510">Boolean</span></span>|<span data-ttu-id="d9a52-511">用于禁用安全过程下设备安全疑难解答的显示。</span><span class="sxs-lookup"><span data-stu-id="d9a52-511">Used to disable the display of the security process troubleshooting under Device security.</span></span>|
|<span data-ttu-id="d9a52-512">defenderSecurityCenterOrganizationDisplayName</span><span class="sxs-lookup"><span data-stu-id="d9a52-512">defenderSecurityCenterOrganizationDisplayName</span></span>|<span data-ttu-id="d9a52-513">String</span><span class="sxs-lookup"><span data-stu-id="d9a52-513">String</span></span>|<span data-ttu-id="d9a52-514">向用户显示公司名称。</span><span class="sxs-lookup"><span data-stu-id="d9a52-514">The company name that is displayed to the users.</span></span>|
|<span data-ttu-id="d9a52-515">defenderSecurityCenterHelpEmail</span><span class="sxs-lookup"><span data-stu-id="d9a52-515">defenderSecurityCenterHelpEmail</span></span>|<span data-ttu-id="d9a52-516">String</span><span class="sxs-lookup"><span data-stu-id="d9a52-516">String</span></span>|<span data-ttu-id="d9a52-517">向用户显示的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="d9a52-517">The email address that is displayed to users.</span></span>|
|<span data-ttu-id="d9a52-518">defenderSecurityCenterHelpPhone</span><span class="sxs-lookup"><span data-stu-id="d9a52-518">defenderSecurityCenterHelpPhone</span></span>|<span data-ttu-id="d9a52-519">String</span><span class="sxs-lookup"><span data-stu-id="d9a52-519">String</span></span>|<span data-ttu-id="d9a52-520">电话号码或向用户显示的 Skype ID 中。</span><span class="sxs-lookup"><span data-stu-id="d9a52-520">The phone number or Skype ID that is displayed to users.</span></span>|
|<span data-ttu-id="d9a52-521">defenderSecurityCenterHelpURL</span><span class="sxs-lookup"><span data-stu-id="d9a52-521">defenderSecurityCenterHelpURL</span></span>|<span data-ttu-id="d9a52-522">String</span><span class="sxs-lookup"><span data-stu-id="d9a52-522">String</span></span>|<span data-ttu-id="d9a52-523">帮助门户这向用户显示的 URL。</span><span class="sxs-lookup"><span data-stu-id="d9a52-523">The help portal URL this is displayed to users.</span></span>|
|<span data-ttu-id="d9a52-524">defenderSecurityCenterNotificationsFromApp</span><span class="sxs-lookup"><span data-stu-id="d9a52-524">defenderSecurityCenterNotificationsFromApp</span></span>|[<span data-ttu-id="d9a52-525">defenderSecurityCenterNotificationsFromAppType</span><span class="sxs-lookup"><span data-stu-id="d9a52-525">defenderSecurityCenterNotificationsFromAppType</span></span>](../resources/intune-deviceconfig-defendersecuritycenternotificationsfromapptype.md)|<span data-ttu-id="d9a52-526">若要从应用程序的显示区域显示的通知。</span><span class="sxs-lookup"><span data-stu-id="d9a52-526">Notifications to show from the displayed areas of app.</span></span> <span data-ttu-id="d9a52-527">可取值为：`notConfigured`、`blockNoncriticalNotifications`、`blockAllNotifications`。</span><span class="sxs-lookup"><span data-stu-id="d9a52-527">Possible values are: `notConfigured`, `blockNoncriticalNotifications`, `blockAllNotifications`.</span></span>|
|<span data-ttu-id="d9a52-528">defenderSecurityCenterITContactDisplay</span><span class="sxs-lookup"><span data-stu-id="d9a52-528">defenderSecurityCenterITContactDisplay</span></span>|[<span data-ttu-id="d9a52-529">defenderSecurityCenterITContactDisplayType</span><span class="sxs-lookup"><span data-stu-id="d9a52-529">defenderSecurityCenterITContactDisplayType</span></span>](../resources/intune-deviceconfig-defendersecuritycenteritcontactdisplaytype.md)|<span data-ttu-id="d9a52-530">配置显示 IT 联系人位置向最终用户的信息。</span><span class="sxs-lookup"><span data-stu-id="d9a52-530">Configure where to display IT contact information to end users.</span></span> <span data-ttu-id="d9a52-531">可取值为：`notConfigured`、`displayInAppAndInNotifications`、`displayOnlyInApp`、`displayOnlyInNotifications`。</span><span class="sxs-lookup"><span data-stu-id="d9a52-531">Possible values are: `notConfigured`, `displayInAppAndInNotifications`, `displayOnlyInApp`, `displayOnlyInNotifications`.</span></span>|
|<span data-ttu-id="d9a52-532">firewallBlockStatefulFTP</span><span class="sxs-lookup"><span data-stu-id="d9a52-532">firewallBlockStatefulFTP</span></span>|<span data-ttu-id="d9a52-533">Boolean</span><span class="sxs-lookup"><span data-stu-id="d9a52-533">Boolean</span></span>|<span data-ttu-id="d9a52-534">阻止到设备的有状态 FTP 连接</span><span class="sxs-lookup"><span data-stu-id="d9a52-534">Blocks stateful FTP connections to the device</span></span>|
|<span data-ttu-id="d9a52-535">firewallIdleTimeoutForSecurityAssociationInSeconds</span><span class="sxs-lookup"><span data-stu-id="d9a52-535">firewallIdleTimeoutForSecurityAssociationInSeconds</span></span>|<span data-ttu-id="d9a52-536">Int32</span><span class="sxs-lookup"><span data-stu-id="d9a52-536">Int32</span></span>|<span data-ttu-id="d9a52-537">配置安全关联的空闲超时（以秒为单位），值范围为 300 到 3600（包括这两个值）。</span><span class="sxs-lookup"><span data-stu-id="d9a52-537">Configures the idle timeout for security associations, in seconds, from 300 to 3600 inclusive.</span></span> <span data-ttu-id="d9a52-538">这是一个时间段，在此之后安全关联将过期并被删除。</span><span class="sxs-lookup"><span data-stu-id="d9a52-538">This is the period after which security associations will expire and be deleted.</span></span> <span data-ttu-id="d9a52-539">有效值为 300 至 3600。</span><span class="sxs-lookup"><span data-stu-id="d9a52-539">Valid values 300 to 3600</span></span>|
|<span data-ttu-id="d9a52-540">firewallPreSharedKeyEncodingMethod</span><span class="sxs-lookup"><span data-stu-id="d9a52-540">firewallPreSharedKeyEncodingMethod</span></span>|[<span data-ttu-id="d9a52-541">firewallPreSharedKeyEncodingMethodType</span><span class="sxs-lookup"><span data-stu-id="d9a52-541">firewallPreSharedKeyEncodingMethodType</span></span>](../resources/intune-deviceconfig-firewallpresharedkeyencodingmethodtype.md)|<span data-ttu-id="d9a52-542">选择要使用编码的预共享的键。</span><span class="sxs-lookup"><span data-stu-id="d9a52-542">Select the preshared key encoding to be used.</span></span> <span data-ttu-id="d9a52-543">可取值为：`deviceDefault`、`none`、`utF8`。</span><span class="sxs-lookup"><span data-stu-id="d9a52-543">Possible values are: `deviceDefault`, `none`, `utF8`.</span></span>|
|<span data-ttu-id="d9a52-544">firewallIPSecExemptionsAllowNeighborDiscovery</span><span class="sxs-lookup"><span data-stu-id="d9a52-544">firewallIPSecExemptionsAllowNeighborDiscovery</span></span>|<span data-ttu-id="d9a52-545">Boolean</span><span class="sxs-lookup"><span data-stu-id="d9a52-545">Boolean</span></span>|<span data-ttu-id="d9a52-546">配置 IPSec 免除项以允许邻居发现 IPv6 ICMP 类型代码</span><span class="sxs-lookup"><span data-stu-id="d9a52-546">Configures IPSec exemptions to allow neighbor discovery IPv6 ICMP type-codes</span></span>|
|<span data-ttu-id="d9a52-547">firewallIPSecExemptionsAllowICMP</span><span class="sxs-lookup"><span data-stu-id="d9a52-547">firewallIPSecExemptionsAllowICMP</span></span>|<span data-ttu-id="d9a52-548">Boolean</span><span class="sxs-lookup"><span data-stu-id="d9a52-548">Boolean</span></span>|<span data-ttu-id="d9a52-549">配置 IPSec 免除项以允许 ICMP</span><span class="sxs-lookup"><span data-stu-id="d9a52-549">Configures IPSec exemptions to allow ICMP</span></span>|
|<span data-ttu-id="d9a52-550">firewallIPSecExemptionsAllowRouterDiscovery</span><span class="sxs-lookup"><span data-stu-id="d9a52-550">firewallIPSecExemptionsAllowRouterDiscovery</span></span>|<span data-ttu-id="d9a52-551">Boolean</span><span class="sxs-lookup"><span data-stu-id="d9a52-551">Boolean</span></span>|<span data-ttu-id="d9a52-552">配置 IPSec 免除项以允许路由器发现 IPv6 ICMP 类型代码</span><span class="sxs-lookup"><span data-stu-id="d9a52-552">Configures IPSec exemptions to allow router discovery IPv6 ICMP type-codes</span></span>|
|<span data-ttu-id="d9a52-553">firewallIPSecExemptionsAllowDHCP</span><span class="sxs-lookup"><span data-stu-id="d9a52-553">firewallIPSecExemptionsAllowDHCP</span></span>|<span data-ttu-id="d9a52-554">Boolean</span><span class="sxs-lookup"><span data-stu-id="d9a52-554">Boolean</span></span>|<span data-ttu-id="d9a52-555">配置 IPSec 免除项以允许 IPv4 和 IPv6 DHCP 通信</span><span class="sxs-lookup"><span data-stu-id="d9a52-555">Configures IPSec exemptions to allow both IPv4 and IPv6 DHCP traffic</span></span>|
|<span data-ttu-id="d9a52-556">firewallCertificateRevocationListCheckMethod</span><span class="sxs-lookup"><span data-stu-id="d9a52-556">firewallCertificateRevocationListCheckMethod</span></span>|[<span data-ttu-id="d9a52-557">firewallCertificateRevocationListCheckMethodType</span><span class="sxs-lookup"><span data-stu-id="d9a52-557">firewallCertificateRevocationListCheckMethodType</span></span>](../resources/intune-deviceconfig-firewallcertificaterevocationlistcheckmethodtype.md)|<span data-ttu-id="d9a52-558">指定如何强制实施证书吊销列表。</span><span class="sxs-lookup"><span data-stu-id="d9a52-558">Specify how the certificate revocation list is to be enforced.</span></span> <span data-ttu-id="d9a52-559">可取值为：`deviceDefault`、`none`、`attempt`、`require`。</span><span class="sxs-lookup"><span data-stu-id="d9a52-559">Possible values are: `deviceDefault`, `none`, `attempt`, `require`.</span></span>|
|<span data-ttu-id="d9a52-560">firewallMergeKeyingModuleSettings</span><span class="sxs-lookup"><span data-stu-id="d9a52-560">firewallMergeKeyingModuleSettings</span></span>|<span data-ttu-id="d9a52-561">Boolean</span><span class="sxs-lookup"><span data-stu-id="d9a52-561">Boolean</span></span>|<span data-ttu-id="d9a52-562">如果键控模块不完全支持身份验证集，请指示模块仅忽略不受支持的身份验证套件而不是整个集</span><span class="sxs-lookup"><span data-stu-id="d9a52-562">If an authentication set is not fully supported by a keying module, direct the module to ignore only unsupported authentication suites rather than the entire set</span></span>|
|<span data-ttu-id="d9a52-563">firewallPacketQueueingMethod</span><span class="sxs-lookup"><span data-stu-id="d9a52-563">firewallPacketQueueingMethod</span></span>|[<span data-ttu-id="d9a52-564">firewallPacketQueueingMethodType</span><span class="sxs-lookup"><span data-stu-id="d9a52-564">firewallPacketQueueingMethodType</span></span>](../resources/intune-deviceconfig-firewallpacketqueueingmethodtype.md)|<span data-ttu-id="d9a52-565">配置数据包 queueing 应如何应用隧道网关方案中。</span><span class="sxs-lookup"><span data-stu-id="d9a52-565">Configures how packet queueing should be applied in the tunnel gateway scenario.</span></span> <span data-ttu-id="d9a52-566">可取值为：`deviceDefault`、`disabled`、`queueInbound`、`queueOutbound`、`queueBoth`。</span><span class="sxs-lookup"><span data-stu-id="d9a52-566">Possible values are: `deviceDefault`, `disabled`, `queueInbound`, `queueOutbound`, `queueBoth`.</span></span>|
|<span data-ttu-id="d9a52-567">firewallProfileDomain</span><span class="sxs-lookup"><span data-stu-id="d9a52-567">firewallProfileDomain</span></span>|[<span data-ttu-id="d9a52-568">windowsFirewallNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="d9a52-568">windowsFirewallNetworkProfile</span></span>](../resources/intune-deviceconfig-windowsfirewallnetworkprofile.md)|<span data-ttu-id="d9a52-569">配置域网络的防火墙配置文件设置</span><span class="sxs-lookup"><span data-stu-id="d9a52-569">Configures the firewall profile settings for domain networks</span></span>|
|<span data-ttu-id="d9a52-570">firewallProfilePublic</span><span class="sxs-lookup"><span data-stu-id="d9a52-570">firewallProfilePublic</span></span>|[<span data-ttu-id="d9a52-571">windowsFirewallNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="d9a52-571">windowsFirewallNetworkProfile</span></span>](../resources/intune-deviceconfig-windowsfirewallnetworkprofile.md)|<span data-ttu-id="d9a52-572">配置公用网络的防火墙配置文件设置</span><span class="sxs-lookup"><span data-stu-id="d9a52-572">Configures the firewall profile settings for public networks</span></span>|
|<span data-ttu-id="d9a52-573">firewallProfilePrivate</span><span class="sxs-lookup"><span data-stu-id="d9a52-573">firewallProfilePrivate</span></span>|[<span data-ttu-id="d9a52-574">windowsFirewallNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="d9a52-574">windowsFirewallNetworkProfile</span></span>](../resources/intune-deviceconfig-windowsfirewallnetworkprofile.md)|<span data-ttu-id="d9a52-575">配置专用网络的防火墙配置文件设置</span><span class="sxs-lookup"><span data-stu-id="d9a52-575">Configures the firewall profile settings for private networks</span></span>|
|<span data-ttu-id="d9a52-576">defenderAttackSurfaceReductionExcludedPaths</span><span class="sxs-lookup"><span data-stu-id="d9a52-576">defenderAttackSurfaceReductionExcludedPaths</span></span>|<span data-ttu-id="d9a52-577">String 集合</span><span class="sxs-lookup"><span data-stu-id="d9a52-577">String collection</span></span>|<span data-ttu-id="d9a52-578">要从攻击面减少规则中排除的 exe 文件和文件夹的列表</span><span class="sxs-lookup"><span data-stu-id="d9a52-578">List of exe files and folders to be excluded from attack surface reduction rules</span></span>|
|<span data-ttu-id="d9a52-579">defenderOfficeAppsOtherProcessInjectionType</span><span class="sxs-lookup"><span data-stu-id="d9a52-579">defenderOfficeAppsOtherProcessInjectionType</span></span>|[<span data-ttu-id="d9a52-580">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="d9a52-580">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="d9a52-581">值，指示将到其他进程的 Office 应用程序的行为。</span><span class="sxs-lookup"><span data-stu-id="d9a52-581">Value indicating the behavior of Office applications injecting into other processes.</span></span> <span data-ttu-id="d9a52-582">可取值为：`userDefined`、`block`、`auditMode`。</span><span class="sxs-lookup"><span data-stu-id="d9a52-582">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="d9a52-583">defenderOfficeAppsOtherProcessInjection</span><span class="sxs-lookup"><span data-stu-id="d9a52-583">defenderOfficeAppsOtherProcessInjection</span></span>|[<span data-ttu-id="d9a52-584">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="d9a52-584">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="d9a52-585">值，指示将到其他进程的 Office 应用程序的行为。</span><span class="sxs-lookup"><span data-stu-id="d9a52-585">Value indicating the behavior of  Office applications injecting into other processes.</span></span> <span data-ttu-id="d9a52-586">可取值为：`userDefined`、`enable`、`auditMode`。</span><span class="sxs-lookup"><span data-stu-id="d9a52-586">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="d9a52-587">defenderOfficeAppsExecutableContentCreationOrLaunchType</span><span class="sxs-lookup"><span data-stu-id="d9a52-587">defenderOfficeAppsExecutableContentCreationOrLaunchType</span></span>|[<span data-ttu-id="d9a52-588">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="d9a52-588">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="d9a52-589">指示 Office 应用程序/宏创建或启动可执行文件内容的行为的值。</span><span class="sxs-lookup"><span data-stu-id="d9a52-589">Value indicating the behavior of Office applications/macros creating or launching executable content.</span></span> <span data-ttu-id="d9a52-590">可取值为：`userDefined`、`block`、`auditMode`。</span><span class="sxs-lookup"><span data-stu-id="d9a52-590">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="d9a52-591">defenderOfficeAppsExecutableContentCreationOrLaunch</span><span class="sxs-lookup"><span data-stu-id="d9a52-591">defenderOfficeAppsExecutableContentCreationOrLaunch</span></span>|[<span data-ttu-id="d9a52-592">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="d9a52-592">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="d9a52-593">指示 Office 应用程序/宏创建或启动可执行文件内容的行为的值。</span><span class="sxs-lookup"><span data-stu-id="d9a52-593">Value indicating the behavior of Office applications/macros creating or launching executable content.</span></span> <span data-ttu-id="d9a52-594">可取值为：`userDefined`、`enable`、`auditMode`。</span><span class="sxs-lookup"><span data-stu-id="d9a52-594">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="d9a52-595">defenderOfficeAppsLaunchChildProcessType</span><span class="sxs-lookup"><span data-stu-id="d9a52-595">defenderOfficeAppsLaunchChildProcessType</span></span>|[<span data-ttu-id="d9a52-596">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="d9a52-596">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="d9a52-597">指示启动子进程的 Office 应用程序的行为的值。</span><span class="sxs-lookup"><span data-stu-id="d9a52-597">Value indicating the behavior of Office application launching child processes.</span></span> <span data-ttu-id="d9a52-598">可取值为：`userDefined`、`block`、`auditMode`。</span><span class="sxs-lookup"><span data-stu-id="d9a52-598">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="d9a52-599">defenderOfficeAppsLaunchChildProcess</span><span class="sxs-lookup"><span data-stu-id="d9a52-599">defenderOfficeAppsLaunchChildProcess</span></span>|[<span data-ttu-id="d9a52-600">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="d9a52-600">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="d9a52-601">指示启动子进程的 Office 应用程序的行为的值。</span><span class="sxs-lookup"><span data-stu-id="d9a52-601">Value indicating the behavior of Office application launching child processes.</span></span> <span data-ttu-id="d9a52-602">可取值为：`userDefined`、`enable`、`auditMode`。</span><span class="sxs-lookup"><span data-stu-id="d9a52-602">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="d9a52-603">defenderOfficeMacroCodeAllowWin32ImportsType</span><span class="sxs-lookup"><span data-stu-id="d9a52-603">defenderOfficeMacroCodeAllowWin32ImportsType</span></span>|[<span data-ttu-id="d9a52-604">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="d9a52-604">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="d9a52-605">值，该值指示的 Win32 行为导入从 Office 中的宏代码。</span><span class="sxs-lookup"><span data-stu-id="d9a52-605">Value indicating the behavior of Win32 imports from Macro code in Office.</span></span> <span data-ttu-id="d9a52-606">可取值为：`userDefined`、`block`、`auditMode`。</span><span class="sxs-lookup"><span data-stu-id="d9a52-606">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="d9a52-607">defenderOfficeMacroCodeAllowWin32Imports</span><span class="sxs-lookup"><span data-stu-id="d9a52-607">defenderOfficeMacroCodeAllowWin32Imports</span></span>|[<span data-ttu-id="d9a52-608">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="d9a52-608">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="d9a52-609">值，该值指示的 Win32 行为导入从 Office 中的宏代码。</span><span class="sxs-lookup"><span data-stu-id="d9a52-609">Value indicating the behavior of Win32 imports from Macro code in Office.</span></span> <span data-ttu-id="d9a52-610">可取值为：`userDefined`、`enable`、`auditMode`。</span><span class="sxs-lookup"><span data-stu-id="d9a52-610">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="d9a52-611">defenderScriptObfuscatedMacroCodeType</span><span class="sxs-lookup"><span data-stu-id="d9a52-611">defenderScriptObfuscatedMacroCodeType</span></span>|[<span data-ttu-id="d9a52-612">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="d9a52-612">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="d9a52-613">值，该值指示经过模糊处理 js/vbs/ps/macro 代码的行为。</span><span class="sxs-lookup"><span data-stu-id="d9a52-613">Value indicating the behavior of obfuscated js/vbs/ps/macro code.</span></span> <span data-ttu-id="d9a52-614">可取值为：`userDefined`、`block`、`auditMode`。</span><span class="sxs-lookup"><span data-stu-id="d9a52-614">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="d9a52-615">defenderScriptObfuscatedMacroCode</span><span class="sxs-lookup"><span data-stu-id="d9a52-615">defenderScriptObfuscatedMacroCode</span></span>|[<span data-ttu-id="d9a52-616">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="d9a52-616">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="d9a52-617">值，该值指示经过模糊处理 js/vbs/ps/macro 代码的行为。</span><span class="sxs-lookup"><span data-stu-id="d9a52-617">Value indicating the behavior of obfuscated js/vbs/ps/macro code.</span></span> <span data-ttu-id="d9a52-618">可取值为：`userDefined`、`enable`、`auditMode`。</span><span class="sxs-lookup"><span data-stu-id="d9a52-618">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="d9a52-619">defenderScriptDownloadedPayloadExecutionType</span><span class="sxs-lookup"><span data-stu-id="d9a52-619">defenderScriptDownloadedPayloadExecutionType</span></span>|[<span data-ttu-id="d9a52-620">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="d9a52-620">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="d9a52-621">从 Internet 下载的值，该值指示 js/vbs 执行负载的行为。</span><span class="sxs-lookup"><span data-stu-id="d9a52-621">Value indicating the behavior of js/vbs executing payload downloaded from Internet.</span></span> <span data-ttu-id="d9a52-622">可取值为：`userDefined`、`block`、`auditMode`。</span><span class="sxs-lookup"><span data-stu-id="d9a52-622">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="d9a52-623">defenderScriptDownloadedPayloadExecution</span><span class="sxs-lookup"><span data-stu-id="d9a52-623">defenderScriptDownloadedPayloadExecution</span></span>|[<span data-ttu-id="d9a52-624">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="d9a52-624">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="d9a52-625">从 Internet 下载的值，该值指示 js/vbs 执行负载的行为。</span><span class="sxs-lookup"><span data-stu-id="d9a52-625">Value indicating the behavior of js/vbs executing payload downloaded from Internet.</span></span> <span data-ttu-id="d9a52-626">可取值为：`userDefined`、`enable`、`auditMode`。</span><span class="sxs-lookup"><span data-stu-id="d9a52-626">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="d9a52-627">defenderPreventCredentialStealingType</span><span class="sxs-lookup"><span data-stu-id="d9a52-627">defenderPreventCredentialStealingType</span></span>|[<span data-ttu-id="d9a52-628">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="d9a52-628">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="d9a52-629">值，该值指示是否允许从 Windows 本地安全机构子系统窃取的凭据。</span><span class="sxs-lookup"><span data-stu-id="d9a52-629">Value indicating if credential stealing from the Windows local security authority subsystem is permitted.</span></span> <span data-ttu-id="d9a52-630">可取值为：`userDefined`、`enable`、`auditMode`。</span><span class="sxs-lookup"><span data-stu-id="d9a52-630">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="d9a52-631">defenderProcessCreationType</span><span class="sxs-lookup"><span data-stu-id="d9a52-631">defenderProcessCreationType</span></span>|[<span data-ttu-id="d9a52-632">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="d9a52-632">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="d9a52-633">值，该值指示响应来自 PSExec 和 WMI 命令的过程创建。</span><span class="sxs-lookup"><span data-stu-id="d9a52-633">Value indicating response to process creations originating from PSExec and WMI commands.</span></span> <span data-ttu-id="d9a52-634">可取值为：`userDefined`、`block`、`auditMode`。</span><span class="sxs-lookup"><span data-stu-id="d9a52-634">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="d9a52-635">defenderProcessCreation</span><span class="sxs-lookup"><span data-stu-id="d9a52-635">defenderProcessCreation</span></span>|[<span data-ttu-id="d9a52-636">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="d9a52-636">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="d9a52-637">值，该值指示响应来自 PSExec 和 WMI 命令的过程创建。</span><span class="sxs-lookup"><span data-stu-id="d9a52-637">Value indicating response to process creations originating from PSExec and WMI commands.</span></span> <span data-ttu-id="d9a52-638">可取值为：`userDefined`、`enable`、`auditMode`。</span><span class="sxs-lookup"><span data-stu-id="d9a52-638">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="d9a52-639">defenderUntrustedUSBProcessType</span><span class="sxs-lookup"><span data-stu-id="d9a52-639">defenderUntrustedUSBProcessType</span></span>|[<span data-ttu-id="d9a52-640">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="d9a52-640">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="d9a52-641">值，该值指示从 USB 运行的受信任和无符号流程的响应。</span><span class="sxs-lookup"><span data-stu-id="d9a52-641">Value indicating response to untrusted and unsigned processes that run from USB.</span></span> <span data-ttu-id="d9a52-642">可取值为：`userDefined`、`block`、`auditMode`。</span><span class="sxs-lookup"><span data-stu-id="d9a52-642">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="d9a52-643">defenderUntrustedUSBProcess</span><span class="sxs-lookup"><span data-stu-id="d9a52-643">defenderUntrustedUSBProcess</span></span>|[<span data-ttu-id="d9a52-644">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="d9a52-644">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="d9a52-645">值，该值指示从 USB 运行的受信任和无符号流程的响应。</span><span class="sxs-lookup"><span data-stu-id="d9a52-645">Value indicating response to untrusted and unsigned processes that run from USB.</span></span> <span data-ttu-id="d9a52-646">可取值为：`userDefined`、`enable`、`auditMode`。</span><span class="sxs-lookup"><span data-stu-id="d9a52-646">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="d9a52-647">defenderUntrustedExecutableType</span><span class="sxs-lookup"><span data-stu-id="d9a52-647">defenderUntrustedExecutableType</span></span>|[<span data-ttu-id="d9a52-648">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="d9a52-648">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="d9a52-649">值，该值指示响应可执行文件的传播、 年龄或受信任的列表不满足条件。</span><span class="sxs-lookup"><span data-stu-id="d9a52-649">Value indicating response to executables that don't meet a prevalence, age, or trusted list criteria.</span></span> <span data-ttu-id="d9a52-650">可取值为：`userDefined`、`block`、`auditMode`。</span><span class="sxs-lookup"><span data-stu-id="d9a52-650">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="d9a52-651">defenderUntrustedExecutable</span><span class="sxs-lookup"><span data-stu-id="d9a52-651">defenderUntrustedExecutable</span></span>|[<span data-ttu-id="d9a52-652">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="d9a52-652">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="d9a52-653">值，该值指示响应可执行文件的传播、 年龄或受信任的列表不满足条件。</span><span class="sxs-lookup"><span data-stu-id="d9a52-653">Value indicating response to executables that don't meet a prevalence, age, or trusted list criteria.</span></span> <span data-ttu-id="d9a52-654">可取值为：`userDefined`、`enable`、`auditMode`。</span><span class="sxs-lookup"><span data-stu-id="d9a52-654">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="d9a52-655">defenderEmailContentExecutionType</span><span class="sxs-lookup"><span data-stu-id="d9a52-655">defenderEmailContentExecutionType</span></span>|[<span data-ttu-id="d9a52-656">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="d9a52-656">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="d9a52-657">指示是否应该从电子邮件 （客户端 webmail/邮件） 放执行 （exe、 dll，ps、 js、 vbs 等） 的可执行内容的值。</span><span class="sxs-lookup"><span data-stu-id="d9a52-657">Value indicating if execution of executable content (exe, dll, ps, js, vbs, etc) should be dropped from email (webmail/mail-client).</span></span> <span data-ttu-id="d9a52-658">可取值为：`userDefined`、`block`、`auditMode`。</span><span class="sxs-lookup"><span data-stu-id="d9a52-658">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="d9a52-659">defenderEmailContentExecution</span><span class="sxs-lookup"><span data-stu-id="d9a52-659">defenderEmailContentExecution</span></span>|[<span data-ttu-id="d9a52-660">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="d9a52-660">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="d9a52-661">指示是否应该从电子邮件 （客户端 webmail/邮件） 放执行 （exe、 dll，ps、 js、 vbs 等） 的可执行内容的值。</span><span class="sxs-lookup"><span data-stu-id="d9a52-661">Value indicating if execution of executable content (exe, dll, ps, js, vbs, etc) should be dropped from email (webmail/mail-client).</span></span> <span data-ttu-id="d9a52-662">可取值为：`userDefined`、`enable`、`auditMode`。</span><span class="sxs-lookup"><span data-stu-id="d9a52-662">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="d9a52-663">defenderAdvancedRansomewareProtectionType</span><span class="sxs-lookup"><span data-stu-id="d9a52-663">defenderAdvancedRansomewareProtectionType</span></span>|[<span data-ttu-id="d9a52-664">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="d9a52-664">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="d9a52-665">指示使用高级防范 ransomeware 值。</span><span class="sxs-lookup"><span data-stu-id="d9a52-665">Value indicating use of advanced protection against ransomeware.</span></span> <span data-ttu-id="d9a52-666">可取值为：`userDefined`、`enable`、`auditMode`。</span><span class="sxs-lookup"><span data-stu-id="d9a52-666">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="d9a52-667">defenderGuardMyFoldersType</span><span class="sxs-lookup"><span data-stu-id="d9a52-667">defenderGuardMyFoldersType</span></span>|[<span data-ttu-id="d9a52-668">folderProtectionType</span><span class="sxs-lookup"><span data-stu-id="d9a52-668">folderProtectionType</span></span>](../resources/intune-deviceconfig-folderprotectiontype.md)|<span data-ttu-id="d9a52-669">指示受保护的文件夹的行为的值。</span><span class="sxs-lookup"><span data-stu-id="d9a52-669">Value indicating the behavior of protected folders.</span></span> <span data-ttu-id="d9a52-670">可取值为：`userDefined`、`enable`、`auditMode`、`blockDiskModification`、`auditDiskModification`。</span><span class="sxs-lookup"><span data-stu-id="d9a52-670">Possible values are: `userDefined`, `enable`, `auditMode`, `blockDiskModification`, `auditDiskModification`.</span></span>|
|<span data-ttu-id="d9a52-671">defenderGuardedFoldersAllowedAppPaths</span><span class="sxs-lookup"><span data-stu-id="d9a52-671">defenderGuardedFoldersAllowedAppPaths</span></span>|<span data-ttu-id="d9a52-672">String 集合</span><span class="sxs-lookup"><span data-stu-id="d9a52-672">String collection</span></span>|<span data-ttu-id="d9a52-673">允许访问受保护文件夹的 exe 路径列表</span><span class="sxs-lookup"><span data-stu-id="d9a52-673">List of paths to exe that are allowed to access protected folders</span></span>|
|<span data-ttu-id="d9a52-674">defenderAdditionalGuardedFolders</span><span class="sxs-lookup"><span data-stu-id="d9a52-674">defenderAdditionalGuardedFolders</span></span>|<span data-ttu-id="d9a52-675">String 集合</span><span class="sxs-lookup"><span data-stu-id="d9a52-675">String collection</span></span>|<span data-ttu-id="d9a52-676">要添加到受保护文件夹列表的文件夹路径列表</span><span class="sxs-lookup"><span data-stu-id="d9a52-676">List of folder paths to be added to the list of protected folders</span></span>|
|<span data-ttu-id="d9a52-677">defenderNetworkProtectionType</span><span class="sxs-lookup"><span data-stu-id="d9a52-677">defenderNetworkProtectionType</span></span>|[<span data-ttu-id="d9a52-678">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="d9a52-678">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="d9a52-679">指示 NetworkProtection 的行为的值。</span><span class="sxs-lookup"><span data-stu-id="d9a52-679">Value indicating the behavior of NetworkProtection.</span></span> <span data-ttu-id="d9a52-680">可取值为：`userDefined`、`enable`、`auditMode`。</span><span class="sxs-lookup"><span data-stu-id="d9a52-680">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="d9a52-681">defenderExploitProtectionXml</span><span class="sxs-lookup"><span data-stu-id="d9a52-681">defenderExploitProtectionXml</span></span>|<span data-ttu-id="d9a52-682">Binary</span><span class="sxs-lookup"><span data-stu-id="d9a52-682">Binary</span></span>|<span data-ttu-id="d9a52-683">包含有关 Exploit Protection 详细信息的 xml 内容。</span><span class="sxs-lookup"><span data-stu-id="d9a52-683">Xml content containing information regarding exploit protection details.</span></span>|
|<span data-ttu-id="d9a52-684">defenderExploitProtectionXmlFileName</span><span class="sxs-lookup"><span data-stu-id="d9a52-684">defenderExploitProtectionXmlFileName</span></span>|<span data-ttu-id="d9a52-685">String</span><span class="sxs-lookup"><span data-stu-id="d9a52-685">String</span></span>|<span data-ttu-id="d9a52-686">从中获取 DefenderExploitProtectionXml 的文件的名称。</span><span class="sxs-lookup"><span data-stu-id="d9a52-686">Name of the file from which DefenderExploitProtectionXml was obtained.</span></span>|
|<span data-ttu-id="d9a52-687">defenderSecurityCenterBlockExploitProtectionOverride</span><span class="sxs-lookup"><span data-stu-id="d9a52-687">defenderSecurityCenterBlockExploitProtectionOverride</span></span>|<span data-ttu-id="d9a52-688">Boolean</span><span class="sxs-lookup"><span data-stu-id="d9a52-688">Boolean</span></span>|<span data-ttu-id="d9a52-689">指示是否阻止用户覆盖 Exploit Protection 设置。</span><span class="sxs-lookup"><span data-stu-id="d9a52-689">Indicates whether or not to block user from overriding Exploit Protection settings.</span></span>|
|<span data-ttu-id="d9a52-690">appLockerApplicationControl</span><span class="sxs-lookup"><span data-stu-id="d9a52-690">appLockerApplicationControl</span></span>|[<span data-ttu-id="d9a52-691">appLockerApplicationControlType</span><span class="sxs-lookup"><span data-stu-id="d9a52-691">appLockerApplicationControlType</span></span>](../resources/intune-deviceconfig-applockerapplicationcontroltype.md)|<span data-ttu-id="d9a52-692">使管理员能够选择在设备上允许哪些类型的应用。</span><span class="sxs-lookup"><span data-stu-id="d9a52-692">Enables the Admin to choose what types of app to allow on devices.</span></span> <span data-ttu-id="d9a52-693">可取值为：`notConfigured`、`enforceComponentsAndStoreApps`、`auditComponentsAndStoreApps`、`enforceComponentsStoreAppsAndSmartlocker`、`auditComponentsStoreAppsAndSmartlocker`。</span><span class="sxs-lookup"><span data-stu-id="d9a52-693">Possible values are: `notConfigured`, `enforceComponentsAndStoreApps`, `auditComponentsAndStoreApps`, `enforceComponentsStoreAppsAndSmartlocker`, `auditComponentsStoreAppsAndSmartlocker`.</span></span>|
|<span data-ttu-id="d9a52-694">deviceGuardLocalSystemAuthorityCredentialGuardSettings</span><span class="sxs-lookup"><span data-stu-id="d9a52-694">deviceGuardLocalSystemAuthorityCredentialGuardSettings</span></span>|[<span data-ttu-id="d9a52-695">deviceGuardLocalSystemAuthorityCredentialGuardType</span><span class="sxs-lookup"><span data-stu-id="d9a52-695">deviceGuardLocalSystemAuthorityCredentialGuardType</span></span>](../resources/intune-deviceconfig-deviceguardlocalsystemauthoritycredentialguardtype.md)|<span data-ttu-id="d9a52-696">在凭据 Guard 时同时启用对安全启动和虚拟化基于安全平台安全级别打开。</span><span class="sxs-lookup"><span data-stu-id="d9a52-696">Turn on Credential Guard when Platform Security Level with Secure Boot and Virtualization Based Security are both enabled.</span></span> <span data-ttu-id="d9a52-697">可取值为：`notConfigured`、`enableWithUEFILock`、`enableWithoutUEFILock`。</span><span class="sxs-lookup"><span data-stu-id="d9a52-697">Possible values are: `notConfigured`, `enableWithUEFILock`, `enableWithoutUEFILock`.</span></span>|
|<span data-ttu-id="d9a52-698">deviceGuardEnableVirtualizationBasedSecurity</span><span class="sxs-lookup"><span data-stu-id="d9a52-698">deviceGuardEnableVirtualizationBasedSecurity</span></span>|<span data-ttu-id="d9a52-699">Boolean</span><span class="sxs-lookup"><span data-stu-id="d9a52-699">Boolean</span></span>|<span data-ttu-id="d9a52-700">虚拟化选项会启用基于 Security(VBS)。</span><span class="sxs-lookup"><span data-stu-id="d9a52-700">Turns On Virtualization Based Security(VBS).</span></span>|
|<span data-ttu-id="d9a52-701">deviceGuardEnableSecureBootWithDMA</span><span class="sxs-lookup"><span data-stu-id="d9a52-701">deviceGuardEnableSecureBootWithDMA</span></span>|<span data-ttu-id="d9a52-702">Boolean</span><span class="sxs-lookup"><span data-stu-id="d9a52-702">Boolean</span></span>|<span data-ttu-id="d9a52-703">指定是否将在下次重新启动启用平台安全级别。</span><span class="sxs-lookup"><span data-stu-id="d9a52-703">Specifies whether Platform Security Level is enabled at next reboot.</span></span>|
|<span data-ttu-id="d9a52-704">deviceGuardLaunchSystemGuard</span><span class="sxs-lookup"><span data-stu-id="d9a52-704">deviceGuardLaunchSystemGuard</span></span>|<span data-ttu-id="d9a52-705">[启用](../resources/intune-shared-enablement</span><span class="sxs-lookup"><span data-stu-id="d9a52-705">[enablement](../resources/intune-shared-enablement</span></span>
<span data-ttu-id="d9a52-706">.md)</span><span class="sxs-lookup"><span data-stu-id="d9a52-706">.md)</span></span>|<span data-ttu-id="d9a52-707">允许 IT 管理员配置的系统 Guard 启动。</span><span class="sxs-lookup"><span data-stu-id="d9a52-707">Allows the IT admin to configure the launch of System Guard.</span></span> <span data-ttu-id="d9a52-708">可取值为：`notConfigured`、`enabled`、`disabled`。</span><span class="sxs-lookup"><span data-stu-id="d9a52-708">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="d9a52-709">smartScreenEnableInShell</span><span class="sxs-lookup"><span data-stu-id="d9a52-709">smartScreenEnableInShell</span></span>|<span data-ttu-id="d9a52-710">Boolean</span><span class="sxs-lookup"><span data-stu-id="d9a52-710">Boolean</span></span>|<span data-ttu-id="d9a52-711">允许 IT 管理员配置适用于 Windows 的 SmartScreen。</span><span class="sxs-lookup"><span data-stu-id="d9a52-711">Allows IT Admins to configure SmartScreen for Windows.</span></span>|
|<span data-ttu-id="d9a52-712">smartScreenBlockOverrideForFiles</span><span class="sxs-lookup"><span data-stu-id="d9a52-712">smartScreenBlockOverrideForFiles</span></span>|<span data-ttu-id="d9a52-713">Boolean</span><span class="sxs-lookup"><span data-stu-id="d9a52-713">Boolean</span></span>|<span data-ttu-id="d9a52-714">允许 IT 管理员控制用户是否可以忽略 SmartScreen 警告并运行恶意文件。</span><span class="sxs-lookup"><span data-stu-id="d9a52-714">Allows IT Admins to control whether users can can ignore SmartScreen warnings and run malicious files.</span></span>|
|<span data-ttu-id="d9a52-715">applicationGuardEnabled</span><span class="sxs-lookup"><span data-stu-id="d9a52-715">applicationGuardEnabled</span></span>|<span data-ttu-id="d9a52-716">Boolean</span><span class="sxs-lookup"><span data-stu-id="d9a52-716">Boolean</span></span>|<span data-ttu-id="d9a52-717">启用 Windows Defender 应用程序防护</span><span class="sxs-lookup"><span data-stu-id="d9a52-717">Enable Windows Defender Application Guard</span></span>|
|<span data-ttu-id="d9a52-718">applicationGuardEnabledOptions</span><span class="sxs-lookup"><span data-stu-id="d9a52-718">applicationGuardEnabledOptions</span></span>|[<span data-ttu-id="d9a52-719">applicationGuardEnabledOptions</span><span class="sxs-lookup"><span data-stu-id="d9a52-719">applicationGuardEnabledOptions</span></span>](../resources/intune-deviceconfig-applicationguardenabledoptions.md)|<span data-ttu-id="d9a52-720">Windows Defender 应用程序 Guard 启用更高版本的 Windows 版本。</span><span class="sxs-lookup"><span data-stu-id="d9a52-720">Enable Windows Defender Application Guard for newer Windows builds.</span></span> <span data-ttu-id="d9a52-721">可取值为：`notConfigured`、`enabledForEdge`、`enabledForOffice`、`enabledForEdgeAndOffice`。</span><span class="sxs-lookup"><span data-stu-id="d9a52-721">Possible values are: `notConfigured`, `enabledForEdge`, `enabledForOffice`, `enabledForEdgeAndOffice`.</span></span>|
|<span data-ttu-id="d9a52-722">applicationGuardBlockFileTransfer</span><span class="sxs-lookup"><span data-stu-id="d9a52-722">applicationGuardBlockFileTransfer</span></span>|[<span data-ttu-id="d9a52-723">applicationGuardBlockFileTransferType</span><span class="sxs-lookup"><span data-stu-id="d9a52-723">applicationGuardBlockFileTransferType</span></span>](../resources/intune-deviceconfig-applicationguardblockfiletransfertype.md)|<span data-ttu-id="d9a52-724">阻止传输图像文件、 文本文件或两者到剪贴板。</span><span class="sxs-lookup"><span data-stu-id="d9a52-724">Block clipboard to transfer image file, text file or neither of them.</span></span> <span data-ttu-id="d9a52-725">可取值为：`notConfigured`、`blockImageAndTextFile`、`blockImageFile`、`blockNone`、`blockTextFile`。</span><span class="sxs-lookup"><span data-stu-id="d9a52-725">Possible values are: `notConfigured`, `blockImageAndTextFile`, `blockImageFile`, `blockNone`, `blockTextFile`.</span></span>|
|<span data-ttu-id="d9a52-726">applicationGuardBlockNonEnterpriseContent</span><span class="sxs-lookup"><span data-stu-id="d9a52-726">applicationGuardBlockNonEnterpriseContent</span></span>|<span data-ttu-id="d9a52-727">Boolean</span><span class="sxs-lookup"><span data-stu-id="d9a52-727">Boolean</span></span>|<span data-ttu-id="d9a52-728">阻止企业站点加载非企业内容，例如第三方插件</span><span class="sxs-lookup"><span data-stu-id="d9a52-728">Block enterprise sites to load non-enterprise content, such as third party plug-ins</span></span>|
|<span data-ttu-id="d9a52-729">applicationGuardAllowPersistence</span><span class="sxs-lookup"><span data-stu-id="d9a52-729">applicationGuardAllowPersistence</span></span>|<span data-ttu-id="d9a52-730">Boolean</span><span class="sxs-lookup"><span data-stu-id="d9a52-730">Boolean</span></span>|<span data-ttu-id="d9a52-731">允许 App Guard 容器（收藏夹、Cookie、Web 密码等）内的持久用户生成数据</span><span class="sxs-lookup"><span data-stu-id="d9a52-731">Allow persisting user generated data inside the App Guard Containter (favorites, cookies, web passwords, etc.)</span></span>|
|<span data-ttu-id="d9a52-732">applicationGuardForceAuditing</span><span class="sxs-lookup"><span data-stu-id="d9a52-732">applicationGuardForceAuditing</span></span>|<span data-ttu-id="d9a52-733">Boolean</span><span class="sxs-lookup"><span data-stu-id="d9a52-733">Boolean</span></span>|<span data-ttu-id="d9a52-734">强制审核将存留 Windows 日志和事件以满足安全/符合性条件（示例事件是用户登录注销、特权使用、软件安装、系统更改等）</span><span class="sxs-lookup"><span data-stu-id="d9a52-734">Force auditing will persist Windows logs and events to meet security/compliance criteria (sample events are user login-logoff, use of privilege rights, software installation, system changes, etc.)</span></span>|
|<span data-ttu-id="d9a52-735">applicationGuardBlockClipboardSharing</span><span class="sxs-lookup"><span data-stu-id="d9a52-735">applicationGuardBlockClipboardSharing</span></span>|[<span data-ttu-id="d9a52-736">applicationGuardBlockClipboardSharingType</span><span class="sxs-lookup"><span data-stu-id="d9a52-736">applicationGuardBlockClipboardSharingType</span></span>](../resources/intune-deviceconfig-applicationguardblockclipboardsharingtype.md)|<span data-ttu-id="d9a52-737">阻止剪贴板将数据从主机共享到容器或从容器共享到主机，或阻止两种方式，或两种方式均不阻止。</span><span class="sxs-lookup"><span data-stu-id="d9a52-737">Block clipboard to share data from Host to Container, or from Container to Host, or both ways, or neither ways.</span></span> <span data-ttu-id="d9a52-738">可取值为：`notConfigured`、`blockBoth`、`blockHostToContainer`、`blockContainerToHost`、`blockNone`。</span><span class="sxs-lookup"><span data-stu-id="d9a52-738">Possible values are: `notConfigured`, `blockBoth`, `blockHostToContainer`, `blockContainerToHost`, `blockNone`.</span></span>|
|<span data-ttu-id="d9a52-739">applicationGuardAllowPrintToPDF</span><span class="sxs-lookup"><span data-stu-id="d9a52-739">applicationGuardAllowPrintToPDF</span></span>|<span data-ttu-id="d9a52-740">Boolean</span><span class="sxs-lookup"><span data-stu-id="d9a52-740">Boolean</span></span>|<span data-ttu-id="d9a52-741">允许从容器打印为 PDF 格式</span><span class="sxs-lookup"><span data-stu-id="d9a52-741">Allow printing to PDF from Container</span></span>|
|<span data-ttu-id="d9a52-742">applicationGuardAllowPrintToXPS</span><span class="sxs-lookup"><span data-stu-id="d9a52-742">applicationGuardAllowPrintToXPS</span></span>|<span data-ttu-id="d9a52-743">Boolean</span><span class="sxs-lookup"><span data-stu-id="d9a52-743">Boolean</span></span>|<span data-ttu-id="d9a52-744">允许从容器打印为 XPS 格式</span><span class="sxs-lookup"><span data-stu-id="d9a52-744">Allow printing to XPS from Container</span></span>|
|<span data-ttu-id="d9a52-745">applicationGuardAllowPrintToLocalPrinters</span><span class="sxs-lookup"><span data-stu-id="d9a52-745">applicationGuardAllowPrintToLocalPrinters</span></span>|<span data-ttu-id="d9a52-746">Boolean</span><span class="sxs-lookup"><span data-stu-id="d9a52-746">Boolean</span></span>|<span data-ttu-id="d9a52-747">允许从容器打印到本地打印机</span><span class="sxs-lookup"><span data-stu-id="d9a52-747">Allow printing to Local Printers from Container</span></span>|
|<span data-ttu-id="d9a52-748">applicationGuardAllowPrintToNetworkPrinters</span><span class="sxs-lookup"><span data-stu-id="d9a52-748">applicationGuardAllowPrintToNetworkPrinters</span></span>|<span data-ttu-id="d9a52-749">Boolean</span><span class="sxs-lookup"><span data-stu-id="d9a52-749">Boolean</span></span>|<span data-ttu-id="d9a52-750">允许从容器打印到网络打印机</span><span class="sxs-lookup"><span data-stu-id="d9a52-750">Allow printing to Network Printers from Container</span></span>|
|<span data-ttu-id="d9a52-751">applicationGuardAllowVirtualGPU</span><span class="sxs-lookup"><span data-stu-id="d9a52-751">applicationGuardAllowVirtualGPU</span></span>|<span data-ttu-id="d9a52-752">Boolean</span><span class="sxs-lookup"><span data-stu-id="d9a52-752">Boolean</span></span>|<span data-ttu-id="d9a52-753">允许应用程序 guard 用于虚拟 GPU</span><span class="sxs-lookup"><span data-stu-id="d9a52-753">Allow application guard to use virtual GPU</span></span>|
|<span data-ttu-id="d9a52-754">applicationGuardAllowFileSaveOnHost</span><span class="sxs-lookup"><span data-stu-id="d9a52-754">applicationGuardAllowFileSaveOnHost</span></span>|<span data-ttu-id="d9a52-755">Boolean</span><span class="sxs-lookup"><span data-stu-id="d9a52-755">Boolean</span></span>|<span data-ttu-id="d9a52-756">允许用户从应用程序 guard 容器中的边缘下载文件并将其保存在主机上文件系统</span><span class="sxs-lookup"><span data-stu-id="d9a52-756">Allow users to download files from Edge in the application guard container and save them on the host file system</span></span>|
|<span data-ttu-id="d9a52-757">bitLockerAllowStandardUserEncryption</span><span class="sxs-lookup"><span data-stu-id="d9a52-757">bitLockerAllowStandardUserEncryption</span></span>|<span data-ttu-id="d9a52-758">Boolean</span><span class="sxs-lookup"><span data-stu-id="d9a52-758">Boolean</span></span>|<span data-ttu-id="d9a52-759">允许管理员允许在 Azure AD 加入过程中启用 encrpytion 标准用户。</span><span class="sxs-lookup"><span data-stu-id="d9a52-759">Allows the admin to allow standard users to enable encrpytion during Azure AD Join.</span></span>|
|<span data-ttu-id="d9a52-760">bitLockerDisableWarningForOtherDiskEncryption</span><span class="sxs-lookup"><span data-stu-id="d9a52-760">bitLockerDisableWarningForOtherDiskEncryption</span></span>|<span data-ttu-id="d9a52-761">Boolean</span><span class="sxs-lookup"><span data-stu-id="d9a52-761">Boolean</span></span>|<span data-ttu-id="d9a52-762">允许管理员禁用对用户计算机上其他磁盘加密的警告提示。</span><span class="sxs-lookup"><span data-stu-id="d9a52-762">Allows the Admin to disable the warning prompt for other disk encryption on the user machines.</span></span>|
|<span data-ttu-id="d9a52-763">bitLockerEnableStorageCardEncryptionOnMobile</span><span class="sxs-lookup"><span data-stu-id="d9a52-763">bitLockerEnableStorageCardEncryptionOnMobile</span></span>|<span data-ttu-id="d9a52-764">Boolean</span><span class="sxs-lookup"><span data-stu-id="d9a52-764">Boolean</span></span>|<span data-ttu-id="d9a52-765">允许管理员要求使用 BitLocker 开启加密功能。</span><span class="sxs-lookup"><span data-stu-id="d9a52-765">Allows the admin to require encryption to be turned on using BitLocker.</span></span> <span data-ttu-id="d9a52-766">此策略仅适用于移动 SKU。</span><span class="sxs-lookup"><span data-stu-id="d9a52-766">This policy is valid only for a mobile SKU.</span></span>|
|<span data-ttu-id="d9a52-767">bitLockerEncryptDevice</span><span class="sxs-lookup"><span data-stu-id="d9a52-767">bitLockerEncryptDevice</span></span>|<span data-ttu-id="d9a52-768">Boolean</span><span class="sxs-lookup"><span data-stu-id="d9a52-768">Boolean</span></span>|<span data-ttu-id="d9a52-769">允许管理员要求使用 BitLocker 开启加密功能。</span><span class="sxs-lookup"><span data-stu-id="d9a52-769">Allows the admin to require encryption to be turned on using BitLocker.</span></span>|
|<span data-ttu-id="d9a52-770">bitLockerSystemDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="d9a52-770">bitLockerSystemDrivePolicy</span></span>|[<span data-ttu-id="d9a52-771">bitLockerSystemDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="d9a52-771">bitLockerSystemDrivePolicy</span></span>](../resources/intune-deviceconfig-bitlockersystemdrivepolicy.md)|<span data-ttu-id="d9a52-772">BitLocker 系统驱动器策略。</span><span class="sxs-lookup"><span data-stu-id="d9a52-772">BitLocker System Drive Policy.</span></span>|
|<span data-ttu-id="d9a52-773">bitLockerFixedDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="d9a52-773">bitLockerFixedDrivePolicy</span></span>|[<span data-ttu-id="d9a52-774">bitLockerFixedDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="d9a52-774">bitLockerFixedDrivePolicy</span></span>](../resources/intune-deviceconfig-bitlockerfixeddrivepolicy.md)|<span data-ttu-id="d9a52-775">BitLocker 固定驱动器策略。</span><span class="sxs-lookup"><span data-stu-id="d9a52-775">BitLocker Fixed Drive Policy.</span></span>|
|<span data-ttu-id="d9a52-776">bitLockerRemovableDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="d9a52-776">bitLockerRemovableDrivePolicy</span></span>|[<span data-ttu-id="d9a52-777">bitLockerRemovableDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="d9a52-777">bitLockerRemovableDrivePolicy</span></span>](../resources/intune-deviceconfig-bitlockerremovabledrivepolicy.md)|<span data-ttu-id="d9a52-778">BitLocker 可移动驱动器策略。</span><span class="sxs-lookup"><span data-stu-id="d9a52-778">BitLocker Removable Drive Policy.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d9a52-779">关系</span><span class="sxs-lookup"><span data-stu-id="d9a52-779">Relationships</span></span>
|<span data-ttu-id="d9a52-780">关系</span><span class="sxs-lookup"><span data-stu-id="d9a52-780">Relationship</span></span>|<span data-ttu-id="d9a52-781">类型</span><span class="sxs-lookup"><span data-stu-id="d9a52-781">Type</span></span>|<span data-ttu-id="d9a52-782">说明</span><span class="sxs-lookup"><span data-stu-id="d9a52-782">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d9a52-783">groupAssignments</span><span class="sxs-lookup"><span data-stu-id="d9a52-783">groupAssignments</span></span>|<span data-ttu-id="d9a52-784">[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)集合</span><span class="sxs-lookup"><span data-stu-id="d9a52-784">[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) collection</span></span>|<span data-ttu-id="d9a52-785">设备配置文件的组分配列表。</span><span class="sxs-lookup"><span data-stu-id="d9a52-785">The list of group assignments for the device configuration profile.</span></span> <span data-ttu-id="d9a52-786">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d9a52-786">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d9a52-787">assignments</span><span class="sxs-lookup"><span data-stu-id="d9a52-787">assignments</span></span>|<span data-ttu-id="d9a52-788">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="d9a52-788">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection</span></span>|<span data-ttu-id="d9a52-789">设备配置文件的分配列表。</span><span class="sxs-lookup"><span data-stu-id="d9a52-789">The list of assignments for the device configuration profile.</span></span> <span data-ttu-id="d9a52-790">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d9a52-790">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d9a52-791">deviceStatuses</span><span class="sxs-lookup"><span data-stu-id="d9a52-791">deviceStatuses</span></span>|<span data-ttu-id="d9a52-792">[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) 集合</span><span class="sxs-lookup"><span data-stu-id="d9a52-792">[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) collection</span></span>|<span data-ttu-id="d9a52-793">按设备的设备配置安装状态。</span><span class="sxs-lookup"><span data-stu-id="d9a52-793">Device configuration installation status by device.</span></span> <span data-ttu-id="d9a52-794">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d9a52-794">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d9a52-795">userStatuses</span><span class="sxs-lookup"><span data-stu-id="d9a52-795">userStatuses</span></span>|<span data-ttu-id="d9a52-796">[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) 集合</span><span class="sxs-lookup"><span data-stu-id="d9a52-796">[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) collection</span></span>|<span data-ttu-id="d9a52-797">用户的设备配置安装状态。</span><span class="sxs-lookup"><span data-stu-id="d9a52-797">Device configuration installation status by user.</span></span> <span data-ttu-id="d9a52-798">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d9a52-798">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d9a52-799">deviceStatusOverview</span><span class="sxs-lookup"><span data-stu-id="d9a52-799">deviceStatusOverview</span></span>|[<span data-ttu-id="d9a52-800">deviceConfigurationDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="d9a52-800">deviceConfigurationDeviceOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|<span data-ttu-id="d9a52-801">设备配置设备状态概述 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d9a52-801">Device Configuration devices status overview Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d9a52-802">userStatusOverview</span><span class="sxs-lookup"><span data-stu-id="d9a52-802">userStatusOverview</span></span>|[<span data-ttu-id="d9a52-803">deviceConfigurationUserOverview</span><span class="sxs-lookup"><span data-stu-id="d9a52-803">deviceConfigurationUserOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|<span data-ttu-id="d9a52-804">设备配置用户状态概述 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d9a52-804">Device Configuration users status overview Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d9a52-805">deviceSettingStateSummaries</span><span class="sxs-lookup"><span data-stu-id="d9a52-805">deviceSettingStateSummaries</span></span>|<span data-ttu-id="d9a52-806">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) 集合</span><span class="sxs-lookup"><span data-stu-id="d9a52-806">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) collection</span></span>|<span data-ttu-id="d9a52-807">设备配置设置状态设备摘要 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d9a52-807">Device Configuration Setting State Device Summary Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d9a52-808">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d9a52-808">JSON Representation</span></span>
<span data-ttu-id="d9a52-809">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d9a52-809">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windows10EndpointProtectionConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windows10EndpointProtectionConfiguration",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "roleScopeTagIds": [
    "String"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "displayName": "String",
  "version": 1024,
  "dmaGuardDeviceEnumerationPolicy": "String",
  "userRightsAccessCredentialManagerAsTrustedCaller": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "String",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "String",
        "description": "String",
        "securityIdentifier": "String"
      }
    ]
  },
  "userRightsAllowAccessFromNetwork": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "String",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "String",
        "description": "String",
        "securityIdentifier": "String"
      }
    ]
  },
  "userRightsBlockAccessFromNetwork": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "String",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "String",
        "description": "String",
        "securityIdentifier": "String"
      }
    ]
  },
  "userRightsActAsPartOfTheOperatingSystem": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "String",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "String",
        "description": "String",
        "securityIdentifier": "String"
      }
    ]
  },
  "userRightsLocalLogOn": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "String",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "String",
        "description": "String",
        "securityIdentifier": "String"
      }
    ]
  },
  "userRightsBackupData": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "String",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "String",
        "description": "String",
        "securityIdentifier": "String"
      }
    ]
  },
  "userRightsChangeSystemTime": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "String",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "String",
        "description": "String",
        "securityIdentifier": "String"
      }
    ]
  },
  "userRightsCreateGlobalObjects": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "String",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "String",
        "description": "String",
        "securityIdentifier": "String"
      }
    ]
  },
  "userRightsCreatePageFile": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "String",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "String",
        "description": "String",
        "securityIdentifier": "String"
      }
    ]
  },
  "userRightsCreatePermanentSharedObjects": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "String",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "String",
        "description": "String",
        "securityIdentifier": "String"
      }
    ]
  },
  "userRightsCreateSymbolicLinks": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "String",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "String",
        "description": "String",
        "securityIdentifier": "String"
      }
    ]
  },
  "userRightsCreateToken": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "String",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "String",
        "description": "String",
        "securityIdentifier": "String"
      }
    ]
  },
  "userRightsDebugPrograms": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "String",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "String",
        "description": "String",
        "securityIdentifier": "String"
      }
    ]
  },
  "userRightsRemoteDesktopServicesLogOn": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "String",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "String",
        "description": "String",
        "securityIdentifier": "String"
      }
    ]
  },
  "userRightsDelegation": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "String",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "String",
        "description": "String",
        "securityIdentifier": "String"
      }
    ]
  },
  "userRightsGenerateSecurityAudits": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "String",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "String",
        "description": "String",
        "securityIdentifier": "String"
      }
    ]
  },
  "userRightsImpersonateClient": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "String",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "String",
        "description": "String",
        "securityIdentifier": "String"
      }
    ]
  },
  "userRightsIncreaseSchedulingPriority": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "String",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "String",
        "description": "String",
        "securityIdentifier": "String"
      }
    ]
  },
  "userRightsLoadUnloadDrivers": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "String",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "String",
        "description": "String",
        "securityIdentifier": "String"
      }
    ]
  },
  "userRightsLockMemory": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "String",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "String",
        "description": "String",
        "securityIdentifier": "String"
      }
    ]
  },
  "userRightsManageAuditingAndSecurityLogs": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "String",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "String",
        "description": "String",
        "securityIdentifier": "String"
      }
    ]
  },
  "userRightsManageVolumes": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "String",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "String",
        "description": "String",
        "securityIdentifier": "String"
      }
    ]
  },
  "userRightsModifyFirmwareEnvironment": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "String",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "String",
        "description": "String",
        "securityIdentifier": "String"
      }
    ]
  },
  "userRightsModifyObjectLabels": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "String",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "String",
        "description": "String",
        "securityIdentifier": "String"
      }
    ]
  },
  "userRightsProfileSingleProcess": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "String",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "String",
        "description": "String",
        "securityIdentifier": "String"
      }
    ]
  },
  "userRightsRemoteShutdown": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "String",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "String",
        "description": "String",
        "securityIdentifier": "String"
      }
    ]
  },
  "userRightsRestoreData": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "String",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "String",
        "description": "String",
        "securityIdentifier": "String"
      }
    ]
  },
  "userRightsTakeOwnership": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "String",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "String",
        "description": "String",
        "securityIdentifier": "String"
      }
    ]
  },
  "userRightsRegisterProcessAsService": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "String",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "String",
        "description": "String",
        "securityIdentifier": "String"
      }
    ]
  },
  "xboxServicesEnableXboxGameSaveTask": true,
  "xboxServicesAccessoryManagementServiceStartupMode": "String",
  "xboxServicesLiveAuthManagerServiceStartupMode": "String",
  "xboxServicesLiveGameSaveServiceStartupMode": "String",
  "xboxServicesLiveNetworkingServiceStartupMode": "String",
  "localSecurityOptionsBlockMicrosoftAccounts": true,
  "localSecurityOptionsBlockRemoteLogonWithBlankPassword": true,
  "localSecurityOptionsDisableAdministratorAccount": true,
  "localSecurityOptionsAdministratorAccountName": "String",
  "localSecurityOptionsDisableGuestAccount": true,
  "localSecurityOptionsGuestAccountName": "String",
  "localSecurityOptionsAllowUndockWithoutHavingToLogon": true,
  "localSecurityOptionsBlockUsersInstallingPrinterDrivers": true,
  "localSecurityOptionsBlockRemoteOpticalDriveAccess": true,
  "localSecurityOptionsFormatAndEjectOfRemovableMediaAllowedUser": "String",
  "localSecurityOptionsMachineInactivityLimit": 1024,
  "localSecurityOptionsMachineInactivityLimitInMinutes": 1024,
  "localSecurityOptionsDoNotRequireCtrlAltDel": true,
  "localSecurityOptionsHideLastSignedInUser": true,
  "localSecurityOptionsHideUsernameAtSignIn": true,
  "localSecurityOptionsLogOnMessageTitle": "String",
  "localSecurityOptionsLogOnMessageText": "String",
  "localSecurityOptionsAllowPKU2UAuthenticationRequests": true,
  "localSecurityOptionsAllowRemoteCallsToSecurityAccountsManagerHelperBool": true,
  "localSecurityOptionsAllowRemoteCallsToSecurityAccountsManager": "String",
  "localSecurityOptionsMinimumSessionSecurityForNtlmSspBasedClients": "String",
  "localSecurityOptionsMinimumSessionSecurityForNtlmSspBasedServers": "String",
  "lanManagerAuthenticationLevel": "String",
  "lanManagerWorkstationDisableInsecureGuestLogons": true,
  "localSecurityOptionsClearVirtualMemoryPageFile": true,
  "localSecurityOptionsAllowSystemToBeShutDownWithoutHavingToLogOn": true,
  "localSecurityOptionsAllowUIAccessApplicationElevation": true,
  "localSecurityOptionsVirtualizeFileAndRegistryWriteFailuresToPerUserLocations": true,
  "localSecurityOptionsOnlyElevateSignedExecutables": true,
  "localSecurityOptionsAdministratorElevationPromptBehavior": "String",
  "localSecurityOptionsStandardUserElevationPromptBehavior": "String",
  "localSecurityOptionsSwitchToSecureDesktopWhenPromptingForElevation": true,
  "localSecurityOptionsDetectApplicationInstallationsAndPromptForElevation": true,
  "localSecurityOptionsAllowUIAccessApplicationsForSecureLocations": true,
  "localSecurityOptionsUseAdminApprovalMode": true,
  "localSecurityOptionsUseAdminApprovalModeForAdministrators": true,
  "localSecurityOptionsInformationShownOnLockScreen": "String",
  "localSecurityOptionsInformationDisplayedOnLockScreen": "String",
  "localSecurityOptionsDisableClientDigitallySignCommunicationsIfServerAgrees": true,
  "localSecurityOptionsClientDigitallySignCommunicationsAlways": true,
  "localSecurityOptionsClientSendUnencryptedPasswordToThirdPartySMBServers": true,
  "localSecurityOptionsDisableServerDigitallySignCommunicationsAlways": true,
  "localSecurityOptionsDisableServerDigitallySignCommunicationsIfClientAgrees": true,
  "localSecurityOptionsRestrictAnonymousAccessToNamedPipesAndShares": true,
  "localSecurityOptionsDoNotAllowAnonymousEnumerationOfSAMAccounts": true,
  "localSecurityOptionsAllowAnonymousEnumerationOfSAMAccountsAndShares": true,
  "localSecurityOptionsDoNotStoreLANManagerHashValueOnNextPasswordChange": true,
  "localSecurityOptionsSmartCardRemovalBehavior": "String",
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
  "defenderSecurityCenterOrganizationDisplayName": "String",
  "defenderSecurityCenterHelpEmail": "String",
  "defenderSecurityCenterHelpPhone": "String",
  "defenderSecurityCenterHelpURL": "String",
  "defenderSecurityCenterNotificationsFromApp": "String",
  "defenderSecurityCenterITContactDisplay": "String",
  "firewallBlockStatefulFTP": true,
  "firewallIdleTimeoutForSecurityAssociationInSeconds": 1024,
  "firewallPreSharedKeyEncodingMethod": "String",
  "firewallIPSecExemptionsAllowNeighborDiscovery": true,
  "firewallIPSecExemptionsAllowICMP": true,
  "firewallIPSecExemptionsAllowRouterDiscovery": true,
  "firewallIPSecExemptionsAllowDHCP": true,
  "firewallCertificateRevocationListCheckMethod": "String",
  "firewallMergeKeyingModuleSettings": true,
  "firewallPacketQueueingMethod": "String",
  "firewallProfileDomain": {
    "@odata.type": "microsoft.graph.windowsFirewallNetworkProfile",
    "firewallEnabled": "String",
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
    "firewallEnabled": "String",
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
    "firewallEnabled": "String",
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
    "String"
  ],
  "defenderOfficeAppsOtherProcessInjectionType": "String",
  "defenderOfficeAppsOtherProcessInjection": "String",
  "defenderOfficeAppsExecutableContentCreationOrLaunchType": "String",
  "defenderOfficeAppsExecutableContentCreationOrLaunch": "String",
  "defenderOfficeAppsLaunchChildProcessType": "String",
  "defenderOfficeAppsLaunchChildProcess": "String",
  "defenderOfficeMacroCodeAllowWin32ImportsType": "String",
  "defenderOfficeMacroCodeAllowWin32Imports": "String",
  "defenderScriptObfuscatedMacroCodeType": "String",
  "defenderScriptObfuscatedMacroCode": "String",
  "defenderScriptDownloadedPayloadExecutionType": "String",
  "defenderScriptDownloadedPayloadExecution": "String",
  "defenderPreventCredentialStealingType": "String",
  "defenderProcessCreationType": "String",
  "defenderProcessCreation": "String",
  "defenderUntrustedUSBProcessType": "String",
  "defenderUntrustedUSBProcess": "String",
  "defenderUntrustedExecutableType": "String",
  "defenderUntrustedExecutable": "String",
  "defenderEmailContentExecutionType": "String",
  "defenderEmailContentExecution": "String",
  "defenderAdvancedRansomewareProtectionType": "String",
  "defenderGuardMyFoldersType": "String",
  "defenderGuardedFoldersAllowedAppPaths": [
    "String"
  ],
  "defenderAdditionalGuardedFolders": [
    "String"
  ],
  "defenderNetworkProtectionType": "String",
  "defenderExploitProtectionXml": "binary",
  "defenderExploitProtectionXmlFileName": "String",
  "defenderSecurityCenterBlockExploitProtectionOverride": true,
  "appLockerApplicationControl": "String",
  "deviceGuardLocalSystemAuthorityCredentialGuardSettings": "String",
  "deviceGuardEnableVirtualizationBasedSecurity": true,
  "deviceGuardEnableSecureBootWithDMA": true,
  "deviceGuardLaunchSystemGuard": "String",
  "smartScreenEnableInShell": true,
  "smartScreenBlockOverrideForFiles": true,
  "applicationGuardEnabled": true,
  "applicationGuardEnabledOptions": "String",
  "applicationGuardBlockFileTransfer": "String",
  "applicationGuardBlockNonEnterpriseContent": true,
  "applicationGuardAllowPersistence": true,
  "applicationGuardForceAuditing": true,
  "applicationGuardBlockClipboardSharing": "String",
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
    "encryptionMethod": "String",
    "startupAuthenticationRequired": true,
    "startupAuthenticationBlockWithoutTpmChip": true,
    "startupAuthenticationTpmUsage": "String",
    "startupAuthenticationTpmPinUsage": "String",
    "startupAuthenticationTpmKeyUsage": "String",
    "startupAuthenticationTpmPinAndKeyUsage": "String",
    "minimumPinLength": 1024,
    "recoveryOptions": {
      "@odata.type": "microsoft.graph.bitLockerRecoveryOptions",
      "blockDataRecoveryAgent": true,
      "recoveryPasswordUsage": "String",
      "recoveryKeyUsage": "String",
      "hideRecoveryOptions": true,
      "enableRecoveryInformationSaveToStore": true,
      "recoveryInformationToStore": "String",
      "enableBitLockerAfterRecoveryInformationToStore": true
    },
    "prebootRecoveryEnableMessageAndUrl": true,
    "prebootRecoveryMessage": "String",
    "prebootRecoveryUrl": "String"
  },
  "bitLockerFixedDrivePolicy": {
    "@odata.type": "microsoft.graph.bitLockerFixedDrivePolicy",
    "encryptionMethod": "String",
    "requireEncryptionForWriteAccess": true,
    "recoveryOptions": {
      "@odata.type": "microsoft.graph.bitLockerRecoveryOptions",
      "blockDataRecoveryAgent": true,
      "recoveryPasswordUsage": "String",
      "recoveryKeyUsage": "String",
      "hideRecoveryOptions": true,
      "enableRecoveryInformationSaveToStore": true,
      "recoveryInformationToStore": "String",
      "enableBitLockerAfterRecoveryInformationToStore": true
    }
  },
  "bitLockerRemovableDrivePolicy": {
    "@odata.type": "microsoft.graph.bitLockerRemovableDrivePolicy",
    "encryptionMethod": "String",
    "requireEncryptionForWriteAccess": true,
    "blockCrossOrganizationWriteAccess": true
  }
}
```




