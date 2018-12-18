---
title: 更新 windowsPhone81VpnConfiguration
description: 更新 windowsPhone81VpnConfiguration 对象的属性。
author: tfitzmac
ms.openlocfilehash: 5decc13b53ba632dd8ee37134ff245c2e9c18ba2
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27317540"
---
# <a name="update-windowsphone81vpnconfiguration"></a><span data-ttu-id="aa1e9-103">更新 windowsPhone81VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="aa1e9-103">Update windowsPhone81VpnConfiguration</span></span>

> <span data-ttu-id="aa1e9-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="aa1e9-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="aa1e9-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="aa1e9-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="aa1e9-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="aa1e9-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="aa1e9-107">更新[windowsPhone81VpnConfiguration](../resources/intune-deviceconfig-windowsphone81vpnconfiguration.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="aa1e9-107">Update the properties of a [windowsPhone81VpnConfiguration](../resources/intune-deviceconfig-windowsphone81vpnconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="aa1e9-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="aa1e9-108">Prerequisites</span></span>
<span data-ttu-id="aa1e9-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="aa1e9-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="aa1e9-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="aa1e9-111">Permission type</span></span>|<span data-ttu-id="aa1e9-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="aa1e9-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="aa1e9-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="aa1e9-113">Delegated (work or school account)</span></span>|<span data-ttu-id="aa1e9-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aa1e9-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="aa1e9-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="aa1e9-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="aa1e9-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="aa1e9-116">Not supported.</span></span>|
|<span data-ttu-id="aa1e9-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="aa1e9-117">Application</span></span>|<span data-ttu-id="aa1e9-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="aa1e9-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="aa1e9-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="aa1e9-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="aa1e9-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="aa1e9-120">Request headers</span></span>
|<span data-ttu-id="aa1e9-121">标头</span><span class="sxs-lookup"><span data-stu-id="aa1e9-121">Header</span></span>|<span data-ttu-id="aa1e9-122">值</span><span class="sxs-lookup"><span data-stu-id="aa1e9-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="aa1e9-123">授权</span><span class="sxs-lookup"><span data-stu-id="aa1e9-123">Authorization</span></span>|<span data-ttu-id="aa1e9-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="aa1e9-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="aa1e9-125">Accept</span><span class="sxs-lookup"><span data-stu-id="aa1e9-125">Accept</span></span>|<span data-ttu-id="aa1e9-126">application/json</span><span class="sxs-lookup"><span data-stu-id="aa1e9-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="aa1e9-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="aa1e9-127">Request body</span></span>
<span data-ttu-id="aa1e9-128">在请求正文中，提供[windowsPhone81VpnConfiguration](../resources/intune-deviceconfig-windowsphone81vpnconfiguration.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="aa1e9-128">In the request body, supply a JSON representation for the [windowsPhone81VpnConfiguration](../resources/intune-deviceconfig-windowsphone81vpnconfiguration.md) object.</span></span>

<span data-ttu-id="aa1e9-129">下表显示时创建[windowsPhone81VpnConfiguration](../resources/intune-deviceconfig-windowsphone81vpnconfiguration.md)所需的属性。</span><span class="sxs-lookup"><span data-stu-id="aa1e9-129">The following table shows the properties that are required when you create the [windowsPhone81VpnConfiguration](../resources/intune-deviceconfig-windowsphone81vpnconfiguration.md).</span></span>

|<span data-ttu-id="aa1e9-130">属性</span><span class="sxs-lookup"><span data-stu-id="aa1e9-130">Property</span></span>|<span data-ttu-id="aa1e9-131">类型</span><span class="sxs-lookup"><span data-stu-id="aa1e9-131">Type</span></span>|<span data-ttu-id="aa1e9-132">说明</span><span class="sxs-lookup"><span data-stu-id="aa1e9-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="aa1e9-133">id</span><span class="sxs-lookup"><span data-stu-id="aa1e9-133">id</span></span>|<span data-ttu-id="aa1e9-134">String</span><span class="sxs-lookup"><span data-stu-id="aa1e9-134">String</span></span>|<span data-ttu-id="aa1e9-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="aa1e9-135">Key of the entity.</span></span> <span data-ttu-id="aa1e9-136">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="aa1e9-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="aa1e9-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="aa1e9-137">lastModifiedDateTime</span></span>|<span data-ttu-id="aa1e9-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="aa1e9-138">DateTimeOffset</span></span>|<span data-ttu-id="aa1e9-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="aa1e9-139">DateTime the object was last modified.</span></span> <span data-ttu-id="aa1e9-140">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="aa1e9-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="aa1e9-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="aa1e9-141">roleScopeTagIds</span></span>|<span data-ttu-id="aa1e9-142">String 集合</span><span class="sxs-lookup"><span data-stu-id="aa1e9-142">String collection</span></span>|<span data-ttu-id="aa1e9-143">此实体实例范围标记的列表。</span><span class="sxs-lookup"><span data-stu-id="aa1e9-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="aa1e9-144">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="aa1e9-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="aa1e9-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="aa1e9-145">supportsScopeTags</span></span>|<span data-ttu-id="aa1e9-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="aa1e9-146">Boolean</span></span>|<span data-ttu-id="aa1e9-147">指示基础的设备配置支持分配的范围标记。</span><span class="sxs-lookup"><span data-stu-id="aa1e9-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="aa1e9-148">此值为 false，并且实体将不会对作用域的用户可见时，不允许将分配给 ScopeTags 属性。</span><span class="sxs-lookup"><span data-stu-id="aa1e9-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="aa1e9-149">这将发生在 Silverlight 中创建的旧策略，并可以解析通过删除并重新创建 Azure 门户中的策略。</span><span class="sxs-lookup"><span data-stu-id="aa1e9-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="aa1e9-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="aa1e9-150">This property is read-only.</span></span> <span data-ttu-id="aa1e9-151">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="aa1e9-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="aa1e9-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="aa1e9-152">createdDateTime</span></span>|<span data-ttu-id="aa1e9-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="aa1e9-153">DateTimeOffset</span></span>|<span data-ttu-id="aa1e9-154">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="aa1e9-154">DateTime the object was created.</span></span> <span data-ttu-id="aa1e9-155">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="aa1e9-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="aa1e9-156">description</span><span class="sxs-lookup"><span data-stu-id="aa1e9-156">description</span></span>|<span data-ttu-id="aa1e9-157">String</span><span class="sxs-lookup"><span data-stu-id="aa1e9-157">String</span></span>|<span data-ttu-id="aa1e9-158">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="aa1e9-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="aa1e9-159">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="aa1e9-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="aa1e9-160">displayName</span><span class="sxs-lookup"><span data-stu-id="aa1e9-160">displayName</span></span>|<span data-ttu-id="aa1e9-161">String</span><span class="sxs-lookup"><span data-stu-id="aa1e9-161">String</span></span>|<span data-ttu-id="aa1e9-162">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="aa1e9-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="aa1e9-163">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="aa1e9-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="aa1e9-164">version</span><span class="sxs-lookup"><span data-stu-id="aa1e9-164">version</span></span>|<span data-ttu-id="aa1e9-165">Int32</span><span class="sxs-lookup"><span data-stu-id="aa1e9-165">Int32</span></span>|<span data-ttu-id="aa1e9-166">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="aa1e9-166">Version of the device configuration.</span></span> <span data-ttu-id="aa1e9-167">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="aa1e9-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="aa1e9-168">connectionName</span><span class="sxs-lookup"><span data-stu-id="aa1e9-168">connectionName</span></span>|<span data-ttu-id="aa1e9-169">字符串</span><span class="sxs-lookup"><span data-stu-id="aa1e9-169">String</span></span>|<span data-ttu-id="aa1e9-170">向用户显示的连接名称。</span><span class="sxs-lookup"><span data-stu-id="aa1e9-170">Connection name displayed to the user.</span></span> <span data-ttu-id="aa1e9-171">继承自[windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="aa1e9-171">Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="aa1e9-172">服务器</span><span class="sxs-lookup"><span data-stu-id="aa1e9-172">servers</span></span>|<span data-ttu-id="aa1e9-173">[vpnServer](../resources/intune-deviceconfig-vpnserver.md)集合</span><span class="sxs-lookup"><span data-stu-id="aa1e9-173">[vpnServer](../resources/intune-deviceconfig-vpnserver.md) collection</span></span>|<span data-ttu-id="aa1e9-174">VPN 服务器的网络上的列表。</span><span class="sxs-lookup"><span data-stu-id="aa1e9-174">List of VPN Servers on the network.</span></span> <span data-ttu-id="aa1e9-175">确保最终用户可以访问这些网络位置。</span><span class="sxs-lookup"><span data-stu-id="aa1e9-175">Make sure end users can access these network locations.</span></span> <span data-ttu-id="aa1e9-176">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="aa1e9-176">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="aa1e9-177">继承自[windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="aa1e9-177">Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="aa1e9-178">customXml</span><span class="sxs-lookup"><span data-stu-id="aa1e9-178">customXml</span></span>|<span data-ttu-id="aa1e9-179">Binary</span><span class="sxs-lookup"><span data-stu-id="aa1e9-179">Binary</span></span>|<span data-ttu-id="aa1e9-180">配置 VPN 连接的自定义 XML 命令。</span><span class="sxs-lookup"><span data-stu-id="aa1e9-180">Custom XML commands that configures the VPN connection.</span></span> <span data-ttu-id="aa1e9-181">（UTF8 编码的字节数组）继承自[windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="aa1e9-181">(UTF8 encoded byte array) Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="aa1e9-182">applyOnlyToWindows81</span><span class="sxs-lookup"><span data-stu-id="aa1e9-182">applyOnlyToWindows81</span></span>|<span data-ttu-id="aa1e9-183">Boolean</span><span class="sxs-lookup"><span data-stu-id="aa1e9-183">Boolean</span></span>|<span data-ttu-id="aa1e9-184">指示此策略是否仅适用于 Windows 8.1 的值。</span><span class="sxs-lookup"><span data-stu-id="aa1e9-184">Value indicating whether this policy only applies to Windows 8.1.</span></span> <span data-ttu-id="aa1e9-185">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="aa1e9-185">This property is read-only.</span></span> <span data-ttu-id="aa1e9-186">继承自[windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="aa1e9-186">Inherited from [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)</span></span>|
|<span data-ttu-id="aa1e9-187">连接</span><span class="sxs-lookup"><span data-stu-id="aa1e9-187">connectionType</span></span>|[<span data-ttu-id="aa1e9-188">windowsVpnConnectionType</span><span class="sxs-lookup"><span data-stu-id="aa1e9-188">windowsVpnConnectionType</span></span>](../resources/intune-deviceconfig-windowsvpnconnectiontype.md)|<span data-ttu-id="aa1e9-189">连接类型。</span><span class="sxs-lookup"><span data-stu-id="aa1e9-189">Connection type.</span></span> <span data-ttu-id="aa1e9-190">继承自[windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)。</span><span class="sxs-lookup"><span data-stu-id="aa1e9-190">Inherited from [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md).</span></span> <span data-ttu-id="aa1e9-191">可取值为：`pulseSecure`、`f5EdgeClient`、`dellSonicWallMobileConnect`、`checkPointCapsuleVpn`。</span><span class="sxs-lookup"><span data-stu-id="aa1e9-191">Possible values are: `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`.</span></span>|
|<span data-ttu-id="aa1e9-192">loginGroupOrDomain</span><span class="sxs-lookup"><span data-stu-id="aa1e9-192">loginGroupOrDomain</span></span>|<span data-ttu-id="aa1e9-193">字符串</span><span class="sxs-lookup"><span data-stu-id="aa1e9-193">String</span></span>|<span data-ttu-id="aa1e9-194">登录组或域时连接类型设置为 Dell 使 SonicWALL Mobile 连接。</span><span class="sxs-lookup"><span data-stu-id="aa1e9-194">Login group or domain when connection type is set to Dell SonicWALL Mobile Connection.</span></span> <span data-ttu-id="aa1e9-195">继承自[windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="aa1e9-195">Inherited from [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)</span></span>|
|<span data-ttu-id="aa1e9-196">enableSplitTunneling</span><span class="sxs-lookup"><span data-stu-id="aa1e9-196">enableSplitTunneling</span></span>|<span data-ttu-id="aa1e9-197">Boolean</span><span class="sxs-lookup"><span data-stu-id="aa1e9-197">Boolean</span></span>|<span data-ttu-id="aa1e9-198">启用拆分隧道的 VPN。</span><span class="sxs-lookup"><span data-stu-id="aa1e9-198">Enable split tunneling for the VPN.</span></span> <span data-ttu-id="aa1e9-199">继承自[windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="aa1e9-199">Inherited from [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)</span></span>|
|<span data-ttu-id="aa1e9-200">代理服务器</span><span class="sxs-lookup"><span data-stu-id="aa1e9-200">proxyServer</span></span>|[<span data-ttu-id="aa1e9-201">windows81VpnProxyServer</span><span class="sxs-lookup"><span data-stu-id="aa1e9-201">windows81VpnProxyServer</span></span>](../resources/intune-deviceconfig-windows81vpnproxyserver.md)|<span data-ttu-id="aa1e9-202">代理服务器。</span><span class="sxs-lookup"><span data-stu-id="aa1e9-202">Proxy Server.</span></span> <span data-ttu-id="aa1e9-203">继承自[windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="aa1e9-203">Inherited from [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)</span></span>|
|<span data-ttu-id="aa1e9-204">bypassVpnOnCompanyWifi</span><span class="sxs-lookup"><span data-stu-id="aa1e9-204">bypassVpnOnCompanyWifi</span></span>|<span data-ttu-id="aa1e9-205">Boolean</span><span class="sxs-lookup"><span data-stu-id="aa1e9-205">Boolean</span></span>|<span data-ttu-id="aa1e9-206">在公司 Wi-fi 绕过 VPN。</span><span class="sxs-lookup"><span data-stu-id="aa1e9-206">Bypass VPN on company Wi-Fi.</span></span>|
|<span data-ttu-id="aa1e9-207">bypassVpnOnHomeWifi</span><span class="sxs-lookup"><span data-stu-id="aa1e9-207">bypassVpnOnHomeWifi</span></span>|<span data-ttu-id="aa1e9-208">Boolean</span><span class="sxs-lookup"><span data-stu-id="aa1e9-208">Boolean</span></span>|<span data-ttu-id="aa1e9-209">绕过 Wi-fi 主页上的 VPN。</span><span class="sxs-lookup"><span data-stu-id="aa1e9-209">Bypass VPN on home Wi-Fi.</span></span>|
|<span data-ttu-id="aa1e9-210">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="aa1e9-210">authenticationMethod</span></span>|[<span data-ttu-id="aa1e9-211">vpnAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="aa1e9-211">vpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-vpnauthenticationmethod.md)|<span data-ttu-id="aa1e9-212">身份验证方法。</span><span class="sxs-lookup"><span data-stu-id="aa1e9-212">Authentication method.</span></span> <span data-ttu-id="aa1e9-213">可取值为：`certificate`、`usernameAndPassword`。</span><span class="sxs-lookup"><span data-stu-id="aa1e9-213">Possible values are: `certificate`, `usernameAndPassword`.</span></span>|
|<span data-ttu-id="aa1e9-214">rememberUserCredentials</span><span class="sxs-lookup"><span data-stu-id="aa1e9-214">rememberUserCredentials</span></span>|<span data-ttu-id="aa1e9-215">Boolean</span><span class="sxs-lookup"><span data-stu-id="aa1e9-215">Boolean</span></span>|<span data-ttu-id="aa1e9-216">请记住用户凭据。</span><span class="sxs-lookup"><span data-stu-id="aa1e9-216">Remember user credentials.</span></span>|
|<span data-ttu-id="aa1e9-217">dnsSuffixSearchList</span><span class="sxs-lookup"><span data-stu-id="aa1e9-217">dnsSuffixSearchList</span></span>|<span data-ttu-id="aa1e9-218">String 集合</span><span class="sxs-lookup"><span data-stu-id="aa1e9-218">String collection</span></span>|<span data-ttu-id="aa1e9-219">DNS 后缀搜索列表。</span><span class="sxs-lookup"><span data-stu-id="aa1e9-219">DNS suffix search list.</span></span>|



## <a name="response"></a><span data-ttu-id="aa1e9-220">响应</span><span class="sxs-lookup"><span data-stu-id="aa1e9-220">Response</span></span>
<span data-ttu-id="aa1e9-221">如果成功，此方法返回`200 OK`响应代码和响应正文中的更新的[windowsPhone81VpnConfiguration](../resources/intune-deviceconfig-windowsphone81vpnconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="aa1e9-221">If successful, this method returns a `200 OK` response code and an updated [windowsPhone81VpnConfiguration](../resources/intune-deviceconfig-windowsphone81vpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="aa1e9-222">示例</span><span class="sxs-lookup"><span data-stu-id="aa1e9-222">Example</span></span>
### <a name="request"></a><span data-ttu-id="aa1e9-223">请求</span><span class="sxs-lookup"><span data-stu-id="aa1e9-223">Request</span></span>
<span data-ttu-id="aa1e9-224">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="aa1e9-224">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1238

{
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

### <a name="response"></a><span data-ttu-id="aa1e9-225">响应</span><span class="sxs-lookup"><span data-stu-id="aa1e9-225">Response</span></span>
<span data-ttu-id="aa1e9-p120">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="aa1e9-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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





