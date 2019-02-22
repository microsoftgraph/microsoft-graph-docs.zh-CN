---
title: 更新 windowsPhone81VpnConfiguration
description: 更新 windowsPhone81VpnConfiguration 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c12b314b2b7971cd0f85d0ef7908fde7c1181af6
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30163516"
---
# <a name="update-windowsphone81vpnconfiguration"></a><span data-ttu-id="4ed38-103">更新 windowsPhone81VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="4ed38-103">Update windowsPhone81VpnConfiguration</span></span>

> <span data-ttu-id="4ed38-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="4ed38-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4ed38-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="4ed38-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4ed38-106">更新[windowsPhone81VpnConfiguration](../resources/intune-deviceconfig-windowsphone81vpnconfiguration.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="4ed38-106">Update the properties of a [windowsPhone81VpnConfiguration](../resources/intune-deviceconfig-windowsphone81vpnconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4ed38-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="4ed38-107">Prerequisites</span></span>
<span data-ttu-id="4ed38-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="4ed38-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="4ed38-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="4ed38-110">Permission type</span></span>|<span data-ttu-id="4ed38-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="4ed38-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4ed38-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4ed38-112">Delegated (work or school account)</span></span>|<span data-ttu-id="4ed38-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4ed38-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="4ed38-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4ed38-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4ed38-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="4ed38-115">Not supported.</span></span>|
|<span data-ttu-id="4ed38-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="4ed38-116">Application</span></span>|<span data-ttu-id="4ed38-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="4ed38-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4ed38-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4ed38-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="4ed38-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="4ed38-119">Request headers</span></span>
|<span data-ttu-id="4ed38-120">标头</span><span class="sxs-lookup"><span data-stu-id="4ed38-120">Header</span></span>|<span data-ttu-id="4ed38-121">值</span><span class="sxs-lookup"><span data-stu-id="4ed38-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4ed38-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="4ed38-122">Authorization</span></span>|<span data-ttu-id="4ed38-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="4ed38-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4ed38-124">Accept</span><span class="sxs-lookup"><span data-stu-id="4ed38-124">Accept</span></span>|<span data-ttu-id="4ed38-125">application/json</span><span class="sxs-lookup"><span data-stu-id="4ed38-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4ed38-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="4ed38-126">Request body</span></span>
<span data-ttu-id="4ed38-127">在请求正文中, 提供[windowsPhone81VpnConfiguration](../resources/intune-deviceconfig-windowsphone81vpnconfiguration.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4ed38-127">In the request body, supply a JSON representation for the [windowsPhone81VpnConfiguration](../resources/intune-deviceconfig-windowsphone81vpnconfiguration.md) object.</span></span>

<span data-ttu-id="4ed38-128">下表显示创建[windowsPhone81VpnConfiguration](../resources/intune-deviceconfig-windowsphone81vpnconfiguration.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="4ed38-128">The following table shows the properties that are required when you create the [windowsPhone81VpnConfiguration](../resources/intune-deviceconfig-windowsphone81vpnconfiguration.md).</span></span>

|<span data-ttu-id="4ed38-129">属性</span><span class="sxs-lookup"><span data-stu-id="4ed38-129">Property</span></span>|<span data-ttu-id="4ed38-130">类型</span><span class="sxs-lookup"><span data-stu-id="4ed38-130">Type</span></span>|<span data-ttu-id="4ed38-131">说明</span><span class="sxs-lookup"><span data-stu-id="4ed38-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4ed38-132">id</span><span class="sxs-lookup"><span data-stu-id="4ed38-132">id</span></span>|<span data-ttu-id="4ed38-133">String</span><span class="sxs-lookup"><span data-stu-id="4ed38-133">String</span></span>|<span data-ttu-id="4ed38-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="4ed38-134">Key of the entity.</span></span> <span data-ttu-id="4ed38-135">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4ed38-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4ed38-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4ed38-136">lastModifiedDateTime</span></span>|<span data-ttu-id="4ed38-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4ed38-137">DateTimeOffset</span></span>|<span data-ttu-id="4ed38-138">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="4ed38-138">DateTime the object was last modified.</span></span> <span data-ttu-id="4ed38-139">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4ed38-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4ed38-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="4ed38-140">roleScopeTagIds</span></span>|<span data-ttu-id="4ed38-141">String collection</span><span class="sxs-lookup"><span data-stu-id="4ed38-141">String collection</span></span>|<span data-ttu-id="4ed38-142">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="4ed38-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="4ed38-143">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4ed38-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4ed38-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="4ed38-144">supportsScopeTags</span></span>|<span data-ttu-id="4ed38-145">布尔</span><span class="sxs-lookup"><span data-stu-id="4ed38-145">Boolean</span></span>|<span data-ttu-id="4ed38-146">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="4ed38-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="4ed38-147">如果此值为 false, 则不允许分配给 ScopeTags 属性, 并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="4ed38-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="4ed38-148">这适用于在 Silverlight 中创建的旧版策略, 可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="4ed38-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="4ed38-149">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="4ed38-149">This property is read-only.</span></span> <span data-ttu-id="4ed38-150">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4ed38-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4ed38-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="4ed38-151">createdDateTime</span></span>|<span data-ttu-id="4ed38-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4ed38-152">DateTimeOffset</span></span>|<span data-ttu-id="4ed38-153">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="4ed38-153">DateTime the object was created.</span></span> <span data-ttu-id="4ed38-154">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4ed38-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4ed38-155">description</span><span class="sxs-lookup"><span data-stu-id="4ed38-155">description</span></span>|<span data-ttu-id="4ed38-156">String</span><span class="sxs-lookup"><span data-stu-id="4ed38-156">String</span></span>|<span data-ttu-id="4ed38-157">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="4ed38-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="4ed38-158">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4ed38-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4ed38-159">displayName</span><span class="sxs-lookup"><span data-stu-id="4ed38-159">displayName</span></span>|<span data-ttu-id="4ed38-160">String</span><span class="sxs-lookup"><span data-stu-id="4ed38-160">String</span></span>|<span data-ttu-id="4ed38-161">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="4ed38-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="4ed38-162">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4ed38-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4ed38-163">version</span><span class="sxs-lookup"><span data-stu-id="4ed38-163">version</span></span>|<span data-ttu-id="4ed38-164">Int32</span><span class="sxs-lookup"><span data-stu-id="4ed38-164">Int32</span></span>|<span data-ttu-id="4ed38-165">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="4ed38-165">Version of the device configuration.</span></span> <span data-ttu-id="4ed38-166">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4ed38-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4ed38-167">connectionName</span><span class="sxs-lookup"><span data-stu-id="4ed38-167">connectionName</span></span>|<span data-ttu-id="4ed38-168">字符串</span><span class="sxs-lookup"><span data-stu-id="4ed38-168">String</span></span>|<span data-ttu-id="4ed38-169">向用户显示的连接名称。</span><span class="sxs-lookup"><span data-stu-id="4ed38-169">Connection name displayed to the user.</span></span> <span data-ttu-id="4ed38-170">继承自[windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4ed38-170">Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="4ed38-171">服务器</span><span class="sxs-lookup"><span data-stu-id="4ed38-171">servers</span></span>|<span data-ttu-id="4ed38-172">[vpnServer](../resources/intune-deviceconfig-vpnserver.md)集合</span><span class="sxs-lookup"><span data-stu-id="4ed38-172">[vpnServer](../resources/intune-deviceconfig-vpnserver.md) collection</span></span>|<span data-ttu-id="4ed38-173">网络上的 VPN 服务器的列表。</span><span class="sxs-lookup"><span data-stu-id="4ed38-173">List of VPN Servers on the network.</span></span> <span data-ttu-id="4ed38-174">请确保最终用户可以访问这些网络位置。</span><span class="sxs-lookup"><span data-stu-id="4ed38-174">Make sure end users can access these network locations.</span></span> <span data-ttu-id="4ed38-175">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="4ed38-175">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="4ed38-176">继承自[windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4ed38-176">Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="4ed38-177">customXml</span><span class="sxs-lookup"><span data-stu-id="4ed38-177">customXml</span></span>|<span data-ttu-id="4ed38-178">Binary</span><span class="sxs-lookup"><span data-stu-id="4ed38-178">Binary</span></span>|<span data-ttu-id="4ed38-179">配置 VPN 连接的自定义 XML 命令。</span><span class="sxs-lookup"><span data-stu-id="4ed38-179">Custom XML commands that configures the VPN connection.</span></span> <span data-ttu-id="4ed38-180">(UTF8 编码的字节数组)继承自[windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4ed38-180">(UTF8 encoded byte array) Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="4ed38-181">applyOnlyToWindows81</span><span class="sxs-lookup"><span data-stu-id="4ed38-181">applyOnlyToWindows81</span></span>|<span data-ttu-id="4ed38-182">Boolean</span><span class="sxs-lookup"><span data-stu-id="4ed38-182">Boolean</span></span>|<span data-ttu-id="4ed38-183">指示此策略是否仅适用于 Windows 8.1 的值。</span><span class="sxs-lookup"><span data-stu-id="4ed38-183">Value indicating whether this policy only applies to Windows 8.1.</span></span> <span data-ttu-id="4ed38-184">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="4ed38-184">This property is read-only.</span></span> <span data-ttu-id="4ed38-185">继承自[windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4ed38-185">Inherited from [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)</span></span>|
|<span data-ttu-id="4ed38-186">connectionType</span><span class="sxs-lookup"><span data-stu-id="4ed38-186">connectionType</span></span>|[<span data-ttu-id="4ed38-187">windowsVpnConnectionType</span><span class="sxs-lookup"><span data-stu-id="4ed38-187">windowsVpnConnectionType</span></span>](../resources/intune-deviceconfig-windowsvpnconnectiontype.md)|<span data-ttu-id="4ed38-188">连接类型。</span><span class="sxs-lookup"><span data-stu-id="4ed38-188">Connection type.</span></span> <span data-ttu-id="4ed38-189">继承自[windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)。</span><span class="sxs-lookup"><span data-stu-id="4ed38-189">Inherited from [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md).</span></span> <span data-ttu-id="4ed38-190">可取值为：`pulseSecure`、`f5EdgeClient`、`dellSonicWallMobileConnect`、`checkPointCapsuleVpn`。</span><span class="sxs-lookup"><span data-stu-id="4ed38-190">Possible values are: `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`.</span></span>|
|<span data-ttu-id="4ed38-191">loginGroupOrDomain</span><span class="sxs-lookup"><span data-stu-id="4ed38-191">loginGroupOrDomain</span></span>|<span data-ttu-id="4ed38-192">字符串</span><span class="sxs-lookup"><span data-stu-id="4ed38-192">String</span></span>|<span data-ttu-id="4ed38-193">将连接类型设置为 Dell SonicWALL Mobile 连接时的登录组或域。</span><span class="sxs-lookup"><span data-stu-id="4ed38-193">Login group or domain when connection type is set to Dell SonicWALL Mobile Connection.</span></span> <span data-ttu-id="4ed38-194">继承自[windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4ed38-194">Inherited from [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)</span></span>|
|<span data-ttu-id="4ed38-195">enableSplitTunneling</span><span class="sxs-lookup"><span data-stu-id="4ed38-195">enableSplitTunneling</span></span>|<span data-ttu-id="4ed38-196">布尔</span><span class="sxs-lookup"><span data-stu-id="4ed38-196">Boolean</span></span>|<span data-ttu-id="4ed38-197">为 VPN 启用拆分隧道。</span><span class="sxs-lookup"><span data-stu-id="4ed38-197">Enable split tunneling for the VPN.</span></span> <span data-ttu-id="4ed38-198">继承自[windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4ed38-198">Inherited from [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)</span></span>|
|<span data-ttu-id="4ed38-199">proxyServer</span><span class="sxs-lookup"><span data-stu-id="4ed38-199">proxyServer</span></span>|[<span data-ttu-id="4ed38-200">windows81VpnProxyServer</span><span class="sxs-lookup"><span data-stu-id="4ed38-200">windows81VpnProxyServer</span></span>](../resources/intune-deviceconfig-windows81vpnproxyserver.md)|<span data-ttu-id="4ed38-201">代理服务器。</span><span class="sxs-lookup"><span data-stu-id="4ed38-201">Proxy Server.</span></span> <span data-ttu-id="4ed38-202">继承自[windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4ed38-202">Inherited from [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)</span></span>|
|<span data-ttu-id="4ed38-203">bypassVpnOnCompanyWifi</span><span class="sxs-lookup"><span data-stu-id="4ed38-203">bypassVpnOnCompanyWifi</span></span>|<span data-ttu-id="4ed38-204">布尔</span><span class="sxs-lookup"><span data-stu-id="4ed38-204">Boolean</span></span>|<span data-ttu-id="4ed38-205">在公司 wi-fi 上绕过 VPN。</span><span class="sxs-lookup"><span data-stu-id="4ed38-205">Bypass VPN on company Wi-Fi.</span></span>|
|<span data-ttu-id="4ed38-206">bypassVpnOnHomeWifi</span><span class="sxs-lookup"><span data-stu-id="4ed38-206">bypassVpnOnHomeWifi</span></span>|<span data-ttu-id="4ed38-207">布尔</span><span class="sxs-lookup"><span data-stu-id="4ed38-207">Boolean</span></span>|<span data-ttu-id="4ed38-208">绕过家庭 wi-fi 上的 VPN。</span><span class="sxs-lookup"><span data-stu-id="4ed38-208">Bypass VPN on home Wi-Fi.</span></span>|
|<span data-ttu-id="4ed38-209">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="4ed38-209">authenticationMethod</span></span>|[<span data-ttu-id="4ed38-210">vpnAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="4ed38-210">vpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-vpnauthenticationmethod.md)|<span data-ttu-id="4ed38-211">身份验证方法。</span><span class="sxs-lookup"><span data-stu-id="4ed38-211">Authentication method.</span></span> <span data-ttu-id="4ed38-212">可取值为：`certificate`、`usernameAndPassword`。</span><span class="sxs-lookup"><span data-stu-id="4ed38-212">Possible values are: `certificate`, `usernameAndPassword`.</span></span>|
|<span data-ttu-id="4ed38-213">rememberUserCredentials</span><span class="sxs-lookup"><span data-stu-id="4ed38-213">rememberUserCredentials</span></span>|<span data-ttu-id="4ed38-214">布尔</span><span class="sxs-lookup"><span data-stu-id="4ed38-214">Boolean</span></span>|<span data-ttu-id="4ed38-215">记住用户凭据。</span><span class="sxs-lookup"><span data-stu-id="4ed38-215">Remember user credentials.</span></span>|
|<span data-ttu-id="4ed38-216">dnsSuffixSearchList</span><span class="sxs-lookup"><span data-stu-id="4ed38-216">dnsSuffixSearchList</span></span>|<span data-ttu-id="4ed38-217">String collection</span><span class="sxs-lookup"><span data-stu-id="4ed38-217">String collection</span></span>|<span data-ttu-id="4ed38-218">DNS 后缀搜索列表。</span><span class="sxs-lookup"><span data-stu-id="4ed38-218">DNS suffix search list.</span></span>|



## <a name="response"></a><span data-ttu-id="4ed38-219">响应</span><span class="sxs-lookup"><span data-stu-id="4ed38-219">Response</span></span>
<span data-ttu-id="4ed38-220">如果成功, 此方法在响应`200 OK`正文中返回响应代码和更新的[windowsPhone81VpnConfiguration](../resources/intune-deviceconfig-windowsphone81vpnconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="4ed38-220">If successful, this method returns a `200 OK` response code and an updated [windowsPhone81VpnConfiguration](../resources/intune-deviceconfig-windowsphone81vpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4ed38-221">示例</span><span class="sxs-lookup"><span data-stu-id="4ed38-221">Example</span></span>

### <a name="request"></a><span data-ttu-id="4ed38-222">请求</span><span class="sxs-lookup"><span data-stu-id="4ed38-222">Request</span></span>
<span data-ttu-id="4ed38-223">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="4ed38-223">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1243

{
  "@odata.type": "#microsoft.graph.windowsPhone81VpnConfiguration",
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

### <a name="response"></a><span data-ttu-id="4ed38-224">响应</span><span class="sxs-lookup"><span data-stu-id="4ed38-224">Response</span></span>
<span data-ttu-id="4ed38-p119">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="4ed38-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




