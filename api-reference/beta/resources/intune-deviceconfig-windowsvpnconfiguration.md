---
title: windowsVpnConfiguration 资源类型
description: Windows VPN 配置文件。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: c7466e0e0c5b2b9a4a4de64518b32cc1187a6fae
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43456925"
---
# <a name="windowsvpnconfiguration-resource-type"></a><span data-ttu-id="3efc3-103">windowsVpnConfiguration 资源类型</span><span class="sxs-lookup"><span data-stu-id="3efc3-103">windowsVpnConfiguration resource type</span></span>

<span data-ttu-id="3efc3-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3efc3-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3efc3-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="3efc3-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3efc3-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="3efc3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3efc3-107">Windows VPN 配置文件。</span><span class="sxs-lookup"><span data-stu-id="3efc3-107">Windows VPN configuration profile.</span></span>


<span data-ttu-id="3efc3-108">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3efc3-108">Inherits from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>

## <a name="methods"></a><span data-ttu-id="3efc3-109">方法</span><span class="sxs-lookup"><span data-stu-id="3efc3-109">Methods</span></span>
|<span data-ttu-id="3efc3-110">方法</span><span class="sxs-lookup"><span data-stu-id="3efc3-110">Method</span></span>|<span data-ttu-id="3efc3-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="3efc3-111">Return Type</span></span>|<span data-ttu-id="3efc3-112">说明</span><span class="sxs-lookup"><span data-stu-id="3efc3-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="3efc3-113">列出 windowsVpnConfigurations</span><span class="sxs-lookup"><span data-stu-id="3efc3-113">List windowsVpnConfigurations</span></span>](../api/intune-deviceconfig-windowsvpnconfiguration-list.md)|<span data-ttu-id="3efc3-114">[windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)集合</span><span class="sxs-lookup"><span data-stu-id="3efc3-114">[windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md) collection</span></span>|<span data-ttu-id="3efc3-115">列出[windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="3efc3-115">List properties and relationships of the [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="3efc3-116">获取 windowsVpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="3efc3-116">Get windowsVpnConfiguration</span></span>](../api/intune-deviceconfig-windowsvpnconfiguration-get.md)|[<span data-ttu-id="3efc3-117">windowsVpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="3efc3-117">windowsVpnConfiguration</span></span>](../resources/intune-deviceconfig-windowsvpnconfiguration.md)|<span data-ttu-id="3efc3-118">读取[windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="3efc3-118">Read properties and relationships of the [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="3efc3-119">属性</span><span class="sxs-lookup"><span data-stu-id="3efc3-119">Properties</span></span>
|<span data-ttu-id="3efc3-120">属性</span><span class="sxs-lookup"><span data-stu-id="3efc3-120">Property</span></span>|<span data-ttu-id="3efc3-121">类型</span><span class="sxs-lookup"><span data-stu-id="3efc3-121">Type</span></span>|<span data-ttu-id="3efc3-122">说明</span><span class="sxs-lookup"><span data-stu-id="3efc3-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3efc3-123">id</span><span class="sxs-lookup"><span data-stu-id="3efc3-123">id</span></span>|<span data-ttu-id="3efc3-124">字符串</span><span class="sxs-lookup"><span data-stu-id="3efc3-124">String</span></span>|<span data-ttu-id="3efc3-125">实体的键。</span><span class="sxs-lookup"><span data-stu-id="3efc3-125">Key of the entity.</span></span> <span data-ttu-id="3efc3-126">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3efc3-126">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3efc3-127">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3efc3-127">lastModifiedDateTime</span></span>|<span data-ttu-id="3efc3-128">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3efc3-128">DateTimeOffset</span></span>|<span data-ttu-id="3efc3-129">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="3efc3-129">DateTime the object was last modified.</span></span> <span data-ttu-id="3efc3-130">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3efc3-130">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3efc3-131">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="3efc3-131">roleScopeTagIds</span></span>|<span data-ttu-id="3efc3-132">String 集合</span><span class="sxs-lookup"><span data-stu-id="3efc3-132">String collection</span></span>|<span data-ttu-id="3efc3-133">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="3efc3-133">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="3efc3-134">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3efc3-134">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3efc3-135">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="3efc3-135">supportsScopeTags</span></span>|<span data-ttu-id="3efc3-136">Boolean</span><span class="sxs-lookup"><span data-stu-id="3efc3-136">Boolean</span></span>|<span data-ttu-id="3efc3-137">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="3efc3-137">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="3efc3-138">如果此值为 false，则不允许分配给 ScopeTags 属性，并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="3efc3-138">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="3efc3-139">这适用于在 Silverlight 中创建的旧版策略，可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="3efc3-139">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="3efc3-140">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="3efc3-140">This property is read-only.</span></span> <span data-ttu-id="3efc3-141">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3efc3-141">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3efc3-142">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="3efc3-142">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="3efc3-143">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="3efc3-143">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="3efc3-144">适用于此策略的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="3efc3-144">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="3efc3-145">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3efc3-145">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3efc3-146">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="3efc3-146">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="3efc3-147">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="3efc3-147">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="3efc3-148">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="3efc3-148">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="3efc3-149">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3efc3-149">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3efc3-150">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="3efc3-150">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="3efc3-151">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="3efc3-151">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="3efc3-152">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="3efc3-152">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="3efc3-153">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3efc3-153">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3efc3-154">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3efc3-154">createdDateTime</span></span>|<span data-ttu-id="3efc3-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3efc3-155">DateTimeOffset</span></span>|<span data-ttu-id="3efc3-156">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="3efc3-156">DateTime the object was created.</span></span> <span data-ttu-id="3efc3-157">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3efc3-157">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3efc3-158">description</span><span class="sxs-lookup"><span data-stu-id="3efc3-158">description</span></span>|<span data-ttu-id="3efc3-159">String</span><span class="sxs-lookup"><span data-stu-id="3efc3-159">String</span></span>|<span data-ttu-id="3efc3-160">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="3efc3-160">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="3efc3-161">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3efc3-161">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3efc3-162">displayName</span><span class="sxs-lookup"><span data-stu-id="3efc3-162">displayName</span></span>|<span data-ttu-id="3efc3-163">String</span><span class="sxs-lookup"><span data-stu-id="3efc3-163">String</span></span>|<span data-ttu-id="3efc3-164">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="3efc3-164">Admin provided name of the device configuration.</span></span> <span data-ttu-id="3efc3-165">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3efc3-165">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3efc3-166">version</span><span class="sxs-lookup"><span data-stu-id="3efc3-166">version</span></span>|<span data-ttu-id="3efc3-167">Int32</span><span class="sxs-lookup"><span data-stu-id="3efc3-167">Int32</span></span>|<span data-ttu-id="3efc3-168">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="3efc3-168">Version of the device configuration.</span></span> <span data-ttu-id="3efc3-169">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3efc3-169">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3efc3-170">connectionName</span><span class="sxs-lookup"><span data-stu-id="3efc3-170">connectionName</span></span>|<span data-ttu-id="3efc3-171">String</span><span class="sxs-lookup"><span data-stu-id="3efc3-171">String</span></span>|<span data-ttu-id="3efc3-172">向用户显示的连接名称。</span><span class="sxs-lookup"><span data-stu-id="3efc3-172">Connection name displayed to the user.</span></span>|
|<span data-ttu-id="3efc3-173">台</span><span class="sxs-lookup"><span data-stu-id="3efc3-173">servers</span></span>|<span data-ttu-id="3efc3-174">[vpnServer](../resources/intune-deviceconfig-vpnserver.md)集合</span><span class="sxs-lookup"><span data-stu-id="3efc3-174">[vpnServer](../resources/intune-deviceconfig-vpnserver.md) collection</span></span>|<span data-ttu-id="3efc3-175">网络上的 VPN 服务器的列表。</span><span class="sxs-lookup"><span data-stu-id="3efc3-175">List of VPN Servers on the network.</span></span> <span data-ttu-id="3efc3-176">请确保最终用户可以访问这些网络位置。</span><span class="sxs-lookup"><span data-stu-id="3efc3-176">Make sure end users can access these network locations.</span></span> <span data-ttu-id="3efc3-177">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="3efc3-177">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="3efc3-178">customXml</span><span class="sxs-lookup"><span data-stu-id="3efc3-178">customXml</span></span>|<span data-ttu-id="3efc3-179">Binary</span><span class="sxs-lookup"><span data-stu-id="3efc3-179">Binary</span></span>|<span data-ttu-id="3efc3-180">配置 VPN 连接的自定义 XML 命令。</span><span class="sxs-lookup"><span data-stu-id="3efc3-180">Custom XML commands that configures the VPN connection.</span></span> <span data-ttu-id="3efc3-181">（UTF8 编码的字节数组）</span><span class="sxs-lookup"><span data-stu-id="3efc3-181">(UTF8 encoded byte array)</span></span>|

## <a name="relationships"></a><span data-ttu-id="3efc3-182">关系</span><span class="sxs-lookup"><span data-stu-id="3efc3-182">Relationships</span></span>
|<span data-ttu-id="3efc3-183">关系</span><span class="sxs-lookup"><span data-stu-id="3efc3-183">Relationship</span></span>|<span data-ttu-id="3efc3-184">类型</span><span class="sxs-lookup"><span data-stu-id="3efc3-184">Type</span></span>|<span data-ttu-id="3efc3-185">说明</span><span class="sxs-lookup"><span data-stu-id="3efc3-185">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3efc3-186">groupAssignments</span><span class="sxs-lookup"><span data-stu-id="3efc3-186">groupAssignments</span></span>|<span data-ttu-id="3efc3-187">[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)集合</span><span class="sxs-lookup"><span data-stu-id="3efc3-187">[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) collection</span></span>|<span data-ttu-id="3efc3-188">设备配置文件的组分配列表。</span><span class="sxs-lookup"><span data-stu-id="3efc3-188">The list of group assignments for the device configuration profile.</span></span> <span data-ttu-id="3efc3-189">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3efc3-189">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3efc3-190">assignments</span><span class="sxs-lookup"><span data-stu-id="3efc3-190">assignments</span></span>|<span data-ttu-id="3efc3-191">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="3efc3-191">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection</span></span>|<span data-ttu-id="3efc3-192">设备配置文件的分配列表。</span><span class="sxs-lookup"><span data-stu-id="3efc3-192">The list of assignments for the device configuration profile.</span></span> <span data-ttu-id="3efc3-193">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3efc3-193">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3efc3-194">deviceStatuses</span><span class="sxs-lookup"><span data-stu-id="3efc3-194">deviceStatuses</span></span>|<span data-ttu-id="3efc3-195">[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) 集合</span><span class="sxs-lookup"><span data-stu-id="3efc3-195">[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) collection</span></span>|<span data-ttu-id="3efc3-196">按设备的设备配置安装状态。</span><span class="sxs-lookup"><span data-stu-id="3efc3-196">Device configuration installation status by device.</span></span> <span data-ttu-id="3efc3-197">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3efc3-197">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3efc3-198">userStatuses</span><span class="sxs-lookup"><span data-stu-id="3efc3-198">userStatuses</span></span>|<span data-ttu-id="3efc3-199">[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) 集合</span><span class="sxs-lookup"><span data-stu-id="3efc3-199">[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) collection</span></span>|<span data-ttu-id="3efc3-200">按用户的设备配置安装状态。</span><span class="sxs-lookup"><span data-stu-id="3efc3-200">Device configuration installation status by user.</span></span> <span data-ttu-id="3efc3-201">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3efc3-201">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3efc3-202">deviceStatusOverview</span><span class="sxs-lookup"><span data-stu-id="3efc3-202">deviceStatusOverview</span></span>|[<span data-ttu-id="3efc3-203">deviceConfigurationDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="3efc3-203">deviceConfigurationDeviceOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|<span data-ttu-id="3efc3-204">设备配置设备状态概述 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3efc3-204">Device Configuration devices status overview Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3efc3-205">userStatusOverview</span><span class="sxs-lookup"><span data-stu-id="3efc3-205">userStatusOverview</span></span>|[<span data-ttu-id="3efc3-206">deviceConfigurationUserOverview</span><span class="sxs-lookup"><span data-stu-id="3efc3-206">deviceConfigurationUserOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|<span data-ttu-id="3efc3-207">设备配置用户状态概述 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3efc3-207">Device Configuration users status overview Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3efc3-208">deviceSettingStateSummaries</span><span class="sxs-lookup"><span data-stu-id="3efc3-208">deviceSettingStateSummaries</span></span>|<span data-ttu-id="3efc3-209">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) 集合</span><span class="sxs-lookup"><span data-stu-id="3efc3-209">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) collection</span></span>|<span data-ttu-id="3efc3-210">设备配置设置状态设备摘要 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3efc3-210">Device Configuration Setting State Device Summary Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|

## <a name="json-representation"></a><span data-ttu-id="3efc3-211">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="3efc3-211">JSON Representation</span></span>
<span data-ttu-id="3efc3-212">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3efc3-212">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsVpnConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsVpnConfiguration",
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
  "connectionName": "String",
  "servers": [
    {
      "@odata.type": "microsoft.graph.vpnServer",
      "description": "String",
      "address": "String",
      "isDefaultServer": true
    }
  ],
  "customXml": "binary"
}
```



