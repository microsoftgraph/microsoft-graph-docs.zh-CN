---
title: vpnConfiguration 资源类型
description: 基本 VPN 配置文件。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: fcedf7232502d1830312323fe68ccf66d41d8b0e
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48728389"
---
# <a name="vpnconfiguration-resource-type"></a><span data-ttu-id="6f59e-103">vpnConfiguration 资源类型</span><span class="sxs-lookup"><span data-stu-id="6f59e-103">vpnConfiguration resource type</span></span>

<span data-ttu-id="6f59e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6f59e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6f59e-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="6f59e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6f59e-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="6f59e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6f59e-107">基本 VPN 配置文件。</span><span class="sxs-lookup"><span data-stu-id="6f59e-107">Base VPN Configuration profile.</span></span>


<span data-ttu-id="6f59e-108">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6f59e-108">Inherits from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>

## <a name="methods"></a><span data-ttu-id="6f59e-109">Methods</span><span class="sxs-lookup"><span data-stu-id="6f59e-109">Methods</span></span>
|<span data-ttu-id="6f59e-110">方法</span><span class="sxs-lookup"><span data-stu-id="6f59e-110">Method</span></span>|<span data-ttu-id="6f59e-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="6f59e-111">Return Type</span></span>|<span data-ttu-id="6f59e-112">说明</span><span class="sxs-lookup"><span data-stu-id="6f59e-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="6f59e-113">列出 vpnConfigurations</span><span class="sxs-lookup"><span data-stu-id="6f59e-113">List vpnConfigurations</span></span>](../api/intune-deviceconfig-vpnconfiguration-list.md)|<span data-ttu-id="6f59e-114">[vpnConfiguration](../resources/intune-deviceconfig-vpnconfiguration.md) 集合</span><span class="sxs-lookup"><span data-stu-id="6f59e-114">[vpnConfiguration](../resources/intune-deviceconfig-vpnconfiguration.md) collection</span></span>|<span data-ttu-id="6f59e-115">列出 [vpnConfiguration](../resources/intune-deviceconfig-vpnconfiguration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="6f59e-115">List properties and relationships of the [vpnConfiguration](../resources/intune-deviceconfig-vpnconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="6f59e-116">获取 vpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="6f59e-116">Get vpnConfiguration</span></span>](../api/intune-deviceconfig-vpnconfiguration-get.md)|[<span data-ttu-id="6f59e-117">vpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="6f59e-117">vpnConfiguration</span></span>](../resources/intune-deviceconfig-vpnconfiguration.md)|<span data-ttu-id="6f59e-118">读取 [vpnConfiguration](../resources/intune-deviceconfig-vpnconfiguration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="6f59e-118">Read properties and relationships of the [vpnConfiguration](../resources/intune-deviceconfig-vpnconfiguration.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="6f59e-119">属性</span><span class="sxs-lookup"><span data-stu-id="6f59e-119">Properties</span></span>
|<span data-ttu-id="6f59e-120">属性</span><span class="sxs-lookup"><span data-stu-id="6f59e-120">Property</span></span>|<span data-ttu-id="6f59e-121">类型</span><span class="sxs-lookup"><span data-stu-id="6f59e-121">Type</span></span>|<span data-ttu-id="6f59e-122">说明</span><span class="sxs-lookup"><span data-stu-id="6f59e-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6f59e-123">id</span><span class="sxs-lookup"><span data-stu-id="6f59e-123">id</span></span>|<span data-ttu-id="6f59e-124">String</span><span class="sxs-lookup"><span data-stu-id="6f59e-124">String</span></span>|<span data-ttu-id="6f59e-125">实体的键。</span><span class="sxs-lookup"><span data-stu-id="6f59e-125">Key of the entity.</span></span> <span data-ttu-id="6f59e-126">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6f59e-126">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6f59e-127">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6f59e-127">lastModifiedDateTime</span></span>|<span data-ttu-id="6f59e-128">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6f59e-128">DateTimeOffset</span></span>|<span data-ttu-id="6f59e-129">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="6f59e-129">DateTime the object was last modified.</span></span> <span data-ttu-id="6f59e-130">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6f59e-130">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6f59e-131">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="6f59e-131">roleScopeTagIds</span></span>|<span data-ttu-id="6f59e-132">String collection</span><span class="sxs-lookup"><span data-stu-id="6f59e-132">String collection</span></span>|<span data-ttu-id="6f59e-133">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="6f59e-133">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="6f59e-134">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6f59e-134">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6f59e-135">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="6f59e-135">supportsScopeTags</span></span>|<span data-ttu-id="6f59e-136">布尔</span><span class="sxs-lookup"><span data-stu-id="6f59e-136">Boolean</span></span>|<span data-ttu-id="6f59e-137">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="6f59e-137">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="6f59e-138">如果此值为 false，则不允许分配给 ScopeTags 属性，并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="6f59e-138">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="6f59e-139">这适用于在 Silverlight 中创建的旧版策略，可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="6f59e-139">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="6f59e-140">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="6f59e-140">This property is read-only.</span></span> <span data-ttu-id="6f59e-141">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6f59e-141">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6f59e-142">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="6f59e-142">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="6f59e-143">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="6f59e-143">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="6f59e-144">适用于此策略的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="6f59e-144">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="6f59e-145">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6f59e-145">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6f59e-146">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="6f59e-146">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="6f59e-147">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="6f59e-147">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="6f59e-148">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="6f59e-148">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="6f59e-149">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6f59e-149">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6f59e-150">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="6f59e-150">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="6f59e-151">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="6f59e-151">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="6f59e-152">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="6f59e-152">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="6f59e-153">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6f59e-153">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6f59e-154">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6f59e-154">createdDateTime</span></span>|<span data-ttu-id="6f59e-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6f59e-155">DateTimeOffset</span></span>|<span data-ttu-id="6f59e-156">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="6f59e-156">DateTime the object was created.</span></span> <span data-ttu-id="6f59e-157">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6f59e-157">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6f59e-158">说明</span><span class="sxs-lookup"><span data-stu-id="6f59e-158">description</span></span>|<span data-ttu-id="6f59e-159">String</span><span class="sxs-lookup"><span data-stu-id="6f59e-159">String</span></span>|<span data-ttu-id="6f59e-160">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="6f59e-160">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="6f59e-161">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6f59e-161">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6f59e-162">displayName</span><span class="sxs-lookup"><span data-stu-id="6f59e-162">displayName</span></span>|<span data-ttu-id="6f59e-163">String</span><span class="sxs-lookup"><span data-stu-id="6f59e-163">String</span></span>|<span data-ttu-id="6f59e-164">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="6f59e-164">Admin provided name of the device configuration.</span></span> <span data-ttu-id="6f59e-165">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6f59e-165">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6f59e-166">version</span><span class="sxs-lookup"><span data-stu-id="6f59e-166">version</span></span>|<span data-ttu-id="6f59e-167">Int32</span><span class="sxs-lookup"><span data-stu-id="6f59e-167">Int32</span></span>|<span data-ttu-id="6f59e-168">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="6f59e-168">Version of the device configuration.</span></span> <span data-ttu-id="6f59e-169">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6f59e-169">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6f59e-170">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="6f59e-170">authenticationMethod</span></span>|[<span data-ttu-id="6f59e-171">vpnAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="6f59e-171">vpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-vpnauthenticationmethod.md)|<span data-ttu-id="6f59e-172">身份验证方法。</span><span class="sxs-lookup"><span data-stu-id="6f59e-172">Authentication method.</span></span> <span data-ttu-id="6f59e-173">可取值为：`certificate`、`usernameAndPassword`、`sharedSecret`、`derivedCredential`、`azureAD`。</span><span class="sxs-lookup"><span data-stu-id="6f59e-173">Possible values are: `certificate`, `usernameAndPassword`, `sharedSecret`, `derivedCredential`, `azureAD`.</span></span>|
|<span data-ttu-id="6f59e-174">connectionName</span><span class="sxs-lookup"><span data-stu-id="6f59e-174">connectionName</span></span>|<span data-ttu-id="6f59e-175">String</span><span class="sxs-lookup"><span data-stu-id="6f59e-175">String</span></span>|<span data-ttu-id="6f59e-176">向用户显示的连接名称。</span><span class="sxs-lookup"><span data-stu-id="6f59e-176">Connection name displayed to the user.</span></span>|
|<span data-ttu-id="6f59e-177">role</span><span class="sxs-lookup"><span data-stu-id="6f59e-177">role</span></span>|<span data-ttu-id="6f59e-178">String</span><span class="sxs-lookup"><span data-stu-id="6f59e-178">String</span></span>|<span data-ttu-id="6f59e-179">将 "连接类型" 设置为 "脉冲安全" 时的角色。</span><span class="sxs-lookup"><span data-stu-id="6f59e-179">Role when connection type is set to Pulse Secure.</span></span>|
|<span data-ttu-id="6f59e-180">型</span><span class="sxs-lookup"><span data-stu-id="6f59e-180">realm</span></span>|<span data-ttu-id="6f59e-181">String</span><span class="sxs-lookup"><span data-stu-id="6f59e-181">String</span></span>|<span data-ttu-id="6f59e-182">连接类型设置为脉冲安全时的领域。</span><span class="sxs-lookup"><span data-stu-id="6f59e-182">Realm when connection type is set to Pulse Secure.</span></span>|
|<span data-ttu-id="6f59e-183">台</span><span class="sxs-lookup"><span data-stu-id="6f59e-183">servers</span></span>|<span data-ttu-id="6f59e-184">[vpnServer](../resources/intune-deviceconfig-vpnserver.md) 集合</span><span class="sxs-lookup"><span data-stu-id="6f59e-184">[vpnServer](../resources/intune-deviceconfig-vpnserver.md) collection</span></span>|<span data-ttu-id="6f59e-185">网络上的 VPN 服务器的列表。</span><span class="sxs-lookup"><span data-stu-id="6f59e-185">List of VPN Servers on the network.</span></span> <span data-ttu-id="6f59e-186">请确保最终用户可以访问这些网络位置。</span><span class="sxs-lookup"><span data-stu-id="6f59e-186">Make sure end users can access these network locations.</span></span> <span data-ttu-id="6f59e-187">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="6f59e-187">This collection can contain a maximum of 500 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6f59e-188">关系</span><span class="sxs-lookup"><span data-stu-id="6f59e-188">Relationships</span></span>
|<span data-ttu-id="6f59e-189">关系</span><span class="sxs-lookup"><span data-stu-id="6f59e-189">Relationship</span></span>|<span data-ttu-id="6f59e-190">类型</span><span class="sxs-lookup"><span data-stu-id="6f59e-190">Type</span></span>|<span data-ttu-id="6f59e-191">说明</span><span class="sxs-lookup"><span data-stu-id="6f59e-191">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6f59e-192">groupAssignments</span><span class="sxs-lookup"><span data-stu-id="6f59e-192">groupAssignments</span></span>|<span data-ttu-id="6f59e-193">[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="6f59e-193">[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) collection</span></span>|<span data-ttu-id="6f59e-194">设备配置文件的组分配列表。</span><span class="sxs-lookup"><span data-stu-id="6f59e-194">The list of group assignments for the device configuration profile.</span></span> <span data-ttu-id="6f59e-195">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6f59e-195">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6f59e-196">assignments</span><span class="sxs-lookup"><span data-stu-id="6f59e-196">assignments</span></span>|<span data-ttu-id="6f59e-197">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="6f59e-197">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection</span></span>|<span data-ttu-id="6f59e-198">设备配置文件的分配列表。</span><span class="sxs-lookup"><span data-stu-id="6f59e-198">The list of assignments for the device configuration profile.</span></span> <span data-ttu-id="6f59e-199">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6f59e-199">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6f59e-200">deviceStatuses</span><span class="sxs-lookup"><span data-stu-id="6f59e-200">deviceStatuses</span></span>|<span data-ttu-id="6f59e-201">[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) 集合</span><span class="sxs-lookup"><span data-stu-id="6f59e-201">[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) collection</span></span>|<span data-ttu-id="6f59e-202">按设备的设备配置安装状态。</span><span class="sxs-lookup"><span data-stu-id="6f59e-202">Device configuration installation status by device.</span></span> <span data-ttu-id="6f59e-203">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6f59e-203">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6f59e-204">userStatuses</span><span class="sxs-lookup"><span data-stu-id="6f59e-204">userStatuses</span></span>|<span data-ttu-id="6f59e-205">[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) 集合</span><span class="sxs-lookup"><span data-stu-id="6f59e-205">[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) collection</span></span>|<span data-ttu-id="6f59e-206">按用户的设备配置安装状态。</span><span class="sxs-lookup"><span data-stu-id="6f59e-206">Device configuration installation status by user.</span></span> <span data-ttu-id="6f59e-207">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6f59e-207">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6f59e-208">deviceStatusOverview</span><span class="sxs-lookup"><span data-stu-id="6f59e-208">deviceStatusOverview</span></span>|[<span data-ttu-id="6f59e-209">deviceConfigurationDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="6f59e-209">deviceConfigurationDeviceOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|<span data-ttu-id="6f59e-210">设备配置设备状态概述 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6f59e-210">Device Configuration devices status overview Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6f59e-211">userStatusOverview</span><span class="sxs-lookup"><span data-stu-id="6f59e-211">userStatusOverview</span></span>|[<span data-ttu-id="6f59e-212">deviceConfigurationUserOverview</span><span class="sxs-lookup"><span data-stu-id="6f59e-212">deviceConfigurationUserOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|<span data-ttu-id="6f59e-213">设备配置用户状态概述 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6f59e-213">Device Configuration users status overview Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6f59e-214">deviceSettingStateSummaries</span><span class="sxs-lookup"><span data-stu-id="6f59e-214">deviceSettingStateSummaries</span></span>|<span data-ttu-id="6f59e-215">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) 集合</span><span class="sxs-lookup"><span data-stu-id="6f59e-215">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) collection</span></span>|<span data-ttu-id="6f59e-216">设备配置设置状态设备摘要 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6f59e-216">Device Configuration Setting State Device Summary Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|

## <a name="json-representation"></a><span data-ttu-id="6f59e-217">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6f59e-217">JSON Representation</span></span>
<span data-ttu-id="6f59e-218">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6f59e-218">Here is a JSON representation of the resource.</span></span>
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





