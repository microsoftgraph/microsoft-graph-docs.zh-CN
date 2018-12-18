---
title: 创建 windowsWifiConfiguration
description: 创建新的 windowsWifiConfiguration 对象。
author: tfitzmac
ms.openlocfilehash: 0d09897844acd0e0ea52103a371ff6825df10379
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27305010"
---
# <a name="create-windowswificonfiguration"></a><span data-ttu-id="b8cc7-103">创建 windowsWifiConfiguration</span><span class="sxs-lookup"><span data-stu-id="b8cc7-103">Create windowsWifiConfiguration</span></span>

> <span data-ttu-id="b8cc7-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="b8cc7-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b8cc7-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="b8cc7-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b8cc7-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="b8cc7-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b8cc7-107">创建新的[windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="b8cc7-107">Create a new [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="b8cc7-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="b8cc7-108">Prerequisites</span></span>
<span data-ttu-id="b8cc7-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="b8cc7-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b8cc7-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="b8cc7-111">Permission type</span></span>|<span data-ttu-id="b8cc7-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="b8cc7-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b8cc7-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b8cc7-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b8cc7-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b8cc7-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b8cc7-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b8cc7-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b8cc7-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="b8cc7-116">Not supported.</span></span>|
|<span data-ttu-id="b8cc7-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="b8cc7-117">Application</span></span>|<span data-ttu-id="b8cc7-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="b8cc7-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b8cc7-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b8cc7-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="b8cc7-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="b8cc7-120">Request headers</span></span>
|<span data-ttu-id="b8cc7-121">标头</span><span class="sxs-lookup"><span data-stu-id="b8cc7-121">Header</span></span>|<span data-ttu-id="b8cc7-122">值</span><span class="sxs-lookup"><span data-stu-id="b8cc7-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b8cc7-123">授权</span><span class="sxs-lookup"><span data-stu-id="b8cc7-123">Authorization</span></span>|<span data-ttu-id="b8cc7-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="b8cc7-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b8cc7-125">Accept</span><span class="sxs-lookup"><span data-stu-id="b8cc7-125">Accept</span></span>|<span data-ttu-id="b8cc7-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b8cc7-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b8cc7-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="b8cc7-127">Request body</span></span>
<span data-ttu-id="b8cc7-128">在请求正文中，提供 windowsWifiConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b8cc7-128">In the request body, supply a JSON representation for the windowsWifiConfiguration object.</span></span>

<span data-ttu-id="b8cc7-129">下表显示时创建 windowsWifiConfiguration 所需的属性。</span><span class="sxs-lookup"><span data-stu-id="b8cc7-129">The following table shows the properties that are required when you create the windowsWifiConfiguration.</span></span>

|<span data-ttu-id="b8cc7-130">属性</span><span class="sxs-lookup"><span data-stu-id="b8cc7-130">Property</span></span>|<span data-ttu-id="b8cc7-131">类型</span><span class="sxs-lookup"><span data-stu-id="b8cc7-131">Type</span></span>|<span data-ttu-id="b8cc7-132">说明</span><span class="sxs-lookup"><span data-stu-id="b8cc7-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b8cc7-133">id</span><span class="sxs-lookup"><span data-stu-id="b8cc7-133">id</span></span>|<span data-ttu-id="b8cc7-134">String</span><span class="sxs-lookup"><span data-stu-id="b8cc7-134">String</span></span>|<span data-ttu-id="b8cc7-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="b8cc7-135">Key of the entity.</span></span> <span data-ttu-id="b8cc7-136">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b8cc7-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b8cc7-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b8cc7-137">lastModifiedDateTime</span></span>|<span data-ttu-id="b8cc7-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b8cc7-138">DateTimeOffset</span></span>|<span data-ttu-id="b8cc7-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="b8cc7-139">DateTime the object was last modified.</span></span> <span data-ttu-id="b8cc7-140">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b8cc7-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b8cc7-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="b8cc7-141">roleScopeTagIds</span></span>|<span data-ttu-id="b8cc7-142">String 集合</span><span class="sxs-lookup"><span data-stu-id="b8cc7-142">String collection</span></span>|<span data-ttu-id="b8cc7-143">此实体实例范围标记的列表。</span><span class="sxs-lookup"><span data-stu-id="b8cc7-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="b8cc7-144">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b8cc7-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b8cc7-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="b8cc7-145">supportsScopeTags</span></span>|<span data-ttu-id="b8cc7-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="b8cc7-146">Boolean</span></span>|<span data-ttu-id="b8cc7-147">指示基础的设备配置支持分配的范围标记。</span><span class="sxs-lookup"><span data-stu-id="b8cc7-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="b8cc7-148">此值为 false，并且实体将不会对作用域的用户可见时，不允许将分配给 ScopeTags 属性。</span><span class="sxs-lookup"><span data-stu-id="b8cc7-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="b8cc7-149">这将发生在 Silverlight 中创建的旧策略，并可以解析通过删除并重新创建 Azure 门户中的策略。</span><span class="sxs-lookup"><span data-stu-id="b8cc7-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="b8cc7-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="b8cc7-150">This property is read-only.</span></span> <span data-ttu-id="b8cc7-151">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b8cc7-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b8cc7-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b8cc7-152">createdDateTime</span></span>|<span data-ttu-id="b8cc7-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b8cc7-153">DateTimeOffset</span></span>|<span data-ttu-id="b8cc7-154">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="b8cc7-154">DateTime the object was created.</span></span> <span data-ttu-id="b8cc7-155">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b8cc7-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b8cc7-156">description</span><span class="sxs-lookup"><span data-stu-id="b8cc7-156">description</span></span>|<span data-ttu-id="b8cc7-157">String</span><span class="sxs-lookup"><span data-stu-id="b8cc7-157">String</span></span>|<span data-ttu-id="b8cc7-158">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="b8cc7-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="b8cc7-159">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b8cc7-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b8cc7-160">displayName</span><span class="sxs-lookup"><span data-stu-id="b8cc7-160">displayName</span></span>|<span data-ttu-id="b8cc7-161">String</span><span class="sxs-lookup"><span data-stu-id="b8cc7-161">String</span></span>|<span data-ttu-id="b8cc7-162">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="b8cc7-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="b8cc7-163">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b8cc7-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b8cc7-164">version</span><span class="sxs-lookup"><span data-stu-id="b8cc7-164">version</span></span>|<span data-ttu-id="b8cc7-165">Int32</span><span class="sxs-lookup"><span data-stu-id="b8cc7-165">Int32</span></span>|<span data-ttu-id="b8cc7-166">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="b8cc7-166">Version of the device configuration.</span></span> <span data-ttu-id="b8cc7-167">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b8cc7-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b8cc7-168">preSharedKey</span><span class="sxs-lookup"><span data-stu-id="b8cc7-168">preSharedKey</span></span>|<span data-ttu-id="b8cc7-169">字符串</span><span class="sxs-lookup"><span data-stu-id="b8cc7-169">String</span></span>|<span data-ttu-id="b8cc7-170">这是预共享的 WPA 个人 Wi-fi 网络密钥。</span><span class="sxs-lookup"><span data-stu-id="b8cc7-170">This is the pre-shared key for WPA Personal Wi-Fi network.</span></span>|
|<span data-ttu-id="b8cc7-171">wifiSecurityType</span><span class="sxs-lookup"><span data-stu-id="b8cc7-171">wifiSecurityType</span></span>|[<span data-ttu-id="b8cc7-172">wiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="b8cc7-172">wiFiSecurityType</span></span>](../resources/intune-deviceconfig-wifisecuritytype.md)|<span data-ttu-id="b8cc7-173">指定的 Wifi 安全类型。</span><span class="sxs-lookup"><span data-stu-id="b8cc7-173">Specify the Wifi Security Type.</span></span> <span data-ttu-id="b8cc7-174">可取值为：`open`、`wpaPersonal`、`wpaEnterprise`、`wep`、`wpa2Personal`、`wpa2Enterprise`。</span><span class="sxs-lookup"><span data-stu-id="b8cc7-174">Possible values are: `open`, `wpaPersonal`, `wpaEnterprise`, `wep`, `wpa2Personal`, `wpa2Enterprise`.</span></span>|
|<span data-ttu-id="b8cc7-175">meteredConnectionLimit</span><span class="sxs-lookup"><span data-stu-id="b8cc7-175">meteredConnectionLimit</span></span>|[<span data-ttu-id="b8cc7-176">meteredConnectionLimitType</span><span class="sxs-lookup"><span data-stu-id="b8cc7-176">meteredConnectionLimitType</span></span>](../resources/intune-deviceconfig-meteredconnectionlimittype.md)|<span data-ttu-id="b8cc7-177">指定 wifi 连接的按流量计费的连接限制类型。</span><span class="sxs-lookup"><span data-stu-id="b8cc7-177">Specify the metered connection limit type for the wifi connection.</span></span> <span data-ttu-id="b8cc7-178">可取值为：`unrestricted`、`fixed`、`variable`。</span><span class="sxs-lookup"><span data-stu-id="b8cc7-178">Possible values are: `unrestricted`, `fixed`, `variable`.</span></span>|
|<span data-ttu-id="b8cc7-179">ssid</span><span class="sxs-lookup"><span data-stu-id="b8cc7-179">ssid</span></span>|<span data-ttu-id="b8cc7-180">字符串</span><span class="sxs-lookup"><span data-stu-id="b8cc7-180">String</span></span>|<span data-ttu-id="b8cc7-181">指定 wifi 连接的 SSID。</span><span class="sxs-lookup"><span data-stu-id="b8cc7-181">Specify the SSID of the wifi connection.</span></span>|
|<span data-ttu-id="b8cc7-182">networkName</span><span class="sxs-lookup"><span data-stu-id="b8cc7-182">networkName</span></span>|<span data-ttu-id="b8cc7-183">字符串</span><span class="sxs-lookup"><span data-stu-id="b8cc7-183">String</span></span>|<span data-ttu-id="b8cc7-184">指定的网络配置名称。</span><span class="sxs-lookup"><span data-stu-id="b8cc7-184">Specify the network configuration name.</span></span>|
|<span data-ttu-id="b8cc7-185">connectAutomatically</span><span class="sxs-lookup"><span data-stu-id="b8cc7-185">connectAutomatically</span></span>|<span data-ttu-id="b8cc7-186">Boolean</span><span class="sxs-lookup"><span data-stu-id="b8cc7-186">Boolean</span></span>|<span data-ttu-id="b8cc7-187">指定应在范围中自动连接是否 wifi 连接。</span><span class="sxs-lookup"><span data-stu-id="b8cc7-187">Specify whether the wifi connection should connect automatically when in range.</span></span>|
|<span data-ttu-id="b8cc7-188">connectToPreferredNetwork</span><span class="sxs-lookup"><span data-stu-id="b8cc7-188">connectToPreferredNetwork</span></span>|<span data-ttu-id="b8cc7-189">Boolean</span><span class="sxs-lookup"><span data-stu-id="b8cc7-189">Boolean</span></span>|<span data-ttu-id="b8cc7-190">指定 wifi 连接是否应连接到时已连接到此的更多首选网络。</span><span class="sxs-lookup"><span data-stu-id="b8cc7-190">Specify whether the wifi connection should connect to more preferred networks when already connected to this one.</span></span>  <span data-ttu-id="b8cc7-191">需要 ConnectAutomatically 为 true。</span><span class="sxs-lookup"><span data-stu-id="b8cc7-191">Requires ConnectAutomatically to be true.</span></span>|
|<span data-ttu-id="b8cc7-192">connectWhenNetworkNameIsHidden</span><span class="sxs-lookup"><span data-stu-id="b8cc7-192">connectWhenNetworkNameIsHidden</span></span>|<span data-ttu-id="b8cc7-193">Boolean</span><span class="sxs-lookup"><span data-stu-id="b8cc7-193">Boolean</span></span>|<span data-ttu-id="b8cc7-194">指定是否 wifi 连接应自动连接即使时 SSID 未进行广播。</span><span class="sxs-lookup"><span data-stu-id="b8cc7-194">Specify whether the wifi connection should connect automatically even when the SSID is not broadcasting.</span></span>|
|<span data-ttu-id="b8cc7-195">proxySetting</span><span class="sxs-lookup"><span data-stu-id="b8cc7-195">proxySetting</span></span>|[<span data-ttu-id="b8cc7-196">wiFiProxySetting</span><span class="sxs-lookup"><span data-stu-id="b8cc7-196">wiFiProxySetting</span></span>](../resources/intune-deviceconfig-wifiproxysetting.md)|<span data-ttu-id="b8cc7-197">指定代理 Wi-fi 配置设置。</span><span class="sxs-lookup"><span data-stu-id="b8cc7-197">Specify the proxy setting for Wi-Fi configuration.</span></span> <span data-ttu-id="b8cc7-198">可取值为：`none`、`manual`、`automatic`。</span><span class="sxs-lookup"><span data-stu-id="b8cc7-198">Possible values are: `none`, `manual`, `automatic`.</span></span>|
|<span data-ttu-id="b8cc7-199">proxyManualAddress</span><span class="sxs-lookup"><span data-stu-id="b8cc7-199">proxyManualAddress</span></span>|<span data-ttu-id="b8cc7-200">字符串</span><span class="sxs-lookup"><span data-stu-id="b8cc7-200">String</span></span>|<span data-ttu-id="b8cc7-201">指定代理服务器的 IP 地址。</span><span class="sxs-lookup"><span data-stu-id="b8cc7-201">Specify the IP address for the proxy server.</span></span>|
|<span data-ttu-id="b8cc7-202">proxyManualPort</span><span class="sxs-lookup"><span data-stu-id="b8cc7-202">proxyManualPort</span></span>|<span data-ttu-id="b8cc7-203">Int32</span><span class="sxs-lookup"><span data-stu-id="b8cc7-203">Int32</span></span>|<span data-ttu-id="b8cc7-204">指定的代理服务器的端口。</span><span class="sxs-lookup"><span data-stu-id="b8cc7-204">Specify the port for the proxy server.</span></span>|
|<span data-ttu-id="b8cc7-205">proxyAutomaticConfigurationUrl</span><span class="sxs-lookup"><span data-stu-id="b8cc7-205">proxyAutomaticConfigurationUrl</span></span>|<span data-ttu-id="b8cc7-206">字符串</span><span class="sxs-lookup"><span data-stu-id="b8cc7-206">String</span></span>|<span data-ttu-id="b8cc7-207">指定代理服务器配置脚本的 URL。</span><span class="sxs-lookup"><span data-stu-id="b8cc7-207">Specify the URL for the proxy server configuration script.</span></span>|
|<span data-ttu-id="b8cc7-208">forceFIPSCompliance</span><span class="sxs-lookup"><span data-stu-id="b8cc7-208">forceFIPSCompliance</span></span>|<span data-ttu-id="b8cc7-209">Boolean</span><span class="sxs-lookup"><span data-stu-id="b8cc7-209">Boolean</span></span>|<span data-ttu-id="b8cc7-210">指定是否强制 FIPS 合规性。</span><span class="sxs-lookup"><span data-stu-id="b8cc7-210">Specify whether to force FIPS compliance.</span></span>|



## <a name="response"></a><span data-ttu-id="b8cc7-211">响应</span><span class="sxs-lookup"><span data-stu-id="b8cc7-211">Response</span></span>
<span data-ttu-id="b8cc7-212">如果成功，此方法返回`201 Created`响应代码和响应正文中的[windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="b8cc7-212">If successful, this method returns a `201 Created` response code and a [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b8cc7-213">示例</span><span class="sxs-lookup"><span data-stu-id="b8cc7-213">Example</span></span>
### <a name="request"></a><span data-ttu-id="b8cc7-214">请求</span><span class="sxs-lookup"><span data-stu-id="b8cc7-214">Request</span></span>
<span data-ttu-id="b8cc7-215">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="b8cc7-215">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 850

{
  "@odata.type": "#microsoft.graph.windowsWifiConfiguration",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "preSharedKey": "Pre Shared Key value",
  "wifiSecurityType": "wpaPersonal",
  "meteredConnectionLimit": "fixed",
  "ssid": "Ssid value",
  "networkName": "Network Name value",
  "connectAutomatically": true,
  "connectToPreferredNetwork": true,
  "connectWhenNetworkNameIsHidden": true,
  "proxySetting": "manual",
  "proxyManualAddress": "Proxy Manual Address value",
  "proxyManualPort": 15,
  "proxyAutomaticConfigurationUrl": "https://example.com/proxyAutomaticConfigurationUrl/",
  "forceFIPSCompliance": true
}
```

### <a name="response"></a><span data-ttu-id="b8cc7-216">响应</span><span class="sxs-lookup"><span data-stu-id="b8cc7-216">Response</span></span>
<span data-ttu-id="b8cc7-p115">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="b8cc7-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 958

{
  "@odata.type": "#microsoft.graph.windowsWifiConfiguration",
  "id": "8a9e790f-790f-8a9e-0f79-9e8a0f799e8a",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "preSharedKey": "Pre Shared Key value",
  "wifiSecurityType": "wpaPersonal",
  "meteredConnectionLimit": "fixed",
  "ssid": "Ssid value",
  "networkName": "Network Name value",
  "connectAutomatically": true,
  "connectToPreferredNetwork": true,
  "connectWhenNetworkNameIsHidden": true,
  "proxySetting": "manual",
  "proxyManualAddress": "Proxy Manual Address value",
  "proxyManualPort": 15,
  "proxyAutomaticConfigurationUrl": "https://example.com/proxyAutomaticConfigurationUrl/",
  "forceFIPSCompliance": true
}
```





