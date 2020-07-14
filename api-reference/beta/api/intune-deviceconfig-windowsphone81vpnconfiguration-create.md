---
title: 创建 windowsPhone81VpnConfiguration
description: 创建新的 windowsPhone81VpnConfiguration 对象。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: bceb99dd1d59ff8e6ac64707d484abed11c0a013
ms.sourcegitcommit: f3dda172d95ef1eda8f6dd9e3ffdc7d3c0744c0a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/14/2020
ms.locfileid: "45122768"
---
# <a name="create-windowsphone81vpnconfiguration"></a><span data-ttu-id="15488-103">创建 windowsPhone81VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="15488-103">Create windowsPhone81VpnConfiguration</span></span>

<span data-ttu-id="15488-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="15488-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="15488-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="15488-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="15488-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="15488-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="15488-107">创建新的[windowsPhone81VpnConfiguration](../resources/intune-deviceconfig-windowsphone81vpnconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="15488-107">Create a new [windowsPhone81VpnConfiguration](../resources/intune-deviceconfig-windowsphone81vpnconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="15488-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="15488-108">Prerequisites</span></span>
<span data-ttu-id="15488-109">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="15488-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="15488-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="15488-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="15488-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="15488-111">Permission type</span></span>|<span data-ttu-id="15488-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="15488-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="15488-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="15488-113">Delegated (work or school account)</span></span>|<span data-ttu-id="15488-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="15488-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="15488-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="15488-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="15488-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="15488-116">Not supported.</span></span>|
|<span data-ttu-id="15488-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="15488-117">Application</span></span>|<span data-ttu-id="15488-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="15488-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="15488-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="15488-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="15488-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="15488-120">Request headers</span></span>
|<span data-ttu-id="15488-121">标头</span><span class="sxs-lookup"><span data-stu-id="15488-121">Header</span></span>|<span data-ttu-id="15488-122">值</span><span class="sxs-lookup"><span data-stu-id="15488-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="15488-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="15488-123">Authorization</span></span>|<span data-ttu-id="15488-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="15488-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="15488-125">接受</span><span class="sxs-lookup"><span data-stu-id="15488-125">Accept</span></span>|<span data-ttu-id="15488-126">application/json</span><span class="sxs-lookup"><span data-stu-id="15488-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="15488-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="15488-127">Request body</span></span>
<span data-ttu-id="15488-128">在请求正文中，提供 windowsPhone81VpnConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="15488-128">In the request body, supply a JSON representation for the windowsPhone81VpnConfiguration object.</span></span>

<span data-ttu-id="15488-129">下表显示创建 windowsPhone81VpnConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="15488-129">The following table shows the properties that are required when you create the windowsPhone81VpnConfiguration.</span></span>

|<span data-ttu-id="15488-130">属性</span><span class="sxs-lookup"><span data-stu-id="15488-130">Property</span></span>|<span data-ttu-id="15488-131">类型</span><span class="sxs-lookup"><span data-stu-id="15488-131">Type</span></span>|<span data-ttu-id="15488-132">说明</span><span class="sxs-lookup"><span data-stu-id="15488-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="15488-133">id</span><span class="sxs-lookup"><span data-stu-id="15488-133">id</span></span>|<span data-ttu-id="15488-134">字符串</span><span class="sxs-lookup"><span data-stu-id="15488-134">String</span></span>|<span data-ttu-id="15488-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="15488-135">Key of the entity.</span></span> <span data-ttu-id="15488-136">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="15488-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="15488-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="15488-137">lastModifiedDateTime</span></span>|<span data-ttu-id="15488-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="15488-138">DateTimeOffset</span></span>|<span data-ttu-id="15488-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="15488-139">DateTime the object was last modified.</span></span> <span data-ttu-id="15488-140">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="15488-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="15488-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="15488-141">roleScopeTagIds</span></span>|<span data-ttu-id="15488-142">String collection</span><span class="sxs-lookup"><span data-stu-id="15488-142">String collection</span></span>|<span data-ttu-id="15488-143">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="15488-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="15488-144">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="15488-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="15488-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="15488-145">supportsScopeTags</span></span>|<span data-ttu-id="15488-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="15488-146">Boolean</span></span>|<span data-ttu-id="15488-147">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="15488-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="15488-148">如果此值为 false，则不允许分配给 ScopeTags 属性，并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="15488-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="15488-149">这适用于在 Silverlight 中创建的旧版策略，可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="15488-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="15488-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="15488-150">This property is read-only.</span></span> <span data-ttu-id="15488-151">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="15488-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="15488-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="15488-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="15488-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="15488-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="15488-154">适用于此策略的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="15488-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="15488-155">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="15488-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="15488-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="15488-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="15488-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="15488-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="15488-158">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="15488-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="15488-159">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="15488-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="15488-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="15488-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="15488-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="15488-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="15488-162">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="15488-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="15488-163">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="15488-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="15488-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="15488-164">createdDateTime</span></span>|<span data-ttu-id="15488-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="15488-165">DateTimeOffset</span></span>|<span data-ttu-id="15488-166">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="15488-166">DateTime the object was created.</span></span> <span data-ttu-id="15488-167">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="15488-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="15488-168">说明</span><span class="sxs-lookup"><span data-stu-id="15488-168">description</span></span>|<span data-ttu-id="15488-169">String</span><span class="sxs-lookup"><span data-stu-id="15488-169">String</span></span>|<span data-ttu-id="15488-170">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="15488-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="15488-171">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="15488-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="15488-172">displayName</span><span class="sxs-lookup"><span data-stu-id="15488-172">displayName</span></span>|<span data-ttu-id="15488-173">String</span><span class="sxs-lookup"><span data-stu-id="15488-173">String</span></span>|<span data-ttu-id="15488-174">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="15488-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="15488-175">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="15488-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="15488-176">version</span><span class="sxs-lookup"><span data-stu-id="15488-176">version</span></span>|<span data-ttu-id="15488-177">Int32</span><span class="sxs-lookup"><span data-stu-id="15488-177">Int32</span></span>|<span data-ttu-id="15488-178">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="15488-178">Version of the device configuration.</span></span> <span data-ttu-id="15488-179">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="15488-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="15488-180">connectionName</span><span class="sxs-lookup"><span data-stu-id="15488-180">connectionName</span></span>|<span data-ttu-id="15488-181">String</span><span class="sxs-lookup"><span data-stu-id="15488-181">String</span></span>|<span data-ttu-id="15488-182">向用户显示的连接名称。</span><span class="sxs-lookup"><span data-stu-id="15488-182">Connection name displayed to the user.</span></span> <span data-ttu-id="15488-183">继承自[windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="15488-183">Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="15488-184">台</span><span class="sxs-lookup"><span data-stu-id="15488-184">servers</span></span>|<span data-ttu-id="15488-185">[vpnServer](../resources/intune-deviceconfig-vpnserver.md)集合</span><span class="sxs-lookup"><span data-stu-id="15488-185">[vpnServer](../resources/intune-deviceconfig-vpnserver.md) collection</span></span>|<span data-ttu-id="15488-186">网络上的 VPN 服务器的列表。</span><span class="sxs-lookup"><span data-stu-id="15488-186">List of VPN Servers on the network.</span></span> <span data-ttu-id="15488-187">请确保最终用户可以访问这些网络位置。</span><span class="sxs-lookup"><span data-stu-id="15488-187">Make sure end users can access these network locations.</span></span> <span data-ttu-id="15488-188">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="15488-188">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="15488-189">继承自[windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="15488-189">Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="15488-190">customXml</span><span class="sxs-lookup"><span data-stu-id="15488-190">customXml</span></span>|<span data-ttu-id="15488-191">Binary</span><span class="sxs-lookup"><span data-stu-id="15488-191">Binary</span></span>|<span data-ttu-id="15488-192">配置 VPN 连接的自定义 XML 命令。</span><span class="sxs-lookup"><span data-stu-id="15488-192">Custom XML commands that configures the VPN connection.</span></span> <span data-ttu-id="15488-193">从[WindowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)继承的 (UTF8 编码的字节数组) </span><span class="sxs-lookup"><span data-stu-id="15488-193">(UTF8 encoded byte array) Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="15488-194">applyOnlyToWindows81</span><span class="sxs-lookup"><span data-stu-id="15488-194">applyOnlyToWindows81</span></span>|<span data-ttu-id="15488-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="15488-195">Boolean</span></span>|<span data-ttu-id="15488-196">指示此策略是否仅适用于 Windows 8.1 的值。</span><span class="sxs-lookup"><span data-stu-id="15488-196">Value indicating whether this policy only applies to Windows 8.1.</span></span> <span data-ttu-id="15488-197">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="15488-197">This property is read-only.</span></span> <span data-ttu-id="15488-198">继承自[windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="15488-198">Inherited from [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)</span></span>|
|<span data-ttu-id="15488-199">connectionType</span><span class="sxs-lookup"><span data-stu-id="15488-199">connectionType</span></span>|[<span data-ttu-id="15488-200">windowsVpnConnectionType</span><span class="sxs-lookup"><span data-stu-id="15488-200">windowsVpnConnectionType</span></span>](../resources/intune-deviceconfig-windowsvpnconnectiontype.md)|<span data-ttu-id="15488-201">连接类型。</span><span class="sxs-lookup"><span data-stu-id="15488-201">Connection type.</span></span> <span data-ttu-id="15488-202">继承自[windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)。</span><span class="sxs-lookup"><span data-stu-id="15488-202">Inherited from [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md).</span></span> <span data-ttu-id="15488-203">可取值为：`pulseSecure`、`f5EdgeClient`、`dellSonicWallMobileConnect`、`checkPointCapsuleVpn`。</span><span class="sxs-lookup"><span data-stu-id="15488-203">Possible values are: `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`.</span></span>|
|<span data-ttu-id="15488-204">loginGroupOrDomain</span><span class="sxs-lookup"><span data-stu-id="15488-204">loginGroupOrDomain</span></span>|<span data-ttu-id="15488-205">String</span><span class="sxs-lookup"><span data-stu-id="15488-205">String</span></span>|<span data-ttu-id="15488-206">将连接类型设置为 Dell SonicWALL Mobile 连接时的登录组或域。</span><span class="sxs-lookup"><span data-stu-id="15488-206">Login group or domain when connection type is set to Dell SonicWALL Mobile Connection.</span></span> <span data-ttu-id="15488-207">继承自[windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="15488-207">Inherited from [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)</span></span>|
|<span data-ttu-id="15488-208">enableSplitTunneling</span><span class="sxs-lookup"><span data-stu-id="15488-208">enableSplitTunneling</span></span>|<span data-ttu-id="15488-209">Boolean</span><span class="sxs-lookup"><span data-stu-id="15488-209">Boolean</span></span>|<span data-ttu-id="15488-210">为 VPN 启用拆分隧道。</span><span class="sxs-lookup"><span data-stu-id="15488-210">Enable split tunneling for the VPN.</span></span> <span data-ttu-id="15488-211">继承自[windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="15488-211">Inherited from [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)</span></span>|
|<span data-ttu-id="15488-212">proxyServer</span><span class="sxs-lookup"><span data-stu-id="15488-212">proxyServer</span></span>|[<span data-ttu-id="15488-213">windows81VpnProxyServer</span><span class="sxs-lookup"><span data-stu-id="15488-213">windows81VpnProxyServer</span></span>](../resources/intune-deviceconfig-windows81vpnproxyserver.md)|<span data-ttu-id="15488-214">代理服务器。</span><span class="sxs-lookup"><span data-stu-id="15488-214">Proxy Server.</span></span> <span data-ttu-id="15488-215">继承自[windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="15488-215">Inherited from [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)</span></span>|
|<span data-ttu-id="15488-216">bypassVpnOnCompanyWifi</span><span class="sxs-lookup"><span data-stu-id="15488-216">bypassVpnOnCompanyWifi</span></span>|<span data-ttu-id="15488-217">Boolean</span><span class="sxs-lookup"><span data-stu-id="15488-217">Boolean</span></span>|<span data-ttu-id="15488-218">在公司 Wi-fi 上绕过 VPN。</span><span class="sxs-lookup"><span data-stu-id="15488-218">Bypass VPN on company Wi-Fi.</span></span>|
|<span data-ttu-id="15488-219">bypassVpnOnHomeWifi</span><span class="sxs-lookup"><span data-stu-id="15488-219">bypassVpnOnHomeWifi</span></span>|<span data-ttu-id="15488-220">Boolean</span><span class="sxs-lookup"><span data-stu-id="15488-220">Boolean</span></span>|<span data-ttu-id="15488-221">绕过家庭 Wi-fi 上的 VPN。</span><span class="sxs-lookup"><span data-stu-id="15488-221">Bypass VPN on home Wi-Fi.</span></span>|
|<span data-ttu-id="15488-222">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="15488-222">authenticationMethod</span></span>|[<span data-ttu-id="15488-223">vpnAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="15488-223">vpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-vpnauthenticationmethod.md)|<span data-ttu-id="15488-224">身份验证方法。</span><span class="sxs-lookup"><span data-stu-id="15488-224">Authentication method.</span></span> <span data-ttu-id="15488-225">可取值为：`certificate`、`usernameAndPassword`、`sharedSecret`、`derivedCredential`、`azureAD`。</span><span class="sxs-lookup"><span data-stu-id="15488-225">Possible values are: `certificate`, `usernameAndPassword`, `sharedSecret`, `derivedCredential`, `azureAD`.</span></span>|
|<span data-ttu-id="15488-226">rememberUserCredentials</span><span class="sxs-lookup"><span data-stu-id="15488-226">rememberUserCredentials</span></span>|<span data-ttu-id="15488-227">Boolean</span><span class="sxs-lookup"><span data-stu-id="15488-227">Boolean</span></span>|<span data-ttu-id="15488-228">记住用户凭据。</span><span class="sxs-lookup"><span data-stu-id="15488-228">Remember user credentials.</span></span>|
|<span data-ttu-id="15488-229">dnsSuffixSearchList</span><span class="sxs-lookup"><span data-stu-id="15488-229">dnsSuffixSearchList</span></span>|<span data-ttu-id="15488-230">String collection</span><span class="sxs-lookup"><span data-stu-id="15488-230">String collection</span></span>|<span data-ttu-id="15488-231">DNS 后缀搜索列表。</span><span class="sxs-lookup"><span data-stu-id="15488-231">DNS suffix search list.</span></span>|



## <a name="response"></a><span data-ttu-id="15488-232">响应</span><span class="sxs-lookup"><span data-stu-id="15488-232">Response</span></span>
<span data-ttu-id="15488-233">如果成功，此方法 `201 Created` 在响应正文中返回响应代码和[windowsPhone81VpnConfiguration](../resources/intune-deviceconfig-windowsphone81vpnconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="15488-233">If successful, this method returns a `201 Created` response code and a [windowsPhone81VpnConfiguration](../resources/intune-deviceconfig-windowsphone81vpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="15488-234">示例</span><span class="sxs-lookup"><span data-stu-id="15488-234">Example</span></span>

### <a name="request"></a><span data-ttu-id="15488-235">请求</span><span class="sxs-lookup"><span data-stu-id="15488-235">Request</span></span>
<span data-ttu-id="15488-236">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="15488-236">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 2016

{
  "@odata.type": "#microsoft.graph.windowsPhone81VpnConfiguration",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "deviceManagementApplicabilityRuleOsEdition": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsEdition",
    "osEditionTypes": [
      "windows10EnterpriseN"
    ],
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleOsVersion": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsVersion",
    "minOSVersion": "Min OSVersion value",
    "maxOSVersion": "Max OSVersion value",
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleDeviceMode": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleDeviceMode",
    "deviceMode": "sModeConfiguration",
    "name": "Name value",
    "ruleType": "exclude"
  },
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

### <a name="response"></a><span data-ttu-id="15488-237">响应</span><span class="sxs-lookup"><span data-stu-id="15488-237">Response</span></span>
<span data-ttu-id="15488-238">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="15488-238">Here is an example of the response.</span></span> <span data-ttu-id="15488-239">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="15488-239">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="15488-240">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="15488-240">All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 2188

{
  "@odata.type": "#microsoft.graph.windowsPhone81VpnConfiguration",
  "id": "7cecc0db-c0db-7cec-dbc0-ec7cdbc0ec7c",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "deviceManagementApplicabilityRuleOsEdition": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsEdition",
    "osEditionTypes": [
      "windows10EnterpriseN"
    ],
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleOsVersion": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsVersion",
    "minOSVersion": "Min OSVersion value",
    "maxOSVersion": "Max OSVersion value",
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleDeviceMode": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleDeviceMode",
    "deviceMode": "sModeConfiguration",
    "name": "Name value",
    "ruleType": "exclude"
  },
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



