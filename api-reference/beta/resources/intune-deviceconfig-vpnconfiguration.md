---
title: vpnConfiguration 资源类型
description: 基本 VPN 配置文件。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 03cb730e465ce04ac798902c39827b325d2f28f6
ms.sourcegitcommit: f3dda172d95ef1eda8f6dd9e3ffdc7d3c0744c0a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/14/2020
ms.locfileid: "45124091"
---
# <a name="vpnconfiguration-resource-type"></a><span data-ttu-id="3407d-103">vpnConfiguration 资源类型</span><span class="sxs-lookup"><span data-stu-id="3407d-103">vpnConfiguration resource type</span></span>

<span data-ttu-id="3407d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3407d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3407d-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="3407d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3407d-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="3407d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3407d-107">基本 VPN 配置文件。</span><span class="sxs-lookup"><span data-stu-id="3407d-107">Base VPN Configuration profile.</span></span>


<span data-ttu-id="3407d-108">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3407d-108">Inherits from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>

## <a name="methods"></a><span data-ttu-id="3407d-109">方法</span><span class="sxs-lookup"><span data-stu-id="3407d-109">Methods</span></span>
|<span data-ttu-id="3407d-110">方法</span><span class="sxs-lookup"><span data-stu-id="3407d-110">Method</span></span>|<span data-ttu-id="3407d-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="3407d-111">Return Type</span></span>|<span data-ttu-id="3407d-112">说明</span><span class="sxs-lookup"><span data-stu-id="3407d-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="3407d-113">列出 vpnConfigurations</span><span class="sxs-lookup"><span data-stu-id="3407d-113">List vpnConfigurations</span></span>](../api/intune-deviceconfig-vpnconfiguration-list.md)|<span data-ttu-id="3407d-114">[vpnConfiguration](../resources/intune-deviceconfig-vpnconfiguration.md)集合</span><span class="sxs-lookup"><span data-stu-id="3407d-114">[vpnConfiguration](../resources/intune-deviceconfig-vpnconfiguration.md) collection</span></span>|<span data-ttu-id="3407d-115">列出[vpnConfiguration](../resources/intune-deviceconfig-vpnconfiguration.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="3407d-115">List properties and relationships of the [vpnConfiguration](../resources/intune-deviceconfig-vpnconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="3407d-116">获取 vpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="3407d-116">Get vpnConfiguration</span></span>](../api/intune-deviceconfig-vpnconfiguration-get.md)|[<span data-ttu-id="3407d-117">vpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="3407d-117">vpnConfiguration</span></span>](../resources/intune-deviceconfig-vpnconfiguration.md)|<span data-ttu-id="3407d-118">读取[vpnConfiguration](../resources/intune-deviceconfig-vpnconfiguration.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="3407d-118">Read properties and relationships of the [vpnConfiguration](../resources/intune-deviceconfig-vpnconfiguration.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="3407d-119">属性</span><span class="sxs-lookup"><span data-stu-id="3407d-119">Properties</span></span>
|<span data-ttu-id="3407d-120">属性</span><span class="sxs-lookup"><span data-stu-id="3407d-120">Property</span></span>|<span data-ttu-id="3407d-121">类型</span><span class="sxs-lookup"><span data-stu-id="3407d-121">Type</span></span>|<span data-ttu-id="3407d-122">说明</span><span class="sxs-lookup"><span data-stu-id="3407d-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3407d-123">id</span><span class="sxs-lookup"><span data-stu-id="3407d-123">id</span></span>|<span data-ttu-id="3407d-124">字符串</span><span class="sxs-lookup"><span data-stu-id="3407d-124">String</span></span>|<span data-ttu-id="3407d-125">实体的键。</span><span class="sxs-lookup"><span data-stu-id="3407d-125">Key of the entity.</span></span> <span data-ttu-id="3407d-126">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3407d-126">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3407d-127">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3407d-127">lastModifiedDateTime</span></span>|<span data-ttu-id="3407d-128">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3407d-128">DateTimeOffset</span></span>|<span data-ttu-id="3407d-129">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="3407d-129">DateTime the object was last modified.</span></span> <span data-ttu-id="3407d-130">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3407d-130">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3407d-131">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="3407d-131">roleScopeTagIds</span></span>|<span data-ttu-id="3407d-132">String collection</span><span class="sxs-lookup"><span data-stu-id="3407d-132">String collection</span></span>|<span data-ttu-id="3407d-133">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="3407d-133">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="3407d-134">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3407d-134">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3407d-135">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="3407d-135">supportsScopeTags</span></span>|<span data-ttu-id="3407d-136">Boolean</span><span class="sxs-lookup"><span data-stu-id="3407d-136">Boolean</span></span>|<span data-ttu-id="3407d-137">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="3407d-137">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="3407d-138">如果此值为 false，则不允许分配给 ScopeTags 属性，并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="3407d-138">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="3407d-139">这适用于在 Silverlight 中创建的旧版策略，可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="3407d-139">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="3407d-140">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="3407d-140">This property is read-only.</span></span> <span data-ttu-id="3407d-141">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3407d-141">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3407d-142">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="3407d-142">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="3407d-143">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="3407d-143">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="3407d-144">适用于此策略的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="3407d-144">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="3407d-145">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3407d-145">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3407d-146">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="3407d-146">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="3407d-147">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="3407d-147">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="3407d-148">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="3407d-148">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="3407d-149">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3407d-149">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3407d-150">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="3407d-150">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="3407d-151">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="3407d-151">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="3407d-152">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="3407d-152">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="3407d-153">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3407d-153">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3407d-154">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3407d-154">createdDateTime</span></span>|<span data-ttu-id="3407d-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3407d-155">DateTimeOffset</span></span>|<span data-ttu-id="3407d-156">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="3407d-156">DateTime the object was created.</span></span> <span data-ttu-id="3407d-157">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3407d-157">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3407d-158">说明</span><span class="sxs-lookup"><span data-stu-id="3407d-158">description</span></span>|<span data-ttu-id="3407d-159">String</span><span class="sxs-lookup"><span data-stu-id="3407d-159">String</span></span>|<span data-ttu-id="3407d-160">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="3407d-160">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="3407d-161">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3407d-161">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3407d-162">displayName</span><span class="sxs-lookup"><span data-stu-id="3407d-162">displayName</span></span>|<span data-ttu-id="3407d-163">String</span><span class="sxs-lookup"><span data-stu-id="3407d-163">String</span></span>|<span data-ttu-id="3407d-164">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="3407d-164">Admin provided name of the device configuration.</span></span> <span data-ttu-id="3407d-165">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3407d-165">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3407d-166">version</span><span class="sxs-lookup"><span data-stu-id="3407d-166">version</span></span>|<span data-ttu-id="3407d-167">Int32</span><span class="sxs-lookup"><span data-stu-id="3407d-167">Int32</span></span>|<span data-ttu-id="3407d-168">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="3407d-168">Version of the device configuration.</span></span> <span data-ttu-id="3407d-169">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3407d-169">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3407d-170">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="3407d-170">authenticationMethod</span></span>|[<span data-ttu-id="3407d-171">vpnAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="3407d-171">vpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-vpnauthenticationmethod.md)|<span data-ttu-id="3407d-172">身份验证方法。</span><span class="sxs-lookup"><span data-stu-id="3407d-172">Authentication method.</span></span> <span data-ttu-id="3407d-173">可取值为：`certificate`、`usernameAndPassword`、`sharedSecret`、`derivedCredential`、`azureAD`。</span><span class="sxs-lookup"><span data-stu-id="3407d-173">Possible values are: `certificate`, `usernameAndPassword`, `sharedSecret`, `derivedCredential`, `azureAD`.</span></span>|
|<span data-ttu-id="3407d-174">connectionName</span><span class="sxs-lookup"><span data-stu-id="3407d-174">connectionName</span></span>|<span data-ttu-id="3407d-175">String</span><span class="sxs-lookup"><span data-stu-id="3407d-175">String</span></span>|<span data-ttu-id="3407d-176">向用户显示的连接名称。</span><span class="sxs-lookup"><span data-stu-id="3407d-176">Connection name displayed to the user.</span></span>|
|<span data-ttu-id="3407d-177">role</span><span class="sxs-lookup"><span data-stu-id="3407d-177">role</span></span>|<span data-ttu-id="3407d-178">String</span><span class="sxs-lookup"><span data-stu-id="3407d-178">String</span></span>|<span data-ttu-id="3407d-179">将 "连接类型" 设置为 "脉冲安全" 时的角色。</span><span class="sxs-lookup"><span data-stu-id="3407d-179">Role when connection type is set to Pulse Secure.</span></span>|
|<span data-ttu-id="3407d-180">型</span><span class="sxs-lookup"><span data-stu-id="3407d-180">realm</span></span>|<span data-ttu-id="3407d-181">String</span><span class="sxs-lookup"><span data-stu-id="3407d-181">String</span></span>|<span data-ttu-id="3407d-182">连接类型设置为脉冲安全时的领域。</span><span class="sxs-lookup"><span data-stu-id="3407d-182">Realm when connection type is set to Pulse Secure.</span></span>|
|<span data-ttu-id="3407d-183">台</span><span class="sxs-lookup"><span data-stu-id="3407d-183">servers</span></span>|<span data-ttu-id="3407d-184">[vpnServer](../resources/intune-deviceconfig-vpnserver.md)集合</span><span class="sxs-lookup"><span data-stu-id="3407d-184">[vpnServer](../resources/intune-deviceconfig-vpnserver.md) collection</span></span>|<span data-ttu-id="3407d-185">网络上的 VPN 服务器的列表。</span><span class="sxs-lookup"><span data-stu-id="3407d-185">List of VPN Servers on the network.</span></span> <span data-ttu-id="3407d-186">请确保最终用户可以访问这些网络位置。</span><span class="sxs-lookup"><span data-stu-id="3407d-186">Make sure end users can access these network locations.</span></span> <span data-ttu-id="3407d-187">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="3407d-187">This collection can contain a maximum of 500 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3407d-188">关系</span><span class="sxs-lookup"><span data-stu-id="3407d-188">Relationships</span></span>
|<span data-ttu-id="3407d-189">关系</span><span class="sxs-lookup"><span data-stu-id="3407d-189">Relationship</span></span>|<span data-ttu-id="3407d-190">类型</span><span class="sxs-lookup"><span data-stu-id="3407d-190">Type</span></span>|<span data-ttu-id="3407d-191">说明</span><span class="sxs-lookup"><span data-stu-id="3407d-191">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3407d-192">groupAssignments</span><span class="sxs-lookup"><span data-stu-id="3407d-192">groupAssignments</span></span>|<span data-ttu-id="3407d-193">[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)集合</span><span class="sxs-lookup"><span data-stu-id="3407d-193">[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) collection</span></span>|<span data-ttu-id="3407d-194">设备配置文件的组分配列表。</span><span class="sxs-lookup"><span data-stu-id="3407d-194">The list of group assignments for the device configuration profile.</span></span> <span data-ttu-id="3407d-195">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3407d-195">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3407d-196">assignments</span><span class="sxs-lookup"><span data-stu-id="3407d-196">assignments</span></span>|<span data-ttu-id="3407d-197">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="3407d-197">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection</span></span>|<span data-ttu-id="3407d-198">设备配置文件的分配列表。</span><span class="sxs-lookup"><span data-stu-id="3407d-198">The list of assignments for the device configuration profile.</span></span> <span data-ttu-id="3407d-199">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3407d-199">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3407d-200">deviceStatuses</span><span class="sxs-lookup"><span data-stu-id="3407d-200">deviceStatuses</span></span>|<span data-ttu-id="3407d-201">[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) 集合</span><span class="sxs-lookup"><span data-stu-id="3407d-201">[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) collection</span></span>|<span data-ttu-id="3407d-202">按设备的设备配置安装状态。</span><span class="sxs-lookup"><span data-stu-id="3407d-202">Device configuration installation status by device.</span></span> <span data-ttu-id="3407d-203">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3407d-203">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3407d-204">userStatuses</span><span class="sxs-lookup"><span data-stu-id="3407d-204">userStatuses</span></span>|<span data-ttu-id="3407d-205">[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) 集合</span><span class="sxs-lookup"><span data-stu-id="3407d-205">[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) collection</span></span>|<span data-ttu-id="3407d-206">按用户的设备配置安装状态。</span><span class="sxs-lookup"><span data-stu-id="3407d-206">Device configuration installation status by user.</span></span> <span data-ttu-id="3407d-207">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3407d-207">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3407d-208">deviceStatusOverview</span><span class="sxs-lookup"><span data-stu-id="3407d-208">deviceStatusOverview</span></span>|[<span data-ttu-id="3407d-209">deviceConfigurationDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="3407d-209">deviceConfigurationDeviceOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|<span data-ttu-id="3407d-210">设备配置设备状态概述 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3407d-210">Device Configuration devices status overview Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3407d-211">userStatusOverview</span><span class="sxs-lookup"><span data-stu-id="3407d-211">userStatusOverview</span></span>|[<span data-ttu-id="3407d-212">deviceConfigurationUserOverview</span><span class="sxs-lookup"><span data-stu-id="3407d-212">deviceConfigurationUserOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|<span data-ttu-id="3407d-213">设备配置用户状态概述 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3407d-213">Device Configuration users status overview Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3407d-214">deviceSettingStateSummaries</span><span class="sxs-lookup"><span data-stu-id="3407d-214">deviceSettingStateSummaries</span></span>|<span data-ttu-id="3407d-215">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) 集合</span><span class="sxs-lookup"><span data-stu-id="3407d-215">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) collection</span></span>|<span data-ttu-id="3407d-216">设备配置设置状态设备摘要 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3407d-216">Device Configuration Setting State Device Summary Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|

## <a name="json-representation"></a><span data-ttu-id="3407d-217">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="3407d-217">JSON Representation</span></span>
<span data-ttu-id="3407d-218">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3407d-218">Here is a JSON representation of the resource.</span></span>
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



