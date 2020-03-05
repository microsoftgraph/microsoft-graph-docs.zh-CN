---
title: windows10VpnConfiguration 资源类型
description: 通过提供此配置文件中的配置，可以指示 Windows 10 设备（桌面或移动版）连接到所需的 VPN 终结点。 通过指定 VPN 终结点预期的身份验证方法和安全类型，可以为最终用户进行无缝的 VPN 连接。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: fa280abad6a6d70681936d071d395b163ca85785
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42525619"
---
# <a name="windows10vpnconfiguration-resource-type"></a><span data-ttu-id="faaa9-104">windows10VpnConfiguration 资源类型</span><span class="sxs-lookup"><span data-stu-id="faaa9-104">windows10VpnConfiguration resource type</span></span>

<span data-ttu-id="faaa9-105">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="faaa9-105">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="faaa9-106">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="faaa9-106">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="faaa9-107">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="faaa9-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="faaa9-108">通过提供此配置文件中的配置，可以指示 Windows 10 设备（桌面或移动版）连接到所需的 VPN 终结点。</span><span class="sxs-lookup"><span data-stu-id="faaa9-108">By providing the configurations in this profile you can instruct the Windows 10 device (desktop or mobile) to connect to desired VPN endpoint.</span></span> <span data-ttu-id="faaa9-109">通过指定 VPN 终结点预期的身份验证方法和安全类型，可以为最终用户进行无缝的 VPN 连接。</span><span class="sxs-lookup"><span data-stu-id="faaa9-109">By specifying the authentication method and security types expected by VPN endpoint you can make the VPN connection seamless for end user.</span></span>


<span data-ttu-id="faaa9-110">继承自[windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="faaa9-110">Inherits from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>

## <a name="methods"></a><span data-ttu-id="faaa9-111">方法</span><span class="sxs-lookup"><span data-stu-id="faaa9-111">Methods</span></span>
|<span data-ttu-id="faaa9-112">方法</span><span class="sxs-lookup"><span data-stu-id="faaa9-112">Method</span></span>|<span data-ttu-id="faaa9-113">返回类型</span><span class="sxs-lookup"><span data-stu-id="faaa9-113">Return Type</span></span>|<span data-ttu-id="faaa9-114">说明</span><span class="sxs-lookup"><span data-stu-id="faaa9-114">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="faaa9-115">列出 windows10VpnConfigurations</span><span class="sxs-lookup"><span data-stu-id="faaa9-115">List windows10VpnConfigurations</span></span>](../api/intune-deviceconfig-windows10vpnconfiguration-list.md)|<span data-ttu-id="faaa9-116">[windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md)集合</span><span class="sxs-lookup"><span data-stu-id="faaa9-116">[windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) collection</span></span>|<span data-ttu-id="faaa9-117">列出[windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="faaa9-117">List properties and relationships of the [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="faaa9-118">获取 windows10VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="faaa9-118">Get windows10VpnConfiguration</span></span>](../api/intune-deviceconfig-windows10vpnconfiguration-get.md)|[<span data-ttu-id="faaa9-119">windows10VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="faaa9-119">windows10VpnConfiguration</span></span>](../resources/intune-deviceconfig-windows10vpnconfiguration.md)|<span data-ttu-id="faaa9-120">读取[windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="faaa9-120">Read properties and relationships of the [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) object.</span></span>|
|[<span data-ttu-id="faaa9-121">创建 windows10VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="faaa9-121">Create windows10VpnConfiguration</span></span>](../api/intune-deviceconfig-windows10vpnconfiguration-create.md)|[<span data-ttu-id="faaa9-122">windows10VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="faaa9-122">windows10VpnConfiguration</span></span>](../resources/intune-deviceconfig-windows10vpnconfiguration.md)|<span data-ttu-id="faaa9-123">创建新的[windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="faaa9-123">Create a new [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) object.</span></span>|
|[<span data-ttu-id="faaa9-124">删除 windows10VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="faaa9-124">Delete windows10VpnConfiguration</span></span>](../api/intune-deviceconfig-windows10vpnconfiguration-delete.md)|<span data-ttu-id="faaa9-125">无</span><span class="sxs-lookup"><span data-stu-id="faaa9-125">None</span></span>|<span data-ttu-id="faaa9-126">删除[windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md)。</span><span class="sxs-lookup"><span data-stu-id="faaa9-126">Deletes a [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md).</span></span>|
|[<span data-ttu-id="faaa9-127">更新 windows10VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="faaa9-127">Update windows10VpnConfiguration</span></span>](../api/intune-deviceconfig-windows10vpnconfiguration-update.md)|[<span data-ttu-id="faaa9-128">windows10VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="faaa9-128">windows10VpnConfiguration</span></span>](../resources/intune-deviceconfig-windows10vpnconfiguration.md)|<span data-ttu-id="faaa9-129">更新[windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="faaa9-129">Update the properties of a [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="faaa9-130">属性</span><span class="sxs-lookup"><span data-stu-id="faaa9-130">Properties</span></span>
|<span data-ttu-id="faaa9-131">属性</span><span class="sxs-lookup"><span data-stu-id="faaa9-131">Property</span></span>|<span data-ttu-id="faaa9-132">类型</span><span class="sxs-lookup"><span data-stu-id="faaa9-132">Type</span></span>|<span data-ttu-id="faaa9-133">说明</span><span class="sxs-lookup"><span data-stu-id="faaa9-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="faaa9-134">id</span><span class="sxs-lookup"><span data-stu-id="faaa9-134">id</span></span>|<span data-ttu-id="faaa9-135">字符串</span><span class="sxs-lookup"><span data-stu-id="faaa9-135">String</span></span>|<span data-ttu-id="faaa9-136">实体的键。</span><span class="sxs-lookup"><span data-stu-id="faaa9-136">Key of the entity.</span></span> <span data-ttu-id="faaa9-137">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="faaa9-137">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="faaa9-138">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="faaa9-138">lastModifiedDateTime</span></span>|<span data-ttu-id="faaa9-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="faaa9-139">DateTimeOffset</span></span>|<span data-ttu-id="faaa9-140">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="faaa9-140">DateTime the object was last modified.</span></span> <span data-ttu-id="faaa9-141">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="faaa9-141">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="faaa9-142">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="faaa9-142">roleScopeTagIds</span></span>|<span data-ttu-id="faaa9-143">String 集合</span><span class="sxs-lookup"><span data-stu-id="faaa9-143">String collection</span></span>|<span data-ttu-id="faaa9-144">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="faaa9-144">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="faaa9-145">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="faaa9-145">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="faaa9-146">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="faaa9-146">supportsScopeTags</span></span>|<span data-ttu-id="faaa9-147">布尔</span><span class="sxs-lookup"><span data-stu-id="faaa9-147">Boolean</span></span>|<span data-ttu-id="faaa9-148">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="faaa9-148">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="faaa9-149">如果此值为 false，则不允许分配给 ScopeTags 属性，并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="faaa9-149">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="faaa9-150">这适用于在 Silverlight 中创建的旧版策略，可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="faaa9-150">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="faaa9-151">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="faaa9-151">This property is read-only.</span></span> <span data-ttu-id="faaa9-152">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="faaa9-152">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="faaa9-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="faaa9-153">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="faaa9-154">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="faaa9-154">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="faaa9-155">适用于此策略的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="faaa9-155">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="faaa9-156">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="faaa9-156">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="faaa9-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="faaa9-157">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="faaa9-158">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="faaa9-158">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="faaa9-159">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="faaa9-159">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="faaa9-160">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="faaa9-160">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="faaa9-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="faaa9-161">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="faaa9-162">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="faaa9-162">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="faaa9-163">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="faaa9-163">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="faaa9-164">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="faaa9-164">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="faaa9-165">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="faaa9-165">createdDateTime</span></span>|<span data-ttu-id="faaa9-166">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="faaa9-166">DateTimeOffset</span></span>|<span data-ttu-id="faaa9-167">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="faaa9-167">DateTime the object was created.</span></span> <span data-ttu-id="faaa9-168">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="faaa9-168">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="faaa9-169">说明</span><span class="sxs-lookup"><span data-stu-id="faaa9-169">description</span></span>|<span data-ttu-id="faaa9-170">String</span><span class="sxs-lookup"><span data-stu-id="faaa9-170">String</span></span>|<span data-ttu-id="faaa9-171">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="faaa9-171">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="faaa9-172">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="faaa9-172">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="faaa9-173">displayName</span><span class="sxs-lookup"><span data-stu-id="faaa9-173">displayName</span></span>|<span data-ttu-id="faaa9-174">String</span><span class="sxs-lookup"><span data-stu-id="faaa9-174">String</span></span>|<span data-ttu-id="faaa9-175">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="faaa9-175">Admin provided name of the device configuration.</span></span> <span data-ttu-id="faaa9-176">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="faaa9-176">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="faaa9-177">version</span><span class="sxs-lookup"><span data-stu-id="faaa9-177">version</span></span>|<span data-ttu-id="faaa9-178">Int32</span><span class="sxs-lookup"><span data-stu-id="faaa9-178">Int32</span></span>|<span data-ttu-id="faaa9-179">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="faaa9-179">Version of the device configuration.</span></span> <span data-ttu-id="faaa9-180">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="faaa9-180">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="faaa9-181">connectionName</span><span class="sxs-lookup"><span data-stu-id="faaa9-181">connectionName</span></span>|<span data-ttu-id="faaa9-182">String</span><span class="sxs-lookup"><span data-stu-id="faaa9-182">String</span></span>|<span data-ttu-id="faaa9-183">向用户显示的连接名称。</span><span class="sxs-lookup"><span data-stu-id="faaa9-183">Connection name displayed to the user.</span></span> <span data-ttu-id="faaa9-184">继承自[windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="faaa9-184">Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="faaa9-185">台</span><span class="sxs-lookup"><span data-stu-id="faaa9-185">servers</span></span>|<span data-ttu-id="faaa9-186">[vpnServer](../resources/intune-deviceconfig-vpnserver.md)集合</span><span class="sxs-lookup"><span data-stu-id="faaa9-186">[vpnServer](../resources/intune-deviceconfig-vpnserver.md) collection</span></span>|<span data-ttu-id="faaa9-187">网络上的 VPN 服务器的列表。</span><span class="sxs-lookup"><span data-stu-id="faaa9-187">List of VPN Servers on the network.</span></span> <span data-ttu-id="faaa9-188">请确保最终用户可以访问这些网络位置。</span><span class="sxs-lookup"><span data-stu-id="faaa9-188">Make sure end users can access these network locations.</span></span> <span data-ttu-id="faaa9-189">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="faaa9-189">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="faaa9-190">继承自[windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="faaa9-190">Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="faaa9-191">customXml</span><span class="sxs-lookup"><span data-stu-id="faaa9-191">customXml</span></span>|<span data-ttu-id="faaa9-192">Binary</span><span class="sxs-lookup"><span data-stu-id="faaa9-192">Binary</span></span>|<span data-ttu-id="faaa9-193">配置 VPN 连接的自定义 XML 命令。</span><span class="sxs-lookup"><span data-stu-id="faaa9-193">Custom XML commands that configures the VPN connection.</span></span> <span data-ttu-id="faaa9-194">（UTF8 编码的字节数组）继承自[windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="faaa9-194">(UTF8 encoded byte array) Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="faaa9-195">profileTarget</span><span class="sxs-lookup"><span data-stu-id="faaa9-195">profileTarget</span></span>|[<span data-ttu-id="faaa9-196">windows10VpnProfileTarget</span><span class="sxs-lookup"><span data-stu-id="faaa9-196">windows10VpnProfileTarget</span></span>](../resources/intune-deviceconfig-windows10vpnprofiletarget.md)|<span data-ttu-id="faaa9-197">配置文件目标类型。</span><span class="sxs-lookup"><span data-stu-id="faaa9-197">Profile target type.</span></span> <span data-ttu-id="faaa9-198">可取值为：`user`、`device`、`autoPilotDevice`。</span><span class="sxs-lookup"><span data-stu-id="faaa9-198">Possible values are: `user`, `device`, `autoPilotDevice`.</span></span>|
|<span data-ttu-id="faaa9-199">connectionType</span><span class="sxs-lookup"><span data-stu-id="faaa9-199">connectionType</span></span>|[<span data-ttu-id="faaa9-200">windows10VpnConnectionType</span><span class="sxs-lookup"><span data-stu-id="faaa9-200">windows10VpnConnectionType</span></span>](../resources/intune-deviceconfig-windows10vpnconnectiontype.md)|<span data-ttu-id="faaa9-201">连接类型。</span><span class="sxs-lookup"><span data-stu-id="faaa9-201">Connection type.</span></span> <span data-ttu-id="faaa9-202">可取值为：`pulseSecure`、`f5EdgeClient`、`dellSonicWallMobileConnect`、`checkPointCapsuleVpn`、`automatic`、`ikEv2`、`l2tp`、`pptp`、`citrix`、`paloAltoGlobalProtect`。</span><span class="sxs-lookup"><span data-stu-id="faaa9-202">Possible values are: `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `automatic`, `ikEv2`, `l2tp`, `pptp`, `citrix`, `paloAltoGlobalProtect`.</span></span>|
|<span data-ttu-id="faaa9-203">enableSplitTunneling</span><span class="sxs-lookup"><span data-stu-id="faaa9-203">enableSplitTunneling</span></span>|<span data-ttu-id="faaa9-204">布尔</span><span class="sxs-lookup"><span data-stu-id="faaa9-204">Boolean</span></span>|<span data-ttu-id="faaa9-205">启用拆分隧道。</span><span class="sxs-lookup"><span data-stu-id="faaa9-205">Enable split tunneling.</span></span>|
|<span data-ttu-id="faaa9-206">enableAlwaysOn</span><span class="sxs-lookup"><span data-stu-id="faaa9-206">enableAlwaysOn</span></span>|<span data-ttu-id="faaa9-207">布尔</span><span class="sxs-lookup"><span data-stu-id="faaa9-207">Boolean</span></span>|<span data-ttu-id="faaa9-208">启用始终打开模式。</span><span class="sxs-lookup"><span data-stu-id="faaa9-208">Enable Always On mode.</span></span>|
|<span data-ttu-id="faaa9-209">enableDeviceTunnel</span><span class="sxs-lookup"><span data-stu-id="faaa9-209">enableDeviceTunnel</span></span>|<span data-ttu-id="faaa9-210">布尔</span><span class="sxs-lookup"><span data-stu-id="faaa9-210">Boolean</span></span>|<span data-ttu-id="faaa9-211">启用设备隧道。</span><span class="sxs-lookup"><span data-stu-id="faaa9-211">Enable device tunnel.</span></span>|
|<span data-ttu-id="faaa9-212">enableDnsRegistration</span><span class="sxs-lookup"><span data-stu-id="faaa9-212">enableDnsRegistration</span></span>|<span data-ttu-id="faaa9-213">布尔</span><span class="sxs-lookup"><span data-stu-id="faaa9-213">Boolean</span></span>|<span data-ttu-id="faaa9-214">使用内部 DNS 启用 IP 地址注册。</span><span class="sxs-lookup"><span data-stu-id="faaa9-214">Enable IP address registration with internal DNS.</span></span>|
|<span data-ttu-id="faaa9-215">dnsSuffixes</span><span class="sxs-lookup"><span data-stu-id="faaa9-215">dnsSuffixes</span></span>|<span data-ttu-id="faaa9-216">String 集合</span><span class="sxs-lookup"><span data-stu-id="faaa9-216">String collection</span></span>|<span data-ttu-id="faaa9-217">指定要添加到 DNS 搜索列表以正确路由短名称的 DNS 后缀。</span><span class="sxs-lookup"><span data-stu-id="faaa9-217">Specify DNS suffixes to add to the DNS search list to properly route short names.</span></span>|
|<span data-ttu-id="faaa9-218">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="faaa9-218">authenticationMethod</span></span>|[<span data-ttu-id="faaa9-219">windows10VpnAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="faaa9-219">windows10VpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-windows10vpnauthenticationmethod.md)|<span data-ttu-id="faaa9-220">身份验证方法。</span><span class="sxs-lookup"><span data-stu-id="faaa9-220">Authentication method.</span></span> <span data-ttu-id="faaa9-221">可取值为：`certificate`、`usernameAndPassword`、`customEapXml`。</span><span class="sxs-lookup"><span data-stu-id="faaa9-221">Possible values are: `certificate`, `usernameAndPassword`, `customEapXml`.</span></span>|
|<span data-ttu-id="faaa9-222">rememberUserCredentials</span><span class="sxs-lookup"><span data-stu-id="faaa9-222">rememberUserCredentials</span></span>|<span data-ttu-id="faaa9-223">布尔</span><span class="sxs-lookup"><span data-stu-id="faaa9-223">Boolean</span></span>|<span data-ttu-id="faaa9-224">记住用户凭据。</span><span class="sxs-lookup"><span data-stu-id="faaa9-224">Remember user credentials.</span></span>|
|<span data-ttu-id="faaa9-225">enableConditionalAccess</span><span class="sxs-lookup"><span data-stu-id="faaa9-225">enableConditionalAccess</span></span>|<span data-ttu-id="faaa9-226">布尔</span><span class="sxs-lookup"><span data-stu-id="faaa9-226">Boolean</span></span>|<span data-ttu-id="faaa9-227">启用条件访问。</span><span class="sxs-lookup"><span data-stu-id="faaa9-227">Enable conditional access.</span></span>|
|<span data-ttu-id="faaa9-228">enableSingleSignOnWithAlternateCertificate</span><span class="sxs-lookup"><span data-stu-id="faaa9-228">enableSingleSignOnWithAlternateCertificate</span></span>|<span data-ttu-id="faaa9-229">布尔</span><span class="sxs-lookup"><span data-stu-id="faaa9-229">Boolean</span></span>|<span data-ttu-id="faaa9-230">启用具有备用证书的单一登录（SSO）。</span><span class="sxs-lookup"><span data-stu-id="faaa9-230">Enable single sign-on (SSO) with alternate certificate.</span></span>|
|<span data-ttu-id="faaa9-231">singleSignOnEku</span><span class="sxs-lookup"><span data-stu-id="faaa9-231">singleSignOnEku</span></span>|[<span data-ttu-id="faaa9-232">extendedKeyUsage</span><span class="sxs-lookup"><span data-stu-id="faaa9-232">extendedKeyUsage</span></span>](../resources/intune-deviceconfig-extendedkeyusage.md)|<span data-ttu-id="faaa9-233">单一登录扩展密钥用法（EKU）。</span><span class="sxs-lookup"><span data-stu-id="faaa9-233">Single sign-on Extended Key Usage (EKU).</span></span>|
|<span data-ttu-id="faaa9-234">singleSignOnIssuerHash</span><span class="sxs-lookup"><span data-stu-id="faaa9-234">singleSignOnIssuerHash</span></span>|<span data-ttu-id="faaa9-235">String</span><span class="sxs-lookup"><span data-stu-id="faaa9-235">String</span></span>|<span data-ttu-id="faaa9-236">单一登录颁发者哈希。</span><span class="sxs-lookup"><span data-stu-id="faaa9-236">Single sign-on issuer hash.</span></span>|
|<span data-ttu-id="faaa9-237">eapXml</span><span class="sxs-lookup"><span data-stu-id="faaa9-237">eapXml</span></span>|<span data-ttu-id="faaa9-238">Binary</span><span class="sxs-lookup"><span data-stu-id="faaa9-238">Binary</span></span>|<span data-ttu-id="faaa9-239">可扩展的身份验证协议（EAP） XML。</span><span class="sxs-lookup"><span data-stu-id="faaa9-239">Extensible Authentication Protocol (EAP) XML.</span></span> <span data-ttu-id="faaa9-240">（UTF8 编码的字节数组）</span><span class="sxs-lookup"><span data-stu-id="faaa9-240">(UTF8 encoded byte array)</span></span>|
|<span data-ttu-id="faaa9-241">proxyServer</span><span class="sxs-lookup"><span data-stu-id="faaa9-241">proxyServer</span></span>|[<span data-ttu-id="faaa9-242">windows10VpnProxyServer</span><span class="sxs-lookup"><span data-stu-id="faaa9-242">windows10VpnProxyServer</span></span>](../resources/intune-deviceconfig-windows10vpnproxyserver.md)|<span data-ttu-id="faaa9-243">代理服务器。</span><span class="sxs-lookup"><span data-stu-id="faaa9-243">Proxy Server.</span></span>|
|<span data-ttu-id="faaa9-244">associatedApps</span><span class="sxs-lookup"><span data-stu-id="faaa9-244">associatedApps</span></span>|<span data-ttu-id="faaa9-245">[windows10AssociatedApps](../resources/intune-deviceconfig-windows10associatedapps.md)集合</span><span class="sxs-lookup"><span data-stu-id="faaa9-245">[windows10AssociatedApps](../resources/intune-deviceconfig-windows10associatedapps.md) collection</span></span>|<span data-ttu-id="faaa9-246">关联的应用。</span><span class="sxs-lookup"><span data-stu-id="faaa9-246">Associated Apps.</span></span> <span data-ttu-id="faaa9-247">该集合最多可包含 10000 个元素。</span><span class="sxs-lookup"><span data-stu-id="faaa9-247">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="faaa9-248">onlyAssociatedAppsCanUseConnection</span><span class="sxs-lookup"><span data-stu-id="faaa9-248">onlyAssociatedAppsCanUseConnection</span></span>|<span data-ttu-id="faaa9-249">布尔</span><span class="sxs-lookup"><span data-stu-id="faaa9-249">Boolean</span></span>|<span data-ttu-id="faaa9-250">仅关联的应用程序可以使用连接（每个应用 VPN）。</span><span class="sxs-lookup"><span data-stu-id="faaa9-250">Only associated Apps can use connection (per-app VPN).</span></span>|
|<span data-ttu-id="faaa9-251">windowsInformationProtectionDomain</span><span class="sxs-lookup"><span data-stu-id="faaa9-251">windowsInformationProtectionDomain</span></span>|<span data-ttu-id="faaa9-252">String</span><span class="sxs-lookup"><span data-stu-id="faaa9-252">String</span></span>|<span data-ttu-id="faaa9-253">与此连接关联的 Windows 信息保护（WIP）域。</span><span class="sxs-lookup"><span data-stu-id="faaa9-253">Windows Information Protection (WIP) domain to associate with this connection.</span></span>|
|<span data-ttu-id="faaa9-254">trafficRules</span><span class="sxs-lookup"><span data-stu-id="faaa9-254">trafficRules</span></span>|<span data-ttu-id="faaa9-255">[vpnTrafficRule](../resources/intune-deviceconfig-vpntrafficrule.md)集合</span><span class="sxs-lookup"><span data-stu-id="faaa9-255">[vpnTrafficRule](../resources/intune-deviceconfig-vpntrafficrule.md) collection</span></span>|<span data-ttu-id="faaa9-256">流量规则。</span><span class="sxs-lookup"><span data-stu-id="faaa9-256">Traffic rules.</span></span> <span data-ttu-id="faaa9-257">该集合最多可包含 1000 个元素。</span><span class="sxs-lookup"><span data-stu-id="faaa9-257">This collection can contain a maximum of 1000 elements.</span></span>|
|<span data-ttu-id="faaa9-258">航线</span><span class="sxs-lookup"><span data-stu-id="faaa9-258">routes</span></span>|<span data-ttu-id="faaa9-259">[vpnRoute](../resources/intune-deviceconfig-vpnroute.md)集合</span><span class="sxs-lookup"><span data-stu-id="faaa9-259">[vpnRoute](../resources/intune-deviceconfig-vpnroute.md) collection</span></span>|<span data-ttu-id="faaa9-260">路由（可选用于第三方提供程序）。</span><span class="sxs-lookup"><span data-stu-id="faaa9-260">Routes (optional for third-party providers).</span></span> <span data-ttu-id="faaa9-261">该集合最多可包含 1000 个元素。</span><span class="sxs-lookup"><span data-stu-id="faaa9-261">This collection can contain a maximum of 1000 elements.</span></span>|
|<span data-ttu-id="faaa9-262">dnsRules</span><span class="sxs-lookup"><span data-stu-id="faaa9-262">dnsRules</span></span>|<span data-ttu-id="faaa9-263">[vpnDnsRule](../resources/intune-deviceconfig-vpndnsrule.md)集合</span><span class="sxs-lookup"><span data-stu-id="faaa9-263">[vpnDnsRule](../resources/intune-deviceconfig-vpndnsrule.md) collection</span></span>|<span data-ttu-id="faaa9-264">DNS 规则。</span><span class="sxs-lookup"><span data-stu-id="faaa9-264">DNS rules.</span></span> <span data-ttu-id="faaa9-265">该集合最多可包含 1000 个元素。</span><span class="sxs-lookup"><span data-stu-id="faaa9-265">This collection can contain a maximum of 1000 elements.</span></span>|
|<span data-ttu-id="faaa9-266">trustedNetworkDomains</span><span class="sxs-lookup"><span data-stu-id="faaa9-266">trustedNetworkDomains</span></span>|<span data-ttu-id="faaa9-267">String 集合</span><span class="sxs-lookup"><span data-stu-id="faaa9-267">String collection</span></span>|<span data-ttu-id="faaa9-268">受信任的网络域</span><span class="sxs-lookup"><span data-stu-id="faaa9-268">Trusted Network Domains</span></span>|

## <a name="relationships"></a><span data-ttu-id="faaa9-269">关系</span><span class="sxs-lookup"><span data-stu-id="faaa9-269">Relationships</span></span>
|<span data-ttu-id="faaa9-270">关系</span><span class="sxs-lookup"><span data-stu-id="faaa9-270">Relationship</span></span>|<span data-ttu-id="faaa9-271">类型</span><span class="sxs-lookup"><span data-stu-id="faaa9-271">Type</span></span>|<span data-ttu-id="faaa9-272">说明</span><span class="sxs-lookup"><span data-stu-id="faaa9-272">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="faaa9-273">groupAssignments</span><span class="sxs-lookup"><span data-stu-id="faaa9-273">groupAssignments</span></span>|<span data-ttu-id="faaa9-274">[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)集合</span><span class="sxs-lookup"><span data-stu-id="faaa9-274">[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) collection</span></span>|<span data-ttu-id="faaa9-275">设备配置文件的组分配列表。</span><span class="sxs-lookup"><span data-stu-id="faaa9-275">The list of group assignments for the device configuration profile.</span></span> <span data-ttu-id="faaa9-276">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="faaa9-276">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="faaa9-277">assignments</span><span class="sxs-lookup"><span data-stu-id="faaa9-277">assignments</span></span>|<span data-ttu-id="faaa9-278">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="faaa9-278">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection</span></span>|<span data-ttu-id="faaa9-279">设备配置文件的分配列表。</span><span class="sxs-lookup"><span data-stu-id="faaa9-279">The list of assignments for the device configuration profile.</span></span> <span data-ttu-id="faaa9-280">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="faaa9-280">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="faaa9-281">deviceStatuses</span><span class="sxs-lookup"><span data-stu-id="faaa9-281">deviceStatuses</span></span>|<span data-ttu-id="faaa9-282">[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) 集合</span><span class="sxs-lookup"><span data-stu-id="faaa9-282">[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) collection</span></span>|<span data-ttu-id="faaa9-283">按设备的设备配置安装状态。</span><span class="sxs-lookup"><span data-stu-id="faaa9-283">Device configuration installation status by device.</span></span> <span data-ttu-id="faaa9-284">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="faaa9-284">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="faaa9-285">userStatuses</span><span class="sxs-lookup"><span data-stu-id="faaa9-285">userStatuses</span></span>|<span data-ttu-id="faaa9-286">[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) 集合</span><span class="sxs-lookup"><span data-stu-id="faaa9-286">[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) collection</span></span>|<span data-ttu-id="faaa9-287">按用户的设备配置安装状态。</span><span class="sxs-lookup"><span data-stu-id="faaa9-287">Device configuration installation status by user.</span></span> <span data-ttu-id="faaa9-288">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="faaa9-288">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="faaa9-289">deviceStatusOverview</span><span class="sxs-lookup"><span data-stu-id="faaa9-289">deviceStatusOverview</span></span>|[<span data-ttu-id="faaa9-290">deviceConfigurationDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="faaa9-290">deviceConfigurationDeviceOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|<span data-ttu-id="faaa9-291">设备配置设备状态概述 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="faaa9-291">Device Configuration devices status overview Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="faaa9-292">userStatusOverview</span><span class="sxs-lookup"><span data-stu-id="faaa9-292">userStatusOverview</span></span>|[<span data-ttu-id="faaa9-293">deviceConfigurationUserOverview</span><span class="sxs-lookup"><span data-stu-id="faaa9-293">deviceConfigurationUserOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|<span data-ttu-id="faaa9-294">设备配置用户状态概述 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="faaa9-294">Device Configuration users status overview Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="faaa9-295">deviceSettingStateSummaries</span><span class="sxs-lookup"><span data-stu-id="faaa9-295">deviceSettingStateSummaries</span></span>|<span data-ttu-id="faaa9-296">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) 集合</span><span class="sxs-lookup"><span data-stu-id="faaa9-296">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) collection</span></span>|<span data-ttu-id="faaa9-297">设备配置设置状态设备摘要 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="faaa9-297">Device Configuration Setting State Device Summary Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="faaa9-298">将 identitycertificate</span><span class="sxs-lookup"><span data-stu-id="faaa9-298">identityCertificate</span></span>|[<span data-ttu-id="faaa9-299">windowsCertificateProfileBase</span><span class="sxs-lookup"><span data-stu-id="faaa9-299">windowsCertificateProfileBase</span></span>](../resources/intune-deviceconfig-windowscertificateprofilebase.md)|<span data-ttu-id="faaa9-300">在身份验证方法为证书时，用于客户端身份验证的标识证书。</span><span class="sxs-lookup"><span data-stu-id="faaa9-300">Identity certificate for client authentication when authentication method is certificate.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="faaa9-301">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="faaa9-301">JSON Representation</span></span>
<span data-ttu-id="faaa9-302">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="faaa9-302">Here is a JSON representation of the resource.</span></span>
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
  ]
}
```



