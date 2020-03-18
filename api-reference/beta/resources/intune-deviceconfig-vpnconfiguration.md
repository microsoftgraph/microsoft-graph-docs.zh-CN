---
title: vpnConfiguration 资源类型
description: 基本 VPN 配置文件。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 03deaea51f125fddd8ed47e241c0d2fe63f1c6c5
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42787402"
---
# <a name="vpnconfiguration-resource-type"></a><span data-ttu-id="83ff7-103">vpnConfiguration 资源类型</span><span class="sxs-lookup"><span data-stu-id="83ff7-103">vpnConfiguration resource type</span></span>

> <span data-ttu-id="83ff7-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="83ff7-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="83ff7-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="83ff7-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="83ff7-106">基本 VPN 配置文件。</span><span class="sxs-lookup"><span data-stu-id="83ff7-106">Base VPN Configuration profile.</span></span>


<span data-ttu-id="83ff7-107">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="83ff7-107">Inherits from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>

## <a name="methods"></a><span data-ttu-id="83ff7-108">方法</span><span class="sxs-lookup"><span data-stu-id="83ff7-108">Methods</span></span>
|<span data-ttu-id="83ff7-109">方法</span><span class="sxs-lookup"><span data-stu-id="83ff7-109">Method</span></span>|<span data-ttu-id="83ff7-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="83ff7-110">Return Type</span></span>|<span data-ttu-id="83ff7-111">说明</span><span class="sxs-lookup"><span data-stu-id="83ff7-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="83ff7-112">列出 vpnConfigurations</span><span class="sxs-lookup"><span data-stu-id="83ff7-112">List vpnConfigurations</span></span>](../api/intune-deviceconfig-vpnconfiguration-list.md)|<span data-ttu-id="83ff7-113">[vpnConfiguration](../resources/intune-deviceconfig-vpnconfiguration.md)集合</span><span class="sxs-lookup"><span data-stu-id="83ff7-113">[vpnConfiguration](../resources/intune-deviceconfig-vpnconfiguration.md) collection</span></span>|<span data-ttu-id="83ff7-114">列出[vpnConfiguration](../resources/intune-deviceconfig-vpnconfiguration.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="83ff7-114">List properties and relationships of the [vpnConfiguration](../resources/intune-deviceconfig-vpnconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="83ff7-115">获取 vpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="83ff7-115">Get vpnConfiguration</span></span>](../api/intune-deviceconfig-vpnconfiguration-get.md)|[<span data-ttu-id="83ff7-116">vpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="83ff7-116">vpnConfiguration</span></span>](../resources/intune-deviceconfig-vpnconfiguration.md)|<span data-ttu-id="83ff7-117">读取[vpnConfiguration](../resources/intune-deviceconfig-vpnconfiguration.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="83ff7-117">Read properties and relationships of the [vpnConfiguration](../resources/intune-deviceconfig-vpnconfiguration.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="83ff7-118">属性</span><span class="sxs-lookup"><span data-stu-id="83ff7-118">Properties</span></span>
|<span data-ttu-id="83ff7-119">属性</span><span class="sxs-lookup"><span data-stu-id="83ff7-119">Property</span></span>|<span data-ttu-id="83ff7-120">类型</span><span class="sxs-lookup"><span data-stu-id="83ff7-120">Type</span></span>|<span data-ttu-id="83ff7-121">说明</span><span class="sxs-lookup"><span data-stu-id="83ff7-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="83ff7-122">id</span><span class="sxs-lookup"><span data-stu-id="83ff7-122">id</span></span>|<span data-ttu-id="83ff7-123">字符串</span><span class="sxs-lookup"><span data-stu-id="83ff7-123">String</span></span>|<span data-ttu-id="83ff7-124">实体的键。</span><span class="sxs-lookup"><span data-stu-id="83ff7-124">Key of the entity.</span></span> <span data-ttu-id="83ff7-125">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="83ff7-125">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="83ff7-126">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="83ff7-126">lastModifiedDateTime</span></span>|<span data-ttu-id="83ff7-127">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="83ff7-127">DateTimeOffset</span></span>|<span data-ttu-id="83ff7-128">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="83ff7-128">DateTime the object was last modified.</span></span> <span data-ttu-id="83ff7-129">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="83ff7-129">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="83ff7-130">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="83ff7-130">roleScopeTagIds</span></span>|<span data-ttu-id="83ff7-131">String collection</span><span class="sxs-lookup"><span data-stu-id="83ff7-131">String collection</span></span>|<span data-ttu-id="83ff7-132">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="83ff7-132">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="83ff7-133">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="83ff7-133">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="83ff7-134">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="83ff7-134">supportsScopeTags</span></span>|<span data-ttu-id="83ff7-135">布尔值</span><span class="sxs-lookup"><span data-stu-id="83ff7-135">Boolean</span></span>|<span data-ttu-id="83ff7-136">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="83ff7-136">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="83ff7-137">如果此值为 false，则不允许分配给 ScopeTags 属性，并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="83ff7-137">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="83ff7-138">这适用于在 Silverlight 中创建的旧版策略，可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="83ff7-138">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="83ff7-139">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="83ff7-139">This property is read-only.</span></span> <span data-ttu-id="83ff7-140">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="83ff7-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="83ff7-141">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="83ff7-141">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="83ff7-142">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="83ff7-142">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="83ff7-143">适用于此策略的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="83ff7-143">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="83ff7-144">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="83ff7-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="83ff7-145">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="83ff7-145">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="83ff7-146">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="83ff7-146">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="83ff7-147">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="83ff7-147">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="83ff7-148">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="83ff7-148">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="83ff7-149">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="83ff7-149">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="83ff7-150">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="83ff7-150">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="83ff7-151">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="83ff7-151">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="83ff7-152">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="83ff7-152">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="83ff7-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="83ff7-153">createdDateTime</span></span>|<span data-ttu-id="83ff7-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="83ff7-154">DateTimeOffset</span></span>|<span data-ttu-id="83ff7-155">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="83ff7-155">DateTime the object was created.</span></span> <span data-ttu-id="83ff7-156">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="83ff7-156">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="83ff7-157">说明</span><span class="sxs-lookup"><span data-stu-id="83ff7-157">description</span></span>|<span data-ttu-id="83ff7-158">String</span><span class="sxs-lookup"><span data-stu-id="83ff7-158">String</span></span>|<span data-ttu-id="83ff7-159">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="83ff7-159">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="83ff7-160">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="83ff7-160">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="83ff7-161">displayName</span><span class="sxs-lookup"><span data-stu-id="83ff7-161">displayName</span></span>|<span data-ttu-id="83ff7-162">String</span><span class="sxs-lookup"><span data-stu-id="83ff7-162">String</span></span>|<span data-ttu-id="83ff7-163">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="83ff7-163">Admin provided name of the device configuration.</span></span> <span data-ttu-id="83ff7-164">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="83ff7-164">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="83ff7-165">version</span><span class="sxs-lookup"><span data-stu-id="83ff7-165">version</span></span>|<span data-ttu-id="83ff7-166">Int32</span><span class="sxs-lookup"><span data-stu-id="83ff7-166">Int32</span></span>|<span data-ttu-id="83ff7-167">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="83ff7-167">Version of the device configuration.</span></span> <span data-ttu-id="83ff7-168">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="83ff7-168">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="83ff7-169">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="83ff7-169">authenticationMethod</span></span>|[<span data-ttu-id="83ff7-170">vpnAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="83ff7-170">vpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-vpnauthenticationmethod.md)|<span data-ttu-id="83ff7-171">身份验证方法。</span><span class="sxs-lookup"><span data-stu-id="83ff7-171">Authentication method.</span></span> <span data-ttu-id="83ff7-172">可取值为：`certificate`、`usernameAndPassword`、`sharedSecret`、`derivedCredential`。</span><span class="sxs-lookup"><span data-stu-id="83ff7-172">Possible values are: `certificate`, `usernameAndPassword`, `sharedSecret`, `derivedCredential`.</span></span>|
|<span data-ttu-id="83ff7-173">connectionName</span><span class="sxs-lookup"><span data-stu-id="83ff7-173">connectionName</span></span>|<span data-ttu-id="83ff7-174">String</span><span class="sxs-lookup"><span data-stu-id="83ff7-174">String</span></span>|<span data-ttu-id="83ff7-175">向用户显示的连接名称。</span><span class="sxs-lookup"><span data-stu-id="83ff7-175">Connection name displayed to the user.</span></span>|
|<span data-ttu-id="83ff7-176">role</span><span class="sxs-lookup"><span data-stu-id="83ff7-176">role</span></span>|<span data-ttu-id="83ff7-177">String</span><span class="sxs-lookup"><span data-stu-id="83ff7-177">String</span></span>|<span data-ttu-id="83ff7-178">将 "连接类型" 设置为 "脉冲安全" 时的角色。</span><span class="sxs-lookup"><span data-stu-id="83ff7-178">Role when connection type is set to Pulse Secure.</span></span>|
|<span data-ttu-id="83ff7-179">型</span><span class="sxs-lookup"><span data-stu-id="83ff7-179">realm</span></span>|<span data-ttu-id="83ff7-180">String</span><span class="sxs-lookup"><span data-stu-id="83ff7-180">String</span></span>|<span data-ttu-id="83ff7-181">连接类型设置为脉冲安全时的领域。</span><span class="sxs-lookup"><span data-stu-id="83ff7-181">Realm when connection type is set to Pulse Secure.</span></span>|
|<span data-ttu-id="83ff7-182">台</span><span class="sxs-lookup"><span data-stu-id="83ff7-182">servers</span></span>|<span data-ttu-id="83ff7-183">[vpnServer](../resources/intune-deviceconfig-vpnserver.md)集合</span><span class="sxs-lookup"><span data-stu-id="83ff7-183">[vpnServer](../resources/intune-deviceconfig-vpnserver.md) collection</span></span>|<span data-ttu-id="83ff7-184">网络上的 VPN 服务器的列表。</span><span class="sxs-lookup"><span data-stu-id="83ff7-184">List of VPN Servers on the network.</span></span> <span data-ttu-id="83ff7-185">请确保最终用户可以访问这些网络位置。</span><span class="sxs-lookup"><span data-stu-id="83ff7-185">Make sure end users can access these network locations.</span></span> <span data-ttu-id="83ff7-186">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="83ff7-186">This collection can contain a maximum of 500 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="83ff7-187">关系</span><span class="sxs-lookup"><span data-stu-id="83ff7-187">Relationships</span></span>
|<span data-ttu-id="83ff7-188">关系</span><span class="sxs-lookup"><span data-stu-id="83ff7-188">Relationship</span></span>|<span data-ttu-id="83ff7-189">类型</span><span class="sxs-lookup"><span data-stu-id="83ff7-189">Type</span></span>|<span data-ttu-id="83ff7-190">说明</span><span class="sxs-lookup"><span data-stu-id="83ff7-190">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="83ff7-191">groupAssignments</span><span class="sxs-lookup"><span data-stu-id="83ff7-191">groupAssignments</span></span>|<span data-ttu-id="83ff7-192">[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)集合</span><span class="sxs-lookup"><span data-stu-id="83ff7-192">[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) collection</span></span>|<span data-ttu-id="83ff7-193">设备配置文件的组分配列表。</span><span class="sxs-lookup"><span data-stu-id="83ff7-193">The list of group assignments for the device configuration profile.</span></span> <span data-ttu-id="83ff7-194">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="83ff7-194">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="83ff7-195">assignments</span><span class="sxs-lookup"><span data-stu-id="83ff7-195">assignments</span></span>|<span data-ttu-id="83ff7-196">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="83ff7-196">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection</span></span>|<span data-ttu-id="83ff7-197">设备配置文件的分配列表。</span><span class="sxs-lookup"><span data-stu-id="83ff7-197">The list of assignments for the device configuration profile.</span></span> <span data-ttu-id="83ff7-198">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="83ff7-198">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="83ff7-199">deviceStatuses</span><span class="sxs-lookup"><span data-stu-id="83ff7-199">deviceStatuses</span></span>|<span data-ttu-id="83ff7-200">[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) 集合</span><span class="sxs-lookup"><span data-stu-id="83ff7-200">[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) collection</span></span>|<span data-ttu-id="83ff7-201">按设备的设备配置安装状态。</span><span class="sxs-lookup"><span data-stu-id="83ff7-201">Device configuration installation status by device.</span></span> <span data-ttu-id="83ff7-202">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="83ff7-202">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="83ff7-203">userStatuses</span><span class="sxs-lookup"><span data-stu-id="83ff7-203">userStatuses</span></span>|<span data-ttu-id="83ff7-204">[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) 集合</span><span class="sxs-lookup"><span data-stu-id="83ff7-204">[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) collection</span></span>|<span data-ttu-id="83ff7-205">按用户的设备配置安装状态。</span><span class="sxs-lookup"><span data-stu-id="83ff7-205">Device configuration installation status by user.</span></span> <span data-ttu-id="83ff7-206">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="83ff7-206">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="83ff7-207">deviceStatusOverview</span><span class="sxs-lookup"><span data-stu-id="83ff7-207">deviceStatusOverview</span></span>|[<span data-ttu-id="83ff7-208">deviceConfigurationDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="83ff7-208">deviceConfigurationDeviceOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|<span data-ttu-id="83ff7-209">设备配置设备状态概述 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="83ff7-209">Device Configuration devices status overview Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="83ff7-210">userStatusOverview</span><span class="sxs-lookup"><span data-stu-id="83ff7-210">userStatusOverview</span></span>|[<span data-ttu-id="83ff7-211">deviceConfigurationUserOverview</span><span class="sxs-lookup"><span data-stu-id="83ff7-211">deviceConfigurationUserOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|<span data-ttu-id="83ff7-212">设备配置用户状态概述 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="83ff7-212">Device Configuration users status overview Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="83ff7-213">deviceSettingStateSummaries</span><span class="sxs-lookup"><span data-stu-id="83ff7-213">deviceSettingStateSummaries</span></span>|<span data-ttu-id="83ff7-214">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) 集合</span><span class="sxs-lookup"><span data-stu-id="83ff7-214">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) collection</span></span>|<span data-ttu-id="83ff7-215">设备配置设置状态设备摘要 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="83ff7-215">Device Configuration Setting State Device Summary Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|

## <a name="json-representation"></a><span data-ttu-id="83ff7-216">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="83ff7-216">JSON Representation</span></span>
<span data-ttu-id="83ff7-217">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="83ff7-217">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.vpnConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.vpnConfiguration",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "roleScopeTagIds": [
    "String"
  ],
  "supportsScopeTags": true,
  "deviceManagementApplicabilityRuleOsEdition": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsEdition",
    "osEditionTypes": [
      "String"
    ],
    "name": "String",
    "ruleType": "String"
  },
  "deviceManagementApplicabilityRuleOsVersion": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsVersion",
    "minOSVersion": "String",
    "maxOSVersion": "String",
    "name": "String",
    "ruleType": "String"
  },
  "deviceManagementApplicabilityRuleDeviceMode": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleDeviceMode",
    "deviceMode": "String",
    "name": "String",
    "ruleType": "String"
  },
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "displayName": "String",
  "version": 1024,
  "authenticationMethod": "String",
  "connectionName": "String",
  "role": "String",
  "realm": "String",
  "servers": [
    {
      "@odata.type": "microsoft.graph.vpnServer",
      "description": "String",
      "address": "String",
      "isDefaultServer": true
    }
  ]
}
```



