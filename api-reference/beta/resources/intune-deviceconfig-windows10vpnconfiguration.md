---
title: windows10VpnConfiguration 资源类型
description: 通过提供此配置文件中的配置，您可以指示要连接到所需 VPN 终结点的 Windows 10 设备 （桌面或移动）。 通过指定的身份验证方法和安全类型预期 VPN 终结点，可进行 VPN 连接无缝的最终用户。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 775a4dfbeb46c27264b5539c51c63b29b488565b
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27937766"
---
# <a name="windows10vpnconfiguration-resource-type"></a><span data-ttu-id="c2395-104">windows10VpnConfiguration 资源类型</span><span class="sxs-lookup"><span data-stu-id="c2395-104">windows10VpnConfiguration resource type</span></span>

> <span data-ttu-id="c2395-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="c2395-105">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c2395-106">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="c2395-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c2395-107">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="c2395-107">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c2395-108">通过提供此配置文件中的配置，您可以指示要连接到所需 VPN 终结点的 Windows 10 设备 （桌面或移动）。</span><span class="sxs-lookup"><span data-stu-id="c2395-108">By providing the configurations in this profile you can instruct the Windows 10 device (desktop or mobile) to connect to desired VPN endpoint.</span></span> <span data-ttu-id="c2395-109">通过指定的身份验证方法和安全类型预期 VPN 终结点，可进行 VPN 连接无缝的最终用户。</span><span class="sxs-lookup"><span data-stu-id="c2395-109">By specifying the authentication method and security types expected by VPN endpoint you can make the VPN connection seamless for end user.</span></span>

<span data-ttu-id="c2395-110">继承自[windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c2395-110">Inherits from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>

## <a name="methods"></a><span data-ttu-id="c2395-111">方法</span><span class="sxs-lookup"><span data-stu-id="c2395-111">Methods</span></span>
|<span data-ttu-id="c2395-112">方法</span><span class="sxs-lookup"><span data-stu-id="c2395-112">Method</span></span>|<span data-ttu-id="c2395-113">返回类型</span><span class="sxs-lookup"><span data-stu-id="c2395-113">Return Type</span></span>|<span data-ttu-id="c2395-114">说明</span><span class="sxs-lookup"><span data-stu-id="c2395-114">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="c2395-115">列表 windows10VpnConfigurations</span><span class="sxs-lookup"><span data-stu-id="c2395-115">List windows10VpnConfigurations</span></span>](../api/intune-deviceconfig-windows10vpnconfiguration-list.md)|<span data-ttu-id="c2395-116">[windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md)集合</span><span class="sxs-lookup"><span data-stu-id="c2395-116">[windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) collection</span></span>|<span data-ttu-id="c2395-117">列出属性和[windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md)对象之间的关系。</span><span class="sxs-lookup"><span data-stu-id="c2395-117">List properties and relationships of the [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="c2395-118">获取 windows10VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="c2395-118">Get windows10VpnConfiguration</span></span>](../api/intune-deviceconfig-windows10vpnconfiguration-get.md)|[<span data-ttu-id="c2395-119">windows10VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="c2395-119">windows10VpnConfiguration</span></span>](../resources/intune-deviceconfig-windows10vpnconfiguration.md)|<span data-ttu-id="c2395-120">读取属性和[windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md)对象的关系。</span><span class="sxs-lookup"><span data-stu-id="c2395-120">Read properties and relationships of the [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) object.</span></span>|
|[<span data-ttu-id="c2395-121">创建 windows10VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="c2395-121">Create windows10VpnConfiguration</span></span>](../api/intune-deviceconfig-windows10vpnconfiguration-create.md)|[<span data-ttu-id="c2395-122">windows10VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="c2395-122">windows10VpnConfiguration</span></span>](../resources/intune-deviceconfig-windows10vpnconfiguration.md)|<span data-ttu-id="c2395-123">创建新的[windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="c2395-123">Create a new [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) object.</span></span>|
|[<span data-ttu-id="c2395-124">删除 windows10VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="c2395-124">Delete windows10VpnConfiguration</span></span>](../api/intune-deviceconfig-windows10vpnconfiguration-delete.md)|<span data-ttu-id="c2395-125">无</span><span class="sxs-lookup"><span data-stu-id="c2395-125">None</span></span>|<span data-ttu-id="c2395-126">删除[windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md)。</span><span class="sxs-lookup"><span data-stu-id="c2395-126">Deletes a [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md).</span></span>|
|[<span data-ttu-id="c2395-127">更新 windows10VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="c2395-127">Update windows10VpnConfiguration</span></span>](../api/intune-deviceconfig-windows10vpnconfiguration-update.md)|[<span data-ttu-id="c2395-128">windows10VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="c2395-128">windows10VpnConfiguration</span></span>](../resources/intune-deviceconfig-windows10vpnconfiguration.md)|<span data-ttu-id="c2395-129">更新[windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="c2395-129">Update the properties of a [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="c2395-130">属性</span><span class="sxs-lookup"><span data-stu-id="c2395-130">Properties</span></span>
|<span data-ttu-id="c2395-131">属性</span><span class="sxs-lookup"><span data-stu-id="c2395-131">Property</span></span>|<span data-ttu-id="c2395-132">类型</span><span class="sxs-lookup"><span data-stu-id="c2395-132">Type</span></span>|<span data-ttu-id="c2395-133">说明</span><span class="sxs-lookup"><span data-stu-id="c2395-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c2395-134">id</span><span class="sxs-lookup"><span data-stu-id="c2395-134">id</span></span>|<span data-ttu-id="c2395-135">String</span><span class="sxs-lookup"><span data-stu-id="c2395-135">String</span></span>|<span data-ttu-id="c2395-136">实体的键。</span><span class="sxs-lookup"><span data-stu-id="c2395-136">Key of the entity.</span></span> <span data-ttu-id="c2395-137">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c2395-137">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c2395-138">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c2395-138">lastModifiedDateTime</span></span>|<span data-ttu-id="c2395-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c2395-139">DateTimeOffset</span></span>|<span data-ttu-id="c2395-140">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="c2395-140">DateTime the object was last modified.</span></span> <span data-ttu-id="c2395-141">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c2395-141">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c2395-142">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="c2395-142">roleScopeTagIds</span></span>|<span data-ttu-id="c2395-143">String 集合</span><span class="sxs-lookup"><span data-stu-id="c2395-143">String collection</span></span>|<span data-ttu-id="c2395-144">此实体实例范围标记的列表。</span><span class="sxs-lookup"><span data-stu-id="c2395-144">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="c2395-145">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c2395-145">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c2395-146">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="c2395-146">supportsScopeTags</span></span>|<span data-ttu-id="c2395-147">布尔</span><span class="sxs-lookup"><span data-stu-id="c2395-147">Boolean</span></span>|<span data-ttu-id="c2395-148">指示基础的设备配置支持分配的范围标记。</span><span class="sxs-lookup"><span data-stu-id="c2395-148">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="c2395-149">此值为 false，并且实体将不会对作用域的用户可见时，不允许将分配给 ScopeTags 属性。</span><span class="sxs-lookup"><span data-stu-id="c2395-149">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="c2395-150">这将发生在 Silverlight 中创建的旧策略，并可以解析通过删除并重新创建 Azure 门户中的策略。</span><span class="sxs-lookup"><span data-stu-id="c2395-150">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="c2395-151">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="c2395-151">This property is read-only.</span></span> <span data-ttu-id="c2395-152">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c2395-152">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c2395-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c2395-153">createdDateTime</span></span>|<span data-ttu-id="c2395-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c2395-154">DateTimeOffset</span></span>|<span data-ttu-id="c2395-155">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="c2395-155">DateTime the object was created.</span></span> <span data-ttu-id="c2395-156">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c2395-156">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c2395-157">description</span><span class="sxs-lookup"><span data-stu-id="c2395-157">description</span></span>|<span data-ttu-id="c2395-158">String</span><span class="sxs-lookup"><span data-stu-id="c2395-158">String</span></span>|<span data-ttu-id="c2395-159">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="c2395-159">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="c2395-160">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c2395-160">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c2395-161">displayName</span><span class="sxs-lookup"><span data-stu-id="c2395-161">displayName</span></span>|<span data-ttu-id="c2395-162">String</span><span class="sxs-lookup"><span data-stu-id="c2395-162">String</span></span>|<span data-ttu-id="c2395-163">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="c2395-163">Admin provided name of the device configuration.</span></span> <span data-ttu-id="c2395-164">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c2395-164">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c2395-165">version</span><span class="sxs-lookup"><span data-stu-id="c2395-165">version</span></span>|<span data-ttu-id="c2395-166">Int32</span><span class="sxs-lookup"><span data-stu-id="c2395-166">Int32</span></span>|<span data-ttu-id="c2395-167">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="c2395-167">Version of the device configuration.</span></span> <span data-ttu-id="c2395-168">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c2395-168">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c2395-169">connectionName</span><span class="sxs-lookup"><span data-stu-id="c2395-169">connectionName</span></span>|<span data-ttu-id="c2395-170">字符串</span><span class="sxs-lookup"><span data-stu-id="c2395-170">String</span></span>|<span data-ttu-id="c2395-171">向用户显示的连接名称。</span><span class="sxs-lookup"><span data-stu-id="c2395-171">Connection name displayed to the user.</span></span> <span data-ttu-id="c2395-172">继承自[windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c2395-172">Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="c2395-173">服务器</span><span class="sxs-lookup"><span data-stu-id="c2395-173">servers</span></span>|<span data-ttu-id="c2395-174">[vpnServer](../resources/intune-deviceconfig-vpnserver.md)集合</span><span class="sxs-lookup"><span data-stu-id="c2395-174">[vpnServer](../resources/intune-deviceconfig-vpnserver.md) collection</span></span>|<span data-ttu-id="c2395-175">VPN 服务器的网络上的列表。</span><span class="sxs-lookup"><span data-stu-id="c2395-175">List of VPN Servers on the network.</span></span> <span data-ttu-id="c2395-176">确保最终用户可以访问这些网络位置。</span><span class="sxs-lookup"><span data-stu-id="c2395-176">Make sure end users can access these network locations.</span></span> <span data-ttu-id="c2395-177">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="c2395-177">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="c2395-178">继承自[windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c2395-178">Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="c2395-179">customXml</span><span class="sxs-lookup"><span data-stu-id="c2395-179">customXml</span></span>|<span data-ttu-id="c2395-180">Binary</span><span class="sxs-lookup"><span data-stu-id="c2395-180">Binary</span></span>|<span data-ttu-id="c2395-181">配置 VPN 连接的自定义 XML 命令。</span><span class="sxs-lookup"><span data-stu-id="c2395-181">Custom XML commands that configures the VPN connection.</span></span> <span data-ttu-id="c2395-182">（UTF8 编码的字节数组）继承自[windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c2395-182">(UTF8 encoded byte array) Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="c2395-183">profileTarget</span><span class="sxs-lookup"><span data-stu-id="c2395-183">profileTarget</span></span>|[<span data-ttu-id="c2395-184">windows10VpnProfileTarget</span><span class="sxs-lookup"><span data-stu-id="c2395-184">windows10VpnProfileTarget</span></span>](../resources/intune-deviceconfig-windows10vpnprofiletarget.md)|<span data-ttu-id="c2395-185">配置文件的目标类型。</span><span class="sxs-lookup"><span data-stu-id="c2395-185">Profile target type.</span></span> <span data-ttu-id="c2395-186">可取值为：`user`、`device`、`autoPilotDevice`。</span><span class="sxs-lookup"><span data-stu-id="c2395-186">Possible values are: `user`, `device`, `autoPilotDevice`.</span></span>|
|<span data-ttu-id="c2395-187">连接</span><span class="sxs-lookup"><span data-stu-id="c2395-187">connectionType</span></span>|[<span data-ttu-id="c2395-188">windows10VpnConnectionType</span><span class="sxs-lookup"><span data-stu-id="c2395-188">windows10VpnConnectionType</span></span>](../resources/intune-deviceconfig-windows10vpnconnectiontype.md)|<span data-ttu-id="c2395-189">连接类型。</span><span class="sxs-lookup"><span data-stu-id="c2395-189">Connection type.</span></span> <span data-ttu-id="c2395-190">可取值为：`pulseSecure`、`f5EdgeClient`、`dellSonicWallMobileConnect`、`checkPointCapsuleVpn`、`automatic`、`ikEv2`、`l2tp`、`pptp`、`citrix`、`paloAltoGlobalProtect`。</span><span class="sxs-lookup"><span data-stu-id="c2395-190">Possible values are: `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `automatic`, `ikEv2`, `l2tp`, `pptp`, `citrix`, `paloAltoGlobalProtect`.</span></span>|
|<span data-ttu-id="c2395-191">enableSplitTunneling</span><span class="sxs-lookup"><span data-stu-id="c2395-191">enableSplitTunneling</span></span>|<span data-ttu-id="c2395-192">布尔</span><span class="sxs-lookup"><span data-stu-id="c2395-192">Boolean</span></span>|<span data-ttu-id="c2395-193">启用拆分隧道。</span><span class="sxs-lookup"><span data-stu-id="c2395-193">Enable split tunneling.</span></span>|
|<span data-ttu-id="c2395-194">enableAlwaysOn</span><span class="sxs-lookup"><span data-stu-id="c2395-194">enableAlwaysOn</span></span>|<span data-ttu-id="c2395-195">布尔</span><span class="sxs-lookup"><span data-stu-id="c2395-195">Boolean</span></span>|<span data-ttu-id="c2395-196">启用 Always On 模式。</span><span class="sxs-lookup"><span data-stu-id="c2395-196">Enable Always On mode.</span></span>|
|<span data-ttu-id="c2395-197">enableDeviceTunnel</span><span class="sxs-lookup"><span data-stu-id="c2395-197">enableDeviceTunnel</span></span>|<span data-ttu-id="c2395-198">布尔</span><span class="sxs-lookup"><span data-stu-id="c2395-198">Boolean</span></span>|<span data-ttu-id="c2395-199">启用设备隧道。</span><span class="sxs-lookup"><span data-stu-id="c2395-199">Enable device tunnel.</span></span>|
|<span data-ttu-id="c2395-200">enableDnsRegistration</span><span class="sxs-lookup"><span data-stu-id="c2395-200">enableDnsRegistration</span></span>|<span data-ttu-id="c2395-201">布尔</span><span class="sxs-lookup"><span data-stu-id="c2395-201">Boolean</span></span>|<span data-ttu-id="c2395-202">启用内部 DNS 注册的 IP 地址。</span><span class="sxs-lookup"><span data-stu-id="c2395-202">Enable IP address registration with internal DNS.</span></span>|
|<span data-ttu-id="c2395-203">dnsSuffixes</span><span class="sxs-lookup"><span data-stu-id="c2395-203">dnsSuffixes</span></span>|<span data-ttu-id="c2395-204">String 集合</span><span class="sxs-lookup"><span data-stu-id="c2395-204">String collection</span></span>|<span data-ttu-id="c2395-205">指定要向 DNS 搜索列表正确路由短名称添加 DNS 后缀。</span><span class="sxs-lookup"><span data-stu-id="c2395-205">Specify DNS suffixes to add to the DNS search list to properly route short names.</span></span>|
|<span data-ttu-id="c2395-206">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="c2395-206">authenticationMethod</span></span>|[<span data-ttu-id="c2395-207">windows10VpnAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="c2395-207">windows10VpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-windows10vpnauthenticationmethod.md)|<span data-ttu-id="c2395-208">身份验证方法。</span><span class="sxs-lookup"><span data-stu-id="c2395-208">Authentication method.</span></span> <span data-ttu-id="c2395-209">可取值为：`certificate`、`usernameAndPassword`、`customEapXml`。</span><span class="sxs-lookup"><span data-stu-id="c2395-209">Possible values are: `certificate`, `usernameAndPassword`, `customEapXml`.</span></span>|
|<span data-ttu-id="c2395-210">rememberUserCredentials</span><span class="sxs-lookup"><span data-stu-id="c2395-210">rememberUserCredentials</span></span>|<span data-ttu-id="c2395-211">布尔</span><span class="sxs-lookup"><span data-stu-id="c2395-211">Boolean</span></span>|<span data-ttu-id="c2395-212">请记住用户凭据。</span><span class="sxs-lookup"><span data-stu-id="c2395-212">Remember user credentials.</span></span>|
|<span data-ttu-id="c2395-213">enableConditionalAccess</span><span class="sxs-lookup"><span data-stu-id="c2395-213">enableConditionalAccess</span></span>|<span data-ttu-id="c2395-214">布尔</span><span class="sxs-lookup"><span data-stu-id="c2395-214">Boolean</span></span>|<span data-ttu-id="c2395-215">启用条件的访问。</span><span class="sxs-lookup"><span data-stu-id="c2395-215">Enable conditional access.</span></span>|
|<span data-ttu-id="c2395-216">enableSingleSignOnWithAlternateCertificate</span><span class="sxs-lookup"><span data-stu-id="c2395-216">enableSingleSignOnWithAlternateCertificate</span></span>|<span data-ttu-id="c2395-217">布尔</span><span class="sxs-lookup"><span data-stu-id="c2395-217">Boolean</span></span>|<span data-ttu-id="c2395-218">启用单一登录 (SSO) 与备用证书。</span><span class="sxs-lookup"><span data-stu-id="c2395-218">Enable single sign-on (SSO) with alternate certificate.</span></span>|
|<span data-ttu-id="c2395-219">singleSignOnEku</span><span class="sxs-lookup"><span data-stu-id="c2395-219">singleSignOnEku</span></span>|[<span data-ttu-id="c2395-220">extendedKeyUsage</span><span class="sxs-lookup"><span data-stu-id="c2395-220">extendedKeyUsage</span></span>](../resources/intune-deviceconfig-extendedkeyusage.md)|<span data-ttu-id="c2395-221">单一登录扩展密钥用法 (EKU)。</span><span class="sxs-lookup"><span data-stu-id="c2395-221">Single sign-on Extended Key Usage (EKU).</span></span>|
|<span data-ttu-id="c2395-222">singleSignOnIssuerHash</span><span class="sxs-lookup"><span data-stu-id="c2395-222">singleSignOnIssuerHash</span></span>|<span data-ttu-id="c2395-223">字符串</span><span class="sxs-lookup"><span data-stu-id="c2395-223">String</span></span>|<span data-ttu-id="c2395-224">单一登录颁发者哈希值。</span><span class="sxs-lookup"><span data-stu-id="c2395-224">Single sign-on issuer hash.</span></span>|
|<span data-ttu-id="c2395-225">eapXml</span><span class="sxs-lookup"><span data-stu-id="c2395-225">eapXml</span></span>|<span data-ttu-id="c2395-226">Binary</span><span class="sxs-lookup"><span data-stu-id="c2395-226">Binary</span></span>|<span data-ttu-id="c2395-227">可扩展的身份验证协议 (EAP) XML。</span><span class="sxs-lookup"><span data-stu-id="c2395-227">Extensible Authentication Protocol (EAP) XML.</span></span> <span data-ttu-id="c2395-228">（UTF8 编码的字节数组）</span><span class="sxs-lookup"><span data-stu-id="c2395-228">(UTF8 encoded byte array)</span></span>|
|<span data-ttu-id="c2395-229">代理服务器</span><span class="sxs-lookup"><span data-stu-id="c2395-229">proxyServer</span></span>|[<span data-ttu-id="c2395-230">windows10VpnProxyServer</span><span class="sxs-lookup"><span data-stu-id="c2395-230">windows10VpnProxyServer</span></span>](../resources/intune-deviceconfig-windows10vpnproxyserver.md)|<span data-ttu-id="c2395-231">代理服务器。</span><span class="sxs-lookup"><span data-stu-id="c2395-231">Proxy Server.</span></span>|
|<span data-ttu-id="c2395-232">associatedApps</span><span class="sxs-lookup"><span data-stu-id="c2395-232">associatedApps</span></span>|<span data-ttu-id="c2395-233">[windows10AssociatedApps](../resources/intune-deviceconfig-windows10associatedapps.md)集合</span><span class="sxs-lookup"><span data-stu-id="c2395-233">[windows10AssociatedApps](../resources/intune-deviceconfig-windows10associatedapps.md) collection</span></span>|<span data-ttu-id="c2395-234">关联的应用程序。</span><span class="sxs-lookup"><span data-stu-id="c2395-234">Associated Apps.</span></span> <span data-ttu-id="c2395-235">该集合最多可包含 10000 个元素。</span><span class="sxs-lookup"><span data-stu-id="c2395-235">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="c2395-236">onlyAssociatedAppsCanUseConnection</span><span class="sxs-lookup"><span data-stu-id="c2395-236">onlyAssociatedAppsCanUseConnection</span></span>|<span data-ttu-id="c2395-237">布尔</span><span class="sxs-lookup"><span data-stu-id="c2395-237">Boolean</span></span>|<span data-ttu-id="c2395-238">仅关联的应用程序可以使用 (每个应用程序 VPN) 连接。</span><span class="sxs-lookup"><span data-stu-id="c2395-238">Only associated Apps can use connection (per-app VPN).</span></span>|
|<span data-ttu-id="c2395-239">windowsInformationProtectionDomain</span><span class="sxs-lookup"><span data-stu-id="c2395-239">windowsInformationProtectionDomain</span></span>|<span data-ttu-id="c2395-240">字符串</span><span class="sxs-lookup"><span data-stu-id="c2395-240">String</span></span>|<span data-ttu-id="c2395-241">要与此连接关联的 Windows 的信息保护 (WIP) 域。</span><span class="sxs-lookup"><span data-stu-id="c2395-241">Windows Information Protection (WIP) domain to associate with this connection.</span></span>|
|<span data-ttu-id="c2395-242">trafficRules</span><span class="sxs-lookup"><span data-stu-id="c2395-242">trafficRules</span></span>|<span data-ttu-id="c2395-243">[vpnTrafficRule](../resources/intune-deviceconfig-vpntrafficrule.md)集合</span><span class="sxs-lookup"><span data-stu-id="c2395-243">[vpnTrafficRule](../resources/intune-deviceconfig-vpntrafficrule.md) collection</span></span>|<span data-ttu-id="c2395-244">流量的规则。</span><span class="sxs-lookup"><span data-stu-id="c2395-244">Traffic rules.</span></span> <span data-ttu-id="c2395-245">该集合最多可包含 1000 个元素。</span><span class="sxs-lookup"><span data-stu-id="c2395-245">This collection can contain a maximum of 1000 elements.</span></span>|
|<span data-ttu-id="c2395-246">路由</span><span class="sxs-lookup"><span data-stu-id="c2395-246">routes</span></span>|<span data-ttu-id="c2395-247">[vpnRoute](../resources/intune-deviceconfig-vpnroute.md)集合</span><span class="sxs-lookup"><span data-stu-id="c2395-247">[vpnRoute](../resources/intune-deviceconfig-vpnroute.md) collection</span></span>|<span data-ttu-id="c2395-248">（可选第三方提供程序） 的路由。</span><span class="sxs-lookup"><span data-stu-id="c2395-248">Routes (optional for third-party providers).</span></span> <span data-ttu-id="c2395-249">该集合最多可包含 1000 个元素。</span><span class="sxs-lookup"><span data-stu-id="c2395-249">This collection can contain a maximum of 1000 elements.</span></span>|
|<span data-ttu-id="c2395-250">dnsRules</span><span class="sxs-lookup"><span data-stu-id="c2395-250">dnsRules</span></span>|<span data-ttu-id="c2395-251">[vpnDnsRule](../resources/intune-deviceconfig-vpndnsrule.md)集合</span><span class="sxs-lookup"><span data-stu-id="c2395-251">[vpnDnsRule](../resources/intune-deviceconfig-vpndnsrule.md) collection</span></span>|<span data-ttu-id="c2395-252">DNS 规则。</span><span class="sxs-lookup"><span data-stu-id="c2395-252">DNS rules.</span></span> <span data-ttu-id="c2395-253">该集合最多可包含 1000 个元素。</span><span class="sxs-lookup"><span data-stu-id="c2395-253">This collection can contain a maximum of 1000 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c2395-254">关系</span><span class="sxs-lookup"><span data-stu-id="c2395-254">Relationships</span></span>
|<span data-ttu-id="c2395-255">关系</span><span class="sxs-lookup"><span data-stu-id="c2395-255">Relationship</span></span>|<span data-ttu-id="c2395-256">类型</span><span class="sxs-lookup"><span data-stu-id="c2395-256">Type</span></span>|<span data-ttu-id="c2395-257">Description</span><span class="sxs-lookup"><span data-stu-id="c2395-257">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c2395-258">groupAssignments</span><span class="sxs-lookup"><span data-stu-id="c2395-258">groupAssignments</span></span>|<span data-ttu-id="c2395-259">[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)集合</span><span class="sxs-lookup"><span data-stu-id="c2395-259">[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) collection</span></span>|<span data-ttu-id="c2395-260">设备配置文件的组分配列表。</span><span class="sxs-lookup"><span data-stu-id="c2395-260">The list of group assignments for the device configuration profile.</span></span> <span data-ttu-id="c2395-261">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c2395-261">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c2395-262">assignments</span><span class="sxs-lookup"><span data-stu-id="c2395-262">assignments</span></span>|<span data-ttu-id="c2395-263">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="c2395-263">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection</span></span>|<span data-ttu-id="c2395-264">设备配置文件的分配列表。</span><span class="sxs-lookup"><span data-stu-id="c2395-264">The list of assignments for the device configuration profile.</span></span> <span data-ttu-id="c2395-265">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c2395-265">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c2395-266">deviceStatuses</span><span class="sxs-lookup"><span data-stu-id="c2395-266">deviceStatuses</span></span>|<span data-ttu-id="c2395-267">[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) 集合</span><span class="sxs-lookup"><span data-stu-id="c2395-267">[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) collection</span></span>|<span data-ttu-id="c2395-268">按设备的设备配置安装状态。</span><span class="sxs-lookup"><span data-stu-id="c2395-268">Device configuration installation status by device.</span></span> <span data-ttu-id="c2395-269">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c2395-269">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c2395-270">userStatuses</span><span class="sxs-lookup"><span data-stu-id="c2395-270">userStatuses</span></span>|<span data-ttu-id="c2395-271">[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) 集合</span><span class="sxs-lookup"><span data-stu-id="c2395-271">[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) collection</span></span>|<span data-ttu-id="c2395-272">用户的设备配置安装状态。</span><span class="sxs-lookup"><span data-stu-id="c2395-272">Device configuration installation status by user.</span></span> <span data-ttu-id="c2395-273">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c2395-273">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c2395-274">deviceStatusOverview</span><span class="sxs-lookup"><span data-stu-id="c2395-274">deviceStatusOverview</span></span>|[<span data-ttu-id="c2395-275">deviceConfigurationDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="c2395-275">deviceConfigurationDeviceOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|<span data-ttu-id="c2395-276">设备配置设备状态概述 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c2395-276">Device Configuration devices status overview Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c2395-277">userStatusOverview</span><span class="sxs-lookup"><span data-stu-id="c2395-277">userStatusOverview</span></span>|[<span data-ttu-id="c2395-278">deviceConfigurationUserOverview</span><span class="sxs-lookup"><span data-stu-id="c2395-278">deviceConfigurationUserOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|<span data-ttu-id="c2395-279">设备配置用户状态概述 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c2395-279">Device Configuration users status overview Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c2395-280">deviceSettingStateSummaries</span><span class="sxs-lookup"><span data-stu-id="c2395-280">deviceSettingStateSummaries</span></span>|<span data-ttu-id="c2395-281">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) 集合</span><span class="sxs-lookup"><span data-stu-id="c2395-281">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) collection</span></span>|<span data-ttu-id="c2395-282">设备配置设置状态设备摘要 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c2395-282">Device Configuration Setting State Device Summary Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c2395-283">identityCertificate</span><span class="sxs-lookup"><span data-stu-id="c2395-283">identityCertificate</span></span>|[<span data-ttu-id="c2395-284">windowsCertificateProfileBase</span><span class="sxs-lookup"><span data-stu-id="c2395-284">windowsCertificateProfileBase</span></span>](../resources/intune-deviceconfig-windowscertificateprofilebase.md)|<span data-ttu-id="c2395-285">客户端身份验证证书身份验证方法时的标识证书。</span><span class="sxs-lookup"><span data-stu-id="c2395-285">Identity certificate for client authentication when authentication method is certificate.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c2395-286">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c2395-286">JSON Representation</span></span>
<span data-ttu-id="c2395-287">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c2395-287">Here is a JSON representation of the resource.</span></span>
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
      "proxyServerUri": "String"
    }
  ]
}
```





