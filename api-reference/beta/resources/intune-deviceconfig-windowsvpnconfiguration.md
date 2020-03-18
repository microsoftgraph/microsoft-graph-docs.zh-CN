---
title: windowsVpnConfiguration 资源类型
description: Windows VPN 配置文件。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 3b43fe44121095d2850069c683bb693dc782d64b
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42786135"
---
# <a name="windowsvpnconfiguration-resource-type"></a><span data-ttu-id="a252f-103">windowsVpnConfiguration 资源类型</span><span class="sxs-lookup"><span data-stu-id="a252f-103">windowsVpnConfiguration resource type</span></span>

> <span data-ttu-id="a252f-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="a252f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a252f-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="a252f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a252f-106">Windows VPN 配置文件。</span><span class="sxs-lookup"><span data-stu-id="a252f-106">Windows VPN configuration profile.</span></span>


<span data-ttu-id="a252f-107">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a252f-107">Inherits from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>

## <a name="methods"></a><span data-ttu-id="a252f-108">方法</span><span class="sxs-lookup"><span data-stu-id="a252f-108">Methods</span></span>
|<span data-ttu-id="a252f-109">方法</span><span class="sxs-lookup"><span data-stu-id="a252f-109">Method</span></span>|<span data-ttu-id="a252f-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="a252f-110">Return Type</span></span>|<span data-ttu-id="a252f-111">说明</span><span class="sxs-lookup"><span data-stu-id="a252f-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="a252f-112">列出 windowsVpnConfigurations</span><span class="sxs-lookup"><span data-stu-id="a252f-112">List windowsVpnConfigurations</span></span>](../api/intune-deviceconfig-windowsvpnconfiguration-list.md)|<span data-ttu-id="a252f-113">[windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)集合</span><span class="sxs-lookup"><span data-stu-id="a252f-113">[windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md) collection</span></span>|<span data-ttu-id="a252f-114">列出[windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="a252f-114">List properties and relationships of the [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="a252f-115">获取 windowsVpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="a252f-115">Get windowsVpnConfiguration</span></span>](../api/intune-deviceconfig-windowsvpnconfiguration-get.md)|[<span data-ttu-id="a252f-116">windowsVpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="a252f-116">windowsVpnConfiguration</span></span>](../resources/intune-deviceconfig-windowsvpnconfiguration.md)|<span data-ttu-id="a252f-117">读取[windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="a252f-117">Read properties and relationships of the [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="a252f-118">属性</span><span class="sxs-lookup"><span data-stu-id="a252f-118">Properties</span></span>
|<span data-ttu-id="a252f-119">属性</span><span class="sxs-lookup"><span data-stu-id="a252f-119">Property</span></span>|<span data-ttu-id="a252f-120">类型</span><span class="sxs-lookup"><span data-stu-id="a252f-120">Type</span></span>|<span data-ttu-id="a252f-121">说明</span><span class="sxs-lookup"><span data-stu-id="a252f-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a252f-122">id</span><span class="sxs-lookup"><span data-stu-id="a252f-122">id</span></span>|<span data-ttu-id="a252f-123">字符串</span><span class="sxs-lookup"><span data-stu-id="a252f-123">String</span></span>|<span data-ttu-id="a252f-124">实体的键。</span><span class="sxs-lookup"><span data-stu-id="a252f-124">Key of the entity.</span></span> <span data-ttu-id="a252f-125">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a252f-125">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a252f-126">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a252f-126">lastModifiedDateTime</span></span>|<span data-ttu-id="a252f-127">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a252f-127">DateTimeOffset</span></span>|<span data-ttu-id="a252f-128">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="a252f-128">DateTime the object was last modified.</span></span> <span data-ttu-id="a252f-129">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a252f-129">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a252f-130">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="a252f-130">roleScopeTagIds</span></span>|<span data-ttu-id="a252f-131">String collection</span><span class="sxs-lookup"><span data-stu-id="a252f-131">String collection</span></span>|<span data-ttu-id="a252f-132">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="a252f-132">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="a252f-133">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a252f-133">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a252f-134">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="a252f-134">supportsScopeTags</span></span>|<span data-ttu-id="a252f-135">布尔值</span><span class="sxs-lookup"><span data-stu-id="a252f-135">Boolean</span></span>|<span data-ttu-id="a252f-136">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="a252f-136">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="a252f-137">如果此值为 false，则不允许分配给 ScopeTags 属性，并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="a252f-137">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="a252f-138">这适用于在 Silverlight 中创建的旧版策略，可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="a252f-138">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="a252f-139">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="a252f-139">This property is read-only.</span></span> <span data-ttu-id="a252f-140">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a252f-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a252f-141">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="a252f-141">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="a252f-142">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="a252f-142">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="a252f-143">适用于此策略的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="a252f-143">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="a252f-144">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a252f-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a252f-145">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="a252f-145">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="a252f-146">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="a252f-146">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="a252f-147">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="a252f-147">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="a252f-148">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a252f-148">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a252f-149">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="a252f-149">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="a252f-150">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="a252f-150">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="a252f-151">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="a252f-151">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="a252f-152">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a252f-152">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a252f-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a252f-153">createdDateTime</span></span>|<span data-ttu-id="a252f-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a252f-154">DateTimeOffset</span></span>|<span data-ttu-id="a252f-155">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="a252f-155">DateTime the object was created.</span></span> <span data-ttu-id="a252f-156">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a252f-156">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a252f-157">说明</span><span class="sxs-lookup"><span data-stu-id="a252f-157">description</span></span>|<span data-ttu-id="a252f-158">String</span><span class="sxs-lookup"><span data-stu-id="a252f-158">String</span></span>|<span data-ttu-id="a252f-159">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="a252f-159">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="a252f-160">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a252f-160">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a252f-161">displayName</span><span class="sxs-lookup"><span data-stu-id="a252f-161">displayName</span></span>|<span data-ttu-id="a252f-162">String</span><span class="sxs-lookup"><span data-stu-id="a252f-162">String</span></span>|<span data-ttu-id="a252f-163">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="a252f-163">Admin provided name of the device configuration.</span></span> <span data-ttu-id="a252f-164">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a252f-164">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a252f-165">version</span><span class="sxs-lookup"><span data-stu-id="a252f-165">version</span></span>|<span data-ttu-id="a252f-166">Int32</span><span class="sxs-lookup"><span data-stu-id="a252f-166">Int32</span></span>|<span data-ttu-id="a252f-167">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="a252f-167">Version of the device configuration.</span></span> <span data-ttu-id="a252f-168">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a252f-168">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a252f-169">connectionName</span><span class="sxs-lookup"><span data-stu-id="a252f-169">connectionName</span></span>|<span data-ttu-id="a252f-170">String</span><span class="sxs-lookup"><span data-stu-id="a252f-170">String</span></span>|<span data-ttu-id="a252f-171">向用户显示的连接名称。</span><span class="sxs-lookup"><span data-stu-id="a252f-171">Connection name displayed to the user.</span></span>|
|<span data-ttu-id="a252f-172">台</span><span class="sxs-lookup"><span data-stu-id="a252f-172">servers</span></span>|<span data-ttu-id="a252f-173">[vpnServer](../resources/intune-deviceconfig-vpnserver.md)集合</span><span class="sxs-lookup"><span data-stu-id="a252f-173">[vpnServer](../resources/intune-deviceconfig-vpnserver.md) collection</span></span>|<span data-ttu-id="a252f-174">网络上的 VPN 服务器的列表。</span><span class="sxs-lookup"><span data-stu-id="a252f-174">List of VPN Servers on the network.</span></span> <span data-ttu-id="a252f-175">请确保最终用户可以访问这些网络位置。</span><span class="sxs-lookup"><span data-stu-id="a252f-175">Make sure end users can access these network locations.</span></span> <span data-ttu-id="a252f-176">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="a252f-176">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="a252f-177">customXml</span><span class="sxs-lookup"><span data-stu-id="a252f-177">customXml</span></span>|<span data-ttu-id="a252f-178">Binary</span><span class="sxs-lookup"><span data-stu-id="a252f-178">Binary</span></span>|<span data-ttu-id="a252f-179">配置 VPN 连接的自定义 XML 命令。</span><span class="sxs-lookup"><span data-stu-id="a252f-179">Custom XML commands that configures the VPN connection.</span></span> <span data-ttu-id="a252f-180">（UTF8 编码的字节数组）</span><span class="sxs-lookup"><span data-stu-id="a252f-180">(UTF8 encoded byte array)</span></span>|

## <a name="relationships"></a><span data-ttu-id="a252f-181">关系</span><span class="sxs-lookup"><span data-stu-id="a252f-181">Relationships</span></span>
|<span data-ttu-id="a252f-182">关系</span><span class="sxs-lookup"><span data-stu-id="a252f-182">Relationship</span></span>|<span data-ttu-id="a252f-183">类型</span><span class="sxs-lookup"><span data-stu-id="a252f-183">Type</span></span>|<span data-ttu-id="a252f-184">说明</span><span class="sxs-lookup"><span data-stu-id="a252f-184">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a252f-185">groupAssignments</span><span class="sxs-lookup"><span data-stu-id="a252f-185">groupAssignments</span></span>|<span data-ttu-id="a252f-186">[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)集合</span><span class="sxs-lookup"><span data-stu-id="a252f-186">[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) collection</span></span>|<span data-ttu-id="a252f-187">设备配置文件的组分配列表。</span><span class="sxs-lookup"><span data-stu-id="a252f-187">The list of group assignments for the device configuration profile.</span></span> <span data-ttu-id="a252f-188">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a252f-188">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a252f-189">assignments</span><span class="sxs-lookup"><span data-stu-id="a252f-189">assignments</span></span>|<span data-ttu-id="a252f-190">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="a252f-190">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection</span></span>|<span data-ttu-id="a252f-191">设备配置文件的分配列表。</span><span class="sxs-lookup"><span data-stu-id="a252f-191">The list of assignments for the device configuration profile.</span></span> <span data-ttu-id="a252f-192">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a252f-192">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a252f-193">deviceStatuses</span><span class="sxs-lookup"><span data-stu-id="a252f-193">deviceStatuses</span></span>|<span data-ttu-id="a252f-194">[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) 集合</span><span class="sxs-lookup"><span data-stu-id="a252f-194">[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) collection</span></span>|<span data-ttu-id="a252f-195">按设备的设备配置安装状态。</span><span class="sxs-lookup"><span data-stu-id="a252f-195">Device configuration installation status by device.</span></span> <span data-ttu-id="a252f-196">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a252f-196">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a252f-197">userStatuses</span><span class="sxs-lookup"><span data-stu-id="a252f-197">userStatuses</span></span>|<span data-ttu-id="a252f-198">[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) 集合</span><span class="sxs-lookup"><span data-stu-id="a252f-198">[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) collection</span></span>|<span data-ttu-id="a252f-199">按用户的设备配置安装状态。</span><span class="sxs-lookup"><span data-stu-id="a252f-199">Device configuration installation status by user.</span></span> <span data-ttu-id="a252f-200">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a252f-200">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a252f-201">deviceStatusOverview</span><span class="sxs-lookup"><span data-stu-id="a252f-201">deviceStatusOverview</span></span>|[<span data-ttu-id="a252f-202">deviceConfigurationDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="a252f-202">deviceConfigurationDeviceOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|<span data-ttu-id="a252f-203">设备配置设备状态概述 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a252f-203">Device Configuration devices status overview Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a252f-204">userStatusOverview</span><span class="sxs-lookup"><span data-stu-id="a252f-204">userStatusOverview</span></span>|[<span data-ttu-id="a252f-205">deviceConfigurationUserOverview</span><span class="sxs-lookup"><span data-stu-id="a252f-205">deviceConfigurationUserOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|<span data-ttu-id="a252f-206">设备配置用户状态概述 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a252f-206">Device Configuration users status overview Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a252f-207">deviceSettingStateSummaries</span><span class="sxs-lookup"><span data-stu-id="a252f-207">deviceSettingStateSummaries</span></span>|<span data-ttu-id="a252f-208">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) 集合</span><span class="sxs-lookup"><span data-stu-id="a252f-208">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) collection</span></span>|<span data-ttu-id="a252f-209">设备配置设置状态设备摘要 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a252f-209">Device Configuration Setting State Device Summary Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a252f-210">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a252f-210">JSON Representation</span></span>
<span data-ttu-id="a252f-211">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a252f-211">Here is a JSON representation of the resource.</span></span>
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



