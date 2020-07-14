---
title: windows10VpnConfiguration 资源类型
description: 通过提供此配置文件中的配置，可以指示 Windows 10 设备 (桌面或移动) 连接到所需的 VPN 终结点。 通过指定 VPN 终结点预期的身份验证方法和安全类型，可以为最终用户进行无缝的 VPN 连接。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: b51d85a894a07ab62f31ceab51bc222e42fa7b50
ms.sourcegitcommit: f3dda172d95ef1eda8f6dd9e3ffdc7d3c0744c0a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/14/2020
ms.locfileid: "45122509"
---
# <a name="windows10vpnconfiguration-resource-type"></a><span data-ttu-id="6bde5-104">windows10VpnConfiguration 资源类型</span><span class="sxs-lookup"><span data-stu-id="6bde5-104">windows10VpnConfiguration resource type</span></span>

<span data-ttu-id="6bde5-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6bde5-105">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6bde5-106">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="6bde5-106">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6bde5-107">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="6bde5-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6bde5-108">通过提供此配置文件中的配置，可以指示 Windows 10 设备 (桌面或移动) 连接到所需的 VPN 终结点。</span><span class="sxs-lookup"><span data-stu-id="6bde5-108">By providing the configurations in this profile you can instruct the Windows 10 device (desktop or mobile) to connect to desired VPN endpoint.</span></span> <span data-ttu-id="6bde5-109">通过指定 VPN 终结点预期的身份验证方法和安全类型，可以为最终用户进行无缝的 VPN 连接。</span><span class="sxs-lookup"><span data-stu-id="6bde5-109">By specifying the authentication method and security types expected by VPN endpoint you can make the VPN connection seamless for end user.</span></span>


<span data-ttu-id="6bde5-110">继承自[windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6bde5-110">Inherits from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>

## <a name="methods"></a><span data-ttu-id="6bde5-111">方法</span><span class="sxs-lookup"><span data-stu-id="6bde5-111">Methods</span></span>
|<span data-ttu-id="6bde5-112">方法</span><span class="sxs-lookup"><span data-stu-id="6bde5-112">Method</span></span>|<span data-ttu-id="6bde5-113">返回类型</span><span class="sxs-lookup"><span data-stu-id="6bde5-113">Return Type</span></span>|<span data-ttu-id="6bde5-114">说明</span><span class="sxs-lookup"><span data-stu-id="6bde5-114">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="6bde5-115">列出 windows10VpnConfigurations</span><span class="sxs-lookup"><span data-stu-id="6bde5-115">List windows10VpnConfigurations</span></span>](../api/intune-deviceconfig-windows10vpnconfiguration-list.md)|<span data-ttu-id="6bde5-116">[windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md)集合</span><span class="sxs-lookup"><span data-stu-id="6bde5-116">[windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) collection</span></span>|<span data-ttu-id="6bde5-117">列出[windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="6bde5-117">List properties and relationships of the [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="6bde5-118">获取 windows10VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="6bde5-118">Get windows10VpnConfiguration</span></span>](../api/intune-deviceconfig-windows10vpnconfiguration-get.md)|[<span data-ttu-id="6bde5-119">windows10VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="6bde5-119">windows10VpnConfiguration</span></span>](../resources/intune-deviceconfig-windows10vpnconfiguration.md)|<span data-ttu-id="6bde5-120">读取[windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="6bde5-120">Read properties and relationships of the [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) object.</span></span>|
|[<span data-ttu-id="6bde5-121">创建 windows10VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="6bde5-121">Create windows10VpnConfiguration</span></span>](../api/intune-deviceconfig-windows10vpnconfiguration-create.md)|[<span data-ttu-id="6bde5-122">windows10VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="6bde5-122">windows10VpnConfiguration</span></span>](../resources/intune-deviceconfig-windows10vpnconfiguration.md)|<span data-ttu-id="6bde5-123">创建新的[windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="6bde5-123">Create a new [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) object.</span></span>|
|[<span data-ttu-id="6bde5-124">删除 windows10VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="6bde5-124">Delete windows10VpnConfiguration</span></span>](../api/intune-deviceconfig-windows10vpnconfiguration-delete.md)|<span data-ttu-id="6bde5-125">无</span><span class="sxs-lookup"><span data-stu-id="6bde5-125">None</span></span>|<span data-ttu-id="6bde5-126">删除[windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md)。</span><span class="sxs-lookup"><span data-stu-id="6bde5-126">Deletes a [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md).</span></span>|
|[<span data-ttu-id="6bde5-127">更新 windows10VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="6bde5-127">Update windows10VpnConfiguration</span></span>](../api/intune-deviceconfig-windows10vpnconfiguration-update.md)|[<span data-ttu-id="6bde5-128">windows10VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="6bde5-128">windows10VpnConfiguration</span></span>](../resources/intune-deviceconfig-windows10vpnconfiguration.md)|<span data-ttu-id="6bde5-129">更新[windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="6bde5-129">Update the properties of a [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="6bde5-130">属性</span><span class="sxs-lookup"><span data-stu-id="6bde5-130">Properties</span></span>
|<span data-ttu-id="6bde5-131">属性</span><span class="sxs-lookup"><span data-stu-id="6bde5-131">Property</span></span>|<span data-ttu-id="6bde5-132">类型</span><span class="sxs-lookup"><span data-stu-id="6bde5-132">Type</span></span>|<span data-ttu-id="6bde5-133">说明</span><span class="sxs-lookup"><span data-stu-id="6bde5-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6bde5-134">id</span><span class="sxs-lookup"><span data-stu-id="6bde5-134">id</span></span>|<span data-ttu-id="6bde5-135">字符串</span><span class="sxs-lookup"><span data-stu-id="6bde5-135">String</span></span>|<span data-ttu-id="6bde5-136">实体的键。</span><span class="sxs-lookup"><span data-stu-id="6bde5-136">Key of the entity.</span></span> <span data-ttu-id="6bde5-137">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6bde5-137">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6bde5-138">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6bde5-138">lastModifiedDateTime</span></span>|<span data-ttu-id="6bde5-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6bde5-139">DateTimeOffset</span></span>|<span data-ttu-id="6bde5-140">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="6bde5-140">DateTime the object was last modified.</span></span> <span data-ttu-id="6bde5-141">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6bde5-141">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6bde5-142">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="6bde5-142">roleScopeTagIds</span></span>|<span data-ttu-id="6bde5-143">String collection</span><span class="sxs-lookup"><span data-stu-id="6bde5-143">String collection</span></span>|<span data-ttu-id="6bde5-144">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="6bde5-144">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="6bde5-145">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6bde5-145">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6bde5-146">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="6bde5-146">supportsScopeTags</span></span>|<span data-ttu-id="6bde5-147">Boolean</span><span class="sxs-lookup"><span data-stu-id="6bde5-147">Boolean</span></span>|<span data-ttu-id="6bde5-148">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="6bde5-148">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="6bde5-149">如果此值为 false，则不允许分配给 ScopeTags 属性，并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="6bde5-149">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="6bde5-150">这适用于在 Silverlight 中创建的旧版策略，可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="6bde5-150">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="6bde5-151">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="6bde5-151">This property is read-only.</span></span> <span data-ttu-id="6bde5-152">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6bde5-152">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6bde5-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="6bde5-153">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="6bde5-154">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="6bde5-154">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="6bde5-155">适用于此策略的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="6bde5-155">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="6bde5-156">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6bde5-156">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6bde5-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="6bde5-157">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="6bde5-158">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="6bde5-158">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="6bde5-159">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="6bde5-159">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="6bde5-160">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6bde5-160">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6bde5-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="6bde5-161">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="6bde5-162">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="6bde5-162">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="6bde5-163">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="6bde5-163">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="6bde5-164">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6bde5-164">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6bde5-165">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6bde5-165">createdDateTime</span></span>|<span data-ttu-id="6bde5-166">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6bde5-166">DateTimeOffset</span></span>|<span data-ttu-id="6bde5-167">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="6bde5-167">DateTime the object was created.</span></span> <span data-ttu-id="6bde5-168">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6bde5-168">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6bde5-169">说明</span><span class="sxs-lookup"><span data-stu-id="6bde5-169">description</span></span>|<span data-ttu-id="6bde5-170">String</span><span class="sxs-lookup"><span data-stu-id="6bde5-170">String</span></span>|<span data-ttu-id="6bde5-171">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="6bde5-171">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="6bde5-172">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6bde5-172">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6bde5-173">displayName</span><span class="sxs-lookup"><span data-stu-id="6bde5-173">displayName</span></span>|<span data-ttu-id="6bde5-174">String</span><span class="sxs-lookup"><span data-stu-id="6bde5-174">String</span></span>|<span data-ttu-id="6bde5-175">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="6bde5-175">Admin provided name of the device configuration.</span></span> <span data-ttu-id="6bde5-176">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6bde5-176">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6bde5-177">version</span><span class="sxs-lookup"><span data-stu-id="6bde5-177">version</span></span>|<span data-ttu-id="6bde5-178">Int32</span><span class="sxs-lookup"><span data-stu-id="6bde5-178">Int32</span></span>|<span data-ttu-id="6bde5-179">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="6bde5-179">Version of the device configuration.</span></span> <span data-ttu-id="6bde5-180">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6bde5-180">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6bde5-181">connectionName</span><span class="sxs-lookup"><span data-stu-id="6bde5-181">connectionName</span></span>|<span data-ttu-id="6bde5-182">String</span><span class="sxs-lookup"><span data-stu-id="6bde5-182">String</span></span>|<span data-ttu-id="6bde5-183">向用户显示的连接名称。</span><span class="sxs-lookup"><span data-stu-id="6bde5-183">Connection name displayed to the user.</span></span> <span data-ttu-id="6bde5-184">继承自[windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6bde5-184">Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="6bde5-185">台</span><span class="sxs-lookup"><span data-stu-id="6bde5-185">servers</span></span>|<span data-ttu-id="6bde5-186">[vpnServer](../resources/intune-deviceconfig-vpnserver.md)集合</span><span class="sxs-lookup"><span data-stu-id="6bde5-186">[vpnServer](../resources/intune-deviceconfig-vpnserver.md) collection</span></span>|<span data-ttu-id="6bde5-187">网络上的 VPN 服务器的列表。</span><span class="sxs-lookup"><span data-stu-id="6bde5-187">List of VPN Servers on the network.</span></span> <span data-ttu-id="6bde5-188">请确保最终用户可以访问这些网络位置。</span><span class="sxs-lookup"><span data-stu-id="6bde5-188">Make sure end users can access these network locations.</span></span> <span data-ttu-id="6bde5-189">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="6bde5-189">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="6bde5-190">继承自[windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6bde5-190">Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="6bde5-191">customXml</span><span class="sxs-lookup"><span data-stu-id="6bde5-191">customXml</span></span>|<span data-ttu-id="6bde5-192">Binary</span><span class="sxs-lookup"><span data-stu-id="6bde5-192">Binary</span></span>|<span data-ttu-id="6bde5-193">配置 VPN 连接的自定义 XML 命令。</span><span class="sxs-lookup"><span data-stu-id="6bde5-193">Custom XML commands that configures the VPN connection.</span></span> <span data-ttu-id="6bde5-194">从[WindowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)继承的 (UTF8 编码的字节数组) </span><span class="sxs-lookup"><span data-stu-id="6bde5-194">(UTF8 encoded byte array) Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="6bde5-195">profileTarget</span><span class="sxs-lookup"><span data-stu-id="6bde5-195">profileTarget</span></span>|[<span data-ttu-id="6bde5-196">windows10VpnProfileTarget</span><span class="sxs-lookup"><span data-stu-id="6bde5-196">windows10VpnProfileTarget</span></span>](../resources/intune-deviceconfig-windows10vpnprofiletarget.md)|<span data-ttu-id="6bde5-197">配置文件目标类型。</span><span class="sxs-lookup"><span data-stu-id="6bde5-197">Profile target type.</span></span> <span data-ttu-id="6bde5-198">可取值为：`user`、`device`、`autoPilotDevice`。</span><span class="sxs-lookup"><span data-stu-id="6bde5-198">Possible values are: `user`, `device`, `autoPilotDevice`.</span></span>|
|<span data-ttu-id="6bde5-199">connectionType</span><span class="sxs-lookup"><span data-stu-id="6bde5-199">connectionType</span></span>|[<span data-ttu-id="6bde5-200">windows10VpnConnectionType</span><span class="sxs-lookup"><span data-stu-id="6bde5-200">windows10VpnConnectionType</span></span>](../resources/intune-deviceconfig-windows10vpnconnectiontype.md)|<span data-ttu-id="6bde5-201">连接类型。</span><span class="sxs-lookup"><span data-stu-id="6bde5-201">Connection type.</span></span> <span data-ttu-id="6bde5-202">可取值为：`pulseSecure`、`f5EdgeClient`、`dellSonicWallMobileConnect`、`checkPointCapsuleVpn`、`automatic`、`ikEv2`、`l2tp`、`pptp`、`citrix`、`paloAltoGlobalProtect`。</span><span class="sxs-lookup"><span data-stu-id="6bde5-202">Possible values are: `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `automatic`, `ikEv2`, `l2tp`, `pptp`, `citrix`, `paloAltoGlobalProtect`.</span></span>|
|<span data-ttu-id="6bde5-203">enableSplitTunneling</span><span class="sxs-lookup"><span data-stu-id="6bde5-203">enableSplitTunneling</span></span>|<span data-ttu-id="6bde5-204">Boolean</span><span class="sxs-lookup"><span data-stu-id="6bde5-204">Boolean</span></span>|<span data-ttu-id="6bde5-205">启用拆分隧道。</span><span class="sxs-lookup"><span data-stu-id="6bde5-205">Enable split tunneling.</span></span>|
|<span data-ttu-id="6bde5-206">enableAlwaysOn</span><span class="sxs-lookup"><span data-stu-id="6bde5-206">enableAlwaysOn</span></span>|<span data-ttu-id="6bde5-207">Boolean</span><span class="sxs-lookup"><span data-stu-id="6bde5-207">Boolean</span></span>|<span data-ttu-id="6bde5-208">启用始终打开模式。</span><span class="sxs-lookup"><span data-stu-id="6bde5-208">Enable Always On mode.</span></span>|
|<span data-ttu-id="6bde5-209">enableDeviceTunnel</span><span class="sxs-lookup"><span data-stu-id="6bde5-209">enableDeviceTunnel</span></span>|<span data-ttu-id="6bde5-210">Boolean</span><span class="sxs-lookup"><span data-stu-id="6bde5-210">Boolean</span></span>|<span data-ttu-id="6bde5-211">启用设备隧道。</span><span class="sxs-lookup"><span data-stu-id="6bde5-211">Enable device tunnel.</span></span>|
|<span data-ttu-id="6bde5-212">enableDnsRegistration</span><span class="sxs-lookup"><span data-stu-id="6bde5-212">enableDnsRegistration</span></span>|<span data-ttu-id="6bde5-213">Boolean</span><span class="sxs-lookup"><span data-stu-id="6bde5-213">Boolean</span></span>|<span data-ttu-id="6bde5-214">使用内部 DNS 启用 IP 地址注册。</span><span class="sxs-lookup"><span data-stu-id="6bde5-214">Enable IP address registration with internal DNS.</span></span>|
|<span data-ttu-id="6bde5-215">dnsSuffixes</span><span class="sxs-lookup"><span data-stu-id="6bde5-215">dnsSuffixes</span></span>|<span data-ttu-id="6bde5-216">String collection</span><span class="sxs-lookup"><span data-stu-id="6bde5-216">String collection</span></span>|<span data-ttu-id="6bde5-217">指定要添加到 DNS 搜索列表以正确路由短名称的 DNS 后缀。</span><span class="sxs-lookup"><span data-stu-id="6bde5-217">Specify DNS suffixes to add to the DNS search list to properly route short names.</span></span>|
|<span data-ttu-id="6bde5-218">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="6bde5-218">authenticationMethod</span></span>|[<span data-ttu-id="6bde5-219">windows10VpnAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="6bde5-219">windows10VpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-windows10vpnauthenticationmethod.md)|<span data-ttu-id="6bde5-220">身份验证方法。</span><span class="sxs-lookup"><span data-stu-id="6bde5-220">Authentication method.</span></span> <span data-ttu-id="6bde5-221">可取值为：`certificate`、`usernameAndPassword`、`customEapXml`、`derivedCredential`。</span><span class="sxs-lookup"><span data-stu-id="6bde5-221">Possible values are: `certificate`, `usernameAndPassword`, `customEapXml`, `derivedCredential`.</span></span>|
|<span data-ttu-id="6bde5-222">rememberUserCredentials</span><span class="sxs-lookup"><span data-stu-id="6bde5-222">rememberUserCredentials</span></span>|<span data-ttu-id="6bde5-223">Boolean</span><span class="sxs-lookup"><span data-stu-id="6bde5-223">Boolean</span></span>|<span data-ttu-id="6bde5-224">记住用户凭据。</span><span class="sxs-lookup"><span data-stu-id="6bde5-224">Remember user credentials.</span></span>|
|<span data-ttu-id="6bde5-225">enableConditionalAccess</span><span class="sxs-lookup"><span data-stu-id="6bde5-225">enableConditionalAccess</span></span>|<span data-ttu-id="6bde5-226">Boolean</span><span class="sxs-lookup"><span data-stu-id="6bde5-226">Boolean</span></span>|<span data-ttu-id="6bde5-227">启用条件访问。</span><span class="sxs-lookup"><span data-stu-id="6bde5-227">Enable conditional access.</span></span>|
|<span data-ttu-id="6bde5-228">enableSingleSignOnWithAlternateCertificate</span><span class="sxs-lookup"><span data-stu-id="6bde5-228">enableSingleSignOnWithAlternateCertificate</span></span>|<span data-ttu-id="6bde5-229">Boolean</span><span class="sxs-lookup"><span data-stu-id="6bde5-229">Boolean</span></span>|<span data-ttu-id="6bde5-230">启用具有备用证书的单一登录 (SSO) 。</span><span class="sxs-lookup"><span data-stu-id="6bde5-230">Enable single sign-on (SSO) with alternate certificate.</span></span>|
|<span data-ttu-id="6bde5-231">singleSignOnEku</span><span class="sxs-lookup"><span data-stu-id="6bde5-231">singleSignOnEku</span></span>|[<span data-ttu-id="6bde5-232">extendedKeyUsage</span><span class="sxs-lookup"><span data-stu-id="6bde5-232">extendedKeyUsage</span></span>](../resources/intune-deviceconfig-extendedkeyusage.md)|<span data-ttu-id="6bde5-233">单一登录扩展密钥用法 (EKU) 。</span><span class="sxs-lookup"><span data-stu-id="6bde5-233">Single sign-on Extended Key Usage (EKU).</span></span>|
|<span data-ttu-id="6bde5-234">singleSignOnIssuerHash</span><span class="sxs-lookup"><span data-stu-id="6bde5-234">singleSignOnIssuerHash</span></span>|<span data-ttu-id="6bde5-235">String</span><span class="sxs-lookup"><span data-stu-id="6bde5-235">String</span></span>|<span data-ttu-id="6bde5-236">单一登录颁发者哈希。</span><span class="sxs-lookup"><span data-stu-id="6bde5-236">Single sign-on issuer hash.</span></span>|
|<span data-ttu-id="6bde5-237">eapXml</span><span class="sxs-lookup"><span data-stu-id="6bde5-237">eapXml</span></span>|<span data-ttu-id="6bde5-238">Binary</span><span class="sxs-lookup"><span data-stu-id="6bde5-238">Binary</span></span>|<span data-ttu-id="6bde5-239">可扩展的身份验证协议 (EAP) XML。</span><span class="sxs-lookup"><span data-stu-id="6bde5-239">Extensible Authentication Protocol (EAP) XML.</span></span> <span data-ttu-id="6bde5-240">（UTF8 编码的字节数组）</span><span class="sxs-lookup"><span data-stu-id="6bde5-240">(UTF8 encoded byte array)</span></span>|
|<span data-ttu-id="6bde5-241">proxyServer</span><span class="sxs-lookup"><span data-stu-id="6bde5-241">proxyServer</span></span>|[<span data-ttu-id="6bde5-242">windows10VpnProxyServer</span><span class="sxs-lookup"><span data-stu-id="6bde5-242">windows10VpnProxyServer</span></span>](../resources/intune-deviceconfig-windows10vpnproxyserver.md)|<span data-ttu-id="6bde5-243">代理服务器。</span><span class="sxs-lookup"><span data-stu-id="6bde5-243">Proxy Server.</span></span>|
|<span data-ttu-id="6bde5-244">associatedApps</span><span class="sxs-lookup"><span data-stu-id="6bde5-244">associatedApps</span></span>|<span data-ttu-id="6bde5-245">[windows10AssociatedApps](../resources/intune-deviceconfig-windows10associatedapps.md)集合</span><span class="sxs-lookup"><span data-stu-id="6bde5-245">[windows10AssociatedApps](../resources/intune-deviceconfig-windows10associatedapps.md) collection</span></span>|<span data-ttu-id="6bde5-246">关联的应用。</span><span class="sxs-lookup"><span data-stu-id="6bde5-246">Associated Apps.</span></span> <span data-ttu-id="6bde5-247">该集合最多可包含 10000 个元素。</span><span class="sxs-lookup"><span data-stu-id="6bde5-247">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="6bde5-248">onlyAssociatedAppsCanUseConnection</span><span class="sxs-lookup"><span data-stu-id="6bde5-248">onlyAssociatedAppsCanUseConnection</span></span>|<span data-ttu-id="6bde5-249">Boolean</span><span class="sxs-lookup"><span data-stu-id="6bde5-249">Boolean</span></span>|<span data-ttu-id="6bde5-250">仅关联的应用程序可以使用 (每应用 VPN) 的连接。</span><span class="sxs-lookup"><span data-stu-id="6bde5-250">Only associated Apps can use connection (per-app VPN).</span></span>|
|<span data-ttu-id="6bde5-251">windowsInformationProtectionDomain</span><span class="sxs-lookup"><span data-stu-id="6bde5-251">windowsInformationProtectionDomain</span></span>|<span data-ttu-id="6bde5-252">String</span><span class="sxs-lookup"><span data-stu-id="6bde5-252">String</span></span>|<span data-ttu-id="6bde5-253">与此连接关联的 Windows 信息保护 (与此连接关联的 WIP) 域。</span><span class="sxs-lookup"><span data-stu-id="6bde5-253">Windows Information Protection (WIP) domain to associate with this connection.</span></span>|
|<span data-ttu-id="6bde5-254">trafficRules</span><span class="sxs-lookup"><span data-stu-id="6bde5-254">trafficRules</span></span>|<span data-ttu-id="6bde5-255">[vpnTrafficRule](../resources/intune-deviceconfig-vpntrafficrule.md)集合</span><span class="sxs-lookup"><span data-stu-id="6bde5-255">[vpnTrafficRule](../resources/intune-deviceconfig-vpntrafficrule.md) collection</span></span>|<span data-ttu-id="6bde5-256">流量规则。</span><span class="sxs-lookup"><span data-stu-id="6bde5-256">Traffic rules.</span></span> <span data-ttu-id="6bde5-257">该集合最多可包含 1000 个元素。</span><span class="sxs-lookup"><span data-stu-id="6bde5-257">This collection can contain a maximum of 1000 elements.</span></span>|
|<span data-ttu-id="6bde5-258">航线</span><span class="sxs-lookup"><span data-stu-id="6bde5-258">routes</span></span>|<span data-ttu-id="6bde5-259">[vpnRoute](../resources/intune-deviceconfig-vpnroute.md)集合</span><span class="sxs-lookup"><span data-stu-id="6bde5-259">[vpnRoute](../resources/intune-deviceconfig-vpnroute.md) collection</span></span>|<span data-ttu-id="6bde5-260"> (第三方提供商) 的路由可选。</span><span class="sxs-lookup"><span data-stu-id="6bde5-260">Routes (optional for third-party providers).</span></span> <span data-ttu-id="6bde5-261">该集合最多可包含 1000 个元素。</span><span class="sxs-lookup"><span data-stu-id="6bde5-261">This collection can contain a maximum of 1000 elements.</span></span>|
|<span data-ttu-id="6bde5-262">dnsRules</span><span class="sxs-lookup"><span data-stu-id="6bde5-262">dnsRules</span></span>|<span data-ttu-id="6bde5-263">[vpnDnsRule](../resources/intune-deviceconfig-vpndnsrule.md)集合</span><span class="sxs-lookup"><span data-stu-id="6bde5-263">[vpnDnsRule](../resources/intune-deviceconfig-vpndnsrule.md) collection</span></span>|<span data-ttu-id="6bde5-264">DNS 规则。</span><span class="sxs-lookup"><span data-stu-id="6bde5-264">DNS rules.</span></span> <span data-ttu-id="6bde5-265">该集合最多可包含 1000 个元素。</span><span class="sxs-lookup"><span data-stu-id="6bde5-265">This collection can contain a maximum of 1000 elements.</span></span>|
|<span data-ttu-id="6bde5-266">trustedNetworkDomains</span><span class="sxs-lookup"><span data-stu-id="6bde5-266">trustedNetworkDomains</span></span>|<span data-ttu-id="6bde5-267">String collection</span><span class="sxs-lookup"><span data-stu-id="6bde5-267">String collection</span></span>|<span data-ttu-id="6bde5-268">受信任的网络域</span><span class="sxs-lookup"><span data-stu-id="6bde5-268">Trusted Network Domains</span></span>|
|<span data-ttu-id="6bde5-269">cryptographySuite</span><span class="sxs-lookup"><span data-stu-id="6bde5-269">cryptographySuite</span></span>|[<span data-ttu-id="6bde5-270">cryptographySuite</span><span class="sxs-lookup"><span data-stu-id="6bde5-270">cryptographySuite</span></span>](../resources/intune-deviceconfig-cryptographysuite.md)|<span data-ttu-id="6bde5-271">Windows10 及更高版本中 IKEv2 VPN 的加密套件安全设置</span><span class="sxs-lookup"><span data-stu-id="6bde5-271">Cryptography Suite security settings for IKEv2 VPN in Windows10 and above</span></span> |

## <a name="relationships"></a><span data-ttu-id="6bde5-272">关系</span><span class="sxs-lookup"><span data-stu-id="6bde5-272">Relationships</span></span>
|<span data-ttu-id="6bde5-273">关系</span><span class="sxs-lookup"><span data-stu-id="6bde5-273">Relationship</span></span>|<span data-ttu-id="6bde5-274">类型</span><span class="sxs-lookup"><span data-stu-id="6bde5-274">Type</span></span>|<span data-ttu-id="6bde5-275">说明</span><span class="sxs-lookup"><span data-stu-id="6bde5-275">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6bde5-276">groupAssignments</span><span class="sxs-lookup"><span data-stu-id="6bde5-276">groupAssignments</span></span>|<span data-ttu-id="6bde5-277">[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)集合</span><span class="sxs-lookup"><span data-stu-id="6bde5-277">[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) collection</span></span>|<span data-ttu-id="6bde5-278">设备配置文件的组分配列表。</span><span class="sxs-lookup"><span data-stu-id="6bde5-278">The list of group assignments for the device configuration profile.</span></span> <span data-ttu-id="6bde5-279">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6bde5-279">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6bde5-280">assignments</span><span class="sxs-lookup"><span data-stu-id="6bde5-280">assignments</span></span>|<span data-ttu-id="6bde5-281">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="6bde5-281">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection</span></span>|<span data-ttu-id="6bde5-282">设备配置文件的分配列表。</span><span class="sxs-lookup"><span data-stu-id="6bde5-282">The list of assignments for the device configuration profile.</span></span> <span data-ttu-id="6bde5-283">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6bde5-283">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6bde5-284">deviceStatuses</span><span class="sxs-lookup"><span data-stu-id="6bde5-284">deviceStatuses</span></span>|<span data-ttu-id="6bde5-285">[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) 集合</span><span class="sxs-lookup"><span data-stu-id="6bde5-285">[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) collection</span></span>|<span data-ttu-id="6bde5-286">按设备的设备配置安装状态。</span><span class="sxs-lookup"><span data-stu-id="6bde5-286">Device configuration installation status by device.</span></span> <span data-ttu-id="6bde5-287">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6bde5-287">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6bde5-288">userStatuses</span><span class="sxs-lookup"><span data-stu-id="6bde5-288">userStatuses</span></span>|<span data-ttu-id="6bde5-289">[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) 集合</span><span class="sxs-lookup"><span data-stu-id="6bde5-289">[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) collection</span></span>|<span data-ttu-id="6bde5-290">按用户的设备配置安装状态。</span><span class="sxs-lookup"><span data-stu-id="6bde5-290">Device configuration installation status by user.</span></span> <span data-ttu-id="6bde5-291">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6bde5-291">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6bde5-292">deviceStatusOverview</span><span class="sxs-lookup"><span data-stu-id="6bde5-292">deviceStatusOverview</span></span>|[<span data-ttu-id="6bde5-293">deviceConfigurationDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="6bde5-293">deviceConfigurationDeviceOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|<span data-ttu-id="6bde5-294">设备配置设备状态概述 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6bde5-294">Device Configuration devices status overview Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6bde5-295">userStatusOverview</span><span class="sxs-lookup"><span data-stu-id="6bde5-295">userStatusOverview</span></span>|[<span data-ttu-id="6bde5-296">deviceConfigurationUserOverview</span><span class="sxs-lookup"><span data-stu-id="6bde5-296">deviceConfigurationUserOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|<span data-ttu-id="6bde5-297">设备配置用户状态概述 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6bde5-297">Device Configuration users status overview Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6bde5-298">deviceSettingStateSummaries</span><span class="sxs-lookup"><span data-stu-id="6bde5-298">deviceSettingStateSummaries</span></span>|<span data-ttu-id="6bde5-299">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) 集合</span><span class="sxs-lookup"><span data-stu-id="6bde5-299">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) collection</span></span>|<span data-ttu-id="6bde5-300">设备配置设置状态设备摘要 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6bde5-300">Device Configuration Setting State Device Summary Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6bde5-301">将 identitycertificate</span><span class="sxs-lookup"><span data-stu-id="6bde5-301">identityCertificate</span></span>|[<span data-ttu-id="6bde5-302">windowsCertificateProfileBase</span><span class="sxs-lookup"><span data-stu-id="6bde5-302">windowsCertificateProfileBase</span></span>](../resources/intune-deviceconfig-windowscertificateprofilebase.md)|<span data-ttu-id="6bde5-303">在身份验证方法为证书时，用于客户端身份验证的标识证书。</span><span class="sxs-lookup"><span data-stu-id="6bde5-303">Identity certificate for client authentication when authentication method is certificate.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="6bde5-304">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6bde5-304">JSON Representation</span></span>
<span data-ttu-id="6bde5-305">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6bde5-305">Here is a JSON representation of the resource.</span></span>
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



