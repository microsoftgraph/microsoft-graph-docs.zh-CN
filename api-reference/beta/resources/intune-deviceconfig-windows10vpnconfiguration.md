---
title: windows10VpnConfiguration 资源类型
description: 通过提供此配置文件中的配置，可以指示 Windows 10 设备（桌面或移动版）连接到所需的 VPN 终结点。 通过指定 VPN 终结点预期的身份验证方法和安全类型，可以为最终用户进行无缝的 VPN 连接。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: e534767fc61ae1f8de3634c7d1655b46c2def993
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/26/2019
ms.locfileid: "37197328"
---
# <a name="windows10vpnconfiguration-resource-type"></a><span data-ttu-id="6fc2f-104">windows10VpnConfiguration 资源类型</span><span class="sxs-lookup"><span data-stu-id="6fc2f-104">windows10VpnConfiguration resource type</span></span>

> <span data-ttu-id="6fc2f-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="6fc2f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6fc2f-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="6fc2f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6fc2f-107">通过提供此配置文件中的配置，可以指示 Windows 10 设备（桌面或移动版）连接到所需的 VPN 终结点。</span><span class="sxs-lookup"><span data-stu-id="6fc2f-107">By providing the configurations in this profile you can instruct the Windows 10 device (desktop or mobile) to connect to desired VPN endpoint.</span></span> <span data-ttu-id="6fc2f-108">通过指定 VPN 终结点预期的身份验证方法和安全类型，可以为最终用户进行无缝的 VPN 连接。</span><span class="sxs-lookup"><span data-stu-id="6fc2f-108">By specifying the authentication method and security types expected by VPN endpoint you can make the VPN connection seamless for end user.</span></span>


<span data-ttu-id="6fc2f-109">继承自[windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6fc2f-109">Inherits from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>

## <a name="methods"></a><span data-ttu-id="6fc2f-110">方法</span><span class="sxs-lookup"><span data-stu-id="6fc2f-110">Methods</span></span>
|<span data-ttu-id="6fc2f-111">方法</span><span class="sxs-lookup"><span data-stu-id="6fc2f-111">Method</span></span>|<span data-ttu-id="6fc2f-112">返回类型</span><span class="sxs-lookup"><span data-stu-id="6fc2f-112">Return Type</span></span>|<span data-ttu-id="6fc2f-113">说明</span><span class="sxs-lookup"><span data-stu-id="6fc2f-113">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="6fc2f-114">列出 windows10VpnConfigurations</span><span class="sxs-lookup"><span data-stu-id="6fc2f-114">List windows10VpnConfigurations</span></span>](../api/intune-deviceconfig-windows10vpnconfiguration-list.md)|<span data-ttu-id="6fc2f-115">[windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md)集合</span><span class="sxs-lookup"><span data-stu-id="6fc2f-115">[windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) collection</span></span>|<span data-ttu-id="6fc2f-116">列出[windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="6fc2f-116">List properties and relationships of the [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="6fc2f-117">获取 windows10VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="6fc2f-117">Get windows10VpnConfiguration</span></span>](../api/intune-deviceconfig-windows10vpnconfiguration-get.md)|[<span data-ttu-id="6fc2f-118">windows10VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="6fc2f-118">windows10VpnConfiguration</span></span>](../resources/intune-deviceconfig-windows10vpnconfiguration.md)|<span data-ttu-id="6fc2f-119">读取[windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="6fc2f-119">Read properties and relationships of the [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) object.</span></span>|
|[<span data-ttu-id="6fc2f-120">创建 windows10VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="6fc2f-120">Create windows10VpnConfiguration</span></span>](../api/intune-deviceconfig-windows10vpnconfiguration-create.md)|[<span data-ttu-id="6fc2f-121">windows10VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="6fc2f-121">windows10VpnConfiguration</span></span>](../resources/intune-deviceconfig-windows10vpnconfiguration.md)|<span data-ttu-id="6fc2f-122">创建新的[windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="6fc2f-122">Create a new [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) object.</span></span>|
|[<span data-ttu-id="6fc2f-123">删除 windows10VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="6fc2f-123">Delete windows10VpnConfiguration</span></span>](../api/intune-deviceconfig-windows10vpnconfiguration-delete.md)|<span data-ttu-id="6fc2f-124">无</span><span class="sxs-lookup"><span data-stu-id="6fc2f-124">None</span></span>|<span data-ttu-id="6fc2f-125">删除[windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md)。</span><span class="sxs-lookup"><span data-stu-id="6fc2f-125">Deletes a [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md).</span></span>|
|[<span data-ttu-id="6fc2f-126">更新 windows10VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="6fc2f-126">Update windows10VpnConfiguration</span></span>](../api/intune-deviceconfig-windows10vpnconfiguration-update.md)|[<span data-ttu-id="6fc2f-127">windows10VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="6fc2f-127">windows10VpnConfiguration</span></span>](../resources/intune-deviceconfig-windows10vpnconfiguration.md)|<span data-ttu-id="6fc2f-128">更新[windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="6fc2f-128">Update the properties of a [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="6fc2f-129">属性</span><span class="sxs-lookup"><span data-stu-id="6fc2f-129">Properties</span></span>
|<span data-ttu-id="6fc2f-130">属性</span><span class="sxs-lookup"><span data-stu-id="6fc2f-130">Property</span></span>|<span data-ttu-id="6fc2f-131">类型</span><span class="sxs-lookup"><span data-stu-id="6fc2f-131">Type</span></span>|<span data-ttu-id="6fc2f-132">说明</span><span class="sxs-lookup"><span data-stu-id="6fc2f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6fc2f-133">id</span><span class="sxs-lookup"><span data-stu-id="6fc2f-133">id</span></span>|<span data-ttu-id="6fc2f-134">字符串</span><span class="sxs-lookup"><span data-stu-id="6fc2f-134">String</span></span>|<span data-ttu-id="6fc2f-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="6fc2f-135">Key of the entity.</span></span> <span data-ttu-id="6fc2f-136">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6fc2f-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6fc2f-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6fc2f-137">lastModifiedDateTime</span></span>|<span data-ttu-id="6fc2f-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6fc2f-138">DateTimeOffset</span></span>|<span data-ttu-id="6fc2f-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="6fc2f-139">DateTime the object was last modified.</span></span> <span data-ttu-id="6fc2f-140">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6fc2f-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6fc2f-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="6fc2f-141">roleScopeTagIds</span></span>|<span data-ttu-id="6fc2f-142">String collection</span><span class="sxs-lookup"><span data-stu-id="6fc2f-142">String collection</span></span>|<span data-ttu-id="6fc2f-143">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="6fc2f-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="6fc2f-144">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6fc2f-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6fc2f-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="6fc2f-145">supportsScopeTags</span></span>|<span data-ttu-id="6fc2f-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="6fc2f-146">Boolean</span></span>|<span data-ttu-id="6fc2f-147">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="6fc2f-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="6fc2f-148">如果此值为 false，则不允许分配给 ScopeTags 属性，并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="6fc2f-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="6fc2f-149">这适用于在 Silverlight 中创建的旧版策略，可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="6fc2f-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="6fc2f-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="6fc2f-150">This property is read-only.</span></span> <span data-ttu-id="6fc2f-151">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6fc2f-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6fc2f-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="6fc2f-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="6fc2f-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="6fc2f-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="6fc2f-154">适用于此策略的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="6fc2f-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="6fc2f-155">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6fc2f-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6fc2f-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="6fc2f-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="6fc2f-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="6fc2f-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="6fc2f-158">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="6fc2f-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="6fc2f-159">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6fc2f-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6fc2f-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="6fc2f-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="6fc2f-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="6fc2f-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="6fc2f-162">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="6fc2f-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="6fc2f-163">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6fc2f-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6fc2f-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6fc2f-164">createdDateTime</span></span>|<span data-ttu-id="6fc2f-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6fc2f-165">DateTimeOffset</span></span>|<span data-ttu-id="6fc2f-166">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="6fc2f-166">DateTime the object was created.</span></span> <span data-ttu-id="6fc2f-167">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6fc2f-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6fc2f-168">说明</span><span class="sxs-lookup"><span data-stu-id="6fc2f-168">description</span></span>|<span data-ttu-id="6fc2f-169">String</span><span class="sxs-lookup"><span data-stu-id="6fc2f-169">String</span></span>|<span data-ttu-id="6fc2f-170">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="6fc2f-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="6fc2f-171">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6fc2f-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6fc2f-172">displayName</span><span class="sxs-lookup"><span data-stu-id="6fc2f-172">displayName</span></span>|<span data-ttu-id="6fc2f-173">String</span><span class="sxs-lookup"><span data-stu-id="6fc2f-173">String</span></span>|<span data-ttu-id="6fc2f-174">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="6fc2f-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="6fc2f-175">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6fc2f-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6fc2f-176">version</span><span class="sxs-lookup"><span data-stu-id="6fc2f-176">version</span></span>|<span data-ttu-id="6fc2f-177">Int32</span><span class="sxs-lookup"><span data-stu-id="6fc2f-177">Int32</span></span>|<span data-ttu-id="6fc2f-178">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="6fc2f-178">Version of the device configuration.</span></span> <span data-ttu-id="6fc2f-179">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6fc2f-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6fc2f-180">connectionName</span><span class="sxs-lookup"><span data-stu-id="6fc2f-180">connectionName</span></span>|<span data-ttu-id="6fc2f-181">String</span><span class="sxs-lookup"><span data-stu-id="6fc2f-181">String</span></span>|<span data-ttu-id="6fc2f-182">向用户显示的连接名称。</span><span class="sxs-lookup"><span data-stu-id="6fc2f-182">Connection name displayed to the user.</span></span> <span data-ttu-id="6fc2f-183">继承自[windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6fc2f-183">Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="6fc2f-184">台</span><span class="sxs-lookup"><span data-stu-id="6fc2f-184">servers</span></span>|<span data-ttu-id="6fc2f-185">[vpnServer](../resources/intune-deviceconfig-vpnserver.md)集合</span><span class="sxs-lookup"><span data-stu-id="6fc2f-185">[vpnServer](../resources/intune-deviceconfig-vpnserver.md) collection</span></span>|<span data-ttu-id="6fc2f-186">网络上的 VPN 服务器的列表。</span><span class="sxs-lookup"><span data-stu-id="6fc2f-186">List of VPN Servers on the network.</span></span> <span data-ttu-id="6fc2f-187">请确保最终用户可以访问这些网络位置。</span><span class="sxs-lookup"><span data-stu-id="6fc2f-187">Make sure end users can access these network locations.</span></span> <span data-ttu-id="6fc2f-188">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="6fc2f-188">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="6fc2f-189">继承自[windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6fc2f-189">Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="6fc2f-190">customXml</span><span class="sxs-lookup"><span data-stu-id="6fc2f-190">customXml</span></span>|<span data-ttu-id="6fc2f-191">Binary</span><span class="sxs-lookup"><span data-stu-id="6fc2f-191">Binary</span></span>|<span data-ttu-id="6fc2f-192">配置 VPN 连接的自定义 XML 命令。</span><span class="sxs-lookup"><span data-stu-id="6fc2f-192">Custom XML commands that configures the VPN connection.</span></span> <span data-ttu-id="6fc2f-193">（UTF8 编码的字节数组）继承自[windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6fc2f-193">(UTF8 encoded byte array) Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="6fc2f-194">profileTarget</span><span class="sxs-lookup"><span data-stu-id="6fc2f-194">profileTarget</span></span>|[<span data-ttu-id="6fc2f-195">windows10VpnProfileTarget</span><span class="sxs-lookup"><span data-stu-id="6fc2f-195">windows10VpnProfileTarget</span></span>](../resources/intune-deviceconfig-windows10vpnprofiletarget.md)|<span data-ttu-id="6fc2f-196">配置文件目标类型。</span><span class="sxs-lookup"><span data-stu-id="6fc2f-196">Profile target type.</span></span> <span data-ttu-id="6fc2f-197">可取值为：`user`、`device`、`autoPilotDevice`。</span><span class="sxs-lookup"><span data-stu-id="6fc2f-197">Possible values are: `user`, `device`, `autoPilotDevice`.</span></span>|
|<span data-ttu-id="6fc2f-198">connectionType</span><span class="sxs-lookup"><span data-stu-id="6fc2f-198">connectionType</span></span>|[<span data-ttu-id="6fc2f-199">windows10VpnConnectionType</span><span class="sxs-lookup"><span data-stu-id="6fc2f-199">windows10VpnConnectionType</span></span>](../resources/intune-deviceconfig-windows10vpnconnectiontype.md)|<span data-ttu-id="6fc2f-200">连接类型。</span><span class="sxs-lookup"><span data-stu-id="6fc2f-200">Connection type.</span></span> <span data-ttu-id="6fc2f-201">可取值为：`pulseSecure`、`f5EdgeClient`、`dellSonicWallMobileConnect`、`checkPointCapsuleVpn`、`automatic`、`ikEv2`、`l2tp`、`pptp`、`citrix`、`paloAltoGlobalProtect`。</span><span class="sxs-lookup"><span data-stu-id="6fc2f-201">Possible values are: `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `automatic`, `ikEv2`, `l2tp`, `pptp`, `citrix`, `paloAltoGlobalProtect`.</span></span>|
|<span data-ttu-id="6fc2f-202">enableSplitTunneling</span><span class="sxs-lookup"><span data-stu-id="6fc2f-202">enableSplitTunneling</span></span>|<span data-ttu-id="6fc2f-203">Boolean</span><span class="sxs-lookup"><span data-stu-id="6fc2f-203">Boolean</span></span>|<span data-ttu-id="6fc2f-204">启用拆分隧道。</span><span class="sxs-lookup"><span data-stu-id="6fc2f-204">Enable split tunneling.</span></span>|
|<span data-ttu-id="6fc2f-205">enableAlwaysOn</span><span class="sxs-lookup"><span data-stu-id="6fc2f-205">enableAlwaysOn</span></span>|<span data-ttu-id="6fc2f-206">Boolean</span><span class="sxs-lookup"><span data-stu-id="6fc2f-206">Boolean</span></span>|<span data-ttu-id="6fc2f-207">启用始终打开模式。</span><span class="sxs-lookup"><span data-stu-id="6fc2f-207">Enable Always On mode.</span></span>|
|<span data-ttu-id="6fc2f-208">enableDeviceTunnel</span><span class="sxs-lookup"><span data-stu-id="6fc2f-208">enableDeviceTunnel</span></span>|<span data-ttu-id="6fc2f-209">Boolean</span><span class="sxs-lookup"><span data-stu-id="6fc2f-209">Boolean</span></span>|<span data-ttu-id="6fc2f-210">启用设备隧道。</span><span class="sxs-lookup"><span data-stu-id="6fc2f-210">Enable device tunnel.</span></span>|
|<span data-ttu-id="6fc2f-211">enableDnsRegistration</span><span class="sxs-lookup"><span data-stu-id="6fc2f-211">enableDnsRegistration</span></span>|<span data-ttu-id="6fc2f-212">Boolean</span><span class="sxs-lookup"><span data-stu-id="6fc2f-212">Boolean</span></span>|<span data-ttu-id="6fc2f-213">使用内部 DNS 启用 IP 地址注册。</span><span class="sxs-lookup"><span data-stu-id="6fc2f-213">Enable IP address registration with internal DNS.</span></span>|
|<span data-ttu-id="6fc2f-214">dnsSuffixes</span><span class="sxs-lookup"><span data-stu-id="6fc2f-214">dnsSuffixes</span></span>|<span data-ttu-id="6fc2f-215">String collection</span><span class="sxs-lookup"><span data-stu-id="6fc2f-215">String collection</span></span>|<span data-ttu-id="6fc2f-216">指定要添加到 DNS 搜索列表以正确路由短名称的 DNS 后缀。</span><span class="sxs-lookup"><span data-stu-id="6fc2f-216">Specify DNS suffixes to add to the DNS search list to properly route short names.</span></span>|
|<span data-ttu-id="6fc2f-217">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="6fc2f-217">authenticationMethod</span></span>|[<span data-ttu-id="6fc2f-218">windows10VpnAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="6fc2f-218">windows10VpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-windows10vpnauthenticationmethod.md)|<span data-ttu-id="6fc2f-219">身份验证方法。</span><span class="sxs-lookup"><span data-stu-id="6fc2f-219">Authentication method.</span></span> <span data-ttu-id="6fc2f-220">可取值为：`certificate`、`usernameAndPassword`、`customEapXml`。</span><span class="sxs-lookup"><span data-stu-id="6fc2f-220">Possible values are: `certificate`, `usernameAndPassword`, `customEapXml`.</span></span>|
|<span data-ttu-id="6fc2f-221">rememberUserCredentials</span><span class="sxs-lookup"><span data-stu-id="6fc2f-221">rememberUserCredentials</span></span>|<span data-ttu-id="6fc2f-222">Boolean</span><span class="sxs-lookup"><span data-stu-id="6fc2f-222">Boolean</span></span>|<span data-ttu-id="6fc2f-223">记住用户凭据。</span><span class="sxs-lookup"><span data-stu-id="6fc2f-223">Remember user credentials.</span></span>|
|<span data-ttu-id="6fc2f-224">enableConditionalAccess</span><span class="sxs-lookup"><span data-stu-id="6fc2f-224">enableConditionalAccess</span></span>|<span data-ttu-id="6fc2f-225">Boolean</span><span class="sxs-lookup"><span data-stu-id="6fc2f-225">Boolean</span></span>|<span data-ttu-id="6fc2f-226">启用条件访问。</span><span class="sxs-lookup"><span data-stu-id="6fc2f-226">Enable conditional access.</span></span>|
|<span data-ttu-id="6fc2f-227">enableSingleSignOnWithAlternateCertificate</span><span class="sxs-lookup"><span data-stu-id="6fc2f-227">enableSingleSignOnWithAlternateCertificate</span></span>|<span data-ttu-id="6fc2f-228">Boolean</span><span class="sxs-lookup"><span data-stu-id="6fc2f-228">Boolean</span></span>|<span data-ttu-id="6fc2f-229">启用具有备用证书的单一登录（SSO）。</span><span class="sxs-lookup"><span data-stu-id="6fc2f-229">Enable single sign-on (SSO) with alternate certificate.</span></span>|
|<span data-ttu-id="6fc2f-230">singleSignOnEku</span><span class="sxs-lookup"><span data-stu-id="6fc2f-230">singleSignOnEku</span></span>|[<span data-ttu-id="6fc2f-231">extendedKeyUsage</span><span class="sxs-lookup"><span data-stu-id="6fc2f-231">extendedKeyUsage</span></span>](../resources/intune-deviceconfig-extendedkeyusage.md)|<span data-ttu-id="6fc2f-232">单一登录扩展密钥用法（EKU）。</span><span class="sxs-lookup"><span data-stu-id="6fc2f-232">Single sign-on Extended Key Usage (EKU).</span></span>|
|<span data-ttu-id="6fc2f-233">singleSignOnIssuerHash</span><span class="sxs-lookup"><span data-stu-id="6fc2f-233">singleSignOnIssuerHash</span></span>|<span data-ttu-id="6fc2f-234">String</span><span class="sxs-lookup"><span data-stu-id="6fc2f-234">String</span></span>|<span data-ttu-id="6fc2f-235">单一登录颁发者哈希。</span><span class="sxs-lookup"><span data-stu-id="6fc2f-235">Single sign-on issuer hash.</span></span>|
|<span data-ttu-id="6fc2f-236">eapXml</span><span class="sxs-lookup"><span data-stu-id="6fc2f-236">eapXml</span></span>|<span data-ttu-id="6fc2f-237">Binary</span><span class="sxs-lookup"><span data-stu-id="6fc2f-237">Binary</span></span>|<span data-ttu-id="6fc2f-238">可扩展的身份验证协议（EAP） XML。</span><span class="sxs-lookup"><span data-stu-id="6fc2f-238">Extensible Authentication Protocol (EAP) XML.</span></span> <span data-ttu-id="6fc2f-239">（UTF8 编码的字节数组）</span><span class="sxs-lookup"><span data-stu-id="6fc2f-239">(UTF8 encoded byte array)</span></span>|
|<span data-ttu-id="6fc2f-240">proxyServer</span><span class="sxs-lookup"><span data-stu-id="6fc2f-240">proxyServer</span></span>|[<span data-ttu-id="6fc2f-241">windows10VpnProxyServer</span><span class="sxs-lookup"><span data-stu-id="6fc2f-241">windows10VpnProxyServer</span></span>](../resources/intune-deviceconfig-windows10vpnproxyserver.md)|<span data-ttu-id="6fc2f-242">代理服务器。</span><span class="sxs-lookup"><span data-stu-id="6fc2f-242">Proxy Server.</span></span>|
|<span data-ttu-id="6fc2f-243">associatedApps</span><span class="sxs-lookup"><span data-stu-id="6fc2f-243">associatedApps</span></span>|<span data-ttu-id="6fc2f-244">[windows10AssociatedApps](../resources/intune-deviceconfig-windows10associatedapps.md)集合</span><span class="sxs-lookup"><span data-stu-id="6fc2f-244">[windows10AssociatedApps](../resources/intune-deviceconfig-windows10associatedapps.md) collection</span></span>|<span data-ttu-id="6fc2f-245">关联的应用。</span><span class="sxs-lookup"><span data-stu-id="6fc2f-245">Associated Apps.</span></span> <span data-ttu-id="6fc2f-246">该集合最多可包含 10000 个元素。</span><span class="sxs-lookup"><span data-stu-id="6fc2f-246">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="6fc2f-247">onlyAssociatedAppsCanUseConnection</span><span class="sxs-lookup"><span data-stu-id="6fc2f-247">onlyAssociatedAppsCanUseConnection</span></span>|<span data-ttu-id="6fc2f-248">Boolean</span><span class="sxs-lookup"><span data-stu-id="6fc2f-248">Boolean</span></span>|<span data-ttu-id="6fc2f-249">仅关联的应用程序可以使用连接（每个应用 VPN）。</span><span class="sxs-lookup"><span data-stu-id="6fc2f-249">Only associated Apps can use connection (per-app VPN).</span></span>|
|<span data-ttu-id="6fc2f-250">windowsInformationProtectionDomain</span><span class="sxs-lookup"><span data-stu-id="6fc2f-250">windowsInformationProtectionDomain</span></span>|<span data-ttu-id="6fc2f-251">String</span><span class="sxs-lookup"><span data-stu-id="6fc2f-251">String</span></span>|<span data-ttu-id="6fc2f-252">与此连接关联的 Windows 信息保护（WIP）域。</span><span class="sxs-lookup"><span data-stu-id="6fc2f-252">Windows Information Protection (WIP) domain to associate with this connection.</span></span>|
|<span data-ttu-id="6fc2f-253">trafficRules</span><span class="sxs-lookup"><span data-stu-id="6fc2f-253">trafficRules</span></span>|<span data-ttu-id="6fc2f-254">[vpnTrafficRule](../resources/intune-deviceconfig-vpntrafficrule.md)集合</span><span class="sxs-lookup"><span data-stu-id="6fc2f-254">[vpnTrafficRule](../resources/intune-deviceconfig-vpntrafficrule.md) collection</span></span>|<span data-ttu-id="6fc2f-255">流量规则。</span><span class="sxs-lookup"><span data-stu-id="6fc2f-255">Traffic rules.</span></span> <span data-ttu-id="6fc2f-256">该集合最多可包含 1000 个元素。</span><span class="sxs-lookup"><span data-stu-id="6fc2f-256">This collection can contain a maximum of 1000 elements.</span></span>|
|<span data-ttu-id="6fc2f-257">航线</span><span class="sxs-lookup"><span data-stu-id="6fc2f-257">routes</span></span>|<span data-ttu-id="6fc2f-258">[vpnRoute](../resources/intune-deviceconfig-vpnroute.md)集合</span><span class="sxs-lookup"><span data-stu-id="6fc2f-258">[vpnRoute](../resources/intune-deviceconfig-vpnroute.md) collection</span></span>|<span data-ttu-id="6fc2f-259">路由（可选用于第三方提供程序）。</span><span class="sxs-lookup"><span data-stu-id="6fc2f-259">Routes (optional for third-party providers).</span></span> <span data-ttu-id="6fc2f-260">该集合最多可包含 1000 个元素。</span><span class="sxs-lookup"><span data-stu-id="6fc2f-260">This collection can contain a maximum of 1000 elements.</span></span>|
|<span data-ttu-id="6fc2f-261">dnsRules</span><span class="sxs-lookup"><span data-stu-id="6fc2f-261">dnsRules</span></span>|<span data-ttu-id="6fc2f-262">[vpnDnsRule](../resources/intune-deviceconfig-vpndnsrule.md)集合</span><span class="sxs-lookup"><span data-stu-id="6fc2f-262">[vpnDnsRule](../resources/intune-deviceconfig-vpndnsrule.md) collection</span></span>|<span data-ttu-id="6fc2f-263">DNS 规则。</span><span class="sxs-lookup"><span data-stu-id="6fc2f-263">DNS rules.</span></span> <span data-ttu-id="6fc2f-264">该集合最多可包含 1000 个元素。</span><span class="sxs-lookup"><span data-stu-id="6fc2f-264">This collection can contain a maximum of 1000 elements.</span></span>|
|<span data-ttu-id="6fc2f-265">trustedNetworkDomains</span><span class="sxs-lookup"><span data-stu-id="6fc2f-265">trustedNetworkDomains</span></span>|<span data-ttu-id="6fc2f-266">String collection</span><span class="sxs-lookup"><span data-stu-id="6fc2f-266">String collection</span></span>|<span data-ttu-id="6fc2f-267">受信任的网络域</span><span class="sxs-lookup"><span data-stu-id="6fc2f-267">Trusted Network Domains</span></span>|

## <a name="relationships"></a><span data-ttu-id="6fc2f-268">关系</span><span class="sxs-lookup"><span data-stu-id="6fc2f-268">Relationships</span></span>
|<span data-ttu-id="6fc2f-269">关系</span><span class="sxs-lookup"><span data-stu-id="6fc2f-269">Relationship</span></span>|<span data-ttu-id="6fc2f-270">类型</span><span class="sxs-lookup"><span data-stu-id="6fc2f-270">Type</span></span>|<span data-ttu-id="6fc2f-271">说明</span><span class="sxs-lookup"><span data-stu-id="6fc2f-271">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6fc2f-272">groupAssignments</span><span class="sxs-lookup"><span data-stu-id="6fc2f-272">groupAssignments</span></span>|<span data-ttu-id="6fc2f-273">[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)集合</span><span class="sxs-lookup"><span data-stu-id="6fc2f-273">[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) collection</span></span>|<span data-ttu-id="6fc2f-274">设备配置文件的组分配列表。</span><span class="sxs-lookup"><span data-stu-id="6fc2f-274">The list of group assignments for the device configuration profile.</span></span> <span data-ttu-id="6fc2f-275">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6fc2f-275">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6fc2f-276">assignments</span><span class="sxs-lookup"><span data-stu-id="6fc2f-276">assignments</span></span>|<span data-ttu-id="6fc2f-277">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="6fc2f-277">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection</span></span>|<span data-ttu-id="6fc2f-278">设备配置文件的分配列表。</span><span class="sxs-lookup"><span data-stu-id="6fc2f-278">The list of assignments for the device configuration profile.</span></span> <span data-ttu-id="6fc2f-279">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6fc2f-279">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6fc2f-280">deviceStatuses</span><span class="sxs-lookup"><span data-stu-id="6fc2f-280">deviceStatuses</span></span>|<span data-ttu-id="6fc2f-281">[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) 集合</span><span class="sxs-lookup"><span data-stu-id="6fc2f-281">[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) collection</span></span>|<span data-ttu-id="6fc2f-282">按设备的设备配置安装状态。</span><span class="sxs-lookup"><span data-stu-id="6fc2f-282">Device configuration installation status by device.</span></span> <span data-ttu-id="6fc2f-283">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6fc2f-283">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6fc2f-284">userStatuses</span><span class="sxs-lookup"><span data-stu-id="6fc2f-284">userStatuses</span></span>|<span data-ttu-id="6fc2f-285">[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) 集合</span><span class="sxs-lookup"><span data-stu-id="6fc2f-285">[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) collection</span></span>|<span data-ttu-id="6fc2f-286">按用户的设备配置安装状态。</span><span class="sxs-lookup"><span data-stu-id="6fc2f-286">Device configuration installation status by user.</span></span> <span data-ttu-id="6fc2f-287">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6fc2f-287">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6fc2f-288">deviceStatusOverview</span><span class="sxs-lookup"><span data-stu-id="6fc2f-288">deviceStatusOverview</span></span>|[<span data-ttu-id="6fc2f-289">deviceConfigurationDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="6fc2f-289">deviceConfigurationDeviceOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|<span data-ttu-id="6fc2f-290">设备配置设备状态概述 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6fc2f-290">Device Configuration devices status overview Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6fc2f-291">userStatusOverview</span><span class="sxs-lookup"><span data-stu-id="6fc2f-291">userStatusOverview</span></span>|[<span data-ttu-id="6fc2f-292">deviceConfigurationUserOverview</span><span class="sxs-lookup"><span data-stu-id="6fc2f-292">deviceConfigurationUserOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|<span data-ttu-id="6fc2f-293">设备配置用户状态概述 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6fc2f-293">Device Configuration users status overview Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6fc2f-294">deviceSettingStateSummaries</span><span class="sxs-lookup"><span data-stu-id="6fc2f-294">deviceSettingStateSummaries</span></span>|<span data-ttu-id="6fc2f-295">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) 集合</span><span class="sxs-lookup"><span data-stu-id="6fc2f-295">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) collection</span></span>|<span data-ttu-id="6fc2f-296">设备配置设置状态设备摘要 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6fc2f-296">Device Configuration Setting State Device Summary Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6fc2f-297">将 identitycertificate</span><span class="sxs-lookup"><span data-stu-id="6fc2f-297">identityCertificate</span></span>|[<span data-ttu-id="6fc2f-298">windowsCertificateProfileBase</span><span class="sxs-lookup"><span data-stu-id="6fc2f-298">windowsCertificateProfileBase</span></span>](../resources/intune-deviceconfig-windowscertificateprofilebase.md)|<span data-ttu-id="6fc2f-299">在身份验证方法为证书时，用于客户端身份验证的标识证书。</span><span class="sxs-lookup"><span data-stu-id="6fc2f-299">Identity certificate for client authentication when authentication method is certificate.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="6fc2f-300">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6fc2f-300">JSON Representation</span></span>
<span data-ttu-id="6fc2f-301">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6fc2f-301">Here is a JSON representation of the resource.</span></span>
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



