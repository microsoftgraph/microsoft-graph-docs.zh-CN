---
title: 创建 windows81VpnConfiguration
description: 创建新的 windows81VpnConfiguration 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 7118b29d7b18e36c20d9794af682ff9358d1b36c
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51147194"
---
# <a name="create-windows81vpnconfiguration"></a><span data-ttu-id="3bfe7-103">创建 windows81VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="3bfe7-103">Create windows81VpnConfiguration</span></span>

<span data-ttu-id="3bfe7-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3bfe7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3bfe7-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="3bfe7-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3bfe7-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="3bfe7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3bfe7-107">创建新的 [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="3bfe7-107">Create a new [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3bfe7-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="3bfe7-108">Prerequisites</span></span>
<span data-ttu-id="3bfe7-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="3bfe7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3bfe7-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="3bfe7-111">Permission type</span></span>|<span data-ttu-id="3bfe7-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="3bfe7-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3bfe7-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3bfe7-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3bfe7-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3bfe7-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="3bfe7-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3bfe7-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3bfe7-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="3bfe7-116">Not supported.</span></span>|
|<span data-ttu-id="3bfe7-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="3bfe7-117">Application</span></span>|<span data-ttu-id="3bfe7-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3bfe7-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3bfe7-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3bfe7-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="3bfe7-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="3bfe7-120">Request headers</span></span>
|<span data-ttu-id="3bfe7-121">标头</span><span class="sxs-lookup"><span data-stu-id="3bfe7-121">Header</span></span>|<span data-ttu-id="3bfe7-122">值</span><span class="sxs-lookup"><span data-stu-id="3bfe7-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3bfe7-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="3bfe7-123">Authorization</span></span>|<span data-ttu-id="3bfe7-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="3bfe7-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3bfe7-125">接受</span><span class="sxs-lookup"><span data-stu-id="3bfe7-125">Accept</span></span>|<span data-ttu-id="3bfe7-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3bfe7-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3bfe7-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="3bfe7-127">Request body</span></span>
<span data-ttu-id="3bfe7-128">在请求正文中，提供 windows81VpnConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3bfe7-128">In the request body, supply a JSON representation for the windows81VpnConfiguration object.</span></span>

<span data-ttu-id="3bfe7-129">下表显示创建 windows81VpnConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="3bfe7-129">The following table shows the properties that are required when you create the windows81VpnConfiguration.</span></span>

|<span data-ttu-id="3bfe7-130">属性</span><span class="sxs-lookup"><span data-stu-id="3bfe7-130">Property</span></span>|<span data-ttu-id="3bfe7-131">类型</span><span class="sxs-lookup"><span data-stu-id="3bfe7-131">Type</span></span>|<span data-ttu-id="3bfe7-132">说明</span><span class="sxs-lookup"><span data-stu-id="3bfe7-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3bfe7-133">id</span><span class="sxs-lookup"><span data-stu-id="3bfe7-133">id</span></span>|<span data-ttu-id="3bfe7-134">String</span><span class="sxs-lookup"><span data-stu-id="3bfe7-134">String</span></span>|<span data-ttu-id="3bfe7-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="3bfe7-135">Key of the entity.</span></span> <span data-ttu-id="3bfe7-136">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3bfe7-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3bfe7-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3bfe7-137">lastModifiedDateTime</span></span>|<span data-ttu-id="3bfe7-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3bfe7-138">DateTimeOffset</span></span>|<span data-ttu-id="3bfe7-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="3bfe7-139">DateTime the object was last modified.</span></span> <span data-ttu-id="3bfe7-140">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3bfe7-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3bfe7-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="3bfe7-141">roleScopeTagIds</span></span>|<span data-ttu-id="3bfe7-142">String collection</span><span class="sxs-lookup"><span data-stu-id="3bfe7-142">String collection</span></span>|<span data-ttu-id="3bfe7-143">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="3bfe7-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="3bfe7-144">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3bfe7-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3bfe7-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="3bfe7-145">supportsScopeTags</span></span>|<span data-ttu-id="3bfe7-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="3bfe7-146">Boolean</span></span>|<span data-ttu-id="3bfe7-147">指示基础设备配置是否支持分配范围标记。</span><span class="sxs-lookup"><span data-stu-id="3bfe7-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="3bfe7-148">当此值为 false 且实体对作用域用户不可见时，不允许分配给 ScopeTags 属性。</span><span class="sxs-lookup"><span data-stu-id="3bfe7-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="3bfe7-149">这适用于在 Silverlight 中创建的旧版策略，可通过在 Azure 门户中删除和重新创建策略来解决。</span><span class="sxs-lookup"><span data-stu-id="3bfe7-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="3bfe7-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="3bfe7-150">This property is read-only.</span></span> <span data-ttu-id="3bfe7-151">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3bfe7-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3bfe7-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="3bfe7-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="3bfe7-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="3bfe7-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="3bfe7-154">此策略的操作系统版本适用性。</span><span class="sxs-lookup"><span data-stu-id="3bfe7-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="3bfe7-155">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3bfe7-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3bfe7-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="3bfe7-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="3bfe7-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="3bfe7-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="3bfe7-158">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="3bfe7-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="3bfe7-159">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3bfe7-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3bfe7-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="3bfe7-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="3bfe7-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="3bfe7-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="3bfe7-162">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="3bfe7-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="3bfe7-163">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3bfe7-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3bfe7-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3bfe7-164">createdDateTime</span></span>|<span data-ttu-id="3bfe7-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3bfe7-165">DateTimeOffset</span></span>|<span data-ttu-id="3bfe7-166">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="3bfe7-166">DateTime the object was created.</span></span> <span data-ttu-id="3bfe7-167">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3bfe7-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3bfe7-168">说明</span><span class="sxs-lookup"><span data-stu-id="3bfe7-168">description</span></span>|<span data-ttu-id="3bfe7-169">String</span><span class="sxs-lookup"><span data-stu-id="3bfe7-169">String</span></span>|<span data-ttu-id="3bfe7-170">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="3bfe7-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="3bfe7-171">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3bfe7-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3bfe7-172">displayName</span><span class="sxs-lookup"><span data-stu-id="3bfe7-172">displayName</span></span>|<span data-ttu-id="3bfe7-173">String</span><span class="sxs-lookup"><span data-stu-id="3bfe7-173">String</span></span>|<span data-ttu-id="3bfe7-174">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="3bfe7-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="3bfe7-175">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3bfe7-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3bfe7-176">version</span><span class="sxs-lookup"><span data-stu-id="3bfe7-176">version</span></span>|<span data-ttu-id="3bfe7-177">Int32</span><span class="sxs-lookup"><span data-stu-id="3bfe7-177">Int32</span></span>|<span data-ttu-id="3bfe7-178">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="3bfe7-178">Version of the device configuration.</span></span> <span data-ttu-id="3bfe7-179">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3bfe7-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3bfe7-180">connectionName</span><span class="sxs-lookup"><span data-stu-id="3bfe7-180">connectionName</span></span>|<span data-ttu-id="3bfe7-181">String</span><span class="sxs-lookup"><span data-stu-id="3bfe7-181">String</span></span>|<span data-ttu-id="3bfe7-182">向用户显示的连接名称。</span><span class="sxs-lookup"><span data-stu-id="3bfe7-182">Connection name displayed to the user.</span></span> <span data-ttu-id="3bfe7-183">继承自 [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3bfe7-183">Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="3bfe7-184">服务器</span><span class="sxs-lookup"><span data-stu-id="3bfe7-184">servers</span></span>|<span data-ttu-id="3bfe7-185">[vpnServer](../resources/intune-deviceconfig-vpnserver.md) 集合</span><span class="sxs-lookup"><span data-stu-id="3bfe7-185">[vpnServer](../resources/intune-deviceconfig-vpnserver.md) collection</span></span>|<span data-ttu-id="3bfe7-186">网络上 VPN 服务器的列表。</span><span class="sxs-lookup"><span data-stu-id="3bfe7-186">List of VPN Servers on the network.</span></span> <span data-ttu-id="3bfe7-187">确保最终用户可以访问这些网络位置。</span><span class="sxs-lookup"><span data-stu-id="3bfe7-187">Make sure end users can access these network locations.</span></span> <span data-ttu-id="3bfe7-188">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="3bfe7-188">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="3bfe7-189">继承自 [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3bfe7-189">Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="3bfe7-190">customXml</span><span class="sxs-lookup"><span data-stu-id="3bfe7-190">customXml</span></span>|<span data-ttu-id="3bfe7-191">Binary</span><span class="sxs-lookup"><span data-stu-id="3bfe7-191">Binary</span></span>|<span data-ttu-id="3bfe7-192">配置 VPN 连接的自定义 XML 命令。</span><span class="sxs-lookup"><span data-stu-id="3bfe7-192">Custom XML commands that configures the VPN connection.</span></span> <span data-ttu-id="3bfe7-193"> (UTF8 编码的字节数组) 继承自 [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3bfe7-193">(UTF8 encoded byte array) Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="3bfe7-194">applyOnlyToWindows81</span><span class="sxs-lookup"><span data-stu-id="3bfe7-194">applyOnlyToWindows81</span></span>|<span data-ttu-id="3bfe7-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="3bfe7-195">Boolean</span></span>|<span data-ttu-id="3bfe7-196">指示此策略是否仅适用于 Windows 8.1 的值。</span><span class="sxs-lookup"><span data-stu-id="3bfe7-196">Value indicating whether this policy only applies to Windows 8.1.</span></span> <span data-ttu-id="3bfe7-197">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="3bfe7-197">This property is read-only.</span></span>|
|<span data-ttu-id="3bfe7-198">connectionType</span><span class="sxs-lookup"><span data-stu-id="3bfe7-198">connectionType</span></span>|[<span data-ttu-id="3bfe7-199">windowsVpnConnectionType</span><span class="sxs-lookup"><span data-stu-id="3bfe7-199">windowsVpnConnectionType</span></span>](../resources/intune-deviceconfig-windowsvpnconnectiontype.md)|<span data-ttu-id="3bfe7-200">连接类型。</span><span class="sxs-lookup"><span data-stu-id="3bfe7-200">Connection type.</span></span> <span data-ttu-id="3bfe7-201">可取值为：`pulseSecure`、`f5EdgeClient`、`dellSonicWallMobileConnect`、`checkPointCapsuleVpn`。</span><span class="sxs-lookup"><span data-stu-id="3bfe7-201">Possible values are: `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`.</span></span>|
|<span data-ttu-id="3bfe7-202">loginGroupOrDomain</span><span class="sxs-lookup"><span data-stu-id="3bfe7-202">loginGroupOrDomain</span></span>|<span data-ttu-id="3bfe7-203">String</span><span class="sxs-lookup"><span data-stu-id="3bfe7-203">String</span></span>|<span data-ttu-id="3bfe7-204">连接类型设置为 Dell SonicWALL 移动连接时登录组或域。</span><span class="sxs-lookup"><span data-stu-id="3bfe7-204">Login group or domain when connection type is set to Dell SonicWALL Mobile Connection.</span></span>|
|<span data-ttu-id="3bfe7-205">enableSplitTunneling</span><span class="sxs-lookup"><span data-stu-id="3bfe7-205">enableSplitTunneling</span></span>|<span data-ttu-id="3bfe7-206">Boolean</span><span class="sxs-lookup"><span data-stu-id="3bfe7-206">Boolean</span></span>|<span data-ttu-id="3bfe7-207">为 VPN 启用拆分隧道。</span><span class="sxs-lookup"><span data-stu-id="3bfe7-207">Enable split tunneling for the VPN.</span></span>|
|<span data-ttu-id="3bfe7-208">proxyServer</span><span class="sxs-lookup"><span data-stu-id="3bfe7-208">proxyServer</span></span>|[<span data-ttu-id="3bfe7-209">windows81VpnProxyServer</span><span class="sxs-lookup"><span data-stu-id="3bfe7-209">windows81VpnProxyServer</span></span>](../resources/intune-deviceconfig-windows81vpnproxyserver.md)|<span data-ttu-id="3bfe7-210">代理服务器。</span><span class="sxs-lookup"><span data-stu-id="3bfe7-210">Proxy Server.</span></span>|



## <a name="response"></a><span data-ttu-id="3bfe7-211">响应</span><span class="sxs-lookup"><span data-stu-id="3bfe7-211">Response</span></span>
<span data-ttu-id="3bfe7-212">如果成功，此方法在响应正文中返回 响应代码和 `201 Created` [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="3bfe7-212">If successful, this method returns a `201 Created` response code and a [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3bfe7-213">示例</span><span class="sxs-lookup"><span data-stu-id="3bfe7-213">Example</span></span>

### <a name="request"></a><span data-ttu-id="3bfe7-214">请求</span><span class="sxs-lookup"><span data-stu-id="3bfe7-214">Request</span></span>
<span data-ttu-id="3bfe7-215">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="3bfe7-215">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1788

{
  "@odata.type": "#microsoft.graph.windows81VpnConfiguration",
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
  }
}
```

### <a name="response"></a><span data-ttu-id="3bfe7-216">响应</span><span class="sxs-lookup"><span data-stu-id="3bfe7-216">Response</span></span>
<span data-ttu-id="3bfe7-p118">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="3bfe7-p118">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1960

{
  "@odata.type": "#microsoft.graph.windows81VpnConfiguration",
  "id": "6aa07da3-7da3-6aa0-a37d-a06aa37da06a",
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
  }
}
```




