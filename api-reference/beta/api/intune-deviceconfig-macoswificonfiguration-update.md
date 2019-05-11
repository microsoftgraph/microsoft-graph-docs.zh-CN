---
title: 更新 macOSWiFiConfiguration
description: 更新 macOSWiFiConfiguration 对象的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d1c94ab6a9edf8d690356f1dd1b33ceb8d566847
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2019
ms.locfileid: "33922253"
---
# <a name="update-macoswificonfiguration"></a><span data-ttu-id="0f65e-103">更新 macOSWiFiConfiguration</span><span class="sxs-lookup"><span data-stu-id="0f65e-103">Update macOSWiFiConfiguration</span></span>

> <span data-ttu-id="0f65e-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="0f65e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0f65e-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="0f65e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0f65e-106">更新[macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="0f65e-106">Update the properties of a [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0f65e-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="0f65e-107">Prerequisites</span></span>
<span data-ttu-id="0f65e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0f65e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0f65e-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="0f65e-110">Permission type</span></span>|<span data-ttu-id="0f65e-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="0f65e-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0f65e-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0f65e-112">Delegated (work or school account)</span></span>|<span data-ttu-id="0f65e-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0f65e-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="0f65e-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0f65e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0f65e-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="0f65e-115">Not supported.</span></span>|
|<span data-ttu-id="0f65e-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="0f65e-116">Application</span></span>|<span data-ttu-id="0f65e-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="0f65e-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0f65e-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0f65e-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="0f65e-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="0f65e-119">Request headers</span></span>
|<span data-ttu-id="0f65e-120">标头</span><span class="sxs-lookup"><span data-stu-id="0f65e-120">Header</span></span>|<span data-ttu-id="0f65e-121">值</span><span class="sxs-lookup"><span data-stu-id="0f65e-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0f65e-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="0f65e-122">Authorization</span></span>|<span data-ttu-id="0f65e-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="0f65e-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0f65e-124">接受</span><span class="sxs-lookup"><span data-stu-id="0f65e-124">Accept</span></span>|<span data-ttu-id="0f65e-125">application/json</span><span class="sxs-lookup"><span data-stu-id="0f65e-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0f65e-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="0f65e-126">Request body</span></span>
<span data-ttu-id="0f65e-127">在请求正文中, 提供[macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0f65e-127">In the request body, supply a JSON representation for the [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md) object.</span></span>

<span data-ttu-id="0f65e-128">下表显示创建[macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="0f65e-128">The following table shows the properties that are required when you create the [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md).</span></span>

|<span data-ttu-id="0f65e-129">属性</span><span class="sxs-lookup"><span data-stu-id="0f65e-129">Property</span></span>|<span data-ttu-id="0f65e-130">类型</span><span class="sxs-lookup"><span data-stu-id="0f65e-130">Type</span></span>|<span data-ttu-id="0f65e-131">说明</span><span class="sxs-lookup"><span data-stu-id="0f65e-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0f65e-132">id</span><span class="sxs-lookup"><span data-stu-id="0f65e-132">id</span></span>|<span data-ttu-id="0f65e-133">字符串</span><span class="sxs-lookup"><span data-stu-id="0f65e-133">String</span></span>|<span data-ttu-id="0f65e-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="0f65e-134">Key of the entity.</span></span> <span data-ttu-id="0f65e-135">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0f65e-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0f65e-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0f65e-136">lastModifiedDateTime</span></span>|<span data-ttu-id="0f65e-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0f65e-137">DateTimeOffset</span></span>|<span data-ttu-id="0f65e-138">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="0f65e-138">DateTime the object was last modified.</span></span> <span data-ttu-id="0f65e-139">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0f65e-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0f65e-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="0f65e-140">roleScopeTagIds</span></span>|<span data-ttu-id="0f65e-141">String collection</span><span class="sxs-lookup"><span data-stu-id="0f65e-141">String collection</span></span>|<span data-ttu-id="0f65e-142">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="0f65e-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="0f65e-143">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0f65e-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0f65e-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="0f65e-144">supportsScopeTags</span></span>|<span data-ttu-id="0f65e-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="0f65e-145">Boolean</span></span>|<span data-ttu-id="0f65e-146">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="0f65e-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="0f65e-147">如果此值为 false, 则不允许分配给 ScopeTags 属性, 并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="0f65e-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="0f65e-148">这适用于在 Silverlight 中创建的旧版策略, 可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="0f65e-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="0f65e-149">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="0f65e-149">This property is read-only.</span></span> <span data-ttu-id="0f65e-150">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0f65e-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0f65e-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0f65e-151">createdDateTime</span></span>|<span data-ttu-id="0f65e-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0f65e-152">DateTimeOffset</span></span>|<span data-ttu-id="0f65e-153">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="0f65e-153">DateTime the object was created.</span></span> <span data-ttu-id="0f65e-154">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0f65e-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0f65e-155">说明</span><span class="sxs-lookup"><span data-stu-id="0f65e-155">description</span></span>|<span data-ttu-id="0f65e-156">String</span><span class="sxs-lookup"><span data-stu-id="0f65e-156">String</span></span>|<span data-ttu-id="0f65e-157">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="0f65e-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="0f65e-158">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0f65e-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0f65e-159">displayName</span><span class="sxs-lookup"><span data-stu-id="0f65e-159">displayName</span></span>|<span data-ttu-id="0f65e-160">String</span><span class="sxs-lookup"><span data-stu-id="0f65e-160">String</span></span>|<span data-ttu-id="0f65e-161">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="0f65e-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="0f65e-162">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0f65e-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0f65e-163">version</span><span class="sxs-lookup"><span data-stu-id="0f65e-163">version</span></span>|<span data-ttu-id="0f65e-164">Int32</span><span class="sxs-lookup"><span data-stu-id="0f65e-164">Int32</span></span>|<span data-ttu-id="0f65e-165">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="0f65e-165">Version of the device configuration.</span></span> <span data-ttu-id="0f65e-166">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0f65e-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0f65e-167">networkName</span><span class="sxs-lookup"><span data-stu-id="0f65e-167">networkName</span></span>|<span data-ttu-id="0f65e-168">String</span><span class="sxs-lookup"><span data-stu-id="0f65e-168">String</span></span>|<span data-ttu-id="0f65e-169">网络名称</span><span class="sxs-lookup"><span data-stu-id="0f65e-169">Network Name</span></span>|
|<span data-ttu-id="0f65e-170">ssid</span><span class="sxs-lookup"><span data-stu-id="0f65e-170">ssid</span></span>|<span data-ttu-id="0f65e-171">String</span><span class="sxs-lookup"><span data-stu-id="0f65e-171">String</span></span>|<span data-ttu-id="0f65e-172">这是广播到所有设备的 Wi-fi 网络的名称。</span><span class="sxs-lookup"><span data-stu-id="0f65e-172">This is the name of the Wi-Fi network that is broadcast to all devices.</span></span>|
|<span data-ttu-id="0f65e-173">connectAutomatically</span><span class="sxs-lookup"><span data-stu-id="0f65e-173">connectAutomatically</span></span>|<span data-ttu-id="0f65e-174">Boolean</span><span class="sxs-lookup"><span data-stu-id="0f65e-174">Boolean</span></span>|<span data-ttu-id="0f65e-175">当此网络在范围内时自动连接。</span><span class="sxs-lookup"><span data-stu-id="0f65e-175">Connect automatically when this network is in range.</span></span> <span data-ttu-id="0f65e-176">将此设置为 true 将跳过用户提示, 并自动将设备连接到 Wlan 网络。</span><span class="sxs-lookup"><span data-stu-id="0f65e-176">Setting this to true will skip the user prompt and automatically connect the device to Wi-Fi network.</span></span>|
|<span data-ttu-id="0f65e-177">connectWhenNetworkNameIsHidden</span><span class="sxs-lookup"><span data-stu-id="0f65e-177">connectWhenNetworkNameIsHidden</span></span>|<span data-ttu-id="0f65e-178">Boolean</span><span class="sxs-lookup"><span data-stu-id="0f65e-178">Boolean</span></span>|<span data-ttu-id="0f65e-179">网络未广播其名称 (SSID) 时连接。</span><span class="sxs-lookup"><span data-stu-id="0f65e-179">Connect when the network is not broadcasting its name (SSID).</span></span> <span data-ttu-id="0f65e-180">当设置为 true 时, 此配置文件将强制设备连接到不会将其 SSID 广播给所有设备的网络。</span><span class="sxs-lookup"><span data-stu-id="0f65e-180">When set to true, this profile forces the device to connect to a network that doesn't broadcast its SSID to all devices.</span></span>|
|<span data-ttu-id="0f65e-181">wiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="0f65e-181">wiFiSecurityType</span></span>|[<span data-ttu-id="0f65e-182">wiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="0f65e-182">wiFiSecurityType</span></span>](../resources/intune-deviceconfig-wifisecuritytype.md)|<span data-ttu-id="0f65e-183">指示 Wi-fi 终结点是否使用基于 EAP 的安全类型。</span><span class="sxs-lookup"><span data-stu-id="0f65e-183">Indicates whether Wi-Fi endpoint uses an EAP based security type.</span></span> <span data-ttu-id="0f65e-184">可取值为：`open`、`wpaPersonal`、`wpaEnterprise`、`wep`、`wpa2Personal`、`wpa2Enterprise`。</span><span class="sxs-lookup"><span data-stu-id="0f65e-184">Possible values are: `open`, `wpaPersonal`, `wpaEnterprise`, `wep`, `wpa2Personal`, `wpa2Enterprise`.</span></span>|
|<span data-ttu-id="0f65e-185">proxySettings</span><span class="sxs-lookup"><span data-stu-id="0f65e-185">proxySettings</span></span>|[<span data-ttu-id="0f65e-186">wiFiProxySetting</span><span class="sxs-lookup"><span data-stu-id="0f65e-186">wiFiProxySetting</span></span>](../resources/intune-deviceconfig-wifiproxysetting.md)|<span data-ttu-id="0f65e-187">此 Wlan 连接的代理类型。</span><span class="sxs-lookup"><span data-stu-id="0f65e-187">Proxy Type for this Wi-Fi connection.</span></span> <span data-ttu-id="0f65e-188">可取值为：`none`、`manual`、`automatic`。</span><span class="sxs-lookup"><span data-stu-id="0f65e-188">Possible values are: `none`, `manual`, `automatic`.</span></span>|
|<span data-ttu-id="0f65e-189">proxyManualAddress</span><span class="sxs-lookup"><span data-stu-id="0f65e-189">proxyManualAddress</span></span>|<span data-ttu-id="0f65e-190">String</span><span class="sxs-lookup"><span data-stu-id="0f65e-190">String</span></span>|<span data-ttu-id="0f65e-191">选择手动配置时代理服务器的 IP 地址或 DNS 主机名。</span><span class="sxs-lookup"><span data-stu-id="0f65e-191">IP Address or DNS hostname of the proxy server when manual configuration is selected.</span></span>|
|<span data-ttu-id="0f65e-192">proxyManualPort</span><span class="sxs-lookup"><span data-stu-id="0f65e-192">proxyManualPort</span></span>|<span data-ttu-id="0f65e-193">Int32</span><span class="sxs-lookup"><span data-stu-id="0f65e-193">Int32</span></span>|<span data-ttu-id="0f65e-194">选择手动配置时代理服务器的端口。</span><span class="sxs-lookup"><span data-stu-id="0f65e-194">Port of the proxy server when manual configuration is selected.</span></span>|
|<span data-ttu-id="0f65e-195">proxyAutomaticConfigurationUrl</span><span class="sxs-lookup"><span data-stu-id="0f65e-195">proxyAutomaticConfigurationUrl</span></span>|<span data-ttu-id="0f65e-196">String</span><span class="sxs-lookup"><span data-stu-id="0f65e-196">String</span></span>|<span data-ttu-id="0f65e-197">选择 "自动配置" 时代理服务器的 "自动配置" 脚本的 URL。</span><span class="sxs-lookup"><span data-stu-id="0f65e-197">URL of the proxy server automatic configuration script when automatic configuration is selected.</span></span> <span data-ttu-id="0f65e-198">此 URL 通常是 PAC (代理自动配置) 文件的位置。</span><span class="sxs-lookup"><span data-stu-id="0f65e-198">This URL is typically the location of PAC (Proxy Auto Configuration) file.</span></span>|
|<span data-ttu-id="0f65e-199">preSharedKey</span><span class="sxs-lookup"><span data-stu-id="0f65e-199">preSharedKey</span></span>|<span data-ttu-id="0f65e-200">String</span><span class="sxs-lookup"><span data-stu-id="0f65e-200">String</span></span>|<span data-ttu-id="0f65e-201">这是 WPA 个人 Wi-fi 网络的预共享密钥。</span><span class="sxs-lookup"><span data-stu-id="0f65e-201">This is the pre-shared key for WPA Personal Wi-Fi network.</span></span>|



## <a name="response"></a><span data-ttu-id="0f65e-202">响应</span><span class="sxs-lookup"><span data-stu-id="0f65e-202">Response</span></span>
<span data-ttu-id="0f65e-203">如果成功, 此方法在响应`200 OK`正文中返回响应代码和更新的[macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="0f65e-203">If successful, this method returns a `200 OK` response code and an updated [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0f65e-204">示例</span><span class="sxs-lookup"><span data-stu-id="0f65e-204">Example</span></span>

### <a name="request"></a><span data-ttu-id="0f65e-205">请求</span><span class="sxs-lookup"><span data-stu-id="0f65e-205">Request</span></span>
<span data-ttu-id="0f65e-206">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="0f65e-206">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
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

### <a name="response"></a><span data-ttu-id="0f65e-207">响应</span><span class="sxs-lookup"><span data-stu-id="0f65e-207">Response</span></span>
<span data-ttu-id="0f65e-p115">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="0f65e-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




