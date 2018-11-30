---
title: 创建 windowsPhone81VpnConfiguration
description: 创建新的 windowsPhone81VpnConfiguration 对象。
ms.openlocfilehash: 8b4fb7ad9118ae91712cfd74ca78e7654e5db601
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27048716"
---
# <a name="create-windowsphone81vpnconfiguration"></a><span data-ttu-id="6890c-103">创建 windowsPhone81VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="6890c-103">Create windowsPhone81VpnConfiguration</span></span>

> <span data-ttu-id="6890c-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="6890c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6890c-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="6890c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="6890c-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="6890c-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6890c-107">创建新的[windowsPhone81VpnConfiguration](../resources/intune-deviceconfig-windowsphone81vpnconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="6890c-107">Create a new [windowsPhone81VpnConfiguration](../resources/intune-deviceconfig-windowsphone81vpnconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="6890c-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="6890c-108">Prerequisites</span></span>
<span data-ttu-id="6890c-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="6890c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6890c-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="6890c-111">Permission type</span></span>|<span data-ttu-id="6890c-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="6890c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6890c-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6890c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6890c-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6890c-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="6890c-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6890c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6890c-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="6890c-116">Not supported.</span></span>|
|<span data-ttu-id="6890c-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="6890c-117">Application</span></span>|<span data-ttu-id="6890c-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="6890c-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6890c-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6890c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="6890c-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="6890c-120">Request headers</span></span>
|<span data-ttu-id="6890c-121">标头</span><span class="sxs-lookup"><span data-stu-id="6890c-121">Header</span></span>|<span data-ttu-id="6890c-122">值</span><span class="sxs-lookup"><span data-stu-id="6890c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6890c-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="6890c-123">Authorization</span></span>|<span data-ttu-id="6890c-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="6890c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6890c-125">Accept</span><span class="sxs-lookup"><span data-stu-id="6890c-125">Accept</span></span>|<span data-ttu-id="6890c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6890c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6890c-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="6890c-127">Request body</span></span>
<span data-ttu-id="6890c-128">在请求正文中，提供 windowsPhone81VpnConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6890c-128">In the request body, supply a JSON representation for the windowsPhone81VpnConfiguration object.</span></span>

<span data-ttu-id="6890c-129">下表显示时创建 windowsPhone81VpnConfiguration 所需的属性。</span><span class="sxs-lookup"><span data-stu-id="6890c-129">The following table shows the properties that are required when you create the windowsPhone81VpnConfiguration.</span></span>

|<span data-ttu-id="6890c-130">属性</span><span class="sxs-lookup"><span data-stu-id="6890c-130">Property</span></span>|<span data-ttu-id="6890c-131">类型</span><span class="sxs-lookup"><span data-stu-id="6890c-131">Type</span></span>|<span data-ttu-id="6890c-132">说明</span><span class="sxs-lookup"><span data-stu-id="6890c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6890c-133">id</span><span class="sxs-lookup"><span data-stu-id="6890c-133">id</span></span>|<span data-ttu-id="6890c-134">String</span><span class="sxs-lookup"><span data-stu-id="6890c-134">String</span></span>|<span data-ttu-id="6890c-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="6890c-135">Key of the entity.</span></span> <span data-ttu-id="6890c-136">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6890c-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6890c-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6890c-137">lastModifiedDateTime</span></span>|<span data-ttu-id="6890c-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6890c-138">DateTimeOffset</span></span>|<span data-ttu-id="6890c-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="6890c-139">DateTime the object was last modified.</span></span> <span data-ttu-id="6890c-140">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6890c-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6890c-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="6890c-141">roleScopeTagIds</span></span>|<span data-ttu-id="6890c-142">String 集合</span><span class="sxs-lookup"><span data-stu-id="6890c-142">String collection</span></span>|<span data-ttu-id="6890c-143">此实体实例范围标记的列表。</span><span class="sxs-lookup"><span data-stu-id="6890c-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="6890c-144">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6890c-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6890c-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="6890c-145">supportsScopeTags</span></span>|<span data-ttu-id="6890c-146">布尔</span><span class="sxs-lookup"><span data-stu-id="6890c-146">Boolean</span></span>|<span data-ttu-id="6890c-147">指示基础的设备配置支持分配的范围标记。</span><span class="sxs-lookup"><span data-stu-id="6890c-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="6890c-148">此值为 false，并且实体将不会对作用域的用户可见时，不允许将分配给 ScopeTags 属性。</span><span class="sxs-lookup"><span data-stu-id="6890c-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="6890c-149">这将发生在 Silverlight 中创建的旧策略，并可以解析通过删除并重新创建 Azure 门户中的策略。</span><span class="sxs-lookup"><span data-stu-id="6890c-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="6890c-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="6890c-150">This property is read-only.</span></span> <span data-ttu-id="6890c-151">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6890c-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6890c-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6890c-152">createdDateTime</span></span>|<span data-ttu-id="6890c-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6890c-153">DateTimeOffset</span></span>|<span data-ttu-id="6890c-154">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="6890c-154">DateTime the object was created.</span></span> <span data-ttu-id="6890c-155">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6890c-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6890c-156">description</span><span class="sxs-lookup"><span data-stu-id="6890c-156">description</span></span>|<span data-ttu-id="6890c-157">String</span><span class="sxs-lookup"><span data-stu-id="6890c-157">String</span></span>|<span data-ttu-id="6890c-158">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="6890c-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="6890c-159">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6890c-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6890c-160">displayName</span><span class="sxs-lookup"><span data-stu-id="6890c-160">displayName</span></span>|<span data-ttu-id="6890c-161">String</span><span class="sxs-lookup"><span data-stu-id="6890c-161">String</span></span>|<span data-ttu-id="6890c-162">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="6890c-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="6890c-163">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6890c-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6890c-164">version</span><span class="sxs-lookup"><span data-stu-id="6890c-164">version</span></span>|<span data-ttu-id="6890c-165">Int32</span><span class="sxs-lookup"><span data-stu-id="6890c-165">Int32</span></span>|<span data-ttu-id="6890c-166">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="6890c-166">Version of the device configuration.</span></span> <span data-ttu-id="6890c-167">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6890c-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6890c-168">connectionName</span><span class="sxs-lookup"><span data-stu-id="6890c-168">connectionName</span></span>|<span data-ttu-id="6890c-169">字符串</span><span class="sxs-lookup"><span data-stu-id="6890c-169">String</span></span>|<span data-ttu-id="6890c-170">向用户显示的连接名称。</span><span class="sxs-lookup"><span data-stu-id="6890c-170">Connection name displayed to the user.</span></span> <span data-ttu-id="6890c-171">继承自[windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6890c-171">Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="6890c-172">服务器</span><span class="sxs-lookup"><span data-stu-id="6890c-172">servers</span></span>|<span data-ttu-id="6890c-173">[vpnServer](../resources/intune-deviceconfig-vpnserver.md)集合</span><span class="sxs-lookup"><span data-stu-id="6890c-173">[vpnServer](../resources/intune-deviceconfig-vpnserver.md) collection</span></span>|<span data-ttu-id="6890c-174">VPN 服务器的网络上的列表。</span><span class="sxs-lookup"><span data-stu-id="6890c-174">List of VPN Servers on the network.</span></span> <span data-ttu-id="6890c-175">确保最终用户可以访问这些网络位置。</span><span class="sxs-lookup"><span data-stu-id="6890c-175">Make sure end users can access these network locations.</span></span> <span data-ttu-id="6890c-176">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="6890c-176">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="6890c-177">继承自[windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6890c-177">Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="6890c-178">customXml</span><span class="sxs-lookup"><span data-stu-id="6890c-178">customXml</span></span>|<span data-ttu-id="6890c-179">二进制数</span><span class="sxs-lookup"><span data-stu-id="6890c-179">Binary</span></span>|<span data-ttu-id="6890c-180">配置 VPN 连接的自定义 XML 命令。</span><span class="sxs-lookup"><span data-stu-id="6890c-180">Custom XML commands that configures the VPN connection.</span></span> <span data-ttu-id="6890c-181">（UTF8 编码的字节数组）继承自[windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6890c-181">(UTF8 encoded byte array) Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="6890c-182">applyOnlyToWindows81</span><span class="sxs-lookup"><span data-stu-id="6890c-182">applyOnlyToWindows81</span></span>|<span data-ttu-id="6890c-183">Boolean</span><span class="sxs-lookup"><span data-stu-id="6890c-183">Boolean</span></span>|<span data-ttu-id="6890c-184">指示此策略是否仅适用于 Windows 8.1 的值。</span><span class="sxs-lookup"><span data-stu-id="6890c-184">Value indicating whether this policy only applies to Windows 8.1.</span></span> <span data-ttu-id="6890c-185">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="6890c-185">This property is read-only.</span></span> <span data-ttu-id="6890c-186">继承自[windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6890c-186">Inherited from [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)</span></span>|
|<span data-ttu-id="6890c-187">连接</span><span class="sxs-lookup"><span data-stu-id="6890c-187">connectionType</span></span>|[<span data-ttu-id="6890c-188">windowsVpnConnectionType</span><span class="sxs-lookup"><span data-stu-id="6890c-188">windowsVpnConnectionType</span></span>](../resources/intune-deviceconfig-windowsvpnconnectiontype.md)|<span data-ttu-id="6890c-189">连接类型。</span><span class="sxs-lookup"><span data-stu-id="6890c-189">Connection type.</span></span> <span data-ttu-id="6890c-190">继承自[windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)。</span><span class="sxs-lookup"><span data-stu-id="6890c-190">Inherited from [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md).</span></span> <span data-ttu-id="6890c-191">可取值为：`pulseSecure`、`f5EdgeClient`、`dellSonicWallMobileConnect`、`checkPointCapsuleVpn`。</span><span class="sxs-lookup"><span data-stu-id="6890c-191">Possible values are: `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`.</span></span>|
|<span data-ttu-id="6890c-192">loginGroupOrDomain</span><span class="sxs-lookup"><span data-stu-id="6890c-192">loginGroupOrDomain</span></span>|<span data-ttu-id="6890c-193">字符串</span><span class="sxs-lookup"><span data-stu-id="6890c-193">String</span></span>|<span data-ttu-id="6890c-194">登录组或域时连接类型设置为 Dell 使 SonicWALL Mobile 连接。</span><span class="sxs-lookup"><span data-stu-id="6890c-194">Login group or domain when connection type is set to Dell SonicWALL Mobile Connection.</span></span> <span data-ttu-id="6890c-195">继承自[windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6890c-195">Inherited from [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)</span></span>|
|<span data-ttu-id="6890c-196">enableSplitTunneling</span><span class="sxs-lookup"><span data-stu-id="6890c-196">enableSplitTunneling</span></span>|<span data-ttu-id="6890c-197">布尔</span><span class="sxs-lookup"><span data-stu-id="6890c-197">Boolean</span></span>|<span data-ttu-id="6890c-198">启用拆分隧道的 VPN。</span><span class="sxs-lookup"><span data-stu-id="6890c-198">Enable split tunneling for the VPN.</span></span> <span data-ttu-id="6890c-199">继承自[windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6890c-199">Inherited from [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)</span></span>|
|<span data-ttu-id="6890c-200">代理服务器</span><span class="sxs-lookup"><span data-stu-id="6890c-200">proxyServer</span></span>|[<span data-ttu-id="6890c-201">windows81VpnProxyServer</span><span class="sxs-lookup"><span data-stu-id="6890c-201">windows81VpnProxyServer</span></span>](../resources/intune-deviceconfig-windows81vpnproxyserver.md)|<span data-ttu-id="6890c-202">代理服务器。</span><span class="sxs-lookup"><span data-stu-id="6890c-202">Proxy Server.</span></span> <span data-ttu-id="6890c-203">继承自[windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6890c-203">Inherited from [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)</span></span>|
|<span data-ttu-id="6890c-204">bypassVpnOnCompanyWifi</span><span class="sxs-lookup"><span data-stu-id="6890c-204">bypassVpnOnCompanyWifi</span></span>|<span data-ttu-id="6890c-205">布尔</span><span class="sxs-lookup"><span data-stu-id="6890c-205">Boolean</span></span>|<span data-ttu-id="6890c-206">在公司 Wi-fi 绕过 VPN。</span><span class="sxs-lookup"><span data-stu-id="6890c-206">Bypass VPN on company Wi-Fi.</span></span>|
|<span data-ttu-id="6890c-207">bypassVpnOnHomeWifi</span><span class="sxs-lookup"><span data-stu-id="6890c-207">bypassVpnOnHomeWifi</span></span>|<span data-ttu-id="6890c-208">布尔</span><span class="sxs-lookup"><span data-stu-id="6890c-208">Boolean</span></span>|<span data-ttu-id="6890c-209">绕过 Wi-fi 主页上的 VPN。</span><span class="sxs-lookup"><span data-stu-id="6890c-209">Bypass VPN on home Wi-Fi.</span></span>|
|<span data-ttu-id="6890c-210">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="6890c-210">authenticationMethod</span></span>|[<span data-ttu-id="6890c-211">vpnAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="6890c-211">vpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-vpnauthenticationmethod.md)|<span data-ttu-id="6890c-212">身份验证方法。</span><span class="sxs-lookup"><span data-stu-id="6890c-212">Authentication method.</span></span> <span data-ttu-id="6890c-213">可取值为：`certificate`、`usernameAndPassword`。</span><span class="sxs-lookup"><span data-stu-id="6890c-213">Possible values are: `certificate`, `usernameAndPassword`.</span></span>|
|<span data-ttu-id="6890c-214">rememberUserCredentials</span><span class="sxs-lookup"><span data-stu-id="6890c-214">rememberUserCredentials</span></span>|<span data-ttu-id="6890c-215">布尔</span><span class="sxs-lookup"><span data-stu-id="6890c-215">Boolean</span></span>|<span data-ttu-id="6890c-216">请记住用户凭据。</span><span class="sxs-lookup"><span data-stu-id="6890c-216">Remember user credentials.</span></span>|
|<span data-ttu-id="6890c-217">dnsSuffixSearchList</span><span class="sxs-lookup"><span data-stu-id="6890c-217">dnsSuffixSearchList</span></span>|<span data-ttu-id="6890c-218">String 集合</span><span class="sxs-lookup"><span data-stu-id="6890c-218">String collection</span></span>|<span data-ttu-id="6890c-219">DNS 后缀搜索列表。</span><span class="sxs-lookup"><span data-stu-id="6890c-219">DNS suffix search list.</span></span>|



## <a name="response"></a><span data-ttu-id="6890c-220">响应</span><span class="sxs-lookup"><span data-stu-id="6890c-220">Response</span></span>
<span data-ttu-id="6890c-221">如果成功，此方法返回`201 Created`响应代码和响应正文中的[windowsPhone81VpnConfiguration](../resources/intune-deviceconfig-windowsphone81vpnconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="6890c-221">If successful, this method returns a `201 Created` response code and a [windowsPhone81VpnConfiguration](../resources/intune-deviceconfig-windowsphone81vpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6890c-222">示例</span><span class="sxs-lookup"><span data-stu-id="6890c-222">Example</span></span>
### <a name="request"></a><span data-ttu-id="6890c-223">请求</span><span class="sxs-lookup"><span data-stu-id="6890c-223">Request</span></span>
<span data-ttu-id="6890c-224">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="6890c-224">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1307

{
  "@odata.type": "#microsoft.graph.windowsPhone81VpnConfiguration",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "connectionName": "Connection Name value",
  "servers": [
    {
      "@odata.type": "microsoft.graph.vpnServer",
      "description": "Description value",
      "address": "Address value",
      "isDefaultServer": true
    }
  ],
  "customXml": "Y3VzdG9tWG1s",
  "applyOnlyToWindows81": true,
  "connectionType": "f5EdgeClient",
  "loginGroupOrDomain": "Login Group Or Domain value",
  "enableSplitTunneling": true,
  "proxyServer": {
    "@odata.type": "microsoft.graph.windows81VpnProxyServer",
    "automaticConfigurationScriptUrl": "https://example.com/automaticConfigurationScriptUrl/",
    "address": "Address value",
    "port": 4,
    "automaticallyDetectProxySettings": true,
    "bypassProxyServerForLocalAddress": true
  },
  "bypassVpnOnCompanyWifi": true,
  "bypassVpnOnHomeWifi": true,
  "authenticationMethod": "usernameAndPassword",
  "rememberUserCredentials": true,
  "dnsSuffixSearchList": [
    "Dns Suffix Search List value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="6890c-225">响应</span><span class="sxs-lookup"><span data-stu-id="6890c-225">Response</span></span>
<span data-ttu-id="6890c-p120">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="6890c-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1415

{
  "@odata.type": "#microsoft.graph.windowsPhone81VpnConfiguration",
  "id": "7cecc0db-c0db-7cec-dbc0-ec7cdbc0ec7c",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "connectionName": "Connection Name value",
  "servers": [
    {
      "@odata.type": "microsoft.graph.vpnServer",
      "description": "Description value",
      "address": "Address value",
      "isDefaultServer": true
    }
  ],
  "customXml": "Y3VzdG9tWG1s",
  "applyOnlyToWindows81": true,
  "connectionType": "f5EdgeClient",
  "loginGroupOrDomain": "Login Group Or Domain value",
  "enableSplitTunneling": true,
  "proxyServer": {
    "@odata.type": "microsoft.graph.windows81VpnProxyServer",
    "automaticConfigurationScriptUrl": "https://example.com/automaticConfigurationScriptUrl/",
    "address": "Address value",
    "port": 4,
    "automaticallyDetectProxySettings": true,
    "bypassProxyServerForLocalAddress": true
  },
  "bypassVpnOnCompanyWifi": true,
  "bypassVpnOnHomeWifi": true,
  "authenticationMethod": "usernameAndPassword",
  "rememberUserCredentials": true,
  "dnsSuffixSearchList": [
    "Dns Suffix Search List value"
  ]
}
```





