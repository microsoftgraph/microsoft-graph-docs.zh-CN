---
title: windows10VpnConfiguration 资源类型
description: 通过提供此配置文件中的配置, 可以指示 Windows 10 设备 (桌面或移动版) 连接到所需的 VPN 终结点。 通过指定 vpn 终结点预期的身份验证方法和安全类型, 可以为最终用户进行无缝的 VPN 连接。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 88d32aedb16516f7659ff6e8094172e4a59f6345
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32572015"
---
# <a name="windows10vpnconfiguration-resource-type"></a><span data-ttu-id="c0f9f-104">windows10VpnConfiguration 资源类型</span><span class="sxs-lookup"><span data-stu-id="c0f9f-104">windows10VpnConfiguration resource type</span></span>

> <span data-ttu-id="c0f9f-105">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="c0f9f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c0f9f-106">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c0f9f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c0f9f-107">通过提供此配置文件中的配置, 可以指示 Windows 10 设备 (桌面或移动版) 连接到所需的 VPN 终结点。</span><span class="sxs-lookup"><span data-stu-id="c0f9f-107">By providing the configurations in this profile you can instruct the Windows 10 device (desktop or mobile) to connect to desired VPN endpoint.</span></span> <span data-ttu-id="c0f9f-108">通过指定 vpn 终结点预期的身份验证方法和安全类型, 可以为最终用户进行无缝的 VPN 连接。</span><span class="sxs-lookup"><span data-stu-id="c0f9f-108">By specifying the authentication method and security types expected by VPN endpoint you can make the VPN connection seamless for end user.</span></span>


<span data-ttu-id="c0f9f-109">继承自[windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c0f9f-109">Inherits from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>

## <a name="methods"></a><span data-ttu-id="c0f9f-110">方法</span><span class="sxs-lookup"><span data-stu-id="c0f9f-110">Methods</span></span>
|<span data-ttu-id="c0f9f-111">方法</span><span class="sxs-lookup"><span data-stu-id="c0f9f-111">Method</span></span>|<span data-ttu-id="c0f9f-112">返回类型</span><span class="sxs-lookup"><span data-stu-id="c0f9f-112">Return Type</span></span>|<span data-ttu-id="c0f9f-113">说明</span><span class="sxs-lookup"><span data-stu-id="c0f9f-113">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="c0f9f-114">列出 windows10VpnConfigurations</span><span class="sxs-lookup"><span data-stu-id="c0f9f-114">List windows10VpnConfigurations</span></span>](../api/intune-deviceconfig-windows10vpnconfiguration-list.md)|<span data-ttu-id="c0f9f-115">[windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md)集合</span><span class="sxs-lookup"><span data-stu-id="c0f9f-115">[windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) collection</span></span>|<span data-ttu-id="c0f9f-116">列出[windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="c0f9f-116">List properties and relationships of the [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="c0f9f-117">获取 windows10VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="c0f9f-117">Get windows10VpnConfiguration</span></span>](../api/intune-deviceconfig-windows10vpnconfiguration-get.md)|[<span data-ttu-id="c0f9f-118">windows10VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="c0f9f-118">windows10VpnConfiguration</span></span>](../resources/intune-deviceconfig-windows10vpnconfiguration.md)|<span data-ttu-id="c0f9f-119">读取[windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="c0f9f-119">Read properties and relationships of the [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) object.</span></span>|
|[<span data-ttu-id="c0f9f-120">创建 windows10VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="c0f9f-120">Create windows10VpnConfiguration</span></span>](../api/intune-deviceconfig-windows10vpnconfiguration-create.md)|[<span data-ttu-id="c0f9f-121">windows10VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="c0f9f-121">windows10VpnConfiguration</span></span>](../resources/intune-deviceconfig-windows10vpnconfiguration.md)|<span data-ttu-id="c0f9f-122">创建新的[windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="c0f9f-122">Create a new [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) object.</span></span>|
|[<span data-ttu-id="c0f9f-123">删除 windows10VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="c0f9f-123">Delete windows10VpnConfiguration</span></span>](../api/intune-deviceconfig-windows10vpnconfiguration-delete.md)|<span data-ttu-id="c0f9f-124">无</span><span class="sxs-lookup"><span data-stu-id="c0f9f-124">None</span></span>|<span data-ttu-id="c0f9f-125">删除[windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md)。</span><span class="sxs-lookup"><span data-stu-id="c0f9f-125">Deletes a [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md).</span></span>|
|[<span data-ttu-id="c0f9f-126">更新 windows10VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="c0f9f-126">Update windows10VpnConfiguration</span></span>](../api/intune-deviceconfig-windows10vpnconfiguration-update.md)|[<span data-ttu-id="c0f9f-127">windows10VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="c0f9f-127">windows10VpnConfiguration</span></span>](../resources/intune-deviceconfig-windows10vpnconfiguration.md)|<span data-ttu-id="c0f9f-128">更新[windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="c0f9f-128">Update the properties of a [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="c0f9f-129">属性</span><span class="sxs-lookup"><span data-stu-id="c0f9f-129">Properties</span></span>
|<span data-ttu-id="c0f9f-130">属性</span><span class="sxs-lookup"><span data-stu-id="c0f9f-130">Property</span></span>|<span data-ttu-id="c0f9f-131">类型</span><span class="sxs-lookup"><span data-stu-id="c0f9f-131">Type</span></span>|<span data-ttu-id="c0f9f-132">说明</span><span class="sxs-lookup"><span data-stu-id="c0f9f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c0f9f-133">id</span><span class="sxs-lookup"><span data-stu-id="c0f9f-133">id</span></span>|<span data-ttu-id="c0f9f-134">字符串</span><span class="sxs-lookup"><span data-stu-id="c0f9f-134">String</span></span>|<span data-ttu-id="c0f9f-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="c0f9f-135">Key of the entity.</span></span> <span data-ttu-id="c0f9f-136">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c0f9f-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c0f9f-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c0f9f-137">lastModifiedDateTime</span></span>|<span data-ttu-id="c0f9f-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c0f9f-138">DateTimeOffset</span></span>|<span data-ttu-id="c0f9f-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="c0f9f-139">DateTime the object was last modified.</span></span> <span data-ttu-id="c0f9f-140">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c0f9f-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c0f9f-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="c0f9f-141">roleScopeTagIds</span></span>|<span data-ttu-id="c0f9f-142">String collection</span><span class="sxs-lookup"><span data-stu-id="c0f9f-142">String collection</span></span>|<span data-ttu-id="c0f9f-143">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="c0f9f-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="c0f9f-144">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c0f9f-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c0f9f-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="c0f9f-145">supportsScopeTags</span></span>|<span data-ttu-id="c0f9f-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="c0f9f-146">Boolean</span></span>|<span data-ttu-id="c0f9f-147">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="c0f9f-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="c0f9f-148">如果此值为 false, 则不允许分配给 ScopeTags 属性, 并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="c0f9f-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="c0f9f-149">这适用于在 Silverlight 中创建的旧版策略, 可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="c0f9f-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="c0f9f-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="c0f9f-150">This property is read-only.</span></span> <span data-ttu-id="c0f9f-151">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c0f9f-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c0f9f-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c0f9f-152">createdDateTime</span></span>|<span data-ttu-id="c0f9f-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c0f9f-153">DateTimeOffset</span></span>|<span data-ttu-id="c0f9f-154">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="c0f9f-154">DateTime the object was created.</span></span> <span data-ttu-id="c0f9f-155">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c0f9f-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c0f9f-156">说明</span><span class="sxs-lookup"><span data-stu-id="c0f9f-156">description</span></span>|<span data-ttu-id="c0f9f-157">String</span><span class="sxs-lookup"><span data-stu-id="c0f9f-157">String</span></span>|<span data-ttu-id="c0f9f-158">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="c0f9f-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="c0f9f-159">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c0f9f-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c0f9f-160">displayName</span><span class="sxs-lookup"><span data-stu-id="c0f9f-160">displayName</span></span>|<span data-ttu-id="c0f9f-161">String</span><span class="sxs-lookup"><span data-stu-id="c0f9f-161">String</span></span>|<span data-ttu-id="c0f9f-162">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="c0f9f-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="c0f9f-163">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c0f9f-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c0f9f-164">version</span><span class="sxs-lookup"><span data-stu-id="c0f9f-164">version</span></span>|<span data-ttu-id="c0f9f-165">Int32</span><span class="sxs-lookup"><span data-stu-id="c0f9f-165">Int32</span></span>|<span data-ttu-id="c0f9f-166">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="c0f9f-166">Version of the device configuration.</span></span> <span data-ttu-id="c0f9f-167">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c0f9f-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c0f9f-168">connectionName</span><span class="sxs-lookup"><span data-stu-id="c0f9f-168">connectionName</span></span>|<span data-ttu-id="c0f9f-169">String</span><span class="sxs-lookup"><span data-stu-id="c0f9f-169">String</span></span>|<span data-ttu-id="c0f9f-170">向用户显示的连接名称。</span><span class="sxs-lookup"><span data-stu-id="c0f9f-170">Connection name displayed to the user.</span></span> <span data-ttu-id="c0f9f-171">继承自[windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c0f9f-171">Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="c0f9f-172">台</span><span class="sxs-lookup"><span data-stu-id="c0f9f-172">servers</span></span>|<span data-ttu-id="c0f9f-173">[vpnServer](../resources/intune-deviceconfig-vpnserver.md)集合</span><span class="sxs-lookup"><span data-stu-id="c0f9f-173">[vpnServer](../resources/intune-deviceconfig-vpnserver.md) collection</span></span>|<span data-ttu-id="c0f9f-174">网络上的 VPN 服务器的列表。</span><span class="sxs-lookup"><span data-stu-id="c0f9f-174">List of VPN Servers on the network.</span></span> <span data-ttu-id="c0f9f-175">请确保最终用户可以访问这些网络位置。</span><span class="sxs-lookup"><span data-stu-id="c0f9f-175">Make sure end users can access these network locations.</span></span> <span data-ttu-id="c0f9f-176">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="c0f9f-176">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="c0f9f-177">继承自[windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c0f9f-177">Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="c0f9f-178">customXml</span><span class="sxs-lookup"><span data-stu-id="c0f9f-178">customXml</span></span>|<span data-ttu-id="c0f9f-179">Binary</span><span class="sxs-lookup"><span data-stu-id="c0f9f-179">Binary</span></span>|<span data-ttu-id="c0f9f-180">配置 VPN 连接的自定义 XML 命令。</span><span class="sxs-lookup"><span data-stu-id="c0f9f-180">Custom XML commands that configures the VPN connection.</span></span> <span data-ttu-id="c0f9f-181">(UTF8 编码的字节数组)继承自[windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c0f9f-181">(UTF8 encoded byte array) Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="c0f9f-182">profileTarget</span><span class="sxs-lookup"><span data-stu-id="c0f9f-182">profileTarget</span></span>|[<span data-ttu-id="c0f9f-183">windows10VpnProfileTarget</span><span class="sxs-lookup"><span data-stu-id="c0f9f-183">windows10VpnProfileTarget</span></span>](../resources/intune-deviceconfig-windows10vpnprofiletarget.md)|<span data-ttu-id="c0f9f-184">配置文件目标类型。</span><span class="sxs-lookup"><span data-stu-id="c0f9f-184">Profile target type.</span></span> <span data-ttu-id="c0f9f-185">可取值为：`user`、`device`、`autoPilotDevice`。</span><span class="sxs-lookup"><span data-stu-id="c0f9f-185">Possible values are: `user`, `device`, `autoPilotDevice`.</span></span>|
|<span data-ttu-id="c0f9f-186">connectionType</span><span class="sxs-lookup"><span data-stu-id="c0f9f-186">connectionType</span></span>|[<span data-ttu-id="c0f9f-187">windows10VpnConnectionType</span><span class="sxs-lookup"><span data-stu-id="c0f9f-187">windows10VpnConnectionType</span></span>](../resources/intune-deviceconfig-windows10vpnconnectiontype.md)|<span data-ttu-id="c0f9f-188">连接类型。</span><span class="sxs-lookup"><span data-stu-id="c0f9f-188">Connection type.</span></span> <span data-ttu-id="c0f9f-189">可取值为：`pulseSecure`、`f5EdgeClient`、`dellSonicWallMobileConnect`、`checkPointCapsuleVpn`、`automatic`、`ikEv2`、`l2tp`、`pptp`、`citrix`、`paloAltoGlobalProtect`。</span><span class="sxs-lookup"><span data-stu-id="c0f9f-189">Possible values are: `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `automatic`, `ikEv2`, `l2tp`, `pptp`, `citrix`, `paloAltoGlobalProtect`.</span></span>|
|<span data-ttu-id="c0f9f-190">enableSplitTunneling</span><span class="sxs-lookup"><span data-stu-id="c0f9f-190">enableSplitTunneling</span></span>|<span data-ttu-id="c0f9f-191">Boolean</span><span class="sxs-lookup"><span data-stu-id="c0f9f-191">Boolean</span></span>|<span data-ttu-id="c0f9f-192">启用拆分隧道。</span><span class="sxs-lookup"><span data-stu-id="c0f9f-192">Enable split tunneling.</span></span>|
|<span data-ttu-id="c0f9f-193">enableAlwaysOn</span><span class="sxs-lookup"><span data-stu-id="c0f9f-193">enableAlwaysOn</span></span>|<span data-ttu-id="c0f9f-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="c0f9f-194">Boolean</span></span>|<span data-ttu-id="c0f9f-195">启用始终打开模式。</span><span class="sxs-lookup"><span data-stu-id="c0f9f-195">Enable Always On mode.</span></span>|
|<span data-ttu-id="c0f9f-196">enableDeviceTunnel</span><span class="sxs-lookup"><span data-stu-id="c0f9f-196">enableDeviceTunnel</span></span>|<span data-ttu-id="c0f9f-197">Boolean</span><span class="sxs-lookup"><span data-stu-id="c0f9f-197">Boolean</span></span>|<span data-ttu-id="c0f9f-198">启用设备隧道。</span><span class="sxs-lookup"><span data-stu-id="c0f9f-198">Enable device tunnel.</span></span>|
|<span data-ttu-id="c0f9f-199">enableDnsRegistration</span><span class="sxs-lookup"><span data-stu-id="c0f9f-199">enableDnsRegistration</span></span>|<span data-ttu-id="c0f9f-200">Boolean</span><span class="sxs-lookup"><span data-stu-id="c0f9f-200">Boolean</span></span>|<span data-ttu-id="c0f9f-201">使用内部 DNS 启用 IP 地址注册。</span><span class="sxs-lookup"><span data-stu-id="c0f9f-201">Enable IP address registration with internal DNS.</span></span>|
|<span data-ttu-id="c0f9f-202">dnsSuffixes</span><span class="sxs-lookup"><span data-stu-id="c0f9f-202">dnsSuffixes</span></span>|<span data-ttu-id="c0f9f-203">String collection</span><span class="sxs-lookup"><span data-stu-id="c0f9f-203">String collection</span></span>|<span data-ttu-id="c0f9f-204">指定要添加到 dns 搜索列表以正确路由短名称的 dns 后缀。</span><span class="sxs-lookup"><span data-stu-id="c0f9f-204">Specify DNS suffixes to add to the DNS search list to properly route short names.</span></span>|
|<span data-ttu-id="c0f9f-205">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="c0f9f-205">authenticationMethod</span></span>|[<span data-ttu-id="c0f9f-206">windows10VpnAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="c0f9f-206">windows10VpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-windows10vpnauthenticationmethod.md)|<span data-ttu-id="c0f9f-207">身份验证方法。</span><span class="sxs-lookup"><span data-stu-id="c0f9f-207">Authentication method.</span></span> <span data-ttu-id="c0f9f-208">可取值为：`certificate`、`usernameAndPassword`、`customEapXml`。</span><span class="sxs-lookup"><span data-stu-id="c0f9f-208">Possible values are: `certificate`, `usernameAndPassword`, `customEapXml`.</span></span>|
|<span data-ttu-id="c0f9f-209">rememberUserCredentials</span><span class="sxs-lookup"><span data-stu-id="c0f9f-209">rememberUserCredentials</span></span>|<span data-ttu-id="c0f9f-210">Boolean</span><span class="sxs-lookup"><span data-stu-id="c0f9f-210">Boolean</span></span>|<span data-ttu-id="c0f9f-211">记住用户凭据。</span><span class="sxs-lookup"><span data-stu-id="c0f9f-211">Remember user credentials.</span></span>|
|<span data-ttu-id="c0f9f-212">enableConditionalAccess</span><span class="sxs-lookup"><span data-stu-id="c0f9f-212">enableConditionalAccess</span></span>|<span data-ttu-id="c0f9f-213">Boolean</span><span class="sxs-lookup"><span data-stu-id="c0f9f-213">Boolean</span></span>|<span data-ttu-id="c0f9f-214">启用条件访问。</span><span class="sxs-lookup"><span data-stu-id="c0f9f-214">Enable conditional access.</span></span>|
|<span data-ttu-id="c0f9f-215">enableSingleSignOnWithAlternateCertificate</span><span class="sxs-lookup"><span data-stu-id="c0f9f-215">enableSingleSignOnWithAlternateCertificate</span></span>|<span data-ttu-id="c0f9f-216">Boolean</span><span class="sxs-lookup"><span data-stu-id="c0f9f-216">Boolean</span></span>|<span data-ttu-id="c0f9f-217">启用具有备用证书的单一登录 (SSO)。</span><span class="sxs-lookup"><span data-stu-id="c0f9f-217">Enable single sign-on (SSO) with alternate certificate.</span></span>|
|<span data-ttu-id="c0f9f-218">singleSignOnEku</span><span class="sxs-lookup"><span data-stu-id="c0f9f-218">singleSignOnEku</span></span>|[<span data-ttu-id="c0f9f-219">extendedKeyUsage</span><span class="sxs-lookup"><span data-stu-id="c0f9f-219">extendedKeyUsage</span></span>](../resources/intune-deviceconfig-extendedkeyusage.md)|<span data-ttu-id="c0f9f-220">单一登录扩展密钥用法 (EKU)。</span><span class="sxs-lookup"><span data-stu-id="c0f9f-220">Single sign-on Extended Key Usage (EKU).</span></span>|
|<span data-ttu-id="c0f9f-221">singleSignOnIssuerHash</span><span class="sxs-lookup"><span data-stu-id="c0f9f-221">singleSignOnIssuerHash</span></span>|<span data-ttu-id="c0f9f-222">String</span><span class="sxs-lookup"><span data-stu-id="c0f9f-222">String</span></span>|<span data-ttu-id="c0f9f-223">单一登录颁发者哈希。</span><span class="sxs-lookup"><span data-stu-id="c0f9f-223">Single sign-on issuer hash.</span></span>|
|<span data-ttu-id="c0f9f-224">eapXml</span><span class="sxs-lookup"><span data-stu-id="c0f9f-224">eapXml</span></span>|<span data-ttu-id="c0f9f-225">Binary</span><span class="sxs-lookup"><span data-stu-id="c0f9f-225">Binary</span></span>|<span data-ttu-id="c0f9f-226">可扩展的身份验证协议 (EAP) XML。</span><span class="sxs-lookup"><span data-stu-id="c0f9f-226">Extensible Authentication Protocol (EAP) XML.</span></span> <span data-ttu-id="c0f9f-227">（UTF8 编码的字节数组）</span><span class="sxs-lookup"><span data-stu-id="c0f9f-227">(UTF8 encoded byte array)</span></span>|
|<span data-ttu-id="c0f9f-228">proxyServer</span><span class="sxs-lookup"><span data-stu-id="c0f9f-228">proxyServer</span></span>|[<span data-ttu-id="c0f9f-229">windows10VpnProxyServer</span><span class="sxs-lookup"><span data-stu-id="c0f9f-229">windows10VpnProxyServer</span></span>](../resources/intune-deviceconfig-windows10vpnproxyserver.md)|<span data-ttu-id="c0f9f-230">代理服务器。</span><span class="sxs-lookup"><span data-stu-id="c0f9f-230">Proxy Server.</span></span>|
|<span data-ttu-id="c0f9f-231">associatedApps</span><span class="sxs-lookup"><span data-stu-id="c0f9f-231">associatedApps</span></span>|<span data-ttu-id="c0f9f-232">[windows10AssociatedApps](../resources/intune-deviceconfig-windows10associatedapps.md)集合</span><span class="sxs-lookup"><span data-stu-id="c0f9f-232">[windows10AssociatedApps](../resources/intune-deviceconfig-windows10associatedapps.md) collection</span></span>|<span data-ttu-id="c0f9f-233">关联的应用。</span><span class="sxs-lookup"><span data-stu-id="c0f9f-233">Associated Apps.</span></span> <span data-ttu-id="c0f9f-234">该集合最多可包含 10000 个元素。</span><span class="sxs-lookup"><span data-stu-id="c0f9f-234">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="c0f9f-235">onlyAssociatedAppsCanUseConnection</span><span class="sxs-lookup"><span data-stu-id="c0f9f-235">onlyAssociatedAppsCanUseConnection</span></span>|<span data-ttu-id="c0f9f-236">Boolean</span><span class="sxs-lookup"><span data-stu-id="c0f9f-236">Boolean</span></span>|<span data-ttu-id="c0f9f-237">仅关联的应用程序可以使用连接 (每个应用 VPN)。</span><span class="sxs-lookup"><span data-stu-id="c0f9f-237">Only associated Apps can use connection (per-app VPN).</span></span>|
|<span data-ttu-id="c0f9f-238">windowsInformationProtectionDomain</span><span class="sxs-lookup"><span data-stu-id="c0f9f-238">windowsInformationProtectionDomain</span></span>|<span data-ttu-id="c0f9f-239">String</span><span class="sxs-lookup"><span data-stu-id="c0f9f-239">String</span></span>|<span data-ttu-id="c0f9f-240">与此连接关联的 Windows 信息保护 (WIP) 域。</span><span class="sxs-lookup"><span data-stu-id="c0f9f-240">Windows Information Protection (WIP) domain to associate with this connection.</span></span>|
|<span data-ttu-id="c0f9f-241">trafficRules</span><span class="sxs-lookup"><span data-stu-id="c0f9f-241">trafficRules</span></span>|<span data-ttu-id="c0f9f-242">[vpnTrafficRule](../resources/intune-deviceconfig-vpntrafficrule.md)集合</span><span class="sxs-lookup"><span data-stu-id="c0f9f-242">[vpnTrafficRule](../resources/intune-deviceconfig-vpntrafficrule.md) collection</span></span>|<span data-ttu-id="c0f9f-243">流量规则。</span><span class="sxs-lookup"><span data-stu-id="c0f9f-243">Traffic rules.</span></span> <span data-ttu-id="c0f9f-244">该集合最多可包含 1000 个元素。</span><span class="sxs-lookup"><span data-stu-id="c0f9f-244">This collection can contain a maximum of 1000 elements.</span></span>|
|<span data-ttu-id="c0f9f-245">航线</span><span class="sxs-lookup"><span data-stu-id="c0f9f-245">routes</span></span>|<span data-ttu-id="c0f9f-246">[vpnRoute](../resources/intune-deviceconfig-vpnroute.md)集合</span><span class="sxs-lookup"><span data-stu-id="c0f9f-246">[vpnRoute](../resources/intune-deviceconfig-vpnroute.md) collection</span></span>|<span data-ttu-id="c0f9f-247">路由 (可选用于第三方提供程序)。</span><span class="sxs-lookup"><span data-stu-id="c0f9f-247">Routes (optional for third-party providers).</span></span> <span data-ttu-id="c0f9f-248">该集合最多可包含 1000 个元素。</span><span class="sxs-lookup"><span data-stu-id="c0f9f-248">This collection can contain a maximum of 1000 elements.</span></span>|
|<span data-ttu-id="c0f9f-249">dnsRules</span><span class="sxs-lookup"><span data-stu-id="c0f9f-249">dnsRules</span></span>|<span data-ttu-id="c0f9f-250">[vpnDnsRule](../resources/intune-deviceconfig-vpndnsrule.md)集合</span><span class="sxs-lookup"><span data-stu-id="c0f9f-250">[vpnDnsRule](../resources/intune-deviceconfig-vpndnsrule.md) collection</span></span>|<span data-ttu-id="c0f9f-251">DNS 规则。</span><span class="sxs-lookup"><span data-stu-id="c0f9f-251">DNS rules.</span></span> <span data-ttu-id="c0f9f-252">该集合最多可包含 1000 个元素。</span><span class="sxs-lookup"><span data-stu-id="c0f9f-252">This collection can contain a maximum of 1000 elements.</span></span>|
|<span data-ttu-id="c0f9f-253">trustedNetworkDomains</span><span class="sxs-lookup"><span data-stu-id="c0f9f-253">trustedNetworkDomains</span></span>|<span data-ttu-id="c0f9f-254">String collection</span><span class="sxs-lookup"><span data-stu-id="c0f9f-254">String collection</span></span>|<span data-ttu-id="c0f9f-255">受信任的网络域</span><span class="sxs-lookup"><span data-stu-id="c0f9f-255">Trusted Network Domains</span></span>|

## <a name="relationships"></a><span data-ttu-id="c0f9f-256">关系</span><span class="sxs-lookup"><span data-stu-id="c0f9f-256">Relationships</span></span>
|<span data-ttu-id="c0f9f-257">关系</span><span class="sxs-lookup"><span data-stu-id="c0f9f-257">Relationship</span></span>|<span data-ttu-id="c0f9f-258">类型</span><span class="sxs-lookup"><span data-stu-id="c0f9f-258">Type</span></span>|<span data-ttu-id="c0f9f-259">说明</span><span class="sxs-lookup"><span data-stu-id="c0f9f-259">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c0f9f-260">groupAssignments</span><span class="sxs-lookup"><span data-stu-id="c0f9f-260">groupAssignments</span></span>|<span data-ttu-id="c0f9f-261">[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)集合</span><span class="sxs-lookup"><span data-stu-id="c0f9f-261">[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) collection</span></span>|<span data-ttu-id="c0f9f-262">设备配置文件的组分配列表。</span><span class="sxs-lookup"><span data-stu-id="c0f9f-262">The list of group assignments for the device configuration profile.</span></span> <span data-ttu-id="c0f9f-263">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c0f9f-263">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c0f9f-264">assignments</span><span class="sxs-lookup"><span data-stu-id="c0f9f-264">assignments</span></span>|<span data-ttu-id="c0f9f-265">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="c0f9f-265">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection</span></span>|<span data-ttu-id="c0f9f-266">设备配置文件的分配列表。</span><span class="sxs-lookup"><span data-stu-id="c0f9f-266">The list of assignments for the device configuration profile.</span></span> <span data-ttu-id="c0f9f-267">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c0f9f-267">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c0f9f-268">deviceStatuses</span><span class="sxs-lookup"><span data-stu-id="c0f9f-268">deviceStatuses</span></span>|<span data-ttu-id="c0f9f-269">[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) 集合</span><span class="sxs-lookup"><span data-stu-id="c0f9f-269">[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) collection</span></span>|<span data-ttu-id="c0f9f-270">按设备的设备配置安装状态。</span><span class="sxs-lookup"><span data-stu-id="c0f9f-270">Device configuration installation status by device.</span></span> <span data-ttu-id="c0f9f-271">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c0f9f-271">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c0f9f-272">userStatuses</span><span class="sxs-lookup"><span data-stu-id="c0f9f-272">userStatuses</span></span>|<span data-ttu-id="c0f9f-273">[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) 集合</span><span class="sxs-lookup"><span data-stu-id="c0f9f-273">[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) collection</span></span>|<span data-ttu-id="c0f9f-274">按用户的设备配置安装状态。</span><span class="sxs-lookup"><span data-stu-id="c0f9f-274">Device configuration installation status by user.</span></span> <span data-ttu-id="c0f9f-275">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c0f9f-275">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c0f9f-276">deviceStatusOverview</span><span class="sxs-lookup"><span data-stu-id="c0f9f-276">deviceStatusOverview</span></span>|[<span data-ttu-id="c0f9f-277">deviceConfigurationDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="c0f9f-277">deviceConfigurationDeviceOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|<span data-ttu-id="c0f9f-278">设备配置设备状态概述 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c0f9f-278">Device Configuration devices status overview Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c0f9f-279">userStatusOverview</span><span class="sxs-lookup"><span data-stu-id="c0f9f-279">userStatusOverview</span></span>|[<span data-ttu-id="c0f9f-280">deviceConfigurationUserOverview</span><span class="sxs-lookup"><span data-stu-id="c0f9f-280">deviceConfigurationUserOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|<span data-ttu-id="c0f9f-281">设备配置用户状态概述 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c0f9f-281">Device Configuration users status overview Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c0f9f-282">deviceSettingStateSummaries</span><span class="sxs-lookup"><span data-stu-id="c0f9f-282">deviceSettingStateSummaries</span></span>|<span data-ttu-id="c0f9f-283">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) 集合</span><span class="sxs-lookup"><span data-stu-id="c0f9f-283">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) collection</span></span>|<span data-ttu-id="c0f9f-284">设备配置设置状态设备摘要 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c0f9f-284">Device Configuration Setting State Device Summary Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c0f9f-285">将 identitycertificate</span><span class="sxs-lookup"><span data-stu-id="c0f9f-285">identityCertificate</span></span>|[<span data-ttu-id="c0f9f-286">windowsCertificateProfileBase</span><span class="sxs-lookup"><span data-stu-id="c0f9f-286">windowsCertificateProfileBase</span></span>](../resources/intune-deviceconfig-windowscertificateprofilebase.md)|<span data-ttu-id="c0f9f-287">在身份验证方法为证书时, 用于客户端身份验证的标识证书。</span><span class="sxs-lookup"><span data-stu-id="c0f9f-287">Identity certificate for client authentication when authentication method is certificate.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c0f9f-288">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c0f9f-288">JSON Representation</span></span>
<span data-ttu-id="c0f9f-289">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c0f9f-289">Here is a JSON representation of the resource.</span></span>
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





