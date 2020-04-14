---
title: 更新 windows81VpnConfiguration
description: 更新 windows81VpnConfiguration 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: e7d15210ddbb6c9b00e5b36b0327b0a0551290f1
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43430157"
---
# <a name="update-windows81vpnconfiguration"></a><span data-ttu-id="1f745-103">更新 windows81VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="1f745-103">Update windows81VpnConfiguration</span></span>

<span data-ttu-id="1f745-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1f745-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1f745-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="1f745-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1f745-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="1f745-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1f745-107">更新[windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="1f745-107">Update the properties of a [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1f745-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="1f745-108">Prerequisites</span></span>
<span data-ttu-id="1f745-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="1f745-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1f745-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="1f745-111">Permission type</span></span>|<span data-ttu-id="1f745-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="1f745-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1f745-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1f745-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1f745-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1f745-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="1f745-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1f745-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1f745-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="1f745-116">Not supported.</span></span>|
|<span data-ttu-id="1f745-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="1f745-117">Application</span></span>|<span data-ttu-id="1f745-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1f745-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1f745-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1f745-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="1f745-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="1f745-120">Request headers</span></span>
|<span data-ttu-id="1f745-121">标头</span><span class="sxs-lookup"><span data-stu-id="1f745-121">Header</span></span>|<span data-ttu-id="1f745-122">值</span><span class="sxs-lookup"><span data-stu-id="1f745-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1f745-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="1f745-123">Authorization</span></span>|<span data-ttu-id="1f745-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="1f745-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1f745-125">接受</span><span class="sxs-lookup"><span data-stu-id="1f745-125">Accept</span></span>|<span data-ttu-id="1f745-126">application/json</span><span class="sxs-lookup"><span data-stu-id="1f745-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1f745-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="1f745-127">Request body</span></span>
<span data-ttu-id="1f745-128">在请求正文中，提供[windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1f745-128">In the request body, supply a JSON representation for the [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md) object.</span></span>

<span data-ttu-id="1f745-129">下表显示创建[windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="1f745-129">The following table shows the properties that are required when you create the [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md).</span></span>

|<span data-ttu-id="1f745-130">属性</span><span class="sxs-lookup"><span data-stu-id="1f745-130">Property</span></span>|<span data-ttu-id="1f745-131">类型</span><span class="sxs-lookup"><span data-stu-id="1f745-131">Type</span></span>|<span data-ttu-id="1f745-132">说明</span><span class="sxs-lookup"><span data-stu-id="1f745-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1f745-133">id</span><span class="sxs-lookup"><span data-stu-id="1f745-133">id</span></span>|<span data-ttu-id="1f745-134">字符串</span><span class="sxs-lookup"><span data-stu-id="1f745-134">String</span></span>|<span data-ttu-id="1f745-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="1f745-135">Key of the entity.</span></span> <span data-ttu-id="1f745-136">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1f745-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1f745-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1f745-137">lastModifiedDateTime</span></span>|<span data-ttu-id="1f745-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1f745-138">DateTimeOffset</span></span>|<span data-ttu-id="1f745-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="1f745-139">DateTime the object was last modified.</span></span> <span data-ttu-id="1f745-140">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1f745-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1f745-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="1f745-141">roleScopeTagIds</span></span>|<span data-ttu-id="1f745-142">String 集合</span><span class="sxs-lookup"><span data-stu-id="1f745-142">String collection</span></span>|<span data-ttu-id="1f745-143">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="1f745-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="1f745-144">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1f745-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1f745-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="1f745-145">supportsScopeTags</span></span>|<span data-ttu-id="1f745-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="1f745-146">Boolean</span></span>|<span data-ttu-id="1f745-147">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="1f745-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="1f745-148">如果此值为 false，则不允许分配给 ScopeTags 属性，并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="1f745-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="1f745-149">这适用于在 Silverlight 中创建的旧版策略，可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="1f745-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="1f745-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="1f745-150">This property is read-only.</span></span> <span data-ttu-id="1f745-151">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1f745-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1f745-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="1f745-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="1f745-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="1f745-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="1f745-154">适用于此策略的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="1f745-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="1f745-155">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1f745-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1f745-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="1f745-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="1f745-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="1f745-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="1f745-158">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="1f745-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="1f745-159">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1f745-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1f745-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="1f745-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="1f745-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="1f745-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="1f745-162">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="1f745-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="1f745-163">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1f745-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1f745-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1f745-164">createdDateTime</span></span>|<span data-ttu-id="1f745-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1f745-165">DateTimeOffset</span></span>|<span data-ttu-id="1f745-166">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="1f745-166">DateTime the object was created.</span></span> <span data-ttu-id="1f745-167">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1f745-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1f745-168">description</span><span class="sxs-lookup"><span data-stu-id="1f745-168">description</span></span>|<span data-ttu-id="1f745-169">String</span><span class="sxs-lookup"><span data-stu-id="1f745-169">String</span></span>|<span data-ttu-id="1f745-170">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="1f745-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="1f745-171">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1f745-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1f745-172">displayName</span><span class="sxs-lookup"><span data-stu-id="1f745-172">displayName</span></span>|<span data-ttu-id="1f745-173">String</span><span class="sxs-lookup"><span data-stu-id="1f745-173">String</span></span>|<span data-ttu-id="1f745-174">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="1f745-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="1f745-175">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1f745-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1f745-176">version</span><span class="sxs-lookup"><span data-stu-id="1f745-176">version</span></span>|<span data-ttu-id="1f745-177">Int32</span><span class="sxs-lookup"><span data-stu-id="1f745-177">Int32</span></span>|<span data-ttu-id="1f745-178">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="1f745-178">Version of the device configuration.</span></span> <span data-ttu-id="1f745-179">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1f745-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1f745-180">connectionName</span><span class="sxs-lookup"><span data-stu-id="1f745-180">connectionName</span></span>|<span data-ttu-id="1f745-181">String</span><span class="sxs-lookup"><span data-stu-id="1f745-181">String</span></span>|<span data-ttu-id="1f745-182">向用户显示的连接名称。</span><span class="sxs-lookup"><span data-stu-id="1f745-182">Connection name displayed to the user.</span></span> <span data-ttu-id="1f745-183">继承自[windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1f745-183">Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="1f745-184">台</span><span class="sxs-lookup"><span data-stu-id="1f745-184">servers</span></span>|<span data-ttu-id="1f745-185">[vpnServer](../resources/intune-deviceconfig-vpnserver.md)集合</span><span class="sxs-lookup"><span data-stu-id="1f745-185">[vpnServer](../resources/intune-deviceconfig-vpnserver.md) collection</span></span>|<span data-ttu-id="1f745-186">网络上的 VPN 服务器的列表。</span><span class="sxs-lookup"><span data-stu-id="1f745-186">List of VPN Servers on the network.</span></span> <span data-ttu-id="1f745-187">请确保最终用户可以访问这些网络位置。</span><span class="sxs-lookup"><span data-stu-id="1f745-187">Make sure end users can access these network locations.</span></span> <span data-ttu-id="1f745-188">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="1f745-188">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="1f745-189">继承自[windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1f745-189">Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="1f745-190">customXml</span><span class="sxs-lookup"><span data-stu-id="1f745-190">customXml</span></span>|<span data-ttu-id="1f745-191">Binary</span><span class="sxs-lookup"><span data-stu-id="1f745-191">Binary</span></span>|<span data-ttu-id="1f745-192">配置 VPN 连接的自定义 XML 命令。</span><span class="sxs-lookup"><span data-stu-id="1f745-192">Custom XML commands that configures the VPN connection.</span></span> <span data-ttu-id="1f745-193">（UTF8 编码的字节数组）继承自[windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1f745-193">(UTF8 encoded byte array) Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="1f745-194">applyOnlyToWindows81</span><span class="sxs-lookup"><span data-stu-id="1f745-194">applyOnlyToWindows81</span></span>|<span data-ttu-id="1f745-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="1f745-195">Boolean</span></span>|<span data-ttu-id="1f745-196">指示此策略是否仅适用于 Windows 8.1 的值。</span><span class="sxs-lookup"><span data-stu-id="1f745-196">Value indicating whether this policy only applies to Windows 8.1.</span></span> <span data-ttu-id="1f745-197">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="1f745-197">This property is read-only.</span></span>|
|<span data-ttu-id="1f745-198">connectionType</span><span class="sxs-lookup"><span data-stu-id="1f745-198">connectionType</span></span>|[<span data-ttu-id="1f745-199">windowsVpnConnectionType</span><span class="sxs-lookup"><span data-stu-id="1f745-199">windowsVpnConnectionType</span></span>](../resources/intune-deviceconfig-windowsvpnconnectiontype.md)|<span data-ttu-id="1f745-200">连接类型。</span><span class="sxs-lookup"><span data-stu-id="1f745-200">Connection type.</span></span> <span data-ttu-id="1f745-201">可取值为：`pulseSecure`、`f5EdgeClient`、`dellSonicWallMobileConnect`、`checkPointCapsuleVpn`。</span><span class="sxs-lookup"><span data-stu-id="1f745-201">Possible values are: `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`.</span></span>|
|<span data-ttu-id="1f745-202">loginGroupOrDomain</span><span class="sxs-lookup"><span data-stu-id="1f745-202">loginGroupOrDomain</span></span>|<span data-ttu-id="1f745-203">String</span><span class="sxs-lookup"><span data-stu-id="1f745-203">String</span></span>|<span data-ttu-id="1f745-204">将连接类型设置为 Dell SonicWALL Mobile 连接时的登录组或域。</span><span class="sxs-lookup"><span data-stu-id="1f745-204">Login group or domain when connection type is set to Dell SonicWALL Mobile Connection.</span></span>|
|<span data-ttu-id="1f745-205">enableSplitTunneling</span><span class="sxs-lookup"><span data-stu-id="1f745-205">enableSplitTunneling</span></span>|<span data-ttu-id="1f745-206">Boolean</span><span class="sxs-lookup"><span data-stu-id="1f745-206">Boolean</span></span>|<span data-ttu-id="1f745-207">为 VPN 启用拆分隧道。</span><span class="sxs-lookup"><span data-stu-id="1f745-207">Enable split tunneling for the VPN.</span></span>|
|<span data-ttu-id="1f745-208">proxyServer</span><span class="sxs-lookup"><span data-stu-id="1f745-208">proxyServer</span></span>|[<span data-ttu-id="1f745-209">windows81VpnProxyServer</span><span class="sxs-lookup"><span data-stu-id="1f745-209">windows81VpnProxyServer</span></span>](../resources/intune-deviceconfig-windows81vpnproxyserver.md)|<span data-ttu-id="1f745-210">代理服务器。</span><span class="sxs-lookup"><span data-stu-id="1f745-210">Proxy Server.</span></span>|



## <a name="response"></a><span data-ttu-id="1f745-211">响应</span><span class="sxs-lookup"><span data-stu-id="1f745-211">Response</span></span>
<span data-ttu-id="1f745-212">如果成功，此方法在响应`200 OK`正文中返回响应代码和更新的[windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="1f745-212">If successful, this method returns a `200 OK` response code and an updated [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1f745-213">示例</span><span class="sxs-lookup"><span data-stu-id="1f745-213">Example</span></span>

### <a name="request"></a><span data-ttu-id="1f745-214">请求</span><span class="sxs-lookup"><span data-stu-id="1f745-214">Request</span></span>
<span data-ttu-id="1f745-215">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="1f745-215">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
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

### <a name="response"></a><span data-ttu-id="1f745-216">响应</span><span class="sxs-lookup"><span data-stu-id="1f745-216">Response</span></span>
<span data-ttu-id="1f745-p118">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="1f745-p118">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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



