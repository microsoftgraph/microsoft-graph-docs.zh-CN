---
title: 更新 windows10EndpointProtectionConfiguration
description: 更新 windows10EndpointProtectionConfiguration 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 36d71a14900d3400874ac39bd1fa59c534208676
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27983028"
---
# <a name="update-windows10endpointprotectionconfiguration"></a><span data-ttu-id="6e0e5-103">更新 windows10EndpointProtectionConfiguration</span><span class="sxs-lookup"><span data-stu-id="6e0e5-103">Update windows10EndpointProtectionConfiguration</span></span>

> <span data-ttu-id="6e0e5-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="6e0e5-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6e0e5-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="6e0e5-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="6e0e5-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="6e0e5-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6e0e5-107">更新 [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="6e0e5-107">Update the properties of a [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="6e0e5-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="6e0e5-108">Prerequisites</span></span>
<span data-ttu-id="6e0e5-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="6e0e5-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6e0e5-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="6e0e5-111">Permission type</span></span>|<span data-ttu-id="6e0e5-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="6e0e5-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6e0e5-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6e0e5-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6e0e5-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6e0e5-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="6e0e5-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6e0e5-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6e0e5-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="6e0e5-116">Not supported.</span></span>|
|<span data-ttu-id="6e0e5-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="6e0e5-117">Application</span></span>|<span data-ttu-id="6e0e5-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="6e0e5-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6e0e5-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6e0e5-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="6e0e5-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="6e0e5-120">Request headers</span></span>
|<span data-ttu-id="6e0e5-121">标头</span><span class="sxs-lookup"><span data-stu-id="6e0e5-121">Header</span></span>|<span data-ttu-id="6e0e5-122">值</span><span class="sxs-lookup"><span data-stu-id="6e0e5-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6e0e5-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="6e0e5-123">Authorization</span></span>|<span data-ttu-id="6e0e5-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="6e0e5-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6e0e5-125">Accept</span><span class="sxs-lookup"><span data-stu-id="6e0e5-125">Accept</span></span>|<span data-ttu-id="6e0e5-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6e0e5-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6e0e5-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="6e0e5-127">Request body</span></span>
<span data-ttu-id="6e0e5-128">在请求正文中，提供 [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6e0e5-128">In the request body, supply a JSON representation for the [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) object.</span></span>

<span data-ttu-id="6e0e5-129">下表显示了创建 [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="6e0e5-129">The following table shows the properties that are required when you create the [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md).</span></span>

|<span data-ttu-id="6e0e5-130">属性</span><span class="sxs-lookup"><span data-stu-id="6e0e5-130">Property</span></span>|<span data-ttu-id="6e0e5-131">类型</span><span class="sxs-lookup"><span data-stu-id="6e0e5-131">Type</span></span>|<span data-ttu-id="6e0e5-132">说明</span><span class="sxs-lookup"><span data-stu-id="6e0e5-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6e0e5-133">id</span><span class="sxs-lookup"><span data-stu-id="6e0e5-133">id</span></span>|<span data-ttu-id="6e0e5-134">String</span><span class="sxs-lookup"><span data-stu-id="6e0e5-134">String</span></span>|<span data-ttu-id="6e0e5-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="6e0e5-135">Key of the entity.</span></span> <span data-ttu-id="6e0e5-136">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6e0e5-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6e0e5-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6e0e5-137">lastModifiedDateTime</span></span>|<span data-ttu-id="6e0e5-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6e0e5-138">DateTimeOffset</span></span>|<span data-ttu-id="6e0e5-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="6e0e5-139">DateTime the object was last modified.</span></span> <span data-ttu-id="6e0e5-140">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6e0e5-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6e0e5-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="6e0e5-141">roleScopeTagIds</span></span>|<span data-ttu-id="6e0e5-142">String 集合</span><span class="sxs-lookup"><span data-stu-id="6e0e5-142">String collection</span></span>|<span data-ttu-id="6e0e5-143">此实体实例范围标记的列表。</span><span class="sxs-lookup"><span data-stu-id="6e0e5-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="6e0e5-144">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6e0e5-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6e0e5-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="6e0e5-145">supportsScopeTags</span></span>|<span data-ttu-id="6e0e5-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="6e0e5-146">Boolean</span></span>|<span data-ttu-id="6e0e5-147">指示基础的设备配置支持分配的范围标记。</span><span class="sxs-lookup"><span data-stu-id="6e0e5-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="6e0e5-148">此值为 false，并且实体将不会对作用域的用户可见时，不允许将分配给 ScopeTags 属性。</span><span class="sxs-lookup"><span data-stu-id="6e0e5-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="6e0e5-149">这将发生在 Silverlight 中创建的旧策略，并可以解析通过删除并重新创建 Azure 门户中的策略。</span><span class="sxs-lookup"><span data-stu-id="6e0e5-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="6e0e5-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="6e0e5-150">This property is read-only.</span></span> <span data-ttu-id="6e0e5-151">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6e0e5-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6e0e5-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6e0e5-152">createdDateTime</span></span>|<span data-ttu-id="6e0e5-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6e0e5-153">DateTimeOffset</span></span>|<span data-ttu-id="6e0e5-154">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="6e0e5-154">DateTime the object was created.</span></span> <span data-ttu-id="6e0e5-155">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6e0e5-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6e0e5-156">description</span><span class="sxs-lookup"><span data-stu-id="6e0e5-156">description</span></span>|<span data-ttu-id="6e0e5-157">String</span><span class="sxs-lookup"><span data-stu-id="6e0e5-157">String</span></span>|<span data-ttu-id="6e0e5-158">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="6e0e5-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="6e0e5-159">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6e0e5-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6e0e5-160">displayName</span><span class="sxs-lookup"><span data-stu-id="6e0e5-160">displayName</span></span>|<span data-ttu-id="6e0e5-161">String</span><span class="sxs-lookup"><span data-stu-id="6e0e5-161">String</span></span>|<span data-ttu-id="6e0e5-162">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="6e0e5-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="6e0e5-163">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6e0e5-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6e0e5-164">version</span><span class="sxs-lookup"><span data-stu-id="6e0e5-164">version</span></span>|<span data-ttu-id="6e0e5-165">Int32</span><span class="sxs-lookup"><span data-stu-id="6e0e5-165">Int32</span></span>|<span data-ttu-id="6e0e5-166">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="6e0e5-166">Version of the device configuration.</span></span> <span data-ttu-id="6e0e5-167">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6e0e5-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6e0e5-168">userRightsAccessCredentialManagerAsTrustedCaller</span><span class="sxs-lookup"><span data-stu-id="6e0e5-168">userRightsAccessCredentialManagerAsTrustedCaller</span></span>|[<span data-ttu-id="6e0e5-169">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="6e0e5-169">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="6e0e5-170">此用户权限备份/还原过程中使用的凭据管理器中。</span><span class="sxs-lookup"><span data-stu-id="6e0e5-170">This user right is used by Credential Manager during Backup/Restore.</span></span> <span data-ttu-id="6e0e5-171">用户的已保存的凭据可能受到威胁，如果此权限授予的其他实体。</span><span class="sxs-lookup"><span data-stu-id="6e0e5-171">Users' saved credentials might be compromised if this privilege is given to other entities.</span></span> <span data-ttu-id="6e0e5-172">支持状态 NotConfigured 和允许</span><span class="sxs-lookup"><span data-stu-id="6e0e5-172">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="6e0e5-173">userRightsAllowAccessFromNetwork</span><span class="sxs-lookup"><span data-stu-id="6e0e5-173">userRightsAllowAccessFromNetwork</span></span>|[<span data-ttu-id="6e0e5-174">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="6e0e5-174">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="6e0e5-175">此用户权限确定哪些用户和组允许通过网络连接到计算机。</span><span class="sxs-lookup"><span data-stu-id="6e0e5-175">This user right determines which users and groups are allowed to connect to the computer over the network.</span></span> <span data-ttu-id="6e0e5-176">支持状态允许。</span><span class="sxs-lookup"><span data-stu-id="6e0e5-176">State Allowed is supported.</span></span>|
|<span data-ttu-id="6e0e5-177">userRightsBlockAccessFromNetwork</span><span class="sxs-lookup"><span data-stu-id="6e0e5-177">userRightsBlockAccessFromNetwork</span></span>|[<span data-ttu-id="6e0e5-178">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="6e0e5-178">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="6e0e5-179">此用户权限确定哪些用户和组是通过网络连接到计算机的块。</span><span class="sxs-lookup"><span data-stu-id="6e0e5-179">This user right determines which users and groups are block from connecting to the computer over the network.</span></span> <span data-ttu-id="6e0e5-180">支持状态块。</span><span class="sxs-lookup"><span data-stu-id="6e0e5-180">State Block is supported.</span></span>|
|<span data-ttu-id="6e0e5-181">userRightsActAsPartOfTheOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="6e0e5-181">userRightsActAsPartOfTheOperatingSystem</span></span>|[<span data-ttu-id="6e0e5-182">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="6e0e5-182">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="6e0e5-183">此用户权限允许模拟任何用户无需身份验证的过程。</span><span class="sxs-lookup"><span data-stu-id="6e0e5-183">This user right allows a process to impersonate any user without authentication.</span></span> <span data-ttu-id="6e0e5-184">过程因此可以访问与该用户相同的本地资源。</span><span class="sxs-lookup"><span data-stu-id="6e0e5-184">The process can therefore gain access to the same local resources as that user.</span></span> <span data-ttu-id="6e0e5-185">支持状态 NotConfigured 和允许</span><span class="sxs-lookup"><span data-stu-id="6e0e5-185">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="6e0e5-186">userRightsLocalLogOn</span><span class="sxs-lookup"><span data-stu-id="6e0e5-186">userRightsLocalLogOn</span></span>|[<span data-ttu-id="6e0e5-187">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="6e0e5-187">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="6e0e5-188">此用户权限确定哪些用户可以登录到计算机。</span><span class="sxs-lookup"><span data-stu-id="6e0e5-188">This user right determines which users can log on to the computer.</span></span> <span data-ttu-id="6e0e5-189">状态 NotConfigured、 允许和已阻止所有支持</span><span class="sxs-lookup"><span data-stu-id="6e0e5-189">States NotConfigured, Allowed and Blocked are all supported</span></span> |
|<span data-ttu-id="6e0e5-190">userRightsBackupData</span><span class="sxs-lookup"><span data-stu-id="6e0e5-190">userRightsBackupData</span></span>|[<span data-ttu-id="6e0e5-191">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="6e0e5-191">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="6e0e5-192">此用户权限确定哪些用户可以跳过文件、 目录、 注册表和其他永久对象权限时备份文件和目录。</span><span class="sxs-lookup"><span data-stu-id="6e0e5-192">This user right determines which users can bypass file, directory, registry, and other persistent objects permissions when backing up files and directories.</span></span> <span data-ttu-id="6e0e5-193">支持状态 NotConfigured 和允许</span><span class="sxs-lookup"><span data-stu-id="6e0e5-193">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="6e0e5-194">userRightsChangeSystemTime</span><span class="sxs-lookup"><span data-stu-id="6e0e5-194">userRightsChangeSystemTime</span></span>|[<span data-ttu-id="6e0e5-195">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="6e0e5-195">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="6e0e5-196">此用户权限确定哪些用户和组可以更改计算机内部时钟的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="6e0e5-196">This user right determines which users and groups can change the time and date on the internal clock of the computer.</span></span> <span data-ttu-id="6e0e5-197">支持状态 NotConfigured 和允许</span><span class="sxs-lookup"><span data-stu-id="6e0e5-197">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="6e0e5-198">userRightsCreateGlobalObjects</span><span class="sxs-lookup"><span data-stu-id="6e0e5-198">userRightsCreateGlobalObjects</span></span>|[<span data-ttu-id="6e0e5-199">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="6e0e5-199">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="6e0e5-200">此安全设置确定用户是否可以创建可供所有会话的全局对象。</span><span class="sxs-lookup"><span data-stu-id="6e0e5-200">This security setting determines whether users can create global objects that are available to all sessions.</span></span> <span data-ttu-id="6e0e5-201">可以创建全局对象的用户可能会影响其他用户的会话，这可能导致应用程序故障或数据损坏下运行的进程。</span><span class="sxs-lookup"><span data-stu-id="6e0e5-201">Users who can create global objects could affect processes that run under other users' sessions, which could lead to application failure or data corruption.</span></span> <span data-ttu-id="6e0e5-202">支持状态 NotConfigured 和允许</span><span class="sxs-lookup"><span data-stu-id="6e0e5-202">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="6e0e5-203">userRightsCreatePageFile</span><span class="sxs-lookup"><span data-stu-id="6e0e5-203">userRightsCreatePageFile</span></span>|[<span data-ttu-id="6e0e5-204">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="6e0e5-204">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="6e0e5-205">此用户权限确定哪些用户和组可以呼叫内部 API 创建和更改页面文件的大小。</span><span class="sxs-lookup"><span data-stu-id="6e0e5-205">This user right determines which users and groups can call an internal API to create and change the size of a page file.</span></span> <span data-ttu-id="6e0e5-206">支持状态 NotConfigured 和允许</span><span class="sxs-lookup"><span data-stu-id="6e0e5-206">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="6e0e5-207">userRightsCreatePermanentSharedObjects</span><span class="sxs-lookup"><span data-stu-id="6e0e5-207">userRightsCreatePermanentSharedObjects</span></span>|[<span data-ttu-id="6e0e5-208">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="6e0e5-208">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="6e0e5-209">此用户权限确定哪些帐户可用于通过流程管理器中创建使用对象的目录对象。</span><span class="sxs-lookup"><span data-stu-id="6e0e5-209">This user right determines which accounts can be used by processes to create a directory object using the object manager.</span></span> <span data-ttu-id="6e0e5-210">支持状态 NotConfigured 和允许</span><span class="sxs-lookup"><span data-stu-id="6e0e5-210">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="6e0e5-211">userRightsCreateSymbolicLinks</span><span class="sxs-lookup"><span data-stu-id="6e0e5-211">userRightsCreateSymbolicLinks</span></span>|[<span data-ttu-id="6e0e5-212">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="6e0e5-212">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="6e0e5-213">此用户权限确定是否用户可以从与他们登录到计算机创建符号链接。</span><span class="sxs-lookup"><span data-stu-id="6e0e5-213">This user right determines if the user can create a symbolic link from the computer to which they are logged on.</span></span> <span data-ttu-id="6e0e5-214">支持状态 NotConfigured 和允许</span><span class="sxs-lookup"><span data-stu-id="6e0e5-214">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="6e0e5-215">userRightsCreateToken</span><span class="sxs-lookup"><span data-stu-id="6e0e5-215">userRightsCreateToken</span></span>|[<span data-ttu-id="6e0e5-216">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="6e0e5-216">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="6e0e5-217">此用户权限确定哪些用户/组可以由进程来创建用于时过程使用内部 API 来创建访问令牌获取对任何本地资源的访问令牌。</span><span class="sxs-lookup"><span data-stu-id="6e0e5-217">This user right determines which users/groups can be used by processes to create a token that can then be used to get access to any local resources when the process uses an internal API to create an access token.</span></span> <span data-ttu-id="6e0e5-218">支持状态 NotConfigured 和允许</span><span class="sxs-lookup"><span data-stu-id="6e0e5-218">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="6e0e5-219">userRightsDebugPrograms</span><span class="sxs-lookup"><span data-stu-id="6e0e5-219">userRightsDebugPrograms</span></span>|[<span data-ttu-id="6e0e5-220">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="6e0e5-220">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="6e0e5-221">此用户权限确定哪些用户可以将调试器附加到任何进程或内核。</span><span class="sxs-lookup"><span data-stu-id="6e0e5-221">This user right determines which users can attach a debugger to any process or to the kernel.</span></span> <span data-ttu-id="6e0e5-222">支持状态 NotConfigured 和允许</span><span class="sxs-lookup"><span data-stu-id="6e0e5-222">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="6e0e5-223">userRightsRemoteDesktopServicesLogOn</span><span class="sxs-lookup"><span data-stu-id="6e0e5-223">userRightsRemoteDesktopServicesLogOn</span></span>|[<span data-ttu-id="6e0e5-224">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="6e0e5-224">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="6e0e5-225">此用户权限确定禁止哪些用户和组作为远程桌面服务客户端登录。</span><span class="sxs-lookup"><span data-stu-id="6e0e5-225">This user right determines which users and groups are prohibited from logging on as a Remote Desktop Services client.</span></span> <span data-ttu-id="6e0e5-226">支持状态 NotConfigured 和被阻止</span><span class="sxs-lookup"><span data-stu-id="6e0e5-226">Only states NotConfigured and Blocked are supported</span></span>|
|<span data-ttu-id="6e0e5-227">userRightsDelegation</span><span class="sxs-lookup"><span data-stu-id="6e0e5-227">userRightsDelegation</span></span>|[<span data-ttu-id="6e0e5-228">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="6e0e5-228">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="6e0e5-229">此用户权限确定哪些用户可以在用户或计算机对象上设置委派设置受信任。</span><span class="sxs-lookup"><span data-stu-id="6e0e5-229">This user right determines which users can set the Trusted for Delegation setting on a user or computer object.</span></span> <span data-ttu-id="6e0e5-230">支持状态 NotConfigured 和允许。</span><span class="sxs-lookup"><span data-stu-id="6e0e5-230">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="6e0e5-231">userRightsGenerateSecurityAudits</span><span class="sxs-lookup"><span data-stu-id="6e0e5-231">userRightsGenerateSecurityAudits</span></span>|[<span data-ttu-id="6e0e5-232">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="6e0e5-232">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="6e0e5-233">此用户权限确定哪些帐户可用于由进程将条目添加到安全日志。</span><span class="sxs-lookup"><span data-stu-id="6e0e5-233">This user right determines which accounts can be used by a process to add entries to the security log.</span></span> <span data-ttu-id="6e0e5-234">安全日志用于跟踪未经授权的系统的访问。</span><span class="sxs-lookup"><span data-stu-id="6e0e5-234">The security log is used to trace unauthorized system access.</span></span>  <span data-ttu-id="6e0e5-235">支持状态 NotConfigured 和允许。</span><span class="sxs-lookup"><span data-stu-id="6e0e5-235">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="6e0e5-236">userRightsImpersonateClient</span><span class="sxs-lookup"><span data-stu-id="6e0e5-236">userRightsImpersonateClient</span></span>|[<span data-ttu-id="6e0e5-237">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="6e0e5-237">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="6e0e5-238">分配给用户此用户权限允许代表该用户模拟客户端运行的程序。</span><span class="sxs-lookup"><span data-stu-id="6e0e5-238">Assigning this user right to a user allows programs running on behalf of that user to impersonate a client.</span></span> <span data-ttu-id="6e0e5-239">对于此种模拟需要此用户权限可防止未经授权的用户从诱使客户端连接到他们创建的服务，然后这样可以将提升未经授权的用户的权限模拟该客户端，管理或系统级别。</span><span class="sxs-lookup"><span data-stu-id="6e0e5-239">Requiring this user right for this kind of impersonation prevents an unauthorized user from convincing a client to connect to a service that they have created and then impersonating that client, which can elevate the unauthorized user's permissions to administrative or system levels.</span></span> <span data-ttu-id="6e0e5-240">支持状态 NotConfigured 和允许。</span><span class="sxs-lookup"><span data-stu-id="6e0e5-240">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="6e0e5-241">userRightsIncreaseSchedulingPriority</span><span class="sxs-lookup"><span data-stu-id="6e0e5-241">userRightsIncreaseSchedulingPriority</span></span>|[<span data-ttu-id="6e0e5-242">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="6e0e5-242">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="6e0e5-243">此用户权限确定哪些帐户可用于过程写入属性访问另一个进程增加分配给其他进程的执行优先级。</span><span class="sxs-lookup"><span data-stu-id="6e0e5-243">This user right determines which accounts can use a process with Write Property access to another process to increase the execution priority assigned to the other process.</span></span> <span data-ttu-id="6e0e5-244">支持状态 NotConfigured 和允许。</span><span class="sxs-lookup"><span data-stu-id="6e0e5-244">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="6e0e5-245">userRightsLoadUnloadDrivers</span><span class="sxs-lookup"><span data-stu-id="6e0e5-245">userRightsLoadUnloadDrivers</span></span>|[<span data-ttu-id="6e0e5-246">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="6e0e5-246">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="6e0e5-247">此用户权限确定哪些用户可以动态加载和卸载设备驱动程序或内核模式中的其他代码。</span><span class="sxs-lookup"><span data-stu-id="6e0e5-247">This user right determines which users can dynamically load and unload device drivers or other code in to kernel mode.</span></span> <span data-ttu-id="6e0e5-248">支持状态 NotConfigured 和允许。</span><span class="sxs-lookup"><span data-stu-id="6e0e5-248">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="6e0e5-249">userRightsLockMemory</span><span class="sxs-lookup"><span data-stu-id="6e0e5-249">userRightsLockMemory</span></span>|[<span data-ttu-id="6e0e5-250">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="6e0e5-250">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="6e0e5-251">此用户权限确定哪些帐户可使用过程可在物理内存，防止系统分页数据写到磁盘上的虚拟内存中保留数据。</span><span class="sxs-lookup"><span data-stu-id="6e0e5-251">This user right determines which accounts can use a process to keep data in physical memory, which prevents the system from paging the data to virtual memory on disk.</span></span> <span data-ttu-id="6e0e5-252">支持状态 NotConfigured 和允许。</span><span class="sxs-lookup"><span data-stu-id="6e0e5-252">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="6e0e5-253">userRightsManageAuditingAndSecurityLogs</span><span class="sxs-lookup"><span data-stu-id="6e0e5-253">userRightsManageAuditingAndSecurityLogs</span></span>|[<span data-ttu-id="6e0e5-254">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="6e0e5-254">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="6e0e5-255">此用户权限确定哪些用户可以指定对象访问审核各个资源，如文件、 Active Directory 对象和注册表项选项。</span><span class="sxs-lookup"><span data-stu-id="6e0e5-255">This user right determines which users can specify object access auditing options for individual resources, such as files, Active Directory objects, and registry keys.</span></span> <span data-ttu-id="6e0e5-256">支持状态 NotConfigured 和允许。</span><span class="sxs-lookup"><span data-stu-id="6e0e5-256">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="6e0e5-257">userRightsManageVolumes</span><span class="sxs-lookup"><span data-stu-id="6e0e5-257">userRightsManageVolumes</span></span>|[<span data-ttu-id="6e0e5-258">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="6e0e5-258">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="6e0e5-259">此用户权限确定哪些用户和组可以在卷上，如远程磁盘碎片整理运行维护任务。</span><span class="sxs-lookup"><span data-stu-id="6e0e5-259">This user right determines which users and groups can run maintenance tasks on a volume, such as remote defragmentation.</span></span> <span data-ttu-id="6e0e5-260">支持状态 NotConfigured 和允许。</span><span class="sxs-lookup"><span data-stu-id="6e0e5-260">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="6e0e5-261">userRightsModifyFirmwareEnvironment</span><span class="sxs-lookup"><span data-stu-id="6e0e5-261">userRightsModifyFirmwareEnvironment</span></span>|[<span data-ttu-id="6e0e5-262">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="6e0e5-262">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="6e0e5-263">此用户权限确定谁可以修改固件环境值。</span><span class="sxs-lookup"><span data-stu-id="6e0e5-263">This user right determines who can modify firmware environment values.</span></span> <span data-ttu-id="6e0e5-264">支持状态 NotConfigured 和允许。</span><span class="sxs-lookup"><span data-stu-id="6e0e5-264">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="6e0e5-265">userRightsModifyObjectLabels</span><span class="sxs-lookup"><span data-stu-id="6e0e5-265">userRightsModifyObjectLabels</span></span>|[<span data-ttu-id="6e0e5-266">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="6e0e5-266">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="6e0e5-267">此用户权限确定哪些用户帐户可以修改对象，如文件、 注册表项或由其他用户拥有的进程的完整性标签。</span><span class="sxs-lookup"><span data-stu-id="6e0e5-267">This user right determines which user accounts can modify the integrity label of objects, such as files, registry keys, or processes owned by other users.</span></span> <span data-ttu-id="6e0e5-268">支持状态 NotConfigured 和允许。</span><span class="sxs-lookup"><span data-stu-id="6e0e5-268">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="6e0e5-269">userRightsProfileSingleProcess</span><span class="sxs-lookup"><span data-stu-id="6e0e5-269">userRightsProfileSingleProcess</span></span>|[<span data-ttu-id="6e0e5-270">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="6e0e5-270">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="6e0e5-271">此用户权限确定哪些用户可以使用性能监视工具来监视系统进程的性能。</span><span class="sxs-lookup"><span data-stu-id="6e0e5-271">This user right determines which users can use performance monitoring tools to monitor the performance of system processes.</span></span> <span data-ttu-id="6e0e5-272">支持状态 NotConfigured 和允许。</span><span class="sxs-lookup"><span data-stu-id="6e0e5-272">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="6e0e5-273">userRightsRemoteShutdown</span><span class="sxs-lookup"><span data-stu-id="6e0e5-273">userRightsRemoteShutdown</span></span>|[<span data-ttu-id="6e0e5-274">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="6e0e5-274">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="6e0e5-275">此用户权限确定允许哪些用户关闭，将计算机从网络上的远程位置。</span><span class="sxs-lookup"><span data-stu-id="6e0e5-275">This user right determines which users are allowed to shut down a computer from a remote location on the network.</span></span> <span data-ttu-id="6e0e5-276">此用户权限的误用会导致拒绝服务。</span><span class="sxs-lookup"><span data-stu-id="6e0e5-276">Misuse of this user right can result in a denial of service.</span></span> <span data-ttu-id="6e0e5-277">支持状态 NotConfigured 和允许。</span><span class="sxs-lookup"><span data-stu-id="6e0e5-277">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="6e0e5-278">userRightsRestoreData</span><span class="sxs-lookup"><span data-stu-id="6e0e5-278">userRightsRestoreData</span></span>|[<span data-ttu-id="6e0e5-279">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="6e0e5-279">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="6e0e5-280">此用户权限决定哪些用户可以跳过文件、 目录、 注册表和权限还原时备份文件和目录，其他持久对象，决定哪些用户可以设置为对象的所有者的任何有效的安全主体。</span><span class="sxs-lookup"><span data-stu-id="6e0e5-280">This user right determines which users can bypass file, directory, registry, and other persistent objects permissions when restoring backed up files and directories, and determines which users can set any valid security principal as the owner of an object.</span></span> <span data-ttu-id="6e0e5-281">支持状态 NotConfigured 和允许。</span><span class="sxs-lookup"><span data-stu-id="6e0e5-281">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="6e0e5-282">userRightsTakeOwnership</span><span class="sxs-lookup"><span data-stu-id="6e0e5-282">userRightsTakeOwnership</span></span>|[<span data-ttu-id="6e0e5-283">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="6e0e5-283">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="6e0e5-284">此用户权限决定哪些用户可以在系统中，包括 Active Directory 对象、 文件和文件夹、 打印机、 注册表项、 流程和线程执行任何安全对象的所有权。</span><span class="sxs-lookup"><span data-stu-id="6e0e5-284">This user right determines which users can take ownership of any securable object in the system, including Active Directory objects, files and folders, printers, registry keys, processes, and threads.</span></span> <span data-ttu-id="6e0e5-285">支持状态 NotConfigured 和允许。</span><span class="sxs-lookup"><span data-stu-id="6e0e5-285">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="6e0e5-286">userRightsRegisterProcessAsService</span><span class="sxs-lookup"><span data-stu-id="6e0e5-286">userRightsRegisterProcessAsService</span></span>|[<span data-ttu-id="6e0e5-287">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="6e0e5-287">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="6e0e5-288">此安全设置确定被阻止的服务帐户注册为服务的进程。</span><span class="sxs-lookup"><span data-stu-id="6e0e5-288">This security setting determines which service accounts are prevented from registering a process as a service.</span></span> <span data-ttu-id="6e0e5-289">注意： 此安全设置不适用于系统、 本地服务或网络服务帐户。</span><span class="sxs-lookup"><span data-stu-id="6e0e5-289">Note: This security setting does not apply to the System, Local Service, or Network Service accounts.</span></span> <span data-ttu-id="6e0e5-290">仅支持已阻止的状态。</span><span class="sxs-lookup"><span data-stu-id="6e0e5-290">Only state Blocked is supported.</span></span>|
|<span data-ttu-id="6e0e5-291">xboxServicesEnableXboxGameSaveTask</span><span class="sxs-lookup"><span data-stu-id="6e0e5-291">xboxServicesEnableXboxGameSaveTask</span></span>|<span data-ttu-id="6e0e5-292">Boolean</span><span class="sxs-lookup"><span data-stu-id="6e0e5-292">Boolean</span></span>|<span data-ttu-id="6e0e5-293">此设置确定 xbox 游戏保存是否启用 (1) 或禁用 (0)。</span><span class="sxs-lookup"><span data-stu-id="6e0e5-293">This setting determines whether xbox game save is enabled (1) or disabled (0).</span></span>|
|<span data-ttu-id="6e0e5-294">xboxServicesAccessoryManagementServiceStartupMode</span><span class="sxs-lookup"><span data-stu-id="6e0e5-294">xboxServicesAccessoryManagementServiceStartupMode</span></span>|[<span data-ttu-id="6e0e5-295">serviceStartType</span><span class="sxs-lookup"><span data-stu-id="6e0e5-295">serviceStartType</span></span>](../resources/intune-deviceconfig-servicestarttype.md)|<span data-ttu-id="6e0e5-296">此设置确定的附件管理服务启动类型是 Automatic(2) Manual(3)、 Disabled(4)。</span><span class="sxs-lookup"><span data-stu-id="6e0e5-296">This setting determines whether the Accessory management service's start type is Automatic(2), Manual(3), Disabled(4).</span></span> <span data-ttu-id="6e0e5-297">默认： 手动。</span><span class="sxs-lookup"><span data-stu-id="6e0e5-297">Default: Manual.</span></span> <span data-ttu-id="6e0e5-298">可取值为：`manual`、`automatic`、`disabled`。</span><span class="sxs-lookup"><span data-stu-id="6e0e5-298">Possible values are: `manual`, `automatic`, `disabled`.</span></span>|
|<span data-ttu-id="6e0e5-299">xboxServicesLiveAuthManagerServiceStartupMode</span><span class="sxs-lookup"><span data-stu-id="6e0e5-299">xboxServicesLiveAuthManagerServiceStartupMode</span></span>|[<span data-ttu-id="6e0e5-300">serviceStartType</span><span class="sxs-lookup"><span data-stu-id="6e0e5-300">serviceStartType</span></span>](../resources/intune-deviceconfig-servicestarttype.md)|<span data-ttu-id="6e0e5-301">此设置确定 Live 身份验证管理器服务启动类型是 Automatic(2) Manual(3)、 Disabled(4)。</span><span class="sxs-lookup"><span data-stu-id="6e0e5-301">This setting determines whether Live Auth Manager service's start type is Automatic(2), Manual(3), Disabled(4).</span></span> <span data-ttu-id="6e0e5-302">默认： 手动。</span><span class="sxs-lookup"><span data-stu-id="6e0e5-302">Default: Manual.</span></span> <span data-ttu-id="6e0e5-303">可取值为：`manual`、`automatic`、`disabled`。</span><span class="sxs-lookup"><span data-stu-id="6e0e5-303">Possible values are: `manual`, `automatic`, `disabled`.</span></span>|
|<span data-ttu-id="6e0e5-304">xboxServicesLiveGameSaveServiceStartupMode</span><span class="sxs-lookup"><span data-stu-id="6e0e5-304">xboxServicesLiveGameSaveServiceStartupMode</span></span>|[<span data-ttu-id="6e0e5-305">serviceStartType</span><span class="sxs-lookup"><span data-stu-id="6e0e5-305">serviceStartType</span></span>](../resources/intune-deviceconfig-servicestarttype.md)|<span data-ttu-id="6e0e5-306">此设置确定是否 Automatic(2) Manual(3)、 Disabled(4) Live 保存服务的启动类型的游戏。</span><span class="sxs-lookup"><span data-stu-id="6e0e5-306">This setting determines whether Live Game save service's start type is Automatic(2), Manual(3), Disabled(4).</span></span> <span data-ttu-id="6e0e5-307">默认： 手动。</span><span class="sxs-lookup"><span data-stu-id="6e0e5-307">Default: Manual.</span></span> <span data-ttu-id="6e0e5-308">可取值为：`manual`、`automatic`、`disabled`。</span><span class="sxs-lookup"><span data-stu-id="6e0e5-308">Possible values are: `manual`, `automatic`, `disabled`.</span></span>|
|<span data-ttu-id="6e0e5-309">xboxServicesLiveNetworkingServiceStartupMode</span><span class="sxs-lookup"><span data-stu-id="6e0e5-309">xboxServicesLiveNetworkingServiceStartupMode</span></span>|[<span data-ttu-id="6e0e5-310">serviceStartType</span><span class="sxs-lookup"><span data-stu-id="6e0e5-310">serviceStartType</span></span>](../resources/intune-deviceconfig-servicestarttype.md)|<span data-ttu-id="6e0e5-311">此设置确定网络服务启动类型是 Automatic(2) Manual(3)、 Disabled(4)。</span><span class="sxs-lookup"><span data-stu-id="6e0e5-311">This setting determines whether Networking service's start type is Automatic(2), Manual(3), Disabled(4).</span></span> <span data-ttu-id="6e0e5-312">默认： 手动。</span><span class="sxs-lookup"><span data-stu-id="6e0e5-312">Default: Manual.</span></span> <span data-ttu-id="6e0e5-313">可取值为：`manual`、`automatic`、`disabled`。</span><span class="sxs-lookup"><span data-stu-id="6e0e5-313">Possible values are: `manual`, `automatic`, `disabled`.</span></span>|
|<span data-ttu-id="6e0e5-314">localSecurityOptionsBlockMicrosoftAccounts</span><span class="sxs-lookup"><span data-stu-id="6e0e5-314">localSecurityOptionsBlockMicrosoftAccounts</span></span>|<span data-ttu-id="6e0e5-315">Boolean</span><span class="sxs-lookup"><span data-stu-id="6e0e5-315">Boolean</span></span>|<span data-ttu-id="6e0e5-316">禁止用户添加到此计算机的新的 Microsoft 帐户。</span><span class="sxs-lookup"><span data-stu-id="6e0e5-316">Prevent users from adding new Microsoft accounts to this computer.</span></span>|
|<span data-ttu-id="6e0e5-317">localSecurityOptionsBlockRemoteLogonWithBlankPassword</span><span class="sxs-lookup"><span data-stu-id="6e0e5-317">localSecurityOptionsBlockRemoteLogonWithBlankPassword</span></span>|<span data-ttu-id="6e0e5-318">Boolean</span><span class="sxs-lookup"><span data-stu-id="6e0e5-318">Boolean</span></span>|<span data-ttu-id="6e0e5-319">启用本地帐户不受密码保护登录从物理设备以外的位置。将启用默认值</span><span class="sxs-lookup"><span data-stu-id="6e0e5-319">Enable Local accounts that are not password protected to log on from locations other than the physical device.Default is enabled</span></span>|
|<span data-ttu-id="6e0e5-320">localSecurityOptionsEnableAdministratorAccount</span><span class="sxs-lookup"><span data-stu-id="6e0e5-320">localSecurityOptionsEnableAdministratorAccount</span></span>|<span data-ttu-id="6e0e5-321">Boolean</span><span class="sxs-lookup"><span data-stu-id="6e0e5-321">Boolean</span></span>|<span data-ttu-id="6e0e5-322">确定是否启用或禁用的本地管理员帐户。</span><span class="sxs-lookup"><span data-stu-id="6e0e5-322">Determines whether the Local Administrator account is enabled or disabled.</span></span>|
|<span data-ttu-id="6e0e5-323">localSecurityOptionsAdministratorAccountName</span><span class="sxs-lookup"><span data-stu-id="6e0e5-323">localSecurityOptionsAdministratorAccountName</span></span>|<span data-ttu-id="6e0e5-324">字符串</span><span class="sxs-lookup"><span data-stu-id="6e0e5-324">String</span></span>|<span data-ttu-id="6e0e5-325">定义要与"管理员"的帐户的安全标识符 (SID) 关联的不同的帐户名称。</span><span class="sxs-lookup"><span data-stu-id="6e0e5-325">Define a different account name to be associated with the security identifier (SID) for the account “Administrator”.</span></span>|
|<span data-ttu-id="6e0e5-326">localSecurityOptionsEnableGuestAccount</span><span class="sxs-lookup"><span data-stu-id="6e0e5-326">localSecurityOptionsEnableGuestAccount</span></span>|<span data-ttu-id="6e0e5-327">Boolean</span><span class="sxs-lookup"><span data-stu-id="6e0e5-327">Boolean</span></span>|<span data-ttu-id="6e0e5-328">确定是启用还是禁用来宾帐户。</span><span class="sxs-lookup"><span data-stu-id="6e0e5-328">Determines if the Guest account is enabled or disabled.</span></span>|
|<span data-ttu-id="6e0e5-329">localSecurityOptionsGuestAccountName</span><span class="sxs-lookup"><span data-stu-id="6e0e5-329">localSecurityOptionsGuestAccountName</span></span>|<span data-ttu-id="6e0e5-330">字符串</span><span class="sxs-lookup"><span data-stu-id="6e0e5-330">String</span></span>|<span data-ttu-id="6e0e5-331">定义要为"来宾"的帐户的安全标识符 (SID) 关联的不同的帐户名称。</span><span class="sxs-lookup"><span data-stu-id="6e0e5-331">Define a different account name to be associated with the security identifier (SID) for the account “Guest”.</span></span>|
|<span data-ttu-id="6e0e5-332">localSecurityOptionsAllowUndockWithoutHavingToLogon</span><span class="sxs-lookup"><span data-stu-id="6e0e5-332">localSecurityOptionsAllowUndockWithoutHavingToLogon</span></span>|<span data-ttu-id="6e0e5-333">Boolean</span><span class="sxs-lookup"><span data-stu-id="6e0e5-333">Boolean</span></span>|<span data-ttu-id="6e0e5-334">正在取消停靠而无需登录阻止便携式计算机。</span><span class="sxs-lookup"><span data-stu-id="6e0e5-334">Prevent a portable computer from being undocked without having to log in.</span></span>|
|<span data-ttu-id="6e0e5-335">localSecurityOptionsBlockUsersInstallingPrinterDrivers</span><span class="sxs-lookup"><span data-stu-id="6e0e5-335">localSecurityOptionsBlockUsersInstallingPrinterDrivers</span></span>|<span data-ttu-id="6e0e5-336">Boolean</span><span class="sxs-lookup"><span data-stu-id="6e0e5-336">Boolean</span></span>|<span data-ttu-id="6e0e5-337">限制为连接到向管理员仅共享打印机的一部分安装的打印机驱动程序。</span><span class="sxs-lookup"><span data-stu-id="6e0e5-337">Restrict installing printer drivers as part of connecting to a shared printer to admins only.</span></span>|
|<span data-ttu-id="6e0e5-338">localSecurityOptionsBlockRemoteOpticalDriveAccess</span><span class="sxs-lookup"><span data-stu-id="6e0e5-338">localSecurityOptionsBlockRemoteOpticalDriveAccess</span></span>|<span data-ttu-id="6e0e5-339">Boolean</span><span class="sxs-lookup"><span data-stu-id="6e0e5-339">Boolean</span></span>|<span data-ttu-id="6e0e5-340">启用此设置允许访问 CD-ROM 媒体仅以交互方式登录的用户。</span><span class="sxs-lookup"><span data-stu-id="6e0e5-340">Enabling this settings allows only interactively logged on user to access CD-ROM media.</span></span>|
|<span data-ttu-id="6e0e5-341">localSecurityOptionsFormatAndEjectOfRemovableMediaAllowedUser</span><span class="sxs-lookup"><span data-stu-id="6e0e5-341">localSecurityOptionsFormatAndEjectOfRemovableMediaAllowedUser</span></span>|[<span data-ttu-id="6e0e5-342">localSecurityOptionsFormatAndEjectOfRemovableMediaAllowedUserType</span><span class="sxs-lookup"><span data-stu-id="6e0e5-342">localSecurityOptionsFormatAndEjectOfRemovableMediaAllowedUserType</span></span>](../resources/intune-deviceconfig-localsecurityoptionsformatandejectofremovablemediaallowedusertype.md)|<span data-ttu-id="6e0e5-343">定义允许谁格式化和弹出可移动 NTFS 媒体。</span><span class="sxs-lookup"><span data-stu-id="6e0e5-343">Define who is allowed to format and eject removable NTFS media.</span></span> <span data-ttu-id="6e0e5-344">可取值为：`notConfigured`、`administrators`、`administratorsAndPowerUsers`、`administratorsAndInteractiveUsers`。</span><span class="sxs-lookup"><span data-stu-id="6e0e5-344">Possible values are: `notConfigured`, `administrators`, `administratorsAndPowerUsers`, `administratorsAndInteractiveUsers`.</span></span>|
|<span data-ttu-id="6e0e5-345">localSecurityOptionsMachineInactivityLimit</span><span class="sxs-lookup"><span data-stu-id="6e0e5-345">localSecurityOptionsMachineInactivityLimit</span></span>|<span data-ttu-id="6e0e5-346">Int32</span><span class="sxs-lookup"><span data-stu-id="6e0e5-346">Int32</span></span>|<span data-ttu-id="6e0e5-347">交互式桌面上登录屏幕上定义最大分钟无活动，直到屏幕保护程序运行。</span><span class="sxs-lookup"><span data-stu-id="6e0e5-347">Define maximum minutes of inactivity on the interactive desktop’s login screen until the screen saver runs.</span></span> <span data-ttu-id="6e0e5-348">有效的值 0 到 9999 之间</span><span class="sxs-lookup"><span data-stu-id="6e0e5-348">Valid values 0 to 9999</span></span>|
|<span data-ttu-id="6e0e5-349">localSecurityOptionsMachineInactivityLimitInMinutes</span><span class="sxs-lookup"><span data-stu-id="6e0e5-349">localSecurityOptionsMachineInactivityLimitInMinutes</span></span>|<span data-ttu-id="6e0e5-350">Int32</span><span class="sxs-lookup"><span data-stu-id="6e0e5-350">Int32</span></span>|<span data-ttu-id="6e0e5-351">交互式桌面上登录屏幕上定义最大分钟无活动，直到屏幕保护程序运行。</span><span class="sxs-lookup"><span data-stu-id="6e0e5-351">Define maximum minutes of inactivity on the interactive desktop’s login screen until the screen saver runs.</span></span> <span data-ttu-id="6e0e5-352">有效的值 0 到 9999 之间</span><span class="sxs-lookup"><span data-stu-id="6e0e5-352">Valid values 0 to 9999</span></span>|
|<span data-ttu-id="6e0e5-353">localSecurityOptionsDoNotRequireCtrlAltDel</span><span class="sxs-lookup"><span data-stu-id="6e0e5-353">localSecurityOptionsDoNotRequireCtrlAltDel</span></span>|<span data-ttu-id="6e0e5-354">Boolean</span><span class="sxs-lookup"><span data-stu-id="6e0e5-354">Boolean</span></span>|<span data-ttu-id="6e0e5-355">需要 CTRL + ALT + DEL 要按用户登录之前。</span><span class="sxs-lookup"><span data-stu-id="6e0e5-355">Require CTRL+ALT+DEL to be pressed before a user can log on.</span></span>|
|<span data-ttu-id="6e0e5-356">localSecurityOptionsHideLastSignedInUser</span><span class="sxs-lookup"><span data-stu-id="6e0e5-356">localSecurityOptionsHideLastSignedInUser</span></span>|<span data-ttu-id="6e0e5-357">Boolean</span><span class="sxs-lookup"><span data-stu-id="6e0e5-357">Boolean</span></span>|<span data-ttu-id="6e0e5-358">不在此设备上显示的签名的最后一个人的用户名。</span><span class="sxs-lookup"><span data-stu-id="6e0e5-358">Do not display the username of the last person who signed in on this device.</span></span>|
|<span data-ttu-id="6e0e5-359">localSecurityOptionsHideUsernameAtSignIn</span><span class="sxs-lookup"><span data-stu-id="6e0e5-359">localSecurityOptionsHideUsernameAtSignIn</span></span>|<span data-ttu-id="6e0e5-360">Boolean</span><span class="sxs-lookup"><span data-stu-id="6e0e5-360">Boolean</span></span>|<span data-ttu-id="6e0e5-361">不显示登录到此设备输入凭据之后和之前显示设备的桌面的人员的用户名。</span><span class="sxs-lookup"><span data-stu-id="6e0e5-361">Do not display the username of the person signing in to this device after credentials are entered and before the device’s desktop is shown.</span></span>|
|<span data-ttu-id="6e0e5-362">localSecurityOptionsLogOnMessageTitle</span><span class="sxs-lookup"><span data-stu-id="6e0e5-362">localSecurityOptionsLogOnMessageTitle</span></span>|<span data-ttu-id="6e0e5-363">字符串</span><span class="sxs-lookup"><span data-stu-id="6e0e5-363">String</span></span>|<span data-ttu-id="6e0e5-364">用户尝试登录的设置邮件标题。</span><span class="sxs-lookup"><span data-stu-id="6e0e5-364">Set message title for users attempting to log in.</span></span>|
|<span data-ttu-id="6e0e5-365">localSecurityOptionsLogOnMessageText</span><span class="sxs-lookup"><span data-stu-id="6e0e5-365">localSecurityOptionsLogOnMessageText</span></span>|<span data-ttu-id="6e0e5-366">字符串</span><span class="sxs-lookup"><span data-stu-id="6e0e5-366">String</span></span>|<span data-ttu-id="6e0e5-367">设置用户试图登录消息文本。</span><span class="sxs-lookup"><span data-stu-id="6e0e5-367">Set message text for users attempting to log in.</span></span>|
|<span data-ttu-id="6e0e5-368">localSecurityOptionsAllowPKU2UAuthenticationRequests</span><span class="sxs-lookup"><span data-stu-id="6e0e5-368">localSecurityOptionsAllowPKU2UAuthenticationRequests</span></span>|<span data-ttu-id="6e0e5-369">Boolean</span><span class="sxs-lookup"><span data-stu-id="6e0e5-369">Boolean</span></span>|<span data-ttu-id="6e0e5-370">对此设备块 PKU2U 身份验证请求使用联机标识。</span><span class="sxs-lookup"><span data-stu-id="6e0e5-370">Block PKU2U authentication requests to this device to use online identities.</span></span>|
|<span data-ttu-id="6e0e5-371">localSecurityOptionsAllowRemoteCallsToSecurityAccountsManagerHelperBool</span><span class="sxs-lookup"><span data-stu-id="6e0e5-371">localSecurityOptionsAllowRemoteCallsToSecurityAccountsManagerHelperBool</span></span>|<span data-ttu-id="6e0e5-372">Boolean</span><span class="sxs-lookup"><span data-stu-id="6e0e5-372">Boolean</span></span>|<span data-ttu-id="6e0e5-373">用户界面帮助程序布尔 LocalSecurityOptionsAllowRemoteCallsToSecurityAccountsManager 实体</span><span class="sxs-lookup"><span data-stu-id="6e0e5-373">UI helper boolean for LocalSecurityOptionsAllowRemoteCallsToSecurityAccountsManager entity</span></span>|
|<span data-ttu-id="6e0e5-374">localSecurityOptionsAllowRemoteCallsToSecurityAccountsManager</span><span class="sxs-lookup"><span data-stu-id="6e0e5-374">localSecurityOptionsAllowRemoteCallsToSecurityAccountsManager</span></span>|<span data-ttu-id="6e0e5-375">字符串</span><span class="sxs-lookup"><span data-stu-id="6e0e5-375">String</span></span>|<span data-ttu-id="6e0e5-376">编辑默认安全描述符定义语言字符串，以允许或拒绝远程调用 SAM 用户和组。</span><span class="sxs-lookup"><span data-stu-id="6e0e5-376">Edit the default Security Descriptor Definition Language string to allow or deny users and groups to make remote calls to the SAM.</span></span>|
|<span data-ttu-id="6e0e5-377">localSecurityOptionsMinimumSessionSecurityForNtlmSspBasedClients</span><span class="sxs-lookup"><span data-stu-id="6e0e5-377">localSecurityOptionsMinimumSessionSecurityForNtlmSspBasedClients</span></span>|[<span data-ttu-id="6e0e5-378">localSecurityOptionsMinimumSessionSecurity</span><span class="sxs-lookup"><span data-stu-id="6e0e5-378">localSecurityOptionsMinimumSessionSecurity</span></span>](../resources/intune-deviceconfig-localsecurityoptionsminimumsessionsecurity.md)|<span data-ttu-id="6e0e5-379">此安全设置允许客户端要求 128 位加密和/或 NTLMv2 会话安全协商。</span><span class="sxs-lookup"><span data-stu-id="6e0e5-379">This security setting allows a client to require the negotiation of 128-bit encryption and/or NTLMv2 session security.</span></span> <span data-ttu-id="6e0e5-380">可取值为：`none`、`requireNtmlV2SessionSecurity`、`require128BitEncryption`、`ntlmV2And128BitEncryption`。</span><span class="sxs-lookup"><span data-stu-id="6e0e5-380">Possible values are: `none`, `requireNtmlV2SessionSecurity`, `require128BitEncryption`, `ntlmV2And128BitEncryption`.</span></span>|
|<span data-ttu-id="6e0e5-381">localSecurityOptionsMinimumSessionSecurityForNtlmSspBasedServers</span><span class="sxs-lookup"><span data-stu-id="6e0e5-381">localSecurityOptionsMinimumSessionSecurityForNtlmSspBasedServers</span></span>|[<span data-ttu-id="6e0e5-382">localSecurityOptionsMinimumSessionSecurity</span><span class="sxs-lookup"><span data-stu-id="6e0e5-382">localSecurityOptionsMinimumSessionSecurity</span></span>](../resources/intune-deviceconfig-localsecurityoptionsminimumsessionsecurity.md)|<span data-ttu-id="6e0e5-383">此安全设置允许服务器要求 128 位加密和/或 NTLMv2 会话安全协商。</span><span class="sxs-lookup"><span data-stu-id="6e0e5-383">This security setting allows a server to require the negotiation of 128-bit encryption and/or NTLMv2 session security.</span></span> <span data-ttu-id="6e0e5-384">可取值为：`none`、`requireNtmlV2SessionSecurity`、`require128BitEncryption`、`ntlmV2And128BitEncryption`。</span><span class="sxs-lookup"><span data-stu-id="6e0e5-384">Possible values are: `none`, `requireNtmlV2SessionSecurity`, `require128BitEncryption`, `ntlmV2And128BitEncryption`.</span></span>|
|<span data-ttu-id="6e0e5-385">lanManagerAuthenticationLevel</span><span class="sxs-lookup"><span data-stu-id="6e0e5-385">lanManagerAuthenticationLevel</span></span>|[<span data-ttu-id="6e0e5-386">lanManagerAuthenticationLevel</span><span class="sxs-lookup"><span data-stu-id="6e0e5-386">lanManagerAuthenticationLevel</span></span>](../resources/intune-deviceconfig-lanmanagerauthenticationlevel.md)|<span data-ttu-id="6e0e5-387">此安全设置确定哪个质询/响应身份验证协议用于网络登录。</span><span class="sxs-lookup"><span data-stu-id="6e0e5-387">This security setting determines which challenge/response authentication protocol is used for network logons.</span></span> <span data-ttu-id="6e0e5-388">可取值为：`lmAndNltm`、`lmNtlmAndNtlmV2`、`lmAndNtlmOnly`、`lmAndNtlmV2`、`lmNtlmV2AndNotLm`、`lmNtlmV2AndNotLmOrNtm`。</span><span class="sxs-lookup"><span data-stu-id="6e0e5-388">Possible values are: `lmAndNltm`, `lmNtlmAndNtlmV2`, `lmAndNtlmOnly`, `lmAndNtlmV2`, `lmNtlmV2AndNotLm`, `lmNtlmV2AndNotLmOrNtm`.</span></span>|
|<span data-ttu-id="6e0e5-389">lanManagerWorkstationEnableInsecureGuestLogons</span><span class="sxs-lookup"><span data-stu-id="6e0e5-389">lanManagerWorkstationEnableInsecureGuestLogons</span></span>|<span data-ttu-id="6e0e5-390">Boolean</span><span class="sxs-lookup"><span data-stu-id="6e0e5-390">Boolean</span></span>|<span data-ttu-id="6e0e5-391">如果启用，则 SMB 客户端将允许不安全的来宾登录。</span><span class="sxs-lookup"><span data-stu-id="6e0e5-391">If enabled,the SMB client will allow insecure guest logons.</span></span> <span data-ttu-id="6e0e5-392">如果未配置，SMB 客户端将拒绝不安全的来宾登录。</span><span class="sxs-lookup"><span data-stu-id="6e0e5-392">If not configured, the SMB client will reject insecure guest logons.</span></span>|
|<span data-ttu-id="6e0e5-393">localSecurityOptionsClearVirtualMemoryPageFile</span><span class="sxs-lookup"><span data-stu-id="6e0e5-393">localSecurityOptionsClearVirtualMemoryPageFile</span></span>|<span data-ttu-id="6e0e5-394">Boolean</span><span class="sxs-lookup"><span data-stu-id="6e0e5-394">Boolean</span></span>|<span data-ttu-id="6e0e5-395">此安全设置确定系统关闭时是否清除虚拟内存页面文件。</span><span class="sxs-lookup"><span data-stu-id="6e0e5-395">This security setting determines whether the virtual memory pagefile is cleared when the system is shut down.</span></span>|
|<span data-ttu-id="6e0e5-396">localSecurityOptionsAllowSystemToBeShutDownWithoutHavingToLogOn</span><span class="sxs-lookup"><span data-stu-id="6e0e5-396">localSecurityOptionsAllowSystemToBeShutDownWithoutHavingToLogOn</span></span>|<span data-ttu-id="6e0e5-397">Boolean</span><span class="sxs-lookup"><span data-stu-id="6e0e5-397">Boolean</span></span>|<span data-ttu-id="6e0e5-398">此安全设置确定是否可以关闭计算机而无需登录到 Windows。</span><span class="sxs-lookup"><span data-stu-id="6e0e5-398">This security setting determines whether a computer can be shut down without having to log on to Windows.</span></span>|
|<span data-ttu-id="6e0e5-399">localSecurityOptionsAllowUIAccessApplicationElevation</span><span class="sxs-lookup"><span data-stu-id="6e0e5-399">localSecurityOptionsAllowUIAccessApplicationElevation</span></span>|<span data-ttu-id="6e0e5-400">Boolean</span><span class="sxs-lookup"><span data-stu-id="6e0e5-400">Boolean</span></span>|<span data-ttu-id="6e0e5-401">允许 UIAccess 应用程序无需使用安全桌面提示提升。</span><span class="sxs-lookup"><span data-stu-id="6e0e5-401">Allow UIAccess apps to prompt for elevation without using the secure desktop.</span></span>|
|<span data-ttu-id="6e0e5-402">localSecurityOptionsVirtualizeFileAndRegistryWriteFailuresToPerUserLocations</span><span class="sxs-lookup"><span data-stu-id="6e0e5-402">localSecurityOptionsVirtualizeFileAndRegistryWriteFailuresToPerUserLocations</span></span>|<span data-ttu-id="6e0e5-403">Boolean</span><span class="sxs-lookup"><span data-stu-id="6e0e5-403">Boolean</span></span>|<span data-ttu-id="6e0e5-404">虚拟化文件和注册表写入失败次数为每用户位置</span><span class="sxs-lookup"><span data-stu-id="6e0e5-404">Virtualize file and registry write failures to per user locations</span></span>|
|<span data-ttu-id="6e0e5-405">localSecurityOptionsOnlyElevateSignedExecutables</span><span class="sxs-lookup"><span data-stu-id="6e0e5-405">localSecurityOptionsOnlyElevateSignedExecutables</span></span>|<span data-ttu-id="6e0e5-406">Boolean</span><span class="sxs-lookup"><span data-stu-id="6e0e5-406">Boolean</span></span>|<span data-ttu-id="6e0e5-407">允许运行之前，强制实施 PKI 证书路径验证给定的可执行文件。</span><span class="sxs-lookup"><span data-stu-id="6e0e5-407">Enforce PKI certification path validation for a given executable file before it is permitted to run.</span></span>|
|<span data-ttu-id="6e0e5-408">localSecurityOptionsAdministratorElevationPromptBehavior</span><span class="sxs-lookup"><span data-stu-id="6e0e5-408">localSecurityOptionsAdministratorElevationPromptBehavior</span></span>|[<span data-ttu-id="6e0e5-409">localSecurityOptionsAdministratorElevationPromptBehaviorType</span><span class="sxs-lookup"><span data-stu-id="6e0e5-409">localSecurityOptionsAdministratorElevationPromptBehaviorType</span></span>](../resources/intune-deviceconfig-localsecurityoptionsadministratorelevationpromptbehaviortype.md)|<span data-ttu-id="6e0e5-410">管理员批准模式中定义管理员的提升提示的行为。</span><span class="sxs-lookup"><span data-stu-id="6e0e5-410">Define the behavior of the elevation prompt for admins in Admin Approval Mode.</span></span> <span data-ttu-id="6e0e5-411">可取值为：`notConfigured`、`elevateWithoutPrompting`、`promptForCredentialsOnTheSecureDesktop`、`promptForConsentOnTheSecureDesktop`、`promptForCredentials`、`promptForConsent`、`promptForConsentForNonWindowsBinaries`。</span><span class="sxs-lookup"><span data-stu-id="6e0e5-411">Possible values are: `notConfigured`, `elevateWithoutPrompting`, `promptForCredentialsOnTheSecureDesktop`, `promptForConsentOnTheSecureDesktop`, `promptForCredentials`, `promptForConsent`, `promptForConsentForNonWindowsBinaries`.</span></span>|
|<span data-ttu-id="6e0e5-412">localSecurityOptionsStandardUserElevationPromptBehavior</span><span class="sxs-lookup"><span data-stu-id="6e0e5-412">localSecurityOptionsStandardUserElevationPromptBehavior</span></span>|[<span data-ttu-id="6e0e5-413">localSecurityOptionsStandardUserElevationPromptBehaviorType</span><span class="sxs-lookup"><span data-stu-id="6e0e5-413">localSecurityOptionsStandardUserElevationPromptBehaviorType</span></span>](../resources/intune-deviceconfig-localsecurityoptionsstandarduserelevationpromptbehaviortype.md)|<span data-ttu-id="6e0e5-414">定义标准用户的提升提示的行为。</span><span class="sxs-lookup"><span data-stu-id="6e0e5-414">Define the behavior of the elevation prompt for standard users.</span></span> <span data-ttu-id="6e0e5-415">可取值为：`notConfigured`、`automaticallyDenyElevationRequests`、`promptForCredentialsOnTheSecureDesktop`、`promptForCredentials`。</span><span class="sxs-lookup"><span data-stu-id="6e0e5-415">Possible values are: `notConfigured`, `automaticallyDenyElevationRequests`, `promptForCredentialsOnTheSecureDesktop`, `promptForCredentials`.</span></span>|
|<span data-ttu-id="6e0e5-416">localSecurityOptionsSwitchToSecureDesktopWhenPromptingForElevation</span><span class="sxs-lookup"><span data-stu-id="6e0e5-416">localSecurityOptionsSwitchToSecureDesktopWhenPromptingForElevation</span></span>|<span data-ttu-id="6e0e5-417">Boolean</span><span class="sxs-lookup"><span data-stu-id="6e0e5-417">Boolean</span></span>|<span data-ttu-id="6e0e5-418">启用所有提升请求，以转到交互式用户的桌面，而不是安全的桌面。</span><span class="sxs-lookup"><span data-stu-id="6e0e5-418">Enable all elevation requests to go to the interactive user's desktop rather than the secure desktop.</span></span> <span data-ttu-id="6e0e5-419">使用提示行为 admins 和标准用户的策略设置。</span><span class="sxs-lookup"><span data-stu-id="6e0e5-419">Prompt behavior policy settings for admins and standard users are used.</span></span>|
|<span data-ttu-id="6e0e5-420">localSecurityOptionsDetectApplicationInstallationsAndPromptForElevation</span><span class="sxs-lookup"><span data-stu-id="6e0e5-420">localSecurityOptionsDetectApplicationInstallationsAndPromptForElevation</span></span>|<span data-ttu-id="6e0e5-421">Boolean</span><span class="sxs-lookup"><span data-stu-id="6e0e5-421">Boolean</span></span>|<span data-ttu-id="6e0e5-422">需要提升的权限的应用程序安装将会进行提示管理员凭据。将启用默认值</span><span class="sxs-lookup"><span data-stu-id="6e0e5-422">App installations requiring elevated privileges will prompt for admin credentials.Default is enabled</span></span>|
|<span data-ttu-id="6e0e5-423">localSecurityOptionsAllowUIAccessApplicationsForSecureLocations</span><span class="sxs-lookup"><span data-stu-id="6e0e5-423">localSecurityOptionsAllowUIAccessApplicationsForSecureLocations</span></span>|<span data-ttu-id="6e0e5-424">Boolean</span><span class="sxs-lookup"><span data-stu-id="6e0e5-424">Boolean</span></span>|<span data-ttu-id="6e0e5-425">允许 UIAccess 应用程序无需使用安全桌面提示提升。将启用默认值</span><span class="sxs-lookup"><span data-stu-id="6e0e5-425">Allow UIAccess apps to prompt for elevation without using the secure desktop.Default is enabled</span></span>|
|<span data-ttu-id="6e0e5-426">localSecurityOptionsUseAdminApprovalMode</span><span class="sxs-lookup"><span data-stu-id="6e0e5-426">localSecurityOptionsUseAdminApprovalMode</span></span>|<span data-ttu-id="6e0e5-427">Boolean</span><span class="sxs-lookup"><span data-stu-id="6e0e5-427">Boolean</span></span>|<span data-ttu-id="6e0e5-428">定义的内置的管理帐户使用管理员批准模式还是具有完整的管理员权限运行所有应用程序。将启用默认值</span><span class="sxs-lookup"><span data-stu-id="6e0e5-428">Defines whether the built-in admin account uses Admin Approval Mode or runs all apps with full admin privileges.Default is enabled</span></span>|
|<span data-ttu-id="6e0e5-429">localSecurityOptionsUseAdminApprovalModeForAdministrators</span><span class="sxs-lookup"><span data-stu-id="6e0e5-429">localSecurityOptionsUseAdminApprovalModeForAdministrators</span></span>|<span data-ttu-id="6e0e5-430">Boolean</span><span class="sxs-lookup"><span data-stu-id="6e0e5-430">Boolean</span></span>|<span data-ttu-id="6e0e5-431">定义是否启用管理员批准模式和所有 UAC 策略设置，将启用默认值</span><span class="sxs-lookup"><span data-stu-id="6e0e5-431">Define whether Admin Approval Mode and all UAC policy settings are enabled, default is enabled</span></span>|
|<span data-ttu-id="6e0e5-432">localSecurityOptionsInformationShownOnLockScreen</span><span class="sxs-lookup"><span data-stu-id="6e0e5-432">localSecurityOptionsInformationShownOnLockScreen</span></span>|[<span data-ttu-id="6e0e5-433">localSecurityOptionsInformationShownOnLockScreenType</span><span class="sxs-lookup"><span data-stu-id="6e0e5-433">localSecurityOptionsInformationShownOnLockScreenType</span></span>](../resources/intune-deviceconfig-localsecurityoptionsinformationshownonlockscreentype.md)|<span data-ttu-id="6e0e5-434">配置会话已被锁定时显示的用户信息。</span><span class="sxs-lookup"><span data-stu-id="6e0e5-434">Configure the user information that is displayed when the session is locked.</span></span> <span data-ttu-id="6e0e5-435">如果未配置，将显示用户的显示名称、 域和用户名。</span><span class="sxs-lookup"><span data-stu-id="6e0e5-435">If not configured, user display name, domain and username are shown.</span></span> <span data-ttu-id="6e0e5-436">可取值为：`notConfigured`、`userDisplayNameDomainUser`、`userDisplayNameOnly`、`doNotDisplayUser`。</span><span class="sxs-lookup"><span data-stu-id="6e0e5-436">Possible values are: `notConfigured`, `userDisplayNameDomainUser`, `userDisplayNameOnly`, `doNotDisplayUser`.</span></span>|
|<span data-ttu-id="6e0e5-437">localSecurityOptionsInformationDisplayedOnLockScreen</span><span class="sxs-lookup"><span data-stu-id="6e0e5-437">localSecurityOptionsInformationDisplayedOnLockScreen</span></span>|[<span data-ttu-id="6e0e5-438">localSecurityOptionsInformationDisplayedOnLockScreenType</span><span class="sxs-lookup"><span data-stu-id="6e0e5-438">localSecurityOptionsInformationDisplayedOnLockScreenType</span></span>](../resources/intune-deviceconfig-localsecurityoptionsinformationdisplayedonlockscreentype.md)|<span data-ttu-id="6e0e5-439">配置会话已被锁定时显示的用户信息。</span><span class="sxs-lookup"><span data-stu-id="6e0e5-439">Configure the user information that is displayed when the session is locked.</span></span> <span data-ttu-id="6e0e5-440">如果未配置，将显示用户的显示名称、 域和用户名。</span><span class="sxs-lookup"><span data-stu-id="6e0e5-440">If not configured, user display name, domain and username are shown.</span></span> <span data-ttu-id="6e0e5-441">可取值为：`notConfigured`、`administrators`、`administratorsAndPowerUsers`、`administratorsAndInteractiveUsers`。</span><span class="sxs-lookup"><span data-stu-id="6e0e5-441">Possible values are: `notConfigured`, `administrators`, `administratorsAndPowerUsers`, `administratorsAndInteractiveUsers`.</span></span>|
|<span data-ttu-id="6e0e5-442">localSecurityOptionsDisableClientDigitallySignCommunicationsIfServerAgrees</span><span class="sxs-lookup"><span data-stu-id="6e0e5-442">localSecurityOptionsDisableClientDigitallySignCommunicationsIfServerAgrees</span></span>|<span data-ttu-id="6e0e5-443">Boolean</span><span class="sxs-lookup"><span data-stu-id="6e0e5-443">Boolean</span></span>|<span data-ttu-id="6e0e5-444">此安全设置确定是否 SMB 客户端尝试协商 SMB 数据包签名。</span><span class="sxs-lookup"><span data-stu-id="6e0e5-444">This security setting determines whether the SMB client attempts to negotiate SMB packet signing.</span></span>|
|<span data-ttu-id="6e0e5-445">localSecurityOptionsClientDigitallySignCommunicationsAlways</span><span class="sxs-lookup"><span data-stu-id="6e0e5-445">localSecurityOptionsClientDigitallySignCommunicationsAlways</span></span>|<span data-ttu-id="6e0e5-446">Boolean</span><span class="sxs-lookup"><span data-stu-id="6e0e5-446">Boolean</span></span>|<span data-ttu-id="6e0e5-447">此安全设置确定是否数据包签名所需 SMB 客户端组件。</span><span class="sxs-lookup"><span data-stu-id="6e0e5-447">This security setting determines whether packet signing is required by the SMB client component.</span></span>|
|<span data-ttu-id="6e0e5-448">localSecurityOptionsClientSendUnencryptedPasswordToThirdPartySMBServers</span><span class="sxs-lookup"><span data-stu-id="6e0e5-448">localSecurityOptionsClientSendUnencryptedPasswordToThirdPartySMBServers</span></span>|<span data-ttu-id="6e0e5-449">Boolean</span><span class="sxs-lookup"><span data-stu-id="6e0e5-449">Boolean</span></span>|<span data-ttu-id="6e0e5-450">如果启用此安全设置，则允许服务器消息块 (SMB) 重定向到不支持期间身份验证的密码加密的非 Microsoft SMB 服务器发送纯文本密码。</span><span class="sxs-lookup"><span data-stu-id="6e0e5-450">If this security setting is enabled, the Server Message Block (SMB) redirector is allowed to send plaintext passwords to non-Microsoft SMB servers that do not support password encryption during authentication.</span></span>|
|<span data-ttu-id="6e0e5-451">localSecurityOptionsDisableServerDigitallySignCommunicationsAlways</span><span class="sxs-lookup"><span data-stu-id="6e0e5-451">localSecurityOptionsDisableServerDigitallySignCommunicationsAlways</span></span>|<span data-ttu-id="6e0e5-452">Boolean</span><span class="sxs-lookup"><span data-stu-id="6e0e5-452">Boolean</span></span>|<span data-ttu-id="6e0e5-453">此安全设置确定是否由 SMB 服务器组件要求签名数据包。</span><span class="sxs-lookup"><span data-stu-id="6e0e5-453">This security setting determines whether packet signing is required by the SMB server component.</span></span>|
|<span data-ttu-id="6e0e5-454">localSecurityOptionsDisableServerDigitallySignCommunicationsIfClientAgrees</span><span class="sxs-lookup"><span data-stu-id="6e0e5-454">localSecurityOptionsDisableServerDigitallySignCommunicationsIfClientAgrees</span></span>|<span data-ttu-id="6e0e5-455">Boolean</span><span class="sxs-lookup"><span data-stu-id="6e0e5-455">Boolean</span></span>|<span data-ttu-id="6e0e5-456">此安全设置确定 SMB 服务器是否协商 SMB 数据包签名与请求的客户端。</span><span class="sxs-lookup"><span data-stu-id="6e0e5-456">This security setting determines whether the SMB server will negotiate SMB packet signing with clients that request it.</span></span>|
|<span data-ttu-id="6e0e5-457">localSecurityOptionsRestrictAnonymousAccessToNamedPipesAndShares</span><span class="sxs-lookup"><span data-stu-id="6e0e5-457">localSecurityOptionsRestrictAnonymousAccessToNamedPipesAndShares</span></span>|<span data-ttu-id="6e0e5-458">Boolean</span><span class="sxs-lookup"><span data-stu-id="6e0e5-458">Boolean</span></span>|<span data-ttu-id="6e0e5-459">默认情况下，此安全设置将匿名访问限制为共享和管道的可匿名访问的命名的管道和可匿名访问的共享的设置</span><span class="sxs-lookup"><span data-stu-id="6e0e5-459">By default, this security setting restricts anonymous access to shares and pipes to the settings for named pipes that can be accessed anonymously and Shares that can be accessed anonymously</span></span>|
|<span data-ttu-id="6e0e5-460">localSecurityOptionsDoNotAllowAnonymousEnumerationOfSAMAccounts</span><span class="sxs-lookup"><span data-stu-id="6e0e5-460">localSecurityOptionsDoNotAllowAnonymousEnumerationOfSAMAccounts</span></span>|<span data-ttu-id="6e0e5-461">Boolean</span><span class="sxs-lookup"><span data-stu-id="6e0e5-461">Boolean</span></span>|<span data-ttu-id="6e0e5-462">此安全设置确定将对匿名连接到计算机上授予其他权限。</span><span class="sxs-lookup"><span data-stu-id="6e0e5-462">This security setting determines what additional permissions will be granted for anonymous connections to the computer.</span></span>|
|<span data-ttu-id="6e0e5-463">localSecurityOptionsAllowAnonymousEnumerationOfSAMAccountsAndShares</span><span class="sxs-lookup"><span data-stu-id="6e0e5-463">localSecurityOptionsAllowAnonymousEnumerationOfSAMAccountsAndShares</span></span>|<span data-ttu-id="6e0e5-464">Boolean</span><span class="sxs-lookup"><span data-stu-id="6e0e5-464">Boolean</span></span>|<span data-ttu-id="6e0e5-465">此安全设置确定是否允许匿名用户执行某些活动，如枚举的域帐户和网络共享名称。</span><span class="sxs-lookup"><span data-stu-id="6e0e5-465">This security setting determines whether to allows anonymous users to perform certain activities, such as enumerating the names of domain accounts and network shares.</span></span>|
|<span data-ttu-id="6e0e5-466">localSecurityOptionsDoNotStoreLANManagerHashValueOnNextPasswordChange</span><span class="sxs-lookup"><span data-stu-id="6e0e5-466">localSecurityOptionsDoNotStoreLANManagerHashValueOnNextPasswordChange</span></span>|<span data-ttu-id="6e0e5-467">Boolean</span><span class="sxs-lookup"><span data-stu-id="6e0e5-467">Boolean</span></span>|<span data-ttu-id="6e0e5-468">此安全设置确定，是否在下次密码更改，存储新密码的 LAN Manager (LM) 哈希值。</span><span class="sxs-lookup"><span data-stu-id="6e0e5-468">This security setting determines if, at the next password change, the LAN Manager (LM) hash value for the new password is stored.</span></span> <span data-ttu-id="6e0e5-469">默认情况下，它不存储。</span><span class="sxs-lookup"><span data-stu-id="6e0e5-469">It’s not stored by default.</span></span>|
|<span data-ttu-id="6e0e5-470">localSecurityOptionsSmartCardRemovalBehavior</span><span class="sxs-lookup"><span data-stu-id="6e0e5-470">localSecurityOptionsSmartCardRemovalBehavior</span></span>|[<span data-ttu-id="6e0e5-471">localSecurityOptionsSmartCardRemovalBehaviorType</span><span class="sxs-lookup"><span data-stu-id="6e0e5-471">localSecurityOptionsSmartCardRemovalBehaviorType</span></span>](../resources/intune-deviceconfig-localsecurityoptionssmartcardremovalbehaviortype.md)|<span data-ttu-id="6e0e5-472">此安全设置确定智能卡读卡器从移除智能卡登录的用户时，会发生什么情况。</span><span class="sxs-lookup"><span data-stu-id="6e0e5-472">This security setting determines what happens when the smart card for a logged-on user is removed from the smart card reader.</span></span> <span data-ttu-id="6e0e5-473">可取值为：`lockWorkstation`、`noAction`、`forceLogoff`、`disconnectRemoteDesktopSession`。</span><span class="sxs-lookup"><span data-stu-id="6e0e5-473">Possible values are: `lockWorkstation`, `noAction`, `forceLogoff`, `disconnectRemoteDesktopSession`.</span></span>|
|<span data-ttu-id="6e0e5-474">defenderSecurityCenterDisableAppBrowserUI</span><span class="sxs-lookup"><span data-stu-id="6e0e5-474">defenderSecurityCenterDisableAppBrowserUI</span></span>|<span data-ttu-id="6e0e5-475">Boolean</span><span class="sxs-lookup"><span data-stu-id="6e0e5-475">Boolean</span></span>|<span data-ttu-id="6e0e5-476">用于禁用的应用程序和浏览器的保护区域显示。</span><span class="sxs-lookup"><span data-stu-id="6e0e5-476">Used to disable the display of the app and browser protection area.</span></span>|
|<span data-ttu-id="6e0e5-477">defenderSecurityCenterDisableFamilyUI</span><span class="sxs-lookup"><span data-stu-id="6e0e5-477">defenderSecurityCenterDisableFamilyUI</span></span>|<span data-ttu-id="6e0e5-478">Boolean</span><span class="sxs-lookup"><span data-stu-id="6e0e5-478">Boolean</span></span>|<span data-ttu-id="6e0e5-479">用于禁用系列选项区域的显示。</span><span class="sxs-lookup"><span data-stu-id="6e0e5-479">Used to disable the display of the family options area.</span></span>|
|<span data-ttu-id="6e0e5-480">defenderSecurityCenterDisableHealthUI</span><span class="sxs-lookup"><span data-stu-id="6e0e5-480">defenderSecurityCenterDisableHealthUI</span></span>|<span data-ttu-id="6e0e5-481">Boolean</span><span class="sxs-lookup"><span data-stu-id="6e0e5-481">Boolean</span></span>|<span data-ttu-id="6e0e5-482">用于禁用设备性能和运行状况区域的显示。</span><span class="sxs-lookup"><span data-stu-id="6e0e5-482">Used to disable the display of the device performance and health area.</span></span>|
|<span data-ttu-id="6e0e5-483">defenderSecurityCenterDisableNetworkUI</span><span class="sxs-lookup"><span data-stu-id="6e0e5-483">defenderSecurityCenterDisableNetworkUI</span></span>|<span data-ttu-id="6e0e5-484">Boolean</span><span class="sxs-lookup"><span data-stu-id="6e0e5-484">Boolean</span></span>|<span data-ttu-id="6e0e5-485">用于禁用防火墙和网络保护区域的显示。</span><span class="sxs-lookup"><span data-stu-id="6e0e5-485">Used to disable the display of the firewall and network protection area.</span></span>|
|<span data-ttu-id="6e0e5-486">defenderSecurityCenterDisableVirusUI</span><span class="sxs-lookup"><span data-stu-id="6e0e5-486">defenderSecurityCenterDisableVirusUI</span></span>|<span data-ttu-id="6e0e5-487">Boolean</span><span class="sxs-lookup"><span data-stu-id="6e0e5-487">Boolean</span></span>|<span data-ttu-id="6e0e5-488">用于禁用病毒和威胁保护区域的显示。</span><span class="sxs-lookup"><span data-stu-id="6e0e5-488">Used to disable the display of the virus and threat protection area.</span></span>|
|<span data-ttu-id="6e0e5-489">defenderSecurityCenterDisableAccountUI</span><span class="sxs-lookup"><span data-stu-id="6e0e5-489">defenderSecurityCenterDisableAccountUI</span></span>|<span data-ttu-id="6e0e5-490">Boolean</span><span class="sxs-lookup"><span data-stu-id="6e0e5-490">Boolean</span></span>|<span data-ttu-id="6e0e5-491">用于禁用帐户保护区域的显示。</span><span class="sxs-lookup"><span data-stu-id="6e0e5-491">Used to disable the display of the account protection area.</span></span>|
|<span data-ttu-id="6e0e5-492">defenderSecurityCenterDisableHardwareUI</span><span class="sxs-lookup"><span data-stu-id="6e0e5-492">defenderSecurityCenterDisableHardwareUI</span></span>|<span data-ttu-id="6e0e5-493">Boolean</span><span class="sxs-lookup"><span data-stu-id="6e0e5-493">Boolean</span></span>|<span data-ttu-id="6e0e5-494">用于禁用硬件保护区域的显示。</span><span class="sxs-lookup"><span data-stu-id="6e0e5-494">Used to disable the display of the hardware protection area.</span></span>|
|<span data-ttu-id="6e0e5-495">defenderSecurityCenterDisableRansomwareUI</span><span class="sxs-lookup"><span data-stu-id="6e0e5-495">defenderSecurityCenterDisableRansomwareUI</span></span>|<span data-ttu-id="6e0e5-496">Boolean</span><span class="sxs-lookup"><span data-stu-id="6e0e5-496">Boolean</span></span>|<span data-ttu-id="6e0e5-497">用于禁用勒索软件保护区域的显示。</span><span class="sxs-lookup"><span data-stu-id="6e0e5-497">Used to disable the display of the ransomware protection area.</span></span> |
|<span data-ttu-id="6e0e5-498">defenderSecurityCenterDisableSecureBootUI</span><span class="sxs-lookup"><span data-stu-id="6e0e5-498">defenderSecurityCenterDisableSecureBootUI</span></span>|<span data-ttu-id="6e0e5-499">Boolean</span><span class="sxs-lookup"><span data-stu-id="6e0e5-499">Boolean</span></span>|<span data-ttu-id="6e0e5-500">用于禁用的设备安全下的安全启动区域显示。</span><span class="sxs-lookup"><span data-stu-id="6e0e5-500">Used to disable the display of the secure boot area under Device security.</span></span>|
|<span data-ttu-id="6e0e5-501">defenderSecurityCenterDisableTroubleshootingUI</span><span class="sxs-lookup"><span data-stu-id="6e0e5-501">defenderSecurityCenterDisableTroubleshootingUI</span></span>|<span data-ttu-id="6e0e5-502">Boolean</span><span class="sxs-lookup"><span data-stu-id="6e0e5-502">Boolean</span></span>|<span data-ttu-id="6e0e5-503">用于禁用安全过程下设备安全疑难解答的显示。</span><span class="sxs-lookup"><span data-stu-id="6e0e5-503">Used to disable the display of the security process troubleshooting under Device security.</span></span>|
|<span data-ttu-id="6e0e5-504">defenderSecurityCenterOrganizationDisplayName</span><span class="sxs-lookup"><span data-stu-id="6e0e5-504">defenderSecurityCenterOrganizationDisplayName</span></span>|<span data-ttu-id="6e0e5-505">字符串</span><span class="sxs-lookup"><span data-stu-id="6e0e5-505">String</span></span>|<span data-ttu-id="6e0e5-506">向用户显示公司名称。</span><span class="sxs-lookup"><span data-stu-id="6e0e5-506">The company name that is displayed to the users.</span></span>|
|<span data-ttu-id="6e0e5-507">defenderSecurityCenterHelpEmail</span><span class="sxs-lookup"><span data-stu-id="6e0e5-507">defenderSecurityCenterHelpEmail</span></span>|<span data-ttu-id="6e0e5-508">字符串</span><span class="sxs-lookup"><span data-stu-id="6e0e5-508">String</span></span>|<span data-ttu-id="6e0e5-509">向用户显示的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="6e0e5-509">The email address that is displayed to users.</span></span>|
|<span data-ttu-id="6e0e5-510">defenderSecurityCenterHelpPhone</span><span class="sxs-lookup"><span data-stu-id="6e0e5-510">defenderSecurityCenterHelpPhone</span></span>|<span data-ttu-id="6e0e5-511">字符串</span><span class="sxs-lookup"><span data-stu-id="6e0e5-511">String</span></span>|<span data-ttu-id="6e0e5-512">电话号码或向用户显示的 Skype ID 中。</span><span class="sxs-lookup"><span data-stu-id="6e0e5-512">The phone number or Skype ID that is displayed to users.</span></span>|
|<span data-ttu-id="6e0e5-513">defenderSecurityCenterHelpURL</span><span class="sxs-lookup"><span data-stu-id="6e0e5-513">defenderSecurityCenterHelpURL</span></span>|<span data-ttu-id="6e0e5-514">字符串</span><span class="sxs-lookup"><span data-stu-id="6e0e5-514">String</span></span>|<span data-ttu-id="6e0e5-515">帮助门户这向用户显示的 URL。</span><span class="sxs-lookup"><span data-stu-id="6e0e5-515">The help portal URL this is displayed to users.</span></span>|
|<span data-ttu-id="6e0e5-516">defenderSecurityCenterNotificationsFromApp</span><span class="sxs-lookup"><span data-stu-id="6e0e5-516">defenderSecurityCenterNotificationsFromApp</span></span>|[<span data-ttu-id="6e0e5-517">defenderSecurityCenterNotificationsFromAppType</span><span class="sxs-lookup"><span data-stu-id="6e0e5-517">defenderSecurityCenterNotificationsFromAppType</span></span>](../resources/intune-deviceconfig-defendersecuritycenternotificationsfromapptype.md)|<span data-ttu-id="6e0e5-518">若要从应用程序的显示区域显示的通知。</span><span class="sxs-lookup"><span data-stu-id="6e0e5-518">Notifications to show from the displayed areas of app.</span></span> <span data-ttu-id="6e0e5-519">可取值为：`notConfigured`、`blockNoncriticalNotifications`、`blockAllNotifications`。</span><span class="sxs-lookup"><span data-stu-id="6e0e5-519">Possible values are: `notConfigured`, `blockNoncriticalNotifications`, `blockAllNotifications`.</span></span>|
|<span data-ttu-id="6e0e5-520">defenderSecurityCenterITContactDisplay</span><span class="sxs-lookup"><span data-stu-id="6e0e5-520">defenderSecurityCenterITContactDisplay</span></span>|[<span data-ttu-id="6e0e5-521">defenderSecurityCenterITContactDisplayType</span><span class="sxs-lookup"><span data-stu-id="6e0e5-521">defenderSecurityCenterITContactDisplayType</span></span>](../resources/intune-deviceconfig-defendersecuritycenteritcontactdisplaytype.md)|<span data-ttu-id="6e0e5-522">配置显示 IT 联系人位置向最终用户的信息。</span><span class="sxs-lookup"><span data-stu-id="6e0e5-522">Configure where to display IT contact information to end users.</span></span> <span data-ttu-id="6e0e5-523">可取值为：`notConfigured`、`displayInAppAndInNotifications`、`displayOnlyInApp`、`displayOnlyInNotifications`。</span><span class="sxs-lookup"><span data-stu-id="6e0e5-523">Possible values are: `notConfigured`, `displayInAppAndInNotifications`, `displayOnlyInApp`, `displayOnlyInNotifications`.</span></span>|
|<span data-ttu-id="6e0e5-524">firewallBlockStatefulFTP</span><span class="sxs-lookup"><span data-stu-id="6e0e5-524">firewallBlockStatefulFTP</span></span>|<span data-ttu-id="6e0e5-525">Boolean</span><span class="sxs-lookup"><span data-stu-id="6e0e5-525">Boolean</span></span>|<span data-ttu-id="6e0e5-526">阻止到设备的有状态 FTP 连接</span><span class="sxs-lookup"><span data-stu-id="6e0e5-526">Blocks stateful FTP connections to the device</span></span>|
|<span data-ttu-id="6e0e5-527">firewallIdleTimeoutForSecurityAssociationInSeconds</span><span class="sxs-lookup"><span data-stu-id="6e0e5-527">firewallIdleTimeoutForSecurityAssociationInSeconds</span></span>|<span data-ttu-id="6e0e5-528">Int32</span><span class="sxs-lookup"><span data-stu-id="6e0e5-528">Int32</span></span>|<span data-ttu-id="6e0e5-529">配置安全关联的空闲超时（以秒为单位），值范围为 300 到 3600（包括这两个值）。</span><span class="sxs-lookup"><span data-stu-id="6e0e5-529">Configures the idle timeout for security associations, in seconds, from 300 to 3600 inclusive.</span></span> <span data-ttu-id="6e0e5-530">这是一个时间段，在此之后安全关联将过期并被删除。</span><span class="sxs-lookup"><span data-stu-id="6e0e5-530">This is the period after which security associations will expire and be deleted.</span></span> <span data-ttu-id="6e0e5-531">有效值为 300 至 3600。</span><span class="sxs-lookup"><span data-stu-id="6e0e5-531">Valid values 300 to 3600</span></span>|
|<span data-ttu-id="6e0e5-532">firewallPreSharedKeyEncodingMethod</span><span class="sxs-lookup"><span data-stu-id="6e0e5-532">firewallPreSharedKeyEncodingMethod</span></span>|[<span data-ttu-id="6e0e5-533">firewallPreSharedKeyEncodingMethodType</span><span class="sxs-lookup"><span data-stu-id="6e0e5-533">firewallPreSharedKeyEncodingMethodType</span></span>](../resources/intune-deviceconfig-firewallpresharedkeyencodingmethodtype.md)|<span data-ttu-id="6e0e5-534">选择要使用编码的预共享的键。</span><span class="sxs-lookup"><span data-stu-id="6e0e5-534">Select the preshared key encoding to be used.</span></span> <span data-ttu-id="6e0e5-535">可取值为：`deviceDefault`、`none`、`utF8`。</span><span class="sxs-lookup"><span data-stu-id="6e0e5-535">Possible values are: `deviceDefault`, `none`, `utF8`.</span></span>|
|<span data-ttu-id="6e0e5-536">firewallIPSecExemptionsAllowNeighborDiscovery</span><span class="sxs-lookup"><span data-stu-id="6e0e5-536">firewallIPSecExemptionsAllowNeighborDiscovery</span></span>|<span data-ttu-id="6e0e5-537">Boolean</span><span class="sxs-lookup"><span data-stu-id="6e0e5-537">Boolean</span></span>|<span data-ttu-id="6e0e5-538">配置 IPSec 免除项以允许邻居发现 IPv6 ICMP 类型代码</span><span class="sxs-lookup"><span data-stu-id="6e0e5-538">Configures IPSec exemptions to allow neighbor discovery IPv6 ICMP type-codes</span></span>|
|<span data-ttu-id="6e0e5-539">firewallIPSecExemptionsAllowICMP</span><span class="sxs-lookup"><span data-stu-id="6e0e5-539">firewallIPSecExemptionsAllowICMP</span></span>|<span data-ttu-id="6e0e5-540">Boolean</span><span class="sxs-lookup"><span data-stu-id="6e0e5-540">Boolean</span></span>|<span data-ttu-id="6e0e5-541">配置 IPSec 免除项以允许 ICMP</span><span class="sxs-lookup"><span data-stu-id="6e0e5-541">Configures IPSec exemptions to allow ICMP</span></span>|
|<span data-ttu-id="6e0e5-542">firewallIPSecExemptionsAllowRouterDiscovery</span><span class="sxs-lookup"><span data-stu-id="6e0e5-542">firewallIPSecExemptionsAllowRouterDiscovery</span></span>|<span data-ttu-id="6e0e5-543">Boolean</span><span class="sxs-lookup"><span data-stu-id="6e0e5-543">Boolean</span></span>|<span data-ttu-id="6e0e5-544">配置 IPSec 免除项以允许路由器发现 IPv6 ICMP 类型代码</span><span class="sxs-lookup"><span data-stu-id="6e0e5-544">Configures IPSec exemptions to allow router discovery IPv6 ICMP type-codes</span></span>|
|<span data-ttu-id="6e0e5-545">firewallIPSecExemptionsAllowDHCP</span><span class="sxs-lookup"><span data-stu-id="6e0e5-545">firewallIPSecExemptionsAllowDHCP</span></span>|<span data-ttu-id="6e0e5-546">Boolean</span><span class="sxs-lookup"><span data-stu-id="6e0e5-546">Boolean</span></span>|<span data-ttu-id="6e0e5-547">配置 IPSec 免除项以允许 IPv4 和 IPv6 DHCP 通信</span><span class="sxs-lookup"><span data-stu-id="6e0e5-547">Configures IPSec exemptions to allow both IPv4 and IPv6 DHCP traffic</span></span>|
|<span data-ttu-id="6e0e5-548">firewallCertificateRevocationListCheckMethod</span><span class="sxs-lookup"><span data-stu-id="6e0e5-548">firewallCertificateRevocationListCheckMethod</span></span>|[<span data-ttu-id="6e0e5-549">firewallCertificateRevocationListCheckMethodType</span><span class="sxs-lookup"><span data-stu-id="6e0e5-549">firewallCertificateRevocationListCheckMethodType</span></span>](../resources/intune-deviceconfig-firewallcertificaterevocationlistcheckmethodtype.md)|<span data-ttu-id="6e0e5-550">指定如何强制实施证书吊销列表。</span><span class="sxs-lookup"><span data-stu-id="6e0e5-550">Specify how the certificate revocation list is to be enforced.</span></span> <span data-ttu-id="6e0e5-551">可取值为：`deviceDefault`、`none`、`attempt`、`require`。</span><span class="sxs-lookup"><span data-stu-id="6e0e5-551">Possible values are: `deviceDefault`, `none`, `attempt`, `require`.</span></span>|
|<span data-ttu-id="6e0e5-552">firewallMergeKeyingModuleSettings</span><span class="sxs-lookup"><span data-stu-id="6e0e5-552">firewallMergeKeyingModuleSettings</span></span>|<span data-ttu-id="6e0e5-553">Boolean</span><span class="sxs-lookup"><span data-stu-id="6e0e5-553">Boolean</span></span>|<span data-ttu-id="6e0e5-554">如果键控模块不完全支持身份验证集，请指示模块仅忽略不受支持的身份验证套件而不是整个集</span><span class="sxs-lookup"><span data-stu-id="6e0e5-554">If an authentication set is not fully supported by a keying module, direct the module to ignore only unsupported authentication suites rather than the entire set</span></span>|
|<span data-ttu-id="6e0e5-555">firewallPacketQueueingMethod</span><span class="sxs-lookup"><span data-stu-id="6e0e5-555">firewallPacketQueueingMethod</span></span>|[<span data-ttu-id="6e0e5-556">firewallPacketQueueingMethodType</span><span class="sxs-lookup"><span data-stu-id="6e0e5-556">firewallPacketQueueingMethodType</span></span>](../resources/intune-deviceconfig-firewallpacketqueueingmethodtype.md)|<span data-ttu-id="6e0e5-557">配置数据包 queueing 应如何应用隧道网关方案中。</span><span class="sxs-lookup"><span data-stu-id="6e0e5-557">Configures how packet queueing should be applied in the tunnel gateway scenario.</span></span> <span data-ttu-id="6e0e5-558">可取值为：`deviceDefault`、`disabled`、`queueInbound`、`queueOutbound`、`queueBoth`。</span><span class="sxs-lookup"><span data-stu-id="6e0e5-558">Possible values are: `deviceDefault`, `disabled`, `queueInbound`, `queueOutbound`, `queueBoth`.</span></span>|
|<span data-ttu-id="6e0e5-559">firewallProfileDomain</span><span class="sxs-lookup"><span data-stu-id="6e0e5-559">firewallProfileDomain</span></span>|[<span data-ttu-id="6e0e5-560">windowsFirewallNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="6e0e5-560">windowsFirewallNetworkProfile</span></span>](../resources/intune-deviceconfig-windowsfirewallnetworkprofile.md)|<span data-ttu-id="6e0e5-561">配置域网络的防火墙配置文件设置</span><span class="sxs-lookup"><span data-stu-id="6e0e5-561">Configures the firewall profile settings for domain networks</span></span>|
|<span data-ttu-id="6e0e5-562">firewallProfilePublic</span><span class="sxs-lookup"><span data-stu-id="6e0e5-562">firewallProfilePublic</span></span>|[<span data-ttu-id="6e0e5-563">windowsFirewallNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="6e0e5-563">windowsFirewallNetworkProfile</span></span>](../resources/intune-deviceconfig-windowsfirewallnetworkprofile.md)|<span data-ttu-id="6e0e5-564">配置公用网络的防火墙配置文件设置</span><span class="sxs-lookup"><span data-stu-id="6e0e5-564">Configures the firewall profile settings for public networks</span></span>|
|<span data-ttu-id="6e0e5-565">firewallProfilePrivate</span><span class="sxs-lookup"><span data-stu-id="6e0e5-565">firewallProfilePrivate</span></span>|[<span data-ttu-id="6e0e5-566">windowsFirewallNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="6e0e5-566">windowsFirewallNetworkProfile</span></span>](../resources/intune-deviceconfig-windowsfirewallnetworkprofile.md)|<span data-ttu-id="6e0e5-567">配置专用网络的防火墙配置文件设置</span><span class="sxs-lookup"><span data-stu-id="6e0e5-567">Configures the firewall profile settings for private networks</span></span>|
|<span data-ttu-id="6e0e5-568">defenderAttackSurfaceReductionExcludedPaths</span><span class="sxs-lookup"><span data-stu-id="6e0e5-568">defenderAttackSurfaceReductionExcludedPaths</span></span>|<span data-ttu-id="6e0e5-569">String 集合</span><span class="sxs-lookup"><span data-stu-id="6e0e5-569">String collection</span></span>|<span data-ttu-id="6e0e5-570">要从攻击面减少规则中排除的 exe 文件和文件夹的列表</span><span class="sxs-lookup"><span data-stu-id="6e0e5-570">List of exe files and folders to be excluded from attack surface reduction rules</span></span>|
|<span data-ttu-id="6e0e5-571">defenderOfficeAppsOtherProcessInjectionType</span><span class="sxs-lookup"><span data-stu-id="6e0e5-571">defenderOfficeAppsOtherProcessInjectionType</span></span>|[<span data-ttu-id="6e0e5-572">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="6e0e5-572">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="6e0e5-573">值，指示将到其他进程的 Office 应用程序的行为。</span><span class="sxs-lookup"><span data-stu-id="6e0e5-573">Value indicating the behavior of Office applications injecting into other processes.</span></span> <span data-ttu-id="6e0e5-574">可取值为：`userDefined`、`block`、`auditMode`。</span><span class="sxs-lookup"><span data-stu-id="6e0e5-574">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="6e0e5-575">defenderOfficeAppsOtherProcessInjection</span><span class="sxs-lookup"><span data-stu-id="6e0e5-575">defenderOfficeAppsOtherProcessInjection</span></span>|[<span data-ttu-id="6e0e5-576">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="6e0e5-576">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="6e0e5-577">值，指示将到其他进程的 Office 应用程序的行为。</span><span class="sxs-lookup"><span data-stu-id="6e0e5-577">Value indicating the behavior of  Office applications injecting into other processes.</span></span> <span data-ttu-id="6e0e5-578">可取值为：`userDefined`、`enable`、`auditMode`。</span><span class="sxs-lookup"><span data-stu-id="6e0e5-578">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="6e0e5-579">defenderOfficeAppsExecutableContentCreationOrLaunchType</span><span class="sxs-lookup"><span data-stu-id="6e0e5-579">defenderOfficeAppsExecutableContentCreationOrLaunchType</span></span>|[<span data-ttu-id="6e0e5-580">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="6e0e5-580">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="6e0e5-581">指示 Office 应用程序/宏创建或启动可执行文件内容的行为的值。</span><span class="sxs-lookup"><span data-stu-id="6e0e5-581">Value indicating the behavior of Office applications/macros creating or launching executable content.</span></span> <span data-ttu-id="6e0e5-582">可取值为：`userDefined`、`block`、`auditMode`。</span><span class="sxs-lookup"><span data-stu-id="6e0e5-582">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="6e0e5-583">defenderOfficeAppsExecutableContentCreationOrLaunch</span><span class="sxs-lookup"><span data-stu-id="6e0e5-583">defenderOfficeAppsExecutableContentCreationOrLaunch</span></span>|[<span data-ttu-id="6e0e5-584">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="6e0e5-584">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="6e0e5-585">指示 Office 应用程序/宏创建或启动可执行文件内容的行为的值。</span><span class="sxs-lookup"><span data-stu-id="6e0e5-585">Value indicating the behavior of Office applications/macros creating or launching executable content.</span></span> <span data-ttu-id="6e0e5-586">可取值为：`userDefined`、`enable`、`auditMode`。</span><span class="sxs-lookup"><span data-stu-id="6e0e5-586">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="6e0e5-587">defenderOfficeAppsLaunchChildProcessType</span><span class="sxs-lookup"><span data-stu-id="6e0e5-587">defenderOfficeAppsLaunchChildProcessType</span></span>|[<span data-ttu-id="6e0e5-588">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="6e0e5-588">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="6e0e5-589">指示启动子进程的 Office 应用程序的行为的值。</span><span class="sxs-lookup"><span data-stu-id="6e0e5-589">Value indicating the behavior of Office application launching child processes.</span></span> <span data-ttu-id="6e0e5-590">可取值为：`userDefined`、`block`、`auditMode`。</span><span class="sxs-lookup"><span data-stu-id="6e0e5-590">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="6e0e5-591">defenderOfficeAppsLaunchChildProcess</span><span class="sxs-lookup"><span data-stu-id="6e0e5-591">defenderOfficeAppsLaunchChildProcess</span></span>|[<span data-ttu-id="6e0e5-592">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="6e0e5-592">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="6e0e5-593">指示启动子进程的 Office 应用程序的行为的值。</span><span class="sxs-lookup"><span data-stu-id="6e0e5-593">Value indicating the behavior of Office application launching child processes.</span></span> <span data-ttu-id="6e0e5-594">可取值为：`userDefined`、`enable`、`auditMode`。</span><span class="sxs-lookup"><span data-stu-id="6e0e5-594">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="6e0e5-595">defenderOfficeMacroCodeAllowWin32ImportsType</span><span class="sxs-lookup"><span data-stu-id="6e0e5-595">defenderOfficeMacroCodeAllowWin32ImportsType</span></span>|[<span data-ttu-id="6e0e5-596">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="6e0e5-596">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="6e0e5-597">值，该值指示的 Win32 行为导入从 Office 中的宏代码。</span><span class="sxs-lookup"><span data-stu-id="6e0e5-597">Value indicating the behavior of Win32 imports from Macro code in Office.</span></span> <span data-ttu-id="6e0e5-598">可取值为：`userDefined`、`block`、`auditMode`。</span><span class="sxs-lookup"><span data-stu-id="6e0e5-598">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="6e0e5-599">defenderOfficeMacroCodeAllowWin32Imports</span><span class="sxs-lookup"><span data-stu-id="6e0e5-599">defenderOfficeMacroCodeAllowWin32Imports</span></span>|[<span data-ttu-id="6e0e5-600">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="6e0e5-600">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="6e0e5-601">值，该值指示的 Win32 行为导入从 Office 中的宏代码。</span><span class="sxs-lookup"><span data-stu-id="6e0e5-601">Value indicating the behavior of Win32 imports from Macro code in Office.</span></span> <span data-ttu-id="6e0e5-602">可取值为：`userDefined`、`enable`、`auditMode`。</span><span class="sxs-lookup"><span data-stu-id="6e0e5-602">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="6e0e5-603">defenderScriptObfuscatedMacroCodeType</span><span class="sxs-lookup"><span data-stu-id="6e0e5-603">defenderScriptObfuscatedMacroCodeType</span></span>|[<span data-ttu-id="6e0e5-604">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="6e0e5-604">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="6e0e5-605">值，该值指示经过模糊处理 js/vbs/ps/macro 代码的行为。</span><span class="sxs-lookup"><span data-stu-id="6e0e5-605">Value indicating the behavior of obfuscated js/vbs/ps/macro code.</span></span> <span data-ttu-id="6e0e5-606">可取值为：`userDefined`、`block`、`auditMode`。</span><span class="sxs-lookup"><span data-stu-id="6e0e5-606">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="6e0e5-607">defenderScriptObfuscatedMacroCode</span><span class="sxs-lookup"><span data-stu-id="6e0e5-607">defenderScriptObfuscatedMacroCode</span></span>|[<span data-ttu-id="6e0e5-608">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="6e0e5-608">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="6e0e5-609">值，该值指示经过模糊处理 js/vbs/ps/macro 代码的行为。</span><span class="sxs-lookup"><span data-stu-id="6e0e5-609">Value indicating the behavior of obfuscated js/vbs/ps/macro code.</span></span> <span data-ttu-id="6e0e5-610">可取值为：`userDefined`、`enable`、`auditMode`。</span><span class="sxs-lookup"><span data-stu-id="6e0e5-610">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="6e0e5-611">defenderScriptDownloadedPayloadExecutionType</span><span class="sxs-lookup"><span data-stu-id="6e0e5-611">defenderScriptDownloadedPayloadExecutionType</span></span>|[<span data-ttu-id="6e0e5-612">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="6e0e5-612">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="6e0e5-613">从 Internet 下载的值，该值指示 js/vbs 执行负载的行为。</span><span class="sxs-lookup"><span data-stu-id="6e0e5-613">Value indicating the behavior of js/vbs executing payload downloaded from Internet.</span></span> <span data-ttu-id="6e0e5-614">可取值为：`userDefined`、`block`、`auditMode`。</span><span class="sxs-lookup"><span data-stu-id="6e0e5-614">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="6e0e5-615">defenderScriptDownloadedPayloadExecution</span><span class="sxs-lookup"><span data-stu-id="6e0e5-615">defenderScriptDownloadedPayloadExecution</span></span>|[<span data-ttu-id="6e0e5-616">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="6e0e5-616">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="6e0e5-617">从 Internet 下载的值，该值指示 js/vbs 执行负载的行为。</span><span class="sxs-lookup"><span data-stu-id="6e0e5-617">Value indicating the behavior of js/vbs executing payload downloaded from Internet.</span></span> <span data-ttu-id="6e0e5-618">可取值为：`userDefined`、`enable`、`auditMode`。</span><span class="sxs-lookup"><span data-stu-id="6e0e5-618">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="6e0e5-619">defenderPreventCredentialStealingType</span><span class="sxs-lookup"><span data-stu-id="6e0e5-619">defenderPreventCredentialStealingType</span></span>|[<span data-ttu-id="6e0e5-620">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="6e0e5-620">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="6e0e5-621">值，该值指示是否允许从 Windows 本地安全机构子系统窃取的凭据。</span><span class="sxs-lookup"><span data-stu-id="6e0e5-621">Value indicating if credential stealing from the Windows local security authority subsystem is permitted.</span></span> <span data-ttu-id="6e0e5-622">可取值为：`userDefined`、`enable`、`auditMode`。</span><span class="sxs-lookup"><span data-stu-id="6e0e5-622">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="6e0e5-623">defenderProcessCreationType</span><span class="sxs-lookup"><span data-stu-id="6e0e5-623">defenderProcessCreationType</span></span>|[<span data-ttu-id="6e0e5-624">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="6e0e5-624">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="6e0e5-625">值，该值指示响应来自 PSExec 和 WMI 命令的过程创建。</span><span class="sxs-lookup"><span data-stu-id="6e0e5-625">Value indicating response to process creations originating from PSExec and WMI commands.</span></span> <span data-ttu-id="6e0e5-626">可取值为：`userDefined`、`block`、`auditMode`。</span><span class="sxs-lookup"><span data-stu-id="6e0e5-626">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="6e0e5-627">defenderProcessCreation</span><span class="sxs-lookup"><span data-stu-id="6e0e5-627">defenderProcessCreation</span></span>|[<span data-ttu-id="6e0e5-628">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="6e0e5-628">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="6e0e5-629">值，该值指示响应来自 PSExec 和 WMI 命令的过程创建。</span><span class="sxs-lookup"><span data-stu-id="6e0e5-629">Value indicating response to process creations originating from PSExec and WMI commands.</span></span> <span data-ttu-id="6e0e5-630">可取值为：`userDefined`、`enable`、`auditMode`。</span><span class="sxs-lookup"><span data-stu-id="6e0e5-630">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="6e0e5-631">defenderUntrustedUSBProcessType</span><span class="sxs-lookup"><span data-stu-id="6e0e5-631">defenderUntrustedUSBProcessType</span></span>|[<span data-ttu-id="6e0e5-632">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="6e0e5-632">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="6e0e5-633">值，该值指示从 USB 运行的受信任和无符号流程的响应。</span><span class="sxs-lookup"><span data-stu-id="6e0e5-633">Value indicating response to untrusted and unsigned processes that run from USB.</span></span> <span data-ttu-id="6e0e5-634">可取值为：`userDefined`、`block`、`auditMode`。</span><span class="sxs-lookup"><span data-stu-id="6e0e5-634">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="6e0e5-635">defenderUntrustedUSBProcess</span><span class="sxs-lookup"><span data-stu-id="6e0e5-635">defenderUntrustedUSBProcess</span></span>|[<span data-ttu-id="6e0e5-636">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="6e0e5-636">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="6e0e5-637">值，该值指示从 USB 运行的受信任和无符号流程的响应。</span><span class="sxs-lookup"><span data-stu-id="6e0e5-637">Value indicating response to untrusted and unsigned processes that run from USB.</span></span> <span data-ttu-id="6e0e5-638">可取值为：`userDefined`、`enable`、`auditMode`。</span><span class="sxs-lookup"><span data-stu-id="6e0e5-638">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="6e0e5-639">defenderUntrustedExecutableType</span><span class="sxs-lookup"><span data-stu-id="6e0e5-639">defenderUntrustedExecutableType</span></span>|[<span data-ttu-id="6e0e5-640">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="6e0e5-640">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="6e0e5-641">值，该值指示响应可执行文件的传播、 年龄或受信任的列表不满足条件。</span><span class="sxs-lookup"><span data-stu-id="6e0e5-641">Value indicating response to executables that don't meet a prevalence, age, or trusted list criteria.</span></span> <span data-ttu-id="6e0e5-642">可取值为：`userDefined`、`block`、`auditMode`。</span><span class="sxs-lookup"><span data-stu-id="6e0e5-642">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="6e0e5-643">defenderUntrustedExecutable</span><span class="sxs-lookup"><span data-stu-id="6e0e5-643">defenderUntrustedExecutable</span></span>|[<span data-ttu-id="6e0e5-644">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="6e0e5-644">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="6e0e5-645">值，该值指示响应可执行文件的传播、 年龄或受信任的列表不满足条件。</span><span class="sxs-lookup"><span data-stu-id="6e0e5-645">Value indicating response to executables that don't meet a prevalence, age, or trusted list criteria.</span></span> <span data-ttu-id="6e0e5-646">可取值为：`userDefined`、`enable`、`auditMode`。</span><span class="sxs-lookup"><span data-stu-id="6e0e5-646">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="6e0e5-647">defenderEmailContentExecutionType</span><span class="sxs-lookup"><span data-stu-id="6e0e5-647">defenderEmailContentExecutionType</span></span>|[<span data-ttu-id="6e0e5-648">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="6e0e5-648">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="6e0e5-649">指示是否应该从电子邮件 （客户端 webmail/邮件） 放执行 （exe、 dll，ps、 js、 vbs 等） 的可执行内容的值。</span><span class="sxs-lookup"><span data-stu-id="6e0e5-649">Value indicating if execution of executable content (exe, dll, ps, js, vbs, etc) should be dropped from email (webmail/mail-client).</span></span> <span data-ttu-id="6e0e5-650">可取值为：`userDefined`、`block`、`auditMode`。</span><span class="sxs-lookup"><span data-stu-id="6e0e5-650">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="6e0e5-651">defenderEmailContentExecution</span><span class="sxs-lookup"><span data-stu-id="6e0e5-651">defenderEmailContentExecution</span></span>|[<span data-ttu-id="6e0e5-652">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="6e0e5-652">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="6e0e5-653">指示是否应该从电子邮件 （客户端 webmail/邮件） 放执行 （exe、 dll，ps、 js、 vbs 等） 的可执行内容的值。</span><span class="sxs-lookup"><span data-stu-id="6e0e5-653">Value indicating if execution of executable content (exe, dll, ps, js, vbs, etc) should be dropped from email (webmail/mail-client).</span></span> <span data-ttu-id="6e0e5-654">可取值为：`userDefined`、`enable`、`auditMode`。</span><span class="sxs-lookup"><span data-stu-id="6e0e5-654">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="6e0e5-655">defenderAdvancedRansomewareProtectionType</span><span class="sxs-lookup"><span data-stu-id="6e0e5-655">defenderAdvancedRansomewareProtectionType</span></span>|[<span data-ttu-id="6e0e5-656">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="6e0e5-656">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="6e0e5-657">指示使用高级防范 ransomeware 值。</span><span class="sxs-lookup"><span data-stu-id="6e0e5-657">Value indicating use of advanced protection against ransomeware.</span></span> <span data-ttu-id="6e0e5-658">可取值为：`userDefined`、`enable`、`auditMode`。</span><span class="sxs-lookup"><span data-stu-id="6e0e5-658">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="6e0e5-659">defenderGuardMyFoldersType</span><span class="sxs-lookup"><span data-stu-id="6e0e5-659">defenderGuardMyFoldersType</span></span>|[<span data-ttu-id="6e0e5-660">folderProtectionType</span><span class="sxs-lookup"><span data-stu-id="6e0e5-660">folderProtectionType</span></span>](../resources/intune-deviceconfig-folderprotectiontype.md)|<span data-ttu-id="6e0e5-661">指示受保护的文件夹的行为的值。</span><span class="sxs-lookup"><span data-stu-id="6e0e5-661">Value indicating the behavior of protected folders.</span></span> <span data-ttu-id="6e0e5-662">可取值为：`userDefined`、`enable`、`auditMode`、`blockDiskModification`、`auditDiskModification`。</span><span class="sxs-lookup"><span data-stu-id="6e0e5-662">Possible values are: `userDefined`, `enable`, `auditMode`, `blockDiskModification`, `auditDiskModification`.</span></span>|
|<span data-ttu-id="6e0e5-663">defenderGuardedFoldersAllowedAppPaths</span><span class="sxs-lookup"><span data-stu-id="6e0e5-663">defenderGuardedFoldersAllowedAppPaths</span></span>|<span data-ttu-id="6e0e5-664">String 集合</span><span class="sxs-lookup"><span data-stu-id="6e0e5-664">String collection</span></span>|<span data-ttu-id="6e0e5-665">允许访问受保护文件夹的 exe 路径列表</span><span class="sxs-lookup"><span data-stu-id="6e0e5-665">List of paths to exe that are allowed to access protected folders</span></span>|
|<span data-ttu-id="6e0e5-666">defenderAdditionalGuardedFolders</span><span class="sxs-lookup"><span data-stu-id="6e0e5-666">defenderAdditionalGuardedFolders</span></span>|<span data-ttu-id="6e0e5-667">String 集合</span><span class="sxs-lookup"><span data-stu-id="6e0e5-667">String collection</span></span>|<span data-ttu-id="6e0e5-668">要添加到受保护文件夹列表的文件夹路径列表</span><span class="sxs-lookup"><span data-stu-id="6e0e5-668">List of folder paths to be added to the list of protected folders</span></span>|
|<span data-ttu-id="6e0e5-669">defenderNetworkProtectionType</span><span class="sxs-lookup"><span data-stu-id="6e0e5-669">defenderNetworkProtectionType</span></span>|[<span data-ttu-id="6e0e5-670">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="6e0e5-670">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="6e0e5-671">指示 NetworkProtection 的行为的值。</span><span class="sxs-lookup"><span data-stu-id="6e0e5-671">Value indicating the behavior of NetworkProtection.</span></span> <span data-ttu-id="6e0e5-672">可取值为：`userDefined`、`enable`、`auditMode`。</span><span class="sxs-lookup"><span data-stu-id="6e0e5-672">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="6e0e5-673">defenderExploitProtectionXml</span><span class="sxs-lookup"><span data-stu-id="6e0e5-673">defenderExploitProtectionXml</span></span>|<span data-ttu-id="6e0e5-674">Binary</span><span class="sxs-lookup"><span data-stu-id="6e0e5-674">Binary</span></span>|<span data-ttu-id="6e0e5-675">包含有关 Exploit Protection 详细信息的 xml 内容。</span><span class="sxs-lookup"><span data-stu-id="6e0e5-675">Xml content containing information regarding exploit protection details.</span></span>|
|<span data-ttu-id="6e0e5-676">defenderExploitProtectionXmlFileName</span><span class="sxs-lookup"><span data-stu-id="6e0e5-676">defenderExploitProtectionXmlFileName</span></span>|<span data-ttu-id="6e0e5-677">String</span><span class="sxs-lookup"><span data-stu-id="6e0e5-677">String</span></span>|<span data-ttu-id="6e0e5-678">从中获取 DefenderExploitProtectionXml 的文件的名称。</span><span class="sxs-lookup"><span data-stu-id="6e0e5-678">Name of the file from which DefenderExploitProtectionXml was obtained.</span></span>|
|<span data-ttu-id="6e0e5-679">defenderSecurityCenterBlockExploitProtectionOverride</span><span class="sxs-lookup"><span data-stu-id="6e0e5-679">defenderSecurityCenterBlockExploitProtectionOverride</span></span>|<span data-ttu-id="6e0e5-680">Boolean</span><span class="sxs-lookup"><span data-stu-id="6e0e5-680">Boolean</span></span>|<span data-ttu-id="6e0e5-681">指示是否阻止用户覆盖 Exploit Protection 设置。</span><span class="sxs-lookup"><span data-stu-id="6e0e5-681">Indicates whether or not to block user from overriding Exploit Protection settings.</span></span>|
|<span data-ttu-id="6e0e5-682">appLockerApplicationControl</span><span class="sxs-lookup"><span data-stu-id="6e0e5-682">appLockerApplicationControl</span></span>|[<span data-ttu-id="6e0e5-683">appLockerApplicationControlType</span><span class="sxs-lookup"><span data-stu-id="6e0e5-683">appLockerApplicationControlType</span></span>](../resources/intune-deviceconfig-applockerapplicationcontroltype.md)|<span data-ttu-id="6e0e5-684">使管理员能够选择在设备上允许哪些类型的应用。</span><span class="sxs-lookup"><span data-stu-id="6e0e5-684">Enables the Admin to choose what types of app to allow on devices.</span></span> <span data-ttu-id="6e0e5-685">可取值为：`notConfigured`、`enforceComponentsAndStoreApps`、`auditComponentsAndStoreApps`、`enforceComponentsStoreAppsAndSmartlocker`、`auditComponentsStoreAppsAndSmartlocker`。</span><span class="sxs-lookup"><span data-stu-id="6e0e5-685">Possible values are: `notConfigured`, `enforceComponentsAndStoreApps`, `auditComponentsAndStoreApps`, `enforceComponentsStoreAppsAndSmartlocker`, `auditComponentsStoreAppsAndSmartlocker`.</span></span>|
|<span data-ttu-id="6e0e5-686">deviceGuardLocalSystemAuthorityCredentialGuardSettings</span><span class="sxs-lookup"><span data-stu-id="6e0e5-686">deviceGuardLocalSystemAuthorityCredentialGuardSettings</span></span>|[<span data-ttu-id="6e0e5-687">deviceGuardLocalSystemAuthorityCredentialGuardType</span><span class="sxs-lookup"><span data-stu-id="6e0e5-687">deviceGuardLocalSystemAuthorityCredentialGuardType</span></span>](../resources/intune-deviceconfig-deviceguardlocalsystemauthoritycredentialguardtype.md)|<span data-ttu-id="6e0e5-688">在凭据 Guard 时同时启用对安全启动和虚拟化基于安全平台安全级别打开。</span><span class="sxs-lookup"><span data-stu-id="6e0e5-688">Turn on Credential Guard when Platform Security Level with Secure Boot and Virtualization Based Security are both enabled.</span></span> <span data-ttu-id="6e0e5-689">可取值为：`notConfigured`、`enableWithUEFILock`、`enableWithoutUEFILock`。</span><span class="sxs-lookup"><span data-stu-id="6e0e5-689">Possible values are: `notConfigured`, `enableWithUEFILock`, `enableWithoutUEFILock`.</span></span>|
|<span data-ttu-id="6e0e5-690">deviceGuardEnableVirtualizationBasedSecurity</span><span class="sxs-lookup"><span data-stu-id="6e0e5-690">deviceGuardEnableVirtualizationBasedSecurity</span></span>|<span data-ttu-id="6e0e5-691">Boolean</span><span class="sxs-lookup"><span data-stu-id="6e0e5-691">Boolean</span></span>|<span data-ttu-id="6e0e5-692">虚拟化选项会启用基于 Security(VBS)。</span><span class="sxs-lookup"><span data-stu-id="6e0e5-692">Turns On Virtualization Based Security(VBS).</span></span>|
|<span data-ttu-id="6e0e5-693">deviceGuardEnableSecureBootWithDMA</span><span class="sxs-lookup"><span data-stu-id="6e0e5-693">deviceGuardEnableSecureBootWithDMA</span></span>|<span data-ttu-id="6e0e5-694">Boolean</span><span class="sxs-lookup"><span data-stu-id="6e0e5-694">Boolean</span></span>|<span data-ttu-id="6e0e5-695">指定是否将在下次重新启动启用平台安全级别。</span><span class="sxs-lookup"><span data-stu-id="6e0e5-695">Specifies whether Platform Security Level is enabled at next reboot.</span></span>|
|<span data-ttu-id="6e0e5-696">smartScreenEnableInShell</span><span class="sxs-lookup"><span data-stu-id="6e0e5-696">smartScreenEnableInShell</span></span>|<span data-ttu-id="6e0e5-697">Boolean</span><span class="sxs-lookup"><span data-stu-id="6e0e5-697">Boolean</span></span>|<span data-ttu-id="6e0e5-698">允许 IT 管理员配置适用于 Windows 的 SmartScreen。</span><span class="sxs-lookup"><span data-stu-id="6e0e5-698">Allows IT Admins to configure SmartScreen for Windows.</span></span>|
|<span data-ttu-id="6e0e5-699">smartScreenBlockOverrideForFiles</span><span class="sxs-lookup"><span data-stu-id="6e0e5-699">smartScreenBlockOverrideForFiles</span></span>|<span data-ttu-id="6e0e5-700">Boolean</span><span class="sxs-lookup"><span data-stu-id="6e0e5-700">Boolean</span></span>|<span data-ttu-id="6e0e5-701">允许 IT 管理员控制用户是否可以忽略 SmartScreen 警告并运行恶意文件。</span><span class="sxs-lookup"><span data-stu-id="6e0e5-701">Allows IT Admins to control whether users can can ignore SmartScreen warnings and run malicious files.</span></span>|
|<span data-ttu-id="6e0e5-702">applicationGuardEnabled</span><span class="sxs-lookup"><span data-stu-id="6e0e5-702">applicationGuardEnabled</span></span>|<span data-ttu-id="6e0e5-703">Boolean</span><span class="sxs-lookup"><span data-stu-id="6e0e5-703">Boolean</span></span>|<span data-ttu-id="6e0e5-704">启用 Windows Defender 应用程序防护</span><span class="sxs-lookup"><span data-stu-id="6e0e5-704">Enable Windows Defender Application Guard</span></span>|
|<span data-ttu-id="6e0e5-705">applicationGuardEnabledOptions</span><span class="sxs-lookup"><span data-stu-id="6e0e5-705">applicationGuardEnabledOptions</span></span>|[<span data-ttu-id="6e0e5-706">applicationGuardEnabledOptions</span><span class="sxs-lookup"><span data-stu-id="6e0e5-706">applicationGuardEnabledOptions</span></span>](../resources/intune-deviceconfig-applicationguardenabledoptions.md)|<span data-ttu-id="6e0e5-707">Windows Defender 应用程序 Guard 启用更高版本的 Windows 版本。</span><span class="sxs-lookup"><span data-stu-id="6e0e5-707">Enable Windows Defender Application Guard for newer Windows builds.</span></span> <span data-ttu-id="6e0e5-708">可取值为：`notConfigured`、`enabledForEdge`、`enabledForOffice`、`enabledForEdgeAndOffice`。</span><span class="sxs-lookup"><span data-stu-id="6e0e5-708">Possible values are: `notConfigured`, `enabledForEdge`, `enabledForOffice`, `enabledForEdgeAndOffice`.</span></span>|
|<span data-ttu-id="6e0e5-709">applicationGuardBlockFileTransfer</span><span class="sxs-lookup"><span data-stu-id="6e0e5-709">applicationGuardBlockFileTransfer</span></span>|[<span data-ttu-id="6e0e5-710">applicationGuardBlockFileTransferType</span><span class="sxs-lookup"><span data-stu-id="6e0e5-710">applicationGuardBlockFileTransferType</span></span>](../resources/intune-deviceconfig-applicationguardblockfiletransfertype.md)|<span data-ttu-id="6e0e5-711">阻止传输图像文件、 文本文件或两者到剪贴板。</span><span class="sxs-lookup"><span data-stu-id="6e0e5-711">Block clipboard to transfer image file, text file or neither of them.</span></span> <span data-ttu-id="6e0e5-712">可取值为：`notConfigured`、`blockImageAndTextFile`、`blockImageFile`、`blockNone`、`blockTextFile`。</span><span class="sxs-lookup"><span data-stu-id="6e0e5-712">Possible values are: `notConfigured`, `blockImageAndTextFile`, `blockImageFile`, `blockNone`, `blockTextFile`.</span></span>|
|<span data-ttu-id="6e0e5-713">applicationGuardBlockNonEnterpriseContent</span><span class="sxs-lookup"><span data-stu-id="6e0e5-713">applicationGuardBlockNonEnterpriseContent</span></span>|<span data-ttu-id="6e0e5-714">Boolean</span><span class="sxs-lookup"><span data-stu-id="6e0e5-714">Boolean</span></span>|<span data-ttu-id="6e0e5-715">阻止企业站点加载非企业内容，例如第三方插件</span><span class="sxs-lookup"><span data-stu-id="6e0e5-715">Block enterprise sites to load non-enterprise content, such as third party plug-ins</span></span>|
|<span data-ttu-id="6e0e5-716">applicationGuardAllowPersistence</span><span class="sxs-lookup"><span data-stu-id="6e0e5-716">applicationGuardAllowPersistence</span></span>|<span data-ttu-id="6e0e5-717">Boolean</span><span class="sxs-lookup"><span data-stu-id="6e0e5-717">Boolean</span></span>|<span data-ttu-id="6e0e5-718">允许 App Guard 容器（收藏夹、Cookie、Web 密码等）内的持久用户生成数据</span><span class="sxs-lookup"><span data-stu-id="6e0e5-718">Allow persisting user generated data inside the App Guard Containter (favorites, cookies, web passwords, etc.)</span></span>|
|<span data-ttu-id="6e0e5-719">applicationGuardForceAuditing</span><span class="sxs-lookup"><span data-stu-id="6e0e5-719">applicationGuardForceAuditing</span></span>|<span data-ttu-id="6e0e5-720">Boolean</span><span class="sxs-lookup"><span data-stu-id="6e0e5-720">Boolean</span></span>|<span data-ttu-id="6e0e5-721">强制审核将存留 Windows 日志和事件以满足安全/符合性条件（示例事件是用户登录注销、特权使用、软件安装、系统更改等）</span><span class="sxs-lookup"><span data-stu-id="6e0e5-721">Force auditing will persist Windows logs and events to meet security/compliance criteria (sample events are user login-logoff, use of privilege rights, software installation, system changes, etc.)</span></span>|
|<span data-ttu-id="6e0e5-722">applicationGuardBlockClipboardSharing</span><span class="sxs-lookup"><span data-stu-id="6e0e5-722">applicationGuardBlockClipboardSharing</span></span>|[<span data-ttu-id="6e0e5-723">applicationGuardBlockClipboardSharingType</span><span class="sxs-lookup"><span data-stu-id="6e0e5-723">applicationGuardBlockClipboardSharingType</span></span>](../resources/intune-deviceconfig-applicationguardblockclipboardsharingtype.md)|<span data-ttu-id="6e0e5-724">阻止剪贴板将数据从主机共享到容器或从容器共享到主机，或阻止两种方式，或两种方式均不阻止。</span><span class="sxs-lookup"><span data-stu-id="6e0e5-724">Block clipboard to share data from Host to Container, or from Container to Host, or both ways, or neither ways.</span></span> <span data-ttu-id="6e0e5-725">可取值为：`notConfigured`、`blockBoth`、`blockHostToContainer`、`blockContainerToHost`、`blockNone`。</span><span class="sxs-lookup"><span data-stu-id="6e0e5-725">Possible values are: `notConfigured`, `blockBoth`, `blockHostToContainer`, `blockContainerToHost`, `blockNone`.</span></span>|
|<span data-ttu-id="6e0e5-726">applicationGuardAllowPrintToPDF</span><span class="sxs-lookup"><span data-stu-id="6e0e5-726">applicationGuardAllowPrintToPDF</span></span>|<span data-ttu-id="6e0e5-727">Boolean</span><span class="sxs-lookup"><span data-stu-id="6e0e5-727">Boolean</span></span>|<span data-ttu-id="6e0e5-728">允许从容器打印为 PDF 格式</span><span class="sxs-lookup"><span data-stu-id="6e0e5-728">Allow printing to PDF from Container</span></span>|
|<span data-ttu-id="6e0e5-729">applicationGuardAllowPrintToXPS</span><span class="sxs-lookup"><span data-stu-id="6e0e5-729">applicationGuardAllowPrintToXPS</span></span>|<span data-ttu-id="6e0e5-730">Boolean</span><span class="sxs-lookup"><span data-stu-id="6e0e5-730">Boolean</span></span>|<span data-ttu-id="6e0e5-731">允许从容器打印为 XPS 格式</span><span class="sxs-lookup"><span data-stu-id="6e0e5-731">Allow printing to XPS from Container</span></span>|
|<span data-ttu-id="6e0e5-732">applicationGuardAllowPrintToLocalPrinters</span><span class="sxs-lookup"><span data-stu-id="6e0e5-732">applicationGuardAllowPrintToLocalPrinters</span></span>|<span data-ttu-id="6e0e5-733">Boolean</span><span class="sxs-lookup"><span data-stu-id="6e0e5-733">Boolean</span></span>|<span data-ttu-id="6e0e5-734">允许从容器打印到本地打印机</span><span class="sxs-lookup"><span data-stu-id="6e0e5-734">Allow printing to Local Printers from Container</span></span>|
|<span data-ttu-id="6e0e5-735">applicationGuardAllowPrintToNetworkPrinters</span><span class="sxs-lookup"><span data-stu-id="6e0e5-735">applicationGuardAllowPrintToNetworkPrinters</span></span>|<span data-ttu-id="6e0e5-736">Boolean</span><span class="sxs-lookup"><span data-stu-id="6e0e5-736">Boolean</span></span>|<span data-ttu-id="6e0e5-737">允许从容器打印到网络打印机</span><span class="sxs-lookup"><span data-stu-id="6e0e5-737">Allow printing to Network Printers from Container</span></span>|
|<span data-ttu-id="6e0e5-738">applicationGuardAllowVirtualGPU</span><span class="sxs-lookup"><span data-stu-id="6e0e5-738">applicationGuardAllowVirtualGPU</span></span>|<span data-ttu-id="6e0e5-739">Boolean</span><span class="sxs-lookup"><span data-stu-id="6e0e5-739">Boolean</span></span>|<span data-ttu-id="6e0e5-740">允许应用程序 guard 用于虚拟 GPU</span><span class="sxs-lookup"><span data-stu-id="6e0e5-740">Allow application guard to use virtual GPU</span></span>|
|<span data-ttu-id="6e0e5-741">applicationGuardAllowFileSaveOnHost</span><span class="sxs-lookup"><span data-stu-id="6e0e5-741">applicationGuardAllowFileSaveOnHost</span></span>|<span data-ttu-id="6e0e5-742">Boolean</span><span class="sxs-lookup"><span data-stu-id="6e0e5-742">Boolean</span></span>|<span data-ttu-id="6e0e5-743">允许用户从应用程序 guard 容器中的边缘下载文件并将其保存在主机上文件系统</span><span class="sxs-lookup"><span data-stu-id="6e0e5-743">Allow users to download files from Edge in the application guard container and save them on the host file system</span></span>|
|<span data-ttu-id="6e0e5-744">bitLockerDisableWarningForOtherDiskEncryption</span><span class="sxs-lookup"><span data-stu-id="6e0e5-744">bitLockerDisableWarningForOtherDiskEncryption</span></span>|<span data-ttu-id="6e0e5-745">Boolean</span><span class="sxs-lookup"><span data-stu-id="6e0e5-745">Boolean</span></span>|<span data-ttu-id="6e0e5-746">允许管理员禁用对用户计算机上其他磁盘加密的警告提示。</span><span class="sxs-lookup"><span data-stu-id="6e0e5-746">Allows the Admin to disable the warning prompt for other disk encryption on the user machines.</span></span>|
|<span data-ttu-id="6e0e5-747">bitLockerEnableStorageCardEncryptionOnMobile</span><span class="sxs-lookup"><span data-stu-id="6e0e5-747">bitLockerEnableStorageCardEncryptionOnMobile</span></span>|<span data-ttu-id="6e0e5-748">Boolean</span><span class="sxs-lookup"><span data-stu-id="6e0e5-748">Boolean</span></span>|<span data-ttu-id="6e0e5-749">允许管理员要求使用 BitLocker 开启加密功能。</span><span class="sxs-lookup"><span data-stu-id="6e0e5-749">Allows the admin to require encryption to be turned on using BitLocker.</span></span> <span data-ttu-id="6e0e5-750">此策略仅适用于移动 SKU。</span><span class="sxs-lookup"><span data-stu-id="6e0e5-750">This policy is valid only for a mobile SKU.</span></span>|
|<span data-ttu-id="6e0e5-751">bitLockerEncryptDevice</span><span class="sxs-lookup"><span data-stu-id="6e0e5-751">bitLockerEncryptDevice</span></span>|<span data-ttu-id="6e0e5-752">Boolean</span><span class="sxs-lookup"><span data-stu-id="6e0e5-752">Boolean</span></span>|<span data-ttu-id="6e0e5-753">允许管理员要求使用 BitLocker 开启加密功能。</span><span class="sxs-lookup"><span data-stu-id="6e0e5-753">Allows the admin to require encryption to be turned on using BitLocker.</span></span>|
|<span data-ttu-id="6e0e5-754">bitLockerSystemDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="6e0e5-754">bitLockerSystemDrivePolicy</span></span>|[<span data-ttu-id="6e0e5-755">bitLockerSystemDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="6e0e5-755">bitLockerSystemDrivePolicy</span></span>](../resources/intune-deviceconfig-bitlockersystemdrivepolicy.md)|<span data-ttu-id="6e0e5-756">BitLocker 系统驱动器策略。</span><span class="sxs-lookup"><span data-stu-id="6e0e5-756">BitLocker System Drive Policy.</span></span>|
|<span data-ttu-id="6e0e5-757">bitLockerFixedDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="6e0e5-757">bitLockerFixedDrivePolicy</span></span>|[<span data-ttu-id="6e0e5-758">bitLockerFixedDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="6e0e5-758">bitLockerFixedDrivePolicy</span></span>](../resources/intune-deviceconfig-bitlockerfixeddrivepolicy.md)|<span data-ttu-id="6e0e5-759">BitLocker 固定驱动器策略。</span><span class="sxs-lookup"><span data-stu-id="6e0e5-759">BitLocker Fixed Drive Policy.</span></span>|
|<span data-ttu-id="6e0e5-760">bitLockerRemovableDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="6e0e5-760">bitLockerRemovableDrivePolicy</span></span>|[<span data-ttu-id="6e0e5-761">bitLockerRemovableDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="6e0e5-761">bitLockerRemovableDrivePolicy</span></span>](../resources/intune-deviceconfig-bitlockerremovabledrivepolicy.md)|<span data-ttu-id="6e0e5-762">BitLocker 可移动驱动器策略。</span><span class="sxs-lookup"><span data-stu-id="6e0e5-762">BitLocker Removable Drive Policy.</span></span>|



## <a name="response"></a><span data-ttu-id="6e0e5-763">响应</span><span class="sxs-lookup"><span data-stu-id="6e0e5-763">Response</span></span>
<span data-ttu-id="6e0e5-764">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="6e0e5-764">If successful, this method returns a `200 OK` response code and an updated [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6e0e5-765">示例</span><span class="sxs-lookup"><span data-stu-id="6e0e5-765">Example</span></span>
### <a name="request"></a><span data-ttu-id="6e0e5-766">请求</span><span class="sxs-lookup"><span data-stu-id="6e0e5-766">Request</span></span>
<span data-ttu-id="6e0e5-767">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="6e0e5-767">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 26312

{
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
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
  "localSecurityOptionsEnableAdministratorAccount": true,
  "localSecurityOptionsAdministratorAccountName": "Local Security Options Administrator Account Name value",
  "localSecurityOptionsEnableGuestAccount": true,
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
  "lanManagerWorkstationEnableInsecureGuestLogons": true,
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

### <a name="response"></a><span data-ttu-id="6e0e5-768">响应</span><span class="sxs-lookup"><span data-stu-id="6e0e5-768">Response</span></span>
<span data-ttu-id="6e0e5-p194">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="6e0e5-p194">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 26499

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
  "localSecurityOptionsEnableAdministratorAccount": true,
  "localSecurityOptionsAdministratorAccountName": "Local Security Options Administrator Account Name value",
  "localSecurityOptionsEnableGuestAccount": true,
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
  "lanManagerWorkstationEnableInsecureGuestLogons": true,
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





