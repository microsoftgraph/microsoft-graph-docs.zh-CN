---
title: 创建 windows81VpnConfiguration
description: 创建新的 windows81VpnConfiguration 对象。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: f448d021c1135725cd372115acca1e5a0f8a807e
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29419777"
---
# <a name="create-windows81vpnconfiguration"></a><span data-ttu-id="1fe56-103">创建 windows81VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="1fe56-103">Create windows81VpnConfiguration</span></span>

> <span data-ttu-id="1fe56-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="1fe56-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="1fe56-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="1fe56-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="1fe56-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="1fe56-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1fe56-107">创建新的[windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="1fe56-107">Create a new [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1fe56-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="1fe56-108">Prerequisites</span></span>
<span data-ttu-id="1fe56-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="1fe56-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="1fe56-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="1fe56-111">Permission type</span></span>|<span data-ttu-id="1fe56-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="1fe56-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1fe56-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1fe56-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1fe56-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1fe56-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="1fe56-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1fe56-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1fe56-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="1fe56-116">Not supported.</span></span>|
|<span data-ttu-id="1fe56-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="1fe56-117">Application</span></span>|<span data-ttu-id="1fe56-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="1fe56-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1fe56-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1fe56-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="1fe56-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="1fe56-120">Request headers</span></span>
|<span data-ttu-id="1fe56-121">标头</span><span class="sxs-lookup"><span data-stu-id="1fe56-121">Header</span></span>|<span data-ttu-id="1fe56-122">值</span><span class="sxs-lookup"><span data-stu-id="1fe56-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1fe56-123">授权</span><span class="sxs-lookup"><span data-stu-id="1fe56-123">Authorization</span></span>|<span data-ttu-id="1fe56-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="1fe56-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1fe56-125">Accept</span><span class="sxs-lookup"><span data-stu-id="1fe56-125">Accept</span></span>|<span data-ttu-id="1fe56-126">application/json</span><span class="sxs-lookup"><span data-stu-id="1fe56-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1fe56-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="1fe56-127">Request body</span></span>
<span data-ttu-id="1fe56-128">在请求正文中，提供 windows81VpnConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1fe56-128">In the request body, supply a JSON representation for the windows81VpnConfiguration object.</span></span>

<span data-ttu-id="1fe56-129">下表显示时创建 windows81VpnConfiguration 所需的属性。</span><span class="sxs-lookup"><span data-stu-id="1fe56-129">The following table shows the properties that are required when you create the windows81VpnConfiguration.</span></span>

|<span data-ttu-id="1fe56-130">属性</span><span class="sxs-lookup"><span data-stu-id="1fe56-130">Property</span></span>|<span data-ttu-id="1fe56-131">类型</span><span class="sxs-lookup"><span data-stu-id="1fe56-131">Type</span></span>|<span data-ttu-id="1fe56-132">说明</span><span class="sxs-lookup"><span data-stu-id="1fe56-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1fe56-133">id</span><span class="sxs-lookup"><span data-stu-id="1fe56-133">id</span></span>|<span data-ttu-id="1fe56-134">String</span><span class="sxs-lookup"><span data-stu-id="1fe56-134">String</span></span>|<span data-ttu-id="1fe56-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="1fe56-135">Key of the entity.</span></span> <span data-ttu-id="1fe56-136">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1fe56-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1fe56-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1fe56-137">lastModifiedDateTime</span></span>|<span data-ttu-id="1fe56-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1fe56-138">DateTimeOffset</span></span>|<span data-ttu-id="1fe56-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="1fe56-139">DateTime the object was last modified.</span></span> <span data-ttu-id="1fe56-140">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1fe56-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1fe56-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="1fe56-141">roleScopeTagIds</span></span>|<span data-ttu-id="1fe56-142">String 集合</span><span class="sxs-lookup"><span data-stu-id="1fe56-142">String collection</span></span>|<span data-ttu-id="1fe56-143">此实体实例范围标记的列表。</span><span class="sxs-lookup"><span data-stu-id="1fe56-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="1fe56-144">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1fe56-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1fe56-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="1fe56-145">supportsScopeTags</span></span>|<span data-ttu-id="1fe56-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="1fe56-146">Boolean</span></span>|<span data-ttu-id="1fe56-147">指示基础的设备配置支持分配的范围标记。</span><span class="sxs-lookup"><span data-stu-id="1fe56-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="1fe56-148">此值为 false，并且实体将不会对作用域的用户可见时，不允许将分配给 ScopeTags 属性。</span><span class="sxs-lookup"><span data-stu-id="1fe56-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="1fe56-149">这将发生在 Silverlight 中创建的旧策略，并可以解析通过删除并重新创建 Azure 门户中的策略。</span><span class="sxs-lookup"><span data-stu-id="1fe56-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="1fe56-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="1fe56-150">This property is read-only.</span></span> <span data-ttu-id="1fe56-151">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1fe56-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1fe56-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1fe56-152">createdDateTime</span></span>|<span data-ttu-id="1fe56-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1fe56-153">DateTimeOffset</span></span>|<span data-ttu-id="1fe56-154">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="1fe56-154">DateTime the object was created.</span></span> <span data-ttu-id="1fe56-155">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1fe56-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1fe56-156">description</span><span class="sxs-lookup"><span data-stu-id="1fe56-156">description</span></span>|<span data-ttu-id="1fe56-157">String</span><span class="sxs-lookup"><span data-stu-id="1fe56-157">String</span></span>|<span data-ttu-id="1fe56-158">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="1fe56-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="1fe56-159">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1fe56-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1fe56-160">displayName</span><span class="sxs-lookup"><span data-stu-id="1fe56-160">displayName</span></span>|<span data-ttu-id="1fe56-161">String</span><span class="sxs-lookup"><span data-stu-id="1fe56-161">String</span></span>|<span data-ttu-id="1fe56-162">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="1fe56-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="1fe56-163">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1fe56-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1fe56-164">version</span><span class="sxs-lookup"><span data-stu-id="1fe56-164">version</span></span>|<span data-ttu-id="1fe56-165">Int32</span><span class="sxs-lookup"><span data-stu-id="1fe56-165">Int32</span></span>|<span data-ttu-id="1fe56-166">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="1fe56-166">Version of the device configuration.</span></span> <span data-ttu-id="1fe56-167">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1fe56-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1fe56-168">connectionName</span><span class="sxs-lookup"><span data-stu-id="1fe56-168">connectionName</span></span>|<span data-ttu-id="1fe56-169">String</span><span class="sxs-lookup"><span data-stu-id="1fe56-169">String</span></span>|<span data-ttu-id="1fe56-170">向用户显示的连接名称。</span><span class="sxs-lookup"><span data-stu-id="1fe56-170">Connection name displayed to the user.</span></span> <span data-ttu-id="1fe56-171">继承自[windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1fe56-171">Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="1fe56-172">服务器</span><span class="sxs-lookup"><span data-stu-id="1fe56-172">servers</span></span>|<span data-ttu-id="1fe56-173">[vpnServer](../resources/intune-deviceconfig-vpnserver.md)集合</span><span class="sxs-lookup"><span data-stu-id="1fe56-173">[vpnServer](../resources/intune-deviceconfig-vpnserver.md) collection</span></span>|<span data-ttu-id="1fe56-174">VPN 服务器的网络上的列表。</span><span class="sxs-lookup"><span data-stu-id="1fe56-174">List of VPN Servers on the network.</span></span> <span data-ttu-id="1fe56-175">确保最终用户可以访问这些网络位置。</span><span class="sxs-lookup"><span data-stu-id="1fe56-175">Make sure end users can access these network locations.</span></span> <span data-ttu-id="1fe56-176">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="1fe56-176">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="1fe56-177">继承自[windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1fe56-177">Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="1fe56-178">customXml</span><span class="sxs-lookup"><span data-stu-id="1fe56-178">customXml</span></span>|<span data-ttu-id="1fe56-179">Binary</span><span class="sxs-lookup"><span data-stu-id="1fe56-179">Binary</span></span>|<span data-ttu-id="1fe56-180">配置 VPN 连接的自定义 XML 命令。</span><span class="sxs-lookup"><span data-stu-id="1fe56-180">Custom XML commands that configures the VPN connection.</span></span> <span data-ttu-id="1fe56-181">（UTF8 编码的字节数组）继承自[windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1fe56-181">(UTF8 encoded byte array) Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="1fe56-182">applyOnlyToWindows81</span><span class="sxs-lookup"><span data-stu-id="1fe56-182">applyOnlyToWindows81</span></span>|<span data-ttu-id="1fe56-183">Boolean</span><span class="sxs-lookup"><span data-stu-id="1fe56-183">Boolean</span></span>|<span data-ttu-id="1fe56-184">指示此策略是否仅适用于 Windows 8.1 的值。</span><span class="sxs-lookup"><span data-stu-id="1fe56-184">Value indicating whether this policy only applies to Windows 8.1.</span></span> <span data-ttu-id="1fe56-185">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="1fe56-185">This property is read-only.</span></span>|
|<span data-ttu-id="1fe56-186">连接</span><span class="sxs-lookup"><span data-stu-id="1fe56-186">connectionType</span></span>|[<span data-ttu-id="1fe56-187">windowsVpnConnectionType</span><span class="sxs-lookup"><span data-stu-id="1fe56-187">windowsVpnConnectionType</span></span>](../resources/intune-deviceconfig-windowsvpnconnectiontype.md)|<span data-ttu-id="1fe56-188">连接类型。</span><span class="sxs-lookup"><span data-stu-id="1fe56-188">Connection type.</span></span> <span data-ttu-id="1fe56-189">可取值为：`pulseSecure`、`f5EdgeClient`、`dellSonicWallMobileConnect`、`checkPointCapsuleVpn`。</span><span class="sxs-lookup"><span data-stu-id="1fe56-189">Possible values are: `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`.</span></span>|
|<span data-ttu-id="1fe56-190">loginGroupOrDomain</span><span class="sxs-lookup"><span data-stu-id="1fe56-190">loginGroupOrDomain</span></span>|<span data-ttu-id="1fe56-191">String</span><span class="sxs-lookup"><span data-stu-id="1fe56-191">String</span></span>|<span data-ttu-id="1fe56-192">登录组或域时连接类型设置为 Dell 使 SonicWALL Mobile 连接。</span><span class="sxs-lookup"><span data-stu-id="1fe56-192">Login group or domain when connection type is set to Dell SonicWALL Mobile Connection.</span></span>|
|<span data-ttu-id="1fe56-193">enableSplitTunneling</span><span class="sxs-lookup"><span data-stu-id="1fe56-193">enableSplitTunneling</span></span>|<span data-ttu-id="1fe56-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="1fe56-194">Boolean</span></span>|<span data-ttu-id="1fe56-195">启用拆分隧道的 VPN。</span><span class="sxs-lookup"><span data-stu-id="1fe56-195">Enable split tunneling for the VPN.</span></span>|
|<span data-ttu-id="1fe56-196">代理服务器</span><span class="sxs-lookup"><span data-stu-id="1fe56-196">proxyServer</span></span>|[<span data-ttu-id="1fe56-197">windows81VpnProxyServer</span><span class="sxs-lookup"><span data-stu-id="1fe56-197">windows81VpnProxyServer</span></span>](../resources/intune-deviceconfig-windows81vpnproxyserver.md)|<span data-ttu-id="1fe56-198">代理服务器。</span><span class="sxs-lookup"><span data-stu-id="1fe56-198">Proxy Server.</span></span>|



## <a name="response"></a><span data-ttu-id="1fe56-199">响应</span><span class="sxs-lookup"><span data-stu-id="1fe56-199">Response</span></span>
<span data-ttu-id="1fe56-200">如果成功，此方法返回`201 Created`响应代码和响应正文中的[windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="1fe56-200">If successful, this method returns a `201 Created` response code and a [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1fe56-201">示例</span><span class="sxs-lookup"><span data-stu-id="1fe56-201">Example</span></span>

### <a name="request"></a><span data-ttu-id="1fe56-202">请求</span><span class="sxs-lookup"><span data-stu-id="1fe56-202">Request</span></span>
<span data-ttu-id="1fe56-203">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="1fe56-203">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
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

### <a name="response"></a><span data-ttu-id="1fe56-204">响应</span><span class="sxs-lookup"><span data-stu-id="1fe56-204">Response</span></span>
<span data-ttu-id="1fe56-p116">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="1fe56-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




