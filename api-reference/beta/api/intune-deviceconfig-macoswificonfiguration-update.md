---
title: 更新 macOSWiFiConfiguration
description: 更新 macOSWiFiConfiguration 对象的属性。
author: tfitzmac
ms.openlocfilehash: 59422770cf3d6877829492485b9ed11cd30bda1e
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27322937"
---
# <a name="update-macoswificonfiguration"></a><span data-ttu-id="df96c-103">更新 macOSWiFiConfiguration</span><span class="sxs-lookup"><span data-stu-id="df96c-103">Update macOSWiFiConfiguration</span></span>

> <span data-ttu-id="df96c-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="df96c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="df96c-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="df96c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="df96c-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="df96c-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="df96c-107">更新[macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="df96c-107">Update the properties of a [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="df96c-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="df96c-108">Prerequisites</span></span>
<span data-ttu-id="df96c-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="df96c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="df96c-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="df96c-111">Permission type</span></span>|<span data-ttu-id="df96c-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="df96c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="df96c-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="df96c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="df96c-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="df96c-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="df96c-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="df96c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="df96c-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="df96c-116">Not supported.</span></span>|
|<span data-ttu-id="df96c-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="df96c-117">Application</span></span>|<span data-ttu-id="df96c-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="df96c-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="df96c-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="df96c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="df96c-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="df96c-120">Request headers</span></span>
|<span data-ttu-id="df96c-121">标头</span><span class="sxs-lookup"><span data-stu-id="df96c-121">Header</span></span>|<span data-ttu-id="df96c-122">值</span><span class="sxs-lookup"><span data-stu-id="df96c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="df96c-123">授权</span><span class="sxs-lookup"><span data-stu-id="df96c-123">Authorization</span></span>|<span data-ttu-id="df96c-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="df96c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="df96c-125">Accept</span><span class="sxs-lookup"><span data-stu-id="df96c-125">Accept</span></span>|<span data-ttu-id="df96c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="df96c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="df96c-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="df96c-127">Request body</span></span>
<span data-ttu-id="df96c-128">在请求正文中，提供[macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="df96c-128">In the request body, supply a JSON representation for the [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md) object.</span></span>

<span data-ttu-id="df96c-129">下表显示时创建[macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md)所需的属性。</span><span class="sxs-lookup"><span data-stu-id="df96c-129">The following table shows the properties that are required when you create the [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md).</span></span>

|<span data-ttu-id="df96c-130">属性</span><span class="sxs-lookup"><span data-stu-id="df96c-130">Property</span></span>|<span data-ttu-id="df96c-131">类型</span><span class="sxs-lookup"><span data-stu-id="df96c-131">Type</span></span>|<span data-ttu-id="df96c-132">说明</span><span class="sxs-lookup"><span data-stu-id="df96c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="df96c-133">id</span><span class="sxs-lookup"><span data-stu-id="df96c-133">id</span></span>|<span data-ttu-id="df96c-134">String</span><span class="sxs-lookup"><span data-stu-id="df96c-134">String</span></span>|<span data-ttu-id="df96c-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="df96c-135">Key of the entity.</span></span> <span data-ttu-id="df96c-136">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="df96c-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="df96c-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="df96c-137">lastModifiedDateTime</span></span>|<span data-ttu-id="df96c-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="df96c-138">DateTimeOffset</span></span>|<span data-ttu-id="df96c-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="df96c-139">DateTime the object was last modified.</span></span> <span data-ttu-id="df96c-140">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="df96c-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="df96c-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="df96c-141">roleScopeTagIds</span></span>|<span data-ttu-id="df96c-142">String 集合</span><span class="sxs-lookup"><span data-stu-id="df96c-142">String collection</span></span>|<span data-ttu-id="df96c-143">此实体实例范围标记的列表。</span><span class="sxs-lookup"><span data-stu-id="df96c-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="df96c-144">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="df96c-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="df96c-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="df96c-145">supportsScopeTags</span></span>|<span data-ttu-id="df96c-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="df96c-146">Boolean</span></span>|<span data-ttu-id="df96c-147">指示基础的设备配置支持分配的范围标记。</span><span class="sxs-lookup"><span data-stu-id="df96c-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="df96c-148">此值为 false，并且实体将不会对作用域的用户可见时，不允许将分配给 ScopeTags 属性。</span><span class="sxs-lookup"><span data-stu-id="df96c-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="df96c-149">这将发生在 Silverlight 中创建的旧策略，并可以解析通过删除并重新创建 Azure 门户中的策略。</span><span class="sxs-lookup"><span data-stu-id="df96c-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="df96c-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="df96c-150">This property is read-only.</span></span> <span data-ttu-id="df96c-151">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="df96c-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="df96c-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="df96c-152">createdDateTime</span></span>|<span data-ttu-id="df96c-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="df96c-153">DateTimeOffset</span></span>|<span data-ttu-id="df96c-154">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="df96c-154">DateTime the object was created.</span></span> <span data-ttu-id="df96c-155">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="df96c-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="df96c-156">description</span><span class="sxs-lookup"><span data-stu-id="df96c-156">description</span></span>|<span data-ttu-id="df96c-157">String</span><span class="sxs-lookup"><span data-stu-id="df96c-157">String</span></span>|<span data-ttu-id="df96c-158">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="df96c-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="df96c-159">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="df96c-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="df96c-160">displayName</span><span class="sxs-lookup"><span data-stu-id="df96c-160">displayName</span></span>|<span data-ttu-id="df96c-161">String</span><span class="sxs-lookup"><span data-stu-id="df96c-161">String</span></span>|<span data-ttu-id="df96c-162">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="df96c-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="df96c-163">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="df96c-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="df96c-164">version</span><span class="sxs-lookup"><span data-stu-id="df96c-164">version</span></span>|<span data-ttu-id="df96c-165">Int32</span><span class="sxs-lookup"><span data-stu-id="df96c-165">Int32</span></span>|<span data-ttu-id="df96c-166">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="df96c-166">Version of the device configuration.</span></span> <span data-ttu-id="df96c-167">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="df96c-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="df96c-168">networkName</span><span class="sxs-lookup"><span data-stu-id="df96c-168">networkName</span></span>|<span data-ttu-id="df96c-169">字符串</span><span class="sxs-lookup"><span data-stu-id="df96c-169">String</span></span>|<span data-ttu-id="df96c-170">网络名称</span><span class="sxs-lookup"><span data-stu-id="df96c-170">Network Name</span></span>|
|<span data-ttu-id="df96c-171">ssid</span><span class="sxs-lookup"><span data-stu-id="df96c-171">ssid</span></span>|<span data-ttu-id="df96c-172">字符串</span><span class="sxs-lookup"><span data-stu-id="df96c-172">String</span></span>|<span data-ttu-id="df96c-173">这是广播到所有设备 Wi-fi 网络的名称。</span><span class="sxs-lookup"><span data-stu-id="df96c-173">This is the name of the Wi-Fi network that is broadcast to all devices.</span></span>|
|<span data-ttu-id="df96c-174">connectAutomatically</span><span class="sxs-lookup"><span data-stu-id="df96c-174">connectAutomatically</span></span>|<span data-ttu-id="df96c-175">Boolean</span><span class="sxs-lookup"><span data-stu-id="df96c-175">Boolean</span></span>|<span data-ttu-id="df96c-176">自动连接此网络何时范围中。</span><span class="sxs-lookup"><span data-stu-id="df96c-176">Connect automatically when this network is in range.</span></span> <span data-ttu-id="df96c-177">将此值设置为 true 将跳过的用户提示并自动将设备连接到 Wi-fi 网络。</span><span class="sxs-lookup"><span data-stu-id="df96c-177">Setting this to true will skip the user prompt and automatically connect the device to Wi-Fi network.</span></span>|
|<span data-ttu-id="df96c-178">connectWhenNetworkNameIsHidden</span><span class="sxs-lookup"><span data-stu-id="df96c-178">connectWhenNetworkNameIsHidden</span></span>|<span data-ttu-id="df96c-179">Boolean</span><span class="sxs-lookup"><span data-stu-id="df96c-179">Boolean</span></span>|<span data-ttu-id="df96c-180">网络未进行广播其名称 (SSID) 连接。</span><span class="sxs-lookup"><span data-stu-id="df96c-180">Connect when the network is not broadcasting its name (SSID).</span></span> <span data-ttu-id="df96c-181">当设置为 true，该配置文件强制设备连接到不广播到所有设备其 SSID 网络。</span><span class="sxs-lookup"><span data-stu-id="df96c-181">When set to true, this profile forces the device to connect to a network that doesn't broadcast its SSID to all devices.</span></span>|
|<span data-ttu-id="df96c-182">wiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="df96c-182">wiFiSecurityType</span></span>|[<span data-ttu-id="df96c-183">wiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="df96c-183">wiFiSecurityType</span></span>](../resources/intune-deviceconfig-wifisecuritytype.md)|<span data-ttu-id="df96c-184">指示是否 Wi-fi 终结点使用 EAP 基于安全类型。</span><span class="sxs-lookup"><span data-stu-id="df96c-184">Indicates whether Wi-Fi endpoint uses an EAP based security type.</span></span> <span data-ttu-id="df96c-185">可取值为：`open`、`wpaPersonal`、`wpaEnterprise`、`wep`、`wpa2Personal`、`wpa2Enterprise`。</span><span class="sxs-lookup"><span data-stu-id="df96c-185">Possible values are: `open`, `wpaPersonal`, `wpaEnterprise`, `wep`, `wpa2Personal`, `wpa2Enterprise`.</span></span>|
|<span data-ttu-id="df96c-186">proxySettings</span><span class="sxs-lookup"><span data-stu-id="df96c-186">proxySettings</span></span>|[<span data-ttu-id="df96c-187">wiFiProxySetting</span><span class="sxs-lookup"><span data-stu-id="df96c-187">wiFiProxySetting</span></span>](../resources/intune-deviceconfig-wifiproxysetting.md)|<span data-ttu-id="df96c-188">此 Wi-fi 连接的代理类型。</span><span class="sxs-lookup"><span data-stu-id="df96c-188">Proxy Type for this Wi-Fi connection.</span></span> <span data-ttu-id="df96c-189">可取值为：`none`、`manual`、`automatic`。</span><span class="sxs-lookup"><span data-stu-id="df96c-189">Possible values are: `none`, `manual`, `automatic`.</span></span>|
|<span data-ttu-id="df96c-190">proxyManualAddress</span><span class="sxs-lookup"><span data-stu-id="df96c-190">proxyManualAddress</span></span>|<span data-ttu-id="df96c-191">字符串</span><span class="sxs-lookup"><span data-stu-id="df96c-191">String</span></span>|<span data-ttu-id="df96c-192">选择手动配置时，代理服务器的 IP 地址或 DNS 主机名。</span><span class="sxs-lookup"><span data-stu-id="df96c-192">IP Address or DNS hostname of the proxy server when manual configuration is selected.</span></span>|
|<span data-ttu-id="df96c-193">proxyManualPort</span><span class="sxs-lookup"><span data-stu-id="df96c-193">proxyManualPort</span></span>|<span data-ttu-id="df96c-194">Int32</span><span class="sxs-lookup"><span data-stu-id="df96c-194">Int32</span></span>|<span data-ttu-id="df96c-195">选择手动配置时的代理服务器的端口。</span><span class="sxs-lookup"><span data-stu-id="df96c-195">Port of the proxy server when manual configuration is selected.</span></span>|
|<span data-ttu-id="df96c-196">proxyAutomaticConfigurationUrl</span><span class="sxs-lookup"><span data-stu-id="df96c-196">proxyAutomaticConfigurationUrl</span></span>|<span data-ttu-id="df96c-197">字符串</span><span class="sxs-lookup"><span data-stu-id="df96c-197">String</span></span>|<span data-ttu-id="df96c-198">代理服务器自动配置脚本时选择了自动配置的 URL。</span><span class="sxs-lookup"><span data-stu-id="df96c-198">URL of the proxy server automatic configuration script when automatic configuration is selected.</span></span> <span data-ttu-id="df96c-199">此 URL 通常是 PAC （代理自动配置） 文件的位置。</span><span class="sxs-lookup"><span data-stu-id="df96c-199">This URL is typically the location of PAC (Proxy Auto Configuration) file.</span></span>|
|<span data-ttu-id="df96c-200">preSharedKey</span><span class="sxs-lookup"><span data-stu-id="df96c-200">preSharedKey</span></span>|<span data-ttu-id="df96c-201">字符串</span><span class="sxs-lookup"><span data-stu-id="df96c-201">String</span></span>|<span data-ttu-id="df96c-202">这是预共享的 WPA 个人 Wi-fi 网络密钥。</span><span class="sxs-lookup"><span data-stu-id="df96c-202">This is the pre-shared key for WPA Personal Wi-Fi network.</span></span>|



## <a name="response"></a><span data-ttu-id="df96c-203">响应</span><span class="sxs-lookup"><span data-stu-id="df96c-203">Response</span></span>
<span data-ttu-id="df96c-204">如果成功，此方法返回`200 OK`响应代码和响应正文中的更新的[macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="df96c-204">If successful, this method returns a `200 OK` response code and an updated [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="df96c-205">示例</span><span class="sxs-lookup"><span data-stu-id="df96c-205">Example</span></span>
### <a name="request"></a><span data-ttu-id="df96c-206">请求</span><span class="sxs-lookup"><span data-stu-id="df96c-206">Request</span></span>
<span data-ttu-id="df96c-207">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="df96c-207">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 680

{
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
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

### <a name="response"></a><span data-ttu-id="df96c-208">响应</span><span class="sxs-lookup"><span data-stu-id="df96c-208">Response</span></span>
<span data-ttu-id="df96c-p116">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="df96c-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





