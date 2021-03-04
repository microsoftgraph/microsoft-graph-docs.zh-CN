---
title: windows10VpnConfiguration 资源类型
description: 通过在此配置文件中提供配置，你可以指示 Windows 10 设备 (桌面或移动) 连接到所需的 VPN 终结点。 通过指定 VPN 终结点预期的身份验证方法和安全类型，可以使最终用户无缝进行 VPN 连接。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: c9cfc4fb3fc36ba2187458ded6072b992c278e7b
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50444537"
---
# <a name="windows10vpnconfiguration-resource-type"></a><span data-ttu-id="73ed8-104">windows10VpnConfiguration 资源类型</span><span class="sxs-lookup"><span data-stu-id="73ed8-104">windows10VpnConfiguration resource type</span></span>

<span data-ttu-id="73ed8-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="73ed8-105">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="73ed8-106">**重要提示：** /beta 版本的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="73ed8-106">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="73ed8-107">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="73ed8-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="73ed8-108">通过在此配置文件中提供配置，你可以指示 Windows 10 设备 (桌面或移动) 连接到所需的 VPN 终结点。</span><span class="sxs-lookup"><span data-stu-id="73ed8-108">By providing the configurations in this profile you can instruct the Windows 10 device (desktop or mobile) to connect to desired VPN endpoint.</span></span> <span data-ttu-id="73ed8-109">通过指定 VPN 终结点预期的身份验证方法和安全类型，可以使最终用户无缝进行 VPN 连接。</span><span class="sxs-lookup"><span data-stu-id="73ed8-109">By specifying the authentication method and security types expected by VPN endpoint you can make the VPN connection seamless for end user.</span></span>


<span data-ttu-id="73ed8-110">继承自 [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="73ed8-110">Inherits from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>

## <a name="methods"></a><span data-ttu-id="73ed8-111">Methods</span><span class="sxs-lookup"><span data-stu-id="73ed8-111">Methods</span></span>
|<span data-ttu-id="73ed8-112">方法</span><span class="sxs-lookup"><span data-stu-id="73ed8-112">Method</span></span>|<span data-ttu-id="73ed8-113">返回类型</span><span class="sxs-lookup"><span data-stu-id="73ed8-113">Return Type</span></span>|<span data-ttu-id="73ed8-114">说明</span><span class="sxs-lookup"><span data-stu-id="73ed8-114">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="73ed8-115">列出 windows10VpnConfigurations</span><span class="sxs-lookup"><span data-stu-id="73ed8-115">List windows10VpnConfigurations</span></span>](../api/intune-deviceconfig-windows10vpnconfiguration-list.md)|<span data-ttu-id="73ed8-116">[windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) 集合</span><span class="sxs-lookup"><span data-stu-id="73ed8-116">[windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) collection</span></span>|<span data-ttu-id="73ed8-117">列出 [windows10VpnConfiguration 对象的属性和](../resources/intune-deviceconfig-windows10vpnconfiguration.md) 关系。</span><span class="sxs-lookup"><span data-stu-id="73ed8-117">List properties and relationships of the [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="73ed8-118">获取 windows10VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="73ed8-118">Get windows10VpnConfiguration</span></span>](../api/intune-deviceconfig-windows10vpnconfiguration-get.md)|[<span data-ttu-id="73ed8-119">windows10VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="73ed8-119">windows10VpnConfiguration</span></span>](../resources/intune-deviceconfig-windows10vpnconfiguration.md)|<span data-ttu-id="73ed8-120">读取 [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="73ed8-120">Read properties and relationships of the [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) object.</span></span>|
|[<span data-ttu-id="73ed8-121">创建 windows10VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="73ed8-121">Create windows10VpnConfiguration</span></span>](../api/intune-deviceconfig-windows10vpnconfiguration-create.md)|[<span data-ttu-id="73ed8-122">windows10VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="73ed8-122">windows10VpnConfiguration</span></span>](../resources/intune-deviceconfig-windows10vpnconfiguration.md)|<span data-ttu-id="73ed8-123">创建新的 [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="73ed8-123">Create a new [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) object.</span></span>|
|[<span data-ttu-id="73ed8-124">删除 windows10VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="73ed8-124">Delete windows10VpnConfiguration</span></span>](../api/intune-deviceconfig-windows10vpnconfiguration-delete.md)|<span data-ttu-id="73ed8-125">无</span><span class="sxs-lookup"><span data-stu-id="73ed8-125">None</span></span>|<span data-ttu-id="73ed8-126">删除 [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md)。</span><span class="sxs-lookup"><span data-stu-id="73ed8-126">Deletes a [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md).</span></span>|
|[<span data-ttu-id="73ed8-127">更新 windows10VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="73ed8-127">Update windows10VpnConfiguration</span></span>](../api/intune-deviceconfig-windows10vpnconfiguration-update.md)|[<span data-ttu-id="73ed8-128">windows10VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="73ed8-128">windows10VpnConfiguration</span></span>](../resources/intune-deviceconfig-windows10vpnconfiguration.md)|<span data-ttu-id="73ed8-129">更新 [windows10VpnConfiguration 对象](../resources/intune-deviceconfig-windows10vpnconfiguration.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="73ed8-129">Update the properties of a [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="73ed8-130">属性</span><span class="sxs-lookup"><span data-stu-id="73ed8-130">Properties</span></span>
|<span data-ttu-id="73ed8-131">属性</span><span class="sxs-lookup"><span data-stu-id="73ed8-131">Property</span></span>|<span data-ttu-id="73ed8-132">类型</span><span class="sxs-lookup"><span data-stu-id="73ed8-132">Type</span></span>|<span data-ttu-id="73ed8-133">说明</span><span class="sxs-lookup"><span data-stu-id="73ed8-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="73ed8-134">id</span><span class="sxs-lookup"><span data-stu-id="73ed8-134">id</span></span>|<span data-ttu-id="73ed8-135">String</span><span class="sxs-lookup"><span data-stu-id="73ed8-135">String</span></span>|<span data-ttu-id="73ed8-136">实体的键。</span><span class="sxs-lookup"><span data-stu-id="73ed8-136">Key of the entity.</span></span> <span data-ttu-id="73ed8-137">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="73ed8-137">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="73ed8-138">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="73ed8-138">lastModifiedDateTime</span></span>|<span data-ttu-id="73ed8-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="73ed8-139">DateTimeOffset</span></span>|<span data-ttu-id="73ed8-140">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="73ed8-140">DateTime the object was last modified.</span></span> <span data-ttu-id="73ed8-141">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="73ed8-141">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="73ed8-142">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="73ed8-142">roleScopeTagIds</span></span>|<span data-ttu-id="73ed8-143">字符串集合</span><span class="sxs-lookup"><span data-stu-id="73ed8-143">String collection</span></span>|<span data-ttu-id="73ed8-144">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="73ed8-144">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="73ed8-145">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="73ed8-145">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="73ed8-146">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="73ed8-146">supportsScopeTags</span></span>|<span data-ttu-id="73ed8-147">布尔</span><span class="sxs-lookup"><span data-stu-id="73ed8-147">Boolean</span></span>|<span data-ttu-id="73ed8-148">指示基础设备配置是否支持分配范围标记。</span><span class="sxs-lookup"><span data-stu-id="73ed8-148">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="73ed8-149">当此值为 false 且实体对范围用户不可见时，不允许向 ScopeTags 属性赋值。</span><span class="sxs-lookup"><span data-stu-id="73ed8-149">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="73ed8-150">对于在 Silverlight 中创建的旧策略，会发生此情况，可通过在 Azure 门户中删除和重新创建策略来解决此问题。</span><span class="sxs-lookup"><span data-stu-id="73ed8-150">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="73ed8-151">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="73ed8-151">This property is read-only.</span></span> <span data-ttu-id="73ed8-152">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="73ed8-152">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="73ed8-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="73ed8-153">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="73ed8-154">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="73ed8-154">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="73ed8-155">此策略的操作系统版本适用性。</span><span class="sxs-lookup"><span data-stu-id="73ed8-155">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="73ed8-156">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="73ed8-156">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="73ed8-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="73ed8-157">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="73ed8-158">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="73ed8-158">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="73ed8-159">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="73ed8-159">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="73ed8-160">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="73ed8-160">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="73ed8-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="73ed8-161">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="73ed8-162">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="73ed8-162">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="73ed8-163">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="73ed8-163">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="73ed8-164">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="73ed8-164">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="73ed8-165">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="73ed8-165">createdDateTime</span></span>|<span data-ttu-id="73ed8-166">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="73ed8-166">DateTimeOffset</span></span>|<span data-ttu-id="73ed8-167">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="73ed8-167">DateTime the object was created.</span></span> <span data-ttu-id="73ed8-168">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="73ed8-168">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="73ed8-169">说明</span><span class="sxs-lookup"><span data-stu-id="73ed8-169">description</span></span>|<span data-ttu-id="73ed8-170">String</span><span class="sxs-lookup"><span data-stu-id="73ed8-170">String</span></span>|<span data-ttu-id="73ed8-171">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="73ed8-171">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="73ed8-172">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="73ed8-172">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="73ed8-173">displayName</span><span class="sxs-lookup"><span data-stu-id="73ed8-173">displayName</span></span>|<span data-ttu-id="73ed8-174">String</span><span class="sxs-lookup"><span data-stu-id="73ed8-174">String</span></span>|<span data-ttu-id="73ed8-175">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="73ed8-175">Admin provided name of the device configuration.</span></span> <span data-ttu-id="73ed8-176">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="73ed8-176">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="73ed8-177">version</span><span class="sxs-lookup"><span data-stu-id="73ed8-177">version</span></span>|<span data-ttu-id="73ed8-178">Int32</span><span class="sxs-lookup"><span data-stu-id="73ed8-178">Int32</span></span>|<span data-ttu-id="73ed8-179">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="73ed8-179">Version of the device configuration.</span></span> <span data-ttu-id="73ed8-180">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="73ed8-180">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="73ed8-181">connectionName</span><span class="sxs-lookup"><span data-stu-id="73ed8-181">connectionName</span></span>|<span data-ttu-id="73ed8-182">String</span><span class="sxs-lookup"><span data-stu-id="73ed8-182">String</span></span>|<span data-ttu-id="73ed8-183">向用户显示的连接名称。</span><span class="sxs-lookup"><span data-stu-id="73ed8-183">Connection name displayed to the user.</span></span> <span data-ttu-id="73ed8-184">继承自 [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="73ed8-184">Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="73ed8-185">服务器</span><span class="sxs-lookup"><span data-stu-id="73ed8-185">servers</span></span>|<span data-ttu-id="73ed8-186">[vpnServer](../resources/intune-deviceconfig-vpnserver.md) 集合</span><span class="sxs-lookup"><span data-stu-id="73ed8-186">[vpnServer](../resources/intune-deviceconfig-vpnserver.md) collection</span></span>|<span data-ttu-id="73ed8-187">网络上 VPN 服务器的列表。</span><span class="sxs-lookup"><span data-stu-id="73ed8-187">List of VPN Servers on the network.</span></span> <span data-ttu-id="73ed8-188">确保最终用户可以访问这些网络位置。</span><span class="sxs-lookup"><span data-stu-id="73ed8-188">Make sure end users can access these network locations.</span></span> <span data-ttu-id="73ed8-189">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="73ed8-189">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="73ed8-190">继承自 [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="73ed8-190">Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="73ed8-191">customXml</span><span class="sxs-lookup"><span data-stu-id="73ed8-191">customXml</span></span>|<span data-ttu-id="73ed8-192">Binary</span><span class="sxs-lookup"><span data-stu-id="73ed8-192">Binary</span></span>|<span data-ttu-id="73ed8-193">配置 VPN 连接的自定义 XML 命令。</span><span class="sxs-lookup"><span data-stu-id="73ed8-193">Custom XML commands that configures the VPN connection.</span></span> <span data-ttu-id="73ed8-194"> (UTF8 编码的字节数组) 继承自 [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="73ed8-194">(UTF8 encoded byte array) Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="73ed8-195">profileTarget</span><span class="sxs-lookup"><span data-stu-id="73ed8-195">profileTarget</span></span>|[<span data-ttu-id="73ed8-196">windows10VpnProfileTarget</span><span class="sxs-lookup"><span data-stu-id="73ed8-196">windows10VpnProfileTarget</span></span>](../resources/intune-deviceconfig-windows10vpnprofiletarget.md)|<span data-ttu-id="73ed8-197">配置文件目标类型。</span><span class="sxs-lookup"><span data-stu-id="73ed8-197">Profile target type.</span></span> <span data-ttu-id="73ed8-198">可取值为：`user`、`device`、`autoPilotDevice`。</span><span class="sxs-lookup"><span data-stu-id="73ed8-198">Possible values are: `user`, `device`, `autoPilotDevice`.</span></span>|
|<span data-ttu-id="73ed8-199">connectionType</span><span class="sxs-lookup"><span data-stu-id="73ed8-199">connectionType</span></span>|[<span data-ttu-id="73ed8-200">windows10VpnConnectionType</span><span class="sxs-lookup"><span data-stu-id="73ed8-200">windows10VpnConnectionType</span></span>](../resources/intune-deviceconfig-windows10vpnconnectiontype.md)|<span data-ttu-id="73ed8-201">连接类型。</span><span class="sxs-lookup"><span data-stu-id="73ed8-201">Connection type.</span></span> <span data-ttu-id="73ed8-202">可取值为：`pulseSecure`、`f5EdgeClient`、`dellSonicWallMobileConnect`、`checkPointCapsuleVpn`、`automatic`、`ikEv2`、`l2tp`、`pptp`、`citrix`、`paloAltoGlobalProtect`、`ciscoAnyConnect`。</span><span class="sxs-lookup"><span data-stu-id="73ed8-202">Possible values are: `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `automatic`, `ikEv2`, `l2tp`, `pptp`, `citrix`, `paloAltoGlobalProtect`, `ciscoAnyConnect`.</span></span>|
|<span data-ttu-id="73ed8-203">enableSplitTunneling</span><span class="sxs-lookup"><span data-stu-id="73ed8-203">enableSplitTunneling</span></span>|<span data-ttu-id="73ed8-204">布尔</span><span class="sxs-lookup"><span data-stu-id="73ed8-204">Boolean</span></span>|<span data-ttu-id="73ed8-205">启用拆分隧道。</span><span class="sxs-lookup"><span data-stu-id="73ed8-205">Enable split tunneling.</span></span>|
|<span data-ttu-id="73ed8-206">enableAlwaysOn</span><span class="sxs-lookup"><span data-stu-id="73ed8-206">enableAlwaysOn</span></span>|<span data-ttu-id="73ed8-207">布尔</span><span class="sxs-lookup"><span data-stu-id="73ed8-207">Boolean</span></span>|<span data-ttu-id="73ed8-208">启用 Always On 模式。</span><span class="sxs-lookup"><span data-stu-id="73ed8-208">Enable Always On mode.</span></span>|
|<span data-ttu-id="73ed8-209">enableDeviceTunnel</span><span class="sxs-lookup"><span data-stu-id="73ed8-209">enableDeviceTunnel</span></span>|<span data-ttu-id="73ed8-210">布尔</span><span class="sxs-lookup"><span data-stu-id="73ed8-210">Boolean</span></span>|<span data-ttu-id="73ed8-211">启用设备隧道。</span><span class="sxs-lookup"><span data-stu-id="73ed8-211">Enable device tunnel.</span></span>|
|<span data-ttu-id="73ed8-212">enableDnsRegistration</span><span class="sxs-lookup"><span data-stu-id="73ed8-212">enableDnsRegistration</span></span>|<span data-ttu-id="73ed8-213">布尔</span><span class="sxs-lookup"><span data-stu-id="73ed8-213">Boolean</span></span>|<span data-ttu-id="73ed8-214">使用内部 DNS 启用 IP 地址注册。</span><span class="sxs-lookup"><span data-stu-id="73ed8-214">Enable IP address registration with internal DNS.</span></span>|
|<span data-ttu-id="73ed8-215">dnsSuffixes</span><span class="sxs-lookup"><span data-stu-id="73ed8-215">dnsSuffixes</span></span>|<span data-ttu-id="73ed8-216">字符串集合</span><span class="sxs-lookup"><span data-stu-id="73ed8-216">String collection</span></span>|<span data-ttu-id="73ed8-217">指定要添加到 DNS 搜索列表的 DNS 后缀，以正确路由短名称。</span><span class="sxs-lookup"><span data-stu-id="73ed8-217">Specify DNS suffixes to add to the DNS search list to properly route short names.</span></span>|
|<span data-ttu-id="73ed8-218">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="73ed8-218">authenticationMethod</span></span>|[<span data-ttu-id="73ed8-219">windows10VpnAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="73ed8-219">windows10VpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-windows10vpnauthenticationmethod.md)|<span data-ttu-id="73ed8-220">身份验证方法。</span><span class="sxs-lookup"><span data-stu-id="73ed8-220">Authentication method.</span></span> <span data-ttu-id="73ed8-221">可取值为：`certificate`、`usernameAndPassword`、`customEapXml`、`derivedCredential`。</span><span class="sxs-lookup"><span data-stu-id="73ed8-221">Possible values are: `certificate`, `usernameAndPassword`, `customEapXml`, `derivedCredential`.</span></span>|
|<span data-ttu-id="73ed8-222">rememberUserCredentials</span><span class="sxs-lookup"><span data-stu-id="73ed8-222">rememberUserCredentials</span></span>|<span data-ttu-id="73ed8-223">布尔</span><span class="sxs-lookup"><span data-stu-id="73ed8-223">Boolean</span></span>|<span data-ttu-id="73ed8-224">请记住用户凭据。</span><span class="sxs-lookup"><span data-stu-id="73ed8-224">Remember user credentials.</span></span>|
|<span data-ttu-id="73ed8-225">enableConditionalAccess</span><span class="sxs-lookup"><span data-stu-id="73ed8-225">enableConditionalAccess</span></span>|<span data-ttu-id="73ed8-226">布尔</span><span class="sxs-lookup"><span data-stu-id="73ed8-226">Boolean</span></span>|<span data-ttu-id="73ed8-227">启用条件访问。</span><span class="sxs-lookup"><span data-stu-id="73ed8-227">Enable conditional access.</span></span>|
|<span data-ttu-id="73ed8-228">enableSingleSignOnWithAlternateCertificate</span><span class="sxs-lookup"><span data-stu-id="73ed8-228">enableSingleSignOnWithAlternateCertificate</span></span>|<span data-ttu-id="73ed8-229">布尔</span><span class="sxs-lookup"><span data-stu-id="73ed8-229">Boolean</span></span>|<span data-ttu-id="73ed8-230">使用备用证书为 SSO (单一) 登录。</span><span class="sxs-lookup"><span data-stu-id="73ed8-230">Enable single sign-on (SSO) with alternate certificate.</span></span>|
|<span data-ttu-id="73ed8-231">singleSignOnEku</span><span class="sxs-lookup"><span data-stu-id="73ed8-231">singleSignOnEku</span></span>|[<span data-ttu-id="73ed8-232">extendedKeyUsage</span><span class="sxs-lookup"><span data-stu-id="73ed8-232">extendedKeyUsage</span></span>](../resources/intune-shared-extendedkeyusage.md)|<span data-ttu-id="73ed8-233">单一登录扩展密钥使用 (EKU) 。</span><span class="sxs-lookup"><span data-stu-id="73ed8-233">Single sign-on Extended Key Usage (EKU).</span></span>|
|<span data-ttu-id="73ed8-234">singleSignOnIssuerHash</span><span class="sxs-lookup"><span data-stu-id="73ed8-234">singleSignOnIssuerHash</span></span>|<span data-ttu-id="73ed8-235">String</span><span class="sxs-lookup"><span data-stu-id="73ed8-235">String</span></span>|<span data-ttu-id="73ed8-236">单一登录颁发者哈希。</span><span class="sxs-lookup"><span data-stu-id="73ed8-236">Single sign-on issuer hash.</span></span>|
|<span data-ttu-id="73ed8-237">eapXml</span><span class="sxs-lookup"><span data-stu-id="73ed8-237">eapXml</span></span>|<span data-ttu-id="73ed8-238">Binary</span><span class="sxs-lookup"><span data-stu-id="73ed8-238">Binary</span></span>|<span data-ttu-id="73ed8-239">可扩展身份验证协议 (EAP) XML。</span><span class="sxs-lookup"><span data-stu-id="73ed8-239">Extensible Authentication Protocol (EAP) XML.</span></span> <span data-ttu-id="73ed8-240">（UTF8 编码的字节数组）</span><span class="sxs-lookup"><span data-stu-id="73ed8-240">(UTF8 encoded byte array)</span></span>|
|<span data-ttu-id="73ed8-241">proxyServer</span><span class="sxs-lookup"><span data-stu-id="73ed8-241">proxyServer</span></span>|[<span data-ttu-id="73ed8-242">windows10VpnProxyServer</span><span class="sxs-lookup"><span data-stu-id="73ed8-242">windows10VpnProxyServer</span></span>](../resources/intune-deviceconfig-windows10vpnproxyserver.md)|<span data-ttu-id="73ed8-243">代理服务器。</span><span class="sxs-lookup"><span data-stu-id="73ed8-243">Proxy Server.</span></span>|
|<span data-ttu-id="73ed8-244">associatedApps</span><span class="sxs-lookup"><span data-stu-id="73ed8-244">associatedApps</span></span>|<span data-ttu-id="73ed8-245">[windows10AssociatedApps](../resources/intune-deviceconfig-windows10associatedapps.md) 集合</span><span class="sxs-lookup"><span data-stu-id="73ed8-245">[windows10AssociatedApps](../resources/intune-deviceconfig-windows10associatedapps.md) collection</span></span>|<span data-ttu-id="73ed8-246">关联的应用。</span><span class="sxs-lookup"><span data-stu-id="73ed8-246">Associated Apps.</span></span> <span data-ttu-id="73ed8-247">该集合最多可包含 10000 个元素。</span><span class="sxs-lookup"><span data-stu-id="73ed8-247">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="73ed8-248">仅AssociatedAppsCanUseConnection</span><span class="sxs-lookup"><span data-stu-id="73ed8-248">onlyAssociatedAppsCanUseConnection</span></span>|<span data-ttu-id="73ed8-249">布尔</span><span class="sxs-lookup"><span data-stu-id="73ed8-249">Boolean</span></span>|<span data-ttu-id="73ed8-250">只有关联的应用可以使用每个应用 VPN (连接) 。</span><span class="sxs-lookup"><span data-stu-id="73ed8-250">Only associated Apps can use connection (per-app VPN).</span></span>|
|<span data-ttu-id="73ed8-251">windowsInformationProtectionDomain</span><span class="sxs-lookup"><span data-stu-id="73ed8-251">windowsInformationProtectionDomain</span></span>|<span data-ttu-id="73ed8-252">String</span><span class="sxs-lookup"><span data-stu-id="73ed8-252">String</span></span>|<span data-ttu-id="73ed8-253">Windows 信息保护 (WIP) 域，以与此连接关联。</span><span class="sxs-lookup"><span data-stu-id="73ed8-253">Windows Information Protection (WIP) domain to associate with this connection.</span></span>|
|<span data-ttu-id="73ed8-254">trafficRules</span><span class="sxs-lookup"><span data-stu-id="73ed8-254">trafficRules</span></span>|<span data-ttu-id="73ed8-255">[vpnTrafficRule](../resources/intune-deviceconfig-vpntrafficrule.md) 集合</span><span class="sxs-lookup"><span data-stu-id="73ed8-255">[vpnTrafficRule](../resources/intune-deviceconfig-vpntrafficrule.md) collection</span></span>|<span data-ttu-id="73ed8-256">流量规则。</span><span class="sxs-lookup"><span data-stu-id="73ed8-256">Traffic rules.</span></span> <span data-ttu-id="73ed8-257">该集合最多可包含 1000 个元素。</span><span class="sxs-lookup"><span data-stu-id="73ed8-257">This collection can contain a maximum of 1000 elements.</span></span>|
|<span data-ttu-id="73ed8-258">routes</span><span class="sxs-lookup"><span data-stu-id="73ed8-258">routes</span></span>|<span data-ttu-id="73ed8-259">[vpnRoute](../resources/intune-deviceconfig-vpnroute.md) 集合</span><span class="sxs-lookup"><span data-stu-id="73ed8-259">[vpnRoute](../resources/intune-deviceconfig-vpnroute.md) collection</span></span>|<span data-ttu-id="73ed8-260">路由 (第三方提供商的可选) 。</span><span class="sxs-lookup"><span data-stu-id="73ed8-260">Routes (optional for third-party providers).</span></span> <span data-ttu-id="73ed8-261">该集合最多可包含 1000 个元素。</span><span class="sxs-lookup"><span data-stu-id="73ed8-261">This collection can contain a maximum of 1000 elements.</span></span>|
|<span data-ttu-id="73ed8-262">dnsRules</span><span class="sxs-lookup"><span data-stu-id="73ed8-262">dnsRules</span></span>|<span data-ttu-id="73ed8-263">[vpnDnsRule](../resources/intune-deviceconfig-vpndnsrule.md) 集合</span><span class="sxs-lookup"><span data-stu-id="73ed8-263">[vpnDnsRule](../resources/intune-deviceconfig-vpndnsrule.md) collection</span></span>|<span data-ttu-id="73ed8-264">DNS 规则。</span><span class="sxs-lookup"><span data-stu-id="73ed8-264">DNS rules.</span></span> <span data-ttu-id="73ed8-265">该集合最多可包含 1000 个元素。</span><span class="sxs-lookup"><span data-stu-id="73ed8-265">This collection can contain a maximum of 1000 elements.</span></span>|
|<span data-ttu-id="73ed8-266">trustedNetworkDomains</span><span class="sxs-lookup"><span data-stu-id="73ed8-266">trustedNetworkDomains</span></span>|<span data-ttu-id="73ed8-267">字符串集合</span><span class="sxs-lookup"><span data-stu-id="73ed8-267">String collection</span></span>|<span data-ttu-id="73ed8-268">受信任的网络域</span><span class="sxs-lookup"><span data-stu-id="73ed8-268">Trusted Network Domains</span></span>|
|<span data-ttu-id="73ed8-269">cryptographySuite</span><span class="sxs-lookup"><span data-stu-id="73ed8-269">cryptographySuite</span></span>|[<span data-ttu-id="73ed8-270">cryptographySuite</span><span class="sxs-lookup"><span data-stu-id="73ed8-270">cryptographySuite</span></span>](../resources/intune-deviceconfig-cryptographysuite.md)|<span data-ttu-id="73ed8-271">Windows 10 及以上版 IKEv2 VPN 的加密套件安全设置</span><span class="sxs-lookup"><span data-stu-id="73ed8-271">Cryptography Suite security settings for IKEv2 VPN in Windows10 and above</span></span> |

## <a name="relationships"></a><span data-ttu-id="73ed8-272">关系</span><span class="sxs-lookup"><span data-stu-id="73ed8-272">Relationships</span></span>
|<span data-ttu-id="73ed8-273">关系</span><span class="sxs-lookup"><span data-stu-id="73ed8-273">Relationship</span></span>|<span data-ttu-id="73ed8-274">类型</span><span class="sxs-lookup"><span data-stu-id="73ed8-274">Type</span></span>|<span data-ttu-id="73ed8-275">说明</span><span class="sxs-lookup"><span data-stu-id="73ed8-275">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="73ed8-276">groupAssignments</span><span class="sxs-lookup"><span data-stu-id="73ed8-276">groupAssignments</span></span>|<span data-ttu-id="73ed8-277">[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="73ed8-277">[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) collection</span></span>|<span data-ttu-id="73ed8-278">设备配置文件的组分配列表。</span><span class="sxs-lookup"><span data-stu-id="73ed8-278">The list of group assignments for the device configuration profile.</span></span> <span data-ttu-id="73ed8-279">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="73ed8-279">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="73ed8-280">assignments</span><span class="sxs-lookup"><span data-stu-id="73ed8-280">assignments</span></span>|<span data-ttu-id="73ed8-281">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="73ed8-281">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection</span></span>|<span data-ttu-id="73ed8-282">设备配置文件的分配列表。</span><span class="sxs-lookup"><span data-stu-id="73ed8-282">The list of assignments for the device configuration profile.</span></span> <span data-ttu-id="73ed8-283">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="73ed8-283">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="73ed8-284">deviceStatuses</span><span class="sxs-lookup"><span data-stu-id="73ed8-284">deviceStatuses</span></span>|<span data-ttu-id="73ed8-285">[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) 集合</span><span class="sxs-lookup"><span data-stu-id="73ed8-285">[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) collection</span></span>|<span data-ttu-id="73ed8-286">按设备的设备配置安装状态。</span><span class="sxs-lookup"><span data-stu-id="73ed8-286">Device configuration installation status by device.</span></span> <span data-ttu-id="73ed8-287">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="73ed8-287">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="73ed8-288">userStatuses</span><span class="sxs-lookup"><span data-stu-id="73ed8-288">userStatuses</span></span>|<span data-ttu-id="73ed8-289">[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) 集合</span><span class="sxs-lookup"><span data-stu-id="73ed8-289">[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) collection</span></span>|<span data-ttu-id="73ed8-290">用户的设备配置安装状态。</span><span class="sxs-lookup"><span data-stu-id="73ed8-290">Device configuration installation status by user.</span></span> <span data-ttu-id="73ed8-291">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="73ed8-291">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="73ed8-292">deviceStatusOverview</span><span class="sxs-lookup"><span data-stu-id="73ed8-292">deviceStatusOverview</span></span>|[<span data-ttu-id="73ed8-293">deviceConfigurationDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="73ed8-293">deviceConfigurationDeviceOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|<span data-ttu-id="73ed8-294">设备配置设备状态概述 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="73ed8-294">Device Configuration devices status overview Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="73ed8-295">userStatusOverview</span><span class="sxs-lookup"><span data-stu-id="73ed8-295">userStatusOverview</span></span>|[<span data-ttu-id="73ed8-296">deviceConfigurationUserOverview</span><span class="sxs-lookup"><span data-stu-id="73ed8-296">deviceConfigurationUserOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|<span data-ttu-id="73ed8-297">设备配置用户状态概述 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="73ed8-297">Device Configuration users status overview Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="73ed8-298">deviceSettingStateSummaries</span><span class="sxs-lookup"><span data-stu-id="73ed8-298">deviceSettingStateSummaries</span></span>|<span data-ttu-id="73ed8-299">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) 集合</span><span class="sxs-lookup"><span data-stu-id="73ed8-299">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) collection</span></span>|<span data-ttu-id="73ed8-300">设备配置设置状态设备摘要 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="73ed8-300">Device Configuration Setting State Device Summary Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="73ed8-301">identityCertificate</span><span class="sxs-lookup"><span data-stu-id="73ed8-301">identityCertificate</span></span>|[<span data-ttu-id="73ed8-302">windowsCertificateProfileBase</span><span class="sxs-lookup"><span data-stu-id="73ed8-302">windowsCertificateProfileBase</span></span>](../resources/intune-deviceconfig-windowscertificateprofilebase.md)|<span data-ttu-id="73ed8-303">身份验证方法是证书时用于客户端身份验证的标识证书。</span><span class="sxs-lookup"><span data-stu-id="73ed8-303">Identity certificate for client authentication when authentication method is certificate.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="73ed8-304">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="73ed8-304">JSON Representation</span></span>
<span data-ttu-id="73ed8-305">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="73ed8-305">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windows10VpnConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windows10VpnConfiguration",
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
  "customXml": "binary",
  "profileTarget": "String",
  "connectionType": "String",
  "enableSplitTunneling": true,
  "enableAlwaysOn": true,
  "enableDeviceTunnel": true,
  "enableDnsRegistration": true,
  "dnsSuffixes": [
    "String"
  ],
  "authenticationMethod": "String",
  "rememberUserCredentials": true,
  "enableConditionalAccess": true,
  "enableSingleSignOnWithAlternateCertificate": true,
  "singleSignOnEku": {
    "@odata.type": "microsoft.graph.extendedKeyUsage",
    "name": "String",
    "objectIdentifier": "String"
  },
  "singleSignOnIssuerHash": "String",
  "eapXml": "binary",
  "proxyServer": {
    "@odata.type": "microsoft.graph.windows10VpnProxyServer",
    "automaticConfigurationScriptUrl": "String",
    "address": "String",
    "port": 1024,
    "bypassProxyServerForLocalAddress": true
  },
  "associatedApps": [
    {
      "@odata.type": "microsoft.graph.windows10AssociatedApps",
      "appType": "String",
      "identifier": "String"
    }
  ],
  "onlyAssociatedAppsCanUseConnection": true,
  "windowsInformationProtectionDomain": "String",
  "trafficRules": [
    {
      "@odata.type": "microsoft.graph.vpnTrafficRule",
      "name": "String",
      "protocols": 1024,
      "localPortRanges": [
        {
          "@odata.type": "microsoft.graph.numberRange",
          "lowerNumber": 1024,
          "upperNumber": 1024
        }
      ],
      "remotePortRanges": [
        {
          "@odata.type": "microsoft.graph.numberRange",
          "lowerNumber": 1024,
          "upperNumber": 1024
        }
      ],
      "localAddressRanges": [
        {
          "@odata.type": "microsoft.graph.iPv4Range",
          "lowerAddress": "String",
          "upperAddress": "String"
        }
      ],
      "remoteAddressRanges": [
        {
          "@odata.type": "microsoft.graph.iPv4Range",
          "lowerAddress": "String",
          "upperAddress": "String"
        }
      ],
      "appId": "String",
      "appType": "String",
      "routingPolicyType": "String",
      "claims": "String"
    }
  ],
  "routes": [
    {
      "@odata.type": "microsoft.graph.vpnRoute",
      "destinationPrefix": "String",
      "prefixSize": 1024
    }
  ],
  "dnsRules": [
    {
      "@odata.type": "microsoft.graph.vpnDnsRule",
      "name": "String",
      "servers": [
        "String"
      ],
      "proxyServerUri": "String",
      "autoTrigger": true,
      "persistent": true
    }
  ],
  "trustedNetworkDomains": [
    "String"
  ],
  "cryptographySuite": {
    "@odata.type": "microsoft.graph.cryptographySuite",
    "encryptionMethod": "String",
    "integrityCheckMethod": "String",
    "dhGroup": "String",
    "cipherTransformConstants": "String",
    "authenticationTransformConstants": "String",
    "pfsGroup": "String"
  }
}
```




