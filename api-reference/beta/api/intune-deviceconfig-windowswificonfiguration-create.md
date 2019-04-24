---
title: 创建 windowsWifiConfiguration
description: 创建新的 windowsWifiConfiguration 对象。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6896149b9b9f90f8099600372d3d03627ae4bebe
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32510904"
---
# <a name="create-windowswificonfiguration"></a><span data-ttu-id="ecb4d-103">创建 windowsWifiConfiguration</span><span class="sxs-lookup"><span data-stu-id="ecb4d-103">Create windowsWifiConfiguration</span></span>

> <span data-ttu-id="ecb4d-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="ecb4d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ecb4d-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="ecb4d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ecb4d-106">创建新的[windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="ecb4d-106">Create a new [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ecb4d-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="ecb4d-107">Prerequisites</span></span>
<span data-ttu-id="ecb4d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ecb4d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ecb4d-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="ecb4d-110">Permission type</span></span>|<span data-ttu-id="ecb4d-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="ecb4d-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ecb4d-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ecb4d-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ecb4d-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ecb4d-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="ecb4d-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ecb4d-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ecb4d-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="ecb4d-115">Not supported.</span></span>|
|<span data-ttu-id="ecb4d-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="ecb4d-116">Application</span></span>|<span data-ttu-id="ecb4d-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="ecb4d-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ecb4d-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ecb4d-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="ecb4d-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="ecb4d-119">Request headers</span></span>
|<span data-ttu-id="ecb4d-120">标头</span><span class="sxs-lookup"><span data-stu-id="ecb4d-120">Header</span></span>|<span data-ttu-id="ecb4d-121">值</span><span class="sxs-lookup"><span data-stu-id="ecb4d-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ecb4d-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="ecb4d-122">Authorization</span></span>|<span data-ttu-id="ecb4d-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="ecb4d-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ecb4d-124">接受</span><span class="sxs-lookup"><span data-stu-id="ecb4d-124">Accept</span></span>|<span data-ttu-id="ecb4d-125">application/json</span><span class="sxs-lookup"><span data-stu-id="ecb4d-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ecb4d-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="ecb4d-126">Request body</span></span>
<span data-ttu-id="ecb4d-127">在请求正文中, 提供 windowsWifiConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ecb4d-127">In the request body, supply a JSON representation for the windowsWifiConfiguration object.</span></span>

<span data-ttu-id="ecb4d-128">下表显示创建 windowsWifiConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="ecb4d-128">The following table shows the properties that are required when you create the windowsWifiConfiguration.</span></span>

|<span data-ttu-id="ecb4d-129">属性</span><span class="sxs-lookup"><span data-stu-id="ecb4d-129">Property</span></span>|<span data-ttu-id="ecb4d-130">类型</span><span class="sxs-lookup"><span data-stu-id="ecb4d-130">Type</span></span>|<span data-ttu-id="ecb4d-131">说明</span><span class="sxs-lookup"><span data-stu-id="ecb4d-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ecb4d-132">id</span><span class="sxs-lookup"><span data-stu-id="ecb4d-132">id</span></span>|<span data-ttu-id="ecb4d-133">String</span><span class="sxs-lookup"><span data-stu-id="ecb4d-133">String</span></span>|<span data-ttu-id="ecb4d-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="ecb4d-134">Key of the entity.</span></span> <span data-ttu-id="ecb4d-135">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ecb4d-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ecb4d-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ecb4d-136">lastModifiedDateTime</span></span>|<span data-ttu-id="ecb4d-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ecb4d-137">DateTimeOffset</span></span>|<span data-ttu-id="ecb4d-138">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="ecb4d-138">DateTime the object was last modified.</span></span> <span data-ttu-id="ecb4d-139">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ecb4d-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ecb4d-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="ecb4d-140">roleScopeTagIds</span></span>|<span data-ttu-id="ecb4d-141">String collection</span><span class="sxs-lookup"><span data-stu-id="ecb4d-141">String collection</span></span>|<span data-ttu-id="ecb4d-142">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="ecb4d-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="ecb4d-143">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ecb4d-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ecb4d-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="ecb4d-144">supportsScopeTags</span></span>|<span data-ttu-id="ecb4d-145">布尔</span><span class="sxs-lookup"><span data-stu-id="ecb4d-145">Boolean</span></span>|<span data-ttu-id="ecb4d-146">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="ecb4d-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="ecb4d-147">如果此值为 false, 则不允许分配给 ScopeTags 属性, 并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="ecb4d-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="ecb4d-148">这适用于在 Silverlight 中创建的旧版策略, 可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="ecb4d-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="ecb4d-149">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="ecb4d-149">This property is read-only.</span></span> <span data-ttu-id="ecb4d-150">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ecb4d-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ecb4d-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ecb4d-151">createdDateTime</span></span>|<span data-ttu-id="ecb4d-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ecb4d-152">DateTimeOffset</span></span>|<span data-ttu-id="ecb4d-153">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="ecb4d-153">DateTime the object was created.</span></span> <span data-ttu-id="ecb4d-154">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ecb4d-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ecb4d-155">description</span><span class="sxs-lookup"><span data-stu-id="ecb4d-155">description</span></span>|<span data-ttu-id="ecb4d-156">字符串</span><span class="sxs-lookup"><span data-stu-id="ecb4d-156">String</span></span>|<span data-ttu-id="ecb4d-157">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="ecb4d-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="ecb4d-158">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ecb4d-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ecb4d-159">displayName</span><span class="sxs-lookup"><span data-stu-id="ecb4d-159">displayName</span></span>|<span data-ttu-id="ecb4d-160">String</span><span class="sxs-lookup"><span data-stu-id="ecb4d-160">String</span></span>|<span data-ttu-id="ecb4d-161">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="ecb4d-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="ecb4d-162">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ecb4d-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ecb4d-163">version</span><span class="sxs-lookup"><span data-stu-id="ecb4d-163">version</span></span>|<span data-ttu-id="ecb4d-164">Int32</span><span class="sxs-lookup"><span data-stu-id="ecb4d-164">Int32</span></span>|<span data-ttu-id="ecb4d-165">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="ecb4d-165">Version of the device configuration.</span></span> <span data-ttu-id="ecb4d-166">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ecb4d-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ecb4d-167">preSharedKey</span><span class="sxs-lookup"><span data-stu-id="ecb4d-167">preSharedKey</span></span>|<span data-ttu-id="ecb4d-168">字符串</span><span class="sxs-lookup"><span data-stu-id="ecb4d-168">String</span></span>|<span data-ttu-id="ecb4d-169">这是 WPA 个人 wi-fi 网络的预共享密钥。</span><span class="sxs-lookup"><span data-stu-id="ecb4d-169">This is the pre-shared key for WPA Personal Wi-Fi network.</span></span>|
|<span data-ttu-id="ecb4d-170">wifiSecurityType</span><span class="sxs-lookup"><span data-stu-id="ecb4d-170">wifiSecurityType</span></span>|[<span data-ttu-id="ecb4d-171">wiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="ecb4d-171">wiFiSecurityType</span></span>](../resources/intune-deviceconfig-wifisecuritytype.md)|<span data-ttu-id="ecb4d-172">指定 Wifi 安全类型。</span><span class="sxs-lookup"><span data-stu-id="ecb4d-172">Specify the Wifi Security Type.</span></span> <span data-ttu-id="ecb4d-173">可取值为：`open`、`wpaPersonal`、`wpaEnterprise`、`wep`、`wpa2Personal`、`wpa2Enterprise`。</span><span class="sxs-lookup"><span data-stu-id="ecb4d-173">Possible values are: `open`, `wpaPersonal`, `wpaEnterprise`, `wep`, `wpa2Personal`, `wpa2Enterprise`.</span></span>|
|<span data-ttu-id="ecb4d-174">meteredConnectionLimit</span><span class="sxs-lookup"><span data-stu-id="ecb4d-174">meteredConnectionLimit</span></span>|[<span data-ttu-id="ecb4d-175">meteredConnectionLimitType</span><span class="sxs-lookup"><span data-stu-id="ecb4d-175">meteredConnectionLimitType</span></span>](../resources/intune-deviceconfig-meteredconnectionlimittype.md)|<span data-ttu-id="ecb4d-176">为 wifi 连接指定按流量计费的连接限制类型。</span><span class="sxs-lookup"><span data-stu-id="ecb4d-176">Specify the metered connection limit type for the wifi connection.</span></span> <span data-ttu-id="ecb4d-177">可取值为：`unrestricted`、`fixed`、`variable`。</span><span class="sxs-lookup"><span data-stu-id="ecb4d-177">Possible values are: `unrestricted`, `fixed`, `variable`.</span></span>|
|<span data-ttu-id="ecb4d-178">ssid</span><span class="sxs-lookup"><span data-stu-id="ecb4d-178">ssid</span></span>|<span data-ttu-id="ecb4d-179">字符串</span><span class="sxs-lookup"><span data-stu-id="ecb4d-179">String</span></span>|<span data-ttu-id="ecb4d-180">指定 wifi 连接的 SSID。</span><span class="sxs-lookup"><span data-stu-id="ecb4d-180">Specify the SSID of the wifi connection.</span></span>|
|<span data-ttu-id="ecb4d-181">networkName</span><span class="sxs-lookup"><span data-stu-id="ecb4d-181">networkName</span></span>|<span data-ttu-id="ecb4d-182">字符串</span><span class="sxs-lookup"><span data-stu-id="ecb4d-182">String</span></span>|<span data-ttu-id="ecb4d-183">指定网络配置名称。</span><span class="sxs-lookup"><span data-stu-id="ecb4d-183">Specify the network configuration name.</span></span>|
|<span data-ttu-id="ecb4d-184">connectAutomatically</span><span class="sxs-lookup"><span data-stu-id="ecb4d-184">connectAutomatically</span></span>|<span data-ttu-id="ecb4d-185">布尔</span><span class="sxs-lookup"><span data-stu-id="ecb4d-185">Boolean</span></span>|<span data-ttu-id="ecb4d-186">指定是否在范围内自动连接 wifi 连接。</span><span class="sxs-lookup"><span data-stu-id="ecb4d-186">Specify whether the wifi connection should connect automatically when in range.</span></span>|
|<span data-ttu-id="ecb4d-187">connectToPreferredNetwork</span><span class="sxs-lookup"><span data-stu-id="ecb4d-187">connectToPreferredNetwork</span></span>|<span data-ttu-id="ecb4d-188">布尔</span><span class="sxs-lookup"><span data-stu-id="ecb4d-188">Boolean</span></span>|<span data-ttu-id="ecb4d-189">指定 wifi 连接是否应连接到更多的首选网络 (如果已连接到此连接的话)。</span><span class="sxs-lookup"><span data-stu-id="ecb4d-189">Specify whether the wifi connection should connect to more preferred networks when already connected to this one.</span></span>  <span data-ttu-id="ecb4d-190">要求 ConnectAutomatically 为 true。</span><span class="sxs-lookup"><span data-stu-id="ecb4d-190">Requires ConnectAutomatically to be true.</span></span>|
|<span data-ttu-id="ecb4d-191">connectWhenNetworkNameIsHidden</span><span class="sxs-lookup"><span data-stu-id="ecb4d-191">connectWhenNetworkNameIsHidden</span></span>|<span data-ttu-id="ecb4d-192">布尔</span><span class="sxs-lookup"><span data-stu-id="ecb4d-192">Boolean</span></span>|<span data-ttu-id="ecb4d-193">指定是否应自动连接 wifi 连接, 即使 SSID 未进行广播也是如此。</span><span class="sxs-lookup"><span data-stu-id="ecb4d-193">Specify whether the wifi connection should connect automatically even when the SSID is not broadcasting.</span></span>|
|<span data-ttu-id="ecb4d-194">proxySetting</span><span class="sxs-lookup"><span data-stu-id="ecb4d-194">proxySetting</span></span>|[<span data-ttu-id="ecb4d-195">wiFiProxySetting</span><span class="sxs-lookup"><span data-stu-id="ecb4d-195">wiFiProxySetting</span></span>](../resources/intune-deviceconfig-wifiproxysetting.md)|<span data-ttu-id="ecb4d-196">指定 wlan 配置的代理设置。</span><span class="sxs-lookup"><span data-stu-id="ecb4d-196">Specify the proxy setting for Wi-Fi configuration.</span></span> <span data-ttu-id="ecb4d-197">可取值为：`none`、`manual`、`automatic`。</span><span class="sxs-lookup"><span data-stu-id="ecb4d-197">Possible values are: `none`, `manual`, `automatic`.</span></span>|
|<span data-ttu-id="ecb4d-198">proxyManualAddress</span><span class="sxs-lookup"><span data-stu-id="ecb4d-198">proxyManualAddress</span></span>|<span data-ttu-id="ecb4d-199">字符串</span><span class="sxs-lookup"><span data-stu-id="ecb4d-199">String</span></span>|<span data-ttu-id="ecb4d-200">指定代理服务器的 IP 地址。</span><span class="sxs-lookup"><span data-stu-id="ecb4d-200">Specify the IP address for the proxy server.</span></span>|
|<span data-ttu-id="ecb4d-201">proxyManualPort</span><span class="sxs-lookup"><span data-stu-id="ecb4d-201">proxyManualPort</span></span>|<span data-ttu-id="ecb4d-202">Int32</span><span class="sxs-lookup"><span data-stu-id="ecb4d-202">Int32</span></span>|<span data-ttu-id="ecb4d-203">指定代理服务器的端口。</span><span class="sxs-lookup"><span data-stu-id="ecb4d-203">Specify the port for the proxy server.</span></span>|
|<span data-ttu-id="ecb4d-204">proxyAutomaticConfigurationUrl</span><span class="sxs-lookup"><span data-stu-id="ecb4d-204">proxyAutomaticConfigurationUrl</span></span>|<span data-ttu-id="ecb4d-205">字符串</span><span class="sxs-lookup"><span data-stu-id="ecb4d-205">String</span></span>|<span data-ttu-id="ecb4d-206">指定代理服务器配置脚本的 URL。</span><span class="sxs-lookup"><span data-stu-id="ecb4d-206">Specify the URL for the proxy server configuration script.</span></span>|
|<span data-ttu-id="ecb4d-207">forceFIPSCompliance</span><span class="sxs-lookup"><span data-stu-id="ecb4d-207">forceFIPSCompliance</span></span>|<span data-ttu-id="ecb4d-208">布尔</span><span class="sxs-lookup"><span data-stu-id="ecb4d-208">Boolean</span></span>|<span data-ttu-id="ecb4d-209">指定是否强制进行 FIPS 合规性。</span><span class="sxs-lookup"><span data-stu-id="ecb4d-209">Specify whether to force FIPS compliance.</span></span>|



## <a name="response"></a><span data-ttu-id="ecb4d-210">响应</span><span class="sxs-lookup"><span data-stu-id="ecb4d-210">Response</span></span>
<span data-ttu-id="ecb4d-211">如果成功, 此方法在响应`201 Created`正文中返回响应代码和[windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="ecb4d-211">If successful, this method returns a `201 Created` response code and a [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ecb4d-212">示例</span><span class="sxs-lookup"><span data-stu-id="ecb4d-212">Example</span></span>

### <a name="request"></a><span data-ttu-id="ecb4d-213">请求</span><span class="sxs-lookup"><span data-stu-id="ecb4d-213">Request</span></span>
<span data-ttu-id="ecb4d-214">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="ecb4d-214">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 786

{
  "@odata.type": "#microsoft.graph.windowsWifiConfiguration",
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

### <a name="response"></a><span data-ttu-id="ecb4d-215">响应</span><span class="sxs-lookup"><span data-stu-id="ecb4d-215">Response</span></span>
<span data-ttu-id="ecb4d-p114">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="ecb4d-p114">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





