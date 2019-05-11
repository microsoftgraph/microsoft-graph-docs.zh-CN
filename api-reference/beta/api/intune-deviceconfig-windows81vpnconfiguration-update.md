---
title: 更新 windows81VpnConfiguration
description: 更新 windows81VpnConfiguration 对象的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e8a874138880610a2eb25caa49aa1943da646829
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2019
ms.locfileid: "33918155"
---
# <a name="update-windows81vpnconfiguration"></a><span data-ttu-id="1981d-103">更新 windows81VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="1981d-103">Update windows81VpnConfiguration</span></span>

> <span data-ttu-id="1981d-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="1981d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1981d-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="1981d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1981d-106">更新[windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="1981d-106">Update the properties of a [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1981d-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="1981d-107">Prerequisites</span></span>
<span data-ttu-id="1981d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="1981d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1981d-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="1981d-110">Permission type</span></span>|<span data-ttu-id="1981d-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="1981d-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1981d-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1981d-112">Delegated (work or school account)</span></span>|<span data-ttu-id="1981d-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1981d-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="1981d-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1981d-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1981d-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="1981d-115">Not supported.</span></span>|
|<span data-ttu-id="1981d-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="1981d-116">Application</span></span>|<span data-ttu-id="1981d-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="1981d-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1981d-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1981d-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="1981d-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="1981d-119">Request headers</span></span>
|<span data-ttu-id="1981d-120">标头</span><span class="sxs-lookup"><span data-stu-id="1981d-120">Header</span></span>|<span data-ttu-id="1981d-121">值</span><span class="sxs-lookup"><span data-stu-id="1981d-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1981d-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="1981d-122">Authorization</span></span>|<span data-ttu-id="1981d-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="1981d-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1981d-124">接受</span><span class="sxs-lookup"><span data-stu-id="1981d-124">Accept</span></span>|<span data-ttu-id="1981d-125">application/json</span><span class="sxs-lookup"><span data-stu-id="1981d-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1981d-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="1981d-126">Request body</span></span>
<span data-ttu-id="1981d-127">在请求正文中, 提供[windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1981d-127">In the request body, supply a JSON representation for the [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md) object.</span></span>

<span data-ttu-id="1981d-128">下表显示创建[windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="1981d-128">The following table shows the properties that are required when you create the [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md).</span></span>

|<span data-ttu-id="1981d-129">属性</span><span class="sxs-lookup"><span data-stu-id="1981d-129">Property</span></span>|<span data-ttu-id="1981d-130">类型</span><span class="sxs-lookup"><span data-stu-id="1981d-130">Type</span></span>|<span data-ttu-id="1981d-131">说明</span><span class="sxs-lookup"><span data-stu-id="1981d-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1981d-132">id</span><span class="sxs-lookup"><span data-stu-id="1981d-132">id</span></span>|<span data-ttu-id="1981d-133">字符串</span><span class="sxs-lookup"><span data-stu-id="1981d-133">String</span></span>|<span data-ttu-id="1981d-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="1981d-134">Key of the entity.</span></span> <span data-ttu-id="1981d-135">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1981d-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1981d-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1981d-136">lastModifiedDateTime</span></span>|<span data-ttu-id="1981d-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1981d-137">DateTimeOffset</span></span>|<span data-ttu-id="1981d-138">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="1981d-138">DateTime the object was last modified.</span></span> <span data-ttu-id="1981d-139">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1981d-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1981d-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="1981d-140">roleScopeTagIds</span></span>|<span data-ttu-id="1981d-141">String collection</span><span class="sxs-lookup"><span data-stu-id="1981d-141">String collection</span></span>|<span data-ttu-id="1981d-142">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="1981d-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="1981d-143">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1981d-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1981d-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="1981d-144">supportsScopeTags</span></span>|<span data-ttu-id="1981d-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="1981d-145">Boolean</span></span>|<span data-ttu-id="1981d-146">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="1981d-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="1981d-147">如果此值为 false, 则不允许分配给 ScopeTags 属性, 并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="1981d-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="1981d-148">这适用于在 Silverlight 中创建的旧版策略, 可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="1981d-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="1981d-149">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="1981d-149">This property is read-only.</span></span> <span data-ttu-id="1981d-150">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1981d-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1981d-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1981d-151">createdDateTime</span></span>|<span data-ttu-id="1981d-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1981d-152">DateTimeOffset</span></span>|<span data-ttu-id="1981d-153">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="1981d-153">DateTime the object was created.</span></span> <span data-ttu-id="1981d-154">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1981d-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1981d-155">说明</span><span class="sxs-lookup"><span data-stu-id="1981d-155">description</span></span>|<span data-ttu-id="1981d-156">String</span><span class="sxs-lookup"><span data-stu-id="1981d-156">String</span></span>|<span data-ttu-id="1981d-157">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="1981d-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="1981d-158">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1981d-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1981d-159">displayName</span><span class="sxs-lookup"><span data-stu-id="1981d-159">displayName</span></span>|<span data-ttu-id="1981d-160">String</span><span class="sxs-lookup"><span data-stu-id="1981d-160">String</span></span>|<span data-ttu-id="1981d-161">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="1981d-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="1981d-162">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1981d-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1981d-163">version</span><span class="sxs-lookup"><span data-stu-id="1981d-163">version</span></span>|<span data-ttu-id="1981d-164">Int32</span><span class="sxs-lookup"><span data-stu-id="1981d-164">Int32</span></span>|<span data-ttu-id="1981d-165">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="1981d-165">Version of the device configuration.</span></span> <span data-ttu-id="1981d-166">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1981d-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1981d-167">connectionName</span><span class="sxs-lookup"><span data-stu-id="1981d-167">connectionName</span></span>|<span data-ttu-id="1981d-168">String</span><span class="sxs-lookup"><span data-stu-id="1981d-168">String</span></span>|<span data-ttu-id="1981d-169">向用户显示的连接名称。</span><span class="sxs-lookup"><span data-stu-id="1981d-169">Connection name displayed to the user.</span></span> <span data-ttu-id="1981d-170">继承自[windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1981d-170">Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="1981d-171">台</span><span class="sxs-lookup"><span data-stu-id="1981d-171">servers</span></span>|<span data-ttu-id="1981d-172">[vpnServer](../resources/intune-deviceconfig-vpnserver.md)集合</span><span class="sxs-lookup"><span data-stu-id="1981d-172">[vpnServer](../resources/intune-deviceconfig-vpnserver.md) collection</span></span>|<span data-ttu-id="1981d-173">网络上的 VPN 服务器的列表。</span><span class="sxs-lookup"><span data-stu-id="1981d-173">List of VPN Servers on the network.</span></span> <span data-ttu-id="1981d-174">请确保最终用户可以访问这些网络位置。</span><span class="sxs-lookup"><span data-stu-id="1981d-174">Make sure end users can access these network locations.</span></span> <span data-ttu-id="1981d-175">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="1981d-175">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="1981d-176">继承自[windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1981d-176">Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="1981d-177">customXml</span><span class="sxs-lookup"><span data-stu-id="1981d-177">customXml</span></span>|<span data-ttu-id="1981d-178">Binary</span><span class="sxs-lookup"><span data-stu-id="1981d-178">Binary</span></span>|<span data-ttu-id="1981d-179">配置 VPN 连接的自定义 XML 命令。</span><span class="sxs-lookup"><span data-stu-id="1981d-179">Custom XML commands that configures the VPN connection.</span></span> <span data-ttu-id="1981d-180">(UTF8 编码的字节数组)继承自[windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1981d-180">(UTF8 encoded byte array) Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="1981d-181">applyOnlyToWindows81</span><span class="sxs-lookup"><span data-stu-id="1981d-181">applyOnlyToWindows81</span></span>|<span data-ttu-id="1981d-182">Boolean</span><span class="sxs-lookup"><span data-stu-id="1981d-182">Boolean</span></span>|<span data-ttu-id="1981d-183">指示此策略是否仅适用于 Windows 8.1 的值。</span><span class="sxs-lookup"><span data-stu-id="1981d-183">Value indicating whether this policy only applies to Windows 8.1.</span></span> <span data-ttu-id="1981d-184">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="1981d-184">This property is read-only.</span></span>|
|<span data-ttu-id="1981d-185">connectionType</span><span class="sxs-lookup"><span data-stu-id="1981d-185">connectionType</span></span>|[<span data-ttu-id="1981d-186">windowsVpnConnectionType</span><span class="sxs-lookup"><span data-stu-id="1981d-186">windowsVpnConnectionType</span></span>](../resources/intune-deviceconfig-windowsvpnconnectiontype.md)|<span data-ttu-id="1981d-187">连接类型。</span><span class="sxs-lookup"><span data-stu-id="1981d-187">Connection type.</span></span> <span data-ttu-id="1981d-188">可取值为：`pulseSecure`、`f5EdgeClient`、`dellSonicWallMobileConnect`、`checkPointCapsuleVpn`。</span><span class="sxs-lookup"><span data-stu-id="1981d-188">Possible values are: `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`.</span></span>|
|<span data-ttu-id="1981d-189">loginGroupOrDomain</span><span class="sxs-lookup"><span data-stu-id="1981d-189">loginGroupOrDomain</span></span>|<span data-ttu-id="1981d-190">String</span><span class="sxs-lookup"><span data-stu-id="1981d-190">String</span></span>|<span data-ttu-id="1981d-191">将连接类型设置为 Dell SonicWALL Mobile 连接时的登录组或域。</span><span class="sxs-lookup"><span data-stu-id="1981d-191">Login group or domain when connection type is set to Dell SonicWALL Mobile Connection.</span></span>|
|<span data-ttu-id="1981d-192">enableSplitTunneling</span><span class="sxs-lookup"><span data-stu-id="1981d-192">enableSplitTunneling</span></span>|<span data-ttu-id="1981d-193">Boolean</span><span class="sxs-lookup"><span data-stu-id="1981d-193">Boolean</span></span>|<span data-ttu-id="1981d-194">为 VPN 启用拆分隧道。</span><span class="sxs-lookup"><span data-stu-id="1981d-194">Enable split tunneling for the VPN.</span></span>|
|<span data-ttu-id="1981d-195">proxyServer</span><span class="sxs-lookup"><span data-stu-id="1981d-195">proxyServer</span></span>|[<span data-ttu-id="1981d-196">windows81VpnProxyServer</span><span class="sxs-lookup"><span data-stu-id="1981d-196">windows81VpnProxyServer</span></span>](../resources/intune-deviceconfig-windows81vpnproxyserver.md)|<span data-ttu-id="1981d-197">代理服务器。</span><span class="sxs-lookup"><span data-stu-id="1981d-197">Proxy Server.</span></span>|



## <a name="response"></a><span data-ttu-id="1981d-198">响应</span><span class="sxs-lookup"><span data-stu-id="1981d-198">Response</span></span>
<span data-ttu-id="1981d-199">如果成功, 此方法在响应`200 OK`正文中返回响应代码和更新的[windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="1981d-199">If successful, this method returns a `200 OK` response code and an updated [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1981d-200">示例</span><span class="sxs-lookup"><span data-stu-id="1981d-200">Example</span></span>

### <a name="request"></a><span data-ttu-id="1981d-201">请求</span><span class="sxs-lookup"><span data-stu-id="1981d-201">Request</span></span>
<span data-ttu-id="1981d-202">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="1981d-202">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1015

{
  "@odata.type": "#microsoft.graph.windows81VpnConfiguration",
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
  }
}
```

### <a name="response"></a><span data-ttu-id="1981d-203">响应</span><span class="sxs-lookup"><span data-stu-id="1981d-203">Response</span></span>
<span data-ttu-id="1981d-p115">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="1981d-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1187

{
  "@odata.type": "#microsoft.graph.windows81VpnConfiguration",
  "id": "6aa07da3-7da3-6aa0-a37d-a06aa37da06a",
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
  }
}
```




