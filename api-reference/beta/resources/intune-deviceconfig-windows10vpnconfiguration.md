---
title: windows10VpnConfiguration 资源类型
description: 通过提供此配置文件中的配置，可以指示 Windows 10 设备（桌面或移动版）连接到所需的 VPN 终结点。 通过指定 VPN 终结点预期的身份验证方法和安全类型，可以为最终用户进行无缝的 VPN 连接。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: fb7eb030856d622ffdbeeba384fc88cab9930234
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42786633"
---
# <a name="windows10vpnconfiguration-resource-type"></a><span data-ttu-id="a20d6-104">windows10VpnConfiguration 资源类型</span><span class="sxs-lookup"><span data-stu-id="a20d6-104">windows10VpnConfiguration resource type</span></span>

> <span data-ttu-id="a20d6-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="a20d6-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a20d6-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="a20d6-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a20d6-107">通过提供此配置文件中的配置，可以指示 Windows 10 设备（桌面或移动版）连接到所需的 VPN 终结点。</span><span class="sxs-lookup"><span data-stu-id="a20d6-107">By providing the configurations in this profile you can instruct the Windows 10 device (desktop or mobile) to connect to desired VPN endpoint.</span></span> <span data-ttu-id="a20d6-108">通过指定 VPN 终结点预期的身份验证方法和安全类型，可以为最终用户进行无缝的 VPN 连接。</span><span class="sxs-lookup"><span data-stu-id="a20d6-108">By specifying the authentication method and security types expected by VPN endpoint you can make the VPN connection seamless for end user.</span></span>


<span data-ttu-id="a20d6-109">继承自[windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a20d6-109">Inherits from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>

## <a name="methods"></a><span data-ttu-id="a20d6-110">方法</span><span class="sxs-lookup"><span data-stu-id="a20d6-110">Methods</span></span>
|<span data-ttu-id="a20d6-111">方法</span><span class="sxs-lookup"><span data-stu-id="a20d6-111">Method</span></span>|<span data-ttu-id="a20d6-112">返回类型</span><span class="sxs-lookup"><span data-stu-id="a20d6-112">Return Type</span></span>|<span data-ttu-id="a20d6-113">说明</span><span class="sxs-lookup"><span data-stu-id="a20d6-113">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="a20d6-114">列出 windows10VpnConfigurations</span><span class="sxs-lookup"><span data-stu-id="a20d6-114">List windows10VpnConfigurations</span></span>](../api/intune-deviceconfig-windows10vpnconfiguration-list.md)|<span data-ttu-id="a20d6-115">[windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md)集合</span><span class="sxs-lookup"><span data-stu-id="a20d6-115">[windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) collection</span></span>|<span data-ttu-id="a20d6-116">列出[windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="a20d6-116">List properties and relationships of the [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="a20d6-117">获取 windows10VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="a20d6-117">Get windows10VpnConfiguration</span></span>](../api/intune-deviceconfig-windows10vpnconfiguration-get.md)|[<span data-ttu-id="a20d6-118">windows10VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="a20d6-118">windows10VpnConfiguration</span></span>](../resources/intune-deviceconfig-windows10vpnconfiguration.md)|<span data-ttu-id="a20d6-119">读取[windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="a20d6-119">Read properties and relationships of the [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) object.</span></span>|
|[<span data-ttu-id="a20d6-120">创建 windows10VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="a20d6-120">Create windows10VpnConfiguration</span></span>](../api/intune-deviceconfig-windows10vpnconfiguration-create.md)|[<span data-ttu-id="a20d6-121">windows10VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="a20d6-121">windows10VpnConfiguration</span></span>](../resources/intune-deviceconfig-windows10vpnconfiguration.md)|<span data-ttu-id="a20d6-122">创建新的[windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="a20d6-122">Create a new [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) object.</span></span>|
|[<span data-ttu-id="a20d6-123">删除 windows10VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="a20d6-123">Delete windows10VpnConfiguration</span></span>](../api/intune-deviceconfig-windows10vpnconfiguration-delete.md)|<span data-ttu-id="a20d6-124">None</span><span class="sxs-lookup"><span data-stu-id="a20d6-124">None</span></span>|<span data-ttu-id="a20d6-125">删除[windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md)。</span><span class="sxs-lookup"><span data-stu-id="a20d6-125">Deletes a [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md).</span></span>|
|[<span data-ttu-id="a20d6-126">更新 windows10VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="a20d6-126">Update windows10VpnConfiguration</span></span>](../api/intune-deviceconfig-windows10vpnconfiguration-update.md)|[<span data-ttu-id="a20d6-127">windows10VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="a20d6-127">windows10VpnConfiguration</span></span>](../resources/intune-deviceconfig-windows10vpnconfiguration.md)|<span data-ttu-id="a20d6-128">更新[windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="a20d6-128">Update the properties of a [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="a20d6-129">属性</span><span class="sxs-lookup"><span data-stu-id="a20d6-129">Properties</span></span>
|<span data-ttu-id="a20d6-130">属性</span><span class="sxs-lookup"><span data-stu-id="a20d6-130">Property</span></span>|<span data-ttu-id="a20d6-131">类型</span><span class="sxs-lookup"><span data-stu-id="a20d6-131">Type</span></span>|<span data-ttu-id="a20d6-132">说明</span><span class="sxs-lookup"><span data-stu-id="a20d6-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a20d6-133">id</span><span class="sxs-lookup"><span data-stu-id="a20d6-133">id</span></span>|<span data-ttu-id="a20d6-134">字符串</span><span class="sxs-lookup"><span data-stu-id="a20d6-134">String</span></span>|<span data-ttu-id="a20d6-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="a20d6-135">Key of the entity.</span></span> <span data-ttu-id="a20d6-136">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a20d6-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a20d6-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a20d6-137">lastModifiedDateTime</span></span>|<span data-ttu-id="a20d6-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a20d6-138">DateTimeOffset</span></span>|<span data-ttu-id="a20d6-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="a20d6-139">DateTime the object was last modified.</span></span> <span data-ttu-id="a20d6-140">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a20d6-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a20d6-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="a20d6-141">roleScopeTagIds</span></span>|<span data-ttu-id="a20d6-142">String collection</span><span class="sxs-lookup"><span data-stu-id="a20d6-142">String collection</span></span>|<span data-ttu-id="a20d6-143">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="a20d6-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="a20d6-144">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a20d6-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a20d6-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="a20d6-145">supportsScopeTags</span></span>|<span data-ttu-id="a20d6-146">布尔值</span><span class="sxs-lookup"><span data-stu-id="a20d6-146">Boolean</span></span>|<span data-ttu-id="a20d6-147">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="a20d6-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="a20d6-148">如果此值为 false，则不允许分配给 ScopeTags 属性，并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="a20d6-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="a20d6-149">这适用于在 Silverlight 中创建的旧版策略，可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="a20d6-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="a20d6-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="a20d6-150">This property is read-only.</span></span> <span data-ttu-id="a20d6-151">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a20d6-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a20d6-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="a20d6-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="a20d6-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="a20d6-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="a20d6-154">适用于此策略的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="a20d6-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="a20d6-155">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a20d6-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a20d6-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="a20d6-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="a20d6-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="a20d6-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="a20d6-158">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="a20d6-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="a20d6-159">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a20d6-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a20d6-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="a20d6-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="a20d6-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="a20d6-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="a20d6-162">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="a20d6-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="a20d6-163">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a20d6-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a20d6-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a20d6-164">createdDateTime</span></span>|<span data-ttu-id="a20d6-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a20d6-165">DateTimeOffset</span></span>|<span data-ttu-id="a20d6-166">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="a20d6-166">DateTime the object was created.</span></span> <span data-ttu-id="a20d6-167">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a20d6-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a20d6-168">说明</span><span class="sxs-lookup"><span data-stu-id="a20d6-168">description</span></span>|<span data-ttu-id="a20d6-169">String</span><span class="sxs-lookup"><span data-stu-id="a20d6-169">String</span></span>|<span data-ttu-id="a20d6-170">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="a20d6-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="a20d6-171">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a20d6-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a20d6-172">displayName</span><span class="sxs-lookup"><span data-stu-id="a20d6-172">displayName</span></span>|<span data-ttu-id="a20d6-173">String</span><span class="sxs-lookup"><span data-stu-id="a20d6-173">String</span></span>|<span data-ttu-id="a20d6-174">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="a20d6-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="a20d6-175">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a20d6-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a20d6-176">version</span><span class="sxs-lookup"><span data-stu-id="a20d6-176">version</span></span>|<span data-ttu-id="a20d6-177">Int32</span><span class="sxs-lookup"><span data-stu-id="a20d6-177">Int32</span></span>|<span data-ttu-id="a20d6-178">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="a20d6-178">Version of the device configuration.</span></span> <span data-ttu-id="a20d6-179">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a20d6-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a20d6-180">connectionName</span><span class="sxs-lookup"><span data-stu-id="a20d6-180">connectionName</span></span>|<span data-ttu-id="a20d6-181">String</span><span class="sxs-lookup"><span data-stu-id="a20d6-181">String</span></span>|<span data-ttu-id="a20d6-182">向用户显示的连接名称。</span><span class="sxs-lookup"><span data-stu-id="a20d6-182">Connection name displayed to the user.</span></span> <span data-ttu-id="a20d6-183">继承自[windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a20d6-183">Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="a20d6-184">台</span><span class="sxs-lookup"><span data-stu-id="a20d6-184">servers</span></span>|<span data-ttu-id="a20d6-185">[vpnServer](../resources/intune-deviceconfig-vpnserver.md)集合</span><span class="sxs-lookup"><span data-stu-id="a20d6-185">[vpnServer](../resources/intune-deviceconfig-vpnserver.md) collection</span></span>|<span data-ttu-id="a20d6-186">网络上的 VPN 服务器的列表。</span><span class="sxs-lookup"><span data-stu-id="a20d6-186">List of VPN Servers on the network.</span></span> <span data-ttu-id="a20d6-187">请确保最终用户可以访问这些网络位置。</span><span class="sxs-lookup"><span data-stu-id="a20d6-187">Make sure end users can access these network locations.</span></span> <span data-ttu-id="a20d6-188">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="a20d6-188">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="a20d6-189">继承自[windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a20d6-189">Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="a20d6-190">customXml</span><span class="sxs-lookup"><span data-stu-id="a20d6-190">customXml</span></span>|<span data-ttu-id="a20d6-191">Binary</span><span class="sxs-lookup"><span data-stu-id="a20d6-191">Binary</span></span>|<span data-ttu-id="a20d6-192">配置 VPN 连接的自定义 XML 命令。</span><span class="sxs-lookup"><span data-stu-id="a20d6-192">Custom XML commands that configures the VPN connection.</span></span> <span data-ttu-id="a20d6-193">（UTF8 编码的字节数组）继承自[windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a20d6-193">(UTF8 encoded byte array) Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="a20d6-194">profileTarget</span><span class="sxs-lookup"><span data-stu-id="a20d6-194">profileTarget</span></span>|[<span data-ttu-id="a20d6-195">windows10VpnProfileTarget</span><span class="sxs-lookup"><span data-stu-id="a20d6-195">windows10VpnProfileTarget</span></span>](../resources/intune-deviceconfig-windows10vpnprofiletarget.md)|<span data-ttu-id="a20d6-196">配置文件目标类型。</span><span class="sxs-lookup"><span data-stu-id="a20d6-196">Profile target type.</span></span> <span data-ttu-id="a20d6-197">可取值为：`user`、`device`、`autoPilotDevice`。</span><span class="sxs-lookup"><span data-stu-id="a20d6-197">Possible values are: `user`, `device`, `autoPilotDevice`.</span></span>|
|<span data-ttu-id="a20d6-198">connectionType</span><span class="sxs-lookup"><span data-stu-id="a20d6-198">connectionType</span></span>|[<span data-ttu-id="a20d6-199">windows10VpnConnectionType</span><span class="sxs-lookup"><span data-stu-id="a20d6-199">windows10VpnConnectionType</span></span>](../resources/intune-deviceconfig-windows10vpnconnectiontype.md)|<span data-ttu-id="a20d6-200">连接类型。</span><span class="sxs-lookup"><span data-stu-id="a20d6-200">Connection type.</span></span> <span data-ttu-id="a20d6-201">可取值为：`pulseSecure`、`f5EdgeClient`、`dellSonicWallMobileConnect`、`checkPointCapsuleVpn`、`automatic`、`ikEv2`、`l2tp`、`pptp`、`citrix`、`paloAltoGlobalProtect`。</span><span class="sxs-lookup"><span data-stu-id="a20d6-201">Possible values are: `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `automatic`, `ikEv2`, `l2tp`, `pptp`, `citrix`, `paloAltoGlobalProtect`.</span></span>|
|<span data-ttu-id="a20d6-202">enableSplitTunneling</span><span class="sxs-lookup"><span data-stu-id="a20d6-202">enableSplitTunneling</span></span>|<span data-ttu-id="a20d6-203">布尔值</span><span class="sxs-lookup"><span data-stu-id="a20d6-203">Boolean</span></span>|<span data-ttu-id="a20d6-204">启用拆分隧道。</span><span class="sxs-lookup"><span data-stu-id="a20d6-204">Enable split tunneling.</span></span>|
|<span data-ttu-id="a20d6-205">enableAlwaysOn</span><span class="sxs-lookup"><span data-stu-id="a20d6-205">enableAlwaysOn</span></span>|<span data-ttu-id="a20d6-206">布尔值</span><span class="sxs-lookup"><span data-stu-id="a20d6-206">Boolean</span></span>|<span data-ttu-id="a20d6-207">启用始终打开模式。</span><span class="sxs-lookup"><span data-stu-id="a20d6-207">Enable Always On mode.</span></span>|
|<span data-ttu-id="a20d6-208">enableDeviceTunnel</span><span class="sxs-lookup"><span data-stu-id="a20d6-208">enableDeviceTunnel</span></span>|<span data-ttu-id="a20d6-209">布尔值</span><span class="sxs-lookup"><span data-stu-id="a20d6-209">Boolean</span></span>|<span data-ttu-id="a20d6-210">启用设备隧道。</span><span class="sxs-lookup"><span data-stu-id="a20d6-210">Enable device tunnel.</span></span>|
|<span data-ttu-id="a20d6-211">enableDnsRegistration</span><span class="sxs-lookup"><span data-stu-id="a20d6-211">enableDnsRegistration</span></span>|<span data-ttu-id="a20d6-212">布尔值</span><span class="sxs-lookup"><span data-stu-id="a20d6-212">Boolean</span></span>|<span data-ttu-id="a20d6-213">使用内部 DNS 启用 IP 地址注册。</span><span class="sxs-lookup"><span data-stu-id="a20d6-213">Enable IP address registration with internal DNS.</span></span>|
|<span data-ttu-id="a20d6-214">dnsSuffixes</span><span class="sxs-lookup"><span data-stu-id="a20d6-214">dnsSuffixes</span></span>|<span data-ttu-id="a20d6-215">String collection</span><span class="sxs-lookup"><span data-stu-id="a20d6-215">String collection</span></span>|<span data-ttu-id="a20d6-216">指定要添加到 DNS 搜索列表以正确路由短名称的 DNS 后缀。</span><span class="sxs-lookup"><span data-stu-id="a20d6-216">Specify DNS suffixes to add to the DNS search list to properly route short names.</span></span>|
|<span data-ttu-id="a20d6-217">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="a20d6-217">authenticationMethod</span></span>|[<span data-ttu-id="a20d6-218">windows10VpnAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="a20d6-218">windows10VpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-windows10vpnauthenticationmethod.md)|<span data-ttu-id="a20d6-219">身份验证方法。</span><span class="sxs-lookup"><span data-stu-id="a20d6-219">Authentication method.</span></span> <span data-ttu-id="a20d6-220">可取值为：`certificate`、`usernameAndPassword`、`customEapXml`。</span><span class="sxs-lookup"><span data-stu-id="a20d6-220">Possible values are: `certificate`, `usernameAndPassword`, `customEapXml`.</span></span>|
|<span data-ttu-id="a20d6-221">rememberUserCredentials</span><span class="sxs-lookup"><span data-stu-id="a20d6-221">rememberUserCredentials</span></span>|<span data-ttu-id="a20d6-222">布尔值</span><span class="sxs-lookup"><span data-stu-id="a20d6-222">Boolean</span></span>|<span data-ttu-id="a20d6-223">记住用户凭据。</span><span class="sxs-lookup"><span data-stu-id="a20d6-223">Remember user credentials.</span></span>|
|<span data-ttu-id="a20d6-224">enableConditionalAccess</span><span class="sxs-lookup"><span data-stu-id="a20d6-224">enableConditionalAccess</span></span>|<span data-ttu-id="a20d6-225">布尔值</span><span class="sxs-lookup"><span data-stu-id="a20d6-225">Boolean</span></span>|<span data-ttu-id="a20d6-226">启用条件访问。</span><span class="sxs-lookup"><span data-stu-id="a20d6-226">Enable conditional access.</span></span>|
|<span data-ttu-id="a20d6-227">enableSingleSignOnWithAlternateCertificate</span><span class="sxs-lookup"><span data-stu-id="a20d6-227">enableSingleSignOnWithAlternateCertificate</span></span>|<span data-ttu-id="a20d6-228">布尔值</span><span class="sxs-lookup"><span data-stu-id="a20d6-228">Boolean</span></span>|<span data-ttu-id="a20d6-229">启用具有备用证书的单一登录（SSO）。</span><span class="sxs-lookup"><span data-stu-id="a20d6-229">Enable single sign-on (SSO) with alternate certificate.</span></span>|
|<span data-ttu-id="a20d6-230">singleSignOnEku</span><span class="sxs-lookup"><span data-stu-id="a20d6-230">singleSignOnEku</span></span>|[<span data-ttu-id="a20d6-231">extendedKeyUsage</span><span class="sxs-lookup"><span data-stu-id="a20d6-231">extendedKeyUsage</span></span>](../resources/intune-deviceconfig-extendedkeyusage.md)|<span data-ttu-id="a20d6-232">单一登录扩展密钥用法（EKU）。</span><span class="sxs-lookup"><span data-stu-id="a20d6-232">Single sign-on Extended Key Usage (EKU).</span></span>|
|<span data-ttu-id="a20d6-233">singleSignOnIssuerHash</span><span class="sxs-lookup"><span data-stu-id="a20d6-233">singleSignOnIssuerHash</span></span>|<span data-ttu-id="a20d6-234">String</span><span class="sxs-lookup"><span data-stu-id="a20d6-234">String</span></span>|<span data-ttu-id="a20d6-235">单一登录颁发者哈希。</span><span class="sxs-lookup"><span data-stu-id="a20d6-235">Single sign-on issuer hash.</span></span>|
|<span data-ttu-id="a20d6-236">eapXml</span><span class="sxs-lookup"><span data-stu-id="a20d6-236">eapXml</span></span>|<span data-ttu-id="a20d6-237">Binary</span><span class="sxs-lookup"><span data-stu-id="a20d6-237">Binary</span></span>|<span data-ttu-id="a20d6-238">可扩展的身份验证协议（EAP） XML。</span><span class="sxs-lookup"><span data-stu-id="a20d6-238">Extensible Authentication Protocol (EAP) XML.</span></span> <span data-ttu-id="a20d6-239">（UTF8 编码的字节数组）</span><span class="sxs-lookup"><span data-stu-id="a20d6-239">(UTF8 encoded byte array)</span></span>|
|<span data-ttu-id="a20d6-240">proxyServer</span><span class="sxs-lookup"><span data-stu-id="a20d6-240">proxyServer</span></span>|[<span data-ttu-id="a20d6-241">windows10VpnProxyServer</span><span class="sxs-lookup"><span data-stu-id="a20d6-241">windows10VpnProxyServer</span></span>](../resources/intune-deviceconfig-windows10vpnproxyserver.md)|<span data-ttu-id="a20d6-242">代理服务器。</span><span class="sxs-lookup"><span data-stu-id="a20d6-242">Proxy Server.</span></span>|
|<span data-ttu-id="a20d6-243">associatedApps</span><span class="sxs-lookup"><span data-stu-id="a20d6-243">associatedApps</span></span>|<span data-ttu-id="a20d6-244">[windows10AssociatedApps](../resources/intune-deviceconfig-windows10associatedapps.md)集合</span><span class="sxs-lookup"><span data-stu-id="a20d6-244">[windows10AssociatedApps](../resources/intune-deviceconfig-windows10associatedapps.md) collection</span></span>|<span data-ttu-id="a20d6-245">关联的应用。</span><span class="sxs-lookup"><span data-stu-id="a20d6-245">Associated Apps.</span></span> <span data-ttu-id="a20d6-246">该集合最多可包含 10000 个元素。</span><span class="sxs-lookup"><span data-stu-id="a20d6-246">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="a20d6-247">onlyAssociatedAppsCanUseConnection</span><span class="sxs-lookup"><span data-stu-id="a20d6-247">onlyAssociatedAppsCanUseConnection</span></span>|<span data-ttu-id="a20d6-248">布尔值</span><span class="sxs-lookup"><span data-stu-id="a20d6-248">Boolean</span></span>|<span data-ttu-id="a20d6-249">仅关联的应用程序可以使用连接（每个应用 VPN）。</span><span class="sxs-lookup"><span data-stu-id="a20d6-249">Only associated Apps can use connection (per-app VPN).</span></span>|
|<span data-ttu-id="a20d6-250">windowsInformationProtectionDomain</span><span class="sxs-lookup"><span data-stu-id="a20d6-250">windowsInformationProtectionDomain</span></span>|<span data-ttu-id="a20d6-251">String</span><span class="sxs-lookup"><span data-stu-id="a20d6-251">String</span></span>|<span data-ttu-id="a20d6-252">与此连接关联的 Windows 信息保护（WIP）域。</span><span class="sxs-lookup"><span data-stu-id="a20d6-252">Windows Information Protection (WIP) domain to associate with this connection.</span></span>|
|<span data-ttu-id="a20d6-253">trafficRules</span><span class="sxs-lookup"><span data-stu-id="a20d6-253">trafficRules</span></span>|<span data-ttu-id="a20d6-254">[vpnTrafficRule](../resources/intune-deviceconfig-vpntrafficrule.md)集合</span><span class="sxs-lookup"><span data-stu-id="a20d6-254">[vpnTrafficRule](../resources/intune-deviceconfig-vpntrafficrule.md) collection</span></span>|<span data-ttu-id="a20d6-255">流量规则。</span><span class="sxs-lookup"><span data-stu-id="a20d6-255">Traffic rules.</span></span> <span data-ttu-id="a20d6-256">该集合最多可包含 1000 个元素。</span><span class="sxs-lookup"><span data-stu-id="a20d6-256">This collection can contain a maximum of 1000 elements.</span></span>|
|<span data-ttu-id="a20d6-257">航线</span><span class="sxs-lookup"><span data-stu-id="a20d6-257">routes</span></span>|<span data-ttu-id="a20d6-258">[vpnRoute](../resources/intune-deviceconfig-vpnroute.md)集合</span><span class="sxs-lookup"><span data-stu-id="a20d6-258">[vpnRoute](../resources/intune-deviceconfig-vpnroute.md) collection</span></span>|<span data-ttu-id="a20d6-259">路由（可选用于第三方提供程序）。</span><span class="sxs-lookup"><span data-stu-id="a20d6-259">Routes (optional for third-party providers).</span></span> <span data-ttu-id="a20d6-260">该集合最多可包含 1000 个元素。</span><span class="sxs-lookup"><span data-stu-id="a20d6-260">This collection can contain a maximum of 1000 elements.</span></span>|
|<span data-ttu-id="a20d6-261">dnsRules</span><span class="sxs-lookup"><span data-stu-id="a20d6-261">dnsRules</span></span>|<span data-ttu-id="a20d6-262">[vpnDnsRule](../resources/intune-deviceconfig-vpndnsrule.md)集合</span><span class="sxs-lookup"><span data-stu-id="a20d6-262">[vpnDnsRule](../resources/intune-deviceconfig-vpndnsrule.md) collection</span></span>|<span data-ttu-id="a20d6-263">DNS 规则。</span><span class="sxs-lookup"><span data-stu-id="a20d6-263">DNS rules.</span></span> <span data-ttu-id="a20d6-264">该集合最多可包含 1000 个元素。</span><span class="sxs-lookup"><span data-stu-id="a20d6-264">This collection can contain a maximum of 1000 elements.</span></span>|
|<span data-ttu-id="a20d6-265">trustedNetworkDomains</span><span class="sxs-lookup"><span data-stu-id="a20d6-265">trustedNetworkDomains</span></span>|<span data-ttu-id="a20d6-266">String collection</span><span class="sxs-lookup"><span data-stu-id="a20d6-266">String collection</span></span>|<span data-ttu-id="a20d6-267">受信任的网络域</span><span class="sxs-lookup"><span data-stu-id="a20d6-267">Trusted Network Domains</span></span>|

## <a name="relationships"></a><span data-ttu-id="a20d6-268">关系</span><span class="sxs-lookup"><span data-stu-id="a20d6-268">Relationships</span></span>
|<span data-ttu-id="a20d6-269">关系</span><span class="sxs-lookup"><span data-stu-id="a20d6-269">Relationship</span></span>|<span data-ttu-id="a20d6-270">类型</span><span class="sxs-lookup"><span data-stu-id="a20d6-270">Type</span></span>|<span data-ttu-id="a20d6-271">说明</span><span class="sxs-lookup"><span data-stu-id="a20d6-271">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a20d6-272">groupAssignments</span><span class="sxs-lookup"><span data-stu-id="a20d6-272">groupAssignments</span></span>|<span data-ttu-id="a20d6-273">[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)集合</span><span class="sxs-lookup"><span data-stu-id="a20d6-273">[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) collection</span></span>|<span data-ttu-id="a20d6-274">设备配置文件的组分配列表。</span><span class="sxs-lookup"><span data-stu-id="a20d6-274">The list of group assignments for the device configuration profile.</span></span> <span data-ttu-id="a20d6-275">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a20d6-275">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a20d6-276">assignments</span><span class="sxs-lookup"><span data-stu-id="a20d6-276">assignments</span></span>|<span data-ttu-id="a20d6-277">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="a20d6-277">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection</span></span>|<span data-ttu-id="a20d6-278">设备配置文件的分配列表。</span><span class="sxs-lookup"><span data-stu-id="a20d6-278">The list of assignments for the device configuration profile.</span></span> <span data-ttu-id="a20d6-279">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a20d6-279">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a20d6-280">deviceStatuses</span><span class="sxs-lookup"><span data-stu-id="a20d6-280">deviceStatuses</span></span>|<span data-ttu-id="a20d6-281">[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) 集合</span><span class="sxs-lookup"><span data-stu-id="a20d6-281">[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) collection</span></span>|<span data-ttu-id="a20d6-282">按设备的设备配置安装状态。</span><span class="sxs-lookup"><span data-stu-id="a20d6-282">Device configuration installation status by device.</span></span> <span data-ttu-id="a20d6-283">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a20d6-283">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a20d6-284">userStatuses</span><span class="sxs-lookup"><span data-stu-id="a20d6-284">userStatuses</span></span>|<span data-ttu-id="a20d6-285">[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) 集合</span><span class="sxs-lookup"><span data-stu-id="a20d6-285">[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) collection</span></span>|<span data-ttu-id="a20d6-286">按用户的设备配置安装状态。</span><span class="sxs-lookup"><span data-stu-id="a20d6-286">Device configuration installation status by user.</span></span> <span data-ttu-id="a20d6-287">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a20d6-287">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a20d6-288">deviceStatusOverview</span><span class="sxs-lookup"><span data-stu-id="a20d6-288">deviceStatusOverview</span></span>|[<span data-ttu-id="a20d6-289">deviceConfigurationDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="a20d6-289">deviceConfigurationDeviceOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|<span data-ttu-id="a20d6-290">设备配置设备状态概述 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a20d6-290">Device Configuration devices status overview Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a20d6-291">userStatusOverview</span><span class="sxs-lookup"><span data-stu-id="a20d6-291">userStatusOverview</span></span>|[<span data-ttu-id="a20d6-292">deviceConfigurationUserOverview</span><span class="sxs-lookup"><span data-stu-id="a20d6-292">deviceConfigurationUserOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|<span data-ttu-id="a20d6-293">设备配置用户状态概述 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a20d6-293">Device Configuration users status overview Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a20d6-294">deviceSettingStateSummaries</span><span class="sxs-lookup"><span data-stu-id="a20d6-294">deviceSettingStateSummaries</span></span>|<span data-ttu-id="a20d6-295">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) 集合</span><span class="sxs-lookup"><span data-stu-id="a20d6-295">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) collection</span></span>|<span data-ttu-id="a20d6-296">设备配置设置状态设备摘要 继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a20d6-296">Device Configuration Setting State Device Summary Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a20d6-297">将 identitycertificate</span><span class="sxs-lookup"><span data-stu-id="a20d6-297">identityCertificate</span></span>|[<span data-ttu-id="a20d6-298">windowsCertificateProfileBase</span><span class="sxs-lookup"><span data-stu-id="a20d6-298">windowsCertificateProfileBase</span></span>](../resources/intune-deviceconfig-windowscertificateprofilebase.md)|<span data-ttu-id="a20d6-299">在身份验证方法为证书时，用于客户端身份验证的标识证书。</span><span class="sxs-lookup"><span data-stu-id="a20d6-299">Identity certificate for client authentication when authentication method is certificate.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a20d6-300">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a20d6-300">JSON Representation</span></span>
<span data-ttu-id="a20d6-301">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a20d6-301">Here is a JSON representation of the resource.</span></span>
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



