---
title: windowsVpnConfiguration 资源类型
description: Windows VPN 配置文件。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 0e63d52a805c9b95e2a61d38e196ec197644c5ca
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42528923"
---
# <a name="windowsvpnconfiguration-resource-type"></a><span data-ttu-id="0f660-103">windowsVpnConfiguration 资源类型</span><span class="sxs-lookup"><span data-stu-id="0f660-103">windowsVpnConfiguration resource type</span></span>

<span data-ttu-id="0f660-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="0f660-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0f660-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="0f660-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0f660-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="0f660-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0f660-107">Windows VPN 配置文件。</span><span class="sxs-lookup"><span data-stu-id="0f660-107">Windows VPN configuration profile.</span></span>


<span data-ttu-id="0f660-108">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0f660-108">Inherits from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>

## <a name="methods"></a><span data-ttu-id="0f660-109">方法</span><span class="sxs-lookup"><span data-stu-id="0f660-109">Methods</span></span>
|<span data-ttu-id="0f660-110">方法</span><span class="sxs-lookup"><span data-stu-id="0f660-110">Method</span></span>|<span data-ttu-id="0f660-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="0f660-111">Return Type</span></span>|<span data-ttu-id="0f660-112">说明</span><span class="sxs-lookup"><span data-stu-id="0f660-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="0f660-113">列出 windowsVpnConfigurations</span><span class="sxs-lookup"><span data-stu-id="0f660-113">List windowsVpnConfigurations</span></span>](../api/intune-deviceconfig-windowsvpnconfiguration-list.md)|<span data-ttu-id="0f660-114">[windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)集合</span><span class="sxs-lookup"><span data-stu-id="0f660-114">[windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md) collection</span></span>|<span data-ttu-id="0f660-115">列出[windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="0f660-115">List properties and relationships of the [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="0f660-116">获取 windowsVpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="0f660-116">Get windowsVpnConfiguration</span></span>](../api/intune-deviceconfig-windowsvpnconfiguration-get.md)|[<span data-ttu-id="0f660-117">windowsVpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="0f660-117">windowsVpnConfiguration</span></span>](../resources/intune-deviceconfig-windowsvpnconfiguration.md)|<span data-ttu-id="0f660-118">读取[windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="0f660-118">Read properties and relationships of the [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="0f660-119">属性</span><span class="sxs-lookup"><span data-stu-id="0f660-119">Properties</span></span>
|<span data-ttu-id="0f660-120">属性</span><span class="sxs-lookup"><span data-stu-id="0f660-120">Property</span></span>|<span data-ttu-id="0f660-121">类型</span><span class="sxs-lookup"><span data-stu-id="0f660-121">Type</span></span>|<span data-ttu-id="0f660-122">说明</span><span class="sxs-lookup"><span data-stu-id="0f660-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0f660-123">id</span><span class="sxs-lookup"><span data-stu-id="0f660-123">id</span></span>|<span data-ttu-id="0f660-124">字符串</span><span class="sxs-lookup"><span data-stu-id="0f660-124">String</span></span>|<span data-ttu-id="0f660-125">实体的键。</span><span class="sxs-lookup"><span data-stu-id="0f660-125">Key of the entity.</span></span> <span data-ttu-id="0f660-126">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0f660-126">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0f660-127">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0f660-127">lastModifiedDateTime</span></span>|<span data-ttu-id="0f660-128">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0f660-128">DateTimeOffset</span></span>|<span data-ttu-id="0f660-129">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="0f660-129">DateTime the object was last modified.</span></span> <span data-ttu-id="0f660-130">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0f660-130">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0f660-131">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="0f660-131">roleScopeTagIds</span></span>|<span data-ttu-id="0f660-132">String 集合</span><span class="sxs-lookup"><span data-stu-id="0f660-132">String collection</span></span>|<span data-ttu-id="0f660-133">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="0f660-133">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="0f660-134">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0f660-134">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0f660-135">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="0f660-135">supportsScopeTags</span></span>|<span data-ttu-id="0f660-136">布尔</span><span class="sxs-lookup"><span data-stu-id="0f660-136">Boolean</span></span>|<span data-ttu-id="0f660-137">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="0f660-137">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="0f660-138">如果此值为 false，则不允许分配给 ScopeTags 属性，并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="0f660-138">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="0f660-139">这适用于在 Silverlight 中创建的旧版策略，可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="0f660-139">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="0f660-140">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="0f660-140">This property is read-only.</span></span> <span data-ttu-id="0f660-141">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0f660-141">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0f660-142">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="0f660-142">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="0f660-143">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="0f660-143">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="0f660-144">适用于此策略的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="0f660-144">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="0f660-145">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0f660-145">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0f660-146">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="0f660-146">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="0f660-147">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="0f660-147">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="0f660-148">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="0f660-148">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="0f660-149">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0f660-149">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0f660-150">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="0f660-150">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="0f660-151">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="0f660-151">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="0f660-152">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="0f660-152">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="0f660-153">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0f660-153">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0f660-154">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0f660-154">createdDateTime</span></span>|<span data-ttu-id="0f660-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0f660-155">DateTimeOffset</span></span>|<span data-ttu-id="0f660-156">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="0f660-156">DateTime the object was created.</span></span> <span data-ttu-id="0f660-157">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0f660-157">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0f660-158">说明</span><span class="sxs-lookup"><span data-stu-id="0f660-158">description</span></span>|<span data-ttu-id="0f660-159">String</span><span class="sxs-lookup"><span data-stu-id="0f660-159">String</span></span>|<span data-ttu-id="0f660-160">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="0f660-160">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="0f660-161">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0f660-161">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0f660-162">displayName</span><span class="sxs-lookup"><span data-stu-id="0f660-162">displayName</span></span>|<span data-ttu-id="0f660-163">String</span><span class="sxs-lookup"><span data-stu-id="0f660-163">String</span></span>|<span data-ttu-id="0f660-164">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="0f660-164">Admin provided name of the device configuration.</span></span> <span data-ttu-id="0f660-165">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0f660-165">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0f660-166">version</span><span class="sxs-lookup"><span data-stu-id="0f660-166">version</span></span>|<span data-ttu-id="0f660-167">Int32</span><span class="sxs-lookup"><span data-stu-id="0f660-167">Int32</span></span>|<span data-ttu-id="0f660-168">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="0f660-168">Version of the device configuration.</span></span> <span data-ttu-id="0f660-169">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0f660-169">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0f660-170">connectionName</span><span class="sxs-lookup"><span data-stu-id="0f660-170">connectionName</span></span>|<span data-ttu-id="0f660-171">String</span><span class="sxs-lookup"><span data-stu-id="0f660-171">String</span></span>|<span data-ttu-id="0f660-172">向用户显示的连接名称。</span><span class="sxs-lookup"><span data-stu-id="0f660-172">Connection name displayed to the user.</span></span>|
|<span data-ttu-id="0f660-173">台</span><span class="sxs-lookup"><span data-stu-id="0f660-173">servers</span></span>|<span data-ttu-id="0f660-174">[vpnServer](../resources/intune-deviceconfig-vpnserver.md)集合</span><span class="sxs-lookup"><span data-stu-id="0f660-174">[vpnServer](../resources/intune-deviceconfig-vpnserver.md) collection</span></span>|<span data-ttu-id="0f660-175">网络上的 VPN 服务器的列表。</span><span class="sxs-lookup"><span data-stu-id="0f660-175">List of VPN Servers on the network.</span></span> <span data-ttu-id="0f660-176">请确保最终用户可以访问这些网络位置。</span><span class="sxs-lookup"><span data-stu-id="0f660-176">Make sure end users can access these network locations.</span></span> <span data-ttu-id="0f660-177">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="0f660-177">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="0f660-178">customXml</span><span class="sxs-lookup"><span data-stu-id="0f660-178">customXml</span></span>|<span data-ttu-id="0f660-179">Binary</span><span class="sxs-lookup"><span data-stu-id="0f660-179">Binary</span></span>|<span data-ttu-id="0f660-180">配置 VPN 连接的自定义 XML 命令。</span><span class="sxs-lookup"><span data-stu-id="0f660-180">Custom XML commands that configures the VPN connection.</span></span> <span data-ttu-id="0f660-181">（UTF8 编码的字节数组）</span><span class="sxs-lookup"><span data-stu-id="0f660-181">(UTF8 encoded byte array)</span></span>|

## <a name="relationships"></a><span data-ttu-id="0f660-182">关系</span><span class="sxs-lookup"><span data-stu-id="0f660-182">Relationships</span></span>
|<span data-ttu-id="0f660-183">关系</span><span class="sxs-lookup"><span data-stu-id="0f660-183">Relationship</span></span>|<span data-ttu-id="0f660-184">类型</span><span class="sxs-lookup"><span data-stu-id="0f660-184">Type</span></span>|<span data-ttu-id="0f660-185">说明</span><span class="sxs-lookup"><span data-stu-id="0f660-185">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0f660-186">groupAssignments</span><span class="sxs-lookup"><span data-stu-id="0f660-186">groupAssignments</span></span>|<span data-ttu-id="0f660-187">[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)集合</span><span class="sxs-lookup"><span data-stu-id="0f660-187">[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) collection</span></span>|<span data-ttu-id="0f660-188">设备配置文件的组分配列表。</span><span class="sxs-lookup"><span data-stu-id="0f660-188">The list of group assignments for the device configuration profile.</span></span> <span data-ttu-id="0f660-189">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0f660-189">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0f660-190">assignments</span><span class="sxs-lookup"><span data-stu-id="0f660-190">assignments</span></span>|<span data-ttu-id="0f660-191">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="0f660-191">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection</span></span>|<span data-ttu-id="0f660-192">设备配置文件的分配列表。</span><span class="sxs-lookup"><span data-stu-id="0f660-192">The list of assignments for the device configuration profile.</span></span> <span data-ttu-id="0f660-193">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0f660-193">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0f660-194">deviceStatuses</span><span class="sxs-lookup"><span data-stu-id="0f660-194">deviceStatuses</span></span>|<span data-ttu-id="0f660-195">[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) 集合</span><span class="sxs-lookup"><span data-stu-id="0f660-195">[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) collection</span></span>|<span data-ttu-id="0f660-196">按设备的设备配置安装状态。</span><span class="sxs-lookup"><span data-stu-id="0f660-196">Device configuration installation status by device.</span></span> <span data-ttu-id="0f660-197">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0f660-197">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0f660-198">userStatuses</span><span class="sxs-lookup"><span data-stu-id="0f660-198">userStatuses</span></span>|<span data-ttu-id="0f660-199">[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) 集合</span><span class="sxs-lookup"><span data-stu-id="0f660-199">[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) collection</span></span>|<span data-ttu-id="0f660-200">按用户的设备配置安装状态。</span><span class="sxs-lookup"><span data-stu-id="0f660-200">Device configuration installation status by user.</span></span> <span data-ttu-id="0f660-201">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0f660-201">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0f660-202">deviceStatusOverview</span><span class="sxs-lookup"><span data-stu-id="0f660-202">deviceStatusOverview</span></span>|[<span data-ttu-id="0f660-203">deviceConfigurationDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="0f660-203">deviceConfigurationDeviceOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|<span data-ttu-id="0f660-204">设备配置设备状态概述 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0f660-204">Device Configuration devices status overview Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0f660-205">userStatusOverview</span><span class="sxs-lookup"><span data-stu-id="0f660-205">userStatusOverview</span></span>|[<span data-ttu-id="0f660-206">deviceConfigurationUserOverview</span><span class="sxs-lookup"><span data-stu-id="0f660-206">deviceConfigurationUserOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|<span data-ttu-id="0f660-207">设备配置用户状态概述 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0f660-207">Device Configuration users status overview Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0f660-208">deviceSettingStateSummaries</span><span class="sxs-lookup"><span data-stu-id="0f660-208">deviceSettingStateSummaries</span></span>|<span data-ttu-id="0f660-209">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) 集合</span><span class="sxs-lookup"><span data-stu-id="0f660-209">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) collection</span></span>|<span data-ttu-id="0f660-210">设备配置设置状态设备摘要 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0f660-210">Device Configuration Setting State Device Summary Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0f660-211">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0f660-211">JSON Representation</span></span>
<span data-ttu-id="0f660-212">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0f660-212">Here is a JSON representation of the resource.</span></span>
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



