---
title: windows10VpnConfiguration 资源类型
description: 通过提供此配置文件中的配置, 可以指示 Windows 10 设备 (桌面或移动版) 连接到所需的 VPN 终结点。 通过指定 vpn 终结点预期的身份验证方法和安全类型, 可以为最终用户进行无缝的 VPN 连接。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c4b1b906fc4a98895acc6e23a4b3e9a4d78ff28a
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30148711"
---
# <a name="windows10vpnconfiguration-resource-type"></a><span data-ttu-id="86617-104">windows10VpnConfiguration 资源类型</span><span class="sxs-lookup"><span data-stu-id="86617-104">windows10VpnConfiguration resource type</span></span>

> <span data-ttu-id="86617-105">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="86617-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="86617-106">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="86617-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="86617-107">通过提供此配置文件中的配置, 可以指示 Windows 10 设备 (桌面或移动版) 连接到所需的 VPN 终结点。</span><span class="sxs-lookup"><span data-stu-id="86617-107">By providing the configurations in this profile you can instruct the Windows 10 device (desktop or mobile) to connect to desired VPN endpoint.</span></span> <span data-ttu-id="86617-108">通过指定 vpn 终结点预期的身份验证方法和安全类型, 可以为最终用户进行无缝的 VPN 连接。</span><span class="sxs-lookup"><span data-stu-id="86617-108">By specifying the authentication method and security types expected by VPN endpoint you can make the VPN connection seamless for end user.</span></span>


<span data-ttu-id="86617-109">继承自[windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="86617-109">Inherits from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>

## <a name="methods"></a><span data-ttu-id="86617-110">方法</span><span class="sxs-lookup"><span data-stu-id="86617-110">Methods</span></span>
|<span data-ttu-id="86617-111">方法</span><span class="sxs-lookup"><span data-stu-id="86617-111">Method</span></span>|<span data-ttu-id="86617-112">返回类型</span><span class="sxs-lookup"><span data-stu-id="86617-112">Return Type</span></span>|<span data-ttu-id="86617-113">说明</span><span class="sxs-lookup"><span data-stu-id="86617-113">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="86617-114">列出 windows10VpnConfigurations</span><span class="sxs-lookup"><span data-stu-id="86617-114">List windows10VpnConfigurations</span></span>](../api/intune-deviceconfig-windows10vpnconfiguration-list.md)|<span data-ttu-id="86617-115">[windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md)集合</span><span class="sxs-lookup"><span data-stu-id="86617-115">[windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) collection</span></span>|<span data-ttu-id="86617-116">列出[windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="86617-116">List properties and relationships of the [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="86617-117">获取 windows10VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="86617-117">Get windows10VpnConfiguration</span></span>](../api/intune-deviceconfig-windows10vpnconfiguration-get.md)|[<span data-ttu-id="86617-118">windows10VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="86617-118">windows10VpnConfiguration</span></span>](../resources/intune-deviceconfig-windows10vpnconfiguration.md)|<span data-ttu-id="86617-119">读取[windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="86617-119">Read properties and relationships of the [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) object.</span></span>|
|[<span data-ttu-id="86617-120">创建 windows10VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="86617-120">Create windows10VpnConfiguration</span></span>](../api/intune-deviceconfig-windows10vpnconfiguration-create.md)|[<span data-ttu-id="86617-121">windows10VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="86617-121">windows10VpnConfiguration</span></span>](../resources/intune-deviceconfig-windows10vpnconfiguration.md)|<span data-ttu-id="86617-122">创建新的[windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="86617-122">Create a new [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) object.</span></span>|
|[<span data-ttu-id="86617-123">删除 windows10VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="86617-123">Delete windows10VpnConfiguration</span></span>](../api/intune-deviceconfig-windows10vpnconfiguration-delete.md)|<span data-ttu-id="86617-124">无</span><span class="sxs-lookup"><span data-stu-id="86617-124">None</span></span>|<span data-ttu-id="86617-125">删除[windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md)。</span><span class="sxs-lookup"><span data-stu-id="86617-125">Deletes a [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md).</span></span>|
|[<span data-ttu-id="86617-126">更新 windows10VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="86617-126">Update windows10VpnConfiguration</span></span>](../api/intune-deviceconfig-windows10vpnconfiguration-update.md)|[<span data-ttu-id="86617-127">windows10VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="86617-127">windows10VpnConfiguration</span></span>](../resources/intune-deviceconfig-windows10vpnconfiguration.md)|<span data-ttu-id="86617-128">更新[windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="86617-128">Update the properties of a [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="86617-129">属性</span><span class="sxs-lookup"><span data-stu-id="86617-129">Properties</span></span>
|<span data-ttu-id="86617-130">属性</span><span class="sxs-lookup"><span data-stu-id="86617-130">Property</span></span>|<span data-ttu-id="86617-131">类型</span><span class="sxs-lookup"><span data-stu-id="86617-131">Type</span></span>|<span data-ttu-id="86617-132">说明</span><span class="sxs-lookup"><span data-stu-id="86617-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="86617-133">id</span><span class="sxs-lookup"><span data-stu-id="86617-133">id</span></span>|<span data-ttu-id="86617-134">String</span><span class="sxs-lookup"><span data-stu-id="86617-134">String</span></span>|<span data-ttu-id="86617-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="86617-135">Key of the entity.</span></span> <span data-ttu-id="86617-136">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="86617-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="86617-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="86617-137">lastModifiedDateTime</span></span>|<span data-ttu-id="86617-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="86617-138">DateTimeOffset</span></span>|<span data-ttu-id="86617-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="86617-139">DateTime the object was last modified.</span></span> <span data-ttu-id="86617-140">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="86617-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="86617-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="86617-141">roleScopeTagIds</span></span>|<span data-ttu-id="86617-142">String collection</span><span class="sxs-lookup"><span data-stu-id="86617-142">String collection</span></span>|<span data-ttu-id="86617-143">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="86617-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="86617-144">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="86617-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="86617-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="86617-145">supportsScopeTags</span></span>|<span data-ttu-id="86617-146">布尔</span><span class="sxs-lookup"><span data-stu-id="86617-146">Boolean</span></span>|<span data-ttu-id="86617-147">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="86617-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="86617-148">如果此值为 false, 则不允许分配给 ScopeTags 属性, 并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="86617-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="86617-149">这适用于在 Silverlight 中创建的旧版策略, 可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="86617-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="86617-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="86617-150">This property is read-only.</span></span> <span data-ttu-id="86617-151">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="86617-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="86617-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="86617-152">createdDateTime</span></span>|<span data-ttu-id="86617-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="86617-153">DateTimeOffset</span></span>|<span data-ttu-id="86617-154">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="86617-154">DateTime the object was created.</span></span> <span data-ttu-id="86617-155">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="86617-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="86617-156">description</span><span class="sxs-lookup"><span data-stu-id="86617-156">description</span></span>|<span data-ttu-id="86617-157">String</span><span class="sxs-lookup"><span data-stu-id="86617-157">String</span></span>|<span data-ttu-id="86617-158">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="86617-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="86617-159">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="86617-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="86617-160">displayName</span><span class="sxs-lookup"><span data-stu-id="86617-160">displayName</span></span>|<span data-ttu-id="86617-161">String</span><span class="sxs-lookup"><span data-stu-id="86617-161">String</span></span>|<span data-ttu-id="86617-162">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="86617-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="86617-163">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="86617-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="86617-164">version</span><span class="sxs-lookup"><span data-stu-id="86617-164">version</span></span>|<span data-ttu-id="86617-165">Int32</span><span class="sxs-lookup"><span data-stu-id="86617-165">Int32</span></span>|<span data-ttu-id="86617-166">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="86617-166">Version of the device configuration.</span></span> <span data-ttu-id="86617-167">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="86617-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="86617-168">connectionName</span><span class="sxs-lookup"><span data-stu-id="86617-168">connectionName</span></span>|<span data-ttu-id="86617-169">字符串</span><span class="sxs-lookup"><span data-stu-id="86617-169">String</span></span>|<span data-ttu-id="86617-170">向用户显示的连接名称。</span><span class="sxs-lookup"><span data-stu-id="86617-170">Connection name displayed to the user.</span></span> <span data-ttu-id="86617-171">继承自[windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="86617-171">Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="86617-172">服务器</span><span class="sxs-lookup"><span data-stu-id="86617-172">servers</span></span>|<span data-ttu-id="86617-173">[vpnServer](../resources/intune-deviceconfig-vpnserver.md)集合</span><span class="sxs-lookup"><span data-stu-id="86617-173">[vpnServer](../resources/intune-deviceconfig-vpnserver.md) collection</span></span>|<span data-ttu-id="86617-174">网络上的 VPN 服务器的列表。</span><span class="sxs-lookup"><span data-stu-id="86617-174">List of VPN Servers on the network.</span></span> <span data-ttu-id="86617-175">请确保最终用户可以访问这些网络位置。</span><span class="sxs-lookup"><span data-stu-id="86617-175">Make sure end users can access these network locations.</span></span> <span data-ttu-id="86617-176">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="86617-176">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="86617-177">继承自[windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="86617-177">Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="86617-178">customXml</span><span class="sxs-lookup"><span data-stu-id="86617-178">customXml</span></span>|<span data-ttu-id="86617-179">Binary</span><span class="sxs-lookup"><span data-stu-id="86617-179">Binary</span></span>|<span data-ttu-id="86617-180">配置 VPN 连接的自定义 XML 命令。</span><span class="sxs-lookup"><span data-stu-id="86617-180">Custom XML commands that configures the VPN connection.</span></span> <span data-ttu-id="86617-181">(UTF8 编码的字节数组)继承自[windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="86617-181">(UTF8 encoded byte array) Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="86617-182">profileTarget</span><span class="sxs-lookup"><span data-stu-id="86617-182">profileTarget</span></span>|[<span data-ttu-id="86617-183">windows10VpnProfileTarget</span><span class="sxs-lookup"><span data-stu-id="86617-183">windows10VpnProfileTarget</span></span>](../resources/intune-deviceconfig-windows10vpnprofiletarget.md)|<span data-ttu-id="86617-184">配置文件目标类型。</span><span class="sxs-lookup"><span data-stu-id="86617-184">Profile target type.</span></span> <span data-ttu-id="86617-185">可取值为：`user`、`device`、`autoPilotDevice`。</span><span class="sxs-lookup"><span data-stu-id="86617-185">Possible values are: `user`, `device`, `autoPilotDevice`.</span></span>|
|<span data-ttu-id="86617-186">connectionType</span><span class="sxs-lookup"><span data-stu-id="86617-186">connectionType</span></span>|[<span data-ttu-id="86617-187">windows10VpnConnectionType</span><span class="sxs-lookup"><span data-stu-id="86617-187">windows10VpnConnectionType</span></span>](../resources/intune-deviceconfig-windows10vpnconnectiontype.md)|<span data-ttu-id="86617-188">连接类型。</span><span class="sxs-lookup"><span data-stu-id="86617-188">Connection type.</span></span> <span data-ttu-id="86617-189">可取值为：`pulseSecure`、`f5EdgeClient`、`dellSonicWallMobileConnect`、`checkPointCapsuleVpn`、`automatic`、`ikEv2`、`l2tp`、`pptp`、`citrix`、`paloAltoGlobalProtect`。</span><span class="sxs-lookup"><span data-stu-id="86617-189">Possible values are: `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `automatic`, `ikEv2`, `l2tp`, `pptp`, `citrix`, `paloAltoGlobalProtect`.</span></span>|
|<span data-ttu-id="86617-190">enableSplitTunneling</span><span class="sxs-lookup"><span data-stu-id="86617-190">enableSplitTunneling</span></span>|<span data-ttu-id="86617-191">布尔</span><span class="sxs-lookup"><span data-stu-id="86617-191">Boolean</span></span>|<span data-ttu-id="86617-192">启用拆分隧道。</span><span class="sxs-lookup"><span data-stu-id="86617-192">Enable split tunneling.</span></span>|
|<span data-ttu-id="86617-193">enableAlwaysOn</span><span class="sxs-lookup"><span data-stu-id="86617-193">enableAlwaysOn</span></span>|<span data-ttu-id="86617-194">布尔</span><span class="sxs-lookup"><span data-stu-id="86617-194">Boolean</span></span>|<span data-ttu-id="86617-195">启用始终打开模式。</span><span class="sxs-lookup"><span data-stu-id="86617-195">Enable Always On mode.</span></span>|
|<span data-ttu-id="86617-196">enableDeviceTunnel</span><span class="sxs-lookup"><span data-stu-id="86617-196">enableDeviceTunnel</span></span>|<span data-ttu-id="86617-197">布尔</span><span class="sxs-lookup"><span data-stu-id="86617-197">Boolean</span></span>|<span data-ttu-id="86617-198">启用设备隧道。</span><span class="sxs-lookup"><span data-stu-id="86617-198">Enable device tunnel.</span></span>|
|<span data-ttu-id="86617-199">enableDnsRegistration</span><span class="sxs-lookup"><span data-stu-id="86617-199">enableDnsRegistration</span></span>|<span data-ttu-id="86617-200">布尔</span><span class="sxs-lookup"><span data-stu-id="86617-200">Boolean</span></span>|<span data-ttu-id="86617-201">使用内部 DNS 启用 IP 地址注册。</span><span class="sxs-lookup"><span data-stu-id="86617-201">Enable IP address registration with internal DNS.</span></span>|
|<span data-ttu-id="86617-202">dnsSuffixes</span><span class="sxs-lookup"><span data-stu-id="86617-202">dnsSuffixes</span></span>|<span data-ttu-id="86617-203">String collection</span><span class="sxs-lookup"><span data-stu-id="86617-203">String collection</span></span>|<span data-ttu-id="86617-204">指定要添加到 dns 搜索列表以正确路由短名称的 dns 后缀。</span><span class="sxs-lookup"><span data-stu-id="86617-204">Specify DNS suffixes to add to the DNS search list to properly route short names.</span></span>|
|<span data-ttu-id="86617-205">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="86617-205">authenticationMethod</span></span>|[<span data-ttu-id="86617-206">windows10VpnAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="86617-206">windows10VpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-windows10vpnauthenticationmethod.md)|<span data-ttu-id="86617-207">身份验证方法。</span><span class="sxs-lookup"><span data-stu-id="86617-207">Authentication method.</span></span> <span data-ttu-id="86617-208">可取值为：`certificate`、`usernameAndPassword`、`customEapXml`。</span><span class="sxs-lookup"><span data-stu-id="86617-208">Possible values are: `certificate`, `usernameAndPassword`, `customEapXml`.</span></span>|
|<span data-ttu-id="86617-209">rememberUserCredentials</span><span class="sxs-lookup"><span data-stu-id="86617-209">rememberUserCredentials</span></span>|<span data-ttu-id="86617-210">布尔</span><span class="sxs-lookup"><span data-stu-id="86617-210">Boolean</span></span>|<span data-ttu-id="86617-211">记住用户凭据。</span><span class="sxs-lookup"><span data-stu-id="86617-211">Remember user credentials.</span></span>|
|<span data-ttu-id="86617-212">enableConditionalAccess</span><span class="sxs-lookup"><span data-stu-id="86617-212">enableConditionalAccess</span></span>|<span data-ttu-id="86617-213">布尔</span><span class="sxs-lookup"><span data-stu-id="86617-213">Boolean</span></span>|<span data-ttu-id="86617-214">启用条件访问。</span><span class="sxs-lookup"><span data-stu-id="86617-214">Enable conditional access.</span></span>|
|<span data-ttu-id="86617-215">enableSingleSignOnWithAlternateCertificate</span><span class="sxs-lookup"><span data-stu-id="86617-215">enableSingleSignOnWithAlternateCertificate</span></span>|<span data-ttu-id="86617-216">布尔</span><span class="sxs-lookup"><span data-stu-id="86617-216">Boolean</span></span>|<span data-ttu-id="86617-217">启用具有备用证书的单一登录 (SSO)。</span><span class="sxs-lookup"><span data-stu-id="86617-217">Enable single sign-on (SSO) with alternate certificate.</span></span>|
|<span data-ttu-id="86617-218">singleSignOnEku</span><span class="sxs-lookup"><span data-stu-id="86617-218">singleSignOnEku</span></span>|[<span data-ttu-id="86617-219">extendedKeyUsage</span><span class="sxs-lookup"><span data-stu-id="86617-219">extendedKeyUsage</span></span>](../resources/intune-deviceconfig-extendedkeyusage.md)|<span data-ttu-id="86617-220">单一登录扩展密钥用法 (EKU)。</span><span class="sxs-lookup"><span data-stu-id="86617-220">Single sign-on Extended Key Usage (EKU).</span></span>|
|<span data-ttu-id="86617-221">singleSignOnIssuerHash</span><span class="sxs-lookup"><span data-stu-id="86617-221">singleSignOnIssuerHash</span></span>|<span data-ttu-id="86617-222">字符串</span><span class="sxs-lookup"><span data-stu-id="86617-222">String</span></span>|<span data-ttu-id="86617-223">单一登录颁发者哈希。</span><span class="sxs-lookup"><span data-stu-id="86617-223">Single sign-on issuer hash.</span></span>|
|<span data-ttu-id="86617-224">eapXml</span><span class="sxs-lookup"><span data-stu-id="86617-224">eapXml</span></span>|<span data-ttu-id="86617-225">Binary</span><span class="sxs-lookup"><span data-stu-id="86617-225">Binary</span></span>|<span data-ttu-id="86617-226">可扩展的身份验证协议 (EAP) XML。</span><span class="sxs-lookup"><span data-stu-id="86617-226">Extensible Authentication Protocol (EAP) XML.</span></span> <span data-ttu-id="86617-227">（UTF8 编码的字节数组）</span><span class="sxs-lookup"><span data-stu-id="86617-227">(UTF8 encoded byte array)</span></span>|
|<span data-ttu-id="86617-228">proxyServer</span><span class="sxs-lookup"><span data-stu-id="86617-228">proxyServer</span></span>|[<span data-ttu-id="86617-229">windows10VpnProxyServer</span><span class="sxs-lookup"><span data-stu-id="86617-229">windows10VpnProxyServer</span></span>](../resources/intune-deviceconfig-windows10vpnproxyserver.md)|<span data-ttu-id="86617-230">代理服务器。</span><span class="sxs-lookup"><span data-stu-id="86617-230">Proxy Server.</span></span>|
|<span data-ttu-id="86617-231">associatedApps</span><span class="sxs-lookup"><span data-stu-id="86617-231">associatedApps</span></span>|<span data-ttu-id="86617-232">[windows10AssociatedApps](../resources/intune-deviceconfig-windows10associatedapps.md)集合</span><span class="sxs-lookup"><span data-stu-id="86617-232">[windows10AssociatedApps](../resources/intune-deviceconfig-windows10associatedapps.md) collection</span></span>|<span data-ttu-id="86617-233">关联的应用。</span><span class="sxs-lookup"><span data-stu-id="86617-233">Associated Apps.</span></span> <span data-ttu-id="86617-234">该集合最多可包含 10000 个元素。</span><span class="sxs-lookup"><span data-stu-id="86617-234">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="86617-235">onlyAssociatedAppsCanUseConnection</span><span class="sxs-lookup"><span data-stu-id="86617-235">onlyAssociatedAppsCanUseConnection</span></span>|<span data-ttu-id="86617-236">布尔</span><span class="sxs-lookup"><span data-stu-id="86617-236">Boolean</span></span>|<span data-ttu-id="86617-237">仅关联的应用程序可以使用连接 (每个应用 VPN)。</span><span class="sxs-lookup"><span data-stu-id="86617-237">Only associated Apps can use connection (per-app VPN).</span></span>|
|<span data-ttu-id="86617-238">windowsInformationProtectionDomain</span><span class="sxs-lookup"><span data-stu-id="86617-238">windowsInformationProtectionDomain</span></span>|<span data-ttu-id="86617-239">字符串</span><span class="sxs-lookup"><span data-stu-id="86617-239">String</span></span>|<span data-ttu-id="86617-240">与此连接关联的 Windows 信息保护 (WIP) 域。</span><span class="sxs-lookup"><span data-stu-id="86617-240">Windows Information Protection (WIP) domain to associate with this connection.</span></span>|
|<span data-ttu-id="86617-241">trafficRules</span><span class="sxs-lookup"><span data-stu-id="86617-241">trafficRules</span></span>|<span data-ttu-id="86617-242">[vpnTrafficRule](../resources/intune-deviceconfig-vpntrafficrule.md)集合</span><span class="sxs-lookup"><span data-stu-id="86617-242">[vpnTrafficRule](../resources/intune-deviceconfig-vpntrafficrule.md) collection</span></span>|<span data-ttu-id="86617-243">流量规则。</span><span class="sxs-lookup"><span data-stu-id="86617-243">Traffic rules.</span></span> <span data-ttu-id="86617-244">该集合最多可包含 1000 个元素。</span><span class="sxs-lookup"><span data-stu-id="86617-244">This collection can contain a maximum of 1000 elements.</span></span>|
|<span data-ttu-id="86617-245">航线</span><span class="sxs-lookup"><span data-stu-id="86617-245">routes</span></span>|<span data-ttu-id="86617-246">[vpnRoute](../resources/intune-deviceconfig-vpnroute.md)集合</span><span class="sxs-lookup"><span data-stu-id="86617-246">[vpnRoute](../resources/intune-deviceconfig-vpnroute.md) collection</span></span>|<span data-ttu-id="86617-247">路由 (可选用于第三方提供程序)。</span><span class="sxs-lookup"><span data-stu-id="86617-247">Routes (optional for third-party providers).</span></span> <span data-ttu-id="86617-248">该集合最多可包含 1000 个元素。</span><span class="sxs-lookup"><span data-stu-id="86617-248">This collection can contain a maximum of 1000 elements.</span></span>|
|<span data-ttu-id="86617-249">dnsRules</span><span class="sxs-lookup"><span data-stu-id="86617-249">dnsRules</span></span>|<span data-ttu-id="86617-250">[vpnDnsRule](../resources/intune-deviceconfig-vpndnsrule.md)集合</span><span class="sxs-lookup"><span data-stu-id="86617-250">[vpnDnsRule](../resources/intune-deviceconfig-vpndnsrule.md) collection</span></span>|<span data-ttu-id="86617-251">DNS 规则。</span><span class="sxs-lookup"><span data-stu-id="86617-251">DNS rules.</span></span> <span data-ttu-id="86617-252">该集合最多可包含 1000 个元素。</span><span class="sxs-lookup"><span data-stu-id="86617-252">This collection can contain a maximum of 1000 elements.</span></span>|
|<span data-ttu-id="86617-253">trustedNetworkDomains</span><span class="sxs-lookup"><span data-stu-id="86617-253">trustedNetworkDomains</span></span>|<span data-ttu-id="86617-254">String collection</span><span class="sxs-lookup"><span data-stu-id="86617-254">String collection</span></span>|<span data-ttu-id="86617-255">受信任的网络域</span><span class="sxs-lookup"><span data-stu-id="86617-255">Trusted Network Domains</span></span>|

## <a name="relationships"></a><span data-ttu-id="86617-256">关系</span><span class="sxs-lookup"><span data-stu-id="86617-256">Relationships</span></span>
|<span data-ttu-id="86617-257">关系</span><span class="sxs-lookup"><span data-stu-id="86617-257">Relationship</span></span>|<span data-ttu-id="86617-258">类型</span><span class="sxs-lookup"><span data-stu-id="86617-258">Type</span></span>|<span data-ttu-id="86617-259">说明</span><span class="sxs-lookup"><span data-stu-id="86617-259">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="86617-260">groupAssignments</span><span class="sxs-lookup"><span data-stu-id="86617-260">groupAssignments</span></span>|<span data-ttu-id="86617-261">[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)集合</span><span class="sxs-lookup"><span data-stu-id="86617-261">[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) collection</span></span>|<span data-ttu-id="86617-262">设备配置文件的组分配列表。</span><span class="sxs-lookup"><span data-stu-id="86617-262">The list of group assignments for the device configuration profile.</span></span> <span data-ttu-id="86617-263">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="86617-263">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="86617-264">assignments</span><span class="sxs-lookup"><span data-stu-id="86617-264">assignments</span></span>|<span data-ttu-id="86617-265">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="86617-265">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection</span></span>|<span data-ttu-id="86617-266">设备配置文件的分配列表。</span><span class="sxs-lookup"><span data-stu-id="86617-266">The list of assignments for the device configuration profile.</span></span> <span data-ttu-id="86617-267">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="86617-267">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="86617-268">deviceStatuses</span><span class="sxs-lookup"><span data-stu-id="86617-268">deviceStatuses</span></span>|<span data-ttu-id="86617-269">[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) 集合</span><span class="sxs-lookup"><span data-stu-id="86617-269">[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) collection</span></span>|<span data-ttu-id="86617-270">按设备的设备配置安装状态。</span><span class="sxs-lookup"><span data-stu-id="86617-270">Device configuration installation status by device.</span></span> <span data-ttu-id="86617-271">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="86617-271">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="86617-272">userStatuses</span><span class="sxs-lookup"><span data-stu-id="86617-272">userStatuses</span></span>|<span data-ttu-id="86617-273">[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) 集合</span><span class="sxs-lookup"><span data-stu-id="86617-273">[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) collection</span></span>|<span data-ttu-id="86617-274">按用户的设备配置安装状态。</span><span class="sxs-lookup"><span data-stu-id="86617-274">Device configuration installation status by user.</span></span> <span data-ttu-id="86617-275">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="86617-275">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="86617-276">deviceStatusOverview</span><span class="sxs-lookup"><span data-stu-id="86617-276">deviceStatusOverview</span></span>|[<span data-ttu-id="86617-277">deviceConfigurationDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="86617-277">deviceConfigurationDeviceOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|<span data-ttu-id="86617-278">设备配置设备状态概述 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="86617-278">Device Configuration devices status overview Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="86617-279">userStatusOverview</span><span class="sxs-lookup"><span data-stu-id="86617-279">userStatusOverview</span></span>|[<span data-ttu-id="86617-280">deviceConfigurationUserOverview</span><span class="sxs-lookup"><span data-stu-id="86617-280">deviceConfigurationUserOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|<span data-ttu-id="86617-281">设备配置用户状态概述 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="86617-281">Device Configuration users status overview Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="86617-282">deviceSettingStateSummaries</span><span class="sxs-lookup"><span data-stu-id="86617-282">deviceSettingStateSummaries</span></span>|<span data-ttu-id="86617-283">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) 集合</span><span class="sxs-lookup"><span data-stu-id="86617-283">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) collection</span></span>|<span data-ttu-id="86617-284">设备配置设置状态设备摘要 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="86617-284">Device Configuration Setting State Device Summary Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="86617-285">将 identitycertificate</span><span class="sxs-lookup"><span data-stu-id="86617-285">identityCertificate</span></span>|[<span data-ttu-id="86617-286">windowsCertificateProfileBase</span><span class="sxs-lookup"><span data-stu-id="86617-286">windowsCertificateProfileBase</span></span>](../resources/intune-deviceconfig-windowscertificateprofilebase.md)|<span data-ttu-id="86617-287">在身份验证方法为证书时, 用于客户端身份验证的标识证书。</span><span class="sxs-lookup"><span data-stu-id="86617-287">Identity certificate for client authentication when authentication method is certificate.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="86617-288">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="86617-288">JSON Representation</span></span>
<span data-ttu-id="86617-289">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="86617-289">Here is a JSON representation of the resource.</span></span>
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




