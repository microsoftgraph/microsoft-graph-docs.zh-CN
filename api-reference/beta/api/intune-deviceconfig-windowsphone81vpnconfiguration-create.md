---
title: 创建 windowsPhone81VpnConfiguration
description: 创建新的 windowsPhone81VpnConfiguration 对象。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 177ebe905d4b3043f5f8cf06f2c1fac6d578ddac
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42474394"
---
# <a name="create-windowsphone81vpnconfiguration"></a><span data-ttu-id="9c517-103">创建 windowsPhone81VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="9c517-103">Create windowsPhone81VpnConfiguration</span></span>

<span data-ttu-id="9c517-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="9c517-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9c517-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="9c517-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9c517-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="9c517-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9c517-107">创建新的[windowsPhone81VpnConfiguration](../resources/intune-deviceconfig-windowsphone81vpnconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="9c517-107">Create a new [windowsPhone81VpnConfiguration](../resources/intune-deviceconfig-windowsphone81vpnconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9c517-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="9c517-108">Prerequisites</span></span>
<span data-ttu-id="9c517-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9c517-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9c517-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="9c517-111">Permission type</span></span>|<span data-ttu-id="9c517-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="9c517-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9c517-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9c517-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9c517-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9c517-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="9c517-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9c517-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9c517-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="9c517-116">Not supported.</span></span>|
|<span data-ttu-id="9c517-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="9c517-117">Application</span></span>|<span data-ttu-id="9c517-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9c517-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="9c517-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9c517-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="9c517-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="9c517-120">Request headers</span></span>
|<span data-ttu-id="9c517-121">标头</span><span class="sxs-lookup"><span data-stu-id="9c517-121">Header</span></span>|<span data-ttu-id="9c517-122">值</span><span class="sxs-lookup"><span data-stu-id="9c517-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9c517-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="9c517-123">Authorization</span></span>|<span data-ttu-id="9c517-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="9c517-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9c517-125">接受</span><span class="sxs-lookup"><span data-stu-id="9c517-125">Accept</span></span>|<span data-ttu-id="9c517-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9c517-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9c517-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="9c517-127">Request body</span></span>
<span data-ttu-id="9c517-128">在请求正文中，提供 windowsPhone81VpnConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9c517-128">In the request body, supply a JSON representation for the windowsPhone81VpnConfiguration object.</span></span>

<span data-ttu-id="9c517-129">下表显示创建 windowsPhone81VpnConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="9c517-129">The following table shows the properties that are required when you create the windowsPhone81VpnConfiguration.</span></span>

|<span data-ttu-id="9c517-130">属性</span><span class="sxs-lookup"><span data-stu-id="9c517-130">Property</span></span>|<span data-ttu-id="9c517-131">类型</span><span class="sxs-lookup"><span data-stu-id="9c517-131">Type</span></span>|<span data-ttu-id="9c517-132">说明</span><span class="sxs-lookup"><span data-stu-id="9c517-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9c517-133">id</span><span class="sxs-lookup"><span data-stu-id="9c517-133">id</span></span>|<span data-ttu-id="9c517-134">字符串</span><span class="sxs-lookup"><span data-stu-id="9c517-134">String</span></span>|<span data-ttu-id="9c517-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="9c517-135">Key of the entity.</span></span> <span data-ttu-id="9c517-136">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9c517-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9c517-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9c517-137">lastModifiedDateTime</span></span>|<span data-ttu-id="9c517-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9c517-138">DateTimeOffset</span></span>|<span data-ttu-id="9c517-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="9c517-139">DateTime the object was last modified.</span></span> <span data-ttu-id="9c517-140">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9c517-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9c517-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="9c517-141">roleScopeTagIds</span></span>|<span data-ttu-id="9c517-142">String 集合</span><span class="sxs-lookup"><span data-stu-id="9c517-142">String collection</span></span>|<span data-ttu-id="9c517-143">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="9c517-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="9c517-144">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9c517-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9c517-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="9c517-145">supportsScopeTags</span></span>|<span data-ttu-id="9c517-146">布尔</span><span class="sxs-lookup"><span data-stu-id="9c517-146">Boolean</span></span>|<span data-ttu-id="9c517-147">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="9c517-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="9c517-148">如果此值为 false，则不允许分配给 ScopeTags 属性，并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="9c517-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="9c517-149">这适用于在 Silverlight 中创建的旧版策略，可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="9c517-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="9c517-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="9c517-150">This property is read-only.</span></span> <span data-ttu-id="9c517-151">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9c517-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9c517-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="9c517-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="9c517-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="9c517-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="9c517-154">适用于此策略的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="9c517-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="9c517-155">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9c517-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9c517-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="9c517-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="9c517-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="9c517-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="9c517-158">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="9c517-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="9c517-159">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9c517-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9c517-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="9c517-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="9c517-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="9c517-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="9c517-162">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="9c517-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="9c517-163">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9c517-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9c517-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="9c517-164">createdDateTime</span></span>|<span data-ttu-id="9c517-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9c517-165">DateTimeOffset</span></span>|<span data-ttu-id="9c517-166">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="9c517-166">DateTime the object was created.</span></span> <span data-ttu-id="9c517-167">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9c517-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9c517-168">说明</span><span class="sxs-lookup"><span data-stu-id="9c517-168">description</span></span>|<span data-ttu-id="9c517-169">String</span><span class="sxs-lookup"><span data-stu-id="9c517-169">String</span></span>|<span data-ttu-id="9c517-170">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="9c517-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="9c517-171">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9c517-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9c517-172">displayName</span><span class="sxs-lookup"><span data-stu-id="9c517-172">displayName</span></span>|<span data-ttu-id="9c517-173">String</span><span class="sxs-lookup"><span data-stu-id="9c517-173">String</span></span>|<span data-ttu-id="9c517-174">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="9c517-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="9c517-175">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9c517-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9c517-176">version</span><span class="sxs-lookup"><span data-stu-id="9c517-176">version</span></span>|<span data-ttu-id="9c517-177">Int32</span><span class="sxs-lookup"><span data-stu-id="9c517-177">Int32</span></span>|<span data-ttu-id="9c517-178">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="9c517-178">Version of the device configuration.</span></span> <span data-ttu-id="9c517-179">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9c517-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9c517-180">connectionName</span><span class="sxs-lookup"><span data-stu-id="9c517-180">connectionName</span></span>|<span data-ttu-id="9c517-181">String</span><span class="sxs-lookup"><span data-stu-id="9c517-181">String</span></span>|<span data-ttu-id="9c517-182">向用户显示的连接名称。</span><span class="sxs-lookup"><span data-stu-id="9c517-182">Connection name displayed to the user.</span></span> <span data-ttu-id="9c517-183">继承自[windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9c517-183">Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="9c517-184">台</span><span class="sxs-lookup"><span data-stu-id="9c517-184">servers</span></span>|<span data-ttu-id="9c517-185">[vpnServer](../resources/intune-deviceconfig-vpnserver.md)集合</span><span class="sxs-lookup"><span data-stu-id="9c517-185">[vpnServer](../resources/intune-deviceconfig-vpnserver.md) collection</span></span>|<span data-ttu-id="9c517-186">网络上的 VPN 服务器的列表。</span><span class="sxs-lookup"><span data-stu-id="9c517-186">List of VPN Servers on the network.</span></span> <span data-ttu-id="9c517-187">请确保最终用户可以访问这些网络位置。</span><span class="sxs-lookup"><span data-stu-id="9c517-187">Make sure end users can access these network locations.</span></span> <span data-ttu-id="9c517-188">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="9c517-188">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="9c517-189">继承自[windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9c517-189">Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="9c517-190">customXml</span><span class="sxs-lookup"><span data-stu-id="9c517-190">customXml</span></span>|<span data-ttu-id="9c517-191">Binary</span><span class="sxs-lookup"><span data-stu-id="9c517-191">Binary</span></span>|<span data-ttu-id="9c517-192">配置 VPN 连接的自定义 XML 命令。</span><span class="sxs-lookup"><span data-stu-id="9c517-192">Custom XML commands that configures the VPN connection.</span></span> <span data-ttu-id="9c517-193">（UTF8 编码的字节数组）继承自[windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9c517-193">(UTF8 encoded byte array) Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="9c517-194">applyOnlyToWindows81</span><span class="sxs-lookup"><span data-stu-id="9c517-194">applyOnlyToWindows81</span></span>|<span data-ttu-id="9c517-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="9c517-195">Boolean</span></span>|<span data-ttu-id="9c517-196">指示此策略是否仅适用于 Windows 8.1 的值。</span><span class="sxs-lookup"><span data-stu-id="9c517-196">Value indicating whether this policy only applies to Windows 8.1.</span></span> <span data-ttu-id="9c517-197">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="9c517-197">This property is read-only.</span></span> <span data-ttu-id="9c517-198">继承自[windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9c517-198">Inherited from [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)</span></span>|
|<span data-ttu-id="9c517-199">connectionType</span><span class="sxs-lookup"><span data-stu-id="9c517-199">connectionType</span></span>|[<span data-ttu-id="9c517-200">windowsVpnConnectionType</span><span class="sxs-lookup"><span data-stu-id="9c517-200">windowsVpnConnectionType</span></span>](../resources/intune-deviceconfig-windowsvpnconnectiontype.md)|<span data-ttu-id="9c517-201">连接类型。</span><span class="sxs-lookup"><span data-stu-id="9c517-201">Connection type.</span></span> <span data-ttu-id="9c517-202">继承自[windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)。</span><span class="sxs-lookup"><span data-stu-id="9c517-202">Inherited from [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md).</span></span> <span data-ttu-id="9c517-203">可取值为：`pulseSecure`、`f5EdgeClient`、`dellSonicWallMobileConnect`、`checkPointCapsuleVpn`。</span><span class="sxs-lookup"><span data-stu-id="9c517-203">Possible values are: `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`.</span></span>|
|<span data-ttu-id="9c517-204">loginGroupOrDomain</span><span class="sxs-lookup"><span data-stu-id="9c517-204">loginGroupOrDomain</span></span>|<span data-ttu-id="9c517-205">String</span><span class="sxs-lookup"><span data-stu-id="9c517-205">String</span></span>|<span data-ttu-id="9c517-206">将连接类型设置为 Dell SonicWALL Mobile 连接时的登录组或域。</span><span class="sxs-lookup"><span data-stu-id="9c517-206">Login group or domain when connection type is set to Dell SonicWALL Mobile Connection.</span></span> <span data-ttu-id="9c517-207">继承自[windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9c517-207">Inherited from [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)</span></span>|
|<span data-ttu-id="9c517-208">enableSplitTunneling</span><span class="sxs-lookup"><span data-stu-id="9c517-208">enableSplitTunneling</span></span>|<span data-ttu-id="9c517-209">布尔</span><span class="sxs-lookup"><span data-stu-id="9c517-209">Boolean</span></span>|<span data-ttu-id="9c517-210">为 VPN 启用拆分隧道。</span><span class="sxs-lookup"><span data-stu-id="9c517-210">Enable split tunneling for the VPN.</span></span> <span data-ttu-id="9c517-211">继承自[windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9c517-211">Inherited from [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)</span></span>|
|<span data-ttu-id="9c517-212">proxyServer</span><span class="sxs-lookup"><span data-stu-id="9c517-212">proxyServer</span></span>|[<span data-ttu-id="9c517-213">windows81VpnProxyServer</span><span class="sxs-lookup"><span data-stu-id="9c517-213">windows81VpnProxyServer</span></span>](../resources/intune-deviceconfig-windows81vpnproxyserver.md)|<span data-ttu-id="9c517-214">代理服务器。</span><span class="sxs-lookup"><span data-stu-id="9c517-214">Proxy Server.</span></span> <span data-ttu-id="9c517-215">继承自[windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9c517-215">Inherited from [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)</span></span>|
|<span data-ttu-id="9c517-216">bypassVpnOnCompanyWifi</span><span class="sxs-lookup"><span data-stu-id="9c517-216">bypassVpnOnCompanyWifi</span></span>|<span data-ttu-id="9c517-217">布尔</span><span class="sxs-lookup"><span data-stu-id="9c517-217">Boolean</span></span>|<span data-ttu-id="9c517-218">在公司 Wi-fi 上绕过 VPN。</span><span class="sxs-lookup"><span data-stu-id="9c517-218">Bypass VPN on company Wi-Fi.</span></span>|
|<span data-ttu-id="9c517-219">bypassVpnOnHomeWifi</span><span class="sxs-lookup"><span data-stu-id="9c517-219">bypassVpnOnHomeWifi</span></span>|<span data-ttu-id="9c517-220">布尔</span><span class="sxs-lookup"><span data-stu-id="9c517-220">Boolean</span></span>|<span data-ttu-id="9c517-221">绕过家庭 Wi-fi 上的 VPN。</span><span class="sxs-lookup"><span data-stu-id="9c517-221">Bypass VPN on home Wi-Fi.</span></span>|
|<span data-ttu-id="9c517-222">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="9c517-222">authenticationMethod</span></span>|[<span data-ttu-id="9c517-223">vpnAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="9c517-223">vpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-vpnauthenticationmethod.md)|<span data-ttu-id="9c517-224">身份验证方法。</span><span class="sxs-lookup"><span data-stu-id="9c517-224">Authentication method.</span></span> <span data-ttu-id="9c517-225">可取值为：`certificate`、`usernameAndPassword`、`sharedSecret`、`derivedCredential`。</span><span class="sxs-lookup"><span data-stu-id="9c517-225">Possible values are: `certificate`, `usernameAndPassword`, `sharedSecret`, `derivedCredential`.</span></span>|
|<span data-ttu-id="9c517-226">rememberUserCredentials</span><span class="sxs-lookup"><span data-stu-id="9c517-226">rememberUserCredentials</span></span>|<span data-ttu-id="9c517-227">布尔</span><span class="sxs-lookup"><span data-stu-id="9c517-227">Boolean</span></span>|<span data-ttu-id="9c517-228">记住用户凭据。</span><span class="sxs-lookup"><span data-stu-id="9c517-228">Remember user credentials.</span></span>|
|<span data-ttu-id="9c517-229">dnsSuffixSearchList</span><span class="sxs-lookup"><span data-stu-id="9c517-229">dnsSuffixSearchList</span></span>|<span data-ttu-id="9c517-230">String 集合</span><span class="sxs-lookup"><span data-stu-id="9c517-230">String collection</span></span>|<span data-ttu-id="9c517-231">DNS 后缀搜索列表。</span><span class="sxs-lookup"><span data-stu-id="9c517-231">DNS suffix search list.</span></span>|



## <a name="response"></a><span data-ttu-id="9c517-232">响应</span><span class="sxs-lookup"><span data-stu-id="9c517-232">Response</span></span>
<span data-ttu-id="9c517-233">如果成功，此方法在响应`201 Created`正文中返回响应代码和[windowsPhone81VpnConfiguration](../resources/intune-deviceconfig-windowsphone81vpnconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="9c517-233">If successful, this method returns a `201 Created` response code and a [windowsPhone81VpnConfiguration](../resources/intune-deviceconfig-windowsphone81vpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9c517-234">示例</span><span class="sxs-lookup"><span data-stu-id="9c517-234">Example</span></span>

### <a name="request"></a><span data-ttu-id="9c517-235">请求</span><span class="sxs-lookup"><span data-stu-id="9c517-235">Request</span></span>
<span data-ttu-id="9c517-236">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="9c517-236">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="9c517-237">响应</span><span class="sxs-lookup"><span data-stu-id="9c517-237">Response</span></span>
<span data-ttu-id="9c517-p122">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="9c517-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





