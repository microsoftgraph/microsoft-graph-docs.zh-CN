---
title: 创建 windows81VpnConfiguration
description: 创建新的 windows81VpnConfiguration 对象。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: e036ac960cf90d11987f88a19137b443dd4e178c
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27975909"
---
# <a name="create-windows81vpnconfiguration"></a><span data-ttu-id="0517d-103">创建 windows81VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="0517d-103">Create windows81VpnConfiguration</span></span>

> <span data-ttu-id="0517d-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="0517d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0517d-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="0517d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0517d-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="0517d-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0517d-107">创建新的[windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="0517d-107">Create a new [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="0517d-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="0517d-108">Prerequisites</span></span>
<span data-ttu-id="0517d-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="0517d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0517d-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="0517d-111">Permission type</span></span>|<span data-ttu-id="0517d-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="0517d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0517d-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0517d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0517d-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0517d-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="0517d-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0517d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0517d-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="0517d-116">Not supported.</span></span>|
|<span data-ttu-id="0517d-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="0517d-117">Application</span></span>|<span data-ttu-id="0517d-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="0517d-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0517d-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0517d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="0517d-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="0517d-120">Request headers</span></span>
|<span data-ttu-id="0517d-121">标头</span><span class="sxs-lookup"><span data-stu-id="0517d-121">Header</span></span>|<span data-ttu-id="0517d-122">值</span><span class="sxs-lookup"><span data-stu-id="0517d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0517d-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="0517d-123">Authorization</span></span>|<span data-ttu-id="0517d-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="0517d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0517d-125">Accept</span><span class="sxs-lookup"><span data-stu-id="0517d-125">Accept</span></span>|<span data-ttu-id="0517d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0517d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0517d-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="0517d-127">Request body</span></span>
<span data-ttu-id="0517d-128">在请求正文中，提供 windows81VpnConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0517d-128">In the request body, supply a JSON representation for the windows81VpnConfiguration object.</span></span>

<span data-ttu-id="0517d-129">下表显示时创建 windows81VpnConfiguration 所需的属性。</span><span class="sxs-lookup"><span data-stu-id="0517d-129">The following table shows the properties that are required when you create the windows81VpnConfiguration.</span></span>

|<span data-ttu-id="0517d-130">属性</span><span class="sxs-lookup"><span data-stu-id="0517d-130">Property</span></span>|<span data-ttu-id="0517d-131">类型</span><span class="sxs-lookup"><span data-stu-id="0517d-131">Type</span></span>|<span data-ttu-id="0517d-132">说明</span><span class="sxs-lookup"><span data-stu-id="0517d-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0517d-133">id</span><span class="sxs-lookup"><span data-stu-id="0517d-133">id</span></span>|<span data-ttu-id="0517d-134">String</span><span class="sxs-lookup"><span data-stu-id="0517d-134">String</span></span>|<span data-ttu-id="0517d-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="0517d-135">Key of the entity.</span></span> <span data-ttu-id="0517d-136">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0517d-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0517d-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0517d-137">lastModifiedDateTime</span></span>|<span data-ttu-id="0517d-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0517d-138">DateTimeOffset</span></span>|<span data-ttu-id="0517d-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="0517d-139">DateTime the object was last modified.</span></span> <span data-ttu-id="0517d-140">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0517d-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0517d-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="0517d-141">roleScopeTagIds</span></span>|<span data-ttu-id="0517d-142">String 集合</span><span class="sxs-lookup"><span data-stu-id="0517d-142">String collection</span></span>|<span data-ttu-id="0517d-143">此实体实例范围标记的列表。</span><span class="sxs-lookup"><span data-stu-id="0517d-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="0517d-144">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0517d-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0517d-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="0517d-145">supportsScopeTags</span></span>|<span data-ttu-id="0517d-146">布尔</span><span class="sxs-lookup"><span data-stu-id="0517d-146">Boolean</span></span>|<span data-ttu-id="0517d-147">指示基础的设备配置支持分配的范围标记。</span><span class="sxs-lookup"><span data-stu-id="0517d-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="0517d-148">此值为 false，并且实体将不会对作用域的用户可见时，不允许将分配给 ScopeTags 属性。</span><span class="sxs-lookup"><span data-stu-id="0517d-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="0517d-149">这将发生在 Silverlight 中创建的旧策略，并可以解析通过删除并重新创建 Azure 门户中的策略。</span><span class="sxs-lookup"><span data-stu-id="0517d-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="0517d-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="0517d-150">This property is read-only.</span></span> <span data-ttu-id="0517d-151">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0517d-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0517d-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0517d-152">createdDateTime</span></span>|<span data-ttu-id="0517d-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0517d-153">DateTimeOffset</span></span>|<span data-ttu-id="0517d-154">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="0517d-154">DateTime the object was created.</span></span> <span data-ttu-id="0517d-155">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0517d-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0517d-156">description</span><span class="sxs-lookup"><span data-stu-id="0517d-156">description</span></span>|<span data-ttu-id="0517d-157">String</span><span class="sxs-lookup"><span data-stu-id="0517d-157">String</span></span>|<span data-ttu-id="0517d-158">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="0517d-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="0517d-159">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0517d-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0517d-160">displayName</span><span class="sxs-lookup"><span data-stu-id="0517d-160">displayName</span></span>|<span data-ttu-id="0517d-161">String</span><span class="sxs-lookup"><span data-stu-id="0517d-161">String</span></span>|<span data-ttu-id="0517d-162">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="0517d-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="0517d-163">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0517d-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0517d-164">version</span><span class="sxs-lookup"><span data-stu-id="0517d-164">version</span></span>|<span data-ttu-id="0517d-165">Int32</span><span class="sxs-lookup"><span data-stu-id="0517d-165">Int32</span></span>|<span data-ttu-id="0517d-166">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="0517d-166">Version of the device configuration.</span></span> <span data-ttu-id="0517d-167">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0517d-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0517d-168">connectionName</span><span class="sxs-lookup"><span data-stu-id="0517d-168">connectionName</span></span>|<span data-ttu-id="0517d-169">字符串</span><span class="sxs-lookup"><span data-stu-id="0517d-169">String</span></span>|<span data-ttu-id="0517d-170">向用户显示的连接名称。</span><span class="sxs-lookup"><span data-stu-id="0517d-170">Connection name displayed to the user.</span></span> <span data-ttu-id="0517d-171">继承自[windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0517d-171">Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="0517d-172">服务器</span><span class="sxs-lookup"><span data-stu-id="0517d-172">servers</span></span>|<span data-ttu-id="0517d-173">[vpnServer](../resources/intune-deviceconfig-vpnserver.md)集合</span><span class="sxs-lookup"><span data-stu-id="0517d-173">[vpnServer](../resources/intune-deviceconfig-vpnserver.md) collection</span></span>|<span data-ttu-id="0517d-174">VPN 服务器的网络上的列表。</span><span class="sxs-lookup"><span data-stu-id="0517d-174">List of VPN Servers on the network.</span></span> <span data-ttu-id="0517d-175">确保最终用户可以访问这些网络位置。</span><span class="sxs-lookup"><span data-stu-id="0517d-175">Make sure end users can access these network locations.</span></span> <span data-ttu-id="0517d-176">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="0517d-176">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="0517d-177">继承自[windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0517d-177">Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="0517d-178">customXml</span><span class="sxs-lookup"><span data-stu-id="0517d-178">customXml</span></span>|<span data-ttu-id="0517d-179">Binary</span><span class="sxs-lookup"><span data-stu-id="0517d-179">Binary</span></span>|<span data-ttu-id="0517d-180">配置 VPN 连接的自定义 XML 命令。</span><span class="sxs-lookup"><span data-stu-id="0517d-180">Custom XML commands that configures the VPN connection.</span></span> <span data-ttu-id="0517d-181">（UTF8 编码的字节数组）继承自[windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0517d-181">(UTF8 encoded byte array) Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="0517d-182">applyOnlyToWindows81</span><span class="sxs-lookup"><span data-stu-id="0517d-182">applyOnlyToWindows81</span></span>|<span data-ttu-id="0517d-183">Boolean</span><span class="sxs-lookup"><span data-stu-id="0517d-183">Boolean</span></span>|<span data-ttu-id="0517d-184">指示此策略是否仅适用于 Windows 8.1 的值。</span><span class="sxs-lookup"><span data-stu-id="0517d-184">Value indicating whether this policy only applies to Windows 8.1.</span></span> <span data-ttu-id="0517d-185">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="0517d-185">This property is read-only.</span></span>|
|<span data-ttu-id="0517d-186">连接</span><span class="sxs-lookup"><span data-stu-id="0517d-186">connectionType</span></span>|[<span data-ttu-id="0517d-187">windowsVpnConnectionType</span><span class="sxs-lookup"><span data-stu-id="0517d-187">windowsVpnConnectionType</span></span>](../resources/intune-deviceconfig-windowsvpnconnectiontype.md)|<span data-ttu-id="0517d-188">连接类型。</span><span class="sxs-lookup"><span data-stu-id="0517d-188">Connection type.</span></span> <span data-ttu-id="0517d-189">可取值为：`pulseSecure`、`f5EdgeClient`、`dellSonicWallMobileConnect`、`checkPointCapsuleVpn`。</span><span class="sxs-lookup"><span data-stu-id="0517d-189">Possible values are: `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`.</span></span>|
|<span data-ttu-id="0517d-190">loginGroupOrDomain</span><span class="sxs-lookup"><span data-stu-id="0517d-190">loginGroupOrDomain</span></span>|<span data-ttu-id="0517d-191">字符串</span><span class="sxs-lookup"><span data-stu-id="0517d-191">String</span></span>|<span data-ttu-id="0517d-192">登录组或域时连接类型设置为 Dell 使 SonicWALL Mobile 连接。</span><span class="sxs-lookup"><span data-stu-id="0517d-192">Login group or domain when connection type is set to Dell SonicWALL Mobile Connection.</span></span>|
|<span data-ttu-id="0517d-193">enableSplitTunneling</span><span class="sxs-lookup"><span data-stu-id="0517d-193">enableSplitTunneling</span></span>|<span data-ttu-id="0517d-194">布尔</span><span class="sxs-lookup"><span data-stu-id="0517d-194">Boolean</span></span>|<span data-ttu-id="0517d-195">启用拆分隧道的 VPN。</span><span class="sxs-lookup"><span data-stu-id="0517d-195">Enable split tunneling for the VPN.</span></span>|
|<span data-ttu-id="0517d-196">代理服务器</span><span class="sxs-lookup"><span data-stu-id="0517d-196">proxyServer</span></span>|[<span data-ttu-id="0517d-197">windows81VpnProxyServer</span><span class="sxs-lookup"><span data-stu-id="0517d-197">windows81VpnProxyServer</span></span>](../resources/intune-deviceconfig-windows81vpnproxyserver.md)|<span data-ttu-id="0517d-198">代理服务器。</span><span class="sxs-lookup"><span data-stu-id="0517d-198">Proxy Server.</span></span>|



## <a name="response"></a><span data-ttu-id="0517d-199">响应</span><span class="sxs-lookup"><span data-stu-id="0517d-199">Response</span></span>
<span data-ttu-id="0517d-200">如果成功，此方法返回`201 Created`响应代码和响应正文中的[windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="0517d-200">If successful, this method returns a `201 Created` response code and a [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0517d-201">示例</span><span class="sxs-lookup"><span data-stu-id="0517d-201">Example</span></span>
### <a name="request"></a><span data-ttu-id="0517d-202">请求</span><span class="sxs-lookup"><span data-stu-id="0517d-202">Request</span></span>
<span data-ttu-id="0517d-203">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="0517d-203">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1079

{
  "@odata.type": "#microsoft.graph.windows81VpnConfiguration",
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
  }
}
```

### <a name="response"></a><span data-ttu-id="0517d-204">响应</span><span class="sxs-lookup"><span data-stu-id="0517d-204">Response</span></span>
<span data-ttu-id="0517d-p116">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="0517d-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





