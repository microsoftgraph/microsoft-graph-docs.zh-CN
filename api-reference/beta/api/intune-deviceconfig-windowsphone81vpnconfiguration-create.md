---
title: 创建 windowsPhone81VpnConfiguration
description: 创建新的 windowsPhone81VpnConfiguration 对象。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 09252f2a1d9b55d64979c2b34bffa9de07e26c8f
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36313830"
---
# <a name="create-windowsphone81vpnconfiguration"></a><span data-ttu-id="88db3-103">创建 windowsPhone81VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="88db3-103">Create windowsPhone81VpnConfiguration</span></span>

> <span data-ttu-id="88db3-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="88db3-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="88db3-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="88db3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="88db3-106">创建新的[windowsPhone81VpnConfiguration](../resources/intune-deviceconfig-windowsphone81vpnconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="88db3-106">Create a new [windowsPhone81VpnConfiguration](../resources/intune-deviceconfig-windowsphone81vpnconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="88db3-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="88db3-107">Prerequisites</span></span>
<span data-ttu-id="88db3-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="88db3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="88db3-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="88db3-110">Permission type</span></span>|<span data-ttu-id="88db3-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="88db3-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="88db3-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="88db3-112">Delegated (work or school account)</span></span>|<span data-ttu-id="88db3-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="88db3-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="88db3-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="88db3-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="88db3-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="88db3-115">Not supported.</span></span>|
|<span data-ttu-id="88db3-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="88db3-116">Application</span></span>|<span data-ttu-id="88db3-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="88db3-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="88db3-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="88db3-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="88db3-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="88db3-119">Request headers</span></span>
|<span data-ttu-id="88db3-120">标头</span><span class="sxs-lookup"><span data-stu-id="88db3-120">Header</span></span>|<span data-ttu-id="88db3-121">值</span><span class="sxs-lookup"><span data-stu-id="88db3-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="88db3-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="88db3-122">Authorization</span></span>|<span data-ttu-id="88db3-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="88db3-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="88db3-124">接受</span><span class="sxs-lookup"><span data-stu-id="88db3-124">Accept</span></span>|<span data-ttu-id="88db3-125">application/json</span><span class="sxs-lookup"><span data-stu-id="88db3-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="88db3-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="88db3-126">Request body</span></span>
<span data-ttu-id="88db3-127">在请求正文中, 提供 windowsPhone81VpnConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="88db3-127">In the request body, supply a JSON representation for the windowsPhone81VpnConfiguration object.</span></span>

<span data-ttu-id="88db3-128">下表显示创建 windowsPhone81VpnConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="88db3-128">The following table shows the properties that are required when you create the windowsPhone81VpnConfiguration.</span></span>

|<span data-ttu-id="88db3-129">属性</span><span class="sxs-lookup"><span data-stu-id="88db3-129">Property</span></span>|<span data-ttu-id="88db3-130">类型</span><span class="sxs-lookup"><span data-stu-id="88db3-130">Type</span></span>|<span data-ttu-id="88db3-131">说明</span><span class="sxs-lookup"><span data-stu-id="88db3-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="88db3-132">id</span><span class="sxs-lookup"><span data-stu-id="88db3-132">id</span></span>|<span data-ttu-id="88db3-133">字符串</span><span class="sxs-lookup"><span data-stu-id="88db3-133">String</span></span>|<span data-ttu-id="88db3-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="88db3-134">Key of the entity.</span></span> <span data-ttu-id="88db3-135">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="88db3-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="88db3-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="88db3-136">lastModifiedDateTime</span></span>|<span data-ttu-id="88db3-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="88db3-137">DateTimeOffset</span></span>|<span data-ttu-id="88db3-138">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="88db3-138">DateTime the object was last modified.</span></span> <span data-ttu-id="88db3-139">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="88db3-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="88db3-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="88db3-140">roleScopeTagIds</span></span>|<span data-ttu-id="88db3-141">String collection</span><span class="sxs-lookup"><span data-stu-id="88db3-141">String collection</span></span>|<span data-ttu-id="88db3-142">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="88db3-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="88db3-143">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="88db3-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="88db3-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="88db3-144">supportsScopeTags</span></span>|<span data-ttu-id="88db3-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="88db3-145">Boolean</span></span>|<span data-ttu-id="88db3-146">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="88db3-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="88db3-147">如果此值为 false, 则不允许分配给 ScopeTags 属性, 并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="88db3-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="88db3-148">这适用于在 Silverlight 中创建的旧版策略, 可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="88db3-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="88db3-149">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="88db3-149">This property is read-only.</span></span> <span data-ttu-id="88db3-150">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="88db3-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="88db3-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="88db3-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="88db3-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="88db3-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="88db3-153">适用于此策略的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="88db3-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="88db3-154">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="88db3-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="88db3-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="88db3-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="88db3-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="88db3-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="88db3-157">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="88db3-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="88db3-158">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="88db3-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="88db3-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="88db3-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="88db3-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="88db3-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="88db3-161">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="88db3-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="88db3-162">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="88db3-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="88db3-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="88db3-163">createdDateTime</span></span>|<span data-ttu-id="88db3-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="88db3-164">DateTimeOffset</span></span>|<span data-ttu-id="88db3-165">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="88db3-165">DateTime the object was created.</span></span> <span data-ttu-id="88db3-166">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="88db3-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="88db3-167">说明</span><span class="sxs-lookup"><span data-stu-id="88db3-167">description</span></span>|<span data-ttu-id="88db3-168">String</span><span class="sxs-lookup"><span data-stu-id="88db3-168">String</span></span>|<span data-ttu-id="88db3-169">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="88db3-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="88db3-170">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="88db3-170">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="88db3-171">displayName</span><span class="sxs-lookup"><span data-stu-id="88db3-171">displayName</span></span>|<span data-ttu-id="88db3-172">String</span><span class="sxs-lookup"><span data-stu-id="88db3-172">String</span></span>|<span data-ttu-id="88db3-173">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="88db3-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="88db3-174">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="88db3-174">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="88db3-175">version</span><span class="sxs-lookup"><span data-stu-id="88db3-175">version</span></span>|<span data-ttu-id="88db3-176">Int32</span><span class="sxs-lookup"><span data-stu-id="88db3-176">Int32</span></span>|<span data-ttu-id="88db3-177">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="88db3-177">Version of the device configuration.</span></span> <span data-ttu-id="88db3-178">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="88db3-178">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="88db3-179">connectionName</span><span class="sxs-lookup"><span data-stu-id="88db3-179">connectionName</span></span>|<span data-ttu-id="88db3-180">String</span><span class="sxs-lookup"><span data-stu-id="88db3-180">String</span></span>|<span data-ttu-id="88db3-181">向用户显示的连接名称。</span><span class="sxs-lookup"><span data-stu-id="88db3-181">Connection name displayed to the user.</span></span> <span data-ttu-id="88db3-182">继承自[windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="88db3-182">Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="88db3-183">台</span><span class="sxs-lookup"><span data-stu-id="88db3-183">servers</span></span>|<span data-ttu-id="88db3-184">[vpnServer](../resources/intune-deviceconfig-vpnserver.md)集合</span><span class="sxs-lookup"><span data-stu-id="88db3-184">[vpnServer](../resources/intune-deviceconfig-vpnserver.md) collection</span></span>|<span data-ttu-id="88db3-185">网络上的 VPN 服务器的列表。</span><span class="sxs-lookup"><span data-stu-id="88db3-185">List of VPN Servers on the network.</span></span> <span data-ttu-id="88db3-186">请确保最终用户可以访问这些网络位置。</span><span class="sxs-lookup"><span data-stu-id="88db3-186">Make sure end users can access these network locations.</span></span> <span data-ttu-id="88db3-187">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="88db3-187">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="88db3-188">继承自[windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="88db3-188">Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="88db3-189">customXml</span><span class="sxs-lookup"><span data-stu-id="88db3-189">customXml</span></span>|<span data-ttu-id="88db3-190">Binary</span><span class="sxs-lookup"><span data-stu-id="88db3-190">Binary</span></span>|<span data-ttu-id="88db3-191">配置 VPN 连接的自定义 XML 命令。</span><span class="sxs-lookup"><span data-stu-id="88db3-191">Custom XML commands that configures the VPN connection.</span></span> <span data-ttu-id="88db3-192">(UTF8 编码的字节数组)继承自[windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="88db3-192">(UTF8 encoded byte array) Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="88db3-193">applyOnlyToWindows81</span><span class="sxs-lookup"><span data-stu-id="88db3-193">applyOnlyToWindows81</span></span>|<span data-ttu-id="88db3-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="88db3-194">Boolean</span></span>|<span data-ttu-id="88db3-195">指示此策略是否仅适用于 Windows 8.1 的值。</span><span class="sxs-lookup"><span data-stu-id="88db3-195">Value indicating whether this policy only applies to Windows 8.1.</span></span> <span data-ttu-id="88db3-196">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="88db3-196">This property is read-only.</span></span> <span data-ttu-id="88db3-197">继承自[windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="88db3-197">Inherited from [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)</span></span>|
|<span data-ttu-id="88db3-198">connectionType</span><span class="sxs-lookup"><span data-stu-id="88db3-198">connectionType</span></span>|[<span data-ttu-id="88db3-199">windowsVpnConnectionType</span><span class="sxs-lookup"><span data-stu-id="88db3-199">windowsVpnConnectionType</span></span>](../resources/intune-deviceconfig-windowsvpnconnectiontype.md)|<span data-ttu-id="88db3-200">连接类型。</span><span class="sxs-lookup"><span data-stu-id="88db3-200">Connection type.</span></span> <span data-ttu-id="88db3-201">继承自[windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)。</span><span class="sxs-lookup"><span data-stu-id="88db3-201">Inherited from [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md).</span></span> <span data-ttu-id="88db3-202">可取值为：`pulseSecure`、`f5EdgeClient`、`dellSonicWallMobileConnect`、`checkPointCapsuleVpn`。</span><span class="sxs-lookup"><span data-stu-id="88db3-202">Possible values are: `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`.</span></span>|
|<span data-ttu-id="88db3-203">loginGroupOrDomain</span><span class="sxs-lookup"><span data-stu-id="88db3-203">loginGroupOrDomain</span></span>|<span data-ttu-id="88db3-204">String</span><span class="sxs-lookup"><span data-stu-id="88db3-204">String</span></span>|<span data-ttu-id="88db3-205">将连接类型设置为 Dell SonicWALL Mobile 连接时的登录组或域。</span><span class="sxs-lookup"><span data-stu-id="88db3-205">Login group or domain when connection type is set to Dell SonicWALL Mobile Connection.</span></span> <span data-ttu-id="88db3-206">继承自[windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="88db3-206">Inherited from [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)</span></span>|
|<span data-ttu-id="88db3-207">enableSplitTunneling</span><span class="sxs-lookup"><span data-stu-id="88db3-207">enableSplitTunneling</span></span>|<span data-ttu-id="88db3-208">Boolean</span><span class="sxs-lookup"><span data-stu-id="88db3-208">Boolean</span></span>|<span data-ttu-id="88db3-209">为 VPN 启用拆分隧道。</span><span class="sxs-lookup"><span data-stu-id="88db3-209">Enable split tunneling for the VPN.</span></span> <span data-ttu-id="88db3-210">继承自[windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="88db3-210">Inherited from [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)</span></span>|
|<span data-ttu-id="88db3-211">proxyServer</span><span class="sxs-lookup"><span data-stu-id="88db3-211">proxyServer</span></span>|[<span data-ttu-id="88db3-212">windows81VpnProxyServer</span><span class="sxs-lookup"><span data-stu-id="88db3-212">windows81VpnProxyServer</span></span>](../resources/intune-deviceconfig-windows81vpnproxyserver.md)|<span data-ttu-id="88db3-213">代理服务器。</span><span class="sxs-lookup"><span data-stu-id="88db3-213">Proxy Server.</span></span> <span data-ttu-id="88db3-214">继承自[windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="88db3-214">Inherited from [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)</span></span>|
|<span data-ttu-id="88db3-215">bypassVpnOnCompanyWifi</span><span class="sxs-lookup"><span data-stu-id="88db3-215">bypassVpnOnCompanyWifi</span></span>|<span data-ttu-id="88db3-216">Boolean</span><span class="sxs-lookup"><span data-stu-id="88db3-216">Boolean</span></span>|<span data-ttu-id="88db3-217">在公司 Wi-fi 上绕过 VPN。</span><span class="sxs-lookup"><span data-stu-id="88db3-217">Bypass VPN on company Wi-Fi.</span></span>|
|<span data-ttu-id="88db3-218">bypassVpnOnHomeWifi</span><span class="sxs-lookup"><span data-stu-id="88db3-218">bypassVpnOnHomeWifi</span></span>|<span data-ttu-id="88db3-219">Boolean</span><span class="sxs-lookup"><span data-stu-id="88db3-219">Boolean</span></span>|<span data-ttu-id="88db3-220">绕过家庭 Wi-fi 上的 VPN。</span><span class="sxs-lookup"><span data-stu-id="88db3-220">Bypass VPN on home Wi-Fi.</span></span>|
|<span data-ttu-id="88db3-221">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="88db3-221">authenticationMethod</span></span>|[<span data-ttu-id="88db3-222">vpnAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="88db3-222">vpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-vpnauthenticationmethod.md)|<span data-ttu-id="88db3-223">身份验证方法。</span><span class="sxs-lookup"><span data-stu-id="88db3-223">Authentication method.</span></span> <span data-ttu-id="88db3-224">可取值为：`certificate`、`usernameAndPassword`、`sharedSecret`、`derivedCredential`。</span><span class="sxs-lookup"><span data-stu-id="88db3-224">Possible values are: `certificate`, `usernameAndPassword`, `sharedSecret`, `derivedCredential`.</span></span>|
|<span data-ttu-id="88db3-225">rememberUserCredentials</span><span class="sxs-lookup"><span data-stu-id="88db3-225">rememberUserCredentials</span></span>|<span data-ttu-id="88db3-226">Boolean</span><span class="sxs-lookup"><span data-stu-id="88db3-226">Boolean</span></span>|<span data-ttu-id="88db3-227">记住用户凭据。</span><span class="sxs-lookup"><span data-stu-id="88db3-227">Remember user credentials.</span></span>|
|<span data-ttu-id="88db3-228">dnsSuffixSearchList</span><span class="sxs-lookup"><span data-stu-id="88db3-228">dnsSuffixSearchList</span></span>|<span data-ttu-id="88db3-229">String collection</span><span class="sxs-lookup"><span data-stu-id="88db3-229">String collection</span></span>|<span data-ttu-id="88db3-230">DNS 后缀搜索列表。</span><span class="sxs-lookup"><span data-stu-id="88db3-230">DNS suffix search list.</span></span>|



## <a name="response"></a><span data-ttu-id="88db3-231">响应</span><span class="sxs-lookup"><span data-stu-id="88db3-231">Response</span></span>
<span data-ttu-id="88db3-232">如果成功, 此方法在响应`201 Created`正文中返回响应代码和[windowsPhone81VpnConfiguration](../resources/intune-deviceconfig-windowsphone81vpnconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="88db3-232">If successful, this method returns a `201 Created` response code and a [windowsPhone81VpnConfiguration](../resources/intune-deviceconfig-windowsphone81vpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="88db3-233">示例</span><span class="sxs-lookup"><span data-stu-id="88db3-233">Example</span></span>

### <a name="request"></a><span data-ttu-id="88db3-234">请求</span><span class="sxs-lookup"><span data-stu-id="88db3-234">Request</span></span>
<span data-ttu-id="88db3-235">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="88db3-235">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="88db3-236">响应</span><span class="sxs-lookup"><span data-stu-id="88db3-236">Response</span></span>
<span data-ttu-id="88db3-p122">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="88db3-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






