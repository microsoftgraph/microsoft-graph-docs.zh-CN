---
title: windows10EndpointProtectionConfiguration 资源类型
description: 本主题提供由 Windows10EndpointProtectionConfiguration 资源公开的已声明方法、属性和关系的说明。
ms.openlocfilehash: 6d982a2296bdc4b70abc6c75db913fb79702c53c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27045725"
---
# <a name="windows10endpointprotectionconfiguration-resource-type"></a><span data-ttu-id="b588a-103">windows10EndpointProtectionConfiguration 资源类型</span><span class="sxs-lookup"><span data-stu-id="b588a-103">windows10EndpointProtectionConfiguration resource type</span></span>

> <span data-ttu-id="b588a-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="b588a-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b588a-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="b588a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b588a-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="b588a-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b588a-107">本主题提供由 Windows10EndpointProtectionConfiguration 资源公开的已声明方法、属性和关系的说明。</span><span class="sxs-lookup"><span data-stu-id="b588a-107">This topic provides descriptions of the declared methods, properties and relationships exposed by the Windows10EndpointProtectionConfiguration resource.</span></span>

<span data-ttu-id="b588a-108">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b588a-108">Inherits from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>

## <a name="methods"></a><span data-ttu-id="b588a-109">方法</span><span class="sxs-lookup"><span data-stu-id="b588a-109">Methods</span></span>
|<span data-ttu-id="b588a-110">方法</span><span class="sxs-lookup"><span data-stu-id="b588a-110">Method</span></span>|<span data-ttu-id="b588a-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="b588a-111">Return Type</span></span>|<span data-ttu-id="b588a-112">说明</span><span class="sxs-lookup"><span data-stu-id="b588a-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="b588a-113">List windows10EndpointProtectionConfigurations</span><span class="sxs-lookup"><span data-stu-id="b588a-113">List windows10EndpointProtectionConfigurations</span></span>](../api/intune-deviceconfig-windows10endpointprotectionconfiguration-list.md)|<span data-ttu-id="b588a-114">[windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) 集合</span><span class="sxs-lookup"><span data-stu-id="b588a-114">[windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) collection</span></span>|<span data-ttu-id="b588a-115">列出 [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="b588a-115">List properties and relationships of the [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="b588a-116">Get windows10EndpointProtectionConfiguration</span><span class="sxs-lookup"><span data-stu-id="b588a-116">Get windows10EndpointProtectionConfiguration</span></span>](../api/intune-deviceconfig-windows10endpointprotectionconfiguration-get.md)|[<span data-ttu-id="b588a-117">windows10EndpointProtectionConfiguration</span><span class="sxs-lookup"><span data-stu-id="b588a-117">windows10EndpointProtectionConfiguration</span></span>](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md)|<span data-ttu-id="b588a-118">读取 [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="b588a-118">Read properties and relationships of the [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) object.</span></span>|
|[<span data-ttu-id="b588a-119">Create windows10EndpointProtectionConfiguration</span><span class="sxs-lookup"><span data-stu-id="b588a-119">Create windows10EndpointProtectionConfiguration</span></span>](../api/intune-deviceconfig-windows10endpointprotectionconfiguration-create.md)|[<span data-ttu-id="b588a-120">windows10EndpointProtectionConfiguration</span><span class="sxs-lookup"><span data-stu-id="b588a-120">windows10EndpointProtectionConfiguration</span></span>](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md)|<span data-ttu-id="b588a-121">创建新的 [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="b588a-121">Create a new [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) object.</span></span>|
|[<span data-ttu-id="b588a-122">Delete windows10EndpointProtectionConfiguration</span><span class="sxs-lookup"><span data-stu-id="b588a-122">Delete windows10EndpointProtectionConfiguration</span></span>](../api/intune-deviceconfig-windows10endpointprotectionconfiguration-delete.md)|<span data-ttu-id="b588a-123">无</span><span class="sxs-lookup"><span data-stu-id="b588a-123">None</span></span>|<span data-ttu-id="b588a-124">删除 [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md)。</span><span class="sxs-lookup"><span data-stu-id="b588a-124">Deletes a [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md).</span></span>|
|[<span data-ttu-id="b588a-125">Update windows10EndpointProtectionConfiguration</span><span class="sxs-lookup"><span data-stu-id="b588a-125">Update windows10EndpointProtectionConfiguration</span></span>](../api/intune-deviceconfig-windows10endpointprotectionconfiguration-update.md)|[<span data-ttu-id="b588a-126">windows10EndpointProtectionConfiguration</span><span class="sxs-lookup"><span data-stu-id="b588a-126">windows10EndpointProtectionConfiguration</span></span>](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md)|<span data-ttu-id="b588a-127">更新 [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="b588a-127">Update the properties of a [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="b588a-128">属性</span><span class="sxs-lookup"><span data-stu-id="b588a-128">Properties</span></span>
|<span data-ttu-id="b588a-129">属性</span><span class="sxs-lookup"><span data-stu-id="b588a-129">Property</span></span>|<span data-ttu-id="b588a-130">类型</span><span class="sxs-lookup"><span data-stu-id="b588a-130">Type</span></span>|<span data-ttu-id="b588a-131">说明</span><span class="sxs-lookup"><span data-stu-id="b588a-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b588a-132">id</span><span class="sxs-lookup"><span data-stu-id="b588a-132">id</span></span>|<span data-ttu-id="b588a-133">String</span><span class="sxs-lookup"><span data-stu-id="b588a-133">String</span></span>|<span data-ttu-id="b588a-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="b588a-134">Key of the entity.</span></span> <span data-ttu-id="b588a-135">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b588a-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b588a-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b588a-136">lastModifiedDateTime</span></span>|<span data-ttu-id="b588a-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b588a-137">DateTimeOffset</span></span>|<span data-ttu-id="b588a-138">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="b588a-138">DateTime the object was last modified.</span></span> <span data-ttu-id="b588a-139">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b588a-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b588a-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="b588a-140">roleScopeTagIds</span></span>|<span data-ttu-id="b588a-141">String 集合</span><span class="sxs-lookup"><span data-stu-id="b588a-141">String collection</span></span>|<span data-ttu-id="b588a-142">此实体实例范围标记的列表。</span><span class="sxs-lookup"><span data-stu-id="b588a-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="b588a-143">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b588a-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b588a-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="b588a-144">supportsScopeTags</span></span>|<span data-ttu-id="b588a-145">布尔</span><span class="sxs-lookup"><span data-stu-id="b588a-145">Boolean</span></span>|<span data-ttu-id="b588a-146">指示基础的设备配置支持分配的范围标记。</span><span class="sxs-lookup"><span data-stu-id="b588a-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="b588a-147">此值为 false，并且实体将不会对作用域的用户可见时，不允许将分配给 ScopeTags 属性。</span><span class="sxs-lookup"><span data-stu-id="b588a-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="b588a-148">这将发生在 Silverlight 中创建的旧策略，并可以解析通过删除并重新创建 Azure 门户中的策略。</span><span class="sxs-lookup"><span data-stu-id="b588a-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="b588a-149">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="b588a-149">This property is read-only.</span></span> <span data-ttu-id="b588a-150">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b588a-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b588a-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b588a-151">createdDateTime</span></span>|<span data-ttu-id="b588a-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b588a-152">DateTimeOffset</span></span>|<span data-ttu-id="b588a-153">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="b588a-153">DateTime the object was created.</span></span> <span data-ttu-id="b588a-154">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b588a-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b588a-155">description</span><span class="sxs-lookup"><span data-stu-id="b588a-155">description</span></span>|<span data-ttu-id="b588a-156">String</span><span class="sxs-lookup"><span data-stu-id="b588a-156">String</span></span>|<span data-ttu-id="b588a-157">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="b588a-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="b588a-158">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b588a-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b588a-159">displayName</span><span class="sxs-lookup"><span data-stu-id="b588a-159">displayName</span></span>|<span data-ttu-id="b588a-160">String</span><span class="sxs-lookup"><span data-stu-id="b588a-160">String</span></span>|<span data-ttu-id="b588a-161">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="b588a-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="b588a-162">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b588a-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b588a-163">version</span><span class="sxs-lookup"><span data-stu-id="b588a-163">version</span></span>|<span data-ttu-id="b588a-164">Int32</span><span class="sxs-lookup"><span data-stu-id="b588a-164">Int32</span></span>|<span data-ttu-id="b588a-165">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="b588a-165">Version of the device configuration.</span></span> <span data-ttu-id="b588a-166">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b588a-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b588a-167">userRightsAccessCredentialManagerAsTrustedCaller</span><span class="sxs-lookup"><span data-stu-id="b588a-167">userRightsAccessCredentialManagerAsTrustedCaller</span></span>|[<span data-ttu-id="b588a-168">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="b588a-168">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="b588a-169">此用户权限备份/还原过程中使用的凭据管理器中。</span><span class="sxs-lookup"><span data-stu-id="b588a-169">This user right is used by Credential Manager during Backup/Restore.</span></span> <span data-ttu-id="b588a-170">用户的已保存的凭据可能受到威胁，如果此权限授予的其他实体。</span><span class="sxs-lookup"><span data-stu-id="b588a-170">Users' saved credentials might be compromised if this privilege is given to other entities.</span></span> <span data-ttu-id="b588a-171">支持状态 NotConfigured 和允许</span><span class="sxs-lookup"><span data-stu-id="b588a-171">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="b588a-172">userRightsAllowAccessFromNetwork</span><span class="sxs-lookup"><span data-stu-id="b588a-172">userRightsAllowAccessFromNetwork</span></span>|[<span data-ttu-id="b588a-173">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="b588a-173">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="b588a-174">此用户权限确定哪些用户和组允许通过网络连接到计算机。</span><span class="sxs-lookup"><span data-stu-id="b588a-174">This user right determines which users and groups are allowed to connect to the computer over the network.</span></span> <span data-ttu-id="b588a-175">支持状态允许。</span><span class="sxs-lookup"><span data-stu-id="b588a-175">State Allowed is supported.</span></span>|
|<span data-ttu-id="b588a-176">userRightsBlockAccessFromNetwork</span><span class="sxs-lookup"><span data-stu-id="b588a-176">userRightsBlockAccessFromNetwork</span></span>|[<span data-ttu-id="b588a-177">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="b588a-177">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="b588a-178">此用户权限确定哪些用户和组是通过网络连接到计算机的块。</span><span class="sxs-lookup"><span data-stu-id="b588a-178">This user right determines which users and groups are block from connecting to the computer over the network.</span></span> <span data-ttu-id="b588a-179">支持状态块。</span><span class="sxs-lookup"><span data-stu-id="b588a-179">State Block is supported.</span></span>|
|<span data-ttu-id="b588a-180">userRightsActAsPartOfTheOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="b588a-180">userRightsActAsPartOfTheOperatingSystem</span></span>|[<span data-ttu-id="b588a-181">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="b588a-181">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="b588a-182">此用户权限允许模拟任何用户无需身份验证的过程。</span><span class="sxs-lookup"><span data-stu-id="b588a-182">This user right allows a process to impersonate any user without authentication.</span></span> <span data-ttu-id="b588a-183">过程因此可以访问与该用户相同的本地资源。</span><span class="sxs-lookup"><span data-stu-id="b588a-183">The process can therefore gain access to the same local resources as that user.</span></span> <span data-ttu-id="b588a-184">支持状态 NotConfigured 和允许</span><span class="sxs-lookup"><span data-stu-id="b588a-184">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="b588a-185">userRightsLocalLogOn</span><span class="sxs-lookup"><span data-stu-id="b588a-185">userRightsLocalLogOn</span></span>|[<span data-ttu-id="b588a-186">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="b588a-186">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="b588a-187">此用户权限确定哪些用户可以登录到计算机。</span><span class="sxs-lookup"><span data-stu-id="b588a-187">This user right determines which users can log on to the computer.</span></span> <span data-ttu-id="b588a-188">状态 NotConfigured、 允许和已阻止所有支持</span><span class="sxs-lookup"><span data-stu-id="b588a-188">States NotConfigured, Allowed and Blocked are all supported</span></span> |
|<span data-ttu-id="b588a-189">userRightsBackupData</span><span class="sxs-lookup"><span data-stu-id="b588a-189">userRightsBackupData</span></span>|[<span data-ttu-id="b588a-190">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="b588a-190">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="b588a-191">此用户权限确定哪些用户可以跳过文件、 目录、 注册表和其他永久对象权限时备份文件和目录。</span><span class="sxs-lookup"><span data-stu-id="b588a-191">This user right determines which users can bypass file, directory, registry, and other persistent objects permissions when backing up files and directories.</span></span> <span data-ttu-id="b588a-192">支持状态 NotConfigured 和允许</span><span class="sxs-lookup"><span data-stu-id="b588a-192">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="b588a-193">userRightsChangeSystemTime</span><span class="sxs-lookup"><span data-stu-id="b588a-193">userRightsChangeSystemTime</span></span>|[<span data-ttu-id="b588a-194">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="b588a-194">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="b588a-195">此用户权限确定哪些用户和组可以更改计算机内部时钟的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="b588a-195">This user right determines which users and groups can change the time and date on the internal clock of the computer.</span></span> <span data-ttu-id="b588a-196">支持状态 NotConfigured 和允许</span><span class="sxs-lookup"><span data-stu-id="b588a-196">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="b588a-197">userRightsCreateGlobalObjects</span><span class="sxs-lookup"><span data-stu-id="b588a-197">userRightsCreateGlobalObjects</span></span>|[<span data-ttu-id="b588a-198">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="b588a-198">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="b588a-199">此安全设置确定用户是否可以创建可供所有会话的全局对象。</span><span class="sxs-lookup"><span data-stu-id="b588a-199">This security setting determines whether users can create global objects that are available to all sessions.</span></span> <span data-ttu-id="b588a-200">可以创建全局对象的用户可能会影响其他用户的会话，这可能导致应用程序故障或数据损坏下运行的进程。</span><span class="sxs-lookup"><span data-stu-id="b588a-200">Users who can create global objects could affect processes that run under other users' sessions, which could lead to application failure or data corruption.</span></span> <span data-ttu-id="b588a-201">支持状态 NotConfigured 和允许</span><span class="sxs-lookup"><span data-stu-id="b588a-201">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="b588a-202">userRightsCreatePageFile</span><span class="sxs-lookup"><span data-stu-id="b588a-202">userRightsCreatePageFile</span></span>|[<span data-ttu-id="b588a-203">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="b588a-203">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="b588a-204">此用户权限确定哪些用户和组可以呼叫内部 API 创建和更改页面文件的大小。</span><span class="sxs-lookup"><span data-stu-id="b588a-204">This user right determines which users and groups can call an internal API to create and change the size of a page file.</span></span> <span data-ttu-id="b588a-205">支持状态 NotConfigured 和允许</span><span class="sxs-lookup"><span data-stu-id="b588a-205">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="b588a-206">userRightsCreatePermanentSharedObjects</span><span class="sxs-lookup"><span data-stu-id="b588a-206">userRightsCreatePermanentSharedObjects</span></span>|[<span data-ttu-id="b588a-207">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="b588a-207">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="b588a-208">此用户权限确定哪些帐户可用于通过流程管理器中创建使用对象的目录对象。</span><span class="sxs-lookup"><span data-stu-id="b588a-208">This user right determines which accounts can be used by processes to create a directory object using the object manager.</span></span> <span data-ttu-id="b588a-209">支持状态 NotConfigured 和允许</span><span class="sxs-lookup"><span data-stu-id="b588a-209">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="b588a-210">userRightsCreateSymbolicLinks</span><span class="sxs-lookup"><span data-stu-id="b588a-210">userRightsCreateSymbolicLinks</span></span>|[<span data-ttu-id="b588a-211">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="b588a-211">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="b588a-212">此用户权限确定是否用户可以从与他们登录到计算机创建符号链接。</span><span class="sxs-lookup"><span data-stu-id="b588a-212">This user right determines if the user can create a symbolic link from the computer to which they are logged on.</span></span> <span data-ttu-id="b588a-213">支持状态 NotConfigured 和允许</span><span class="sxs-lookup"><span data-stu-id="b588a-213">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="b588a-214">userRightsCreateToken</span><span class="sxs-lookup"><span data-stu-id="b588a-214">userRightsCreateToken</span></span>|[<span data-ttu-id="b588a-215">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="b588a-215">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="b588a-216">此用户权限确定哪些用户/组可以由进程来创建用于时过程使用内部 API 来创建访问令牌获取对任何本地资源的访问令牌。</span><span class="sxs-lookup"><span data-stu-id="b588a-216">This user right determines which users/groups can be used by processes to create a token that can then be used to get access to any local resources when the process uses an internal API to create an access token.</span></span> <span data-ttu-id="b588a-217">支持状态 NotConfigured 和允许</span><span class="sxs-lookup"><span data-stu-id="b588a-217">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="b588a-218">userRightsDebugPrograms</span><span class="sxs-lookup"><span data-stu-id="b588a-218">userRightsDebugPrograms</span></span>|[<span data-ttu-id="b588a-219">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="b588a-219">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="b588a-220">此用户权限确定哪些用户可以将调试器附加到任何进程或内核。</span><span class="sxs-lookup"><span data-stu-id="b588a-220">This user right determines which users can attach a debugger to any process or to the kernel.</span></span> <span data-ttu-id="b588a-221">支持状态 NotConfigured 和允许</span><span class="sxs-lookup"><span data-stu-id="b588a-221">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="b588a-222">userRightsRemoteDesktopServicesLogOn</span><span class="sxs-lookup"><span data-stu-id="b588a-222">userRightsRemoteDesktopServicesLogOn</span></span>|[<span data-ttu-id="b588a-223">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="b588a-223">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="b588a-224">此用户权限确定禁止哪些用户和组作为远程桌面服务客户端登录。</span><span class="sxs-lookup"><span data-stu-id="b588a-224">This user right determines which users and groups are prohibited from logging on as a Remote Desktop Services client.</span></span> <span data-ttu-id="b588a-225">支持状态 NotConfigured 和被阻止</span><span class="sxs-lookup"><span data-stu-id="b588a-225">Only states NotConfigured and Blocked are supported</span></span>|
|<span data-ttu-id="b588a-226">userRightsDelegation</span><span class="sxs-lookup"><span data-stu-id="b588a-226">userRightsDelegation</span></span>|[<span data-ttu-id="b588a-227">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="b588a-227">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="b588a-228">此用户权限确定哪些用户可以在用户或计算机对象上设置委派设置受信任。</span><span class="sxs-lookup"><span data-stu-id="b588a-228">This user right determines which users can set the Trusted for Delegation setting on a user or computer object.</span></span> <span data-ttu-id="b588a-229">支持状态 NotConfigured 和允许。</span><span class="sxs-lookup"><span data-stu-id="b588a-229">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="b588a-230">userRightsGenerateSecurityAudits</span><span class="sxs-lookup"><span data-stu-id="b588a-230">userRightsGenerateSecurityAudits</span></span>|[<span data-ttu-id="b588a-231">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="b588a-231">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="b588a-232">此用户权限确定哪些帐户可用于由进程将条目添加到安全日志。</span><span class="sxs-lookup"><span data-stu-id="b588a-232">This user right determines which accounts can be used by a process to add entries to the security log.</span></span> <span data-ttu-id="b588a-233">安全日志用于跟踪未经授权的系统的访问。</span><span class="sxs-lookup"><span data-stu-id="b588a-233">The security log is used to trace unauthorized system access.</span></span>  <span data-ttu-id="b588a-234">支持状态 NotConfigured 和允许。</span><span class="sxs-lookup"><span data-stu-id="b588a-234">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="b588a-235">userRightsImpersonateClient</span><span class="sxs-lookup"><span data-stu-id="b588a-235">userRightsImpersonateClient</span></span>|[<span data-ttu-id="b588a-236">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="b588a-236">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="b588a-237">分配给用户此用户权限允许代表该用户模拟客户端运行的程序。</span><span class="sxs-lookup"><span data-stu-id="b588a-237">Assigning this user right to a user allows programs running on behalf of that user to impersonate a client.</span></span> <span data-ttu-id="b588a-238">对于此种模拟需要此用户权限可防止未经授权的用户从诱使客户端连接到他们创建的服务，然后这样可以将提升未经授权的用户的权限模拟该客户端，管理或系统级别。</span><span class="sxs-lookup"><span data-stu-id="b588a-238">Requiring this user right for this kind of impersonation prevents an unauthorized user from convincing a client to connect to a service that they have created and then impersonating that client, which can elevate the unauthorized user's permissions to administrative or system levels.</span></span> <span data-ttu-id="b588a-239">支持状态 NotConfigured 和允许。</span><span class="sxs-lookup"><span data-stu-id="b588a-239">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="b588a-240">userRightsIncreaseSchedulingPriority</span><span class="sxs-lookup"><span data-stu-id="b588a-240">userRightsIncreaseSchedulingPriority</span></span>|[<span data-ttu-id="b588a-241">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="b588a-241">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="b588a-242">此用户权限确定哪些帐户可用于过程写入属性访问另一个进程增加分配给其他进程的执行优先级。</span><span class="sxs-lookup"><span data-stu-id="b588a-242">This user right determines which accounts can use a process with Write Property access to another process to increase the execution priority assigned to the other process.</span></span> <span data-ttu-id="b588a-243">支持状态 NotConfigured 和允许。</span><span class="sxs-lookup"><span data-stu-id="b588a-243">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="b588a-244">userRightsLoadUnloadDrivers</span><span class="sxs-lookup"><span data-stu-id="b588a-244">userRightsLoadUnloadDrivers</span></span>|[<span data-ttu-id="b588a-245">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="b588a-245">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="b588a-246">此用户权限确定哪些用户可以动态加载和卸载设备驱动程序或内核模式中的其他代码。</span><span class="sxs-lookup"><span data-stu-id="b588a-246">This user right determines which users can dynamically load and unload device drivers or other code in to kernel mode.</span></span> <span data-ttu-id="b588a-247">支持状态 NotConfigured 和允许。</span><span class="sxs-lookup"><span data-stu-id="b588a-247">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="b588a-248">userRightsLockMemory</span><span class="sxs-lookup"><span data-stu-id="b588a-248">userRightsLockMemory</span></span>|[<span data-ttu-id="b588a-249">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="b588a-249">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="b588a-250">此用户权限确定哪些帐户可使用过程可在物理内存，防止系统分页数据写到磁盘上的虚拟内存中保留数据。</span><span class="sxs-lookup"><span data-stu-id="b588a-250">This user right determines which accounts can use a process to keep data in physical memory, which prevents the system from paging the data to virtual memory on disk.</span></span> <span data-ttu-id="b588a-251">支持状态 NotConfigured 和允许。</span><span class="sxs-lookup"><span data-stu-id="b588a-251">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="b588a-252">userRightsManageAuditingAndSecurityLogs</span><span class="sxs-lookup"><span data-stu-id="b588a-252">userRightsManageAuditingAndSecurityLogs</span></span>|[<span data-ttu-id="b588a-253">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="b588a-253">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="b588a-254">此用户权限确定哪些用户可以指定对象访问审核各个资源，如文件、 Active Directory 对象和注册表项选项。</span><span class="sxs-lookup"><span data-stu-id="b588a-254">This user right determines which users can specify object access auditing options for individual resources, such as files, Active Directory objects, and registry keys.</span></span> <span data-ttu-id="b588a-255">支持状态 NotConfigured 和允许。</span><span class="sxs-lookup"><span data-stu-id="b588a-255">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="b588a-256">userRightsManageVolumes</span><span class="sxs-lookup"><span data-stu-id="b588a-256">userRightsManageVolumes</span></span>|[<span data-ttu-id="b588a-257">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="b588a-257">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="b588a-258">此用户权限确定哪些用户和组可以在卷上，如远程磁盘碎片整理运行维护任务。</span><span class="sxs-lookup"><span data-stu-id="b588a-258">This user right determines which users and groups can run maintenance tasks on a volume, such as remote defragmentation.</span></span> <span data-ttu-id="b588a-259">支持状态 NotConfigured 和允许。</span><span class="sxs-lookup"><span data-stu-id="b588a-259">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="b588a-260">userRightsModifyFirmwareEnvironment</span><span class="sxs-lookup"><span data-stu-id="b588a-260">userRightsModifyFirmwareEnvironment</span></span>|[<span data-ttu-id="b588a-261">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="b588a-261">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="b588a-262">此用户权限确定谁可以修改固件环境值。</span><span class="sxs-lookup"><span data-stu-id="b588a-262">This user right determines who can modify firmware environment values.</span></span> <span data-ttu-id="b588a-263">支持状态 NotConfigured 和允许。</span><span class="sxs-lookup"><span data-stu-id="b588a-263">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="b588a-264">userRightsModifyObjectLabels</span><span class="sxs-lookup"><span data-stu-id="b588a-264">userRightsModifyObjectLabels</span></span>|[<span data-ttu-id="b588a-265">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="b588a-265">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="b588a-266">此用户权限确定哪些用户帐户可以修改对象，如文件、 注册表项或由其他用户拥有的进程的完整性标签。</span><span class="sxs-lookup"><span data-stu-id="b588a-266">This user right determines which user accounts can modify the integrity label of objects, such as files, registry keys, or processes owned by other users.</span></span> <span data-ttu-id="b588a-267">支持状态 NotConfigured 和允许。</span><span class="sxs-lookup"><span data-stu-id="b588a-267">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="b588a-268">userRightsProfileSingleProcess</span><span class="sxs-lookup"><span data-stu-id="b588a-268">userRightsProfileSingleProcess</span></span>|[<span data-ttu-id="b588a-269">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="b588a-269">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="b588a-270">此用户权限确定哪些用户可以使用性能监视工具来监视系统进程的性能。</span><span class="sxs-lookup"><span data-stu-id="b588a-270">This user right determines which users can use performance monitoring tools to monitor the performance of system processes.</span></span> <span data-ttu-id="b588a-271">支持状态 NotConfigured 和允许。</span><span class="sxs-lookup"><span data-stu-id="b588a-271">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="b588a-272">userRightsRemoteShutdown</span><span class="sxs-lookup"><span data-stu-id="b588a-272">userRightsRemoteShutdown</span></span>|[<span data-ttu-id="b588a-273">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="b588a-273">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="b588a-274">此用户权限确定允许哪些用户关闭，将计算机从网络上的远程位置。</span><span class="sxs-lookup"><span data-stu-id="b588a-274">This user right determines which users are allowed to shut down a computer from a remote location on the network.</span></span> <span data-ttu-id="b588a-275">此用户权限的误用会导致拒绝服务。</span><span class="sxs-lookup"><span data-stu-id="b588a-275">Misuse of this user right can result in a denial of service.</span></span> <span data-ttu-id="b588a-276">支持状态 NotConfigured 和允许。</span><span class="sxs-lookup"><span data-stu-id="b588a-276">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="b588a-277">userRightsRestoreData</span><span class="sxs-lookup"><span data-stu-id="b588a-277">userRightsRestoreData</span></span>|[<span data-ttu-id="b588a-278">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="b588a-278">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="b588a-279">此用户权限决定哪些用户可以跳过文件、 目录、 注册表和权限还原时备份文件和目录，其他持久对象，决定哪些用户可以设置为对象的所有者的任何有效的安全主体。</span><span class="sxs-lookup"><span data-stu-id="b588a-279">This user right determines which users can bypass file, directory, registry, and other persistent objects permissions when restoring backed up files and directories, and determines which users can set any valid security principal as the owner of an object.</span></span> <span data-ttu-id="b588a-280">支持状态 NotConfigured 和允许。</span><span class="sxs-lookup"><span data-stu-id="b588a-280">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="b588a-281">userRightsTakeOwnership</span><span class="sxs-lookup"><span data-stu-id="b588a-281">userRightsTakeOwnership</span></span>|[<span data-ttu-id="b588a-282">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="b588a-282">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="b588a-283">此用户权限决定哪些用户可以在系统中，包括 Active Directory 对象、 文件和文件夹、 打印机、 注册表项、 流程和线程执行任何安全对象的所有权。</span><span class="sxs-lookup"><span data-stu-id="b588a-283">This user right determines which users can take ownership of any securable object in the system, including Active Directory objects, files and folders, printers, registry keys, processes, and threads.</span></span> <span data-ttu-id="b588a-284">支持状态 NotConfigured 和允许。</span><span class="sxs-lookup"><span data-stu-id="b588a-284">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="b588a-285">userRightsRegisterProcessAsService</span><span class="sxs-lookup"><span data-stu-id="b588a-285">userRightsRegisterProcessAsService</span></span>|[<span data-ttu-id="b588a-286">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="b588a-286">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="b588a-287">此安全设置确定被阻止的服务帐户注册为服务的进程。</span><span class="sxs-lookup"><span data-stu-id="b588a-287">This security setting determines which service accounts are prevented from registering a process as a service.</span></span> <span data-ttu-id="b588a-288">注意： 此安全设置不适用于系统、 本地服务或网络服务帐户。</span><span class="sxs-lookup"><span data-stu-id="b588a-288">Note: This security setting does not apply to the System, Local Service, or Network Service accounts.</span></span> <span data-ttu-id="b588a-289">仅支持已阻止的状态。</span><span class="sxs-lookup"><span data-stu-id="b588a-289">Only state Blocked is supported.</span></span>|
|<span data-ttu-id="b588a-290">xboxServicesEnableXboxGameSaveTask</span><span class="sxs-lookup"><span data-stu-id="b588a-290">xboxServicesEnableXboxGameSaveTask</span></span>|<span data-ttu-id="b588a-291">布尔</span><span class="sxs-lookup"><span data-stu-id="b588a-291">Boolean</span></span>|<span data-ttu-id="b588a-292">此设置确定 xbox 游戏保存是否启用 (1) 或禁用 (0)。</span><span class="sxs-lookup"><span data-stu-id="b588a-292">This setting determines whether xbox game save is enabled (1) or disabled (0).</span></span>|
|<span data-ttu-id="b588a-293">xboxServicesAccessoryManagementServiceStartupMode</span><span class="sxs-lookup"><span data-stu-id="b588a-293">xboxServicesAccessoryManagementServiceStartupMode</span></span>|[<span data-ttu-id="b588a-294">serviceStartType</span><span class="sxs-lookup"><span data-stu-id="b588a-294">serviceStartType</span></span>](../resources/intune-deviceconfig-servicestarttype.md)|<span data-ttu-id="b588a-295">此设置确定的附件管理服务启动类型是 Automatic(2) Manual(3)、 Disabled(4)。</span><span class="sxs-lookup"><span data-stu-id="b588a-295">This setting determines whether the Accessory management service's start type is Automatic(2), Manual(3), Disabled(4).</span></span> <span data-ttu-id="b588a-296">默认： 手动。</span><span class="sxs-lookup"><span data-stu-id="b588a-296">Default: Manual.</span></span> <span data-ttu-id="b588a-297">可取值为：`manual`、`automatic`、`disabled`。</span><span class="sxs-lookup"><span data-stu-id="b588a-297">Possible values are: `manual`, `automatic`, `disabled`.</span></span>|
|<span data-ttu-id="b588a-298">xboxServicesLiveAuthManagerServiceStartupMode</span><span class="sxs-lookup"><span data-stu-id="b588a-298">xboxServicesLiveAuthManagerServiceStartupMode</span></span>|[<span data-ttu-id="b588a-299">serviceStartType</span><span class="sxs-lookup"><span data-stu-id="b588a-299">serviceStartType</span></span>](../resources/intune-deviceconfig-servicestarttype.md)|<span data-ttu-id="b588a-300">此设置确定 Live 身份验证管理器服务启动类型是 Automatic(2) Manual(3)、 Disabled(4)。</span><span class="sxs-lookup"><span data-stu-id="b588a-300">This setting determines whether Live Auth Manager service's start type is Automatic(2), Manual(3), Disabled(4).</span></span> <span data-ttu-id="b588a-301">默认： 手动。</span><span class="sxs-lookup"><span data-stu-id="b588a-301">Default: Manual.</span></span> <span data-ttu-id="b588a-302">可取值为：`manual`、`automatic`、`disabled`。</span><span class="sxs-lookup"><span data-stu-id="b588a-302">Possible values are: `manual`, `automatic`, `disabled`.</span></span>|
|<span data-ttu-id="b588a-303">xboxServicesLiveGameSaveServiceStartupMode</span><span class="sxs-lookup"><span data-stu-id="b588a-303">xboxServicesLiveGameSaveServiceStartupMode</span></span>|[<span data-ttu-id="b588a-304">serviceStartType</span><span class="sxs-lookup"><span data-stu-id="b588a-304">serviceStartType</span></span>](../resources/intune-deviceconfig-servicestarttype.md)|<span data-ttu-id="b588a-305">此设置确定是否 Automatic(2) Manual(3)、 Disabled(4) Live 保存服务的启动类型的游戏。</span><span class="sxs-lookup"><span data-stu-id="b588a-305">This setting determines whether Live Game save service's start type is Automatic(2), Manual(3), Disabled(4).</span></span> <span data-ttu-id="b588a-306">默认： 手动。</span><span class="sxs-lookup"><span data-stu-id="b588a-306">Default: Manual.</span></span> <span data-ttu-id="b588a-307">可取值为：`manual`、`automatic`、`disabled`。</span><span class="sxs-lookup"><span data-stu-id="b588a-307">Possible values are: `manual`, `automatic`, `disabled`.</span></span>|
|<span data-ttu-id="b588a-308">xboxServicesLiveNetworkingServiceStartupMode</span><span class="sxs-lookup"><span data-stu-id="b588a-308">xboxServicesLiveNetworkingServiceStartupMode</span></span>|[<span data-ttu-id="b588a-309">serviceStartType</span><span class="sxs-lookup"><span data-stu-id="b588a-309">serviceStartType</span></span>](../resources/intune-deviceconfig-servicestarttype.md)|<span data-ttu-id="b588a-310">此设置确定网络服务启动类型是 Automatic(2) Manual(3)、 Disabled(4)。</span><span class="sxs-lookup"><span data-stu-id="b588a-310">This setting determines whether Networking service's start type is Automatic(2), Manual(3), Disabled(4).</span></span> <span data-ttu-id="b588a-311">默认： 手动。</span><span class="sxs-lookup"><span data-stu-id="b588a-311">Default: Manual.</span></span> <span data-ttu-id="b588a-312">可取值为：`manual`、`automatic`、`disabled`。</span><span class="sxs-lookup"><span data-stu-id="b588a-312">Possible values are: `manual`, `automatic`, `disabled`.</span></span>|
|<span data-ttu-id="b588a-313">localSecurityOptionsBlockMicrosoftAccounts</span><span class="sxs-lookup"><span data-stu-id="b588a-313">localSecurityOptionsBlockMicrosoftAccounts</span></span>|<span data-ttu-id="b588a-314">布尔</span><span class="sxs-lookup"><span data-stu-id="b588a-314">Boolean</span></span>|<span data-ttu-id="b588a-315">禁止用户添加到此计算机的新的 Microsoft 帐户。</span><span class="sxs-lookup"><span data-stu-id="b588a-315">Prevent users from adding new Microsoft accounts to this computer.</span></span>|
|<span data-ttu-id="b588a-316">localSecurityOptionsBlockRemoteLogonWithBlankPassword</span><span class="sxs-lookup"><span data-stu-id="b588a-316">localSecurityOptionsBlockRemoteLogonWithBlankPassword</span></span>|<span data-ttu-id="b588a-317">布尔</span><span class="sxs-lookup"><span data-stu-id="b588a-317">Boolean</span></span>|<span data-ttu-id="b588a-318">启用本地帐户不受密码保护登录从物理设备以外的位置。将启用默认值</span><span class="sxs-lookup"><span data-stu-id="b588a-318">Enable Local accounts that are not password protected to log on from locations other than the physical device.Default is enabled</span></span>|
|<span data-ttu-id="b588a-319">localSecurityOptionsEnableAdministratorAccount</span><span class="sxs-lookup"><span data-stu-id="b588a-319">localSecurityOptionsEnableAdministratorAccount</span></span>|<span data-ttu-id="b588a-320">布尔</span><span class="sxs-lookup"><span data-stu-id="b588a-320">Boolean</span></span>|<span data-ttu-id="b588a-321">确定是否启用或禁用的本地管理员帐户。</span><span class="sxs-lookup"><span data-stu-id="b588a-321">Determines whether the Local Administrator account is enabled or disabled.</span></span>|
|<span data-ttu-id="b588a-322">localSecurityOptionsAdministratorAccountName</span><span class="sxs-lookup"><span data-stu-id="b588a-322">localSecurityOptionsAdministratorAccountName</span></span>|<span data-ttu-id="b588a-323">字符串</span><span class="sxs-lookup"><span data-stu-id="b588a-323">String</span></span>|<span data-ttu-id="b588a-324">定义要与"管理员"的帐户的安全标识符 (SID) 关联的不同的帐户名称。</span><span class="sxs-lookup"><span data-stu-id="b588a-324">Define a different account name to be associated with the security identifier (SID) for the account “Administrator”.</span></span>|
|<span data-ttu-id="b588a-325">localSecurityOptionsEnableGuestAccount</span><span class="sxs-lookup"><span data-stu-id="b588a-325">localSecurityOptionsEnableGuestAccount</span></span>|<span data-ttu-id="b588a-326">布尔</span><span class="sxs-lookup"><span data-stu-id="b588a-326">Boolean</span></span>|<span data-ttu-id="b588a-327">确定是启用还是禁用来宾帐户。</span><span class="sxs-lookup"><span data-stu-id="b588a-327">Determines if the Guest account is enabled or disabled.</span></span>|
|<span data-ttu-id="b588a-328">localSecurityOptionsGuestAccountName</span><span class="sxs-lookup"><span data-stu-id="b588a-328">localSecurityOptionsGuestAccountName</span></span>|<span data-ttu-id="b588a-329">字符串</span><span class="sxs-lookup"><span data-stu-id="b588a-329">String</span></span>|<span data-ttu-id="b588a-330">定义要为"来宾"的帐户的安全标识符 (SID) 关联的不同的帐户名称。</span><span class="sxs-lookup"><span data-stu-id="b588a-330">Define a different account name to be associated with the security identifier (SID) for the account “Guest”.</span></span>|
|<span data-ttu-id="b588a-331">localSecurityOptionsAllowUndockWithoutHavingToLogon</span><span class="sxs-lookup"><span data-stu-id="b588a-331">localSecurityOptionsAllowUndockWithoutHavingToLogon</span></span>|<span data-ttu-id="b588a-332">布尔</span><span class="sxs-lookup"><span data-stu-id="b588a-332">Boolean</span></span>|<span data-ttu-id="b588a-333">正在取消停靠而无需登录阻止便携式计算机。</span><span class="sxs-lookup"><span data-stu-id="b588a-333">Prevent a portable computer from being undocked without having to log in.</span></span>|
|<span data-ttu-id="b588a-334">localSecurityOptionsBlockUsersInstallingPrinterDrivers</span><span class="sxs-lookup"><span data-stu-id="b588a-334">localSecurityOptionsBlockUsersInstallingPrinterDrivers</span></span>|<span data-ttu-id="b588a-335">布尔</span><span class="sxs-lookup"><span data-stu-id="b588a-335">Boolean</span></span>|<span data-ttu-id="b588a-336">限制为连接到向管理员仅共享打印机的一部分安装的打印机驱动程序。</span><span class="sxs-lookup"><span data-stu-id="b588a-336">Restrict installing printer drivers as part of connecting to a shared printer to admins only.</span></span>|
|<span data-ttu-id="b588a-337">localSecurityOptionsBlockRemoteOpticalDriveAccess</span><span class="sxs-lookup"><span data-stu-id="b588a-337">localSecurityOptionsBlockRemoteOpticalDriveAccess</span></span>|<span data-ttu-id="b588a-338">布尔</span><span class="sxs-lookup"><span data-stu-id="b588a-338">Boolean</span></span>|<span data-ttu-id="b588a-339">启用此设置允许访问 CD-ROM 媒体仅以交互方式登录的用户。</span><span class="sxs-lookup"><span data-stu-id="b588a-339">Enabling this settings allows only interactively logged on user to access CD-ROM media.</span></span>|
|<span data-ttu-id="b588a-340">localSecurityOptionsFormatAndEjectOfRemovableMediaAllowedUser</span><span class="sxs-lookup"><span data-stu-id="b588a-340">localSecurityOptionsFormatAndEjectOfRemovableMediaAllowedUser</span></span>|[<span data-ttu-id="b588a-341">localSecurityOptionsFormatAndEjectOfRemovableMediaAllowedUserType</span><span class="sxs-lookup"><span data-stu-id="b588a-341">localSecurityOptionsFormatAndEjectOfRemovableMediaAllowedUserType</span></span>](../resources/intune-deviceconfig-localsecurityoptionsformatandejectofremovablemediaallowedusertype.md)|<span data-ttu-id="b588a-342">定义允许谁格式化和弹出可移动 NTFS 媒体。</span><span class="sxs-lookup"><span data-stu-id="b588a-342">Define who is allowed to format and eject removable NTFS media.</span></span> <span data-ttu-id="b588a-343">可取值为：`notConfigured`、`administrators`、`administratorsAndPowerUsers`、`administratorsAndInteractiveUsers`。</span><span class="sxs-lookup"><span data-stu-id="b588a-343">Possible values are: `notConfigured`, `administrators`, `administratorsAndPowerUsers`, `administratorsAndInteractiveUsers`.</span></span>|
|<span data-ttu-id="b588a-344">localSecurityOptionsMachineInactivityLimit</span><span class="sxs-lookup"><span data-stu-id="b588a-344">localSecurityOptionsMachineInactivityLimit</span></span>|<span data-ttu-id="b588a-345">Int32</span><span class="sxs-lookup"><span data-stu-id="b588a-345">Int32</span></span>|<span data-ttu-id="b588a-346">交互式桌面上登录屏幕上定义最大分钟无活动，直到屏幕保护程序运行。</span><span class="sxs-lookup"><span data-stu-id="b588a-346">Define maximum minutes of inactivity on the interactive desktop’s login screen until the screen saver runs.</span></span> <span data-ttu-id="b588a-347">有效的值 0 到 9999 之间</span><span class="sxs-lookup"><span data-stu-id="b588a-347">Valid values 0 to 9999</span></span>|
|<span data-ttu-id="b588a-348">localSecurityOptionsMachineInactivityLimitInMinutes</span><span class="sxs-lookup"><span data-stu-id="b588a-348">localSecurityOptionsMachineInactivityLimitInMinutes</span></span>|<span data-ttu-id="b588a-349">Int32</span><span class="sxs-lookup"><span data-stu-id="b588a-349">Int32</span></span>|<span data-ttu-id="b588a-350">交互式桌面上登录屏幕上定义最大分钟无活动，直到屏幕保护程序运行。</span><span class="sxs-lookup"><span data-stu-id="b588a-350">Define maximum minutes of inactivity on the interactive desktop’s login screen until the screen saver runs.</span></span> <span data-ttu-id="b588a-351">有效的值 0 到 9999 之间</span><span class="sxs-lookup"><span data-stu-id="b588a-351">Valid values 0 to 9999</span></span>|
|<span data-ttu-id="b588a-352">localSecurityOptionsDoNotRequireCtrlAltDel</span><span class="sxs-lookup"><span data-stu-id="b588a-352">localSecurityOptionsDoNotRequireCtrlAltDel</span></span>|<span data-ttu-id="b588a-353">布尔</span><span class="sxs-lookup"><span data-stu-id="b588a-353">Boolean</span></span>|<span data-ttu-id="b588a-354">需要 CTRL + ALT + DEL 要按用户登录之前。</span><span class="sxs-lookup"><span data-stu-id="b588a-354">Require CTRL+ALT+DEL to be pressed before a user can log on.</span></span>|
|<span data-ttu-id="b588a-355">localSecurityOptionsHideLastSignedInUser</span><span class="sxs-lookup"><span data-stu-id="b588a-355">localSecurityOptionsHideLastSignedInUser</span></span>|<span data-ttu-id="b588a-356">布尔</span><span class="sxs-lookup"><span data-stu-id="b588a-356">Boolean</span></span>|<span data-ttu-id="b588a-357">不在此设备上显示的签名的最后一个人的用户名。</span><span class="sxs-lookup"><span data-stu-id="b588a-357">Do not display the username of the last person who signed in on this device.</span></span>|
|<span data-ttu-id="b588a-358">localSecurityOptionsHideUsernameAtSignIn</span><span class="sxs-lookup"><span data-stu-id="b588a-358">localSecurityOptionsHideUsernameAtSignIn</span></span>|<span data-ttu-id="b588a-359">布尔</span><span class="sxs-lookup"><span data-stu-id="b588a-359">Boolean</span></span>|<span data-ttu-id="b588a-360">不显示登录到此设备输入凭据之后和之前显示设备的桌面的人员的用户名。</span><span class="sxs-lookup"><span data-stu-id="b588a-360">Do not display the username of the person signing in to this device after credentials are entered and before the device’s desktop is shown.</span></span>|
|<span data-ttu-id="b588a-361">localSecurityOptionsLogOnMessageTitle</span><span class="sxs-lookup"><span data-stu-id="b588a-361">localSecurityOptionsLogOnMessageTitle</span></span>|<span data-ttu-id="b588a-362">字符串</span><span class="sxs-lookup"><span data-stu-id="b588a-362">String</span></span>|<span data-ttu-id="b588a-363">用户尝试登录的设置邮件标题。</span><span class="sxs-lookup"><span data-stu-id="b588a-363">Set message title for users attempting to log in.</span></span>|
|<span data-ttu-id="b588a-364">localSecurityOptionsLogOnMessageText</span><span class="sxs-lookup"><span data-stu-id="b588a-364">localSecurityOptionsLogOnMessageText</span></span>|<span data-ttu-id="b588a-365">字符串</span><span class="sxs-lookup"><span data-stu-id="b588a-365">String</span></span>|<span data-ttu-id="b588a-366">设置用户试图登录消息文本。</span><span class="sxs-lookup"><span data-stu-id="b588a-366">Set message text for users attempting to log in.</span></span>|
|<span data-ttu-id="b588a-367">localSecurityOptionsAllowPKU2UAuthenticationRequests</span><span class="sxs-lookup"><span data-stu-id="b588a-367">localSecurityOptionsAllowPKU2UAuthenticationRequests</span></span>|<span data-ttu-id="b588a-368">布尔</span><span class="sxs-lookup"><span data-stu-id="b588a-368">Boolean</span></span>|<span data-ttu-id="b588a-369">对此设备块 PKU2U 身份验证请求使用联机标识。</span><span class="sxs-lookup"><span data-stu-id="b588a-369">Block PKU2U authentication requests to this device to use online identities.</span></span>|
|<span data-ttu-id="b588a-370">localSecurityOptionsAllowRemoteCallsToSecurityAccountsManagerHelperBool</span><span class="sxs-lookup"><span data-stu-id="b588a-370">localSecurityOptionsAllowRemoteCallsToSecurityAccountsManagerHelperBool</span></span>|<span data-ttu-id="b588a-371">布尔</span><span class="sxs-lookup"><span data-stu-id="b588a-371">Boolean</span></span>|<span data-ttu-id="b588a-372">用户界面帮助程序布尔 LocalSecurityOptionsAllowRemoteCallsToSecurityAccountsManager 实体</span><span class="sxs-lookup"><span data-stu-id="b588a-372">UI helper boolean for LocalSecurityOptionsAllowRemoteCallsToSecurityAccountsManager entity</span></span>|
|<span data-ttu-id="b588a-373">localSecurityOptionsAllowRemoteCallsToSecurityAccountsManager</span><span class="sxs-lookup"><span data-stu-id="b588a-373">localSecurityOptionsAllowRemoteCallsToSecurityAccountsManager</span></span>|<span data-ttu-id="b588a-374">字符串</span><span class="sxs-lookup"><span data-stu-id="b588a-374">String</span></span>|<span data-ttu-id="b588a-375">编辑默认安全描述符定义语言字符串，以允许或拒绝远程调用 SAM 用户和组。</span><span class="sxs-lookup"><span data-stu-id="b588a-375">Edit the default Security Descriptor Definition Language string to allow or deny users and groups to make remote calls to the SAM.</span></span>|
|<span data-ttu-id="b588a-376">localSecurityOptionsMinimumSessionSecurityForNtlmSspBasedClients</span><span class="sxs-lookup"><span data-stu-id="b588a-376">localSecurityOptionsMinimumSessionSecurityForNtlmSspBasedClients</span></span>|[<span data-ttu-id="b588a-377">localSecurityOptionsMinimumSessionSecurity</span><span class="sxs-lookup"><span data-stu-id="b588a-377">localSecurityOptionsMinimumSessionSecurity</span></span>](../resources/intune-deviceconfig-localsecurityoptionsminimumsessionsecurity.md)|<span data-ttu-id="b588a-378">此安全设置允许客户端要求 128 位加密和/或 NTLMv2 会话安全协商。</span><span class="sxs-lookup"><span data-stu-id="b588a-378">This security setting allows a client to require the negotiation of 128-bit encryption and/or NTLMv2 session security.</span></span> <span data-ttu-id="b588a-379">可取值为：`none`、`requireNtmlV2SessionSecurity`、`require128BitEncryption`、`ntlmV2And128BitEncryption`。</span><span class="sxs-lookup"><span data-stu-id="b588a-379">Possible values are: `none`, `requireNtmlV2SessionSecurity`, `require128BitEncryption`, `ntlmV2And128BitEncryption`.</span></span>|
|<span data-ttu-id="b588a-380">localSecurityOptionsMinimumSessionSecurityForNtlmSspBasedServers</span><span class="sxs-lookup"><span data-stu-id="b588a-380">localSecurityOptionsMinimumSessionSecurityForNtlmSspBasedServers</span></span>|[<span data-ttu-id="b588a-381">localSecurityOptionsMinimumSessionSecurity</span><span class="sxs-lookup"><span data-stu-id="b588a-381">localSecurityOptionsMinimumSessionSecurity</span></span>](../resources/intune-deviceconfig-localsecurityoptionsminimumsessionsecurity.md)|<span data-ttu-id="b588a-382">此安全设置允许服务器要求 128 位加密和/或 NTLMv2 会话安全协商。</span><span class="sxs-lookup"><span data-stu-id="b588a-382">This security setting allows a server to require the negotiation of 128-bit encryption and/or NTLMv2 session security.</span></span> <span data-ttu-id="b588a-383">可取值为：`none`、`requireNtmlV2SessionSecurity`、`require128BitEncryption`、`ntlmV2And128BitEncryption`。</span><span class="sxs-lookup"><span data-stu-id="b588a-383">Possible values are: `none`, `requireNtmlV2SessionSecurity`, `require128BitEncryption`, `ntlmV2And128BitEncryption`.</span></span>|
|<span data-ttu-id="b588a-384">lanManagerAuthenticationLevel</span><span class="sxs-lookup"><span data-stu-id="b588a-384">lanManagerAuthenticationLevel</span></span>|[<span data-ttu-id="b588a-385">lanManagerAuthenticationLevel</span><span class="sxs-lookup"><span data-stu-id="b588a-385">lanManagerAuthenticationLevel</span></span>](../resources/intune-deviceconfig-lanmanagerauthenticationlevel.md)|<span data-ttu-id="b588a-386">此安全设置确定哪个质询/响应身份验证协议用于网络登录。</span><span class="sxs-lookup"><span data-stu-id="b588a-386">This security setting determines which challenge/response authentication protocol is used for network logons.</span></span> <span data-ttu-id="b588a-387">可取值为：`lmAndNltm`、`lmNtlmAndNtlmV2`、`lmAndNtlmOnly`、`lmAndNtlmV2`、`lmNtlmV2AndNotLm`、`lmNtlmV2AndNotLmOrNtm`。</span><span class="sxs-lookup"><span data-stu-id="b588a-387">Possible values are: `lmAndNltm`, `lmNtlmAndNtlmV2`, `lmAndNtlmOnly`, `lmAndNtlmV2`, `lmNtlmV2AndNotLm`, `lmNtlmV2AndNotLmOrNtm`.</span></span>|
|<span data-ttu-id="b588a-388">lanManagerWorkstationEnableInsecureGuestLogons</span><span class="sxs-lookup"><span data-stu-id="b588a-388">lanManagerWorkstationEnableInsecureGuestLogons</span></span>|<span data-ttu-id="b588a-389">布尔</span><span class="sxs-lookup"><span data-stu-id="b588a-389">Boolean</span></span>|<span data-ttu-id="b588a-390">如果启用，则 SMB 客户端将允许不安全的来宾登录。</span><span class="sxs-lookup"><span data-stu-id="b588a-390">If enabled,the SMB client will allow insecure guest logons.</span></span> <span data-ttu-id="b588a-391">如果未配置，SMB 客户端将拒绝不安全的来宾登录。</span><span class="sxs-lookup"><span data-stu-id="b588a-391">If not configured, the SMB client will reject insecure guest logons.</span></span>|
|<span data-ttu-id="b588a-392">localSecurityOptionsClearVirtualMemoryPageFile</span><span class="sxs-lookup"><span data-stu-id="b588a-392">localSecurityOptionsClearVirtualMemoryPageFile</span></span>|<span data-ttu-id="b588a-393">布尔</span><span class="sxs-lookup"><span data-stu-id="b588a-393">Boolean</span></span>|<span data-ttu-id="b588a-394">此安全设置确定系统关闭时是否清除虚拟内存页面文件。</span><span class="sxs-lookup"><span data-stu-id="b588a-394">This security setting determines whether the virtual memory pagefile is cleared when the system is shut down.</span></span>|
|<span data-ttu-id="b588a-395">localSecurityOptionsAllowSystemToBeShutDownWithoutHavingToLogOn</span><span class="sxs-lookup"><span data-stu-id="b588a-395">localSecurityOptionsAllowSystemToBeShutDownWithoutHavingToLogOn</span></span>|<span data-ttu-id="b588a-396">布尔</span><span class="sxs-lookup"><span data-stu-id="b588a-396">Boolean</span></span>|<span data-ttu-id="b588a-397">此安全设置确定是否可以关闭计算机而无需登录到 Windows。</span><span class="sxs-lookup"><span data-stu-id="b588a-397">This security setting determines whether a computer can be shut down without having to log on to Windows.</span></span>|
|<span data-ttu-id="b588a-398">localSecurityOptionsAllowUIAccessApplicationElevation</span><span class="sxs-lookup"><span data-stu-id="b588a-398">localSecurityOptionsAllowUIAccessApplicationElevation</span></span>|<span data-ttu-id="b588a-399">布尔</span><span class="sxs-lookup"><span data-stu-id="b588a-399">Boolean</span></span>|<span data-ttu-id="b588a-400">允许 UIAccess 应用程序无需使用安全桌面提示提升。</span><span class="sxs-lookup"><span data-stu-id="b588a-400">Allow UIAccess apps to prompt for elevation without using the secure desktop.</span></span>|
|<span data-ttu-id="b588a-401">localSecurityOptionsVirtualizeFileAndRegistryWriteFailuresToPerUserLocations</span><span class="sxs-lookup"><span data-stu-id="b588a-401">localSecurityOptionsVirtualizeFileAndRegistryWriteFailuresToPerUserLocations</span></span>|<span data-ttu-id="b588a-402">布尔</span><span class="sxs-lookup"><span data-stu-id="b588a-402">Boolean</span></span>|<span data-ttu-id="b588a-403">虚拟化文件和注册表写入失败次数为每用户位置</span><span class="sxs-lookup"><span data-stu-id="b588a-403">Virtualize file and registry write failures to per user locations</span></span>|
|<span data-ttu-id="b588a-404">localSecurityOptionsOnlyElevateSignedExecutables</span><span class="sxs-lookup"><span data-stu-id="b588a-404">localSecurityOptionsOnlyElevateSignedExecutables</span></span>|<span data-ttu-id="b588a-405">布尔</span><span class="sxs-lookup"><span data-stu-id="b588a-405">Boolean</span></span>|<span data-ttu-id="b588a-406">允许运行之前，强制实施 PKI 证书路径验证给定的可执行文件。</span><span class="sxs-lookup"><span data-stu-id="b588a-406">Enforce PKI certification path validation for a given executable file before it is permitted to run.</span></span>|
|<span data-ttu-id="b588a-407">localSecurityOptionsAdministratorElevationPromptBehavior</span><span class="sxs-lookup"><span data-stu-id="b588a-407">localSecurityOptionsAdministratorElevationPromptBehavior</span></span>|[<span data-ttu-id="b588a-408">localSecurityOptionsAdministratorElevationPromptBehaviorType</span><span class="sxs-lookup"><span data-stu-id="b588a-408">localSecurityOptionsAdministratorElevationPromptBehaviorType</span></span>](../resources/intune-deviceconfig-localsecurityoptionsadministratorelevationpromptbehaviortype.md)|<span data-ttu-id="b588a-409">管理员批准模式中定义管理员的提升提示的行为。</span><span class="sxs-lookup"><span data-stu-id="b588a-409">Define the behavior of the elevation prompt for admins in Admin Approval Mode.</span></span> <span data-ttu-id="b588a-410">可取值为：`notConfigured`、`elevateWithoutPrompting`、`promptForCredentialsOnTheSecureDesktop`、`promptForConsentOnTheSecureDesktop`、`promptForCredentials`、`promptForConsent`、`promptForConsentForNonWindowsBinaries`。</span><span class="sxs-lookup"><span data-stu-id="b588a-410">Possible values are: `notConfigured`, `elevateWithoutPrompting`, `promptForCredentialsOnTheSecureDesktop`, `promptForConsentOnTheSecureDesktop`, `promptForCredentials`, `promptForConsent`, `promptForConsentForNonWindowsBinaries`.</span></span>|
|<span data-ttu-id="b588a-411">localSecurityOptionsStandardUserElevationPromptBehavior</span><span class="sxs-lookup"><span data-stu-id="b588a-411">localSecurityOptionsStandardUserElevationPromptBehavior</span></span>|[<span data-ttu-id="b588a-412">localSecurityOptionsStandardUserElevationPromptBehaviorType</span><span class="sxs-lookup"><span data-stu-id="b588a-412">localSecurityOptionsStandardUserElevationPromptBehaviorType</span></span>](../resources/intune-deviceconfig-localsecurityoptionsstandarduserelevationpromptbehaviortype.md)|<span data-ttu-id="b588a-413">定义标准用户的提升提示的行为。</span><span class="sxs-lookup"><span data-stu-id="b588a-413">Define the behavior of the elevation prompt for standard users.</span></span> <span data-ttu-id="b588a-414">可取值为：`notConfigured`、`automaticallyDenyElevationRequests`、`promptForCredentialsOnTheSecureDesktop`、`promptForCredentials`。</span><span class="sxs-lookup"><span data-stu-id="b588a-414">Possible values are: `notConfigured`, `automaticallyDenyElevationRequests`, `promptForCredentialsOnTheSecureDesktop`, `promptForCredentials`.</span></span>|
|<span data-ttu-id="b588a-415">localSecurityOptionsSwitchToSecureDesktopWhenPromptingForElevation</span><span class="sxs-lookup"><span data-stu-id="b588a-415">localSecurityOptionsSwitchToSecureDesktopWhenPromptingForElevation</span></span>|<span data-ttu-id="b588a-416">布尔</span><span class="sxs-lookup"><span data-stu-id="b588a-416">Boolean</span></span>|<span data-ttu-id="b588a-417">启用所有提升请求，以转到交互式用户的桌面，而不是安全的桌面。</span><span class="sxs-lookup"><span data-stu-id="b588a-417">Enable all elevation requests to go to the interactive user's desktop rather than the secure desktop.</span></span> <span data-ttu-id="b588a-418">使用提示行为 admins 和标准用户的策略设置。</span><span class="sxs-lookup"><span data-stu-id="b588a-418">Prompt behavior policy settings for admins and standard users are used.</span></span>|
|<span data-ttu-id="b588a-419">localSecurityOptionsDetectApplicationInstallationsAndPromptForElevation</span><span class="sxs-lookup"><span data-stu-id="b588a-419">localSecurityOptionsDetectApplicationInstallationsAndPromptForElevation</span></span>|<span data-ttu-id="b588a-420">布尔</span><span class="sxs-lookup"><span data-stu-id="b588a-420">Boolean</span></span>|<span data-ttu-id="b588a-421">需要提升的权限的应用程序安装将会进行提示管理员凭据。将启用默认值</span><span class="sxs-lookup"><span data-stu-id="b588a-421">App installations requiring elevated privileges will prompt for admin credentials.Default is enabled</span></span>|
|<span data-ttu-id="b588a-422">localSecurityOptionsAllowUIAccessApplicationsForSecureLocations</span><span class="sxs-lookup"><span data-stu-id="b588a-422">localSecurityOptionsAllowUIAccessApplicationsForSecureLocations</span></span>|<span data-ttu-id="b588a-423">布尔</span><span class="sxs-lookup"><span data-stu-id="b588a-423">Boolean</span></span>|<span data-ttu-id="b588a-424">允许 UIAccess 应用程序无需使用安全桌面提示提升。将启用默认值</span><span class="sxs-lookup"><span data-stu-id="b588a-424">Allow UIAccess apps to prompt for elevation without using the secure desktop.Default is enabled</span></span>|
|<span data-ttu-id="b588a-425">localSecurityOptionsUseAdminApprovalMode</span><span class="sxs-lookup"><span data-stu-id="b588a-425">localSecurityOptionsUseAdminApprovalMode</span></span>|<span data-ttu-id="b588a-426">布尔</span><span class="sxs-lookup"><span data-stu-id="b588a-426">Boolean</span></span>|<span data-ttu-id="b588a-427">定义的内置的管理帐户使用管理员批准模式还是具有完整的管理员权限运行所有应用程序。将启用默认值</span><span class="sxs-lookup"><span data-stu-id="b588a-427">Defines whether the built-in admin account uses Admin Approval Mode or runs all apps with full admin privileges.Default is enabled</span></span>|
|<span data-ttu-id="b588a-428">localSecurityOptionsUseAdminApprovalModeForAdministrators</span><span class="sxs-lookup"><span data-stu-id="b588a-428">localSecurityOptionsUseAdminApprovalModeForAdministrators</span></span>|<span data-ttu-id="b588a-429">布尔</span><span class="sxs-lookup"><span data-stu-id="b588a-429">Boolean</span></span>|<span data-ttu-id="b588a-430">定义是否启用管理员批准模式和所有 UAC 策略设置，将启用默认值</span><span class="sxs-lookup"><span data-stu-id="b588a-430">Define whether Admin Approval Mode and all UAC policy settings are enabled, default is enabled</span></span>|
|<span data-ttu-id="b588a-431">localSecurityOptionsInformationShownOnLockScreen</span><span class="sxs-lookup"><span data-stu-id="b588a-431">localSecurityOptionsInformationShownOnLockScreen</span></span>|[<span data-ttu-id="b588a-432">localSecurityOptionsInformationShownOnLockScreenType</span><span class="sxs-lookup"><span data-stu-id="b588a-432">localSecurityOptionsInformationShownOnLockScreenType</span></span>](../resources/intune-deviceconfig-localsecurityoptionsinformationshownonlockscreentype.md)|<span data-ttu-id="b588a-433">配置会话已被锁定时显示的用户信息。</span><span class="sxs-lookup"><span data-stu-id="b588a-433">Configure the user information that is displayed when the session is locked.</span></span> <span data-ttu-id="b588a-434">如果未配置，将显示用户的显示名称、 域和用户名。</span><span class="sxs-lookup"><span data-stu-id="b588a-434">If not configured, user display name, domain and username are shown.</span></span> <span data-ttu-id="b588a-435">可取值为：`notConfigured`、`userDisplayNameDomainUser`、`userDisplayNameOnly`、`doNotDisplayUser`。</span><span class="sxs-lookup"><span data-stu-id="b588a-435">Possible values are: `notConfigured`, `userDisplayNameDomainUser`, `userDisplayNameOnly`, `doNotDisplayUser`.</span></span>|
|<span data-ttu-id="b588a-436">localSecurityOptionsInformationDisplayedOnLockScreen</span><span class="sxs-lookup"><span data-stu-id="b588a-436">localSecurityOptionsInformationDisplayedOnLockScreen</span></span>|[<span data-ttu-id="b588a-437">localSecurityOptionsInformationDisplayedOnLockScreenType</span><span class="sxs-lookup"><span data-stu-id="b588a-437">localSecurityOptionsInformationDisplayedOnLockScreenType</span></span>](../resources/intune-deviceconfig-localsecurityoptionsinformationdisplayedonlockscreentype.md)|<span data-ttu-id="b588a-438">配置会话已被锁定时显示的用户信息。</span><span class="sxs-lookup"><span data-stu-id="b588a-438">Configure the user information that is displayed when the session is locked.</span></span> <span data-ttu-id="b588a-439">如果未配置，将显示用户的显示名称、 域和用户名。</span><span class="sxs-lookup"><span data-stu-id="b588a-439">If not configured, user display name, domain and username are shown.</span></span> <span data-ttu-id="b588a-440">可取值为：`notConfigured`、`administrators`、`administratorsAndPowerUsers`、`administratorsAndInteractiveUsers`。</span><span class="sxs-lookup"><span data-stu-id="b588a-440">Possible values are: `notConfigured`, `administrators`, `administratorsAndPowerUsers`, `administratorsAndInteractiveUsers`.</span></span>|
|<span data-ttu-id="b588a-441">localSecurityOptionsDisableClientDigitallySignCommunicationsIfServerAgrees</span><span class="sxs-lookup"><span data-stu-id="b588a-441">localSecurityOptionsDisableClientDigitallySignCommunicationsIfServerAgrees</span></span>|<span data-ttu-id="b588a-442">布尔</span><span class="sxs-lookup"><span data-stu-id="b588a-442">Boolean</span></span>|<span data-ttu-id="b588a-443">此安全设置确定是否 SMB 客户端尝试协商 SMB 数据包签名。</span><span class="sxs-lookup"><span data-stu-id="b588a-443">This security setting determines whether the SMB client attempts to negotiate SMB packet signing.</span></span>|
|<span data-ttu-id="b588a-444">localSecurityOptionsClientDigitallySignCommunicationsAlways</span><span class="sxs-lookup"><span data-stu-id="b588a-444">localSecurityOptionsClientDigitallySignCommunicationsAlways</span></span>|<span data-ttu-id="b588a-445">布尔</span><span class="sxs-lookup"><span data-stu-id="b588a-445">Boolean</span></span>|<span data-ttu-id="b588a-446">此安全设置确定是否数据包签名所需 SMB 客户端组件。</span><span class="sxs-lookup"><span data-stu-id="b588a-446">This security setting determines whether packet signing is required by the SMB client component.</span></span>|
|<span data-ttu-id="b588a-447">localSecurityOptionsClientSendUnencryptedPasswordToThirdPartySMBServers</span><span class="sxs-lookup"><span data-stu-id="b588a-447">localSecurityOptionsClientSendUnencryptedPasswordToThirdPartySMBServers</span></span>|<span data-ttu-id="b588a-448">布尔</span><span class="sxs-lookup"><span data-stu-id="b588a-448">Boolean</span></span>|<span data-ttu-id="b588a-449">如果启用此安全设置，则允许服务器消息块 (SMB) 重定向到不支持期间身份验证的密码加密的非 Microsoft SMB 服务器发送纯文本密码。</span><span class="sxs-lookup"><span data-stu-id="b588a-449">If this security setting is enabled, the Server Message Block (SMB) redirector is allowed to send plaintext passwords to non-Microsoft SMB servers that do not support password encryption during authentication.</span></span>|
|<span data-ttu-id="b588a-450">localSecurityOptionsDisableServerDigitallySignCommunicationsAlways</span><span class="sxs-lookup"><span data-stu-id="b588a-450">localSecurityOptionsDisableServerDigitallySignCommunicationsAlways</span></span>|<span data-ttu-id="b588a-451">布尔</span><span class="sxs-lookup"><span data-stu-id="b588a-451">Boolean</span></span>|<span data-ttu-id="b588a-452">此安全设置确定是否由 SMB 服务器组件要求签名数据包。</span><span class="sxs-lookup"><span data-stu-id="b588a-452">This security setting determines whether packet signing is required by the SMB server component.</span></span>|
|<span data-ttu-id="b588a-453">localSecurityOptionsDisableServerDigitallySignCommunicationsIfClientAgrees</span><span class="sxs-lookup"><span data-stu-id="b588a-453">localSecurityOptionsDisableServerDigitallySignCommunicationsIfClientAgrees</span></span>|<span data-ttu-id="b588a-454">布尔</span><span class="sxs-lookup"><span data-stu-id="b588a-454">Boolean</span></span>|<span data-ttu-id="b588a-455">此安全设置确定 SMB 服务器是否协商 SMB 数据包签名与请求的客户端。</span><span class="sxs-lookup"><span data-stu-id="b588a-455">This security setting determines whether the SMB server will negotiate SMB packet signing with clients that request it.</span></span>|
|<span data-ttu-id="b588a-456">localSecurityOptionsRestrictAnonymousAccessToNamedPipesAndShares</span><span class="sxs-lookup"><span data-stu-id="b588a-456">localSecurityOptionsRestrictAnonymousAccessToNamedPipesAndShares</span></span>|<span data-ttu-id="b588a-457">布尔</span><span class="sxs-lookup"><span data-stu-id="b588a-457">Boolean</span></span>|<span data-ttu-id="b588a-458">默认情况下，此安全设置将匿名访问限制为共享和管道的可匿名访问的命名的管道和可匿名访问的共享的设置</span><span class="sxs-lookup"><span data-stu-id="b588a-458">By default, this security setting restricts anonymous access to shares and pipes to the settings for named pipes that can be accessed anonymously and Shares that can be accessed anonymously</span></span>|
|<span data-ttu-id="b588a-459">localSecurityOptionsDoNotAllowAnonymousEnumerationOfSAMAccounts</span><span class="sxs-lookup"><span data-stu-id="b588a-459">localSecurityOptionsDoNotAllowAnonymousEnumerationOfSAMAccounts</span></span>|<span data-ttu-id="b588a-460">布尔</span><span class="sxs-lookup"><span data-stu-id="b588a-460">Boolean</span></span>|<span data-ttu-id="b588a-461">此安全设置确定将对匿名连接到计算机上授予其他权限。</span><span class="sxs-lookup"><span data-stu-id="b588a-461">This security setting determines what additional permissions will be granted for anonymous connections to the computer.</span></span>|
|<span data-ttu-id="b588a-462">localSecurityOptionsAllowAnonymousEnumerationOfSAMAccountsAndShares</span><span class="sxs-lookup"><span data-stu-id="b588a-462">localSecurityOptionsAllowAnonymousEnumerationOfSAMAccountsAndShares</span></span>|<span data-ttu-id="b588a-463">布尔</span><span class="sxs-lookup"><span data-stu-id="b588a-463">Boolean</span></span>|<span data-ttu-id="b588a-464">此安全设置确定是否允许匿名用户执行某些活动，如枚举的域帐户和网络共享名称。</span><span class="sxs-lookup"><span data-stu-id="b588a-464">This security setting determines whether to allows anonymous users to perform certain activities, such as enumerating the names of domain accounts and network shares.</span></span>|
|<span data-ttu-id="b588a-465">localSecurityOptionsDoNotStoreLANManagerHashValueOnNextPasswordChange</span><span class="sxs-lookup"><span data-stu-id="b588a-465">localSecurityOptionsDoNotStoreLANManagerHashValueOnNextPasswordChange</span></span>|<span data-ttu-id="b588a-466">布尔</span><span class="sxs-lookup"><span data-stu-id="b588a-466">Boolean</span></span>|<span data-ttu-id="b588a-467">此安全设置确定，是否在下次密码更改，存储新密码的 LAN Manager (LM) 哈希值。</span><span class="sxs-lookup"><span data-stu-id="b588a-467">This security setting determines if, at the next password change, the LAN Manager (LM) hash value for the new password is stored.</span></span> <span data-ttu-id="b588a-468">默认情况下，它不存储。</span><span class="sxs-lookup"><span data-stu-id="b588a-468">It’s not stored by default.</span></span>|
|<span data-ttu-id="b588a-469">localSecurityOptionsSmartCardRemovalBehavior</span><span class="sxs-lookup"><span data-stu-id="b588a-469">localSecurityOptionsSmartCardRemovalBehavior</span></span>|[<span data-ttu-id="b588a-470">localSecurityOptionsSmartCardRemovalBehaviorType</span><span class="sxs-lookup"><span data-stu-id="b588a-470">localSecurityOptionsSmartCardRemovalBehaviorType</span></span>](../resources/intune-deviceconfig-localsecurityoptionssmartcardremovalbehaviortype.md)|<span data-ttu-id="b588a-471">此安全设置确定智能卡读卡器从移除智能卡登录的用户时，会发生什么情况。</span><span class="sxs-lookup"><span data-stu-id="b588a-471">This security setting determines what happens when the smart card for a logged-on user is removed from the smart card reader.</span></span> <span data-ttu-id="b588a-472">可取值为：`lockWorkstation`、`noAction`、`forceLogoff`、`disconnectRemoteDesktopSession`。</span><span class="sxs-lookup"><span data-stu-id="b588a-472">Possible values are: `lockWorkstation`, `noAction`, `forceLogoff`, `disconnectRemoteDesktopSession`.</span></span>|
|<span data-ttu-id="b588a-473">defenderSecurityCenterDisableAppBrowserUI</span><span class="sxs-lookup"><span data-stu-id="b588a-473">defenderSecurityCenterDisableAppBrowserUI</span></span>|<span data-ttu-id="b588a-474">布尔</span><span class="sxs-lookup"><span data-stu-id="b588a-474">Boolean</span></span>|<span data-ttu-id="b588a-475">用于禁用的应用程序和浏览器的保护区域显示。</span><span class="sxs-lookup"><span data-stu-id="b588a-475">Used to disable the display of the app and browser protection area.</span></span>|
|<span data-ttu-id="b588a-476">defenderSecurityCenterDisableFamilyUI</span><span class="sxs-lookup"><span data-stu-id="b588a-476">defenderSecurityCenterDisableFamilyUI</span></span>|<span data-ttu-id="b588a-477">布尔</span><span class="sxs-lookup"><span data-stu-id="b588a-477">Boolean</span></span>|<span data-ttu-id="b588a-478">用于禁用系列选项区域的显示。</span><span class="sxs-lookup"><span data-stu-id="b588a-478">Used to disable the display of the family options area.</span></span>|
|<span data-ttu-id="b588a-479">defenderSecurityCenterDisableHealthUI</span><span class="sxs-lookup"><span data-stu-id="b588a-479">defenderSecurityCenterDisableHealthUI</span></span>|<span data-ttu-id="b588a-480">布尔</span><span class="sxs-lookup"><span data-stu-id="b588a-480">Boolean</span></span>|<span data-ttu-id="b588a-481">用于禁用设备性能和运行状况区域的显示。</span><span class="sxs-lookup"><span data-stu-id="b588a-481">Used to disable the display of the device performance and health area.</span></span>|
|<span data-ttu-id="b588a-482">defenderSecurityCenterDisableNetworkUI</span><span class="sxs-lookup"><span data-stu-id="b588a-482">defenderSecurityCenterDisableNetworkUI</span></span>|<span data-ttu-id="b588a-483">布尔</span><span class="sxs-lookup"><span data-stu-id="b588a-483">Boolean</span></span>|<span data-ttu-id="b588a-484">用于禁用防火墙和网络保护区域的显示。</span><span class="sxs-lookup"><span data-stu-id="b588a-484">Used to disable the display of the firewall and network protection area.</span></span>|
|<span data-ttu-id="b588a-485">defenderSecurityCenterDisableVirusUI</span><span class="sxs-lookup"><span data-stu-id="b588a-485">defenderSecurityCenterDisableVirusUI</span></span>|<span data-ttu-id="b588a-486">布尔</span><span class="sxs-lookup"><span data-stu-id="b588a-486">Boolean</span></span>|<span data-ttu-id="b588a-487">用于禁用病毒和威胁保护区域的显示。</span><span class="sxs-lookup"><span data-stu-id="b588a-487">Used to disable the display of the virus and threat protection area.</span></span>|
|<span data-ttu-id="b588a-488">defenderSecurityCenterDisableAccountUI</span><span class="sxs-lookup"><span data-stu-id="b588a-488">defenderSecurityCenterDisableAccountUI</span></span>|<span data-ttu-id="b588a-489">布尔</span><span class="sxs-lookup"><span data-stu-id="b588a-489">Boolean</span></span>|<span data-ttu-id="b588a-490">用于禁用帐户保护区域的显示。</span><span class="sxs-lookup"><span data-stu-id="b588a-490">Used to disable the display of the account protection area.</span></span>|
|<span data-ttu-id="b588a-491">defenderSecurityCenterDisableHardwareUI</span><span class="sxs-lookup"><span data-stu-id="b588a-491">defenderSecurityCenterDisableHardwareUI</span></span>|<span data-ttu-id="b588a-492">布尔</span><span class="sxs-lookup"><span data-stu-id="b588a-492">Boolean</span></span>|<span data-ttu-id="b588a-493">用于禁用硬件保护区域的显示。</span><span class="sxs-lookup"><span data-stu-id="b588a-493">Used to disable the display of the hardware protection area.</span></span>|
|<span data-ttu-id="b588a-494">defenderSecurityCenterDisableRansomwareUI</span><span class="sxs-lookup"><span data-stu-id="b588a-494">defenderSecurityCenterDisableRansomwareUI</span></span>|<span data-ttu-id="b588a-495">布尔</span><span class="sxs-lookup"><span data-stu-id="b588a-495">Boolean</span></span>|<span data-ttu-id="b588a-496">用于禁用勒索软件保护区域的显示。</span><span class="sxs-lookup"><span data-stu-id="b588a-496">Used to disable the display of the ransomware protection area.</span></span> |
|<span data-ttu-id="b588a-497">defenderSecurityCenterDisableSecureBootUI</span><span class="sxs-lookup"><span data-stu-id="b588a-497">defenderSecurityCenterDisableSecureBootUI</span></span>|<span data-ttu-id="b588a-498">布尔</span><span class="sxs-lookup"><span data-stu-id="b588a-498">Boolean</span></span>|<span data-ttu-id="b588a-499">用于禁用的设备安全下的安全启动区域显示。</span><span class="sxs-lookup"><span data-stu-id="b588a-499">Used to disable the display of the secure boot area under Device security.</span></span>|
|<span data-ttu-id="b588a-500">defenderSecurityCenterDisableTroubleshootingUI</span><span class="sxs-lookup"><span data-stu-id="b588a-500">defenderSecurityCenterDisableTroubleshootingUI</span></span>|<span data-ttu-id="b588a-501">布尔</span><span class="sxs-lookup"><span data-stu-id="b588a-501">Boolean</span></span>|<span data-ttu-id="b588a-502">用于禁用安全过程下设备安全疑难解答的显示。</span><span class="sxs-lookup"><span data-stu-id="b588a-502">Used to disable the display of the security process troubleshooting under Device security.</span></span>|
|<span data-ttu-id="b588a-503">defenderSecurityCenterOrganizationDisplayName</span><span class="sxs-lookup"><span data-stu-id="b588a-503">defenderSecurityCenterOrganizationDisplayName</span></span>|<span data-ttu-id="b588a-504">字符串</span><span class="sxs-lookup"><span data-stu-id="b588a-504">String</span></span>|<span data-ttu-id="b588a-505">向用户显示公司名称。</span><span class="sxs-lookup"><span data-stu-id="b588a-505">The company name that is displayed to the users.</span></span>|
|<span data-ttu-id="b588a-506">defenderSecurityCenterHelpEmail</span><span class="sxs-lookup"><span data-stu-id="b588a-506">defenderSecurityCenterHelpEmail</span></span>|<span data-ttu-id="b588a-507">字符串</span><span class="sxs-lookup"><span data-stu-id="b588a-507">String</span></span>|<span data-ttu-id="b588a-508">向用户显示的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="b588a-508">The email address that is displayed to users.</span></span>|
|<span data-ttu-id="b588a-509">defenderSecurityCenterHelpPhone</span><span class="sxs-lookup"><span data-stu-id="b588a-509">defenderSecurityCenterHelpPhone</span></span>|<span data-ttu-id="b588a-510">字符串</span><span class="sxs-lookup"><span data-stu-id="b588a-510">String</span></span>|<span data-ttu-id="b588a-511">电话号码或向用户显示的 Skype ID 中。</span><span class="sxs-lookup"><span data-stu-id="b588a-511">The phone number or Skype ID that is displayed to users.</span></span>|
|<span data-ttu-id="b588a-512">defenderSecurityCenterHelpURL</span><span class="sxs-lookup"><span data-stu-id="b588a-512">defenderSecurityCenterHelpURL</span></span>|<span data-ttu-id="b588a-513">字符串</span><span class="sxs-lookup"><span data-stu-id="b588a-513">String</span></span>|<span data-ttu-id="b588a-514">帮助门户这向用户显示的 URL。</span><span class="sxs-lookup"><span data-stu-id="b588a-514">The help portal URL this is displayed to users.</span></span>|
|<span data-ttu-id="b588a-515">defenderSecurityCenterNotificationsFromApp</span><span class="sxs-lookup"><span data-stu-id="b588a-515">defenderSecurityCenterNotificationsFromApp</span></span>|[<span data-ttu-id="b588a-516">defenderSecurityCenterNotificationsFromAppType</span><span class="sxs-lookup"><span data-stu-id="b588a-516">defenderSecurityCenterNotificationsFromAppType</span></span>](../resources/intune-deviceconfig-defendersecuritycenternotificationsfromapptype.md)|<span data-ttu-id="b588a-517">若要从应用程序的显示区域显示的通知。</span><span class="sxs-lookup"><span data-stu-id="b588a-517">Notifications to show from the displayed areas of app.</span></span> <span data-ttu-id="b588a-518">可取值为：`notConfigured`、`blockNoncriticalNotifications`、`blockAllNotifications`。</span><span class="sxs-lookup"><span data-stu-id="b588a-518">Possible values are: `notConfigured`, `blockNoncriticalNotifications`, `blockAllNotifications`.</span></span>|
|<span data-ttu-id="b588a-519">defenderSecurityCenterITContactDisplay</span><span class="sxs-lookup"><span data-stu-id="b588a-519">defenderSecurityCenterITContactDisplay</span></span>|[<span data-ttu-id="b588a-520">defenderSecurityCenterITContactDisplayType</span><span class="sxs-lookup"><span data-stu-id="b588a-520">defenderSecurityCenterITContactDisplayType</span></span>](../resources/intune-deviceconfig-defendersecuritycenteritcontactdisplaytype.md)|<span data-ttu-id="b588a-521">配置显示 IT 联系人位置向最终用户的信息。</span><span class="sxs-lookup"><span data-stu-id="b588a-521">Configure where to display IT contact information to end users.</span></span> <span data-ttu-id="b588a-522">可取值为：`notConfigured`、`displayInAppAndInNotifications`、`displayOnlyInApp`、`displayOnlyInNotifications`。</span><span class="sxs-lookup"><span data-stu-id="b588a-522">Possible values are: `notConfigured`, `displayInAppAndInNotifications`, `displayOnlyInApp`, `displayOnlyInNotifications`.</span></span>|
|<span data-ttu-id="b588a-523">firewallBlockStatefulFTP</span><span class="sxs-lookup"><span data-stu-id="b588a-523">firewallBlockStatefulFTP</span></span>|<span data-ttu-id="b588a-524">Boolean</span><span class="sxs-lookup"><span data-stu-id="b588a-524">Boolean</span></span>|<span data-ttu-id="b588a-525">阻止到设备的有状态 FTP 连接</span><span class="sxs-lookup"><span data-stu-id="b588a-525">Blocks stateful FTP connections to the device</span></span>|
|<span data-ttu-id="b588a-526">firewallIdleTimeoutForSecurityAssociationInSeconds</span><span class="sxs-lookup"><span data-stu-id="b588a-526">firewallIdleTimeoutForSecurityAssociationInSeconds</span></span>|<span data-ttu-id="b588a-527">Int32</span><span class="sxs-lookup"><span data-stu-id="b588a-527">Int32</span></span>|<span data-ttu-id="b588a-528">配置安全关联的空闲超时（以秒为单位），值范围为 300 到 3600（包括这两个值）。</span><span class="sxs-lookup"><span data-stu-id="b588a-528">Configures the idle timeout for security associations, in seconds, from 300 to 3600 inclusive.</span></span> <span data-ttu-id="b588a-529">这是一个时间段，在此之后安全关联将过期并被删除。</span><span class="sxs-lookup"><span data-stu-id="b588a-529">This is the period after which security associations will expire and be deleted.</span></span> <span data-ttu-id="b588a-530">有效值为 300 至 3600。</span><span class="sxs-lookup"><span data-stu-id="b588a-530">Valid values 300 to 3600</span></span>|
|<span data-ttu-id="b588a-531">firewallPreSharedKeyEncodingMethod</span><span class="sxs-lookup"><span data-stu-id="b588a-531">firewallPreSharedKeyEncodingMethod</span></span>|[<span data-ttu-id="b588a-532">firewallPreSharedKeyEncodingMethodType</span><span class="sxs-lookup"><span data-stu-id="b588a-532">firewallPreSharedKeyEncodingMethodType</span></span>](../resources/intune-deviceconfig-firewallpresharedkeyencodingmethodtype.md)|<span data-ttu-id="b588a-533">选择要使用编码的预共享的键。</span><span class="sxs-lookup"><span data-stu-id="b588a-533">Select the preshared key encoding to be used.</span></span> <span data-ttu-id="b588a-534">可取值为：`deviceDefault`、`none`、`utF8`。</span><span class="sxs-lookup"><span data-stu-id="b588a-534">Possible values are: `deviceDefault`, `none`, `utF8`.</span></span>|
|<span data-ttu-id="b588a-535">firewallIPSecExemptionsAllowNeighborDiscovery</span><span class="sxs-lookup"><span data-stu-id="b588a-535">firewallIPSecExemptionsAllowNeighborDiscovery</span></span>|<span data-ttu-id="b588a-536">Boolean</span><span class="sxs-lookup"><span data-stu-id="b588a-536">Boolean</span></span>|<span data-ttu-id="b588a-537">配置 IPSec 免除项以允许邻居发现 IPv6 ICMP 类型代码</span><span class="sxs-lookup"><span data-stu-id="b588a-537">Configures IPSec exemptions to allow neighbor discovery IPv6 ICMP type-codes</span></span>|
|<span data-ttu-id="b588a-538">firewallIPSecExemptionsAllowICMP</span><span class="sxs-lookup"><span data-stu-id="b588a-538">firewallIPSecExemptionsAllowICMP</span></span>|<span data-ttu-id="b588a-539">Boolean</span><span class="sxs-lookup"><span data-stu-id="b588a-539">Boolean</span></span>|<span data-ttu-id="b588a-540">配置 IPSec 免除项以允许 ICMP</span><span class="sxs-lookup"><span data-stu-id="b588a-540">Configures IPSec exemptions to allow ICMP</span></span>|
|<span data-ttu-id="b588a-541">firewallIPSecExemptionsAllowRouterDiscovery</span><span class="sxs-lookup"><span data-stu-id="b588a-541">firewallIPSecExemptionsAllowRouterDiscovery</span></span>|<span data-ttu-id="b588a-542">Boolean</span><span class="sxs-lookup"><span data-stu-id="b588a-542">Boolean</span></span>|<span data-ttu-id="b588a-543">配置 IPSec 免除项以允许路由器发现 IPv6 ICMP 类型代码</span><span class="sxs-lookup"><span data-stu-id="b588a-543">Configures IPSec exemptions to allow router discovery IPv6 ICMP type-codes</span></span>|
|<span data-ttu-id="b588a-544">firewallIPSecExemptionsAllowDHCP</span><span class="sxs-lookup"><span data-stu-id="b588a-544">firewallIPSecExemptionsAllowDHCP</span></span>|<span data-ttu-id="b588a-545">Boolean</span><span class="sxs-lookup"><span data-stu-id="b588a-545">Boolean</span></span>|<span data-ttu-id="b588a-546">配置 IPSec 免除项以允许 IPv4 和 IPv6 DHCP 通信</span><span class="sxs-lookup"><span data-stu-id="b588a-546">Configures IPSec exemptions to allow both IPv4 and IPv6 DHCP traffic</span></span>|
|<span data-ttu-id="b588a-547">firewallCertificateRevocationListCheckMethod</span><span class="sxs-lookup"><span data-stu-id="b588a-547">firewallCertificateRevocationListCheckMethod</span></span>|[<span data-ttu-id="b588a-548">firewallCertificateRevocationListCheckMethodType</span><span class="sxs-lookup"><span data-stu-id="b588a-548">firewallCertificateRevocationListCheckMethodType</span></span>](../resources/intune-deviceconfig-firewallcertificaterevocationlistcheckmethodtype.md)|<span data-ttu-id="b588a-549">指定如何强制实施证书吊销列表。</span><span class="sxs-lookup"><span data-stu-id="b588a-549">Specify how the certificate revocation list is to be enforced.</span></span> <span data-ttu-id="b588a-550">可取值为：`deviceDefault`、`none`、`attempt`、`require`。</span><span class="sxs-lookup"><span data-stu-id="b588a-550">Possible values are: `deviceDefault`, `none`, `attempt`, `require`.</span></span>|
|<span data-ttu-id="b588a-551">firewallMergeKeyingModuleSettings</span><span class="sxs-lookup"><span data-stu-id="b588a-551">firewallMergeKeyingModuleSettings</span></span>|<span data-ttu-id="b588a-552">Boolean</span><span class="sxs-lookup"><span data-stu-id="b588a-552">Boolean</span></span>|<span data-ttu-id="b588a-553">如果键控模块不完全支持身份验证集，请指示模块仅忽略不受支持的身份验证套件而不是整个集</span><span class="sxs-lookup"><span data-stu-id="b588a-553">If an authentication set is not fully supported by a keying module, direct the module to ignore only unsupported authentication suites rather than the entire set</span></span>|
|<span data-ttu-id="b588a-554">firewallPacketQueueingMethod</span><span class="sxs-lookup"><span data-stu-id="b588a-554">firewallPacketQueueingMethod</span></span>|[<span data-ttu-id="b588a-555">firewallPacketQueueingMethodType</span><span class="sxs-lookup"><span data-stu-id="b588a-555">firewallPacketQueueingMethodType</span></span>](../resources/intune-deviceconfig-firewallpacketqueueingmethodtype.md)|<span data-ttu-id="b588a-556">配置数据包 queueing 应如何应用隧道网关方案中。</span><span class="sxs-lookup"><span data-stu-id="b588a-556">Configures how packet queueing should be applied in the tunnel gateway scenario.</span></span> <span data-ttu-id="b588a-557">可取值为：`deviceDefault`、`disabled`、`queueInbound`、`queueOutbound`、`queueBoth`。</span><span class="sxs-lookup"><span data-stu-id="b588a-557">Possible values are: `deviceDefault`, `disabled`, `queueInbound`, `queueOutbound`, `queueBoth`.</span></span>|
|<span data-ttu-id="b588a-558">firewallProfileDomain</span><span class="sxs-lookup"><span data-stu-id="b588a-558">firewallProfileDomain</span></span>|[<span data-ttu-id="b588a-559">windowsFirewallNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="b588a-559">windowsFirewallNetworkProfile</span></span>](../resources/intune-deviceconfig-windowsfirewallnetworkprofile.md)|<span data-ttu-id="b588a-560">配置域网络的防火墙配置文件设置</span><span class="sxs-lookup"><span data-stu-id="b588a-560">Configures the firewall profile settings for domain networks</span></span>|
|<span data-ttu-id="b588a-561">firewallProfilePublic</span><span class="sxs-lookup"><span data-stu-id="b588a-561">firewallProfilePublic</span></span>|[<span data-ttu-id="b588a-562">windowsFirewallNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="b588a-562">windowsFirewallNetworkProfile</span></span>](../resources/intune-deviceconfig-windowsfirewallnetworkprofile.md)|<span data-ttu-id="b588a-563">配置公用网络的防火墙配置文件设置</span><span class="sxs-lookup"><span data-stu-id="b588a-563">Configures the firewall profile settings for public networks</span></span>|
|<span data-ttu-id="b588a-564">firewallProfilePrivate</span><span class="sxs-lookup"><span data-stu-id="b588a-564">firewallProfilePrivate</span></span>|[<span data-ttu-id="b588a-565">windowsFirewallNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="b588a-565">windowsFirewallNetworkProfile</span></span>](../resources/intune-deviceconfig-windowsfirewallnetworkprofile.md)|<span data-ttu-id="b588a-566">配置专用网络的防火墙配置文件设置</span><span class="sxs-lookup"><span data-stu-id="b588a-566">Configures the firewall profile settings for private networks</span></span>|
|<span data-ttu-id="b588a-567">defenderAttackSurfaceReductionExcludedPaths</span><span class="sxs-lookup"><span data-stu-id="b588a-567">defenderAttackSurfaceReductionExcludedPaths</span></span>|<span data-ttu-id="b588a-568">String 集合</span><span class="sxs-lookup"><span data-stu-id="b588a-568">String collection</span></span>|<span data-ttu-id="b588a-569">要从攻击面减少规则中排除的 exe 文件和文件夹的列表</span><span class="sxs-lookup"><span data-stu-id="b588a-569">List of exe files and folders to be excluded from attack surface reduction rules</span></span>|
|<span data-ttu-id="b588a-570">defenderOfficeAppsOtherProcessInjectionType</span><span class="sxs-lookup"><span data-stu-id="b588a-570">defenderOfficeAppsOtherProcessInjectionType</span></span>|[<span data-ttu-id="b588a-571">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="b588a-571">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="b588a-572">值，指示将到其他进程的 Office 应用程序的行为。</span><span class="sxs-lookup"><span data-stu-id="b588a-572">Value indicating the behavior of Office applications injecting into other processes.</span></span> <span data-ttu-id="b588a-573">可取值为：`userDefined`、`block`、`auditMode`。</span><span class="sxs-lookup"><span data-stu-id="b588a-573">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="b588a-574">defenderOfficeAppsOtherProcessInjection</span><span class="sxs-lookup"><span data-stu-id="b588a-574">defenderOfficeAppsOtherProcessInjection</span></span>|[<span data-ttu-id="b588a-575">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="b588a-575">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="b588a-576">值，指示将到其他进程的 Office 应用程序的行为。</span><span class="sxs-lookup"><span data-stu-id="b588a-576">Value indicating the behavior of  Office applications injecting into other processes.</span></span> <span data-ttu-id="b588a-577">可取值为：`userDefined`、`enable`、`auditMode`。</span><span class="sxs-lookup"><span data-stu-id="b588a-577">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="b588a-578">defenderOfficeAppsExecutableContentCreationOrLaunchType</span><span class="sxs-lookup"><span data-stu-id="b588a-578">defenderOfficeAppsExecutableContentCreationOrLaunchType</span></span>|[<span data-ttu-id="b588a-579">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="b588a-579">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="b588a-580">指示 Office 应用程序/宏创建或启动可执行文件内容的行为的值。</span><span class="sxs-lookup"><span data-stu-id="b588a-580">Value indicating the behavior of Office applications/macros creating or launching executable content.</span></span> <span data-ttu-id="b588a-581">可取值为：`userDefined`、`block`、`auditMode`。</span><span class="sxs-lookup"><span data-stu-id="b588a-581">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="b588a-582">defenderOfficeAppsExecutableContentCreationOrLaunch</span><span class="sxs-lookup"><span data-stu-id="b588a-582">defenderOfficeAppsExecutableContentCreationOrLaunch</span></span>|[<span data-ttu-id="b588a-583">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="b588a-583">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="b588a-584">指示 Office 应用程序/宏创建或启动可执行文件内容的行为的值。</span><span class="sxs-lookup"><span data-stu-id="b588a-584">Value indicating the behavior of Office applications/macros creating or launching executable content.</span></span> <span data-ttu-id="b588a-585">可取值为：`userDefined`、`enable`、`auditMode`。</span><span class="sxs-lookup"><span data-stu-id="b588a-585">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="b588a-586">defenderOfficeAppsLaunchChildProcessType</span><span class="sxs-lookup"><span data-stu-id="b588a-586">defenderOfficeAppsLaunchChildProcessType</span></span>|[<span data-ttu-id="b588a-587">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="b588a-587">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="b588a-588">指示启动子进程的 Office 应用程序的行为的值。</span><span class="sxs-lookup"><span data-stu-id="b588a-588">Value indicating the behavior of Office application launching child processes.</span></span> <span data-ttu-id="b588a-589">可取值为：`userDefined`、`block`、`auditMode`。</span><span class="sxs-lookup"><span data-stu-id="b588a-589">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="b588a-590">defenderOfficeAppsLaunchChildProcess</span><span class="sxs-lookup"><span data-stu-id="b588a-590">defenderOfficeAppsLaunchChildProcess</span></span>|[<span data-ttu-id="b588a-591">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="b588a-591">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="b588a-592">指示启动子进程的 Office 应用程序的行为的值。</span><span class="sxs-lookup"><span data-stu-id="b588a-592">Value indicating the behavior of Office application launching child processes.</span></span> <span data-ttu-id="b588a-593">可取值为：`userDefined`、`enable`、`auditMode`。</span><span class="sxs-lookup"><span data-stu-id="b588a-593">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="b588a-594">defenderOfficeMacroCodeAllowWin32ImportsType</span><span class="sxs-lookup"><span data-stu-id="b588a-594">defenderOfficeMacroCodeAllowWin32ImportsType</span></span>|[<span data-ttu-id="b588a-595">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="b588a-595">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="b588a-596">值，该值指示的 Win32 行为导入从 Office 中的宏代码。</span><span class="sxs-lookup"><span data-stu-id="b588a-596">Value indicating the behavior of Win32 imports from Macro code in Office.</span></span> <span data-ttu-id="b588a-597">可取值为：`userDefined`、`block`、`auditMode`。</span><span class="sxs-lookup"><span data-stu-id="b588a-597">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="b588a-598">defenderOfficeMacroCodeAllowWin32Imports</span><span class="sxs-lookup"><span data-stu-id="b588a-598">defenderOfficeMacroCodeAllowWin32Imports</span></span>|[<span data-ttu-id="b588a-599">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="b588a-599">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="b588a-600">值，该值指示的 Win32 行为导入从 Office 中的宏代码。</span><span class="sxs-lookup"><span data-stu-id="b588a-600">Value indicating the behavior of Win32 imports from Macro code in Office.</span></span> <span data-ttu-id="b588a-601">可取值为：`userDefined`、`enable`、`auditMode`。</span><span class="sxs-lookup"><span data-stu-id="b588a-601">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="b588a-602">defenderScriptObfuscatedMacroCodeType</span><span class="sxs-lookup"><span data-stu-id="b588a-602">defenderScriptObfuscatedMacroCodeType</span></span>|[<span data-ttu-id="b588a-603">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="b588a-603">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="b588a-604">值，该值指示经过模糊处理 js/vbs/ps/macro 代码的行为。</span><span class="sxs-lookup"><span data-stu-id="b588a-604">Value indicating the behavior of obfuscated js/vbs/ps/macro code.</span></span> <span data-ttu-id="b588a-605">可取值为：`userDefined`、`block`、`auditMode`。</span><span class="sxs-lookup"><span data-stu-id="b588a-605">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="b588a-606">defenderScriptObfuscatedMacroCode</span><span class="sxs-lookup"><span data-stu-id="b588a-606">defenderScriptObfuscatedMacroCode</span></span>|[<span data-ttu-id="b588a-607">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="b588a-607">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="b588a-608">值，该值指示经过模糊处理 js/vbs/ps/macro 代码的行为。</span><span class="sxs-lookup"><span data-stu-id="b588a-608">Value indicating the behavior of obfuscated js/vbs/ps/macro code.</span></span> <span data-ttu-id="b588a-609">可取值为：`userDefined`、`enable`、`auditMode`。</span><span class="sxs-lookup"><span data-stu-id="b588a-609">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="b588a-610">defenderScriptDownloadedPayloadExecutionType</span><span class="sxs-lookup"><span data-stu-id="b588a-610">defenderScriptDownloadedPayloadExecutionType</span></span>|[<span data-ttu-id="b588a-611">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="b588a-611">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="b588a-612">从 Internet 下载的值，该值指示 js/vbs 执行负载的行为。</span><span class="sxs-lookup"><span data-stu-id="b588a-612">Value indicating the behavior of js/vbs executing payload downloaded from Internet.</span></span> <span data-ttu-id="b588a-613">可取值为：`userDefined`、`block`、`auditMode`。</span><span class="sxs-lookup"><span data-stu-id="b588a-613">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="b588a-614">defenderScriptDownloadedPayloadExecution</span><span class="sxs-lookup"><span data-stu-id="b588a-614">defenderScriptDownloadedPayloadExecution</span></span>|[<span data-ttu-id="b588a-615">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="b588a-615">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="b588a-616">从 Internet 下载的值，该值指示 js/vbs 执行负载的行为。</span><span class="sxs-lookup"><span data-stu-id="b588a-616">Value indicating the behavior of js/vbs executing payload downloaded from Internet.</span></span> <span data-ttu-id="b588a-617">可取值为：`userDefined`、`enable`、`auditMode`。</span><span class="sxs-lookup"><span data-stu-id="b588a-617">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="b588a-618">defenderPreventCredentialStealingType</span><span class="sxs-lookup"><span data-stu-id="b588a-618">defenderPreventCredentialStealingType</span></span>|[<span data-ttu-id="b588a-619">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="b588a-619">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="b588a-620">值，该值指示是否允许从 Windows 本地安全机构子系统窃取的凭据。</span><span class="sxs-lookup"><span data-stu-id="b588a-620">Value indicating if credential stealing from the Windows local security authority subsystem is permitted.</span></span> <span data-ttu-id="b588a-621">可取值为：`userDefined`、`enable`、`auditMode`。</span><span class="sxs-lookup"><span data-stu-id="b588a-621">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="b588a-622">defenderProcessCreationType</span><span class="sxs-lookup"><span data-stu-id="b588a-622">defenderProcessCreationType</span></span>|[<span data-ttu-id="b588a-623">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="b588a-623">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="b588a-624">值，该值指示响应来自 PSExec 和 WMI 命令的过程创建。</span><span class="sxs-lookup"><span data-stu-id="b588a-624">Value indicating response to process creations originating from PSExec and WMI commands.</span></span> <span data-ttu-id="b588a-625">可取值为：`userDefined`、`block`、`auditMode`。</span><span class="sxs-lookup"><span data-stu-id="b588a-625">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="b588a-626">defenderProcessCreation</span><span class="sxs-lookup"><span data-stu-id="b588a-626">defenderProcessCreation</span></span>|[<span data-ttu-id="b588a-627">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="b588a-627">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="b588a-628">值，该值指示响应来自 PSExec 和 WMI 命令的过程创建。</span><span class="sxs-lookup"><span data-stu-id="b588a-628">Value indicating response to process creations originating from PSExec and WMI commands.</span></span> <span data-ttu-id="b588a-629">可取值为：`userDefined`、`enable`、`auditMode`。</span><span class="sxs-lookup"><span data-stu-id="b588a-629">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="b588a-630">defenderUntrustedUSBProcessType</span><span class="sxs-lookup"><span data-stu-id="b588a-630">defenderUntrustedUSBProcessType</span></span>|[<span data-ttu-id="b588a-631">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="b588a-631">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="b588a-632">值，该值指示从 USB 运行的受信任和无符号流程的响应。</span><span class="sxs-lookup"><span data-stu-id="b588a-632">Value indicating response to untrusted and unsigned processes that run from USB.</span></span> <span data-ttu-id="b588a-633">可取值为：`userDefined`、`block`、`auditMode`。</span><span class="sxs-lookup"><span data-stu-id="b588a-633">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="b588a-634">defenderUntrustedUSBProcess</span><span class="sxs-lookup"><span data-stu-id="b588a-634">defenderUntrustedUSBProcess</span></span>|[<span data-ttu-id="b588a-635">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="b588a-635">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="b588a-636">值，该值指示从 USB 运行的受信任和无符号流程的响应。</span><span class="sxs-lookup"><span data-stu-id="b588a-636">Value indicating response to untrusted and unsigned processes that run from USB.</span></span> <span data-ttu-id="b588a-637">可取值为：`userDefined`、`enable`、`auditMode`。</span><span class="sxs-lookup"><span data-stu-id="b588a-637">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="b588a-638">defenderUntrustedExecutableType</span><span class="sxs-lookup"><span data-stu-id="b588a-638">defenderUntrustedExecutableType</span></span>|[<span data-ttu-id="b588a-639">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="b588a-639">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="b588a-640">值，该值指示响应可执行文件的传播、 年龄或受信任的列表不满足条件。</span><span class="sxs-lookup"><span data-stu-id="b588a-640">Value indicating response to executables that don't meet a prevalence, age, or trusted list criteria.</span></span> <span data-ttu-id="b588a-641">可取值为：`userDefined`、`block`、`auditMode`。</span><span class="sxs-lookup"><span data-stu-id="b588a-641">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="b588a-642">defenderUntrustedExecutable</span><span class="sxs-lookup"><span data-stu-id="b588a-642">defenderUntrustedExecutable</span></span>|[<span data-ttu-id="b588a-643">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="b588a-643">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="b588a-644">值，该值指示响应可执行文件的传播、 年龄或受信任的列表不满足条件。</span><span class="sxs-lookup"><span data-stu-id="b588a-644">Value indicating response to executables that don't meet a prevalence, age, or trusted list criteria.</span></span> <span data-ttu-id="b588a-645">可取值为：`userDefined`、`enable`、`auditMode`。</span><span class="sxs-lookup"><span data-stu-id="b588a-645">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="b588a-646">defenderEmailContentExecutionType</span><span class="sxs-lookup"><span data-stu-id="b588a-646">defenderEmailContentExecutionType</span></span>|[<span data-ttu-id="b588a-647">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="b588a-647">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="b588a-648">指示是否应该从电子邮件 （客户端 webmail/邮件） 放执行 （exe、 dll，ps、 js、 vbs 等） 的可执行内容的值。</span><span class="sxs-lookup"><span data-stu-id="b588a-648">Value indicating if execution of executable content (exe, dll, ps, js, vbs, etc) should be dropped from email (webmail/mail-client).</span></span> <span data-ttu-id="b588a-649">可取值为：`userDefined`、`block`、`auditMode`。</span><span class="sxs-lookup"><span data-stu-id="b588a-649">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="b588a-650">defenderEmailContentExecution</span><span class="sxs-lookup"><span data-stu-id="b588a-650">defenderEmailContentExecution</span></span>|[<span data-ttu-id="b588a-651">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="b588a-651">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="b588a-652">指示是否应该从电子邮件 （客户端 webmail/邮件） 放执行 （exe、 dll，ps、 js、 vbs 等） 的可执行内容的值。</span><span class="sxs-lookup"><span data-stu-id="b588a-652">Value indicating if execution of executable content (exe, dll, ps, js, vbs, etc) should be dropped from email (webmail/mail-client).</span></span> <span data-ttu-id="b588a-653">可取值为：`userDefined`、`enable`、`auditMode`。</span><span class="sxs-lookup"><span data-stu-id="b588a-653">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="b588a-654">defenderAdvancedRansomewareProtectionType</span><span class="sxs-lookup"><span data-stu-id="b588a-654">defenderAdvancedRansomewareProtectionType</span></span>|[<span data-ttu-id="b588a-655">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="b588a-655">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="b588a-656">指示使用高级防范 ransomeware 值。</span><span class="sxs-lookup"><span data-stu-id="b588a-656">Value indicating use of advanced protection against ransomeware.</span></span> <span data-ttu-id="b588a-657">可取值为：`userDefined`、`enable`、`auditMode`。</span><span class="sxs-lookup"><span data-stu-id="b588a-657">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="b588a-658">defenderGuardMyFoldersType</span><span class="sxs-lookup"><span data-stu-id="b588a-658">defenderGuardMyFoldersType</span></span>|[<span data-ttu-id="b588a-659">folderProtectionType</span><span class="sxs-lookup"><span data-stu-id="b588a-659">folderProtectionType</span></span>](../resources/intune-deviceconfig-folderprotectiontype.md)|<span data-ttu-id="b588a-660">指示受保护的文件夹的行为的值。</span><span class="sxs-lookup"><span data-stu-id="b588a-660">Value indicating the behavior of protected folders.</span></span> <span data-ttu-id="b588a-661">可取值为：`userDefined`、`enable`、`auditMode`、`blockDiskModification`、`auditDiskModification`。</span><span class="sxs-lookup"><span data-stu-id="b588a-661">Possible values are: `userDefined`, `enable`, `auditMode`, `blockDiskModification`, `auditDiskModification`.</span></span>|
|<span data-ttu-id="b588a-662">defenderGuardedFoldersAllowedAppPaths</span><span class="sxs-lookup"><span data-stu-id="b588a-662">defenderGuardedFoldersAllowedAppPaths</span></span>|<span data-ttu-id="b588a-663">String 集合</span><span class="sxs-lookup"><span data-stu-id="b588a-663">String collection</span></span>|<span data-ttu-id="b588a-664">允许访问受保护文件夹的 exe 路径列表</span><span class="sxs-lookup"><span data-stu-id="b588a-664">List of paths to exe that are allowed to access protected folders</span></span>|
|<span data-ttu-id="b588a-665">defenderAdditionalGuardedFolders</span><span class="sxs-lookup"><span data-stu-id="b588a-665">defenderAdditionalGuardedFolders</span></span>|<span data-ttu-id="b588a-666">String 集合</span><span class="sxs-lookup"><span data-stu-id="b588a-666">String collection</span></span>|<span data-ttu-id="b588a-667">要添加到受保护文件夹列表的文件夹路径列表</span><span class="sxs-lookup"><span data-stu-id="b588a-667">List of folder paths to be added to the list of protected folders</span></span>|
|<span data-ttu-id="b588a-668">defenderNetworkProtectionType</span><span class="sxs-lookup"><span data-stu-id="b588a-668">defenderNetworkProtectionType</span></span>|[<span data-ttu-id="b588a-669">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="b588a-669">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="b588a-670">指示 NetworkProtection 的行为的值。</span><span class="sxs-lookup"><span data-stu-id="b588a-670">Value indicating the behavior of NetworkProtection.</span></span> <span data-ttu-id="b588a-671">可取值为：`userDefined`、`enable`、`auditMode`。</span><span class="sxs-lookup"><span data-stu-id="b588a-671">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="b588a-672">defenderExploitProtectionXml</span><span class="sxs-lookup"><span data-stu-id="b588a-672">defenderExploitProtectionXml</span></span>|<span data-ttu-id="b588a-673">Binary</span><span class="sxs-lookup"><span data-stu-id="b588a-673">Binary</span></span>|<span data-ttu-id="b588a-674">包含有关 Exploit Protection 详细信息的 xml 内容。</span><span class="sxs-lookup"><span data-stu-id="b588a-674">Xml content containing information regarding exploit protection details.</span></span>|
|<span data-ttu-id="b588a-675">defenderExploitProtectionXmlFileName</span><span class="sxs-lookup"><span data-stu-id="b588a-675">defenderExploitProtectionXmlFileName</span></span>|<span data-ttu-id="b588a-676">String</span><span class="sxs-lookup"><span data-stu-id="b588a-676">String</span></span>|<span data-ttu-id="b588a-677">从中获取 DefenderExploitProtectionXml 的文件的名称。</span><span class="sxs-lookup"><span data-stu-id="b588a-677">Name of the file from which DefenderExploitProtectionXml was obtained.</span></span>|
|<span data-ttu-id="b588a-678">defenderSecurityCenterBlockExploitProtectionOverride</span><span class="sxs-lookup"><span data-stu-id="b588a-678">defenderSecurityCenterBlockExploitProtectionOverride</span></span>|<span data-ttu-id="b588a-679">Boolean</span><span class="sxs-lookup"><span data-stu-id="b588a-679">Boolean</span></span>|<span data-ttu-id="b588a-680">指示是否阻止用户覆盖 Exploit Protection 设置。</span><span class="sxs-lookup"><span data-stu-id="b588a-680">Indicates whether or not to block user from overriding Exploit Protection settings.</span></span>|
|<span data-ttu-id="b588a-681">appLockerApplicationControl</span><span class="sxs-lookup"><span data-stu-id="b588a-681">appLockerApplicationControl</span></span>|[<span data-ttu-id="b588a-682">appLockerApplicationControlType</span><span class="sxs-lookup"><span data-stu-id="b588a-682">appLockerApplicationControlType</span></span>](../resources/intune-deviceconfig-applockerapplicationcontroltype.md)|<span data-ttu-id="b588a-683">使管理员能够选择在设备上允许哪些类型的应用。</span><span class="sxs-lookup"><span data-stu-id="b588a-683">Enables the Admin to choose what types of app to allow on devices.</span></span> <span data-ttu-id="b588a-684">可取值为：`notConfigured`、`enforceComponentsAndStoreApps`、`auditComponentsAndStoreApps`、`enforceComponentsStoreAppsAndSmartlocker`、`auditComponentsStoreAppsAndSmartlocker`。</span><span class="sxs-lookup"><span data-stu-id="b588a-684">Possible values are: `notConfigured`, `enforceComponentsAndStoreApps`, `auditComponentsAndStoreApps`, `enforceComponentsStoreAppsAndSmartlocker`, `auditComponentsStoreAppsAndSmartlocker`.</span></span>|
|<span data-ttu-id="b588a-685">deviceGuardLocalSystemAuthorityCredentialGuardSettings</span><span class="sxs-lookup"><span data-stu-id="b588a-685">deviceGuardLocalSystemAuthorityCredentialGuardSettings</span></span>|[<span data-ttu-id="b588a-686">deviceGuardLocalSystemAuthorityCredentialGuardType</span><span class="sxs-lookup"><span data-stu-id="b588a-686">deviceGuardLocalSystemAuthorityCredentialGuardType</span></span>](../resources/intune-deviceconfig-deviceguardlocalsystemauthoritycredentialguardtype.md)|<span data-ttu-id="b588a-687">在凭据 Guard 时同时启用对安全启动和虚拟化基于安全平台安全级别打开。</span><span class="sxs-lookup"><span data-stu-id="b588a-687">Turn on Credential Guard when Platform Security Level with Secure Boot and Virtualization Based Security are both enabled.</span></span> <span data-ttu-id="b588a-688">可取值为：`notConfigured`、`enableWithUEFILock`、`enableWithoutUEFILock`。</span><span class="sxs-lookup"><span data-stu-id="b588a-688">Possible values are: `notConfigured`, `enableWithUEFILock`, `enableWithoutUEFILock`.</span></span>|
|<span data-ttu-id="b588a-689">deviceGuardEnableVirtualizationBasedSecurity</span><span class="sxs-lookup"><span data-stu-id="b588a-689">deviceGuardEnableVirtualizationBasedSecurity</span></span>|<span data-ttu-id="b588a-690">布尔</span><span class="sxs-lookup"><span data-stu-id="b588a-690">Boolean</span></span>|<span data-ttu-id="b588a-691">虚拟化选项会启用基于 Security(VBS)。</span><span class="sxs-lookup"><span data-stu-id="b588a-691">Turns On Virtualization Based Security(VBS).</span></span>|
|<span data-ttu-id="b588a-692">deviceGuardEnableSecureBootWithDMA</span><span class="sxs-lookup"><span data-stu-id="b588a-692">deviceGuardEnableSecureBootWithDMA</span></span>|<span data-ttu-id="b588a-693">布尔</span><span class="sxs-lookup"><span data-stu-id="b588a-693">Boolean</span></span>|<span data-ttu-id="b588a-694">指定是否将在下次重新启动启用平台安全级别。</span><span class="sxs-lookup"><span data-stu-id="b588a-694">Specifies whether Platform Security Level is enabled at next reboot.</span></span>|
|<span data-ttu-id="b588a-695">smartScreenEnableInShell</span><span class="sxs-lookup"><span data-stu-id="b588a-695">smartScreenEnableInShell</span></span>|<span data-ttu-id="b588a-696">Boolean</span><span class="sxs-lookup"><span data-stu-id="b588a-696">Boolean</span></span>|<span data-ttu-id="b588a-697">允许 IT 管理员配置适用于 Windows 的 SmartScreen。</span><span class="sxs-lookup"><span data-stu-id="b588a-697">Allows IT Admins to configure SmartScreen for Windows.</span></span>|
|<span data-ttu-id="b588a-698">smartScreenBlockOverrideForFiles</span><span class="sxs-lookup"><span data-stu-id="b588a-698">smartScreenBlockOverrideForFiles</span></span>|<span data-ttu-id="b588a-699">Boolean</span><span class="sxs-lookup"><span data-stu-id="b588a-699">Boolean</span></span>|<span data-ttu-id="b588a-700">允许 IT 管理员控制用户是否可以忽略 SmartScreen 警告并运行恶意文件。</span><span class="sxs-lookup"><span data-stu-id="b588a-700">Allows IT Admins to control whether users can can ignore SmartScreen warnings and run malicious files.</span></span>|
|<span data-ttu-id="b588a-701">applicationGuardEnabled</span><span class="sxs-lookup"><span data-stu-id="b588a-701">applicationGuardEnabled</span></span>|<span data-ttu-id="b588a-702">Boolean</span><span class="sxs-lookup"><span data-stu-id="b588a-702">Boolean</span></span>|<span data-ttu-id="b588a-703">启用 Windows Defender 应用程序防护</span><span class="sxs-lookup"><span data-stu-id="b588a-703">Enable Windows Defender Application Guard</span></span>|
|<span data-ttu-id="b588a-704">applicationGuardEnabledOptions</span><span class="sxs-lookup"><span data-stu-id="b588a-704">applicationGuardEnabledOptions</span></span>|[<span data-ttu-id="b588a-705">applicationGuardEnabledOptions</span><span class="sxs-lookup"><span data-stu-id="b588a-705">applicationGuardEnabledOptions</span></span>](../resources/intune-deviceconfig-applicationguardenabledoptions.md)|<span data-ttu-id="b588a-706">Windows Defender 应用程序 Guard 启用更高版本的 Windows 版本。</span><span class="sxs-lookup"><span data-stu-id="b588a-706">Enable Windows Defender Application Guard for newer Windows builds.</span></span> <span data-ttu-id="b588a-707">可取值为：`notConfigured`、`enabledForEdge`、`enabledForOffice`、`enabledForEdgeAndOffice`。</span><span class="sxs-lookup"><span data-stu-id="b588a-707">Possible values are: `notConfigured`, `enabledForEdge`, `enabledForOffice`, `enabledForEdgeAndOffice`.</span></span>|
|<span data-ttu-id="b588a-708">applicationGuardBlockFileTransfer</span><span class="sxs-lookup"><span data-stu-id="b588a-708">applicationGuardBlockFileTransfer</span></span>|[<span data-ttu-id="b588a-709">applicationGuardBlockFileTransferType</span><span class="sxs-lookup"><span data-stu-id="b588a-709">applicationGuardBlockFileTransferType</span></span>](../resources/intune-deviceconfig-applicationguardblockfiletransfertype.md)|<span data-ttu-id="b588a-710">阻止传输图像文件、 文本文件或两者到剪贴板。</span><span class="sxs-lookup"><span data-stu-id="b588a-710">Block clipboard to transfer image file, text file or neither of them.</span></span> <span data-ttu-id="b588a-711">可取值为：`notConfigured`、`blockImageAndTextFile`、`blockImageFile`、`blockNone`、`blockTextFile`。</span><span class="sxs-lookup"><span data-stu-id="b588a-711">Possible values are: `notConfigured`, `blockImageAndTextFile`, `blockImageFile`, `blockNone`, `blockTextFile`.</span></span>|
|<span data-ttu-id="b588a-712">applicationGuardBlockNonEnterpriseContent</span><span class="sxs-lookup"><span data-stu-id="b588a-712">applicationGuardBlockNonEnterpriseContent</span></span>|<span data-ttu-id="b588a-713">Boolean</span><span class="sxs-lookup"><span data-stu-id="b588a-713">Boolean</span></span>|<span data-ttu-id="b588a-714">阻止企业站点加载非企业内容，例如第三方插件</span><span class="sxs-lookup"><span data-stu-id="b588a-714">Block enterprise sites to load non-enterprise content, such as third party plug-ins</span></span>|
|<span data-ttu-id="b588a-715">applicationGuardAllowPersistence</span><span class="sxs-lookup"><span data-stu-id="b588a-715">applicationGuardAllowPersistence</span></span>|<span data-ttu-id="b588a-716">Boolean</span><span class="sxs-lookup"><span data-stu-id="b588a-716">Boolean</span></span>|<span data-ttu-id="b588a-717">允许 App Guard 容器（收藏夹、Cookie、Web 密码等）内的持久用户生成数据</span><span class="sxs-lookup"><span data-stu-id="b588a-717">Allow persisting user generated data inside the App Guard Containter (favorites, cookies, web passwords, etc.)</span></span>|
|<span data-ttu-id="b588a-718">applicationGuardForceAuditing</span><span class="sxs-lookup"><span data-stu-id="b588a-718">applicationGuardForceAuditing</span></span>|<span data-ttu-id="b588a-719">Boolean</span><span class="sxs-lookup"><span data-stu-id="b588a-719">Boolean</span></span>|<span data-ttu-id="b588a-720">强制审核将存留 Windows 日志和事件以满足安全/符合性条件（示例事件是用户登录注销、特权使用、软件安装、系统更改等）</span><span class="sxs-lookup"><span data-stu-id="b588a-720">Force auditing will persist Windows logs and events to meet security/compliance criteria (sample events are user login-logoff, use of privilege rights, software installation, system changes, etc.)</span></span>|
|<span data-ttu-id="b588a-721">applicationGuardBlockClipboardSharing</span><span class="sxs-lookup"><span data-stu-id="b588a-721">applicationGuardBlockClipboardSharing</span></span>|[<span data-ttu-id="b588a-722">applicationGuardBlockClipboardSharingType</span><span class="sxs-lookup"><span data-stu-id="b588a-722">applicationGuardBlockClipboardSharingType</span></span>](../resources/intune-deviceconfig-applicationguardblockclipboardsharingtype.md)|<span data-ttu-id="b588a-723">阻止剪贴板将数据从主机共享到容器或从容器共享到主机，或阻止两种方式，或两种方式均不阻止。</span><span class="sxs-lookup"><span data-stu-id="b588a-723">Block clipboard to share data from Host to Container, or from Container to Host, or both ways, or neither ways.</span></span> <span data-ttu-id="b588a-724">可取值为：`notConfigured`、`blockBoth`、`blockHostToContainer`、`blockContainerToHost`、`blockNone`。</span><span class="sxs-lookup"><span data-stu-id="b588a-724">Possible values are: `notConfigured`, `blockBoth`, `blockHostToContainer`, `blockContainerToHost`, `blockNone`.</span></span>|
|<span data-ttu-id="b588a-725">applicationGuardAllowPrintToPDF</span><span class="sxs-lookup"><span data-stu-id="b588a-725">applicationGuardAllowPrintToPDF</span></span>|<span data-ttu-id="b588a-726">Boolean</span><span class="sxs-lookup"><span data-stu-id="b588a-726">Boolean</span></span>|<span data-ttu-id="b588a-727">允许从容器打印为 PDF 格式</span><span class="sxs-lookup"><span data-stu-id="b588a-727">Allow printing to PDF from Container</span></span>|
|<span data-ttu-id="b588a-728">applicationGuardAllowPrintToXPS</span><span class="sxs-lookup"><span data-stu-id="b588a-728">applicationGuardAllowPrintToXPS</span></span>|<span data-ttu-id="b588a-729">Boolean</span><span class="sxs-lookup"><span data-stu-id="b588a-729">Boolean</span></span>|<span data-ttu-id="b588a-730">允许从容器打印为 XPS 格式</span><span class="sxs-lookup"><span data-stu-id="b588a-730">Allow printing to XPS from Container</span></span>|
|<span data-ttu-id="b588a-731">applicationGuardAllowPrintToLocalPrinters</span><span class="sxs-lookup"><span data-stu-id="b588a-731">applicationGuardAllowPrintToLocalPrinters</span></span>|<span data-ttu-id="b588a-732">Boolean</span><span class="sxs-lookup"><span data-stu-id="b588a-732">Boolean</span></span>|<span data-ttu-id="b588a-733">允许从容器打印到本地打印机</span><span class="sxs-lookup"><span data-stu-id="b588a-733">Allow printing to Local Printers from Container</span></span>|
|<span data-ttu-id="b588a-734">applicationGuardAllowPrintToNetworkPrinters</span><span class="sxs-lookup"><span data-stu-id="b588a-734">applicationGuardAllowPrintToNetworkPrinters</span></span>|<span data-ttu-id="b588a-735">Boolean</span><span class="sxs-lookup"><span data-stu-id="b588a-735">Boolean</span></span>|<span data-ttu-id="b588a-736">允许从容器打印到网络打印机</span><span class="sxs-lookup"><span data-stu-id="b588a-736">Allow printing to Network Printers from Container</span></span>|
|<span data-ttu-id="b588a-737">applicationGuardAllowVirtualGPU</span><span class="sxs-lookup"><span data-stu-id="b588a-737">applicationGuardAllowVirtualGPU</span></span>|<span data-ttu-id="b588a-738">布尔</span><span class="sxs-lookup"><span data-stu-id="b588a-738">Boolean</span></span>|<span data-ttu-id="b588a-739">允许应用程序 guard 用于虚拟 GPU</span><span class="sxs-lookup"><span data-stu-id="b588a-739">Allow application guard to use virtual GPU</span></span>|
|<span data-ttu-id="b588a-740">applicationGuardAllowFileSaveOnHost</span><span class="sxs-lookup"><span data-stu-id="b588a-740">applicationGuardAllowFileSaveOnHost</span></span>|<span data-ttu-id="b588a-741">布尔</span><span class="sxs-lookup"><span data-stu-id="b588a-741">Boolean</span></span>|<span data-ttu-id="b588a-742">允许用户从应用程序 guard 容器中的边缘下载文件并将其保存在主机上文件系统</span><span class="sxs-lookup"><span data-stu-id="b588a-742">Allow users to download files from Edge in the application guard container and save them on the host file system</span></span>|
|<span data-ttu-id="b588a-743">bitLockerDisableWarningForOtherDiskEncryption</span><span class="sxs-lookup"><span data-stu-id="b588a-743">bitLockerDisableWarningForOtherDiskEncryption</span></span>|<span data-ttu-id="b588a-744">Boolean</span><span class="sxs-lookup"><span data-stu-id="b588a-744">Boolean</span></span>|<span data-ttu-id="b588a-745">允许管理员禁用对用户计算机上其他磁盘加密的警告提示。</span><span class="sxs-lookup"><span data-stu-id="b588a-745">Allows the Admin to disable the warning prompt for other disk encryption on the user machines.</span></span>|
|<span data-ttu-id="b588a-746">bitLockerEnableStorageCardEncryptionOnMobile</span><span class="sxs-lookup"><span data-stu-id="b588a-746">bitLockerEnableStorageCardEncryptionOnMobile</span></span>|<span data-ttu-id="b588a-747">Boolean</span><span class="sxs-lookup"><span data-stu-id="b588a-747">Boolean</span></span>|<span data-ttu-id="b588a-748">允许管理员要求使用 BitLocker 开启加密功能。</span><span class="sxs-lookup"><span data-stu-id="b588a-748">Allows the admin to require encryption to be turned on using BitLocker.</span></span> <span data-ttu-id="b588a-749">此策略仅适用于移动 SKU。</span><span class="sxs-lookup"><span data-stu-id="b588a-749">This policy is valid only for a mobile SKU.</span></span>|
|<span data-ttu-id="b588a-750">bitLockerEncryptDevice</span><span class="sxs-lookup"><span data-stu-id="b588a-750">bitLockerEncryptDevice</span></span>|<span data-ttu-id="b588a-751">Boolean</span><span class="sxs-lookup"><span data-stu-id="b588a-751">Boolean</span></span>|<span data-ttu-id="b588a-752">允许管理员要求使用 BitLocker 开启加密功能。</span><span class="sxs-lookup"><span data-stu-id="b588a-752">Allows the admin to require encryption to be turned on using BitLocker.</span></span>|
|<span data-ttu-id="b588a-753">bitLockerSystemDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="b588a-753">bitLockerSystemDrivePolicy</span></span>|[<span data-ttu-id="b588a-754">bitLockerSystemDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="b588a-754">bitLockerSystemDrivePolicy</span></span>](../resources/intune-deviceconfig-bitlockersystemdrivepolicy.md)|<span data-ttu-id="b588a-755">BitLocker 系统驱动器策略。</span><span class="sxs-lookup"><span data-stu-id="b588a-755">BitLocker System Drive Policy.</span></span>|
|<span data-ttu-id="b588a-756">bitLockerFixedDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="b588a-756">bitLockerFixedDrivePolicy</span></span>|[<span data-ttu-id="b588a-757">bitLockerFixedDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="b588a-757">bitLockerFixedDrivePolicy</span></span>](../resources/intune-deviceconfig-bitlockerfixeddrivepolicy.md)|<span data-ttu-id="b588a-758">BitLocker 固定驱动器策略。</span><span class="sxs-lookup"><span data-stu-id="b588a-758">BitLocker Fixed Drive Policy.</span></span>|
|<span data-ttu-id="b588a-759">bitLockerRemovableDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="b588a-759">bitLockerRemovableDrivePolicy</span></span>|[<span data-ttu-id="b588a-760">bitLockerRemovableDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="b588a-760">bitLockerRemovableDrivePolicy</span></span>](../resources/intune-deviceconfig-bitlockerremovabledrivepolicy.md)|<span data-ttu-id="b588a-761">BitLocker 可移动驱动器策略。</span><span class="sxs-lookup"><span data-stu-id="b588a-761">BitLocker Removable Drive Policy.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b588a-762">关系</span><span class="sxs-lookup"><span data-stu-id="b588a-762">Relationships</span></span>
|<span data-ttu-id="b588a-763">关系</span><span class="sxs-lookup"><span data-stu-id="b588a-763">Relationship</span></span>|<span data-ttu-id="b588a-764">类型</span><span class="sxs-lookup"><span data-stu-id="b588a-764">Type</span></span>|<span data-ttu-id="b588a-765">说明</span><span class="sxs-lookup"><span data-stu-id="b588a-765">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b588a-766">groupAssignments</span><span class="sxs-lookup"><span data-stu-id="b588a-766">groupAssignments</span></span>|<span data-ttu-id="b588a-767">[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)集合</span><span class="sxs-lookup"><span data-stu-id="b588a-767">[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) collection</span></span>|<span data-ttu-id="b588a-768">设备配置文件的组分配列表。</span><span class="sxs-lookup"><span data-stu-id="b588a-768">The list of group assignments for the device configuration profile.</span></span> <span data-ttu-id="b588a-769">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b588a-769">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b588a-770">assignments</span><span class="sxs-lookup"><span data-stu-id="b588a-770">assignments</span></span>|<span data-ttu-id="b588a-771">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="b588a-771">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection</span></span>|<span data-ttu-id="b588a-772">设备配置文件的分配列表。</span><span class="sxs-lookup"><span data-stu-id="b588a-772">The list of assignments for the device configuration profile.</span></span> <span data-ttu-id="b588a-773">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b588a-773">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b588a-774">deviceStatuses</span><span class="sxs-lookup"><span data-stu-id="b588a-774">deviceStatuses</span></span>|<span data-ttu-id="b588a-775">[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) 集合</span><span class="sxs-lookup"><span data-stu-id="b588a-775">[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) collection</span></span>|<span data-ttu-id="b588a-776">按设备的设备配置安装状态。</span><span class="sxs-lookup"><span data-stu-id="b588a-776">Device configuration installation status by device.</span></span> <span data-ttu-id="b588a-777">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b588a-777">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b588a-778">userStatuses</span><span class="sxs-lookup"><span data-stu-id="b588a-778">userStatuses</span></span>|<span data-ttu-id="b588a-779">[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) 集合</span><span class="sxs-lookup"><span data-stu-id="b588a-779">[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) collection</span></span>|<span data-ttu-id="b588a-780">用户的设备配置安装状态。</span><span class="sxs-lookup"><span data-stu-id="b588a-780">Device configuration installation status by user.</span></span> <span data-ttu-id="b588a-781">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b588a-781">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b588a-782">deviceStatusOverview</span><span class="sxs-lookup"><span data-stu-id="b588a-782">deviceStatusOverview</span></span>|[<span data-ttu-id="b588a-783">deviceConfigurationDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="b588a-783">deviceConfigurationDeviceOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|<span data-ttu-id="b588a-784">设备配置设备状态概述 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b588a-784">Device Configuration devices status overview Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b588a-785">userStatusOverview</span><span class="sxs-lookup"><span data-stu-id="b588a-785">userStatusOverview</span></span>|[<span data-ttu-id="b588a-786">deviceConfigurationUserOverview</span><span class="sxs-lookup"><span data-stu-id="b588a-786">deviceConfigurationUserOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|<span data-ttu-id="b588a-787">设备配置用户状态概述 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b588a-787">Device Configuration users status overview Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b588a-788">deviceSettingStateSummaries</span><span class="sxs-lookup"><span data-stu-id="b588a-788">deviceSettingStateSummaries</span></span>|<span data-ttu-id="b588a-789">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) 集合</span><span class="sxs-lookup"><span data-stu-id="b588a-789">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) collection</span></span>|<span data-ttu-id="b588a-790">设备配置设置状态设备摘要 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b588a-790">Device Configuration Setting State Device Summary Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b588a-791">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b588a-791">JSON Representation</span></span>
<span data-ttu-id="b588a-792">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b588a-792">Here is a JSON representation of the resource.</span></span>
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
  "localSecurityOptionsEnableAdministratorAccount": true,
  "localSecurityOptionsAdministratorAccountName": "String",
  "localSecurityOptionsEnableGuestAccount": true,
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
  "lanManagerWorkstationEnableInsecureGuestLogons": true,
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





