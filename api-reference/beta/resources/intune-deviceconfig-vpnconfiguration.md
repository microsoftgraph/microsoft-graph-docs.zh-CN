---
title: vpnConfiguration 资源类型
description: 基本 VPN 配置文件。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: ffe1f271c6b99c5b1d80ab78392c86627dbd8ec7
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/26/2019
ms.locfileid: "37197573"
---
# <a name="vpnconfiguration-resource-type"></a><span data-ttu-id="d95fe-103">vpnConfiguration 资源类型</span><span class="sxs-lookup"><span data-stu-id="d95fe-103">vpnConfiguration resource type</span></span>

> <span data-ttu-id="d95fe-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="d95fe-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d95fe-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d95fe-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d95fe-106">基本 VPN 配置文件。</span><span class="sxs-lookup"><span data-stu-id="d95fe-106">Base VPN Configuration profile.</span></span>


<span data-ttu-id="d95fe-107">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d95fe-107">Inherits from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>

## <a name="methods"></a><span data-ttu-id="d95fe-108">方法</span><span class="sxs-lookup"><span data-stu-id="d95fe-108">Methods</span></span>
|<span data-ttu-id="d95fe-109">方法</span><span class="sxs-lookup"><span data-stu-id="d95fe-109">Method</span></span>|<span data-ttu-id="d95fe-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="d95fe-110">Return Type</span></span>|<span data-ttu-id="d95fe-111">说明</span><span class="sxs-lookup"><span data-stu-id="d95fe-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="d95fe-112">列出 vpnConfigurations</span><span class="sxs-lookup"><span data-stu-id="d95fe-112">List vpnConfigurations</span></span>](../api/intune-deviceconfig-vpnconfiguration-list.md)|<span data-ttu-id="d95fe-113">[vpnConfiguration](../resources/intune-deviceconfig-vpnconfiguration.md)集合</span><span class="sxs-lookup"><span data-stu-id="d95fe-113">[vpnConfiguration](../resources/intune-deviceconfig-vpnconfiguration.md) collection</span></span>|<span data-ttu-id="d95fe-114">列出[vpnConfiguration](../resources/intune-deviceconfig-vpnconfiguration.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="d95fe-114">List properties and relationships of the [vpnConfiguration](../resources/intune-deviceconfig-vpnconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="d95fe-115">获取 vpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="d95fe-115">Get vpnConfiguration</span></span>](../api/intune-deviceconfig-vpnconfiguration-get.md)|[<span data-ttu-id="d95fe-116">vpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="d95fe-116">vpnConfiguration</span></span>](../resources/intune-deviceconfig-vpnconfiguration.md)|<span data-ttu-id="d95fe-117">读取[vpnConfiguration](../resources/intune-deviceconfig-vpnconfiguration.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="d95fe-117">Read properties and relationships of the [vpnConfiguration](../resources/intune-deviceconfig-vpnconfiguration.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="d95fe-118">属性</span><span class="sxs-lookup"><span data-stu-id="d95fe-118">Properties</span></span>
|<span data-ttu-id="d95fe-119">属性</span><span class="sxs-lookup"><span data-stu-id="d95fe-119">Property</span></span>|<span data-ttu-id="d95fe-120">类型</span><span class="sxs-lookup"><span data-stu-id="d95fe-120">Type</span></span>|<span data-ttu-id="d95fe-121">说明</span><span class="sxs-lookup"><span data-stu-id="d95fe-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d95fe-122">id</span><span class="sxs-lookup"><span data-stu-id="d95fe-122">id</span></span>|<span data-ttu-id="d95fe-123">字符串</span><span class="sxs-lookup"><span data-stu-id="d95fe-123">String</span></span>|<span data-ttu-id="d95fe-124">实体的键。</span><span class="sxs-lookup"><span data-stu-id="d95fe-124">Key of the entity.</span></span> <span data-ttu-id="d95fe-125">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d95fe-125">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d95fe-126">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d95fe-126">lastModifiedDateTime</span></span>|<span data-ttu-id="d95fe-127">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d95fe-127">DateTimeOffset</span></span>|<span data-ttu-id="d95fe-128">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="d95fe-128">DateTime the object was last modified.</span></span> <span data-ttu-id="d95fe-129">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d95fe-129">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d95fe-130">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="d95fe-130">roleScopeTagIds</span></span>|<span data-ttu-id="d95fe-131">String collection</span><span class="sxs-lookup"><span data-stu-id="d95fe-131">String collection</span></span>|<span data-ttu-id="d95fe-132">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="d95fe-132">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="d95fe-133">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d95fe-133">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d95fe-134">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="d95fe-134">supportsScopeTags</span></span>|<span data-ttu-id="d95fe-135">Boolean</span><span class="sxs-lookup"><span data-stu-id="d95fe-135">Boolean</span></span>|<span data-ttu-id="d95fe-136">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="d95fe-136">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="d95fe-137">如果此值为 false，则不允许分配给 ScopeTags 属性，并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="d95fe-137">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="d95fe-138">这适用于在 Silverlight 中创建的旧版策略，可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="d95fe-138">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="d95fe-139">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="d95fe-139">This property is read-only.</span></span> <span data-ttu-id="d95fe-140">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d95fe-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d95fe-141">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="d95fe-141">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="d95fe-142">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="d95fe-142">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="d95fe-143">适用于此策略的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="d95fe-143">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="d95fe-144">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d95fe-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d95fe-145">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="d95fe-145">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="d95fe-146">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="d95fe-146">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="d95fe-147">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="d95fe-147">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="d95fe-148">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d95fe-148">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d95fe-149">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="d95fe-149">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="d95fe-150">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="d95fe-150">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="d95fe-151">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="d95fe-151">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="d95fe-152">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d95fe-152">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d95fe-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d95fe-153">createdDateTime</span></span>|<span data-ttu-id="d95fe-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d95fe-154">DateTimeOffset</span></span>|<span data-ttu-id="d95fe-155">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="d95fe-155">DateTime the object was created.</span></span> <span data-ttu-id="d95fe-156">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d95fe-156">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d95fe-157">说明</span><span class="sxs-lookup"><span data-stu-id="d95fe-157">description</span></span>|<span data-ttu-id="d95fe-158">String</span><span class="sxs-lookup"><span data-stu-id="d95fe-158">String</span></span>|<span data-ttu-id="d95fe-159">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="d95fe-159">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="d95fe-160">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d95fe-160">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d95fe-161">displayName</span><span class="sxs-lookup"><span data-stu-id="d95fe-161">displayName</span></span>|<span data-ttu-id="d95fe-162">String</span><span class="sxs-lookup"><span data-stu-id="d95fe-162">String</span></span>|<span data-ttu-id="d95fe-163">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="d95fe-163">Admin provided name of the device configuration.</span></span> <span data-ttu-id="d95fe-164">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d95fe-164">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d95fe-165">version</span><span class="sxs-lookup"><span data-stu-id="d95fe-165">version</span></span>|<span data-ttu-id="d95fe-166">Int32</span><span class="sxs-lookup"><span data-stu-id="d95fe-166">Int32</span></span>|<span data-ttu-id="d95fe-167">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="d95fe-167">Version of the device configuration.</span></span> <span data-ttu-id="d95fe-168">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d95fe-168">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d95fe-169">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="d95fe-169">authenticationMethod</span></span>|[<span data-ttu-id="d95fe-170">vpnAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="d95fe-170">vpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-vpnauthenticationmethod.md)|<span data-ttu-id="d95fe-171">身份验证方法。</span><span class="sxs-lookup"><span data-stu-id="d95fe-171">Authentication method.</span></span> <span data-ttu-id="d95fe-172">可取值为：`certificate`、`usernameAndPassword`、`sharedSecret`、`derivedCredential`。</span><span class="sxs-lookup"><span data-stu-id="d95fe-172">Possible values are: `certificate`, `usernameAndPassword`, `sharedSecret`, `derivedCredential`.</span></span>|
|<span data-ttu-id="d95fe-173">connectionName</span><span class="sxs-lookup"><span data-stu-id="d95fe-173">connectionName</span></span>|<span data-ttu-id="d95fe-174">String</span><span class="sxs-lookup"><span data-stu-id="d95fe-174">String</span></span>|<span data-ttu-id="d95fe-175">向用户显示的连接名称。</span><span class="sxs-lookup"><span data-stu-id="d95fe-175">Connection name displayed to the user.</span></span>|
|<span data-ttu-id="d95fe-176">role</span><span class="sxs-lookup"><span data-stu-id="d95fe-176">role</span></span>|<span data-ttu-id="d95fe-177">String</span><span class="sxs-lookup"><span data-stu-id="d95fe-177">String</span></span>|<span data-ttu-id="d95fe-178">将 "连接类型" 设置为 "脉冲安全" 时的角色。</span><span class="sxs-lookup"><span data-stu-id="d95fe-178">Role when connection type is set to Pulse Secure.</span></span>|
|<span data-ttu-id="d95fe-179">型</span><span class="sxs-lookup"><span data-stu-id="d95fe-179">realm</span></span>|<span data-ttu-id="d95fe-180">String</span><span class="sxs-lookup"><span data-stu-id="d95fe-180">String</span></span>|<span data-ttu-id="d95fe-181">连接类型设置为脉冲安全时的领域。</span><span class="sxs-lookup"><span data-stu-id="d95fe-181">Realm when connection type is set to Pulse Secure.</span></span>|
|<span data-ttu-id="d95fe-182">台</span><span class="sxs-lookup"><span data-stu-id="d95fe-182">servers</span></span>|<span data-ttu-id="d95fe-183">[vpnServer](../resources/intune-deviceconfig-vpnserver.md)集合</span><span class="sxs-lookup"><span data-stu-id="d95fe-183">[vpnServer](../resources/intune-deviceconfig-vpnserver.md) collection</span></span>|<span data-ttu-id="d95fe-184">网络上的 VPN 服务器的列表。</span><span class="sxs-lookup"><span data-stu-id="d95fe-184">List of VPN Servers on the network.</span></span> <span data-ttu-id="d95fe-185">请确保最终用户可以访问这些网络位置。</span><span class="sxs-lookup"><span data-stu-id="d95fe-185">Make sure end users can access these network locations.</span></span> <span data-ttu-id="d95fe-186">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="d95fe-186">This collection can contain a maximum of 500 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d95fe-187">关系</span><span class="sxs-lookup"><span data-stu-id="d95fe-187">Relationships</span></span>
|<span data-ttu-id="d95fe-188">关系</span><span class="sxs-lookup"><span data-stu-id="d95fe-188">Relationship</span></span>|<span data-ttu-id="d95fe-189">类型</span><span class="sxs-lookup"><span data-stu-id="d95fe-189">Type</span></span>|<span data-ttu-id="d95fe-190">说明</span><span class="sxs-lookup"><span data-stu-id="d95fe-190">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d95fe-191">groupAssignments</span><span class="sxs-lookup"><span data-stu-id="d95fe-191">groupAssignments</span></span>|<span data-ttu-id="d95fe-192">[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)集合</span><span class="sxs-lookup"><span data-stu-id="d95fe-192">[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) collection</span></span>|<span data-ttu-id="d95fe-193">设备配置文件的组分配列表。</span><span class="sxs-lookup"><span data-stu-id="d95fe-193">The list of group assignments for the device configuration profile.</span></span> <span data-ttu-id="d95fe-194">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d95fe-194">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d95fe-195">assignments</span><span class="sxs-lookup"><span data-stu-id="d95fe-195">assignments</span></span>|<span data-ttu-id="d95fe-196">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="d95fe-196">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection</span></span>|<span data-ttu-id="d95fe-197">设备配置文件的分配列表。</span><span class="sxs-lookup"><span data-stu-id="d95fe-197">The list of assignments for the device configuration profile.</span></span> <span data-ttu-id="d95fe-198">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d95fe-198">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d95fe-199">deviceStatuses</span><span class="sxs-lookup"><span data-stu-id="d95fe-199">deviceStatuses</span></span>|<span data-ttu-id="d95fe-200">[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) 集合</span><span class="sxs-lookup"><span data-stu-id="d95fe-200">[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) collection</span></span>|<span data-ttu-id="d95fe-201">按设备的设备配置安装状态。</span><span class="sxs-lookup"><span data-stu-id="d95fe-201">Device configuration installation status by device.</span></span> <span data-ttu-id="d95fe-202">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d95fe-202">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d95fe-203">userStatuses</span><span class="sxs-lookup"><span data-stu-id="d95fe-203">userStatuses</span></span>|<span data-ttu-id="d95fe-204">[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) 集合</span><span class="sxs-lookup"><span data-stu-id="d95fe-204">[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) collection</span></span>|<span data-ttu-id="d95fe-205">按用户的设备配置安装状态。</span><span class="sxs-lookup"><span data-stu-id="d95fe-205">Device configuration installation status by user.</span></span> <span data-ttu-id="d95fe-206">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d95fe-206">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d95fe-207">deviceStatusOverview</span><span class="sxs-lookup"><span data-stu-id="d95fe-207">deviceStatusOverview</span></span>|[<span data-ttu-id="d95fe-208">deviceConfigurationDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="d95fe-208">deviceConfigurationDeviceOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|<span data-ttu-id="d95fe-209">设备配置设备状态概述 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d95fe-209">Device Configuration devices status overview Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d95fe-210">userStatusOverview</span><span class="sxs-lookup"><span data-stu-id="d95fe-210">userStatusOverview</span></span>|[<span data-ttu-id="d95fe-211">deviceConfigurationUserOverview</span><span class="sxs-lookup"><span data-stu-id="d95fe-211">deviceConfigurationUserOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|<span data-ttu-id="d95fe-212">设备配置用户状态概述 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d95fe-212">Device Configuration users status overview Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d95fe-213">deviceSettingStateSummaries</span><span class="sxs-lookup"><span data-stu-id="d95fe-213">deviceSettingStateSummaries</span></span>|<span data-ttu-id="d95fe-214">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) 集合</span><span class="sxs-lookup"><span data-stu-id="d95fe-214">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) collection</span></span>|<span data-ttu-id="d95fe-215">设备配置设置状态设备摘要 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d95fe-215">Device Configuration Setting State Device Summary Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d95fe-216">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d95fe-216">JSON Representation</span></span>
<span data-ttu-id="d95fe-217">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d95fe-217">Here is a JSON representation of the resource.</span></span>
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



