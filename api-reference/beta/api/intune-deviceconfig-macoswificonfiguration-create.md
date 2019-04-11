---
title: 创建 macOSWiFiConfiguration
description: 创建新的 macOSWiFiConfiguration 对象。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 37de63ee477e4e72b50ace82aac49c1add1c7613
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/11/2019
ms.locfileid: "31804940"
---
# <a name="create-macoswificonfiguration"></a><span data-ttu-id="b3be0-103">创建 macOSWiFiConfiguration</span><span class="sxs-lookup"><span data-stu-id="b3be0-103">Create macOSWiFiConfiguration</span></span>

> <span data-ttu-id="b3be0-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="b3be0-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b3be0-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b3be0-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b3be0-106">创建新的[macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="b3be0-106">Create a new [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b3be0-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="b3be0-107">Prerequisites</span></span>
<span data-ttu-id="b3be0-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b3be0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b3be0-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="b3be0-110">Permission type</span></span>|<span data-ttu-id="b3be0-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="b3be0-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b3be0-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b3be0-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b3be0-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b3be0-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b3be0-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b3be0-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b3be0-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="b3be0-115">Not supported.</span></span>|
|<span data-ttu-id="b3be0-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="b3be0-116">Application</span></span>|<span data-ttu-id="b3be0-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="b3be0-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b3be0-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b3be0-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="b3be0-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="b3be0-119">Request headers</span></span>
|<span data-ttu-id="b3be0-120">标头</span><span class="sxs-lookup"><span data-stu-id="b3be0-120">Header</span></span>|<span data-ttu-id="b3be0-121">值</span><span class="sxs-lookup"><span data-stu-id="b3be0-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b3be0-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="b3be0-122">Authorization</span></span>|<span data-ttu-id="b3be0-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="b3be0-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b3be0-124">接受</span><span class="sxs-lookup"><span data-stu-id="b3be0-124">Accept</span></span>|<span data-ttu-id="b3be0-125">application/json</span><span class="sxs-lookup"><span data-stu-id="b3be0-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b3be0-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="b3be0-126">Request body</span></span>
<span data-ttu-id="b3be0-127">在请求正文中, 提供 macOSWiFiConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b3be0-127">In the request body, supply a JSON representation for the macOSWiFiConfiguration object.</span></span>

<span data-ttu-id="b3be0-128">下表显示创建 macOSWiFiConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="b3be0-128">The following table shows the properties that are required when you create the macOSWiFiConfiguration.</span></span>

|<span data-ttu-id="b3be0-129">属性</span><span class="sxs-lookup"><span data-stu-id="b3be0-129">Property</span></span>|<span data-ttu-id="b3be0-130">类型</span><span class="sxs-lookup"><span data-stu-id="b3be0-130">Type</span></span>|<span data-ttu-id="b3be0-131">说明</span><span class="sxs-lookup"><span data-stu-id="b3be0-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b3be0-132">id</span><span class="sxs-lookup"><span data-stu-id="b3be0-132">id</span></span>|<span data-ttu-id="b3be0-133">String</span><span class="sxs-lookup"><span data-stu-id="b3be0-133">String</span></span>|<span data-ttu-id="b3be0-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="b3be0-134">Key of the entity.</span></span> <span data-ttu-id="b3be0-135">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b3be0-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b3be0-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b3be0-136">lastModifiedDateTime</span></span>|<span data-ttu-id="b3be0-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b3be0-137">DateTimeOffset</span></span>|<span data-ttu-id="b3be0-138">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="b3be0-138">DateTime the object was last modified.</span></span> <span data-ttu-id="b3be0-139">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b3be0-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b3be0-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="b3be0-140">roleScopeTagIds</span></span>|<span data-ttu-id="b3be0-141">String 集合</span><span class="sxs-lookup"><span data-stu-id="b3be0-141">String collection</span></span>|<span data-ttu-id="b3be0-142">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="b3be0-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="b3be0-143">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b3be0-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b3be0-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="b3be0-144">supportsScopeTags</span></span>|<span data-ttu-id="b3be0-145">布尔值</span><span class="sxs-lookup"><span data-stu-id="b3be0-145">Boolean</span></span>|<span data-ttu-id="b3be0-146">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="b3be0-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="b3be0-147">如果此值为 false, 则不允许分配给 ScopeTags 属性, 并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="b3be0-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="b3be0-148">这适用于在 Silverlight 中创建的旧版策略, 可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="b3be0-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="b3be0-149">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="b3be0-149">This property is read-only.</span></span> <span data-ttu-id="b3be0-150">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b3be0-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b3be0-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b3be0-151">createdDateTime</span></span>|<span data-ttu-id="b3be0-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b3be0-152">DateTimeOffset</span></span>|<span data-ttu-id="b3be0-153">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="b3be0-153">DateTime the object was created.</span></span> <span data-ttu-id="b3be0-154">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b3be0-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b3be0-155">description</span><span class="sxs-lookup"><span data-stu-id="b3be0-155">description</span></span>|<span data-ttu-id="b3be0-156">String</span><span class="sxs-lookup"><span data-stu-id="b3be0-156">String</span></span>|<span data-ttu-id="b3be0-157">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="b3be0-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="b3be0-158">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b3be0-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b3be0-159">displayName</span><span class="sxs-lookup"><span data-stu-id="b3be0-159">displayName</span></span>|<span data-ttu-id="b3be0-160">String</span><span class="sxs-lookup"><span data-stu-id="b3be0-160">String</span></span>|<span data-ttu-id="b3be0-161">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="b3be0-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="b3be0-162">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b3be0-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b3be0-163">version</span><span class="sxs-lookup"><span data-stu-id="b3be0-163">version</span></span>|<span data-ttu-id="b3be0-164">Int32</span><span class="sxs-lookup"><span data-stu-id="b3be0-164">Int32</span></span>|<span data-ttu-id="b3be0-165">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="b3be0-165">Version of the device configuration.</span></span> <span data-ttu-id="b3be0-166">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b3be0-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b3be0-167">networkName</span><span class="sxs-lookup"><span data-stu-id="b3be0-167">networkName</span></span>|<span data-ttu-id="b3be0-168">String</span><span class="sxs-lookup"><span data-stu-id="b3be0-168">String</span></span>|<span data-ttu-id="b3be0-169">网络名称</span><span class="sxs-lookup"><span data-stu-id="b3be0-169">Network Name</span></span>|
|<span data-ttu-id="b3be0-170">ssid</span><span class="sxs-lookup"><span data-stu-id="b3be0-170">ssid</span></span>|<span data-ttu-id="b3be0-171">String</span><span class="sxs-lookup"><span data-stu-id="b3be0-171">String</span></span>|<span data-ttu-id="b3be0-172">这是广播到所有设备的 wi-fi 网络的名称。</span><span class="sxs-lookup"><span data-stu-id="b3be0-172">This is the name of the Wi-Fi network that is broadcast to all devices.</span></span>|
|<span data-ttu-id="b3be0-173">connectAutomatically</span><span class="sxs-lookup"><span data-stu-id="b3be0-173">connectAutomatically</span></span>|<span data-ttu-id="b3be0-174">布尔值</span><span class="sxs-lookup"><span data-stu-id="b3be0-174">Boolean</span></span>|<span data-ttu-id="b3be0-175">当此网络在范围内时自动连接。</span><span class="sxs-lookup"><span data-stu-id="b3be0-175">Connect automatically when this network is in range.</span></span> <span data-ttu-id="b3be0-176">将此设置为 true 将跳过用户提示, 并自动将设备连接到 wlan 网络。</span><span class="sxs-lookup"><span data-stu-id="b3be0-176">Setting this to true will skip the user prompt and automatically connect the device to Wi-Fi network.</span></span>|
|<span data-ttu-id="b3be0-177">connectWhenNetworkNameIsHidden</span><span class="sxs-lookup"><span data-stu-id="b3be0-177">connectWhenNetworkNameIsHidden</span></span>|<span data-ttu-id="b3be0-178">布尔值</span><span class="sxs-lookup"><span data-stu-id="b3be0-178">Boolean</span></span>|<span data-ttu-id="b3be0-179">网络未广播其名称 (SSID) 时连接。</span><span class="sxs-lookup"><span data-stu-id="b3be0-179">Connect when the network is not broadcasting its name (SSID).</span></span> <span data-ttu-id="b3be0-180">当设置为 true 时, 此配置文件将强制设备连接到不会将其 SSID 广播给所有设备的网络。</span><span class="sxs-lookup"><span data-stu-id="b3be0-180">When set to true, this profile forces the device to connect to a network that doesn't broadcast its SSID to all devices.</span></span>|
|<span data-ttu-id="b3be0-181">wiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="b3be0-181">wiFiSecurityType</span></span>|[<span data-ttu-id="b3be0-182">wiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="b3be0-182">wiFiSecurityType</span></span>](../resources/intune-deviceconfig-wifisecuritytype.md)|<span data-ttu-id="b3be0-183">指示 wi-fi 终结点是否使用基于 EAP 的安全类型。</span><span class="sxs-lookup"><span data-stu-id="b3be0-183">Indicates whether Wi-Fi endpoint uses an EAP based security type.</span></span> <span data-ttu-id="b3be0-184">可取值为：`open`、`wpaPersonal`、`wpaEnterprise`、`wep`、`wpa2Personal`、`wpa2Enterprise`。</span><span class="sxs-lookup"><span data-stu-id="b3be0-184">Possible values are: `open`, `wpaPersonal`, `wpaEnterprise`, `wep`, `wpa2Personal`, `wpa2Enterprise`.</span></span>|
|<span data-ttu-id="b3be0-185">proxySettings</span><span class="sxs-lookup"><span data-stu-id="b3be0-185">proxySettings</span></span>|[<span data-ttu-id="b3be0-186">wiFiProxySetting</span><span class="sxs-lookup"><span data-stu-id="b3be0-186">wiFiProxySetting</span></span>](../resources/intune-deviceconfig-wifiproxysetting.md)|<span data-ttu-id="b3be0-187">此 wlan 连接的代理类型。</span><span class="sxs-lookup"><span data-stu-id="b3be0-187">Proxy Type for this Wi-Fi connection.</span></span> <span data-ttu-id="b3be0-188">可取值为：`none`、`manual`、`automatic`。</span><span class="sxs-lookup"><span data-stu-id="b3be0-188">Possible values are: `none`, `manual`, `automatic`.</span></span>|
|<span data-ttu-id="b3be0-189">proxyManualAddress</span><span class="sxs-lookup"><span data-stu-id="b3be0-189">proxyManualAddress</span></span>|<span data-ttu-id="b3be0-190">String</span><span class="sxs-lookup"><span data-stu-id="b3be0-190">String</span></span>|<span data-ttu-id="b3be0-191">选择手动配置时代理服务器的 IP 地址或 DNS 主机名。</span><span class="sxs-lookup"><span data-stu-id="b3be0-191">IP Address or DNS hostname of the proxy server when manual configuration is selected.</span></span>|
|<span data-ttu-id="b3be0-192">proxyManualPort</span><span class="sxs-lookup"><span data-stu-id="b3be0-192">proxyManualPort</span></span>|<span data-ttu-id="b3be0-193">Int32</span><span class="sxs-lookup"><span data-stu-id="b3be0-193">Int32</span></span>|<span data-ttu-id="b3be0-194">选择手动配置时代理服务器的端口。</span><span class="sxs-lookup"><span data-stu-id="b3be0-194">Port of the proxy server when manual configuration is selected.</span></span>|
|<span data-ttu-id="b3be0-195">proxyAutomaticConfigurationUrl</span><span class="sxs-lookup"><span data-stu-id="b3be0-195">proxyAutomaticConfigurationUrl</span></span>|<span data-ttu-id="b3be0-196">String</span><span class="sxs-lookup"><span data-stu-id="b3be0-196">String</span></span>|<span data-ttu-id="b3be0-197">选择 "自动配置" 时代理服务器的 "自动配置" 脚本的 URL。</span><span class="sxs-lookup"><span data-stu-id="b3be0-197">URL of the proxy server automatic configuration script when automatic configuration is selected.</span></span> <span data-ttu-id="b3be0-198">此 URL 通常是 PAC (代理自动配置) 文件的位置。</span><span class="sxs-lookup"><span data-stu-id="b3be0-198">This URL is typically the location of PAC (Proxy Auto Configuration) file.</span></span>|
|<span data-ttu-id="b3be0-199">preSharedKey</span><span class="sxs-lookup"><span data-stu-id="b3be0-199">preSharedKey</span></span>|<span data-ttu-id="b3be0-200">String</span><span class="sxs-lookup"><span data-stu-id="b3be0-200">String</span></span>|<span data-ttu-id="b3be0-201">这是 WPA 个人 wi-fi 网络的预共享密钥。</span><span class="sxs-lookup"><span data-stu-id="b3be0-201">This is the pre-shared key for WPA Personal Wi-Fi network.</span></span>|



## <a name="response"></a><span data-ttu-id="b3be0-202">响应</span><span class="sxs-lookup"><span data-stu-id="b3be0-202">Response</span></span>
<span data-ttu-id="b3be0-203">如果成功, 此方法在响应`201 Created`正文中返回响应代码和[macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="b3be0-203">If successful, this method returns a `201 Created` response code and a [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b3be0-204">示例</span><span class="sxs-lookup"><span data-stu-id="b3be0-204">Example</span></span>

### <a name="request"></a><span data-ttu-id="b3be0-205">请求</span><span class="sxs-lookup"><span data-stu-id="b3be0-205">Request</span></span>
<span data-ttu-id="b3be0-206">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="b3be0-206">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 677

{
  "@odata.type": "#microsoft.graph.macOSWiFiConfiguration",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "networkName": "Network Name value",
  "ssid": "Ssid value",
  "connectAutomatically": true,
  "connectWhenNetworkNameIsHidden": true,
  "wiFiSecurityType": "wpaPersonal",
  "proxySettings": "manual",
  "proxyManualAddress": "Proxy Manual Address value",
  "proxyManualPort": 15,
  "proxyAutomaticConfigurationUrl": "https://example.com/proxyAutomaticConfigurationUrl/",
  "preSharedKey": "Pre Shared Key value"
}
```

### <a name="response"></a><span data-ttu-id="b3be0-207">响应</span><span class="sxs-lookup"><span data-stu-id="b3be0-207">Response</span></span>
<span data-ttu-id="b3be0-p115">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="b3be0-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 849

{
  "@odata.type": "#microsoft.graph.macOSWiFiConfiguration",
  "id": "471203fb-03fb-4712-fb03-1247fb031247",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "networkName": "Network Name value",
  "ssid": "Ssid value",
  "connectAutomatically": true,
  "connectWhenNetworkNameIsHidden": true,
  "wiFiSecurityType": "wpaPersonal",
  "proxySettings": "manual",
  "proxyManualAddress": "Proxy Manual Address value",
  "proxyManualPort": 15,
  "proxyAutomaticConfigurationUrl": "https://example.com/proxyAutomaticConfigurationUrl/",
  "preSharedKey": "Pre Shared Key value"
}
```





